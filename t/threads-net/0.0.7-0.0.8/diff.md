# Comparing `tmp/threads-net-0.0.7.tar.gz` & `tmp/threads-net-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-net-0.0.7.tar", last modified: Sat Jul  8 07:57:48 2023, max compression
+gzip compressed data, was "threads-net-0.0.8.tar", last modified: Sun Jul  9 09:40:02 2023, max compression
```

## Comparing `threads-net-0.0.7.tar` & `threads-net-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:57:48.439509 threads-net-0.0.7/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.7/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.7/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44708 2023-07-08 07:57:48.439399 threads-net-0.0.7/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43857 2023-07-08 07:56:37.000000 threads-net-0.0.7/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:57:48.438254 threads-net-0.0.7/examples/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.7/examples/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      242 2023-07-08 07:12:45.000000 threads-net-0.0.7/examples/get_post.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      478 2023-07-08 07:56:37.000000 threads-net-0.0.7/examples/get_user.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      261 2023-07-08 07:09:17.000000 threads-net-0.0.7/examples/get_user_replies.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      263 2023-07-08 07:09:25.000000 threads-net-0.0.7/examples/get_user_threads.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-07 19:07:00.000000 threads-net-0.0.7/examples/login.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:57:48.438358 threads-net-0.0.7/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:45:44.000000 threads-net-0.0.7/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-08 07:57:48.439539 threads-net-0.0.7/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-08 07:57:05.000000 threads-net-0.0.7/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:57:48.438599 threads-net-0.0.7/threads/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.7/threads/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5610 2023-07-08 07:56:45.000000 threads-net-0.0.7/threads/main.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:57:48.439226 threads-net-0.0.7/threads_net.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44708 2023-07-08 07:57:48.000000 threads-net-0.0.7/threads_net.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      412 2023-07-08 07:57:48.000000 threads-net-0.0.7/threads_net.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-08 07:57:48.000000 threads-net-0.0.7/threads_net.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-08 07:57:48.000000 threads-net-0.0.7/threads_net.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-08 07:57:48.000000 threads-net-0.0.7/threads_net.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-09 09:40:02.192796 threads-net-0.0.8/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.8/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.8/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    35255 2023-07-09 09:40:02.192678 threads-net-0.0.8/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    34404 2023-07-09 09:39:15.000000 threads-net-0.0.8/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-09 09:40:02.191553 threads-net-0.0.8/examples/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.8/examples/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      242 2023-07-08 07:12:45.000000 threads-net-0.0.8/examples/get_post.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      454 2023-07-09 09:19:54.000000 threads-net-0.0.8/examples/get_user.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      261 2023-07-08 07:09:17.000000 threads-net-0.0.8/examples/get_user_replies.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      263 2023-07-08 07:09:25.000000 threads-net-0.0.8/examples/get_user_threads.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-09 09:22:39.000000 threads-net-0.0.8/examples/login.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1344 2023-07-09 09:39:13.000000 threads-net-0.0.8/examples/post_thread.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-09 09:40:02.191671 threads-net-0.0.8/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:45:44.000000 threads-net-0.0.8/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-09 09:40:02.192836 threads-net-0.0.8/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-09 09:36:38.000000 threads-net-0.0.8/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-09 09:40:02.191892 threads-net-0.0.8/threads/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.8/threads/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     6148 2023-07-09 09:36:55.000000 threads-net-0.0.8/threads/main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-09 09:40:02.192509 threads-net-0.0.8/threads_net.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    35255 2023-07-09 09:40:02.000000 threads-net-0.0.8/threads_net.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      436 2023-07-09 09:40:02.000000 threads-net-0.0.8/threads_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-09 09:40:02.000000 threads-net-0.0.8/threads_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-09 09:40:02.000000 threads-net-0.0.8/threads_net.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-09 09:40:02.000000 threads-net-0.0.8/threads_net.egg-info/top_level.txt
```

### Comparing `threads-net-0.0.7/LICENSE` & `threads-net-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.7/PKG-INFO` & `threads-net-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.7
+Version: 0.0.8
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -18,46 +18,49 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
 
-Threads (threads.net) Python API wrapper
+Threads (threads.net) Python API wrapper.
 
