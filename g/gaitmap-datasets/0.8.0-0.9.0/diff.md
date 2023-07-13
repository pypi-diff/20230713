# Comparing `tmp/gaitmap_datasets-0.8.0.tar.gz` & `tmp/gaitmap_datasets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap_datasets-0.8.0.tar", max compression
+gzip compressed data, was "gaitmap_datasets-0.9.0.tar", max compression
```

## Comparing `gaitmap_datasets-0.8.0.tar` & `gaitmap_datasets-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0     1072 2023-01-30 09:01:17.736926 gaitmap_datasets-0.8.0/LICENSE
--rw-r--r--   0        0        0     7165 2023-01-30 09:01:17.736926 gaitmap_datasets-0.8.0/README.md
--rw-r--r--   0        0        0     1299 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/__init__.py
--rw-r--r--   0        0        0     6418 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/_config.py
--rw-r--r--   0        0        0      208 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/egait_parameter_validation_2013/__init__.py
--rw-r--r--   0        0        0     2843 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/egait_parameter_validation_2013/_dataset.py
--rw-r--r--   0        0        0     4752 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/egait_parameter_validation_2013/helper.py
--rw-r--r--   0        0        0      227 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/egait_segmentation_validation_2014/__init__.py
--rw-r--r--   0        0        0     3262 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/egait_segmentation_validation_2014/_dataset.py
--rw-r--r--   0        0        0     5791 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/egait_segmentation_validation_2014/helper.py
--rw-r--r--   0        0        0      270 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/pyshoe_2019/__init__.py
--rw-r--r--   0        0        0     8562 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/pyshoe_2019/_dataset.py
--rw-r--r--   0        0        0     4073 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/pyshoe_2019/helper.py
--rw-r--r--   0        0        0      333 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/sensor_position_comparison_2019/__init__.py
--rw-r--r--   0        0        0    14724 2023-01-30 09:01:17.740926 gaitmap_datasets-0.8.0/gaitmap_datasets/sensor_position_comparison_2019/_dataset.py
--rw-r--r--   0        0        0    13031 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/sensor_position_comparison_2019/helper.py
--rw-r--r--   0        0        0      267 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/__init__.py
--rw-r--r--   0        0        0    16375 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/_dataset.py
--rw-r--r--   0        0        0     7662 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/helper.py
--rw-r--r--   0        0        0    11444 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/pressure_sensor_helper.py
--rw-r--r--   0        0        0        0 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/scripts/__init__.py
--rw-r--r--   0        0        0     3261 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/scripts/create_pressure_events.py
--rw-r--r--   0        0        0       43 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/utils/__init__.py
--rw-r--r--   0        0        0     1068 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/utils/consts.py
--rw-r--r--   0        0        0     8212 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/utils/coordinate_transforms.py
--rw-r--r--   0        0        0     1333 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/utils/data_loading.py
--rw-r--r--   0        0        0     4351 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/utils/egait_loading_helper.py
--rw-r--r--   0        0        0     5036 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/gaitmap_datasets/utils/event_detection.py
--rw-r--r--   0        0        0     2338 2023-01-30 09:01:17.744926 gaitmap_datasets-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8505 1970-01-01 00:00:00.000000 gaitmap_datasets-0.8.0/setup.py
--rw-r--r--   0        0        0     8139 1970-01-01 00:00:00.000000 gaitmap_datasets-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-02 17:14:02.998180 gaitmap_datasets-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7305 2023-02-02 17:14:02.998180 gaitmap_datasets-0.9.0/README.md
+-rw-r--r--   0        0        0     1361 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/__init__.py
+-rw-r--r--   0        0        0     6430 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/_config.py
+-rw-r--r--   0        0        0      154 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_adidas_2014/__init__.py
+-rw-r--r--   0        0        0     8426 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_adidas_2014/_dataset.py
+-rw-r--r--   0        0        0    14841 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_adidas_2014/helper.py
+-rw-r--r--   0        0        0      208 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_parameter_validation_2013/__init__.py
+-rw-r--r--   0        0        0     3691 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_parameter_validation_2013/_dataset.py
+-rw-r--r--   0        0        0     5178 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_parameter_validation_2013/helper.py
+-rw-r--r--   0        0        0      227 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_segmentation_validation_2014/__init__.py
+-rw-r--r--   0        0        0     3262 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_segmentation_validation_2014/_dataset.py
+-rw-r--r--   0        0        0     5791 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/egait_segmentation_validation_2014/helper.py
+-rw-r--r--   0        0        0      270 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/pyshoe_2019/__init__.py
+-rw-r--r--   0        0        0     8562 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/pyshoe_2019/_dataset.py
+-rw-r--r--   0        0        0     4073 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/pyshoe_2019/helper.py
+-rw-r--r--   0        0        0      333 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/sensor_position_comparison_2019/__init__.py
+-rw-r--r--   0        0        0    14744 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/sensor_position_comparison_2019/_dataset.py
+-rw-r--r--   0        0        0    12179 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/sensor_position_comparison_2019/helper.py
+-rw-r--r--   0        0        0      267 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/__init__.py
+-rw-r--r--   0        0        0    16375 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/_dataset.py
+-rw-r--r--   0        0        0     7672 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/helper.py
+-rw-r--r--   0        0        0    11427 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/pressure_sensor_helper.py
+-rw-r--r--   0        0        0       63 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/scripts/__init__.py
+-rw-r--r--   0        0        0     3261 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/scripts/create_pressure_events.py
+-rw-r--r--   0        0        0      170 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1034 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/c3d_loading.py
+-rw-r--r--   0        0        0     1068 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/consts.py
+-rw-r--r--   0        0        0     8198 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/coordinate_transforms.py
+-rw-r--r--   0        0        0     1333 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/data_loading.py
+-rw-r--r--   0        0        0     5142 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/egait_loading_helper.py
+-rw-r--r--   0        0        0     9043 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/gaitmap_datasets/utils/event_detection.py
+-rw-r--r--   0        0        0     3931 2023-02-02 17:14:03.006194 gaitmap_datasets-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8685 1970-01-01 00:00:00.000000 gaitmap_datasets-0.9.0/setup.py
+-rw-r--r--   0        0        0     8279 1970-01-01 00:00:00.000000 gaitmap_datasets-0.9.0/PKG-INFO
```

### Comparing `gaitmap_datasets-0.8.0/LICENSE` & `gaitmap_datasets-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/README.md` & `gaitmap_datasets-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 | Dataset                         | Info Link                                                       | Download                            |
 |---------------------------------|-----------------------------------------------------------------|-------------------------------------|
 | EgaitSegmentationValidation2014 | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |
 | EgaitParameterValidation2013    | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |
 | StairAmbulationHealthy2021      | https://osf.io/sgbw7/                                           | https://osf.io/download/5ueq6/      |
 | SensorPositionDataset2019       | https://zenodo.org/record/5747173                               | https://zenodo.org/record/5747173   |
