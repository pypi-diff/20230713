# Comparing `tmp/homeassistant-historical-sensor-1.0.1.tar.gz` & `tmp/homeassistant-historical-sensor-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-1.0.1.tar", last modified: Wed Jun 21 15:14:42 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-2.0.0b0.tar", last modified: Thu Jul 13 17:04:54 2023, max compression
```

## Comparing `homeassistant-historical-sensor-1.0.1.tar` & `homeassistant-historical-sensor-2.0.0b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/recorderutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/recorderutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 17:04:54.000000 homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 17:04:42.000000 homeassistant-historical-sensor-2.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-13 17:04:54.034500 homeassistant-historical-sensor-2.0.0b0/setup.cfg
```

### Comparing `homeassistant-historical-sensor-1.0.1/PKG-INFO` & `homeassistant-historical-sensor-2.0.0b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 1.0.1
+Version: 2.0.0b0
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 #  Historical sensors for Home Assistant ![](icon-64.png)
 
 <!-- Code and releases -->
 ![GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/ldotlopez/ha-historical-sensor?include_prereleases)
 [![CodeQL](https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-analysis.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <!-- Sponsors -->
 <a href="https://www.buymeacoffee.com/zepolson" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 105px !important;" ></a>
 
-Feed historical data into Home Assistant database. 
+Feed historical data into Home Assistant database.
 
 HomeAssistant architecture is built around polling (or pushing) data from devices, or data providers, in "real-time". Some data sources (e.g, energy, water or gas providers) can't be polled in real-time or readings are not accurate. However reading historical data, like last month consumption, it's possible and accurate. This module adds support to this.
 
 This module uses the `recoder` component and custom state creation to store states "from the past".
 
 Current projects using this module:
 
@@ -32,15 +32,15 @@
 
 
 ## Technical details
 
 Q. How it's accomplished?.
 
 A. It's a relatively easy answer but needs to be broken into some pieces:
-  
+
   1. A new property for sensors: `historical_states`. This property holds a list of `HistoricalState`s which are, basically, a `state`+`datetime`  (with tzinfo), so… the data we want.
 
   2. A new hook for sensor: `async_update_historical_states`. This method is responsible to update `historical_states` property.  
      **This is the only function that needs to be implemented**.
 
   3. A new method, implemented by HistoricalSensor class: `async_write_ha_historical_states`. This method handles the details of creating tweaked states in the past and write them into the database using the `recorder` component of Home Assistant core.
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.1
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0b0
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
-historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
-markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
-Release (latest SemVer including pre-releases)](https://img.shields.io/github/
-v/release/ldotlopez/ha-historical-sensor?include_prereleases) [![CodeQL](https:
-//github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-
+historical-sensor/issues Requires-Python: >=3.10 Description-Content-Type:
+text/markdown # Historical sensors for Home Assistant ![](icon-64.png)  !
+[GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/
+github/v/release/ldotlopez/ha-historical-sensor?include_prereleases) [![CodeQL]
+(https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-
 analysis.yml/badge.svg)](https://github.com/ldotlopez/ha-historical-sensor/
 actions/workflows/codeql-analysis.yml) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black)  [Buy_Me_A_Coffee] Feed historical data into Home Assistant database.
 HomeAssistant architecture is built around polling (or pushing) data from
 devices, or data providers, in "real-time". Some data sources (e.g, energy,
 water or gas providers) can't be polled in real-time or readings are not
```

### Comparing `homeassistant-historical-sensor-1.0.1/README.md` & `homeassistant-historical-sensor-2.0.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/ldotlopez/ha-historical-sensor?include_prereleases)
 [![CodeQL](https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-analysis.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <!-- Sponsors -->
 <a href="https://www.buymeacoffee.com/zepolson" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 105px !important;" ></a>
 
-Feed historical data into Home Assistant database. 
+Feed historical data into Home Assistant database.
 
 HomeAssistant architecture is built around polling (or pushing) data from devices, or data providers, in "real-time". Some data sources (e.g, energy, water or gas providers) can't be polled in real-time or readings are not accurate. However reading historical data, like last month consumption, it's possible and accurate. This module adds support to this.
 
 This module uses the `recoder` component and custom state creation to store states "from the past".
 
 Current projects using this module:
 
@@ -20,15 +20,15 @@
 
 
 ## Technical details
 
 Q. How it's accomplished?.
 
 A. It's a relatively easy answer but needs to be broken into some pieces:
-  
+
   1. A new property for sensors: `historical_states`. This property holds a list of `HistoricalState`s which are, basically, a `state`+`datetime`  (with tzinfo), so… the data we want.
 
   2. A new hook for sensor: `async_update_historical_states`. This method is responsible to update `historical_states` property.  
      **This is the only function that needs to be implemented**.
 
   3. A new method, implemented by HistoricalSensor class: `async_write_ha_historical_states`. This method handles the details of creating tweaked states in the past and write them into the database using the `recorder` component of Home Assistant core.
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2021-2023 Luis López <luis@cuarentaydos.com>
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
@@ -16,23 +14,20 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
 import logging
 
-from homeassistant.const import (
-    MAJOR_VERSION,
-    MINOR_VERSION,
-    __version__ as HA_FULL_VERSION,
-)
+from homeassistant.const import MAJOR_VERSION, MINOR_VERSION
+from homeassistant.const import __version__ as HA_FULL_VERSION
 
+from .consts import MIN_REQ_MAJOR_VERSION, MIN_REQ_MINOR_VERSION
 from .sensor import HistoricalSensor, PollUpdateMixin
 from .state import HistoricalState
-from .consts import MIN_REQ_MAJOR_VERSION, MIN_REQ_MINOR_VERSION
 
 LOGGER = logging.getLogger(__name__)
 
 if not (
     (MAJOR_VERSION >= MIN_REQ_MAJOR_VERSION)
     and (MINOR_VERSION >= MIN_REQ_MINOR_VERSION)
 ):
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/consts.py` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/consts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2021-2023 Luis López <luis@cuarentaydos.com>
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2021-2023 Luis López <luis@cuarentaydos.com>
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
@@ -16,15 +14,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
 import math
 import sys
-from typing import Any, Dict
+from typing import Any
 
 from homeassistant.config import DATA_CUSTOMIZE
 from homeassistant.const import (
     ATTR_ASSUMED_STATE,
     ATTR_ATTRIBUTION,
     ATTR_DEVICE_CLASS,
     ATTR_ENTITY_PICTURE,
@@ -33,15 +31,14 @@
     ATTR_SUPPORTED_FEATURES,
     ATTR_UNIT_OF_MEASUREMENT,
     STATE_UNAVAILABLE,
     STATE_UNKNOWN,
     TEMP_CELSIUS,
     TEMP_FAHRENHEIT,
 )
-
 from homeassistant.helpers.entity import Entity
 
 FLOAT_PRECISION = abs(int(math.floor(math.log10(abs(sys.float_info.epsilon))))) - 1
 
 
 # Modified version of
 # homeassistant.helpers.entity.Entity._stringify_state
@@ -62,15 +59,15 @@
 
 
 # Code extracted and modified from
 # homeassistant.helpers.entity.Entity._async_write_ha_state
 # https://github.com/home-assistant/core/blob/dev/homeassistant/helpers/entity.py
 
 
-def _build_attributes(self: Entity, state: Any) -> Dict[str, str]:
+def _build_attributes(self: Entity, state: Any) -> dict[str, str]:
     attr = self.capability_attributes
     attr = dict(attr) if attr else {}
 
     state = _stringify_state(self, state)
     if self.available:
         attr.update(self.state_attributes or {})
         extra_state_attributes = self.extra_state_attributes
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/recorderutil.py` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/recorderutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2021-2023 Luis López <luis@cuarentaydos.com>
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
@@ -16,15 +14,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
 import logging
 from contextlib import contextmanager
-from typing import List, Optional
+from typing import Literal
 
 from homeassistant.components import recorder
 from homeassistant.components.recorder import db_schema
 from homeassistant.components.recorder.statistics import (
     StatisticsRow,
     get_last_statistics,
 )
@@ -41,23 +39,34 @@
 def hass_recorder_session(hass: HomeAssistant):
     r = recorder.get_instance(hass)
     with recorder.util.session_scope(session=r.get_session()) as session:
         yield session
 
 
 async def get_last_statistics_wrapper(
-    hass: HomeAssistant, statistic_id: str
-) -> Optional[StatisticsRow]:
+    hass: HomeAssistant,
+    statistic_id: str,
+    *,
+    convert_units: bool = True,
+    types: set[Literal["last_reset", "max", "mean", "min", "state", "sum"]] = {
+        "last_reset",
+        "max",
+        "mean",
+        "min",
+        "state",
+        "sum",
+    },
+) -> StatisticsRow | None:
     res = await recorder.get_instance(hass).async_add_executor_job(
         get_last_statistics,
         hass,
         1,
         statistic_id,
-        True,
-        set(["last_reset", "max", "mean", "min", "state", "sum"]),
+        convert_units,
+        types,
     )
     if not res:
         return None
 
     return res[statistic_id][0]
 
 
@@ -129,10 +138,10 @@
             )
         )
         .order_by(db_schema.States.last_updated_ts.desc())
     )
     return session.execute(stmt).scalar()
 
 
