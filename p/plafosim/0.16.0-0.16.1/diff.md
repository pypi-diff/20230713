# Comparing `tmp/plafosim-0.16.0.tar.gz` & `tmp/plafosim-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plafosim-0.16.0.tar", max compression
+gzip compressed data, was "plafosim-0.16.1.tar", max compression
```

## Comparing `plafosim-0.16.0.tar` & `plafosim-0.16.1.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0    35149 2021-02-01 21:06:08.184543 plafosim-0.16.0/LICENSE
--rw-r--r--   0        0        0     9934 2023-04-28 13:34:00.128362 plafosim-0.16.0/README.md
--rw-r--r--   0        0        0     2427 2023-04-28 13:34:00.128362 plafosim-0.16.0/pyproject.toml
--rw-r--r--   0        0        0     2527 2023-04-28 13:34:00.128362 plafosim-0.16.0/src/plafosim/__init__.py
--rw-r--r--   0        0        0      738 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/algorithms/__init__.py
--rw-r--r--   0        0        0     2407 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/algorithms/dummy.py
--rw-r--r--   0        0        0    30567 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/algorithms/speed_position.py
--rw-r--r--   0        0        0      738 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/cli/__init__.py
--rw-r--r--   0        0        0    23667 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/cli/plafosim.py
--rw-r--r--   0        0        0     5357 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/cli/trace_replay.py
--rw-r--r--   0        0        0     1716 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/emissions.py
--rw-r--r--   0        0        0     2664 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/formation_algorithm.py
--rw-r--r--   0        0        0     9372 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/gui.py
--rw-r--r--   0        0        0     4398 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/infrastructure.py
--rw-r--r--   0        0        0     6646 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/message.py
--rw-r--r--   0        0        0    19006 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/mobility.py
--rw-r--r--   0        0        0     5190 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/neighbortable.py
--rw-r--r--   0        0        0     7553 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/platoon.py
--rw-r--r--   0        0        0     1180 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/platoon_role.py
--rw-r--r--   0        0        0    56157 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/platooning_vehicle.py
--rw-r--r--   0        0        0    76270 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/simulator.py
--rw-r--r--   0        0        0     4661 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/spawning.py
--rw-r--r--   0        0        0    19290 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/statistics.py
--rw-r--r--   0        0        0    42487 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.gui.xml
--rw-r--r--   0        0        0     1907 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.net.xml
--rw-r--r--   0        0        0     1083 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.rou.xml
--rw-r--r--   0        0        0     1328 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.sumo.cfg
--rw-r--r--   0        0        0     5756 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/util.py
--rw-r--r--   0        0        0    21551 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/vehicle.py
--rw-r--r--   0        0        0     4188 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/vehicle_type.py
--rw-r--r--   0        0        0    11244 2023-04-28 13:38:46.620355 plafosim-0.16.0/setup.py
--rw-r--r--   0        0        0    11132 2023-04-28 13:38:46.620857 plafosim-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-02-01 21:06:08.184543 plafosim-0.16.1/LICENSE
+-rw-r--r--   0        0        0    10138 2023-07-13 13:04:17.434694 plafosim-0.16.1/README.md
+-rw-r--r--   0        0        0     2427 2023-07-13 13:04:17.434694 plafosim-0.16.1/pyproject.toml
+-rw-r--r--   0        0        0     2527 2023-07-13 13:04:17.434694 plafosim-0.16.1/src/plafosim/__init__.py
+-rw-r--r--   0        0        0      738 2023-07-13 13:02:58.293789 plafosim-0.16.1/src/plafosim/algorithms/__init__.py
+-rw-r--r--   0        0        0     2428 2023-07-13 13:02:58.293789 plafosim-0.16.1/src/plafosim/algorithms/dummy.py
+-rw-r--r--   0        0        0    30588 2023-07-13 13:02:58.293789 plafosim-0.16.1/src/plafosim/algorithms/speed_position.py
+-rw-r--r--   0        0        0      738 2023-07-13 13:02:58.293789 plafosim-0.16.1/src/plafosim/cli/__init__.py
+-rw-r--r--   0        0        0    30528 2023-07-13 13:02:58.293789 plafosim-0.16.1/src/plafosim/cli/plafosim.py
+-rw-r--r--   0        0        0     5343 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/cli/trace_replay.py
+-rw-r--r--   0        0        0     1716 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/emissions.py
+-rw-r--r--   0        0        0     2664 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/formation_algorithm.py
+-rw-r--r--   0        0        0     9372 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/gui.py
+-rw-r--r--   0        0        0     4398 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/infrastructure.py
+-rw-r--r--   0        0        0    19006 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/mobility.py
+-rw-r--r--   0        0        0     7553 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/platoon.py
+-rw-r--r--   0        0        0     1180 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/platoon_role.py
+-rw-r--r--   0        0        0    53694 2023-07-13 13:02:58.297789 plafosim-0.16.1/src/plafosim/platooning_vehicle.py
+-rw-r--r--   0        0        0    76270 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/simulator.py
+-rw-r--r--   0        0        0     4661 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/spawning.py
+-rw-r--r--   0        0        0    19290 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/statistics.py
+-rw-r--r--   0        0        0    42487 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/sumocfg/freeway.gui.xml
+-rw-r--r--   0        0        0     1907 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/sumocfg/freeway.net.xml
+-rw-r--r--   0        0        0     1083 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/sumocfg/freeway.rou.xml
+-rw-r--r--   0        0        0     1328 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/sumocfg/freeway.sumo.cfg
+-rw-r--r--   0        0        0     5768 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/util.py
+-rw-r--r--   0        0        0    18564 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/vehicle.py
+-rw-r--r--   0        0        0     4188 2023-07-13 13:02:58.301789 plafosim-0.16.1/src/plafosim/vehicle_type.py
+-rw-r--r--   0        0        0    11448 2023-07-13 13:04:55.989320 plafosim-0.16.1/setup.py
+-rw-r--r--   0        0        0    11336 2023-07-13 13:04:55.989940 plafosim-0.16.1/PKG-INFO
```

### Comparing `plafosim-0.16.0/LICENSE` & `plafosim-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plafosim-0.16.0/README.md` & `plafosim-0.16.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Platoon Formation Simulator (PlaFoSim)
 
