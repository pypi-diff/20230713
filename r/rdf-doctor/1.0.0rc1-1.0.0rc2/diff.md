# Comparing `tmp/rdf_doctor-1.0.0rc1-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.0.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 23547 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-11 07:23 doctor/__init__.py
+Zip file size: 23802 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-12 07:39 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jul-10 00:40 doctor/consts.py
--rw-r--r--  2.0 unx    36512 b- defN 23-Jul-11 06:03 doctor/doctor.py
+-rw-r--r--  2.0 unx    39018 b- defN 23-Jul-12 07:39 doctor/doctor.py
 -rw-r--r--  2.0 unx    43474 b- defN 23-Jul-11 05:56 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 23-Jul-10 00:40 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 23-Jul-10 05:15 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8514 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1010 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/RECORD
-12 files, 92045 bytes uncompressed, 21831 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8514 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1010 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/RECORD
+12 files, 94551 bytes uncompressed, 22086 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc1.dist-info/LICENSE
+Filename: rdf_doctor-1.0.0rc2.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc1.dist-info/METADATA
+Filename: rdf_doctor-1.0.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc1.dist-info/WHEEL
+Filename: rdf_doctor-1.0.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc1.dist-info/entry_points.txt
+Filename: rdf_doctor-1.0.0rc2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc1.dist-info/top_level.txt
+Filename: rdf_doctor-1.0.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc1.dist-info/RECORD
+Filename: rdf_doctor-1.0.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0rc1"
+__version__ = "1.0.0rc2"
```

## doctor/doctor.py

```diff
@@ -46,46 +46,61 @@
         elif args.report == REPORT_FORMAT_MARKDOWN or args.report == REPORT_FORMAT_MD:
             # markdown/md
             thread_calc = threading.Thread(target=get_markdown_result, args=(args, input_format, compression_mode, result_queue,))
 
         else:
             # Else case does not occur.
             # Prevented by validate_command_line_args function.
-            raise ValueError(args.report + '" is an unsupported report format. "' + REPORT_FORMAT_SHEX + '" and "' + REPORT_FORMAT_MD+ '"(same as "' + REPORT_FORMAT_MARKDOWN + '") are supported.')
+            raise ValueError('"' + args.report + '" is an unsupported report format. "' + REPORT_FORMAT_SHEX + '" and "' + REPORT_FORMAT_MD+ '"(same as "' + REPORT_FORMAT_MARKDOWN + '") are supported.')
 
         thread_calc.setDaemon(True)
         thread_calc.start()
         if args.verbose:
             # Thread for displaying dots during processing
             thread_monitor = threading.Thread(target=monitor_thread, args=(result_queue,))
             thread_monitor.setDaemon(True)
             thread_monitor.start()
 
         thread_calc.join()
         if args.verbose:
             thread_monitor.join()
 
-        # Output result to specified destination (standard output or file)
-        if args.output is None:
-            print_overwrite("".join(result_queue.get()))
-        else:
-            with open(args.output, "w", encoding="utf-8") as f:
-                f.write("".join(result_queue.get()))
+        result_output = result_queue.get()
+        if type(result_output) is list:
+            # Normal case
+            if args.output is None:
+                # Standard output
+                print_overwrite("".join(result_output))
+            else:
+                # Output to file
+                with open(args.output, "w", encoding="utf-8") as f:
+                    f.write("".join(result_output))
+
+            if args.verbose:
+                print_overwrite(get_dt_now() + " -- Done!")
+
+        elif type(result_output) is IndexError or type(result_output) is Exception:
+            # Error case
+            raise result_output
 
-        if args.verbose:
-            print_overwrite(get_dt_now() + " -- Done!")
+        else:
+            # Else case does not occur.
+            raise Exception("An exception error has occurred. Not the expected processing result.")
 
     except ValueError as e:
         print(e)
 
+    except IndexError as e:
+        print(e)
+
     except KeyboardInterrupt:
         print ("Keyboard interrupt occurred.")
 
-    except:
-        print("An exception error has occurred. There may be a problem with your input data. Please review the data.")
+    except Exception as e:
+        print(e)
 
     return
 
 
 # Function for displaying dots during processing
 def monitor_thread(result_queue):
     i = 0
