# Comparing `tmp/lemonai-0.1.0.tar.gz` & `tmp/lemonai-0.1.1.tar.gz`

## Comparing `lemonai-0.1.0.tar` & `lemonai-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.0/heatmap-example.gif
--rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.0/heatmap-example.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lemonai-0.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.0/docs/tools.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.0/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.0/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.0/LICENSE
--rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 lemonai-0.1.0/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 lemonai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.1/heatmap-example.gif
+-rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.1/heatmap-example.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lemonai-0.1.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.1/docs/tools.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.1/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.1/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 lemonai-0.1.1/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 lemonai-0.1.1/PKG-INFO
```

### Comparing `lemonai-0.1.0/heatmap-example.gif` & `lemonai-0.1.1/heatmap-example.gif`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/heatmap-example.png` & `lemonai-0.1.1/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/docs/tools.md` & `lemonai-0.1.1/docs/tools.md`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/src/lemonai/api_wrapper.py` & `lemonai-0.1.1/src/lemonai/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/src/lemonai/execute_workflow.py` & `lemonai-0.1.1/src/lemonai/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/src/lemonai/filter_tools.py` & `lemonai-0.1.1/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/src/lemonai/get_integrations.py` & `lemonai-0.1.1/src/lemonai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/src/lemonai/tool.py` & `lemonai-0.1.1/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/src/lemonai/toolkit.py` & `lemonai-0.1.1/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/.gitignore` & `lemonai-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/LICENSE` & `lemonai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.0/README.md` & `lemonai-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
   </a>
   <br />
     <a href="">
     <img alt="Run Notebook in LangChain Docs" src="https://img.shields.io/badge/Run Notebook From LangChain Docs-x?style=for-the-badge&logoColor=white&label&labelColor=gray&color=gray">
   </a>
   <br />
   <br />
+  <figure>
+    <img src="heatmap-example.gif" alt="Demo" />
+  </figure>
 </div>
 
