# Comparing `tmp/metalmaps-2.0.0.tar.gz` & `tmp/metalmaps-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalmaps-2.0.0.tar", last modified: Tue Jul 11 18:11:05 2023, max compression
+gzip compressed data, was "metalmaps-2.1.0.tar", last modified: Thu Jul 13 16:26:39 2023, max compression
```

## Comparing `metalmaps-2.0.0.tar` & `metalmaps-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:11:05.254760 metalmaps-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-11 18:10:55.000000 metalmaps-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 18:10:55.000000 metalmaps-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-07-11 18:11:05.254760 metalmaps-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-11 18:10:55.000000 metalmaps-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:11:05.254760 metalmaps-2.0.0/metalmaps/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/colorcycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/make_cmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:11:05.254760 metalmaps-2.0.0/metalmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-11 18:10:55.000000 metalmaps-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:11:05.254760 metalmaps-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:26:39.534991 metalmaps-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-13 16:26:29.000000 metalmaps-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 16:26:29.000000 metalmaps-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-07-13 16:26:39.534991 metalmaps-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-13 16:26:29.000000 metalmaps-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:26:39.530991 metalmaps-2.1.0/metalmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-13 16:26:29.000000 metalmaps-2.1.0/metalmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:26:29.000000 metalmaps-2.1.0/metalmaps/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-13 16:26:29.000000 metalmaps-2.1.0/metalmaps/colorcycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-13 16:26:29.000000 metalmaps-2.1.0/metalmaps/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 16:26:29.000000 metalmaps-2.1.0/metalmaps/make_cmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:26:39.534991 metalmaps-2.1.0/metalmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-07-13 16:26:39.000000 metalmaps-2.1.0/metalmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-13 16:26:39.000000 metalmaps-2.1.0/metalmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:26:39.000000 metalmaps-2.1.0/metalmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 16:26:39.000000 metalmaps-2.1.0/metalmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 16:26:39.000000 metalmaps-2.1.0/metalmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-13 16:26:29.000000 metalmaps-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:26:39.534991 metalmaps-2.1.0/setup.cfg
```

### Comparing `metalmaps-2.0.0/LICENSE.txt` & `metalmaps-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metalmaps-2.0.0/PKG-INFO` & `metalmaps-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalmaps
-Version: 2.0.0
+Version: 2.1.0
 Summary: Metal and rock inspired Matplotlib colormaps.
 Author-email: Mladen Ivkovic <mladen.ivkovic@hotmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -260,15 +260,15 @@
 x = np.linspace(0, 1.4, 200)
 def y(x, phi):
     return np.sin(1.2 * np.pi * (x + 0.25) - 0.1 * phi)
 
 plt.figure()
 
 for i in range(10):
-    labelname = label="C"+str(i)
+    labelname = "C"+str(i)
     plt.plot(x, y(x, i), linewidth=5, label=labelname)
 
 plt.legend(ncols=2)
 plt.tight_layout()
 plt.savefig("my_figure.png")
 
 ```
@@ -289,38 +289,41 @@
 
 Examples
 --------
 
 This package currently includes 30 colormaps: 
 
 
++   Animals (Pink Floyd)
 +   The Apostasy (Behemoth)
 +   Ashes of the Wake (Lamb of God)
 +   Black Sabbath (Black Sabbath)
 +   The Blues Brothers (The Blues Brothers)
 +   Blues Pills (Blues Pills)
 +   Cosmo's Factory (Creedence Clearwater Revival)
 +   Deep Purple in Rock (Deep Purple)
 +   The Dethalbum (Dethklok)
 +   Fear of the Dark (Iron Maiden)
 +   From Mars to Sirius (Gojira)
++   Hybrid Theory (Linkin Park)
 +   Hypnotize (System of a Down)
 +   In Utero (Nirvana)
 +   L.A. Woman (The Doors)
 +   L'enfant Sauvage (Gojira)
 +   London Calling (The Clash)
 +   Master of Puppets (Metallica)
 +   Made in Japan (Deep Purple)
 +   Meteora (Linkin Park)
 +   The Number of the Beast (Iron Maiden)
 +   obZen (Meshuggah)
 +   Overkill (Motörhead)
 +   Painkiller (Judas Priest)
 +   Paranoid (Black Sabbath)
 +   Powerslave (Iron Maiden)
++   Rage Against The Machine (Rage Against The Machine)
 +   Reign in Blood (Slayer)
 +   Ride the Lightning (Metallica)
 +   Rock 'n' Roll (Motörhead)
 +   Screaming for Vengeance (Judas Priest)
 +   South of Heaven (Slayer)
 +   The Hunter (Mastodon)
 +   The Rise and Fall of Ziggy Stardust and the Spiders From Mars (David Bowie)
```

