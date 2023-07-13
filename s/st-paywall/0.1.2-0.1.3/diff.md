# Comparing `tmp/st-paywall-0.1.2.tar.gz` & `tmp/st-paywall-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-paywall-0.1.2.tar", last modified: Mon Jul 10 04:35:47 2023, max compression
+gzip compressed data, was "st-paywall-0.1.3.tar", last modified: Thu Jul 13 05:42:18 2023, max compression
```

## Comparing `st-paywall-0.1.2.tar` & `st-paywall-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.621211 st-paywall-0.1.2/
--rw-r--r--   0 trichards   (501) staff       (20)     6062 2023-07-10 04:35:47.621000 st-paywall-0.1.2/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     5839 2023-07-10 04:34:35.000000 st-paywall-0.1.2/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      358 2023-07-10 04:35:29.000000 st-paywall-0.1.2/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-10 04:35:47.621272 st-paywall-0.1.2/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.616163 st-paywall-0.1.2/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.618414 st-paywall-0.1.2/src/st_paywall/
--rw-r--r--   0 trichards   (501) staff       (20)       36 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     1616 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-10 04:34:35.000000 st-paywall-0.1.2/src/st_paywall/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-10 04:35:47.620691 st-paywall-0.1.2/src/st_paywall.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     6062 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      333 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       11 2023-07-10 04:35:47.000000 st-paywall-0.1.2/src/st_paywall.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.704770 st-paywall-0.1.3/
+-rw-r--r--   0 trichards   (501) staff       (20)     7311 2023-07-13 05:42:18.704561 st-paywall-0.1.3/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     7054 2023-07-13 05:37:47.000000 st-paywall-0.1.3/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      396 2023-07-13 03:05:04.000000 st-paywall-0.1.3/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-13 05:42:18.704820 st-paywall-0.1.3/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.697859 st-paywall-0.1.3/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.701305 st-paywall-0.1.3/src/st_paywall/
+-rw-r--r--   0 trichards   (501) staff       (20)       36 2023-07-10 04:34:35.000000 st-paywall-0.1.3/src/st_paywall/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     2089 2023-07-13 05:28:47.000000 st-paywall-0.1.3/src/st_paywall/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1218 2023-07-13 05:26:48.000000 st-paywall-0.1.3/src/st_paywall/buymeacoffee_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-10 04:34:35.000000 st-paywall-0.1.3/src/st_paywall/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1243 2023-07-13 05:31:13.000000 st-paywall-0.1.3/src/st_paywall/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.703538 st-paywall-0.1.3/src/st_paywall.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     7311 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      369 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       11 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/top_level.txt
```

### Comparing `st-paywall-0.1.2/PKG-INFO` & `st-paywall-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: st-paywall
-Version: 0.1.2
-Summary: A Python package for creating subscription Streamlit apps
-Author-email: Tyler <tylerjrichards@gmail.com>
-License: MIT
-Description-Content-Type: text/markdown
-
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
 
 Kind consultant: [@blackary](https://github.com/blackary)
@@ -26,57 +18,61 @@
 
 <p>&nbsp;</p>
 
 # 🥟 st-paywall
 
 <strong>A python package for creating paid Streamlit apps with a paywall! </strong>
 
+## Why st-paywall?
+
+I made st-paywall so data scientists and LLM developers can create small businesses around their Streamlit apps. Every week I see dozens of new incredible apps built in Streamlit that are adored by users, but eventually shut down or moved off of Streamlit as authentication and payment integration are too hard. This is my attempt at a dead-simple API around each, abstracting the both away into a single function (`add_auth`). Enjoy!
+
 ## Overview
 
-This package gives you one basic functions (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
+This package gives you one basic function (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
 If the `required` parameter is `True`, the app will stop with `st.stop()` if the user is not logged in and subscribed. Otherwise, you the developer will have control over exactly how you want to paywall the apps!
 
  I hope you use this to create tons of value, and capture some of it with the magic of Streamlit.
 
 This package expects that you have a `.streamlit/secrets.toml` file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
 The subscription link should be added to secrets.toml like this.
 
 ```toml
-stripe_link = 'https://buy.stripe.com/test_...'`
+stripe_link = 'https://buy.stripe.com/test_...'
 ```
 
 You also need to create an [Standard API key](https://dashboard.stripe.com/test/apikeys), which just like subscription links have test options as well. Store your API key in your secrets file as stripe_api_key and you're off to the races. If you make a restricted API key instead of a Standard key, make sure to add read permission on Customers
 
 
 <img src="readme_img/stripe_api_rest.png" width="500">
 
 
 The API key should be added to `secrets.toml` like this
 
 
 ```toml
-stripe_api_key = 'sk_...'`
+stripe_api_key = 'sk_...'
 ```
 
 By default this repo links to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info! To run st-paywall in test mode, add the following to your secrets file.
 
 ```toml
 testing_mode = true
 ```
 
 Then, the package will look for the following secrets. Otherwise, it will look for the production api and link secrets. I highly encourage you to start out in test mode!
 
 ```toml
-stripe_api_key_test = 'sk_test_...'`
-stripe_link_test = 'https://buy.stripe.com/test_...'`
+stripe_api_key_test = 'sk_test_...'
+stripe_link_test = 'https://buy.stripe.com/test_...'
 ```
 
 Once you decide to leave test mode and publish your subscription app, it is a good idea to have Stripe send the user back to your app once they've subscribed. To do this, go to the [payment links](https://dashboard.stripe.com/payment-links) page, edit your payment link, click 'After payment' and fill out your app's url.
 
 
 <img src="readme_img/payment_link_after.png" width="500">
 
@@ -102,11 +98,22 @@
 redirect_url_test = 'http://localhost.com:8501'
 ```
 
 For my test application at subscription.streamlit.app, my Google console looks like this.
 
 <img src="readme_img/google_oauth_console.png" width="300">
 
+### Buy Me A Coffee
+
+Not everywhere in the world is covered by Stripe! Buy Me A Coffee is a lighter, less business-y service that allows folks to support you online. To link to your buy me a coffee page instead of your Stripe payment link, go to their [dev page](https://developers.buymeacoffee.com/dashboard) and create an access token. You will also add a [membership product offering](https://www.buymeacoffee.com/membership) as well. Once you have the membership link and the key, add the following to your secrets file.
+
+```toml
+payment_provider = "bmac"
+bmac_api_key = "eyJ0...."
+bmac_link = "https://www.buymeacoffee.com/..."
+```
+
+This will change your app to link out to buymeacoffee instead of Stripe, and will get your customer list from there as well!
 
 ### Feedback:
 
 If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
```

### Comparing `st-paywall-0.1.2/README.md` & `st-paywall-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: st-paywall
+Version: 0.1.3
+Summary: A Python package for creating subscription Streamlit apps
+Author-email: Tyler Richards <tylerjrichards@gmail.com>
+License: MIT
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
 
 Kind consultant: [@blackary](https://github.com/blackary)
@@ -18,57 +27,61 @@
 
 <p>&nbsp;</p>
 
 # 🥟 st-paywall
 
 <strong>A python package for creating paid Streamlit apps with a paywall! </strong>
 
+## Why st-paywall?
+
+I made st-paywall so data scientists and LLM developers can create small businesses around their Streamlit apps. Every week I see dozens of new incredible apps built in Streamlit that are adored by users, but eventually shut down or moved off of Streamlit as authentication and payment integration are too hard. This is my attempt at a dead-simple API around each, abstracting the both away into a single function (`add_auth`). Enjoy!
+
 ## Overview
 
-This package gives you one basic functions (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
+This package gives you one basic function (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
 If the `required` parameter is `True`, the app will stop with `st.stop()` if the user is not logged in and subscribed. Otherwise, you the developer will have control over exactly how you want to paywall the apps!
 
  I hope you use this to create tons of value, and capture some of it with the magic of Streamlit.
 
 This package expects that you have a `.streamlit/secrets.toml` file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
 The subscription link should be added to secrets.toml like this.
 
 ```toml
-stripe_link = 'https://buy.stripe.com/test_...'`
+stripe_link = 'https://buy.stripe.com/test_...'
 ```
 
 You also need to create an [Standard API key](https://dashboard.stripe.com/test/apikeys), which just like subscription links have test options as well. Store your API key in your secrets file as stripe_api_key and you're off to the races. If you make a restricted API key instead of a Standard key, make sure to add read permission on Customers
 
 
 <img src="readme_img/stripe_api_rest.png" width="500">
 
 
 The API key should be added to `secrets.toml` like this
 
 
 ```toml
-stripe_api_key = 'sk_...'`
+stripe_api_key = 'sk_...'
 ```
 
 By default this repo links to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info! To run st-paywall in test mode, add the following to your secrets file.
 
 ```toml
 testing_mode = true
 ```
 
 Then, the package will look for the following secrets. Otherwise, it will look for the production api and link secrets. I highly encourage you to start out in test mode!
 
 ```toml
-stripe_api_key_test = 'sk_test_...'`
-stripe_link_test = 'https://buy.stripe.com/test_...'`
+stripe_api_key_test = 'sk_test_...'
+stripe_link_test = 'https://buy.stripe.com/test_...'
 ```
 
 Once you decide to leave test mode and publish your subscription app, it is a good idea to have Stripe send the user back to your app once they've subscribed. To do this, go to the [payment links](https://dashboard.stripe.com/payment-links) page, edit your payment link, click 'After payment' and fill out your app's url.
 
 
 <img src="readme_img/payment_link_after.png" width="500">
 
@@ -94,11 +107,22 @@
 redirect_url_test = 'http://localhost.com:8501'
 ```
 
 For my test application at subscription.streamlit.app, my Google console looks like this.
 
 <img src="readme_img/google_oauth_console.png" width="300">
 
+### Buy Me A Coffee
+
+Not everywhere in the world is covered by Stripe! Buy Me A Coffee is a lighter, less business-y service that allows folks to support you online. To link to your buy me a coffee page instead of your Stripe payment link, go to their [dev page](https://developers.buymeacoffee.com/dashboard) and create an access token. You will also add a [membership product offering](https://www.buymeacoffee.com/membership) as well. Once you have the membership link and the key, add the following to your secrets file.
+
+```toml
+payment_provider = "bmac"
+bmac_api_key = "eyJ0...."
+bmac_link = "https://www.buymeacoffee.com/..."
+```
+
+This will change your app to link out to buymeacoffee instead of Stripe, and will get your customer list from there as well!
 
 ### Feedback:
 
-If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
+If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
```

### Comparing `st-paywall-0.1.2/src/st_paywall/aggregate_auth.py` & `st-paywall-0.1.3/src/st_paywall/aggregate_auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import streamlit as st
 from .google_auth import get_logged_in_user_email, show_login_button
 from .stripe_auth import get_customer_emails, redirect_button
+from .buymeacoffee_auth import get_bmac_payers
+
+payment_provider = st.secrets.get("payment_provider", "stripe")
 
 def add_auth(required=True):
     if required:
         require_auth()
     else:
         optional_auth()
 
 def require_auth():
     user_email = get_logged_in_user_email()
 
     if not user_email:
         show_login_button()
         st.stop()
-
-    customer_emails = get_customer_emails()
+    if payment_provider == "stripe":
+        customer_emails = get_customer_emails()
+    elif payment_provider == "bmac":
+        customer_emails = get_bmac_payers()
 
     if user_email not in customer_emails:
-        redirect_button(text="Subscribe now!", customer_email=user_email)
+        redirect_button(text="Subscribe now!",
+                        customer_email=user_email,
+                        payment_provider=payment_provider)
         st.session_state.user_subscribed = False
         st.stop()
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
     if st.sidebar.button("Logout", type="primary"):
         del st.session_state.email
         del st.session_state.user_subscribed
         st.experimental_rerun()
 
 def optional_auth():
     user_email = get_logged_in_user_email()
-    customer_emails = get_customer_emails()
+    if payment_provider == "stripe":
+        customer_emails = get_customer_emails()
+    elif payment_provider == "bmac":
+        customer_emails = get_bmac_payers()
 
     if not user_email:
         show_login_button()
         st.session_state.email = ""
         st.sidebar.markdown("")
 
     if user_email and user_email not in customer_emails:
-        redirect_button(text="Subscribe now!", customer_email="")
+        redirect_button(text="Subscribe now!", customer_email="", payment_provider=payment_provider)
         st.sidebar.markdown("")
         st.session_state.user_subscribed = False
 
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
     if st.session_state.email != "":
```

### Comparing `st-paywall-0.1.2/src/st_paywall/google_auth.py` & `st-paywall-0.1.3/src/st_paywall/google_auth.py`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.2/src/st_paywall/stripe_auth.py` & `st-paywall-0.1.3/src/st_paywall/stripe_auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,21 @@
 stripe_link = st.secrets["stripe_link_test"] if testing_mode else st.secrets["stripe_link"]
 
 
 def redirect_button(
     text: str,
     customer_email: str,
     color="#FD504D",
+    payment_provider: str = "stripe",
 ):
     encoded_email = urllib.parse.quote(customer_email)
-    button_url = f"{stripe_link}?prefilled_email={encoded_email}"
+    if payment_provider == "stripe":
+        button_url = f"{stripe_link}?prefilled_email={encoded_email}"
+    elif payment_provider == "bmac":
+        button_url = f"{st.secrets['bmac_link']}"
 
     st.sidebar.markdown(
         f"""
     <a href="{button_url}" target="_blank">
         <div style="
             display: inline-block;
             padding: 0.5em 1em;
```

### Comparing `st-paywall-0.1.2/src/st_paywall.egg-info/PKG-INFO` & `st-paywall-0.1.3/src/st_paywall.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: st-paywall
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for creating subscription Streamlit apps
-Author-email: Tyler <tylerjrichards@gmail.com>
+Author-email: Tyler Richards <tylerjrichards@gmail.com>
 License: MIT
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
@@ -26,57 +27,61 @@
 
 <p>&nbsp;</p>
 
 # 🥟 st-paywall
 
 <strong>A python package for creating paid Streamlit apps with a paywall! </strong>
 
+## Why st-paywall?
+
+I made st-paywall so data scientists and LLM developers can create small businesses around their Streamlit apps. Every week I see dozens of new incredible apps built in Streamlit that are adored by users, but eventually shut down or moved off of Streamlit as authentication and payment integration are too hard. This is my attempt at a dead-simple API around each, abstracting the both away into a single function (`add_auth`). Enjoy!
+
 ## Overview
 
-This package gives you one basic functions (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
+This package gives you one basic function (`add_auth`) that adds subscription functionality to your Streamlit apps. `add_auth` will add both a Google login button if they are not logged in, and a Stripe subscription button to your sidebar if they are not subscribed. If they are subscribed, `st.session_state.user_subscribed` will be true, and if they are logged in, `st.session_state.email` will have their email.
 If the `required` parameter is `True`, the app will stop with `st.stop()` if the user is not logged in and subscribed. Otherwise, you the developer will have control over exactly how you want to paywall the apps!
 
  I hope you use this to create tons of value, and capture some of it with the magic of Streamlit.
 
 This package expects that you have a `.streamlit/secrets.toml` file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
 The subscription link should be added to secrets.toml like this.
 
 ```toml
-stripe_link = 'https://buy.stripe.com/test_...'`
+stripe_link = 'https://buy.stripe.com/test_...'
 ```
 
 You also need to create an [Standard API key](https://dashboard.stripe.com/test/apikeys), which just like subscription links have test options as well. Store your API key in your secrets file as stripe_api_key and you're off to the races. If you make a restricted API key instead of a Standard key, make sure to add read permission on Customers
 
 
 <img src="readme_img/stripe_api_rest.png" width="500">
 
 
 The API key should be added to `secrets.toml` like this
 
 
 ```toml
-stripe_api_key = 'sk_...'`
+stripe_api_key = 'sk_...'
 ```
 
 By default this repo links to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info! To run st-paywall in test mode, add the following to your secrets file.
 
 ```toml
 testing_mode = true
 ```
 
 Then, the package will look for the following secrets. Otherwise, it will look for the production api and link secrets. I highly encourage you to start out in test mode!
 
 ```toml
-stripe_api_key_test = 'sk_test_...'`
-stripe_link_test = 'https://buy.stripe.com/test_...'`
+stripe_api_key_test = 'sk_test_...'
+stripe_link_test = 'https://buy.stripe.com/test_...'
 ```
 
 Once you decide to leave test mode and publish your subscription app, it is a good idea to have Stripe send the user back to your app once they've subscribed. To do this, go to the [payment links](https://dashboard.stripe.com/payment-links) page, edit your payment link, click 'After payment' and fill out your app's url.
 
 
 <img src="readme_img/payment_link_after.png" width="500">
 
@@ -102,11 +107,22 @@
 redirect_url_test = 'http://localhost.com:8501'
 ```
 
 For my test application at subscription.streamlit.app, my Google console looks like this.
 
 <img src="readme_img/google_oauth_console.png" width="300">
 
+### Buy Me A Coffee
+
+Not everywhere in the world is covered by Stripe! Buy Me A Coffee is a lighter, less business-y service that allows folks to support you online. To link to your buy me a coffee page instead of your Stripe payment link, go to their [dev page](https://developers.buymeacoffee.com/dashboard) and create an access token. You will also add a [membership product offering](https://www.buymeacoffee.com/membership) as well. Once you have the membership link and the key, add the following to your secrets file.
+
+```toml
+payment_provider = "bmac"
+bmac_api_key = "eyJ0...."
+bmac_link = "https://www.buymeacoffee.com/..."
+```
+
+This will change your app to link out to buymeacoffee instead of Stripe, and will get your customer list from there as well!
 
 ### Feedback:
 
 If you have feedback about this package, please reach out to me on [twitter](https://twitter.com/tylerjrichards) or file an issue in [this repo](https://github.com/tylerjrichards/st-paywall/issues) and I will do my best to help you out.
```

