# Comparing `tmp/torchphysics-1.0.0.tar.gz` & `tmp/torchphysics-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchphysics-1.0.0.tar", last modified: Wed Mar 29 13:01:47 2023, max compression
+gzip compressed data, was "torchphysics-1.0.1.tar", last modified: Thu Jul 13 06:51:19 2023, max compression
```

## Comparing `torchphysics-1.0.0.tar` & `torchphysics-1.0.1.tar`

### file list

```diff
@@ -1,231 +1,256 @@
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.460330 torchphysics-1.0.0/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      595 2021-10-04 10:45:13.000000 torchphysics-1.0.0/.coveragerc
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.151743 torchphysics-1.0.0/.githooks/
--rwxr-xr-x   0 tomfre   (58750) tomfre   (58750)      475 2022-02-08 08:28:12.000000 torchphysics-1.0.0/.githooks/prepare-commit-msg
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.025712 torchphysics-1.0.0/.github/
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.156351 torchphysics-1.0.0/.github/workflows/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1342 2021-10-04 10:45:13.000000 torchphysics-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      679 2023-02-14 13:03:25.000000 torchphysics-1.0.0/.gitignore
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      461 2021-10-04 10:45:13.000000 torchphysics-1.0.0/.readthedocs.yml
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      148 2021-10-04 10:45:13.000000 torchphysics-1.0.0/AUTHORS.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      173 2023-03-24 09:25:18.000000 torchphysics-1.0.0/CHANGELOG.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5483 2022-02-08 08:28:12.000000 torchphysics-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11357 2021-10-04 10:45:13.000000 torchphysics-1.0.0/LICENSE.txt
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1263 2022-02-08 08:28:12.000000 torchphysics-1.0.0/NOTICE
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6596 2023-03-29 13:01:47.461610 torchphysics-1.0.0/PKG-INFO
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5755 2022-12-10 10:39:20.000000 torchphysics-1.0.0/README.rst
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.173715 torchphysics-1.0.0/batch_scripts/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      314 2021-10-04 10:45:13.000000 torchphysics-1.0.0/batch_scripts/create_environment.bat
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      313 2022-02-08 08:28:12.000000 torchphysics-1.0.0/batch_scripts/environment.yml
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       80 2022-02-08 08:28:12.000000 torchphysics-1.0.0/batch_scripts/start_Jupyter_notebook.bat
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       65 2021-10-04 10:45:13.000000 torchphysics-1.0.0/batch_scripts/start_spyder.bat
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.215208 torchphysics-1.0.0/docs/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1153 2021-10-04 10:45:13.000000 torchphysics-1.0.0/docs/Makefile
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.219916 torchphysics-1.0.0/docs/_static/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       18 2021-10-04 10:45:13.000000 torchphysics-1.0.0/docs/_static/.gitignore
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       41 2021-10-04 10:45:13.000000 torchphysics-1.0.0/docs/authors.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       43 2021-10-04 10:45:13.000000 torchphysics-1.0.0/docs/changelog.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9737 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/conf.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5537 2022-12-03 09:10:12.000000 torchphysics-1.0.0/docs/examples.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2256 2022-02-28 18:15:06.000000 torchphysics-1.0.0/docs/index.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       67 2021-10-04 10:45:13.000000 torchphysics-1.0.0/docs/license.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       39 2021-10-04 10:45:13.000000 torchphysics-1.0.0/docs/readme.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      428 2022-06-29 10:52:11.000000 torchphysics-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.379729 torchphysics-1.0.0/docs/tutorial/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5748 2022-11-24 20:13:48.000000 torchphysics-1.0.0/docs/tutorial/condition_tutorial.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3415 2022-02-27 13:33:49.000000 torchphysics-1.0.0/docs/tutorial/differentialoperators.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4174 2022-02-27 13:23:32.000000 torchphysics-1.0.0/docs/tutorial/external_domains.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3421 2022-02-27 13:28:42.000000 torchphysics-1.0.0/docs/tutorial/model_creation.rst
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.453324 torchphysics-1.0.0/docs/tutorial/pictures/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    49789 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/L_domain.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13077 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/L_slice.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    53461 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/complex_domain.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    55491 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/cylinder.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    36261 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/error.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    34488 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/operation.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10693 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/polygon.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    25175 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/rect_circle_domain.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   621591 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/sampler_combis.PNG
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    31720 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/simplex.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    25172 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/solution.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    69882 2022-02-08 08:28:12.000000 torchphysics-1.0.0/docs/tutorial/pictures/torchphysics_structure.png
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2934 2022-02-27 13:35:37.000000 torchphysics-1.0.0/docs/tutorial/plotting.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6269 2022-11-24 19:53:15.000000 torchphysics-1.0.0/docs/tutorial/sampler_tutorial.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9130 2022-12-10 10:20:38.000000 torchphysics-1.0.0/docs/tutorial/solve_pde.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3501 2022-11-25 13:43:27.000000 torchphysics-1.0.0/docs/tutorial/solver_info.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5314 2022-02-27 13:20:10.000000 torchphysics-1.0.0/docs/tutorial/tutorial_domain_basics.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3360 2022-02-27 13:17:17.000000 torchphysics-1.0.0/docs/tutorial/tutorial_spaces_and_points.rst
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3092 2022-11-25 13:45:12.000000 torchphysics-1.0.0/docs/tutorial/tutorial_start.rst
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.459392 torchphysics-1.0.0/examples/
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.470044 torchphysics-1.0.0/examples/deeponet/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    48284 2022-10-27 13:03:43.000000 torchphysics-1.0.0/examples/deeponet/ode.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    62489 2022-10-27 13:29:44.000000 torchphysics-1.0.0/examples/deeponet/oscillator.ipynb
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.482361 torchphysics-1.0.0/examples/deepritz/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    47527 2022-12-22 14:03:11.000000 torchphysics-1.0.0/examples/deepritz/corner_pde.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   122885 2022-02-08 08:28:12.000000 torchphysics-1.0.0/examples/deepritz/poisson-equation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5435 2022-02-08 08:28:12.000000 torchphysics-1.0.0/examples/fdm_heat_equation.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.615825 torchphysics-1.0.0/examples/pinn/
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.622100 torchphysics-1.0.0/examples/pinn/data/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)  2743520 2022-02-11 09:06:37.000000 torchphysics-1.0.0/examples/pinn/data/heat-eq-inverse-data.npy
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    36854 2022-06-27 14:51:24.000000 torchphysics-1.0.0/examples/pinn/exp-function-with-param.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   159562 2022-12-08 10:19:42.000000 torchphysics-1.0.0/examples/pinn/hard-constrains.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   319501 2023-02-17 13:04:31.000000 torchphysics-1.0.0/examples/pinn/heat-equation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   137289 2022-12-10 10:11:19.000000 torchphysics-1.0.0/examples/pinn/interface-jump.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)  2270511 2023-02-14 13:03:04.000000 torchphysics-1.0.0/examples/pinn/inverse-heat-eq.gif
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   129923 2022-02-14 12:02:55.000000 torchphysics-1.0.0/examples/pinn/inverse-heat-equation-D-function.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    43125 2022-02-08 08:28:12.000000 torchphysics-1.0.0/examples/pinn/inverse-heat-equation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   545785 2022-08-29 11:27:04.000000 torchphysics-1.0.0/examples/pinn/moving-heat-eq.gif
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    76239 2022-06-27 12:52:35.000000 torchphysics-1.0.0/examples/pinn/moving-heat-equation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    38491 2022-03-07 09:08:10.000000 torchphysics-1.0.0/examples/pinn/periodic-boundary-problem.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   894932 2022-02-08 08:28:13.000000 torchphysics-1.0.0/examples/pinn/poisson-equation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    63548 2022-02-08 08:28:13.000000 torchphysics-1.0.0/examples/pinn/poisson-with-input-params.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    51323 2022-02-09 09:25:14.000000 torchphysics-1.0.0/examples/pinn/signorini-equation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    45111 2022-03-04 20:41:47.000000 torchphysics-1.0.0/examples/pinn/singular-boundary-problem.ipynb
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.696819 torchphysics-1.0.0/examples/tutorial/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   196935 2023-03-10 07:39:00.000000 torchphysics-1.0.0/examples/tutorial/Introduction_Tutorial_PINNs.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1084 2022-02-08 08:28:13.000000 torchphysics-1.0.0/examples/tutorial/L_plate.stl
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    36539 2023-03-10 07:39:00.000000 torchphysics-1.0.0/examples/tutorial/Tutorial_PINNs_Parameter_Dependency.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7888 2022-02-08 08:28:13.000000 torchphysics-1.0.0/examples/tutorial/domain_creation.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6692 2022-02-08 08:28:13.000000 torchphysics-1.0.0/examples/tutorial/polygons_external_objects.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    83220 2023-01-05 18:58:48.000000 torchphysics-1.0.0/examples/tutorial/solve_pde.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    75057 2023-01-02 14:34:09.000000 torchphysics-1.0.0/examples/tutorial/solve_pde_drm.ipynb
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.703527 torchphysics-1.0.0/experiments/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   115121 2022-10-14 10:52:29.000000 torchphysics-1.0.0/experiments/burgers_equation.ipynb
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.758162 torchphysics-1.0.0/experiments/geometry/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    27884 2021-10-04 10:45:13.000000 torchphysics-1.0.0/experiments/geometry/d20_voll.stl
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   772540 2021-10-04 10:45:13.000000 torchphysics-1.0.0/experiments/geometry/heat_equation_D=10.gif
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   721390 2021-10-04 10:45:13.000000 torchphysics-1.0.0/experiments/geometry/heat_equation_bearing.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)   758574 2021-10-04 10:45:13.000000 torchphysics-1.0.0/experiments/geometry/heat_equation_bearing_orig.ipynb
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8084 2021-10-04 10:45:13.000000 torchphysics-1.0.0/experiments/geometry/spalt_ex2_01.stl
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      313 2023-03-24 08:34:43.000000 torchphysics-1.0.0/pyproject.toml
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      179 2022-05-26 14:50:43.000000 torchphysics-1.0.0/requirements.txt
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1683 2023-03-29 13:01:47.466919 torchphysics-1.0.0/setup.cfg
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      732 2023-03-24 08:28:24.000000 torchphysics-1.0.0/setup.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.051275 torchphysics-1.0.0/src/
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.766227 torchphysics-1.0.0/src/torchphysics/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      790 2023-03-24 09:35:58.000000 torchphysics-1.0.0/src/torchphysics/__init__.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.827065 torchphysics-1.0.0/src/torchphysics/models/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1072 2023-03-24 09:05:40.000000 torchphysics-1.0.0/src/torchphysics/models/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2581 2022-06-27 14:08:42.000000 torchphysics-1.0.0/src/torchphysics/models/activation_fn.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.845411 torchphysics-1.0.0/src/torchphysics/models/deeponet/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10656 2023-02-06 14:21:21.000000 torchphysics-1.0.0/src/torchphysics/models/deeponet/branchnets.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4083 2022-10-27 08:53:21.000000 torchphysics-1.0.0/src/torchphysics/models/deeponet/deeponet.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4370 2022-10-27 13:06:50.000000 torchphysics-1.0.0/src/torchphysics/models/deeponet/layers.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5176 2022-10-27 12:32:05.000000 torchphysics-1.0.0/src/torchphysics/models/deeponet/trunknets.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1730 2022-06-27 08:38:07.000000 torchphysics-1.0.0/src/torchphysics/models/deepritz.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6043 2022-10-25 09:23:33.000000 torchphysics-1.0.0/src/torchphysics/models/fcn.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4991 2022-06-27 08:38:07.000000 torchphysics-1.0.0/src/torchphysics/models/model.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10190 2023-02-17 13:05:35.000000 torchphysics-1.0.0/src/torchphysics/models/newmodel.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1214 2022-02-08 08:28:13.000000 torchphysics-1.0.0/src/torchphysics/models/parameter.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4460 2022-05-02 08:07:33.000000 torchphysics-1.0.0/src/torchphysics/models/qres.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.849387 torchphysics-1.0.0/src/torchphysics/problem/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      136 2022-02-08 08:28:13.000000 torchphysics-1.0.0/src/torchphysics/problem/__init__.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.863963 torchphysics-1.0.0/src/torchphysics/problem/conditions/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      972 2022-06-07 16:14:59.000000 torchphysics-1.0.0/src/torchphysics/problem/conditions/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    31732 2023-02-06 13:07:08.000000 torchphysics-1.0.0/src/torchphysics/problem/conditions/condition.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8179 2023-02-06 14:21:00.000000 torchphysics-1.0.0/src/torchphysics/problem/conditions/deeponet_condition.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.872917 torchphysics-1.0.0/src/torchphysics/problem/domains/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1727 2022-09-05 12:01:21.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11520 2022-02-27 13:37:36.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.882215 torchphysics-1.0.0/src/torchphysics/problem/domains/domain0D/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       24 2023-03-24 09:05:54.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain0D/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3350 2022-09-27 10:35:02.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain0D/point.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.923555 torchphysics-1.0.0/src/torchphysics/problem/domains/domain1D/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       30 2023-03-24 09:05:32.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain1D/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7554 2022-09-27 10:35:12.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain1D/interval.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.946650 torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      143 2023-03-24 09:06:17.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6690 2022-09-27 10:35:24.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/circle.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13446 2022-09-27 10:35:29.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/parallelogram.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13074 2023-01-26 10:06:48.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/shapely_polygon.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    14213 2022-09-27 10:35:35.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/triangle.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.960304 torchphysics-1.0.0/src/torchphysics/problem/domains/domain3D/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       26 2023-03-24 09:05:34.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain3D/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8041 2022-09-27 10:35:39.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain3D/sphere.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10552 2022-07-07 18:19:10.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domain3D/trimesh_polyhedron.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.994204 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8073 2022-02-21 12:06:25.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/cut.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7924 2022-02-21 12:06:25.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/intersection.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11624 2023-03-24 09:05:51.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/product.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9126 2022-09-27 10:35:44.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/rotate.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11526 2022-03-08 08:27:46.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/sampler_helper.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4226 2022-09-27 10:35:51.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/translate.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11351 2022-02-21 12:06:25.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/union.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.004464 torchphysics-1.0.0/src/torchphysics/problem/domains/functionsets/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      129 2022-05-26 13:02:10.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/functionsets/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7315 2022-10-27 08:20:03.000000 torchphysics-1.0.0/src/torchphysics/problem/domains/functionsets/functionset.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.032347 torchphysics-1.0.0/src/torchphysics/problem/samplers/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2114 2022-05-18 07:24:22.000000 torchphysics-1.0.0/src/torchphysics/problem/samplers/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1163 2022-03-03 20:48:24.000000 torchphysics-1.0.0/src/torchphysics/problem/samplers/data_samplers.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6698 2023-03-24 09:05:43.000000 torchphysics-1.0.0/src/torchphysics/problem/samplers/grid_samplers.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9416 2022-06-27 14:38:21.000000 torchphysics-1.0.0/src/torchphysics/problem/samplers/plot_samplers.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    14558 2022-05-18 07:24:22.000000 torchphysics-1.0.0/src/torchphysics/problem/samplers/random_samplers.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    15744 2023-01-02 10:24:04.000000 torchphysics-1.0.0/src/torchphysics/problem/samplers/sampler_base.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.051857 torchphysics-1.0.0/src/torchphysics/problem/spaces/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      599 2022-09-21 08:58:41.000000 torchphysics-1.0.0/src/torchphysics/problem/spaces/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      590 2022-05-04 09:24:12.000000 torchphysics-1.0.0/src/torchphysics/problem/spaces/functionspace.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    12217 2022-09-05 11:31:30.000000 torchphysics-1.0.0/src/torchphysics/problem/spaces/points.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6355 2022-09-25 11:53:10.000000 torchphysics-1.0.0/src/torchphysics/problem/spaces/space.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4740 2022-09-23 18:43:50.000000 torchphysics-1.0.0/src/torchphysics/solver.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.261525 torchphysics-1.0.0/src/torchphysics/utils/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1143 2023-01-18 14:04:10.000000 torchphysics-1.0.0/src/torchphysics/utils/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6456 2023-01-18 14:28:26.000000 torchphysics-1.0.0/src/torchphysics/utils/callbacks.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.276384 torchphysics-1.0.0/src/torchphysics/utils/data/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      107 2022-10-27 09:57:41.000000 torchphysics-1.0.0/src/torchphysics/utils/data/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3455 2022-10-27 11:25:30.000000 torchphysics-1.0.0/src/torchphysics/utils/data/dataloader.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    12929 2023-01-20 11:42:25.000000 torchphysics-1.0.0/src/torchphysics/utils/data/deeponet_dataloader.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    14931 2022-09-21 08:44:40.000000 torchphysics-1.0.0/src/torchphysics/utils/differentialoperators.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2037 2022-02-08 08:28:13.000000 torchphysics-1.0.0/src/torchphysics/utils/evaluation.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.297423 torchphysics-1.0.0/src/torchphysics/utils/plotting/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      445 2022-06-27 12:48:09.000000 torchphysics-1.0.0/src/torchphysics/utils/plotting/__init__.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    16158 2022-09-26 07:36:14.000000 torchphysics-1.0.0/src/torchphysics/utils/plotting/animation.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    16950 2022-09-26 07:35:16.000000 torchphysics-1.0.0/src/torchphysics/utils/plotting/plot_functions.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2321 2022-02-08 08:28:13.000000 torchphysics-1.0.0/src/torchphysics/utils/plotting/scatter_points.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11304 2022-09-05 11:13:00.000000 torchphysics-1.0.0/src/torchphysics/utils/user_fun.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:46.792337 torchphysics-1.0.0/src/torchphysics.egg-info/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6596 2023-03-29 13:01:45.000000 torchphysics-1.0.0/src/torchphysics.egg-info/PKG-INFO
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7117 2023-03-29 13:01:46.000000 torchphysics-1.0.0/src/torchphysics.egg-info/SOURCES.txt
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)        1 2023-03-29 13:01:45.000000 torchphysics-1.0.0/src/torchphysics.egg-info/dependency_links.txt
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)        1 2021-10-04 10:53:43.000000 torchphysics-1.0.0/src/torchphysics.egg-info/not-zip-safe
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      250 2023-03-29 13:01:45.000000 torchphysics-1.0.0/src/torchphysics.egg-info/requires.txt
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)       13 2023-03-29 13:01:45.000000 torchphysics-1.0.0/src/torchphysics.egg-info/top_level.txt
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.340163 torchphysics-1.0.0/tests/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      280 2021-10-04 10:45:13.000000 torchphysics-1.0.0/tests/conftest.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8886 2022-05-26 13:02:10.000000 torchphysics-1.0.0/tests/test_conditions.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1828 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/test_data_utils.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    27934 2022-09-21 08:50:05.000000 torchphysics-1.0.0/tests/test_differentialoperators.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1170 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/test_evaluation.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10053 2022-04-12 07:41:01.000000 torchphysics-1.0.0/tests/test_points.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    18503 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/test_samplers.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2587 2022-09-25 11:56:09.000000 torchphysics-1.0.0/tests/test_spaces.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5216 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/test_user_function.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.393153 torchphysics-1.0.0/tests/tests_domain/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6683 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain0D.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11461 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain1D.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    34547 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain2D.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8733 2022-02-21 12:06:25.000000 torchphysics-1.0.0/tests/tests_domain/test_domain2D_shapely.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9296 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain3D.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11036 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain3D_trimesh.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13264 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain_cut.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11755 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain_intersection.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7469 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain_product.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    12938 2022-09-05 14:16:09.000000 torchphysics-1.0.0/tests/tests_domain/test_domain_tranforms.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11495 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_domain/test_domain_union.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.399251 torchphysics-1.0.0/tests/tests_functionsets/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5416 2022-06-01 11:42:37.000000 torchphysics-1.0.0/tests/tests_functionsets/test_FunctionSetMain.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.431976 torchphysics-1.0.0/tests/tests_models/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1948 2022-06-27 14:09:27.000000 torchphysics-1.0.0/tests/tests_models/test_activation_fn.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8167 2022-10-27 09:31:11.000000 torchphysics-1.0.0/tests/tests_models/test_deep_o_net.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1199 2022-04-12 07:33:39.000000 torchphysics-1.0.0/tests/tests_models/test_deepritz.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2663 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_models/test_fcn.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5525 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_models/test_model_base.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      524 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_models/test_parameters.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3024 2022-02-15 08:38:25.000000 torchphysics-1.0.0/tests/tests_models/test_qres.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.446588 torchphysics-1.0.0/tests/tests_plots/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13094 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_plots/test_animation.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9177 2022-06-27 12:47:07.000000 torchphysics-1.0.0/tests/tests_plots/test_plot.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      892 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_plots/test_scatter.py
-drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-03-29 13:01:47.455919 torchphysics-1.0.0/tests/tests_solver/
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2211 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_solver/test_solver.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)      163 2022-02-08 08:28:13.000000 torchphysics-1.0.0/tests/tests_solver/test_training.py
--rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2010 2021-10-04 10:45:14.000000 torchphysics-1.0.0/tox.ini
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.269332 torchphysics-1.0.1/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      595 2021-10-04 10:45:13.000000 torchphysics-1.0.1/.coveragerc
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.167467 torchphysics-1.0.1/.githooks/
+-rwxr-xr-x   0 tomfre   (58750) tomfre   (58750)      475 2022-02-08 08:28:12.000000 torchphysics-1.0.1/.githooks/prepare-commit-msg
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.030749 torchphysics-1.0.1/.github/
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.179837 torchphysics-1.0.1/.github/workflows/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1342 2021-10-04 10:45:13.000000 torchphysics-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      679 2023-07-12 08:40:02.000000 torchphysics-1.0.1/.gitignore
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      461 2021-10-04 10:45:13.000000 torchphysics-1.0.1/.readthedocs.yml
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      148 2021-10-04 10:45:13.000000 torchphysics-1.0.1/AUTHORS.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      346 2023-07-12 09:22:48.000000 torchphysics-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5483 2022-02-08 08:28:12.000000 torchphysics-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11357 2021-10-04 10:45:13.000000 torchphysics-1.0.1/LICENSE.txt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1263 2022-02-08 08:28:12.000000 torchphysics-1.0.1/NOTICE
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7126 2023-07-13 06:51:19.270434 torchphysics-1.0.1/PKG-INFO
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6285 2023-06-12 09:41:13.000000 torchphysics-1.0.1/README.rst
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.214276 torchphysics-1.0.1/batch_scripts/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      314 2021-10-04 10:45:13.000000 torchphysics-1.0.1/batch_scripts/create_environment.bat
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      313 2022-02-08 08:28:12.000000 torchphysics-1.0.1/batch_scripts/environment.yml
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       80 2022-02-08 08:28:12.000000 torchphysics-1.0.1/batch_scripts/start_Jupyter_notebook.bat
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       65 2021-10-04 10:45:13.000000 torchphysics-1.0.1/batch_scripts/start_spyder.bat
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.280365 torchphysics-1.0.1/docs/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1153 2021-10-04 10:45:13.000000 torchphysics-1.0.1/docs/Makefile
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.297923 torchphysics-1.0.1/docs/_static/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       18 2021-10-04 10:45:13.000000 torchphysics-1.0.1/docs/_static/.gitignore
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       41 2021-10-04 10:45:13.000000 torchphysics-1.0.1/docs/authors.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       43 2021-10-04 10:45:13.000000 torchphysics-1.0.1/docs/changelog.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9737 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/conf.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5537 2022-12-03 09:10:12.000000 torchphysics-1.0.1/docs/examples.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2251 2023-05-22 12:37:55.000000 torchphysics-1.0.1/docs/index.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       67 2021-10-04 10:45:13.000000 torchphysics-1.0.1/docs/license.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       39 2021-10-04 10:45:13.000000 torchphysics-1.0.1/docs/readme.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      428 2022-06-29 10:52:11.000000 torchphysics-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.690307 torchphysics-1.0.1/docs/tutorial/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2359 2023-05-22 12:37:32.000000 torchphysics-1.0.1/docs/tutorial/applied_tutorial_start.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5748 2022-11-24 20:13:48.000000 torchphysics-1.0.1/docs/tutorial/condition_tutorial.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3415 2022-02-27 13:33:49.000000 torchphysics-1.0.1/docs/tutorial/differentialoperators.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4174 2022-02-27 13:23:32.000000 torchphysics-1.0.1/docs/tutorial/external_domains.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2114 2023-05-22 12:13:00.000000 torchphysics-1.0.1/docs/tutorial/main_page.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3421 2022-02-27 13:28:42.000000 torchphysics-1.0.1/docs/tutorial/model_creation.rst
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.959345 torchphysics-1.0.1/docs/tutorial/pictures/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    49789 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/L_domain.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13077 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/L_slice.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    53461 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/complex_domain.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    55491 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/cylinder.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    36261 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/error.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    34488 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/operation.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10693 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/polygon.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    25175 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/rect_circle_domain.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   621591 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/sampler_combis.PNG
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    31720 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/simplex.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    25172 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/solution.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    69882 2022-02-08 08:28:12.000000 torchphysics-1.0.1/docs/tutorial/pictures/torchphysics_structure.png
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2934 2022-02-27 13:35:37.000000 torchphysics-1.0.1/docs/tutorial/plotting.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6269 2022-11-24 19:53:15.000000 torchphysics-1.0.1/docs/tutorial/sampler_tutorial.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9130 2022-12-10 10:20:38.000000 torchphysics-1.0.1/docs/tutorial/solve_pde.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3501 2022-11-25 13:43:27.000000 torchphysics-1.0.1/docs/tutorial/solver_info.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5314 2022-02-27 13:20:10.000000 torchphysics-1.0.1/docs/tutorial/tutorial_domain_basics.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3360 2022-02-27 13:17:17.000000 torchphysics-1.0.1/docs/tutorial/tutorial_spaces_and_points.rst
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3092 2022-11-25 13:45:12.000000 torchphysics-1.0.1/docs/tutorial/tutorial_start.rst
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.971703 torchphysics-1.0.1/examples/
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.013612 torchphysics-1.0.1/examples/deeponet/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    55272 2023-05-22 14:11:07.000000 torchphysics-1.0.1/examples/deeponet/inverse_ode.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    47462 2023-05-22 14:13:55.000000 torchphysics-1.0.1/examples/deeponet/ode.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    67699 2023-05-22 14:30:58.000000 torchphysics-1.0.1/examples/deeponet/oscillator.ipynb
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.059125 torchphysics-1.0.1/examples/deepritz/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    47527 2022-12-22 14:03:11.000000 torchphysics-1.0.1/examples/deepritz/corner_pde.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   122885 2022-02-08 08:28:12.000000 torchphysics-1.0.1/examples/deepritz/poisson-equation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5435 2022-02-08 08:28:12.000000 torchphysics-1.0.1/examples/fdm_heat_equation.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.353251 torchphysics-1.0.1/examples/pinn/
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.359666 torchphysics-1.0.1/examples/pinn/data/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)  2743520 2022-02-11 09:06:37.000000 torchphysics-1.0.1/examples/pinn/data/heat-eq-inverse-data.npy
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    36854 2022-06-27 14:51:24.000000 torchphysics-1.0.1/examples/pinn/exp-function-with-param.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   159562 2022-12-08 10:19:42.000000 torchphysics-1.0.1/examples/pinn/hard-constrains.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   319501 2023-02-17 13:04:31.000000 torchphysics-1.0.1/examples/pinn/heat-equation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   137289 2022-12-10 10:11:19.000000 torchphysics-1.0.1/examples/pinn/interface-jump.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)  2270511 2023-02-14 13:03:04.000000 torchphysics-1.0.1/examples/pinn/inverse-heat-eq.gif
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   129923 2022-02-14 12:02:55.000000 torchphysics-1.0.1/examples/pinn/inverse-heat-equation-D-function.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    43125 2023-07-12 09:20:02.000000 torchphysics-1.0.1/examples/pinn/inverse-heat-equation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   545785 2022-08-29 11:27:04.000000 torchphysics-1.0.1/examples/pinn/moving-heat-eq.gif
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    76239 2022-06-27 12:52:35.000000 torchphysics-1.0.1/examples/pinn/moving-heat-equation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    38491 2022-03-07 09:08:10.000000 torchphysics-1.0.1/examples/pinn/periodic-boundary-problem.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   894932 2022-02-08 08:28:13.000000 torchphysics-1.0.1/examples/pinn/poisson-equation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    63548 2022-02-08 08:28:13.000000 torchphysics-1.0.1/examples/pinn/poisson-with-input-params.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    51323 2022-02-09 09:25:14.000000 torchphysics-1.0.1/examples/pinn/signorini-equation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    45111 2022-03-04 20:41:47.000000 torchphysics-1.0.1/examples/pinn/singular-boundary-problem.ipynb
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.468557 torchphysics-1.0.1/examples/tutorial/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   196935 2023-03-10 07:39:00.000000 torchphysics-1.0.1/examples/tutorial/Introduction_Tutorial_PINNs.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1084 2022-02-08 08:28:13.000000 torchphysics-1.0.1/examples/tutorial/L_plate.stl
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    36539 2023-03-10 07:39:00.000000 torchphysics-1.0.1/examples/tutorial/Tutorial_PINNs_Parameter_Dependency.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7888 2022-02-08 08:28:13.000000 torchphysics-1.0.1/examples/tutorial/domain_creation.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6692 2022-02-08 08:28:13.000000 torchphysics-1.0.1/examples/tutorial/polygons_external_objects.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    83220 2023-01-05 18:58:48.000000 torchphysics-1.0.1/examples/tutorial/solve_pde.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    75057 2023-01-02 14:34:09.000000 torchphysics-1.0.1/examples/tutorial/solve_pde_drm.ipynb
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.546620 torchphysics-1.0.1/examples/workshop/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    12529 2023-07-04 09:25:16.000000 torchphysics-1.0.1/examples/workshop/Exercise1_1.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7511 2023-07-04 07:55:57.000000 torchphysics-1.0.1/examples/workshop/Exercise1_2.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8530 2023-07-03 18:15:17.000000 torchphysics-1.0.1/examples/workshop/Exercise1_3.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5637 2023-07-10 13:58:32.000000 torchphysics-1.0.1/examples/workshop/Exercise2_1.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    21668 2023-07-12 08:37:19.000000 torchphysics-1.0.1/examples/workshop/Exercise2_2.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4955 2023-07-12 08:53:50.000000 torchphysics-1.0.1/examples/workshop/Exercise3_1.ipynb
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.055867 torchphysics-1.0.1/examples/workshop/FEMData/
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.566596 torchphysics-1.0.1/examples/workshop/FEMData/Data2_2/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5099 2023-07-10 18:13:19.000000 torchphysics-1.0.1/examples/workshop/FEMData/Data2_2/space_coords.pt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    90283 2023-07-10 18:13:40.000000 torchphysics-1.0.1/examples/workshop/FEMData/Data2_2/temperature.pt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      875 2023-07-10 18:13:56.000000 torchphysics-1.0.1/examples/workshop/FEMData/Data2_2/time_points.pt
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.579787 torchphysics-1.0.1/examples/workshop/FEMData/Data2_3/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1259 2023-07-12 08:23:59.000000 torchphysics-1.0.1/examples/workshop/FEMData/Data2_3/space_coords.pt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1515 2023-07-12 08:23:05.000000 torchphysics-1.0.1/examples/workshop/FEMData/Data2_3/time_points.pt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   105259 2023-07-12 08:20:18.000000 torchphysics-1.0.1/examples/workshop/FEMData/Data2_3/wave_data.pt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1645 2023-07-10 13:23:35.000000 torchphysics-1.0.1/examples/workshop/Lecture_Example.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    63328 2023-07-02 16:59:05.000000 torchphysics-1.0.1/examples/workshop/Sol1_2.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    58143 2023-07-06 14:25:25.000000 torchphysics-1.0.1/examples/workshop/Sol1_3.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    54993 2023-07-05 14:23:26.000000 torchphysics-1.0.1/examples/workshop/Sol2_1.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   146675 2023-07-12 08:25:28.000000 torchphysics-1.0.1/examples/workshop/Sol2_2.ipynb
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.585822 torchphysics-1.0.1/experiments/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   115121 2022-10-14 10:52:29.000000 torchphysics-1.0.1/experiments/burgers_equation.ipynb
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.750854 torchphysics-1.0.1/experiments/geometry/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    27884 2021-10-04 10:45:13.000000 torchphysics-1.0.1/experiments/geometry/d20_voll.stl
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   772540 2021-10-04 10:45:13.000000 torchphysics-1.0.1/experiments/geometry/heat_equation_D=10.gif
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   721390 2021-10-04 10:45:13.000000 torchphysics-1.0.1/experiments/geometry/heat_equation_bearing.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)   758574 2021-10-04 10:45:13.000000 torchphysics-1.0.1/experiments/geometry/heat_equation_bearing_orig.ipynb
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8084 2021-10-04 10:45:13.000000 torchphysics-1.0.1/experiments/geometry/spalt_ex2_01.stl
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      313 2023-03-24 08:34:43.000000 torchphysics-1.0.1/pyproject.toml
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      179 2022-05-26 14:50:43.000000 torchphysics-1.0.1/requirements.txt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1683 2023-07-13 06:51:19.274429 torchphysics-1.0.1/setup.cfg
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      732 2023-03-24 08:28:24.000000 torchphysics-1.0.1/setup.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:17.063331 torchphysics-1.0.1/src/
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.760747 torchphysics-1.0.1/src/torchphysics/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      790 2023-03-24 09:35:58.000000 torchphysics-1.0.1/src/torchphysics/__init__.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.830805 torchphysics-1.0.1/src/torchphysics/models/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2830 2023-06-29 19:22:30.000000 torchphysics-1.0.1/src/torchphysics/models/FNO.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1072 2023-03-24 09:05:40.000000 torchphysics-1.0.1/src/torchphysics/models/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2581 2022-06-27 14:08:42.000000 torchphysics-1.0.1/src/torchphysics/models/activation_fn.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.848378 torchphysics-1.0.1/src/torchphysics/models/deeponet/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10992 2023-06-09 09:00:13.000000 torchphysics-1.0.1/src/torchphysics/models/deeponet/branchnets.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4799 2023-06-09 08:49:46.000000 torchphysics-1.0.1/src/torchphysics/models/deeponet/deeponet.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4370 2022-10-27 13:06:50.000000 torchphysics-1.0.1/src/torchphysics/models/deeponet/layers.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5127 2023-05-22 14:24:05.000000 torchphysics-1.0.1/src/torchphysics/models/deeponet/trunknets.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1730 2022-06-27 08:38:07.000000 torchphysics-1.0.1/src/torchphysics/models/deepritz.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6043 2022-10-25 09:23:33.000000 torchphysics-1.0.1/src/torchphysics/models/fcn.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4991 2022-06-27 08:38:07.000000 torchphysics-1.0.1/src/torchphysics/models/model.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10190 2023-02-17 13:05:35.000000 torchphysics-1.0.1/src/torchphysics/models/newmodel.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1214 2022-02-08 08:28:13.000000 torchphysics-1.0.1/src/torchphysics/models/parameter.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4460 2022-05-02 08:07:33.000000 torchphysics-1.0.1/src/torchphysics/models/qres.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.852532 torchphysics-1.0.1/src/torchphysics/problem/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      136 2022-02-08 08:28:13.000000 torchphysics-1.0.1/src/torchphysics/problem/__init__.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.865976 torchphysics-1.0.1/src/torchphysics/problem/conditions/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      972 2022-06-07 16:14:59.000000 torchphysics-1.0.1/src/torchphysics/problem/conditions/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    31612 2023-05-22 14:31:49.000000 torchphysics-1.0.1/src/torchphysics/problem/conditions/condition.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8179 2023-02-06 14:21:00.000000 torchphysics-1.0.1/src/torchphysics/problem/conditions/deeponet_condition.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.875097 torchphysics-1.0.1/src/torchphysics/problem/domains/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1727 2022-09-05 12:01:21.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11520 2022-02-27 13:37:36.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.884469 torchphysics-1.0.1/src/torchphysics/problem/domains/domain0D/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       24 2023-03-24 09:05:54.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain0D/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3350 2022-09-27 10:35:02.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain0D/point.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.893643 torchphysics-1.0.1/src/torchphysics/problem/domains/domain1D/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       30 2023-03-24 09:05:32.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain1D/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7554 2022-09-27 10:35:12.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain1D/interval.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.919157 torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      143 2023-03-24 09:06:17.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6690 2022-09-27 10:35:24.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/circle.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13446 2022-09-27 10:35:29.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/parallelogram.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13074 2023-01-26 10:06:48.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/shapely_polygon.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    14213 2022-09-27 10:35:35.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/triangle.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.934603 torchphysics-1.0.1/src/torchphysics/problem/domains/domain3D/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       26 2023-03-24 09:05:34.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain3D/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8041 2022-09-27 10:35:39.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain3D/sphere.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10552 2022-07-07 18:19:10.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domain3D/trimesh_polyhedron.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.970330 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8073 2022-02-21 12:06:25.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/cut.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7924 2022-02-21 12:06:25.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/intersection.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11624 2023-03-24 09:05:51.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/product.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9126 2022-09-27 10:35:44.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/rotate.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11526 2022-03-08 08:27:46.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/sampler_helper.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4226 2022-09-27 10:35:51.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/translate.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11351 2022-02-21 12:06:25.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/union.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.980468 torchphysics-1.0.1/src/torchphysics/problem/domains/functionsets/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      129 2022-05-26 13:02:10.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/functionsets/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7315 2022-10-27 08:20:03.000000 torchphysics-1.0.1/src/torchphysics/problem/domains/functionsets/functionset.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.008555 torchphysics-1.0.1/src/torchphysics/problem/samplers/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2114 2022-05-18 07:24:22.000000 torchphysics-1.0.1/src/torchphysics/problem/samplers/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1163 2022-03-03 20:48:24.000000 torchphysics-1.0.1/src/torchphysics/problem/samplers/data_samplers.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6698 2023-03-24 09:05:43.000000 torchphysics-1.0.1/src/torchphysics/problem/samplers/grid_samplers.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9416 2022-06-27 14:38:21.000000 torchphysics-1.0.1/src/torchphysics/problem/samplers/plot_samplers.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    14558 2022-05-18 07:24:22.000000 torchphysics-1.0.1/src/torchphysics/problem/samplers/random_samplers.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    15744 2023-01-02 10:24:04.000000 torchphysics-1.0.1/src/torchphysics/problem/samplers/sampler_base.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.046543 torchphysics-1.0.1/src/torchphysics/problem/spaces/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      599 2022-09-21 08:58:41.000000 torchphysics-1.0.1/src/torchphysics/problem/spaces/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      590 2022-05-04 09:24:12.000000 torchphysics-1.0.1/src/torchphysics/problem/spaces/functionspace.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    12317 2023-07-07 19:59:45.000000 torchphysics-1.0.1/src/torchphysics/problem/spaces/points.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6355 2022-09-25 11:53:10.000000 torchphysics-1.0.1/src/torchphysics/problem/spaces/space.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     4740 2022-09-23 18:43:50.000000 torchphysics-1.0.1/src/torchphysics/solver.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.073126 torchphysics-1.0.1/src/torchphysics/utils/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1143 2023-01-18 14:04:10.000000 torchphysics-1.0.1/src/torchphysics/utils/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6456 2023-01-18 14:28:26.000000 torchphysics-1.0.1/src/torchphysics/utils/callbacks.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.086099 torchphysics-1.0.1/src/torchphysics/utils/data/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      107 2022-10-27 09:57:41.000000 torchphysics-1.0.1/src/torchphysics/utils/data/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3455 2022-10-27 11:25:30.000000 torchphysics-1.0.1/src/torchphysics/utils/data/dataloader.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13562 2023-06-09 08:58:36.000000 torchphysics-1.0.1/src/torchphysics/utils/data/deeponet_dataloader.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    14931 2023-05-17 09:28:59.000000 torchphysics-1.0.1/src/torchphysics/utils/differentialoperators.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2037 2022-02-08 08:28:13.000000 torchphysics-1.0.1/src/torchphysics/utils/evaluation.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.104448 torchphysics-1.0.1/src/torchphysics/utils/plotting/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      445 2022-06-27 12:48:09.000000 torchphysics-1.0.1/src/torchphysics/utils/plotting/__init__.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    16158 2022-09-26 07:36:14.000000 torchphysics-1.0.1/src/torchphysics/utils/plotting/animation.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    16950 2022-09-26 07:35:16.000000 torchphysics-1.0.1/src/torchphysics/utils/plotting/plot_functions.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2321 2022-02-08 08:28:13.000000 torchphysics-1.0.1/src/torchphysics/utils/plotting/scatter_points.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11306 2023-05-25 08:31:08.000000 torchphysics-1.0.1/src/torchphysics/utils/user_fun.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:18.789884 torchphysics-1.0.1/src/torchphysics.egg-info/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7126 2023-07-13 06:51:16.000000 torchphysics-1.0.1/src/torchphysics.egg-info/PKG-INFO
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7924 2023-07-13 06:51:17.000000 torchphysics-1.0.1/src/torchphysics.egg-info/SOURCES.txt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)        1 2023-07-13 06:51:16.000000 torchphysics-1.0.1/src/torchphysics.egg-info/dependency_links.txt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)        1 2021-10-04 10:53:43.000000 torchphysics-1.0.1/src/torchphysics.egg-info/not-zip-safe
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      250 2023-07-13 06:51:16.000000 torchphysics-1.0.1/src/torchphysics.egg-info/requires.txt
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)       13 2023-07-13 06:51:16.000000 torchphysics-1.0.1/src/torchphysics.egg-info/top_level.txt
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.144982 torchphysics-1.0.1/tests/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      280 2021-10-04 10:45:13.000000 torchphysics-1.0.1/tests/conftest.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8886 2022-05-26 13:02:10.000000 torchphysics-1.0.1/tests/test_conditions.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1828 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/test_data_utils.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    28319 2023-05-17 09:33:38.000000 torchphysics-1.0.1/tests/test_differentialoperators.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1170 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/test_evaluation.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    10053 2022-04-12 07:41:01.000000 torchphysics-1.0.1/tests/test_points.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    18503 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/test_samplers.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2587 2022-09-25 11:56:09.000000 torchphysics-1.0.1/tests/test_spaces.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5216 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/test_user_function.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.192440 torchphysics-1.0.1/tests/tests_domain/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     6683 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain0D.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11461 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain1D.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    34547 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain2D.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     8733 2022-02-21 12:06:25.000000 torchphysics-1.0.1/tests/tests_domain/test_domain2D_shapely.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9296 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain3D.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11036 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain3D_trimesh.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13264 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain_cut.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11755 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain_intersection.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7469 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain_product.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    12938 2022-09-05 14:16:09.000000 torchphysics-1.0.1/tests/tests_domain/test_domain_tranforms.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    11495 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_domain/test_domain_union.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.197460 torchphysics-1.0.1/tests/tests_functionsets/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5416 2022-06-01 11:42:37.000000 torchphysics-1.0.1/tests/tests_functionsets/test_FunctionSetMain.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.244055 torchphysics-1.0.1/tests/tests_models/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1948 2022-06-27 14:09:27.000000 torchphysics-1.0.1/tests/tests_models/test_activation_fn.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     7717 2023-05-22 14:27:50.000000 torchphysics-1.0.1/tests/tests_models/test_deep_o_net.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     1199 2022-04-12 07:33:39.000000 torchphysics-1.0.1/tests/tests_models/test_deepritz.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2663 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_models/test_fcn.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     5525 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_models/test_model_base.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      524 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_models/test_parameters.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     3024 2022-02-15 08:38:25.000000 torchphysics-1.0.1/tests/tests_models/test_qres.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.257266 torchphysics-1.0.1/tests/tests_plots/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)    13094 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_plots/test_animation.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     9177 2022-06-27 12:47:07.000000 torchphysics-1.0.1/tests/tests_plots/test_plot.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      892 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_plots/test_scatter.py
+drwxr-xr-x   0 tomfre   (58750) tomfre   (58750)        0 2023-07-13 06:51:19.265638 torchphysics-1.0.1/tests/tests_solver/
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2211 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_solver/test_solver.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)      163 2022-02-08 08:28:13.000000 torchphysics-1.0.1/tests/tests_solver/test_training.py
+-rw-r--r--   0 tomfre   (58750) tomfre   (58750)     2010 2021-10-04 10:45:14.000000 torchphysics-1.0.1/tox.ini
```

### Comparing `torchphysics-1.0.0/.coveragerc` & `torchphysics-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/.github/workflows/python-package.yml` & `torchphysics-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/.gitignore` & `torchphysics-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/CONTRIBUTING.md` & `torchphysics-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/LICENSE.txt` & `torchphysics-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/NOTICE` & `torchphysics-1.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/PKG-INFO` & `torchphysics-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchphysics
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyTorch implementation of Deep Learning methods to solve differential equations
 Home-page: https://github.com/boschresearch/torchphysics
 Author: Nick Heilenkötter, Tom Freudenberg
 Author-email: nick7@uni-bremen.de, tomfre@uni-bremen.de
 License: Apache-2.0
 Project-URL: Documentation, https://torchphysics.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/boschresearch/torchphysics