@@ -196,26 +211,30 @@
         org_extension = os.path.splitext(os.path.splitext(input_file)[0])[1]
         if org_extension == EXTENSION_NT:
             # N-Triples
             return NT
         elif org_extension == EXTENSION_TTL:
             # Turtle
             return TURTLE
+        else:
+            # Else case does not occur.
+            # Prevented by validate_command_line_args function.
+            raise ValueError('"' + org_extension + '.gz" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.')
     else:
         extension = os.path.splitext(input_file)[1]
         if extension == EXTENSION_NT:
             # N-Triples
             return NT
         elif extension == EXTENSION_TTL:
             # Turtle
             return TURTLE
         else:
             # Else case does not occur.
             # Prevented by validate_command_line_args function.
-            raise ValueError(extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.')
+            raise ValueError('"' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.')
 
 
 # Validate args(input, output, report, classes)
 def validate_command_line_args(args):
     compression_mode = ""
     input_format = ""
     for input_file in args.input:
@@ -229,40 +248,40 @@
             return False, error_msg
 
         # Check if the file has read permission
         if os.access(input_file, os.R_OK) == False:
             error_msg = "Input file error: you don't have permission to read the input file."
             return False, error_msg
 
+        # Allow only ".nt" or ".ttl" (and .gz) extensions
+        extension = os.path.splitext(input_file)[1]
+        if extension == EXTENSION_GZ:
+            org_extension = os.path.splitext(os.path.splitext(input_file)[0])[1]
+            # gz
+            if org_extension != EXTENSION_NT and org_extension != EXTENSION_TTL:
+                error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
+                return False, error_msg
+        elif extension != EXTENSION_NT and extension != EXTENSION_TTL:
+            error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
+            return False, error_msg
+
         if compression_mode == "":
             compression_mode = get_compression_mode(input_file)
         else:
             if compression_mode != get_compression_mode(input_file):
                 error_msg = "Input file error: If you enter multiple files, please use the same extension."
                 return False, error_msg
 
         if input_format == "":
             input_format = get_input_format(input_file, compression_mode)
         else:
             if input_format != get_input_format(input_file, compression_mode):
                 error_msg = "Input file error: If you enter multiple files, please use the same extension."
                 return False, error_msg
 
-        # Allow only ".nt" or ".ttl" (and .gz) extensions
-        extension = os.path.splitext(input_file)[1]
-        if extension == EXTENSION_GZ:
-            org_extension = os.path.splitext(os.path.splitext(input_file)[0])[1]
-            # gz
-            if org_extension != EXTENSION_NT and org_extension != EXTENSION_TTL:
-                error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
-                return False, error_msg
-        elif extension != EXTENSION_NT and extension != EXTENSION_TTL:
-            error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
-            return False, error_msg
-
     if args.output is not None:
         # Existence check of file output destination directory
         output_dir = os.path.dirname(args.output)
         if output_dir:
             if os.path.exists(output_dir) == False:
                 error_msg = "Output file error: Output directory does not exist."
                 return False, error_msg
@@ -331,178 +350,192 @@
 
     return True, None
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_format, compression_mode, result_queue):
 
-    # Get Prefix when input file is turtle format
-    if input_format == TURTLE:
+    try:
+        # Get Prefix when input file is turtle format
+        if input_format == TURTLE:
+            if args.verbose:
+                print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
+
+            input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
+        else:
+            input_prefixes = []
+            duplicated_prefixes = []
+
+        shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
+
+        # Prefixes with the same QName but different URIs at the same time
         if args.verbose:
-            print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
+            print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes...")
 
-        input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
-    else:
-        input_prefixes = []
-        duplicated_prefixes = []
+        result_duplicated_prefixes = []
+        if len(duplicated_prefixes) != 0:
+            result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
+            result_duplicated_prefixes.append("\n")
+            result_duplicated_prefixes.append("# Input-QName\tInput-prefix-URI\n")
+            result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
+            result_duplicated_prefixes.append("\n\n")
 
-    shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
+        # Suggest QName based on URI of validation expression output by sheXer and prefixes.tsv
+        if args.verbose:
+            print_overwrite(get_dt_now() + " -- Creating suggestions for QName...")
+
+        result_widely_used_qname = []
+        widely_used_prefixes = get_widely_used_prefixes(args.prefix_list)
+        widely_used_qname = get_widely_used_qname(shaper_result, input_prefixes, widely_used_prefixes)
+        if len(widely_used_qname) != 0:
+            result_widely_used_qname.append("# There is a more widely used QName.\n\n")
+            result_widely_used_qname.append("# Input-QName\tWidely-used-QName\tURI\n")
+            result_widely_used_qname.extend(["# " + s for s in widely_used_qname])
+            result_widely_used_qname.append("\n")
+
+        # List for storing the final result
+        shex_final_result = []
+        shex_final_result.extend(shaper_result)
+        if len(result_duplicated_prefixes) != 0:
+            shex_final_result.extend(result_duplicated_prefixes)
+
+        if len(result_widely_used_qname) != 0:
+            shex_final_result.extend(result_widely_used_qname)
 
-    # Prefixes with the same QName but different URIs at the same time
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes...")
-
-    result_duplicated_prefixes = []
-    if len(duplicated_prefixes) != 0:
-        result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
-        result_duplicated_prefixes.append("\n")
-        result_duplicated_prefixes.append("# Input-QName\tInput-prefix-URI\n")
-        result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
-        result_duplicated_prefixes.append("\n\n")
-
-    # Suggest QName based on URI of validation expression output by sheXer and prefixes.tsv
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Creating suggestions for QName...")
-
-    result_widely_used_qname = []
-    widely_used_prefixes = get_widely_used_prefixes(args.prefix_list)
-    widely_used_qname = get_widely_used_qname(shaper_result, input_prefixes, widely_used_prefixes)
-    if len(widely_used_qname) != 0:
-        result_widely_used_qname.append("# There is a more widely used QName.\n\n")
-        result_widely_used_qname.append("# Input-QName\tWidely-used-QName\tURI\n")
-        result_widely_used_qname.extend(["# " + s for s in widely_used_qname])
-        result_widely_used_qname.append("\n")
-
-    # List for storing the final result
-    shex_final_result = []
-    shex_final_result.extend(shaper_result)
-    if len(result_duplicated_prefixes) != 0:
-        shex_final_result.extend(result_duplicated_prefixes)
+        result_queue.put(shex_final_result)
 
-    if len(result_widely_used_qname) != 0:
-        shex_final_result.extend(result_widely_used_qname)
+    except IndexError:
+        result_queue.put(IndexError('An index error has occurred. If you are using the "-x", "-p" or "-l" option, there may be a problem with the number of columns in the specified tsv file. 2 columns is normal.'))
 
-    result_queue.put(shex_final_result)
+    except Exception:
+        result_queue.put(Exception('An exception error has occurred. There may be a problem with the input data. Check the contents of the file specified by the "-i" option. If there is no problem with the data and you are using the "-x", "-p", or "-l" options, there may be a problem with the contents of the file specified by these options. Please check.'))
 
 
 # Processing when the report format is "md/markdown"
 def get_markdown_result(args, input_format, compression_mode, result_queue):
 
-    # Processing related to prefixes ------------------
-    # Get Prefix when input file is turtle format
-    if input_format == TURTLE:
+    try:
+        # Processing related to prefixes ------------------
+        # Get Prefix when input file is turtle format
+        if input_format == TURTLE:
+            if args.verbose:
+                print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
+
+            input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
+        else:
+            input_prefixes = []
+            duplicated_prefixes = []
+
+        # Get list for result output about prefix reuse percentage
         if args.verbose:
-            print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
+            print_overwrite(get_dt_now() + " -- Calculating prefix reuse percentage...")
 
-        input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
-    else:
-        input_prefixes = []
-        duplicated_prefixes = []
+        result_prefix_reuse_percentage = []
+        result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
+        result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
+        prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes, args.prefix_list)
+        if prefix_reuse_percentage == None:
+            result_prefix_reuse_percentage.append("```\n")
+            result_prefix_reuse_percentage.append("Not calculated because there is no prefix defined.\n")
+            result_prefix_reuse_percentage.append("```\n\n")
+        else:
+            result_prefix_reuse_percentage.append("```\n")
+            result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
+            result_prefix_reuse_percentage.append("```\n\n")
 
