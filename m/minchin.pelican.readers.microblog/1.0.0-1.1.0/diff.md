# Comparing `tmp/minchin.pelican.readers.microblog-1.0.0.tar.gz` & `tmp/minchin.pelican.readers.microblog-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minchin.pelican.readers.microblog-1.0.0.tar", last modified: Thu Jul 13 04:06:20 2023, max compression
+gzip compressed data, was "minchin.pelican.readers.microblog-1.1.0.tar", last modified: Thu Jul 13 21:18:00 2023, max compression
```

## Comparing `minchin.pelican.readers.microblog-1.0.0.tar` & `minchin.pelican.readers.microblog-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:20.593018 minchin.pelican.readers.microblog-1.0.0/
--rw-rw-rw-   0        0        0     1089 2023-07-11 21:21:54.000000 minchin.pelican.readers.microblog-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     8981 2023-07-13 04:06:20.593018 minchin.pelican.readers.microblog-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7871 2023-07-13 04:01:35.000000 minchin.pelican.readers.microblog-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:20.560018 minchin.pelican.readers.microblog-1.0.0/minchin/
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:20.560018 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:20.560018 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:20.592018 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/
--rw-rw-rw-   0        0        0      485 2023-07-12 04:41:29.000000 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/__init__.py
--rw-rw-rw-   0        0        0      303 2023-07-13 04:06:16.000000 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/constants.py
--rw-rw-rw-   0        0        0     3529 2023-07-12 04:45:31.000000 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/generator.py
--rw-rw-rw-   0        0        0     3826 2023-07-12 04:44:37.000000 minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/initialize.py
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:20.589018 minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/
--rw-rw-rw-   0        0        0     8981 2023-07-13 04:06:20.000000 minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-07-13 04:06:20.000000 minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 04:06:20.000000 minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-07-13 04:06:20.000000 minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-13 04:06:20.000000 minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      460 2023-07-11 21:20:38.000000 minchin.pelican.readers.microblog-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 04:06:20.593018 minchin.pelican.readers.microblog-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4752 2023-07-12 04:40:27.000000 minchin.pelican.readers.microblog-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:18:00.767513 minchin.pelican.readers.microblog-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-07-11 21:21:54.000000 minchin.pelican.readers.microblog-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    10140 2023-07-13 21:18:00.766513 minchin.pelican.readers.microblog-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9030 2023-07-13 20:59:52.000000 minchin.pelican.readers.microblog-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-13 21:18:00.738513 minchin.pelican.readers.microblog-1.1.0/minchin/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:18:00.739513 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:18:00.739513 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:18:00.765513 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/
+-rw-rw-rw-   0        0        0      485 2023-07-12 04:41:29.000000 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-07-13 21:17:57.000000 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/constants.py
+-rw-rw-rw-   0        0        0     4074 2023-07-13 21:12:09.000000 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/generator.py
+-rw-rw-rw-   0        0        0     3826 2023-07-12 04:44:37.000000 minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/initialize.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:18:00.763512 minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/
+-rw-rw-rw-   0        0        0    10140 2023-07-13 21:18:00.000000 minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-07-13 21:18:00.000000 minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:18:00.000000 minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-07-13 21:18:00.000000 minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-13 21:18:00.000000 minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      460 2023-07-11 21:20:38.000000 minchin.pelican.readers.microblog-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 21:18:00.767513 minchin.pelican.readers.microblog-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4752 2023-07-12 04:40:27.000000 minchin.pelican.readers.microblog-1.1.0/setup.py
```

### Comparing `minchin.pelican.readers.microblog-1.0.0/LICENSE.txt` & `minchin.pelican.readers.microblog-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minchin.pelican.readers.microblog-1.0.0/PKG-INFO` & `minchin.pelican.readers.microblog-1.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: minchin.pelican.readers.microblog
-Version: 1.0.0
-Summary: Microblogging for Pelican
-Home-page: http://blog.minchin.ca/label/microblog-pelican/
-Author: W. Minchin
-Author-email: w_minchin@hotmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues
-Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.readers.microblog/blob/master/CHANGELOG.rst
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: Pelican :: Plugins
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
-Provides-Extra: build
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE.txt
-
 =====================
 Pelican Microblogging
 =====================
 
 *A Pelican plugin providing "microblogging" capabilities.*
 
 .. image:: https://img.shields.io/pypi/v/minchin.pelican.readers.microblog.svg?style=flat
@@ -93,14 +65,31 @@
 
    Microblog posts can have "feature" images too! (URL of photo should
    automatically be added.)
 
 The image path is relative to your ``content`` folder. A URL of the photo is
 added to the end of the post as well.
 