@@ -95,28 +95,48 @@
 .. _`Tutorial: Understanding the structure of TorchPhysics`: https://torchphysics.readthedocs.io/en/latest/tutorial/tutorial_start.html
 .. _`Examples: Different applications with detailed explanations`: https://github.com/boschresearch/torchphysics/tree/main/examples
 .. _Documentation: https://torchphysics.readthedocs.io/en/latest/api/modules.html
 
 
 Installation
 ============
-TorchPhysics can be installed by using:
+TorchPhysics reqiueres the follwing dependencies to be installed: 
+
+- PyTorch_ >= 1.7.1, < 2.0.0
+- `PyTorch Lightning`_ >= 1.3.4, < 2.0.0
+- Numpy_ >= 1.20.2
+- Matplotlib_ >= 3.0.0
+- Scipy_ >= 1.6.3
+
+Installing TorchPhysics with ``pip``, automatically downloads everything that is needed:
 
 .. code-block:: python
 
-  pip install git+https://github.com/boschresearch/torchphysics
+  pip install torchphysics
+
+Additionally, to use the ``Shapely`` and ``Trimesh`` functionalities, install the library 
+with the option ``all``:
+
+.. code-block:: python
+
+  pip install torchphysics[all]
+
 
-If you want to change or add something to the code. You should first copy the repository and install
-it locally:
+If you want to add functionalities or modify the code. We recommend copying the 
+repository and installing it locally:
 
 .. code-block:: python
 
   git clone https://github.com/boschresearch/torchphysics 
