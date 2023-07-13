# Comparing `tmp/nordvpn-tray-1.0.4.tar.gz` & `tmp/nordvpn-tray-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordvpn-tray-1.0.4.tar", last modified: Thu Jul 13 12:48:27 2023, max compression
+gzip compressed data, was "nordvpn-tray-1.0.5.tar", last modified: Thu Jul 13 19:10:23 2023, max compression
```

## Comparing `nordvpn-tray-1.0.4.tar` & `nordvpn-tray-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.102218 nordvpn-tray-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4702 2023-07-13 12:48:27.096295 nordvpn-tray-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3748 2023-07-11 22:24:38.000000 nordvpn-tray-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 12:48:27.102218 nordvpn-tray-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2530 2023-07-13 12:47:59.000000 nordvpn-tray-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.057839 nordvpn-tray-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.069840 nordvpn-tray-1.0.4/src/nordvpn_tray/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.4/src/nordvpn_tray/__init__.py
--rw-rw-rw-   0        0        0     5374 2023-07-13 09:27:53.000000 nordvpn-tray-1.0.4/src/nordvpn_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.093295 nordvpn-tray-1.0.4/src/nordvpn_tray/resources/
--rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.4/src/nordvpn_tray/resources/nvt.ico
-drwxrwxrwx   0        0        0        0 2023-07-13 12:48:27.091295 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/
--rw-rw-rw-   0        0        0     4702 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-13 12:48:27.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 12:48:26.000000 nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 19:10:23.217444 nordvpn-tray-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4733 2023-07-13 19:10:23.209444 nordvpn-tray-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2023-07-13 18:57:15.000000 nordvpn-tray-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 19:10:23.217444 nordvpn-tray-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2530 2023-07-13 16:26:07.000000 nordvpn-tray-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:10:23.164441 nordvpn-tray-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 19:10:23.179441 nordvpn-tray-1.0.5/src/nordvpn_tray/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.5/src/nordvpn_tray/__init__.py
+-rw-rw-rw-   0        0        0     6342 2023-07-13 18:59:04.000000 nordvpn-tray-1.0.5/src/nordvpn_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:10:23.205445 nordvpn-tray-1.0.5/src/nordvpn_tray/resources/
+-rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.5/src/nordvpn_tray/resources/nvt.ico
+drwxrwxrwx   0        0        0        0 2023-07-13 19:10:23.203443 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/
+-rw-rw-rw-   0        0        0     4733 2023-07-13 19:10:23.000000 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-13 19:10:23.000000 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 19:10:23.000000 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-13 19:10:23.000000 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-13 19:10:23.000000 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 19:10:23.000000 nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/top_level.txt
```

### Comparing `nordvpn-tray-1.0.4/LICENSE` & `nordvpn-tray-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.4/PKG-INFO` & `nordvpn-tray-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.4
+Version: 1.0.5
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
@@ -38,15 +38,15 @@
 
 To address these limitations, the current project introduces a solution in the form of a system tray application. By placing an icon in the system tray, users can easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized by continents and countries, allowing for effortless navigation. Moreover, the servers are ordered by their load, enabling users to select the server with the lowest load for optimal performance.
 
 With just a few clicks, users can now connect to their desired server directly from the system tray, bypassing the restrictions and limitations present in the official NordVPN clients. 
 
 ## Preview
 