-def save_states(session: Session, states: List[db_schema.States]):
+def save_states(session: Session, states: list[db_schema.States]):
     session.add_all(states)
     session.commit()
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2021-2023 Luis López <luis@cuarentaydos.com>
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
@@ -17,15 +15,14 @@
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
 import logging
 from abc import abstractmethod
 from datetime import timedelta
-from typing import List, Optional
 
 import sqlalchemy.exc
 import sqlalchemy.orm
 from homeassistant.components import recorder
 from homeassistant.components.recorder import db_schema
 from homeassistant.components.recorder.models import StatisticData, StatisticMetaData
 from homeassistant.components.recorder.statistics import (
@@ -69,15 +66,32 @@
     Sensors based on HistoricalSensor must provide:
     - self._attr_historical_states
     - self.async_update_historical()
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._attr_historical_states: List[HistoricalState] = []  # type: ignore[annotation-unchecked]
+        self._attr_historical_states: list[HistoricalState] = []  # type: ignore[annotation-unchecked]
+
+    async def async_added_to_hass(self):
+        await super().async_added_to_hass()
+
+        #
+        # Setting state_class enables HomeAssistant to run statistic calculations on
+        # this sensor.
+        # We handle our own statistics and can be different from the Home Assisstant
+        # ones (also, we don't fully understand some internal procedures of
+        # HomeAssistant)
+        #
+
+        if self.statistic_id and hasattr(self, "state_class"):
+            _LOGGER.warning(
+                f"{self.entity_id}: state_class attribute is set. "
+                "This is NOT supported, your statistics will be messed sooner or later"
+            )
 
     @property
     def should_poll(self):
         # HistoricalSensors MUST NOT poll.
         # Polling creates incorrect states at intermediate time points.
 
         return False
@@ -140,23 +154,23 @@
         _LOGGER.debug(f"{self.entity_id}: {n} states written into the database")
 
         # Write statistics
         n = len(await self._async_write_statistic_data(hist_states))
         _LOGGER.debug(f"{self.entity_id}: {n} statistics points written into database")
 
     async def _async_write_recorder_states(
-        self, hist_states: List[HistoricalState]
-    ) -> List[HistoricalState]:
+        self, hist_states: list[HistoricalState]
+    ) -> list[HistoricalState]:
         return await recorder.get_instance(self.hass).async_add_executor_job(
             self._write_recorder_states, hist_states
         )
 
     def _write_recorder_states(
-        self, hist_states: List[HistoricalState]
-    ) -> List[HistoricalState]:
+        self, hist_states: list[HistoricalState]
+    ) -> list[HistoricalState]:
         with hass_recorder_session(self.hass) as session:
             #
             # Delete invalid states
             #
 
             try:
                 n_states = delete_entity_invalid_states(session, self)