-  pip install .
+  cd path_to_torchphysics_folder
+  pip install .[all]
 
+.. _Numpy: https://numpy.org/
+.. _Matplotlib: https://matplotlib.org/
+.. _Scipy: https://scipy.org/
 
 About
 =====
 TorchPhysics was originally developed by Nick Heilenkötter and Tom Freudenberg, 
 as part of a `seminar project`_ at the `University of Bremen`_, in cooperation with the `Robert Bosch GmbH`_. 
 Special thanks belong to Felix Hildebrand, Uwe Iben, Daniel Christopher Kreuter and Johannes Mueller,
 at the Robert Bosch GmbH, for support and supervision while creating this library.
```

### Comparing `torchphysics-1.0.0/README.rst` & `torchphysics-1.0.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -74,28 +74,48 @@
 .. _`Tutorial: Understanding the structure of TorchPhysics`: https://torchphysics.readthedocs.io/en/latest/tutorial/tutorial_start.html
 .. _`Examples: Different applications with detailed explanations`: https://github.com/boschresearch/torchphysics/tree/main/examples
 .. _Documentation: https://torchphysics.readthedocs.io/en/latest/api/modules.html
 
 
 Installation
 ============
-TorchPhysics can be installed by using:
+TorchPhysics reqiueres the follwing dependencies to be installed: 
+
+- PyTorch_ >= 1.7.1, < 2.0.0
+- `PyTorch Lightning`_ >= 1.3.4, < 2.0.0
+- Numpy_ >= 1.20.2
+- Matplotlib_ >= 3.0.0
+- Scipy_ >= 1.6.3
+
+Installing TorchPhysics with ``pip``, automatically downloads everything that is needed:
 
 .. code-block:: python
 
-  pip install git+https://github.com/boschresearch/torchphysics
+  pip install torchphysics
+
+Additionally, to use the ``Shapely`` and ``Trimesh`` functionalities, install the library 
+with the option ``all``:
+
+.. code-block:: python
+
+  pip install torchphysics[all]
+
 
-If you want to change or add something to the code. You should first copy the repository and install
-it locally:
+If you want to add functionalities or modify the code. We recommend copying the 
+repository and installing it locally:
 
 .. code-block:: python
 
   git clone https://github.com/boschresearch/torchphysics 
-  pip install .
+  cd path_to_torchphysics_folder
+  pip install .[all]
 
+.. _Numpy: https://numpy.org/
+.. _Matplotlib: https://matplotlib.org/
+.. _Scipy: https://scipy.org/
 
 About
 =====
 TorchPhysics was originally developed by Nick Heilenkötter and Tom Freudenberg, 
 as part of a `seminar project`_ at the `University of Bremen`_, in cooperation with the `Robert Bosch GmbH`_. 
 Special thanks belong to Felix Hildebrand, Uwe Iben, Daniel Christopher Kreuter and Johannes Mueller,
 at the Robert Bosch GmbH, for support and supervision while creating this library.
```

### Comparing `torchphysics-1.0.0/docs/Makefile` & `torchphysics-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/conf.py` & `torchphysics-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/examples.rst` & `torchphysics-1.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/index.rst` & `torchphysics-1.0.1/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 **Examples** tab additional applications, in form of Jupyter Notebooks,
 can be found.
 
 .. toctree::
    :maxdepth: 2
 
    Overview <readme>
-   Tutorial <tutorial/tutorial_start>
+   Tutorial <tutorial/main_page>
    Examples <examples>
 
 
 API Reference
 =============
 Information for all classes, functions and methods can be found in
 the following documentation:
```

### Comparing `torchphysics-1.0.0/docs/tutorial/condition_tutorial.rst` & `torchphysics-1.0.1/docs/tutorial/condition_tutorial.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/differentialoperators.rst` & `torchphysics-1.0.1/docs/tutorial/differentialoperators.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/external_domains.rst` & `torchphysics-1.0.1/docs/tutorial/external_domains.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/model_creation.rst` & `torchphysics-1.0.1/docs/tutorial/model_creation.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/L_domain.png` & `torchphysics-1.0.1/docs/tutorial/pictures/L_domain.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/L_slice.png` & `torchphysics-1.0.1/docs/tutorial/pictures/L_slice.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/complex_domain.png` & `torchphysics-1.0.1/docs/tutorial/pictures/complex_domain.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/cylinder.png` & `torchphysics-1.0.1/docs/tutorial/pictures/cylinder.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/error.png` & `torchphysics-1.0.1/docs/tutorial/pictures/error.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/operation.png` & `torchphysics-1.0.1/docs/tutorial/pictures/operation.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/polygon.png` & `torchphysics-1.0.1/docs/tutorial/pictures/polygon.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/rect_circle_domain.png` & `torchphysics-1.0.1/docs/tutorial/pictures/rect_circle_domain.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/sampler_combis.PNG` & `torchphysics-1.0.1/docs/tutorial/pictures/sampler_combis.PNG`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/simplex.png` & `torchphysics-1.0.1/docs/tutorial/pictures/simplex.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/solution.png` & `torchphysics-1.0.1/docs/tutorial/pictures/solution.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/pictures/torchphysics_structure.png` & `torchphysics-1.0.1/docs/tutorial/pictures/torchphysics_structure.png`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/plotting.rst` & `torchphysics-1.0.1/docs/tutorial/plotting.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/sampler_tutorial.rst` & `torchphysics-1.0.1/docs/tutorial/sampler_tutorial.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/solve_pde.rst` & `torchphysics-1.0.1/docs/tutorial/solve_pde.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/solver_info.rst` & `torchphysics-1.0.1/docs/tutorial/solver_info.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/tutorial_domain_basics.rst` & `torchphysics-1.0.1/docs/tutorial/tutorial_domain_basics.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/tutorial_spaces_and_points.rst` & `torchphysics-1.0.1/docs/tutorial/tutorial_spaces_and_points.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/docs/tutorial/tutorial_start.rst` & `torchphysics-1.0.1/docs/tutorial/tutorial_start.rst`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/deeponet/ode.ipynb` & `torchphysics-1.0.1/examples/deeponet/ode.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937785594035594%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(1, \'os.environ["CUDA_VISIBLE_DEVICES"] = "2"\\n\')], '*

 * *            "delete: [1]}}, 4: {'source': {insert: [(2, 'trunk_net = tp.models.FCTrunkNet(T, "*

 * *            "hidden=(30, 30))\\n'), (3, 'branch_net = tp.models.FCBranchNet(Fn_space, hidden=(50, "*

 * *            "50), \\n'), (5, 'model = tp.models.DeepONet(trunk_net, branch_net, U, "*

 * *            "output_neurons=50)')], delete: [6, 4, 3, 2]}}, 7: {'outputs': {0: {'text': {insert: "*

 * *            "[(2, 'LOCAL_RANK: 0 - C […]*

```diff
@@ -24,15 +24,15 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
-                "os.environ[\"CUDA_VISIBLE_DEVICES\"] = \"1\"\n",
+                "os.environ[\"CUDA_VISIBLE_DEVICES\"] = \"2\"\n",
                 "import torch\n",
                 "import torchphysics as tp\n",
                 "import pytorch_lightning as pl"
             ]
         },
         {
             "cell_type": "code",
@@ -79,19 +79,18 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Model\n",
                 "dis_sampler = tp.samplers.GridSampler(T_int, 50).make_static()\n",
-                "trunk_net = tp.models.FCTrunkNet(T, U, hidden=(30, 30), output_neurons=50)\n",
-                "branch_net = tp.models.FCBranchNet(Fn_space, U, output_neurons=50, \n",
-                "                                   hidden=(50, 50), \n",
+                "trunk_net = tp.models.FCTrunkNet(T, hidden=(30, 30))\n",
+                "branch_net = tp.models.FCBranchNet(Fn_space, hidden=(50, 50), \n",
                 "                                   discretization_sampler=dis_sampler)\n",
-                "model = tp.models.DeepONet(trunk_net, branch_net)"
+                "model = tp.models.DeepONet(trunk_net, branch_net, U, output_neurons=50)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
@@ -137,49 +136,49 @@
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "GPU available: True, used: True\n",
                         "TPU available: False, using: 0 TPU cores\n",
-                        "LOCAL_RANK: 0 - CUDA_VISIBLE_DEVICES: [1]\n",
+                        "LOCAL_RANK: 0 - CUDA_VISIBLE_DEVICES: [2]\n",
                         "\n",
                         "  | Name             | Type       | Params\n",
                         "------------------------------------------------\n",
                         "0 | train_conditions | ModuleList | 10.2 K\n",
                         "1 | val_conditions   | ModuleList | 0     \n",
                         "------------------------------------------------\n",
                         "10.2 K    Trainable params\n",
                         "0         Non-trainable params\n",
                         "10.2 K    Total params\n",
                         "0.041     Total estimated model params size (MB)\n",
-                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, train dataloader, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 20 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
+                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, train dataloader, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 24 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
                         "  warnings.warn(*args, **kwargs)\n",
-                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, val dataloader 0, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 20 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
+                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, val dataloader 0, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 24 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
                         "  warnings.warn(*args, **kwargs)\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "f0e44390260e4d55acfa5e867c2dd001",
+                            "model_id": "f2349bee03f34d7f8758d4bb2f4eaedd",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Training: 0it [00:00, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "412da0e2778f4c5d9586c39ca9ad83cd",
+                            "model_id": "e4d434a1dc5742bebbe7109a4abcead2",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Validating: 0it [00:00, ?it/s]"
                         ]
                     },
@@ -201,24 +200,24 @@
                 "                     )\n",
                 "\n",
                 "trainer.fit(solver)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "GPU available: True, used: True\n",
                         "TPU available: False, using: 0 TPU cores\n",
-                        "LOCAL_RANK: 0 - CUDA_VISIBLE_DEVICES: [1]\n",
+                        "LOCAL_RANK: 0 - CUDA_VISIBLE_DEVICES: [2]\n",
                         "\n",
                         "  | Name             | Type       | Params\n",
                         "------------------------------------------------\n",
                         "0 | train_conditions | ModuleList | 10.2 K\n",
                         "1 | val_conditions   | ModuleList | 0     \n",
                         "------------------------------------------------\n",
                         "10.2 K    Trainable params\n",
@@ -226,53 +225,43 @@
                         "10.2 K    Total params\n",
                         "0.041     Total estimated model params size (MB)\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "f76819cd01c84b3f94d5f07e112dfa68",
+                            "model_id": "2b2610116f574ffba78d4f60b66d25bb",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Validation sanity check: 0it [00:00, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, val dataloader 0, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 20 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
-                        "  warnings.warn(*args, **kwargs)\n",
-                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, train dataloader, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 20 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
-                        "  warnings.warn(*args, **kwargs)\n"
-                    ]
-                },
-                {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "8b173daf653649f5a0181609dde5e076",
+                            "model_id": "caf835a0baeb42b9b684c43b8eba01ce",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Training: 0it [00:00, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "8cef152b3e804c89b6d7272bb6edb96f",
+                            "model_id": "ae55eac3287f4806b3476dea0284c6d6",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Validating: 0it [00:00, ?it/s]"
                         ]
                     },
@@ -302,30 +291,30 @@
                 "                     checkpoint_callback=False)\n",
                 "                     \n",
                 "trainer.fit(solver)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.legend.Legend at 0x7fed7af12280>"
+                            "<matplotlib.legend.Legend at 0x7fdab0db1580>"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAXoAAAD6CAYAAACvZ4z8AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjQuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8rg+JYAAAACXBIWXMAAAsTAAALEwEAmpwYAAAzTElEQVR4nO3deXxU9fX4/9fJQhIgYQsEAgGiBWQPJIAgIi5oUAQUFBARqEqpYrVa/OCnfoVi68et9VeVVnDD2goqaKQVFxBGRGQJiyggskPYSVgSsmfO748Z0hACGUImk8mc5+ORB3Pvfb/vPScJZ27e9877iqpijDGm5grydQDGGGO8ywq9McbUcFbojTGmhrNCb4wxNZwVemOMqeGs0BtjTA3nUaEXkWQR2Soi20VkygXaDRMRFZGkEuuecPfbKiI3VUbQxhhjPBdSXgMRCQZmAAOANGCNiCxQ1c2l2kUCDwOrSqzrAIwEOgKxwGIRaauqRec7XnR0tLZu3boCqcDp06epU6dOhfr6K8s5MARizhCYeVc057Vr1x5T1cZlbSu30AM9ge2quhNAROYCQ4DNpdo9DTwHTC6xbggwV1XzgF0ist29v+/Od7DWrVuTmprqQVjncjgc9O/fv0J9/ZXlHBgCMWcIzLwrmrOI7DnfNk8KfXNgX4nlNKBXqQN0B+JU9VMRmVyq78pSfZuXEeAEYAJATEwMDofDg7DOlZWVVeG+/spyDgyBmDMEZt7eyNmTQn9BIhIE/AUYV9F9qOosYBZAUlKSVvQd3N79A4PlHDgCMW9v5OxJod8PxJVYbuFed0Yk0AlwiAhAU2CBiAz2oK8xxhgv86TQrwHaiEg8riI9ErjrzEZVPQlEn1kWEQfwO1VNFZEc4D0R+Quui7FtgNUXG2RBQQFpaWnk5uZesF29evXYsmXLxe7erwVCzuHh4bRo0YLQ0FBfh2KMXyq30KtqoYhMAr4AgoG3VHWTiEwHUlV1wQX6bhKRD3BduC0EHrzQHTfnk5aWRmRkJK1bt8b9V0OZMjMziYyMvNjd+7WanrOqkp6eTlpaGvHx8b4Oxxi/5NEYvaouBBaWWvfUedr2L7X8J+BPFYwPgNzc3HKLvKmZRIRGjRpx9OhRX4dijN/ym0/GWpEPXPazN+bSXPJdN8YYYy7d0W/fpU5YEGhspe/bb87ofU1EeOyxx4qXX3zxRaZNm3bBPg6HgxUrVlR6LLNnz2bSpEmVus8TJ07wt7/97ZL2kZKSwubNpT9HZ4wpj+ZlEvrVk2z97O9446l/Vug9FBYWxkcffcSxY8c87uONQl9YWFip+zvDCr0xvrPr079Q33mCQ0mTkaDKL8tW6D0UEhLChAkTeOmll87ZdvToUYYNG0aPHj3o0aMH3377Lbt37+a1117jpZdeIiEhga+//pr4+HhUlRMnThAcHMyyZcsA6NevH9u2bSMjI4OhQ4fSpUsXrrzySjZu3AjAtGnTGDNmDFdddRVjxow569iff/45vXv3PucN6EL7evHFF4vbderUid27dzNlyhR27NhBQkICkydPxuFw0K9fP2655RbatWvHxIkTcTqdANStW7e4/7x58xg3bhwrVqxgwYIFTJ48mYSEBHbs2FEJ33Vjaj7NPk6TH2ayPKgH1w+41SvH8Lsx+j/8exObD5wqc1tRURHBwcEXvc8OsVFMvbVjue0efPBBunTpwuOPP37W+ocffpjf/va39O3bl71793LTTTexZcsWJk6cSN26dfnd734HQLt27di8eTO7du2ie/fufPPNN/Tq1Yt9+/bRpk0bHnroIbp160ZKSgpLlizhnnvuYcOGDQBs3ryZ5cuXExERwezZswH4+OOPeemll1i4cCENGjQ4K6apU6eed19lefbZZ/nxxx+L2zgcDlavXs3mzZtp1aoVycnJfPTRRwwfPrzM/n369GHw4MEMGjTovG2MMefaueD/uFxPk9PvCWqFeOfc2+8KvS9FRUVxzz338PLLLxMREVG8fvHixWcNWZw6dYqsrKxz+l999dUsW7aMXbt28cQTT/D6669zzTXX0KNHDwCWL1/O/PnzAbjuuutIT0/n1CnXm9rgwYPPOuaSJUtITU1l/vz55xT58vblqZ49e3LZZZcBMGrUKJYvX25F3JhKVHTqMLE/zearkH5cd811XjuO3xX6C515V8WHhx555BG6d+/O+PHji9c5nU5WrlxJeHj4Bfv269ePv//97xw4cIDp06fzwgsv4HA4uPrqq8s9bulpSy+//HJ27tzJ9u3bad78nHniziskJKR4CAa44KeNS9/WeGa55PryPq1sjDm/XSnTaa0FBF33vwQHee82Yhujv0gNGzbkzjvv5M033yxed+ONN/LKK68UL58Z/oiMjCQzM7N4fc+ePVmx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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -352,30 +341,30 @@
                 "plt.plot(grid_p, F(grid_p))\n",
                 "plt.grid()\n",
                 "plt.legend(['Network output', 'Analytical solution'])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.legend.Legend at 0x7fed4a72dc10>"
+                            "<matplotlib.legend.Legend at 0x7fdab1a99160>"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAXQAAAD4CAYAAAD8Zh1EAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjQuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8rg+JYAAAACXBIWXMAAAsTAAALEwEAmpwYAAAvxElEQVR4nO3deVxVdf7H8deXHWVRwEgFxQUXBAQFcQ9bMRPTyizTNJccs2UyJ2ep/FnTTNPeZJlb1lha6qSmlmVKuaKIO5ghKpLmAm6orPf7+wN0kBCueLmHe+/n+XjweNxzz/ec8/5y4cPhLN+jtNYIIYSwfU5GBxBCCGEZUtCFEMJOSEEXQgg7IQVdCCHshBR0IYSwEy5GbTggIECHhITUaNkLFy5Qv359ywaq46TPjkH67BhupM/btm07pbVuVNk8wwp6SEgIKSkpNVo2KSmJ+Ph4ywaq46TPjkH67BhupM9KqcPXmieHXIQQwk5IQRdCCDshBV0IIeyEYcfQK1NUVER2djb5+flVtvP19SU9Pd1KqeoGe++zh4cHQUFBuLq6Gh1FCJtVpwp6dnY23t7ehISEoJS6Zrvz58/j7e1txWTGs+c+a63JyckhOzubFi1aGB1HCJtV7SEXpdQcpdQJpdSea8xXSqn3lFIZSqldSqlONQ2Tn5+Pv79/lcVc2B+lFP7+/tX+ZyaEqJo5x9DnAglVzO8LhJZ9jQU+vJFAUswdk3zuQty4ag+5aK1/UkqFVNFkAPCpLh2Hd7NSqoFSqrHW+pilQgohal9BUTE5uTmcPXWMi2eOU3zxLMUFFzEVXqKk8BK6qACFCa2c0E4uaOWMk5Mzzh5eONfzxbVeQ9y8GlLfN4CAgJtoUN9d/lBbmSWOoTcFjpSbzi5773cFXSk1ltK9eAIDA0lKSrpqvq+vL+fPn692gyUlJWa1qwkfHx8mTJjAq6++CsB7771HXl4ef/nLX665zLp163BzcyMuLs6iWT777DNSU1N58803LdbnM2fOsHDhQsaMGVPjdSxfvpzWrVvTrl27G85TXn5+/lU/E3l5eb/7GbF3tdnnkhIT586ewnTmCOrCcdwvHce78Dj+xScI0Lk04DxNVDFNLLCtQu1MNn6cUn6ccfLjgqs/eZ5NKPYKwqlBEL4+DanvVnqAQD5ny7HqSVGt9QxgBkBMTIyueKdUenq6WSf+avMEobu7O8uXL+ell14iICAAd3d3ioqKqtzeli1b8PLy4vbbb7dYjuLiYjw8PHBzc8Pb29tifc7JyWHOnDk8++yzNV7HqlWrcHV1JTY29obzlOfh4UF0dPSVabmDsObyCwrI3JPMmYxkOL4X33P7aVp0iAbqwpU2RdqZU86NOOPZlKP12pHt6Y+TVyNcfRrh7hOIe/0GuHnWw92zPu4e9XHz8ATlhKmkBK2LoaSEouJC8i/kkX8+l6ILZyi6eJrC87mUnPsN57yjeF06TuOCwzQsSMG9oAjOANlwVtfjsFMwp7zacda5KX5dEghp14nGDb0cYq++tn62LVHQfwWCy00Hlb1nk1xcXBg7dixvv/02f//736+ad/LkScaNG0dWVhYA77zzDk2bNmX69Ok4Ozszb9483n33XUaMGEFmZiZnz57F39+ftWvX0rt3b3r37s3s2bPx9/fnscceIzMzk3r16jFjxgwiIyOZMmUKBw4cIDMzk2bNmnHXXXdd2fa3337LW2+9xddff01AQMCV93Nzc6+5Li8vL5577jkAwsPDWb58OZMnT+bAgQNERUVxxx130K9fP1588UW8vb3JyMigT58+fPDBBzg5OeHl5UVeXh4AixYtYvny5YwdO5Zly5bx448/8sorr7B48WJatWpV2x+LqMbp3FMc3PYd+Zmb8Dm1nZaF+wlTBQDk4clRtxYcuOkOnAI74BXcgUbB7fANbE5jZxca38B23QEvcxqaTBTkZpFzaDfnstMpObGf+qd/pvX576jHJfjuAy6tcmOXU0t+axiDc8teNOvYh9ZNb8LJyf4LvKVYoqAvAyYopRYAccBZSxw//7+v95J29Fyl80pKSnB2dr7udYY18eGl/h2qbffEE08QGRnJn/70p6vef/rpp/njH/9Iz549ycrK4q677iI9PZ1x48ZdVTzbtm1LWloaBw8epFOnTqxbt464uDiOHDlCaGgoTz75JNHR0SxZsoQ1a9YwfPhwduzYAUBaWhrr16/H09OTuXPnAvDVV1/x9ttvs3LlSho2bHhVppdeeuma66rMP//5T/bs2XOlTVJSElu2bCEtLY3mzZuTkJDAf//7X+6///5Kl+/evTuJiYncc88912wjal9RYQH7t63l7N7vaPjbBkKL9tNJmSjSzhx2bUnazYm4hXSlcXgvApqG0sbJ4HsInZxwDwihSUAI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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -418,14 +407,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
+            "version": "3.9.15"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `torchphysics-1.0.0/examples/deeponet/oscillator.ipynb` & `torchphysics-1.0.1/examples/deeponet/oscillator.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971413249601742%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(25, 'trunk_net = tp.models.FCTrunkNet(T, hidden=(50, "*

 * *            "50),\\n'), (27, 'branch_net = tp.models.ConvBranchNet1D(Fn_space, "*

 * *            "convolutional_network=ConvolutionLayers(),\\n'), (29, 'model = "*

 * *            "tp.models.DeepONet(trunk_net, branch_net, U, output_neurons=80)')], delete: [30, 28, "*

 * *            "27, 25]}}, 6: {'outputs': {0: {'text': {insert: [(13, "*

 * *            "'/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_light […]*

```diff
@@ -90,20 +90,19 @@
                 "    def forward(self, Tensor):\n",
                 "        alpha = 0.1\n",
                 "        return torch.exp(-alpha * Tensor) * torch.sin(Tensor)\n",
                 "\n",
                 "# Model\n",
                 "dis_sampler = (tp.samplers.GridSampler(A_t.boundary_left, n_points = 1)\n",
                 "                + tp.samplers.GridSampler(A_t, n_points = 800)).make_static()\n",
