# Comparing `tmp/trackthenews-0.1.9.2.tar.gz` & `tmp/trackthenews-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trackthenews-0.1.9.2.tar", last modified: Mon Jul 23 21:38:42 2018, max compression
+gzip compressed data, was "trackthenews-0.2.tar", last modified: Thu Jul 13 19:54:26 2023, max compression
```

## Comparing `trackthenews-0.1.9.2.tar` & `trackthenews-0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/
--rw-rw-r--   0 parker    (1000) parker    (1000)     3887 2018-07-03 14:08:30.000000 trackthenews-0.1.9.2/README.md
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews/
--rw-rw-r--   0 parker    (1000) parker    (1000)       20 2018-06-18 23:07:44.000000 trackthenews-0.1.9.2/trackthenews/__init__.py
--rwxrwxr-x   0 parker    (1000) parker    (1000)    15371 2018-07-23 21:30:57.000000 trackthenews-0.1.9.2/trackthenews/core.py
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews/fonts/
--rw-rw-r--   0 parker    (1000) parker    (1000)     4301 2018-06-18 23:07:44.000000 trackthenews-0.1.9.2/trackthenews/fonts/LICENSE_OFL.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)   552144 2018-06-18 23:07:44.000000 trackthenews-0.1.9.2/trackthenews/fonts/NotoSerif-Regular.ttf
--rwxrwxr-x   0 parker    (1000) parker    (1000)     1049 2018-07-23 21:34:43.000000 trackthenews-0.1.9.2/setup.py
--rw-rw-r--   0 parker    (1000) parker    (1000)       29 2018-06-19 20:58:47.000000 trackthenews-0.1.9.2/MANIFEST.in
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/
--rw-rw-r--   0 parker    (1000) parker    (1000)       13 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/top_level.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)        1 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/dependency_links.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)     5001 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/PKG-INFO
--rw-rw-r--   0 parker    (1000) parker    (1000)       52 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/entry_points.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)      171 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/requires.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)      370 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/trackthenews.egg-info/SOURCES.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)     5001 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/PKG-INFO
--rw-rw-r--   0 parker    (1000) parker    (1000)       38 2018-07-23 21:38:42.000000 trackthenews-0.1.9.2/setup.cfg
+drwxr-xr-x   0 harris     (501) staff       (20)        0 2023-07-13 19:54:26.793815 trackthenews-0.2/
+-rw-r--r--   0 harris     (501) staff       (20)     1104 2023-02-10 17:16:36.000000 trackthenews-0.2/LICENSE
+-rw-r--r--   0 harris     (501) staff       (20)       29 2023-02-10 17:16:36.000000 trackthenews-0.2/MANIFEST.in
+-rw-r--r--   0 harris     (501) staff       (20)     4384 2023-07-13 19:54:26.793690 trackthenews-0.2/PKG-INFO
+-rw-r--r--   0 harris     (501) staff       (20)     3819 2023-07-13 19:50:12.000000 trackthenews-0.2/README.md
+-rw-r--r--   0 harris     (501) staff       (20)       38 2023-07-13 19:54:26.793852 trackthenews-0.2/setup.cfg
+-rwxr-xr-x   0 harris     (501) staff       (20)     1045 2023-07-13 19:50:12.000000 trackthenews-0.2/setup.py
+drwxr-xr-x   0 harris     (501) staff       (20)        0 2023-07-13 19:54:26.792369 trackthenews-0.2/trackthenews/
+-rw-r--r--   0 harris     (501) staff       (20)       20 2023-02-10 17:16:36.000000 trackthenews-0.2/trackthenews/__init__.py
+-rwxr-xr-x   0 harris     (501) staff       (20)    22073 2023-07-13 18:04:52.000000 trackthenews-0.2/trackthenews/core.py
+drwxr-xr-x   0 harris     (501) staff       (20)        0 2023-07-13 19:54:26.793254 trackthenews-0.2/trackthenews/fonts/
+-rw-r--r--   0 harris     (501) staff       (20)     4301 2023-02-10 17:16:36.000000 trackthenews-0.2/trackthenews/fonts/LICENSE_OFL.txt
+-rw-r--r--   0 harris     (501) staff       (20)   552144 2023-02-10 17:16:36.000000 trackthenews-0.2/trackthenews/fonts/NotoSerif-Regular.ttf
+drwxr-xr-x   0 harris     (501) staff       (20)        0 2023-07-13 19:54:26.793035 trackthenews-0.2/trackthenews.egg-info/
+-rw-r--r--   0 harris     (501) staff       (20)     4384 2023-07-13 19:54:26.000000 trackthenews-0.2/trackthenews.egg-info/PKG-INFO
+-rw-r--r--   0 harris     (501) staff       (20)      378 2023-07-13 19:54:26.000000 trackthenews-0.2/trackthenews.egg-info/SOURCES.txt
+-rw-r--r--   0 harris     (501) staff       (20)        1 2023-07-13 19:54:26.000000 trackthenews-0.2/trackthenews.egg-info/dependency_links.txt
+-rw-r--r--   0 harris     (501) staff       (20)       51 2023-07-13 19:54:26.000000 trackthenews-0.2/trackthenews.egg-info/entry_points.txt
+-rw-r--r--   0 harris     (501) staff       (20)      156 2023-07-13 19:54:26.000000 trackthenews-0.2/trackthenews.egg-info/requires.txt
+-rw-r--r--   0 harris     (501) staff       (20)       13 2023-07-13 19:54:26.000000 trackthenews-0.2/trackthenews.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trackthenews-0.1.9.2/README.md` & `trackthenews-0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Track The News
 
 `trackthenews` is the script that powers [@FOIAfeed](https://twitter.com/foiafeed), a Twitter bot that monitors news outlets for reporting that incorporates public records laws like the Freedom of Information Act (FOIA), and tweets links to and excerpts from matching articles. The underlying software can track any collection of RSS feeds for any keywords.
 
 If you want to run your own instance of `trackthenews`, you can download and install the package, and run its built-in configuration process. It can be installed with `pip`:
 
-Python 3.6 is recommend, but if you run [into troubles](https://github.com/freedomofpress/trackthenews/issues/1), you may want to try it with Python 2.7.
+Python 3.9 is what we currently test against, though it may work with other versions.
 
 
 ```bash
 pip3 install trackthenews
 ```
 
 or by cloning the GitHub repository and running `setup.py`:
```

### Comparing `trackthenews-0.1.9.2/trackthenews/fonts/LICENSE_OFL.txt` & `trackthenews-0.2/trackthenews/fonts/LICENSE_OFL.txt`

 * *Files identical despite different names*

### Comparing `trackthenews-0.1.9.2/trackthenews/fonts/NotoSerif-Regular.ttf` & `trackthenews-0.2/trackthenews/fonts/NotoSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `trackthenews-0.1.9.2/setup.py` & `trackthenews-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = f.read().split()
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='trackthenews',
-    version='0.1.9.2',
+    version='0.2',
     description='Monitor RSS feeds for keywords and act on matching results. A special project of the Freedom of the Press Foundation.',
     long_description=readme,
     long_description_content_type='text/markdown',
     install_requires=reqs,
     author='Parker Higgins',
     author_email='parker@freedom.press',
     url='https://github.com/freedomofpress/trackthenews',
@@ -24,10 +24,10 @@
     },
     include_package_data=True,
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6'],
+        'Programming Language :: Python :: 3.9'],
     packages=find_packages(exclude=('ttnconfig',))
 )
```

### Comparing `trackthenews-0.1.9.2/trackthenews.egg-info/PKG-INFO` & `trackthenews-0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 Metadata-Version: 2.1
 Name: trackthenews
-Version: 0.1.9.2
+Version: 0.2
 Summary: Monitor RSS feeds for keywords and act on matching results. A special project of the Freedom of the Press Foundation.
 Home-page: https://github.com/freedomofpress/trackthenews
 Author: Parker Higgins
 Author-email: parker@freedom.press
 License: MIT
-Description: # Track The News
-        
-        `trackthenews` is the script that powers [@FOIAfeed](https://twitter.com/foiafeed), a Twitter bot that monitors news outlets for reporting that incorporates public records laws like the Freedom of Information Act (FOIA), and tweets links to and excerpts from matching articles. The underlying software can track any collection of RSS feeds for any keywords.
-        
-        If you want to run your own instance of `trackthenews`, you can download and install the package, and run its built-in configuration process. It can be installed with `pip`:
-        
-        Python 3.6 is recommend, but if you run [into troubles](https://github.com/freedomofpress/trackthenews/issues/1), you may want to try it with Python 2.7.
-        
-        
-        ```bash
-        pip3 install trackthenews
-        ```
-        
-        or by cloning the GitHub repository and running `setup.py`:
-        
-        ```bash
-        python3 setup.py install
-        ```
-        
-        Once it is installed, you can create a configuration by running the following command in the appropriate directory:
-        
-        ```bash
-        trackthenews --config
-        ```
-        
-        By default, the script will place all configuration files in a new `ttnconfig` folder in your current working directory, but you can also designate a directory for it to use.
-        
-        ```bash
-        python3 trackthenews --config ~/foo/bar/path
-        ```
-        
-        That configuration process will create the necessary files and walk you through setting up a Twitter bot for matching stories. After it is configured, you'll need to use a text editor to add the `matchwords` and RSS feeds to their respective files.
-        
-        Sample RSS feed and matchword files can be found in the project's GitHub repo. The RSS feed file is a JSON array of objects corresponding to each feed. Each object requires a `url` field, and should also have an `outlet` field.
-        
-        The next two fields are optional: if you know the feed uses redirect URLs, you may set `redirectLinks` to `true` and the script will attempt to follow those redirects to store and tweet canonical URLs; if the feed uses URLs that depend on query- or hash-strings to display correctly—basically, if the content relies on text in the URL bar after a `?` or `#`—you can set `delicateURLs` to `true` and the script will leave the URLs exactly as is.
-        
-        Once you've got everything set up, you can run the program without the `--config` flag to check for matching articles.
-        
-        ```bash
-        trackthenews
-        ```
-        
-        If you designated a custom installation directory, or if you're running it from another directory (or a `cron` job, for example) you will need to designate the directory in which the configuration files are installed.
-        
-        ```bash
-        trackthenews ~/foo/bar/path
-        ```
-        
-        Settings, such as the background color for new posts, the font, and the user-agent, are all located in `config.yaml`, in the designated configuration directory. 
-        
-        ## How it works
-        
-        Most of the script is dedicated to the `Article` class.
-        * `Article`s are created based on inputs. Currently those inputs are RSS feeds, which are stored in `rssfeeds.json`, but in future versions other inputs will include direct URLs, news APIs, Twitter feeds, or scraped pages.
-        * A series of `Article` methods then scrape and isolate the contents of each article (currently that cleanup is done with a [Python port of Readability](https://github.com/buriy/python-readability), but future versions may incorporate some per-site parsing), check whether it's suitable for posting, and then prepare images for tweeting.
-        * Finally, the `Article` tweets itself.
-        
-        All articles are recorded in a sqlite database.
-        
-        ### Advanced feature: blocklist
-        
-        In some cases, you may wish to suppress articles from being posted, even though they would otherwise match. You can do so by writing a new function, `check`, and placing it in a file named `blocklist.py` in the configuration directory. `check` takes an Article (and so has access to its `outlet`, `title`, and `url`) and should return `true` for any article that should be skipped.
-        
-        ## License
-        
-        MIT.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Track The News
+
+`trackthenews` is the script that powers [@FOIAfeed](https://twitter.com/foiafeed), a Twitter bot that monitors news outlets for reporting that incorporates public records laws like the Freedom of Information Act (FOIA), and tweets links to and excerpts from matching articles. The underlying software can track any collection of RSS feeds for any keywords.
+
+If you want to run your own instance of `trackthenews`, you can download and install the package, and run its built-in configuration process. It can be installed with `pip`:
+
+Python 3.9 is what we currently test against, though it may work with other versions.
+
+
+```bash
+pip3 install trackthenews
+```
+
+or by cloning the GitHub repository and running `setup.py`:
+
+```bash
+python3 setup.py install
+```
+
+Once it is installed, you can create a configuration by running the following command in the appropriate directory:
+
+```bash
+trackthenews --config
+```
+
+By default, the script will place all configuration files in a new `ttnconfig` folder in your current working directory, but you can also designate a directory for it to use.
+
+```bash
+python3 trackthenews --config ~/foo/bar/path
+```
+
+That configuration process will create the necessary files and walk you through setting up a Twitter bot for matching stories. After it is configured, you'll need to use a text editor to add the `matchwords` and RSS feeds to their respective files.
+
+Sample RSS feed and matchword files can be found in the project's GitHub repo. The RSS feed file is a JSON array of objects corresponding to each feed. Each object requires a `url` field, and should also have an `outlet` field.
+
+The next two fields are optional: if you know the feed uses redirect URLs, you may set `redirectLinks` to `true` and the script will attempt to follow those redirects to store and tweet canonical URLs; if the feed uses URLs that depend on query- or hash-strings to display correctly—basically, if the content relies on text in the URL bar after a `?` or `#`—you can set `delicateURLs` to `true` and the script will leave the URLs exactly as is.
+
+Once you've got everything set up, you can run the program without the `--config` flag to check for matching articles.
+
+```bash
+trackthenews
+```
+
+If you designated a custom installation directory, or if you're running it from another directory (or a `cron` job, for example) you will need to designate the directory in which the configuration files are installed.
+
+```bash
+trackthenews ~/foo/bar/path
+```
+
+Settings, such as the background color for new posts, the font, and the user-agent, are all located in `config.yaml`, in the designated configuration directory. 
+
+## How it works
+
+Most of the script is dedicated to the `Article` class.
+* `Article`s are created based on inputs. Currently those inputs are RSS feeds, which are stored in `rssfeeds.json`, but in future versions other inputs will include direct URLs, news APIs, Twitter feeds, or scraped pages.
+* A series of `Article` methods then scrape and isolate the contents of each article (currently that cleanup is done with a [Python port of Readability](https://github.com/buriy/python-readability), but future versions may incorporate some per-site parsing), check whether it's suitable for posting, and then prepare images for tweeting.
+* Finally, the `Article` tweets itself.
+
+All articles are recorded in a sqlite database.
+
+### Advanced feature: blocklist
+
+In some cases, you may wish to suppress articles from being posted, even though they would otherwise match. You can do so by writing a new function, `check`, and placing it in a file named `blocklist.py` in the configuration directory. `check` takes an Article (and so has access to its `outlet`, `title`, and `url`) and should return `true` for any article that should be skipped.
+
+## License
+
+MIT.
```

### Comparing `trackthenews-0.1.9.2/PKG-INFO` & `trackthenews-0.2/trackthenews.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 Metadata-Version: 2.1
 Name: trackthenews
-Version: 0.1.9.2
+Version: 0.2
 Summary: Monitor RSS feeds for keywords and act on matching results. A special project of the Freedom of the Press Foundation.
 Home-page: https://github.com/freedomofpress/trackthenews
 Author: Parker Higgins
 Author-email: parker@freedom.press
 License: MIT
-Description: # Track The News
-        
-        `trackthenews` is the script that powers [@FOIAfeed](https://twitter.com/foiafeed), a Twitter bot that monitors news outlets for reporting that incorporates public records laws like the Freedom of Information Act (FOIA), and tweets links to and excerpts from matching articles. The underlying software can track any collection of RSS feeds for any keywords.
-        
-        If you want to run your own instance of `trackthenews`, you can download and install the package, and run its built-in configuration process. It can be installed with `pip`:
-        
-        Python 3.6 is recommend, but if you run [into troubles](https://github.com/freedomofpress/trackthenews/issues/1), you may want to try it with Python 2.7.
-        
-        
-        ```bash
-        pip3 install trackthenews
-        ```
-        
-        or by cloning the GitHub repository and running `setup.py`:
-        
-        ```bash
-        python3 setup.py install
-        ```
-        
-        Once it is installed, you can create a configuration by running the following command in the appropriate directory:
-        
-        ```bash
-        trackthenews --config
-        ```
-        
-        By default, the script will place all configuration files in a new `ttnconfig` folder in your current working directory, but you can also designate a directory for it to use.
-        
-        ```bash
-        python3 trackthenews --config ~/foo/bar/path
-        ```
-        
-        That configuration process will create the necessary files and walk you through setting up a Twitter bot for matching stories. After it is configured, you'll need to use a text editor to add the `matchwords` and RSS feeds to their respective files.
-        
-        Sample RSS feed and matchword files can be found in the project's GitHub repo. The RSS feed file is a JSON array of objects corresponding to each feed. Each object requires a `url` field, and should also have an `outlet` field.
-        
-        The next two fields are optional: if you know the feed uses redirect URLs, you may set `redirectLinks` to `true` and the script will attempt to follow those redirects to store and tweet canonical URLs; if the feed uses URLs that depend on query- or hash-strings to display correctly—basically, if the content relies on text in the URL bar after a `?` or `#`—you can set `delicateURLs` to `true` and the script will leave the URLs exactly as is.
-        
-        Once you've got everything set up, you can run the program without the `--config` flag to check for matching articles.
-        
-        ```bash
-        trackthenews
-        ```
-        
-        If you designated a custom installation directory, or if you're running it from another directory (or a `cron` job, for example) you will need to designate the directory in which the configuration files are installed.
-        
-        ```bash
-        trackthenews ~/foo/bar/path
-        ```
-        
-        Settings, such as the background color for new posts, the font, and the user-agent, are all located in `config.yaml`, in the designated configuration directory. 
-        
-        ## How it works
-        
-        Most of the script is dedicated to the `Article` class.
-        * `Article`s are created based on inputs. Currently those inputs are RSS feeds, which are stored in `rssfeeds.json`, but in future versions other inputs will include direct URLs, news APIs, Twitter feeds, or scraped pages.
-        * A series of `Article` methods then scrape and isolate the contents of each article (currently that cleanup is done with a [Python port of Readability](https://github.com/buriy/python-readability), but future versions may incorporate some per-site parsing), check whether it's suitable for posting, and then prepare images for tweeting.
-        * Finally, the `Article` tweets itself.
-        
-        All articles are recorded in a sqlite database.
-        
-        ### Advanced feature: blocklist
-        
-        In some cases, you may wish to suppress articles from being posted, even though they would otherwise match. You can do so by writing a new function, `check`, and placing it in a file named `blocklist.py` in the configuration directory. `check` takes an Article (and so has access to its `outlet`, `title`, and `url`) and should return `true` for any article that should be skipped.
-        
-        ## License
-        
-        MIT.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Track The News
+
+`trackthenews` is the script that powers [@FOIAfeed](https://twitter.com/foiafeed), a Twitter bot that monitors news outlets for reporting that incorporates public records laws like the Freedom of Information Act (FOIA), and tweets links to and excerpts from matching articles. The underlying software can track any collection of RSS feeds for any keywords.
+
+If you want to run your own instance of `trackthenews`, you can download and install the package, and run its built-in configuration process. It can be installed with `pip`:
+
+Python 3.9 is what we currently test against, though it may work with other versions.
+
+
+```bash
+pip3 install trackthenews
+```
+
+or by cloning the GitHub repository and running `setup.py`:
+
+```bash
+python3 setup.py install
+```
+
+Once it is installed, you can create a configuration by running the following command in the appropriate directory:
+
+```bash
+trackthenews --config
+```
+
+By default, the script will place all configuration files in a new `ttnconfig` folder in your current working directory, but you can also designate a directory for it to use.
+
+```bash
+python3 trackthenews --config ~/foo/bar/path
+```
+
+That configuration process will create the necessary files and walk you through setting up a Twitter bot for matching stories. After it is configured, you'll need to use a text editor to add the `matchwords` and RSS feeds to their respective files.
+
+Sample RSS feed and matchword files can be found in the project's GitHub repo. The RSS feed file is a JSON array of objects corresponding to each feed. Each object requires a `url` field, and should also have an `outlet` field.
+
+The next two fields are optional: if you know the feed uses redirect URLs, you may set `redirectLinks` to `true` and the script will attempt to follow those redirects to store and tweet canonical URLs; if the feed uses URLs that depend on query- or hash-strings to display correctly—basically, if the content relies on text in the URL bar after a `?` or `#`—you can set `delicateURLs` to `true` and the script will leave the URLs exactly as is.
+
+Once you've got everything set up, you can run the program without the `--config` flag to check for matching articles.
+
+```bash
+trackthenews
+```
+
+If you designated a custom installation directory, or if you're running it from another directory (or a `cron` job, for example) you will need to designate the directory in which the configuration files are installed.
+
+```bash
+trackthenews ~/foo/bar/path
+```
+
+Settings, such as the background color for new posts, the font, and the user-agent, are all located in `config.yaml`, in the designated configuration directory. 
+
+## How it works
+
+Most of the script is dedicated to the `Article` class.
+* `Article`s are created based on inputs. Currently those inputs are RSS feeds, which are stored in `rssfeeds.json`, but in future versions other inputs will include direct URLs, news APIs, Twitter feeds, or scraped pages.
+* A series of `Article` methods then scrape and isolate the contents of each article (currently that cleanup is done with a [Python port of Readability](https://github.com/buriy/python-readability), but future versions may incorporate some per-site parsing), check whether it's suitable for posting, and then prepare images for tweeting.
+* Finally, the `Article` tweets itself.
+
+All articles are recorded in a sqlite database.
+
+### Advanced feature: blocklist
+
+In some cases, you may wish to suppress articles from being posted, even though they would otherwise match. You can do so by writing a new function, `check`, and placing it in a file named `blocklist.py` in the configuration directory. `check` takes an Article (and so has access to its `outlet`, `title`, and `url`) and should return `true` for any article that should be skipped.
+
+## License
+
+MIT.
```