-[![Downdloads](https://pepy.tech/badge/threads-net)](https://pepy.tech/project/threads-net)
+[![Downloads](https://pepy.tech/badge/threads-net)](https://pepy.tech/project/threads-net)
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
 * [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
   * [How to install](#how-to-install)
   * [Initialization](#initialization)
   * [Examples](#examples)
 * [API](#api)
   * [Login](#login)
-  * [Get User By Username](#get-user-by-username)
+  * [Get User Identifier](#get-user-identifier)
   * [Get User By Identifier](#get-user-by-identifier)
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
 ## Disclaimer
 
-* This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
-  Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
-  needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
-  So use the project at your own risk until the normal `Threads` public `API` is available or this product become more
-  stable for such things.
-* For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
-  is used because `Threads` are backed by `Instagram` and you do a login via it as well.
-* As the library use `Threads API ` private endpoints, they have no defined model for support and backward compatibility. 
-* So, some methods might end up not working until the library maintainers find out hot to fix it.
+* As `Threads` are backed by `Instagram`. It means that `Threads` functionality partially placed in `Instagram API`:
+  you do a login to `Threads` application via `Instagram`'s username and password, posting new threads and fetching user
+  identifier (for further library usage) too. So expect seeing things related to `Instagram` in this library.
+* This project is unofficial and utilize both public and private endpoints of both `Threads` and `Instagram` `APIs`. 
+  Utilizing private endpoints means pretending being a mobile phone or web user (via proper `HTTP` headers and other 
+  things). Thus you might face `rate limits` (because pretending is never ideal) or even your account in `Threads` and 
+  `Instagram` might be suspended if mess up with logining or sending too much requests. So use the project at your own 
+  risk until the normal public `ThreadsAPI` is released or this product become more stable for such things.Also,
+  utilizing such endpoints mean that they might not be stable (because they are under active development and there is
+  no any promise in backward compatibility).
+* For all the `Instagram`-related thing other well-know and already stable library called [instagrapi](https://github.com/adw0rd/instagrapi)
+  is used in `threads-net`.
 
 ## Getting started
 
 ### How to install
 
 Install the library with the following command using `pip3`:
 
@@ -90,15 +93,15 @@
 ```
 
 ## API
 
 ### Login
 
 In order for `Instagram` to trust you more, you must always login from one device and one IP (or from a subnet), for 
-this there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+this there is the dump session functionality. So, once you logged in once, store it into a file:
 
 ```python3
 >>> threads = Threads()
 >>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
 >>> threads.dump_settings('session.json')
 ```
 
@@ -107,230 +110,153 @@
 ```python3
 >>> threads = Threads()
 >>> threads.load_settings('session.json')
 >>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
 ```
 
 The login method might ask for additional username/password entering, confirmation code and other challenges. But if
-you reuse the session, those should be minimum times. For more information, check this out — 
+you reuse the session, those should happen minimum times. For more information, check this out — 
 https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
 
-Also, the login is only needed for getting a user by identifier and username, for other endpoints it is not required, so
-you can easily skip it.
+### Get User Identifier
 
-### Get User by Username
-
-To get a user by a username, use the following commands:
+To get a user's identifier by a username, use the following commands:
 
 ```python3
->>> user = threads.get_user_by_username(username='zuck')
->>> user
-{
-    "pk": 314216,
-    "username": "zuck",
-    "full_name": "Mark Zuckerberg",
-    "is_private": False,
-    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
-    "is_verified": False,
-    "media_count": 102,
-    "follower_count": 576,
-    "following_count": 538,
-    "biography": '',
-    "is_business": False
-}
+>>> user_id = threads.get_user_id(username='zuck')
+>>> user_id
+314216
 ```
 
 ### Get User by Identifier
 
 To get a user by an identifier, use the following commands:
 
 ```python3
 >>> user = threads.get_user_by_id(id=314216)
 >>> user
 {
-    "pk": 314216,
-    "username": "zuck",
-    "full_name": "Mark Zuckerberg",
-    "is_private": False,
-    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
-    "is_verified": False,
-    "media_count": 102,
-    "follower_count": 576,
-    "following_count": 538,
-    "biography": '',
-    "is_business": False
+    "data": {
+        "userData": {
+            "user": {
+                "is_private": false,
+                "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAUZzobOIH6imLnb2Z3iXoWY5H1Fv_kNnyG8T4UGgJegQ&oe=64AED800&_nc_sid=10d13b",
+                "username": "zuck",
+                "hd_profile_pic_versions": [
+                    {
+                        "height": 320,
+                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD5z6UgnQH54dihPnMrXgH2L-mLCMGlFsIF9Ug7U4RWdA&oe=64AED800&_nc_sid=10d13b",
+                        "width": 320
+                    },
+                    {
+                        "height": 640,
+                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD4BaVu4cDcX53xPocD-3o_ZbKIESxUZhlU08FBpycCsA&oe=64AED800&_nc_sid=10d13b",
+                        "width": 640
+                    }
+                ],
+                "is_verified": true,
+                "biography": "",
+                "biography_with_entities": null,
+                "follower_count": 2663947,
+                "profile_context_facepile_users": null,
+                "bio_links": [
+                    {
+                        "url": ""
+                    }
+                ],
+                "pk": "314216",
+                "full_name": "Mark Zuckerberg",
+                "id": null
+            }
+        }
+    },
+    "extensions": {
+        "is_final": true
+    }
 }
 ```
 
 ### Get User Threads
 
 To get a user's threads, use the following commands:
 
 ```python3
 >>> user_threads = threads.get_user_threads(id=314216)
 >>> user_threads
 {
-    "data": {
-        "mediaData": {
-            "threads": [
-                {
-                    "thread_items": [
+    "instagram": {
+        "pk": "314216",
+        "username": "zuck",
+        "full_name": "Mark Zuckerberg",
+        "is_private": false,
+        "profile_pic_url": "https://instagram.fiev6-1.fna.fbcdn.net/v/t51.2885-19/352224138_1028122805231303_1175896139426286760_n.jpg?stp=dst-jpg_s150x150&_nc_ht=instagram.fiev6-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=hbekpcjRfioAX8iYGJv&edm=AKEQFekBAAAA&ccb=7-5&oh=00_AfDf2r6qwujUc84tkzUlYJMfJt66xoWScQ-nsB5bmtYDnw&oe=64B0066A&_nc_sid=29ddf3",
+        "profile_pic_url_hd": "https://instagram.fiev6-1.fna.fbcdn.net/v/t51.2885-19/352224138_1028122805231303_1175896139426286760_n.jpg?stp=dst-jpg_s320x320&_nc_ht=instagram.fiev6-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=hbekpcjRfioAX8iYGJv&edm=AKEQFekBAAAA&ccb=7-5&oh=00_AfCoPcYmzHdc2evDvduZjZK-IxDS07wGf0x9czecY_TgVQ&oe=64B0066A&_nc_sid=29ddf3",
+        "is_verified": true,
+        "media_count": 283,
+        "follower_count": 11924434,
+        "following_count": 523,
+        "biography": "",
+        "external_url": null,
+        "account_type": null,
+        "is_business": false,
+        "public_email": null,
+        "contact_phone_number": null,
+        "public_phone_country_code": null,
+        "public_phone_number": null,
+        "business_contact_method": "UNKNOWN",
+        "business_category_name": null,
+        "category_name": "Entrepreneur",
+        "category": null,
+        "address_street": null,
+        "city_id": null,
+        "city_name": null,
+        "latitude": null,
+        "longitude": null,
+        "zip": null,
+        "instagram_location_id": null,
+        "interop_messaging_user_fbid": null
+    },
+    "threads": {
+        "data": {
+            "userData": {
+                "user": {
+                    "is_private": false,
+                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfCdAMkmk0XL_r0GQi2MRD1Aq1kPZKBLfXLby47e_hsZrg&oe=64AED800&_nc_sid=10d13b",
+                    "username": "zuck",
+                    "hd_profile_pic_versions": [
+                        {
+                            "height": 320,
+                            "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDJeE127_ZFA-eD3qRMM0Fh2NM-jRR4tUFsTywCrMctNA&oe=64AED800&_nc_sid=10d13b",
+                            "width": 320
+                        },
                         {
-                            "post": {
-                                "user": {
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-q_Nrf&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDWsSPBghiIhwJnh4_3kO5maVMhDErg9ky_-dhqUHVtRw&oe=64ACDDC0&_nc_sid=10d13b",
-                                    "username": "zuck",
-                                    "id": null,
-                                    "is_verified": true,
-                                    "pk": "314216"
-                                },
-                                "image_versions2": {
-                                    "candidates": [
-                                        {
-                                            "height": 3000,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfBVkBmYMO2TozQJYlE6xblN10YDdmKXhzzs0hSHHCfUgQ&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 4000,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 810,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s1080x1080&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCl-OTiAWiST-z8pGT0IHQAcdQiuWxdoI44UQccZrvkdw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 1080,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 540,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s720x720&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCQ6PZm83pOL4_QMalEvrzu1TTLWqvHWMVK3WercfrQdA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 720,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 480,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s640x640_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfB6A9bQNJLWiNgczI7Kp7q7wII7TC1ifn4oVd5cN8nTBg&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 640,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 360,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s480x480&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfAtSvruwFWIjemafFJXaFfb_iag6LMjJL7EFaBmZmyP0Q&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 480,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 240,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCCyzKffNLdsvdSRuyHMdAN-F7sEALSVrc0kM3R2nsrQA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 320,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 180,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s240x240&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCq8hu-NdtgzUrS_S4MnBrJX4ogGvCiAIhG_gr6xwp5Ag&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 240,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 1080,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s1080x1080&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfDWf1VGojZDDWQDCDO1x0l3SU34cgdEOceFGPxK_9EZfA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 1080,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 750,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s750x750_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfA-Kqa9UoMluJGqD_wBNG3qtcbWT63RCkq07fDo88ZVaw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 750,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 640,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s640x640_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCh7r-VI_5fLBmsPNp_cb-rZSBsDJTYdrn0PnMKBgATlw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 640,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 480,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s480x480&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfBXkMC4qSLcsgFURS0yXTu02CyydoJpInHfOr5L-FP5ww&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 480,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 320,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCwJtku5xDOM0dxwCvfAzmV64T-_kaA4CZLOIl3OTNiJQ&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 320,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 240,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s240x240&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCxaBgqYV7qj0svYLI1KavhteMygChYAfZma84Fe0tZmw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 240,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 150,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfDwSo36FyoIW052Qvgp7eDCfi-ij8x3NsySfbpfQAlM_Q&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 150,
-                                            "__typename": "XDTImageCandidate"
-                                        }
-                                    ]
-                                },
-                                "original_width": 4000,
-                                "original_height": 3000,
-                                "video_versions": [],
-                                "carousel_media": null,
-                                "carousel_media_count": null,
-                                "pk": "3141002295235099165",
-                                "has_audio": null,
-                                "text_post_app_info": {
-                                    "link_preview_attachment": null,
-                                    "share_info": {
-                                        "quoted_post": null,
-                                        "reposted_post": null
-                                    },
-                                    "reply_to_author": null,
-                                    "is_post_unavailable": false
-                                },
-                                "caption": {
-                                    "text": "Lots of work on basic capabilities this morning."
-                                },
-                                "taken_at": 1688656673,
-                                "like_count": 184611,
-                                "code": "CuXFPIeLLod",
-                                "media_overlay_info": null,
-                                "id": "3141002295235099165_314216"
-                            },
-                            "line_type": "line",
-                            "view_replies_cta_string": "17,882 replies",
-                            "reply_facepile_users": [
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358166568_272137218742674_3025287304976949959_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=106&_nc_ohc=Wl0wRGxM7g4AX-cl1FE&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAaJRzZHv09tlkXbrdFTQC-ZhwW7v2BPih4fIBN3HxdYg&oe=64AC6E7C&_nc_sid=10d13b"
-                                },
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358337983_581973004113850_7681929282916239696_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=110&_nc_ohc=9xd6QhLrfr0AX_jXvvd&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD01Al_ukeQOVXysDuudHw82ZUfn4q_PI1KuWE1Swf1Kw&oe=64AC446D&_nc_sid=10d13b"
-                                },
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358357576_689254799697876_1184079927626851628_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=100&_nc_ohc=95IT8pfSV8MAX8qeB2M&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfBtniKWdsj56GWa3T_UQZG6xEhLv_2ck-q_V9J34Pb4ag&oe=64ADA8C7&_nc_sid=10d13b"
-                                }
-                            ],
-                            "should_show_replies_cta": true,
-                            "__typename": "XDTThreadItem"
+                            "height": 640,
+                            "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAY-75SdPDasc0ophRu3lgeeHmnb3qPZIE-mCPh8PRRBw&oe=64AED800&_nc_sid=10d13b",
+                            "width": 640
                         }
                     ],
-                    "id": "3141002295235099165"
-                },
-                ...
-            ]
+                    "is_verified": true,
+                    "biography": "",
+                    "biography_with_entities": null,
+                    "follower_count": 2663588,
+                    "profile_context_facepile_users": null,
+                    "bio_links": [
+                        {
+                            "url": ""
+                        }
+                    ],
+                    "pk": "314216",
+                    "full_name": "Mark Zuckerberg",
+                    "id": null
+                }
+            }
+        },
+        "extensions": {
+            "is_final": true
         }
-    },
-    "extensions": {
-        "is_final": true
     }
 }
 ```
 
 ### Get User Replies
 
 To get a user's replies, use the following commands:
```

### Comparing `threads-net-0.0.7/README.md` & `threads-net-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
 
-Threads (threads.net) Python API wrapper
+Threads (threads.net) Python API wrapper.
 
-[![Downdloads](https://pepy.tech/badge/threads-net)](https://pepy.tech/project/threads-net)
+[![Downloads](https://pepy.tech/badge/threads-net)](https://pepy.tech/project/threads-net)
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
 * [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
   * [How to install](#how-to-install)
   * [Initialization](#initialization)
   * [Examples](#examples)
 * [API](#api)
   * [Login](#login)
-  * [Get User By Username](#get-user-by-username)
+  * [Get User Identifier](#get-user-identifier)
   * [Get User By Identifier](#get-user-by-identifier)
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
 ## Disclaimer
 
-* This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
-  Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
-  needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
-  So use the project at your own risk until the normal `Threads` public `API` is available or this product become more
-  stable for such things.
-* For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
-  is used because `Threads` are backed by `Instagram` and you do a login via it as well.
-* As the library use `Threads API ` private endpoints, they have no defined model for support and backward compatibility. 
-* So, some methods might end up not working until the library maintainers find out hot to fix it.
+* As `Threads` are backed by `Instagram`. It means that `Threads` functionality partially placed in `Instagram API`:
+  you do a login to `Threads` application via `Instagram`'s username and password, posting new threads and fetching user
+  identifier (for further library usage) too. So expect seeing things related to `Instagram` in this library.
+* This project is unofficial and utilize both public and private endpoints of both `Threads` and `Instagram` `APIs`. 
+  Utilizing private endpoints means pretending being a mobile phone or web user (via proper `HTTP` headers and other 
+  things). Thus you might face `rate limits` (because pretending is never ideal) or even your account in `Threads` and 
+  `Instagram` might be suspended if mess up with logining or sending too much requests. So use the project at your own 
+  risk until the normal public `ThreadsAPI` is released or this product become more stable for such things.Also,
+  utilizing such endpoints mean that they might not be stable (because they are under active development and there is
+  no any promise in backward compatibility).
+* For all the `Instagram`-related thing other well-know and already stable library called [instagrapi](https://github.com/adw0rd/instagrapi)
+  is used in `threads-net`.
 
 ## Getting started
 
 ### How to install
 
 Install the library with the following command using `pip3`:
 
@@ -68,15 +71,15 @@
 ```
 
 ## API
 
 ### Login
 
 In order for `Instagram` to trust you more, you must always login from one device and one IP (or from a subnet), for 
-this there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+this there is the dump session functionality. So, once you logged in once, store it into a file:
 
 ```python3
 >>> threads = Threads()
 >>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
 >>> threads.dump_settings('session.json')
 ```
 
@@ -85,230 +88,153 @@
 ```python3
 >>> threads = Threads()
 >>> threads.load_settings('session.json')
 >>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
 ```
 
 The login method might ask for additional username/password entering, confirmation code and other challenges. But if
-you reuse the session, those should be minimum times. For more information, check this out — 
+you reuse the session, those should happen minimum times. For more information, check this out — 
 https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
 
-Also, the login is only needed for getting a user by identifier and username, for other endpoints it is not required, so
-you can easily skip it.
+### Get User Identifier
 
-### Get User by Username
-
-To get a user by a username, use the following commands:
+To get a user's identifier by a username, use the following commands:
 
 ```python3
->>> user = threads.get_user_by_username(username='zuck')
->>> user
-{
-    "pk": 314216,
-    "username": "zuck",
-    "full_name": "Mark Zuckerberg",
-    "is_private": False,
-    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
-    "is_verified": False,
-    "media_count": 102,
-    "follower_count": 576,
-    "following_count": 538,
-    "biography": '',
-    "is_business": False
-}
+>>> user_id = threads.get_user_id(username='zuck')
+>>> user_id
+314216
 ```
 
 ### Get User by Identifier
 
 To get a user by an identifier, use the following commands:
 
 ```python3
 >>> user = threads.get_user_by_id(id=314216)
 >>> user
 {
-    "pk": 314216,
-    "username": "zuck",
-    "full_name": "Mark Zuckerberg",
-    "is_private": False,
-    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
-    "is_verified": False,
-    "media_count": 102,
-    "follower_count": 576,
-    "following_count": 538,
-    "biography": '',
-    "is_business": False
+    "data": {
+        "userData": {
+            "user": {
+                "is_private": false,
+                "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAUZzobOIH6imLnb2Z3iXoWY5H1Fv_kNnyG8T4UGgJegQ&oe=64AED800&_nc_sid=10d13b",
+                "username": "zuck",
+                "hd_profile_pic_versions": [
+                    {
+                        "height": 320,
+                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD5z6UgnQH54dihPnMrXgH2L-mLCMGlFsIF9Ug7U4RWdA&oe=64AED800&_nc_sid=10d13b",
+                        "width": 320
+                    },
+                    {
+                        "height": 640,
+                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD4BaVu4cDcX53xPocD-3o_ZbKIESxUZhlU08FBpycCsA&oe=64AED800&_nc_sid=10d13b",
+                        "width": 640
+                    }
+                ],
+                "is_verified": true,
+                "biography": "",
+                "biography_with_entities": null,
+                "follower_count": 2663947,
+                "profile_context_facepile_users": null,
+                "bio_links": [
+                    {
+                        "url": ""
+                    }
+                ],
+                "pk": "314216",
+                "full_name": "Mark Zuckerberg",
+                "id": null
+            }
+        }
+    },
+    "extensions": {
+        "is_final": true
+    }
 }
 ```
 
 ### Get User Threads
 
 To get a user's threads, use the following commands:
 
 ```python3
 >>> user_threads = threads.get_user_threads(id=314216)
 >>> user_threads
 {
-    "data": {
-        "mediaData": {
-            "threads": [
-                {
-                    "thread_items": [
+    "instagram": {
+        "pk": "314216",
+        "username": "zuck",
+        "full_name": "Mark Zuckerberg",
+        "is_private": false,
+        "profile_pic_url": "https://instagram.fiev6-1.fna.fbcdn.net/v/t51.2885-19/352224138_1028122805231303_1175896139426286760_n.jpg?stp=dst-jpg_s150x150&_nc_ht=instagram.fiev6-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=hbekpcjRfioAX8iYGJv&edm=AKEQFekBAAAA&ccb=7-5&oh=00_AfDf2r6qwujUc84tkzUlYJMfJt66xoWScQ-nsB5bmtYDnw&oe=64B0066A&_nc_sid=29ddf3",
+        "profile_pic_url_hd": "https://instagram.fiev6-1.fna.fbcdn.net/v/t51.2885-19/352224138_1028122805231303_1175896139426286760_n.jpg?stp=dst-jpg_s320x320&_nc_ht=instagram.fiev6-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=hbekpcjRfioAX8iYGJv&edm=AKEQFekBAAAA&ccb=7-5&oh=00_AfCoPcYmzHdc2evDvduZjZK-IxDS07wGf0x9czecY_TgVQ&oe=64B0066A&_nc_sid=29ddf3",
+        "is_verified": true,
+        "media_count": 283,
+        "follower_count": 11924434,
+        "following_count": 523,
+        "biography": "",
+        "external_url": null,
+        "account_type": null,
+        "is_business": false,
+        "public_email": null,
+        "contact_phone_number": null,
+        "public_phone_country_code": null,
+        "public_phone_number": null,
+        "business_contact_method": "UNKNOWN",
+        "business_category_name": null,
+        "category_name": "Entrepreneur",
+        "category": null,
+        "address_street": null,
+        "city_id": null,
+        "city_name": null,
+        "latitude": null,
+        "longitude": null,
+        "zip": null,
+        "instagram_location_id": null,
+        "interop_messaging_user_fbid": null
+    },
+    "threads": {
+        "data": {
+            "userData": {
+                "user": {
+                    "is_private": false,
+                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfCdAMkmk0XL_r0GQi2MRD1Aq1kPZKBLfXLby47e_hsZrg&oe=64AED800&_nc_sid=10d13b",
+                    "username": "zuck",
+                    "hd_profile_pic_versions": [
+                        {
+                            "height": 320,
+                            "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDJeE127_ZFA-eD3qRMM0Fh2NM-jRR4tUFsTywCrMctNA&oe=64AED800&_nc_sid=10d13b",
+                            "width": 320
+                        },
                         {
-                            "post": {
-                                "user": {
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-q_Nrf&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDWsSPBghiIhwJnh4_3kO5maVMhDErg9ky_-dhqUHVtRw&oe=64ACDDC0&_nc_sid=10d13b",
-                                    "username": "zuck",
-                                    "id": null,
-                                    "is_verified": true,
-                                    "pk": "314216"
-                                },
-                                "image_versions2": {
-                                    "candidates": [
-                                        {
-                                            "height": 3000,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfBVkBmYMO2TozQJYlE6xblN10YDdmKXhzzs0hSHHCfUgQ&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 4000,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 810,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s1080x1080&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCl-OTiAWiST-z8pGT0IHQAcdQiuWxdoI44UQccZrvkdw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 1080,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 540,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s720x720&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCQ6PZm83pOL4_QMalEvrzu1TTLWqvHWMVK3WercfrQdA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 720,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 480,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s640x640_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfB6A9bQNJLWiNgczI7Kp7q7wII7TC1ifn4oVd5cN8nTBg&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 640,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 360,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s480x480&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfAtSvruwFWIjemafFJXaFfb_iag6LMjJL7EFaBmZmyP0Q&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 480,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 240,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCCyzKffNLdsvdSRuyHMdAN-F7sEALSVrc0kM3R2nsrQA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 320,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 180,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s240x240&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCq8hu-NdtgzUrS_S4MnBrJX4ogGvCiAIhG_gr6xwp5Ag&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 240,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 1080,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s1080x1080&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfDWf1VGojZDDWQDCDO1x0l3SU34cgdEOceFGPxK_9EZfA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 1080,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 750,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s750x750_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfA-Kqa9UoMluJGqD_wBNG3qtcbWT63RCkq07fDo88ZVaw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 750,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 640,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s640x640_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCh7r-VI_5fLBmsPNp_cb-rZSBsDJTYdrn0PnMKBgATlw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 640,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 480,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s480x480&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfBXkMC4qSLcsgFURS0yXTu02CyydoJpInHfOr5L-FP5ww&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 480,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 320,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCwJtku5xDOM0dxwCvfAzmV64T-_kaA4CZLOIl3OTNiJQ&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 320,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 240,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s240x240&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCxaBgqYV7qj0svYLI1KavhteMygChYAfZma84Fe0tZmw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 240,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 150,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfDwSo36FyoIW052Qvgp7eDCfi-ij8x3NsySfbpfQAlM_Q&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 150,
-                                            "__typename": "XDTImageCandidate"
-                                        }
-                                    ]
-                                },
-                                "original_width": 4000,
-                                "original_height": 3000,
-                                "video_versions": [],
-                                "carousel_media": null,
-                                "carousel_media_count": null,
-                                "pk": "3141002295235099165",
-                                "has_audio": null,
-                                "text_post_app_info": {
-                                    "link_preview_attachment": null,
-                                    "share_info": {
-                                        "quoted_post": null,
-                                        "reposted_post": null
-                                    },
-                                    "reply_to_author": null,
-                                    "is_post_unavailable": false
-                                },
-                                "caption": {
-                                    "text": "Lots of work on basic capabilities this morning."
-                                },
-                                "taken_at": 1688656673,
-                                "like_count": 184611,
-                                "code": "CuXFPIeLLod",
-                                "media_overlay_info": null,
-                                "id": "3141002295235099165_314216"
-                            },
-                            "line_type": "line",
-                            "view_replies_cta_string": "17,882 replies",
-                            "reply_facepile_users": [
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358166568_272137218742674_3025287304976949959_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=106&_nc_ohc=Wl0wRGxM7g4AX-cl1FE&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAaJRzZHv09tlkXbrdFTQC-ZhwW7v2BPih4fIBN3HxdYg&oe=64AC6E7C&_nc_sid=10d13b"
-                                },
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358337983_581973004113850_7681929282916239696_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=110&_nc_ohc=9xd6QhLrfr0AX_jXvvd&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD01Al_ukeQOVXysDuudHw82ZUfn4q_PI1KuWE1Swf1Kw&oe=64AC446D&_nc_sid=10d13b"
-                                },
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358357576_689254799697876_1184079927626851628_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=100&_nc_ohc=95IT8pfSV8MAX8qeB2M&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfBtniKWdsj56GWa3T_UQZG6xEhLv_2ck-q_V9J34Pb4ag&oe=64ADA8C7&_nc_sid=10d13b"
-                                }
-                            ],
-                            "should_show_replies_cta": true,
-                            "__typename": "XDTThreadItem"
+                            "height": 640,
+                            "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAY-75SdPDasc0ophRu3lgeeHmnb3qPZIE-mCPh8PRRBw&oe=64AED800&_nc_sid=10d13b",
+                            "width": 640
                         }
                     ],
-                    "id": "3141002295235099165"
-                },
-                ...
-            ]
+                    "is_verified": true,
+                    "biography": "",
+                    "biography_with_entities": null,
+                    "follower_count": 2663588,
+                    "profile_context_facepile_users": null,
+                    "bio_links": [
+                        {
+                            "url": ""
+                        }
+                    ],
+                    "pk": "314216",
+                    "full_name": "Mark Zuckerberg",
+                    "id": null
+                }
+            }
+        },
+        "extensions": {
+            "is_final": true
         }
-    },
-    "extensions": {
-        "is_final": true
     }
 }
 ```
 
 ### Get User Replies
 
 To get a user's replies, use the following commands:
```

### Comparing `threads-net-0.0.7/setup.py` & `threads-net-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md', 'r', encoding='utf-8') as read_me:
     long_description = read_me.read()
 
 with open('requirements/project.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.0.7',
+    version='0.0.8',
     name='threads-net',
     description='Threads (threads.net) Python API wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/threads',
     license='MIT',
     author='Dmytro Striletskyi',
```

### Comparing `threads-net-0.0.7/threads/main.py` & `threads-net-0.0.8/threads/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,31 +74,48 @@
         response = requests.get('https://www.threads.net/@instagram')
 
         token_key_position = response.text.find('\"token\"')
         token = response.text[token_key_position + 9:token_key_position + 31]
 
         return token
 
-    def get_user_by_username(self, username: str):
+    def get_user_id(self, username: str):
         """
-        Get a user by identifier.
+        Get a user's identifier.
 
         Arguments:
             username (str): a user's username.
         """
-        return self.user_info_by_username_v1(username=username).dict()
+        return self.user_info_by_username_v1(username=username).dict().get('pk')
 
     def get_user_by_id(self, id: int):
         """
         Get a user.
 
         Arguments:
             id (int): a user's identifier.
         """
-        return self.user_info_gql(user_id=id).dict()
+        response = requests.post(
+            url=self.THREADS_API_URL,
+            headers={
+                'Content-Type': 'application/x-www-form-urlencoded',
+                'X-IG-App-ID': '238260118697367',
+                'X-FB-LSD': self.temporary_token,
+                'Sec-Fetch-Site': 'same-origin',
+            },
+            data={
+                'lsd': self.temporary_token,
+                'variables': json.dumps({
+                    'userID': id,
+                }),
+                'doc_id': '23996318473300828',
+            },
+        )
+
+        return response.json()
 
     def get_user_threads(self, id: int):
         """
         Get a user's threads.
 
         Arguments:
             id (int):
```

### Comparing `threads-net-0.0.7/threads_net.egg-info/PKG-INFO` & `threads-net-0.0.8/threads_net.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.7
+Version: 0.0.8
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -18,46 +18,49 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
 
-Threads (threads.net) Python API wrapper
+Threads (threads.net) Python API wrapper.
 
-[![Downdloads](https://pepy.tech/badge/threads-net)](https://pepy.tech/project/threads-net)
+[![Downloads](https://pepy.tech/badge/threads-net)](https://pepy.tech/project/threads-net)
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
 * [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
   * [How to install](#how-to-install)
   * [Initialization](#initialization)
   * [Examples](#examples)
 * [API](#api)
   * [Login](#login)
-  * [Get User By Username](#get-user-by-username)
+  * [Get User Identifier](#get-user-identifier)
   * [Get User By Identifier](#get-user-by-identifier)
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
 ## Disclaimer
 
-* This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
-  Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
-  needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
-  So use the project at your own risk until the normal `Threads` public `API` is available or this product become more
-  stable for such things.
-* For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
-  is used because `Threads` are backed by `Instagram` and you do a login via it as well.
-* As the library use `Threads API ` private endpoints, they have no defined model for support and backward compatibility. 
-* So, some methods might end up not working until the library maintainers find out hot to fix it.
+* As `Threads` are backed by `Instagram`. It means that `Threads` functionality partially placed in `Instagram API`:
+  you do a login to `Threads` application via `Instagram`'s username and password, posting new threads and fetching user
+  identifier (for further library usage) too. So expect seeing things related to `Instagram` in this library.
+* This project is unofficial and utilize both public and private endpoints of both `Threads` and `Instagram` `APIs`. 
+  Utilizing private endpoints means pretending being a mobile phone or web user (via proper `HTTP` headers and other 
+  things). Thus you might face `rate limits` (because pretending is never ideal) or even your account in `Threads` and 
+  `Instagram` might be suspended if mess up with logining or sending too much requests. So use the project at your own 
+  risk until the normal public `ThreadsAPI` is released or this product become more stable for such things.Also,
+  utilizing such endpoints mean that they might not be stable (because they are under active development and there is
+  no any promise in backward compatibility).
+* For all the `Instagram`-related thing other well-know and already stable library called [instagrapi](https://github.com/adw0rd/instagrapi)
+  is used in `threads-net`.
 
 ## Getting started
 
 ### How to install
 
 Install the library with the following command using `pip3`:
 
@@ -90,15 +93,15 @@
 ```
 
 ## API
 
 ### Login
 
 In order for `Instagram` to trust you more, you must always login from one device and one IP (or from a subnet), for 
-this there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+this there is the dump session functionality. So, once you logged in once, store it into a file:
 
 ```python3
 >>> threads = Threads()
 >>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
 >>> threads.dump_settings('session.json')
 ```
 
@@ -107,230 +110,153 @@
 ```python3
 >>> threads = Threads()
 >>> threads.load_settings('session.json')
 >>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
 ```
 
 The login method might ask for additional username/password entering, confirmation code and other challenges. But if
-you reuse the session, those should be minimum times. For more information, check this out — 
+you reuse the session, those should happen minimum times. For more information, check this out — 
 https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
 
-Also, the login is only needed for getting a user by identifier and username, for other endpoints it is not required, so
-you can easily skip it.
+### Get User Identifier
 
-### Get User by Username
-
-To get a user by a username, use the following commands:
+To get a user's identifier by a username, use the following commands:
 
 ```python3
->>> user = threads.get_user_by_username(username='zuck')
->>> user
-{
-    "pk": 314216,
-    "username": "zuck",
-    "full_name": "Mark Zuckerberg",
-    "is_private": False,
-    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
-    "is_verified": False,
-    "media_count": 102,
-    "follower_count": 576,
-    "following_count": 538,
-    "biography": '',
-    "is_business": False
-}
+>>> user_id = threads.get_user_id(username='zuck')
+>>> user_id
+314216
 ```
 
 ### Get User by Identifier
 
 To get a user by an identifier, use the following commands:
 
 ```python3
 >>> user = threads.get_user_by_id(id=314216)
 >>> user
 {
-    "pk": 314216,
-    "username": "zuck",
-    "full_name": "Mark Zuckerberg",
-    "is_private": False,
-    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
-    "is_verified": False,
-    "media_count": 102,
-    "follower_count": 576,
-    "following_count": 538,
-    "biography": '',
-    "is_business": False
+    "data": {
+        "userData": {
+            "user": {
+                "is_private": false,
+                "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAUZzobOIH6imLnb2Z3iXoWY5H1Fv_kNnyG8T4UGgJegQ&oe=64AED800&_nc_sid=10d13b",
+                "username": "zuck",
+                "hd_profile_pic_versions": [
+                    {
+                        "height": 320,
+                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD5z6UgnQH54dihPnMrXgH2L-mLCMGlFsIF9Ug7U4RWdA&oe=64AED800&_nc_sid=10d13b",
+                        "width": 320
+                    },
+                    {
+                        "height": 640,
+                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX-mW2_l&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD4BaVu4cDcX53xPocD-3o_ZbKIESxUZhlU08FBpycCsA&oe=64AED800&_nc_sid=10d13b",
+                        "width": 640
+                    }
+                ],
+                "is_verified": true,
+                "biography": "",
+                "biography_with_entities": null,
+                "follower_count": 2663947,
+                "profile_context_facepile_users": null,
+                "bio_links": [
+                    {
+                        "url": ""
+                    }
+                ],
+                "pk": "314216",
+                "full_name": "Mark Zuckerberg",
+                "id": null
+            }
+        }
+    },
+    "extensions": {
+        "is_final": true
+    }
 }
 ```
 
 ### Get User Threads
 
 To get a user's threads, use the following commands:
 
 ```python3
 >>> user_threads = threads.get_user_threads(id=314216)
 >>> user_threads
 {
-    "data": {
-        "mediaData": {
-            "threads": [
-                {
-                    "thread_items": [
+    "instagram": {
+        "pk": "314216",
+        "username": "zuck",
+        "full_name": "Mark Zuckerberg",
+        "is_private": false,
+        "profile_pic_url": "https://instagram.fiev6-1.fna.fbcdn.net/v/t51.2885-19/352224138_1028122805231303_1175896139426286760_n.jpg?stp=dst-jpg_s150x150&_nc_ht=instagram.fiev6-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=hbekpcjRfioAX8iYGJv&edm=AKEQFekBAAAA&ccb=7-5&oh=00_AfDf2r6qwujUc84tkzUlYJMfJt66xoWScQ-nsB5bmtYDnw&oe=64B0066A&_nc_sid=29ddf3",
+        "profile_pic_url_hd": "https://instagram.fiev6-1.fna.fbcdn.net/v/t51.2885-19/352224138_1028122805231303_1175896139426286760_n.jpg?stp=dst-jpg_s320x320&_nc_ht=instagram.fiev6-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=hbekpcjRfioAX8iYGJv&edm=AKEQFekBAAAA&ccb=7-5&oh=00_AfCoPcYmzHdc2evDvduZjZK-IxDS07wGf0x9czecY_TgVQ&oe=64B0066A&_nc_sid=29ddf3",
+        "is_verified": true,
+        "media_count": 283,
+        "follower_count": 11924434,
+        "following_count": 523,
+        "biography": "",
+        "external_url": null,
+        "account_type": null,
+        "is_business": false,
+        "public_email": null,
+        "contact_phone_number": null,
+        "public_phone_country_code": null,
+        "public_phone_number": null,
+        "business_contact_method": "UNKNOWN",
+        "business_category_name": null,
+        "category_name": "Entrepreneur",
+        "category": null,
+        "address_street": null,
+        "city_id": null,
+        "city_name": null,
+        "latitude": null,
+        "longitude": null,
+        "zip": null,
+        "instagram_location_id": null,
+        "interop_messaging_user_fbid": null
+    },
+    "threads": {
+        "data": {
+            "userData": {
+                "user": {
+                    "is_private": false,
+                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfCdAMkmk0XL_r0GQi2MRD1Aq1kPZKBLfXLby47e_hsZrg&oe=64AED800&_nc_sid=10d13b",
+                    "username": "zuck",
+                    "hd_profile_pic_versions": [
+                        {
+                            "height": 320,
+                            "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDJeE127_ZFA-eD3qRMM0Fh2NM-jRR4tUFsTywCrMctNA&oe=64AED800&_nc_sid=10d13b",
+                            "width": 320
+                        },
                         {
-                            "post": {
-                                "user": {
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-q_Nrf&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDWsSPBghiIhwJnh4_3kO5maVMhDErg9ky_-dhqUHVtRw&oe=64ACDDC0&_nc_sid=10d13b",
-                                    "username": "zuck",
-                                    "id": null,
-                                    "is_verified": true,
-                                    "pk": "314216"
-                                },
-                                "image_versions2": {
-                                    "candidates": [
-                                        {
-                                            "height": 3000,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfBVkBmYMO2TozQJYlE6xblN10YDdmKXhzzs0hSHHCfUgQ&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 4000,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 810,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s1080x1080&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCl-OTiAWiST-z8pGT0IHQAcdQiuWxdoI44UQccZrvkdw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 1080,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 540,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s720x720&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCQ6PZm83pOL4_QMalEvrzu1TTLWqvHWMVK3WercfrQdA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 720,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 480,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s640x640_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfB6A9bQNJLWiNgczI7Kp7q7wII7TC1ifn4oVd5cN8nTBg&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 640,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 360,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s480x480&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfAtSvruwFWIjemafFJXaFfb_iag6LMjJL7EFaBmZmyP0Q&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 480,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 240,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCCyzKffNLdsvdSRuyHMdAN-F7sEALSVrc0kM3R2nsrQA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 320,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 180,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=dst-jpg_e35_s240x240&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCq8hu-NdtgzUrS_S4MnBrJX4ogGvCiAIhG_gr6xwp5Ag&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 240,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 1080,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s1080x1080&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfDWf1VGojZDDWQDCDO1x0l3SU34cgdEOceFGPxK_9EZfA&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 1080,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 750,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s750x750_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfA-Kqa9UoMluJGqD_wBNG3qtcbWT63RCkq07fDo88ZVaw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 750,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 640,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s640x640_sh0.08&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCh7r-VI_5fLBmsPNp_cb-rZSBsDJTYdrn0PnMKBgATlw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 640,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 480,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s480x480&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfBXkMC4qSLcsgFURS0yXTu02CyydoJpInHfOr5L-FP5ww&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 480,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 320,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCwJtku5xDOM0dxwCvfAzmV64T-_kaA4CZLOIl3OTNiJQ&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 320,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 240,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s240x240&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfCxaBgqYV7qj0svYLI1KavhteMygChYAfZma84Fe0tZmw&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 240,
-                                            "__typename": "XDTImageCandidate"
-                                        },
-                                        {
-                                            "height": 150,
-                                            "url": "https://scontent.cdninstagram.com/v/t51.2885-15/357916630_786901039847062_4398530087245184228_n.jpg?stp=c500.0.3000.3000a_dst-jpg_e35_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=vSLyED13mHsAX-BfOPb&edm=APs17CUBAAAA&ccb=7-5&ig_cache_key=MzE0MTAwMjI5NTIzNTA5OTE2NQ%3D%3D.2-ccb7-5&oh=00_AfDwSo36FyoIW052Qvgp7eDCfi-ij8x3NsySfbpfQAlM_Q&oe=64ACBB47&_nc_sid=10d13b",
-                                            "width": 150,
-                                            "__typename": "XDTImageCandidate"
-                                        }
-                                    ]
-                                },
-                                "original_width": 4000,
-                                "original_height": 3000,
-                                "video_versions": [],
-                                "carousel_media": null,
-                                "carousel_media_count": null,
-                                "pk": "3141002295235099165",
-                                "has_audio": null,
-                                "text_post_app_info": {
-                                    "link_preview_attachment": null,
-                                    "share_info": {
-                                        "quoted_post": null,
-                                        "reposted_post": null
-                                    },
-                                    "reply_to_author": null,
-                                    "is_post_unavailable": false
-                                },
-                                "caption": {
-                                    "text": "Lots of work on basic capabilities this morning."
-                                },
-                                "taken_at": 1688656673,
-                                "like_count": 184611,
-                                "code": "CuXFPIeLLod",
-                                "media_overlay_info": null,
-                                "id": "3141002295235099165_314216"
-                            },
-                            "line_type": "line",
-                            "view_replies_cta_string": "17,882 replies",
-                            "reply_facepile_users": [
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358166568_272137218742674_3025287304976949959_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=106&_nc_ohc=Wl0wRGxM7g4AX-cl1FE&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAaJRzZHv09tlkXbrdFTQC-ZhwW7v2BPih4fIBN3HxdYg&oe=64AC6E7C&_nc_sid=10d13b"
-                                },
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358337983_581973004113850_7681929282916239696_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=110&_nc_ohc=9xd6QhLrfr0AX_jXvvd&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfD01Al_ukeQOVXysDuudHw82ZUfn4q_PI1KuWE1Swf1Kw&oe=64AC446D&_nc_sid=10d13b"
-                                },
-                                {
-                                    "__typename": "XDTUserDict",
-                                    "id": null,
-                                    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/358357576_689254799697876_1184079927626851628_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=100&_nc_ohc=95IT8pfSV8MAX8qeB2M&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfBtniKWdsj56GWa3T_UQZG6xEhLv_2ck-q_V9J34Pb4ag&oe=64ADA8C7&_nc_sid=10d13b"
-                                }
-                            ],
-                            "should_show_replies_cta": true,
-                            "__typename": "XDTThreadItem"
+                            "height": 640,
+                            "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=euIj8dtTGIkAX9JAAZI&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfAY-75SdPDasc0ophRu3lgeeHmnb3qPZIE-mCPh8PRRBw&oe=64AED800&_nc_sid=10d13b",
+                            "width": 640
                         }
                     ],
-                    "id": "3141002295235099165"
-                },
-                ...
-            ]
+                    "is_verified": true,
+                    "biography": "",
+                    "biography_with_entities": null,
+                    "follower_count": 2663588,
+                    "profile_context_facepile_users": null,
+                    "bio_links": [
+                        {
+                            "url": ""
+                        }
+                    ],
+                    "pk": "314216",
+                    "full_name": "Mark Zuckerberg",
+                    "id": null
+                }
+            }
+        },
+        "extensions": {
+            "is_final": true
         }
-    },
-    "extensions": {
-        "is_final": true
     }
 }
 ```
 
 ### Get User Replies
 
 To get a user's replies, use the following commands:
```