-    # Get list for result output about prefix reuse percentage
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Calculating prefix reuse percentage...")
-
-    result_prefix_reuse_percentage = []
-    result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
-    result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
-    prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes, args.prefix_list)
-    if prefix_reuse_percentage == None:
-        result_prefix_reuse_percentage.append("```\n")
-        result_prefix_reuse_percentage.append("Not calculated because there is no prefix defined.\n")
-        result_prefix_reuse_percentage.append("```\n\n")
-    else:
-        result_prefix_reuse_percentage.append("```\n")
-        result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
-        result_prefix_reuse_percentage.append("```\n\n")
-
-    # Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Comparing with prefix URIs dictionary...")
-
-    result_refine_prefix_uris = []
-    prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
-    # When there is data to output
-    if len(prefix_comparison_result) != 0:
-        result_refine_prefix_uris.append("Found a more widely used one for the prefix URI inputed.\n")
-        result_refine_prefix_uris.append("```\n")
-        result_refine_prefix_uris.append("Input-QName\tInput-prefix-URI\tSuggested-prefix-URI\n")
-        result_refine_prefix_uris.extend(prefix_comparison_result)
-        result_refine_prefix_uris.append("```\n\n")
-
-    result_duplicated_prefixes = []
-    if len(duplicated_prefixes) != 0:
-        result_duplicated_prefixes.append("Duplicate prefixes found.\n")
-        result_duplicated_prefixes.append("```\n")
-        result_duplicated_prefixes.append("Input-QName\tInput-prefix-URI\n")
-        result_duplicated_prefixes.extend([s for s in duplicated_prefixes])
-        result_duplicated_prefixes.append("```\n\n")
-    # -------------------------------------------------
-
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Getting classes from input file...")
-
-    # Processing related to classes -------------------
-    input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
-
-    # Refers to the class URIs dictionary, acquires the list for result output that candidate pairs of URI rewrite source and rewrite destinations,
-    # and generate the class corresponding to each key in fingerprint format stored in dictionary format.
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary...")
-
-    result_refine_class_uris = []
-    class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
-    # When there is data to output
-    if len(class_comparison_result) != 0:
-        result_refine_class_uris.append("Found a more widely used one for the class URI inputed.\n")
-        result_refine_class_uris.append("```\n")
-        result_refine_class_uris.append("Input-class-URI\tSuggested-class-URI\n")
-        result_refine_class_uris.extend(class_comparison_result)
-        result_refine_class_uris.append("```\n\n")
-
-    # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
-    if args.verbose:
-        print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...")
-
-    result_class_fingerprint = []
-    fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
-    # When there is data to output
-    if len(fingerprint_comparison_result) != 0:
-        result_class_fingerprint.append("Found multiple strings that appear to represent the same class.\n")
-        result_class_fingerprint.append("```")
-        result_class_fingerprint.extend(fingerprint_comparison_result)
-        result_class_fingerprint.append("\n```\n\n")
-    # -------------------------------------------------
+        # Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
+        if args.verbose:
+            print_overwrite(get_dt_now() + " -- Comparing with prefix URIs dictionary...")
 
