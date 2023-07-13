# Comparing `tmp/nordvpn-tray-1.0.3.tar.gz` & `tmp/nordvpn-tray-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordvpn-tray-1.0.3.tar", last modified: Wed Jul 12 17:51:03 2023, max compression
+gzip compressed data, was "nordvpn-tray-1.0.4.tar", last modified: Thu Jul 13 12:48:27 2023, max compression
```

## Comparing `nordvpn-tray-1.0.3.tar` & `nordvpn-tray-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 17:51:03.268887 nordvpn-tray-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4804 2023-07-12 17:51:03.262886 nordvpn-tray-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3748 2023-07-11 22:24:38.000000 nordvpn-tray-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 17:51:03.268887 nordvpn-tray-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2630 2023-07-12 17:50:55.000000 nordvpn-tray-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:51:03.216809 nordvpn-tray-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 17:51:03.233842 nordvpn-tray-1.0.3/src/nordvpn_tray/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.3/src/nordvpn_tray/__init__.py
--rw-rw-rw-   0        0        0     4899 2023-07-12 16:47:56.000000 nordvpn-tray-1.0.3/src/nordvpn_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:51:03.259125 nordvpn-tray-1.0.3/src/nordvpn_tray/resources/
--rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.3/src/nordvpn_tray/resources/nvt.ico
-drwxrwxrwx   0        0        0        0 2023-07-12 17:51:03.257125 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/
--rw-rw-rw-   0        0        0     4804 2023-07-12 17:51:03.000000 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-12 17:51:03.000000 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 17:51:03.000000 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-12 17:51:03.000000 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-07-12 17:51:03.000000 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 17:51:03.000000 nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.102218 nordvpn-tray-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4702 2023-07-13 12:48:27.096295 nordvpn-tray-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3748 2023-07-11 22:24:38.000000 nordvpn-tray-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:48:27.102218 nordvpn-tray-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2530 2023-07-13 12:47:59.000000 nordvpn-tray-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.057839 nordvpn-tray-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.069840 nordvpn-tray-1.0.4/src/nordvpn_tray/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.4/src/nordvpn_tray/__init__.py
+-rw-rw-rw-   0        0        0     5374 2023-07-13 09:27:53.000000 nordvpn-tray-1.0.4/src/nordvpn_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.093295 nordvpn-tray-1.0.4/src/nordvpn_tray/resources/
+-rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.4/src/nordvpn_tray/resources/nvt.ico
+drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.091295 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/
+-rw-rw-rw-   0        0        0     4702 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-13 12:48:27.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/top_level.txt
```

### Comparing `nordvpn-tray-1.0.3/LICENSE` & `nordvpn-tray-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.3/PKG-INFO` & `nordvpn-tray-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.3
+Version: 1.0.4
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nordvpn-tray-1.0.3/README.md` & `nordvpn-tray-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.3/setup.py` & `nordvpn-tray-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='nordvpn-tray',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "nordvpn_tray": ["*.py"],
         "nordvpn_tray.resources": ["*.ico"],
     },
     description='A cross-platform system tray application for interacting with NordVPN.',
@@ -50,16 +50,14 @@
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: End Users/Desktop',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     ],
 )
```

### Comparing `nordvpn-tray-1.0.3/src/nordvpn_tray/__main__.py` & `nordvpn-tray-1.0.4/src/nordvpn_tray/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,45 +16,61 @@
 along with this program. If not, see <https://www.gnu.org/licenses/>.
 """
 import os
 import subprocess
 import re
 import pkg_resources
 import pystray
+import requests
 from pystray import Icon
 from PIL import Image
-import requests
 from country_converter import CountryConverter
 
 
 def get_full_domain_identifier(short_domain_identifier):
     country_converter = CountryConverter()
     country_code = short_domain_identifier[:2].upper()
     country_name = country_converter.convert(names=country_code, to='name_short')
     if country_name:
         return f"{country_name} #{short_domain_identifier[2:]}"
     else:
         return "Invalid country code"
 
 
-def create_callback(domain):
+def on_quit_selected(icon, item):
+    icon.stop()
+
+
+def create_connect_callback(domain):
     def callback(icon, domain):
         icon.notify(str(domain))
         domain_identifier = re.search(r"\[(\w+)\.nordvpn\.com]", str(domain)).group(1)
         full_domain_identifier = get_full_domain_identifier(domain_identifier)
         if domain_identifier:
             if os.name == 'nt':
                 command = f'cd C:/Program Files/NordVpn/ & nordvpn -c -n "{full_domain_identifier}"'
             else:
                 command = f"nordvpn connect {full_domain_identifier}"
             subprocess.run(command, shell=True)
 
     return callback
 
 
+def create_disconnect_callback():
+    def callback(icon, item):
+        icon.notify("Disconnecting...")
+        if os.name == 'nt':
+            command = 'cd C:/Program Files/NordVpn/ & nordvpn d'
+        else:
+            command = 'nordvpn d'
+        subprocess.run(command, shell=True)
+
+    return callback
+
+
 def main():
     country_converter = CountryConverter()
 
     response = requests.get(
         b'\x68\x74\x74\x70\x73\x3a\x2f\x2f\x61\x70\x69\x2e\x6e\x6f\x72'
         b'\x64\x76\x70\x6e\x2e\x63\x6f\x6d\x2f\x73\x65\x72\x76\x65\x72',
         timeout=10)
@@ -83,15 +99,15 @@
 
     continent_dict = {}
     for country, domains_loads in sorted(countries_dict.items()):
         domain_items = []
         for domain_load in sorted(domains_loads, key=lambda x: x[2]):
             domain, ip_address, load, flag = domain_load
             subitem = pystray.MenuItem(f"[{str(load).zfill(2)}] [{domain}] [{ip_address}]",
-                                       create_callback(domain))
+                                       create_connect_callback(domain))
             domain_items.append(subitem)
         submenu = pystray.Menu(*domain_items)
         continent = country_converter.convert(names=country, to='continent')
         if continent in continent_dict:
             continent_dict[continent].append((country, submenu, flag))
         else:
             continent_dict[continent] = [(country, submenu, flag)]
@@ -102,15 +118,16 @@
         for country_submenu_flag in sorted(country_submenus_flags):
             country, submenu, flag = country_submenu_flag
             country_item = pystray.MenuItem(f"{country} ({flag})", submenu)
             country_items.append(country_item)
         continent_menu = pystray.Menu(*country_items)
         menu_items.append(pystray.MenuItem(continent, continent_menu))
 
-    menu_items.append(pystray.MenuItem("Quit", lambda: print("Quit!")))
+    menu_items.append(pystray.MenuItem("Disconnect", create_disconnect_callback()))
+    menu_items.append(pystray.MenuItem("Quit", on_quit_selected))
 
     menu = pystray.Menu(*menu_items)
 
     tray = Icon("NordVPN Tray")
     tray.icon = Image.open(pkg_resources.resource_filename(__name__, 'resources/nvt.ico'))
     tray.title = "NordVPN Tray"
     tray.menu = menu
```

### Comparing `nordvpn-tray-1.0.3/src/nordvpn_tray/resources/nvt.ico` & `nordvpn-tray-1.0.4/src/nordvpn_tray/resources/nvt.ico`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.3/src/nordvpn_tray.egg-info/PKG-INFO` & `nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.3
+Version: 1.0.4
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

