# Comparing `tmp/np_workflows-1.4.9.tar.gz` & `tmp/np_workflows-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_workflows-1.4.9.tar", max compression
+gzip compressed data, was "np_workflows-1.5.1.tar", last modified: Wed Jul 12 15:17:52 2023, max compression
```

## Comparing `np_workflows-1.4.9.tar` & `np_workflows-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,60 @@
--rw-r--r--   0        0        0     1330 2023-04-12 00:42:18.794128 np_workflows-1.4.9/pyproject.toml
--rw-r--r--   0        0        0      701 2023-03-17 23:19:28.815209 np_workflows-1.4.9/README.md
--rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.4.9/src/np_workflows/__init__.py
--rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_hab.png
--rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_vis.png
--rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.4.9/src/np_workflows/experiments/__init__.py
--rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/__init__.py
--rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
--rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
--rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
--rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
--rw-r--r--   0        0        0     8512 2023-04-03 20:46:08.140120 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
--rw-r--r--   0        0        0     2335 2023-03-17 23:19:28.826207 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
--rw-r--r--   0        0        0     8693 2023-03-17 23:19:28.828209 np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
--rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.4.9/src/np_workflows/shared/__init__.py
--rw-r--r--   0        0        0    14760 2023-04-03 22:57:54.450052 np_workflows-1.4.9/src/np_workflows/shared/base_experiments.py
--rw-r--r--   0        0        0     6074 2023-03-17 23:19:28.830208 np_workflows-1.4.9/src/np_workflows/shared/npxc.py
--rw-r--r--   0        0        0    25569 2023-04-12 00:38:16.173714 np_workflows-1.4.9/src/np_workflows/shared/widgets.py
--rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 np_workflows-1.4.9/setup.py
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 np_workflows-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1614 2023-06-30 17:48:35.853909 np_workflows-1.5.1/README.md
+-rw-r--r--   0        0        0     2557 2023-07-12 15:17:52.596288 np_workflows-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.5.1/src/np_workflows/__init__.py
+-rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.5.1/src/np_workflows/assets/images/logo_np_hab.png
+-rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.5.1/src/np_workflows/assets/images/logo_np_vis.png
+-rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.5.1/src/np_workflows/experiments/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-18 23:17:52.356257 np_workflows-1.5.1/src/np_workflows/experiments/openscope_barcode/__init__.py
+-rw-r--r--   0        0        0     2737 2023-06-08 01:15:00.774997 np_workflows-1.5.1/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py
+-rw-r--r--   0        0        0     4401 2023-05-11 18:20:25.162316 np_workflows-1.5.1/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.1/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py
+-rw-r--r--   0        0        0     7621 2023-06-05 04:11:33.975384 np_workflows-1.5.1/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py
+-rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-18 01:58:07.942705 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py
+-rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_00.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.949928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_01.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_02.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_03.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_04.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_05.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_06.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.919928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_07.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.889928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_08.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_09.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.859928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_10.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.839929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_11.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.829929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_12.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_13.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.799929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_14.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.789932 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_15.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.769930 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_16.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.759930 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_17.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.749930 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_18.stim
+-rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/flash_250ms.stim
+-rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim
+-rw-r--r--   0        0        0      340 2023-03-08 20:59:00.949928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/old_stim.stim
+-rw-r--r--   0        0        0      334 2023-03-08 20:59:00.959929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed.stim
+-rw-r--r--   0        0        0      345 2023-03-08 20:59:00.979929 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_1st.stim
+-rw-r--r--   0        0        0      346 2023-03-08 20:59:00.969928 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_2nd.stim
+-rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
+-rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
+-rw-r--r--   0        0        0     9220 2023-05-18 02:12:21.002654 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
+-rw-r--r--   0        0        0     2684 2023-06-08 00:43:09.047204 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
+-rw-r--r--   0        0        0     8693 2023-05-24 16:37:52.954146 np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
+-rw-r--r--   0        0        0      200 2023-05-19 23:52:58.915202 np_workflows-1.5.1/src/np_workflows/experiments/templeton/__init__.py
+-rw-r--r--   0        0        0    11540 2023-07-11 23:49:48.276146 np_workflows-1.5.1/src/np_workflows/experiments/templeton/main_templeton_pilot.py
+-rw-r--r--   0        0        0     1779 2023-05-19 23:56:16.341090 np_workflows-1.5.1/src/np_workflows/experiments/templeton/templeton_stim_config.py
+-rw-r--r--   0        0        0     2745 2023-07-11 23:54:16.807727 np_workflows-1.5.1/src/np_workflows/experiments/templeton/templeton_widgets.py
+-rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.5.1/src/np_workflows/shared/__init__.py
+-rw-r--r--   0        0        0    18321 2023-06-23 21:12:38.709724 np_workflows-1.5.1/src/np_workflows/shared/base_experiments.py
+-rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.1/src/np_workflows/shared/camstim_scripts/flash_250ms.stim
+-rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.1/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim
+-rw-r--r--   0        0        0     6258 2023-05-04 01:03:37.729885 np_workflows-1.5.1/src/np_workflows/shared/npxc.py
+-rw-r--r--   0        0        0    25914 2023-06-08 00:33:50.617758 np_workflows-1.5.1/src/np_workflows/shared/widgets.py
+-rw-r--r--   0        0        0   753021 2023-04-14 19:17:10.939361 np_workflows-1.5.1/tests/logs/debug.log
+-rw-r--r--   0        0        0   361698 2023-04-14 19:17:10.939361 np_workflows-1.5.1/tests/logs/warning.log
+-rw-r--r--   0        0        0      508 2023-03-17 23:19:28.833208 np_workflows-1.5.1/tests/model_sandbox.py
+-rw-r--r--   0        0        0    34554 2023-07-11 18:40:27.336659 np_workflows-1.5.1/tests/widget_sandbox.ipynb
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 np_workflows-1.5.1/PKG-INFO
```

### Comparing `np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_hab.png` & `np_workflows-1.5.1/src/np_workflows/assets/images/logo_np_hab.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/assets/images/logo_np_vis.png` & `np_workflows-1.5.1/src/np_workflows/assets/images/logo_np_vis.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py` & `np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py` & `np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py` & `np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py` & `np_workflows-1.5.1/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py` & `np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,24 @@
     @property
     def script_names(self) -> dict[Literal["main", "mapping", "opto"], str]:
         return {
             label: f"ttn_{label}_script.py" for label in ("main", "mapping", "opto")
         }
         
     @property
