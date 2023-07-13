# Comparing `tmp/sweepai-0.4.1.tar.gz` & `tmp/sweepai-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.1.tar", max compression
+gzip compressed data, was "sweepai-0.4.2.tar", max compression
```

## Comparing `sweepai-0.4.1.tar` & `sweepai-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.1/LICENSE
--rw-r--r--   0        0        0     6678 2023-07-11 20:05:05.034619 sweepai-0.4.1/README.md
--rw-r--r--   0        0        0     1395 2023-07-11 20:18:44.748666 sweepai-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/__init__.py
--rw-r--r--   0        0        0    12248 2023-07-11 20:05:05.034619 sweepai-0.4.1/sweepai/api.py
--rw-r--r--   0        0        0     6020 2023-07-11 09:20:00.556075 sweepai-0.4.1/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10421 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/app/backend.py
--rw-r--r--   0        0        0     1166 2023-07-09 08:40:46.465379 sweepai-0.4.1/sweepai/app/cli.py
--rw-r--r--   0        0        0     3583 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/app/config.py
--rw-r--r--   0        0        0    14559 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17400 2023-07-08 21:39:15.812977 sweepai-0.4.1/sweepai/core/chat.py
--rw-r--r--   0        0        0     2867 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8306 2023-07-11 20:16:30.901906 sweepai-0.4.1/sweepai/core/entities.py
--rw-r--r--   0        0        0      561 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16814 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/core/react.py
--rw-r--r--   0        0        0    19671 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12695 2023-07-09 08:40:46.468712 sweepai-0.4.1/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3176 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     6475 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2571 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9391 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.4.1/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    17844 2023-07-11 20:05:05.034619 sweepai-0.4.1/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1808 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0     2001 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/utils/config.py
--rw-r--r--   0        0        0      964 2023-07-11 09:20:17.826102 sweepai-0.4.1/sweepai/utils/constants.py
--rw-r--r--   0        0        0     6529 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8225 2023-07-09 08:40:46.468712 sweepai-0.4.1/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/utils.py
--rw-r--r--   0        0        0     7849 2023-07-11 20:19:37.916061 sweepai-0.4.1/setup.py
--rw-r--r--   0        0        0     7630 2023-07-11 20:19:37.916592 sweepai-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6847 2023-07-13 00:07:11.929593 sweepai-0.4.2/README.md
+-rw-r--r--   0        0        0     1395 2023-07-13 00:08:34.469618 sweepai-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/__init__.py
+-rw-r--r--   0        0        0    12248 2023-07-11 20:05:05.034619 sweepai-0.4.2/sweepai/api.py
+-rw-r--r--   0        0        0     6020 2023-07-11 09:20:00.556075 sweepai-0.4.2/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10421 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1166 2023-07-09 08:40:46.465379 sweepai-0.4.2/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3563 2023-07-13 00:08:02.099608 sweepai-0.4.2/sweepai/app/config.py
+-rw-r--r--   0        0        0    14559 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17835 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2867 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8306 2023-07-11 20:16:30.901906 sweepai-0.4.2/sweepai/core/entities.py
+-rw-r--r--   0        0        0      561 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16809 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/core/react.py
+-rw-r--r--   0        0        0    20567 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12695 2023-07-09 08:40:46.468712 sweepai-0.4.2/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3176 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     6715 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2571 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9645 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.4.2/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19731 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3786 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0     2269 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/config.py
+-rw-r--r--   0        0        0     1131 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     6525 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8225 2023-07-09 08:40:46.468712 sweepai-0.4.2/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     8021 2023-07-13 00:10:09.537208 sweepai-0.4.2/setup.py
+-rw-r--r--   0        0        0     7799 2023-07-13 00:10:09.537661 sweepai-0.4.2/PKG-INFO
```

### Comparing `sweepai-0.4.1/LICENSE` & `sweepai-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/README.md` & `sweepai-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
 1. 🔍 reads your codebase
 2. 📝 plans the changes
 3. ⚡**writes a pull request with code**⚡
 
 See highlights at https://docs.sweep.dev/examples.
 
-## ✨ Demo
-For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
-
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
 ## 🌠 Sweep
 * 🔧 Turns issues directly into pull requests (without an IDE)
 * 👀 Addresses developer replies & comments on its PRs
 * 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
 * 🎊 New: Fixes PRs based on Github Actions feedback
@@ -60,14 +57,27 @@
 |-----------|------------|----------------------|
 |In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|
 |In `on_comment.py`|we should not fire an event|because it's possible that the comment is on a closed PR|
 |In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|
 
 If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
 
+#### Limitations:
+Sweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep's limitations(for now):
+- Try to change less than 200 lines of code
+- Try to modify less than 3 files
+- Do not include files with more than 1500 lines of code
+
+### ✨ Sweep Github App
+Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
+
+1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
 1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
     - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
@@ -89,26 +99,18 @@
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
 2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
-### ✨ Sweep Github App
-Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
-We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
-
-1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Create new issue in repo, like "Sweep: Write tests"
-3. Watch the magic happen 🪄
-
 ## 🤝 Contributing
 
 Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).
+For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
 
 ## 📘 Story
 
 We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
 
 Unlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.
```

#### html2text {}

```diff
@@ -5,42 +5,49 @@
 ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
 Sweep is an AI junior developer that transforms bug reports & feature requests
 into code changes. Describe bugs, small features, and refactors like you would
 to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
 changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