-                "trunk_net = tp.models.FCTrunkNet(T, U, hidden=(50, 50), output_neurons=80,\n",
+                "trunk_net = tp.models.FCTrunkNet(T, hidden=(50, 50),\n",
                 "                                 xavier_gains=[3/5, 3/5, 0.0])\n",
-                "branch_net = tp.models.ConvBranchNet1D(Fn_space, U, output_neurons=80, \n",
-                "                                       convolutional_network=ConvolutionLayers(),\n",
+                "branch_net = tp.models.ConvBranchNet1D(Fn_space, convolutional_network=ConvolutionLayers(),\n",
                 "                                       hidden=(600, 500, 250), discretization_sampler=dis_sampler)\n",
-                "model = tp.models.DeepONet(trunk_net, branch_net)"
+                "model = tp.models.DeepONet(trunk_net, branch_net, U, output_neurons=80)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
@@ -178,38 +177,38 @@
                         "0 | train_conditions | ModuleList | 933 K \n",
                         "1 | val_conditions   | ModuleList | 0     \n",
                         "------------------------------------------------\n",
                         "933 K     Trainable params\n",
                         "0         Non-trainable params\n",
                         "933 K     Total params\n",
                         "3.735     Total estimated model params size (MB)\n",
-                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, train dataloader, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 20 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
+                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, train dataloader, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 24 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
                         "  warnings.warn(*args, **kwargs)\n",
-                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, val dataloader 0, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 20 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
+                        "/home/tomfre/miniconda3/envs/bosch/lib/python3.9/site-packages/pytorch_lightning/utilities/distributed.py:69: UserWarning: The dataloader, val dataloader 0, does not have many workers which may be a bottleneck. Consider increasing the value of the `num_workers` argument` (try 24 which is the number of cpus on this machine) in the `DataLoader` init to improve performance.\n",
                         "  warnings.warn(*args, **kwargs)\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "8933d98cf8b742f7aa925ec87bbe3e5c",
+                            "model_id": "59015f1c25d44d81b08ccf672fc9ad54",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Training: 0it [00:00, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "76e8714ecf2a456f858722aa9e41d27b",
+                            "model_id": "460abca5f9a34718afe42d3137125006",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Validating: 0it [00:00, ?it/s]"
                         ]
                     },
@@ -254,43 +253,43 @@
                         "933 K     Total params\n",
                         "3.735     Total estimated model params size (MB)\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "987631479e3d4fcc8175d4e507ba03b8",
+                            "model_id": "17ef34adef49498bb58127bc9d8151b1",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Validation sanity check: 0it [00:00, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "5a2e9b4224c345aaa6fb67e6163d6aed",
+                            "model_id": "d3ed94b3061a4eba88de1a102194739c",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Training: 0it [00:00, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "72aa65012189496c8404ee3fffbaa243",
+                            "model_id": "df5cb8df26d242d98acf98368734a9de",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Validating: 0it [00:00, ?it/s]"
                         ]
                     },
@@ -325,24 +324,24 @@
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.legend.Legend at 0x7fd56a9055e0>"
+                            "<matplotlib.legend.Legend at 0x7fd778c357f0>"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAXwAAAD4CAYAAADvsV2wAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjQuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8rg+JYAAAACXBIWXMAAAsTAAALEwEAmpwYAABORUlEQVR4nO3deVyU19n4/8+ZGXYQBBVUEFBxAwEF90RxN4lRs++JadI0bdOmzdIkTX5JmzZP8zxNk37bpGmzNUmTmN0laqJxwX1DwAWQRUAFVEBkX2fm/P4YsGhQkVnuYea8Xy9eMsM997kOgxc35z7nOkJKiaIoiuL6dFoHoCiKojiGSviKoihuQiV8RVEUN6ESvqIoiptQCV9RFMVNGLQO4GL69esno6Kievz6hoYG/Pz8bBeQk3O3/oLqs7tQfb4y+/fvr5RS9u/qa06b8KOiokhLS+vx61NTU0lJSbFdQE7O3foLqs/uQvX5ygghjl3sa2pIR1EUxU2ohK8oiuImVMJXFEVxE047hq8oin21tbVRUlJCc3Oz1qFcUmBgIDk5OVqH4VDd6bO3tzfh4eF4eHh0+7wq4SuKmyopKSEgIICoqCiEEFqHc1F1dXUEBARoHYZDXa7PUkrOnDlDSUkJ0dHR3T6vGtJRFDfV3NxMSEiIUyd7pWtCCEJCQq74rzOV8BXFjalk33v15L1TQzq9REOLke0FlRytqMfLoCc5si/x4YHqP6yiKN2mrvCdnNkseWdbIVNf3sRP/rOf//sulz+szmbxGzu48c2d5J6q0zpERekxIQSPP/74ucevvPIKv/vd7y75mtTUVHbu3GnzWN5//30eeeQRm56zurqaf/zjH1adY8WKFWRnZ9skHpXwnVhjq5H739/HH9fkMG5IEJ/8eBI5Ly5g77Oz+cOSOE5UNXL969tZl3VK61AVpUe8vLz4+uuvqays7PZr7JHwjUajTc/XQSV8pVsaWowsfW8f2/Ir+OOSOP69dAJTh/XDx1PPgABv7pkcyXe/ms6YgX342cfpHKywzw+sotiTwWDgoYce4rXXXvvB1yoqKrjpppuYMWMGEyZMYMeOHRQXF/PPf/6T1157jcTERLZs2UJ0dDRSSqqrq9Hr9WzduhWA6dOnk5+fT1VVFUuWLCE+Pp7Jkydz8OBBAH73u99xzz33MG3aNO65557z2l6zZg1Tpkz5wS+iS53rlVdeOXdcXFwcxcXFPP300xw9epTExESefPJJUlNTmT59Otdddx0jR47k4Ycfxmw2A+Dv73/u9StWrGDp0qXs3LmTVatW8eSTT5KYmMjRo0et+35b9WrFLsxmyWOfZ5J2rIq/3TGOhfGDujyun78XHz04iVv/uYs3D9Ry7Yx6hg/w7/JYRbmU33+TRXZZrU3POWZQH164Pvayx/385z8nPj6e3/zmN+c9/+ijj/LrX/+ahIQEzp49y/z588nJyeHhhx/G39+fJ554AoCRI0eSnZ1NUVER48ePZ9u2bUyaNIkTJ04QExPDL37xC8aNG8eKFSvYtGkT9957L5mZmQBkZ2ezfft2fHx8eP/99wFYvnw5r776KmvXrqVv377nxfTCCy9c9Fxdefnllzl8+PC5Y1JTU9m7dy/Z2dlERkayYMECvv76a26++eYuXz916lQWLVrEwoULL3rMlVAJ3wn9I7WAdVmnee660RdN9h38vQy8fV8y8/+yicc+z+Trn07FoFd/uCm9R58+fbj33nv529/+ho+Pz7nnN2zYQHZ2NmazGZ1OR21tLfX19T94/dVXX83WrVspKirimWee4e233z73VwHA9u3b+eqrrwCYNWsWZ86cobbW8stt0aJF57W5adMm0tLSWL9+PX369PlBW5c6V3dNnDiRoUOHAnDHHXewfft2myTz7lAJ38lkldXw1w35LIwfyANXdW9BxeAgH+4d48U/DtTw1rZCfpYy3M5RKq6mO1fi9vSrX/2K8ePHc//99597zmw2s3v3btra2i65CGn69Om8+eablJWV8eKLL/LnP/+Z1NRUrr766su2e2EJ4mHDhlFYWEheXh7Jycndjt9gMJwbmgEuOT/+wpl1HY87P2+v1c/qUtCJtBrNPP75Afr6efLHJXFXNOVy4kAD88aE8veNBZyude6l8opyoeDgYG699Vbefffdc8/NmzePv//97+cedwyLBAQEUFf339lpEydOZOfOneh0Ory9vUlMTORf//oX06dPByx/AXz88ceAZUilX79+XV69A0RGRvLVV19x7733kpWV9YOvX+xcUVFRpKenA5Cenk5RUVGXsQLs3buXoqIizGYzn332GVdddRUAoaGh5OTkYDabWb169bnjuzpHT6mE70Te21HEkVN1/M8NYwny9bzi1z973WiMZjN/WZ9rh+gU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",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -376,30 +375,30 @@
                 "plt.plot(grid_p, u)\n",
                 "plt.grid()\n",
                 "plt.legend(['Network output', 'Euler solution'])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.legend.Legend at 0x7fd56a98fe80>"