+| EgaitAdidas2014                 | TBD                                                             | TBD                                 |
 
 ### External Datasets
 
 | Dataset    | Info Link                              | Download                                                                                                                          |
 |------------|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | PyShoe2019 | https://github.com/utiasSTARS/pyshoe/  | https://ieee-dataport.org/open-access/university-toronto-foot-mounted-inertial-navigation-dataset (or bash script in github repo) |
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/__init__.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# -*- coding: utf-8 -*-
 """Methods to access the open source gait datasets of the MaD-Lab."""
 from gaitmap_datasets._config import (
     DatasetsConfig,
     config,
     create_config_template,
     get_dataset_path,
     reset_config,
     set_config,
 )
+from gaitmap_datasets.egait_adidas_2014 import EgaitAdidas2014
 from gaitmap_datasets.egait_parameter_validation_2013 import EgaitParameterValidation2013
 from gaitmap_datasets.egait_segmentation_validation_2014 import EgaitSegmentationValidation2014
 from gaitmap_datasets.pyshoe_2019 import PyShoe2019Hallway, PyShoe2019Stairs, PyShoe2019Vicon
 from gaitmap_datasets.sensor_position_comparison_2019 import (
     SensorPositionComparison2019Mocap,
     SensorPositionComparison2019Segmentation,
 )
@@ -19,22 +19,23 @@
     StairAmbulationHealthy2021Full,
     StairAmbulationHealthy2021PerTest,
 )
 
 __all__ = [
     "EgaitSegmentationValidation2014",
     "EgaitParameterValidation2013",
+    "EgaitAdidas2014",
     "StairAmbulationHealthy2021PerTest",
     "StairAmbulationHealthy2021Full",
     "SensorPositionComparison2019Segmentation",
     "SensorPositionComparison2019Mocap",
     "PyShoe2019Vicon",
     "PyShoe2019Hallway",
     "PyShoe2019Stairs",
     "DatasetsConfig",
     "set_config",
     "reset_config",
     "config",
     "create_config_template",
     "get_dataset_path",
 ]
-__version__ = "0.8.0"
+__version__ = "0.9.0"
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/_config.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,44 +11,45 @@
     """Get config data from json file."""
     config_file = getattr(settings.__config__, "config_file", None)
     using_default = False
     if config_file is None:
         config_file = getattr(settings.__config__, "default_config_file", None)
         using_default = True
     try:
-        with open(config_file, encoding="utf8") as f:
+        with Path(config_file).open(encoding="utf8") as f:
             return json.load(f)["datasets"]
     except FileNotFoundError as e:
         if using_default:
             return {}
         raise ValueError(f"Config file {config_file} not found.") from e
 
 
 class DatasetsConfig(BaseSettings):
     """Configuration class for the dataset paths."""
 
     egait_parameter_validation_2013: Optional[DirectoryPath]
     sensor_position_comparison_2019: Optional[DirectoryPath]
     egait_segmentation_validation_2014: Optional[DirectoryPath]
     pyshoe_2019: Optional[DirectoryPath]
+    egait_adidas_2014: Optional[DirectoryPath]
     stair_ambulation_healthy_2021: Optional[DirectoryPath]
 
     class Config:
         """The config."""
 
         config_file: ClassVar[str]
         default_config_file: ClassVar[str] = (Path(__file__).parent.parent / ".datasets.dev.json").resolve()
         validate_assignment = True
 
         @classmethod
         def customise_sources(
             cls,
             init_settings: SettingsSourceCallable,
-            env_settings: SettingsSourceCallable,  # pylint: disable=unused-argument
-            file_secret_settings: SettingsSourceCallable,  # pylint: disable=unused-argument
+            env_settings: SettingsSourceCallable,  # noqa: ARG003
+            file_secret_settings: SettingsSourceCallable,  # noqa: ARG003
         ) -> Tuple[SettingsSourceCallable, ...]:
             """Customize the sources."""
             return init_settings, json_config_settings_source
 
 
 _GLOBAL_CONFIG: Optional[DatasetsConfig] = None
 
@@ -75,15 +76,15 @@
         raise ValueError("Config is already set!")
     if isinstance(config_obj_or_path, (str, Path)):
         DatasetsConfig.Config.config_file = Path(config_obj_or_path)
         config_obj = DatasetsConfig()
     elif isinstance(config_obj_or_path, DatasetsConfig):
         config_obj = config_obj_or_path
     else:
-        raise ValueError("Unknown config type.")
+        raise TypeError("Unknown config type.")
     _GLOBAL_CONFIG = config_obj
 
 
 def reset_config():
     """Reset the global config to None.
 
     Afterwards you can use `set_config` to set a new config (e.g. to change the config file during runtime).
@@ -122,15 +123,15 @@
         The path to the file where the config should be created.
 
     """
     path = Path(path)
     if path.exists():
         raise ValueError(f"Config file {path} already exists.")
 
