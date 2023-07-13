# Comparing `tmp/nibabies_wrapper-23.1.0rc0.tar.gz` & `tmp/nibabies-wrapper-99.99.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "nibabies-wrapper-99.99.99.tar", last modified: Thu Sep 30 00:12:48 2021, max compression
```

## Comparing `nibabies_wrapper-23.1.0rc0.tar` & `nibabies-wrapper-99.99.99.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/src/nibabies_wrapper/__init__.py
--rwxr-xr-x   0        0        0    24722 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/src/nibabies_wrapper/__main__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/src/nibabies_wrapper/_version.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/LICENSE
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/README.rst
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 nibabies_wrapper-23.1.0rc0/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-30 00:12:48.056883 nibabies-wrapper-99.99.99/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2083 2021-09-30 00:12:48.056883 nibabies-wrapper-99.99.99/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1314 2021-09-30 00:12:37.000000 nibabies-wrapper-99.99.99/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-30 00:12:48.056883 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2083 2021-09-30 00:12:47.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      291 2021-09-30 00:12:48.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-09-30 00:12:47.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-09-30 00:12:47.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2021-09-30 00:12:47.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2021-09-30 00:12:47.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.egg-info/top_level.txt
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    23841 2021-09-30 00:12:47.000000 nibabies-wrapper-99.99.99/nibabies_wrapper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1032 2021-09-30 00:12:48.056883 nibabies-wrapper-99.99.99/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      115 2021-09-30 00:12:37.000000 nibabies-wrapper-99.99.99/setup.py
```

### Comparing `nibabies_wrapper-23.1.0rc0/src/nibabies_wrapper/__main__.py` & `nibabies-wrapper-99.99.99/nibabies_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python
 """
-This is a Python wrapper to facilitate running NiBabies through Docker or Singularity services.
+The NiBabies wrapper for Docker/Singularity
+
+
+This is a Python wrapper to run NiBabies through a container service.
 Docker or Singularity must be installed and running.
-To test installation, you can use one of the following:
+This can be checked by running either ::
 
-```bash
-docker info
-singularity version
-```
+  docker info
+  singularity version
 
 Please report any feedback to our GitHub repository
 (https://github.com/nipreps/nibabies) and do not
 forget to credit all the authors of service that NiBabies
 uses (https://fmriprep.readthedocs.io/en/latest/citing.html).
 """
 import sys
 import os
 import re
 import subprocess
 
-try:
-    from ._version import __version__
-except ImportError:
-    __version__ = '0+unknown'
-__copyright__ = 'Copyright 2023, The NiPreps Developers'
-__bugreports__ = 'https://github.com/nipreps/nibabies/issues'
+__version__ = "99.99.99"
+__copyright__ = (
+    "Copyright 2021, The NiPreps Developers"
+)
+__bugreports__ = "https://github.com/nipreps/nibabies/issues"
 
 MISSING = """
 Image '{}' is missing
 Would you like to download? [Y/n] """
