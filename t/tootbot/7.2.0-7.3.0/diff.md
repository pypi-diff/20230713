# Comparing `tmp/tootbot-7.2.0.tar.gz` & `tmp/tootbot-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootbot-7.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tootbot-7.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tootbot-7.2.0.tar` & `tootbot-7.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4489 2023-06-25 09:00:25.116817 tootbot-7.2.0/README.rst
--rw-r--r--   0        0        0     3833 2023-06-25 09:00:25.120817 tootbot-7.2.0/pyproject.toml
--rw-r--r--   0        0        0      752 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/__init__.py
--rw-r--r--   0        0        0     7645 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/app.py
--rw-r--r--   0        0        0    31346 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/collect.py
--rw-r--r--   0        0        0    18390 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/control.py
--rw-r--r--   0        0        0     4877 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/create_config.py
--rw-r--r--   0        0        0     4466 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/debug.py
--rw-r--r--   0        0        0     2472 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/monitoring.py
--rw-r--r--   0        0        0    16491 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/publish.py
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4489 2023-07-13 06:21:13.997566 tootbot-7.3.0/README.rst
+-rw-r--r--   0        0        0     3772 2023-07-13 06:21:14.001566 tootbot-7.3.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/__init__.py
+-rw-r--r--   0        0        0     7692 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/app.py
+-rw-r--r--   0        0        0    32863 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/collect.py
+-rw-r--r--   0        0        0    19177 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/control.py
+-rw-r--r--   0        0        0     4877 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/create_config.py
+-rw-r--r--   0        0        0     4603 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/debug.py
+-rw-r--r--   0        0        0     2472 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/monitoring.py
+-rw-r--r--   0        0        0    16491 2023-07-13 06:21:14.001566 tootbot-7.3.0/src/tootbot/publish.py
+-rw-r--r--   0        0        0     6314 1970-01-01 00:00:00.000000 tootbot-7.3.0/PKG-INFO
```

### Comparing `tootbot-7.2.0/README.rst` & `tootbot-7.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tootbot-7.2.0/pyproject.toml` & `tootbot-7.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,37 +20,37 @@
   "Intended Audience :: End Users/Desktop"
 ]
 
 dependencies = [
     "imgurpython>=1.1.7",
     "arrow>=1.2.3",
     "python-magic>=0.4.27",
-    "asyncpraw>=7.7.0",
+    "asyncpraw>=7.7.1",
     "outdated>=0.2.2",
     "tqdm>=4.65.0",
     "aiosqlite>=0.17.0",
-    "yt-dlp>=2023.6.22",
+    "yt-dlp>=2023.7.6",
     "minimal-activitypub>=0.5.5",
 ]
 [project.optional-dependencies]
 doc = [
-    "Sphinx>=6.1.3",
-    "python-docs-theme>=2022.1",
-    "sphinx-rtd-theme>=1.2.0",
+    "Sphinx>=6.2.1",
+    "python-docs-theme>=2023.5",
+    "sphinx-rtd-theme>=1.2.2",
 ]
 dev = [
-    "pre-commit>=3.0.4",
-    "black>=23.1.0",
-    "mypy>=1.0.0",
+    "pre-commit>=3.3.3",
+    "black>=23.7.0",
+    "mypy>=1.4.1",
     "safety>=2.3.4",
-    "pip-audit>=2.4.14",
-    "types-aiofiles>=22.1.0.8",
+    "pip-audit>=2.6.0",
+    "types-aiofiles>=23.1.0.4",
     "interrogate>=1.5.0",
-    "ruff>=0.0.247",
-    "flit>=3.8.0",
+    "ruff>=0.0.278",
+    "flit>=3.9.0",
 ]
 
 [project.scripts]
 tootbot = "tootbot.app:start_main"
 tootbot_create_config = "tootbot.create_config:create"
 tootbot_debug_submission = "tootbot.debug:start_debug_single_submission"
 