-    with open(path, "w", encoding="utf8") as f:
+    with path.open("w", encoding="utf8") as f:
         json.dump({"datasets": {k: None for k in DatasetsConfig.__fields__}}, f, indent=4, sort_keys=True)
 
     print(f"Created config template at {path.resolve()}.")
 
 
 def get_dataset_path(dataset_name: str) -> Path:
     """Get the path to a dataset be reading the global config.
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/egait_parameter_validation_2013/_dataset.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/egait_parameter_validation_2013/_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,26 +12,44 @@
     get_all_participants,
     get_gaitrite_parameters,
     get_segmented_stride_list,
 )
 
 
 class EgaitParameterValidation2013(Dataset):
-    """Egait parameter validation 2013 dataset."""
+    """Egait parameter validation 2013 dataset.
+
+    Parameters
+    ----------
+    data_folder
+        The path to the data folder. If None, the path from the config is used.
+    include_bad_data
+        A couple of participants appear to have bad data.
+        If True, these participants are included (as in the original publication).
+        If False, these participants are excluded (recommended).
+    use_alternative_calibrations
+        The original calibration files showed a big acc offset.
+        Therefore, we recommend to use the alternative calibration files.
+        If True, the alternative calibration files are used.
+        If False, the original calibration files are used (as in the original publication).
+
+    """
 
     def __init__(
         self,
         data_folder: Optional[Union[str, Path]] = None,
         *,
+        include_bad_data: bool = False,
         use_alternative_calibrations: bool = True,
         memory: Memory = Memory(None),
         groupby_cols: Optional[Union[List[str], str]] = None,
         subset_index: Optional[pd.DataFrame] = None
     ):
         self.data_folder = data_folder
+        self.include_bad_data = include_bad_data
         self.use_alternative_calibrations = use_alternative_calibrations
         self.memory = memory
         super().__init__(groupby_cols=groupby_cols, subset_index=subset_index)
 
     @property
     def sampling_rate_hz(self) -> float:
         """Get the sampling rate of the IMUs."""
@@ -68,8 +86,11 @@
     def gaitrite_parameters_(self) -> Dict[Literal["left_sensor", "right_sensor"], pd.DataFrame]:
         """Get the gaitrite parameters."""
         self.assert_is_single(None, "gaitrite_parameters_")
         return get_gaitrite_parameters(self.group, base_dir=self._data_folder_path)
 
     def create_index(self) -> pd.DataFrame:
         """Create index."""
-        return pd.DataFrame(get_all_participants(base_dir=self._data_folder_path), columns=["participant"])
+        return pd.DataFrame(
+            get_all_participants(include_bad_data=self.include_bad_data, base_dir=self._data_folder_path),
+            columns=["participant"],
+        )
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/egait_parameter_validation_2013/helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/egait_parameter_validation_2013/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,33 +7,40 @@
 from pathlib import Path
 from typing import Dict, List, Literal, Optional
 
 import pandas as pd
 from scipy.spatial.transform import Rotation
 
 from gaitmap_datasets.utils.coordinate_transforms import flip_sensor
-from gaitmap_datasets.utils.egait_loading_helper import load_shimmer2_data
+from gaitmap_datasets.utils.egait_loading_helper import find_extended_calib_files, load_shimmer2_data
 
 CALIBRATION_FILE_NAMES = {
     "left_sensor": "A917.csv",
     "right_sensor": "A6DF.csv",
 }
 
 ALTERNATIVE_CALIBRATION_FOLDER_NAMES = {
     "left_sensor": Path("A917/2015-01-01_00-01/"),
     "right_sensor": Path("A6DF/2015-01-01_00-01/"),
 }
 
+SENSOR_IDS = {
+    "left_sensor": "A917",
+    "right_sensor": "A6DF",
+}
+
 COORDINATE_SYSTEM_TRANSFORMATION = {  # egait_lateral_shimmer2r
     # [[-y -> +x], [+z -> +y], [-x -> +z]]
     "left_sensor": [[0, -1, 0], [0, 0, 1], [-1, 0, 0]],
     # [[+y -> +x], [-z -> +y], [-x -> +z]]
     "right_sensor": [[0, 1, 0], [0, 0, -1], [-1, 0, 0]],
 }
 
+BAD_DATA = ["P52"]
+
 
 def _raw_data_folder(base_dir: Path) -> Path:
     """Return the relative path to the participant subfolder."""
     return base_dir / "ValidationRawData"
 
 
 def _reference_stride_borders_folder(base_dir: Path) -> Path:
@@ -52,29 +59,36 @@
 
 
 def _alternative_calibration_folder(base_dir: Path) -> Path:
     """Return the relative path to the imu-calibration subfolder."""
     return base_dir / "alternative_calibrations"
 
 
-def get_all_participants(*, base_dir: Optional[Path] = None) -> List[str]:
+def get_all_participants(include_bad_data: bool = False, *, base_dir: Optional[Path] = None) -> List[str]:
     """Get the folder names of all participants."""
-    return [f.name.split("_")[0] for f in _raw_data_folder(base_dir).glob("*_left.dat")]
+    all_participants = sorted([f.name.split("_")[0] for f in _raw_data_folder(base_dir).glob("*_left.dat")])
+    if include_bad_data:
+        return all_participants
+    return list(set(all_participants) - set(BAD_DATA))
 
 
 def get_all_data_for_participant(
     participant_id: str, use_alternative_calibrations: bool = True, *, base_dir: Optional[Path] = None
 ) -> Dict[Literal["left_sensor", "right_sensor"], pd.DataFrame]:
     """Get all data for a participant."""
     all_data = {}
     for foot in ["left", "right"]:
         sensor = foot + "_sensor"
         data_path = _raw_data_folder(base_dir) / f"{participant_id}_E4_{foot}.dat"
         if use_alternative_calibrations:
             calibration_path = _alternative_calibration_folder(base_dir) / ALTERNATIVE_CALIBRATION_FOLDER_NAMES[sensor]
+            calibration_path = find_extended_calib_files(
+                calibration_path,
+                SENSOR_IDS[sensor],
+            )
         else:
             calibration_path = _calibration_folder(base_dir) / CALIBRATION_FILE_NAMES[sensor]
         data = load_shimmer2_data(data_path, calibration_path)
         data = flip_sensor(data, Rotation.from_matrix(COORDINATE_SYSTEM_TRANSFORMATION[sensor]))
         all_data[sensor] = data
     return all_data
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/egait_segmentation_validation_2014/_dataset.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/egait_segmentation_validation_2014/_dataset.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/egait_segmentation_validation_2014/helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/egait_segmentation_validation_2014/helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/pyshoe_2019/_dataset.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/pyshoe_2019/_dataset.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/pyshoe_2019/helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/pyshoe_2019/helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/sensor_position_comparison_2019/_dataset.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/sensor_position_comparison_2019/_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,21 +298,21 @@
         tests = (
             (p, t)
             for p in get_all_participants(self.include_wrong_recording, data_folder=self._data_folder_path)
             for t in get_all_tests(p, self._data_folder_path)
         )
         return pd.DataFrame(tests, columns=["participant", "test"])
 
-    def convert_with_padding(
+    def convert_events_with_padding(
         self,
         events: pd.DataFrame,
         from_time_axis: Literal["mocap", "imu"],
         to_time_axis: Literal["mocap", "imu", "time"],
     ):
-        """Convert the time/sample values of mocap and IMU events into other time domains.
+        """Convert the time/sample values of mocap and IMU events/stride lists into other time domains.
 
         This method will use the respective sampling rates and the padding of the IMU data to convert the time/sample.
 
         ... warning::
             This method will only work, if the provided samples follow the padding conventions used in this class!
             This means, if the input are events in IMU samples (`from_time_axis="imu"`), they must respect the
             padding of the IMU data.
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/sensor_position_comparison_2019/helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/sensor_position_comparison_2019/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 """A set of helpers to load the dataset."""
 
 import json
 import warnings
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
-import c3d
 import numpy as np
 import pandas as pd
 from imucal.management import CalibrationWarning
 from nilspodlib import SyncedSession
 from nilspodlib.exceptions import CorruptedPackageWarning, LegacyWarning, SynchronisationWarning
 from scipy.spatial.transform import Rotation
 from typing_extensions import Literal
 
+from gaitmap_datasets.utils.c3d_loading import load_c3d_data
 from gaitmap_datasets.utils.coordinate_transforms import flip_dataset, rotation_from_angle
 
-COORDINATE_TRANSFORMATION_DICT = dict(
-    qualisis_lateral_nilspodv1={
+COORDINATE_TRANSFORMATION_DICT = {
+    "qualisis_lateral_nilspodv1": {
         # [[+y -> +x], [+z -> +y], [+x -> +z]]
         "left_sensor": [[0, 1, 0], [0, 0, 1], [1, 0, 0]],
         # [[-y -> +x], [-z -> +y], [+x -> +z]]
         "right_sensor": [[0, -1, 0], [0, 0, -1], [1, 0, 0]],
     },
-    qualisis_medial_nilspodv1={
+    "qualisis_medial_nilspodv1": {
         # [[-y -> +x], [-z -> +y], [+x -> +z]]
         "left_sensor": [[0, -1, 0], [0, 0, -1], [1, 0, 0]],
         # [[+y -> +x], [+z -> +y], [+x -> +z]]
         "right_sensor": [[0, 1, 0], [0, 0, 1], [1, 0, 0]],
     },
-    qualisis_instep_nilspodv1={
+    "qualisis_instep_nilspodv1": {
         # [[-x -> +x], [-y -> +y], [+z -> +z]]
         "left_sensor": [[-1, 0, 0], [0, -1, 0], [0, 0, 1]],
         # [[-x -> +x], [-y -> +y], [+z -> +z]]
         "right_sensor": [[-1, 0, 0], [0, -1, 0], [0, 0, 1]],
     },
-    qualisis_cavity_nilspodv1={
+    "qualisis_cavity_nilspodv1": {
         # [[-x -> +x], [-y -> +y], [+z -> +z]]
         "left_sensor": [[-1, 0, 0], [0, -1, 0], [0, 0, 1]],
         # [[-x -> +x], [-y -> +y], [+z -> +z]]
         "right_sensor": [[-1, 0, 0], [0, -1, 0], [0, 0, 1]],
     },
-    qualisis_heel_nilspodv1={
+    "qualisis_heel_nilspodv1": {
         # [[-z -> +x], [+y -> +y], [+x -> +z]]
         "left_sensor": [[0, 0, -1], [0, 1, 0], [1, 0, 0]],
         # [[-z -> +x], [+y -> +y], [+x -> +z]]
         "right_sensor": [[0, 0, -1], [0, 1, 0], [1, 0, 0]],
     },
-    qualisis_insole_nilspodv1={
+    "qualisis_insole_nilspodv1": {
         # [[+y -> +x], [-x -> +y], [+z -> +z]]
         "left_sensor": [[0, 1, 0], [-1, 0, 0], [0, 0, 1]],
         # [[-y -> +x], [+x -> +y], [+z -> +z]]
         "right_sensor": [[0, -1, 0], [1, 0, 0], [0, 0, 1]],
     },
-)
+}
 
 
 def get_data_folder(data_folder=None, data_subfolder=True):
     """Get the data folder or subfolder."""
     data_folder = Path(data_folder)
     if data_subfolder:
         return Path(data_folder) / "data"
@@ -82,16 +82,15 @@
             continue
         yield participant.name
 
 
 def get_all_tests(participant_id: str, data_folder=None):
     """Iterate over all tests of a participant."""
     tests = get_metadata_participant(participant_id, data_folder=data_folder)["mocap_test_start"].keys()
-    for k in tests:
-        yield k
+    yield from tests
 
 
 def get_participant_folder(participant_id: str, data_folder=None) -> Path:
     """Get the toplevel data folder of a participant."""
     return get_data_folder(data_folder) / participant_id
 
 
@@ -259,43 +258,14 @@
     imu = folder / "imu"
     for f in imu.glob("*.bin"):
         if f.name.split("-")[1].startswith(sensor_id.upper()):
             return f
     raise FileNotFoundError(f"No sensor file found for {sensor_name} of {participant_id}")
 
 
-def load_c3d_data(path: Union[Path, str], insert_nan: bool = True) -> pd.DataFrame:
-    """Load a c3d file.
-
-    Parameters
-    ----------
-    path
-        Path to the file
-    insert_nan
-        If True missing values in the marker paths will be indicated with a np.nan.
-        Otherwise, there are just 0 (?).
-
-    """
-    with open(path, "rb") as handle:
-        reader = c3d.Reader(handle)
-        frames = []
-
-        for _, points, _ in reader.read_frames():
-            frames.append(points[:, :3])
-
-        labels = [label.strip().lower() for label in reader.point_labels]
-        frames = np.stack(frames)
-        frames = frames.reshape(frames.shape[0], -1)
-    index = pd.MultiIndex.from_product([labels, list("xyz")])
-    data = pd.DataFrame(frames, columns=index) / 1000  # To get the data in m
-    if insert_nan is True:
-        data[data == 0.000000] = np.nan
-    return data
-
-
 def get_foot_sensor(foot: Literal["left", "right"], include_insole: bool = True) -> List[str]:
     """Get the names of all sensors that are attached to a foot (left or right)."""
     sensors = ["{}_cavity", "{}_heel", "{}_lateral", "{}_medial", "{}_instep"]
     if include_insole is True:
         sensors.append("{}_insole")
     return [s.format(foot[0]) for s in sensors]
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/_dataset.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/_dataset.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ) -> Dict[str, Dict[str, Dict[str, Union[int, Literal["part_1", "part_2"]]]]]:
     """Get a dictionary containing all test information for all participants."""
     all_test_list = _participant_subfolder(base_dir).rglob("test_list.json")
     all_test_per_participant = {}
 
     for test_list in all_test_list:
         participant = test_list.parent.parent.name
-        with open(test_list, "r", encoding="utf8") as f:
+        with test_list.open(encoding="utf8") as f:
             test_data = json.load(f)
         test_data.pop("part_1_transition", None)
         part = test_list.parent.name
         # Avoid name clash of the "full_session" test
         test_data[f"full_session_{part}"] = test_data.pop("full_session")
         # Add the part the test belongs to the test_data
         for test_info in test_data.values():
@@ -70,15 +70,15 @@
         tmp.update(test_data)
 
     return all_test_per_participant
 
 
 def get_participant_metadata(participant_folder_name: str, *, base_dir: Optional[Path] = None) -> Dict[str, Any]:
     """Get the metadata of a participant."""
-    with open((_participant_subfolder(base_dir) / participant_folder_name / "metadata.json"), encoding="utf8") as f:
+    with (_participant_subfolder(base_dir) / participant_folder_name / "metadata.json").open(encoding="utf8") as f:
         metadata = json.load(f)
     return metadata
 
 
 def get_all_data_for_participant(
     participant_folder_name: str,
     part: Literal["part_1", "part_2"],
@@ -101,15 +101,16 @@
             # This is a NilsPod bug that happens sometimes.
             # In this case the index of the last couple of values is broken.
             # Therefore, we simply remove them.
             session = session.cut(stop=-10)
             session = session.align_to_syncregion()
     # apply ferraris calibration on imu data
     session.calibrate_imu(
-        session.find_closest_calibration(folder=_calibration_folder(base_dir), filter_cal_type="ferraris"), inplace=True
+        session.find_closest_calibration(folder=_calibration_folder(base_dir), filter_cal_type="ferraris"),
+        inplace=True,  # noqa: PD002
     )
     session_df = session.data_as_df(concat_df=True)
 
     # load_metadata to rename columns
     metadata = get_participant_metadata(participant_folder_name, base_dir=base_dir)
     sensor_mapping = {v: k for k, v in metadata["sensor_ids"].items()}
     # Rename all columns
@@ -125,15 +126,15 @@
         for s in ["left_sensor", "right_sensor"]:
             calibrated_data = calibrate_analog_data(
                 session_df[s][["analog_0", "analog_1", "analog_2"]].to_numpy(),
                 metadata["fsr_ids"][s],
                 base_dir=base_dir,
             )
             calibrated_data = pd.DataFrame(
-                calibrated_data, columns=[f"{p}_force" for p in metadata["fsr_ids"][s].keys()]
+                calibrated_data, columns=[f"{p}_force" for p in metadata["fsr_ids"][s]]
             ).assign(total_force=lambda df_: df_.sum(axis=1))
             all_calibrated_pressure_data[s] = calibrated_data
 
         all_calibrated_pressure_data = pd.concat(all_calibrated_pressure_data, axis=1)
         session_df = session_df.join(all_calibrated_pressure_data)
 
     session_df = session_df.drop(columns=["analog_0", "analog_1", "analog_2"], level=1)
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/pressure_sensor_helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/pressure_sensor_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
         try:
             min_vel_list.append(
                 detect_min_vel(gyr_bf_stride.to_numpy()[gyr_ml_max_idx:], window_size)
                 + gyr_ml_max_idx
                 + stride_start_end[0]
             )
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:  # noqa: BLE001
             print(f"Failed to detect min-vel for {stride_start_end} ({e})")
 
     # now we need to add "pre_min_vel" events for those strides who have no previous stride (aka strides which do not
     # share their start index with the end index of another stride)
 
     stride_ids_with_no_prev_stride = (
         np.argwhere(
@@ -239,15 +239,15 @@
             total_force = total_force - np.min(total_force)
 
             th = threshold_kg
             zero_crossings = np.array([])
 
             # search for threshold crossings until we found exactly two crossings, gradually increase threshold in
             # "threshold_increment_kg" steps on the way
-            # if we don´t find two crossings until the threshold reaches max_threshold_kg the pressure event detection
+            # if we don`t find two crossings until the threshold reaches max_threshold_kg the pressure event detection
             # failed!
             while len(zero_crossings) != 2:
                 zero_crossings = np.where(np.diff(np.signbit(total_force - th)))[0]
                 th = th + self.threshold_increment_kg
                 if th > self.max_threshold_kg:
                     zero_crossings = np.array([None, None])
                     break
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/stair_ambulation_healthy_2021/scripts/create_pressure_events.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/stair_ambulation_healthy_2021/scripts/create_pressure_events.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/utils/consts.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/utils/consts.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/utils/coordinate_transforms.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/utils/coordinate_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     rotation_dict = rotation
     if not isinstance(rotation_dict, dict):
         rotation_dict = {k: rotation for k in dataset.columns.unique(level=0)}
 
     rotated_dataset = dataset.copy()
     original_cols = dataset.columns
 
-    for key in rotation_dict.keys():
+    for key in rotation_dict:
         rotated_dataset[key] = flip_sensor(dataset[key], rotation_dict[key], inplace=False)
 
     # Restore original order
     rotated_dataset = rotated_dataset[original_cols]
     return rotated_dataset
 
 
@@ -169,15 +169,15 @@
     rotation_dict = rotation
     if not isinstance(rotation_dict, dict):
         rotation_dict = {k: rotation for k in dataset.columns.unique(level=0)}
 
     rotated_dataset = dataset.copy()
     original_cols = dataset.columns
 
-    for key in rotation_dict.keys():
+    for key in rotation_dict:
         rotated_dataset[key] = rotate_sensor(dataset[key], rotation_dict[key], inplace=False)
 
     # Restore original order
     rotated_dataset = rotated_dataset[original_cols]
     return rotated_dataset
```

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/utils/data_loading.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `gaitmap_datasets-0.8.0/gaitmap_datasets/utils/egait_loading_helper.py` & `gaitmap_datasets-0.9.0/gaitmap_datasets/utils/egait_loading_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """Helper to load data of the egait system (specifically the shimmer 2R system)."""
 import copy
+from collections import namedtuple
 from pathlib import Path
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from imucal import FerrarisCalibrationInfo
 
 from gaitmap_datasets.utils.data_loading import load_bin_file
 
-SHIMMER2_DATA_LAYOUT = {
-    "acc_x": np.uint16,
-    "acc_y": np.uint16,
-    "acc_z": np.uint16,
-    "gyr_x": np.uint16,
-    "gyr_y": np.uint16,
-    "gyr_z": np.uint16,
+SHIMMER_DATA_LAYOUT = {
+    "acc_x": np.int16,
+    "acc_y": np.int16,
+    "acc_z": np.int16,
+    "gyr_x": np.int16,
+    "gyr_y": np.int16,
+    "gyr_z": np.int16,
 }
 
+ExtendedCalibFilePath = namedtuple("ExtendedCalibFilePath", ["acc", "gyr"])
+
+CalibFilePath = Union[Path, ExtendedCalibFilePath]
+
 
 def transform_shimmer2_axes(dataset: pd.DataFrame) -> pd.DataFrame:
     """Transform shimmer2 axes to align acc and gyroscope.
 
     Parameters
     ----------
     dataset
