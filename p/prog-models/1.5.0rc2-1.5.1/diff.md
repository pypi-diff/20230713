# Comparing `tmp/prog_models-1.5.0rc2.tar.gz` & `tmp/prog_models-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_models-1.5.0rc2.tar", last modified: Wed Jun 28 22:53:02 2023, max compression
+gzip compressed data, was "prog_models-1.5.1.tar", last modified: Thu Jul 13 03:45:36 2023, max compression
```

## Comparing `prog_models-1.5.0rc2.tar` & `prog_models-1.5.1.tar`

### file list

```diff
@@ -1,179 +1,107 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.601831 prog_models-1.5.0rc2/
--rw-r--r--   0 cteubert   (507) staff       (20)     1295 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/.gitignore
--rw-r--r--   0 cteubert   (507) staff       (20)     7016 2023-06-28 22:53:02.601661 prog_models-1.5.0rc2/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     5153 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/README.md
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.573172 prog_models-1.5.0rc2/docs/
--rw-r--r--   0 cteubert   (507) staff       (20)      230 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.buildinfo
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.574539 prog_models-1.5.0rc2/docs/.doctrees/
--rw-r--r--   0 cteubert   (507) staff       (20)    96339 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/.doctrees/deriv_prog_model.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2831 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/dev_guide.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)    18573 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/environment.pickle
--rw-r--r--   0 cteubert   (507) staff       (20)    12051 2023-06-20 18:40:01.000000 prog_models-1.5.0rc2/docs/.doctrees/exceptions.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2775 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/getting_started.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2837 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/index.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2730 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/models.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     2785 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/.doctrees/prognostics_model.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)   102536 2023-06-20 18:40:01.000000 prog_models-1.5.0rc2/docs/.doctrees/visualize.doctree
--rw-r--r--   0 cteubert   (507) staff       (20)     5271 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/7150.md
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.575595 prog_models-1.5.0rc2/docs/_sources/
--rw-r--r--   0 cteubert   (507) staff       (20)      160 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_sources/deriv_prog_model.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      119 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/dev_guide.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      608 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_sources/exceptions.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)       86 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/getting_started.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      150 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/index.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      123 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/models.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)       96 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_sources/prognostics_model.rst.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      179 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_sources/visualize.rst.txt
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.582662 prog_models-1.5.0rc2/docs/_static/
--rw-r--r--   0 cteubert   (507) staff       (20)    11185 2022-08-23 14:28:13.000000 prog_models-1.5.0rc2/docs/_static/alabaster.css
--rw-r--r--   0 cteubert   (507) staff       (20)    14692 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/basic.css
--rw-r--r--   0 cteubert   (507) staff       (20)     4534 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/classic.css
--rw-r--r--   0 cteubert   (507) staff       (20)       42 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/custom.css
--rw-r--r--   0 cteubert   (507) staff       (20)    10766 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/doctools.js
--rw-r--r--   0 cteubert   (507) staff       (20)      422 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/documentation_options.js
--rw-r--r--   0 cteubert   (507) staff       (20)      286 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/file.png
--rw-r--r--   0 cteubert   (507) staff       (20)   287630 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 cteubert   (507) staff       (20)    89476 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/jquery.js
--rw-r--r--   0 cteubert   (507) staff       (20)    10854 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/language_data.js
--rw-r--r--   0 cteubert   (507) staff       (20)       90 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/minus.png
--rw-r--r--   0 cteubert   (507) staff       (20)       90 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/plus.png
--rw-r--r--   0 cteubert   (507) staff       (20)     5249 2022-08-23 14:28:13.000000 prog_models-1.5.0rc2/docs/_static/pygments.css
--rw-r--r--   0 cteubert   (507) staff       (20)    16634 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/_static/searchtools.js
--rw-r--r--   0 cteubert   (507) staff       (20)     4803 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/sidebar.js
--rw-r--r--   0 cteubert   (507) staff       (20)    67692 2021-05-10 16:37:43.000000 prog_models-1.5.0rc2/docs/_static/underscore-1.12.0.js
--rw-r--r--   0 cteubert   (507) staff       (20)    35168 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/_static/underscore-1.3.1.js
--rw-r--r--   0 cteubert   (507) staff       (20)    19530 2023-06-20 18:40:01.000000 prog_models-1.5.0rc2/docs/_static/underscore.js
--rw-r--r--   0 cteubert   (507) staff       (20)    27376 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/deriv_prog_model.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/dev_guide.html
--rw-r--r--   0 cteubert   (507) staff       (20)     7442 2023-06-20 18:44:15.000000 prog_models-1.5.0rc2/docs/exceptions.html
--rw-r--r--   0 cteubert   (507) staff       (20)     2295 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/genindex.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/getting_started.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/index.html
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/models.html
--rw-r--r--   0 cteubert   (507) staff       (20)      443 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/objects.inv
--rw-r--r--   0 cteubert   (507) staff       (20)      100 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/prognostics_model.html
--rw-r--r--   0 cteubert   (507) staff       (20)     8365 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/py-modindex.html
--rw-r--r--   0 cteubert   (507) staff       (20)     2608 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/search.html
--rw-r--r--   0 cteubert   (507) staff       (20)     1275 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/docs/searchindex.js
--rw-r--r--   0 cteubert   (507) staff       (20)      961 2021-03-10 17:51:45.000000 prog_models-1.5.0rc2/docs/softwareplan.md
--rw-r--r--   0 cteubert   (507) staff       (20)    31639 2023-06-20 18:42:18.000000 prog_models-1.5.0rc2/docs/visualize.html
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.583564 prog_models-1.5.0rc2/examples/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/examples/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      939 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/examples/benchmarking.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6312 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/examples/future_loading.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4767 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/examples/new_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4949 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/examples/noise.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2433 2023-06-20 18:45:28.000000 prog_models-1.5.0rc2/examples/sensitivity.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3608 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/examples/sim.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.583944 prog_models-1.5.0rc2/forms/
--rw-r--r--   0 cteubert   (507) staff       (20)   219343 2023-06-20 18:42:18.000000 prog_models-1.5.0rc2/forms/Corporate CLA.pdf
--rw-r--r--   0 cteubert   (507) staff       (20)   153485 2023-06-20 18:42:18.000000 prog_models-1.5.0rc2/forms/Individual CLA.pdf
--rw-r--r--   0 cteubert   (507) staff       (20)    94594 2021-05-10 16:37:43.000000 prog_models-1.5.0rc2/license.pdf
--rw-r--r--   0 cteubert   (507) staff       (20)    13424 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/prog_model_template.py
--rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-28 22:53:02.601868 prog_models-1.5.0rc2/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2932 2023-06-28 22:52:14.000000 prog_models-1.5.0rc2/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.567757 prog_models-1.5.0rc2/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.585090 prog_models-1.5.0rc2/src/prog_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      468 2023-06-28 22:52:26.000000 prog_models-1.5.0rc2/src/prog_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12776 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/composite_model.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.586479 prog_models-1.5.0rc2/src/prog_models/data_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      476 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/data_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8208 2023-06-28 14:47:51.000000 prog_models-1.5.0rc2/src/prog_models/data_models/data_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    22276 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/data_models/dmd.py
--rw-r--r--   0 cteubert   (507) staff       (20)    35164 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/data_models/lstm_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8465 2023-06-28 21:50:30.000000 prog_models-1.5.0rc2/src/prog_models/data_models/pce.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.587236 prog_models-1.5.0rc2/src/prog_models/datasets/
--rw-r--r--   0 cteubert   (507) staff       (20)      157 2023-06-20 18:44:15.000000 prog_models-1.5.0rc2/src/prog_models/datasets/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6185 2023-06-22 23:28:06.000000 prog_models-1.5.0rc2/src/prog_models/datasets/nasa_battery.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6170 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/datasets/nasa_cmapss.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5558 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/ensemble_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)      543 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/exceptions.py
--rw-r--r--   0 cteubert   (507) staff       (20)     9133 2023-06-28 21:50:30.000000 prog_models-1.5.0rc2/src/prog_models/linear_model.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.589213 prog_models-1.5.0rc2/src/prog_models/loading/
--rw-r--r--   0 cteubert   (507) staff       (20)      347 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    15484 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/controllers.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1495 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/gaussian_wrapper.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2102 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/moving_average.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1772 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/loading/piecewise.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591031 prog_models-1.5.0rc2/src/prog_models/models/
--rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/__init__.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591475 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/
--rw-r--r--   0 cteubert   (507) staff       (20)      242 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      335 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/aircraft.py
--rw-r--r--   0 cteubert   (507) staff       (20)    19213 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/small_rotorcraft.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591737 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/
--rw-r--r--   0 cteubert   (507) staff       (20)        0 2023-06-28 22:49:52.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/__init__.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.591987 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/
--rw-r--r--   0 cteubert   (507) staff       (20)        0 2023-06-28 22:50:32.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1387 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.592987 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/
--rw-r--r--   0 cteubert   (507) staff       (20)        0 2023-06-28 22:50:22.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2583 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12709 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/vehicles.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7882 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/battery_circuit.py
--rw-r--r--   0 cteubert   (507) staff       (20)    32566 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/battery_electrochem.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12741 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/centrifugal_pump.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6530 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/dcmotor.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5649 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/dcmotor_singlephase.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4653 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/esc.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.593516 prog_models-1.5.0rc2/src/prog_models/models/experimental/
--rw-r--r--   0 cteubert   (507) staff       (20)      158 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/experimental/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2949 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/experimental/paris_law.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17214 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/pneumatic_valve.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6555 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/powertrain.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1428 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/propeller_load.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.594067 prog_models-1.5.0rc2/src/prog_models/models/test_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      249 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/test_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4384 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_models.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4050 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_thrown_object.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5714 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/models/thrown_object.py
--rw-r--r--   0 cteubert   (507) staff       (20)    68508 2023-06-28 21:35:58.000000 prog_models-1.5.0rc2/src/prog_models/prognostics_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17091 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/sim_result.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.596241 prog_models-1.5.0rc2/src/prog_models/utils/
--rw-r--r--   0 cteubert   (507) staff       (20)      198 2023-06-20 18:44:15.000000 prog_models-1.5.0rc2/src/prog_models/utils/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    21583 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/calc_error.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8984 2023-06-28 18:01:11.000000 prog_models-1.5.0rc2/src/prog_models/utils/containers.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1014 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/input_validation.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4382 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/next_state.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2242 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/noise_functions.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10374 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/parameters.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1173 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/progress_bar.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1859 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/serialization.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2484 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/size.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.598136 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/
--rw-r--r--   0 cteubert   (507) staff       (20)      221 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    24434 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/geometry.py
--rw-r--r--   0 cteubert   (507) staff       (20)    16044 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/nurbs.py
--rw-r--r--   0 cteubert   (507) staff       (20)    33968 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/trajectory.py
--rw-r--r--   0 cteubert   (507) staff       (20)    27416 2023-06-28 18:01:29.000000 prog_models-1.5.0rc2/src/prog_models/visualize.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.585780 prog_models-1.5.0rc2/src/prog_models.egg-info/
--rw-------   0 cteubert   (507) staff       (20)     7016 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/PKG-INFO
--rw-------   0 cteubert   (507) staff       (20)     4988 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/SOURCES.txt
--rw-------   0 cteubert   (507) staff       (20)        1 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/dependency_links.txt
--rw-------   0 cteubert   (507) staff       (20)      204 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/requires.txt
--rw-------   0 cteubert   (507) staff       (20)       12 2023-06-28 22:53:02.000000 prog_models-1.5.0rc2/src/prog_models.egg-info/top_level.txt
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-28 22:53:02.601462 prog_models-1.5.0rc2/tests/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/tests/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3309 2023-06-20 20:08:13.000000 prog_models-1.5.0rc2/tests/__main__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    56896 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_base_models.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2652 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_battery.py
--rw-r--r--   0 cteubert   (507) staff       (20)    18087 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_calc_error.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8122 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_centrifugal_pump.py
--rw-r--r--   0 cteubert   (507) staff       (20)    14085 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_composite.py
--rw-r--r--   0 cteubert   (507) staff       (20)    13250 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_data_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1872 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_datasets.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4177 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_dict_like_matrix_wrapper.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4622 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_direct.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7537 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_ensemble.py
--rw-r--r--   0 cteubert   (507) staff       (20)    55549 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_estimate_params.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1627 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_examples.py
--rw-r--r--   0 cteubert   (507) staff       (20)    18578 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_linear_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6686 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_manual.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12907 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_pneumatic_valve.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2435 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_powertrain.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4267 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_serialization.py
--rw-r--r--   0 cteubert   (507) staff       (20)    35373 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_sim_result.py
--rw-r--r--   0 cteubert   (507) staff       (20)    32855 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_surrogates.py
--rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_tutorials.py
--rw-r--r--   0 cteubert   (507) staff       (20)    15470 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tests/test_uav_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    47927 2023-06-28 14:48:00.000000 prog_models-1.5.0rc2/tutorial.ipynb
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.557369 prog_models-1.5.1/
+-rw-r--r--   0 cteubert   (507) staff       (20)     7013 2023-07-13 03:45:36.557201 prog_models-1.5.1/PKG-INFO
+-rw-r--r--   0 cteubert   (507) staff       (20)     5153 2023-07-10 14:41:28.000000 prog_models-1.5.1/README.md
+-rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-07-13 03:45:36.557416 prog_models-1.5.1/setup.cfg
+-rw-r--r--   0 cteubert   (507) staff       (20)     2928 2023-07-13 03:44:24.000000 prog_models-1.5.1/setup.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.527922 prog_models-1.5.1/src/
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.531760 prog_models-1.5.1/src/prog_models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      464 2023-07-13 03:44:13.000000 prog_models-1.5.1/src/prog_models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12776 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/composite_model.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.534362 prog_models-1.5.1/src/prog_models/data_models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      476 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/data_models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8208 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/data_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    22276 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/dmd.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    35216 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/lstm_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8465 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/pce.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.534829 prog_models-1.5.1/src/prog_models/datasets/
+-rw-r--r--   0 cteubert   (507) staff       (20)      157 2023-06-20 18:44:15.000000 prog_models-1.5.1/src/prog_models/datasets/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6185 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/datasets/nasa_battery.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6170 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/datasets/nasa_cmapss.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5558 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/ensemble_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      543 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/exceptions.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     9133 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/linear_model.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.536622 prog_models-1.5.1/src/prog_models/loading/
+-rw-r--r--   0 cteubert   (507) staff       (20)      347 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    15484 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/controllers.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1495 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/gaussian_wrapper.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2102 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/moving_average.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1772 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/piecewise.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.540054 prog_models-1.5.1/src/prog_models/models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/models/__init__.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.541365 prog_models-1.5.1/src/prog_models/models/aircraft_model/
+-rw-r--r--   0 cteubert   (507) staff       (20)      242 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      335 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/aircraft.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    19213 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/small_rotorcraft.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.542558 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/__init__.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.543479 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1387 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.543937 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2583 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12709 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/vehicles.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7882 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/battery_circuit.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    32566 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/battery_electrochem.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12741 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/centrifugal_pump.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6530 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/dcmotor.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5649 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/dcmotor_singlephase.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4653 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/esc.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.545257 prog_models-1.5.1/src/prog_models/models/experimental/
+-rw-r--r--   0 cteubert   (507) staff       (20)      158 2023-06-20 20:08:13.000000 prog_models-1.5.1/src/prog_models/models/experimental/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2949 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/experimental/paris_law.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    17214 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/pneumatic_valve.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6555 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/powertrain.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1428 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/propeller_load.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.547681 prog_models-1.5.1/src/prog_models/models/test_models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      249 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/models/test_models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4384 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/models/test_models/linear_models.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4050 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/test_models/linear_thrown_object.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5714 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/thrown_object.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    68654 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/prognostics_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    17189 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/sim_result.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.549997 prog_models-1.5.1/src/prog_models/utils/
+-rw-r--r--   0 cteubert   (507) staff       (20)      198 2023-06-20 18:44:15.000000 prog_models-1.5.1/src/prog_models/utils/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    21583 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/calc_error.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8984 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/containers.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1014 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/input_validation.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4382 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/next_state.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2242 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/noise_functions.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    10374 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/parameters.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1173 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/progress_bar.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1859 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/serialization.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2484 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/size.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.551333 prog_models-1.5.1/src/prog_models/utils/traj_gen/
+-rw-r--r--   0 cteubert   (507) staff       (20)      221 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    24434 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/geometry.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    16044 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/nurbs.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    33968 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/trajectory.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    27416 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/visualize.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.532951 prog_models-1.5.1/src/prog_models.egg-info/
+-rw-r--r--   0 cteubert   (507) staff       (20)     7013 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/PKG-INFO
+-rw-r--r--   0 cteubert   (507) staff       (20)     3302 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/SOURCES.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)        1 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/dependency_links.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)      204 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/requires.txt
+-rw-r--r--   0 cteubert   (507) staff       (20)       12 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/top_level.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.556962 prog_models-1.5.1/tests/
+-rw-r--r--   0 cteubert   (507) staff       (20)    56896 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_base_models.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2652 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_battery.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    18087 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_calc_error.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8122 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_centrifugal_pump.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    14085 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_composite.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    13250 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_data_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1872 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_datasets.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4177 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_dict_like_matrix_wrapper.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4622 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_direct.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7537 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_ensemble.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    55549 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_estimate_params.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1627 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_examples.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    18578 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_linear_model.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6686 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_manual.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    12907 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_pneumatic_valve.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2435 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_powertrain.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4267 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_serialization.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    35373 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_sim_result.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    32855 2023-07-13 03:43:36.000000 prog_models-1.5.1/tests/test_surrogates.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_tutorials.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    15453 2023-07-13 03:43:36.000000 prog_models-1.5.1/tests/test_uav_model.py
```

### Comparing `prog_models-1.5.0rc2/PKG-INFO` & `prog_models-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_models
-Version: 1.5.0rc2
+Version: 1.5.1
 Summary: The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.
 Home-page: https://nasa.github.io/progpy/prog_models_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_models/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_models_guide.html
