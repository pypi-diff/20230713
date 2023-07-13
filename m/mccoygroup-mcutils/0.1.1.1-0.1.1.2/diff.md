# Comparing `tmp/mccoygroup-mcutils-0.1.1.1.tar.gz` & `tmp/mccoygroup-mcutils-0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccoygroup-mcutils-0.1.1.1.tar", last modified: Tue Jul 11 18:52:59 2023, max compression
+gzip compressed data, was "mccoygroup-mcutils-0.1.1.2.tar", last modified: Thu Jul 13 20:33:32 2023, max compression
```

## Comparing `mccoygroup-mcutils-0.1.1.1.tar` & `mccoygroup-mcutils-0.1.1.2.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/
--rw-r--r--   0 runner    (1001) docker     (123)   166453 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/Conveniences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14789 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13283 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6157 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26533 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12958 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/DefaultConverters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8885 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3640 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1573 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.219823 mccoygroup-mcutils-0.1.1.1/McUtils/Data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/AtomData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/BondData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7160 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/CommonData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15316 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/ConstantsData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/PotentialData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7767 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/QuantityArray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/
--rwxr-xr-x   0 runner    (1001) docker     (123)   114295 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/AtomData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13861 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/BondData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61435 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/WavefunctionData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38079 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocsBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/ExamplesParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/MarkdownTemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16442 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ArgumentSignature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15111 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/CLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Module.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4699 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ModuleLoader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7145 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/SharedLibraryManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/Babel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/OpenChem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7680 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/FChkDerivatives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5261 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13822 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianImporter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23349 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianLogComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.223823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/InteractiveTools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/ActiveHTMLWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.227823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   322229 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js
--rw-r--r--   0 runner    (1001) docker     (123)    43040 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js
--rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)   299473 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js
--rw-r--r--   0 runner    (1001) docker     (123)   289256 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.231823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)   750963 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2514969 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.231823 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    52345 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    41729 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTML.py
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HackWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/JHTML.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/WidgetTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/MoleculeGraphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/NBExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/DebugTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/FileMatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/NumbaTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/SBatchHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)    28255 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Symbolics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateWriter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38376 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/AnalyticDerivs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3743 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/EulerSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/SetOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    95985 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Sparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7552 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationMatrices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationTransformations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/VectorOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/
--rw-r--r--   0 runner    (1001) docker     (123)    58677 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Parallelizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/SharedMemory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.235823 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/FileStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/Parsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36223 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/RegexPatterns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43416 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StringParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48561 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StructuredType.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Backends.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    71035 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12351 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Interactive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45079 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29775 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Properties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9360 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Styling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19806 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/VTKInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/CLIs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Caches.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Checkpointing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21633 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/ObjectBackers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6989 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/FittableModels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19361 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Interpolator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/LazyTensors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    81351 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/NeighborBasedInterpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19119 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Polynomials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7602 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/BaseSurface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/Surface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)    64296 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)    73503 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30417 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/Derivatives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34945 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19721 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5570 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.239823 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/McUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-11 18:52:59.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 18:52:58.000000 mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:52:59.243823 mccoygroup-mcutils-0.1.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-07-11 18:52:48.000000 mccoygroup-mcutils-0.1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.413212 mccoygroup-mcutils-0.1.1.2/McUtils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.417212 mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/
+-rw-r--r--   0 runner    (1001) docker     (123)   166453 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/Permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/Sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.417212 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/Conveniences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.421212 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14789 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13283 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6157 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26533 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12958 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/DefaultConverters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8885 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.421212 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3640 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1573 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.425212 mccoygroup-mcutils-0.1.1.2/McUtils/Data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/AtomData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/BondData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7160 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/CommonData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15316 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/ConstantsData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/PotentialData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7767 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/QuantityArray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.425212 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114295 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/AtomData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13861 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/BondData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61435 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/ConstantsData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/PotentialData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/WavefunctionData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/WavefunctionData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/Docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38079 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Docs/DocWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Docs/DocsBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Docs/ExamplesParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Docs/MarkdownTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16442 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/ArgumentSignature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15111 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/CLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/DynamicFFILibrary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/Module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4699 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/ModuleLoader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7145 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/SharedLibraryManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/ExternalPrograms/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/ExternalPrograms/Babel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/ExternalPrograms/OpenChem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/ExternalPrograms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7680 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/FChkDerivatives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5261 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianFChkComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13822 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianImporter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23349 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianLogComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/InteractiveTools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.429212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.433212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/ActiveHTMLWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.433212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.433212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   322229 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43040 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)   299473 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js
+-rw-r--r--   0 runner    (1001) docker     (123)   289256 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.433212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)   750963 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2514969 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.437212 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/Bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52345 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/BootstrapEnums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/BootstrapWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41729 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/HTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/HTMLWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/HackWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/JHTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/WidgetTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/MoleculeGraphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/NBExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.437212 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/DebugTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/Decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/FileMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/NumbaTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/SBatchHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/Singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28255 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/Symbolics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.437212 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateEngine/
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateEngine/ObjectWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateEngine/TemplateEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateEngine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateWriter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.437212 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38376 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/AnalyticDerivs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3743 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/EulerSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/Misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/Options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/SetOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    95985 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/Sparse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7552 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/TransformationMatrices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/TransformationTransformations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/VectorOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.437212 mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    58677 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/Parallelizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/SharedMemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.441212 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/FileStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/Parsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36223 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/RegexPatterns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43416 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/StringParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48561 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/StructuredType.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.441212 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Backends.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71035 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12351 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Interactive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45079 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29775 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9360 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Styling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19806 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/VTKInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.441212 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/CLIs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Checkpointing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21633 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/ObjectBackers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.441212 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6989 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/FittableModels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19361 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Interpolator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/LazyTensors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81351 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/NeighborBasedInterpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19119 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Polynomials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.441212 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7602 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/BaseSurface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/Surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.441212 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)    64296 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/ElementaryFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73503 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/TensorExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30417 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/Derivatives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34945 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19721 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/FunctionExpansions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5570 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/src/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/McUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-13 20:33:32.000000 mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-13 20:33:32.000000 mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:33:32.000000 mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 20:33:32.000000 mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 20:33:32.000000 mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:33:32.445212 mccoygroup-mcutils-0.1.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-07-13 20:33:22.000000 mccoygroup-mcutils-0.1.1.2/setup.py
```

### Comparing `mccoygroup-mcutils-0.1.1.1/LICENSE.txt` & `mccoygroup-mcutils-0.1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/MANIFEST.in` & `mccoygroup-mcutils-0.1.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Permutations.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/Permutations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/Sequences.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/Sequences.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Combinatorics/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Combinatorics/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/Conveniences.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/Conveniences.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateSystems/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/CoordinateTransformations/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Coordinerds/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Coordinerds/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/AtomData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/AtomData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/BondData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/BondData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/CommonData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/CommonData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/ConstantsData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/ConstantsData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/PotentialData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/PotentialData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/QuantityArray.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/QuantityArray.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/AtomData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/AtomData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/BondData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/BondData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/ConstantsData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/PotentialData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/TheRealMcCoy/WavefunctionData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/WavefunctionData.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/WavefunctionData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Data/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocWalker.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Docs/DocWalker.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/DocsBuilder.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Docs/DocsBuilder.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/ExamplesParser.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Docs/ExamplesParser.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Docs/MarkdownTemplates.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Docs/MarkdownTemplates.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ArgumentSignature.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/ArgumentSignature.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/CLoader.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/CLoader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/DynamicFFILibrary.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Loader.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/Loader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/FFI/Module.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/FFI/Module.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 __all__ = [
     "FFIModule",
     "FFIMethod",
     "FFIArgument",
     "FFIType"
 ]
 