-    # List for storing the final result
-    md_final_result = []
+        result_refine_prefix_uris = []
+        prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
+        # When there is data to output
+        if len(prefix_comparison_result) != 0:
+            result_refine_prefix_uris.append("Found a more widely used one for the prefix URI inputed.\n")
+            result_refine_prefix_uris.append("```\n")
+            result_refine_prefix_uris.append("Input-QName\tInput-prefix-URI\tSuggested-prefix-URI\n")
+            result_refine_prefix_uris.extend(prefix_comparison_result)
+            result_refine_prefix_uris.append("```\n\n")
+
+        result_duplicated_prefixes = []
+        if len(duplicated_prefixes) != 0:
+            result_duplicated_prefixes.append("Duplicate prefixes found.\n")
+            result_duplicated_prefixes.append("```\n")
+            result_duplicated_prefixes.append("Input-QName\tInput-prefix-URI\n")
+            result_duplicated_prefixes.extend([s for s in duplicated_prefixes])
+            result_duplicated_prefixes.append("```\n\n")
+        # -------------------------------------------------
 
-    md_final_result.append("# Report on\n")
-    md_final_result.append("```\n")
-    for input_file in args.input:
-        md_final_result.append(os.path.basename(input_file) + "\n")
+        if args.verbose:
+            print_overwrite(get_dt_now() + " -- Getting classes from input file...")
+
+        # Processing related to classes -------------------
+        input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
+
+        # Refers to the class URIs dictionary, acquires the list for result output that candidate pairs of URI rewrite source and rewrite destinations,
+        # and generate the class corresponding to each key in fingerprint format stored in dictionary format.
+        if args.verbose:
+            print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary...")
+
+        result_refine_class_uris = []
+        class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
+        # When there is data to output
+        if len(class_comparison_result) != 0:
+            result_refine_class_uris.append("Found a more widely used one for the class URI inputed.\n")
+            result_refine_class_uris.append("```\n")
+            result_refine_class_uris.append("Input-class-URI\tSuggested-class-URI\n")
+            result_refine_class_uris.extend(class_comparison_result)
+            result_refine_class_uris.append("```\n\n")
+
+        # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
+        if args.verbose:
+            print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...")
 