@@ -43,73 +49,90 @@
     dataset["gyr_x"] = gyr_y_original
     dataset["gyr_y"] = gyr_x_original
     dataset["gyr_z"] = -gyr_z_original
 
     return dataset
 
 
-def calibrate_shimmer2_data(
+def calibrate_shimmer_data(
     data: pd.DataFrame,
-    calibration_file_path: Path,
+    calibration_file_path: CalibFilePath,
 ) -> pd.DataFrame:
     """Calibrate shimmer2 data."""
-    if calibration_file_path.is_file():
+    if isinstance(calibration_file_path, ExtendedCalibFilePath):
+        cal_matrix = load_extended_calib(
+            acc_calib_path=calibration_file_path.acc, gyr_calib_path=calibration_file_path.gyr
+        )
+    elif isinstance(calibration_file_path, Path):
         cal_matrix = load_compact_cal_matrix(calibration_file_path)
-    elif calibration_file_path.is_dir():
-        cal_matrix = load_extended_calib(calibration_file_path)
     else:
-        raise ValueError("Calibration file does not exist.")
+        raise TypeError("Invalid calibration format.")
     data = cal_matrix.calibrate_df(data, "a.u.", "a.u.")
 
     return data
 
 
 def load_shimmer2_data(
     data_path: Path,
-    calibration_file_path: Path,
+    calibration_file_path: CalibFilePath,
 ) -> pd.DataFrame:
     """Load shimmer2 data from a file."""
-    data = load_bin_file(data_path, SHIMMER2_DATA_LAYOUT)
-    data = calibrate_shimmer2_data(data, calibration_file_path)
+    data = load_bin_file(data_path, SHIMMER_DATA_LAYOUT)
+    data = calibrate_shimmer_data(data, calibration_file_path)
     data = transform_shimmer2_axes(data)
     return data
 
 
+def load_shimmer3_data(
+    data_path: Path,
+    calibration_file_path: CalibFilePath,
+) -> pd.DataFrame:
+    """Load shimmer3 data from a file."""
+    data = load_bin_file(data_path, SHIMMER_DATA_LAYOUT)
+    data = calibrate_shimmer_data(data, calibration_file_path)
+    return data
+
+
+def find_extended_calib_files(calib_folder: Path, sensor_id: str) -> ExtendedCalibFilePath:
+    """Find the correct calibration files required for the extended calibration format."""
+    acc_calib_path = next(calib_folder.glob(f"{sensor_id.upper()}_acc.csv"))
+    gyr_calib_path = next(calib_folder.glob(f"{sensor_id.upper()}_gyro.csv"))
+    return ExtendedCalibFilePath(acc=acc_calib_path, gyr=gyr_calib_path)
+
+
 def load_compact_cal_matrix(path: Path) -> FerrarisCalibrationInfo:
     """Load a compact calibration matrix from a file."""
     cal_matrix = np.genfromtxt(path, delimiter=",")
     plus_g = cal_matrix[0]
     minus_g = cal_matrix[1]
-    b_a = (plus_g + minus_g) / 2
-    K_a = np.eye(3) * (plus_g - minus_g) / 2  # pylint: disable=invalid-name
-    K_a /= 9.81  # convert to m/s^2  # pylint: disable=invalid-name
-    R_a = np.eye(3)  # pylint: disable=invalid-name
-    b_g = cal_matrix[2]
-
-    # 2.731 is the digital conversion factor for the gyro
-    K_g = np.eye(3) * 2.731  # pylint: disable=invalid-name
-    R_g = np.eye(3)  # pylint: disable=invalid-name
-    K_ga = np.zeros((3, 3))  # pylint: disable=invalid-name
+    imucal_cal = {
+        "b_a": (plus_g + minus_g) / 2,
+        "K_a": np.eye(3) * (plus_g - minus_g) / 2 / 9.81,
+        "R_a": np.eye(3),
+        "b_g": cal_matrix[2],
+        "K_g": np.eye(3) * 2.731,  # 2.731 is the digital conversion factor for the gyro
+        "R_g": np.eye(3),
+        "K_ga": np.zeros((3, 3)),
+        "acc_unit": "m/s^2",
+        "gyr_unit": "deg/s",
+        "from_acc_unit": "a.u.",
+        "from_gyr_unit": "a.u.",
+    }
 
-    return FerrarisCalibrationInfo(
-        b_a=b_a, K_a=K_a, R_a=R_a, b_g=b_g, K_g=K_g, R_g=R_g, K_ga=K_ga, from_acc_unit="a.u.", from_gyr_unit="a.u."
-    )
+    return FerrarisCalibrationInfo(**imucal_cal)
 
 
-def load_extended_calib(calib_folder: Path) -> FerrarisCalibrationInfo:
+def load_extended_calib(acc_calib_path: Path, gyr_calib_path: Path) -> FerrarisCalibrationInfo:
     """Convert calibration files in format *_acc.csv and *_gyr.csv into a FerrarisCalibrationInfo object.
 
     This calibration format is used by later iterations of the egait system.
     It contains more information than the short calibration matrix and if data in this format is available, it should be
     preferred over the short calibration matrix.
     """
     # Each folder is a calibration
-
-    acc_calib_path = next(calib_folder.glob("*_acc.csv"))
-    gyr_calib_path = next(calib_folder.glob("*_gyro.csv"))
     acc_cal_phct = pd.read_csv(acc_calib_path, header=None)
     gyr_cal_phct = pd.read_csv(gyr_calib_path, header=None)
     imucal_cal = {
         "K_a": acc_cal_phct[[4, 5, 6]].to_numpy() / 9.81,
         "R_a": acc_cal_phct[[1, 2, 3]].to_numpy(),
         "b_a": acc_cal_phct[0].to_numpy(),
         "K_g": gyr_cal_phct[[4, 5, 6]].to_numpy(),
@@ -118,10 +141,11 @@
         "b_g": gyr_cal_phct[0].to_numpy(),
         "acc_unit": "m/s^2",
         "gyr_unit": "deg/s",
         "from_acc_unit": "a.u.",
         "from_gyr_unit": "a.u.",
     }
     imucal_cal = FerrarisCalibrationInfo(
-        **imucal_cal, comment=f"Date: {calib_folder.name}, Sensor Node: " f"{acc_calib_path.stem.split('_')[0]}"
+        **imucal_cal,
+        comment=f"Folder name: {acc_calib_path.parent.name}, Sensor Node: {acc_calib_path.stem.split('_')[0]}",
     )
     return imucal_cal
```

### Comparing `gaitmap_datasets-0.8.0/setup.py` & `gaitmap_datasets-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['gaitmap_datasets',
+ 'gaitmap_datasets.egait_adidas_2014',
  'gaitmap_datasets.egait_parameter_validation_2013',
  'gaitmap_datasets.egait_segmentation_validation_2014',
  'gaitmap_datasets.pyshoe_2019',
  'gaitmap_datasets.sensor_position_comparison_2019',
  'gaitmap_datasets.stair_ambulation_healthy_2021',
  'gaitmap_datasets.stair_ambulation_healthy_2021.scripts',
  'gaitmap_datasets.utils']
@@ -22,17 +23,17 @@
  'pandas>=1.4.2',
  'pydantic>=1.10.4,<2.0.0',
  'scipy>=1.8.1',
  'tpcp>=0.11']
 
 setup_kwargs = {
     'name': 'gaitmap-datasets',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Helper to access to open-source gait datasets used by MaD-Lab',
-    'long_description': '[![PyPI](https://img.shields.io/pypi/v/gaitmap-datasets)](https://pypi.org/project/gaitmap-datasets/)\n[![Documentation status](https://img.shields.io/badge/docs-online-green)](https://mad-lab-fau.github.io/gaitmap-datasets)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/gaitmap-datasets)\n\n# gaitmap-datasets\n\nHelper to access to open-source gait datasets compatible with the MaD-Lab gaitanalysis library gaitmap.\n\nThe aim of this package is to ensure that all datasets can be loaded in a similar fashion and all data (and annotations)\nare in the same format (i.e. the same sensor orientations, units, etc.).\nThis should allow to easily run the same algorithm across multiple datasets.\n\n> :warning: While this makes it easier to work with the datasets, the coordinate system and other data information\n> provided with the dataset might not match the format you get when using this library!\n\n\nAll datasets APIs are built using the \n[`tpcp.Dataset`](https://tpcp.readthedocs.io/en/latest/modules/generated/dataset/tpcp.Dataset.html#tpcp.Dataset)\ninterface.\nFor available datasets see the table below.\n\n## Usage\n\nInstall the package from Pip\n\n```\npip install gaitmap-datasets\n```\n\nThen download/obtain the dataset that you are planning to use (see below).\nThe best way to get started is to then check the example for the respective dataset on the \n[documentation page](https://mad-lab-fau.github.io/gaitmap-datasets/auto_examples/index.html).\n\n## Datasets\n\nBelow is a list of all available datasets with links to all information.\nMake sure you cite the respective papers if you use the data for your research.\nRecommended citations can be found in the respective dataset documentation (info link) and/or in the docstrings of the \nindividual dataset classes.\n\n### MaD-Lab Dataset\n\n| Dataset                         | Info Link                                                       | Download                            |\n|---------------------------------|-----------------------------------------------------------------|-------------------------------------|\n| EgaitSegmentationValidation2014 | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |\n| EgaitParameterValidation2013    | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |\n| StairAmbulationHealthy2021      | https://osf.io/sgbw7/                                           | https://osf.io/download/5ueq6/      |\n| SensorPositionDataset2019       | https://zenodo.org/record/5747173                               | https://zenodo.org/record/5747173   |\n\n### External Datasets\n\n| Dataset    | Info Link                              | Download                                                                                                                          |\n|------------|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|\n| PyShoe2019 | https://github.com/utiasSTARS/pyshoe/  | https://ieee-dataport.org/open-access/university-toronto-foot-mounted-inertial-navigation-dataset (or bash script in github repo) |\n\n\n## Working with datasets\n\nEach dataset is represented by a class.\nTo load the dataset, the path to the dataset folder needs to be provided.\nThere are multiple ways to do this:\n\n1. You can provide the path directly in the constructor of the dataset class.\n\n```python\nfrom gaitmap_datasets import EgaitSegmentationValidation2014\n\ndataset = EgaitSegmentationValidation2014("/path/to/dataset")\n```\n\n2. Alternatively, you can avoid hard-coding path in one location by creating a json config file:\n```python\n# Run the following once, to create the config file\nfrom gaitmap_datasets import create_config_template\n\ncreate_config_template("/path/to/config.json")\n```\nThen open the config file and add the path to the dataset folders you have downloaded.\nYou can just leave the values as `null` if you don\'t need a dataset.\n\n```json\n// file: /path/to/config.json\n{\n    "datasets": {\n        "egait_parameter_validation_2013": null,\n        "egait_segmentation_validation_2014": "/path/to/egait_segmentation_validation_2014/dataset",\n        "pyshoe_2019": null,\n        "sensor_position_comparison_2019": null,\n        "stair_ambulation_healthy_2021": null\n    }\n}\n```\n\nThen you can set the global config for gaitmap-datsets to point to the config file:\n\n```python\nfrom gaitmap_datasets import EgaitSegmentationValidation2014, set_config\n\nset_config("/path/to/config.json")\n# Now you can load the dataset without providing the path\n\ndataset = EgaitSegmentationValidation2014()\n```\n\n\n## Dev setup\n\nFirst clone the repo and install the dependencies using `poetry` (note this project only supports poetry >=1.2).\n\n```\ngit clone https://github.com/mad-lab-fau/gaitmap-datasets.git\ncd gaitmap-datasets\npoetry install\n```\n\n### Downloading and linking datasets\n\nThe datasets are not included in the package, and you need to download them manually (see above).\nStore the datasets you need in whatever folder you like.\n\nThen run `poetry run poe create_dev_config`.\nThis should create a `.datasets.dev.json` file in the root of the repo.\nModify this file to point to the folders of the respective datasets.\n\nWith that setup, all tests and examples should work without any modification to the code.\n\n### Testing\n\nThe `/tests` directory contains a set of tests to check the functionality of the library.\nHowever, most tests rely on the existence of the respective datasets in certain folders outside the library.\nTherefore, the tests can only be run locally and not on the CI server.\n\nTo run them locally, make sure you completed the dataset setup (see above) then run `poe test`.\n\n### Documentation (build instructions)\n\nAs the docs need the datasets to be available, we can not build them automatically on RTD.\nInstead, we host the docs via github pages.\nThe HTML source can be found in the `gh-pages` branch of this repo.\n\nTo make the deployment as easy as possible, we "mounted" the `gh-pages` branch as a submodule in the `docs/_build/html`\nfolder.\nHence, before you attempt to build the docs, you need to initialize the submodule.\n\n```\ngit submodule update --init --recursive\n```\n\nAfter that you can run `poe docs` to build the docs and then `poe upload_docs` to push the changes to the gh-pages\nbranch.\nWe will always just update a single commit on the gh-pages branch to keep the effective file size small.\n\n**WARNING:** Don\'t delete the `docs/_build` folder manually or by running the sphinx make file!\nThis will delete the submodule and might cause issues.\nThe `poe` task is configured to clean all relevant files in the `docs/_build` folder before each run.\n\nAfter an update of the documentation, you will see that you also need to make a commit in the main repo, as the commit \nhash of the docs submodule has changed.\n\nTo make sure you don\'t forget to update the docs, the `poe prepare_release` task will also build and upload the docs \nautomatically.',
+    'long_description': '[![PyPI](https://img.shields.io/pypi/v/gaitmap-datasets)](https://pypi.org/project/gaitmap-datasets/)\n[![Documentation status](https://img.shields.io/badge/docs-online-green)](https://mad-lab-fau.github.io/gaitmap-datasets)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/gaitmap-datasets)\n\n# gaitmap-datasets\n\nHelper to access to open-source gait datasets compatible with the MaD-Lab gaitanalysis library gaitmap.\n\nThe aim of this package is to ensure that all datasets can be loaded in a similar fashion and all data (and annotations)\nare in the same format (i.e. the same sensor orientations, units, etc.).\nThis should allow to easily run the same algorithm across multiple datasets.\n\n> :warning: While this makes it easier to work with the datasets, the coordinate system and other data information\n> provided with the dataset might not match the format you get when using this library!\n\n\nAll datasets APIs are built using the \n[`tpcp.Dataset`](https://tpcp.readthedocs.io/en/latest/modules/generated/dataset/tpcp.Dataset.html#tpcp.Dataset)\ninterface.\nFor available datasets see the table below.\n\n## Usage\n\nInstall the package from Pip\n\n```\npip install gaitmap-datasets\n```\n\nThen download/obtain the dataset that you are planning to use (see below).\nThe best way to get started is to then check the example for the respective dataset on the \n[documentation page](https://mad-lab-fau.github.io/gaitmap-datasets/auto_examples/index.html).\n\n## Datasets\n\nBelow is a list of all available datasets with links to all information.\nMake sure you cite the respective papers if you use the data for your research.\nRecommended citations can be found in the respective dataset documentation (info link) and/or in the docstrings of the \nindividual dataset classes.\n\n### MaD-Lab Dataset\n\n| Dataset                         | Info Link                                                       | Download                            |\n|---------------------------------|-----------------------------------------------------------------|-------------------------------------|\n| EgaitSegmentationValidation2014 | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |\n| EgaitParameterValidation2013    | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |\n| StairAmbulationHealthy2021      | https://osf.io/sgbw7/                                           | https://osf.io/download/5ueq6/      |\n| SensorPositionDataset2019       | https://zenodo.org/record/5747173                               | https://zenodo.org/record/5747173   |\n| EgaitAdidas2014                 | TBD                                                             | TBD                                 |\n\n### External Datasets\n\n| Dataset    | Info Link                              | Download                                                                                                                          |\n|------------|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|\n| PyShoe2019 | https://github.com/utiasSTARS/pyshoe/  | https://ieee-dataport.org/open-access/university-toronto-foot-mounted-inertial-navigation-dataset (or bash script in github repo) |\n\n\n## Working with datasets\n\nEach dataset is represented by a class.\nTo load the dataset, the path to the dataset folder needs to be provided.\nThere are multiple ways to do this:\n\n1. You can provide the path directly in the constructor of the dataset class.\n\n```python\nfrom gaitmap_datasets import EgaitSegmentationValidation2014\n\ndataset = EgaitSegmentationValidation2014("/path/to/dataset")\n```\n\n2. Alternatively, you can avoid hard-coding path in one location by creating a json config file:\n```python\n# Run the following once, to create the config file\nfrom gaitmap_datasets import create_config_template\n\ncreate_config_template("/path/to/config.json")\n```\nThen open the config file and add the path to the dataset folders you have downloaded.\nYou can just leave the values as `null` if you don\'t need a dataset.\n\n```json\n// file: /path/to/config.json\n{\n    "datasets": {\n        "egait_parameter_validation_2013": null,\n        "egait_segmentation_validation_2014": "/path/to/egait_segmentation_validation_2014/dataset",\n        "pyshoe_2019": null,\n        "sensor_position_comparison_2019": null,\n        "stair_ambulation_healthy_2021": null\n    }\n}\n```\n\nThen you can set the global config for gaitmap-datsets to point to the config file:\n\n```python\nfrom gaitmap_datasets import EgaitSegmentationValidation2014, set_config\n\nset_config("/path/to/config.json")\n# Now you can load the dataset without providing the path\n\ndataset = EgaitSegmentationValidation2014()\n```\n\n\n## Dev setup\n\nFirst clone the repo and install the dependencies using `poetry` (note this project only supports poetry >=1.2).\n\n```\ngit clone https://github.com/mad-lab-fau/gaitmap-datasets.git\ncd gaitmap-datasets\npoetry install\n```\n\n### Downloading and linking datasets\n\nThe datasets are not included in the package, and you need to download them manually (see above).\nStore the datasets you need in whatever folder you like.\n\nThen run `poetry run poe create_dev_config`.\nThis should create a `.datasets.dev.json` file in the root of the repo.\nModify this file to point to the folders of the respective datasets.\n\nWith that setup, all tests and examples should work without any modification to the code.\n\n### Testing\n\nThe `/tests` directory contains a set of tests to check the functionality of the library.\nHowever, most tests rely on the existence of the respective datasets in certain folders outside the library.\nTherefore, the tests can only be run locally and not on the CI server.\n\nTo run them locally, make sure you completed the dataset setup (see above) then run `poe test`.\n\n### Documentation (build instructions)\n\nAs the docs need the datasets to be available, we can not build them automatically on RTD.\nInstead, we host the docs via github pages.\nThe HTML source can be found in the `gh-pages` branch of this repo.\n\nTo make the deployment as easy as possible, we "mounted" the `gh-pages` branch as a submodule in the `docs/_build/html`\nfolder.\nHence, before you attempt to build the docs, you need to initialize the submodule.\n\n```\ngit submodule update --init --recursive\n```\n\nAfter that you can run `poe docs` to build the docs and then `poe upload_docs` to push the changes to the gh-pages\nbranch.\nWe will always just update a single commit on the gh-pages branch to keep the effective file size small.\n\n**WARNING:** Don\'t delete the `docs/_build` folder manually or by running the sphinx make file!\nThis will delete the submodule and might cause issues.\nThe `poe` task is configured to clean all relevant files in the `docs/_build` folder before each run.\n\nAfter an update of the documentation, you will see that you also need to make a commit in the main repo, as the commit \nhash of the docs submodule has changed.\n\nTo make sure you don\'t forget to update the docs, the `poe prepare_release` task will also build and upload the docs \nautomatically.',
     'author': 'Arne Küderle',
     'author_email': 'arne.kuederle@fau.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mad-lab-fau/gaitmap-datasets',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gaitmap_datasets-0.8.0/PKG-INFO` & `gaitmap_datasets-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap-datasets
-Version: 0.8.0
+Version: 0.9.0
 Summary: Helper to access to open-source gait datasets used by MaD-Lab
 Home-page: https://github.com/mad-lab-fau/gaitmap-datasets
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -69,14 +69,15 @@
 
 | Dataset                         | Info Link                                                       | Download                            |
 |---------------------------------|-----------------------------------------------------------------|-------------------------------------|
 | EgaitSegmentationValidation2014 | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |
 | EgaitParameterValidation2013    | https://www.mad.tf.fau.de/research/activitynet/digital-biobank/ | Email to data owner (see info link) |
 | StairAmbulationHealthy2021      | https://osf.io/sgbw7/                                           | https://osf.io/download/5ueq6/      |
 | SensorPositionDataset2019       | https://zenodo.org/record/5747173                               | https://zenodo.org/record/5747173   |
+| EgaitAdidas2014                 | TBD                                                             | TBD                                 |
 
 ### External Datasets
 
 | Dataset    | Info Link                              | Download                                                                                                                          |
 |------------|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | PyShoe2019 | https://github.com/utiasSTARS/pyshoe/  | https://ieee-dataport.org/open-access/university-toronto-foot-mounted-inertial-navigation-dataset (or bash script in github repo) |
```