+                            "<matplotlib.legend.Legend at 0x7fd778c355e0>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAYAAAAD5CAYAAAAuneICAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjQuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8rg+JYAAAACXBIWXMAAAsTAAALEwEAmpwYAABH00lEQVR4nO3dd3hUVfrA8e87k94bCSVAQie00EKREqy4IuDaQAV1VVZd7KK4rmVdd1dXf7prWbtiBwVFVlEUISIgHUSK1FBCJ4UU0nN+f9whhhDIJEwySeb9PM88uXPuvee+J4F5595z7zlijEEppZTnsbk7AKWUUu6hCUAppTyUJgCllPJQmgCUUspDaQJQSikPpQlAKaU8lJczG4nISOA/gB140xjzVKX19wI3AyXAEeAPxpjdjnXXA39xbPqkMeZdR3lfYBrgD8wF7jLV3JMaFRVl4uLinGpYZXl5eQQGBtZq38ZK2+wZtM2e4WzavHr16qPGmGanrDDGnPGF9aG/A2gH+AA/AwmVthkBBDiWbwNmOJYjgJ2On+GO5XDHuhXAQECAr4GLq4ulb9++prYWLlxY630bK22zZ9A2e4azaTOwylTxmerMJaAkYLsxZqcxpgiYDoyplEQWGmOOO94uA2IdyxcB3xljMowxmcB3wEgRaQGEGGOWOYJ7DxjrRCxKKaVcxJlLQK2AvRXepwEDzrD9TVjf6E+3byvHK62K8lOIyCRgEkBMTAwpKSlOhHyq3NzcWu/bWGmbPYO22TPURZud6gNwlohcB/QDhruqTmPM68DrAP369TPJycm1qiclJYXa7ttYaZs9g7bZM9RFm51JAPuA1hXexzrKTiIi5wMPA8ONMYUV9k2utG+Kozy2UvkpdSql6k9xcTFpaWkUFBS4O5RqhYaGsnnzZneHUa+cabOfnx+xsbF4e3s7VaczCWAl0FFE4rE+pMcB11TcQER6A68BI40xhyusmgf8Q0TCHe8vBB4yxmSISLaIDASWAxOBF52KWClVJ9LS0ggODiYuLg4RcXc4Z5STk0NwcLC7w6hX1bXZGEN6ejppaWnEx8c7VWe1ncDGmBJgMtaH+WbgE2PMRhF5QkRGOzZ7BggCPhWRdSIyx7FvBvA3rCSyEnjCUQZwO/AmsB3rLqMT/QZKKTcoKCggMjKywX/4q6qJCJGRkTU6g3OqD8AYMxfrXv2KZY9WWD7/DPu+DbxdRfkqoLvTkSql6px++DduNf37ubQTWDkYA/tWw97lUFIIEe2gXTL4h7k7MqWUKqdDQbjawQ3wxrnw5nkw78/w/V/h0+vh+W7w3WNQdLz6OpTyUCLCfffdV/7+2Wef5fHHHz/jPikpKSxdutTlsUybNo3Jkye7tM6srCz++9//nlUds2fPZtOmTS6JRxOAK22dZ334H0uDUf+G+7fDwwfhD/Og88Ww5N/w2lA4ssXdkSrVIPn6+vLZZ59x9OhRp/epiwRQUlLi0vpO0ATQVO1ZBtOvheiucPtP0O9GCGoG3v7QZiBc/iZMnAMF2fDWhbB3hbsjVqrB8fLyYtKkSTz//POnrDty5AiXX345/fv3Z/jw4SxZsoRdu3bx6quv8vzzz5OYmMgPP/xAfHw8xhiysrKw2+0sWrQIgGHDhrFt2zYyMjIYO3YsPXv2ZODAgaxfvx6Axx9/nAkTJnDOOecwYcKEk4791VdfMWjQoFMS05nqevbZZ8u36969O7t27WLq1Kns2LGDxMREpkyZQkpKCsOGDeOSSy6hc+fO3HrrrZSVlQEQFBRUvv/MmTO59dZbWbp0KXPmzGHKlCkkJiayY8eOs/t9n9XeypJ7BD69AUJjYeJs8A+vert2w+Hm7+D938MHV8CNX0HzHvUZqVJO+ev/NrJpf7ZL60xoGcJjl3ardrs//elP9OzZkwceeOCk8rvuuot77rmHIUOGsGnTJi6//HI2b97MrbfeSlBQEPfffz8AnTt3ZtOmTaSmptKnTx9+/PFHBgwYwN69e+nYsSN33HEHvXv3Zvbs2SxYsICJEyeybt06ADZt2sTixYvx9/dn2rRpAHz++ec899xzzJ07l/Dwk/9vP/bYY6etqypPPfUUGzZsKN8mJSWFFStWsGnTJtq2bcvIkSP57LPPuOKKK6rcf/DgwYwePZpRo0addpua0ATgCt8+DMfT4ZYFp//wPyE8DiZ+AW9fZCWCP/4AIS3rJUylGoOQkBAmTpzICy+8gL+/f3n5/Pnzyy99lJWVkZ2dTW5u7in7Dx06lEWLFpGamspDDz3EG2+8wfDhw+nfvz8AixcvZtasWQCce+65pKenk51tJbvRo0efdMwFCxawatUqvv32W0JCQk451pnqclZSUhLt2rUDYPz48SxevNglH+7O0ARwtnYtgfUzYNgU57/Nh7WG62bBm+fDJ9fDDV+Bl0/dxqlUDTjzTb0u3X333fTp04cbb7yxvKysrIxly5bh5+d3xoeihg0bxiuvvML+/ft54okneOaZZ0hJSWHo0KHVHrfycMvt27dn586dbN26lX79+jkdv5eXV/mlHOCM9+ZXvnXzxPuK5XX1dLb2AZwNY2D+YxASC0Purdm+0V1hzEuQtgK+e7T67ZXyIBEREVx11VW89dZb5WUXXnghL77424ABJy6jBAcHk5OTU16elJTE0qVLsdls+Pn5kZiYyGuvvcawYcMA6wzhww8/BKxLMFFRUVV+uwdo27Yts2bNYuLEiWzcuPGU9aerKy4ujjVr1gCwZs0aUlNTq4wVYMWKFaSmplJWVsaMGTMYMmQIYA1+uXnzZsrKyvj888/Lt6+qjtrSBHA2Un+AtJUw9B7wCaj5/t0ug6Q/wvJXIHWR6+NTqhG77777Tup0feGFF1i1ahU9e/akf//+vPrqqwBceumlfP755yQmJvLjjz/i6+tL69atGThwIGB9SOfk5NCjh3WG/vjjj7N69Wp69uzJ1KlTeffdd88YR5cuXfjwww+58sorT+l0PV1dl19+ORkZGXTr1o2XXnqJTp06ARAZGck555xD9+7dmTJlCgD9+/dn8uTJdO3alfj4eC677DLA6i8YNWoUgwcPpkWLFuXHHDduHM888wy9e/c+607gaieEaUivBjchzLRRxjzTyZii/NrXUZhnzH96G/N8d2MKsl0Xm9FJMzyFq9q8adMml9RTH7KzXft/xV0WLlxoLrnkEqe2dbbNVf0dOYsJYVRVjm63vrUn3QLefrWvxycAxr4CWXth/uMuC08ppaqjCaC21kwDmxf0nlDtptVqMwAG3Aor34L9a8++PqVUo5CcnMyXX37ptuNrAqiNkiJY95H1dG9wjGvqHPEQBEbB3ClQ4e4BpZSqK5oAamPH99Z9/6749n+CXyhc8ITVqfzzx66rVymlTkMTQG1snG19YLcb4dp6e46D2CSrL6Dw1AdclFLKlTQB1FRJIWz5GrqMcv3DWzYbXPQPyDsMy85uwCillKqOUwlAREaKyBYR2S4iU6tYP0xE1ohIiYhcUaF8hGOGsBOvAhEZ61g3TURSK6xLdFWj6tTOFCg8Bglj6qb+1v2t5LLkBchzfkREpZoCu91OYmJi+eupp5464/Z1MWTzmcTFxVU7Uum0adPYv39/+fubb77ZZaN3ulq1Q0GIiB14GbgASANWisgcY0zFFu0BbgDur7ivMWYhkOioJwJr+sdvK2wyxRgz8yzir3+/fgU+wdYEL3XlvEdhy0D48f9g5D/r7jhKNTD+/v5nHEztbJWUlODlVbcj4EybNo3u3bvTsqU1xtebb75Zp8c7G86cASQB240xO40xRcB04KSvv8aYXcaY9cCZbl+5AvjaGNN4Z0QxBrZ/b43q6eVbd8dp1hkSr4WVb0Lm7ro7jlKNRMVv3qtWreJ3v/vdKdtUHC66f//+LFmyBDjzMM8HDhxg2LBhJCYm0r17d3788UcAPv74Y3r06EH37t158MEHTznWrl276N79txltT0xcM3PmTFatWsW1115LYmIi+fn5JCcns2rVqjPWGxQUxMMPP0yvXr0YOHAghw4dOsvfmHOcSYWtgL0V3qcBA2pxrHHAc5XK/i4ijwLfA1ONMYWVdxKRScAksMbGSElJqcWhITc3t9b7nhCQt5ek7DS2NB/NgTPUVVhq2JJRyoE8gwDNA4XOEXZ87c7P1+nrm8yAsukcmnEvW7rcUat4XdHmxkbbXHuhoaHlY8z4LnwM2+FTx745G2XR3Sgc8dczbpOfn0/Pnj3L3997771cfvnlGGPIzc3F19eXvLw8jDHk5ORQUFBAUVEROTk53H777fzxj39k0KBB7N27l8suu4xVq1ZRWFjIhg0bmDdvHv7+/ieNo/POO++QnJzMlClTKC0t5fjx42zdupUHHniARYsWERYWxtixY/n4448ZNWpUeRy5ubmUlZWV11VYWEhhYSEXXXQRvXv35sknn6RPnz6UlJRQWlpKXl7eGevNy8ujV69eTJ06lUceeYSXXnrplOGwS0tLnRoDqKCgwOl/D/UyGqiItAB6APMqFD8EHAR8gNeBB4EnKu9rjHndsZ5+/fqZ5OTkWsWQkpJCbfct99PLAHT+3W10DmtzyuqS0jLeWpzKK0t2kHW8+KR1/t52ru7fmtuT2xMd4uSTw2UraLHqLVqMex6qOF51XNLmRkbbXHubN2/+bYRNbx+wu/jjwdsHn9OM4HmCv79/+aQqFYkIQUFBBAcHExgYiIgQHByMn58fPj4+BAcH88MPP7Bt27byfXJzcxERfH19GTt2LNHR0afUO2TIEP7whz9gs9kYO3YsiYmJfPHFF4wYMYL4+HgAJk6cyMqVKxk/fnx5HAA2m6389+Xr60txcTHBwcHY7XYCAwPL1514v3nz5tPW6+Pjw5VXXomIMGjQIL777rtTRjs90wioFfn5+dG7d+9qtwPnEsA+oHWF97GOspq4CvjcGFP+qWiMOeBYLBSRd6jUf9Agbf8eojpV+WGcU1DMLe+tYtnODEZ0bsb1g+PoFRtGmTFsPpDD7HX7eH/ZbmatSePxS7vx+z6tThkG9hTn3AWr34HFz8OoU2dIUqrOXHzmztf6VnF45dMNjVxxuOjKKg/zfMKwYcNYtGgRX331FTfccAP33nsvoaGhNYrnTDE5y9vbu/zzwG6319mUlJU50wewEugoIvEi4oN1KWdODY8zHjjp6SbHWQFitXossKGGddavkiLYvbTKe//zi0qZ8NYKVu3K5JkrevL2Df1J7hxNeKAPkUG+DOkYxbNX9mL+vcPp0jyY+z79mYdnb6C4tJonfkNbQe/rYM371jzDSnmouLg4Vq9eDVA+AUtlpxsu+kx2795NTEwMt9xyCzfffDNr1qwhKSmJH374gaNHj1JaWsrHH3/M8OHDT9ovJiaGw4cPk56eTmFh4UnDOZxuuGZn6q1v1SYAY0wJMBnr8s1m4BNjzEYReUJERgOISH8RSQOuBF4TkfKLhyISh3UG8UOlqj8UkV+AX4Ao4EkXtKfuHFwPJfnQdvBJxcYYpn62np/Tsnjpmj5c2a/1ab/Zx0cFMn3SIG5Lbs9Hy/dw07urKCguPfNxh9wDGFjyHxc1RKmGKz8//6TbQKdOte46f+yxx7jrrrvo168fdru9yn0rDhedkJBQPlz0maSkpNCrVy969+7NjBkzuOuuu2jRogVPPfUUI0aMoFevXvTt25cxY06+7dvb25tHH32UpKQkLrjgArp06VK+7oYbbuDWW28t7wQ+wZl6611VQ4Q21Jdbh4Ne/B9jHgsxJvvgScUzV+01bR/80rwwf2uNqvt4+W4TN/VLc92by0x+UcmZN/5isjFPNDPm2P4aHUOHRvYMOhy0Z9DhoN1pzzKIaHfS4G8ZeUU8+dUm+rYN508jOtSounFJbXj68p4s3n6UP324hpIzXQ4aci+UlcBPL9U2eqWUOoUmAGeUlcGen6DNyZd//jN/K9kFJfz9su7YbM7f4nnCVf1a88Tobnz/62Ge/Grz6TeMiIfuv4fV0yA/q8bHUUqpqmgCcEb6NsjPgDYDy4sOHMvn4xV7ubJvLF2aVz2fqDMmDIrj5iHxTFu6i2lLUk+/4eA7oSgXVr1d62MpVR3raoFqrGr699ME4Iw9P1k/2wwqL3olZQdlxtT40k9VHvpdVy5IiOFvX21m+c70qjdq0RPanwvLX7UGpFPKxfz8/EhPT9ck0EgZY0hPT6/yNtjTqZcHwRq9fWvALwwi2wNw7Hgxn6zay+V9YmkdUYvJ4Cux24TnrurF6JeWcMfHa/nqzqE0C65iqInBd8L7Y2H9DOgz8ayPq1RFsbGxpKWlceTIEXeHUq2CgoIafdA1Bc602c/Pj9jYWKfr1ATgjP1roWUiOG7vnLkmjYLiMq4fHOeyQwT7efPfa/sw9uUl3DV9Le/fNAB75X6FdsnQvKc1Umjiddbw0Uq5iLe3d/lTqg1dSkqK00+7NhV10Wb9BKlOcQEc3gwtrV+8MYYPl+2mT5swElrW/tp/Vbq2COFvY7qzdEc6Ly3YfuoGItbTwenbYOs3Lj22UsrzaAKozuGNUFZcngBWpGaw82ge1w5oWyeHu6p/a8YktuSFBdtYn5Z16gYJY62hKPTBMKXUWdIEUJ39a62fLRIBmPPzfvy97Vzco3mdHfKJ0d1pFuTLPTPWnfqksN0LBk2Gvctgz/I6i0Ep1fRpAqjO/nXgHwFhbSgpLePrDQc5r2s0AT51130SGuDNs1f2YseRPJ76+tdTN+h9nTUnsU4bqZQ6C5oAqrN/XXkH8NId6WTkFXFpr5Z1ftghHaO4YXAc05buYsn2SlPQ+QRC3xtg8xzI2lPnsSilmiZNAGdSUgRHNkOLXgB8veEAQb5eDO/UrF4O/+DILrSLCuTBWes5XlRpeNj+twACK96ol1iUUk2PJoAzSd9mjcET0x1jDAt/PcKwTlH4eVc9GqGr+fvYeerynqRl5vPct1tPXhnWGhJGw5p3oSivXuJRSjUtmgDO5JBj3vvorvx6MIeD2QUkdzp1VqG6lBQfwbUD2vD2klR+3pt18sqBt0PBMfj54yr3VUqpM9EEcCaHN4HNCyI7krLFejpyeOf6ufxT0dSLuxAd7MeDs9ZTVFJh1NDY/tCqLyx71RqwTimlasCpBCAiI0Vki4hsF5GpVawfJiJrRKRERK6otK5URNY5XnMqlMeLyHJHnTMcs401LIc3QWRH8PIhZcthElqEEOPsfL4uFOznzZNju/PrwRxeX7TjtxUi1llA+jbY8X29x6WUatyqTQAiYgdeBi4GEoDxIpJQabM9wA3AR1VUkW+MSXS8Rlcofxp43hjTAcgEbqpF/HXr8CaISSCnoJjVuzNJdsO3/xPOT4hhVM8WvPD9drYfzv1tRcIYCG6ht4QqpWrMmTOAJGC7MWanMaYImA6cNI+ZMWaXMWY94NR1CMc8wOcCMx1F72LNC9xwFOZYt1hGd2XVrkxKygxDOkS5NaTHLu2Gn7eNR7/Y8NuIjXZv6H8z7FhgDVmhlFJOcuZpplbA3grv04ABNTiGn4isAkqAp4wxs4FIIMtY8w2fqLNVVTuLyCRgElgTMaekpNTg0L/Jzc2t0b4hx7bQB/jlcBkzN6/DLpCz+xdS0mo+8YsrjW1n471N6Tz98fcMbGn9+byLOjHQ5sOhzx9ja+fby7etaZubAm2zZ9A2u0Z9jAba1hizT0TaAQscE8Efc3ZnY8zrwOsA/fr1M8nJybUKIiUlhRrtu3o3rIUe517FwRkH6NXacNF559Tq2K40tMzw83+XMCu1gNt/fw4hft7WioLxtFw/g5YTXoWACKAWbW4CtM2eQdvsGs5cAtoHtK7wPtZR5hRjzD7Hz51ACtAbSAfCROREAqpRnfXi6Fbw8qcgKJb1aVkkxUe6OyLAmjvgybE9OJpbePKzAQNvg5ICWP2O+4JTSjUqziSAlUBHx107PsA4YE41+wAgIuEi4utYjgLOATY5ZqlfCJy4Y+h64IuaBl+njm6DyPas3ZtNcalhQHyEuyMq1yM2lAkD2/LeT7vYsM9xMhXdFdqNsJ4MLi12b4BKqUah2gTguE4/GZgHbAY+McZsFJEnRGQ0gIj0F5E04ErgNRHZ6Ni9K7BKRH7G+sB/yhjjeLqKB4F7RWQ7Vp/AW65s2FlL3w6RHViRmoEI9I0Ld3dEJ7nvws5EBPrw8OwNlJU5OoQH3g45B2BTw8qlSqmGyak+AGPMXGBupbJHKyyvxLqMU3m/pUCP09S5E+sOo4anpAgyd0G3y1i9O5POMcG/XWtvIEL9vXn4kq7cM+Nnpq/cyzUD2kCH8yGyAyx7BXpcUX0lSimPpk8CVyVrN5hSTGR71qdlkdg6zN0RVWlsYisGxEfw9De/cjS30JoicsCtsG8V7F3p7vCUUg2cJoCqpFvTMR72aUPW8WJ6xIa6OaCqiQhPju1OXmHJb/MG9BoPvjpXgFKqepoAqnJ0GwDrjlt3/vSKDXNjMGfWMSaYm4bEM3N1Gmv3ZIJvEPSZAJu+wLfgaPUVKKU8liaAqqRvh4AoVh8GHy8bnWKC3R3RGd1xXkeig315fM5Gq0M4aRJgaLl/brX7KqU8lyaAqjjuAFqflkXXFiH4eDXsX1OQrxcP/a4LP6cd49PVeyG8LXS5hJb7v4Wi4+4OTynVQDXsTzZ3Sd+OiezAhn3Z9Gqg1/8rG5vYir5tw/nXN1s4ll8MA2/HuyQH1s9wd2hKqQZKE0BlBdmQe4h0vzbkFpbQo1XjSAAiwl9HdyPjeBHPf7cV2gwiJ6g9LH8VTgwcp5RSFWgCqCxjJwC7TAwACS1D3BlNjXRvFcr4pDa8v2w3Ww7lkhY7Co78CjsXujs0pVQDpAmgsqzdAGzOj8BuEzpEB7k5oJqZcmFngny9eHzORg41GwKB0daDYUopVYkmgMoyrQSw4lgI8VGB+HrVzwTwrhIe6MP9F3bip53prDhis+YK2PZt+a2tSil1giaAyjJ3gV8Y646U0aV5w77983SuGdCWri1CmP5rEcd7TgC7Dyx/zd1hKaUaGE0AlWXtpjSsLXsz8httArDbHB3CBYZXVuVAjyth3UeQn+Xu0JRSDYgmgMoyd5PtZ01O1rl54+kAriwpPoKBLey8tmgnB7rcAMV5sPZ9d4ellGpANAFUVFYGWXs4INYdQI31DOCEqzv74GUTHllug7ZDYPnrUFpS/Y5KKY+gCaCi3INQWsiO4kiCfL2IDfd3d0RnJdzPxuRzOzB/8yE2tLkGju2BLV+5OyylVAPhVAIQkZEiskVEtovI1CrWDxORNSJSIiJXVChPFJGfRGSjiKwXkasrrJsmIqkiss7xSnRJi86G4w6gDcfD6BgThIh7J4B3hZuGxBMXGcA9a5tjwtrCslfdHZJSqoGoNgGIiB14GbgYSADGi0hCpc32ADcAH1UqPw5MNMZ0A0YC/xaRsArrpxhjEh2vdbVqgSs5ngFYnR1Ku6jGdf//6fh62Xn4kgS2HS1gRbMrYM9S2L/O3WEppRoAZ84AkoDtxpidxpgiYDowpuIGxphdxpj1QFml8q3GmG2O5f3AYaCZSyKvC5m7MAjrc0No1yzQ3dG4zPldoxnSIYp7tvXAeAdaw0MopTyeMwmgFbC3wvs0R1mNiEgS4APsqFD8d8eloedPTB7vVpm7KQ6IoQhv2jehBCAiPDIqgUNFviwLvRh+mQk5h9wdllLKzZyaE/hsiUgL4H3gemPMibOEh4CDWEnhdaxJ4p+oYt9JwCSAmJgYUlJSahVDbm5utfsm7vqZHGNN/p6eupmUo1tqdayGonKbk2Pt/HnvIBb4zmL3zEfYFX+N+4KrI878nZsabbNnqIs2O5MA9gGtK7yPdZQ5RURCgK+Ah40xy06UG2MOOBYLReQd4P6q9jfGvI6VIOjXr59JTk529tAnSUlJodp91+awP6gbtiy44uLhjW4YiMoqt7lX/yKSn01hrW8SvY8uIO66F8Dbz30B1gGn/s5NjLbZM9RFm525BLQS6Cgi8SLiA4wD5jhTuWP7z4H3jDEzK61r4fgpwFhgQw3idr2yUsjZz97ScFpHBDT6D/+qhAf6cPf5HXk2+zwk7whsmOXukJRSblRtAjDGlACTgXnAZuATY8xGEXlCREYDiEh/EUkDrgReE5GNjt2vAoYBN1Rxu+eHIvIL8AsQBTzpyobVWO5hKCthW0EY7aKazvX/yq4b2JbDkQPYKW0oW/ZfnStAKQ/mVB+AMWYuMLdS2aMVlldiXRqqvN8HwAenqfPcGkVa17Ktq1obcgJpl9A0bgGtirfdxl9GJfDaexfx9KE3YNdiiB/q7rCUUm6gTwKfcCwNgN0lEU3qFtCqJHeOJrPdGNJNCEWL/u3ucJRSbqIJ4ATHGcB+E9lkHgI7kwdH9+bd0ovwSZ0Phza5OxyllBtoAjjh2D5K7H4cI5D4JtwHcEL7ZkGU9L2J48aXzO//z93hKKXcQBPACdlpHPOOwdfLTnSw+59Jqw9/vKgfn8t5BG/9HOO4BKaU8hyaAE44to/DEkVsuD82W+MfBM4ZoQHe+A+/E4wh9ctn3R2OUqqeaQI4IXsfe0vDaRMR4O5I6tXoYQNY5DOU5ts+piAnw93hKKXqkSYAgNJiTM5BdhSGeVwC8LLbiLjgfgIoYO1n2heglCfRBACQcwDBsKvEegrY0yQmDWOjfz867PyAw5nH3B2OUqqeaAIAOGbdAnrARHhkAgCIuHAKzSSLRZ++7O5QlFL1RBMAnPQMgKddAjqhReJFHAjoTO+099iQlunucJRS9UATAJQ/BXzARHrsGQAihJ53H+1tB/h61tsYHSNIqSZPEwBAzkEKbAH4BoYS5FsvUyQ0SAGJl5PjH8sF6R/wzS8Hqt9BKdWoaQIAyDlAps1zr/+Xs3sRcO79JNp28t1X0ykoLnV3REqpOqQJACD3EAfLQmkd7u/uSNzO3vsaCgOac3X+DN5Zssvd4Sil6pAmAMDkHCStOETPAAC8fPEdfh8DbL+yfOEcDucUuDsipVQd0QRgDCbnIAdNOLF6BmDpM4GSgGbcYmby3Ldb3R2NUqqOOJUARGSkiGwRke0iMrWK9cNEZI2IlIjIFZXWXS8i2xyv6yuU9xWRXxx1vuCYGrL+FWZjK8nnsAmjZagmAAC8/fE6507OsW1gy+oFbNyvD4cp1RRVmwBExA68DFwMJADjRSSh0mZ7gBuAjyrtGwE8BgwAkoDHRCTcsfoV4Bago+M1statOBs5hwCsBBCmCaBcvz9Q5h/B3T5zeOJ/m/S2UKWaIGfOAJKA7caYncaYImA6MKbiBsaYXcaY9UBZpX0vAr4zxmQYYzKB74CRjgnhQ4wxy4z1yfIe1sTw9S/3IACHCadFmJ9bQmiQfIOwDbqd4awmd9ca5m086O6IlFIu5sxN762AvRXep2F9o3dGVfu2crzSqig/hYhMAiYBxMTEkJKS4uShT5abm1vlvtGHUkgAsiSMNcuW1Kruhup0bXaWvSSBgfYA7vebzQOz4rEf/hXvBj5U9tm2uTHSNnuGumhzg3/qyRjzOvA6QL9+/UxycnKt6klJSaHKfZesh83gExFb9fpG7LRtrgnbZEYs+heRhbvZYb+QW4e3d0lsdcUlbW5ktM2eoS7a7MwloH1A6wrvYx1lzjjdvvscy7Wp07VyD1GIL6FhkW45fIM36HbwDeUf4f/jpQXbOZJT6O6IlFIu4kwCWAl0FJF4EfEBxgFznKx/HnChiIQ7On8vBOYZYw4A2SIy0HH3z0Tgi1rEf/ZyDnCYcFrpLaBV8w+HwZPpc3wJ7Uu28dx3W9wdkVLKRapNAMaYEmAy1of5ZuATY8xGEXlCREYDiEh/EUkDrgReE5GNjn0zgL9hJZGVwBOOMoDbgTeB7cAO4GuXtsxJZdkHOVAWSgu9BfT0BtwK/hE8G/kl01fu1dtClWoinOoDMMbMBeZWKnu0wvJKTr6kU3G7t4G3qyhfBXSvSbB1oTT7AIdNM1qE6h1Ap+UXAkPupuN3jzLc73f87csIPr5lIO56dEMp5Roe/ySwLfcQR/QZgOr1vwUCo3kqfA7LdmYwb+Mhd0eklDpLnp0ACnOxl+RxyITrGUB1fAJg6H00z1jJlRE7+MfczRSW6GihSjVmnp0AcvUp4BrpewOEtOIvAZ+xJyOPaTpaqFKNmmcngBxr0pN8v2b4edvdHEwj4O0Hw+4n9Oha7mmTyot6W6hSjZpnJwDHGYAExbg5kEak9wSIaM9tJe9TVFzMc9/paKFKNVaenQDyjgLgHdrczYE0InZvOP8xfDK28GzHjcxYuYdN+7PdHZVSqhY8PAEcoRQbgWFR7o6kcek6GmL7Myr9baL9yvjblzpaqFKNkUcngLLcw2SaIKJCAt0dSuMiAhf8DVvuQV5pv4yfdqbrbaFKNUIenQCKjh3mqAklJsTX3aE0Pm0HQZdRJO55lwHRpTzxv43kFZa4OyqlVA14dAIozTlMugkhOlifAaiV8x5Dio/zYqvv2H+sgH/P1w5hpRoTj04Acvwo6YToGUBtNesEfa8nestHTO4lvL1kl3YIK9WIeHQC8CpI1zOAs5X8EHj5cVfpu4T5e/Pnz3+hrEw7hJVqDDw3ARQX4FOSSzqhRAX5uDuaxisoGoZNwXv7N7yQlM66vVl8tGKPu6NSSjnBcxPAcesZgAKfCLzsnvtrcImBt0FEOwZvfZah7UJ4+ptf9QlhpRoBz/3kyz0MQFlAMzcH0gR4+cLIp5D0bfw7fgWFxWU8Pmeju6NSSlXDqQQgIiNFZIuIbBeRqVWs9xWRGY71y0UkzlF+rYisq/AqE5FEx7oUR50n1kW7smHVcjwFLEH6EJhLdLoIOl5I5Kp/M3VYBF/9coAv1+93d1RKqTOoNgGIiB14GbgYSADGi0hCpc1uAjKNMR2A54GnAYwxHxpjEo0xicAEINUYs67CfteeWG+MOXzWramJvCMA+IToMBAuc9E/oTifG/Lfo1dsKI/M3qCXgpRqwJw5A0gCthtjdhpjioDpwJhK24wB3nUszwTOk1Onixrv2LdBKHVcAgoI14HgXCaqAwy8Ddu6D3hxWBl5RaX8ZfYvOkyEUg2UMwmgFbC3wvs0R1mV2zjmED4GRFba5mrg40pl7zgu/zxSRcKoUwVZh8g3PoSFhdfnYZu+YVMgqDltlj7M/ee1Y97GQ8z5WS8FKdUQOTUn8NkSkQHAcWPMhgrF1xpj9olIMDAL6xLRe1XsOwmYBBATE0NKSkqtYsjNzT1p39idm/AjhCN7tpNSuKtWdTZ0ldtcX5q1mUi3Tf9iROCrfBJ2IVNnrqNo/xaaBdT9PQfuarM7aZs9Q5202RhzxhcwCJhX4f1DwEOVtpkHDHIsewFHAamw/nngz2c4xg3AS9XF0rdvX1NbCxcuPOn9kVcuMWsfSTRr92TWus6GrnKb601ZmTEfXGnMky1MWuoW0/3Rb8zYlxebopLSOj+029rsRtpmz3A2bQZWmSo+U535SrYS6Cgi8SLiA4wD5lTaZg5wvWP5CmCB46CIiA24igrX/0XES0SiHMvewChgA/XIdvwo6SaU6GAdBsLlROCSZwFDq6WP8tTve7B2T5ZOHqNUA1NtAjDWNf3JWN/yNwOfGGM2isgTIjLasdlbQKSIbAfuBSreKjoM2GuM2VmhzBeYJyLrgXXAPuCNs21MTfg4hoGI1KeA60ZYGxjxZ9j6NZd4r2J8UhteSdnBoq1H3B2ZUsrBqT4AY8xcYG6lskcrLBcAV55m3xRgYKWyPKBvDWN1HWPwK84gxysMXy+dC7jODLgNfp4BXz/Ao5N+Ys3uTO6cvpY5fxpCm8gAd0enlMfzzCeBC47hZUoo9Kl8o5JyKbsXXPofyD2Ef8pfeX1iX4yBW95bRa7OHaCU23lmAnA8BVzirwmgzsX2hUGTYfU7tM1cxsvX9GH7kVzunbFORw1Vys08MwEcTwdAAjQB1IsRD0NUJ5hzJ0Nae/Pw77ry7aZD/PPrze6OTCmP5pkJID8DAK9gTQD1wtsPxr4KOfth3sPceE4cEwe15Y0fU3n1hx3ujk4pj1UvD4I1NKW5R7EDPsE6Emi9ie0L59wFi59HEsbw+KXnk3m8mKe+/pXwAG+u7t/G3REq5XE88gzg+DHrVsTA8PodgNTjJT8EzbrCnDuwFWTyf1f2YlinZkz97Bc+Wbm3+v2VUi7lkQmgMPsoxcZOaIiOA1SvvHzhsleskVj/dxc+duG16/oytGMzHpi1nneX7nJ3hEp5FI9MAMU5R8gkmEidC7j+tewN5z4Cm+fAmnfx97HzxsS+XJgQw2NzNvLct1v07iCl6olHJgBzPINME6RzAbvL4Dshfjh8PRWObMHXy87L1/bhqn6xvLBgO5M/XkN+Uam7o1SqyfPIBCD5GWQRRGSQjgPkFjYbXPYaePvDzJuguABvu42nL+/Jw7/rytcbDnLFq0vZeSTX3ZEq1aR5ZALwKswkixBC/DzyJqiGIaQFjP0vHPoF5j8OgIhwy7B2vHV9P/Zl5XPJC4v5ZOVenVBGqTrikQnAr/gY+V6h1PMcNKqyzhdD0h9h+Suw6Yvy4nO7xPD1XUNJbB3GA7PWc9O7q9iTftyNgSrVNHleAjAG/5JjFPuEujsSBXDh36BVX5j9Jzi6rby4Rag/H948gL9c0pXlO9M5//kf+Pf8rRQUa9+AUq7ieQmgMBsvSin1j3B3JAqsW0Oveg+8fGDGdVD423V/m024eWg7vr8vmYu6Neff87eR/EwK7/+0i8ISTQRKnS3PSwDHrWEg0IHgGo7QWLj8LTi6Ff53J1S65t881I8Xx/dm+qSBxIb788gXGxnxTArvLt1Fno4qqlSteVwCMI4EYA/UM4AGpf0IOPcvsGEWLH+1yk0Gtovk01sH8f5NSTQP9eOxORsZ+M/v+cfczaRlah+BUjXlVAIQkZEiskVEtovI1CrW+4rIDMf65SIS5yiPE5F8EVnneL1aYZ++IvKLY58XpJ56ZPOPHQbAOySqPg6nauKce6DzJTDvYdj+fZWbiAhDOzZj1m2DmXXbYIZ1asZbi1MZ9q+F3PzuKtYfKaFUHyRTyinVJgARsQMvAxcDCcB4EUmotNlNQKYxpgPWBPBPV1i3wxiT6HjdWqH8FeAWoKPjNbL2zXDe8SxrHCC/EB0HqMGx2eD3r0F0V/j0Bjiy5bSbigh924bz8jV9+PGBEfxxeHvW7c3kudWFDPvXQl5euJ3DOQX1F7tSjZAzZwBJwHZjzE5jTBHW5O5jKm0zBnjXsTwTOO9M3+hFpAUQYoxZ5pg8/j1gbE2Dr43CbGsyGP9QPQNokHyDYfx08PKDj66CvPRqd2kZ5s+DI7uwdOp53J7oS9vIAJ6Zt4XB/1zA5I/WsHJXhj5LoFQVnHkSqhVQcajGNGDA6bYxxpSIyDHgRC9rvIisBbKBvxhjfnRsn1apzlZVHVxEJgGTAGJiYkhJSXEi5FPl5uaSkpJCwI6NNDfC9tQ9mKyDtaqrsTjR5sYopNP9JK57mOzXR/FzrycwNm+n9ksIKiCpuRejW/qzcG8xCzYd4Mv1B2gdbOP8Nl4MbOmFr71pPf/RmP/OtaVtdo26fhT2ANDGGJMuIn2B2SLSrSYVGGNeB14H6Nevn0lOTq5VICkpKSQnJ7Nz10ccOxLIuUPPIT4qsFZ1NRYn2tw4JUO7SMJm3cTwzE+soSNs1Z+wVmzzOCC/qJTZ6/bx7tJdvLMxh1k7ypg4KI4bz4lrMkOBNO6/c+1om13DmQSwD2hd4X2so6yqbdJExAsIBdIdl3cKAYwxq0VkB9DJsX1sNXXWjfxMMk0wUQE6EFyD1+MKyEyFBU9CUDRc+CTU8F4Bfx8745PaMK5/a1buyuStxTt5OWU7by7eydX9WnPz0Ha0jgioowYo1bA5kwBWAh1FJB7rQ3occE2lbeYA1wM/AVcAC4wxRkSaARnGmFIRaYfV2bvTGJMhItkiMhBYDkwEXnRNk87MXpDBEYKJ13GAGoeh90PuEfjpJQhsBkPurlU1IkJSfARJ8RFsP5zL64t28NGKPXy4fA/jklpzx7kdiQnR4cGVZ6n2U9BxTX8yMA+wA28bYzaKyBPAKmPMHOAt4H0R2Q5kYCUJgGHAEyJSDJQBtxpjHE9icTswDfAHvna86pxPYRZ5tjBstqZ1HbjJEoGRT8HxdJj/GARGQe/rzqrKDtFB/OuKXtx9fif+m7Kd6Sv28umqNG4YHMetw9sTHqhnh8ozOPU12BgzF5hbqezRCssFwJVV7DcLmHWaOlcB3WsSrCv4lRzjuFfb+j6sOhs2G4x9BfIzYM6d4BsCCaPPutqWYf48ObYHk4a259/zt/L6jzv5cPkebhnajpuGxhPkq2eJqmnzuCeBA0qzdSC4xsjLB6563xo4buaN8OtXLqu6TWQAz12dyLy7hzGkQxTPz9/KsH8t5J0lqTrmkGrSPCsBFBfgawop9Q1zdySqNnyD4LqZ0KIXfHI9bPnGpdV3ignm1Ql9+eJP59CleTB//d8mzn/uB75Yt0+nqVRNkmclgIJj1k+/MLeGoc6CXyhc9xk07w6fTICt37r8EL1ah/HhzQN47w9JBPt6c9f0dVz60mJ+3HbE5cdSyp08KgGY/EwAbAFh7g1EnR3/MJjwuTVkxIxrXXo56AQRYVinZnx5xxD+My6RY/nFTHhrBde+uYxf0o65/HhKuYNHJYCCHCsBeAeGuzkSddb8w2HCbGjeE2ZMgHUf18lhbDZhTGIrvr9vOI9dmsDmAzlc+tJiJn+0hl1H8+rkmErVF4+6zSH32FH8AZ9gHQq6SQiIgIlfwPRrYPatjkt8XerkUL5edm48J54r+sbyxqKdvPFjKt9sOMi4pNb8cVh7fZhMNUoedQaQn209guAfrJPBNBm+QXDtp9D1UvjmQeJSPzplQhlXCvbz5t4LO/PDlGSu7t+aGSv3kvxsCnd+vJaN+/XSkGpcPCoBFOZaI0sGhWkCaFK8fOGKadD7OuJ2z4DZt0FJYZ0eMjrEj79f1oNFD4zgD+fE8f3mQ1zywmLGvf4Tn69N07mLVaPgUQmgJM/qAwgK06Ggmxy7F4x+idS4a+Dnj+H9y36b/rMOtQj15+FLElj60Hk8OLIL+7MKuGfGz/T/+3z+MvsXlmw/SnFpWZ3HoVRteFQfQOnxLI4bXyKCg9wdiqoLIuyOu5r4vufB7NvhzfPgmk8hqkOdHzrU35vbktvzx2HtWJ6awSerrOElPli2h2BfL4Z3bsbwTs1Iio+gTUQA9TQBnlJn5FEJgPxMsgmgmb9zY8urRqrHFRDaGqaPhzfPhd+/AZ0uqpdD22zCoPaRDGofyd8v687ibUeZv/kQC349zJfrDwAQFeRLQssQOkYH0TE6iPbRQTQP8SM6xBdfL3u9xKkUeFgCkMJsciWI5joQXNPXZgDcsgBmXGfNLDbsAUieCrb6+4AN8PHiwm7NubBbc8rKDNsO57JyVwZr9mSy9VAOHy5Pp6D45MtDYQHeRAf7EuLnTZCfF8F+3gT5ehHi50WQr1d5WbCfF8F+XkQG+pJdaCgtM9j137WqIY9KAF5F2Ry3Bbs7DFVfwuPgpu/gq/tg0b9g3yq4/C3r9tF6ZrMJnZsH07l5MNcNtAYjLCsz7MvKZ8eRXA5nF3Iou4DDOYUczikgp6CEjLwidqcfJ6eghNzC4lOSRUV3pcwlIsCH1hEBtIsKpF2zQNo1C6Jds0DiIgPx89YzC3Uqj0oAPiU55HjpMwAexdsfxrwMsf3h6wfg1aHWxPNxQ9wdGTab0DoiwOlnCIpKysgtLCG3oITsgmKyC4rJyCti2dqNRLRow5HcQnanH2fpjnQ+W/vb/Eoi0C4qkF6xYSTFRzCkYxSx4frcgvKwBOBfmkNRQJy7w1D1TQT63WgNIjfrJpg2yppYJvnP1iijjYSPl40ILx8iKs1XEJSxleTkzieV5RWWkHo0j51H89hxOJeN+4+xaNuR8sQQHxXIkA5RDOkYxaD2kYT4ab+YJ3IqAYjISOA/WBPCvGmMearSel/gPaAvkA5cbYzZJSIXAE8BPkARMMUYs8CxTwrQAsh3VHOhMebwWbfoDALLcijVoaA9V6s+8Mcf4ZupsPh52LEQLn8Tojq6OzKXC/T1onurULq3+u3fuzFWP8SP246yeNsRZq1J4/1lu7HbhEHtIhndqyUXdW9OqN4k4TGqTQAiYgdeBi4A0oCVIjLHGLOpwmY3AZnGmA4iMg54GrgaOApcaozZLyLdsWYVa1Vhv2sdE8PUPVNGoMnH+GoC8Gi+QTDmJeuuoDl3WJeERvwZBt5uPUvQhIkInWKC6RQTzE1D4ikqKWPtnkx+2HqEr345wAOz1vOX2RtI7tyM0YktOa9LDP4+2nfQlDnzLz4J2G6M2QkgItOBMUDFBDAGeNyxPBN4SUTEGLO2wjYbAX8R8TXG1O1jmlUpysMmxhpJUqmul0KrfvDVvfDdI7BhFox+EVr0dHdk9cbHy8aAdpEMaBfJlIs6sz7tGHN+3s+X6/fz7aZDBPl68fs+rZgwsC0dY/TmiaZITDXjpojIFcBIY8zNjvcTgAHGmMkVttng2CbN8X6HY5ujleq51RhzvuN9ChAJlGJNG/mkqSIYEZkETAKIiYnpO3369Fo1NPvgTkb/eg+zov5EZPcLa1VHY5Obm0tQkGc99FbjNhtDsyNL6bjtNbyLc9jT5jJ2t72KMnvjmSDe1X/nMmPYklHG4n0lLD9YQkkZdImwcV4bb3pH2/FqALeb6r/tmhkxYsRqY0y/yuX1cs4rIt2wLgtV/OS91hizT0SCsRLABKx+hJMYY14HXgfo16+fSU5OrlUMX8/YBkBs+y4MqGUdjU1KSgq1/X01VrVr8wg4fht8+xfarvuQtlnL4IInoPvlVgdyA1cXf+dzgduAjLwiZqzcywfLdvPyunxiQny5Jqkt45NaEx3iviSp/7Zdw5mxgPYBrSu8j3WUVbmNiHgBoVidwYhILPA5MNEYs+PEDsaYfY6fOcBHWJea6owpzAXAJ0jnAlBVCIiAsf+FG7+BgEjrbqF3LoYDP7s7MreKCPThtuT2LHpgBG9O7Efn5iE8P38rg59awOSP1rAiNYPqriKohsuZM4CVQEcRicf6oB8HXFNpmznA9cBPwBXAAmOMEZEw4CtgqjFmyYmNHUkizBhzVES8gVHA/LNtzJmYYisB+OlQ0OpM2g6CSSmw9gP4/gl4bTj0Gmc9RRwe5+7o3MZuE85PiOH8hBhSj+bxwbLdfLpqL1+uP0CX5sFMGNSWsYmtCPRt2h3pTU21ZwDGmBJgMtYdPJuBT4wxG0XkCREZ7djsLSBSRLYD9wJTHeWTgQ7AoyKyzvGKBnyBeSKyHliHlVjecGG7TlVkzd7kH6IJQFXDZoe+18Mdq2HwHbDxc3ixH3x5L2QfcHd0bhcfFcgjoxJY/ufzeer3PbCJ8PDnGxj4j+95fM5GdhzJdXeIyklOpWtjzFxgbqWyRyssFwBXVrHfk8CTp6m2r/Nhnj2b4wwgWIeCVs7yD4ML/2bdIrroGVjzLqz7EPrfDIMmQ0gLd0foVv4+dsYlteHq/q1ZsyeL93/axYfLdzNt6S6Gdoxi4qA4zu0SrWMUNWAeMx+AV3EuJcZGSEiYu0NRjU1ICxj1HExeBd0ug2WvwH96Ws8RHN3u7ujcTkTo2zacf4/rzdKp53H/hZ3YdiiXW95bxbB/LeQ/87exPyu/+opUvfOYBOBdkkcOgXjrcLuqtiLi4bJX4c410Od6WP8JvNTPmpR+9091OhVlY9Es2JfJ53Zk8YMjeOXaPsRHBfL8/K0MeXoBN76zgnkbD+oEOQ2Ix/TY+JTmkWsLQu8BUmctPA4ueRaGPwjLX4WVb8DmORDT3bo81PMq8Al0d5Ru5WW3cXGPFlzcowV7M47zyaq9fLJqL398fzWRgT5c1L05F3dvzsB2kXjbPeZ7aIPjMQnArzSP4zbPenBE1bGgZnDeIzD0XvjlU1jxJnx5N3z3GCSOh8RroHnPRvEsQV1qHRHAfRd25q7zOpKy5Qiz1+1j9tp9fLR8D2EB3lzQNYbf9WjB4A6ROiFOPfOcBFCWR4G3Ps6u6oBPIPS9wbostHc5rHwTVr1tnR1Ed7NuI+15FQQ3d3ekbuVlt5XfSlpQXMqirUf4esNBvtlwkE9XpxHs68X5CTGM7N6cIR2i9JbSeuAxv+FAk8dh71bVb6hUbYlAm4HW6+J/wcbPYN3H1lhD8x+DdiOg21jofAkEevbtyH7e9vLZ0gpLSlm6PZ25vxzg202H+HztPuw2oXurUAbER9A/LoL+ceGEBTSeobsbC49JAEHkst9HzwBUPQmIsPoD+t8MR7fBz9Oty0Rz7gC5C9qeAwljoMsoj7+d1NfLzogu0YzoEs0/SstYvjODZTvTWZGawbQlu3h90U4AujQPJik+gr5tw8nLLdNpMF3AMxKAMQSb45T5hrk7EuWJojpafQXn/gUOrodNc6xO47n3W6+WvaH9edDhfGvmsiY+LPWZeNttDOloTVQDUFBcys97s1iRmsGKXRnMXJ3Gez/tBuBvy+fRpUUw3VqGkNAilG4tQ+jcPFinv6wBj/iXVlyYh4+UgJ/OBaDcSMSalaxFLyshHNliJYLt31sT1Pz4LPiGQrthVkKIGwKRHTy6E9nP214+ZDVAcWkZWw/l8NmCFZSFtmTj/my+WLufD5btAawhK9o3CyShRQjdWobSrVUIvWLDtD/hNDzit5KTlU4EYNO5AFRD0qwzNJsCw6ZAfhak/gDb51sJYfP/rG0Cm0HbwdBmsPUzpps1VIWH8rbb6NYylCOx3iQndwOsmc72ZuSz6cAxNu7PZtP+bJbtzGD2uv0A2AS6tgihT5tw+rYNp0+bcFpH+CMenFhP8IgEkJt1lAjAHqhPAagGyj/M6hNIGGM9UHZ0G+xZaj1gtnspbPrC2s43xDqDaNnbmuKyZR+PfwBNRGgTGUCbyABGdv+tPyU9t5D1+46xdncmq/dk8pljCkyAqCCf8oRwbpdoj53wxiMSQH52OgA+mgBUYyACzTpZr743WGVZe2HPT7BnGexfa91iWloEwGDvENiXZJ0dRCdAdFeI6gTe/u5rQwMQGeTLiM7RjOgcDUBpmWHLwRzW7Mlkze5M1uzJ5NtNh/jn17/SvlkgI7s3Z2S3FnRvFeIxZwcekQAKczMA8NORQFVjFdbaevW8ynpfUgiHN8G+NaSvnkuLnEOQuqg8KSA2iGhnJYNmXa2+hIh21isgwiP7Few2IaFlCAktQ7huYFsADh4r4LtNB/lm40Fe/WEnLy/cQaswfysZdG9Ov7bhTToZeEQCKM7NBHQoaNWEePlal4Fa9mZLXntaJCdDaTFk7LQSw+HNv/389SswFcbf8Qv9LRlEtLOGtghpBaGtIaQl+AS4q1X1rnmoHxMGxTFhUBwZeUXM33yIeRsO8v5Pu3lrcSqdYoL4wznxjO3dqkneXeQRCaD0uJUAgkI1AagmzO7t6FjubI1aekJJIWTuhowdVoI48dq32prrwFQanM0/AkJbQUgshMZaSSEoBoKirU7pEz/t3vXbvjoWEejDVf1ac1W/1uQUFDNv4yHeXpzK1M9+4V/ztnDdgDZcN6gt0cGNZ77o6nhEAig7ngVASLjOBaA8kJfvb30KlZUUQXYaHNsH2fvgWNpvP7P2WB3RBceqrtc/HAKjf0sIARFWmV+Y1aldvhxuvfcLs/olGsEllWA/b67oG8vlfVqxbGcGby1O5cWF23n1h51c2qslNw2JJ6FliLvDPGtOJQARGQn8B7ADbxpjnqq03hdrQve+WHMBX22M2eVY9xBwE1AK3GmMmedMna4kBVnkGT8CvfVRcqVO4uXz26Wg0ynMhbzDkHvE8fMw5B1x/HSUH1gH+ZlWsqh8RlGR3ddKBj5B1hhKvsEVloPAJ7jCsuPlG2QlDi+/8pdf/gFrdjYvX2ud3Rdsrh9VVEQY1D6SQe0jST2ax7QlqXy6Oo1Za9IY1C6SW4bFM6JzdKPtJ6g2AYiIHXgZuABIA1aKyBxjzKYKm90EZBpjOojIOOBp4GoRScCaQ7gb0BKYLyInvoZUV6fL2IqyyZZAPHuAXqVqydfxIXymJHFCWRkUZkNBlvVsQ35m1ctFeVCUayWX3IPW+8Jcq6yo+iklBwIsr1Ro9wVvv5MSBd5+YPcBm7f1hHX58omXD9i8Ki37/Lbe5l3+Pt5m56+xdh5sDst2ZfHjtuXMfq+U1VFBXJrYmi4twqxnNMRuJSOxV3h/mnKxOZYr/Kz8QqyfprQmfzWnOHMGkARsN8bsBBCR6cAYoOKH9RjgccfyTOAlsVLiGGC6MaYQSHXMGZzk2K66Ol3Gu+gYeXhOx5ZSbmOzOS7/hFHryTfKyqD4+G8JoigHigug5LfX5l/W0rVDnNW/UZxv/SzJP2U7igugrNjqIC8psuo78b60+OTl8vdFUFZy2vACgHMdL3yAbGBRLdtaAwH9X3Z5nc4kgFbA3grv04ABp9vGGFMiIseASEf5skr7nhiSs7o6ARCRScAkgJiYGFJSUpwI+WR5Pu2BGNJqsW9jlpubW6vfV2OmbW7KBPAH/MkNSuJQbtDJq7wdL1cwBjGliCnBVlaCmBLH+zLElAFljmVDcWkpqw4WsXhvEQUlZXSLgHNb22nmZyptW3nfqtYZwCDGONad+AmZxd4u/zs3+E5gY8zrwOsA/fr1M8nJyTWvJDmZlJQUarVvI6Zt9gzaZvc7B/hDQTFvLU7lzR9T+eTnEi7rHcvd53ekdYRrrj7sq4M2O9Nrsg9oXeF9rKOsym1ExAsIxeoMPt2+ztSplFKNRrCfN3ef34lFD4zgpiHx/G/9fs79vxQen7ORIzmF7g6vSs4kgJVARxGJFxEfrE7dOZW2mQNc71i+AlhgjDGO8nEi4isi8UBHYIWTdSqlVKMTEejDw5ck8MOUZK7oG8v7y3Yz7F8LeWberxzLL3Z3eCepNgEYY0qAycA8YDPwiTFmo4g8ISKjHZu9BUQ6OnnvBaY69t0IfILVufsN8CdjTOnp6nRt05RSyn1ahPrzz9/3ZP69wzk/IYaXF+5g6NMLePH7bRw73jASgVN9AMaYucDcSmWPVlguAK48zb5/B/7uTJ1KKdXUxEcF8uL43tw6vB3PfbuV//tuK68t2sn4pNZMHBTnsj6C2mjwncBKKdUUdGsZyls39GfT/mxe/WEHby/ZxRs/ptI/LpyxvVtxSY8W9T7vsSYApZSqRwktQ3hhfG8evLgLs9fuY/bafTz8+QYen7OR4Z2iGdYpir5tw2kTEUCQr1edPmWsCUAppdygVZg/fxrRgduT27PpQDaz1+7jy/UHmL/5UPk23nYh1N+HQF87k7u5fuIfTQBKKeVGImLNX9wylD//ritpmfms2ZPJoewCso4Xk3m8mONFJdhtmS4/tiYApZRqIESE1hEBVXYM18XT3q4fPk8ppVSjoAlAKaU8lCYApZTyUJoAlFLKQ2kCUEopD6UJQCmlPJQmAKWU8lCaAJRSykOJNWx/4yAiR4Ddtdw9CjjqwnAaA22zZ9A2e4azaXNbY0yzyoWNKgGcDRFZZYzp5+446pO22TNomz1DXbRZLwEppZSH0gSglFIeypMSwOvuDsANtM2eQdvsGVzeZo/pA1BKKXUyTzoDUEopVYEmAKWU8lAekQBEZKSIbBGR7SIy1d3x1DURaS0iC0Vkk4hsFJG73B1TfRARu4isFZEv3R1LfRCRMBGZKSK/ishmERnk7pjqmojc4/g3vUFEPhYRP3fH5Goi8raIHBaRDRXKIkTkOxHZ5vgZ7opjNfkEICJ24GXgYiABGC8iCe6Nqs6VAPcZYxKAgcCfPKDNAHcBm90dRD36D/CNMaYL0Ism3nYRaQXcCfQzxnQH7MA490ZVJ6YBIyuVTQW+N8Z0BL53vD9rTT4BAEnAdmPMTmNMETAdGOPmmOqUMeaAMWaNYzkH64OhlXujqlsiEgtcArzp7ljqg4iEAsOAtwCMMUXGmCy3BlU/vAB/EfECAoD9bo7H5Ywxi4CMSsVjgHcdy+8CY11xLE9IAK2AvRXep9HEPwwrEpE4oDew3M2h1LV/Aw8AZW6Oo77EA0eAdxyXvd4UkUB3B1WXjDH7gGeBPcAB4Jgx5lv3RlVvYowxBxzLB4EYV1TqCQnAY4lIEDALuNsYk+3ueOqKiIwCDhtjVrs7lnrkBfQBXjHG9AbycNFlgYbKcd17DFbyawkEish17o2q/hnr3n2X3L/vCQlgH9C6wvtYR1mTJiLeWB/+HxpjPnN3PHXsHGC0iOzCusR3roh84N6Q6lwakGaMOXFmNxMrITRl5wOpxpgjxphi4DNgsJtjqi+HRKQFgOPnYVdU6gkJYCXQUUTiRcQHq9NojptjqlMiIljXhjcbY55zdzx1zRjzkDEm1hgTh/X3XWCMadLfDI0xB4G9ItLZUXQesMmNIdWHPcBAEQlw/Bs/jybe8V3BHOB6x/L1wBeuqNTLFZU0ZMaYEhGZDMzDumvgbWPMRjeHVdfOASYAv4jIOkfZn40xc90XkqoDdwAfOr7Y7ARudHM8dcoYs1xEZgJrsO50W0sTHBJCRD4GkoEoEUkDHgOeAj4RkZuwhsS/yiXH0qEglFLKM3nCJSCllFJV0ASglFIeShOAUkp5KE0ASinloTQBKKWUh9IEoJRSHkoTgFJKeaj/B8aev/2kCfRmAAAAAElFTkSuQmCC",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -451,14 +450,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
+            "version": "3.9.15"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `torchphysics-1.0.0/examples/deepritz/corner_pde.ipynb` & `torchphysics-1.0.1/examples/deepritz/corner_pde.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/deepritz/poisson-equation.ipynb` & `torchphysics-1.0.1/examples/deepritz/poisson-equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/fdm_heat_equation.py` & `torchphysics-1.0.1/examples/fdm_heat_equation.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/data/heat-eq-inverse-data.npy` & `torchphysics-1.0.1/examples/pinn/data/heat-eq-inverse-data.npy`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/exp-function-with-param.ipynb` & `torchphysics-1.0.1/examples/pinn/exp-function-with-param.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/hard-constrains.ipynb` & `torchphysics-1.0.1/examples/pinn/hard-constrains.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/heat-equation.ipynb` & `torchphysics-1.0.1/examples/pinn/heat-equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/interface-jump.ipynb` & `torchphysics-1.0.1/examples/pinn/interface-jump.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/inverse-heat-eq.gif` & `torchphysics-1.0.1/examples/pinn/inverse-heat-eq.gif`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/inverse-heat-equation-D-function.ipynb` & `torchphysics-1.0.1/examples/pinn/inverse-heat-equation-D-function.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/inverse-heat-equation.ipynb` & `torchphysics-1.0.1/examples/pinn/inverse-heat-equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/moving-heat-eq.gif` & `torchphysics-1.0.1/examples/pinn/moving-heat-eq.gif`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/moving-heat-equation.ipynb` & `torchphysics-1.0.1/examples/pinn/moving-heat-equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/periodic-boundary-problem.ipynb` & `torchphysics-1.0.1/examples/pinn/periodic-boundary-problem.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/poisson-equation.ipynb` & `torchphysics-1.0.1/examples/pinn/poisson-equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/poisson-with-input-params.ipynb` & `torchphysics-1.0.1/examples/pinn/poisson-with-input-params.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/signorini-equation.ipynb` & `torchphysics-1.0.1/examples/pinn/signorini-equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/pinn/singular-boundary-problem.ipynb` & `torchphysics-1.0.1/examples/pinn/singular-boundary-problem.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/Introduction_Tutorial_PINNs.ipynb` & `torchphysics-1.0.1/examples/tutorial/Introduction_Tutorial_PINNs.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/L_plate.stl` & `torchphysics-1.0.1/examples/tutorial/L_plate.stl`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/Tutorial_PINNs_Parameter_Dependency.ipynb` & `torchphysics-1.0.1/examples/tutorial/Tutorial_PINNs_Parameter_Dependency.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/domain_creation.ipynb` & `torchphysics-1.0.1/examples/tutorial/domain_creation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/polygons_external_objects.ipynb` & `torchphysics-1.0.1/examples/tutorial/polygons_external_objects.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/solve_pde.ipynb` & `torchphysics-1.0.1/examples/tutorial/solve_pde.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/examples/tutorial/solve_pde_drm.ipynb` & `torchphysics-1.0.1/examples/tutorial/solve_pde_drm.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/experiments/burgers_equation.ipynb` & `torchphysics-1.0.1/experiments/burgers_equation.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/experiments/geometry/d20_voll.stl` & `torchphysics-1.0.1/experiments/geometry/d20_voll.stl`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/experiments/geometry/heat_equation_D=10.gif` & `torchphysics-1.0.1/experiments/geometry/heat_equation_D=10.gif`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/experiments/geometry/heat_equation_bearing.ipynb` & `torchphysics-1.0.1/experiments/geometry/heat_equation_bearing.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/experiments/geometry/heat_equation_bearing_orig.ipynb` & `torchphysics-1.0.1/experiments/geometry/heat_equation_bearing_orig.ipynb`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/experiments/geometry/spalt_ex2_01.stl` & `torchphysics-1.0.1/experiments/geometry/spalt_ex2_01.stl`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/setup.cfg` & `torchphysics-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = torchphysics
 description = PyTorch implementation of Deep Learning methods to solve differential equations
 author = Nick Heilenkötter, Tom Freudenberg
-version = 1.0.0
+version = 1.0.1
 author_email = nick7@uni-bremen.de, tomfre@uni-bremen.de
 license = Apache-2.0
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/boschresearch/torchphysics
 project_urls = 
 	Documentation = https://torchphysics.readthedocs.io/en/latest/
```