-    md_final_result.append("```\n\n")
+        result_class_fingerprint = []
+        fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
+        # When there is data to output
+        if len(fingerprint_comparison_result) != 0:
+            result_class_fingerprint.append("Found multiple strings that appear to represent the same class.\n")
+            result_class_fingerprint.append("```")
+            result_class_fingerprint.extend(fingerprint_comparison_result)
+            result_class_fingerprint.append("\n```\n\n")
+        # -------------------------------------------------
+
+        # List for storing the final result
+        md_final_result = []
+
+        md_final_result.append("# Report on\n")
+        md_final_result.append("```\n")
+        for input_file in args.input:
+            md_final_result.append(os.path.basename(input_file) + "\n")
+
+        md_final_result.append("```\n\n")
+
+        # Merge result
+        md_final_result.extend(result_prefix_reuse_percentage)
+
+        prefix_result_exists = len(result_refine_prefix_uris) != 0
+        if prefix_result_exists:
+            md_final_result.append("## Refine prefix URIs ([?](" + HELP_LINK_URL + "))\n")
+            md_final_result.extend(result_refine_prefix_uris)
+            md_final_result.extend(result_duplicated_prefixes)
+
+        class_result_exists = len(result_refine_class_uris) != 0 or len(result_class_fingerprint) != 0
+        if class_result_exists:
+            md_final_result.append("## Refine class URIs ([?](" + HELP_LINK_URL + "))\n")
+            md_final_result.extend(result_refine_class_uris)
+            md_final_result.extend(result_class_fingerprint)
 
-    # Merge result
-    md_final_result.extend(result_prefix_reuse_percentage)
+        result_queue.put(md_final_result)
 
-    prefix_result_exists = len(result_refine_prefix_uris) != 0
-    if prefix_result_exists:
-        md_final_result.append("## Refine prefix URIs ([?](" + HELP_LINK_URL + "))\n")
-        md_final_result.extend(result_refine_prefix_uris)
-        md_final_result.extend(result_duplicated_prefixes)
-
-    class_result_exists = len(result_refine_class_uris) != 0 or len(result_class_fingerprint) != 0
-    if class_result_exists:
-        md_final_result.append("## Refine class URIs ([?](" + HELP_LINK_URL + "))\n")
-        md_final_result.extend(result_refine_class_uris)
-        md_final_result.extend(result_class_fingerprint)
+    except IndexError:
+        result_queue.put(IndexError('An index error has occurred. If you are using the "-x", "-p" or "-l" option, there may be a problem with the number of columns in the specified tsv file. 2 columns is normal.'))
 