@@ -94,16 +94,14 @@
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
-[tool.pdm]
-
 [tool.ruff]
 select = ["ARG", "B", "C4", "C90", "D", "E", "ERA", "F", "I", "PL", "RUF", "S", "UP", "W"]
 ignore = ["D203", "D205", "D213"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
 unfixable = []
@@ -126,15 +124,14 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
-per-file-ignores = {}
 
 # Same as Black.
 line-length = 120
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
@@ -144,13 +141,11 @@
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.isort]
 force-single-line = true
 
-[tool.ruff.pycodestyle]
-
 [tool.scriv]
 categories = "Breaking, Added, Changed, Deprecated, Removed, Fixed, Security"
 format = "rst"
 version = "literal: src/tootbot/__init__.py: __version__"
```

### Comparing `tootbot-7.2.0/src/tootbot/__init__.py` & `tootbot-7.3.0/src/tootbot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Package 'tootbot' level definitions."""
 import sys
 from typing import Final
 
-__version__: Final[str] = "7.2.0"
+__version__: Final[str] = "7.3.0"
 __display_name__: Final[str] = "Tootbot"
 __package_name__: Final[str] = __display_name__.lower()
 
 # Package level Static Variables
 POST_RECORDER_SQLITE_DB: Final[str] = "history.db"
 POST_RECORDER_HISTORY_RETENTION_DAYS: Final[int] = 31
 USER_AGENT: Final[str] = __display_name__
```

### Comparing `tootbot-7.2.0/src/tootbot/app.py` & `tootbot-7.3.0/src/tootbot/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
     # Run the main script
     while True:
         if config.health.enabled:
             await healthcheck.check_start()
 
         await reddit.get_all_reddit_posts()
         await reddit.winnow_reddit_posts()
+        reddit.remove_posts_by_ignored_users()
         await mastodon_publisher.make_post(reddit.posts, reddit, media_helper)
 
         if config.health.enabled:
             await healthcheck.check_ok()
 
         await config.bot.post_recorder.save_setting(
             PostRecorder.LAST_POST_TS,
```

### Comparing `tootbot-7.2.0/src/tootbot/collect.py` & `tootbot-7.3.0/src/tootbot/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,14 +234,50 @@
             logger.warning(
                 "Error when getting reddit posts from r/%s: %s",
                 subreddit.name,
                 reddit_error,
             )
         return posts
 
+    def remove_posts_by_ignored_users(self: RH) -> None:
+        """Remove posts by users on the ignore list."""
+        logger.debug("RedditHelper.remove_posts_by_ignored_users() started")
+        logger.debug(
+            "RedditHelper.remove_posts_by_ignored_users() - Ingore list is: %s",
+            self.config.ignore_users_list,
+        )
+        # Guard against empty or undefined ignore users list
+        if (
+            self.config.ignore_users_list is None
+            or len(self.config.ignore_users_list) == 0
+        ):
+            logger.debug(
+                "RedditHelper.remove_posts_by_ignored_users() ignore list empty"
+            )
+            return
+
+        title = "Remove posts by 'ingored users'"
+        for posts in tqdm(
+            self.posts.values(),
+            desc=f"{title:.<60}",
+            total=len(self.posts),
+            ncols=120,
+            bar_format=PROGRESS_BAR_FORMAT,
+        ):
+            post_ids = list(posts.keys())
+            for id in post_ids:
+                logger.debug(
+                    "RedditHelper.remove_posts_by_ignored_users() - Checking post: %s from user: %s",
+                    id,
+                    posts[id].author.name,
+                )
+                if str(posts[id].author.name) in self.config.ignore_users_list:
+                    del posts[id]
+                    logger.debug("Removed post %s; post made by ignored user.", id)
+
     async def winnow_reddit_posts(self: RH) -> None:
         """Filter out reddit posts according to configuration and whether it has already been posted."""
         recorder = self.config.bot.post_recorder
         nsfw_allowed = self.config.reddit.nsfw_allowed
         self_posts_allowed = self.config.reddit.self_posts
         spoilers_allowed = self.config.reddit.spoilers
         stickied_allowed = self.config.reddit.stickied_allowed
@@ -320,15 +356,16 @@
             add_hash_tags,
             promo_message,
         )
 
         author_tag = ""
         if self.config.mastodon_config.use_redditor_tag:
             redditor: Redditor = submission.author
-            reddit_user = redditor.name
+            # "-" breaks hashtags on Mastodon, so replace any "-" with "_"
+            reddit_user = redditor.name.replace("-", "_")
             author_tag = f"posted by #u{reddit_user} "
 
         hashtags_for_post = self.config.bot.hash_tags
 
         # Workout hashtags for post
         hashtag_string = ""
         if add_hash_tags:
```

### Comparing `tootbot-7.2.0/src/tootbot/control.py` & `tootbot-7.3.0/src/tootbot/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -359,14 +359,15 @@
     bot: BotConfig
     subreddits: List[SubredditConfig]
     promo: PromoConfig
     health: HealthCheckConfig
     media: MediaConfig
     mastodon_config: MastodonConfig
     reddit: RedditReaderConfig
+    ignore_users_list: List[str]
 
     @classmethod
     async def load_config(
         cls: Type[ConfigClass],
         config_dir: str,
         debug_log: str,
     ) -> ConfigClass:
@@ -394,14 +395,17 @@
             mal = getLogger(minimal_activitypub_logger)
             mal.setLevel(DEBUG)
             mal.addHandler(file_handler)
 
         # Make sure config file exists
         try:
             config = configparser.ConfigParser()
+            # This next lines makes ConfigParser have case-sensitive settings keys which we need
+            # for dealing with reddit usernames in the config
+            config.optionxform = str  # type: ignore[method-assign, assignment]
             config.read(f"{config_dir}/config.ini")
         except configparser.Error as config_error:
             print("[ERROR] Error while reading config file: %s", config_error)
             sys.exit(1)
 
         await cls._set_up_logging(config)
         bot = await Configuration._load_bot_settings(
@@ -438,22 +442,25 @@
             link_to_media=config["Mastodon"].getboolean("MediaLink", fallback=False),
             use_redditor_tag=config["Mastodon"].getboolean(
                 "UseRedditorTag", fallback=False
             ),
         )
         subreddits = await Configuration._load_subreddits_settings(config)
 
+        ignore_users_list = Configuration._load_ignore_users_list(config)
+
         configuration = cls(
             bot=bot,
             subreddits=subreddits,
             promo=promo,
             health=health,
             media=media,
             mastodon_config=mastodon_config,
             reddit=reddit,
+            ignore_users_list=ignore_users_list,
         )
         logger.debug("After loading of config: %s", configuration)
         return configuration
 
     @staticmethod
     async def _load_subreddits_settings(
         config: configparser.ConfigParser,
@@ -461,14 +468,27 @@
         """Load Subreddit configuration options."""
         subreddits = []
         for subreddit, hashtags in config.items("Subreddits"):
             subreddits.append(SubredditConfig(subreddit, hashtags.strip()))
         return subreddits
 
     @staticmethod
+    def _load_ignore_users_list(
+        config: configparser.ConfigParser,
+    ) -> List[str]:
+        """Load ignore_users_list."""
+        ignore_users: List[str] = []
+
+        if config.has_section("IgnoreUsersList"):
+            for ignore_user, _ in config.items("IgnoreUsersList"):
+                ignore_users.append(str(ignore_user))
+
+        return ignore_users
+
+    @staticmethod
     async def _load_healthchecks_settings(
         config: configparser.ConfigParser,
     ) -> HealthCheckConfig:
         """Load HealthChecks configuration options."""
         health_enabled = False
         if len(config["HealthChecks"]["BaseUrl"]) > 0:
             health_enabled = True
```

### Comparing `tootbot-7.2.0/src/tootbot/create_config.py` & `tootbot-7.3.0/src/tootbot/create_config.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.2.0/src/tootbot/debug.py` & `tootbot-7.3.0/src/tootbot/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,17 @@
 
         submission = await reddit_con.submission(id=args.submission_id)
         logger.debug(
             "Single Submission retrieved: %s\n%s",
             args.submission_id,
             inspect.getmembers(submission),
         )
+        reddit.posts = {submission.subreddit_name_prefixed: {submission.id: submission}}
+        reddit.remove_posts_by_ignored_users()
+
         await mastodon_publisher.make_post(
             posts={submission.subreddit_name_prefixed: {submission.id: submission}},
             reddit_helper=reddit,
             media_helper=media_helper,
             duplicate_checks=False,
         )
         logger.debug("Single Submission posted successfully")
```

### Comparing `tootbot-7.2.0/src/tootbot/monitoring.py` & `tootbot-7.3.0/src/tootbot/monitoring.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.2.0/src/tootbot/publish.py` & `tootbot-7.3.0/src/tootbot/publish.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.2.0/PKG-INFO` & `tootbot-7.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: tootbot
-Version: 7.2.0
+Version: 7.3.0
 Summary: A Python bot that looks up posts from specified subreddits and automatically posts them on Mastodon
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Dist: imgurpython>=1.1.7
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: python-magic>=0.4.27
-Requires-Dist: asyncpraw>=7.7.0
+Requires-Dist: asyncpraw>=7.7.1
 Requires-Dist: outdated>=0.2.2
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: aiosqlite>=0.17.0
-Requires-Dist: yt-dlp>=2023.6.22
+Requires-Dist: yt-dlp>=2023.7.6
 Requires-Dist: minimal-activitypub>=0.5.5
-Requires-Dist: pre-commit>=3.0.4 ; extra == "dev"
-Requires-Dist: black>=23.1.0 ; extra == "dev"
-Requires-Dist: mypy>=1.0.0 ; extra == "dev"
+Requires-Dist: pre-commit>=3.3.3 ; extra == "dev"
+Requires-Dist: black>=23.7.0 ; extra == "dev"
+Requires-Dist: mypy>=1.4.1 ; extra == "dev"
 Requires-Dist: safety>=2.3.4 ; extra == "dev"
-Requires-Dist: pip-audit>=2.4.14 ; extra == "dev"
-Requires-Dist: types-aiofiles>=22.1.0.8 ; extra == "dev"
+Requires-Dist: pip-audit>=2.6.0 ; extra == "dev"
+Requires-Dist: types-aiofiles>=23.1.0.4 ; extra == "dev"
 Requires-Dist: interrogate>=1.5.0 ; extra == "dev"
-Requires-Dist: ruff>=0.0.247 ; extra == "dev"
-Requires-Dist: flit>=3.8.0 ; extra == "dev"
-Requires-Dist: Sphinx>=6.1.3 ; extra == "doc"
-Requires-Dist: python-docs-theme>=2022.1 ; extra == "doc"
-Requires-Dist: sphinx-rtd-theme>=1.2.0 ; extra == "doc"
+Requires-Dist: ruff>=0.0.278 ; extra == "dev"
+Requires-Dist: flit>=3.9.0 ; extra == "dev"
+Requires-Dist: Sphinx>=6.2.1 ; extra == "doc"
+Requires-Dist: python-docs-theme>=2023.5 ; extra == "doc"
+Requires-Dist: sphinx-rtd-theme>=1.2.2 ; extra == "doc"
 Project-URL: Bug Tracker, https://codeberg.org/MarvinsMastodonTools/tootbot/issues
 Project-URL: Changelog, https://codeberg.org/MarvinsMastodonTools/tootbot/src/branch/main/CHANGELOG.rst
 Project-URL: Wiki, https://codeberg.org/MarvinsMastodonTools/tootbot/wiki
 Project-URL: homepage, https://codeberg.org/MarvinsMastodonTools/tootbot
 Project-URL: repository, https://codeberg.org/MarvinsMastodonTools/tootbot
 Provides-Extra: dev
 Provides-Extra: doc
```

