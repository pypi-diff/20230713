# Comparing `tmp/GPT4Readability-0.0.2.tar.gz` & `tmp/GPT4Readability-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPT4Readability-0.0.2.tar", last modified: Thu Jul 13 00:20:53 2023, max compression
+gzip compressed data, was "GPT4Readability-0.0.3.tar", last modified: Thu Jul 13 00:50:23 2023, max compression
```

## Comparing `GPT4Readability-0.0.2.tar` & `GPT4Readability-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/GPT4Readability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/GPT4Readability/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/prompts/readme_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/prompts/refactor_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/readme_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/suggestions_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/GPT4Readability/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/GPT4Readability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 00:20:53.000000 GPT4Readability-0.0.2/GPT4Readability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:20:53.412774 GPT4Readability-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 00:20:40.000000 GPT4Readability-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/GPT4Readability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/GPT4Readability/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/prompts/readme_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/prompts/refactor_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/readme_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/suggestions_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/GPT4Readability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/setup.py
```

### Comparing `GPT4Readability-0.0.2/GPT4Readability/__main__.py` & `GPT4Readability-0.0.3/GPT4Readability/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     # Append '.md' if it's not there
     if not output_readme.endswith('.md'):
         output_readme += '.md'
     
     if not output_suggestions.endswith('.md'):
         output_suggestions += '.md'
     
+    # You can choose to use OpenAI's GPT-3.5-turbo or GPT-4 model
     if 'readme' in function or 'both' in function:
         print(f"\n[INFO] Commencing README generation using {model}. Initiating a detailed search and understanding of your codebase. This may take a while depending on the size of your codebase.\n")
         generate_readme(path, output_readme, model)
         print(f"\n[SUCCESS] README has been successfully generated! You can find it at: {os.path.join(path,output_readme)}\n")
         
     if 'suggestions' in function or 'both' in function:
         generate_suggestions(path, output_suggestions, model)
```

### Comparing `GPT4Readability-0.0.2/GPT4Readability/prompts/readme_prompt.txt` & `GPT4Readability-0.0.3/GPT4Readability/prompts/readme_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.2/GPT4Readability/prompts/refactor_prompt.txt` & `GPT4Readability-0.0.3/GPT4Readability/prompts/refactor_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.2/GPT4Readability/readme_gen.py` & `GPT4Readability-0.0.3/GPT4Readability/readme_gen.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     inb_msg += file_check_result
     special_file_check_result = check_special_files(root_dir) # Checking for the code of conduct and the style guide
     inb_msg += special_file_check_result
 
     username, reponame = get_github_info_from_local_repo(root_dir)
 
     if username:
-        inb_msg = inb_msg.replace("[username]", username)
+        inb_msg = inb_msg.replace("[username]", username.replace("git@github.com:",""))
         inb_msg = inb_msg.replace("[repo_name]", reponame.replace(".git",""))
     else:
         inb_msg = remove_line_with_pattern_from_string(inb_msg)
 
 
     docs = get_docs(root_dir)
     texts = split_docs(docs)
```

### Comparing `GPT4Readability-0.0.2/GPT4Readability/suggestions_gen.py` & `GPT4Readability-0.0.3/GPT4Readability/suggestions_gen.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.2/GPT4Readability/utils.py` & `GPT4Readability-0.0.3/GPT4Readability/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,22 +130,22 @@
                 style_guide_path = os.path.join(root, file)
 
     result = '\n'
     
     if code_of_conduct_exists:
         result += f"A code of conduct exists at the following path: {code_of_conduct_path}. "
     else:
-        result += "There is no code of conduct in the directory. Do not bring up a code of conduct in the readme."
+        result += "There is no code of conduct in the directory. \n\nDO NOT bring up a code of conduct in the readme."
     
     result += "\n"
     
     if style_guide_exists:
         result += f"A style guide exists at the following path: {style_guide_path}."
     else:
-        result += "There is no style guide in the directory.  Do not bring up a style guide in the readme."
+        result += "There is no style guide in the directory.  \n\nDO NOT bring up a style guide in the readme."
         
     return result
 
 def split_docs(docs):
     text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
     texts = text_splitter.split_documents(docs)
     return texts
```

### Comparing `GPT4Readability-0.0.2/GPT4Readability.egg-info/PKG-INFO` & `GPT4Readability-0.0.3/GPT4Readability.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -21,87 +21,73 @@
 
 [![License Badge](https://img.shields.io/github/license/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE)
 [![Issues Badge](https://img.shields.io/github/issues/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
-GPT4Readability is a powerful tool designed to automatically generate a README.md file and suggest code improvements for any Python code repository. It leverages advanced AI capabilities to analyze and interpret the codebase, providing comprehensive and accurate documentation.  Other than **this sentence** this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) was generated by GPT4Readability using gpt-3.5-turbo.
+GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
-## Main Functionalities
+> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.
 
-- Automatic generation of README.md file for Python codebases
-- Suggestions for code improvements
-- Integration with GPT-3.5 Turbo and GPT-4 models for enhanced analysis
+## Features
 
-## Installation
-
-To install GPT4Readability, follow these steps:
-
-1. Clone the repository:
-
-   ```shell
-   git clone https://github.com/loevlie/GPT4Readability.git
-   ```
-
-2. Navigate to the project directory:
+- Automatic generation of a detailed README.md file for your Python codebase
+- Suggestions for code improvements to enhance readability and maintainability
 
-   ```shell
-   cd GPT4Readability
-   ```
-
-3. Install the required dependencies:
-
-   ```shell
-   pip install -e .
-   ```
-
-## Dependencies
+## Installation
 
-GPT4Readability requires the following dependencies:
+To use GPT4Readability, you need to have Python 3.6 or higher installed on your system. You can install GPT4Readability and its dependencies using the following command:
 
-- langchain
-- openai
-- faiss-cpu
-- tiktoken
-- click
-- tqdm
+```shell
+pip install GPT4Readability
+```
 
 ## Usage
 
-GPT4Readability provides two main functionalities: generating a README.md file and suggesting code improvements. You can choose to use either of these functions or both.
+GPT4Readability provides two main functionalities: README generation and code improvement suggestions. You can choose to use either one or both of these functions.
 
-To generate a README.md file, use the following command:
+### README Generation
 
-```shell
-gpt4readability <path> --function readme --output_readme <output_name> --model <model>
+To generate a README.md file for your codebase, use the following command:
+
+```bash
+gpt4readability <path> --function readme --output_readme README.md --model <model>
 ```
 
-Replace `<path>` with the root directory of the Python package you want to parse and generate a README for. `<output_name>` should be the desired filename for the generated README.md file. `<model>` specifies the model to use, either "gpt-3.5-turbo" or "gpt-4".
+Replace `<path>` with the path to your codebase directory and `<model>` with the desired model to use (either "gpt-3.5-turbo" or "gpt-4").
 
-To suggest code improvements, use the following command:
+### Code Improvement Suggestions
 
-```shell
-gpt4readability <path> --function suggestions --output_suggestions <output_name> --model <model>
+To generate code improvement suggestions for your codebase, use the following command:
+
+```bash
+gpt4readability <path> --function suggestions --output_suggestions suggestions.md --model <model>
 ```
 
-Replace `<path>` with the root directory of the Python package you want to analyze and suggest improvements for. `<output_name>` should be the desired filename for the generated suggestions.md file. `<model>` specifies the model to use, either "gpt-3.5-turbo" or "gpt-4".
+Replace `<path>` with the path to your codebase directory and `<model>` with the desired model to use (either "gpt-3.5-turbo" or "gpt-4").
 
 ## Authors
 
 GPT4Readability is developed and maintained by Dennis Johan Loevlie. For any inquiries or support, please contact Dennis Johan Loevlie at loevliedenny@gmail.com.
 
 ## Contributing
 
-Contributions to GPT4Readability are welcome! If you encounter any issues or have suggestions for improvements, please report them on the [GitHub Issues](https://github.com/loevlie/GPT4Readability/issues) page.
+Contributions to GPT4Readability are welcome! If you encounter any issues or have suggestions for improvements, please report them by opening an issue on the [GitHub repository](https://github.com/loevlie/GPT4Readability/issues).
 
-## Support
+To contribute code changes, follow these steps:
 
-For support or assistance with GPT4Readability, please reach out to Dennis Johan Loevlie at loevliedenny@gmail.com.
+1. Fork the repository on GitHub.
+2. Create a new branch from the main branch.
+3. Make your desired changes and commit them.
+4. Push your branch to your forked repository.
+5. Open a pull request on the main repository.
 
-## License
+Please ensure that your code changes adhere to the coding style and guidelines of the project.
 
-GPT4Readability is licensed under the [MIT License](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE). Feel free to use, modify, and distribute this codebase as per the terms of the license.
+## Support
 
-## Acknowledgements
+For support or assistance with using GPT4Readability, please contact Dennis Johan Loevlie at loevliedenny@gmail.com.
+
+## License
 
-We would like to express our gratitude to the developers and contributors of the dependencies used in this project. Their hard work and dedication have made GPT4Readability possible.
+GPT4Readability is licensed under the MIT License. See the [LICENSE](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE) file for more details.
```

### Comparing `GPT4Readability-0.0.2/LICENSE` & `GPT4Readability-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.2/PKG-INFO` & `GPT4Readability-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -21,87 +21,73 @@
 
 [![License Badge](https://img.shields.io/github/license/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE)
 [![Issues Badge](https://img.shields.io/github/issues/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
-GPT4Readability is a powerful tool designed to automatically generate a README.md file and suggest code improvements for any Python code repository. It leverages advanced AI capabilities to analyze and interpret the codebase, providing comprehensive and accurate documentation.  Other than **this sentence** this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) was generated by GPT4Readability using gpt-3.5-turbo.
+GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
-## Main Functionalities
+> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.
 
-- Automatic generation of README.md file for Python codebases
-- Suggestions for code improvements
-- Integration with GPT-3.5 Turbo and GPT-4 models for enhanced analysis
+## Features
 
-## Installation
-
-To install GPT4Readability, follow these steps:
-
-1. Clone the repository:
-
-   ```shell
-   git clone https://github.com/loevlie/GPT4Readability.git
-   ```
-
-2. Navigate to the project directory:
+- Automatic generation of a detailed README.md file for your Python codebase
+- Suggestions for code improvements to enhance readability and maintainability
 
-   ```shell
-   cd GPT4Readability
-   ```
-
-3. Install the required dependencies:
-
-   ```shell
-   pip install -e .
-   ```
-
-## Dependencies
+## Installation
 
-GPT4Readability requires the following dependencies:
+To use GPT4Readability, you need to have Python 3.6 or higher installed on your system. You can install GPT4Readability and its dependencies using the following command:
 
-- langchain
-- openai
-- faiss-cpu
-- tiktoken
-- click
-- tqdm
+```shell
+pip install GPT4Readability
+```
 
 ## Usage
 
-GPT4Readability provides two main functionalities: generating a README.md file and suggesting code improvements. You can choose to use either of these functions or both.
+GPT4Readability provides two main functionalities: README generation and code improvement suggestions. You can choose to use either one or both of these functions.
 
-To generate a README.md file, use the following command:
+### README Generation
 
-```shell
-gpt4readability <path> --function readme --output_readme <output_name> --model <model>
+To generate a README.md file for your codebase, use the following command:
+
+```bash
+gpt4readability <path> --function readme --output_readme README.md --model <model>
 ```
 
-Replace `<path>` with the root directory of the Python package you want to parse and generate a README for. `<output_name>` should be the desired filename for the generated README.md file. `<model>` specifies the model to use, either "gpt-3.5-turbo" or "gpt-4".
+Replace `<path>` with the path to your codebase directory and `<model>` with the desired model to use (either "gpt-3.5-turbo" or "gpt-4").
 
-To suggest code improvements, use the following command:
+### Code Improvement Suggestions
 
-```shell
-gpt4readability <path> --function suggestions --output_suggestions <output_name> --model <model>
+To generate code improvement suggestions for your codebase, use the following command:
+
+```bash
+gpt4readability <path> --function suggestions --output_suggestions suggestions.md --model <model>
 ```
 
-Replace `<path>` with the root directory of the Python package you want to analyze and suggest improvements for. `<output_name>` should be the desired filename for the generated suggestions.md file. `<model>` specifies the model to use, either "gpt-3.5-turbo" or "gpt-4".
+Replace `<path>` with the path to your codebase directory and `<model>` with the desired model to use (either "gpt-3.5-turbo" or "gpt-4").
 
 ## Authors
 
 GPT4Readability is developed and maintained by Dennis Johan Loevlie. For any inquiries or support, please contact Dennis Johan Loevlie at loevliedenny@gmail.com.
 
 ## Contributing
 
-Contributions to GPT4Readability are welcome! If you encounter any issues or have suggestions for improvements, please report them on the [GitHub Issues](https://github.com/loevlie/GPT4Readability/issues) page.
+Contributions to GPT4Readability are welcome! If you encounter any issues or have suggestions for improvements, please report them by opening an issue on the [GitHub repository](https://github.com/loevlie/GPT4Readability/issues).
 
-## Support
+To contribute code changes, follow these steps:
 
-For support or assistance with GPT4Readability, please reach out to Dennis Johan Loevlie at loevliedenny@gmail.com.
+1. Fork the repository on GitHub.
+2. Create a new branch from the main branch.
+3. Make your desired changes and commit them.
+4. Push your branch to your forked repository.
+5. Open a pull request on the main repository.
 
-## License
+Please ensure that your code changes adhere to the coding style and guidelines of the project.
 
-GPT4Readability is licensed under the [MIT License](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE). Feel free to use, modify, and distribute this codebase as per the terms of the license.
+## Support
 
-## Acknowledgements
+For support or assistance with using GPT4Readability, please contact Dennis Johan Loevlie at loevliedenny@gmail.com.
+
+## License
 
-We would like to express our gratitude to the developers and contributors of the dependencies used in this project. Their hard work and dedication have made GPT4Readability possible.
+GPT4Readability is licensed under the MIT License. See the [LICENSE](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE) file for more details.
```

### Comparing `GPT4Readability-0.0.2/README.md` & `GPT4Readability-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,87 +2,73 @@
 
 [![License Badge](https://img.shields.io/github/license/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE)
 [![Issues Badge](https://img.shields.io/github/issues/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
-GPT4Readability is a powerful tool designed to automatically generate a README.md file and suggest code improvements for any Python code repository. It leverages advanced AI capabilities to analyze and interpret the codebase, providing comprehensive and accurate documentation.  Other than **this sentence** this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) was generated by GPT4Readability using gpt-3.5-turbo.
+GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
-## Main Functionalities
+> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.
 
-- Automatic generation of README.md file for Python codebases
-- Suggestions for code improvements
-- Integration with GPT-3.5 Turbo and GPT-4 models for enhanced analysis
+## Features
 
-## Installation
-
-To install GPT4Readability, follow these steps:
-
-1. Clone the repository:
-
-   ```shell
-   git clone https://github.com/loevlie/GPT4Readability.git
-   ```
-
-2. Navigate to the project directory:
+- Automatic generation of a detailed README.md file for your Python codebase
+- Suggestions for code improvements to enhance readability and maintainability
 
-   ```shell
-   cd GPT4Readability
-   ```
-
-3. Install the required dependencies:
-
-   ```shell
-   pip install -e .
-   ```
-
-## Dependencies
+## Installation
 
-GPT4Readability requires the following dependencies:
+To use GPT4Readability, you need to have Python 3.6 or higher installed on your system. You can install GPT4Readability and its dependencies using the following command:
 
-- langchain
-- openai
-- faiss-cpu
-- tiktoken
-- click
-- tqdm
+```shell
+pip install GPT4Readability
+```
 
 ## Usage
 
-GPT4Readability provides two main functionalities: generating a README.md file and suggesting code improvements. You can choose to use either of these functions or both.
+GPT4Readability provides two main functionalities: README generation and code improvement suggestions. You can choose to use either one or both of these functions.
 
-To generate a README.md file, use the following command:
+### README Generation
 
-```shell
-gpt4readability <path> --function readme --output_readme <output_name> --model <model>
+To generate a README.md file for your codebase, use the following command:
+
+```bash
+gpt4readability <path> --function readme --output_readme README.md --model <model>
 ```
 
-Replace `<path>` with the root directory of the Python package you want to parse and generate a README for. `<output_name>` should be the desired filename for the generated README.md file. `<model>` specifies the model to use, either "gpt-3.5-turbo" or "gpt-4".
+Replace `<path>` with the path to your codebase directory and `<model>` with the desired model to use (either "gpt-3.5-turbo" or "gpt-4").
 
-To suggest code improvements, use the following command:
+### Code Improvement Suggestions
 
-```shell
-gpt4readability <path> --function suggestions --output_suggestions <output_name> --model <model>
+To generate code improvement suggestions for your codebase, use the following command:
+
+```bash
+gpt4readability <path> --function suggestions --output_suggestions suggestions.md --model <model>
 ```
 
-Replace `<path>` with the root directory of the Python package you want to analyze and suggest improvements for. `<output_name>` should be the desired filename for the generated suggestions.md file. `<model>` specifies the model to use, either "gpt-3.5-turbo" or "gpt-4".
+Replace `<path>` with the path to your codebase directory and `<model>` with the desired model to use (either "gpt-3.5-turbo" or "gpt-4").
 
 ## Authors
 
 GPT4Readability is developed and maintained by Dennis Johan Loevlie. For any inquiries or support, please contact Dennis Johan Loevlie at loevliedenny@gmail.com.
 
 ## Contributing
 
-Contributions to GPT4Readability are welcome! If you encounter any issues or have suggestions for improvements, please report them on the [GitHub Issues](https://github.com/loevlie/GPT4Readability/issues) page.
+Contributions to GPT4Readability are welcome! If you encounter any issues or have suggestions for improvements, please report them by opening an issue on the [GitHub repository](https://github.com/loevlie/GPT4Readability/issues).
 
-## Support
+To contribute code changes, follow these steps:
 
-For support or assistance with GPT4Readability, please reach out to Dennis Johan Loevlie at loevliedenny@gmail.com.
+1. Fork the repository on GitHub.
+2. Create a new branch from the main branch.
+3. Make your desired changes and commit them.
+4. Push your branch to your forked repository.
+5. Open a pull request on the main repository.
 
-## License
+Please ensure that your code changes adhere to the coding style and guidelines of the project.
 
-GPT4Readability is licensed under the [MIT License](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE). Feel free to use, modify, and distribute this codebase as per the terms of the license.
+## Support
 
-## Acknowledgements
+For support or assistance with using GPT4Readability, please contact Dennis Johan Loevlie at loevliedenny@gmail.com.
+
+## License
 
-We would like to express our gratitude to the developers and contributors of the dependencies used in this project. Their hard work and dedication have made GPT4Readability possible.
+GPT4Readability is licensed under the MIT License. See the [LICENSE](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE) file for more details.
```

### Comparing `GPT4Readability-0.0.2/setup.py` & `GPT4Readability-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as readme:
     # ignore gifs
     description = ''.join([i for i in readme.readlines()
                            if not i.startswith('![')])
 
 setup(
     name='GPT4Readability',
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/loevlie/GPT4Readability',
     author='Dennis Johan Loevlie',
     author_email='loevliedenny@gmail.com',
     description='A tool to automatically generate a README.md and suggest code improvements for any python code repository',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),  # automatically discover all packages and subpackages
```