-[![Code Version](https://img.shields.io/badge/code-v0.16.0-blue)](CHANGELOG.md)
+[![Code Version](https://img.shields.io/badge/code-v0.16.1-blue)](CHANGELOG.md)
 [![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)
 [![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)
 [![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)
 
 [PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.
 
@@ -22,29 +22,29 @@
 
 Please note that PlaFoSim is still under heavy development.
 
 ---
 
 ## Installation
 
-- Install Python (>=3.7.0,<3.10)
-- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)
+- Install Python (>=3.7,<=3.9)
 - Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):
 ```pip install plafosim```
+- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)
 
-NOTE: The project is currently only tested under Linux.
+NOTE: The project is developed and currently only tested on Linux.
 
 ## Running a Simulation
 
-You can use the simulator as module as well as from the command-line.
+You can use the PlaFoSim as Python module as well as from the command-line.
 Currently, only command-line is thoroughly tested and thus completely available though.
 
 ### Quickstart
 
-Use PlaFoSim's binary to run a simulation with the default configuration:
+Use PlaFoSim's binary to run a simulation with the default configuration (`-d`):
 
 ```plafosim -d```
 
 ### Advanced Simulation Control
 
 You can use a variety of different parameters to customize the scenario and the simulation itself.
 E.g., use the parameter `vehicles` to configure the number of vehicles in the simulation:
@@ -109,55 +109,55 @@
 
 ```PYTHONOPTIMIZE=1 plafosim```
 
 See the Python [documention](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE) for more details.
 
 ## Re-Playing a Simulation
 
-The simulation can write a trace file for every simulated vehicle (default `results_vehicle_traces.csv`).
-You can replay the simulation based on the trace file by using a corresponding binary:
+The simulation can write a trace file including the mobility details of every simulated vehicle (default `results_vehicle_traces.csv`).
+You can replay the simulation in the GUI (see above) based on the trace file by using the corresponding binary:
 
 ```plafosim-replay results_vehicle_traces.csv```
 
 To see all options of this script, run:
 
 ```plafosim-replay -h, --help```
 
-## Extending
+## Extending the Simulator
 
-- Clone the repository
 - Install [poetry](https://python-poetry.org/):
 ```pip install poetry```
+- Clone the repository
 - Install PlaFoSim from source in editable mode:
 ```poetry install```
 - Run PlaFoSim in the virtual environment with
 ```poetry run plafosim```
 or activate the virtual enviroment first with
 ```poetry shell```
 and run the commands as usual (see above)
 
 NOTE: The project is currently only tested under Linux.
 
 In order to add a new formation algorithm, you need to follow these steps:
 - Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.
 - Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.
-- Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.
+- Add specific properties of your algorithm via an argument parser group and a corresponding help message to `cli/plafosim.py` if necessary.
 - Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).
 
 You should now be able to use your new algorithm with
 ```
 plafosim --formation-algorithm dummy_algorithm_name
 ```
 
-## Contributing
+## Contributing to the Project
 
 In order to contribute, please follow these steps:
 - Install PlaFoSim from source (see above)
 - Make desired changes
-- Run the tests located in `scripts` (see `.drone.yml`)
+- Run the tests located in `tests` as well as the validation scripts located in `scripts` (see `.drone.yml` for details)
 - Submit a Pull Request (PR)
 
 ### Testing
 
 When adding methods and functions, make sure to add corresponding unit tests for `py.test`.
 The tests are located under `tests` and can be executed with `./scripts/run-pytest.sh`.
 This will also generate a test coverage report.
@@ -205,15 +205,15 @@
 ```
 
 ## License
 
 PlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.
 
 ```
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/pyproject.toml` & `plafosim-0.16.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -15,15 +15,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 [tool.poetry]
 name = "plafosim"
-version = "0.16.0"
+version = "0.16.1"
 description = "A simple and scalable simulator for platoon formation."
 license = "GPL-3.0-or-later"
 authors = [
     "Julian Heinovski <heinovski@ccs-labs.org>",
     "Dominik S. Buse <buse@ccs-labs.org",
 ]
 maintainers = [
```

### Comparing `plafosim-0.16.0/src/plafosim/__init__.py` & `plafosim-0.16.1/src/plafosim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -18,21 +18,21 @@
 #
 
 import argparse
 import textwrap
 
 from plafosim.util import addLoggingLevel
 
-__version__ = "0.16.0"
+__version__ = "0.16.1"
 
 __description__ = textwrap.dedent(f"""\
     Platoon Formation Simulator (PlaFoSim) -- Version {__version__}.
     A simple and scalable simulator for platoon formation.
 
-    Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+    Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 
     SPDX-License-Identifier: GPL-3.0-or-later
 
     This program comes with ABSOLUTELY NO WARRANTY.
     This is free software, and you are welcome to redistribute it under certain conditions.
 
     If you are working with PlaFoSim, please cite the following paper:
```

### Comparing `plafosim-0.16.0/src/plafosim/algorithms/__init__.py` & `plafosim-0.16.1/src/plafosim/algorithms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/algorithms/dummy.py` & `plafosim-0.16.1/src/plafosim/algorithms/dummy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -53,14 +53,15 @@
         group = parser.add_argument_group(f"Formation Algorithm -- {cls.__name__}")
         group.add_argument(
             "--dummy",
             type=int,
             default=-1,
             help="A dummy parameter",
         )
+        return group
 
     def do_formation(self):
         """
         Run platoon formation algorithm to search for a platooning opportunity
         and performs the corresponding maneuvers.
         """
```

### Comparing `plafosim-0.16.0/src/plafosim/algorithms/speed_position.py` & `plafosim-0.16.1/src/plafosim/algorithms/speed_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -140,14 +140,15 @@
         )
         group.add_argument(
             "--solver-time-limit",
             type=int,
             default=int(DEFAULTS['solver_time_limit'] / 1000),  # ms -> s
             help="The time limit for the optimal solver per assignment problem in s. Influences the quality of the solution.",
         )
+        return group
 
     def ds(self, vehicle: 'PlatooningVehicle', platoon: 'Platoon'):
         """
         Return the deviation in speed from a given platoon.
 
         NOTE: In the original version of the paper, the deviation calculated here was not normalized.
```

### Comparing `plafosim-0.16.0/src/plafosim/cli/__init__.py` & `plafosim-0.16.1/src/plafosim/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/cli/plafosim.py` & `plafosim-0.16.1/src/plafosim/cli/plafosim.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -14,39 +14,102 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 import argparse
+import json
 import logging
 import pickle
 import sys
 from distutils.util import strtobool
 from signal import SIGINT, signal
 from timeit import default_timer as timer
 
 from plafosim import CustomFormatter, __citation__, __description__, __version__
 from plafosim.algorithms.speed_position import SpeedPosition
 from plafosim.simulator import DEFAULTS, Simulator
 from plafosim.util import find_resource
 
+__epilog__ = """\
+Examples:
+  # Configure a 100km freeway with ramps at every 10km
+  plafosim --road-length 100 --ramp-interval 10
+
+  # Configure random (normally distributed) desired driving speed of 130km/h
+  plafosim --random-desired-speed true --desired-speed 36
+
+  # Configure random trips for 500 vehicles
+  plafosim --vehicles 500 --random-depart-position true --random-arrival-position true --depart-desired true
+
+  # Pre fill the freeway with 1000 vehicles
+  plafosim --vehicles 1000 --pre-fill true
+
+  # Configure 50% of the vehicles with Advanced Cruise Control (ACC) and a headway time of 1.5s
+  plafosim --penetration 0.5 --acc-headway-time 1.5
+
+  # Enable a simple, distributed platoon formation algorithm [1] in order to form platoons every 30s
+  plafosim --formation-algorithm SpeedPosition --formation-strategy distributed --execution-interval 30
+"""
+
+
+def format_help(parser: argparse.ArgumentParser, groups=None) -> str:
+    """
+    Format help message for argument groups
+
+    Taken from https://stackoverflow.com/a/40730878.
+    """
+
+    formatter = parser._get_formatter()
+
+    # usage
+    formatter.add_usage(
+        parser.usage,
+        parser._actions,
+        parser._mutually_exclusive_groups,
+    )
+
+    # description
+    formatter.add_text(parser.description)
+
+    if groups is None:
+        groups = parser._action_groups
+
+    # positionals, optionals and user-defined groups
+    for action_group in groups:
+        formatter.start_section(action_group.title)
+        formatter.add_text(action_group.description)
+        formatter.add_arguments(action_group._group_actions)
+        formatter.end_section()
+
+    # determine help from format above
+    return formatter.format_help()
+
 
 # TODO duplicated code with trace replay
 def parse_args() -> (argparse.Namespace, argparse._ArgumentGroup):
 
     # parse some parameters
     parser = argparse.ArgumentParser(
         formatter_class=CustomFormatter,
         allow_abbrev=False,
         description=__description__,
+        add_help=False,
+        epilog=__epilog__,
     )
 
     # miscellaneous
     parser.add_argument(
+        '-h', '--help',
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help='show this help message and exit',
+    )
+    parser.add_argument(
         "-C", "--citation",
         action="version",
         help="show the citation information and exit",
         version=__citation__,
     )
     parser.add_argument(
         "-V", "--version",
@@ -86,537 +149,665 @@
         "--load-snapshot",
         type=str,
         default=None,
         metavar="FILE",
         help="Load a snapshot of the scenario from FILE and run the simulation",
     )
 
+    # custom help messages
+    g_help = parser.add_argument_group("help messages")
+    g_help.add_argument(
+        "--help-all",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show complete help message and exit",
+    )
+
     # road network properties
-    road = parser.add_argument_group("road network properties")
-    road.add_argument(
+    g_road = parser.add_argument_group("road network properties")
+    g_help.add_argument(
+        "--help-road",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for road network properties and exit",
+    )
+    g_road.add_argument(
         "--road-length",
         type=int,
         default=int(DEFAULTS['road_length'] / 1000),  # m -> km
         help="The length of the road in km",
     )
-    road.add_argument(
+    g_road.add_argument(
         "--lanes",
         type=int,
         dest='number_of_lanes',
         default=DEFAULTS['lanes'],
         help="The number of lanes",
     )
-    road.add_argument(
+    g_road.add_argument(
         "--ramp-interval",
         type=int,
         default=int(DEFAULTS['ramp_interval'] / 1000),  # m -> km
         help="The distance between any two on-/off-ramps in km",
     )
-    road.add_argument(
+    g_road.add_argument(
         "--pre-fill",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['pre_fill'],
         choices=(True, False),
         help="Whether to fill the road network with vehicles using random positions and given vehicle number/density before the simulation starts",
     )
 
     # vehicle properties
-    vehicle = parser.add_argument_group("vehicle properties")
-    vehicle.add_argument(
+    g_vehicles = parser.add_argument_group("vehicle properties")
+    g_help.add_argument(
+        "--help-vehicles",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for vehicle properties and exit",
+    )
+    g_vehicles.add_argument(
         "--vehicles",
         type=int,
         dest='number_of_vehicles',
         default=DEFAULTS['vehicles'],
         help="The (maximum) number of vehicles that are in the simulation at once. Is used for pre-fill, without a depart flow, and for some depart methods. A value of -1 disables this value.",
     )
-    vehicle.add_argument(
+    g_vehicles.add_argument(
         "--density",
         type=float,
         dest='vehicle_density',
         default=DEFAULTS['vehicle_density'],
         help="The (maximum) density (i.e., number of vehicles per km per lane) of vehicles that are in the simulation at once. Overrides --vehicles but behaves similarly. A value of -1 disables this value",
     )
-    vehicle.add_argument(
+    g_vehicles.add_argument(
         "--max-speed",
         type=float,
         default=DEFAULTS['max_speed'],
         help="The maximum possible driving speed in m/s",
     )
-    vehicle.add_argument(
+    g_vehicles.add_argument(
         "--acc-headway-time",
         type=float,
         default=DEFAULTS['acc_headway_time'],
         help="The headway time to be used for the ACC in s",
     )
-    vehicle.add_argument(
+    g_vehicles.add_argument(
         "--cacc-spacing",
         type=float,
         default=DEFAULTS['cacc_spacing'],
         help="The constant spacing to be used for the CACC in m",
     )
-    vehicle.add_argument(
+    g_vehicles.add_argument(
         "--penetration",
         type=float,
         dest='penetration_rate',
         default=DEFAULTS['penetration_rate'],
         help="Penetration rate of vehicles with platooning capabilities",
     )
 
     # trip properties
-    trip = parser.add_argument_group("trip properties")
-    trip.add_argument(
+    g_trips = parser.add_argument_group("trip properties")
+    g_help.add_argument(
+        "--help-trips",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for trip properties and exit",
+    )
+    g_trips.add_argument(
         "--random-depart-position",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['random_depart_position'],
         choices=(True, False),
         help="Whether to use a random depart position for every vehicle instead of 0 m",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--desired-speed",
         type=float,
         default=DEFAULTS['desired_speed'],
         help="The desired driving speed im m/s",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--random-desired-speed",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['random_desired_speed'],
         choices=(True, False),
         help="Whether to pick a random (normally distributed) desired driving speed",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--speed-variation",
         type=float,
         default=DEFAULTS['speed_variation'],
         help="The deviation from the desired driving speed in ratio",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--min-desired-speed",
         type=float,
         default=DEFAULTS['min_desired_speed'],
         help="The minimum desired driving speed im m/s",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--max-desired-speed",
         type=float,
         default=DEFAULTS['max_desired_speed'],
         help="The maximum desired driving speed im m/s",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--random-depart-speed",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['random_depart_speed'],
         choices=(True, False),
         help="Whether to use a random depart speed for every vehicle instead of 0 m/s",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--depart-desired",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['depart_desired'],
         choices=(True, False),
         help="Whether the vehicle should depart with its desired speed. Overrides --random-depart-speed",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--depart-flow",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['depart_flow'],
         choices=(True, False),
         help="Whether to spawn vehicles in a continuous flow or as fixed number of vehicles",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--depart-method",
         type=str,
         choices=("interval", "probability", "rate", "number"),
         default=DEFAULTS['depart_method'],
         help="The departure method of vehicles. Can be limited when depart-flow is disabled.",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--depart-interval",
         type=float,
         default=DEFAULTS['depart_interval'],
         help="The interval between two vehicle departures in s for depart method 'interval'",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--depart-probability",
         type=float,
         default=DEFAULTS['depart_probability'],
         help="The probability of departure per time step for depart method 'probability'",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--depart-rate",
         type=int,
         default=DEFAULTS['depart_rate'],
         help="The rate of departure in vehicles per hour for depart method 'rate'",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--random-arrival-position",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['random_arrival_position'],
         choices=(True, False),
         help="Whether to use a random arrival position for every vehicle instead of the end of the road",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--minimum-trip-length",
         type=int,
         default=int(DEFAULTS['minimum_trip_length'] / 1000),  # m -> km
         help="The minimum trip length for a vehicle in km",
     )
-    trip.add_argument(
+    g_trips.add_argument(
         "--maximum-trip-length",
         type=int,
         default=int(DEFAULTS['maximum_trip_length'] / 1000),  # m -> km
         help="The maximum trip length for a vehicle in km",
     )
 
     # communication properties
-    communication = parser.add_argument_group("communication properties")
-    communication.add_argument(
+    g_communication = parser.add_argument_group("communication properties")
+    g_help.add_argument(
+        "--help-communication",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for communication properties and exit",
+    )
+    g_communication.add_argument(
         "--communication-range",
         type=int,
         default=DEFAULTS['communication_range'],
         help="The maximum communication range between two vehicles in m. A value of -1 disables the communication range check",
     )
 
     # platoon properties
-    platoon = parser.add_argument_group("platoon properties")
-    platoon.add_argument(
+    g_platoon = parser.add_argument_group("platoon properties")
+    g_help.add_argument(
+        "--help-platoon",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for platoon properties and exit",
+    )
+    g_platoon.add_argument(
         "--start-as-platoon",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['start_as_platoon'],
         choices=(True, False),
         help="Whether vehicles should automatically start as one platoon",
     )
-    platoon.add_argument(
+    g_platoon.add_argument(
         "--reduced-air-drag",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['reduced_air_drag'],
         choices=(True, False),
         help="Whether the reduced air drag due to platooning should be considered in the emissions calculation",
     )
-    platoon.add_argument(
+    g_platoon.add_argument(
         "--maximum-teleport-distance",
         type=int,
         default=DEFAULTS['maximum_teleport_distance'],
         help="The maximum teleport distance in m. A value of -1 disables the check",
     )
-    platoon.add_argument(
+    g_platoon.add_argument(
         "--maximum-approach-time",
         type=int,
         default=DEFAULTS['maximum_approach_time'],
         help="The maximum time for approaching a platoon during a join maneuver in s. A value of -1 disables the check",
     )
-    platoon.add_argument(
+    g_platoon.add_argument(
         "--delay-teleports",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['delay_teleports'],
         choices=(True, False),
         help="Whether teleports (i.e., during a join maneuver) should be delayed by the time for approaching the target platoon",
     )
-    platoon.add_argument(
+    g_platoon.add_argument(
         "--update-desired-speed",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['update_desired_speed'],
         choices=(True, False),
         help="Whether to update the platoon's desired driving speed to the average speed of all members after the formation changed",
     )
 
     # formation properties
-    formation = parser.add_argument_group("formation properties")
-    formation.add_argument(
+    g_formation = parser.add_argument_group("formation properties")
+    g_help.add_argument(
+        "--help-formation",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for formation properties and exit",
+    )
+    g_formation.add_argument(
         "--formation-algorithm",
         type=str,
         default=DEFAULTS['formation_algorithm'],
         # TODO use enum
         choices=[SpeedPosition.__name__],
         help="The formation algorithm to use",
     )
-    formation.add_argument(
+    g_formation.add_argument(
         "--formation-strategy",
         type=str,
         default=DEFAULTS['formation_strategy'],
         choices=["distributed", "centralized"],
         help="The formation strategy to use",
     )
-    formation.add_argument(
+    g_formation.add_argument(
         "--execution-interval",
         type=int,
         default=DEFAULTS['execution_interval'],
         help="The interval between two iterations of a formation algorithm in s",
     )
 
-    # formation algorithm specific properties
-    ## speed position
-    SpeedPosition.add_parser_argument_group(parser)
-
     # infrastructure properties
-    infrastructures = parser.add_argument_group("infrastructure properties")
-    infrastructures.add_argument(
+    g_infrastructure = parser.add_argument_group("infrastructure properties")
+    g_help.add_argument(
+        "--help-infrastructure",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for infrastructure properties and exit",
+    )
+    g_infrastructure.add_argument(
         "--infrastructures",
         type=int,
         dest='number_of_infrastructures',
         default=DEFAULTS['infrastructures'],
         help="The number of infrastructures",
     )
 
     # simulation properties
-    simulation = parser.add_argument_group("simulation properties")
-    simulation.add_argument(
+    g_simulation = parser.add_argument_group("simulation properties")
+    g_help.add_argument(
+        "--help-simulation",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for simulation properties and exit",
+    )
+    g_simulation.add_argument(
         "--step-length",
         type=int,
         default=DEFAULTS['step_length'],
         help="The step length in s",
     )
-    simulation.add_argument(
+    g_simulation.add_argument(
         "--time-limit",
         type=float,
         dest='max_step',
         default=float(DEFAULTS['max_step'] / 3600),  # s -> h
         help="The simulation limit in h",
     )
-    simulation.add_argument(
+    g_simulation.add_argument(
         "--actions",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['actions'],
         choices=(True, False),
         help="Whether to enable actions",
     )
-    simulation.add_argument(
+    g_simulation.add_argument(
         "--collisions",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['collisions'],
         choices=(True, False),
         help="Whether to enable collision checks",
     )
-    simulation.add_argument(
+    g_simulation.add_argument(
         "--random-seed",
         type=int,
         default=DEFAULTS['random_seed'],
         help="The seed (>=0) for the random number generator instead of the current system time",
     )
-    simulation.add_argument(
+    g_simulation.add_argument(
         "--progress",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['progress'],
         choices=(True, False),
         help="Whether to enable the (simulation) progress bar",
     )
 
     # gui properties
-    gui = parser.add_argument_group("gui properties")
-    gui.add_argument(
+    g_gui = parser.add_argument_group("gui properties")
+    g_help.add_argument(
+        "--help-gui",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for gui properties and exit",
+    )
+    g_gui.add_argument(
         "--gui",
         action="store_true",
         help="Enable a live SUMO GUI"
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--gui-delay",
         type=int,
         default=int(DEFAULTS['gui_delay'] * 1000),  # s -> ms
         help="The delay used in every simulation step to visualize the current network state in ms",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--track-vehicle",
         type=int,
         dest='gui_track_vehicle',
         default=DEFAULTS['gui_track_vehicle'],
         help="The id of a vehicle to track in the gui",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--sumo-config",
         type=find_resource,
         default=DEFAULTS['sumo_config'],
         help="The name of the SUMO config file",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--gui-play",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['gui_play'],
         choices=(True, False),
         help="Whether to start the simulation immediately",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--gui-start",
         type=int,
         default=DEFAULTS['gui_start'],
         help="The time to connect to the GUI in s",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--draw-ramps",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['draw_ramps'],
         choices=(True, False),
         help="Whether to draw on-/off-ramps",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--draw-ramp-labels",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['draw_ramp_labels'],
         choices=(True, False),
         help="Whether to draw labels for on-/off-ramps",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--draw-road-end",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['draw_road_end'],
         choices=(True, False),
         help="Whether to draw the end of the road",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--draw-road-end-label",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['draw_road_end_label'],
         choices=(True, False),
         help="Whether to draw a label for the end of the road",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--draw-infrastructures",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['draw_infrastructures'],
         choices=(True, False),
         help="Whether to draw infrastructures",
     )
-    gui.add_argument(
+    g_gui.add_argument(
         "--draw-infrastructure-labels",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['draw_infrastructure_labels'],
         choices=(True, False),
         help="Whether to draw labels for infrastructures",
     )
 
     # result recording properties
-    results = parser.add_argument_group("result recording properties")
-    results.add_argument(
+    g_results = parser.add_argument_group("result recording properties")
+    g_help.add_argument(
+        "--help-results",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help="show help message for result recording properties and exit",
+    )
+    g_results.add_argument(
         "--result-base-filename",
         type=str,
         default=DEFAULTS['result_base_filename'],
         help="The base filename of the result files",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-simulation-trace",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_simulation_trace'],
         choices=(True, False),
         help="Whether to record a continuous simulation trace",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-end-trace",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_end_trace'],
         choices=(True, False),
         help="Whether to record another trace item at the trip end",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-vehicle-trips",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_vehicle_trips'],
         choices=(True, False),
         help="Whether to record vehicle trips",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-vehicle-emissions",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_vehicle_emissions'],
         choices=(True, False),
         help="Whether to record vehicle emissions",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-vehicle-traces",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_vehicle_traces'],
         choices=(True, False),
         help="Whether to record continuous vehicles traces",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-vehicle-changes",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_vehicle_changes'],
         choices=(True, False),
         help="Whether to record vehicle lane changes",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-emission-traces",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_emission_traces'],
         choices=(True, False),
         help="Whether to record continuous emission traces",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-platoon-trips",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_platoon_trips'],
         choices=(True, False),
         help="Whether to record platoon trips",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-platoon-maneuvers",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_platoon_maneuvers'],
         choices=(True, False),
         help="Whether to record platoon maneuvers",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-platoon-formation",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_platoon_formation'],
         choices=(True, False),
         help="Whether to record platoon formation results",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-platoon-traces",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_platoon_traces'],
         choices=(True, False),
         help="Whether to record continuous platoon traces",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-platoon-changes",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_platoon_changes'],
         choices=(True, False),
         help="Whether to record platoon lane changes",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-infrastructure-assignments",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_infrastructure_assignments'],
         choices=(True, False),
         help="Whether to record infrastructure assignments",
     )
-    results.add_argument(
+    g_results.add_argument(
         "--record-prefilled",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['record_prefilled'],
         choices=(True, False),
         help="Whether to record results for pre-filled vehicles",
     )
 
+    # formation algorithm specific properties
+    ## speed position
+    g_sp = SpeedPosition.add_parser_argument_group(parser)
+    g_help.add_argument(
+        f"--help-{SpeedPosition.__name__}",
+        action='store_true',
+        default=argparse.SUPPRESS,
+        help=f"show help message for {SpeedPosition.__name__} formation algorithm and exit",
+    )
+
     # print usage without any arguments
     if len(sys.argv) < 2:
         # no argument has been passed
         print(
-            parser.description,
-            '\n',
             parser.format_usage(),
-            sep='',
+            parser.description,
+            parser.epilog,
+            sep='\n',
             end='',
         )
-        sys.exit(0)
+        parser.exit()
 
     args = parser.parse_args()
 
+    # simple help
+    misc_groups = parser._action_groups[:2]
+    if 'help' in args and args.help:
+        print(format_help(parser, misc_groups + [g_help]), end='')
+        parser.exit()
+    # complete help
+    elif 'help_all' in args and args.help_all:
+        print(format_help(parser), end='')
+        parser.exit()
+    # road network properties
+    elif 'help_road' in args and args.help_road:
+        print(format_help(parser, misc_groups + [g_road]), end='')
+        parser.exit()
+    # vehicle properties
+    elif 'help_vehicles' in args and args.help_vehicles:
+        print(format_help(parser, misc_groups + [g_vehicles]), end='')
+        parser.exit()
+    # trip properties
+    elif 'help_trips' in args and args.help_trips:
+        print(format_help(parser, misc_groups + [g_trips]), end='')
+        parser.exit()
+    # communication properties
+    elif 'help_communication' in args and args.help_communication:
+        print(format_help(parser, misc_groups + [g_communication]), end='')
+        parser.exit()
+    # platoon properties
+    elif 'help_platoon' in args and args.help_platoon:
+        print(format_help(parser, misc_groups + [g_platoon]), end='')
+        parser.exit()
+    # formation properties
+    elif 'help_formation' in args and args.help_formation:
+        print(format_help(parser, misc_groups + [g_formation]), end='')
+        parser.exit()
+    # infrastructure properties
+    elif 'help_infrastructure' in args and args.help_infrastructure:
+        print(format_help(parser, misc_groups + [g_infrastructure]), end='')
+        parser.exit()
+    # simulation properties
+    elif 'help_simulation' in args and args.help_simulation:
+        print(format_help(parser, misc_groups + [g_simulation]), end='')
+        parser.exit()
+    # GUI properties
+    elif 'help_gui' in args and args.help_gui:
+        print(format_help(parser, misc_groups + [g_gui]), end='')
+        parser.exit()
+    # result recording properties
+    elif 'help_results' in args and args.help_results:
+        print(format_help(parser, misc_groups + [g_results]), end='')
+        parser.exit()
+    elif f'help_{SpeedPosition.__name__}' in args and getattr(args, f'help_{SpeedPosition.__name__}'):
+        print(format_help(parser, misc_groups + [g_sp]), end='')
+        parser.exit()
+
     # transform argument values into correct units
     args.road_length *= 1000  # km -> m
     args.ramp_interval *= 1000  # km -> m
     args.minimum_trip_length *= 1000  # km -> m
     args.maximum_trip_length *= 1000  # km -> m
     args.solver_time_limit *= 1000  # s -> ms
     args.max_step *= 3600  # h -> s
     args.gui_delay /= 1000  # ms -> s
 
-    return args, gui
+    return args, g_gui
 
 
 def load_snapshot(snapshot_filename: str) -> Simulator:
     assert snapshot_filename
 
     with open(snapshot_filename, "rb") as f:
         # load saved state
@@ -652,15 +843,15 @@
     # get argument values (and gui argument group)
     args, gui = parse_args()
 
     if args.default:
         print("Running with default configuration...")
 
     if args.dry_run:
-        print(f"Current configuration:\n{dict(sorted(vars(args).items()))}")
+        print(f"Current configuration:\n{json.dumps(dict(sorted(vars(args).items())),indent=2)}")
         return
 
     simulator = None
     if args.load_snapshot:
         # load snapshot
         simulator = load_snapshot(snapshot_filename=args.load_snapshot)
 
@@ -683,14 +874,15 @@
         # save snapshot
         save_snapshot(simulator, snapshot_filename=args.save_snapshot)
         print(f"Saved a snapshot of the simulation to {args.save_snapshot}. Exiting...")
         return
 
     def handler(signal, frame):
         simulator.stop("SIGINT or CTRL-C detected! Stopping simulation...")
+        exit(1)
 
     signal(SIGINT, handler)
 
     # execute simulation
     start_time = timer()
 
     steps = simulator.run()
```

### Comparing `plafosim-0.16.0/src/plafosim/cli/trace_replay.py` & `plafosim-0.16.1/src/plafosim/cli/trace_replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -108,21 +108,20 @@
         help="The last step to re-play from the trace file. -1 is no limit"
     )
 
     # print usage without any arguments
     if len(sys.argv) < 2:
         # no argument has been passed
         print(
-            parser.description,
-            '\n',
             parser.format_usage(),
-            sep='',
+            parser.description,
+            sep='\n',
             end='',
         )
-        sys.exit(0)
+        parser.exit()
 
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
```

### Comparing `plafosim-0.16.0/src/plafosim/emissions.py` & `plafosim-0.16.1/src/plafosim/emissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/formation_algorithm.py` & `plafosim-0.16.1/src/plafosim/formation_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/gui.py` & `plafosim-0.16.1/src/plafosim/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/infrastructure.py` & `plafosim-0.16.1/src/plafosim/infrastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/mobility.py` & `plafosim-0.16.1/src/plafosim/mobility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/platoon.py` & `plafosim-0.16.1/src/plafosim/platoon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/platoon_role.py` & `plafosim-0.16.1/src/plafosim/platoon_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/platooning_vehicle.py` & `plafosim-0.16.1/src/plafosim/platooning_vehicle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -20,15 +20,14 @@
 import logging
 import math
 import sys
 from typing import TYPE_CHECKING
 
 from .algorithms.speed_position import SpeedPosition  # noqa 401
 from .gui import change_gui_vehicle_color
-from .message import Message, PlatoonAdvertisement
 from .mobility import CF_Model
 from .platoon import Platoon
 from .platoon_role import PlatoonRole
 from .statistics import (
     record_platoon_formation,
     record_platoon_trace,
     record_platoon_trip,
@@ -489,17 +488,14 @@
                 self._join_data_leader._joiner = None
                 self._join_data_leader = None
                 self._join_data_last = None
                 self._join_data_new_position = None
 
         # do platoon formation
         if self._formation_algorithm:
-            # transmit regular platoon advertisements
-            self._advertise()
-
             # execute formation algorithm at every execution interval
             if step >= self._last_formation_step + self._execution_interval:
                 # search for a platoon (depending on the algorithm)
                 self._formation_algorithm.do_formation()
                 self._last_formation_step = step
 
     def info(self) -> str:
@@ -1226,84 +1222,7 @@
             leader.in_maneuver = False
 
         assert self._last_platoon_join_time >= 0
         self._time_in_platoon += self._simulator.step - self._last_platoon_join_time
         assert self._last_platoon_join_position >= 0
         self._distance_in_platoon += self._position - self._last_platoon_join_position
         self._leaves_successful += 1
-
-    def _advertise(self):
-        """
-        Maintains regular sending of platoon advertisements.
-
-        Advertisement are in general not used at the moment.
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        return  # TODO this is not necessary as a perfect communication guarantees information
-
-        advertisement_interval = 600  # in s # TODO make parameter
-        if (
-            not self._last_advertisement_step
-            or self._last_advertisement_step + advertisement_interval <= self._simulator.step
-        ):
-            self._send_advertisements()
-            self._last_advertisement_step = self._simulator.step
-
-    def _send_advertisements(self):
-        """
-        Transmit a broadcast to advertise as platoon.
-
-        Advertisement are in general not used at the moment.
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        for vehicle in self._simulator._vehicles.values():
-            self._transmit(-1, PlatoonAdvertisement(
-                self._vid,
-                vehicle.vid,
-                self._vid,
-                self._vid,
-                self._speed,
-                self._lane,
-                self._vid,
-                self._position,
-                self.rear_position,
-            ))
-
-    def _handle_message(self, message: Message):
-        """
-        Handle a message of arbitrary type Message.
-
-        Messages are in general not used at the moment.
-
-        Parameters
-        ----------
-        message : Message
-            The message to be handled
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        func = self.__class__.__dict__.get(
-            '_receive_' + message.__class__.__name__,
-            super().__dict__.get('_handle_message'))
-        return func(self, message)
-
-    def _receive_PlatoonAdvertisement(self, advertisement: PlatoonAdvertisement):
-        """
-        Handle a message of the specific type PlatoonAdvertisement.
-
-        Messages are in general not used at the moment.
-
-        Parameters
-        ----------
-        advertisement : PlatoonAdvertisement
-            The advertisement to be received
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        # TODO add contents to the neighbor table
-        LOG.debug(f"{self._vid} received an advertisement from {advertisement.origin}")
```

### Comparing `plafosim-0.16.0/src/plafosim/simulator.py` & `plafosim-0.16.1/src/plafosim/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/spawning.py` & `plafosim-0.16.1/src/plafosim/spawning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/statistics.py` & `plafosim-0.16.1/src/plafosim/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.gui.xml` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.gui.xml`

 * *Files 0% similar despite different names*

#### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.gui.xml` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.gui.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 
 SPDX-License-Identifier: GPL-3.0-or-later
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.net.xml` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.net.xml`

 * *Files 1% similar despite different names*

#### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.net.xml` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.net.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 
 SPDX-License-Identifier: GPL-3.0-or-later
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.rou.xml` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.rou.xml`

 * *Files 1% similar despite different names*

#### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.rou.xml` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.rou.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 
 SPDX-License-Identifier: GPL-3.0-or-later
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.sumo.cfg` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.sumo.cfg`

 * *Files 0% similar despite different names*

#### Comparing `plafosim-0.16.0/src/plafosim/sumocfg/freeway.sumo.cfg` & `plafosim-0.16.1/src/plafosim/sumocfg/freeway.sumo.cfg`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 
 SPDX-License-Identifier: GPL-3.0-or-later
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
```

### Comparing `plafosim-0.16.0/src/plafosim/util.py` & `plafosim-0.16.1/src/plafosim/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -132,21 +132,21 @@
     """
 
     return (speed_to - speed_from) / time_interval
 
 
 def addLoggingLevel(levelName, levelNum, methodName=None):
     """
-    https://stackoverflow.com/a/35804945.
-
     Comprehensively adds a new logging level to the `logging` module and the currently configured logging class.
 
     `levelName` becomes an attribute of the `logging` module with the value `levelNum`. `methodName` becomes a convenience method for both `logging` itself and the class returned by `logging.getLoggerClass()` (usually just `logging.Logger`). If `methodName` is not specified, `levelName.lower()` is used.
 
-    To avoid accidental clobberings of existing attributes, this method will raise an `AttributeError` if the level name is already an attribute of the `logging` module or if the method name is already present
+    To avoid accidental clobberings of existing attributes, this method will raise an `AttributeError` if the level name is already an attribute of the `logging` module or if the method name is already present.
+
+    Taken from https://stackoverflow.com/a/35804945.
     """
 
     if not methodName:
         methodName = levelName.lower()
 
     if hasattr(logging, levelName):
         raise AttributeError('{} already defined in logging module'.format(levelName))
```

### Comparing `plafosim-0.16.0/src/plafosim/vehicle.py` & `plafosim-0.16.1/src/plafosim/vehicle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 import logging
 from typing import TYPE_CHECKING
 
-from .message import Message
 from .mobility import CF_Model
 from .statistics import (
     record_emission_trace_prefix,
     record_emission_trace_suffix,
     record_emission_trace_value,
     record_vehicle_emission,
     record_vehicle_trace,
@@ -575,98 +574,7 @@
         """
         Return the str representation of the vehicle.
         """
 
         self_dict = self.__dict__.copy()
         self_dict.update({'_vehicle_type': str(self._vehicle_type)})  # use str representation of vehicle type
         return str(self_dict)
-
-    def _transmit(self, destination_vid: int, message: Message) -> bool:
-        """
-        Transmit a message of type Message.
-
-        Messages are in general not used at the moment.
-
-        Parameters
-        ----------
-        destination_vid : int
-            The id of the destination vehicle
-        message : Message
-            The message to transmit
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        if isinstance(message, Message):
-            if destination_vid == -1:
-                # TODO do we really want access the private field of the vehicles here (i.e., within this class)?
-                for vehicle in self._simulator._vehicles.values():
-                    vehicle.receive(message)
-            else:
-                # TODO do we really want access the private field of the vehicles here (i.e., within this class)?
-                self._simulator._vehicles[destination_vid].receive(message)
-
-            return True  # this should always be true, at least currently
-        raise RuntimeError("Message is not an instance of type Message")
-
-    def receive(self, message) -> bool:
-        """
-        Receives a message of arbitrary type.
-
-        Messages are in general not used at the moment.
-
-        Parameters
-        ----------
-        message :
-            The message to be received
-
-        Raises
-        ------
-        RuntimeError
-            If the message to be received is not an instance of the Message type.
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        if self._simulator.step < self._depart_time:
-            # we cannot receive anything since we did not start yet
-            return False
-        if isinstance(message, Message):
-            if message.destination == self._vid or message.destination == -1:
-                self._handle_message(message)
-            # we cannot receive this message since it was not for us
-            return False
-        raise RuntimeError("Message is not an instance of type Message")
-
-    def _handle_message(self, message: Message):
-        """
-        Handle a message of arbitrary type Message.
-
-        Messages are in general not used at the moment.
-
-        Parameters
-        ----------
-        message : Message
-            The message to be handled
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        func = self.__class__.__dict__.get('_receive_' + message.__class__.__name__,
-                                           lambda v, m: print("cannot handle message", m))
-        return func(self, message)
-
-    def _receive_Message(self, message: Message):
-        """
-        Handle a message of the specific type Message.
-
-        Messages are in general not used at the moment.
-
-        Parameters
-        ----------
-        message : Message
-            The message to be received
-
-        THIS IS DEPRECATED AT THE MOMENT!!!
-        """
-
-        LOG.warning(f"{self._vid} received non-sense message {message}")
```

### Comparing `plafosim-0.16.0/src/plafosim/vehicle_type.py` & `plafosim-0.16.1/src/plafosim/vehicle_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

### Comparing `plafosim-0.16.0/setup.py` & `plafosim-0.16.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['plafosim = plafosim.cli.plafosim:main',
                      'plafosim-replay = plafosim.cli.trace_replay:main']}
 
 setup_kwargs = {
     'name': 'plafosim',
-    'version': '0.16.0',
+    'version': '0.16.1',
     'description': 'A simple and scalable simulator for platoon formation.',
-    'long_description': '# Platoon Formation Simulator (PlaFoSim)\n\n[![Code Version](https://img.shields.io/badge/code-v0.16.0-blue)](CHANGELOG.md)\n[![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)\n[![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)\n[![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)\n\n[PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.\n\nPlaFoSim aims to facilitate and accelerate the research of platoon maneuvers and formation for individually driven vehicles.\nWhile the main focus of the simulator is on the assignment process, simulation of advertisements and maneuvers is implemented in a more abstract way.\n\nConceptual view on the process of Platoon Formation [1-2]:\n| Scenario | Advertisement | Assignment | Maneuver |\n| -------- | ------------- | ---------- | -------- |\n| ![Scenario](docs/scenario.png)*A new vehicle enters the highway.* | ![Advertisement](docs/advertisement.png)*The vehicle advertises itself as interested in Platooning.* | ![Assignment](docs/assignment.png)*A Vehicle-to-Platoon assignment is calculated.* | ![Maneuver](docs/maneuver.png)*The new vehicle performs a join maneuver.* |\n\nPlaFoSim is published [here](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.\n\nPlease note that PlaFoSim is still under heavy development.\n\n---\n\n## Installation\n\n- Install Python (>=3.7.0,<3.10)\n- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)\n- Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):\n```pip install plafosim```\n\nNOTE: The project is currently only tested under Linux.\n\n## Running a Simulation\n\nYou can use the simulator as module as well as from the command-line.\nCurrently, only command-line is thoroughly tested and thus completely available though.\n\n### Quickstart\n\nUse PlaFoSim\'s binary to run a simulation with the default configuration:\n\n```plafosim -d```\n\n### Advanced Simulation Control\n\nYou can use a variety of different parameters to customize the scenario and the simulation itself.\nE.g., use the parameter `vehicles` to configure the number of vehicles in the simulation:\n\n```plafosim --vehicles 1000```\n\nThe available parameters are grouped into different categories:\n\n```\n- road network properties\n- vehicle properties\n- trip properties\n- communication properties\n- platoon properties\n- formation properties\n- infrastructure properties\n- simulation properties\n- GUI properties\n- result recording properties\n```\n\nYou can see the complete list of available parameters in the help:\n\n```plafosim -h, --help```\n\n### Examples\n\n```\n# Configure a 100km freeway with ramps at every 10km\nplafosim --road-length 100 --ramp-interval 10\n\n# Configure random (normally distributed) desired driving speed of 130km/h\nplafosim --random-desired-speed true --desired-speed 36\n\n# Configure random trips for 500 vehicles\nplafosim --vehicles 500 --random-depart-position true --random-arrival-position true --depart-desired true\n\n# Pre fill the freeway with 1000 vehicles\nplafosim --vehicles 1000 --pre-fill true\n\n# Configure 50% of the vehicles with Advanced Cruise Control (ACC) and a headway time of 1.5s\nplafosim --penetration 0.5 --acc-headway-time 1.5\n\n# Enable a simple, distributed platoon formation algorithm [1] in order to form platoons every 30s\nplafosim --formation-algorithm SpeedPosition --formation-strategy distributed --execution-interval 30\n```\n\n### Live GUI\n\nYou can get a very simple live GUI based on SUMO by using the parameter `gui` (requires installation of SUMO and decleration of `SUMO_HOME` variable):\n\n```plafosim --gui```\n\n![](docs/gui.png)\n*A screenshot of PlaFoSim\'s live GUI showing 2 platoons and various individual vehicles. Copyright © 2021 IEEE.*\n\nMore options for the live GUI can be found within the ``gui properties`` section of the help.\n\n### Faster Simulation\n\nYou can speed up the simulation performance by enabling Python\'s optimization ```PYTHONOPTIMIZE```, e.g., in order to disable assertions:\n\n```PYTHONOPTIMIZE=1 plafosim```\n\nSee the Python [documention](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE) for more details.\n\n## Re-Playing a Simulation\n\nThe simulation can write a trace file for every simulated vehicle (default `results_vehicle_traces.csv`).\nYou can replay the simulation based on the trace file by using a corresponding binary:\n\n```plafosim-replay results_vehicle_traces.csv```\n\nTo see all options of this script, run:\n\n```plafosim-replay -h, --help```\n\n## Extending\n\n- Clone the repository\n- Install [poetry](https://python-poetry.org/):\n```pip install poetry```\n- Install PlaFoSim from source in editable mode:\n```poetry install```\n- Run PlaFoSim in the virtual environment with\n```poetry run plafosim```\nor activate the virtual enviroment first with\n```poetry shell```\nand run the commands as usual (see above)\n\nNOTE: The project is currently only tested under Linux.\n\nIn order to add a new formation algorithm, you need to follow these steps:\n- Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.\n- Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.\n- Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.\n- Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).\n\nYou should now be able to use your new algorithm with\n```\nplafosim --formation-algorithm dummy_algorithm_name\n```\n\n## Contributing\n\nIn order to contribute, please follow these steps:\n- Install PlaFoSim from source (see above)\n- Make desired changes\n- Run the tests located in `scripts` (see `.drone.yml`)\n- Submit a Pull Request (PR)\n\n### Testing\n\nWhen adding methods and functions, make sure to add corresponding unit tests for `py.test`.\nThe tests are located under `tests` and can be executed with `./scripts/run-pytest.sh`.\nThis will also generate a test coverage report.\n\n### Validation\n\nTo validate the behavior of PlaFoSim, it is compared to SUMO 1.6.0 by means of simulation results (e.g., vehicle traces).\nThe corresponding scripts are located under `scripts` and executed withn CI/CD pipelines.\nYou can have a look at `.drone.yml` for details regarding the execution.\n\n### Profiling\n\nYou can profile the runtime of PlaFoSim\'s code by using [cProfile](https://docs.python.org/3/library/profile.html#module-cProfile):\n\n```poetry run python -m cProfile -o profile.out -m plafosim.cli.plafosim```\n\nYou can visualize the results of the profiling run by using [SnakeViz](https://docs.python.org/3/library/profile.html#module-cProfile):\n\n```snakeviz profile.out```\n\n## Contributors & Citing\n\nPlaFoSim was designed and built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).\nIt is currently maintained by [Julian Heinovski](https://github.com/heinovski/).\nThe list of all authors can be found [here](AUTHORS.md).\n\nIf you are working with `PlaFoSim`, please cite the [following paper](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.\n\n```bibtex\n@inproceedings{heinovski2021scalable,\n    author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},\n    doi = {10.1109/VNC52810.2021.9644678},\n    title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},\n    pages = {137--138},\n    publisher = {IEEE},\n    issn = {2157-9865},\n    isbn = {978-1-66544-450-7},\n    address = {Virtual Conference},\n    booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},\n    month = {11},\n    year = {2021},\n}\n```\n\n## License\n\nPlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.\n\n```\n# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>\n#\n# SPDX-License-Identifier: GPL-3.0-or-later\n#\n# This program is free software: you can redistribute it and/or modify\n# it under the terms of the GNU General Public License as published by\n# the Free Software Foundation, either version 3 of the License, or\n# any later version.\n#\n# This program is distributed in the hope that it will be useful,\n# but WITHOUT ANY WARRANTY; without even the implied warranty of\n# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\n# GNU General Public License for more details.\n#\n# You should have received a copy of the GNU General Public License\n# along with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\n## List of References\n\n[1] Julian Heinovski and Falko Dressler, ["Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols,"](https://www.tkn.tu-berlin.de/bib/heinovski2018platoon/) Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.\n\n[2] Julian Heinovski, ["Platoon Formation: Car-to-Platoon Assignments for Individual Cars,"](https://www.tkn.tu-berlin.de/bib/heinovski2019platoon/) Proceedings of International Conference on Networked Systems (NetSys 2019), PhD Forum, Munich, Germany, March 2019.\n',
+    'long_description': '# Platoon Formation Simulator (PlaFoSim)\n\n[![Code Version](https://img.shields.io/badge/code-v0.16.1-blue)](CHANGELOG.md)\n[![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)\n[![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)\n[![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)\n\n[PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.\n\nPlaFoSim aims to facilitate and accelerate the research of platoon maneuvers and formation for individually driven vehicles.\nWhile the main focus of the simulator is on the assignment process, simulation of advertisements and maneuvers is implemented in a more abstract way.\n\nConceptual view on the process of Platoon Formation [1-2]:\n| Scenario | Advertisement | Assignment | Maneuver |\n| -------- | ------------- | ---------- | -------- |\n| ![Scenario](docs/scenario.png)*A new vehicle enters the highway.* | ![Advertisement](docs/advertisement.png)*The vehicle advertises itself as interested in Platooning.* | ![Assignment](docs/assignment.png)*A Vehicle-to-Platoon assignment is calculated.* | ![Maneuver](docs/maneuver.png)*The new vehicle performs a join maneuver.* |\n\nPlaFoSim is published [here](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.\n\nPlease note that PlaFoSim is still under heavy development.\n\n---\n\n## Installation\n\n- Install Python (>=3.7,<=3.9)\n- Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):\n```pip install plafosim```\n- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)\n\nNOTE: The project is developed and currently only tested on Linux.\n\n## Running a Simulation\n\nYou can use the PlaFoSim as Python module as well as from the command-line.\nCurrently, only command-line is thoroughly tested and thus completely available though.\n\n### Quickstart\n\nUse PlaFoSim\'s binary to run a simulation with the default configuration (`-d`):\n\n```plafosim -d```\n\n### Advanced Simulation Control\n\nYou can use a variety of different parameters to customize the scenario and the simulation itself.\nE.g., use the parameter `vehicles` to configure the number of vehicles in the simulation:\n\n```plafosim --vehicles 1000```\n\nThe available parameters are grouped into different categories:\n\n```\n- road network properties\n- vehicle properties\n- trip properties\n- communication properties\n- platoon properties\n- formation properties\n- infrastructure properties\n- simulation properties\n- GUI properties\n- result recording properties\n```\n\nYou can see the complete list of available parameters in the help:\n\n```plafosim -h, --help```\n\n### Examples\n\n```\n# Configure a 100km freeway with ramps at every 10km\nplafosim --road-length 100 --ramp-interval 10\n\n# Configure random (normally distributed) desired driving speed of 130km/h\nplafosim --random-desired-speed true --desired-speed 36\n\n# Configure random trips for 500 vehicles\nplafosim --vehicles 500 --random-depart-position true --random-arrival-position true --depart-desired true\n\n# Pre fill the freeway with 1000 vehicles\nplafosim --vehicles 1000 --pre-fill true\n\n# Configure 50% of the vehicles with Advanced Cruise Control (ACC) and a headway time of 1.5s\nplafosim --penetration 0.5 --acc-headway-time 1.5\n\n# Enable a simple, distributed platoon formation algorithm [1] in order to form platoons every 30s\nplafosim --formation-algorithm SpeedPosition --formation-strategy distributed --execution-interval 30\n```\n\n### Live GUI\n\nYou can get a very simple live GUI based on SUMO by using the parameter `gui` (requires installation of SUMO and decleration of `SUMO_HOME` variable):\n\n```plafosim --gui```\n\n![](docs/gui.png)\n*A screenshot of PlaFoSim\'s live GUI showing 2 platoons and various individual vehicles. Copyright © 2021 IEEE.*\n\nMore options for the live GUI can be found within the ``gui properties`` section of the help.\n\n### Faster Simulation\n\nYou can speed up the simulation performance by enabling Python\'s optimization ```PYTHONOPTIMIZE```, e.g., in order to disable assertions:\n\n```PYTHONOPTIMIZE=1 plafosim```\n\nSee the Python [documention](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE) for more details.\n\n## Re-Playing a Simulation\n\nThe simulation can write a trace file including the mobility details of every simulated vehicle (default `results_vehicle_traces.csv`).\nYou can replay the simulation in the GUI (see above) based on the trace file by using the corresponding binary:\n\n```plafosim-replay results_vehicle_traces.csv```\n\nTo see all options of this script, run:\n\n```plafosim-replay -h, --help```\n\n## Extending the Simulator\n\n- Install [poetry](https://python-poetry.org/):\n```pip install poetry```\n- Clone the repository\n- Install PlaFoSim from source in editable mode:\n```poetry install```\n- Run PlaFoSim in the virtual environment with\n```poetry run plafosim```\nor activate the virtual enviroment first with\n```poetry shell```\nand run the commands as usual (see above)\n\nNOTE: The project is currently only tested under Linux.\n\nIn order to add a new formation algorithm, you need to follow these steps:\n- Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.\n- Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.\n- Add specific properties of your algorithm via an argument parser group and a corresponding help message to `cli/plafosim.py` if necessary.\n- Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).\n\nYou should now be able to use your new algorithm with\n```\nplafosim --formation-algorithm dummy_algorithm_name\n```\n\n## Contributing to the Project\n\nIn order to contribute, please follow these steps:\n- Install PlaFoSim from source (see above)\n- Make desired changes\n- Run the tests located in `tests` as well as the validation scripts located in `scripts` (see `.drone.yml` for details)\n- Submit a Pull Request (PR)\n\n### Testing\n\nWhen adding methods and functions, make sure to add corresponding unit tests for `py.test`.\nThe tests are located under `tests` and can be executed with `./scripts/run-pytest.sh`.\nThis will also generate a test coverage report.\n\n### Validation\n\nTo validate the behavior of PlaFoSim, it is compared to SUMO 1.6.0 by means of simulation results (e.g., vehicle traces).\nThe corresponding scripts are located under `scripts` and executed withn CI/CD pipelines.\nYou can have a look at `.drone.yml` for details regarding the execution.\n\n### Profiling\n\nYou can profile the runtime of PlaFoSim\'s code by using [cProfile](https://docs.python.org/3/library/profile.html#module-cProfile):\n\n```poetry run python -m cProfile -o profile.out -m plafosim.cli.plafosim```\n\nYou can visualize the results of the profiling run by using [SnakeViz](https://docs.python.org/3/library/profile.html#module-cProfile):\n\n```snakeviz profile.out```\n\n## Contributors & Citing\n\nPlaFoSim was designed and built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).\nIt is currently maintained by [Julian Heinovski](https://github.com/heinovski/).\nThe list of all authors can be found [here](AUTHORS.md).\n\nIf you are working with `PlaFoSim`, please cite the [following paper](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.\n\n```bibtex\n@inproceedings{heinovski2021scalable,\n    author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},\n    doi = {10.1109/VNC52810.2021.9644678},\n    title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},\n    pages = {137--138},\n    publisher = {IEEE},\n    issn = {2157-9865},\n    isbn = {978-1-66544-450-7},\n    address = {Virtual Conference},\n    booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},\n    month = {11},\n    year = {2021},\n}\n```\n\n## License\n\nPlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.\n\n```\n# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>\n#\n# SPDX-License-Identifier: GPL-3.0-or-later\n#\n# This program is free software: you can redistribute it and/or modify\n# it under the terms of the GNU General Public License as published by\n# the Free Software Foundation, either version 3 of the License, or\n# any later version.\n#\n# This program is distributed in the hope that it will be useful,\n# but WITHOUT ANY WARRANTY; without even the implied warranty of\n# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\n# GNU General Public License for more details.\n#\n# You should have received a copy of the GNU General Public License\n# along with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\n## List of References\n\n[1] Julian Heinovski and Falko Dressler, ["Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols,"](https://www.tkn.tu-berlin.de/bib/heinovski2018platoon/) Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.\n\n[2] Julian Heinovski, ["Platoon Formation: Car-to-Platoon Assignments for Individual Cars,"](https://www.tkn.tu-berlin.de/bib/heinovski2019platoon/) Proceedings of International Conference on Networked Systems (NetSys 2019), PhD Forum, Munich, Germany, March 2019.\n',
     'author': 'Julian Heinovski',
     'author_email': 'heinovski@ccs-labs.org',
     'maintainer': 'Julian Heinovski',
     'maintainer_email': 'heinovski@ccs-labs.org',
     'url': 'https://www.plafosim.de',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `plafosim-0.16.0/PKG-INFO` & `plafosim-0.16.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plafosim
-Version: 0.16.0
+Version: 0.16.1
 Summary: A simple and scalable simulator for platoon formation.
 Home-page: https://www.plafosim.de
 License: GPL-3.0-or-later
 Author: Julian Heinovski
 Author-email: heinovski@ccs-labs.org
 Maintainer: Julian Heinovski
 Maintainer-email: heinovski@ccs-labs.org
@@ -25,15 +25,15 @@
 Project-URL: Changelog, https://github.com/heinovski/plafosim/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://plafosim.readthedocs.io/
 Project-URL: Repository, https://github.com/heinovski/plafosim
 Description-Content-Type: text/markdown
 
 # Platoon Formation Simulator (PlaFoSim)
 
-[![Code Version](https://img.shields.io/badge/code-v0.16.0-blue)](CHANGELOG.md)
+[![Code Version](https://img.shields.io/badge/code-v0.16.1-blue)](CHANGELOG.md)
 [![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)
 [![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)
 [![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)
 
 [PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.
 
@@ -51,29 +51,29 @@
 
 Please note that PlaFoSim is still under heavy development.
 
 ---
 
 ## Installation
 
-- Install Python (>=3.7.0,<3.10)
-- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)
+- Install Python (>=3.7,<=3.9)
 - Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):
 ```pip install plafosim```
+- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)
 
-NOTE: The project is currently only tested under Linux.
+NOTE: The project is developed and currently only tested on Linux.
 
 ## Running a Simulation
 
-You can use the simulator as module as well as from the command-line.
+You can use the PlaFoSim as Python module as well as from the command-line.
 Currently, only command-line is thoroughly tested and thus completely available though.
 
 ### Quickstart
 
-Use PlaFoSim's binary to run a simulation with the default configuration:
+Use PlaFoSim's binary to run a simulation with the default configuration (`-d`):
 
 ```plafosim -d```
 
 ### Advanced Simulation Control
 
 You can use a variety of different parameters to customize the scenario and the simulation itself.
 E.g., use the parameter `vehicles` to configure the number of vehicles in the simulation:
@@ -138,55 +138,55 @@
 
 ```PYTHONOPTIMIZE=1 plafosim```
 
 See the Python [documention](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE) for more details.
 
 ## Re-Playing a Simulation
 
-The simulation can write a trace file for every simulated vehicle (default `results_vehicle_traces.csv`).
-You can replay the simulation based on the trace file by using a corresponding binary:
+The simulation can write a trace file including the mobility details of every simulated vehicle (default `results_vehicle_traces.csv`).
+You can replay the simulation in the GUI (see above) based on the trace file by using the corresponding binary:
 
 ```plafosim-replay results_vehicle_traces.csv```
 
 To see all options of this script, run:
 
 ```plafosim-replay -h, --help```
 
-## Extending
+## Extending the Simulator
 
-- Clone the repository
 - Install [poetry](https://python-poetry.org/):
 ```pip install poetry```
+- Clone the repository
 - Install PlaFoSim from source in editable mode:
 ```poetry install```
 - Run PlaFoSim in the virtual environment with
 ```poetry run plafosim```
 or activate the virtual enviroment first with
 ```poetry shell```
 and run the commands as usual (see above)
 
 NOTE: The project is currently only tested under Linux.
 
 In order to add a new formation algorithm, you need to follow these steps:
 - Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.
 - Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.
-- Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.
+- Add specific properties of your algorithm via an argument parser group and a corresponding help message to `cli/plafosim.py` if necessary.
 - Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).
 
 You should now be able to use your new algorithm with
 ```
 plafosim --formation-algorithm dummy_algorithm_name
 ```
 
-## Contributing
+## Contributing to the Project
 
 In order to contribute, please follow these steps:
 - Install PlaFoSim from source (see above)
 - Make desired changes
-- Run the tests located in `scripts` (see `.drone.yml`)
+- Run the tests located in `tests` as well as the validation scripts located in `scripts` (see `.drone.yml` for details)
 - Submit a Pull Request (PR)
 
 ### Testing
 
 When adding methods and functions, make sure to add corresponding unit tests for `py.test`.
 The tests are located under `tests` and can be executed with `./scripts/run-pytest.sh`.
 This will also generate a test coverage report.
@@ -234,15 +234,15 @@
 ```
 
 ## License
 
 PlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.
 
 ```
-# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+# Copyright (c) 2020-2023 Julian Heinovski <heinovski@ccs-labs.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
```