+    def stim_root_on_stim(self) -> pathlib.Path:
+        "Path to dev folder on Stim computer, as seen from local machine."
+        return np_config.local_to_unc(self.rig.stim, self.script_root_on_stim)
+    
+    @property
+    def stim_root_on_local(self) -> pathlib.Path:
+        "Path to version controlled stim files on local machine."
+        return self.script_root_on_local / 'stims'
+        
+    @property
     def recorders(self) -> tuple[Service, ...]:
         """Services to be started before stimuli run, and stopped after. Session-dependent."""
         match self.ttn_session:
             case TTNSession.PRETEST | TTNSession.EPHYS:
                 return (Sync, VideoMVR, OpenEphys)
             case TTNSession.HAB_60 | TTNSession.HAB_90 | TTNSession.HAB_120:
                 return (Sync, VideoMVR)
@@ -93,14 +103,15 @@
         NewScaleCoordinateRecorder.log_root = self.session.npexp_path
         NewScaleCoordinateRecorder.log_name = self.platform_json.path.name
 
         self.configure_services()
 
         super().initialize_and_test_services()
 
+
     def update_state(self) -> None:
         "Store useful but non-essential info."
         self.mouse.state['last_session'] = self.session.id
         self.mouse.state['last_ttn_session'] = str(self.ttn_session)
         if self.mouse == 366122:
             return
         match self.ttn_session:
@@ -109,15 +120,15 @@
             case TTNSession.HAB_60 | TTNSession.HAB_90 | TTNSession.HAB_120:
                 self.session.project.state['latest_hab'] = self.session.id
             case TTNSession.EPHYS:
                 self.session.project.state['latest_ephys'] = self.session.id
                 self.session.project.state['sessions'] = self.session.project.state.get('sessions', []) + [self.session.id]
                 
     def run_stim_scripts(self) -> None:
-
+        self.validate_or_copy_stim_files()
         self.update_state()
         
         for stim in ('mapping', 'main', 'opto'):
             
             if not (params := self.params[stim]):
                 logger.info("%s script skipped this session: %r", stim, self.ttn_session)
                 continue
@@ -137,15 +148,19 @@
                     time.sleep(2.5)
                 
             if isinstance(ScriptCamstim, Finalizable):
                 ScriptCamstim.finalize()
 
             with contextlib.suppress(Exception):
                 np_logging.web(f'ttn_{self.ttn_session.name.lower()}').info(f"{stim.capitalize()} stim finished")
-            
+    
+    def validate_or_copy_stim_files(self):
+        for vc_copy in self.stim_root_on_local.iterdir():
+            stim_copy = self.stim_root_on_stim / vc_copy.name
+            validate_or_overwrite(validate=stim_copy, src=vc_copy)
             
     @property
     def params(self) -> dict[Literal["main", "mapping", "opto", "system"], dict[str, Any]]:
         params = copy.deepcopy(DEFAULT_STIM_PARAMS)
         if system := self.system_camstim_params:
             params["system"] = system
         params["main"] = per_session_main_stim_params(self.ttn_session)