-    result_queue.put(md_final_result)
+    except Exception:
+        result_queue.put(Exception('An exception error has occurred. There may be a problem with the input data. Check the contents of the file specified by the "-i" option. If there is no problem with the data and you are using the "-x", "-p", or "-l" options, there may be a problem with the contents of the file specified by these options. Please check.'))
 
 
 # Call the shex_graph method of shexer's shaper class and output the result
 def get_shaper_result(args, input_format, compression_mode, input_prefixes):
     # Set parameters when calling the shaper class depending on whether the class is specified as an argument
     if TARGET_CLASS_ALL in args.classes:
         target_classes = None
@@ -616,32 +649,32 @@
 def get_class_comparison_result(input_classes, refine_class_uris_file):
     refine_class_uris = get_refine_class_uris(refine_class_uris_file)
     class_comparison_result = []
     fingerprint_class_dict = defaultdict(list)
     # Perform clustering by fingerprint for the acquired class name
     for input_class in input_classes:
         fingerprint_class_dict[fingerprint(input_class)].append(input_class)
-        for eratta in refine_class_uris:
-            if input_class == eratta[0]:
-                class_comparison_result.append(input_class+"\t"+eratta[1]+"\n")
+        for refine_class_uri in refine_class_uris:
+            if input_class == refine_class_uri[0]:
+                class_comparison_result.append(input_class+"\t"+refine_class_uri[1]+"\n")
                 break
 
     return class_comparison_result, fingerprint_class_dict
 
 
 # Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
 def get_prefix_comparison_result(input_prefixes, refine_prefix_uris_file):
     refine_prefix_uris = get_refine_prefix_uris(refine_prefix_uris_file)
     prefix_comparison_result = []
 
     # Perform clustering by fingerprint for the acquired class name
     for input_prefix in input_prefixes:
-        for eratta in refine_prefix_uris:
-            if input_prefix[1] == eratta[0] and eratta[1] != "":
-                prefix_comparison_result.append(str(input_prefix[0]+"\t"+input_prefix[1]+"\t"+eratta[1]+"\n"))
+        for refine_prefix_uri in refine_prefix_uris:
+            if input_prefix[1] == refine_prefix_uri[0] and refine_prefix_uri[1] != "":
+                prefix_comparison_result.append(str(input_prefix[0]+"\t"+input_prefix[1]+"\t"+refine_prefix_uri[1]+"\n"))
                 break
 
     return prefix_comparison_result
 
 
 # Get the output result when there are multiple different strings with the same key for the class
 def get_fingerprint_comparison_result(fingerprint_class_dict):
```

## Comparing `rdf_doctor-1.0.0rc1.dist-info/LICENSE` & `rdf_doctor-1.0.0rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.0.0rc1.dist-info/METADATA` & `rdf_doctor-1.0.0rc2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `rdf_doctor-1.0.0rc1.dist-info/RECORD` & `rdf_doctor-1.0.0rc2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=iwDi0TUz45SMYIlshEAh-UPerqIe7nxUavbLYwEgSR8,25
+doctor/__init__.py,sha256=NkOwQwfEdXwwG-cmd9A-IS_-fhgqwRMABKCUsUI45tE,25
 doctor/consts.py,sha256=g8qN1vFAkkiFWF_HMGBpkoED0SdtPsxNUc33fcyLeow,631
-doctor/doctor.py,sha256=O5kON__m9JjcLgjnP1sNpq4GoxD5fGhKPrctstKH5yw,36512
+doctor/doctor.py,sha256=VQQOYUY-9doE06_pL633_yw6RshrJxfNJcxkixzSEQc,39018
 doctor/reference/prefixes.tsv,sha256=9zIvWdCO3X65YnULmiBEsIapiZvmplZbB6MywGJp54s,43474
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.0.0rc1.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.0.0rc1.dist-info/METADATA,sha256=f2ZSFlrGkOv9M6BSq7v_VsukppP5FuOOGLnl8JdYQ8Q,8514
-rdf_doctor-1.0.0rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-1.0.0rc1.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.0.0rc1.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.0.0rc1.dist-info/RECORD,,
+rdf_doctor-1.0.0rc2.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.0.0rc2.dist-info/METADATA,sha256=uJAeYHb9cu0fqq4LT7NIr7WylNEPROj614x9sUV3ZS8,8514
+rdf_doctor-1.0.0rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-1.0.0rc2.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.0.0rc2.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.0.0rc2.dist-info/RECORD,,
```