+Or with tags (or hashtags):
+
+.. code-block:: md
+
+   <!-- ./content/micro/202307131456.md -->
+
+   date: 2023-07-13 14:56 -0600
+   tags: Python, Pelican, Microblogging
+
+   I'm now Microblogging with Pelican!
+
+
+This will add links at the end of your post to the tags to the tag page for
+your (Pelican) site.
+
+For now, it does not pull tags out of the body of your post.
+
 Background Notes (on Micro Blogging)
 ------------------------------------
 
 Microblogging is here considered to be blog posts, but very short in length.
 
 The most common example is Twitter, with an original limit of 140 characters
 (to be less than the SMS max of 160 characters). Twitter has since doubled
@@ -202,38 +191,55 @@
 <http://blog.minchin.ca/label/seafoam/>`_.
 
 Some helpful notes:
 
 - Microblog posts are considered ``Articles`` by Pelican, and will be included
   in the ``articles`` and ``dates`` "lists".
 - Microblog posts all have ``article.micro = True``.
-- Microblog posts are added to the ``Âµ`` category.
+- Microblog posts are added to the ``µ`` category.
 - Generally, you'll want to disregard and now show the title of the microblog
   post. The title is set to the slug.
 - Because of their short length, it may make sense to display the whole body
   (``article.content``) in places that a link via the title of the article is
   typically shown.
 
 Changelog
 ---------
 
 `Changelog <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/blob/master/CHANGELOG.rst>`_
 
 Roadmap
 -------
 