### Comparing `metalmaps-2.0.0/README.md` & `metalmaps-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 x = np.linspace(0, 1.4, 200)
 def y(x, phi):
     return np.sin(1.2 * np.pi * (x + 0.25) - 0.1 * phi)
 
 plt.figure()
 
 for i in range(10):
-    labelname = label="C"+str(i)
+    labelname = "C"+str(i)
     plt.plot(x, y(x, i), linewidth=5, label=labelname)
 
 plt.legend(ncols=2)
 plt.tight_layout()
 plt.savefig("my_figure.png")
 
 ```
@@ -109,38 +109,41 @@
 
 Examples
 --------
 
 This package currently includes 30 colormaps: 
 
 
++   Animals (Pink Floyd)
 +   The Apostasy (Behemoth)
 +   Ashes of the Wake (Lamb of God)
 +   Black Sabbath (Black Sabbath)
 +   The Blues Brothers (The Blues Brothers)
 +   Blues Pills (Blues Pills)
 +   Cosmo's Factory (Creedence Clearwater Revival)
 +   Deep Purple in Rock (Deep Purple)
 +   The Dethalbum (Dethklok)
 +   Fear of the Dark (Iron Maiden)
 +   From Mars to Sirius (Gojira)
++   Hybrid Theory (Linkin Park)
 +   Hypnotize (System of a Down)
 +   In Utero (Nirvana)
 +   L.A. Woman (The Doors)
 +   L'enfant Sauvage (Gojira)
 +   London Calling (The Clash)
 +   Master of Puppets (Metallica)
 +   Made in Japan (Deep Purple)
 +   Meteora (Linkin Park)
 +   The Number of the Beast (Iron Maiden)
 +   obZen (Meshuggah)
 +   Overkill (Motörhead)
 +   Painkiller (Judas Priest)
 +   Paranoid (Black Sabbath)
 +   Powerslave (Iron Maiden)
++   Rage Against The Machine (Rage Against The Machine)
 +   Reign in Blood (Slayer)
 +   Ride the Lightning (Metallica)
 +   Rock 'n' Roll (Motörhead)
 +   Screaming for Vengeance (Judas Priest)
 +   South of Heaven (Slayer)
 +   The Hunter (Mastodon)
 +   The Rise and Fall of Ziggy Stardust and the Spiders From Mars (David Bowie)
```

### Comparing `metalmaps-2.0.0/metalmaps/__init__.py` & `metalmaps-2.1.0/metalmaps/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """
 Heavy Metal and Classic Rock color map collection.
 
 Includes color maps based on the following albums:
 
++   Animals (Pink Floyd)
 +   The Apostasy (Behemoth)
 +   Ashes of the Wake (Lamb of God)
 +   Black Sabbath (Black Sabbath)
 +   The Blues Brothers (The Blues Brothers)
 +   Blues Pills (Blues Pills)
 +   Cosmo's Factory (Creedence Clearwater Revival)
 +   Deep Purple in Rock (Deep Purple)
 +   The Dethalbum (Dethklok)
 +   Fear of the Dark (Iron Maiden)
 +   From Mars to Sirius (Gojira)
++   Hybrid Theory (Linkin Park)
 +   Hypnotize (System of a Down)
 +   In Utero (Nirvana)
 +   L.A. Woman (The Doors)
 +   L'enfant Sauvage (Gojira)
 +   London Calling (The Clash)
 +   Master of Puppets (Metallica)
 +   Made in Japan (Deep Purple)
 +   Meteora (Linkin Park)
 +   The Number of the Beast (Iron Maiden)
 +   obZen (Meshuggah)
 +   Overkill (Motörhead)
 +   Painkiller (Judas Priest)
 +   Paranoid (Black Sabbath)
 +   Powerslave (Iron Maiden)
++   Rage Against The Machine (Rage Against The Machine)
 +   Reign in Blood (Slayer)
 +   Ride the Lightning (Metallica)
 +   Rock 'n' Roll (Motörhead)
 +   Screaming for Vengeance (Judas Priest)
 +   South of Heaven (Slayer)
 +   The Hunter (Mastodon)
 +   The Rise and Fall of Ziggy Stardust and the Spiders From Mars (David Bowie)