-PKG_PATH = "/opt/conda/lib/python3.9/site-packages"
+PKG_PATH = "/usr/local/miniconda/lib/python3.7/site-packages"
 TF_TEMPLATES = (
     "MNI152Lin",
     "MNI152NLin2009cAsym",
     "MNI152NLin6Asym",
     "MNI152NLin6Sym",
     "MNIInfant",
     "MNIPediatricAsym",
@@ -117,15 +117,17 @@
 
         Inputs
         ------
         src : absolute local path
         dst : absolute container path
         read_only : disable writing to bound path
         """
-        self.mounts.append("{0}:{1}{2}".format(src, dst, ":ro" if read_only else ""))
+        self.mounts.append(
+            "{0}:{1}{2}".format(src, dst, ":ro" if read_only else "")
+        )
 
     def check_install(self):
         """Verify that the service is installed and the user has permission to
         run images.
 
         Returns
         -------
@@ -148,15 +150,17 @@
         if ret.stderr.startswith(b"Cannot connect to the Docker daemon."):
             return 0
         return 1
 
     def check_image(self, image):
         """Check whether image is present on local system"""
         if self.service == "docker":
-            ret = subprocess.run(["docker", "images", "-q", image], stdout=subprocess.PIPE)
+            ret = subprocess.run(
+                ["docker", "images", "-q", image], stdout=subprocess.PIPE
+            )
             return bool(ret.stdout)
         elif self.service == "singularity":
             # check if the image file exists
             return os.path.exists(os.path.abspath(image))
         raise NotImplementedError
 
     def check_memory(self, image):
@@ -261,17 +265,14 @@
     # assert w_posargs.replace("]", "").replace("[", "") == t_posargs
 
     # Make sure we're not clobbering options we don't mean to
     overlap = set(w_flags).intersection(t_flags)
     expected_overlap = {
         "anat-derivatives",
         "bids-database-dir",
-        "bids-filter-file",
-        "derivatives",
-        "deriv-filter-file",
         "fs-license-file",
         "fs-subjects-dir",
         "config-file",
         "segmentation-atlases-dir",
         "h",
         "use-plugin",
         "version",
@@ -342,27 +343,29 @@
                 d[k] = os.path.abspath(v)
             setattr(namespace, self.dest, d)
 
     def _is_file(path, parser):
         """Ensure a given path exists and it is a file."""
         path = os.path.abspath(path)
         if not os.path.isfile(path):
-            raise parser.error("Path should point to a file (or symlink of file): <%s>." % path)
+            raise parser.error(
+                "Path should point to a file (or symlink of file): <%s>." % path
+            )
         return path
 
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         add_help=False,
     )
 
     IsFile = partial(_is_file, parser=parser)
 
     # require users to specify container service
-    parser.add_argument("service", nargs="?", choices=("docker", "singularity"))
+    parser.add_argument("service", choices=("docker", "singularity"))
     # Standard NiBabies arguments
     parser.add_argument("bids_dir", nargs="?", type=os.path.abspath, default="")
     parser.add_argument("output_dir", nargs="?", type=os.path.abspath, default="")
     parser.add_argument(
         "analysis_level", nargs="?", choices=["participant"], default="participant"
     )
 
@@ -423,28 +426,29 @@
         help="Path to FreeSurfer license key file. Get it (for free) by registering"
         " at https://surfer.nmr.mgh.harvard.edu/registration.html",
     )
     g_wrap.add_argument(
         "--fs-subjects-dir",
         metavar="PATH",
         type=os.path.abspath,
-        help="Path to existing Infant FreeSurfer subjects directory to reuse. ",
+        help="Path to existing FreeSurfer subjects directory to reuse. "
+        "(default: OUTPUT_DIR/freesurfer)",
     )
     g_wrap.add_argument(
         "--config-file",
         metavar="PATH",
         type=os.path.abspath,
         help="Use pre-generated configuration file. Values in file will be overridden "
         "by command-line arguments.",
     )
     g_wrap.add_argument(
         "--anat-derivatives",
         metavar="PATH",
         type=os.path.abspath,
-        help="Path to existing NiBabies anatomical derivatives to fasttrack "
+        help="Path to existing sMRIPrep/nibabies-anatomical derivatives to fasttrack "
         "the anatomical workflow.",
     )
     g_wrap.add_argument(
         "--use-plugin",
         metavar="PATH",
         action="store",
         default=None,
@@ -458,34 +462,15 @@
         help="Path to an existing PyBIDS database folder, for faster indexing "
         "(especially useful for large datasets).",
     )
     g_wrap.add_argument(
         "--segmentation-atlases-dir",
         metavar="PATH",
         type=os.path.abspath,
-        help="Directory containing prelabeled segmentations to use for JointLabelFusion.",
-    )
-    g_wrap.add_argument(
-        "--derivatives",
-        nargs="+",
-        metavar="PATH",
-        type=os.path.abspath,
-        help="One or more directory containing pre-computed derivatives",
-    )
-    g_wrap.add_argument(
-        "--bids-filter-file",
-        metavar="PATH",
-        type=os.path.abspath,
-        help="Filter file",
-    )
-    g_wrap.add_argument(
-        "--deriv-filter-file",
-        metavar="PATH",
-        type=os.path.abspath,
-        help="Filter file",
+        help="Directory containing prelabeled segmentations to use for JointLabelFusion."
     )
 
     # Developer patch/shell options
     g_dev = parser.add_argument_group(
         "Developer options", "Tools for testing and debugging nibabies"
     )
     g_dev.add_argument(
@@ -524,71 +509,82 @@
     )
     g_dev.add_argument(
         "--network",
         action="store",
         help="Run container with a different network driver "
         '("none" to simulate no internet connection)',
     )