-![Heatmap Example](heatmap-example.gif)
-
-**Build powerful AI assistants in minutes and automate workflows by allowing for accurate and reliable read and write operations in [tools](#🧩-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack and Github.**
+**Lemon AI helps you build powerful AI assistants in minutes and automate workflows by allowing for accurate and reliable read and write operations in [tools](#🧩-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack and Github.**
 
 Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions.
 
 With Lemon AI, it is possible to give your agents access to well-defined APIs for reliable read and write operations. In addition, Lemon AI functions allow you to further reduce the risk of hallucinations by providing a way to statically define workflows that the model can rely on in case of uncertainty.
 
 ## ⚡️ Getting Started
 
@@ -159,18 +160,19 @@
     <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" style="border-radius: 50%;" width="100px;" alt=""/><br /><sub><b>Felix</b></sub></a></td>
     <td style="border:none;">Hey there 🥳 I am Felix, the creator of Lemon AI. Always happy to chat and answer any questions you might have! So feel free to reachout on <a href="https://twitter.com/felixbrockm">Twitter</a> or <a href="mailto:fe.brockmeier@gmail.com">Email</a> </td>
   </tr>
 </table>
 
 ### Active Contributors
 
-> People who actively help out improving the codebase by making PRs and reviewing code.
+> Team members and people who actively help out improving the codebase by making PRs and reviewing code.
 
 <table cellspacing="0" cellpadding="0" style="border:none;">
   <tbody>
     <tr style="border:none;">
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/mohammed-abdus-samad-hannan-3a2687202/"><img src="https://avatars.githubusercontent.com/u/72310364?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Mohammed Hannan</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/haiphunghiem/"><img src="https://avatars.githubusercontent.com/u/16231195?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Hai Nghiem</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://twitter.com/schroeerclemens"><img src="https://avatars.githubusercontent.com/u/84038864?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Clemens Schroeer</b></sub></a></td>
+      <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Felix Brockmeier</b></sub></a></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
                           ****** ð Lemon AI ******
       **** Gateway to empower LLM agents to interact with the world ****
                       [Discord] [Twitter] [MIT_License]
                        [Run Notebook in LangChain Docs]
 
-![Heatmap Example](heatmap-example.gif) **Build powerful AI assistants in
-minutes and automate workflows by allowing for accurate and reliable read and
-write operations in [tools](#ð§©-supported-tools) like Airtable, Hubspot,
-Discord, Notion, Slack and Github.** Most connectors available today are
-focused on read-only operations, limiting the potential of LLMs. Agents, on the
-other hand, have a tendency to hallucinate from time to time due to missing
-context or instructions. With Lemon AI, it is possible to give your agents
-access to well-defined APIs for reliable read and write operations. In
-addition, Lemon AI functions allow you to further reduce the risk of
-hallucinations by providing a way to statically define workflows that the model
-can rely on in case of uncertainty. ## â¡ï¸ Getting Started ### 1.
-Prerequisites Requires Python 3.8.1 and above. ### 2. Installing To use Lemon
-AI in your Python project run `pip install lemonai`. The following example uses
-an OpenAI model. Therefore, we also need to `pip install openai`. Depending on
-which model you want to use this install is optional. ### 3. (Optional) Launch
-the Server The interaction of your agents and all Lemon AI tools is provided by
-the [Lemon AI Server](https://github.com/felixbrock/lemonai-server). Per
-default the Lemon AI Python client is sending requests to a hosted server
-version. To run the Lemon AI server on-prem please refer to the [Server
-Documentation](https://github.com/felixbrock/lemonai-server). ### 4. Use Lemon
-AI with LangChain The easiest way to give Lemon AI a try is via the Jupyter
-Notebook you can find in the [LangChain Docs](https://python.langchain.com/
-docs/modules/agents/tools/integrations/lemonai). Lemon AI automatically solves
-given tasks by finding the right combination of relevant tools or uses Lemon AI
-Functions as an alternative. The following example demonstrates how to retrieve
-a user from Hackernews and write it to a table in Airtable: #### Include Lemon
-AI in your LangChain project ```Python import os from lemonai import
-execute_workflow from langchain import OpenAI ``` #### Load API Keys and Access
-Tokens To use tools that require authentication, you have to store the
-corresponding access credentials in your environment in the format "{tool
-name}\_{authentication string}" where the authentication string is one of
-["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or
-["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are
-"OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN". ```Python
-""" Load all relevant API Keys and Access Tokens into your environment
-variables """ os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*"
-os.environ["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*" ``` ####
-Define your prompt and execute the LangChain Agent ```Python
-hackernews_username = "*INSERT HACKERNEWS USERNAME HERE*" """ Guidelines on
-identifying Airtable ids here: https://www.highviewapps.com/kb/where-can-i-
-find-the-airtable-base-id-and-table-id/ """ airtable_base_id = "*INSERT BASE ID
-HERE*" airtable_table_id = "*INSERT TABLE ID HERE*" """ Define your instruction
-to be given to your LLM """ prompt = f"""Read information from Hackernews for
-user {hackernews_username} and then write the results to Airtable (baseId:
+                                    [Demo]
+**Lemon AI helps you build powerful AI assistants in minutes and automate
+workflows by allowing for accurate and reliable read and write operations in
+[tools](#ð§©-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack
+and Github.** Most connectors available today are focused on read-only
+operations, limiting the potential of LLMs. Agents, on the other hand, have a
+tendency to hallucinate from time to time due to missing context or
+instructions. With Lemon AI, it is possible to give your agents access to well-
+defined APIs for reliable read and write operations. In addition, Lemon AI
+functions allow you to further reduce the risk of hallucinations by providing a
+way to statically define workflows that the model can rely on in case of
+uncertainty. ## â¡ï¸ Getting Started ### 1. Prerequisites Requires Python
+3.8.1 and above. ### 2. Installing To use Lemon AI in your Python project run
+`pip install lemonai`. The following example uses an OpenAI model. Therefore,
+we also need to `pip install openai`. Depending on which model you want to use
+this install is optional. ### 3. (Optional) Launch the Server The interaction
+of your agents and all Lemon AI tools is provided by the [Lemon AI Server]
+(https://github.com/felixbrock/lemonai-server). Per default the Lemon AI Python
+client is sending requests to a hosted server version. To run the Lemon AI
+server on-prem please refer to the [Server Documentation](https://github.com/
+felixbrock/lemonai-server). ### 4. Use Lemon AI with LangChain The easiest way
+to give Lemon AI a try is via the Jupyter Notebook you can find in the
+[LangChain Docs](https://python.langchain.com/docs/modules/agents/tools/
+integrations/lemonai). Lemon AI automatically solves given tasks by finding the
+right combination of relevant tools or uses Lemon AI Functions as an
+alternative. The following example demonstrates how to retrieve a user from
+Hackernews and write it to a table in Airtable: #### Include Lemon AI in your
+LangChain project ```Python import os from lemonai import execute_workflow from
+langchain import OpenAI ``` #### Load API Keys and Access Tokens To use tools
+that require authentication, you have to store the corresponding access
+credentials in your environment in the format "{tool name}\_{authentication
+string}" where the authentication string is one of ["API_KEY", "SECRET_KEY",
+"SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN",
+"SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY",
+"BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN". ```Python """ Load all
+relevant API Keys and Access Tokens into your environment variables """
+os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*" os.environ
+["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*" ``` #### Define your
+prompt and execute the LangChain Agent ```Python hackernews_username = "*INSERT
+HACKERNEWS USERNAME HERE*" """ Guidelines on identifying Airtable ids here:
+https://www.highviewapps.com/kb/where-can-i-find-the-airtable-base-id-and-
+table-id/ """ airtable_base_id = "*INSERT BASE ID HERE*" airtable_table_id =
+"*INSERT TABLE ID HERE*" """ Define your instruction to be given to your LLM
+""" prompt = f"""Read information from Hackernews for user
+{hackernews_username} and then write the results to Airtable (baseId:
 {airtable_base_id}, tableId: {airtable_table_id}). Only write the fields
 "username", "karma" and "created_at_i". Please make sure that Airtable does NOT
 automatically convert the field types. """ """ Use the Lemon AI
 execute_workflow wrapper to run your LangChain agent in combination with Lemon
 AI """ model = OpenAI(temperature=0) execute_workflow(llm=model,
 prompt_string=prompt) ``` #### (Optional) Define your Lemon AI Functions
 Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-
@@ -91,11 +92,11 @@
 We are extremely open to contributions! You can find more information in our
 [CONTRIBUTING.md](https://github.com/felixbrock/lemonai-py-client/blob/
 main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop
 us a message on Discord. ## â¤ï¸âð¥ Team
       Hey there ð¥³ I am Felix, the creator of Lemon AI. Always happy to chat and
 Felix answer any questions you might have! So feel free to reachout on Twitter or
       Email
-### Active Contributors > People who actively help out improving the codebase
-by making PRs and reviewing code.
+### Active Contributors > Team members and people who actively help out
+improving the codebase by making PRs and reviewing code.
 
-Mohammed_Hannan Hai_Nghiem Clemens_Schroeer
+Mohammed_Hannan Hai_Nghiem Clemens_Schroeer Felix_Brockmeier
```

### Comparing `lemonai-0.1.0/pyproject.toml` & `lemonai-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lemonai-0.1.0/PKG-INFO` & `lemonai-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
 Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,19 +28,20 @@
   </a>
   <br />
     <a href="">
     <img alt="Run Notebook in LangChain Docs" src="https://img.shields.io/badge/Run Notebook From LangChain Docs-x?style=for-the-badge&logoColor=white&label&labelColor=gray&color=gray">
   </a>
   <br />
   <br />
+  <figure>
+    <img src="heatmap-example.gif" alt="Demo" />
+  </figure>
 </div>
 
-![Heatmap Example](heatmap-example.gif)
-
-**Build powerful AI assistants in minutes and automate workflows by allowing for accurate and reliable read and write operations in [tools](#🧩-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack and Github.**
+**Lemon AI helps you build powerful AI assistants in minutes and automate workflows by allowing for accurate and reliable read and write operations in [tools](#🧩-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack and Github.**
 
 Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions.
 
 With Lemon AI, it is possible to give your agents access to well-defined APIs for reliable read and write operations. In addition, Lemon AI functions allow you to further reduce the risk of hallucinations by providing a way to statically define workflows that the model can rely on in case of uncertainty.
 
 ## ⚡️ Getting Started
 
@@ -175,18 +176,19 @@
     <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" style="border-radius: 50%;" width="100px;" alt=""/><br /><sub><b>Felix</b></sub></a></td>
     <td style="border:none;">Hey there 🥳 I am Felix, the creator of Lemon AI. Always happy to chat and answer any questions you might have! So feel free to reachout on <a href="https://twitter.com/felixbrockm">Twitter</a> or <a href="mailto:fe.brockmeier@gmail.com">Email</a> </td>
   </tr>
 </table>
 
 ### Active Contributors
 
-> People who actively help out improving the codebase by making PRs and reviewing code.
+> Team members and people who actively help out improving the codebase by making PRs and reviewing code.
 
 <table cellspacing="0" cellpadding="0" style="border:none;">
   <tbody>
     <tr style="border:none;">
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/mohammed-abdus-samad-hannan-3a2687202/"><img src="https://avatars.githubusercontent.com/u/72310364?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Mohammed Hannan</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://www.linkedin.com/in/haiphunghiem/"><img src="https://avatars.githubusercontent.com/u/16231195?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Hai Nghiem</b></sub></a></td>
       <td align="center" style="border:none;"><a href="https://twitter.com/schroeerclemens"><img src="https://avatars.githubusercontent.com/u/84038864?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Clemens Schroeer</b></sub></a></td>
+      <td align="center" style="border:none;"><a href="https://twitter.com/felixbrockm"><img src="https://avatars.githubusercontent.com/u/70200999?s=100&v=4" width="70px;" alt="" style="border-radius: 50%;"/><br /><sub><b>Felix Brockmeier</b></sub></a></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lemonai Version: 0.1.0 Summary: Lemon AI's A Python
+Metadata-Version: 2.1 Name: lemonai Version: 0.1.1 Summary: Lemon AI's A Python
 client. Grant your LLM agents access to a wide range of APIs for read and write
 operations, creating copilots in minutes and unlocking the true potential of
 LLMs. Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/
 issues Author-email: Felix Brockmeier
 brockmeier@gmail.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
@@ -10,58 +10,59 @@
 Requires-Dist: langchain Requires-Dist: loguru Description-Content-Type: text/
 markdown
                           ****** ð Lemon AI ******
       **** Gateway to empower LLM agents to interact with the world ****
                       [Discord] [Twitter] [MIT_License]
                        [Run Notebook in LangChain Docs]
 
-![Heatmap Example](heatmap-example.gif) **Build powerful AI assistants in
-minutes and automate workflows by allowing for accurate and reliable read and
-write operations in [tools](#ð§©-supported-tools) like Airtable, Hubspot,
-Discord, Notion, Slack and Github.** Most connectors available today are
-focused on read-only operations, limiting the potential of LLMs. Agents, on the
-other hand, have a tendency to hallucinate from time to time due to missing
-context or instructions. With Lemon AI, it is possible to give your agents
-access to well-defined APIs for reliable read and write operations. In
-addition, Lemon AI functions allow you to further reduce the risk of
-hallucinations by providing a way to statically define workflows that the model
-can rely on in case of uncertainty. ## â¡ï¸ Getting Started ### 1.
-Prerequisites Requires Python 3.8.1 and above. ### 2. Installing To use Lemon
-AI in your Python project run `pip install lemonai`. The following example uses
-an OpenAI model. Therefore, we also need to `pip install openai`. Depending on
-which model you want to use this install is optional. ### 3. (Optional) Launch
-the Server The interaction of your agents and all Lemon AI tools is provided by
-the [Lemon AI Server](https://github.com/felixbrock/lemonai-server). Per
-default the Lemon AI Python client is sending requests to a hosted server
-version. To run the Lemon AI server on-prem please refer to the [Server
-Documentation](https://github.com/felixbrock/lemonai-server). ### 4. Use Lemon
-AI with LangChain The easiest way to give Lemon AI a try is via the Jupyter
-Notebook you can find in the [LangChain Docs](https://python.langchain.com/
-docs/modules/agents/tools/integrations/lemonai). Lemon AI automatically solves
-given tasks by finding the right combination of relevant tools or uses Lemon AI
-Functions as an alternative. The following example demonstrates how to retrieve
-a user from Hackernews and write it to a table in Airtable: #### Include Lemon
-AI in your LangChain project ```Python import os from lemonai import
-execute_workflow from langchain import OpenAI ``` #### Load API Keys and Access
-Tokens To use tools that require authentication, you have to store the
-corresponding access credentials in your environment in the format "{tool
-name}\_{authentication string}" where the authentication string is one of
-["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or
-["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are
-"OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN". ```Python
-""" Load all relevant API Keys and Access Tokens into your environment
-variables """ os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*"
-os.environ["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*" ``` ####
-Define your prompt and execute the LangChain Agent ```Python
-hackernews_username = "*INSERT HACKERNEWS USERNAME HERE*" """ Guidelines on
-identifying Airtable ids here: https://www.highviewapps.com/kb/where-can-i-
-find-the-airtable-base-id-and-table-id/ """ airtable_base_id = "*INSERT BASE ID
-HERE*" airtable_table_id = "*INSERT TABLE ID HERE*" """ Define your instruction
-to be given to your LLM """ prompt = f"""Read information from Hackernews for
-user {hackernews_username} and then write the results to Airtable (baseId:
+                                    [Demo]
+**Lemon AI helps you build powerful AI assistants in minutes and automate
+workflows by allowing for accurate and reliable read and write operations in
+[tools](#ð§©-supported-tools) like Airtable, Hubspot, Discord, Notion, Slack
+and Github.** Most connectors available today are focused on read-only
+operations, limiting the potential of LLMs. Agents, on the other hand, have a
+tendency to hallucinate from time to time due to missing context or
+instructions. With Lemon AI, it is possible to give your agents access to well-
+defined APIs for reliable read and write operations. In addition, Lemon AI
+functions allow you to further reduce the risk of hallucinations by providing a
+way to statically define workflows that the model can rely on in case of
+uncertainty. ## â¡ï¸ Getting Started ### 1. Prerequisites Requires Python
+3.8.1 and above. ### 2. Installing To use Lemon AI in your Python project run
+`pip install lemonai`. The following example uses an OpenAI model. Therefore,
+we also need to `pip install openai`. Depending on which model you want to use
+this install is optional. ### 3. (Optional) Launch the Server The interaction
+of your agents and all Lemon AI tools is provided by the [Lemon AI Server]
+(https://github.com/felixbrock/lemonai-server). Per default the Lemon AI Python
+client is sending requests to a hosted server version. To run the Lemon AI
+server on-prem please refer to the [Server Documentation](https://github.com/
+felixbrock/lemonai-server). ### 4. Use Lemon AI with LangChain The easiest way
+to give Lemon AI a try is via the Jupyter Notebook you can find in the
+[LangChain Docs](https://python.langchain.com/docs/modules/agents/tools/
+integrations/lemonai). Lemon AI automatically solves given tasks by finding the
+right combination of relevant tools or uses Lemon AI Functions as an
+alternative. The following example demonstrates how to retrieve a user from
+Hackernews and write it to a table in Airtable: #### Include Lemon AI in your
+LangChain project ```Python import os from lemonai import execute_workflow from
+langchain import OpenAI ``` #### Load API Keys and Access Tokens To use tools
+that require authentication, you have to store the corresponding access
+credentials in your environment in the format "{tool name}\_{authentication
+string}" where the authentication string is one of ["API_KEY", "SECRET_KEY",
+"SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN",
+"SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY",
+"BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN". ```Python """ Load all
+relevant API Keys and Access Tokens into your environment variables """
+os.environ["OPENAI_API_KEY"] = "*INSERT OPENAI API KEY HERE*" os.environ
+["AIRTABLE_ACCESS_TOKEN"] = "*INSERT AIRTABLE TOKEN HERE*" ``` #### Define your
+prompt and execute the LangChain Agent ```Python hackernews_username = "*INSERT
+HACKERNEWS USERNAME HERE*" """ Guidelines on identifying Airtable ids here:
+https://www.highviewapps.com/kb/where-can-i-find-the-airtable-base-id-and-
+table-id/ """ airtable_base_id = "*INSERT BASE ID HERE*" airtable_table_id =
+"*INSERT TABLE ID HERE*" """ Define your instruction to be given to your LLM
+""" prompt = f"""Read information from Hackernews for user
+{hackernews_username} and then write the results to Airtable (baseId:
 {airtable_base_id}, tableId: {airtable_table_id}). Only write the fields
 "username", "karma" and "created_at_i". Please make sure that Airtable does NOT
 automatically convert the field types. """ """ Use the Lemon AI
 execute_workflow wrapper to run your LangChain agent in combination with Lemon
 AI """ model = OpenAI(temperature=0) execute_workflow(llm=model,
 prompt_string=prompt) ``` #### (Optional) Define your Lemon AI Functions
 Similar to [OpenAI functions](https://openai.com/blog/function-calling-and-
@@ -102,11 +103,11 @@
 We are extremely open to contributions! You can find more information in our
 [CONTRIBUTING.md](https://github.com/felixbrock/lemonai-py-client/blob/
 main/.github/CONTRIBUTING.md). If you have any more questions feel free to drop
 us a message on Discord. ## â¤ï¸âð¥ Team
       Hey there ð¥³ I am Felix, the creator of Lemon AI. Always happy to chat and
 Felix answer any questions you might have! So feel free to reachout on Twitter or
       Email
-### Active Contributors > People who actively help out improving the codebase
-by making PRs and reviewing code.
+### Active Contributors > Team members and people who actively help out
+improving the codebase by making PRs and reviewing code.
 
-Mohammed_Hannan Hai_Nghiem Clemens_Schroeer
+Mohammed_Hannan Hai_Nghiem Clemens_Schroeer Felix_Brockmeier
```

