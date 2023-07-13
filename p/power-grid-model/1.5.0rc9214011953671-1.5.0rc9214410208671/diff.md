# Comparing `tmp/power-grid-model-1.5.0rc9214011953671.tar.gz` & `tmp/power-grid-model-1.5.0rc9214410208671.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9214011953671.tar", last modified: Wed Jul 12 13:00:50 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9214410208671.tar", last modified: Wed Jul 12 15:46:40 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9214011953671.tar` & `power-grid-model-1.5.0rc9214410208671.tar`

### file list

```diff
@@ -1,642 +1,642 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 13:00:02.000000 power-grid-model-1.5.0rc9214011953671/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.460518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.480518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.480518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.480518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    68835 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.480518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.464518 power-grid-model-1.5.0rc9214011953671/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.488518 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34661 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29948 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.484518 power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-12 13:00:50.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38380 2023-07-12 13:00:50.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:00:50.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-12 13:00:50.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 13:00:50.000000 power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.488518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.488518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.488518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.492518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.492518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.492518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.492518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.496518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.496518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.496518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.496518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.496518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.500518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.500518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.500518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.500518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.500518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.504518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.504518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.504518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.504518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.504518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.508518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.508518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.508518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.508518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.508518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.512518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.512518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.512518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.512518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.512518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.472518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.516518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.516518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.516518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.516518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.520518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.520518 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.520518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.520518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.524518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.524518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.524518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.524518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.524518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.528518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.528518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.528518 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.476518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.528518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.532518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.532518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.532518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.532518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.532518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.532518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:00:50.536518 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-12 12:59:56.000000 power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.103591 power-grid-model-1.5.0rc9214410208671/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-12 15:46:40.103591 power-grid-model-1.5.0rc9214410208671/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 15:46:00.000000 power-grid-model-1.5.0rc9214410208671/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.035592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.047592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.047592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.047592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68835 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.047592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.047592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.047592 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.051591 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.051591 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:46:40.103591 power-grid-model-1.5.0rc9214410208671/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.051591 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.051591 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.055591 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.051591 power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-12 15:46:40.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38380 2023-07-12 15:46:40.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:46:40.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-12 15:46:40.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 15:46:40.000000 power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.055591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.055591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.055591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.059592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.059592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.059592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.059592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.063592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.063592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.063592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.063592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.063592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.067592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.067592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.067592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.067592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.067592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.071591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.071591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.071591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.071591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.071591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.075591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.075591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.075591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.075591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.075591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.075591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.079591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.079591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.079591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.079591 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.039592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.083592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.083592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.083592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.083592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.087592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.087592 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.087592 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.087592 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.087592 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.091591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.091591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.091591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.091591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.095591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.095591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.095591 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.043592 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.095591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.095591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.099591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.099591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.099591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.099591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.099591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.099591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.103591 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.103591 power-grid-model-1.5.0rc9214410208671/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:46:40.103591 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-12 15:45:57.000000 power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9214011953671/LICENSE` & `power-grid-model-1.5.0rc9214410208671/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/PKG-INFO` & `power-grid-model-1.5.0rc9214410208671/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9214011953671
+Version: 1.5.0rc9214410208671
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9214011953671/README.md` & `power-grid-model-1.5.0rc9214410208671/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.0rc9214410208671/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/pyproject.toml` & `power-grid-model-1.5.0rc9214410208671/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/setup.py` & `power-grid-model-1.5.0rc9214410208671/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/core/power_grid_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,46 +38,47 @@
     _batch_error: Optional[PowerGridBatchError]
 
     @property
     def batch_error(self) -> Optional[PowerGridBatchError]:
         """
         Get the batch error object, if present
 
-        Returns: Batch error object, or None
-
+        Returns:
+            Batch error object, or None
         """
         return self._batch_error
 
     @property
     def _model(self):
         if not self._model_ptr:
             raise TypeError("You have an empty instance of PowerGridModel!")
         return self._model_ptr
 
     @property
     def all_component_count(self) -> Dict[str, int]:
         """
         Get count of number of elements per component type.
         If the count for a component type is zero, it will not be in the returned dictionary.
+
         Returns:
-            a dictionary with
-                key: component type name
-                value: integer count of elements of this type
+            A dictionary with
+
+                - key: Component type name
+                - value: Integer count of elements of this type
         """
         if self._all_component_count is None:
             raise TypeError("You have an empty instance of PowerGridModel!")
         return self._all_component_count
 
     def copy(self) -> "PowerGridModel":
         """
-
         Copy the current model
 
         Returns:
-            a copy of PowerGridModel
+            A copy of PowerGridModel
         """
         new_model = PowerGridModel.__new__(PowerGridModel)
         new_model._model_ptr = pgc.copy_model(self._model)  # pylint: disable=W0212
         assert_no_error()
         new_model._all_component_count = self._all_component_count  # pylint: disable=W0212
         return new_model
 
@@ -91,18 +92,20 @@
         return instance
 
     def __init__(self, input_data: Dict[str, np.ndarray], system_frequency: float = 50.0):
         """
         Initialize the model from an input data set.
 
         Args:
-            input_data: input data dictionary
-                key: component type name
-                value: 1D numpy structured array for this component input
-            system_frequency: frequency of the power system, default 50 Hz
+            input_data: Input data dictionary
+
+                - key: Component type name
+                - value: 1D numpy structured array for this component input
+
+            system_frequency: Frequency of the power system, default 50 Hz
         """
         # destroy old instance
         pgc.destroy_model(self._model_ptr)
         self._all_component_count = None
         # create new
         prepared_input = prepare_input_view(input_data)
         self._model_ptr = pgc.create_model(
@@ -116,18 +119,21 @@
         self._all_component_count = {
             k: v.n_elements_per_scenario for k, v in prepared_input.dataset.items() if v.n_elements_per_scenario > 0
         }
 
     def update(self, *, update_data: Dict[str, np.ndarray]):
         """
         Update the model with changes.
+
         Args:
-            update_data: update data dictionary
-                key: component type name
-                value: 1D numpy structured array for this component update
+            update_data: Update data dictionary
+
+                - key: Component type name
+                - value: 1D numpy structured array for this component update
+
         Returns:
             None
         """
         prepared_update = prepare_update_view(update_data)
         pgc.update_model(
             self._model,
             prepared_update.n_components,
@@ -138,20 +144,19 @@
         assert_no_error()
 
     def get_indexer(self, component_type: str, ids: np.ndarray):
         """
         Get array of indexers given array of ids for component type
 
         Args:
-            component_type: type of component
-            ids: array of ids
+            component_type: Type of component
+            ids: Array of ids
 
         Returns:
-            array of inderxers, same shape as input array ids
-
+            Array of indexers, same shape as input array ids
         """
         ids_c = np.ascontiguousarray(ids, dtype=IdNp).ctypes.data_as(IDPtr)
         indexer = np.empty_like(ids, dtype=IdxNp, order="C")
         indexer_c = indexer.ctypes.data_as(IdxPtr)
         size = ids.size
         # call c function
         pgc.get_indexer(self._model, component_type, size, ids_c, indexer_c)
@@ -218,21 +223,22 @@
         options: Options,
         continue_on_batch_error: bool,
     ):
         """
         Core calculation routine
 
         Args:
-            options:
+            calculation_type:
+            symmetric:
             update_data:
             output_component_types:
+            options:
             continue_on_batch_error:
 
         Returns:
-
         """
         self._batch_error = None
         batch_calculation = is_batch_calculation(update_data=update_data)
 
         prepared_update = prepare_update_view(update_data)
         batch_size = prepared_update.batch_size
 
@@ -279,62 +285,71 @@
         update_data: Optional[Dict[str, Union[np.ndarray, Dict[str, np.ndarray]]]] = None,
         threading: int = -1,
         output_component_types: Optional[Union[Set[str], List[str]]] = None,
         continue_on_batch_error: bool = False,
     ) -> Dict[str, np.ndarray]:
         """
         Calculate power flow once with the current model attributes.
-        Or calculate in batch with the given update dataset in batch
+        Or calculate in batch with the given update dataset in batch.
 
         Args:
-            symmetric:
-                True: three-phase symmetric calculation, even for asymmetric loads/generations
-                False: three-phase asymmetric calculation
-            error_tolerance:
-                error tolerance for voltage in p.u., only applicable when the calculation method is iterative
-            max_iterations:
-                maximum number of iterations, only applicable when the calculation method is iterative
-            calculation_method: an enumeration or string
-                newton_raphson: use Newton-Raphson iterative method (default)
-                linear: use linear method
-            update_data:
-                None: calculate power flow once with the current model attributes
-                A dictionary for batch calculation with batch update
-                    key: component type name to be updated in batch
-                    value:
-                        a 2D numpy structured array for homogeneous update batch
-                            Dimension 0: each batch
-                            Dimension 1: each updated element per batch for this component type
-                        **or**
-                        a dictionary containing two keys, for inhomogeneous update batch
-                            indptr: a 1D integer numpy array with length n_batch + 1
-                                given batch number k, the update array for this batch is
-                                data[indptr[k]:indptr[k + 1]]
-                                This is the concept of compressed sparse structure
-                                https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html
-                            data: 1D numpy structured array in flat
-            threading:
-                only applicable for batch calculation
-                < 0 sequential
-                = 0 parallel, use number of hardware threads
-                > 0 specify number of parallel threads
-            output_component_types: list or set of component types you want to be present in the output dict.
-                By default all component types will be in the output
-            continue_on_batch_error: if the program continues (instead of throwing error) if some scenarios fail
+            symmetric (bool, optional): Whether to perform a three-phase symmetric calculation.
+
+                - True: Three-phase symmetric calculation, even for asymmetric loads/generations (Default).
+                - False: Three-phase asymmetric calculation.
+            error_tolerance (float, optional): Error tolerance for voltage in p.u., applicable only when the
+                calculation method is iterative.
+            max_iterations (int, optional): Maximum number of iterations, applicable only when the calculation method
+                is iterative.
+            calculation_method (an enumeration or string): The calculation method to use.
+
+                - newton_raphson: Use Newton-Raphson iterative method (default).
+                - linear: Use linear method.
+            update_data (dict, optional):
+                None: Calculate power flow once with the current model attributes.
+                Or a dictionary for batch calculation with batch update.
+
+                    - key: Component type name to be updated in batch.
+                    - value:
+
+                        - For homogeneous update batch (a 2D numpy structured array):
+
+                            - Dimension 0: Each batch.
+                            - Dimension 1: Each updated element per batch for this component type.
+                        - For inhomogeneous update batch (a dictionary containing two keys):
+
+                            - indptr: A 1D integer numpy array with length n_batch + 1. Given batch number k, the
+                              update array for this batch is data[indptr[k]:indptr[k + 1]]. This is the concept of
+                              compressed sparse structure.
+                              https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html
+                            - data: 1D numpy structured array in flat.
+            threading (int, optional): Applicable only for batch calculation.
+
+                - < 0: Sequential
+                - = 0: Parallel, use number of hardware threads
+                - > 0: Specify number of parallel threads
+            output_component_types ({set, list}, optional): List or set of component types you want to be present in
+                the output dict. By default, all component types will be in the output.
+            continue_on_batch_error (bool, optional): If the program continues (instead of throwing error) if some
+                scenarios fail.
 
         Returns:
-            dictionary of results of all components
-                key: component type name to be updated in batch
-                value:
-                    for single calculation: 1D numpy structured array for the results of this component type
-                    for batch calculation: 2D numpy structured array for the results of this component type
-                        Dimension 0: each batch
-                        Dimension 1: the result of each element for this component type
-            Error handling:
-                in case an error in the core occurs, an exception will be thrown
+            Dictionary of results of all components.
+
+                - key: Component type name to be updated in batch.
+                - value:
+
+                    - For single calculation: 1D numpy structured array for the results of this component type.
+                    - For batch calculation: 2D numpy structured array for the results of this component type.
+
+                        - Dimension 0: Each batch.
+                        - Dimension 1: The result of each element for this component type.
+
+        Raises:
+            Exception: In case an error in the core occurs, an exception will be thrown.
         """
         calculation_type = CalculationType.power_flow
         options = self._options(
             calculation_type=calculation_type,
             symmetric=symmetric,
             error_tolerance=error_tolerance,
             max_iterations=max_iterations,
@@ -360,62 +375,68 @@
         update_data: Optional[Dict[str, Union[np.ndarray, Dict[str, np.ndarray]]]] = None,
         threading: int = -1,
         output_component_types: Optional[Union[Set[str], List[str]]] = None,
         continue_on_batch_error: bool = False,
     ) -> Dict[str, np.ndarray]:
         """
         Calculate state estimation once with the current model attributes.
-        Or calculate in batch with the given update dataset in batch
+        Or calculate in batch with the given update dataset in batch.
 
         Args:
-            symmetric:
-                True: three-phase symmetric calculation, even for asymmetric loads/generations
-                False: three-phase asymmetric calculation
-            error_tolerance:
-                error tolerance for voltage in p.u., only applicable when the calculation method is iterative
-            max_iterations:
-                maximum number of iterations, only applicable when the calculation method is iterative
-            calculation_method: an enumeration
-                iterative_linear: use iterative linear method
-            update_data:
-                None: calculate state estimation once with the current model attributes
-                A dictionary for batch calculation with batch update
-                    key: component type name to be updated in batch
-                    value:
-                        a 2D numpy structured array for homogeneous update batch
-                            Dimension 0: each batch
-                            Dimension 1: each updated element per batch for this component type
-                        **or**
-                        a dictionary containing two keys, for inhomogeneous update batch
-                            indptr: a 1D integer numpy array with length n_batch + 1
-                                given batch number k, the update array for this batch is
-                                data[indptr[k]:indptr[k + 1]]
-                                This is the concept of compressed sparse structure
-                                https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html
-                            data: 1D numpy structured array in flat
-            threading:
-                only applicable for batch calculation
-                < 0 sequential
-                = 0 parallel, use number of hardware threads
-                > 0 specify number of parallel threads
-            output_component_types: list or set of component types you want to be present in the output dict.
-                By default all component types will be in the output
-            continue_on_batch_error: if the program continues (instead of throwing error) if some scenarios fail
+            symmetric (bool, optional): Whether to perform a three-phase symmetric calculation.
 
+                - True: Three-phase symmetric calculation, even for asymmetric loads/generations (Default).
+                - False: Three-phase asymmetric calculation.
+            error_tolerance (float, optional): error tolerance for voltage in p.u., only applicable when the
+                calculation method is iterative.
+            max_iterations (int, optional): Maximum number of iterations, applicable only when the calculation method
+                is iterative.
+            calculation_method (an enumeration): Use iterative linear method.
+            update_data (dict, optional):
+                None: Calculate state estimation once with the current model attributes.
+                Or a dictionary for batch calculation with batch update.
+
+                    - key: Component type name to be updated in batch.
+                    - value:
+
+                        - For homogeneous update batch (a 2D numpy structured array):
+
+                            - Dimension 0: Each batch.
+                            - Dimension 1: Each updated element per batch for this component type.
+                        - For inhomogeneous update batch (a dictionary containing two keys):
+
+                            - indptr: A 1D integer numpy array with length n_batch + 1. Given batch number k, the
+                              update array for this batch is data[indptr[k]:indptr[k + 1]]. This is the concept of
+                              compressed sparse structure.
+                              https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html
+                            - data: 1D numpy structured array in flat.
+            threading (int, optional): Applicable only for batch calculation.
+
+                - < 0: Sequential
+                - = 0: Parallel, use number of hardware threads
+                - > 0: Specify number of parallel threads
+            output_component_types ({set, list}, optional): List or set of component types you want to be present in
+                the output dict. By default, all component types will be in the output.
+            continue_on_batch_error (bool, optional): If the program continues (instead of throwing error) if some
+                scenarios fail.
 
         Returns:
-            dictionary of results of all components
-                key: component type name to be updated in batch
-                value:
-                    for single calculation: 1D numpy structured array for the results of this component type
-                    for batch calculation: 2D numpy structured array for the results of this component type
-                        Dimension 0: each batch
-                        Dimension 1: the result of each element for this component type
-            Error handling:
-                in case an error in the core occurs, an exception will be thrown
+            Dictionary of results of all components.
+
+                - key: Component type name to be updated in batch.
+                - value:
+
+                    - For single calculation: 1D numpy structured array for the results of this component type.
+                    - For batch calculation: 2D numpy structured array for the results of this component type.
+
+                        - Dimension 0: Each batch.
+                        - Dimension 1: The result of each element for this component type.
+
+        Raises:
+            Exception: In case an error in the core occurs, an exception will be thrown.
         """
         calculation_type = CalculationType.state_estimation
         options = self._options(
             calculation_type=calculation_type,
             symmetric=symmetric,
             error_tolerance=error_tolerance,
             max_iterations=max_iterations,
@@ -441,52 +462,56 @@
         continue_on_batch_error: bool = False,
     ) -> Dict[str, np.ndarray]:
         """
         Calculate a short circuit once with the current model attributes.
         Or calculate in batch with the given update dataset in batch
 
         Args:
-            calculation_method: an enumeration
-                iec60909: use the iec60909 standard
+            calculation_method (an enumeration): Use the iec60909 standard.
             update_data:
-                None: calculate a short circuit once with the current model attributes
-                A dictionary for batch calculation with batch update
-                    key: component type name to be updated in batch
-                    value:
-                        a 2D numpy structured array for homogeneous update batch
-                            Dimension 0: each batch
-                            Dimension 1: each updated element per batch for this component type
-                        **or**
-                        a dictionary containing two keys, for inhomogeneous update batch
-                            indptr: a 1D integer numpy array with length n_batch + 1
-                                given batch number k, the update array for this batch is
-                                data[indptr[k]:indptr[k + 1]]
-                                This is the concept of compressed sparse structure
-                                https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html
-                            data: 1D numpy structured array in flat
-            threading:
-                only applicable for batch calculation
-                < 0 sequential
-                = 0 parallel, use number of hardware threads
-                > 0 specify number of parallel threads
-            output_component_types: list or set of component types you want to be present in the output dict.
-                By default all component types will be in the output
-            continue_on_batch_error: if the program continues (instead of throwing error) if some scenarios fail
+                None: calculate a short circuit once with the current model attributes.
+                Or a dictionary for batch calculation with batch update
+
+                    - key: Component type name to be updated in batch
+                    - value:
 
+                        - For homogeneous update batch (a 2D numpy structured array):
+
+                            - Dimension 0: each batch
+                            - Dimension 1: each updated element per batch for this component type
+                        - For inhomogeneous update batch (a dictionary containing two keys):
+
+                            - indptr: A 1D integer numpy array with length n_batch + 1. Given batch number k, the
+                              update array for this batch is data[indptr[k]:indptr[k + 1]]. This is the concept of
+                              compressed sparse structure.
+                              https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html
+                            - data: 1D numpy structured array in flat.
+            threading (int, optional): Applicable only for batch calculation.
+
+                - < 0: Sequential
+                - = 0: Parallel, use number of hardware threads
+                - > 0: Specify number of parallel threads
+            output_component_types ({set, list}, optional): List or set of component types you want to be present in
+                the output dict. By default, all component types will be in the output.
+            continue_on_batch_error (bool, optional): If the program continues (instead of throwing error) if some
+                scenarios fail.
 
         Returns:
-            dictionary of results of all components
-                key: component type name to be updated in batch
-                value:
-                    for single calculation: 1D numpy structured array for the results of this component type
-                    for batch calculation: 2D numpy structured array for the results of this component type
-                        Dimension 0: each batch
-                        Dimension 1: the result of each element for this component type
-            Error handling:
-                in case an error in the core occurs, an exception will be thrown
+            Dictionary of results of all components.
+
+                - key: Component type name to be updated in batch.
+                - value:
+
+                    - For single calculation: 1D numpy structured array for the results of this component type.
+                    - For batch calculation: 2D numpy structured array for the results of this component type.
+
+                        - Dimension 0: Each batch.
+                        - Dimension 1: The result of each element for this component type.
+        Raises:
+            Exception: In case an error in the core occurs, an exception will be thrown.
         """
         calculation_type = CalculationType.short_circuit
         symmetric = False
 
         options = self._options(
             calculation_type=calculation_type,
             symmetric=symmetric,
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
     return batch_data
 
 
 def convert_python_to_numpy(data: PythonDataset, data_type: str, ignore_extra: bool = False) -> Dataset:
     """
     Convert native python data to internal numpy
+
     Args:
         data: data in dict or list
         data_type: type of data: input, update, sym_output, or asym_output
         ignore_extra: Allow (and ignore) extra attributes in the data
 
     Returns:
         A single or batch dataset for power-grid-model
@@ -127,14 +128,15 @@
 
 
 def convert_python_single_dataset_to_single_dataset(
     data: SinglePythonDataset, data_type: str, ignore_extra: bool = False
 ) -> SingleDataset:
     """
     Convert native python data to internal numpy
+
     Args:
         data: data in dict
         data_type: type of data: input, update, sym_output, or asym_output
         ignore_extra: Allow (and ignore) extra attributes in the data
 
     Returns:
         A single dataset for power-grid-model
@@ -151,14 +153,15 @@
 
 
 def convert_component_list_to_numpy(
     objects: ComponentList, component: str, data_type: str, ignore_extra: bool = False
 ) -> np.ndarray:
     """
     Convert native python data to internal numpy
+
     Args:
         objects: data in dict
         component: the name of the component
         data_type: type of data: input, update, sym_output, or asym_output
         ignore_extra: Allow (and ignore) extra attributes in the data
 
     Returns:
@@ -191,16 +194,18 @@
                 raise ValueError(f"Invalid '{attribute}' value for {component} {data_type} data: {ex}") from ex
     return array
 
 
 def convert_batch_dataset_to_batch_list(batch_data: BatchDataset) -> BatchList:
     """
     Convert batch datasets to a list of individual batches
+
     Args:
         batch_data: a batch dataset for power-grid-model
+
     Returns:
         A list of individual batches
     """
 
     # If the batch data is empty, return an empty list
     if len(batch_data) == 0:
         return []
@@ -228,14 +233,15 @@
                 list_data[i][component] = batch
     return list_data
 
 
 def get_and_verify_batch_sizes(batch_data: BatchDataset) -> int:
     """
     Determine the number of batches for each component and verify that each component has the same number of batches
+
     Args:
         batch_data: a batch dataset for power-grid-model
 
     Returns:
         The number of batches
     """
 
@@ -257,14 +263,15 @@
         checked_components.append(component)
     return n_batch_size
 
 
 def get_batch_size(batch_data: BatchArray) -> int:
     """
     Determine the number of batches and verify the data structure while we're at it.
+
     Args:
         batch_data: a batch array for power-grid-model
 
     Returns:
         The number of batches
     """
     if isinstance(batch_data, np.ndarray):
@@ -359,15 +366,16 @@
 
     return [data[indptr[i] : indptr[i + 1]] for i in range(len(indptr) - 1)]
 
 
 def convert_dataset_to_python_dataset(data: Dataset) -> PythonDataset:
     """
     Convert internal numpy arrays to native python data
-    If an attribute is not available (NaN value), it will not be exported.
+      If an attribute is not available (NaN value), it will not be exported.
+
     Args:
         data: A single or batch dataset for power-grid-model
     Returns:
         A python dict for single dataset
         A python list for batch dataset
 
     """
@@ -397,16 +405,18 @@
     return convert_single_dataset_to_python_single_dataset(data=data)
 
 
 def convert_single_dataset_to_python_single_dataset(data: SingleDataset) -> SinglePythonDataset:
     """
     Convert internal numpy arrays to native python data
     If an attribute is not available (NaN value), it will not be exported.
+
     Args:
         data: A single dataset for power-grid-model
+
     Returns:
         A python dict for single dataset
     """
 
     # This should be a single data set
     for component, array in data.items():
         if not isinstance(array, np.ndarray) or array.ndim != 1:
@@ -422,30 +432,32 @@
         for component, objects in data.items()
     }
 
 
 def import_json_data(json_file: Path, data_type: str, ignore_extra: bool = False) -> Dataset:
     """
     import json data
+
     Args:
         json_file: path to the json file
         data_type: type of data: input, update, sym_output, or asym_output
         ignore_extra: Allow (and ignore) extra attributes in the json file
 
     Returns:
-         A single or batch dataset for power-grid-model
+        A single or batch dataset for power-grid-model
     """
     with open(json_file, mode="r", encoding="utf-8") as file_pointer:
         data = json.load(file_pointer)
     return convert_python_to_numpy(data=data, data_type=data_type, ignore_extra=ignore_extra)
 
 
 def import_input_data(json_file: Path) -> SingleDataset:
     """
     import input json data
+
     Args:
         json_file: path to the json file
 
     Returns:
          A single dataset for power-grid-model
     """
     data = import_json_data(json_file=json_file, data_type="input")
@@ -453,26 +465,28 @@
     assert all(isinstance(component, np.ndarray) and component.ndim == 1 for component in data.values())
     return cast(SingleDataset, data)
 
 
 def import_update_data(json_file: Path) -> BatchDataset:
     """
     import update json data
+
     Args:
         json_file: path to the json file
 
     Returns:
          A batch dataset for power-grid-model
     """
     return cast(BatchDataset, import_json_data(json_file=json_file, data_type="update"))
 
 
 def export_json_data(json_file: Path, data: Dataset, indent: Optional[int] = 2, compact: bool = False):
     """
     export json data
+
     Args:
         json_file: path to json file
         data: a single or batch dataset for power-grid-model
         indent: indent of the file, default 2
         compact: write components on a single line
 
     Returns:
@@ -488,15 +502,15 @@
         else:
             json.dump(json_data, file_pointer, indent=indent)
 
 
 def compact_json_dump(data: Any, io_stream: IO[str], indent: int, max_level: int, level: int = 0):
     """Custom compact JSON writer that is intended to put data belonging to a single object on a single line.
 
-    For example:
+    For example::
     {
         "node": [
             {"id": 0, "u_rated": 10500.0},
             {"id": 1, "u_rated": 10500.0},
         ],
         "line": [
             {"id": 2, "node_from": 0, "node_to": 1, ...}
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/assertions.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
     Args:
         input_data: A power-grid-model input dataset
         calculation_type: Supply a calculation method, to allow missing values for unused fields
         symmetric: A boolean to state whether input data will be used for a symmetric or asymmetric calculation
 
     Raises:
-        KeyError, TypeError or ValueError if the data structure is invalid.
-        ValidationException if the contents are invalid.
+        KeyError | TypeError | ValueError: if the data structure is invalid.
+        ValidationException: if the contents are invalid.
     """
     validation_errors = validate_input_data(
         input_data=input_data, calculation_type=calculation_type, symmetric=symmetric
     )
     if validation_errors:
         raise ValidationException(validation_errors, "input_data")
 
@@ -60,15 +60,15 @@
 def assert_valid_batch_data(
     input_data: SingleDataset,
     update_data: BatchDataset,
     calculation_type: Optional[CalculationType] = None,
     symmetric: bool = True,
 ):
     """
-    Ihe input dataset is validated:
+    The input dataset is validated:
 
         1. Is the data structure correct? (checking data types and numpy array shapes)
         2. Are all input data ID's unique? (checking object identifiers across all components)
 
     For each batch the update data is validated:
         3. Is the update data structure correct? (checking data types and numpy array shapes)
         4. Are all update ID's valid? (checking object identifiers across update and input data)
@@ -80,15 +80,15 @@
     Args:
         input_data: a power-grid-model input dataset
         update_data: a power-grid-model update dataset (one or more batches)
         calculation_type: Supply a calculation method, to allow missing values for unused fields
         symmetric: A boolean to state whether input data will be used for a symmetric or asymmetric calculation
 
     Raises:
-        KeyError, TypeError or ValueError if the data structure is invalid.
-        ValidationException if the contents are invalid.
+        KeyError | TypeError | ValueError: if the data structure is invalid.
+        ValidationException: if the contents are invalid.
     """
     validation_errors = validate_batch_data(
         input_data=input_data, update_data=update_data, calculation_type=calculation_type, symmetric=symmetric
     )
     if validation_errors:
         raise ValidationException(validation_errors, "update_data")
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,17 +72,17 @@
 
 def all_greater_than_zero(data: SingleDataset, component: str, field: str) -> List[NotGreaterThanError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are greater than
     zero. Returns an empty list on success, or a list containing a single error object on failure.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        field: The field of interest
+        data (SingleDataset): The input/update data set for all components
+        component (str): The component of interest
+        field (str): The field of interest
 
     Returns:
         A list containing zero or one NotGreaterThanErrors, listing all ids where the value in the field of interest
         was zero or less.
     """
     return all_greater_than(data, component, field, 0.0)
 
@@ -94,20 +94,21 @@
     default_value: Optional[Union[np.ndarray, int, float]] = None,
 ) -> List[NotGreaterOrEqualError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are greater than,
     or equal to zero. Returns an empty list on success, or a list containing a single error object on failure.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        field: The field of interest
-        default_value: Some values are not required, but will receive a default value in the C++ core. To do a proper
-        input validation, these default values should be included in the validation. It can be a fixed value for the
-        entire column (int/float) or be different for each element (np.ndarray).
+        data (SingleDataset): The input/update data set for all components
+        component (str) The component of interest
+        field (str): The field of interest
+        default_value (Optional[Union[np.ndarray, int, float]], optional): Some values are not required, but will
+            receive a default value in the C++ core. To do a proper input validation, these default values should be
+            included in the validation. It can be a fixed value for the entire column (int/float) or be different for
+            each element (np.ndarray).
 
     Returns:
         A list containing zero or one NotGreaterOrEqualErrors, listing all ids where the value in the field of
         interest was less than zero.
     """
     return all_greater_or_equal(data, component, field, 0.0, default_value)
 
@@ -358,17 +359,17 @@
 
 
 def all_identical(data: SingleDataset, component: str, field: str) -> List[NotIdenticalError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are identical.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        field: The field of interest
+        data (SingleDataset): The input/update data set for all components
+        component (str): The component of interest
+        field (str): The field of interest
 
     Returns:
         A list containing zero or one NotIdenticalError, listing all ids of that component if the value in the field
         of interest was not identical across all components, all values for those ids, the set of unique values in
         that field and the number of unique values in that field.
     """
     field_data = data[component][field]
@@ -384,21 +385,22 @@
     data: SingleDataset, component: str, field: str, status_field: str
 ) -> List[NotIdenticalError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are identical.
     Only entries are checked where the 'status' field is not 0.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        field: The field of interest
-        status_field: The status field based on which to decide whether a component is enabled
+        data (SingleDataset): The input/update data set for all components
+        component (str): The component of interest
+        field (str): The field of interest
+        status_field (str): The status field based on which to decide whether a component is enabled
 
     Returns:
         A list containing zero or one NotIdenticalError, listing:
+
             - all ids of enabled components if the value in the field of interest was not identical across all enabled
               components
             - all values of the 'field' column for enabled components (including duplications)
             - the set of unique such values
             - the amount of unique such values.
     """
     return all_identical(
@@ -410,17 +412,17 @@
 
 def all_unique(data: SingleDataset, component: str, field: str) -> List[NotUniqueError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are unique within
     the 'field' column of that component.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        field: The field of interest
+        data (SingleDataset): The input/update data set for all components
+        component (str): The component of interest
+        field (str): The field of interest
 
     Returns:
         A list containing zero or one NotUniqueError, listing all ids where the value in the field of interest was
         not unique. If the field name was 'id' (a very common check), the id is added as many times as it occurred in
         the 'id' column, to maintain object counts.
     """
     field_data = data[component][field]
@@ -435,18 +437,19 @@
     data: SingleDataset, fields: List[Tuple[str, str]], cross_only=True
 ) -> List[MultiComponentNotUniqueError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are unique within
     the 'field' column of that component.
 
     Args:
-        data: The input/update data set for all components
-        fields: The fields of interest, formatted as [(component_1, field_1), (component_2, field_2)]
-        cross_only: Do not include duplicates within a single field. It is advised that you use all_unique() to
-        explicitly check uniqueness within a single field.
+        data (SingleDataset): The input/update data set for all components
+        fields (List[Tuple[str, str]]): The fields of interest, formatted as
+            [(component_1, field_1), (component_2, field_2)]
+        cross_only (bool, optional): Do not include duplicates within a single field. It is advised that you use
+            all_unique() to explicitly check uniqueness within a single field.
 
     Returns:
         A list containing zero or one MultiComponentNotUniqueError, listing all fields and ids where the value was not
         unique between the fields.
     """
     all_values: Dict[int, List[Tuple[Tuple[str, str], int]]] = {}
     duplicate_ids = set()
@@ -470,18 +473,18 @@
     data: SingleDataset, component: str, field: str, enum: Type[Enum]
 ) -> List[InvalidEnumValueError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are valid values for
     the supplied enum class. Returns an empty list on success, or a list containing a single error object on failure.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        field: The field of interest
-        enum: The enum type to validate against
+        data (SingleDataset): The input/update data set for all components
+        component (str): The component of interest
+        field (str): The field of interest
+        enum (Type[Enum]): The enum type to validate against
 
     Returns:
         A list containing zero or one InvalidEnumValueError, listing all ids where the value in the field of interest
         was not a valid value in the supplied enum type.
     """
     valid = [nan_type(component, field)] + list(enum)
     invalid = np.isin(data[component][field], np.array(valid, dtype=np.int8), invert=True)
@@ -729,18 +732,18 @@
 def all_valid_fault_phases(
     data: SingleDataset, component: str, fault_type_field: str, fault_phase_field: str
 ) -> List[FaultPhaseError]:
     """
     Custom validation rule: Only a subset of fault_phases is supported for each fault type.
 
     Args:
-        data: The input/update data set for all components
-        component: The component of interest
-        fault_type_field: The fault type field
-        fault_phase_field: The fault phase field
+        data (SingleDataset): The input/update data set for all components
+        component (str): The component of interest
+        fault_type_field (str): The fault type field
+        fault_phase_field (str): The fault phase field
 
     Returns:
         A list containing zero or more FaultPhaseErrors; listing all the ids of faults where the fault phase was
         invalid, given the fault phase.
     """
     fault_types = data[component][fault_type_field]
     fault_phases = data[component][fault_phase_field]
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,21 +128,23 @@
     errors: Union[List[ValidationError], Dict[int, List[ValidationError]], None],
     name: str = "the data",
     details: bool = False,
     id_lookup: Optional[Union[List[str], Dict[int, str]]] = None,
 ) -> str:
     """
     Convert a set of errors (list or dict) to a human readable string representation.
+
     Args:
         errors: The error objects. List for input_data only, dict for batch data.
         name: Human understandable name of the dataset, e.g. input_data, or update_data.
         details: Display object ids and error specific information.
         id_lookup: A list or dict (int->str) containing textual object ids
 
-    Returns: A human readable string representation of a set of errors.
+    Returns:
+        A human readable string representation of a set of errors.
     """
     if errors is None or len(errors) == 0:
         return f"{name}: OK"
     if isinstance(errors, dict):
         return "\n".join(errors_to_string(err, f"{name}, batch #{i}", details) for i, err in sorted(errors.items()))
     if len(errors) == 1 and not details:
         return f"There is a validation error in {name}:\n\t{errors[0]}"
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model/validation/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,19 +69,19 @@
         4. Are the supplied values valid? (checking limits and other logic as described in "Graph Data Model")
 
     Args:
         input_data: A power-grid-model input dataset
         calculation_type: Supply a calculation method, to allow missing values for unused fields
         symmetric: A boolean to state whether input data will be used for a symmetric or asymmetric calculation
 
-    Raises:
-        KeyError, TypeError or ValueError if the data structure is invalid.
-
     Returns:
         None if the data is valid, or a list containing all validation errors.
+
+    Raises:
+        Error: KeyError | TypeError | ValueError: if the data structure is invalid.
     """
     # A deep copy is made of the input data, since default values will be added in the validation process
     input_data_copy = copy.deepcopy(input_data)
     assert_valid_data_structure(input_data_copy, "input")
 
     errors: List[ValidationError] = []
     errors += validate_required_values(input_data_copy, calculation_type, symmetric)
@@ -93,39 +93,39 @@
 def validate_batch_data(
     input_data: SingleDataset,
     update_data: BatchDataset,
     calculation_type: Optional[CalculationType] = None,
     symmetric: bool = True,
 ) -> Optional[Dict[int, List[ValidationError]]]:
     """
-    Ihe input dataset is validated:
+    The input dataset is validated:
 
         1. Is the data structure correct? (checking data types and numpy array shapes)
         2. Are all input data ID's unique? (checking object identifiers across all components)
 
     For each batch the update data is validated:
         3. Is the update data structure correct? (checking data types and numpy array shapes)
         4. Are all update ID's valid? (checking object identifiers across update and input data)
 
     Then (for each batch independently) the input dataset is updated with the batch's update data and validated:
         5. Are all required values provided? (checking NaNs)
         6. Are the supplied values valid? (checking limits and other logic as described in "Graph Data Model")
 
     Args:
-        input_data: a power-grid-model input dataset
-        update_data: a power-grid-model update dataset (one or more batches)
+        input_data: A power-grid-model input dataset
+        update_data: A power-grid-model update dataset (one or more batches)
         calculation_type: Supply a calculation method, to allow missing values for unused fields
         symmetric: A boolean to state whether input data will be used for a symmetric or asymmetric calculation
 
-    Raises:
-        KeyError, TypeError or ValueError if the data structure is invalid.
-
     Returns:
         None if the data is valid, or a dictionary containing all validation errors,
         where the key is the batch number (0-indexed).
+
+    Raises:
+        Error: KeyError | TypeError | ValueError: if the data structure is invalid.
     """
     assert_valid_data_structure(input_data, "input")
 
     input_errors: List[ValidationError] = list(validate_unique_ids_across_components(input_data))
 
     # Splitting update_data_into_batches may raise TypeErrors and ValueErrors
     batch_data = convert_batch_dataset_to_batch_list(update_data)
@@ -149,18 +149,19 @@
 
 def assert_valid_data_structure(data: Dataset, data_type: str) -> None:
     """
     Checks if all component names are valid and if the data inside the component matches the required Numpy
     structured array as defined in the Power Grid Model meta data.
 
     Args:
-        data: a power-grid-model input/update dataset
+        data: A power-grid-model input/update dataset
         data_type: 'input' or 'update'
 
-    Raises: KeyError, TypeError
+    Raises:
+        Error: KeyError, TypeError
 
     """
     if data_type not in {"input", "update"}:
         raise KeyError(f"Unexpected data type '{data_type}' (should be 'input' or 'update')")
 
     component_dtype = {component: meta.dtype for component, meta in power_grid_meta_data[data_type].items()}
     for component, array in data.items():
@@ -186,55 +187,56 @@
 
 
 def validate_unique_ids_across_components(data: SingleDataset) -> List[MultiComponentNotUniqueError]:
     """
     Checks if all ids in the input dataset are unique
 
     Args:
-        data: a power-grid-model input dataset
-
-    Returns: an empty list if all ids are unique, or a list of MultiComponentNotUniqueErrors for all components that
-             have non-unique ids
+        data: A power-grid-model input dataset
 
+    Returns:
+        An empty list if all ids are unique, or a list of MultiComponentNotUniqueErrors for all components that
+        have non-unique ids
     """
     return all_cross_unique(data, [(component, "id") for component in data])
 
 
 def validate_ids_exist(update_data: Dict[str, np.ndarray], input_data: SingleDataset) -> List[IdNotInDatasetError]:
     """
     Checks if all ids of the components in the update data exist in the input data. This needs to be true, because you
     can only update existing components.
 
     This function should be called for every update dataset in a batch set
 
     Args:
-        update_data: a single update dataset
-        input_data: a power-grid-model input dataset
+        update_data: A single update dataset
+        input_data: A power-grid-model input dataset
 
-    Returns: an empty list if all update data ids exist in the input dataset, or a list of IdNotInDatasetErrors for
-             all update components of which the id does not exist in the input dataset
+    Returns:
+        An empty list if all update data ids exist in the input dataset, or a list of IdNotInDatasetErrors for
+        all update components of which the id does not exist in the input dataset
 
     """
     errors = (all_ids_exist_in_data_set(update_data, input_data, component, "input_data") for component in update_data)
     return list(chain(*errors))
 
 
 def validate_required_values(
     data: SingleDataset, calculation_type: Optional[CalculationType] = None, symmetric: bool = True
 ) -> List[MissingValueError]:
     """
     Checks if all required data is available.
 
     Args:
-        data: a power-grid-model input dataset
+        data: A power-grid-model input dataset
         calculation_type: Supply a calculation method, to allow missing values for unused fields
         symmetric: A boolean to state whether input data will be used for a symmetric or asymmetric calculation
 
-    Returns: an empty list if all required data is available, or a list of MissingValueErrors.
-
+    Returns:
+        An empty list if all required data is available, or a list of MissingValueErrors.
     """
     # Base
     required = {"base": ["id"]}
 
     # Nodes
     required["node"] = required["base"] + ["u_rated"]
 
@@ -332,17 +334,18 @@
 
 
 def validate_values(data: SingleDataset) -> List[ValidationError]:  # pylint: disable=too-many-branches
     """
     For each component supplied in the data, call the appropriate validation function
 
     Args:
-        data: a power-grid-model input dataset
+        data: A power-grid-model input dataset
 
-    Returns: an empty list if all required data is valid, or a list of ValidationErrors.
+    Returns:
+        An empty list if all required data is valid, or a list of ValidationErrors.
 
     """
     errors: List[ValidationError] = list(all_finite(data))
     if "node" in data:
         errors += validate_node(data)
     if "line" in data:
         errors += validate_line(data)
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9214011953671
+Version: 1.5.0rc9214410208671
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9214011953671/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9214410208671/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9214410208671/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/three_phase_abc/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/three_phase_abc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9214410208671/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/utils.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9214011953671/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9214410208671/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