-    g_dev.add_argument("--no-tty", action="store_true", help="Run docker without TTY flag -it")
+    g_dev.add_argument(
+        "--no-tty", action="store_true", help="Run docker without TTY flag -it"
+    )
 
     return parser
 
 
 def main():
     """Entry point"""
 
     parser = get_parser()
     # Capture additional arguments to pass inside container
     opts, unknown_args = parser.parse_known_args()
 
-    if opts.version:
-        print("nibabies wrapper {!s}".format(__version__))
-        return
-
     # Set help if no directories set
-    if opts.help or not all((opts.service, opts.bids_dir, opts.output_dir)):
-        parser.print_help()
-        return
+    if (opts.bids_dir, opts.output_dir, opts.version) == ("", "", False):
+        opts.help = True
 
     container = ContainerManager(opts.service, image=opts.image)
     check = container.check_install()
     if check < 1:
+        if opts.version:
+            print("nibabies wrapper {!s}".format(__version__))
+        if opts.help:
+            parser.print_help()
         if check == -1:
             print(
-                "nibabies: Could not find %s command... Is it installed?" % opts.service,
+                "nibabies: Could not find %s command... Is it installed?"
+                % opts.service
             )
         else:
             print(
-                "nibabies: Make sure you have permission to run '%s'" % opts.service,
+                "nibabies: Make sure you have permission to run '%s'" % opts.service
             )
         return 1
 
+    # For --help or --version, ask before downloading an image
     if not container.check_image(opts.image):
         resp = "Y"
-        if opts.service == "singularity":
-            print("Singularity image must already exist locally.")
-            return 1
-        try:
-            resp = input(MISSING.format(opts.image))
-        except KeyboardInterrupt:
-            print()
+        if opts.version:
+            print("nibabies wrapper {!s}".format(__version__))
+        if opts.help:
+            parser.print_help()
+        if opts.version == "singularity":
+            print("Singularity images must already exist locally.")
             return 1
+        if opts.version or opts.help:
+            try:
+                resp = input(MISSING.format(opts.image))
+            except KeyboardInterrupt:
+                print()
+                return 1
         if resp not in ("y", "Y", ""):
             return 0
         print("Downloading. This may take a while...")
 
     # Warn on low memory allocation
     mem_total = container.check_memory(opts.image)
     if mem_total == -1:
         print(
             "Could not detect memory capacity of Docker container.\n"
             "Do you have permission to run docker?"
         )
         return 1
-    if "--reports-only" not in unknown_args and mem_total < 8000:
+    if (
+        not (opts.help or opts.version or "--reports-only" in unknown_args)
+        and mem_total < 8000
+    ):
         print(
             "Warning: <8GB of RAM is available within your environment.\n"
             "Some parts of nibabies may fail to complete."
         )
         if "--mem_mb" not in unknown_args:
             resp = "N"
             try:
@@ -599,15 +595,19 @@
             if resp not in ("y", "Y", ""):
                 return 0
 
     container.set_version()
 
     if opts.service == "docker":
         if not opts.no_tty:
-            container.add_cmd("-it")
+            if opts.help:
+                # TTY can corrupt stdout
+                container.add_cmd("-i")
+            else:
+                container.add_cmd("-it")
         if opts.user:
             container.add_cmd(("-u", opts.user))
         if opts.network:
             container.add_cmd("--network=%s" % opts.network)
 
     # Patch working repositories into installed package directories
     if opts.patch:
@@ -643,27 +643,14 @@
 
     if opts.anat_derivatives:
         container.add_mount(opts.anat_derivatives, "/opt/smriprep/subjects", read_only=False)
         unknown_args.extend(["--anat-derivatives", "/opt/smriprep/subjects"])
     if opts.segmentation_atlases_dir:
         container.add_mount(opts.segmentation_atlases_dir, "/opt/segmentations")
         unknown_args.extend(["--segmentation-atlases-dir", "/opt/segmentations"])
-    if opts.bids_filter_file:
-        container.add_mount(opts.bids_filter_file, "/opt/bids_filters.json")
-        unknown_args.extend(["--bids-filter-file", "/opt/bids_filters.json"])
-    if opts.deriv_filter_file:
-        container.add_mount(opts.deriv_filter_file, "/opt/derivative_filters.json")
-        unknown_args.extend(["--deriv-filter-file", "/opt/derivative_filters.json"])
-    if opts.derivatives:
-        derivative_args = ["--derivatives"]
-        for derivative in opts.derivatives:
-            derivative_target = "/opt/derivatives/%s" % os.path.basename(derivative)
-            container.add_mount(derivative, derivative_target, read_only=False)
-            derivative_args.append(derivative_target)
-        unknown_args.extend(derivative_args)
 
     # Check that work_dir is not a child of bids_dir
     if opts.work_dir and opts.bids_dir:
         if is_in_directory(opts.work_dir, opts.bids_dir):
             print(
                 "The selected working directory is a subdirectory of the input BIDS folder. "
                 "Please modify the output path."
@@ -689,15 +676,17 @@
 
     if opts.output_spaces:
         spaces = []
         for space in opts.output_spaces:
             if space.split(":")[0] not in (TF_TEMPLATES + NONSTANDARD_REFERENCES):
                 tpl = os.path.basename(space)
                 if not tpl.startswith("tpl-"):
-                    raise RuntimeError("Custom template %s requires a `tpl-` prefix" % tpl)
+                    raise RuntimeError(
+                        "Custom template %s requires a `tpl-` prefix" % tpl
+                    )
                 target = "/home/fmriprep/.cache/templateflow/" + tpl
                 container.add_mount(os.path.abspath(space), target)
                 spaces.append(tpl[4:])
             else:
                 spaces.append(space)
         unknown_args.extend(["--output-spaces"] + spaces)
 
@@ -711,34 +700,31 @@
     container.image = opts.image
     # after this, all call to ``container.add_cmd``
     # will be for nibabies arguments
     container.finalize_container_cmd()
 
     # Override help and version to describe underlying program
     # Respects '-i' flag, so will retrieve information from any image
-    # if opts.help:
-    #     container.add_cmd("-h")
-    #     targethelp = subprocess.check_output(container.command).decode()
-    #     print(merge_help(parser.format_help(), targethelp))
-    #     return 0
-    # elif opts.version:
-    #     # Get version to be run and exit
-    #     container.add_cmd("--version")
-    #     ret = subprocess.run(container.command)
-    #     return ret.returncode
+    if opts.help:
+        container.add_cmd("-h")
+        targethelp = subprocess.check_output(container.command).decode()
+        print(merge_help(parser.format_help(), targethelp))
+        return 0
+    elif opts.version:
+        # Get version to be run and exit
+        container.add_cmd("--version")
+        ret = subprocess.run(container.command)
+        return ret.returncode
 
     if not opts.shell:
         container.add_cmd(main_args)
         container.add_cmd(unknown_args)
 
     print("RUNNING: " + " ".join(container.command))
     ret = subprocess.run(container.command)
     if ret.returncode:
         print("nibabies: Please report errors to {}".format(__bugreports__))
     return ret.returncode
 
 
 if __name__ == "__main__":
-    if '__main__.py' in sys.argv[0]:
-        from . import __name__ as module
-        sys.argv[0] = '%s -m %s' % (sys.executable, module)
     sys.exit(main())
```

### Comparing `nibabies_wrapper-23.1.0rc0/README.rst` & `nibabies-wrapper-99.99.99/README.rst`

 * *Files identical despite different names*