@@ -175,28 +190,28 @@
 
     @functools.cached_property
     def system_camstim_params(self) -> dict[str, Any]:
         "System config on Stim computer, if accessible."
         return camstim_defaults()
     
     
-class Hab(TTNMixin, np_workflows.Hab):
+class Hab(TTNMixin, np_workflows.PipelineHab):
     def __init__(self, *args, **kwargs):
         self.services = (
             MouseDirector,
             Sync,
             VideoMVR,
             self.imager,
             NewScaleCoordinateRecorder,
             ScriptCamstim,
         )
         super().__init__(*args, **kwargs)
 
 
-class Ephys(TTNMixin, np_workflows.Ephys):
+class Ephys(TTNMixin, np_workflows.PipelineEphys):
     def __init__(self, *args, **kwargs):
         self.services = (
             MouseDirector,
             Sync,
             VideoMVR,
             self.imager,
             NewScaleCoordinateRecorder,
```

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py` & `np_workflows-1.5.1/src/np_workflows/experiments/templeton/templeton_widgets.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,63 +9,68 @@
 import ipywidgets as ipw
 import np_config
 import np_logging
 import np_session
 import np_workflows
 from pyparsing import Any
 
-from .ttn_stim_config import TTNSession
+from np_workflows.experiments.templeton.templeton_stim_config import TempletonWorkflow, AVAILABLE_TASK_NAMES
+from np_workflows.experiments.templeton.main_templeton_pilot import Ephys, Hab
 
 # for widget, before creating a experiment --------------------------------------------- #
 
 
-class TTNSelectedSession:
-    def __init__(self, session: str | TTNSession, mouse: str | int | np_session.Mouse):
-        if isinstance(session, str):
-            session = TTNSession(session)
-        self.session = session
+class TempletonSelectedWorkflow:
+    def __init__(self, workflow: str | TempletonWorkflow, mouse: str | int | np_session.Mouse):
+        if isinstance(workflow, str):
+            workflow = TempletonWorkflow(workflow)
+        self.workflow = workflow
         self.mouse = str(mouse)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.session}, {self.mouse})"
+        return f"{self.__class__.__name__}({self.workflow}, {self.mouse})"
 
 
-def stim_session_select_widget(
+def workflow_select_widget(
     mouse: str | int | np_session.Mouse,
-) -> TTNSelectedSession:
+) -> TempletonSelectedWorkflow:
     """Select a stimulus session (hab, pretest, ephys) to run.
 
     An object with mutable attributes is returned, so the selected session can be
     updated along with the GUI selection. (Preference would be to return an enum
     directly, and change it's value, but that doesn't seem possible.)
 
     """
 
-    selection = TTNSelectedSession(TTNSession.PRETEST, mouse)
+    selection = TempletonSelectedWorkflow(TempletonWorkflow.PRETEST, mouse)
 
-    session_dropdown = ipw.Select(
-        options=tuple(_.value for _ in TTNSession),
-        description="Session",
+    workflow_dropdown = ipw.Select(
+        options=tuple(_.value for _ in TempletonWorkflow),
+        description="Workflow",
     )
     console = ipw.Output()
     with console:
-        if last_session := np_session.Mouse(selection.mouse).state.get('last_ttn_session'):
-            print(f"{mouse} last session: {last_session}")
-        print(f"Selected: {selection.session}")
+        if last_workflow := np_session.Mouse(selection.mouse).state.get('last_workflow'):
+            print(f"{mouse} last workflow: {TempletonWorkflow[last_workflow].value}")
+        print(f"Selected: {selection.workflow.name}")
 
     def update(change):
         if change["name"] != "value":
             return
         if (options := getattr(change["owner"], "options", None)) and change[
             "new"
         ] not in options:
             return
         if change["new"] == change["old"]:
             return
-        selection.__init__(str(session_dropdown.value), mouse.id if isinstance(mouse, np_session.Mouse) else str(mouse))
+        selection.__init__(str(workflow_dropdown.value), mouse.id if isinstance(mouse, np_session.Mouse) else str(mouse))
         with console:
-            print(f"Selected: {selection.session}")
-    session_dropdown.observe(update, names='value')
+            print(f"Selected: {selection.workflow}")
+    workflow_dropdown.observe(update, names='value')
 
-    IPython.display.display(ipw.VBox([session_dropdown, console]))
+    IPython.display.display(ipw.VBox([workflow_dropdown, console]))
 
     return selection
+
+
+def photodoc_widget(session: np_session.Session, reminder: str) -> None: 
+    print(f'Take an image in Vimba Viewer and save as:\n{session.npexp_path / reminder}.png')
```

### Comparing `np_workflows-1.4.9/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py` & `np_workflows-1.5.1/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.4.9/src/np_workflows/shared/base_experiments.py` & `np_workflows-1.5.1/src/np_workflows/shared/base_experiments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+import configparser
 import contextlib
 import functools
 import getpass
 import pathlib
 import re
 import shutil
 import time
@@ -30,56 +31,72 @@
     Validatable,
     Shutdownable,
 )
 
 
 logger = np_logging.getLogger(__name__)
 