-docs.sweep.dev/examples. ## â¨ Demo For the best experience, [install Sweep]
-(https://github.com/apps/sweep-ai) to one of your repos and see the magic
-happen. [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-
-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns issues directly into pull
-requests (without an IDE) * ð Addresses developer replies & comments on its
-PRs * ðµï¸ââï¸ Uses embedding-based code search, with popularity
-reranking for repository-level code understanding ([ð Rebuilding our Search
-Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-
-in-a-day)) * ð New: Fixes PRs based on Github Actions feedback * ð New:
-Sweep Chat, a local interface for Sweep (see below) ## ð Getting Started ###
-ð² Recipes #### To get the best performance from Sweep, we recommend the
-following approach to writing github issues/chats. For harder problems, try to
-provide the same information a human would need. For simpler problems,
-providing a single line and a file name should suffice. A good issue might
-include: | Where to look
+docs.sweep.dev/examples. [Demo](https://github.com/sweepai/sweep/assets/
+44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns
+issues directly into pull requests (without an IDE) * ð Addresses developer
+replies & comments on its PRs * ðµï¸ââï¸ Uses embedding-based code
+search, with popularity reranking for repository-level code understanding (
+[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-
+rebuilt-our-code-search-engine-in-a-day)) * ð New: Fixes PRs based on Github
+Actions feedback * ð New: Sweep Chat, a local interface for Sweep (see
+below) ## ð Getting Started ### ð² Recipes #### To get the best
+performance from Sweep, we recommend the following approach to writing github
+issues/chats. For harder problems, try to provide the same information a human
+would need. For simpler problems, providing a single line and a file name
+should suffice. A good issue might include: | Where to look
 **[file name or function name]**| What to do
 **[change the logic to do this]** | Additional Context (optional)
 **[there's a bug/we need this feature/there's this dependency]** | |-----------
 |------------|----------------------| |In `sweepai/app/ui.py`|use an os-
 agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
 event|because it's possible that the comment is on a closed PR| |In the config
 loader in `packages/server/src/config.ts`|add a third option called "env" to
 load the config settings from environment variables| At present, there are two
 options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
 full path. Similarly, to have Sweep use a function, try to mention the class
 method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
-docs.sweep.dev/tricks). ### ð¥ï¸ Sweep Chat Sweep Chat allows you to
-interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
+docs.sweep.dev/tricks). #### Limitations: Sweep is unlikely to complete complex
+issues on the first try, similar to the average junior developer. Here are
+Sweep's limitations(for now): - Try to change less than 200 lines of code - Try
+to modify less than 3 files - Do not include files with more than 1500 lines of
+code ### â¨ Sweep Github App Setting up Sweep is as simple as adding the
+GitHub bot to a repo, then creating an issue for the bot to address. We support
+all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C#
+and C++. 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to
+desired repos 2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py
+use an os-agnostic temp directory" ### ð¥ï¸ Sweep Chat Sweep Chat allows you
+to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
 then have it create the pull request for you. **Prerequisites:** Install [Sweep
 GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
 install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
 run `pip3 install --force-reinstall sweepai && sweep` if the previous command
 fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
 8-digit code from your terminal into the page. You should only need to do the
 authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
@@ -48,24 +55,19 @@
 this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
 gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
 right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
 ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 #### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ### â¨ Sweep
-Github App Setting up Sweep is as simple as adding the GitHub bot to a repo,
-then creating an issue for the bot to address. We support all languages GPT4
-supports, including Python, Typescript, Rust, Go, Java, C# and C++. 1. Add the
-[Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos 2. Create
-new issue in repo, like "Sweep: Write tests" 3. Watch the magic happen ðª ##
-ð¤ Contributing Contributions are welcome and greatly appreciated! For
-detailed guidelines on how to contribute, please see the [CONTRIBUTING.md]
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð¤
+Contributing Contributions are welcome and greatly appreciated! For detailed
+guidelines on how to contribute, please see the [CONTRIBUTING.md]
 (CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/start). ## ð Story We were frustrated by small tickets, like
+docs.sweep.dev/). ## ð Story We were frustrated by small tickets, like
 simple bug fixes, annoying refactors, and small features. Each task required us
 to open our IDE to fix simple bugs. So we decided to leverage the capabilities
 of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
 this can solve entire tickets and can be parallelized + asynchronous:
 developers can spin up 10 tickets and Sweep will address them all at once. ##
 ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
 with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
```

### Comparing `sweepai-0.4.1/pyproject.toml` & `sweepai-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.1"
+version = "0.4.2"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.1/sweepai/api.py` & `sweepai-0.4.2/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/app/api_client.py` & `sweepai-0.4.2/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/app/backend.py` & `sweepai-0.4.2/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/app/cli.py` & `sweepai-0.4.2/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/app/config.py` & `sweepai-0.4.2/sweepai/app/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+from __future__ import annotations
+
 import os
 import time
-from typing import Self
 import requests
 from urllib.parse import parse_qs, unquote
 import webbrowser
 
 from config_path import ConfigPath
 from pydantic import BaseModel
 import yaml
 
-from sweepai.core.entities import Snippet
-
 CLIENT_ID = "Iv1.91fd31586a926a9f"
 
 DEVICE_CODE_ENDPOINT = "https://github.com/login/device/code"
 USER_LOGIN_ENDPOINT = "https://github.com/login/device"
 OAUTH_ACCESS_TOKEN_ENDPOINT = "https://github.com/login/oauth/access_token"
 
 config_path = ConfigPath( 'sweep_chat', 'sweep', '.yaml' )
@@ -83,15 +82,15 @@
             yaml.dump(self.dict(), f)
     
     @staticmethod
     def is_initialized() -> bool:
         return os.path.exists(CONFIG_FILE)
     
     @classmethod
-    def load(cls, recreate=False) -> Self:
+    def load(cls, recreate=False) -> SweepChatConfig:
         if recreate or not SweepChatConfig.is_initialized():
             config = cls.create()
             config.save()
             return config
         with open(CONFIG_FILE, "r") as f:
             return cls(**yaml.load(f, Loader=yaml.FullLoader))
```

### Comparing `sweepai-0.4.1/sweepai/app/ui.py` & `sweepai-0.4.2/sweepai/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/core/chat.py` & `sweepai-0.4.2/sweepai/core/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,25 @@
     
     def call_openai(
         self, 
         model: ChatModel | None = None,
         functions: list[Function] = [],
         function_name: dict | None = None,
     ):
-        if model is None:
-            model = self.model
+        if self.chat_logger:
+            tickets_allocated = 60 if self.chat_logger.is_paying_user() else 3
+            tickets_count = self.chat_logger.get_ticket_count()
+            if tickets_count < tickets_allocated:
+                model = model or self.model
+                logger.warning(f"{tickets_count} tickets found in MongoDB, using {model}")
+            else:
+                model = "gpt-3.5-turbo-16k-0613"
+        else:
+            model = "gpt-3.5-turbo-16k-0613"
+        
         count_tokens = modal.Function.lookup(UTILS_NAME, "Tiktoken.count")
         messages_length = sum(
             [count_tokens.call(message.content or "") for message in self.messages]
         )
         max_tokens = model_to_max_tokens[model] - int(messages_length) - 400 # this is for the function tokens
         # TODO: Add a check to see if the message is too long
         logger.info("file_change_paths" + str(self.file_change_paths))
```

### Comparing `sweepai-0.4.1/sweepai/core/code_repair.py` & `sweepai-0.4.2/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/core/entities.py` & `sweepai-0.4.2/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/core/gha_extraction.py` & `sweepai-0.4.2/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/core/prompts.py` & `sweepai-0.4.2/sweepai/core/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,16 +319,16 @@
 * lines a-b
 ...
 ```
 
 Code Generation:
 ```
 Generate a new_file based on the given plan, ensuring that you:
-1. It is imperative that we do not leave any work to the user/future readers of this code. So, WRITE FUNCTIONS COMPLETELY THAT WILL WORK.
-2. Do not write the original line numbers with the new code.
+1. It is imperative that we do not leave any work to the user/future readers of this code. Therefore write functions with complete business logic.
+2. Only write code, do not write line numbers.
 3. Make sure the new code follows the same programming language conventions as the old code.
 
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copy_lines A-B>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copy_lines 1-50>".
 
 Example: If you want to modify lines 51-52 and add line after line 75:
 <new_file>
```

### Comparing `sweepai-0.4.1/sweepai/core/react.py` & `sweepai-0.4.2/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/core/sweep_bot.py` & `sweepai-0.4.2/sweepai/core/sweep_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     modify_file_prompt_2,
     modify_file_plan_prompt,
 )
 from sweepai.utils.config import SweepConfig
 from sweepai.utils.constants import DB_NAME, SECONDARY_MODEL
 from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown, revert_whitespace_changes
 
+class MaxTokensExceeded(Exception):
+    def __init__(self, filename):
+        self.filename = filename
 
 class CodeGenBot(ChatGPT):
 
     def get_files_to_change(self, retries=2):
         file_change_requests: list[FileChangeRequest] = []
         # Todo: put retries into a constants file
         # also, this retries multiple times as the calls for this function are in a for loop
@@ -130,16 +133,29 @@
     def check_path_exists(self, path: str, branch: str = ""):
         try:
             self.get_contents(path, branch)
             return True
         except Exception:
             return False
 
+    def clean_branch_name(self, branch: str) -> str:
+        # Replace invalid characters with underscores
+        branch = re.sub(r"[^a-zA-Z0-9_\-/]", "_", branch)
+
+        # Remove consecutive underscores
+        branch = re.sub(r"_+", "_", branch)
+
+        # Remove leading or trailing underscores
+        branch = branch.strip("_")
+
+        return branch
+
     def create_branch(self, branch: str, retry=True) -> str:
         # Generate PR if nothing is supplied maybe
+        branch = self.clean_branch_name(branch)
         base_branch = self.repo.get_branch(SweepConfig.get_branch(self.repo))
         try:
             self.repo.create_git_ref(f"refs/heads/{branch}", base_branch.commit.sha)
             return branch
         except GithubException as e:
             logger.error(f"Error: {e}, trying with other branch names...")
             if retry:
@@ -327,23 +343,28 @@
                     ),
                     message_key=f"file_change_{file_change_request.filename}",
                 )
                 """
 
                 # Todo: updated code is outdated by unified v2 prompt! remove?
                 key = f"file_change_modified_{file_change_request.filename}"
-                modify_file_response = self.chat(
-                    modify_file_prompt_2.format(
-                        filename=file_change_request.filename,
-                        instructions=file_change_request.instructions,
-                        code=contents_line_numbers,
-                        line_count=contents.count('\n') + 1
-                    ),
-                    message_key=key,
-                )
+                try:
+                    modify_file_response = self.chat(
+                        modify_file_prompt_2.format(
+                            filename=file_change_request.filename,
+                            instructions=file_change_request.instructions,
+                            code=contents_line_numbers,
+                            line_count=contents.count('\n') + 1
+                        ),
+                        message_key=key,
+                    )
+                except Exception as e: # Check for max tokens error
+                    if "max tokens" in str(e).lower():
+                        raise MaxTokensExceeded(file_change_request.filename)
+
                 try:
                     logger.info(f"modify_file_response: {modify_file_response}")
                     new_file = generate_new_file(modify_file_response, contents)
                     if not is_markdown(file_change_request.filename):
                         code_repairer = CodeRepairer(chat_logger=self.chat_logger)
                         diff = generate_diff(old_code=contents, new_code=new_file)
                         new_file = code_repairer.repair_code(diff=diff, user_code=new_file, feature=file_change_request.instructions)
@@ -378,14 +399,16 @@
         for file_change_request in file_change_requests:
             try:
                 file_markdown = is_markdown(file_change_request.filename)
                 if file_change_request.change_type == "create":
                     self.handle_create_file(file_change_request, branch, file_markdown)
                 elif file_change_request.change_type == "modify":
                     self.handle_modify_file(file_change_request, branch, file_markdown)
+            except MaxTokensExceeded as e:
+                raise e
             except Exception as e:
                 logger.error(f"Error in change_files_in_github {e}")
             completed += 1
         return completed, num_fcr
 
     def handle_create_file(self, file_change_request: FileChangeRequest, branch: str, file_markdown: bool):
         try:
@@ -430,9 +453,11 @@
                 self.repo.update_file(
                     file_name,
                     f'Update {file_name}',
                     new_file_contents,
                     contents.sha,
                     branch=branch,
                 )
+        except MaxTokensExceeded as e:
+            raise e
         except Exception as e:
             logger.info(f"Error in handle_modify_file: {e}")
```

### Comparing `sweepai-0.4.1/sweepai/core/vector_db.py` & `sweepai-0.4.2/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/events.py` & `sweepai-0.4.2/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/handlers/create_pr.py` & `sweepai-0.4.2/sweepai/handlers/create_pr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-"""
-Creates PR given description.
-"""
-
 import os
 import openai
 
 from loguru import logger
 import modal
 from github.Repository import Repository
 
 from sweepai.core.entities import FileChangeRequest, PullRequest
-from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.sweep_bot import SweepBot, MaxTokensExceeded
 from sweepai.handlers.on_review import review_pr
 from sweepai.utils.config import SweepConfig
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client
 from sweepai.utils.constants import DB_NAME, PREFIX, DEFAULT_CONFIG, SWEEP_CONFIG_BRANCH, SWEEP_LOGIN
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
@@ -79,14 +75,26 @@
 
         pr = sweep_bot.repo.create_pull(
             title=pull_request.title,
             body=pr_description,
             head=pull_request.branch_name,
             base=SweepConfig.get_branch(sweep_bot.repo),
         )
+    except MaxTokensExceeded as e:
+        logger.error(e)
+        posthog.capture(
+            username,
+            "failed",
+            properties={
+                "error": str(e),
+                "reason": "Max tokens exceeded",
+                **metadata,
+            },
+        )
+        raise e
     except openai.error.InvalidRequestError as e:
         logger.error(e)
         posthog.capture(
             username,
             "failed",
             properties={
                 "error": str(e),
@@ -106,14 +114,15 @@
                 **metadata,
             },
         )
         raise e
 
     posthog.capture(username, "success", properties={**metadata})
     logger.info("create_pr success")
+    sweep_bot.chat_logger.add_successful_ticket()
     return {"success": True, "pull_request": pr}
 
 def safe_delete_sweep_branch(
     pr, # Github PullRequest
     repo: Repository,
 ) -> bool:
     """
