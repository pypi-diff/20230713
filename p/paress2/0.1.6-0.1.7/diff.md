# Comparing `tmp/paress2-0.1.6.tar.gz` & `tmp/paress2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paress2-0.1.6.tar", last modified: Fri Mar 24 02:08:48 2023, max compression
+gzip compressed data, was "paress2-0.1.7.tar", last modified: Thu Jul 13 21:26:47 2023, max compression
```

## Comparing `paress2-0.1.6.tar` & `paress2-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 02:08:48.399322 paress2-0.1.6/
--rw-rw-rw-   0        0        0    35821 2023-03-02 20:17:52.000000 paress2-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     6948 2023-03-24 02:08:48.384769 paress2-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6044 2023-03-24 02:03:00.000000 paress2-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 02:08:48.219563 paress2-0.1.6/paress2/
--rw-rw-rw-   0        0        0      113 2023-03-23 23:36:45.000000 paress2-0.1.6/paress2/__init__.py
--rw-rw-rw-   0        0        0      324 2023-03-24 02:08:40.000000 paress2-0.1.6/paress2/__version__.py
--rw-rw-rw-   0        0        0     2506 2023-03-24 01:47:02.000000 paress2-0.1.6/paress2/browser_checker.py
--rw-rw-rw-   0        0        0    11512 2023-03-24 01:48:28.000000 paress2-0.1.6/paress2/main.py
-drwxrwxrwx   0        0        0        0 2023-03-24 02:08:48.377246 paress2-0.1.6/paress2.egg-info/
--rw-rw-rw-   0        0        0     6948 2023-03-24 02:08:47.000000 paress2-0.1.6/paress2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-03-24 02:08:47.000000 paress2-0.1.6/paress2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 02:08:47.000000 paress2-0.1.6/paress2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-03-24 02:08:47.000000 paress2-0.1.6/paress2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-24 02:08:47.000000 paress2-0.1.6/paress2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 02:08:48.399322 paress2-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-03-23 00:33:24.000000 paress2-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:26:47.595223 paress2-0.1.7/
+-rw-rw-rw-   0        0        0    35821 2023-03-02 20:17:52.000000 paress2-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     7442 2023-07-13 21:26:47.580217 paress2-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6561 2023-07-13 21:12:03.000000 paress2-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 21:26:47.481224 paress2-0.1.7/paress2/
+-rw-rw-rw-   0        0        0      113 2023-03-24 02:18:36.000000 paress2-0.1.7/paress2/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-07-13 21:12:03.000000 paress2-0.1.7/paress2/__version__.py
+-rw-rw-rw-   0        0        0     3815 2023-07-13 21:12:03.000000 paress2-0.1.7/paress2/browser_checker.py
+-rw-rw-rw-   0        0        0    11512 2023-07-13 21:12:47.000000 paress2-0.1.7/paress2/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:26:47.578221 paress2-0.1.7/paress2.egg-info/
+-rw-rw-rw-   0        0        0     7442 2023-07-13 21:26:47.000000 paress2-0.1.7/paress2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-13 21:26:47.000000 paress2-0.1.7/paress2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:26:47.000000 paress2-0.1.7/paress2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-13 21:26:47.000000 paress2-0.1.7/paress2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 21:26:47.000000 paress2-0.1.7/paress2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 21:26:47.596223 paress2-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-03-23 00:33:24.000000 paress2-0.1.7/setup.py
```

### Comparing `paress2-0.1.6/LICENSE` & `paress2-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paress2-0.1.6/PKG-INFO` & `paress2-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: paress2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Paress2 is a Python package for downloading images from the Pares2 website.
 Home-page: https://github.com/jairomelo/paress2
 Author: Jairo Antonio Melo
 Author-email: jairoantoniomelo@gmail.com
 License: GNU General Public License v3.0
 Keywords: python,paress,paress2,pares2.0,archivos históricos,historical files,historical documents,historical images,historical photos,historical pictures
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires: Python (>=3.7)
@@ -28,15 +27,15 @@
 
 Esta librería permite realizar descargas automatizadas de archivos del Portal de Archivos Españoles PARES2.0. Debido a que el portal no cuenta con una API, se ha desarrollado esta librería para realizar un Web Scrapping de la página web del portal.
 
 <hr>
 
 🆕 Una interfaz gráfica βeta para este módulo está disponible en [GUI-archivos-hispanoamericanos](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/tag/v0.1.0-beta). Por lo pronto solamente está disponible para Windows 10 y 11.
 