+class WithSessionInfo(Protocol):
+    @property
+    def session(self) -> np_session.Session: ...
+    @property
+    def mouse(self) -> np_session.Mouse: ...
+    @property
+    def user(self) -> np_session.User: ...
+    @property
+    def rig(self) -> np_config.Rig: ...
+    
 
-class WithLims(abc.ABC):
+class WithSession(abc.ABC):
     
+    default_session_subclass: ClassVar[Type[np_session.Session]] = np_session.PipelineSession
     default_session_type: Literal['ephys', 'hab'] = 'ephys'
     
     services: tuple[Service, ...] = ()
-    "Devices, databases, etc."
+    "All services. Devices, databases, etc."
 
+    @property
+    @abc.abstractmethod
+    def recorders(self) -> tuple[Startable | Stoppable, ...]:
+        """Services that record data. These are started and stopped as a group."""
+        return NotImplemented
+    
     def __init__(self, 
         mouse: Optional[str | int |  np_session.LIMS2MouseInfo] = None,
         operator: Optional[str | np_session.LIMS2UserInfo] = None, 
-        session: Optional[str | pathlib.Path | int | np_session.Session] = None,
+        session: Optional[str | pathlib.Path | int | np_session.PipelineSession] = None,
         session_type: Optional[Literal['ephys', 'hab']] = None,
         **kwargs,
         ):
         
         if session and not isinstance(session, np_session.Session):
             session = np_session.Session(session)
             logger.debug('%s | Initialized with existing session %s', self.__class__.__name__, session)
             if session_type and ((a := session_type == 'hab') != (b := session.is_hab)):
                 logger.warning('session_type arg specified (%r) does not match that of supplied %r: %r', a, b, session)
         elif operator and mouse:
             logger.debug('%s | Creating new session for mouse %r, operator %r', self.__class__.__name__, mouse, operator)
-            session = np_session.generate_session(mouse, operator, session_type or self.default_session_type)
+            session = self.generate_session(mouse, operator, session_type or self.default_session_type)
         else:
             raise ValueError('Must specify either a mouse + operator, or an existing session')
 
         self.session = session
             
         self.configure_services()
         self.session.npexp_path.mkdir(parents=True, exist_ok=True)
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.session})'
     
+    @classmethod
+    def generate_session(cls, *args, **kwargs):
+        return cls.default_session_subclass.new(*args, **kwargs)
+        
     @property
-    def platform_json(self) -> np_session.PlatformJson:
-        self.session.platform_json.update('rig_id', str(self.rig))
-        return self.session.platform_json
-    
-    @property
-    def session(self) -> np_session.Session:
+    def session(self) -> np_session.PipelineSession:
         return self._session
         
     @session.setter
     def session(self, value: str | np_session.Session | pathlib.Path | int | np_session.LIMS2SessionInfo):
         self._session = np_session.Session(value) if not isinstance(value, np_session.Session) else value
         logger.debug('Set experiment.session to %r', self._session)
     
@@ -92,30 +109,32 @@
                 return 'hab'
             return 'ephys'
         raise AttributeError('Session has not been set')
     
     @session_type.setter
     def session_type(self, value: Literal['ephys', 'hab']):
         if value not in ('ephys', 'hab'):
-            raise ValueError('Session type must be either "ephys" or "hab"')
+            raise ValueError(f'Session type must be either "ephys" or "hab": got {value!r}')
         self._session_type = value
         logger.debug('Set session_type to %r', value)
         
     @property
     def rig(self) -> np_config.Rig | None:
         "Computer hostnames and configuration for the rig we're currently on."
         with contextlib.suppress(AttributeError):
             return self._rig
         with contextlib.suppress(ValueError):
             self._rig = np_config.Rig()
             return self.rig
     
     @property
     def mouse(self) -> np_session.Mouse:
-        return self.session.mouse
+        if isinstance(self.session.mouse, str | int):
+            return np_session.Mouse(self.session.mouse)
+        return self.session.mouse 
     
     @property
     def user(self) -> np_session.User | None:
         return self.session.user
     
     @property
     def imager(self) -> Type[np_services.Cam3d] | Type[np_services.ImageMVR]:
@@ -170,32 +189,32 @@
         stoppables = tuple(_ for _ in recorders if isinstance(_, Stoppable))
         with np_services.stop_on_error(*stoppables):
             for recorder in recorders:
                 recorder.start()
                 time.sleep(2)
                 if isinstance(recorder, Verifiable):
                     recorder.verify()
-        self.platform_json.ExperimentStartTime = npxc.now()        
-        self.platform_json.write()
     
     def stop_recording_after_stim_finished(self, 
-            recorders: Optional[Iterable[Startable]] = None, 
-            stims: Optional[Iterable[Startable]] = None,
+            recorders: Optional[Iterable[Stoppable]] = None, 
+            stims: Optional[Iterable[Stoppable]] = None,
         ) -> None:
-        """Stop recording after all stims have finished."""
+        """Stop recording after all stims have finished.
+        
+        - object's `.recorders` attr used by default, stopped in reverse order.
+        - stims will be awaited
+        """
         if not recorders and hasattr(self, 'recorders'):
-            recorders = self.recorders
+            recorders = reversed(self.recorders)
         if not stims and hasattr(self, 'stims'):
             stims = self.stims
         while not all(_.is_ready_to_start() for _ in stims):
             time.sleep(5)
         for stoppable in (_ for _ in recorders if isinstance(_, Stoppable)):
             stoppable.stop()
-        self.platform_json.ExperimentCompleteTime = npxc.now()        
-        self.platform_json.write()
                 
     def start_services(self, *services: Service) -> None:
         if not services:
             services = self.services
         for service in (_ for _ in services if isinstance(_, Startable)):
             service.start()
             if isinstance(service, Verifiable):
@@ -228,14 +247,75 @@
     def copy_files(self) -> None:
         """Copy files from raw data storage to session folder for all services."""
         self.copy_data_files()
         self.copy_workflow_files()
         if self.session_type != 'hab':
             self.copy_ephys()
     
+    @abc.abstractmethod
+    def copy_data_files(self) -> None:
+        """Copy files from raw data storage to session folder for all services."""
+        return NotImplemented
+    
+    @abc.abstractmethod
+    def copy_ephys(self) -> None:
+        """Copy ephys data from Acq to session folder."""
+        return NotImplemented
+    
+    def copy_workflow_files(self) -> None:
+        """Copy working directory (with ipynb, logs folder) and lock/pyproject files
+        from np_notebooks root."""
+
+        self.save_current_notebook()
+        
+        cwd = pathlib.Path('.').resolve()
+        dest = self.session.npexp_path / 'exp'
+        dest.mkdir(exist_ok=True, parents=True)
+
+        shutil.copytree(cwd, dest, dirs_exist_ok=True)
+
+        lock = cwd.parent / 'pdm.lock'
+        pyproject = cwd.parent / 'pyproject.toml'
+        
+        for _ in (lock, pyproject):
+            shutil.copy2(_, dest)
+        
+    def save_current_notebook(self) -> None:
+        app = ipylab.JupyterFrontEnd()
+        app.commands.execute('docmanager:save')
+        # TODO use the following to export to html (shows input to widgets and
+        # output of cells)
+        #! currently can't be run automatically as save as path dialog opens 
+        # app.commands.execute('notebook:export-to-format', {
+        #     'format': 'html',
+        #     # 'download': 'false',
+        #     # 'path': 'c:/users/svc_neuropix/documents/github/np_notebooks/task_trained_network/ttn_pilot.html',
+        # })       
+        
+class PipelineExperiment(WithSession):
+    @property
+    def platform_json(self) -> np_session.PlatformJson:
+        self.session.platform_json.update('rig_id', str(self.rig))
+        return self.session.platform_json
+    
+    def start_recording(self, *recorders: Startable) -> None:
+        super().start_recording(*recorders)
+        self.platform_json.ExperimentStartTime = npxc.now()        
+        self.platform_json.write()
+
+
+    def stop_recording_after_stim_finished(self, 
+            recorders: Optional[Iterable[Stoppable]] = None, 
+            stims: Optional[Iterable[Stoppable]] = None,
+        ) -> None:
+        """Stop recording after all stims have finished."""
+        super().stop_recording_after_stim_finished(recorders, stims)
+        self.platform_json.ExperimentCompleteTime = npxc.now()        
+        self.platform_json.write()
+                                   
     def rename_split_ephys_folders(self) -> None:
         "Add `_probeABC` or `_probeDEF` to ephys folders recorded on two drives."
         folders = np_services.OpenEphys.data_files
         if not folders:
             logger.info('Renaming: no ephys folders have been recorded')
         renamed_folders = []
         for name in set(_.name for _ in folders):