@@ -161,26 +170,25 @@
         base=SweepConfig.get_branch(sweep_bot.repo),
         head=branch_name,
     )
     for pr in pull_requests:
         if pr.title == title:
             return pr
 
-    pr_description = "Config file allows for customization of Sweep."
     pr = sweep_bot.repo.create_pull(
         title=title,
         body=
 """🎉 Thank you for installing Sweep! We're thrilled to announce the latest update for Sweep, your trusty AI junior developer on GitHub. This PR creates a `sweep.yaml` config file, allowing you to personalize Sweep's performance according to your project requirements.
 
 ## What's new?
 - **Sweep is now configurable**. 
 - To configure Sweep, simply edit the `sweep.yaml` file in the root of your repository.
-- If you need help, check out the [Sweep Default Config](https://github.com/sweepai/sweep/blob/main/.github/sweep.yaml) or [Join Our Discord](https://discord.com/invite/sweep-ai) for help.
+- If you need help, check out the [Sweep Default Config](https://github.com/sweepai/sweep/blob/main/sweep.yaml) or [Join Our Discord](https://discord.gg/sweep-ai) for help.
 
-If you would like me to stop creating this PR, go to issues and say "Sweep: create an empty `.github/sweep.yaml` file".
+If you would like me to stop creating this PR, go to issues and say "Sweep: create an empty `sweep.yaml` file".
 Thank you for using Sweep! 🧹
 """,
         head=branch_name,
         base=SweepConfig.get_branch(sweep_bot.repo),
     )
 
     return pr