```

### Comparing `prog_models-1.5.0rc2/README.md` & `prog_models-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/setup.py` & `prog_models-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'fastdtw',  # For DTW error calculation
         "tensorflow; platform_system!='Darwin' or platform_machine!='arm64'",
         "tensorflow-macos; platform_system=='Darwin' and platform_machine=='arm64'",
     ]
 
 setup(
     name='prog_models',
-    version='1.5.0-rc2',
+    version='1.5.1',
     description='The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://nasa.github.io/progpy/prog_models_guide.html',
     author='Christopher Teubert',
     author_email='christopher.a.teubert@nasa.gov',
     classifiers=[
```

### Comparing `prog_models-1.5.0rc2/src/prog_models/composite_model.py` & `prog_models-1.5.1/src/prog_models/composite_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/data_models/data_model.py` & `prog_models-1.5.1/src/prog_models/data_models/data_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/data_models/dmd.py` & `prog_models-1.5.1/src/prog_models/data_models/dmd.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/data_models/lstm_model.py` & `prog_models-1.5.1/src/prog_models/data_models/lstm_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,16 @@
             return self.StateContainer(np.vstack((states, x.matrix[-self.parameters['state_model'].output_shape[1]:])))
         else:
             # Enough data has been received to calculate output
             # Format input into np array with shape (1, window, num_inputs)
             m_input = states.reshape(1, self.parameters['window'], len(self.inputs))
             m_input = np.array(m_input, dtype=np.float64)
             internal_states = self.parameters['state_model'](m_input).numpy().T
-        return self.StateContainer(np.vstack((states, internal_states)))
+        result = np.array(np.vstack((states, internal_states)), dtype=np.float64)
+        return self.StateContainer(result)
 
     def output(self, x):
         if x.matrix[0, 0] is None:
             warn(f"Output estimation is not available until at least {1+self.parameters['window']} timesteps have passed.")
             return self.OutputContainer(np.array([[None] for _ in self.outputs]))
 
         # Enough data has been received to calculate output
```

### Comparing `prog_models-1.5.0rc2/src/prog_models/data_models/pce.py` & `prog_models-1.5.1/src/prog_models/data_models/pce.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/datasets/nasa_battery.py` & `prog_models-1.5.1/src/prog_models/datasets/nasa_battery.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/datasets/nasa_cmapss.py` & `prog_models-1.5.1/src/prog_models/datasets/nasa_cmapss.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/ensemble_model.py` & `prog_models-1.5.1/src/prog_models/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/exceptions.py` & `prog_models-1.5.1/src/prog_models/exceptions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/linear_model.py` & `prog_models-1.5.1/src/prog_models/linear_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/loading/controllers.py` & `prog_models-1.5.1/src/prog_models/loading/controllers.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/loading/gaussian_wrapper.py` & `prog_models-1.5.1/src/prog_models/loading/gaussian_wrapper.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/loading/moving_average.py` & `prog_models-1.5.1/src/prog_models/loading/moving_average.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/loading/piecewise.py` & `prog_models-1.5.1/src/prog_models/loading/piecewise.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/__init__.py` & `prog_models-1.5.1/src/prog_models/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/small_rotorcraft.py` & `prog_models-1.5.1/src/prog_models/models/aircraft_model/small_rotorcraft.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py` & `prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py` & `prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/aircraft_model/vehicles/vehicles.py` & `prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/vehicles.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/battery_circuit.py` & `prog_models-1.5.1/src/prog_models/models/battery_circuit.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/battery_electrochem.py` & `prog_models-1.5.1/src/prog_models/models/battery_electrochem.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/centrifugal_pump.py` & `prog_models-1.5.1/src/prog_models/models/centrifugal_pump.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/dcmotor.py` & `prog_models-1.5.1/src/prog_models/models/dcmotor.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/dcmotor_singlephase.py` & `prog_models-1.5.1/src/prog_models/models/dcmotor_singlephase.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/esc.py` & `prog_models-1.5.1/src/prog_models/models/esc.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/experimental/paris_law.py` & `prog_models-1.5.1/src/prog_models/models/experimental/paris_law.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/pneumatic_valve.py` & `prog_models-1.5.1/src/prog_models/models/pneumatic_valve.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/powertrain.py` & `prog_models-1.5.1/src/prog_models/models/powertrain.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/propeller_load.py` & `prog_models-1.5.1/src/prog_models/models/propeller_load.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_models.py` & `prog_models-1.5.1/src/prog_models/models/test_models/linear_models.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/test_models/linear_thrown_object.py` & `prog_models-1.5.1/src/prog_models/models/test_models/linear_thrown_object.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/models/thrown_object.py` & `prog_models-1.5.1/src/prog_models/models/thrown_object.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/prognostics_model.py` & `prog_models-1.5.1/src/prog_models/prognostics_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,15 +682,15 @@
             'future_loading_eqn': future_loading_eqn,
         }
         params.update(kwargs)
 
         threshold_keys = self.events.copy()
         t = 0
         time_of_event = {}
-        while len(threshold_keys) > 0:
+        while len(threshold_keys) > 0 and t < params.get('horizon', np.inf):
             result = self.simulate_to_threshold(x = x, t0 = t, **params)
             for key, value in result.event_states[-1].items():
                 if value <= 0 and key not in time_of_event:
                     threshold_keys.remove(key)
                     time_of_event[key] = result.times[-1]
             x = result.states[-1]
             t = result.times[-1]
@@ -1041,19 +1041,19 @@
         if 'integration_method' in config:
             # Update integration method for the duration of the simulation
             old_integration_method = self.parameters.get('integration_method', 'euler')
             self.parameters['integration_method'] = config['integration_method']
        
         while t < horizon:
             dt_i = next_time(t, x)
-            t = t + dt_i/2
+            t_load = t + dt_i/2  # Saving as separate variable reduces likelihood of floating point error
             # Use state at midpoint of step to best represent the load during the duration of the step
             # This is sometimes referred to as 'leapfrog integration'
-            u = load_eqn(t, x)
-            t = t + dt_i/2
+            u = load_eqn(t_load, x)
+            t += dt_i
             x = next_state(x, u, dt_i)
             x = apply_noise(x, dt_i)
             x = apply_limits(x)
 
             # Save if at appropriate time
             if (t >= next_save):
                 next_save = next(iterator)
@@ -1120,16 +1120,16 @@
             inputs (list[InputContainer]): array of input dictionaries where input[x] corresponds to time[x]
             outputs (list[OutputContainer]): array of output dictionaries where output[x] corresponds to time[x]
         
         Keyword Args:
             method (str, optional): Error method to use when calculating error. Supported methods include:
 
               * MSE (Mean Squared Error) - DEFAULT
-              * RMSE (Root Mean Squared Error)
-              * MAX_E (Maximum Error)
+              * RMSE (Root Mean Squared Error) - Squareroot of MSE
+              * MAX_E (Maximum Absolute Error)
               * MAE (Mean Absolute Error)
               * MAPE (Mean Absolute Percentage Error)
               * DTW (Dynamic Time Warping)
             x0 (StateContainer, optional): Initial state
             dt (float, optional): Maximum time step in simulation. Time step used in simulation is lower of dt and time between samples. Defaults to time between samples.
             stability_tol (double, optional): Configurable parameter.
                 Configurable cutoff value, between 0 and 1, that determines the fraction of the data points for which the model must be stable.
```

### Comparing `prog_models-1.5.0rc2/src/prog_models/sim_result.py` & `prog_models-1.5.1/src/prog_models/sim_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,38 +37,38 @@
     def __getitem__(self, item):
         """
             created for deprecation warning. [] continues to be handled by parent
         """
         warn_once('[] for access by row number will be deprecated after version 1.5 of ProgPy. After v1.5, [] will access by column (e.g., data[\'state1\']), Users may use \'iloc\' to access by row number (e.g., data.iloc[10])'
             'data by element.', DeprecationWarning, stacklevel=2)
         return super().__getitem__(item)
-    
+
     def __iter__(self):
         """
             created for deprecation warning. iteration continues to be handled by parent
         """
         warn_once(
             'iteration will be deprecated after version 1.5 of ProgPy. The function will be renamed, iterrows, '
             'and users may begin using it under this name now.',
             DeprecationWarning, stacklevel=2)
         return super().__iter__()
-    
+
     def iterrows(self):
         """
         .. versionadded:: 1.5.0
-        
+
             Iterates -- through keys
         """
         return super().__iter__()
 
     @property
     def frame(self) -> pd.DataFrame:
         """
         .. versionadded:: 1.5.0
-        
+
             pd.DataFrame: A pandas DataFrame representing the SimResult data
         """
         warn_once('frame will be deprecated after version 1.5 of ProgPy.', DeprecationWarning, stacklevel=2)
         if self._frame is None:
             if len(self.data) > 0:  #
                 self._frame = pd.concat([
                     pd.DataFrame(dict(dframe), index=[0]) for dframe in self.data
@@ -77,19 +77,19 @@
                 self._frame = pd.DataFrame()
             if self.times is not None:
                 self._frame.insert(0, "time", self.times)
                 self._frame = self._frame.set_index('time')
             return self._frame
         else:
             return self._frame
-        
+
     def frame_is_empty(self) -> bool:
         """
         .. versionadded:: 1.5.0
-        
+
         Returns:
             bool: If the value has been calculated
         """
         return self._frame.empty
 
     def __setitem__(self, key, value):
         """
@@ -106,34 +106,36 @@
         """
         super().__delitem__(key)
         if self._frame is not None:
             self._frame = self._frame.drop([key])
 
     def insert(self, i: int, item) -> None:
         """
+        .. versionadded:: 1.5.0
+
             in addition to the normal functionality, updates the _frame if it exists
         """
         self.insert(i, item)
         if self._frame is not None:
             for value in item:
                 self._frame.insert(i, column=[value], value=item[value])
 
     @property
     def iloc(self):
         """
         .. versionadded:: 1.5.0
-        
+
             returns the iloc indexer
         """
         return self.frame.iloc
 
     def equals(self, other: "SimResult") -> bool:
         """
         .. versionadded:: 1.5.0
-        
+
         Compare 2 SimResults
 
         Args:
             other (SimResult)
 
         Returns:
             bool: If the two SimResults are equal
@@ -155,24 +157,26 @@
             'and users may begin using it under this name now.',
             DeprecationWarning, stacklevel=2)
 
         return self.equals(other)
 
     def index_of_data(self, other: dict, *args, **kwargs) -> int:
         """
+        .. versionadded:: 1.5.0
+
         Get the index of the first sample where other occurs
 
         Args:
             other (dict)
 
         Returns:
             int: Index of first sample where other occurs
         """
         return self.data.index(other, *args, **kwargs)
-    
+
     def index(self, other: dict, *args, **kwargs) -> int:
         """
         Get the index of the first sample where other occurs
 
         Args:
             other (dict)
 
@@ -197,43 +201,48 @@
             self.data.extend(other.data)
         else:
             raise ValueError(f"ValueError: Argument must be of type {self.__class__}")
         if self._frame is not None:
             self._frame = None
 
     def pop_by_index(self, index: int = -1) -> dict:
-        """Remove and return an element
+        """
+        .. versionadded:: 1.5.0
+
+        Remove and return an element
 
         Args:
             index (int, optional): Index of element to be removed. Defaults to -1.
 
         Returns:
             dict: Element Removed
         """
         self.times.pop(index)
         if self._frame is not None:
             self._frame = self._frame.drop([self._frame.index.values[index]])
         return self.data.pop(index)
 
     def pop(self, index: int = -1) -> dict:
-        """Remove and return an element
+        """
+        Remove and return an element
 
         Args:
             index (int, optional): Index of element to be removed. Defaults to -1.
 
         Returns:
             dict: Element Removed
         """
         warn_once(
             'pop will be deprecated after version 1.5 of ProgPy. The function will be renamed, pop_by_index, and users may begin using it under this name now.',
             DeprecationWarning, stacklevel=2)
         return self.pop_by_index(index)
 
     def remove(self, d: dict = None, t: float = None) -> None:
-        """Remove an element
+        """
+        Remove an element
 
         Args:
             d: Data value to be removed.
             t: Time value to be removed.
         """
         if sum([i is None for i in (d, t)]) != 1:
             raise ValueError("ValueError: Only one named argument (d, t) can be specified.")
@@ -241,21 +250,24 @@
         if (t is not None):
             target_index = self.times.index(t)
         else:
             target_index = self.data.index(d)
         self.pop_by_index(target_index)
 
     def clear(self) -> None:
-        """Clear the SimResult"""
+        """
+        Clear the SimResult
+        """
         self.times = []
         self.data = []
         self._frame = None
 
     def time(self, index: int) -> float:
-        """Get time for data point at index `index`
+        """
+        Get time for data point at index `index`
 
         Args:
             index (int)
 
         Returns:
             float: Time for which the data point at index `index` corresponds
         """
@@ -276,15 +288,15 @@
         if len(self.data[0]) == 0:
             return np.array([[] for _ in self.data], dtype=np.float64)
         if isinstance(self.data[0], DictLikeMatrixWrapper) and keys is None:
             return np.array([u_i.matrix[:, 0] for u_i in self.data], dtype=np.float64)
         if keys is None:
             keys = self.data[0].keys()
         return np.array([[u_i[key] for key in keys] for u_i in self.data], dtype=np.float64)
-    
+
     def plot(self, **kwargs) -> figure:
         """
         Plot the simresult as a line plot
 
         Keyword Args:
             keys (list[str]): list of keys to plot. If not provided, all keys in the series are plotted.
             figsize (tuple[float, float]): width and height of the figure
@@ -416,15 +428,16 @@
         elif (isinstance(other, SimResult)):
             raise ValueError(
                 f"ValueError: {self.__class__} cannot be extended by SimResult. First convert to SimResult using to_simresult() method.")
         else:
             raise ValueError(f"ValueError: Argument must be of type {self.__class__}.")
 
     def pop(self, index: int = -1) -> dict:
-        """Remove an element. If data hasn't been cached, remove the state - so it wont be calculated
+        """
+        Remove an element. If data hasn't been cached, remove the state - so it wont be calculated
 
         Args:
             index (int, optional): Index of element to be removed. Defaults to -1.
 
         Returns:
             dict: Element Removed
         """
```

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/calc_error.py` & `prog_models-1.5.1/src/prog_models/utils/calc_error.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/containers.py` & `prog_models-1.5.1/src/prog_models/utils/containers.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/input_validation.py` & `prog_models-1.5.1/src/prog_models/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/next_state.py` & `prog_models-1.5.1/src/prog_models/utils/next_state.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/noise_functions.py` & `prog_models-1.5.1/src/prog_models/utils/noise_functions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/parameters.py` & `prog_models-1.5.1/src/prog_models/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/progress_bar.py` & `prog_models-1.5.1/src/prog_models/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/serialization.py` & `prog_models-1.5.1/src/prog_models/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/size.py` & `prog_models-1.5.1/src/prog_models/utils/size.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/geometry.py` & `prog_models-1.5.1/src/prog_models/utils/traj_gen/geometry.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/nurbs.py` & `prog_models-1.5.1/src/prog_models/utils/traj_gen/nurbs.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/utils/traj_gen/trajectory.py` & `prog_models-1.5.1/src/prog_models/utils/traj_gen/trajectory.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models/visualize.py` & `prog_models-1.5.1/src/prog_models/visualize.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/src/prog_models.egg-info/PKG-INFO` & `prog_models-1.5.1/src/prog_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-models
-Version: 1.5.0rc2
+Version: 1.5.1
 Summary: The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.
 Home-page: https://nasa.github.io/progpy/prog_models_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_models/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_models_guide.html
```

### Comparing `prog_models-1.5.0rc2/src/prog_models.egg-info/SOURCES.txt` & `prog_models-1.5.1/src/prog_models.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,9 @@
-.gitignore
 README.md
-license.pdf
-prog_model_template.py
 setup.py
-tutorial.ipynb
-docs/.buildinfo
-docs/7150.md
-docs/deriv_prog_model.html
-docs/dev_guide.html
-docs/exceptions.html
-docs/genindex.html
-docs/getting_started.html
-docs/index.html
-docs/models.html
-docs/objects.inv
-docs/prognostics_model.html
-docs/py-modindex.html
-docs/search.html
-docs/searchindex.js
-docs/softwareplan.md
-docs/visualize.html
-docs/.doctrees/deriv_prog_model.doctree
-docs/.doctrees/dev_guide.doctree
-docs/.doctrees/environment.pickle
-docs/.doctrees/exceptions.doctree
-docs/.doctrees/getting_started.doctree
-docs/.doctrees/index.doctree
-docs/.doctrees/models.doctree
-docs/.doctrees/prognostics_model.doctree
-docs/.doctrees/visualize.doctree
-docs/_sources/deriv_prog_model.rst.txt
-docs/_sources/dev_guide.rst.txt
-docs/_sources/exceptions.rst.txt
-docs/_sources/getting_started.rst.txt
-docs/_sources/index.rst.txt
-docs/_sources/models.rst.txt
-docs/_sources/prognostics_model.rst.txt
-docs/_sources/visualize.rst.txt
-docs/_static/alabaster.css
-docs/_static/basic.css
-docs/_static/classic.css
-docs/_static/custom.css
-docs/_static/doctools.js
-docs/_static/documentation_options.js
-docs/_static/file.png
-docs/_static/jquery-3.5.1.js
-docs/_static/jquery.js
-docs/_static/language_data.js
-docs/_static/minus.png
-docs/_static/plus.png
-docs/_static/pygments.css
-docs/_static/searchtools.js
-docs/_static/sidebar.js
-docs/_static/underscore-1.12.0.js
-docs/_static/underscore-1.3.1.js
-docs/_static/underscore.js
-examples/__init__.py
-examples/benchmarking.py
-examples/future_loading.py
-examples/new_model.py
-examples/noise.py
-examples/sensitivity.py
-examples/sim.py
-forms/Corporate CLA.pdf
-forms/Individual CLA.pdf
 src/prog_models/__init__.py
 src/prog_models/composite_model.py
 src/prog_models/ensemble_model.py
 src/prog_models/exceptions.py
 src/prog_models/linear_model.py
 src/prog_models/prognostics_model.py
 src/prog_models/sim_result.py
@@ -125,16 +61,14 @@
 src/prog_models/utils/progress_bar.py
 src/prog_models/utils/serialization.py
 src/prog_models/utils/size.py
 src/prog_models/utils/traj_gen/__init__.py
 src/prog_models/utils/traj_gen/geometry.py
 src/prog_models/utils/traj_gen/nurbs.py
 src/prog_models/utils/traj_gen/trajectory.py
-tests/__init__.py
-tests/__main__.py
 tests/test_base_models.py
 tests/test_battery.py
 tests/test_calc_error.py
 tests/test_centrifugal_pump.py
 tests/test_composite.py
 tests/test_data_model.py
 tests/test_datasets.py
```

### Comparing `prog_models-1.5.0rc2/tests/test_base_models.py` & `prog_models-1.5.1/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_battery.py` & `prog_models-1.5.1/tests/test_battery.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_calc_error.py` & `prog_models-1.5.1/tests/test_calc_error.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_centrifugal_pump.py` & `prog_models-1.5.1/tests/test_centrifugal_pump.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_composite.py` & `prog_models-1.5.1/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_data_model.py` & `prog_models-1.5.1/tests/test_data_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_datasets.py` & `prog_models-1.5.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_dict_like_matrix_wrapper.py` & `prog_models-1.5.1/tests/test_dict_like_matrix_wrapper.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_direct.py` & `prog_models-1.5.1/tests/test_direct.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_ensemble.py` & `prog_models-1.5.1/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_estimate_params.py` & `prog_models-1.5.1/tests/test_estimate_params.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_examples.py` & `prog_models-1.5.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_linear_model.py` & `prog_models-1.5.1/tests/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_manual.py` & `prog_models-1.5.1/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_pneumatic_valve.py` & `prog_models-1.5.1/tests/test_pneumatic_valve.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_powertrain.py` & `prog_models-1.5.1/tests/test_powertrain.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_serialization.py` & `prog_models-1.5.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_sim_result.py` & `prog_models-1.5.1/tests/test_sim_result.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_surrogates.py` & `prog_models-1.5.1/tests/test_surrogates.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,18 +416,18 @@
         self.assertAlmostEqual(surrogate_results.times[-1], surrogate_noise_results.times[-1], delta=20)
         for i in range(min(len(surrogate_results.times), len(surrogate_noise_results.times))):
             self.assertListEqual(list(surrogate_noise_results.inputs[i].keys()), list(surrogate_noise_results.inputs[i].keys()))
             self.assertAlmostEqual(surrogate_noise_results.states[i]['tb'], surrogate_results.states[i]['tb'], delta=10)
             self.assertAlmostEqual(surrogate_noise_results.states[i]['Vo'], surrogate_results.states[i]['Vo'], delta=0.1)
             self.assertAlmostEqual(surrogate_noise_results.states[i]['Vsn'], surrogate_results.states[i]['Vsn'], delta=0.5)
             self.assertAlmostEqual(surrogate_noise_results.states[i]['Vsp'], surrogate_results.states[i]['Vsp'], delta=0.1)
-            self.assertAlmostEqual(surrogate_noise_results.states[i]['qnB'], surrogate_results.states[i]['qnB'], delta=15)
-            self.assertAlmostEqual(surrogate_noise_results.states[i]['qnS'], surrogate_results.states[i]['qnS'], delta=3)
-            self.assertAlmostEqual(surrogate_noise_results.states[i]['qpB'], surrogate_results.states[i]['qpB'], delta=15)
-            self.assertAlmostEqual(surrogate_noise_results.states[i]['qpS'], surrogate_results.states[i]['qpS'], delta=3)
+            self.assertAlmostEqual(surrogate_noise_results.states[i]['qnB'], surrogate_results.states[i]['qnB'], delta=55)
+            self.assertAlmostEqual(surrogate_noise_results.states[i]['qnS'], surrogate_results.states[i]['qnS'], delta=8)
+            self.assertAlmostEqual(surrogate_noise_results.states[i]['qpB'], surrogate_results.states[i]['qpB'], delta=55)
+            self.assertAlmostEqual(surrogate_noise_results.states[i]['qpS'], surrogate_results.states[i]['qpS'], delta=8)
             self.assertAlmostEqual(surrogate_noise_results.states[i]['v'], surrogate_results.states[i]['v'], delta=0.3)
             self.assertAlmostEqual(surrogate_noise_results.states[i]['EOD'], surrogate_results.states[i]['EOD'],delta=0.1)
             self.assertEqual(surrogate_noise_results.states[i]['v'], surrogate_noise_results.outputs[i]['v'])
             self.assertEqual(surrogate_noise_results.states[i]['EOD'], surrogate_noise_results.event_states[i]['EOD'])
             self.assertAlmostEqual(surrogate_noise_results.states[i]['v'], surrogate_results.outputs[i]['v'], delta=0.3)
             self.assertAlmostEqual(surrogate_noise_results.states[i]['EOD'], surrogate_results.event_states[i]['EOD'], delta=0.1)
             if i > 0:
```

### Comparing `prog_models-1.5.0rc2/tests/test_tutorials.py` & `prog_models-1.5.1/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.0rc2/tests/test_uav_model.py` & `prog_models-1.5.1/tests/test_uav_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         sim = vehicle.simulate_to(ref_traj['t'][-1], ctrl, **{'dt': vehicle.parameters['dt'], 'save_freq': vehicle.parameters['dt']})
         x_temp = [sim.outputs[iter]['x'] for iter in range(len(sim.times))]
         y_temp = [sim.outputs[iter]['y'] for iter in range(len(sim.times))]
         z_temp = [sim.outputs[iter]['z'] for iter in range(len(sim.times))]
         x_sim_interp = interp1d(sim.times, x_temp)(ref_traj['t'])
         y_sim_interp = interp1d(sim.times, y_temp)(ref_traj['t'])
         z_sim_interp = interp1d(sim.times, z_temp)(ref_traj['t'])
-        for iter in range(min(len(sim.times), len(ref_traj['t']))):
+        for iter in range(len(ref_traj['t'])):
             self.assertAlmostEqual(ref_traj['x'][iter], x_sim_interp[iter], delta=5)
             self.assertAlmostEqual(ref_traj['y'][iter], y_sim_interp[iter], delta=5)
             self.assertAlmostEqual(ref_traj['z'][iter], z_sim_interp[iter], delta=5)
 
         # Case 2: Speeds provided, no ETAs + LQR_I controller + djis1000 vehicle
         # Define speeds:
         ref_params = {
@@ -264,15 +264,15 @@
         sim_speeds = vehicle_djis.simulate_to(ref_traj_speeds['t'][-1], ctrl_speeds, **{'save_freq': vehicle_djis.parameters['dt']})
         x_speeds_temp = [sim_speeds.outputs[iter]['x'] for iter in range(len(sim_speeds.times))]
         y_speeds_temp = [sim_speeds.outputs[iter]['y'] for iter in range(len(sim_speeds.times))]
         z_speeds_temp = [sim_speeds.outputs[iter]['z'] for iter in range(len(sim_speeds.times))]
         x_speeds_sim_interp = interp1d(sim_speeds.times, x_speeds_temp)(ref_traj_speeds['t'])
         y_speeds_sim_interp = interp1d(sim_speeds.times, y_speeds_temp)(ref_traj_speeds['t'])
         z_speeds_sim_interp = interp1d(sim_speeds.times, z_speeds_temp)(ref_traj_speeds['t'])
-        for iter in range(len(sim_speeds.times)):
+        for iter in range(len(ref_traj_speeds['t'])):
             self.assertAlmostEqual(ref_traj_speeds['x'][iter], x_speeds_sim_interp[iter], delta=8)
             self.assertAlmostEqual(ref_traj_speeds['y'][iter], y_speeds_sim_interp[iter], delta=8)
             self.assertAlmostEqual(ref_traj_speeds['z'][iter], z_speeds_sim_interp[iter], delta=8)
 
         # Reset warnings
         warnings.simplefilter("default", category=UserWarning)
```