### Comparing `torchphysics-1.0.0/setup.py` & `torchphysics-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/__init__.py` & `torchphysics-1.0.1/src/torchphysics/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/__init__.py` & `torchphysics-1.0.1/src/torchphysics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/activation_fn.py` & `torchphysics-1.0.1/src/torchphysics/models/activation_fn.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/deeponet/branchnets.py` & `torchphysics-1.0.1/src/torchphysics/models/deeponet/branchnets.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,37 +11,42 @@
 
 class BranchNet(Model):
     """A neural network that can be used inside a DeepONet-model.
     Parameters
     ----------
     function_space : Space
         The space of functions that can be put in this network.
-    output_space : Space
-        The space of the points that should be
-        returned by the parent DeepONet-model.
-    output_neurons : int
-        The number of output neurons. These neurons will only
-        be used internally. Will be multiplied my the dimension of the output space, 
-        so each dimension will have the same number of intermediate neurons. 
-        The final output of the DeepONet-model will be in the dimension of the 
-        output space. 
     discretization_sampler : torchphysics.sampler
         A sampler that will create the points at which the input functions should 
         evaluated, to create a discrete input for the network.
         The number of input neurons will be equal to the number of sampled points.
         Therefore, the sampler should always return the same number of points!
     """
-    def __init__(self, function_space, output_space, output_neurons, 
-                 discretization_sampler):
-        super().__init__(function_space, output_space)
-        self.output_neurons = output_neurons * output_space.dim
+    def __init__(self, function_space, discretization_sampler):
+        super().__init__(function_space, output_space=None)
+        self.output_neurons = 0
         self.discretization_sampler = discretization_sampler
         self.input_dim = len(self.discretization_sampler)
         self.current_out = torch.empty(0)
 