```

### Comparing `sweepai-0.4.1/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.2/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/handlers/on_comment.py` & `sweepai-0.4.2/sweepai/handlers/on_comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 On Github ticket, get ChatGPT to deal with it
 """
 
 # TODO: Add file validation
 
 import os
 import openai
+import traceback
 
 from loguru import logger
 
 from sweepai.core.entities import NoFilesException, Snippet
 from sweepai.core.sweep_bot import SweepBot
 from sweepai.handlers.on_review import get_pr_diffs
 from sweepai.utils.event_logger import posthog
@@ -21,20 +22,19 @@
 from sweepai.utils.constants import PREFIX
 from sweepai.utils.chat_logger import ChatLogger
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 num_of_snippets_to_query = 30
-max_num_of_snippets = 3
 total_number_of_snippet_tokens = 15_000
 num_full_files = 2
 num_extended_snippets = 2
 
-def post_process_snippets(snippets: list[Snippet]):
+def post_process_snippets(snippets: list[Snippet], max_num_of_snippets: int = 3):
     for snippet in snippets[:num_full_files]:
         snippet = snippet.expand()
 
     # snippet fusing
     i = 0
     while i < len(snippets):
         j = i + 1
@@ -139,17 +139,34 @@
             raise error
         snippets, tree = fetch_file_contents_with_retry()
         logger.info("Fetching relevant files...")
         try:
             snippets, tree = fetch_file_contents_with_retry()
             assert len(snippets) > 0
         except Exception as e:
+            logger.error(traceback.format_exc())
             logger.error(e)
             raise e
-        snippets = post_process_snippets(snippets)
+        chat_logger = ChatLogger({
+            'repo_name': repo_name,
+            'title': '(Comment) ' + pr_title,
+            "issue_url": pr.html_url,
+            "pr_file_path": pr_file_path,  # may be None
+            "pr_line": pr_line,  # may be None
+            "repo_full_name": repo_full_name,
+            "repo_description": repo_description,
+            "comment": comment,
+            "pr_path": pr_path,
+            "pr_line_position": pr_line_position,
+            "username": username,
+            "installation_id": installation_id,
+            "pr_number": pr_number,
+            "type": "comment",
+        })
+        snippets = post_process_snippets(snippets, max_num_of_snippets=2)
 
         logger.info("Getting response from ChatGPT...")
         human_message = HumanMessageCommentPrompt(
             comment=comment,
             repo_name=repo_name,
             repo_description=repo_description if repo_description else "",
             diffs=diffs,
@@ -160,35 +177,20 @@
             summary=pr_body,
             snippets=snippets,
             pr_file_path=pr_file_path, # may be None
             pr_line=pr_line, # may be None
         )
         logger.info(f"Human prompt{human_message.construct_prompt()}")
 
-        chat_logger = ChatLogger({
-            'repo_name': repo_name,
-            'title': '(Comment) ' + pr_title,
-            "issue_url": pr.html_url,
-            "pr_file_path": pr_file_path,  # may be None
-            "pr_line": pr_line,  # may be None
-            "repo_full_name": repo_full_name,
-            "repo_description": repo_description,
-            "comment": comment,
-            "pr_path": pr_path,
-            "pr_line_position": pr_line_position,
-            "username": username,
-            "installation_id": installation_id,
-            "pr_number": pr_number,
-            "type": "comment",
-        })
         sweep_bot = SweepBot.from_system_message_content(
             # human_message=human_message, model="claude-v1.3-100k", repo=repo
-            human_message=human_message, repo=repo, chat_logger=chat_logger
+            human_message=human_message, repo=repo, chat_logger=chat_logger, model="gpt-4-32k-0613"
         )
     except Exception as e:
+        logger.error(traceback.format_exc())
         posthog.capture(username, "failed", properties={
             "error": str(e),
             "reason": "Failed to get files",
             **metadata
         })
         raise e
 
@@ -204,14 +206,15 @@
         posthog.capture(username, "failed", properties={
             "error": "No files to change",
             "reason": "No files to change",
             **metadata
         })
         return {"success": True, "message": "No files to change."}
     except Exception as e:
+        logger.error(traceback.format_exc())
         posthog.capture(username, "failed", properties={
             "error": str(e),
             "reason": "Failed to make changes",
             **metadata
         })
         raise e
 
@@ -243,12 +246,13 @@
     # Check if the file exists in the previous commit
     try:
         previous_content = repo.get_contents(pr_path, ref=previous_commit.sha)
         previous_file_content = previous_content.decoded_content.decode("utf-8")
         # Create a new commit with the previous file content
         repo.update_file(pr_path, "Revert file to previous commit", previous_file_content, current_file_sha, branch=branch_name)
     except Exception as e:
+        logger.error(traceback.format_exc())
         if e.status == 404:
             logger.warning(f"File {pr_path} was not found in previous commit {previous_commit.sha}")
         else:
             raise e
```

### Comparing `sweepai-0.4.1/sweepai/handlers/on_review.py` & `sweepai-0.4.2/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/handlers/on_ticket.py` & `sweepai-0.4.2/sweepai/handlers/on_ticket.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,60 +6,60 @@
 
 import os
 import openai
 
 from loguru import logger
 import modal
 from tabulate import tabulate
+import traceback
 
 from sweepai.core.entities import FileChangeRequest, Snippet, NoFilesException
 from sweepai.core.prompts import (
     reply_prompt,
 )
-from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.sweep_bot import SweepBot, MaxTokensExceeded
 from sweepai.core.prompts import issue_comment_prompt
 from sweepai.handlers.create_pr import create_pr, create_config_pr, safe_delete_sweep_branch
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_review import review_pr
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, search_snippets
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME, SWEEP_LOGIN
 from sweepai.utils.chat_logger import ChatLogger, discord_log_error
 from sweepai.utils.config import SweepConfig
-import traceback
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 sep = "\n---\n"
 bot_suffix_starring = "⭐ If you are enjoying Sweep, please [star our repo](https://github.com/sweepai/sweep) so more people can hear about us!"
-bot_suffix = f"\n{sep}I'm a bot that handles simple bugs and feature requests but I might make mistakes. Please be kind!\n<sup>[Join Our Discord](https://discord.com/invite/sweep-ai)"
+bot_suffix = f"\n{sep}I'm a bot that handles simple bugs and feature requests but I might make mistakes. Please be kind!"
+discord_suffix = f'\n<sup>[Join Our Discord](https://discord.com/invite/sweep-ai)'
 
 stars_suffix = "⭐ In the meantime, consider [starring our repo](https://github.com/sweepai/sweep) so more people can hear about us!"
 
 collapsible_template = '''
 <details>
   <summary>{summary}</summary>
 
   {body}
 </details>
 '''
 
 chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
 
 num_of_snippets_to_query = 30
-max_num_of_snippets = 5
 total_number_of_snippet_tokens = 15_000
 num_full_files = 2
 num_extended_snippets = 2
 
-def post_process_snippets(snippets: list[Snippet]):
+def post_process_snippets(snippets: list[Snippet], max_num_of_snippets: int = 5):
     for snippet in snippets[:num_full_files]:
         snippet = snippet.expand()
 
     # snippet fusing
     i = 0
     while i < len(snippets):
         j = i + 1
@@ -115,35 +115,57 @@
         "function": "on_ticket",
         "mode": PREFIX,
     }
     posthog.capture(username, "started", properties=metadata)
 
     g = get_github_client(installation_id)
 
-    if comment_id:
-        logger.info(f"Replying to comment {comment_id}...")
     logger.info(f"Getting repo {repo_full_name}")
     repo = g.get_repo(repo_full_name)
     current_issue = repo.get_issue(number=issue_number)
     if current_issue.state == 'closed':
         posthog.capture(username, "issue_closed", properties=metadata)
         return {"success": False, "reason": "Issue is closed"}
     item_to_react_to = current_issue.get_comment(comment_id) if comment_id else current_issue
+    replies_text = ""
+    comments = list(current_issue.get_comments())
+    if comment_id:
+        
+        logger.info(f"Replying to comment {comment_id}...")
+        replies_text = "\nComments:\n" + "\n".join(
+            [
+                issue_comment_prompt.format(
+                    username=comment.user.login,
+                    reply=comment.body,
+                ) for comment in comments if comment.user.type == "User"
+            ]
+        )
+    
+    chat_logger = ChatLogger({
+        'repo_name': repo_name,
+        'title': title,
+        'summary': summary + replies_text,
+        "issue_number": issue_number,
+        "issue_url": issue_url,
+        "username": username,
+        "repo_full_name": repo_full_name,
+        "repo_description": repo_description,
+        "installation_id": installation_id,
+        "comment_id": comment_id,
+    })
 
     # Check if branch was already created for this issue
     preexisting_branch = None
     prs = repo.get_pulls(state='open', sort='created', base=SweepConfig.get_branch(repo))
     for pr in prs:
         # Check if this issue is mentioned in the PR, and pr is owned by bot
         # This is done in create_pr, (pr_description = ...)
         if pr.user.login == SWEEP_LOGIN and f'Fixes #{issue_number}.\n' in pr.body:
             success = safe_delete_sweep_branch(pr, repo)
 
-    comments = list(current_issue.get_comments())
-
     # Add emojis
     eyes_reaction = item_to_react_to.create_reaction("eyes")
     # If SWEEP_BOT reacted to item_to_react_to with "rocket", then remove it.
     reactions = item_to_react_to.get_reactions()
     for reaction in reactions:
         if reaction.content == "rocket" and reaction.user.login == SWEEP_LOGIN:
             item_to_react_to.delete_reaction(reaction.id)
@@ -168,15 +190,20 @@
         index = min(100, index)
         if errored:
             return f"![{index}%](https://progress-bar.dev/{index}/?&title=Errored&width=600)"
         return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + ("\n" + stars_suffix + config_pr_message if index != -1 else "")
 
     # Find the first comment made by the bot
     issue_comment = None
-    first_comment = f"{get_comment_header(0)}\n{sep}I am currently looking into this ticket! I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.\n{sep}## {progress_headers[1]}\nWorking on it...{bot_suffix}"
+    is_paying_user = chat_logger.is_paying_user()
+    tickets_allocated = 60 if is_paying_user else 3
+    ticket_count = max(tickets_allocated - chat_logger.get_ticket_count(), 0)
+    use_faster_model = chat_logger.use_faster_model()
+    payment_message = f"To create this ticket, I used {'gpt-3.5. ' if use_faster_model else 'gpt-4. '}You have {ticket_count} gpt-4 tickets left." + (" For more gpt-4 tickets, visit [our payment portal.](https://buy.stripe.com/fZe03512h99u0AE6os)" if not is_paying_user else "")
+    first_comment = f"{get_comment_header(0)}\n{sep}I am currently looking into this ticket!. I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.\n{sep}## {progress_headers[1]}\nWorking on it...{bot_suffix}{discord_suffix}"
     for comment in comments:
         if comment.user.login == SWEEP_LOGIN:
             issue_comment = comment
             issue_comment.edit(first_comment)
             break
     if issue_comment is None:
         issue_comment = current_issue.create_comment(first_comment)
@@ -202,30 +229,22 @@
             if header is not None: header = "## " + header + "\n"
             else: header = "No header\n"
             msg = header + (past_messages.get(i) or "Working on it...")
             if agg_message is None:
                 agg_message = msg
             else:
                 agg_message = agg_message + f"\n{sep}" + msg
+
+        suffix = bot_suffix + discord_suffix
         if errored:
             agg_message = "## ❌ Unable to Complete PR" + '\n' + message + "\nIf you would like to report this bug, please join our **[Discord](https://discord.com/invite/sweep-ai)**."
+            suffix = bot_suffix # don't include discord suffix for error messages
 
         # Update the issue comment
-        issue_comment.edit(f"{get_comment_header(current_index, errored, pr_message)}\n{sep}{agg_message}{bot_suffix}")
-
-    replies_text = ""
-    if comment_id:
-        replies_text = "\nComments:\n" + "\n".join(
-            [
-                issue_comment_prompt.format(
-                    username=comment.user.login,
-                    reply=comment.body,
-                ) for comment in comments if comment.user.type == "User"
-            ]
-        )
+        issue_comment.edit(f"{get_comment_header(current_index, errored, pr_message)}\n{sep}{agg_message}{suffix}")
 
     def log_error(error_type, exception):
         content = f"**{error_type} Error**\n{username}: {issue_url}\n```{exception}```"
         discord_log_error(content)
 
     def fetch_file_contents_with_retry():
         retries = 3
@@ -249,47 +268,38 @@
         raise error
 
     logger.info("Fetching relevant files...")
     try:
         snippets, tree = fetch_file_contents_with_retry()
         assert len(snippets) > 0
     except Exception as e:
+        trace = traceback.format_exc()
         logger.error(e)
+        logger.error(trace)
         edit_sweep_comment(
             "It looks like an issue has occured around fetching the files. Perhaps the repo has not been initialized: try removing this repo and adding it back. I'll try again in a minute. If this error persists contact team@sweep.dev.",
             -1
         )
-        log_error("File Fetch", str(e))
+        log_error("File Fetch", str(e) + "\n" + traceback.format_exc())
         raise e
     
-    snippets = post_process_snippets(snippets)
+    snippets = post_process_snippets(snippets, 
+                                     max_num_of_snippets=2 if use_faster_model else 5)
 
     human_message = HumanMessagePrompt(
         repo_name=repo_name,
         issue_url=issue_url,
         username=username,
         repo_description=repo_description,
         title=title,
         summary=summary + replies_text,
         snippets=snippets,
         tree=tree, # TODO: Anything in repo tree that has something going through is expanded
     )
 
-    chat_logger = ChatLogger({
-        'repo_name': repo_name,
-        'title': title,
-        'summary': summary + replies_text,
-        "issue_number": issue_number,
-        "issue_url": issue_url,
-        "username": username,
-        "repo_full_name": repo_full_name,
-        "repo_description": repo_description,
-        "installation_id": installation_id,
-        "comment_id": comment_id,
-    })
     sweep_bot = SweepBot.from_system_message_content(
         human_message=human_message, repo=repo, is_reply=bool(comments), chat_logger=chat_logger
     )
 
 
     # Check repository for sweep.yml file.
     sweep_yml_exists = False
@@ -302,15 +312,15 @@
     if not sweep_yml_exists:
         try:
             logger.info("Creating sweep.yaml file...")
             config_pr = create_config_pr(sweep_bot)
             config_pr_url = config_pr.html_url
             edit_sweep_comment(message="", index=-2)
         except Exception as e:
-            logger.error("Failed to create new branch for sweep.yaml file.\n", e)
+            logger.error("Failed to create new branch for sweep.yaml file.\n", e, traceback.format_exc())
     else:
         logger.info("sweep.yaml file already exists.")
 
 
     sweepbot_retries = 3
     try:
         for i in range(sweepbot_retries):
@@ -319,15 +329,15 @@
                 logger.info("CoT retrieval...")
                 sweep_bot.cot_retrieval()
             else:
                 logger.info("Did not execute CoT retrieval...")
 
             newline = '\n'
             edit_sweep_comment(
-                "I found the following snippets in your repository. I will now analyze this snippets and come up with a plan."
+                "I found the following snippets in your repository. I will now analyze these snippets and come up with a plan."
                 + "\n\n"
                 + collapsible_template.format(
                     summary="Some code snippets I looked at (click to expand). If some file is missing from here, you can mention the path in the ticket description.",
                     body="\n".join(
                         [
                             f"https://github.com/{organization}/{repo_name}/blob/{repo.get_commits()[0].sha}/{snippet.file_path}#L{max(snippet.start, 1)}-L{min(snippet.end, snippet.content.count(newline))}\n"
                             for snippet in snippets
@@ -353,17 +363,16 @@
             )
 
             # CREATE PR METADATA
             logger.info("Generating PR...")
             pull_request = sweep_bot.generate_pull_request()
             pull_request_content = pull_request.content.strip().replace("\n", "\n>")
             pull_request_summary = f"**{pull_request.title}**\n`{pull_request.branch_name}`\n>{pull_request_content}\n"
-
             edit_sweep_comment(
-                f"I have created a plan for writing the pull request. I am now working on executing my plan and coding the required changes to address this issue. Here is the planned pull request:\n\n{pull_request_summary}",
+                f"I have created a plan for writing the pull request. I am now working my plan and coding the required changes to address this issue. Here is the planned pull request:\n\n{pull_request_summary}",
                 3
             )
 
             # WRITE PULL REQUEST
             logger.info("Making PR...")
             response = create_pr(file_change_requests, pull_request, sweep_bot, username, installation_id, issue_number)
             if not response or not response["success"]: raise Exception("Failed to create PR")
@@ -397,45 +406,57 @@
                 logger.error(traceback.format_exc())
                 logger.error(e)
 
             # Completed code review
             edit_sweep_comment(
                 "Success! 🚀",
                 5,
-                pr_message=f"## Here's the PR! [https://github.com/{repo_full_name}/pull/{pr.number}](https://github.com/{repo_full_name}/pull/{pr.number})",
+                pr_message=f"## Here's the PR! [https://github.com/{repo_full_name}/pull/{pr.number}](https://github.com/{repo_full_name}/pull/{pr.number}).\n{payment_message}",
             )
 
             break
+    except MaxTokensExceeded as e:
+        logger.info("Max tokens exceeded")
+        log_error("Max Tokens Exceeded", str(e) + "\n" + traceback.format_exc())
+        if chat_logger.is_paying_user():
+            edit_sweep_comment(f"Sorry, I could not edit `{e.filename}` as this file is too long. We are currently working on improved file streaming to address this issue.\n", -1)
+        else:
+            edit_sweep_comment(f"Sorry, I could not edit `{e.filename}` as this file is too long.\n\nIf this file is incorrect, please describe the desired file in the prompt. However, if you would like to edit longer files, consider upgrading to [Sweep Pro](https://sweep.dev/) for longer context lengths.\n", -1)
+        raise e
     except NoFilesException:
         logger.info("No files to change.")
+        log_error("No Files to Change", str(e) + "\n" + traceback.format_exc())
         edit_sweep_comment("Sorry, I could find any appropriate files to edit to address this issue. If this is a mistake, please provide more context and I will retry!", -1)
+        raise e
     except openai.error.InvalidRequestError as e:
+        logger.error(traceback.format_exc())
         logger.error(e)
         edit_sweep_comment(
             "I'm sorry, but it looks our model has ran out of context length. We're trying to make this happen less, but one way to mitigate this is to code smaller files. If this error persists contact team@sweep.dev.",
             -1
         )
-        log_error("Context Length", str(e))
+        log_error("Context Length", str(e) + "\n" + traceback.format_exc())
         posthog.capture(
             username,
             "failed",
             properties={
                 "error": str(e),
                 "reason": "Invalid request error / context length",
                 **metadata,
             },
         )
         raise e
     except Exception as e:
+        logger.error(traceback.format_exc())
         logger.error(e)
         edit_sweep_comment(
             "I'm sorry, but it looks like an error has occured. Try removing and re-adding the sweep label. If this error persists contact team@sweep.dev.",
             -1
         )
-        log_error("Workflow", str(e))
+        log_error("Workflow", str(e) + "\n" + traceback.format_exc())
         posthog.capture(
             username,
             "failed",
             properties={"error": str(e), "reason": "Generic error", **metadata},
         )
         raise e
     else:
```

### Comparing `sweepai-0.4.1/sweepai/utils/config.py` & `sweepai-0.4.2/sweepai/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import lru_cache
 from loguru import logger
 import yaml
 from github.Repository import Repository
 from pydantic import BaseModel
 
 class SweepConfig(BaseModel):
@@ -20,15 +22,18 @@
         return cls.parse_obj(data)
 
     @staticmethod
     @lru_cache(maxsize=None)
     def get_branch(repo: Repository) -> str:
         default_branch = repo.default_branch
         try:
-            contents = repo.get_contents(".github/sweep.yaml")
+            try:
+                contents = repo.get_contents("sweep.yaml")
+            except Exception:
+                contents = repo.get_contents(".github/sweep.yaml")
             branch_name = yaml.safe_load(contents.decoded_content.decode("utf-8"))["branch"]
             try:
                 repo.get_branch(branch_name)
                 return branch_name
             except Exception as e:
                 logger.warning(f"Error when getting branch: {e}, creating branch")
                 repo.create_git_ref(f"refs/heads/{branch_name}", repo.get_branch(default_branch).commit.sha)
@@ -37,13 +42,16 @@
             logger.warning(f"Error when getting branch: {e}, falling back to default branch")
             return default_branch
 
     @staticmethod
     @lru_cache(maxsize=None)
     def get_gha_enabled(repo: Repository) -> bool:
         try:
-            contents = repo.get_contents(".github/sweep.yaml")
-            gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8"))["gha_enabled"]
-            return gha_enabled
+            contents = repo.get_contents("sweep.yaml")
         except Exception as e:
-            logger.warning(f"Error when getting gha enabled: {e}, falling back to False")
-            return False
+            try:
+                contents = repo.get_contents(".github/sweep.yaml")
+            except Exception as e:
+                logger.warning(f"Error when getting gha enabled: {e}, falling back to False")
+                return False
+        gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8")).get("gha_enabled", False)
+        return gha_enabled
```

### Comparing `sweepai-0.4.1/sweepai/utils/diff.py` & `sweepai-0.4.2/sweepai/utils/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 def generate_new_file(modify_file_response: str, old_file_content: str) -> str:
     import re
 
     result_file = ""
     old_file_lines = old_file_content.splitlines()
 
     # Extract content between <new_file> tags
-    new_file = re.search(r".*?<new_file>(.*)<\/new_file>", modify_file_response, re.DOTALL).group(1).strip()
+    new_file = re.search(r".*?<new_file>\n(.*)\n<\/new_file>", modify_file_response, re.DOTALL).group(1)
     if "<copy_lines" not in new_file:
         return new_file
 
     # v5
     result = []
     lines = new_file.split('\n')
     for line_number, line in enumerate(lines):
```

### Comparing `sweepai-0.4.1/sweepai/utils/event_logger.py` & `sweepai-0.4.2/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/file_change_functions.py` & `sweepai-0.4.2/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/github_utils.py` & `sweepai-0.4.2/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/huggingface.py` & `sweepai-0.4.2/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.2/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/scorer.py` & `sweepai-0.4.2/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/snippets.py` & `sweepai-0.4.2/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/sweepai/utils/utils.py` & `sweepai-0.4.2/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.1/setup.py` & `sweepai-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. Watch the magic happen 🪄\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep\'s limitations(for now):\n- Try to change less than 200 lines of code\n- Try to modify less than 3 files\n- Do not include files with more than 1500 lines of code\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['GitPython>=3.1.31,<4.0.0',
 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0',
 'loguru>=0.6.0,<0.7.0', 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0',
 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0'] entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai = sweepai.app.cli:
-app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.4.1', 'description':
+app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.4.2', 'description':
 'Sweep software chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
   sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
 month]\n\n\n_[https://img.shields.io/github/stars/sweepai/sweep]\n\n\n_[https:/
   /img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]\n\n
 \n\nSweep is an AI junior developer that transforms bug reports & feature
 requests into code changes.\n\nDescribe bugs, small features, and refactors
 like you would to a junior developer, and Sweep:\n1. ð reads your
 codebase\n2. ð plans the changes\n3. â¡**writes a pull request with
-code**â¡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n## â¨
-Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-
-ai) to one of your repos and see the magic happen.\n\n[Demo](https://
-github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
+code**â¡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo]
+(https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
 0af02f2b0e47)\n\n## ð  Sweep\n* ð§ Turns issues directly into pull requests
 (without an IDE)\n* ð Addresses developer replies & comments on its PRs\n*
 ðµï¸\u200dâï¸ Uses embedding-based code search, with popularity reranking
 for repository-level code understanding ([ð Rebuilding our Search Engine in
 a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-
 day))\n* ð New: Fixes PRs based on Github Actions feedback\n* ð New:
 Sweep Chat, a local interface for Sweep (see below)\n\n## ð Getting
@@ -43,50 +41,54 @@
 agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an
 event|because it\'s possible that the comment is on a closed PR|\n|In the
 config loader in `packages/server/src/config.ts`|add a third option called
 "env" to load the config settings from environment variables| At present, there
 are two options: 1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to
 mention the full path. Similarly, to have Sweep use a function, try to mention
 the class method or what it does. Also see [â¨ Tips and tricks for Sweep]
-(https://docs.sweep.dev/tricks).\n\n### ð¥ï¸ Sweep Chat\nSweep Chat allows
-you to interact with Sweep and GitHub locally. Collaborate on the plan with
-Sweep, then have it create the pull request for you. \n\n**Prerequisites:**
-Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your
-repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need
-**python 3.10+.**\n - Alternatively run `pip3 install --force-reinstall sweepai
-&& sweep` if the previous command fails.\n - This runs GitHub authentication in
-your browser.\n\n2. Copy the ðµ blue 8-digit code from your terminal into the
-page. You should only need to do the authentication once. \n - Wait a few
-seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown
-at the top (the Github app must be installed to this repository).\n\n - â¡
-Start chatting with Sweep Chat! â¡\n\n[https://github.com/sweepai/sweep/blob/
-856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
-screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on the
-right. \n* ð Sweep Chat creates PRs when the "Create PR" button is clicked.
-\n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
+(https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to
+complete complex issues on the first try, similar to the average junior
+developer. Here are Sweep\'s limitations(for now):\n- Try to change less than
+200 lines of code\n- Try to modify less than 3 files\n- Do not include files
+with more than 1500 lines of code\n\n### â¨ Sweep Github App\nSetting up Sweep
+is as simple as adding the GitHub bot to a repo, then creating an issue for the
+bot to address.\nWe support all languages GPT4 supports, including Python,
+Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https:
+//github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like
+"Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### ð¥ï¸
+Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally.
+Collaborate on the plan with Sweep, then have it create the pull request for
+you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/
+sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note
+that you need **python 3.10+.**\n - Alternatively run `pip3 install --force-
+reinstall sweepai && sweep` if the previous command fails.\n - This runs GitHub
+authentication in your browser.\n\n2. Copy the ðµ blue 8-digit code from your
+terminal into the page. You should only need to do the authentication once. \n
+- Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from
+the dropdown at the top (the Github app must be installed to this
+repository).\n\n - â¡ Start chatting with Sweep Chat! â¡\n\n[https://
+github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
+gradio-screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on
+the right. \n* ð Sweep Chat creates PRs when the "Create PR" button is
+clicked. \n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
 ?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the
 latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep &&
 poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python
-3.10+**.\n\n### â¨ Sweep Github App\nSetting up Sweep is as simple as adding
-the GitHub bot to a repo, then creating an issue for the bot to address.\nWe
-support all languages GPT4 supports, including Python, Typescript, Rust, Go,
-Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/
-sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write
-tests"\n3. Watch the magic happen ðª\n\n## ð¤ Contributing\n\nContributions
-are welcome and greatly appreciated! For detailed guidelines on how to
-contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more
-detailed docs, see [ð Quickstart](https://docs.sweep.dev/start).\n\n## ð
-Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying
-refactors, and small features. Each task required us to open our IDE to fix
-simple bugs. So we decided to leverage the capabilities of ChatGPT to address
-this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire
-tickets and can be parallelized + asynchronous: developers can spin up 10
-tickets and Sweep will address them all at once.\n\n## ð The Stack\n- GPT-
-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as
-our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep
+3.10+**.\n\n## ð¤ Contributing\n\nContributions are welcome and greatly
+appreciated! For detailed guidelines on how to contribute, please see the
+[CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [ð
+Quickstart](https://docs.sweep.dev/).\n\n## ð Story\n\nWe were frustrated by
+small tickets, like simple bug fixes, annoying refactors, and small features.
+Each task required us to open our IDE to fix simple bugs. So we decided to
+leverage the capabilities of ChatGPT to address this directly in
+GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can
+be parallelized + asynchronous: developers can spin up 10 tickets and Sweep
+will address them all at once.\n\n## ð The Stack\n- GPT-4 32k 0613
+(default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our
+embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep
 Chat\n\n## ðºï¸ Roadmap\nSee [ðºï¸ Roadmap](https://docs.sweep.dev/
 roadmap)\n\n## â­ Star History\n\n[![Star History Chart](https://api.star-
 history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/
 #sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more
 people hear about us!\n
                          ***** \n Contributors\n *****
 \n
```

### Comparing `sweepai-0.4.1/PKG-INFO` & `sweepai-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.1
+Version: 0.4.2
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -57,17 +57,14 @@
 Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
 1. 🔍 reads your codebase
 2. 📝 plans the changes
 3. ⚡**writes a pull request with code**⚡
 
 See highlights at https://docs.sweep.dev/examples.
 
-## ✨ Demo
-For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
-
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
 ## 🌠 Sweep
 * 🔧 Turns issues directly into pull requests (without an IDE)
 * 👀 Addresses developer replies & comments on its PRs
 * 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
 * 🎊 New: Fixes PRs based on Github Actions feedback
@@ -85,14 +82,27 @@
 |-----------|------------|----------------------|
 |In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|
 |In `on_comment.py`|we should not fire an event|because it's possible that the comment is on a closed PR|
 |In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|
 
 If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
 
+#### Limitations:
+Sweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep's limitations(for now):
+- Try to change less than 200 lines of code
+- Try to modify less than 3 files
+- Do not include files with more than 1500 lines of code
+
+### ✨ Sweep Github App
+Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
+
+1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
 1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
     - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
@@ -114,26 +124,18 @@
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
 2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
-### ✨ Sweep Github App
-Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
-We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
-
-1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Create new issue in repo, like "Sweep: Write tests"
-3. Watch the magic happen 🪄
-
 ## 🤝 Contributing
 
 Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).
+For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
 
 ## 📘 Story
 
 We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
 
 Unlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.1 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.2 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
 tabulate (>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
@@ -18,42 +18,49 @@
 ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
 Sweep is an AI junior developer that transforms bug reports & feature requests
 into code changes. Describe bugs, small features, and refactors like you would
 to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
 changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
-docs.sweep.dev/examples. ## â¨ Demo For the best experience, [install Sweep]
-(https://github.com/apps/sweep-ai) to one of your repos and see the magic
-happen. [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-
-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns issues directly into pull
-requests (without an IDE) * ð Addresses developer replies & comments on its
-PRs * ðµï¸ââï¸ Uses embedding-based code search, with popularity
-reranking for repository-level code understanding ([ð Rebuilding our Search
-Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-
-in-a-day)) * ð New: Fixes PRs based on Github Actions feedback * ð New:
-Sweep Chat, a local interface for Sweep (see below) ## ð Getting Started ###
-ð² Recipes #### To get the best performance from Sweep, we recommend the
-following approach to writing github issues/chats. For harder problems, try to
-provide the same information a human would need. For simpler problems,
-providing a single line and a file name should suffice. A good issue might
-include: | Where to look
+docs.sweep.dev/examples. [Demo](https://github.com/sweepai/sweep/assets/
+44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns
+issues directly into pull requests (without an IDE) * ð Addresses developer
+replies & comments on its PRs * ðµï¸ââï¸ Uses embedding-based code
+search, with popularity reranking for repository-level code understanding (
+[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-
+rebuilt-our-code-search-engine-in-a-day)) * ð New: Fixes PRs based on Github
+Actions feedback * ð New: Sweep Chat, a local interface for Sweep (see
+below) ## ð Getting Started ### ð² Recipes #### To get the best
+performance from Sweep, we recommend the following approach to writing github
+issues/chats. For harder problems, try to provide the same information a human
+would need. For simpler problems, providing a single line and a file name
+should suffice. A good issue might include: | Where to look
 **[file name or function name]**| What to do
 **[change the logic to do this]** | Additional Context (optional)
 **[there's a bug/we need this feature/there's this dependency]** | |-----------
 |------------|----------------------| |In `sweepai/app/ui.py`|use an os-
 agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
 event|because it's possible that the comment is on a closed PR| |In the config
 loader in `packages/server/src/config.ts`|add a third option called "env" to
 load the config settings from environment variables| At present, there are two
 options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
 full path. Similarly, to have Sweep use a function, try to mention the class
 method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
-docs.sweep.dev/tricks). ### ð¥ï¸ Sweep Chat Sweep Chat allows you to
-interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
+docs.sweep.dev/tricks). #### Limitations: Sweep is unlikely to complete complex
+issues on the first try, similar to the average junior developer. Here are
+Sweep's limitations(for now): - Try to change less than 200 lines of code - Try
+to modify less than 3 files - Do not include files with more than 1500 lines of
+code ### â¨ Sweep Github App Setting up Sweep is as simple as adding the
+GitHub bot to a repo, then creating an issue for the bot to address. We support
+all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C#
+and C++. 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to
+desired repos 2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py
+use an os-agnostic temp directory" ### ð¥ï¸ Sweep Chat Sweep Chat allows you
+to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
 then have it create the pull request for you. **Prerequisites:** Install [Sweep
 GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
 install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
 run `pip3 install --force-reinstall sweepai && sweep` if the previous command
 fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
 8-digit code from your terminal into the page. You should only need to do the
 authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
@@ -61,24 +68,19 @@
 this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
 gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
 right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
 ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 #### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ### â¨ Sweep
-Github App Setting up Sweep is as simple as adding the GitHub bot to a repo,
-then creating an issue for the bot to address. We support all languages GPT4
-supports, including Python, Typescript, Rust, Go, Java, C# and C++. 1. Add the
-[Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos 2. Create
-new issue in repo, like "Sweep: Write tests" 3. Watch the magic happen ðª ##
-ð¤ Contributing Contributions are welcome and greatly appreciated! For
-detailed guidelines on how to contribute, please see the [CONTRIBUTING.md]
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð¤
+Contributing Contributions are welcome and greatly appreciated! For detailed
+guidelines on how to contribute, please see the [CONTRIBUTING.md]
 (CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/start). ## ð Story We were frustrated by small tickets, like
+docs.sweep.dev/). ## ð Story We were frustrated by small tickets, like
 simple bug fixes, annoying refactors, and small features. Each task required us
 to open our IDE to fix simple bugs. So we decided to leverage the capabilities
 of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
 this can solve entire tickets and can be parallelized + asynchronous:
 developers can spin up 10 tickets and Sweep will address them all at once. ##
 ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
 with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
```