@@ -293,49 +373,54 @@
                                     'post_experiment_surface_image_left': '_surface-image6-left',
                                     'post_experiment_surface_image_right': '_surface-image6-right',
                                 }.items():
                                 if lims_label in file.name:
                                     renamed = f'{self.session.folder}{img_label}{file.suffix}'
                         shutil.copy2(file, self.session.npexp_path / (renamed or file.name))
                         
-    def copy_workflow_files(self) -> None:
-        """Copy working directory (with ipynb, logs folder) and lock/pyproject files
-        from np_notebooks root."""
-
-        self.save_current_notebook()
-        
-        cwd = pathlib.Path('.').resolve()
-        dest = self.session.npexp_path / 'exp'
-        dest.mkdir(exist_ok=True, parents=True)
-
-        shutil.copytree(cwd, dest, dirs_exist_ok=True)
-
-        lock = cwd.parent / 'pdm.lock'
-        pyproject = cwd.parent / 'pyproject.toml'
-        
-        for _ in (lock, pyproject):
-            shutil.copy2(_, dest)
-        
-    def save_current_notebook(self) -> None:
-        app = ipylab.JupyterFrontEnd()
-        app.commands.execute('docmanager:save')
-        
     def copy_ephys(self) -> None:
         # copy ephys       
         self.rename_split_ephys_folders()
         password = np_config.fetch('/logins')['svc_neuropix']['password']
         ssh = fabric.Connection(host=np_services.OpenEphys.host, user='svc_neuropix', connect_kwargs=dict(password=password))
         for ephys_folder in np_services.OpenEphys.data_files:
             with contextlib.suppress(Exception):
                 with ssh:
                     ssh.run(
-                    f'robocopy "{ephys_folder}" "{self.session.npexp_path / ephys_folder.name} /j /s /xo' 
+                    f'robocopy "{ephys_folder}" "{self.session.npexp_path / ephys_folder.name}" /j /s /xo' 
                     # /j unbuffered, /s incl non-empty subdirs, /xo exclude src files older than dest
-                    ) 
-                           
-                           
-class Ephys(WithLims):
+                    )
+    
+    @functools.cached_property
+    def system_camstim_params(self) -> dict[str, Any]:
+        """Try to load defaults from camstim config file on the Stim computer.
+        
+        May encounter permission error if not running as svc_neuropix.
+        """
+        with contextlib.suppress(OSError):
+            parser = configparser.RawConfigParser()
+            parser.read(
+                (self.rig.paths["Camstim"].parent / "config" / "stim.cfg").as_posix()
+            )
+
+            camstim_default_config = {}
+            for section in parser.sections():
+                camstim_default_config[section] = {}
+                for k, v in parser[section].items():
+                    try:
+                        value = eval(
+                            v
+                        )  # this removes comments in config and converts values to expected datatype
+                    except:
+                        continue
+                    else:
+                        camstim_default_config[section][k] = value
+            return camstim_default_config
+        logger.warning("Could not load camstim defaults from config file on Stim computer.")
+        return {}
+
+class PipelineEphys(PipelineExperiment):
     default_session_type = 'ephys'
 
 
-class Hab(WithLims):
+class PipelineHab(PipelineExperiment):
     default_session_type = 'hab'
```

### Comparing `np_workflows-1.4.9/src/np_workflows/shared/npxc.py` & `np_workflows-1.5.1/src/np_workflows/shared/npxc.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,20 +120,25 @@
                     files = service.data_files or service.get_latest_data('*')
                     if not files:
                         continue
                     files = set(files)
                     print(files)
                     for file in files:
                         shutil.copy2(file, session_folder)
-                    
-    # copy ephys                    
-    for ephys_folder in OpenEphys.data_files:
-        fabric.Connection(host=OpenEphys.host, user='svc_neuropix', connect_kwargs=dict(password=password)).run(
-            f'robocopy "{ephys_folder}" "{session_folder}" /j /s /xo' # /j unbuffered, /s incl non-empty subdirs, /xo exclude src files older than dest
-        ) 
+    
+    password = np_config.fetch('/logins')['svc_neuropix']['password']
+    ssh = fabric.Connection(host=np_services.OpenEphys.host, user='svc_neuropix', connect_kwargs=dict(password=password))
+    for ephys_folder in np_services.OpenEphys.data_files:
+
+        with contextlib.suppress(Exception):
+            with ssh:
+                ssh.run(
+                f'robocopy "{ephys_folder}" "{session_folder / ephys_folder.name}" /j /s /xo' 
+                # /j unbuffered, /s incl non-empty subdirs, /xo exclude src files older than dest
+                )
             
             
 import warnings
 
 def hide_warning_lines(msg:str,category:str,*args,**kwargs):
     print("\n{}: {}\n".format(category.__name__, msg))
 warnings.showwarning = hide_warning_lines