-These are features that I would like to eventually add to the plugin:
+These are features that I would like to eventually add to the plugin (and the
+issues I'm using to track their progress):
+
+- `Issue 1
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/1>`_
+  -- count links as 23 characters (*à la* Twitter)
+- `Issue 2
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/2>`_
+  -- process ReST microblog posts
+- `Issue 3
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/3>`_
+  -- CLI command to create microposts
+- `Issue 4
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/4>`_
+  -- add link previews
+- `Issue 5
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/5>`_
+  -- show (if applicable) that this is a reply to something (or a "re-tweet")
+- `Issue 6
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/6>`_
+  -- show replies to each post (borrow the comment setup?)
+- `Issue 7
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/7>`_
+  -- automatically add hashtags as (Pelican) tags
 
-- count links as 23 characters (*Ã  la* Twitter)
-- process ReST microblog posts
-- CLI command to create microposts
-- add link previews
-- show (if applicable) that this is a reply to something (or a "re-tweet")
-- show replies to each post (borrow the comment setup?)
-- automatically add hashtags as (Pelican) tags
+Pull Requests to implement any of these are welcomed!
 
 - [x] update Seafoam theme
 - [x] make sorting work for microblog posts
 
 
 Known Issues
 ------------
```

### Comparing `minchin.pelican.readers.microblog-1.0.0/README.rst` & `minchin.pelican.readers.microblog-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: minchin.pelican.readers.microblog
+Version: 1.1.0
+Summary: Microblogging for Pelican
+Home-page: http://blog.minchin.ca/label/microblog-pelican/
+Author: W. Minchin
+Author-email: w_minchin@hotmail.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues
+Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.readers.microblog/blob/master/CHANGELOG.rst
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Programming Language :: Python :: 3
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/x-rst
+Provides-Extra: build
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE.txt
+
 =====================
 Pelican Microblogging
 =====================
 
 *A Pelican plugin providing "microblogging" capabilities.*
 
 .. image:: https://img.shields.io/pypi/v/minchin.pelican.readers.microblog.svg?style=flat
@@ -65,14 +93,31 @@
 
    Microblog posts can have "feature" images too! (URL of photo should
    automatically be added.)
 
 The image path is relative to your ``content`` folder. A URL of the photo is
 added to the end of the post as well.
 
+Or with tags (or hashtags):
+
+.. code-block:: md
+
+   <!-- ./content/micro/202307131456.md -->
+
+   date: 2023-07-13 14:56 -0600
+   tags: Python, Pelican, Microblogging
+
+   I'm now Microblogging with Pelican!
+
+
+This will add links at the end of your post to the tags to the tag page for
+your (Pelican) site.
+
+For now, it does not pull tags out of the body of your post.
+
 Background Notes (on Micro Blogging)
 ------------------------------------
 
 Microblogging is here considered to be blog posts, but very short in length.
 
 The most common example is Twitter, with an original limit of 140 characters
 (to be less than the SMS max of 160 characters). Twitter has since doubled
@@ -174,38 +219,55 @@
 <http://blog.minchin.ca/label/seafoam/>`_.
 
 Some helpful notes:
 
 - Microblog posts are considered ``Articles`` by Pelican, and will be included
   in the ``articles`` and ``dates`` "lists".
 - Microblog posts all have ``article.micro = True``.
-- Microblog posts are added to the ``µ`` category.
+- Microblog posts are added to the ``Âµ`` category.
 - Generally, you'll want to disregard and now show the title of the microblog
   post. The title is set to the slug.
 - Because of their short length, it may make sense to display the whole body
   (``article.content``) in places that a link via the title of the article is
   typically shown.
 
 Changelog
 ---------
 
 `Changelog <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/blob/master/CHANGELOG.rst>`_
 
 Roadmap
 -------
 
-These are features that I would like to eventually add to the plugin:
+These are features that I would like to eventually add to the plugin (and the
+issues I'm using to track their progress):
+
+- `Issue 1
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/1>`_
+  -- count links as 23 characters (*Ã  la* Twitter)
+- `Issue 2
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/2>`_
+  -- process ReST microblog posts
+- `Issue 3
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/3>`_
+  -- CLI command to create microposts
+- `Issue 4
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/4>`_
+  -- add link previews
+- `Issue 5
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/5>`_
+  -- show (if applicable) that this is a reply to something (or a "re-tweet")
+- `Issue 6
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/6>`_
+  -- show replies to each post (borrow the comment setup?)
+- `Issue 7
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/7>`_
+  -- automatically add hashtags as (Pelican) tags
 
-- count links as 23 characters (*à la* Twitter)
-- process ReST microblog posts
-- CLI command to create microposts
-- add link previews
-- show (if applicable) that this is a reply to something (or a "re-tweet")
-- show replies to each post (borrow the comment setup?)
-- automatically add hashtags as (Pelican) tags
+Pull Requests to implement any of these are welcomed!
 
 - [x] update Seafoam theme
 - [x] make sorting work for microblog posts
 
 
 Known Issues
 ------------
```

### Comparing `minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/generator.py` & `minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -67,14 +67,26 @@
             image_url = f'{settings["SITEURL"]}/{metadata["image"]}'
             image_url = url_quote(image_url)  # Jinja filter "urlencode"
 
             image_link = f'<a href={image_url}">{image_url}</a>'
 
             content = content.removesuffix("</p>") + " " + image_link + "</p>"
 
+        if "tags" in metadata.keys():
+            # new_article_metadata["tags"] = myBaseReader.process_metadata("tags", metadata["tags"])
+            new_article_metadata["tags"] = metadata["tags"]
+
+            # metadata["tags"] is already a list of `pelican.urlwrappers.Tag`
+            for tag in metadata["tags"]:
+                tag_url = settings["SITEURL"] + "/" + tag.url
+
+                tag_link = f'<a href="{tag_url}">#{tag.name}</a>'
+
+                content = content.removesuffix("</p>") + " " + tag_link + "</p>"
+
         # warn if too long
         safe_content = Markup(content).striptags()
         post_len = len(safe_content)
         if post_len > settings["MICROBLOG_MAX_LENGTH"] + 6:
             relative_filename = post.removeprefix(settings["PATH"])
             logger.warning(
                 '%s micropost "%s" longer than expected (%s > %s).'
@@ -83,15 +95,15 @@
                     relative_filename,
                     post_len,
                     settings["MICROBLOG_MAX_LENGTH"],
                 )
             )
         new_article_metadata["char_len"] = post_len
 
-        print(post_len)
+        # print(post_len)
 
         new_article = Article(
             content,
             new_article_metadata,
         )
 
         articleGenerator.articles.insert(0, new_article)
```

#### html2text {}

```diff
@@ -23,17 +23,24 @@
 ( "url", settings["MICROBLOG_URL"].format(**metadata) ) if "image" in
 metadata.keys(): new_article_metadata["image"] = myBaseReader.process_metadata
 ( "image", metadata["image"] ) # add image link to end of content image_url =
 f'{settings["SITEURL"]}/{metadata["image"]}' image_url = url_quote(image_url) #
 Jinja filter "urlencode" image_link = f'{image_url}' content =
 content.removesuffix("
 ") + " " + image_link + "
+" if "tags" in metadata.keys(): # new_article_metadata["tags"] =
+myBaseReader.process_metadata("tags", metadata["tags"]) new_article_metadata
+["tags"] = metadata["tags"] # metadata["tags"] is already a list of
+`pelican.urlwrappers.Tag` for tag in metadata["tags"]: tag_url = settings
+["SITEURL"] + "/" + tag.url tag_link = f'#{tag.name}' content =
+content.removesuffix("
+") + " " + tag_link + "
 " # warn if too long safe_content = Markup(content).striptags() post_len = len
 (safe_content) if post_len > settings["MICROBLOG_MAX_LENGTH"] + 6:
 relative_filename = post.removeprefix(settings["PATH"]) logger.warning( '%s
 micropost "%s" longer than expected (%s > %s).' % ( LOG_PREFIX,
 relative_filename, post_len, settings["MICROBLOG_MAX_LENGTH"], ) )
-new_article_metadata["char_len"] = post_len print(post_len) new_article =
+new_article_metadata["char_len"] = post_len # print(post_len) new_article =
 Article( content, new_article_metadata, ) articleGenerator.articles.insert(0,
 new_article) _micropost_count += 1 def pelican_finalized(pelican): global
 _micropost_count print( "%s Processed %s micropost%s." % (LOG_PREFIX,
 _micropost_count, "s" if _micropost_count != 1 else ""), )
```

### Comparing `minchin.pelican.readers.microblog-1.0.0/minchin/pelican/readers/microblog/initialize.py` & `minchin.pelican.readers.microblog-1.1.0/minchin/pelican/readers/microblog/initialize.py`

 * *Files identical despite different names*

### Comparing `minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/PKG-INFO` & `minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minchin.pelican.readers.microblog
-Version: 1.0.0
+Version: 1.1.0
 Summary: Microblogging for Pelican
 Home-page: http://blog.minchin.ca/label/microblog-pelican/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/minchin.pelican.readers.microblog/blob/master/CHANGELOG.rst
@@ -93,14 +93,31 @@
 
    Microblog posts can have "feature" images too! (URL of photo should
    automatically be added.)
 
 The image path is relative to your ``content`` folder. A URL of the photo is
 added to the end of the post as well.
 
+Or with tags (or hashtags):
+
+.. code-block:: md
+
+   <!-- ./content/micro/202307131456.md -->
+
+   date: 2023-07-13 14:56 -0600
+   tags: Python, Pelican, Microblogging
+
+   I'm now Microblogging with Pelican!
+
+
+This will add links at the end of your post to the tags to the tag page for
+your (Pelican) site.
+
+For now, it does not pull tags out of the body of your post.
+
 Background Notes (on Micro Blogging)
 ------------------------------------
 
 Microblogging is here considered to be blog posts, but very short in length.
 
 The most common example is Twitter, with an original limit of 140 characters
 (to be less than the SMS max of 160 characters). Twitter has since doubled
@@ -217,23 +234,40 @@
 ---------
 
 `Changelog <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/blob/master/CHANGELOG.rst>`_
 
 Roadmap
 -------
 
-These are features that I would like to eventually add to the plugin:
+These are features that I would like to eventually add to the plugin (and the
+issues I'm using to track their progress):
+
+- `Issue 1
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/1>`_
+  -- count links as 23 characters (*Ã  la* Twitter)
+- `Issue 2
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/2>`_
+  -- process ReST microblog posts
+- `Issue 3
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/3>`_
+  -- CLI command to create microposts
+- `Issue 4
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/4>`_
+  -- add link previews
+- `Issue 5
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/5>`_
+  -- show (if applicable) that this is a reply to something (or a "re-tweet")
+- `Issue 6
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/6>`_
+  -- show replies to each post (borrow the comment setup?)
+- `Issue 7
+  <https://github.com/MinchinWeb/minchin.pelican.readers.microblog/issues/7>`_
+  -- automatically add hashtags as (Pelican) tags
 
-- count links as 23 characters (*Ã  la* Twitter)
-- process ReST microblog posts
-- CLI command to create microposts
-- add link previews
-- show (if applicable) that this is a reply to something (or a "re-tweet")
-- show replies to each post (borrow the comment setup?)
-- automatically add hashtags as (Pelican) tags
+Pull Requests to implement any of these are welcomed!
 
 - [x] update Seafoam theme
 - [x] make sorting work for microblog posts
 
 
 Known Issues
 ------------
```

### Comparing `minchin.pelican.readers.microblog-1.0.0/minchin.pelican.readers.microblog.egg-info/SOURCES.txt` & `minchin.pelican.readers.microblog-1.1.0/minchin.pelican.readers.microblog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minchin.pelican.readers.microblog-1.0.0/setup.py` & `minchin.pelican.readers.microblog-1.1.0/setup.py`

 * *Files identical despite different names*