@@ -217,15 +231,15 @@
             _LOGGER.debug(f"{self.entity_id}: found {n_hist_states} new states")
 
             #
             # Build recorder States
             #
             state_meta = get_entity_states_meta(session, self)
 
-            db_states: List[db_schema.States] = []
+            db_states: list[db_schema.States] = []
             for idx, hist_state in enumerate(hist_states):
                 attrs_as_dict = _build_attributes(self, hist_state.state)
                 attrs_as_dict.update(hist_state.attributes)
                 attrs_as_str = db_schema.JSON_DUMP(attrs_as_dict)
 
                 attrs_as_bytes = (
                     b"{}" if hist_state.state is None else attrs_as_str.encode("utf-8")
@@ -257,21 +271,21 @@
                 db_states.append(state)
 
             save_states(session, db_states)
 
             return hist_states
 
     async def _async_write_statistic_data(
-        self, hist_states: List[HistoricalState]
-    ) -> List[HistoricalState]:
-        if self.statatistic_id is None:
+        self, hist_states: list[HistoricalState]
+    ) -> list[HistoricalState]:
+        if self.statistic_id is None:
             _LOGGER.debug(f"{self.entity_id}: statistics are not enabled")
             return []
 
-        statistics_meta = self.get_statatistic_metadata()
+        statistics_meta = self.get_statistic_metadata()
 
         latest = await get_last_statistics_wrapper(
             self.hass, statistics_meta["statistic_id"]
         )
 
         # Don't do this, see notes above "About deleting intersecting states"
         #