```

### Comparing `np_workflows-1.4.9/src/np_workflows/shared/widgets.py` & `np_workflows-1.5.1/src/np_workflows/shared/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import np_workflows.shared.npxc as npxc
 
 logger = np_logging.getLogger(__name__)
 
 np_logging.getLogger('Comm').propagate = False
 np_logging.getLogger('PIL').propagate = False
 
+global_state = {}
+"""Global variable for persisting widget states."""
 
 def elapsed_time_widget() -> IPython.display.DisplayHandle | None:
     """Displays a clock showing the elapsed time since the cell was first run."""
 
     clock_widget = ipw.Label("")
     reminder_widget = ipw.Label("Remember to restart JupyterLab and run update.bat before every experiment!")
     global start_time
@@ -51,34 +53,41 @@
 
     thread = threading.Thread(target=update_timer, args=())
     thread.start()
     return IPython.display.display(ipw.VBox([clock_widget, reminder_widget]))
 
 
 def user_and_mouse_widget() -> tuple[np_session.User, np_session.Mouse]:
+    console = ipw.Output()
     user_description = "User:"
     mouse_description = "Mouse:"
     user_widget = ipw.Select(options=npxc.lims_user_ids, description=user_description)
     mouse_widget = ipw.Text(value=str(npxc.default_mouse_id), description=mouse_description)
+    for widget, string in zip((user_widget, mouse_widget), ('user', 'mouse')):
+        if (selected := global_state.get(f'selected_{string}')):
+            widget.value = selected
+            with console:
+                print(f'Current {string}: {selected}')
     user = np_session.User(str(user_widget.value))
     mouse = np_session.Mouse(str(mouse_widget.value))
-    console = ipw.Output()
 
     def update_user(new_user: str):
         if str(user) == (new := str(new_user).strip()):
             return
         user.__init__(new)
+        global_state['selected_user'] = new
         with console:
             print(f"User updated: {user}")
 
     def update_mouse(new_mouse: str):
         if str(mouse) == (new := str(new_mouse).strip()):
             return
         if len(new) < 6:
             return
+        global_state['selected_mouse'] = new
         mouse.__init__(new)
         with console:
             print(f"Mouse updated: {mouse}")
         
     def new_value(change) -> None:
         if change['name'] != 'value':
             return
@@ -271,15 +280,15 @@
         "Add quickcast etc.",
         "Remove and water mouse", 
         "Dip probes",     
     )
     IPython.display.display(widget := check_widget(check, *checks))
     
     
-def wheel_height_widget(session: np_session.Session) -> IPython.display.DisplayHandle | None:
+def wheel_height_widget(session: np_session.PipelineSession) -> IPython.display.DisplayHandle | None:
     "Saves wheel height to platform_json and stores in `mouse.state['wheel_height']`."
     
     layout = ipw.Layout(max_width='130px')
     
     prev_height = session.mouse.state.get('wheel_height', 0)
     height_counter = ipw.BoundedFloatText(value=prev_height, min=0, max=10, step=0.1, description="Wheel height", layout=layout)
     save_button = ipw.Button(description='Save', button_style='warning', layout=layout)
@@ -289,15 +298,15 @@
         session.mouse.state['wheel_height'] = height_counter.value
         save_button.button_style = 'success'
         save_button.description = 'Saved'
     save_button.on_click(on_click)
     return IPython.display.display(ipw.VBox([height_counter,save_button]))
     
 
-def di_widget(session: np_session.Session) -> IPython.display.DisplayHandle | None:
+def di_widget(session: np_session.PipelineSession) -> IPython.display.DisplayHandle | None:
     "Supply a path or a platform json instance. Saves a JSON file with the dye used in the session and a timestamp."
     
     di_info: dict[str, int | str] = dict(
         EndTime=0, StartTime=npxc.now(), dii_description="", times_dipped=0, previous_uses="",
     )
     di_info.update(session.platform_json.DiINotes)
     
@@ -321,15 +330,15 @@
         
     save_button.on_click(on_click)
     return IPython.display.display(ipw.VBox([
         dipped_counter, dye_dropdown, 
         usage_counter, save_button]))
 
     