+    def finalize(self, output_space, output_neurons):
+        """Method to set the output space and output neurons of the network. 
+        Will be called once the BranchNet is connected to the TrunkNet, so
+        that both will have a fitting output shape.
+
+        output_space : Space
+            The space in which the final output of the DeepONet will belong to.
+        output_neurons : int
+            The number of output neurons. Will be multiplied my the dimension of the 
+            output space, so each dimension will have the same number of 
+            intermediate neurons.
+        """
+        self.output_neurons = output_neurons
+        self.output_space = output_space
+
     def _reshape_multidimensional_output(self, output):
         return output.reshape(-1, self.output_space.dim, 
                               int(self.output_neurons/self.output_space.dim))
         
     @abc.abstractmethod
     def forward(self, discrete_function_batch, device='cpu'):
         """Evaluated the network at a given function batch. Should not be called
@@ -71,54 +76,59 @@
 
     def fix_input(self, function, device='cpu'):
         """Fixes the branch net for a given function. The branch net will 
         be evaluated for the given function and the output saved in ``current_out``. 
         
         Parameters
         ----------
-        function : callable, torchphysics.domains.FunctionSet
+        function : callable, torchphysics.domains.FunctionSet, torch.Tensor, 
+                    torchphysics.spaces.Points
             The function(s) for which the network should be evaluaded.
         device : str, optional
             The device where the data lays. Default is 'cpu'.
         
         Notes
         -----
         To overwrite the data ``current_out`` (the fixed function) just call 
         ``.fix_input`` again with a new function.
         """
-        # TODO: add  functionality for list of functions and already 
-        # discrete function tensor
         if isinstance(function, FunctionSet):
             function.sample_params(device=device)
             discrete_fn = self._discretize_function_set(function, device=device)
         elif callable(function):
             function = UserFunction(function)
             discrete_points = self.discretization_sampler.sample_points(device=device)
             discrete_fn = function(discrete_points)
             discrete_fn = discrete_fn.unsqueeze(0) # add batch dimension
             discrete_fn = Points(discrete_fn, self.input_space.output_space)
+        elif isinstance(function, Points):
+            # check if we have to add batch dimension
+            if len(function._t.shape) < 3:
+                discrete_fn = Points(function._t.unsqueeze(0), self.input_space.output_space)
+            else:
+                discrete_fn = function
+        elif isinstance(function, torch.Tensor):
+            # check if we have to add batch dimension
+            if len(function.shape) < 3:
+                discrete_fn = function.unsqueeze(0)
+                discrete_fn = Points(discrete_fn, self.input_space.output_space)
+            else:
+                discrete_fn = Points(function, self.input_space.output_space)
         else:
-            raise NotImplementedError("function has to be callable or a FunctionSet")
+            raise NotImplementedError("Function has to be callable, a FunctionSet, a tensor, or a tp.Point")
         self(discrete_fn)
 
 
 class FCBranchNet(BranchNet):
     """A neural network that can be used inside a DeepONet-model.
     
     Parameters
     ----------
     function_space : Space
         The space of functions that can be put in this network.
-    output_space : Space
-        The space of the points that should be
-        returned by the parent DeepONet-model.
-    output_neurons : int
-        The number of output neurons. These neurons will only
-        be used internally. The final output of the DeepONet-model will be 
-        in the dimension of the output space. 
     discretization_sampler : torchphysics.sampler
         A sampler that will create the points at which the input functions should 
         evaluated, to create a discrete input for the network.
         The number of input neurons will be equal to the number of sampled points.
         Therefore, the sampler should always return the same number of points!
     hidden : list or tuple
         The number and size of the hidden layers of the neural network.
@@ -128,22 +138,26 @@
     activations : torch.nn or list, optional
         The activation functions of this network. 
         Deafult is nn.Tanh().
     xavier_gains : float or list, optional
         For the weight initialization a Xavier/Glorot algorithm will be used.
         Default is 5/3. 
     """
-    def __init__(self, function_space, output_space, output_neurons,
-                 discretization_sampler, hidden=(20,20,20), activations=nn.Tanh(),
-                 xavier_gains=5/3):
-        super().__init__(function_space, output_space, 
-                         output_neurons, discretization_sampler)
-        layers = _construct_FC_layers(hidden=hidden, input_dim=self.input_dim, 
-                                      output_dim=self.output_neurons, 
-                                      activations=activations, xavier_gains=xavier_gains)
+    def __init__(self, function_space, discretization_sampler, hidden=(20,20,20), 
+                 activations=nn.Tanh(), xavier_gains=5/3):
+        super().__init__(function_space, discretization_sampler)
+        self.hidden = hidden
+        self.activations = activations
+        self.xavier_gains = xavier_gains
+
+    def finalize(self, output_space, output_neurons):
+        super().finalize(output_space, output_neurons)
+        layers = _construct_FC_layers(hidden=self.hidden, input_dim=self.input_dim, 
+                        output_dim=self.output_neurons, activations=self.activations, 
+                        xavier_gains=self.xavier_gains)
 
         self.sequential = nn.Sequential(*layers)
 
     def forward(self, discrete_function_batch):
         discrete_function_batch = discrete_function_batch.as_tensor.reshape(-1, self.input_dim)
         self.current_out = self._reshape_multidimensional_output(self.sequential(discrete_function_batch))
        
@@ -152,21 +166,14 @@
     """A branch network that first applies a convolution to the input functions
     and afterwards linear FC-layers.
 
     Parameters
     ----------
     function_space : Space
         The space of functions that can be put in this network.
-    output_space : Space
-        The space of the points that should be
-        returned by the parent DeepONet-model.
-    output_neurons : int
-        The number of output neurons. These neurons will only
-        be used internally. The final output of the DeepONet-model will be 
-        in the dimension of the output space. 
     discretization_sampler : torchphysics.sampler
         A sampler that will create the points at which the input functions should 
         evaluated, to create a discrete input for the network.
         The number of input neurons will be equal to the number of sampled points.
         Therefore, the sampler should always return the same number of points!
     convolutional_network : torch.nn.module
         The user defined convolutional network, that should be applied to the 
@@ -187,23 +194,27 @@
     activations : torch.nn or list, optional
         The activation functions of this network. 
         Deafult is nn.Tanh().
     xavier_gains : float or list, optional
         For the weight initialization a Xavier/Glorot algorithm will be used.
         Default is 5/3. 
     """
-    def __init__(self, function_space, output_space, output_neurons,
-                 discretization_sampler, convolutional_network,
+    def __init__(self, function_space, discretization_sampler, convolutional_network,
                  hidden=(20,20,20), activations=nn.Tanh(), xavier_gains=5/3):
-        super().__init__(function_space, output_space, 
-                         output_neurons, discretization_sampler)
+        super().__init__(function_space, discretization_sampler)
         self.conv_net = convolutional_network
-        layers = _construct_FC_layers(hidden=hidden, input_dim=self.input_dim, 
-                                      output_dim=self.output_neurons, 
-                                      activations=activations, xavier_gains=xavier_gains)
+        self.hidden = hidden
+        self.activations = activations
+        self.xavier_gains = xavier_gains
+
+    def finalize(self, output_space, output_neurons):
+        super().finalize(output_space, output_neurons)
+        layers = _construct_FC_layers(hidden=self.hidden, input_dim=self.input_dim, 
+                        output_dim=self.output_neurons, activations=self.activations, 
+                        xavier_gains=self.xavier_gains)
 
         self.sequential = nn.Sequential(*layers)
 
     def _discretize_fn(self, function, device):
         # where is this function used?
         function = UserFunction(function)
         discrete_points = self.discretization_sampler.sample_points(device=device)
```

### Comparing `torchphysics-1.0.0/src/torchphysics/models/deeponet/layers.py` & `torchphysics-1.0.1/src/torchphysics/models/deeponet/layers.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/deeponet/trunknets.py` & `torchphysics-1.0.1/src/torchphysics/models/deeponet/trunknets.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,43 +9,52 @@
 class TrunkNet(Model):
     """A neural network that can be used inside a DeepONet-model.
 
     Parameters
     ----------
     input_space : Space
         The space of the points that can be put into this model.
-    output_space : Space
-        The number of output neurons. These neurons will only
-        be used internally. The final output of the DeepONet-model will be 
-        in the dimension of the output space. 
-    output_neurons : int
-        The number of output neurons. Will be multiplied my the dimension of the output space, 
-        so each dimension will have the same number of intermediate neurons.
     trunk_input_copied : bool, optional
         If every sample function of the branch input gets evaluated at the same trunk input, 
         the evaluation process can be speed up, since the trunk only has to evaluated once
         for the whole data batch of branch inputs. 
         If this is the case, set trunk_input_copied = True.
         If for example a dataset with different trunk inputs for each branch function
         is used, set trunk_input_copied = False. Else this may lead to unexpected 
         behavior.
     """
-    def __init__(self, input_space, output_space, output_neurons, 
-                 trunk_input_copied=True):
-        super().__init__(input_space, output_space)
-        self.output_neurons = output_neurons * output_space.dim
+    def __init__(self, input_space, trunk_input_copied=True):
+        super().__init__(input_space, output_space=None)
+        self.output_neurons = 0
         self.trunk_input_copied = trunk_input_copied
 
+    def finalize(self, output_space, output_neurons):
+        """Method to set the output space and output neurons of the network. 
+        Will be called once the BranchNet is connected to the TrunkNet, so
+        that both will have a fitting output shape.
+
+        output_space : Space
+            The space in which the final output of the DeepONet will belong to.
+        output_neurons : int
+            The number of output neurons. Will be multiplied my the dimension of the 
+            output space, so each dimension will have the same number of 
+            intermediate neurons.
+        """
+        self.output_neurons = output_neurons
+        self.output_space = output_space
+
     def _reshape_multidimensional_output(self, output):
         if len(output.shape) == 3:
             return output.reshape(output.shape[0], output.shape[1], self.output_space.dim, 
                                   int(self.output_neurons/self.output_space.dim))
         return output.reshape(-1, self.output_space.dim, 
                               int(self.output_neurons/self.output_space.dim))
 
+
+
 def construct_FC_trunk_layers(hidden, input_dim, output_dim, activations, xavier_gains):
     """Constructs the layer structure for a fully connected neural network.
     """
     if not isinstance(activations, (list, tuple)):
         activations = len(hidden) * [activations]
     if not isinstance(xavier_gains, (list, tuple)):
         xavier_gains = len(hidden) * [xavier_gains]
@@ -58,53 +67,51 @@
         layers.append(TrunkLinear(hidden[i], hidden[i+1]))
         torch.nn.init.xavier_normal_(layers[-1].weight, gain=xavier_gains[i+1])
         layers.append(activations[i+1])
     layers.append(TrunkLinear(hidden[-1], output_dim))
     torch.nn.init.xavier_normal_(layers[-1].weight, gain=1)
     return layers
 
+
 class FCTrunkNet(TrunkNet):
     """A fully connected neural network that can be used inside a DeepONet.
     Parameters
     ----------
     input_space : Space
         The space of the points the can be put into this model.
-    output_space : Space
-        The space of the points that should be
-        returned by the parent DeepONet-model.
-    output_neurons : int
-        The number of output neurons. These neurons will only
-        be used internally. The final output of the DeepONet-model will be 
-        in the dimension of the output space. 
     hidden : list or tuple
         The number and size of the hidden layers of the neural network.
         The lenght of the list/tuple will be equal to the number
         of hidden layers, while the i-th entry will determine the number
         of neurons of each layer.
     activations : torch.nn or list, optional
         The activation functions of this network. 
         Deafult is nn.Tanh().
     xavier_gains : float or list, optional
         For the weight initialization a Xavier/Glorot algorithm will be used.
         Default is 5/3. 
     """
-    def __init__(self, input_space, output_space, output_neurons, 
-                 hidden=(20,20,20), activations=nn.Tanh(), xavier_gains=5/3, 
+    def __init__(self, input_space, hidden=(20,20,20), activations=nn.Tanh(), xavier_gains=5/3, 
                  trunk_input_copied=True):
-        super().__init__(input_space, output_space, output_neurons, 
-                         trunk_input_copied=trunk_input_copied)
+        super().__init__(input_space, trunk_input_copied=trunk_input_copied)
+        self.hidden = hidden
+        self.activations = activations
+        self.xavier_gains = xavier_gains
+
 
+    def finalize(self, output_space, output_neurons):
+        super().finalize(output_space, output_neurons)
         # special layer architecture is used if trunk data is copied -> faster training
         if self.trunk_input_copied:
-            layers = construct_FC_trunk_layers(hidden=hidden, input_dim=self.input_space.dim, 
-                                            output_dim=self.output_neurons, 
-                                            activations=activations, xavier_gains=xavier_gains)
+            layers = construct_FC_trunk_layers(hidden=self.hidden, input_dim=self.input_space.dim, 
+                        output_dim=self.output_neurons, activations=self.activations, 
+                        xavier_gains=self.xavier_gains)
         else:
-            layers = _construct_FC_layers(hidden=hidden, input_dim=self.input_space.dim, 
-                                          output_dim=self.output_neurons, 
-                                          activations=activations, xavier_gains=xavier_gains)
+            layers = _construct_FC_layers(hidden=self.hidden, input_dim=self.input_space.dim, 
+                        output_dim=self.output_neurons, activations=self.activations, 
+                        xavier_gains=self.xavier_gains)
 
         self.sequential = nn.Sequential(*layers)
 
     def forward(self, points):
         points = self._fix_points_order(points)
         return self._reshape_multidimensional_output(self.sequential(points.as_tensor))
```

### Comparing `torchphysics-1.0.0/src/torchphysics/models/deepritz.py` & `torchphysics-1.0.1/src/torchphysics/models/deepritz.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/fcn.py` & `torchphysics-1.0.1/src/torchphysics/models/fcn.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/model.py` & `torchphysics-1.0.1/src/torchphysics/models/model.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/newmodel.py` & `torchphysics-1.0.1/src/torchphysics/models/newmodel.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/parameter.py` & `torchphysics-1.0.1/src/torchphysics/models/parameter.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/models/qres.py` & `torchphysics-1.0.1/src/torchphysics/models/qres.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/conditions/__init__.py` & `torchphysics-1.0.1/src/torchphysics/problem/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/conditions/condition.py` & `torchphysics-1.0.1/src/torchphysics/problem/conditions/condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,18 +146,14 @@
         else:
             try:
                 batch = next(self.iterator)
             except (StopIteration, AttributeError):
                 self.iterator = iter(self.dataloader)
                 batch = next(self.iterator)
             a = self._compute_dist(batch, device)
-            a[:, :1] /= 100.0
-            a[:, 1:2] /= 100.0
-            a[:, 2:3] /= 0.2
-            a[:, 3:] /= 500.0
             if self.norm == 'inf':
                 loss = torch.max(a)
             else:
                 loss = torch.mean(a**self.norm)
         if self.root != 1.0:
             loss = loss**(1/self.root)
         return loss
```

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/conditions/deeponet_condition.py` & `torchphysics-1.0.1/src/torchphysics/problem/conditions/deeponet_condition.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/__init__.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain0D/point.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain0D/point.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain1D/interval.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain1D/interval.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/circle.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/circle.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/parallelogram.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/parallelogram.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/shapely_polygon.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/shapely_polygon.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain2D/triangle.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain2D/triangle.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain3D/sphere.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain3D/sphere.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domain3D/trimesh_polyhedron.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domain3D/trimesh_polyhedron.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/cut.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/cut.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/intersection.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/intersection.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/product.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/product.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/rotate.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/rotate.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/sampler_helper.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/sampler_helper.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/translate.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/translate.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/domainoperations/union.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/domainoperations/union.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/domains/functionsets/functionset.py` & `torchphysics-1.0.1/src/torchphysics/problem/domains/functionsets/functionset.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/samplers/__init__.py` & `torchphysics-1.0.1/src/torchphysics/problem/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/samplers/data_samplers.py` & `torchphysics-1.0.1/src/torchphysics/problem/samplers/data_samplers.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/samplers/grid_samplers.py` & `torchphysics-1.0.1/src/torchphysics/problem/samplers/grid_samplers.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/samplers/plot_samplers.py` & `torchphysics-1.0.1/src/torchphysics/problem/samplers/plot_samplers.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/samplers/random_samplers.py` & `torchphysics-1.0.1/src/torchphysics/problem/samplers/random_samplers.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/samplers/sampler_base.py` & `torchphysics-1.0.1/src/torchphysics/problem/samplers/sampler_base.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/spaces/__init__.py` & `torchphysics-1.0.1/src/torchphysics/problem/spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/spaces/functionspace.py` & `torchphysics-1.0.1/src/torchphysics/problem/spaces/functionspace.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/spaces/points.py` & `torchphysics-1.0.1/src/torchphysics/problem/spaces/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     have the knowledge of what points belong to which space/variable.
     """
 
     def __init__(self, data, space, **kwargs):
         self._t = torch.as_tensor(data, **kwargs)
         self.space = space
         assert len(self._t.shape) >= 2
-        assert self._t.shape[-1] == self.space.dim
+        assert self._t.shape[-1] == self.space.dim, \
+            "Data dimension does not fit dimension of the space " + str(list(self.space.keys()))
 
     @classmethod
     def empty(cls, **kwargs):
         """Creates an empty Points object.
 
         Returns
         -------
```

### Comparing `torchphysics-1.0.0/src/torchphysics/problem/spaces/space.py` & `torchphysics-1.0.1/src/torchphysics/problem/spaces/space.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/solver.py` & `torchphysics-1.0.1/src/torchphysics/solver.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/__init__.py` & `torchphysics-1.0.1/src/torchphysics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/callbacks.py` & `torchphysics-1.0.1/src/torchphysics/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/data/dataloader.py` & `torchphysics-1.0.1/src/torchphysics/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/data/deeponet_dataloader.py` & `torchphysics-1.0.1/src/torchphysics/utils/data/deeponet_dataloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,17 @@
                [number_of_functions, number_of_trunk_points, input_dim_of_trunk_net]
                If this is the case, remember to set 'trunk_input_copied = false' inside
                the trunk net, to get the right trainings process.
     output_data : torch.tensor
         A tensor containing the expected output of the network. Shape of the 
         data should be: 
         [number_of_functions, number_of_trunk_points, output_dim].
-    branch_output_space : torchphysics.spaces.Space
+    branch_space : torchphysics.spaces.Space
         The output space of the functions, that are used as the branch input.
-    input_space : torchphysics.spaces.Space
+    trunk_space : torchphysics.spaces.Space
         The input space of the trunk network.
     output_space : torchphysics.spaces.Space
         The output space in which the solution is. 
     branch_batch_size, trunk_batch_size : int
         The size of the loaded batches for trunk and branch.
     shuffle_branch : bool
         Whether to shuffle the order of the branch functions at initialization.
@@ -50,14 +50,21 @@
     pin_memory : bool
         Whether to use pinned memory during data loading, see also: the PyTorch documentation
     """
     def __init__(self, branch_data, trunk_data, output_data, branch_space,
                  trunk_space, output_space, branch_batch_size, trunk_batch_size,
                  shuffle_branch=False, shuffle_trunk=True, num_workers=0,
                  pin_memory=False):