-![pr](https://github.com/aviolaris/nordvpn-tray/assets/48277853/c0075f44-9838-40a2-a478-16a83dbeb8db)
+<img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
 - Python 3.6 or higher
 
 ## Installation
```

### Comparing `nordvpn-tray-1.0.4/README.md` & `nordvpn-tray-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 To address these limitations, the current project introduces a solution in the form of a system tray application. By placing an icon in the system tray, users can easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized by continents and countries, allowing for effortless navigation. Moreover, the servers are ordered by their load, enabling users to select the server with the lowest load for optimal performance.
 
 With just a few clicks, users can now connect to their desired server directly from the system tray, bypassing the restrictions and limitations present in the official NordVPN clients. 
 
 ## Preview
 
-![pr](https://github.com/aviolaris/nordvpn-tray/assets/48277853/c0075f44-9838-40a2-a478-16a83dbeb8db)
+<img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
 - Python 3.6 or higher
 
 ## Installation
```

### Comparing `nordvpn-tray-1.0.4/setup.py` & `nordvpn-tray-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='nordvpn-tray',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "nordvpn_tray": ["*.py"],
         "nordvpn_tray.resources": ["*.ico"],
     },
     description='A cross-platform system tray application for interacting with NordVPN.',
```

### Comparing `nordvpn-tray-1.0.4/src/nordvpn_tray/__main__.py` & `nordvpn-tray-1.0.5/src/nordvpn_tray/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,75 +12,94 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <https://www.gnu.org/licenses/>.
 """
 import os
-import subprocess
 import re
+import subprocess
+from country_converter import CountryConverter
+from PIL import Image
 import pkg_resources
 import pystray
-import requests
 from pystray import Icon
-from PIL import Image
-from country_converter import CountryConverter
+import requests
 
 
 def get_full_domain_identifier(short_domain_identifier):
     country_converter = CountryConverter()
     country_code = short_domain_identifier[:2].upper()
     country_name = country_converter.convert(names=country_code, to='name_short')
     if country_name:
         return f"{country_name} #{short_domain_identifier[2:]}"
     else:
         return "Invalid country code"
 
 
-def on_quit_selected(icon, item):
+def quit(icon, item):
     icon.stop()
 
 
+def is_nordvpn_connected():
+    user_info_data = requests.get(
+        b'\x68\x74\x74\x70\x73\x3a\x2f\x2f\x6e\x6f\x72\x64\x76\x70\x6e\x2e\x63\x6f'
+        b'\x6d\x2f\x77\x70\x2d\x61\x64\x6d\x69\x6e\x2f\x61\x64\x6d\x69\x6e\x2d\x61'
+        b'\x6a\x61\x78\x2e\x70\x68\x70\x3f\x61\x63\x74\x69\x6f\x6e\x3d\x67\x65\x74'
+        b'\x5f\x75\x73\x65\x72\x5f\x69\x6e\x66\x6f\x5f\x64\x61\x74\x61',
+        timeout=10)
+    if user_info_data.status_code == 200:
+        data = user_info_data.json()
+        return data.get('status', False)
+    return False
+
+
 def create_connect_callback(domain):
     def callback(icon, domain):
-        icon.notify(str(domain))
         domain_identifier = re.search(r"\[(\w+)\.nordvpn\.com]", str(domain)).group(1)
         full_domain_identifier = get_full_domain_identifier(domain_identifier)
         if domain_identifier:
-            if os.name == 'nt':
-                command = f'cd C:/Program Files/NordVpn/ & nordvpn -c -n "{full_domain_identifier}"'
+            if is_nordvpn_connected():
+                icon.notify("Already connected to a NordVPN server.")
             else:
-                command = f"nordvpn connect {full_domain_identifier}"
-            subprocess.run(command, shell=True)
+                icon.notify(str(domain))
+                if os.name == 'nt':
+                    command = f'cd C:/Program Files/NordVpn/ & nordvpn -c -n "{full_domain_identifier}"'
+                else:
+                    command = f"nordvpn connect {full_domain_identifier}"
+                subprocess.run(command, shell=True)
 
     return callback
 
 
 def create_disconnect_callback():
     def callback(icon, item):
-        icon.notify("Disconnecting...")
-        if os.name == 'nt':
-            command = 'cd C:/Program Files/NordVpn/ & nordvpn d'
+        if is_nordvpn_connected():
+            icon.notify("Disconnecting...")
+            if os.name == 'nt':
+                command = 'cd C:/Program Files/NordVpn/ & nordvpn -d'
+            else:
+                command = 'nordvpn d'
+            subprocess.run(command, shell=True)
         else:
-            command = 'nordvpn d'
-        subprocess.run(command, shell=True)
+            icon.notify("You are not connected to a NordVPN server.")
 
     return callback
 
 
 def main():
     country_converter = CountryConverter()
 
-    response = requests.get(
+    nord_api = requests.get(
         b'\x68\x74\x74\x70\x73\x3a\x2f\x2f\x61\x70\x69\x2e\x6e\x6f\x72'
         b'\x64\x76\x70\x6e\x2e\x63\x6f\x6d\x2f\x73\x65\x72\x76\x65\x72',
         timeout=10)
 
-    if response.status_code == 200:
-        servers = response.json()
+    if nord_api.status_code == 200:
+        servers = nord_api.json()
         countries_dict = {}
         for server in servers:
             country = server['country']
             flag = server['flag']
             domain = server['domain']
             ip_address = server['ip_address']
             load = server['load']
@@ -91,15 +110,15 @@
                     countries_dict['United States'] = [(domain, ip_address, load, flag)]
             else:
                 if country in countries_dict:
                     countries_dict[country].append((domain, ip_address, load, flag))
                 else:
                     countries_dict[country] = [(domain, ip_address, load, flag)]
     else:
-        print(f"Failed to fetch data, status code: {response.status_code}")
+        print(f"Failed to fetch data, status code: {nord_api.status_code}")
 
     continent_dict = {}
     for country, domains_loads in sorted(countries_dict.items()):
         domain_items = []
         for domain_load in sorted(domains_loads, key=lambda x: x[2]):
             domain, ip_address, load, flag = domain_load
             subitem = pystray.MenuItem(f"[{str(load).zfill(2)}] [{domain}] [{ip_address}]",
@@ -118,16 +137,18 @@
         for country_submenu_flag in sorted(country_submenus_flags):
             country, submenu, flag = country_submenu_flag
             country_item = pystray.MenuItem(f"{country} ({flag})", submenu)
             country_items.append(country_item)
         continent_menu = pystray.Menu(*country_items)
         menu_items.append(pystray.MenuItem(continent, continent_menu))
 
+    menu_items.append(pystray.MenuItem('- - - -', None))
+    menu_items.append(pystray.Menu.SEPARATOR)  # Add separator here
     menu_items.append(pystray.MenuItem("Disconnect", create_disconnect_callback()))
-    menu_items.append(pystray.MenuItem("Quit", on_quit_selected))
+    menu_items.append(pystray.MenuItem("Quit", quit))
 
     menu = pystray.Menu(*menu_items)
 
     tray = Icon("NordVPN Tray")
     tray.icon = Image.open(pkg_resources.resource_filename(__name__, 'resources/nvt.ico'))
     tray.title = "NordVPN Tray"
     tray.menu = menu
```

### Comparing `nordvpn-tray-1.0.4/src/nordvpn_tray/resources/nvt.ico` & `nordvpn-tray-1.0.5/src/nordvpn_tray/resources/nvt.ico`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.4/src/nordvpn_tray.egg-info/PKG-INFO` & `nordvpn-tray-1.0.5/src/nordvpn_tray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.4
+Version: 1.0.5
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
@@ -38,15 +38,15 @@
 
 To address these limitations, the current project introduces a solution in the form of a system tray application. By placing an icon in the system tray, users can easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized by continents and countries, allowing for effortless navigation. Moreover, the servers are ordered by their load, enabling users to select the server with the lowest load for optimal performance.
 
 With just a few clicks, users can now connect to their desired server directly from the system tray, bypassing the restrictions and limitations present in the official NordVPN clients. 
 
 ## Preview
 
-![pr](https://github.com/aviolaris/nordvpn-tray/assets/48277853/c0075f44-9838-40a2-a478-16a83dbeb8db)
+<img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
 - Python 3.6 or higher
 
 ## Installation
```