+try: # guard clause
+    np_float128 = np.float128
+except AttributeError:
+    np_float128 = np.longdouble # bad vibes but we'll see what happens
+
 class FFIType(enum.Enum):
     """
     The set of supported enum types.
     Maps onto the native python convertable types and NumPy dtypes.
     In the future, this should be done more elegantly, but for now it suffices
     that these types align on the C++ side and this side.
     Only NumPy arrays are handled using the buffer interface & so if you want to pass a pointer
@@ -95,15 +100,15 @@
     NUMPY_Float16 = NUMPY_TYPES + 20
     _type_map[NUMPY_Float16] = ("float16", np.float16)
     NUMPY_Float32 = NUMPY_TYPES + 21
     _type_map[NUMPY_Float32] = ("float32", np.float32)
     NUMPY_Float64 = NUMPY_TYPES + 22
     _type_map[NUMPY_Float64] = ("float64", np.float64)
     NUMPY_Float128 = NUMPY_TYPES + 23
-    _type_map[NUMPY_Float128] = ("float128", np.float128)
+    _type_map[NUMPY_Float128] = ("float128", np_float128)
 
     NUMPY_Bool = NUMPY_TYPES + 30
     _type_map[NUMPY_Bool] = ("bool", bool)
 
     @classmethod
     def type_data(cls, val):
         mapp = cls._type_map.value
```

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/ModuleLoader.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/ModuleLoader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/SharedLibraryManager.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/SharedLibraryManager.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Extensions/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/Babel.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/ExternalPrograms/Babel.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/ExternalPrograms/OpenChem.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/ExternalPrograms/OpenChem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/FChkDerivatives.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/FChkDerivatives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianFChkComponents.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianImporter.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianImporter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianJob.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianJob.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/GaussianLogComponents.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/GaussianLogComponents.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/GaussianInterface/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/GaussianInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Apps.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Apps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Controls.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Controls.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Interfaces.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Interfaces.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/Variables.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/Variables.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/Apps/types.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/Apps/types.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/InteractiveTools.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/InteractiveTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Bootstrap.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/Bootstrap.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/BootstrapEnums.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/BootstrapWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/Enums.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/Enums.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTML.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/HTML.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/HTMLWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/HackWidgets.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/HackWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/JHTML.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/JHTML.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/WidgetTools.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/WidgetTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/JHTML/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/JHTML/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/MoleculeGraphics.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/MoleculeGraphics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/NBExporter.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/NBExporter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Jupyter/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/DebugTools.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/DebugTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/FileMatcher.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/FileMatcher.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/NumbaTools.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/NumbaTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/SBatchHelper.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/SBatchHelper.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/Symbolics.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/Symbolics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateEngine/ObjectWalker.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateEngine/TemplateEngine.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/TemplateWriter.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/TemplateWriter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Misc/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/AnalyticDerivs.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/AnalyticDerivs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/EulerSystem.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/EulerSystem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Misc.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/Misc.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Options.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/Options.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/SetOps.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/SetOps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/Sparse.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/Sparse.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationMatrices.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/TransformationMatrices.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/TransformationTransformations.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/TransformationTransformations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/VectorOps.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/VectorOps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Numputils/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Numputils/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Parallelizers.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/Parallelizers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/Runner.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/Runner.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/SharedMemory.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/SharedMemory.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parallelizers/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parallelizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/FileStreamer.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/FileStreamer.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/Parsers.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/Parsers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/RegexPatterns.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/RegexPatterns.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StringParser.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/StringParser.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/StructuredType.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/StructuredType.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Parsers/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Graphics.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Graphics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Image.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Image.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Interactive.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Interactive.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Plots.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Plots.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Primitives.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Primitives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Properties.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Properties.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/Styling.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/Styling.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/VTKInterface.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/VTKInterface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Plots/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/CLIs.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/CLIs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Caches.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Caches.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Checkpointing.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Checkpointing.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Configurations.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Configurations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Jobs.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Jobs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Logging.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Logging.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/ObjectBackers.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/ObjectBackers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Persistence.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Persistence.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Schema.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Schema.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/Serializers.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/Serializers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Scaffolding/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/FittableModels.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/FittableModels.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Interpolator.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Interpolator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/LazyTensors.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/LazyTensors.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Mesh.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Mesh.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/NeighborBasedInterpolators.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/NeighborBasedInterpolators.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Polynomials.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Polynomials.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/BaseSurface.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/BaseSurface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/Surface.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/Surface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Surfaces/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/ElementaryFunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/TensorExpressions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Symbolic/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/Derivatives.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/Derivatives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/FunctionExpansions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/Taylor/ZachLib/src/setup.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/Zachary/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/Zachary/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/McUtils/__init__.py` & `mccoygroup-mcutils-0.1.1.2/McUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/PKG-INFO` & `mccoygroup-mcutils-0.1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-mcutils
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # McUtils [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mccoygroup/binder-mcutils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmccoygroup%252FMcUtils%26urlpath%3Dlab%252Ftree%252FMcUtils%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-mcutils-0.1.1.1/README.md` & `mccoygroup-mcutils-0.1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/PKG-INFO` & `mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-mcutils
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # McUtils [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mccoygroup/binder-mcutils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmccoygroup%252FMcUtils%26urlpath%3Dlab%252Ftree%252FMcUtils%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-mcutils-0.1.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt` & `mccoygroup-mcutils-0.1.1.2/mccoygroup_mcutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.1.1/setup.py` & `mccoygroup-mcutils-0.1.1.2/setup.py`

 * *Files identical despite different names*