+        assert len(branch_data.shape) == 3, "Branch data has the wrong shape"
+        assert branch_data.shape[-1] == branch_space.dim , \
+            "Branch data dimension is not correct, is " + str(branch_data.shape[-1]) + " but expected " + str(branch_space.dim)
+        assert trunk_data.shape[-1] == trunk_space.dim, \
+            "Trunk data dimension is not correct, is " + str(trunk_data.shape[-1]) + " but expected " + str(trunk_space.dim)
+        assert output_data.shape[-1] == output_space.dim, \
+            "Solution data dimension is not correct, is " + str(output_data.shape[-1]) + " but expected " + str(output_space.dim)
         if len(trunk_data.shape) == 3:
             super().__init__(DeepONetDataset_Unique(branch_data,
                                                     trunk_data,
                                                     output_data,
                                                     branch_space,
                                                     trunk_space,
                                                     output_space,
```

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/differentialoperators.py` & `torchphysics-1.0.1/src/torchphysics/utils/differentialoperators.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -300,19 +300,19 @@
     ----------
     torch.tensor
         A Tensor, where every row contains the values of the computed partial 
         derivative of the model w.r.t the row of the input variable.
     '''
     du = model_out
     for inp in derivative_variables:
+        if du.grad_fn is None:
+            return torch.zeros_like(inp)
         du = torch.autograd.grad(du.sum(),
                                  inp,
                                  create_graph=True)[0]
-        if du.grad_fn is None:
-            return torch.zeros_like(inp)
     return du
 
 
 def convective(deriv_out, convective_field, *derivative_variable):
     '''Computes the convective term :math:`(v \\cdot \\nabla)u` that appears e.g. in
     material derivatives. Note: This is not the whole material derivative.
```

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/evaluation.py` & `torchphysics-1.0.1/src/torchphysics/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/plotting/animation.py` & `torchphysics-1.0.1/src/torchphysics/utils/plotting/animation.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/plotting/plot_functions.py` & `torchphysics-1.0.1/src/torchphysics/utils/plotting/plot_functions.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/plotting/scatter_points.py` & `torchphysics-1.0.1/src/torchphysics/utils/plotting/scatter_points.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/src/torchphysics/utils/user_fun.py` & `torchphysics-1.0.1/src/torchphysics/utils/user_fun.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             The output values of the function.
         """
         if isinstance(args, Points):
             args = args.coordinates
         # check that every necessary arg is given
         for key in self.necessary_args:
             assert key in args, \
-                f"The argument '{key}' is necessary in {self.__name__} but not given."
+                f"The argument '{key}' is necessary in {self.__name__()} but not given."
         # if necessary, pass defaults
         inp = {key: args[key] for key in self.args if key in args}
         inp.update({key: self.defaults[key] for key in self.args if key not in args})
         if not vectorize:
             return self.evaluate_function(**inp)
         else:
             return self.apply_to_batch(inp)
```

### Comparing `torchphysics-1.0.0/src/torchphysics.egg-info/PKG-INFO` & `torchphysics-1.0.1/src/torchphysics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchphysics
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyTorch implementation of Deep Learning methods to solve differential equations
 Home-page: https://github.com/boschresearch/torchphysics
 Author: Nick Heilenkötter, Tom Freudenberg
 Author-email: nick7@uni-bremen.de, tomfre@uni-bremen.de
 License: Apache-2.0
 Project-URL: Documentation, https://torchphysics.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/boschresearch/torchphysics
@@ -95,28 +95,48 @@
 .. _`Tutorial: Understanding the structure of TorchPhysics`: https://torchphysics.readthedocs.io/en/latest/tutorial/tutorial_start.html
 .. _`Examples: Different applications with detailed explanations`: https://github.com/boschresearch/torchphysics/tree/main/examples
 .. _Documentation: https://torchphysics.readthedocs.io/en/latest/api/modules.html
 
 
 Installation
 ============
-TorchPhysics can be installed by using:
+TorchPhysics reqiueres the follwing dependencies to be installed: 
+
+- PyTorch_ >= 1.7.1, < 2.0.0
+- `PyTorch Lightning`_ >= 1.3.4, < 2.0.0
+- Numpy_ >= 1.20.2
+- Matplotlib_ >= 3.0.0
+- Scipy_ >= 1.6.3
+
+Installing TorchPhysics with ``pip``, automatically downloads everything that is needed:
 
 .. code-block:: python
 
-  pip install git+https://github.com/boschresearch/torchphysics
+  pip install torchphysics
+
+Additionally, to use the ``Shapely`` and ``Trimesh`` functionalities, install the library 
+with the option ``all``:
+
+.. code-block:: python
+
+  pip install torchphysics[all]
+
 
-If you want to change or add something to the code. You should first copy the repository and install
-it locally:
+If you want to add functionalities or modify the code. We recommend copying the 
+repository and installing it locally:
 
 .. code-block:: python
 
   git clone https://github.com/boschresearch/torchphysics 
-  pip install .
+  cd path_to_torchphysics_folder
+  pip install .[all]
 
+.. _Numpy: https://numpy.org/
+.. _Matplotlib: https://matplotlib.org/
+.. _Scipy: https://scipy.org/
 
 About
 =====
 TorchPhysics was originally developed by Nick Heilenkötter and Tom Freudenberg, 
 as part of a `seminar project`_ at the `University of Bremen`_, in cooperation with the `Robert Bosch GmbH`_. 
 Special thanks belong to Felix Hildebrand, Uwe Iben, Daniel Christopher Kreuter and Johannes Mueller,
 at the Robert Bosch GmbH, for support and supervision while creating this library.
```

### Comparing `torchphysics-1.0.0/src/torchphysics.egg-info/SOURCES.txt` & `torchphysics-1.0.1/src/torchphysics.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 docs/conf.py
 docs/examples.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
+docs/tutorial/applied_tutorial_start.rst
 docs/tutorial/condition_tutorial.rst
 docs/tutorial/differentialoperators.rst
 docs/tutorial/external_domains.rst
+docs/tutorial/main_page.rst
 docs/tutorial/model_creation.rst
 docs/tutorial/plotting.rst
 docs/tutorial/sampler_tutorial.rst
 docs/tutorial/solve_pde.rst
 docs/tutorial/solver_info.rst
 docs/tutorial/tutorial_domain_basics.rst
 docs/tutorial/tutorial_spaces_and_points.rst
@@ -48,14 +50,15 @@
 docs/tutorial/pictures/polygon.png
 docs/tutorial/pictures/rect_circle_domain.png
 docs/tutorial/pictures/sampler_combis.PNG
 docs/tutorial/pictures/simplex.png
 docs/tutorial/pictures/solution.png
 docs/tutorial/pictures/torchphysics_structure.png
 examples/fdm_heat_equation.py
+examples/deeponet/inverse_ode.ipynb
 examples/deeponet/ode.ipynb
 examples/deeponet/oscillator.ipynb
 examples/deepritz/corner_pde.ipynb
 examples/deepritz/poisson-equation.ipynb
 examples/pinn/exp-function-with-param.ipynb
 examples/pinn/hard-constrains.ipynb
 examples/pinn/heat-equation.ipynb
@@ -74,28 +77,46 @@
 examples/tutorial/Introduction_Tutorial_PINNs.ipynb
 examples/tutorial/L_plate.stl
 examples/tutorial/Tutorial_PINNs_Parameter_Dependency.ipynb
 examples/tutorial/domain_creation.ipynb
 examples/tutorial/polygons_external_objects.ipynb
 examples/tutorial/solve_pde.ipynb
 examples/tutorial/solve_pde_drm.ipynb
+examples/workshop/Exercise1_1.ipynb
+examples/workshop/Exercise1_2.ipynb
+examples/workshop/Exercise1_3.ipynb
+examples/workshop/Exercise2_1.ipynb
+examples/workshop/Exercise2_2.ipynb
+examples/workshop/Exercise3_1.ipynb
+examples/workshop/Lecture_Example.py
+examples/workshop/Sol1_2.ipynb
+examples/workshop/Sol1_3.ipynb
+examples/workshop/Sol2_1.ipynb
+examples/workshop/Sol2_2.ipynb
+examples/workshop/FEMData/Data2_2/space_coords.pt
+examples/workshop/FEMData/Data2_2/temperature.pt
+examples/workshop/FEMData/Data2_2/time_points.pt
+examples/workshop/FEMData/Data2_3/space_coords.pt
+examples/workshop/FEMData/Data2_3/time_points.pt
+examples/workshop/FEMData/Data2_3/wave_data.pt
 experiments/burgers_equation.ipynb
 experiments/geometry/d20_voll.stl
 experiments/geometry/heat_equation_D=10.gif
 experiments/geometry/heat_equation_bearing.ipynb
 experiments/geometry/heat_equation_bearing_orig.ipynb
 experiments/geometry/spalt_ex2_01.stl
 src/torchphysics/__init__.py
 src/torchphysics/solver.py
 src/torchphysics.egg-info/PKG-INFO
 src/torchphysics.egg-info/SOURCES.txt
 src/torchphysics.egg-info/dependency_links.txt
 src/torchphysics.egg-info/not-zip-safe
 src/torchphysics.egg-info/requires.txt
 src/torchphysics.egg-info/top_level.txt
+src/torchphysics/models/FNO.py
 src/torchphysics/models/__init__.py
 src/torchphysics/models/activation_fn.py
 src/torchphysics/models/deepritz.py
 src/torchphysics/models/fcn.py
 src/torchphysics/models/model.py
 src/torchphysics/models/newmodel.py
 src/torchphysics/models/parameter.py
```

### Comparing `torchphysics-1.0.0/tests/test_conditions.py` & `torchphysics-1.0.1/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/test_data_utils.py` & `torchphysics-1.0.1/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/test_differentialoperators.py` & `torchphysics-1.0.1/tests/test_differentialoperators.py`

 * *Files 4% similar despite different names*

```diff
@@ -655,14 +655,26 @@
     output = part_function(x, y, t)
     p = partial(output, x, x, x)
     assert p.shape == (2, 1)
     d = p.detach().numpy()
     assert np.allclose(d[0], [[0], [0]])
 
 
+def test_partial_repeated_gives_0_2():
+    x = torch.tensor([[1.0], [2.0]], requires_grad=True)
+    y = torch.tensor([[1.0], [3.0]], requires_grad=True)
+    t = torch.tensor([[2.0], [0.0]], requires_grad=True)
+    output = part_function(x, y, t)
+    p = partial(output, x, x, x, x, y)
+    assert p.shape == (2, 1)
+    d = p.detach().numpy()
+    assert np.allclose(d[0], [[0], [0]])
+
+
+
 # Test convective
 def convec_function(x):
     out = torch.zeros((len(x), 3))
     out[:, :1] += x[:, :1]**2 
     out[:, 1:2] += x[:, :1]
     out[:, 2:] += x[:, 1:2] * x[:, 2:]
     return out
```

### Comparing `torchphysics-1.0.0/tests/test_evaluation.py` & `torchphysics-1.0.1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/test_points.py` & `torchphysics-1.0.1/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/test_samplers.py` & `torchphysics-1.0.1/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/test_spaces.py` & `torchphysics-1.0.1/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/test_user_function.py` & `torchphysics-1.0.1/tests/test_user_function.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain0D.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain0D.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain1D.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain1D.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain2D.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain2D.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain2D_shapely.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain2D_shapely.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain3D.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain3D.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain3D_trimesh.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain3D_trimesh.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain_cut.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain_cut.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain_intersection.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain_intersection.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain_product.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain_product.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain_tranforms.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain_tranforms.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_domain/test_domain_union.py` & `torchphysics-1.0.1/tests/tests_domain/test_domain_union.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_functionsets/test_FunctionSetMain.py` & `torchphysics-1.0.1/tests/tests_functionsets/test_FunctionSetMain.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_models/test_activation_fn.py` & `torchphysics-1.0.1/tests/tests_models/test_activation_fn.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_models/test_deep_o_net.py` & `torchphysics-1.0.1/tests/tests_models/test_deep_o_net.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 from torchphysics.problem.samplers.grid_samplers import GridSampler
 
 """
 Tests for trunk net:
 """
 
 def test_create_trunk_net():
-    net = TrunkNet(input_space=R2('x'), output_space=R1('u'), output_neurons=20)
+    net = TrunkNet(input_space=R2('x'))
     assert net.input_space == R2('x')
-    assert net.output_space == R1('u')
-    assert net.output_neurons == 20
+    assert net.output_space == None
+    assert net.output_neurons == 0
 
 
 def test_create_fc_trunk_net():
-    net = FCTrunkNet(input_space=R2('x'), output_space=R1('u'), output_neurons=20)
+    net = FCTrunkNet(input_space=R2('x'))
     assert net.input_space == R2('x')
-    assert net.output_space == R1('u')
-    assert net.output_neurons == 20
+    assert net.output_space == None
+    assert net.output_neurons == 0
 
 
 def test_forward_fc_trunk_net():
-    net =  FCTrunkNet(input_space=R2('x'), output_space=R1('u'), output_neurons=20)
-    test_data = Points(torch.tensor([[[2, 3.0], [0, 1]], [[2, 3.0], [0, 1]]]), R2('x'))
-    out = net(test_data)
-    assert out.size() == torch.Size([2, 2, 1, 20])
+    net = FCTrunkNet(input_space=R2('x'))
+    assert net.input_space == R2('x')
+    assert net.output_space == None
+    assert net.output_neurons == 0
 
 """
 Tests for branch net:
 """
 def helper_fn_set():
     def f(k, t):
         return k*t
@@ -46,157 +46,154 @@
     fn_set =  CustomFunctionSet(fn_space, GridSampler(params, 20), f)
     return fn_space, fn_set
 
 
 def test_create_branch_net():
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 10).make_static()
-    net = BranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                    discretization_sampler=sampler)
+    net = BranchNet(fn_space, discretization_sampler=sampler)
     assert net.discretization_sampler == sampler
-    assert net.output_space == R1('u')
-    assert net.output_neurons == 20
     assert net.input_dim == 10
     assert net.input_space == fn_space
 
 
-def test_discretization_of_function_set():
-    fn_space, fn_set = helper_fn_set()
-    fn_set.sample_params()
-    sampler = GridSampler(fn_space.input_domain, 10).make_static()
-    net = BranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                    discretization_sampler=sampler)
-    fn_batch = net._discretize_function_set(fn_set)
-    assert fn_batch.shape == (20, 10)
-
-
 def test_create_fc_branch_net():
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    net = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=22, 
-                      discretization_sampler=sampler)
+    net = FCBranchNet(fn_space, discretization_sampler=sampler)
     assert net.discretization_sampler == sampler
-    assert net.output_space == R1('u')
-    assert net.output_neurons == 22
     assert net.input_dim == 15
     assert net.input_space == fn_space
 
 
-def test_fix_branch_net_with_function():
-    def f(t):
-        return 20*t
-    fn_space, _ = helper_fn_set()
-    sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    net = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=22, 
-                      discretization_sampler=sampler)
-    net.fix_input(f)
-    assert net.current_out.shape == (1, 1, 22)
+# def test_fix_branch_net_with_function():
+#     def f(t):
+#         return 20*t
+#     fn_space, _ = helper_fn_set()
+#     sampler = GridSampler(fn_space.input_domain, 15).make_static()
+#     net = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=22, 
+#                       discretization_sampler=sampler)
+#     net.fix_input(f)
+#     assert net.current_out.shape == (1, 1, 22)
 
 
 def test_fix_branch_net_with_function_set():
     fn_space, fn_set = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    net = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=22, 
-                      discretization_sampler=sampler)
+    net = FCBranchNet(fn_space, discretization_sampler=sampler)
+    net.finalize(R1('u'), 20)
     net.fix_input(fn_set)
-    assert net.current_out.shape == (20, 1, 22)
 
 
 def test_fix_branch_wrong_input():
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    net = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=22, 
-                      discretization_sampler=sampler)
+    net = FCBranchNet(fn_space, discretization_sampler=sampler)
     with pytest.raises(NotImplementedError):
         net.fix_input(34)
 
 """
 Tests for DeepONet:
 """
 def test_create_deeponet():
-    trunk = TrunkNet(input_space=R1('t'), output_space=R1('u'), output_neurons=20)
+    trunk = TrunkNet(input_space=R1('t'))
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    branch = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                         discretization_sampler=sampler)
-    net = DeepONet(trunk, branch)
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler)
+    net = DeepONet(trunk, branch, output_space=R1('u'), output_neurons=20)
     assert net.trunk == trunk
     assert net.branch == branch
     assert net.input_space == R1('t')
     assert net.output_space == R1('u')
+    assert net.trunk.output_space == R1('u')
+    assert net.branch.output_space == R1('u')
+    assert net.trunk.output_neurons == 20
+    assert net.branch.output_neurons == 20
 
 
 def test_create_deeponet_with_seq_trunk():
-    trunk = TrunkNet(input_space=R1('t'), output_space=R1('u'), output_neurons=20)
+    trunk = TrunkNet(input_space=R1('t'))
     seq_trunk = Sequential(NormalizationLayer(Interval(R1('t'), 0, 1)), trunk)
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    branch = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                         discretization_sampler=sampler)
-    net = DeepONet(seq_trunk, branch)
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler)
+    net = DeepONet(seq_trunk, branch, output_space=R1('u'), output_neurons=20)
     assert net.trunk == seq_trunk
     assert net.branch == branch
     assert net.input_space == R1('t')
     assert net.output_space == R1('u')
     
 
 def test_deeponet_fix_branch():
     def f(t):
         return 20*t
-    trunk = TrunkNet(input_space=R1('t'), output_space=R1('u'), output_neurons=20)
+    trunk = TrunkNet(input_space=R1('t'))
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    branch = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                         discretization_sampler=sampler)
-    net = DeepONet(trunk, branch)
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler)
+    net = DeepONet(trunk, branch, output_space=R1('u'), output_neurons=20)
     net.fix_branch_input(f)
     assert branch.current_out.shape == (1, 1, 20)
 
 
 def test_deeponet_forward():
     def f(t):
         return 20*t
-    trunk = FCTrunkNet(input_space=R1('t'), output_space=R1('u'), output_neurons=20)
+    trunk = FCTrunkNet(input_space=R1('t'), xavier_gains=(1, 1, 1), 
+                        trunk_input_copied=False)
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    branch = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                         discretization_sampler=sampler)
-    net = DeepONet(trunk, branch)
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler, xavier_gains=(1, 1, 1))
+    net = DeepONet(trunk, branch, output_space=R1('u'), output_neurons=20)
     test_data = Points(torch.tensor([[[2], [0], [3.4], [2.9]]]), R1('t'))
     out = net(test_data, f)
     assert 'u' in out.space
     assert out.as_tensor.shape == (1, 4, 1)
 
 
+def test_deeponet_forward_multi_dim_output():
+    def f(t):
+        return 20*t
+    trunk = FCTrunkNet(input_space=R1('t'), activations=[torch.nn.ReLU()], hidden=(10,))
+    fn_space, _ = helper_fn_set()
+    sampler = GridSampler(fn_space.input_domain, 15).make_static()
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler, 
+                         activations=[torch.nn.ReLU()], hidden=(10,))
+    net = DeepONet(trunk, branch, output_space=R2('u'), output_neurons=20)
+    test_data = Points(torch.tensor([[[2], [0], [3.4], [2.9]]]), R1('t'))
+    out = net(test_data, f)
+    assert 'u' in out.space
+    assert out.as_tensor.shape == (1, 4, 2)
+
+
 def test_deeponet_forward_with_fixed_branch():
     def f(t):
         return torch.sin(t)
-    trunk = FCTrunkNet(input_space=R1('t'), output_space=R1('u'), output_neurons=20)
+    trunk = FCTrunkNet(input_space=R1('t'))
     fn_space, _ = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    branch = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                         discretization_sampler=sampler)
-    net = DeepONet(trunk, branch)
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler)
+    net = DeepONet(trunk, branch, output_space=R1('u'), output_neurons=12)
     test_data = Points(torch.tensor([[[2], [0], [3.4], [2.9], [5.2]]]), R1('t'))
     net.fix_branch_input(f)
     out = net(test_data)
     assert 'u' in out.space
     assert out.as_tensor.shape == (1, 5, 1)
 
 
 def test_deeponet_forward_branch_intern():
-    trunk = FCTrunkNet(input_space=R1('t'), output_space=R1('u'), output_neurons=20)
+    trunk = FCTrunkNet(input_space=R1('t'))
     fn_space, fn_set = helper_fn_set()
     sampler = GridSampler(fn_space.input_domain, 15).make_static()
-    branch = FCBranchNet(fn_space, output_space=R1('u'), output_neurons=20, 
-                         discretization_sampler=sampler)
-    net = DeepONet(trunk, branch)
+    branch = FCBranchNet(fn_space, discretization_sampler=sampler)
+    net = DeepONet(trunk, branch, output_space=R1('u'), output_neurons=20)
     net._forward_branch(fn_set, iteration_num=0)
     net._forward_branch(fn_set, iteration_num=0)
 
+
 def test_trunk_linear():
     linear_a = TrunkLinear(30, 20, bias=True)
     linear_b = torch.nn.Linear(30, 20, bias=True)
     linear_b.bias = torch.nn.Parameter(linear_a.bias[:])
     linear_b.weight = torch.nn.Parameter(linear_a.weight[:])
 
     x = torch.randn(2,4,30).expand(5,-1,-1,-1)
```

### Comparing `torchphysics-1.0.0/tests/tests_models/test_deepritz.py` & `torchphysics-1.0.1/tests/tests_models/test_deepritz.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_models/test_fcn.py` & `torchphysics-1.0.1/tests/tests_models/test_fcn.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_models/test_model_base.py` & `torchphysics-1.0.1/tests/tests_models/test_model_base.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_models/test_parameters.py` & `torchphysics-1.0.1/tests/tests_models/test_parameters.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_models/test_qres.py` & `torchphysics-1.0.1/tests/tests_models/test_qres.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_plots/test_animation.py` & `torchphysics-1.0.1/tests/tests_plots/test_animation.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_plots/test_plot.py` & `torchphysics-1.0.1/tests/tests_plots/test_plot.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_plots/test_scatter.py` & `torchphysics-1.0.1/tests/tests_plots/test_scatter.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tests/tests_solver/test_solver.py` & `torchphysics-1.0.1/tests/tests_solver/test_solver.py`

 * *Files identical despite different names*

### Comparing `torchphysics-1.0.0/tox.ini` & `torchphysics-1.0.1/tox.ini`

 * *Files identical despite different names*