-Descargar app para Windows: [![Download](https://img.shields.io/badge/Download-0.1.0--beta-blue)](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/download/v0.1.0-beta/main.exe)
+Descargar app para Windows: [![Download](https://img.shields.io/badge/Download-0.1.0--beta-blue)](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/download/v0.1.0-beta/gui_archivos.exe)
 
 <hr>
 
 Esta librería se encuentra en activo desarrollo, por lo que es posible que algún error ya haya sido resuelto en la versión más reciente. Antes de ejecutar el script, se recomienda actualizar la librería a la última versión disponible.
 
 ## Requisitos
 
@@ -78,14 +77,18 @@
 
 ```python
 Paress("http://pares.mcu.es/ParesBusquedas20/catalogo/show/7255960?nm", destino="C:\Users\usuario\descargas\images", velocidad=1).descargar_imagenes()
 ```
 
 A menos que esté en modo headless, se abrirá una ventana de Google Chrome y se iniciará la descarga de las imágenes. El proceso puede tardar varios minutos, dependiendo de la velocidad de conexión a Internet y de la cantidad de imágenes que tenga el legajo.
 
+## Bugs
+
+Si encuentra algún error, por favor, cree un [issue](https://github.com/jairomelo/paress2/issues/new?title=Error&body=descripci%C3%B3n+del+error) en el repositorio de GitHub. Para facilitar la identificación del error incluya el mensaje de error completo que se muestra en la consola, así como el sistema operativo, el navegador instalado (Chrome o Firefox) y la versión de Python que está usando. También puede compartir el número de catálogo del legajo que está intentando descargar.
+
 ## Licencia
 
 [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Para solicitar cambios o reportar errores, por favor, cree un [issue](https://github.com/jairomelo/paress2/issues/new) en el repositorio de GitHub. Para reportar errores por favor compartir el número de catálogo del legajo y el mensaje de error que se muestra en la consola.
@@ -105,9 +108,7 @@
 El registro de cambios se encuentra en el archivo [CHANGELOG.md](CHANGELOG.md)
 
 ## Patrocinio
 
 Este proyecto ha sido elaborado de manera independiente por el autor. Si desea apoyar el desarrollo de este y otros proyectos, puede considerar patrocinarme a través de [GitHub Sponsors](https://github.com/sponsors/jairomelo)
 
 <a href="https://github.com/sponsors/jairomelo" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&link=%3Curl%3E&color=f88379"></a>
-
-
```

### Comparing `paress2-0.1.6/README.md` & `paress2-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Esta librería permite realizar descargas automatizadas de archivos del Portal de Archivos Españoles PARES2.0. Debido a que el portal no cuenta con una API, se ha desarrollado esta librería para realizar un Web Scrapping de la página web del portal.
 
 <hr>
 
 🆕 Una interfaz gráfica βeta para este módulo está disponible en [GUI-archivos-hispanoamericanos](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/tag/v0.1.0-beta). Por lo pronto solamente está disponible para Windows 10 y 11.
 
-Descargar app para Windows: [![Download](https://img.shields.io/badge/Download-0.1.0--beta-blue)](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/download/v0.1.0-beta/main.exe)
+Descargar app para Windows: [![Download](https://img.shields.io/badge/Download-0.1.0--beta-blue)](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/download/v0.1.0-beta/gui_archivos.exe)
 
 <hr>
 
 Esta librería se encuentra en activo desarrollo, por lo que es posible que algún error ya haya sido resuelto en la versión más reciente. Antes de ejecutar el script, se recomienda actualizar la librería a la última versión disponible.
 
 ## Requisitos
 
@@ -58,14 +58,18 @@
 
 ```python
 Paress("http://pares.mcu.es/ParesBusquedas20/catalogo/show/7255960?nm", destino="C:\Users\usuario\descargas\images", velocidad=1).descargar_imagenes()
 ```
 
 A menos que esté en modo headless, se abrirá una ventana de Google Chrome y se iniciará la descarga de las imágenes. El proceso puede tardar varios minutos, dependiendo de la velocidad de conexión a Internet y de la cantidad de imágenes que tenga el legajo.
 
+## Bugs
+
+Si encuentra algún error, por favor, cree un [issue](https://github.com/jairomelo/paress2/issues/new?title=Error&body=descripci%C3%B3n+del+error) en el repositorio de GitHub. Para facilitar la identificación del error incluya el mensaje de error completo que se muestra en la consola, así como el sistema operativo, el navegador instalado (Chrome o Firefox) y la versión de Python que está usando. También puede compartir el número de catálogo del legajo que está intentando descargar.
+
 ## Licencia
 
 [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Para solicitar cambios o reportar errores, por favor, cree un [issue](https://github.com/jairomelo/paress2/issues/new) en el repositorio de GitHub. Para reportar errores por favor compartir el número de catálogo del legajo y el mensaje de error que se muestra en la consola.
```

### Comparing `paress2-0.1.6/paress2/main.py` & `paress2-0.1.7/paress2/main.py`

 * *Files identical despite different names*

### Comparing `paress2-0.1.6/paress2.egg-info/PKG-INFO` & `paress2-0.1.7/paress2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: paress2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Paress2 is a Python package for downloading images from the Pares2 website.
 Home-page: https://github.com/jairomelo/paress2
 Author: Jairo Antonio Melo
 Author-email: jairoantoniomelo@gmail.com
 License: GNU General Public License v3.0
 Keywords: python,paress,paress2,pares2.0,archivos históricos,historical files,historical documents,historical images,historical photos,historical pictures
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires: Python (>=3.7)
@@ -28,15 +27,15 @@
 
 Esta librería permite realizar descargas automatizadas de archivos del Portal de Archivos Españoles PARES2.0. Debido a que el portal no cuenta con una API, se ha desarrollado esta librería para realizar un Web Scrapping de la página web del portal.
 
 <hr>
 
 🆕 Una interfaz gráfica βeta para este módulo está disponible en [GUI-archivos-hispanoamericanos](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/tag/v0.1.0-beta). Por lo pronto solamente está disponible para Windows 10 y 11.
 
-Descargar app para Windows: [![Download](https://img.shields.io/badge/Download-0.1.0--beta-blue)](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/download/v0.1.0-beta/main.exe)
+Descargar app para Windows: [![Download](https://img.shields.io/badge/Download-0.1.0--beta-blue)](https://github.com/jairomelo/GUI-archivos-hispanoamericanos/releases/download/v0.1.0-beta/gui_archivos.exe)
 
 <hr>
 
 Esta librería se encuentra en activo desarrollo, por lo que es posible que algún error ya haya sido resuelto en la versión más reciente. Antes de ejecutar el script, se recomienda actualizar la librería a la última versión disponible.
 
 ## Requisitos
 
@@ -78,14 +77,18 @@
 
 ```python
 Paress("http://pares.mcu.es/ParesBusquedas20/catalogo/show/7255960?nm", destino="C:\Users\usuario\descargas\images", velocidad=1).descargar_imagenes()
 ```
 
 A menos que esté en modo headless, se abrirá una ventana de Google Chrome y se iniciará la descarga de las imágenes. El proceso puede tardar varios minutos, dependiendo de la velocidad de conexión a Internet y de la cantidad de imágenes que tenga el legajo.
 
+## Bugs
+
+Si encuentra algún error, por favor, cree un [issue](https://github.com/jairomelo/paress2/issues/new?title=Error&body=descripci%C3%B3n+del+error) en el repositorio de GitHub. Para facilitar la identificación del error incluya el mensaje de error completo que se muestra en la consola, así como el sistema operativo, el navegador instalado (Chrome o Firefox) y la versión de Python que está usando. También puede compartir el número de catálogo del legajo que está intentando descargar.
+
 ## Licencia
 
 [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Para solicitar cambios o reportar errores, por favor, cree un [issue](https://github.com/jairomelo/paress2/issues/new) en el repositorio de GitHub. Para reportar errores por favor compartir el número de catálogo del legajo y el mensaje de error que se muestra en la consola.
@@ -105,9 +108,7 @@
 El registro de cambios se encuentra en el archivo [CHANGELOG.md](CHANGELOG.md)
 
 ## Patrocinio
 
 Este proyecto ha sido elaborado de manera independiente por el autor. Si desea apoyar el desarrollo de este y otros proyectos, puede considerar patrocinarme a través de [GitHub Sponsors](https://github.com/sponsors/jairomelo)
 
 <a href="https://github.com/sponsors/jairomelo" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&link=%3Curl%3E&color=f88379"></a>
-
-
```

### Comparing `paress2-0.1.6/setup.py` & `paress2-0.1.7/setup.py`

 * *Files identical despite different names*