@@ -57,14 +60,15 @@
 """
 
 import metalmaps.colors as colors
 from metalmaps.make_cmap import make_custom_cmap
 from metalmaps.colorcycle import set_color_cycle
 from metalmaps.__version__ import __version__
 
+animals, animals_r = make_custom_cmap("animals", colors.animals)
 apostasy, apostasy_r = make_custom_cmap("apostasy", colors.apostasy)
 ashes_of_the_wake, ashes_of_the_wake_r = make_custom_cmap(
     "ashes_of_the_wake", colors.ashes_of_the_wake
 )
 blues_brothers, blues_brothers_r = make_custom_cmap(
     "blues_brothers", colors.blues_brothers
 )
@@ -79,14 +83,15 @@
 dethalbum, dethalbum_r = make_custom_cmap("dethalbum", colors.dethalbum)
 fear_of_the_dark, fear_of_the_dark_r = make_custom_cmap(
     "fear_of_the_dark", colors.fear_of_the_dark
 )
 from_mars_to_sirius, from_mars_to_sirius_r = make_custom_cmap(
     "from_mars_to_sirius", colors.from_mars_to_sirius
 )
+hybrid_theory, hybrid_theory_r = make_custom_cmap("hybrid_theory", colors.hybrid_theory)
 hypnotize, hypnotize_r = make_custom_cmap("hypnotize", colors.hypnotize)
 in_utero, in_utero_r = make_custom_cmap("in_utero", colors.in_utero)
 la_woman, la_woman_r = make_custom_cmap("la_woman", colors.la_woman)
 lenfant_sauvage, lenfant_sauvage_r = make_custom_cmap(
     "lenfant_sauvage", colors.lenfant_sauvage
 )
 london_calling, london_calling_r = make_custom_cmap(
@@ -101,14 +106,17 @@
     "number_of_the_beast", colors.number_of_the_beast
 )
 obzen, obzen_r = make_custom_cmap("obzen", colors.obzen)
 overkill, overkill_r = make_custom_cmap("overkill", colors.overkill)
 paranoid, paranoid_r = make_custom_cmap("paranoid", colors.paranoid)
 painkiller, painkiller_r = make_custom_cmap("painkiller", colors.painkiller)
 powerslave, powerslave_r = make_custom_cmap("powerslave", colors.powerslave)
+rage_against_the_machine, rage_against_the_machine_r = make_custom_cmap(
+    "rage_against_the_machine", colors.rage_against_the_machine
+)
 reign_in_blood, reign_in_blood_r = make_custom_cmap(
     "reign_in_blood", colors.reign_in_blood
 )
 ride_the_lightning, ride_the_lightning = make_custom_cmap(
     "ride_the_lightning", colors.ride_the_lightning
 )
 rock_n_roll, rock_n_roll_r = make_custom_cmap("rock_n_roll", colors.rock_n_roll)
```

### Comparing `metalmaps-2.0.0/metalmaps/colorcycle.py` & `metalmaps-2.1.0/metalmaps/colorcycle.py`

 * *Files identical despite different names*

### Comparing `metalmaps-2.0.0/metalmaps/colors.py` & `metalmaps-2.1.0/metalmaps/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 """
 Colors (defined as RGB values) for the albums.
 """
 
 from metalmaps.make_cmap import hex_to_rgb
 
+animals = hex_to_rgb(
+    [
+        "#2A2722",
+        "#3A3736",
+        "#56575D",
+        "#707386",
+        "#808689",
+        "#AAAE94",
+        "#CDCA94",
+        "#DDC681",
+        "#CF895D",
+        "#E67B67",
+    ]
+)
+
 apostasy = hex_to_rgb(
     [
         "#010508",
         "#051217",
         "#18313C",
         "#37505A",
         "#47636B",
@@ -135,14 +150,29 @@
         "#AA968B",
         "#C5BBAC",
         "#A09689",
         "#110E0A",
     ]
 )
 
+hybrid_theory = hex_to_rgb(
+    [
+        "#4A474E",
+        "#4F4D56",
+        "#5E4D54",
+        "#805A61",
+        "#87565F",
+        "#8F8E92",
+        "#9E999E",
+        "#AAA3A8",
+        "#CAC4C7",
+        "#DFDFE4",
+    ]
+)
+
 hypnotize = hex_to_rgb(
     [
         "#1D2328",
         "#252E33",
         "#372930",
         "#48292E",
         "#7B1815",
@@ -312,25 +342,26 @@
         "#F59C47",
         "#9B8C5E",
         "#A96546",
         "#DBC3BD",
     ]
 )
 
-ride_the_lightning = hex_to_rgb(
+rage_against_the_machine = hex_to_rgb(
     [
-        "#27233D",
-        "#151040",
-        "#22206C",
-        "#423D74",
-        "#5E5E89",
-        "#869ACC",
-        "#298CF1",
-        "#82C7F6",
-        "#EFF1F7",
+        "#060F0D",
+        "#3B4F43",
+        "#5A6757",
+        "#647762",
+        "#9AA48E",
+        "#ABB79F",
+        "#B9C4B2",
+        "#DEE7D6",
+        "#ECF1E0",
+        "#F6F9E9",
     ]
 )
 
 reign_in_blood = hex_to_rgb(
     [
         "#1C1D17",
         "#222115",
@@ -341,14 +372,28 @@
         "#856B38",
         "#BB942E",
         "#943423",
         "#BC3823",
     ]
 )
 
+ride_the_lightning = hex_to_rgb(
+    [
+        "#27233D",
+        "#151040",
+        "#22206C",
+        "#423D74",
+        "#5E5E89",
+        "#869ACC",
+        "#298CF1",
+        "#82C7F6",
+        "#EFF1F7",
+    ]
+)
+
 rock_n_roll = hex_to_rgb(
     [
         "#20202A",
         "#25252F",
         "#2F2E40",
         "#353444",
         "#3D4260",
```

### Comparing `metalmaps-2.0.0/metalmaps/make_cmap.py` & `metalmaps-2.1.0/metalmaps/make_cmap.py`

 * *Files identical despite different names*

### Comparing `metalmaps-2.0.0/metalmaps.egg-info/PKG-INFO` & `metalmaps-2.1.0/metalmaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalmaps
-Version: 2.0.0
+Version: 2.1.0
 Summary: Metal and rock inspired Matplotlib colormaps.
 Author-email: Mladen Ivkovic <mladen.ivkovic@hotmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -260,15 +260,15 @@
 x = np.linspace(0, 1.4, 200)
 def y(x, phi):
     return np.sin(1.2 * np.pi * (x + 0.25) - 0.1 * phi)
 
 plt.figure()
 
 for i in range(10):
-    labelname = label="C"+str(i)
+    labelname = "C"+str(i)
     plt.plot(x, y(x, i), linewidth=5, label=labelname)
 
 plt.legend(ncols=2)
 plt.tight_layout()
 plt.savefig("my_figure.png")
 
 ```
@@ -289,38 +289,41 @@
 
 Examples
 --------
 
 This package currently includes 30 colormaps: 
 
 
++   Animals (Pink Floyd)
 +   The Apostasy (Behemoth)
 +   Ashes of the Wake (Lamb of God)
 +   Black Sabbath (Black Sabbath)
 +   The Blues Brothers (The Blues Brothers)
 +   Blues Pills (Blues Pills)
 +   Cosmo's Factory (Creedence Clearwater Revival)
 +   Deep Purple in Rock (Deep Purple)
 +   The Dethalbum (Dethklok)
 +   Fear of the Dark (Iron Maiden)
 +   From Mars to Sirius (Gojira)
++   Hybrid Theory (Linkin Park)
 +   Hypnotize (System of a Down)
 +   In Utero (Nirvana)
 +   L.A. Woman (The Doors)
 +   L'enfant Sauvage (Gojira)
 +   London Calling (The Clash)
 +   Master of Puppets (Metallica)
 +   Made in Japan (Deep Purple)
 +   Meteora (Linkin Park)
 +   The Number of the Beast (Iron Maiden)
 +   obZen (Meshuggah)
 +   Overkill (Motörhead)
 +   Painkiller (Judas Priest)
 +   Paranoid (Black Sabbath)
 +   Powerslave (Iron Maiden)
++   Rage Against The Machine (Rage Against The Machine)
 +   Reign in Blood (Slayer)
 +   Ride the Lightning (Metallica)
 +   Rock 'n' Roll (Motörhead)
 +   Screaming for Vengeance (Judas Priest)
 +   South of Heaven (Slayer)
 +   The Hunter (Mastodon)
 +   The Rise and Fall of Ziggy Stardust and the Spiders From Mars (David Bowie)
```

### Comparing `metalmaps-2.0.0/pyproject.toml` & `metalmaps-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools]
 packages = ["metalmaps"]
 
 [project]
 name = "metalmaps"
 description="Metal and rock inspired Matplotlib colormaps."
 readme = "README.md"
-version = "2.0.0"
+version = "2.1.0"
 authors= [
     { name = "Mladen Ivkovic", email="mladen.ivkovic@hotmail.com"},
     ]
 license = { file = "LICENSE.txt" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -25,15 +25,15 @@
 
 
 [project.urls]
 "Homepage" = "https://github.com/mladenivkovic/metalmaps"
 "Gallery" = "https://mladenivkovic.github.io/metalmaps/metalmaps.html"
 
 [tool.bumpver]
-current_version = "2.0.0"
+current_version = "2.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