@@ -311,48 +325,48 @@
         )
 
         # for stat in statistics_data:
         #     tmp = dict(stat)
         #     start_dt = dtutil.as_local(tmp.pop("start"))
         #     _LOGGER.debug(f"new statistic: start={start_dt}, value={tmp!r}")
 
-        if valid_statistic_id(self.statatistic_id):
+        if valid_statistic_id(self.statistic_id):
             async_add_external_statistics(self.hass, statistics_meta, statistics_data)
         else:
             async_import_statistics(self.hass, statistics_meta, statistics_data)
 
         return hist_states
 
     @property
-    def statatistic_id(self) -> Optional[str]:
+    def statistic_id(self) -> str | None:
         return None
 
-    def get_statatistic_metadata(self) -> StatisticMetaData:
-        if self.statatistic_id is None:
-            raise ValueError(f"{self.entity_id} statatistics_id is None")
+    def get_statistic_metadata(self) -> StatisticMetaData:
+        if self.statistic_id is None:
+            raise ValueError(f"{self.entity_id} statistic_id is None")
 
-        if valid_statistic_id(self.statatistic_id):
-            source = split_statistic_id(self.statatistic_id)[0]
+        if valid_statistic_id(self.statistic_id):
+            source = split_statistic_id(self.statistic_id)[0]
         else:
             source = "recorder"
 
         metadata = StatisticMetaData(
             has_mean=False,
             has_sum=False,
             name=f"{self.name} Statistics",
             source=source,
-            statistic_id=self.statatistic_id,
+            statistic_id=self.statistic_id,
             unit_of_measurement=self.unit_of_measurement,
         )
 
         return metadata
 
     async def async_calculate_statistic_data(
-        self, hist_states: List[HistoricalState], *, latest: Optional[dict] = None
-    ) -> List[StatisticData]:
+        self, hist_states: list[HistoricalState], *, latest: dict | None = None
+    ) -> list[StatisticData]:
         raise NotImplementedError()
 
 
 class PollUpdateMixin(HistoricalSensor):
     """PollUpdateMixin for simulate poll update model
 
     This mixin provides:
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2021-2023 Luis López <luis@cuarentaydos.com>
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
@@ -14,17 +12,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
-from dataclasses import dataclass, field, asdict
-from typing import Any
+from dataclasses import asdict, dataclass, field
 from datetime import datetime
+from typing import Any
+
 from homeassistant.util import dt as dtutil
 
 
 @dataclass
 class HistoricalState:
     state: Any
     dt: datetime
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 1.0.1
+Version: 2.0.0b0
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 #  Historical sensors for Home Assistant ![](icon-64.png)
 
 <!-- Code and releases -->
 ![GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/ldotlopez/ha-historical-sensor?include_prereleases)
 [![CodeQL](https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-analysis.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <!-- Sponsors -->
 <a href="https://www.buymeacoffee.com/zepolson" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 105px !important;" ></a>
 
-Feed historical data into Home Assistant database. 
+Feed historical data into Home Assistant database.
 
 HomeAssistant architecture is built around polling (or pushing) data from devices, or data providers, in "real-time". Some data sources (e.g, energy, water or gas providers) can't be polled in real-time or readings are not accurate. However reading historical data, like last month consumption, it's possible and accurate. This module adds support to this.
 
 This module uses the `recoder` component and custom state creation to store states "from the past".
 
 Current projects using this module:
 
@@ -32,15 +32,15 @@
 
 
 ## Technical details
 
 Q. How it's accomplished?.
 
 A. It's a relatively easy answer but needs to be broken into some pieces:
-  
+
   1. A new property for sensors: `historical_states`. This property holds a list of `HistoricalState`s which are, basically, a `state`+`datetime`  (with tzinfo), so… the data we want.
 
   2. A new hook for sensor: `async_update_historical_states`. This method is responsible to update `historical_states` property.  
      **This is the only function that needs to be implemented**.
 
   3. A new method, implemented by HistoricalSensor class: `async_write_ha_historical_states`. This method handles the details of creating tweaked states in the past and write them into the database using the `recorder` component of Home Assistant core.
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.1
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0b0
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
-historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
-markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
-Release (latest SemVer including pre-releases)](https://img.shields.io/github/
-v/release/ldotlopez/ha-historical-sensor?include_prereleases) [![CodeQL](https:
-//github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-
+historical-sensor/issues Requires-Python: >=3.10 Description-Content-Type:
+text/markdown # Historical sensors for Home Assistant ![](icon-64.png)  !
+[GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/
+github/v/release/ldotlopez/ha-historical-sensor?include_prereleases) [![CodeQL]
+(https://github.com/ldotlopez/ha-historical-sensor/actions/workflows/codeql-
 analysis.yml/badge.svg)](https://github.com/ldotlopez/ha-historical-sensor/
 actions/workflows/codeql-analysis.yml) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black)  [Buy_Me_A_Coffee] Feed historical data into Home Assistant database.
 HomeAssistant architecture is built around polling (or pushing) data from
 devices, or data providers, in "real-time". Some data sources (e.g, energy,
 water or gas providers) can't be polled in real-time or readings are not
```

### Comparing `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/SOURCES.txt` & `homeassistant-historical-sensor-2.0.0b0/homeassistant_historical_sensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.1/setup.cfg` & `homeassistant-historical-sensor-2.0.0b0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 1.0.1
+version = 2.0.0b0
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls = 
 	Repository = https://github.com/ldotlopez/ha-historical-sensor/
 	Bug Tracker = https://github.com/ldotlopez/ha-historical-sensor/issues
 
 [options]
 package_dir = 
 	homeassistant-historical-sensor = homeassistant_historical_sensor
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 
 [options.packages.find]
 where = 
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