-def dye_info_widget(session: np_session.Session) -> IPython.display.DisplayHandle | None:
+def dye_info_widget(session: np_session.PipelineSession) -> IPython.display.DisplayHandle | None:
     """
     - scan barcode or enter ID number for the dye used
     - change dye description if incorrect (DiI, DiO)
     - increment number of times probes were dipped this session
     - hit `Save` to store info in platform.json
     """
     
@@ -340,33 +349,31 @@
     
     width = lambda w: ipw.Layout(max_width=f'{w}px')
     
     dye_id_entry = ipw.Text(value=None, description='Dye ID', layout=width(250), placeholder='Enter ID or scan barcode')
     dye_usage_button = ipw.Button(description='Record single use', button_style='warning', layout=width(180))
     first_usage = ipw.Text(value='', description="First use", layout=width(250), disabled=True)
     dye_dropdown = ipw.Dropdown(description="Description:", options=np_session.Dye.descriptions, layout=width(180))
-    dipped_counter = ipw.IntText(value=di_info['times_dipped'], min=0, max=99, description="Dipped count", layout=width(150))
-    usage_counter = ipw.IntText(value=int(di_info['previous_uses']), min=0, max=99, description="Previous uses", layout=width(180), disabled=True)
+    dipped_counter = ipw.IntText(value=int(di_info['times_dipped'] or 0), min=0, max=99, description="Dipped count", layout=width(150))
+    usage_counter = ipw.IntText(value=int(di_info['previous_uses'] or 0), min=0, max=99, description="Previous uses", layout=width(180), disabled=True)
     save_button = ipw.Button(description='Save', button_style='warning', layout=width(180))
     if (desc := di_info['dii_description']) in np_session.Dye.descriptions:
         dye_dropdown.value = desc
         
     def update_display(_):
-        with contextlib.suppress(Exception):
-            dye = np_session.Dye(int(str(dye_id_entry.value)))
-            dye_dropdown.value = dye.description
-            usage_counter.value = dye.previous_uses
-            first_usage.value = f'{dye.first_use}'
+        dye = np_session.Dye(int(str(dye_id_entry.value)))
+        dye_dropdown.value = dye.description
+        usage_counter.value = dye.previous_uses
+        first_usage.value = f'{dye.first_use}'
     dye_id_entry.observe(update_display, 'value')
     
     def record_dye_usage():
-        with contextlib.suppress(Exception):
-            dye = np_session.Dye(int(str(dye_id_entry.value)))
-            dye.description = dye_dropdown.value
-            dye.increment_uses()
+        dye = np_session.Dye(int(str(dye_id_entry.value)))
+        dye.description = dye_dropdown.value
+        dye.increment_uses()
         
     def update_di_info():
         di_info['EndTime'] = npxc.now()
         di_info['times_dipped'] = str(dipped_counter.value)
         di_info['dii_description'] = str(dye_dropdown.value)
         di_info['previous_uses'] = str(usage_counter.value)
         
@@ -465,15 +472,15 @@
     # alternative to use ipw with toggle button -------------------------------------------- #
     # import io
     # membuf = io.BytesIO()
     # img.save(membuf, format="png") 
     # return IPython.display.display(ipw.VBox([ipw.Image(value=membuf.getvalue())]))
 
 
-def insertion_notes_widget(session: np_session.Session):
+def insertion_notes_widget(session: np_session.PipelineSession):
     
     probes = 'ABCDEF'
     probe = lambda _: f'Probe{_}'
     fields = (
         "FailedToInsert",
         # "ProbeLocationChanged",
         # "ProbeBendingOnSurface",
@@ -502,33 +509,33 @@
     
     def save(b):
         d = {}
         for letter, row in zip(probes, rows):
             p = d.get(probe(letter), {})
             for widget in row.children:
                 v = widget.value
-                if v in (None, False, ''):
-                    continue
                 if isinstance(widget, ipw.Text):
                     p['Notes'] = widget.value
-                if isinstance(widget, ipw.Checkbox):
+                elif isinstance(widget, ipw.Checkbox):
                     p[save_str(widget.description)] = widget.value
+                else:
+                    continue
             if p:
                 d[probe(letter)] = p  
         
         session.platform_json.InsertionNotes = d 
         with console:
             print('Updated notes')
         button.button_style = 'success'
         
     button.on_click(save)
     return IPython.display.display(widget)
 
 
-def probe_depth_widget(session: np_session.Session):
+def probe_depth_widget(session: np_session.PipelineSession):
     
     probes = 'ABCDEF'
     
     coords = lambda: session.platform_json.manipulator_coordinates
     
     if not coords():
         logger.warning("No photodocs have been captured yet.")
```

