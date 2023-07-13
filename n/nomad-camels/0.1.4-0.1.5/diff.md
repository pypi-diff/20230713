# Comparing `tmp/nomad_camels-0.1.4.tar.gz` & `tmp/nomad_camels-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels-0.1.4.tar", last modified: Thu Jul  6 12:20:13 2023, max compression
+gzip compressed data, was "nomad_camels-0.1.5.tar", last modified: Thu Jul 13 12:51:19 2023, max compression
```

## Comparing `nomad_camels-0.1.4.tar` & `nomad_camels-0.1.5.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/
--rw-rw-rw-   0        0        0    26526 2023-06-28 14:51:17.000000 nomad_camels-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    26525 2023-06-28 14:51:17.000000 nomad_camels-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       27 2023-06-28 14:51:17.000000 nomad_camels-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2317 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1654 2023-07-06 07:41:24.000000 nomad_camels-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.415637 nomad_camels-0.1.4/nomad_camels/
--rw-rw-rw-   0        0        0     4227 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/CAMELS_start.py
--rw-rw-rw-   0        0        0    43072 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/MainApp_v2.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.495956 nomad_camels-0.1.4/nomad_camels/bluesky_handling/
--rw-rw-rw-   0        0        0     5236 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/EpicsFieldSignal.py
--rw-rw-rw-   0        0        0     1827 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/__init__.py
--rw-rw-rw-   0        0        0     6047 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/builder_helper_functions.py
--rw-rw-rw-   0        0        0     4103 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/custom_function_signal.py
--rw-rw-rw-   0        0        0     4841 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/evaluation_helper.py
--rw-rw-rw-   0        0        0    22693 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/helper_functions.py
--rw-rw-rw-   0        0        0     1915 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/make_catalog.py
--rw-rw-rw-   0        0        0    16474 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/protocol_builder.py
--rw-rw-rw-   0        0        0      885 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/special_plan_stubs.py
--rw-rw-rw-   0        0        0    10686 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/visa_signal.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.497955 nomad_camels-0.1.4/nomad_camels/commands/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/commands/__init__.py
--rw-rw-rw-   0        0        0     5509 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/commands/change_sequence.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.593931 nomad_camels-0.1.4/nomad_camels/frontpanels/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/__init__.py
--rw-rw-rw-   0        0        0     9749 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/device_add_dialog.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.632724 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/__init__.py
--rw-rw-rw-   0        0        0     8771 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
--rw-rw-rw-   0        0        0      830 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
--rw-rw-rw-   0        0        0      236 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/pass_ask.py
--rw-rw-rw-   0        0        0    10082 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_config.py
--rw-rw-rw-   0        0        0    13171 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_installer.py
--rw-rw-rw-   0        0        0     2925 2023-06-29 11:51:05.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/manage_instruments.py
--rw-rw-rw-   0        0        0    22774 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/plot_definer.py
--rw-rw-rw-   0        0        0    22381 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/protocol_config.py
--rw-rw-rw-   0        0        0     8557 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/settings_window.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.716860 nomad_camels-0.1.4/nomad_camels/graphics/
--rw-rw-rw-   0        0        0    16958 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/CAMELS.ico
--rw-rw-rw-   0        0        0     2926 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/CAMELS_Icon.png
--rw-rw-rw-   0        0        0   101760 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
--rw-rw-rw-   0        0        0   479310 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
--rw-rw-rw-   0        0        0    13283 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels-horizontal.svg
--rw-rw-rw-   0        0        0    13715 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels-vertical.svg
--rw-rw-rw-   0        0        0    12919 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels_horizontal.png
--rw-rw-rw-   0        0        0    19245 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels_vertical.png
--rw-rw-rw-   0        0        0    40043 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/dark.qss
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.808157 nomad_camels-0.1.4/nomad_camels/graphics/legacy/
--rw-rw-rw-   0        0        0    60728 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS.svg
--rw-rw-rw-   0        0        0    52644 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon.png
--rw-rw-rw-   0        0        0   349358 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
--rw-rw-rw-   0        0        0    34101 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
--rw-rw-rw-   0        0        0    42984 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.png
--rw-rw-rw-   0        0        0    43703 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.svg
--rw-rw-rw-   0        0        0    96186 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
--rw-rw-rw-   0        0        0    18507 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_V1.svg
--rw-rw-rw-   0        0        0    20058 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_v2.svg
--rw-rw-rw-   0        0        0   290607 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels - Kopie.png
--rw-rw-rw-   0        0        0   252699 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels_free.png
--rw-rw-rw-   0        0        0     7058 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/plus_sign.png
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.896284 nomad_camels-0.1.4/nomad_camels/gui/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/__init__.py
--rw-rw-rw-   0        0        0     6130 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/addDeviceDialog.py
--rw-rw-rw-   0        0        0     5535 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/device_installer.py
--rw-rw-rw-   0        0        0     2841 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/enterTextDialog.py
--rw-rw-rw-   0        0        0     4027 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/fit_definer.py
--rw-rw-rw-   0        0        0    11001 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/for_loop.py
--rw-rw-rw-   0        0        0     6623 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/general_protocol_settings.py
--rw-rw-rw-   0        0        0     8501 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/gradient_descent_step.py
--rw-rw-rw-   0        0        0     4572 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/instrument_config.py
--rw-rw-rw-   0        0        0    22581 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/gui/mainWindow_v2.py
--rw-rw-rw-   0        0        0     2893 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/pass_ask.py
--rw-rw-rw-   0        0        0     7219 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/plot_definer.py
--rw-rw-rw-   0        0        0     6027 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/plot_definer_2d.py
--rw-rw-rw-   0        0        0     3885 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/plot_options.py
--rw-rw-rw-   0        0        0     7230 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/protocol_view.py
--rw-rw-rw-   0        0        0     2537 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/read_channels.py
--rw-rw-rw-   0        0        0     1465 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/set_channels.py
--rw-rw-rw-   0        0        0    13462 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/settings_window.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.016280 nomad_camels-0.1.4/nomad_camels/loop_steps/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/__init__.py
--rw-rw-rw-   0        0        0     4577 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/change_device_config.py
--rw-rw-rw-   0        0        0    28468 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/for_while_loops.py
--rw-rw-rw-   0        0        0    10275 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/gradient_descent.py
--rw-rw-rw-   0        0        0     9981 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/if_step.py
--rw-rw-rw-   0        0        0     5520 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/make_step_of_type.py
--rw-rw-rw-   0        0        0    14155 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/nd_sweep.py
--rw-rw-rw-   0        0        0     3550 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/prompt_loop_step.py
--rw-rw-rw-   0        0        0    15156 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/read_channels.py
--rw-rw-rw-   0        0        0     7679 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/run_subprotocol.py
--rw-rw-rw-   0        0        0     4488 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/set_channels.py
--rw-rw-rw-   0        0        0     4099 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/set_value_popup.py
--rw-rw-rw-   0        0        0     2383 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/set_variables.py
--rw-rw-rw-   0        0        0    14715 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/simple_sweep.py
--rw-rw-rw-   0        0        0     2648 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/wait_loop_step.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.126276 nomad_camels-0.1.4/nomad_camels/main_classes/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/__init__.py
--rw-rw-rw-   0        0        0    29151 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/main_classes/device_class.py
--rw-rw-rw-   0        0        0     3595 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/list_plot.py
--rw-rw-rw-   0        0        0    12119 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/main_classes/loop_step.py
--rw-rw-rw-   0        0        0     3993 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/manual_control.py
--rw-rw-rw-   0        0        0     1242 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/measurement_channel.py
--rw-rw-rw-   0        0        0     7869 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/plot_2D.py
--rw-rw-rw-   0        0        0    48782 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/plot_widget.py
--rw-rw-rw-   0        0        0    21225 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/main_classes/protocol_class.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.126276 nomad_camels-0.1.4/nomad_camels/manual_controls/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/get_manual_controls.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.156276 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/__init__.py
--rw-rw-rw-   0        0        0    20282 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/stage_control.py
--rw-rw-rw-   0        0        0    12048 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/ui_stage_control.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.186277 nomad_camels-0.1.4/nomad_camels/tests/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tests/__init__.py
--rw-rw-rw-   0        0        0     3182 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/tests/instrument_management_test.py
--rw-rw-rw-   0        0        0    20124 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/tests/protocol_test.py
--rw-rw-rw-   0        0        0      768 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tests/startup_test.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.206264 nomad_camels-0.1.4/nomad_camels/tools/
--rw-rw-rw-   0        0        0     8933 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/tools/EPICS_driver_builder.py
--rw-rw-rw-   0        0        0     5627 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tools/VISA_builder.py
--rw-rw-rw-   0        0        0    11304 2023-06-30 08:55:10.000000 nomad_camels-0.1.4/nomad_camels/tools/VISA_driver_builder.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tools/__init__.py
--rw-rw-rw-   0        0        0     8548 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tools/databroker_exporter.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.308243 nomad_camels-0.1.4/nomad_camels/ui_widgets/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/__init__.py
--rw-rw-rw-   0        0        0    20475 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/add_remove_table.py
--rw-rw-rw-   0        0        0     9089 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/channels_check_table.py
--rw-rw-rw-   0        0        0     1742 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/console_redirect.py
--rw-rw-rw-   0        0        0     1204 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/drag_drop_tree_view.py
--rw-rw-rw-   0        0        0     6522 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/options_run_button.py
--rw-rw-rw-   0        0        0     2493 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/path_button_edit.py
--rw-rw-rw-   0        0        0     3567 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/variable_tool_tip_box.py
--rw-rw-rw-   0        0        0      451 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/warn_popup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/nomad_camels/utility/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/__init__.py
--rw-rw-rw-   0        0        0    15701 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/databroker_export.py
--rw-rw-rw-   0        0        0     5204 2023-06-29 11:51:05.000000 nomad_camels-0.1.4/nomad_camels/utility/device_handling.py
--rw-rw-rw-   0        0        0     1833 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/exception_hook.py
--rw-rw-rw-   0        0        0      788 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/fit_variable_renaming.py
--rw-rw-rw-   0        0        0    14745 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/utility/load_save_functions.py
--rw-rw-rw-   0        0        0      938 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/load_save_helper_functions.py
--rw-rw-rw-   0        0        0      867 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/number_formatting.py
--rw-rw-rw-   0        0        0     1583 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/plot_placement.py
--rw-rw-rw-   0        0        0     9893 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/utility/qthreads.py
--rw-rw-rw-   0        0        0     2496 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/theme_changing.py
--rw-rw-rw-   0        0        0      330 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/tqdm_progress_bar.py
--rw-rw-rw-   0        0        0     2573 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/treeView_functions.py
--rw-rw-rw-   0        0        0     2674 2023-06-28 15:48:04.000000 nomad_camels-0.1.4/nomad_camels/utility/update_camels.py
--rw-rw-rw-   0        0        0    10431 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/variables_handling.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.428961 nomad_camels-0.1.4/nomad_camels.egg-info/
--rw-rw-rw-   0        0        0     2317 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5717 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1340 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      925 2023-07-06 12:15:55.000000 nomad_camels-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     1340 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.600791 nomad_camels-0.1.5/
+-rw-rw-rw-   0        0        0    26526 2023-06-28 14:51:17.000000 nomad_camels-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    26525 2023-06-28 14:51:17.000000 nomad_camels-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       27 2023-06-28 14:51:17.000000 nomad_camels-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2591 2023-07-13 12:51:19.599790 nomad_camels-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1925 2023-07-13 12:50:18.000000 nomad_camels-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.401614 nomad_camels-0.1.5/nomad_camels/
+-rw-rw-rw-   0        0        0     4227 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/CAMELS_start.py
+-rw-rw-rw-   0        0        0    42777 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/MainApp_v2.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.550762 nomad_camels-0.1.5/nomad_camels/bluesky_handling/
+-rw-rw-rw-   0        0        0     5236 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/EpicsFieldSignal.py
+-rw-rw-rw-   0        0        0     1827 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/__init__.py
+-rw-rw-rw-   0        0        0     6047 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/builder_helper_functions.py
+-rw-rw-rw-   0        0        0     4103 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/custom_function_signal.py
+-rw-rw-rw-   0        0        0     4841 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/evaluation_helper.py
+-rw-rw-rw-   0        0        0    22693 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/helper_functions.py
+-rw-rw-rw-   0        0        0     1915 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/make_catalog.py
+-rw-rw-rw-   0        0        0    16474 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/protocol_builder.py
+-rw-rw-rw-   0        0        0      885 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/special_plan_stubs.py
+-rw-rw-rw-   0        0        0    10686 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/bluesky_handling/visa_signal.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.565570 nomad_camels-0.1.5/nomad_camels/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/commands/__init__.py
+-rw-rw-rw-   0        0        0     5509 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/commands/change_sequence.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.631284 nomad_camels-0.1.5/nomad_camels/frontpanels/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/__init__.py
+-rw-rw-rw-   0        0        0     9749 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/device_add_dialog.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.662593 nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/__init__.py
+-rw-rw-rw-   0        0        0     8771 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
+-rw-rw-rw-   0        0        0      830 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
+-rw-rw-rw-   0        0        0      236 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/pass_ask.py
+-rw-rw-rw-   0        0        0    10082 2023-06-28 15:46:34.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/instrument_config.py
+-rw-rw-rw-   0        0        0    13231 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/instrument_installer.py
+-rw-rw-rw-   0        0        0     2925 2023-06-29 11:51:05.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/manage_instruments.py
+-rw-rw-rw-   0        0        0    22774 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/plot_definer.py
+-rw-rw-rw-   0        0        0    22381 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/protocol_config.py
+-rw-rw-rw-   0        0        0     9534 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/frontpanels/settings_window.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.808427 nomad_camels-0.1.5/nomad_camels/graphics/
+-rw-rw-rw-   0        0        0    16958 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/CAMELS.ico
+-rw-rw-rw-   0        0        0     2926 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/CAMELS_Icon.png
+-rw-rw-rw-   0        0        0   101760 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
+-rw-rw-rw-   0        0        0   479310 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
+-rw-rw-rw-   0        0        0    13283 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/camels-horizontal.svg
+-rw-rw-rw-   0        0        0    13715 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/camels-vertical.svg
+-rw-rw-rw-   0        0        0    12919 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/camels_horizontal.png
+-rw-rw-rw-   0        0        0    19245 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/camels_vertical.png
+-rw-rw-rw-   0        0        0    40043 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/dark.qss
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.916748 nomad_camels-0.1.5/nomad_camels/graphics/legacy/
+-rw-rw-rw-   0        0        0    60728 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS.svg
+-rw-rw-rw-   0        0        0    52644 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Icon.png
+-rw-rw-rw-   0        0        0   349358 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
+-rw-rw-rw-   0        0        0    34101 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
+-rw-rw-rw-   0        0        0    42984 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Logo.png
+-rw-rw-rw-   0        0        0    43703 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Logo.svg
+-rw-rw-rw-   0        0        0    96186 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
+-rw-rw-rw-   0        0        0    18507 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_V1.svg
+-rw-rw-rw-   0        0        0    20058 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_v2.svg
+-rw-rw-rw-   0        0        0   290607 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/camels - Kopie.png
+-rw-rw-rw-   0        0        0   252699 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/camels_free.png
+-rw-rw-rw-   0        0        0     7058 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/graphics/legacy/plus_sign.png
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.131986 nomad_camels-0.1.5/nomad_camels/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/__init__.py
+-rw-rw-rw-   0        0        0     6130 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/addDeviceDialog.py
+-rw-rw-rw-   0        0        0     5535 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/device_installer.py
+-rw-rw-rw-   0        0        0     2841 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/enterTextDialog.py
+-rw-rw-rw-   0        0        0     4027 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/fit_definer.py
+-rw-rw-rw-   0        0        0    11001 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/for_loop.py
+-rw-rw-rw-   0        0        0     6623 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/general_protocol_settings.py
+-rw-rw-rw-   0        0        0     8501 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/gradient_descent_step.py
+-rw-rw-rw-   0        0        0     4572 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/instrument_config.py
+-rw-rw-rw-   0        0        0    22581 2023-06-28 15:46:34.000000 nomad_camels-0.1.5/nomad_camels/gui/mainWindow_v2.py
+-rw-rw-rw-   0        0        0     2893 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/pass_ask.py
+-rw-rw-rw-   0        0        0     7219 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/plot_definer.py
+-rw-rw-rw-   0        0        0     6027 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/plot_definer_2d.py
+-rw-rw-rw-   0        0        0     3885 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/plot_options.py
+-rw-rw-rw-   0        0        0     7230 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/protocol_view.py
+-rw-rw-rw-   0        0        0     2537 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/read_channels.py
+-rw-rw-rw-   0        0        0     1465 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/gui/set_channels.py
+-rw-rw-rw-   0        0        0    15557 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/gui/settings_window.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.252623 nomad_camels-0.1.5/nomad_camels/loop_steps/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/__init__.py
+-rw-rw-rw-   0        0        0     4577 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/change_device_config.py
+-rw-rw-rw-   0        0        0    28468 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/for_while_loops.py
+-rw-rw-rw-   0        0        0    10275 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/gradient_descent.py
+-rw-rw-rw-   0        0        0     9981 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/if_step.py
+-rw-rw-rw-   0        0        0     5520 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/make_step_of_type.py
+-rw-rw-rw-   0        0        0    14836 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/nd_sweep.py
+-rw-rw-rw-   0        0        0     4202 2023-07-06 13:08:27.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/prompt_loop_step.py
+-rw-rw-rw-   0        0        0    16246 2023-07-06 13:08:27.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/read_channels.py
+-rw-rw-rw-   0        0        0     8925 2023-07-06 15:25:17.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/run_subprotocol.py
+-rw-rw-rw-   0        0        0     4894 2023-07-06 15:25:17.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/set_channels.py
+-rw-rw-rw-   0        0        0     4761 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/set_value_popup.py
+-rw-rw-rw-   0        0        0     2427 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/set_variables.py
+-rw-rw-rw-   0        0        0    13474 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/simple_sweep.py
+-rw-rw-rw-   0        0        0     2609 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/loop_steps/wait_loop_step.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.383193 nomad_camels-0.1.5/nomad_camels/main_classes/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/main_classes/__init__.py
+-rw-rw-rw-   0        0        0    30268 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/main_classes/device_class.py
+-rw-rw-rw-   0        0        0     3595 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/main_classes/list_plot.py
+-rw-rw-rw-   0        0        0    12119 2023-07-06 07:34:02.000000 nomad_camels-0.1.5/nomad_camels/main_classes/loop_step.py
+-rw-rw-rw-   0        0        0     4624 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/main_classes/manual_control.py
+-rw-rw-rw-   0        0        0     1242 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/main_classes/measurement_channel.py
+-rw-rw-rw-   0        0        0     7869 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/main_classes/plot_2D.py
+-rw-rw-rw-   0        0        0    48782 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/main_classes/plot_widget.py
+-rw-rw-rw-   0        0        0    25099 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/main_classes/protocol_class.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.386192 nomad_camels-0.1.5/nomad_camels/manual_controls/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/manual_controls/__init__.py
+-rw-rw-rw-   0        0        0     3377 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/manual_controls/get_manual_controls.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.407803 nomad_camels-0.1.5/nomad_camels/manual_controls/stage_control/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/manual_controls/stage_control/__init__.py
+-rw-rw-rw-   0        0        0    20282 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/manual_controls/stage_control/stage_control.py
+-rw-rw-rw-   0        0        0    12048 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/manual_controls/stage_control/ui_stage_control.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.415798 nomad_camels-0.1.5/nomad_camels/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/tests/__init__.py
+-rw-rw-rw-   0        0        0     2908 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/tests/instrument_management_test.py
+-rw-rw-rw-   0        0        0    21030 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/tests/protocol_test.py
+-rw-rw-rw-   0        0        0      689 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/tests/startup_test.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.424793 nomad_camels-0.1.5/nomad_camels/tools/
+-rw-rw-rw-   0        0        0     8908 2023-07-13 08:20:59.000000 nomad_camels-0.1.5/nomad_camels/tools/EPICS_driver_builder.py
+-rw-rw-rw-   0        0        0     5627 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/tools/VISA_builder.py
+-rw-rw-rw-   0        0        0    11274 2023-07-13 08:20:59.000000 nomad_camels-0.1.5/nomad_camels/tools/VISA_driver_builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/tools/__init__.py
+-rw-rw-rw-   0        0        0     8548 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/tools/databroker_exporter.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.505792 nomad_camels-0.1.5/nomad_camels/ui_widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/__init__.py
+-rw-rw-rw-   0        0        0    20475 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/add_remove_table.py
+-rw-rw-rw-   0        0        0     9089 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/channels_check_table.py
+-rw-rw-rw-   0        0        0     1742 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/console_redirect.py
+-rw-rw-rw-   0        0        0     1204 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/drag_drop_tree_view.py
+-rw-rw-rw-   0        0        0     6522 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/options_run_button.py
+-rw-rw-rw-   0        0        0     2493 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/path_button_edit.py
+-rw-rw-rw-   0        0        0     3567 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/variable_tool_tip_box.py
+-rw-rw-rw-   0        0        0      451 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/ui_widgets/warn_popup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:19.597794 nomad_camels-0.1.5/nomad_camels/utility/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/utility/__init__.py
+-rw-rw-rw-   0        0        0    15701 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/utility/databroker_export.py
+-rw-rw-rw-   0        0        0     8008 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/device_handling.py
+-rw-rw-rw-   0        0        0     2099 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/exception_hook.py
+-rw-rw-rw-   0        0        0      989 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/fit_variable_renaming.py
+-rw-rw-rw-   0        0        0    17868 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/load_save_functions.py
+-rw-rw-rw-   0        0        0     1404 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/load_save_helper_functions.py
+-rw-rw-rw-   0        0        0     2076 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/logging_settings.py
+-rw-rw-rw-   0        0        0      975 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/number_formatting.py
+-rw-rw-rw-   0        0        0     2849 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/plot_placement.py
+-rw-rw-rw-   0        0        0    10066 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/qthreads.py
+-rw-rw-rw-   0        0        0     2975 2023-07-13 07:48:21.000000 nomad_camels-0.1.5/nomad_camels/utility/theme_changing.py
+-rw-rw-rw-   0        0        0      907 2023-07-13 08:20:59.000000 nomad_camels-0.1.5/nomad_camels/utility/tqdm_progress_bar.py
+-rw-rw-rw-   0        0        0     2573 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/nomad_camels/utility/treeView_functions.py
+-rw-rw-rw-   0        0        0     4135 2023-07-13 08:20:59.000000 nomad_camels-0.1.5/nomad_camels/utility/update_camels.py
+-rw-rw-rw-   0        0        0    12678 2023-07-13 12:50:18.000000 nomad_camels-0.1.5/nomad_camels/utility/variables_handling.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:51:18.408610 nomad_camels-0.1.5/nomad_camels.egg-info/
+-rw-rw-rw-   0        0        0     2591 2023-07-13 12:51:18.000000 nomad_camels-0.1.5/nomad_camels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5758 2023-07-13 12:51:18.000000 nomad_camels-0.1.5/nomad_camels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:51:18.000000 nomad_camels-0.1.5/nomad_camels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1340 2023-07-13 12:51:18.000000 nomad_camels-0.1.5/nomad_camels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-13 12:51:18.000000 nomad_camels-0.1.5/nomad_camels.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      925 2023-07-13 12:50:46.000000 nomad_camels-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1340 2023-06-28 14:51:20.000000 nomad_camels-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:51:19.600791 nomad_camels-0.1.5/setup.cfg
```

### Comparing `nomad_camels-0.1.4/LICENSE` & `nomad_camels-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/LICENSE.txt` & `nomad_camels-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/PKG-INFO` & `nomad_camels-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels
-Version: 0.1.4
+Version: 0.1.5
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
@@ -27,16 +27,20 @@
 
 ## Documentation
 
 For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 # Changelog
 
+## 0.1.5
+Fixed the 'Update CAMELS' tool.\
+Renamed input and output to read and set in the 'Update CAMELS' tool.\
+Small fix to the VISA device builder.
 
 ## 0.1.4
-Added a timeout setting to all VISA instruments. 
+Added a timeout setting to all VISA instruments. Setting the timeout determines how long the instrument waits after sending a command before raising a timeout exception
 
 ## 0.1.3
 First stable and working release
 
 ## 0.1.0 to 0.1.2 
 &#9888; Broken releases due to minor bugs that were fixed in 0.1.3
```

### Comparing `nomad_camels-0.1.4/README.md` & `nomad_camels-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 
 ## Documentation
 
 For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 # Changelog
 
+## 0.1.5
+Fixed the 'Update CAMELS' tool.\
+Renamed input and output to read and set in the 'Update CAMELS' tool.\
+Small fix to the VISA device builder.
 
 ## 0.1.4
-Added a timeout setting to all VISA instruments. 
+Added a timeout setting to all VISA instruments. Setting the timeout determines how long the instrument waits after sending a command before raising a timeout exception
 
 ## 0.1.3
 First stable and working release
 
 ## 0.1.0 to 0.1.2 
-&#9888; Broken releases due to minor bugs that were fixed in 0.1.3
+&#9888; Broken releases due to minor bugs that were fixed in 0.1.3
```

### Comparing `nomad_camels-0.1.4/nomad_camels/CAMELS_start.py` & `nomad_camels-0.1.5/nomad_camels/CAMELS_start.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/MainApp_v2.py` & `nomad_camels-0.1.5/nomad_camels/MainApp_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PySide6.QtGui import QIcon, QPixmap, QShortcut
 
 from nomad_camels.utility import exception_hook
 from nomad_camels.gui.mainWindow_v2 import Ui_MainWindow
 from pkg_resources import resource_filename
 
 from nomad_camels.frontpanels.helper_panels.button_move_scroll_area import Drop_Scroll_Area
-from nomad_camels.utility import load_save_functions, variables_handling, number_formatting, theme_changing, update_camels
+from nomad_camels.utility import load_save_functions, variables_handling, number_formatting, theme_changing, update_camels, logging_settings
 from nomad_camels.ui_widgets import options_run_button, warn_popup
 
 from collections import OrderedDict
 
 import bluesky
 import ophyd
 from bluesky import RunEngine
@@ -431,23 +431,26 @@
         ----------
 
         Returns
         -------
 
         """
         self.preferences = load_save_functions.get_preferences()
-        variables_handling.preferences = self.preferences
+        self.update_preference_settings()
+
+    def update_preference_settings(self):
         number_formatting.preferences = self.preferences
-        # if 'dark_mode' in self.preferences:
-        #     self.toggle_dark_mode()
+        variables_handling.preferences = self.preferences
+        variables_handling.device_driver_path = self.preferences['device_driver_path']
+        variables_handling.meas_files_path = self.preferences['meas_files_path']
         if 'graphic_theme' in self.preferences:
             self.change_theme()
         self.change_catalog_name()
-        variables_handling.device_driver_path = self.preferences['device_driver_path']
-        variables_handling.meas_files_path = self.preferences['meas_files_path']
+        logging_settings.update_log_settings()
+
 
     def change_theme(self):
         """ """
         theme = self.preferences['graphic_theme']
         if 'material_theme' in self.preferences:
             material_theme = self.preferences['material_theme']
         else:
@@ -500,22 +503,16 @@
         -------
 
         """
         from nomad_camels.frontpanels.settings_window import Settings_Window
         settings_dialog = Settings_Window(parent=self, settings=self.preferences)
         if settings_dialog.exec():
             self.preferences = settings_dialog.get_settings()
-            number_formatting.preferences = self.preferences
-            # self.toggle_dark_mode()
-            self.change_catalog_name()
             load_save_functions.save_preferences(self.preferences)
-            variables_handling.device_driver_path = self.preferences['device_driver_path']
-            variables_handling.meas_files_path = self.preferences['meas_files_path']
-            variables_handling.preferences = self.preferences
-        self.change_theme()
+        self.update_preference_settings()
 
     def save_state(self, fromload=False, do_backup=True):
         """Saves the current states of both presets.
 
         Parameters
         ----------
         fromload :
```

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/EpicsFieldSignal.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/EpicsFieldSignal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/builder_helper_functions.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/builder_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/custom_function_signal.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/custom_function_signal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/evaluation_helper.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/evaluation_helper.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/helper_functions.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/make_catalog.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/make_catalog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/protocol_builder.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/protocol_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/special_plan_stubs.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/special_plan_stubs.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/bluesky_handling/visa_signal.py` & `nomad_camels-0.1.5/nomad_camels/bluesky_handling/visa_signal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/commands/change_sequence.py` & `nomad_camels-0.1.5/nomad_camels/commands/change_sequence.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/device_add_dialog.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/device_add_dialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/enterTextDialog.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/helper_panels/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_config.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_installer.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/instrument_installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,19 +90,21 @@
         url = f'https://raw.githubusercontent.com/{repo_part}/{branch}/{directory}/driver_list.txt'
         devices_str = requests.get(url).text
     except:
         url = 'https://raw.githubusercontent.com/FAU-LAP/CAMELS_drivers/main/driver_list.txt'
         devices_str = requests.get(url).text
     warned = False
     for x in devices_str.splitlines():
+        if '==' not in x:
+            continue
         try:
             name, version = x.split('==')
         except:
             if not warned:
-                WarnPopup(None, 'Could not read driver_list.txt from repo.\n'
+                WarnPopup(None, 'Could not (completely) read driver_list.txt from repo.\n'
                                 'Check settings if repository and branch are correct.',
                           'No online-drivers found')
             warned = True
             continue
         all_instr[name.replace('-', '_')] = version
     return all_instr
```

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/manage_instruments.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/manage_instruments.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/plot_definer.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/protocol_config.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/protocol_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/frontpanels/settings_window.py` & `nomad_camels-0.1.5/nomad_camels/frontpanels/settings_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from PySide6.QtCore import Qt, QCoreApplication
 from PySide6.QtGui import QKeyEvent
 import qt_material
 
 from nomad_camels.gui.settings_window import Ui_settings_window
 from nomad_camels.utility.load_save_functions import standard_pref
 from nomad_camels.utility.theme_changing import change_theme
+from nomad_camels.utility.logging_settings import log_levels
 
 class Settings_Window(Ui_settings_window, QDialog):
     """Dialog to change the settings used in CAMELS."""
     def __init__(self, parent=None, settings=None):
         super().__init__(parent)
         self.setupUi(self)
         self.setWindowTitle('NOMAD-CAMELS - Settings')
@@ -103,14 +104,29 @@
         else:
             self.lineEdit_directory.setText(standard_pref['repo_directory'])
         if 'repo_branch' in settings:
             self.lineEdit_branch.setText(settings['repo_branch'])
         else:
             self.lineEdit_branch.setText(standard_pref['repo_branch'])
 
+        for level in log_levels:
+            self.comboBox_log_level.addItem(level)
+        if 'log_level' in settings:
+            self.comboBox_log_level.setCurrentText(settings['log_level'])
+        else:
+            self.comboBox_log_level.setCurrentText(standard_pref['log_level'])
+        if 'logfile_size' in settings:
+            self.spinBox_logfile_size.setValue(settings['logfile_size'])
+        else:
+            self.spinBox_logfile_size.setValue(standard_pref['logfile_size'])
+        if 'logfile_backups' in settings:
+            self.spinBox_logfile_number.setValue(settings['logfile_backups'])
+        else:
+            self.spinBox_logfile_number.setValue(standard_pref['logfile_backups'])
+
         self.radioButton_mixed.clicked.connect(self.number_change)
         self.radioButton_plain_numbers.clicked.connect(self.number_change)
         self.radioButton_scientific.clicked.connect(self.number_change)
 
 
     def autosave_run_change(self):
         on = self.checkBox_autosave_run.isChecked()
@@ -162,15 +178,18 @@
                 'py_files_path': self.pathButton_py_files.get_path(),
                 'meas_files_path': self.pathButton_meas_files.get_path(),
                 'device_driver_path': self.pathButton_device_path.get_path(),
                 'databroker_catalog_name': self.lineEdit_catalog_name.text(),
                 'driver_repository': self.lineEdit_repo.text(),
                 'repo_branch': self.lineEdit_branch.text(),
                 'repo_directory': self.lineEdit_directory.text(),
-                'play_camel_on_error': self.checkBox_play_camel_on_error.isChecked()}
+                'play_camel_on_error': self.checkBox_play_camel_on_error.isChecked(),
+                'log_level': self.comboBox_log_level.currentText(),
+                'logfile_size': self.spinBox_logfile_size.value(),
+                'logfile_backups': self.spinBox_logfile_number.value()}
 
 
     def keyPressEvent(self, a0: QKeyEvent) -> None:
         """Overwrites the keyPressEvent of the QDialog so that it does
         not close when pressing Enter/Return.
 
         Parameters
```

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/CAMELS.ico` & `nomad_camels-0.1.5/nomad_camels/graphics/CAMELS.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/CAMELS_Icon.png` & `nomad_camels-0.1.5/nomad_camels/graphics/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3` & `nomad_camels-0.1.5/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav` & `nomad_camels-0.1.5/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/camels-horizontal.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/camels-horizontal.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/camels-vertical.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/camels-vertical.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/camels_horizontal.png` & `nomad_camels-0.1.5/nomad_camels/graphics/camels_horizontal.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/camels_vertical.png` & `nomad_camels-0.1.5/nomad_camels/graphics/camels_vertical.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/dark.qss` & `nomad_camels-0.1.5/nomad_camels/graphics/dark.qss`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon.png` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.png` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Logo.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Logo.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_V1.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_V1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_v2.svg` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/CAMELS_v2.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels - Kopie.png` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/camels - Kopie.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels_free.png` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/camels_free.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/graphics/legacy/plus_sign.png` & `nomad_camels-0.1.5/nomad_camels/graphics/legacy/plus_sign.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/addDeviceDialog.py` & `nomad_camels-0.1.5/nomad_camels/gui/addDeviceDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/device_installer.py` & `nomad_camels-0.1.5/nomad_camels/gui/device_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/enterTextDialog.py` & `nomad_camels-0.1.5/nomad_camels/gui/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/fit_definer.py` & `nomad_camels-0.1.5/nomad_camels/gui/fit_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/for_loop.py` & `nomad_camels-0.1.5/nomad_camels/gui/for_loop.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/general_protocol_settings.py` & `nomad_camels-0.1.5/nomad_camels/gui/general_protocol_settings.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/gradient_descent_step.py` & `nomad_camels-0.1.5/nomad_camels/gui/gradient_descent_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/instrument_config.py` & `nomad_camels-0.1.5/nomad_camels/gui/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/mainWindow_v2.py` & `nomad_camels-0.1.5/nomad_camels/gui/mainWindow_v2.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/pass_ask.py` & `nomad_camels-0.1.5/nomad_camels/gui/pass_ask.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/plot_definer.py` & `nomad_camels-0.1.5/nomad_camels/gui/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/plot_definer_2d.py` & `nomad_camels-0.1.5/nomad_camels/gui/plot_definer_2d.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/plot_options.py` & `nomad_camels-0.1.5/nomad_camels/gui/plot_options.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/protocol_view.py` & `nomad_camels-0.1.5/nomad_camels/gui/protocol_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/read_channels.py` & `nomad_camels-0.1.5/nomad_camels/gui/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/set_channels.py` & `nomad_camels-0.1.5/nomad_camels/gui/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/gui/settings_window.py` & `nomad_camels-0.1.5/nomad_camels/gui/settings_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,281 +22,331 @@
 
 from nomad_camels.ui_widgets.path_button_edit import Path_Button_Edit
 
 class Ui_settings_window(object):
     def setupUi(self, settings_window):
         if not settings_window.objectName():
             settings_window.setObjectName(u"settings_window")
-        settings_window.resize(549, 505)
+        settings_window.resize(391, 578)
         self.gridLayout = QGridLayout(settings_window)
         self.gridLayout.setObjectName(u"gridLayout")
-        self.line_6 = QFrame(settings_window)
-        self.line_6.setObjectName(u"line_6")
-        self.line_6.setFrameShadow(QFrame.Raised)
-        self.line_6.setLineWidth(5)
-        self.line_6.setFrameShape(QFrame.HLine)
-
-        self.gridLayout.addWidget(self.line_6, 19, 1, 1, 3)
-
         self.checkBox_play_camel_on_error = QCheckBox(settings_window)
         self.checkBox_play_camel_on_error.setObjectName(u"checkBox_play_camel_on_error")
 
-        self.gridLayout.addWidget(self.checkBox_play_camel_on_error, 26, 1, 1, 3)
+        self.gridLayout.addWidget(self.checkBox_play_camel_on_error, 30, 1, 1, 3)
 
-        self.radioButton_mixed = QRadioButton(settings_window)
-        self.radioButton_mixed.setObjectName(u"radioButton_mixed")
+        self.pathButton_meas_files = Path_Button_Edit(settings_window)
+        self.pathButton_meas_files.setObjectName(u"pathButton_meas_files")
 
-        self.gridLayout.addWidget(self.radioButton_mixed, 9, 3, 1, 1)
+        self.gridLayout.addWidget(self.pathButton_meas_files, 21, 2, 1, 2)
 
-        self.label_14 = QLabel(settings_window)
-        self.label_14.setObjectName(u"label_14")
+        self.pathButton_py_files = Path_Button_Edit(settings_window)
+        self.pathButton_py_files.setObjectName(u"pathButton_py_files")
 
-        self.gridLayout.addWidget(self.label_14, 22, 1, 1, 1)
+        self.gridLayout.addWidget(self.pathButton_py_files, 18, 2, 1, 2)
 
-        self.lineEdit_directory = QLineEdit(settings_window)
-        self.lineEdit_directory.setObjectName(u"lineEdit_directory")
+        self.pathButton_device_path = Path_Button_Edit(settings_window)
+        self.pathButton_device_path.setObjectName(u"pathButton_device_path")
 
-        self.gridLayout.addWidget(self.lineEdit_directory, 22, 3, 1, 1)
+        self.gridLayout.addWidget(self.pathButton_device_path, 27, 2, 1, 2)
 
-        self.label_13 = QLabel(settings_window)
-        self.label_13.setObjectName(u"label_13")
-        font = QFont()
-        font.setBold(True)
-        self.label_13.setFont(font)
+        self.line_6 = QFrame(settings_window)
+        self.line_6.setObjectName(u"line_6")
+        self.line_6.setFrameShadow(QFrame.Raised)
+        self.line_6.setLineWidth(5)
+        self.line_6.setFrameShape(QFrame.HLine)
 
-        self.gridLayout.addWidget(self.label_13, 20, 1, 1, 3)
+        self.gridLayout.addWidget(self.line_6, 23, 1, 1, 3)
 
-        self.label_6 = QLabel(settings_window)
-        self.label_6.setObjectName(u"label_6")
-        self.label_6.setMaximumSize(QSize(16777215, 17))
+        self.lineEdit_branch = QLineEdit(settings_window)
+        self.lineEdit_branch.setObjectName(u"lineEdit_branch")
 
-        self.gridLayout.addWidget(self.label_6, 14, 1, 1, 1)
+        self.gridLayout.addWidget(self.lineEdit_branch, 26, 2, 1, 1)
 
-        self.checkBox_dark = QCheckBox(settings_window)
-        self.checkBox_dark.setObjectName(u"checkBox_dark")
+        self.label_3 = QLabel(settings_window)
+        self.label_3.setObjectName(u"label_3")
+        self.label_3.setMaximumSize(QSize(16777215, 17))
+        font = QFont()
+        font.setBold(True)
+        self.label_3.setFont(font)
 
-        self.gridLayout.addWidget(self.checkBox_dark, 5, 3, 1, 1)
+        self.gridLayout.addWidget(self.label_3, 12, 1, 1, 3)
+
+        self.comboBox_theme = QComboBox(settings_window)
+        self.comboBox_theme.setObjectName(u"comboBox_theme")
+
+        self.gridLayout.addWidget(self.comboBox_theme, 9, 1, 1, 1)
 
         self.line_2 = QFrame(settings_window)
         self.line_2.setObjectName(u"line_2")
         self.line_2.setFrameShadow(QFrame.Raised)
         self.line_2.setLineWidth(5)
         self.line_2.setFrameShape(QFrame.HLine)
 
-        self.gridLayout.addWidget(self.line_2, 6, 1, 1, 3)
+        self.gridLayout.addWidget(self.line_2, 10, 1, 1, 3)
 
-        self.spinBox_scientific_from = QSpinBox(settings_window)
-        self.spinBox_scientific_from.setObjectName(u"spinBox_scientific_from")
-        self.spinBox_scientific_from.setValue(3)
+        self.lineEdit_catalog_name = QLineEdit(settings_window)
+        self.lineEdit_catalog_name.setObjectName(u"lineEdit_catalog_name")
 
-        self.gridLayout.addWidget(self.spinBox_scientific_from, 10, 3, 1, 1)
+        self.gridLayout.addWidget(self.lineEdit_catalog_name, 22, 2, 1, 2)
 
-        self.radioButton_scientific = QRadioButton(settings_window)
-        self.radioButton_scientific.setObjectName(u"radioButton_scientific")
+        self.line_5 = QFrame(settings_window)
+        self.line_5.setObjectName(u"line_5")
+        self.line_5.setFrameShadow(QFrame.Raised)
+        self.line_5.setLineWidth(5)
+        self.line_5.setFrameShape(QFrame.HLine)
 
-        self.gridLayout.addWidget(self.radioButton_scientific, 9, 2, 1, 1)
+        self.gridLayout.addWidget(self.line_5, 28, 1, 1, 3)
 
-        self.lineEdit_catalog_name = QLineEdit(settings_window)
-        self.lineEdit_catalog_name.setObjectName(u"lineEdit_catalog_name")
+        self.radioButton_scientific = QRadioButton(settings_window)
+        self.radioButton_scientific.setObjectName(u"radioButton_scientific")
 
-        self.gridLayout.addWidget(self.lineEdit_catalog_name, 18, 2, 1, 2)
+        self.gridLayout.addWidget(self.radioButton_scientific, 13, 2, 1, 1)
 
         self.label_2 = QLabel(settings_window)
         self.label_2.setObjectName(u"label_2")
         self.label_2.setMaximumSize(QSize(16777215, 17))
         self.label_2.setFont(font)
 
-        self.gridLayout.addWidget(self.label_2, 4, 1, 1, 3)
+        self.gridLayout.addWidget(self.label_2, 8, 1, 1, 3)
 
-        self.label_11 = QLabel(settings_window)
-        self.label_11.setObjectName(u"label_11")
-        self.label_11.setFont(font)
-
-        self.gridLayout.addWidget(self.label_11, 25, 1, 1, 3)
-
-        self.line_5 = QFrame(settings_window)
-        self.line_5.setObjectName(u"line_5")
-        self.line_5.setFrameShadow(QFrame.Raised)
-        self.line_5.setLineWidth(5)
-        self.line_5.setFrameShape(QFrame.HLine)
+        self.label_5 = QLabel(settings_window)
+        self.label_5.setObjectName(u"label_5")
+        self.label_5.setMaximumSize(QSize(16777215, 17))
+        self.label_5.setFont(font)
 
-        self.gridLayout.addWidget(self.line_5, 24, 1, 1, 3)
+        self.gridLayout.addWidget(self.label_5, 17, 1, 1, 3)
 
         self.label_7 = QLabel(settings_window)
         self.label_7.setObjectName(u"label_7")
         self.label_7.setMaximumSize(QSize(16777215, 17))
 
-        self.gridLayout.addWidget(self.label_7, 17, 1, 1, 1)
+        self.gridLayout.addWidget(self.label_7, 21, 1, 1, 1)
 
-        self.lineEdit_branch = QLineEdit(settings_window)
-        self.lineEdit_branch.setObjectName(u"lineEdit_branch")
+        self.label_8 = QLabel(settings_window)
+        self.label_8.setObjectName(u"label_8")
+        self.label_8.setMaximumSize(QSize(16777215, 17))
 
-        self.gridLayout.addWidget(self.lineEdit_branch, 22, 2, 1, 1)
+        self.gridLayout.addWidget(self.label_8, 27, 1, 1, 1)
 
-        self.buttonBox = QDialogButtonBox(settings_window)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
+        self.lineEdit_directory = QLineEdit(settings_window)
+        self.lineEdit_directory.setObjectName(u"lineEdit_directory")
 
-        self.gridLayout.addWidget(self.buttonBox, 27, 1, 1, 3)
+        self.gridLayout.addWidget(self.lineEdit_directory, 26, 3, 1, 1)
 
-        self.label_3 = QLabel(settings_window)
-        self.label_3.setObjectName(u"label_3")
-        self.label_3.setMaximumSize(QSize(16777215, 17))
-        self.label_3.setFont(font)
+        self.lineEdit_repo = QLineEdit(settings_window)
+        self.lineEdit_repo.setObjectName(u"lineEdit_repo")
 
-        self.gridLayout.addWidget(self.label_3, 8, 1, 1, 3)
+        self.gridLayout.addWidget(self.lineEdit_repo, 25, 2, 1, 2)
 
-        self.label_5 = QLabel(settings_window)
-        self.label_5.setObjectName(u"label_5")
-        self.label_5.setMaximumSize(QSize(16777215, 17))
-        self.label_5.setFont(font)
+        self.spinBox_n_decimals = QSpinBox(settings_window)
+        self.spinBox_n_decimals.setObjectName(u"spinBox_n_decimals")
+        self.spinBox_n_decimals.setValue(2)
 
-        self.gridLayout.addWidget(self.label_5, 13, 1, 1, 3)
+        self.gridLayout.addWidget(self.spinBox_n_decimals, 15, 2, 1, 2)
 
-        self.label_12 = QLabel(settings_window)
-        self.label_12.setObjectName(u"label_12")
+        self.line = QFrame(settings_window)
+        self.line.setObjectName(u"line")
+        self.line.setFrameShadow(QFrame.Raised)
+        self.line.setLineWidth(5)
+        self.line.setFrameShape(QFrame.HLine)
 
-        self.gridLayout.addWidget(self.label_12, 21, 1, 1, 1)
+        self.gridLayout.addWidget(self.line, 7, 1, 1, 3)
 
-        self.label_8 = QLabel(settings_window)
-        self.label_8.setObjectName(u"label_8")
-        self.label_8.setMaximumSize(QSize(16777215, 17))
+        self.label_13 = QLabel(settings_window)
+        self.label_13.setObjectName(u"label_13")
+        self.label_13.setFont(font)
 
-        self.gridLayout.addWidget(self.label_8, 23, 1, 1, 1)
+        self.gridLayout.addWidget(self.label_13, 24, 1, 1, 3)
 
-        self.lineEdit_repo = QLineEdit(settings_window)
-        self.lineEdit_repo.setObjectName(u"lineEdit_repo")
+        self.label_6 = QLabel(settings_window)
+        self.label_6.setObjectName(u"label_6")
+        self.label_6.setMaximumSize(QSize(16777215, 17))
 
-        self.gridLayout.addWidget(self.lineEdit_repo, 21, 2, 1, 2)
+        self.gridLayout.addWidget(self.label_6, 18, 1, 1, 1)
 
         self.line_3 = QFrame(settings_window)
         self.line_3.setObjectName(u"line_3")
         self.line_3.setFrameShadow(QFrame.Raised)
         self.line_3.setLineWidth(5)
         self.line_3.setFrameShape(QFrame.HLine)
 
-        self.gridLayout.addWidget(self.line_3, 12, 1, 1, 3)
+        self.gridLayout.addWidget(self.line_3, 16, 1, 1, 3)
 
         self.comboBox_material_theme = QComboBox(settings_window)
         self.comboBox_material_theme.setObjectName(u"comboBox_material_theme")
 
-        self.gridLayout.addWidget(self.comboBox_material_theme, 5, 2, 1, 1)
+        self.gridLayout.addWidget(self.comboBox_material_theme, 9, 2, 1, 1)
 
-        self.comboBox_theme = QComboBox(settings_window)
-        self.comboBox_theme.setObjectName(u"comboBox_theme")
-
-        self.gridLayout.addWidget(self.comboBox_theme, 5, 1, 1, 1)
-
-        self.spinBox_n_decimals = QSpinBox(settings_window)
-        self.spinBox_n_decimals.setObjectName(u"spinBox_n_decimals")
-        self.spinBox_n_decimals.setValue(2)
+        self.radioButton_mixed = QRadioButton(settings_window)
+        self.radioButton_mixed.setObjectName(u"radioButton_mixed")
 
-        self.gridLayout.addWidget(self.spinBox_n_decimals, 11, 2, 1, 2)
+        self.gridLayout.addWidget(self.radioButton_mixed, 13, 3, 1, 1)
 
         self.radioButton_plain_numbers = QRadioButton(settings_window)
         self.radioButton_plain_numbers.setObjectName(u"radioButton_plain_numbers")
         self.radioButton_plain_numbers.setCheckable(True)
         self.radioButton_plain_numbers.setChecked(True)
 
-        self.gridLayout.addWidget(self.radioButton_plain_numbers, 9, 1, 1, 1)
+        self.gridLayout.addWidget(self.radioButton_plain_numbers, 13, 1, 1, 1)
+
+        self.checkBox_dark = QCheckBox(settings_window)
+        self.checkBox_dark.setObjectName(u"checkBox_dark")
+
+        self.gridLayout.addWidget(self.checkBox_dark, 9, 3, 1, 1)
+
+        self.label_11 = QLabel(settings_window)
+        self.label_11.setObjectName(u"label_11")
+        self.label_11.setFont(font)
+
+        self.gridLayout.addWidget(self.label_11, 29, 1, 1, 3)
 
         self.label = QLabel(settings_window)
         self.label.setObjectName(u"label")
         self.label.setMaximumSize(QSize(16777215, 17))
         font1 = QFont()
         font1.setBold(True)
         font1.setItalic(False)
         self.label.setFont(font1)
 
         self.gridLayout.addWidget(self.label, 0, 1, 1, 3)
 
-        self.label_4 = QLabel(settings_window)
-        self.label_4.setObjectName(u"label_4")
-        self.label_4.setMaximumSize(QSize(16777215, 17))
+        self.spinBox_scientific_from = QSpinBox(settings_window)
+        self.spinBox_scientific_from.setObjectName(u"spinBox_scientific_from")
+        self.spinBox_scientific_from.setValue(3)
 
-        self.gridLayout.addWidget(self.label_4, 11, 1, 1, 1)
+        self.gridLayout.addWidget(self.spinBox_scientific_from, 14, 3, 1, 1)
 
-        self.label_10 = QLabel(settings_window)
-        self.label_10.setObjectName(u"label_10")
+        self.label_14 = QLabel(settings_window)
+        self.label_14.setObjectName(u"label_14")
 
-        self.gridLayout.addWidget(self.label_10, 18, 1, 1, 1)
+        self.gridLayout.addWidget(self.label_14, 26, 1, 1, 1)
 
-        self.line = QFrame(settings_window)
-        self.line.setObjectName(u"line")
-        self.line.setFrameShadow(QFrame.Raised)
-        self.line.setLineWidth(5)
-        self.line.setFrameShape(QFrame.HLine)
+        self.buttonBox = QDialogButtonBox(settings_window)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
 
-        self.gridLayout.addWidget(self.line, 3, 1, 1, 3)
+        self.gridLayout.addWidget(self.buttonBox, 31, 1, 1, 3)
 
-        self.pathButton_py_files = Path_Button_Edit(settings_window)
-        self.pathButton_py_files.setObjectName(u"pathButton_py_files")
+        self.label_12 = QLabel(settings_window)
+        self.label_12.setObjectName(u"label_12")
 
-        self.gridLayout.addWidget(self.pathButton_py_files, 14, 2, 1, 2)
+        self.gridLayout.addWidget(self.label_12, 25, 1, 1, 1)
 
-        self.pathButton_device_path = Path_Button_Edit(settings_window)
-        self.pathButton_device_path.setObjectName(u"pathButton_device_path")
+        self.label_4 = QLabel(settings_window)
+        self.label_4.setObjectName(u"label_4")
+        self.label_4.setMaximumSize(QSize(16777215, 17))
 
-        self.gridLayout.addWidget(self.pathButton_device_path, 23, 2, 1, 2)
+        self.gridLayout.addWidget(self.label_4, 15, 1, 1, 1)
 
-        self.pathButton_meas_files = Path_Button_Edit(settings_window)
-        self.pathButton_meas_files.setObjectName(u"pathButton_meas_files")
+        self.label_10 = QLabel(settings_window)
+        self.label_10.setObjectName(u"label_10")
 
-        self.gridLayout.addWidget(self.pathButton_meas_files, 17, 2, 1, 2)
+        self.gridLayout.addWidget(self.label_10, 22, 1, 1, 1)
 
         self.checkBox_autosave = QCheckBox(settings_window)
         self.checkBox_autosave.setObjectName(u"checkBox_autosave")
 
         self.gridLayout.addWidget(self.checkBox_autosave, 1, 1, 1, 1)
 
-        self.checkBox_autosave_run = QCheckBox(settings_window)
-        self.checkBox_autosave_run.setObjectName(u"checkBox_autosave_run")
-
-        self.gridLayout.addWidget(self.checkBox_autosave_run, 1, 2, 1, 1)
-
         self.checkBox_backup_before_run = QCheckBox(settings_window)
         self.checkBox_backup_before_run.setObjectName(u"checkBox_backup_before_run")
 
         self.gridLayout.addWidget(self.checkBox_backup_before_run, 1, 3, 1, 1)
 
+        self.checkBox_autosave_run = QCheckBox(settings_window)
+        self.checkBox_autosave_run.setObjectName(u"checkBox_autosave_run")
+
+        self.gridLayout.addWidget(self.checkBox_autosave_run, 1, 2, 1, 1)
+
         self.checkBox_auto_check_updates = QCheckBox(settings_window)
         self.checkBox_auto_check_updates.setObjectName(u"checkBox_auto_check_updates")
 
         self.gridLayout.addWidget(self.checkBox_auto_check_updates, 2, 1, 1, 3)
 
+        self.line_4 = QFrame(settings_window)
+        self.line_4.setObjectName(u"line_4")
+        self.line_4.setFrameShadow(QFrame.Raised)
+        self.line_4.setLineWidth(5)
+        self.line_4.setFrameShape(QFrame.HLine)
+
+        self.gridLayout.addWidget(self.line_4, 3, 1, 1, 3)
+
+        self.label_17 = QLabel(settings_window)
+        self.label_17.setObjectName(u"label_17")
+
+        self.gridLayout.addWidget(self.label_17, 5, 3, 1, 1)
+
+        self.label_15 = QLabel(settings_window)
+        self.label_15.setObjectName(u"label_15")
+
+        self.gridLayout.addWidget(self.label_15, 5, 1, 1, 1)
+
+        self.label_9 = QLabel(settings_window)
+        self.label_9.setObjectName(u"label_9")
+        self.label_9.setFont(font)
+
+        self.gridLayout.addWidget(self.label_9, 4, 1, 1, 3)
+
+        self.label_16 = QLabel(settings_window)
+        self.label_16.setObjectName(u"label_16")
+
+        self.gridLayout.addWidget(self.label_16, 5, 2, 1, 1)
+
+        self.spinBox_logfile_size = QSpinBox(settings_window)
+        self.spinBox_logfile_size.setObjectName(u"spinBox_logfile_size")
+        self.spinBox_logfile_size.setValue(1)
+
+        self.gridLayout.addWidget(self.spinBox_logfile_size, 6, 2, 1, 1)
+
+        self.spinBox_logfile_number = QSpinBox(settings_window)
+        self.spinBox_logfile_number.setObjectName(u"spinBox_logfile_number")
+        self.spinBox_logfile_number.setValue(1)
+
+        self.gridLayout.addWidget(self.spinBox_logfile_number, 6, 3, 1, 1)
+
+        self.comboBox_log_level = QComboBox(settings_window)
+        self.comboBox_log_level.setObjectName(u"comboBox_log_level")
+
+        self.gridLayout.addWidget(self.comboBox_log_level, 6, 1, 1, 1)
+
 
         self.retranslateUi(settings_window)
         self.buttonBox.accepted.connect(settings_window.accept)
         self.buttonBox.rejected.connect(settings_window.reject)
 
         QMetaObject.connectSlotsByName(settings_window)
     # setupUi
 
     def retranslateUi(self, settings_window):
         settings_window.setWindowTitle(QCoreApplication.translate("settings_window", u"Dialog", None))
         self.checkBox_play_camel_on_error.setText(QCoreApplication.translate("settings_window", u"Play Camel-Roar on error", None))
-        self.radioButton_mixed.setText(QCoreApplication.translate("settings_window", u"Scientific from 1e...", None))
-        self.label_14.setText(QCoreApplication.translate("settings_window", u"Branch / Directory", None))
-        self.lineEdit_directory.setPlaceholderText(QCoreApplication.translate("settings_window", u"directory", None))
-        self.label_13.setText(QCoreApplication.translate("settings_window", u"Drivers", None))
-        self.label_6.setText(QCoreApplication.translate("settings_window", u"Python-Files Path", None))
-        self.checkBox_dark.setText(QCoreApplication.translate("settings_window", u"dark mode", None))
-        self.radioButton_scientific.setText(QCoreApplication.translate("settings_window", u"Scientific", None))
-        self.label_2.setText(QCoreApplication.translate("settings_window", u"Theme", None))
-        self.label_11.setText(QCoreApplication.translate("settings_window", u"Sounds", None))
-        self.label_7.setText(QCoreApplication.translate("settings_window", u"Measurement-Data Path", None))
         self.lineEdit_branch.setPlaceholderText(QCoreApplication.translate("settings_window", u"branch", None))
         self.label_3.setText(QCoreApplication.translate("settings_window", u"Number-Formatting (only visual)", None))
+        self.radioButton_scientific.setText(QCoreApplication.translate("settings_window", u"Scientific", None))
+        self.label_2.setText(QCoreApplication.translate("settings_window", u"Theme", None))
         self.label_5.setText(QCoreApplication.translate("settings_window", u"Files", None))
-        self.label_12.setText(QCoreApplication.translate("settings_window", u"Driver Repository URL", None))
+        self.label_7.setText(QCoreApplication.translate("settings_window", u"Measurement-Data Path", None))
         self.label_8.setText(QCoreApplication.translate("settings_window", u"Local drivers path", None))
+        self.lineEdit_directory.setPlaceholderText(QCoreApplication.translate("settings_window", u"directory", None))
+        self.label_13.setText(QCoreApplication.translate("settings_window", u"Drivers", None))
+        self.label_6.setText(QCoreApplication.translate("settings_window", u"Python-Files Path", None))
+        self.radioButton_mixed.setText(QCoreApplication.translate("settings_window", u"Scientific from 1e...", None))
         self.radioButton_plain_numbers.setText(QCoreApplication.translate("settings_window", u"Plain", None))
+        self.checkBox_dark.setText(QCoreApplication.translate("settings_window", u"dark mode", None))
+        self.label_11.setText(QCoreApplication.translate("settings_window", u"Sounds", None))
         self.label.setText(QCoreApplication.translate("settings_window", u"Saving", None))
+        self.label_14.setText(QCoreApplication.translate("settings_window", u"Branch / Directory", None))
+        self.label_12.setText(QCoreApplication.translate("settings_window", u"Driver Repository URL", None))
         self.label_4.setText(QCoreApplication.translate("settings_window", u"# decimals:", None))
         self.label_10.setText(QCoreApplication.translate("settings_window", u"Databroker catalog-name", None))
         self.checkBox_autosave.setText(QCoreApplication.translate("settings_window", u"autosave on closing", None))
-        self.checkBox_autosave_run.setText(QCoreApplication.translate("settings_window", u"autosave before run", None))
         self.checkBox_backup_before_run.setText(QCoreApplication.translate("settings_window", u"backup before run", None))
+        self.checkBox_autosave_run.setText(QCoreApplication.translate("settings_window", u"autosave before run", None))
         self.checkBox_auto_check_updates.setText(QCoreApplication.translate("settings_window", u"automatically search for updates", None))
+        self.label_17.setText(QCoreApplication.translate("settings_window", u"old logfile backups", None))
+        self.label_15.setText(QCoreApplication.translate("settings_window", u"Log-Level", None))
+        self.label_9.setText(QCoreApplication.translate("settings_window", u"Logging", None))
+        self.label_16.setText(QCoreApplication.translate("settings_window", u"max. logfile size (MB)", None))
     # retranslateUi
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/change_device_config.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/change_device_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/for_while_loops.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/for_while_loops.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/gradient_descent.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/if_step.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/if_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/make_step_of_type.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/make_step_of_type.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/nd_sweep.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/nd_sweep.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,23 @@
                     self.used_devices.append(device)
         for channel in self.sweep_channels:
             if channel in variables_handling.channels:
                 device = variables_handling.channels[channel].device
                 if device not in self.used_devices:
                     self.used_devices.append(device)
 
+    def update_variables(self):
+        """Adds the fit variables from the plots."""
+        variables = {}
+        stream = f'{self.name}'
+        for plot in self.plots:
+            variables.update(plot.get_fit_vars(stream))
+        variables_handling.loop_step_variables.update(variables)
+        super().update_variables()
+
     def get_outer_string(self):
         """Gives the string to create the plots of the sweeps"""
         if self.plots:
             return builder_helper_functions.plot_creator(self.plots, f'create_plots_{self.name}')[0]
         return ''
 
     def get_add_main_string(self):
@@ -73,25 +82,16 @@
         add_main_string = ''
         if self.plots:
             add_main_string += builder_helper_functions.get_plot_add_string(self.name, stream)
         return add_main_string
 
 
     def get_protocol_string(self, n_tabs=1):
-        """The loop is enumerating over the selected points.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """The channels to be read are set up. Then a for loop for each sweep is
+        started, with the channels each being set inside it."""
         tabs = '\t'*n_tabs
 
         stream = f'"{self.name}"'
         if self.data_output == 'main stream':
             stream = 'stream_name'
 
         protocol_string = super().get_protocol_string(n_tabs)
@@ -124,62 +124,65 @@
         protocol_string += f'{tabs}\tyield from bps.wait("A")\n'
         protocol_string += f'{tabs}\tyield from bps.trigger_and_read(channels, name={stream})\n'
         protocol_string += f'{tabs}yield from helper_functions.get_fit_results(all_fits, namespace, True, {stream})\n'
         self.update_time_weight()
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
+        """The read channels and the sweeps are specified."""
         short_string = super().get_protocol_short_string(n_tabs)
         tabs = '\t' * (n_tabs+1)
         short_string += f'{tabs}Read: {self.read_channels}\n'
         for i, channel in enumerate(self.sweep_channels):
             sweep = self.sweep_values[i]
             if not isinstance(sweep, Sweep_Step):
                 sweep = Sweep_Step(sweep)
             short_string += f'{tabs}Sweep {i}: {channel}\n{tabs}Values {i}: {sweep.get_protocol_short_string()}\n'
         return short_string
 
 
 
 
 class Sweep_Step(For_Loop_Step):
-    """ """
+    """
+    One single sweep for the ND sweep. Inherits from For_Loop_Step regarding the
+    steps of the sweep.
+
+    Attributes
+    ----------
+    sweep_channel : str
+        The channel which is used in this sweep-part.
+    wait_time : str, float
+        The time in seconds, how long to wait after setting the channel.
+    """
     def __init__(self, step_info=None):
         step_info = step_info or {}
         super().__init__(step_info=step_info)
         self.step_type = 'ND Sweep Part'
         self.sweep_channel = step_info['sweep_channel'] if 'sweep_channel' in step_info else ''
         self.wait_time = step_info['wait_time'] if 'wait_time' in step_info else ''
 
     def get_protocol_string(self, n_tabs=1):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """Creates a for loop over the sweep_channel and waits for wait_time
+        after setting the channel."""
         tabs = '\t'*n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         name = variables_handling.channels[self.sweep_channel].name
         if '.' in name:
             dev, chan = name.split('.')
             setter = f'devs["{dev}"].{chan}'
         else:
             setter = f'devs["{name}"]'
         protocol_string += f'{tabs}\tyield from bps.abs_set({setter}, {self.name.replace(" ", "_")}_Value, group="A")\n'
         if self.wait_time:
             protocol_string += f'{tabs}\tyield from bps.sleep(eva.eval("{self.wait_time}"))\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
+        """Specifies the same way as the foor loop."""
         return super().get_protocol_short_string(n_tabs)[n_tabs+3:-1]
 
 
 
 class ND_Sweep_Config(Loop_Step_Config):
     """ """
     def __init__(self, loop_step:ND_Sweep, parent=None):
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/read_channels.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/read_channels.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,29 @@
 from nomad_camels.gui.read_channels import Ui_read_channels_config
 
 from nomad_camels.utility import variables_handling, fit_variable_renaming
 from nomad_camels.ui_widgets.channels_check_table import Channels_Check_Table
 
 
 class Read_Channels(Loop_Step):
-    """This step represents the bluesky plan stub `trigger_and_read`."""
+    """
+    This step represents the bluesky plan stub `trigger_and_read`. It may also
+    be split into an additional step for triggering, then doing something else
+    and then reading.
+
+    Attributes
+    ----------
+    read_all : bool
+        If True, the step will read all available channels.
+    split_trigger : bool
+        If True, an additional trigger channels step may be used. This read step
+        will then not use `trigger_and_read`, but only read the channels.
+    channel_list : list[str]
+        The list of channels that should be read in this step.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Read Channels'
         if step_info is None:
             step_info = {}
         self.read_all = step_info['read_all'] if 'read_all' in step_info else False
         self.split_trigger = step_info['split_trigger'] if 'split_trigger' in step_info else False
@@ -29,65 +43,59 @@
         for channel in variables_handling.channels:
             if self.read_all or channel in self.channel_list:
                 device = variables_handling.channels[channel].device
                 if device not in self.used_devices:
                     self.used_devices.append(device)
 
     def get_channels_set(self):
-        """ """
+        """Provides a set of `self.channel_list` to remove possible duplicates.
+        Includes all available channels if `self.read_all`."""
         chan_list = []
         if self.read_all:
             for channel in variables_handling.channels:
                 chan_list.append(channel)
         else:
             chan_list = self.channel_list
         return set(chan_list)
 
     def get_channels_string(self, tabs):
         """
+        Gives a string of the channels that should be read. This may also be
+        used by the Trigger_Channels step.
 
         Parameters
         ----------
-        tabs :
-            
-
-        Returns
-        -------
-
+        tabs : str
+            A string including the tabs for intendation.
         """
         channel_string = f'{tabs}channels_{self.variable_name()} = ['
         if not self.read_all and not self.channel_list:
             raise Exception(f'Trying to read no channel in {self.full_name}!')
         if self.read_all:
             for channel in variables_handling.channels:
                 channel_string += get_channel_string(channel)
         else:
             for channel in self.channel_list:
                 channel_string += get_channel_string(channel)
         channel_string = channel_string[:-2] + ']\n'
         return channel_string
 
     def variable_name(self):
-        """ """
+        """Returns the name of this step as a valid variable name, to specify
+        the channels for this read."""
         return fit_variable_renaming.replace_name(self.name)
 
     def get_protocol_string(self, n_tabs=1):
         """In the protocol, at first a list `channels` is defined,
         including all the channels, that are selected to be read. Then
-        bps.trigger_and_read is called on these channels.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        `bps.trigger_and_read` (or `helper_functions.read_wo_trigger`) is called
+        on these channels.
+        The stream in which the data is written will be numbered if there are
+        other read_channels that are reading different channels, since bluesky
+        only allows reading the same channels inside one stream."""
         # checking compatibility with other readings
         chan_list = self.get_channels_set()
         if set(chan_list) in variables_handling.read_channel_sets:
             n = variables_handling.read_channel_sets.index(set(chan_list))
         else:
             n = len(variables_handling.read_channel_names)
             variables_handling.read_channel_sets.append(chan_list)
@@ -102,40 +110,28 @@
             protocol_string += f'{tabs}yield from helper_functions.read_wo_trigger(channels_{self.variable_name()}, grp_{self.variable_name()}, stream={stream_name})\n'
         else:
             protocol_string += self.get_channels_string(tabs)
             protocol_string += f'{tabs}yield from bps.trigger_and_read(channels_{self.variable_name()}, name={stream_name})\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Includes the channel list in the string."""
         short_string = super().get_protocol_short_string(n_tabs)
         short_string = f'{short_string[:-1]} - {self.channel_list}\n'
         return short_string
 
 def get_channel_string(channel):
     """
+    Gives the string of a channel in the way it is written inside the
+    protocol, i.e. "devs["<device_name>"].<component/channel_name>".
 
     Parameters
     ----------
-    channel :
-        
-
-    Returns
-    -------
-
+    channel : str
+        The channel that should be converted.
     """
     name = variables_handling.channels[channel].name
     if '.' in name:
         dev, chan = name.split('.')
         return f'devs["{dev}"].{chan}, '
     else:
         return f'devs["{name}"], '
@@ -311,60 +307,48 @@
         self.tableWidget_channels.resizeColumnsToContents()
         # for channel in self.loop_step.channel_dict:
         #     if channel not in variables_handling.channels:
         #         self.loop_step.channel_dict.pop(channel)
 
 
 class Trigger_Channels_Step(Loop_Step):
-    """ """
+    """
+    This step provides a split between triggering and reading channels.
+
+    Attributes
+    ----------
+    read_step : str
+        The name of the Read Channels step, for which this step should do the
+        triggering.
+    """
 
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Trigger Channels'
         if step_info is None:
             step_info = {}
         self.read_step = step_info['read_step'] if 'read_step' in step_info else ''
 
     def get_protocol_string(self, n_tabs=1):
         """In the protocol, at first a list `channels` is defined,
         including all the channels, that are selected to be read. Then
-        bps.trigger_and_read is called on these channels.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        these channels are triggered with `helper_functions.trigger_multi`."""
         tabs = '\t' * n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         if self.read_step not in variables_handling.current_protocol.loop_step_dict:
             raise Exception(f'Trying to trigger channels for read_channels "{self.read_step}" but it is not there.\n{self.full_name}')
         read_step = variables_handling.current_protocol.loop_step_dict[self.read_step]
         protocol_string += read_step.get_channels_string(tabs)
         step_name = read_step.variable_name()
         protocol_string += f'{tabs}grp_{step_name} = bps._short_uid("trigger")\n'
         protocol_string += f'{tabs}yield from helper_functions.trigger_multi(channels_{step_name}, grp_{step_name})\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """The corresponding read step is displayed."""
         short_string = super().get_protocol_short_string(n_tabs)
         read_step = variables_handling.current_protocol.loop_step_dict[self.read_step]
         short_string = f'{short_string[:-1]} - {read_step.channel_list}\n'
         return short_string
 
 
 class Trigger_Channels_Config(Loop_Step_Config):
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/run_subprotocol.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/run_subprotocol.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,39 +7,53 @@
 from nomad_camels.utility import variables_handling, load_save_functions
 from nomad_camels.ui_widgets.add_remove_table import AddRemoveTable
 from nomad_camels.bluesky_handling import protocol_builder, builder_helper_functions
 
 
 
 class Run_Subprotocol(Loop_Step):
-    """ """
+    """
+    With this step, one may select another protocol to run inside the main one.
+
+    Attributes
+    ----------
+    prot_path : str, path
+        Path to the file of the subprotocol.
+    vars_in : dict
+        Variables of the subprotocol's namespace and the values they should get
+        before the subprotocol is run. This can be used to e.g. give the
+        subprotocol a new value for each run inside a loop.
+    vars_out : dict
+        Variables of the subprotocol and the name in the main protocol's
+        namespace where they should be put. This can be used to e.g. store some
+        value determined by the subprotocol for later use in the main protocol.
+    data_output : str
+        Whether the data is put into its own stream('sub-stream') or the primary
+        stream ('main-stream').
+    own_plots : bool
+        If True, the plots specified by the protocol will also be shown.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Run Subprotocol'
         if step_info is None:
             step_info = {}
         self.prot_path = step_info['prot_path'] if 'prot_path' in step_info else ''
         self.vars_in = step_info['vars_in'] if 'vars_in' in step_info else {}
         self.vars_out = step_info['vars_out'] if 'vars_out' in step_info else {}
         self.data_output = step_info['data_output'] if 'data_output' in step_info else 'sub-stream'
         self.own_plots = step_info['own_plots'] if 'own_plots' in step_info else True
 
 
     def get_protocol_string(self, n_tabs=1):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """Overwrites the signal for the progressbar and the number of steps in
+        the subprotocol's module. Evaluates the input variables, then writes
+        them into the subprotocol's namespace and starts the subprotocol's
+        _plan_inner function. Afterwards the output variables are written to the
+        main namespace."""
         tabs = '\t' * n_tabs
         prot_name = os.path.basename(self.prot_path)[:-6]
         protocol_string = super().get_protocol_string(n_tabs)
         protocol_string += f'{tabs}{prot_name}_mod.protocol_step_information["protocol_stepper_signal"] = protocol_step_information["protocol_stepper_signal"]\n'
         protocol_string += f'{tabs}{prot_name}_mod.protocol_step_information["total_protocol_steps"] = {self.time_weight}\n'
         for i, var in enumerate(self.vars_in['Variable']):
             protocol_string += f'{tabs}{prot_name}_mod.namespace["{var}"] = eva.eval("{self.vars_in["Value"][i]}")\n'
@@ -48,62 +62,52 @@
             stream = 'primary'
         protocol_string += f'{tabs}yield from {prot_name}_mod.{prot_name}_plan_inner(devs, eva, "{stream}")\n'
         for i, var in enumerate(self.vars_out['Variable']):
             protocol_string += f'{tabs}namespace["{self.vars_out["Write to name"][i]}"] = {prot_name}_mod.namespace["{var}"]\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Specifies the name / path of the subprotocol."""
         short_string = super().get_protocol_short_string(n_tabs)
         short_string = f'{short_string[:-1]} - {self.prot_path}'
         return short_string
 
     def get_outer_string(self):
-        """ """
+        """Imports the subprotocol as <protocol_name>_mod."""
         prot_name = os.path.basename(self.prot_path)[:-6]
         py_file = f'{self.prot_path[:-6]}.py'
         if not os.path.isfile(py_file):
             sub_protocol = load_save_functions.load_protocol(self.prot_path)
             protocol_builder.build_protocol(sub_protocol, py_file)
         outer_string = f'spec = importlib.util.spec_from_file_location("{prot_name}", "{py_file}")\n'
         outer_string += f'{prot_name}_mod = importlib.util.module_from_spec(spec)\n'
         outer_string += f'sys.modules[spec.name] = {prot_name}_mod\n'
         outer_string += f'spec.loader.exec_module({prot_name}_mod)\n'
         return outer_string
 
     def get_add_main_string(self):
-        """ """
-        prot_name = os.path.basename(self.prot_path)[:-6]
-        stream = f'"{prot_name}"'
-        if self.data_output == 'main stream':
-            stream = '"primary"'
+        """If using its own plots, adds them to the steps. In any case, the
+        added steps from the subprotocol are added here as well."""
         prot_name = os.path.basename(self.prot_path)[:-6]
         add_main_string = ''
         if self.own_plots:
+            stream = f'"{prot_name}"'
+            if self.data_output == 'main stream':
+                stream = '"primary"'
             add_main_string += builder_helper_functions.get_plot_add_string(prot_name, stream, True)
         add_main_string += f'\treturner["{prot_name}_steps"] = {prot_name}_mod.steps_add_main(RE)\n'
         return add_main_string
 
     def update_used_devices(self):
-        """ """
+        """Uses the devices that are used in the subprotocol."""
         sub_protocol = load_save_functions.load_protocol(self.prot_path)
         self.used_devices = sub_protocol.get_used_devices()
 
     def update_time_weight(self):
-        """ """
+        """The time weight in the end is the weight of the subprotocol + 1."""
         super().update_time_weight()
         sub_protocol = load_save_functions.load_protocol(self.prot_path)
         self.time_weight += sub_protocol.get_total_steps()
 
 
 
 class Run_Subprotocol_Config(Loop_Step_Config):
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/set_channels.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/set_channels.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,28 @@
 from nomad_camels.main_classes.loop_step import Loop_Step, Loop_Step_Config
 
 from nomad_camels.ui_widgets.channels_check_table import Channels_Check_Table
 from nomad_camels.utility import variables_handling
 
 
 class Set_Channels(Loop_Step):
-    """Simple loop_step to set some channels."""
+    """
+    Simple step to set several channels to a given value. Uses `bps.abs_set`.
+
+    Attributes
+    ----------
+    channels_values : dict{'Channels': list[str], 'Values': list[str]}
+        This dictionary provides a list of the names of the channels that are to
+        be set and a list of the values they should get. The values are strings,
+        since they will be evaluated at runtime, thus providing the ability to
+        set some variable at runtime.
+    wait_for_set : bool, default True
+        Whether to wait after setting for the set channels to have the finished
+        status.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Set Channels'
         if step_info is None:
             step_info = {}
         self.channels_values = step_info['channels_values'] if 'channels_values' in step_info else {'Channels': [], 'Values': []}
         self.wait_for_set = step_info['wait_for_set'] if 'wait_for_set' in step_info else True
@@ -24,49 +37,30 @@
             if channel in variables_handling.channels:
                 device = variables_handling.channels[channel].device
                 if device not in self.used_devices:
                     self.used_devices.append(device)
 
     def get_protocol_string(self, n_tabs=1):
         """If `wait_for_set` is True, then after setting, bps.wait for
-        the set group is called.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        the set group is called. In any case, all the channels are set to their
+        specified value"""
         tabs = '\t' * n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         for i, channel in enumerate(self.channels_values['Channels']):
             if channel not in variables_handling.channels:
                 raise Exception(f'Trying to set channel {channel} in {self.full_name}, but it does not exist!')
             dev, chan = variables_handling.channels[channel].name.split('.')
             val = self.channels_values['Values'][i]
             protocol_string += f'{tabs}yield from bps.abs_set(devs["{dev}"].{chan}, eva.eval("{val}"), group="A")\n'
         if self.wait_for_set:
             protocol_string += f'{tabs}yield from bps.wait("A")\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Displays the channels and their values."""
         short_string = super().get_protocol_short_string(n_tabs)
         short_string = f'{short_string[:-1]} - {self.channels_values}\n'
         return short_string
 
 
 class Set_Channels_Config(Loop_Step_Config):
     """The configuration consists of the checkbox for waiting and a
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/set_value_popup.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/set_value_popup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,37 +3,44 @@
 from nomad_camels.main_classes.loop_step import Loop_Step, Loop_Step_Config
 
 from nomad_camels.ui_widgets.add_remove_table import AddRemoveTable
 from nomad_camels.ui_widgets.channels_check_table import Channels_Check_Table
 
 
 class Set_Value_Popup(Loop_Step):
-    """ """
+    """
+    This step provides the possibility for the user to set a channel or variable
+    to a specific value at runtime with a popup. The protocol execution is
+    paused until the user is finished.
+
+    Attributes
+    ----------
+    variables : list[str]
+        A list of the variables that should be set by the user.
+    channels : list[str]
+        A list of the channels that should be set by the user.
+    free_variables : bool
+        If True, the user has the possibility to set any variable freely.
+    free_channels : bool
+        If True, the user has the possibility to set any channel freely.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Set Value Popup'
         if step_info is None:
             step_info = {}
         self.variables = step_info['variables'] if 'variables' in step_info else []
         self.channels = step_info['channels'] if 'channels' in step_info else []
         self.free_variables = step_info['free_variables'] if 'free_variables' in step_info else False
         self.free_channels = step_info['free_channels'] if 'free_channels' in step_info else False
 
     def get_protocol_string(self, n_tabs=1):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """The value popup box is executed. The protocol waits until its
+        completion. Then all the variables and then the channels are set to the
+        given values."""
         tabs = '\t' * n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         protocol_string += f'{tabs}boxes["values_{self.name}"].done = False\n'
         protocol_string += f'{tabs}boxes["values_{self.name}"].helper.executor.emit()\n'
         protocol_string += f'{tabs}while not boxes["values_{self.name}"].done:\n'
         protocol_string += f'{tabs}\tyield from bps.sleep(0.1)\n'
         protocol_string += f'{tabs}if boxes["values_{self.name}"].was_accepted:\n'
@@ -42,15 +49,15 @@
         protocol_string += f'{tabs}\tfor chan, val in boxes["values_{self.name}"].set_channels.items():\n'
         protocol_string += f'{tabs}\t\tdev, channel_name = boxes["values_{self.name}"].channel_devs[chan]\n'
         protocol_string += f'{tabs}\t\tyield from bps.abs_set(getattr(devs[dev], channel_name), eva.eval(str(val)), group="A")\n'
         protocol_string += f'{tabs}\tyield from bps.wait("A")\n'
         return protocol_string
 
     def get_add_main_string(self):
-        """ """
+        """Adds the setup of the box."""
         add_main_string = super().get_add_main_string()
         add_main_string += f'\tboxes["values_{self.name}"] = helper_functions.Value_Box("", "Set Values!", {self.variables}, {self.channels}, {self.free_variables}, {self.free_channels}, devs=devs)\n'
         return add_main_string
 
 
 class Set_Value_Popup_Config(Loop_Step_Config):
     """ """
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/set_variables.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/set_variables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,44 @@
 from nomad_camels.main_classes.loop_step import Loop_Step, Loop_Step_Config
 
 from nomad_camels.ui_widgets.add_remove_table import AddRemoveTable
 from nomad_camels.utility import variables_handling
 
 class Set_Variables(Loop_Step):
-    """ """
+    """
+    This step enables setting variables to a different value during the protocol.
+
+    Attributes
+    ----------
+    variables_values : dict{'Variable': list[str], 'Value': list[str]}
+        Contains a list of the variables and a list of the respective values to
+        which they should be set.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Set Variables'
         if step_info is None:
             step_info = {}
         self.variables_values = step_info['variables_values'] if 'variables_values' in step_info else {'Variable': [], 'Value': []}
 
     def get_protocol_string(self, n_tabs=1):
-        """If `wait_for_set` is True, then after setting, bps.wait for
-        the set group is called.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """Evaluates the values for the variables, then updates the namespace."""
         tabs = '\t' * n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         for i, variable in enumerate(self.variables_values['Variable']):
             val = variables_handling.get_write_from_data_type(self.variables_values['Value'][i])
             if isinstance(val, str):
                 protocol_string += f'{tabs}{variable} = eva.eval({val})\n'
             else:
                 protocol_string += f'{tabs}{variable} = {val}\n'
             protocol_string += f'{tabs}namespace["{variable}"] = {variable}\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Shows the variables and values."""
         short_string = super().get_protocol_short_string(n_tabs)
         short_string = f'{short_string[:-1]} - {self.variables_values}\n'
         return short_string
 
 
 class Set_Variables_Config(Loop_Step_Config):
     """ """
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/simple_sweep.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/simple_sweep.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,99 +7,85 @@
 from nomad_camels.utility.load_save_helper_functions import load_plots
 from nomad_camels.bluesky_handling import builder_helper_functions
 from nomad_camels.frontpanels.plot_definer import Plot_Button_Overview
 
 from nomad_camels.loop_steps.for_while_loops import For_Loop_Step_Config_Sub, For_Loop_Step
 
 class Simple_Sweep(For_Loop_Step):
-    """ """
+    """
+    A sweep over a single channel reading arbitrary other channels. The
+    information about which values to sweep through are inherited from
+    For_Loop_Step.
+
+    Attributes
+    ----------
+    sweep_channel : str
+        The name of the channel that should be sweeped.
+    data_output : str
+        Whether the data is put into its own stream('sub-stream') or the primary
+        stream ('main-stream').
+    plots : list[Plot_Info]
+        List of the plots that should be created for the sweep.
+    read_channels : list[str]
+        List of the channels that should be read during the sweep.
+    """
     def __init__(self, name='', children=None, parent_step=None, step_info=None,
                  **kwargs):
         super().__init__(name, children, parent_step, step_info, **kwargs)
         step_info = step_info or {}
         self.step_type = 'Simple Sweep'
         self.has_children = False
         self.sweep_channel = step_info['sweep_channel'] if 'sweep_channel' in step_info else ''
         self.data_output = step_info['data_output'] if 'data_output' in step_info else 'sub-stream'
         self.plots = load_plots([], step_info['plots']) if 'plots' in step_info else []
         self.read_channels = step_info['read_channels'] if 'read_channels' in step_info else []
-        self.use_own_plots = step_info['use_own_plots'] if 'use_own_plots' in step_info else False
-        self.calc_minmax = step_info['calc_minmax'] if 'calc_minmax' in step_info else False
-        self.calc_mean = step_info['calc_mean'] if 'calc_mean' in step_info else False
-        self.calc_stddev = step_info['calc_stddev'] if 'calc_stddev' in step_info else False
-        self.use_custom_fit = step_info['use_custom_fit'] if 'use_custom_fit' in step_info else False
-        self.calc_fit = step_info['calc_fit'] if 'calc_fit' in step_info else False
-        self.predef_fit = step_info['predef_fit'] if 'predef_fit' in step_info else 'Linear'
-        self.custom_fit = step_info['custom_fit'] if 'custom_fit' in step_info else ''
-        self.fit_params = step_info['fit_params'] if 'fit_params' in step_info else {}
-        self.guess_fit_params = step_info['guess_fit_params'] if 'guess_fit_params' in step_info else True
 
     def update_used_devices(self):
-        """ """
+        """Includes the devices from the read_channels and the sweep_channel."""
         self.used_devices = []
         set_device = variables_handling.channels[self.sweep_channel].device
         self.used_devices.append(set_device)
         for channel in self.read_channels:
             if channel in variables_handling.channels:
                 device = variables_handling.channels[channel].device
                 if device not in self.used_devices:
                     self.used_devices.append(device)
 
     def update_variables(self):
-        """ """
+        """Adds the fit variables from the plots."""
         variables = {}
         stream = f'{self.name}'
         for plot in self.plots:
             variables.update(plot.get_fit_vars(stream))
         variables_handling.loop_step_variables.update(variables)
         super().update_variables()
 
 
 
     def get_outer_string(self):
-        """ """
-        if self.use_own_plots:
+        """Gives the string to create the plots of the sweeps"""
+        if self.plots:
             return builder_helper_functions.plot_creator(self.plots,
                                                          f'create_plots_{self.name}')[0]
         return ''
 
     def get_add_main_string(self):
-        """ """
+        """Calling the plot_creator from steps_add_main"""
         stream = f'"{self.name}"'
         if self.data_output == 'main stream':
             stream = '"primary"'
         add_main_string = ''
-        if self.use_own_plots:
+        if self.plots:
             add_main_string += builder_helper_functions.get_plot_add_string(self.name, stream)
         return add_main_string
 
     def get_protocol_string(self, n_tabs=1):
-        """The loop is enumerating over the selected points.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """The channels to be read are set up. Then a for loop for the sweep is
+        started, setting the channel, then reading."""
         tabs = '\t'*n_tabs
-        # if self.loop_type in ['start - stop', 'start - min - max - stop',
-        #                       'start - max - min - stop']:
-        #     enumerator = get_space_string(self.start_val, self.stop_val,
-        #                                   self.n_points, self.min_val,
-        #                                   self.max_val, self.loop_type,
-        #                                   self.sweep_mode,
-        #                                   self.include_end_points)
-        # elif self.loop_type == 'Value-List':
-        #     enumerator = self.val_list
-        # else:
-        #     enumerator = f'np.loadtxt("{self.file_path}")'
 
         stream = f'"{self.name}"'
         if self.data_output == 'main stream':
             stream = 'stream_name'
 
         protocol_string = f'{tabs}channels = ['
         for i, channel in enumerate(self.read_channels):
@@ -119,35 +105,23 @@
         name = variables_handling.channels[self.sweep_channel].name
         if '.' in name:
             dev, chan = name.split('.')
             setter = f'devs["{dev}"].{chan}'
         else:
             setter = f'devs["{name}"]'
 
-        # protocol_string += f'{tabs}for {self.name.replace(" ", "_")}_Count, {self.name.replace(" ", "_")}_Value in enumerate({enumerator}):\n'
-        # protocol_string += f'{tabs}\tnamespace.update({{"{self.name.replace(" ", "_")}_Count": {self.name.replace(" ", "_")}_Count, "{self.name.replace(" ", "_")}_Value": {self.name.replace(" ", "_")}_Value}})\n'
         protocol_string += f'{tabs}\tyield from bps.abs_set({setter}, {self.name.replace(" ", "_")}_Value, group="A")\n'
         protocol_string += f'{tabs}\tyield from bps.wait("A")\n'
         protocol_string += f'{tabs}\tyield from bps.trigger_and_read(channels, name={stream})\n'
         protocol_string += f'{tabs}yield from helper_functions.get_fit_results(all_fits, namespace, True, {stream})\n'
         self.update_time_weight()
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """The read and sweep channels and the sweep values are specified."""
         vals = super().get_protocol_short_string(n_tabs)[n_tabs+3:-1]
         tabs = '\t' * n_tabs
         short_string = f'{tabs}Sweep {self.sweep_channel}:\n{tabs}\tRead: {self.read_channels}\n{tabs}\tValues: {vals}'
         return short_string
 
 
 
@@ -181,32 +155,32 @@
         #                                  tableData=loop_step.read_channels,
         #                                  comboBoxes=in_box)
         labels = ['read', 'channel']
         info_dict = {'channel': self.loop_step.read_channels}
         self.read_table = Channels_Check_Table(self, labels, info_dict=info_dict,
                                                title='Read-Channels')
 
-        self.checkBox_use_own_plots = QCheckBox('Use own Plots')
-        self.checkBox_use_own_plots.setChecked(loop_step.use_own_plots)
+        # self.checkBox_use_own_plots = QCheckBox('Use own Plots')
+        # self.checkBox_use_own_plots.setChecked(loop_step.use_own_plots)
 
         self.plot_widge = Plot_Button_Overview(self, self.loop_step.plots)
 
-        label_proc = QLabel('Data processing')
+        # label_proc = QLabel('Data processing')
         font = QFont()
         font.setBold(True)
-        label_proc.setStyleSheet('font-size: 9pt')
-        label_proc.setFont(font)
-        self.checkBox_minmax = QCheckBox('Calculate min/max')
-        self.checkBox_minmax.setChecked(loop_step.calc_minmax)
-        self.checkBox_mean = QCheckBox('Calculate mean')
-        self.checkBox_mean.setChecked(loop_step.calc_mean)
-        self.checkBox_stddev = QCheckBox('Calculate standard deviation')
-        self.checkBox_stddev.setChecked(loop_step.calc_stddev)
+        # label_proc.setStyleSheet('font-size: 9pt')
+        # label_proc.setFont(font)
+        # self.checkBox_minmax = QCheckBox('Calculate min/max')
+        # self.checkBox_minmax.setChecked(loop_step.calc_minmax)
+        # self.checkBox_mean = QCheckBox('Calculate mean')
+        # self.checkBox_mean.setChecked(loop_step.calc_mean)
+        # self.checkBox_stddev = QCheckBox('Calculate standard deviation')
+        # self.checkBox_stddev.setChecked(loop_step.calc_stddev)
         # self.checkBox_fit = QCheckBox('Calculate fit')
-        # self.checkBox_fit.setChecked(loop_step.calc_fit)
+#         # self.checkBox_fit.setChecked(loop_step.calc_fit)
         # self.checkBox_fit.clicked.connect(self.change_fitting)
         # self.checkBox_guess_fit = QCheckBox('Guess initial params')
         # self.checkBox_guess_fit.setChecked(loop_step.guess_fit_params)
         # self.checkBox_guess_fit.clicked.connect(self.change_fitting)
         # self.radioButton_predev = QRadioButton('Predefined function')
         # self.radioButton_own = QRadioButton('Own function')
         # self.radioButton_predev.setChecked(True)
@@ -238,32 +212,32 @@
         self.layout().addWidget(self.comboBox_sweep_channel, 1, 1, 1, 4)
         self.layout().addWidget(label_data, 2, 0)
         self.layout().addWidget(self.comboBox_data_output, 2, 1, 1, 4)
         self.layout().addWidget(self.sweep_widget, 5, 0, 1, 5)
         self.layout().addWidget(self.read_table, 6, 0, 1, 5)
 
         self.layout().addWidget(self.plot_widge, 8, 0, 1, 5)
-        self.layout().addWidget(self.checkBox_use_own_plots, 7, 0, 1, 5)
+        # self.layout().addWidget(self.checkBox_use_own_plots, 7, 0, 1, 5)
         # self.layout().addWidget(self.plot_table, 7, 2, 1, 3)
-        self.checkBox_use_own_plots.clicked.connect(self.use_plot_change)
+        # self.checkBox_use_own_plots.clicked.connect(self.use_plot_change)
 
-        self.layout().addWidget(label_proc, 10, 0, 1, 5)
-        self.layout().addWidget(self.checkBox_minmax, 11, 0, 1, 2)
-        self.layout().addWidget(self.checkBox_mean, 11, 2, 1, 3)
-        self.layout().addWidget(self.checkBox_stddev, 13, 0, 1, 2)
+        # self.layout().addWidget(label_proc, 10, 0, 1, 5)
+        # self.layout().addWidget(self.checkBox_minmax, 11, 0, 1, 2)
+        # self.layout().addWidget(self.checkBox_mean, 11, 2, 1, 3)
+        # self.layout().addWidget(self.checkBox_stddev, 13, 0, 1, 2)
         # self.layout().addWidget(self.checkBox_fit, 20, 0, 1, 2)
         # self.layout().addWidget(self.checkBox_guess_fit, 20, 2, 1, 3)
         # self.layout().addWidget(self.radioButton_predev, 21, 0, 1, 2)
         # self.layout().addWidget(self.radioButton_own, 21, 2, 1, 3)
         # self.layout().addWidget(self.comboBox_fit, 22, 0, 1, 2)
         # self.layout().addWidget(self.lineEdit_fit_func, 22, 2, 1, 3)
         # self.layout().addWidget(self.start_params, 23, 0, 1, 5)
 
 
-        self.use_plot_change()
+        # self.use_plot_change()
 
     # def setup_plots(self):
     #     """Called when any preferences are changed. Makes the dictionary
     #      of preferences and calls save_preferences from the
     #      load_save_functions module."""
     #     plot_dialog = Plot_Definer(self)
     #     plot_dialog.exec()
@@ -275,33 +249,33 @@
         #     load_save_functions.save_preferences(self.preferences)
         #     variables_handling.device_driver_path = self.preferences['device_driver_path']
         #     variables_handling.meas_files_path = self.preferences['meas_files_path']
         # prefs = {'autosave': self.actionAutosave_on_closing.isChecked(),
         #          'dark_mode': self.actionDark_Mode.isChecked()}
         # load_save_functions.save_preferences(prefs)
 
-    def use_plot_change(self):
-        """ """
-        use_plots = self.checkBox_use_own_plots.isChecked()
-        self.plot_widge.setEnabled(use_plots)
+    # def use_plot_change(self):
+    #     """ """
+    #     use_plots = self.checkBox_use_own_plots.isChecked()
+    #     self.plot_widge.setEnabled(use_plots)
 
 
 
 
     def update_step_config(self):
         """ """
         super().update_step_config()
-        self.loop_step.use_own_plots = self.checkBox_use_own_plots.isChecked()
+        # self.loop_step.use_own_plots = self.checkBox_use_own_plots.isChecked()
         self.loop_step.plots = self.plot_widge.plot_data
         # self.loop_step.plots = self.plot_table.update_table_data()
         self.loop_step.read_channels = self.read_table.get_info()['channel']
         self.loop_step.data_output = self.comboBox_data_output.currentText()
         self.loop_step.sweep_channel = self.comboBox_sweep_channel.currentText()
-        self.loop_step.calc_minmax = self.checkBox_minmax.isChecked()
-        self.loop_step.calc_mean = self.checkBox_mean.isChecked()
-        self.loop_step.calc_stddev = self.checkBox_stddev.isChecked()
-        # self.loop_step.calc_fit = self.checkBox_fit.isChecked()
+        # self.loop_step.calc_minmax = self.checkBox_minmax.isChecked()
+        # self.loop_step.calc_mean = self.checkBox_mean.isChecked()
+        # self.loop_step.calc_stddev = self.checkBox_stddev.isChecked()
+        # # self.loop_step.calc_fit = self.checkBox_fit.isChecked()
         # self.loop_step.use_custom_fit = self.radioButton_own.isChecked()
         # self.loop_step.predef_fit = self.comboBox_fit.currentText()
         # self.loop_step.custom_fit = self.lineEdit_fit_func.text()
```

### Comparing `nomad_camels-0.1.4/nomad_camels/loop_steps/wait_loop_step.py` & `nomad_camels-0.1.5/nomad_camels/loop_steps/wait_loop_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 from PySide6.QtWidgets import QWidget, QLabel, QGridLayout
 
 from nomad_camels.main_classes.loop_step import Loop_Step_Config, Loop_Step
 from nomad_camels.ui_widgets.variable_tool_tip_box import Variable_Box
 
 class Wait_Loop_Step(Loop_Step):
-    """A loopstep to simply wait some defined time."""
+    """
+    A loopstep to simply wait some defined time.
+
+    Attributes
+    ----------
+    wait_time : str, float
+        The how long the protocol execution should pause in seconds.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Wait'
         if step_info is None:
             step_info = {}
         self.wait_time = step_info['wait_time'] if 'wait_time' in step_info else 0.0
 
     def get_protocol_string(self, n_tabs=1):
-        """The protocol just calls `bps.wait(`wait_time`)`.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """The protocol just calls `bps.wait(`wait_time`)`, where `wait_time` is
+        evaluated by the protocol's evaluator."""
         tabs = '\t' * n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         protocol_string += f'{tabs}yield from bps.sleep(eva.eval("{self.wait_time}"))\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Tells the wait time."""
         short_string = super().get_protocol_short_string(n_tabs)
         short_string = f'{short_string[:-1]} - {self.wait_time} s\n'
         return short_string
 
 
 class Wait_Loop_Step_Config(Loop_Step_Config):
     """The configuration just provides a line to enter the time to wait."""
```

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/device_class.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/device_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,43 +7,40 @@
 from ophyd import Device as OphydDevice
 from ophyd.signal import SignalRO
 
 from nomad_camels.main_classes.measurement_channel import Measurement_Channel
 
 
 class Device:
-    """General class for all devices
+    """General class for all devices/instruments.
     
-    The subclasses of this class should all be called "subclass", they
-    are imported via importlib in that way.
+    If subclassing this in a driver, subclass should be called "subclass", it
+    will be imported via importlib in that way.
     Any derived device should also provide the name of its ophyd-class
     as a string self.ophyd_class_name.
 
-    Parameters
-    ----------
-
-    Returns
-    -------
-
     Attributes
     ----------
     name : str
         represents the device, should be unique
     virtual : bool
         whether the device does not need any hardware
     tags : list
         list of strings for the device search
     ophyd_class_name : str
         name of the class of ophyd_device
     settings : dict
         settings handed to the ophyd class at runtime of the protocol
     config : dict
-        values, the config-attributes should be set to
+        values, the config-attributes / components of the ophyd device should be
+        set to
     channels : dict
         channels of the device (i.e.: Signals that are not config)
+    controls : dict
+        Dictionary of additional manual controls this device provides
     """
 
     def __init__(self, name='', virtual=False, tags=None, ophyd_device=None,
                  ophyd_class_name='', additional_info=None, **kwargs):
         """
         Parameters
         ----------
@@ -84,69 +81,79 @@
                 if check_output(cls):
                     self.config.update({f'{name}': 0})
                 else:
                     self.passive_config.update({f'{name}': 0})
         self.controls = {}
 
     def get_necessary_devices(self):
-        """ """
+        """Returns a list of the devices that this device needs to function
+        (e.g. for a PID controller)."""
         return []
 
     def get_controls(self):
-        """ """
+        """Returns the device's specific manual controls.
+
+        Returns
+        -------
+        self.controls : dict
+            Dictionary of the device's manual controls
+        """
         return self.controls
 
     def get_finalize_steps(self):
-        """ """
+        """Returns the string used in the 'finally' part of the protocol's main
+        function to e.g. close the instrument communication.
+
+        Returns
+        -------
+        step_str : str
+        """
         return ''
 
     def get_passive_config(self):
-        """ """
+        """Not used."""
         return self.passive_config
 
     def get_config(self):
         """returns self.config, should be overwritten for special
         purposes (e.g. leaving out some keys of the dictionary)
 
-        Parameters
-        ----------
-
         Returns
         -------
-
+        self.config : dict
         """
         return self.config
 
     def get_settings(self):
         """returns self.settings, should be overwritten for special
         purposes (e.g. leaving out some keys of the dictionary)
 
-        Parameters
-        ----------
-
         Returns
         -------
-
+        self.settings : dict
         """
         return self.settings
 
     def get_additional_info(self):
-        """ """
+        """Returns the additional information about the instrument.
+
+        Returns
+        -------
+        self.additional_info : dict
+        """
         return self.additional_info
 
     def get_channels(self):
         """returns self.channels, should be overwritten for special
         purposes (e.g. leaving out some keys of the dictionary)
 
-        Parameters
-        ----------
-
         Returns
         -------
-
+        self.channels : dict
+            dictionary containing the device's channels
         """
         self.channels = {}
         outputs = get_outputs(self.ophyd_instance)
         for chan_info in get_channels(self.ophyd_instance,
                                       include_metadata=True):
             chan, metadata = chan_info
             is_out = chan in outputs
@@ -156,34 +163,28 @@
             self.channels.update({f'{self.custom_name}_{chan}': channel})
         return self.channels
 
     def get_additional_string(self):
         """returns a string that will be added into the protocol after
         connecting to the device.
 
-        Parameters
-        ----------
-
         Returns
         -------
-
+        additional_str : str
         """
         return ''
 
     def get_special_steps(self):
         """returns a dictionary containing containing device-specific
         loopsteps. The key is the loopstep's name, the value a list
         containing the Class of the step, and its config-widget.
 
-        Parameters
-        ----------
-
         Returns
         -------
-
+        steps : dict{'<step_name>': [Step_Class, Step_Config]}
         """
         return {}
 
 def check_output(cls) -> bool:
     """Returns False if the give `cls` is an instance of a read-only Signal."""
     output = not issubclass(cls, EpicsSignalRO)
     output = output and not issubclass(cls, SignalRO)
@@ -191,20 +192,22 @@
 
 def get_outputs(dev:OphydDevice):
     """walks through the components of an ophyd-device and checks
     whether they can be written
 
     Parameters
     ----------
-    dev:OphydDevice :
+    dev : ophyd.Device
+        The device that should be checked
         
 
     Returns
     -------
-
+    outputs : list
+        List of the outputs' names
     """
     outputs = []
     for comp in dev.walk_components():
         cls = comp.item.cls
         name = comp.item.attr
         if check_output(cls):
             outputs.append(name)
@@ -212,21 +215,26 @@
 
 def get_channels(dev:OphydDevice, include_metadata=False):
     """returns the components of an ophyd-device that are not listed in
     the configuration
 
     Parameters
     ----------
-    dev:OphydDevice :
+    dev : ophyd.Device
+        The device that should be checked
 
-    include_metadata: bool
+    include_metadata : bool, default False
+        If True, also returns the compnents' metadata
 
     Returns
     -------
-
+    channels : list
+        list of the device's channels
+        if metadata is True, it will be a list of tuples conaining the channels'
+        names and their metadata
     """
     channels = []
     for comp in dev.walk_components():
         name = comp.item.attr
         if name not in dev.configuration_attrs:
             if include_metadata:
                 if hasattr(comp.item, 'kwargs') and 'metadata' in comp.item.kwargs:
```

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/list_plot.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/list_plot.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/loop_step.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/manual_control.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/manual_control.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,33 @@
 
 from nomad_camels.utility import device_handling, variables_handling
 
 from pkg_resources import resource_filename
 
 
 class Manual_Control(QWidget):
-    """ """
+    """
+    Parent class for manual controls.
+
+    This class provides the core functionality of a manual control in CAMELS.
+    The parameters `device`, `device_list` and `ophyd_device` may or may not be
+    used by the child class.
+
+    Attributes
+    ----------
+    name : str
+        The name of the manual control. It also determines the window title.
+    device : str, None
+        The device the manual control is using
+    device_list : list
+        A list of the devices, used. The specific implementation lies in the
+        child classes.
+    ophyd_device : ophyd.Device
+        The device's representation in ophyd.
+    """
     closing = Signal()
 
     def __init__(self, parent=None, title='Manual Control', control_data=None):
         super().__init__()
         # layout = QGridLayout()
         # self.setLayout(layout)
         control_data = control_data or {}
@@ -27,41 +45,23 @@
 
     # def close(self) -> bool:
     #     # device_handling.close_devices(self.device_list)
     #     self.closing.emit()
     #     return super().close()
 
     def closeEvent(self, a0: QCloseEvent) -> None:
-        """
-
-        Parameters
-        ----------
-        a0: QCloseEvent :
-            
-
-        Returns
-        -------
-
-        """
+        """Overwritten, so that `self.closing` is emitted, telling the main UI
+        window that this manual control is no longer opened."""
         device_handling.close_devices(self.device_list)
         self.closing.emit()
         return super().closeEvent(a0)
 
     def start_device(self, device_name):
-        """
-
-        Parameters
-        ----------
-        device_name :
-            
-
-        Returns
-        -------
-
-        """
+        """Returns self.device as the corresponding device to `device_name`.
+        If it is not None, it will be instantiated."""
         self.device = variables_handling.devices[device_name]
         if self.device:
             self.device_list = self.device.get_necessary_devices()
             self.device_list = list(set(self.device_list))
             if self.device.name in self.device_list:
                 self.device_list.remove(self.device.custom_name)
             self.device_list.append(self.device.custom_name)
```

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/measurement_channel.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/measurement_channel.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/plot_2D.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/plot_2D.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/plot_widget.py` & `nomad_camels-0.1.5/nomad_camels/main_classes/plot_widget.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/main_classes/protocol_class.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/add_remove_table.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,603 +1,525 @@
-from PySide6.QtWidgets import QWidget, QCheckBox, QTextEdit
-from PySide6.QtGui import QStandardItemModel, QStandardItem
-from PySide6.QtCore import Signal
-
-from nomad_camels.frontpanels.plot_definer import Plot_Button_Overview
-from nomad_camels.loop_steps import make_step_of_type
-from nomad_camels.gui.general_protocol_settings import Ui_Protocol_Settings
+from PySide6.QtWidgets import QWidget, QGridLayout, QPushButton, QTableView,\
+    QLabel, QComboBox, QMenu, QDialog, QDialogButtonBox, QMessageBox
+from PySide6.QtGui import QStandardItemModel, QStandardItem, QFont, QBrush,\
+    QKeyEvent
+from PySide6.QtCore import Qt, Signal
+
+import numpy as np
+import pandas as pd
 
-from nomad_camels.ui_widgets.add_remove_table import AddRemoveTable
 from nomad_camels.utility import variables_handling
 
 
-class Measurement_Protocol:
-    """Class for the measurement protocols. It mainly contains
-    loop_steps and plots.
+class AddRemoveTable(QWidget):
+    """This widget provides a QTableView and two buttons for adding /
+    removing rows / columns.
 
     Parameters
     ----------
 
     Returns
     -------
 
     """
-    def __init__(self, loop_steps=None, plots=None, channels=None, name='',
-                 channel_metadata=None, metadata=None, use_nexus=False,
-                 config_metadata=None, **kwargs):
-        if plots is None:
-            plots = []
-        if loop_steps is None:
-            loop_steps = []
-        if channels is None:
-            channels = {}
-        if channel_metadata is None:
-            channel_metadata = {}
-        if metadata is None:
-            metadata = {}
-        self.description = kwargs['description'] if 'description' in kwargs else ''
-        self.export_csv = kwargs['export_csv'] if 'export_csv' in kwargs else False
-        self.export_json = kwargs['export_json'] if 'export_json' in kwargs else False
-        self.session_name = kwargs['session_name'] if 'session_name' in kwargs else ''
-        self.loop_steps = loop_steps
-        self.loop_step_dict = {}
-        for step in self.loop_steps:
-            update_all_children(self.loop_step_dict, step)
-        self.plots = plots
-        self.filename = ''
-        self.variables = {}
-        self.loop_step_variables = {}
-        self.channels = channels
-        self.name = name or 'Protocol'
-        self.channel_metadata = channel_metadata
-        self.config_metadata = config_metadata
-        self.metadata = metadata
-        self.use_nexus = use_nexus
-
-    def update_variables(self):
-        """Update all the variables provided by loopsteps."""
-        self.loop_step_variables.clear()
-        for step in self.loop_steps:
-            step.update_variables()
-
-    def get_nexus_paths(self):
-        """Get a dictionary containing the paths used for the output
-        NeXus-file.
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-
-        """
-        paths = {}
-        for i, name in enumerate(self.metadata['Name']):
-            paths[self.metadata['NeXus-path'][i]] = f'metadata_start/{name}'
-        for i, name in enumerate(self.channel_metadata['Channel']):
-            paths[self.channel_metadata['NeXus-path'][i]] = f'data/{name}'
-        for i, name in enumerate(self.config_metadata['Configuration']):
-            path = ''
-            for dev in variables_handling.devices:
-                if dev in name:
-                    rn = name.split(dev)[1][1:]
-                    device = variables_handling.devices[dev]
-                    if rn in device.get_config() or rn in device.get_config() or rn in device.get_passive_config():
-                        path = f'metadata_start/device_config/{dev}/{name}'
-                        break
-            if not path:
-                raise Exception(f"Cannot find {name} in any configuration!")
-            paths[self.config_metadata['NeXus-path'][i]] = path
-        return paths
-
-    def add_loop_step(self, loop_step, position=-1, parent_step_name=None, model=None):
-        """Adds a loop_step to the protocol (or the parent_step)at the specified
-        position. Also appends the loop_step to the given model. The
-        loop_step is added to the list as well as the dictionary.
-
-        Parameters
-        ----------
-        loop_step :
-            
-        position :
-             (Default value = -1)
-        parent_step_name :
-             (Default value = None)
-        model :
-             (Default value = None)
-
-        Returns
-        -------
-
-        
-        """
-        if parent_step_name is None:
-            if position < 0:
-                self.loop_steps.append(loop_step)
+    sizechange = Signal()
+    added = Signal(int)
+    removed = Signal(int)
+
+    def __init__(self, addLabel='+', removeLabel='-', horizontal=True,
+                 editables=None, checkables=(), headerLabels=None, orderBy=None,
+                 parent=None, tableData=None, title='', comboBoxes=None,
+                 subtables=None, growsize=False, checkstrings=None,
+                 askdelete=False, fixedsize=False, enableds=None):
+        """
+
+        Parameters
+        ----------
+        addLabel : str, default "+"
+            The label of the add-button
+        removeLabel : str, default "-"
+            The label of the remove-button
+        horizontal : bool, default True
+            True if the header is horizontal (thus the data in columns),
+            False if it is the other way round
+        editables : int, list of int, default None
+            Positions of the columns (if horizontal) that are editable,
+            If None, all are
+        checkables : int, list of int, default None
+            Positions of the columns (if horizontal) that have a
+            Checkbox, if None, none have
+        headerLabels : list of str, default None
+            The labels of the header, they are also used to provide the
+            format of the data returned by the AddRemoveTable
+        orderBy : None
+            not used (yet)
+        parent : QWidget
+            Parent of the Widget
+        tableData : dict, pd.DataFrame, list, default None
+            The data that should be put into the table. Should have the
+            format of headerLabels. If it is a dict, the format should
+            best look like {"column1": [data1, data2, ...], ...}
+            A list should be used, if the table is a subtable inside
+            another one
+        title : str, default ""
+            adds a QLabel on the top-right with `title`. If an empty
+            string, no label is added
+        comboBoxes : dict of lists of str
+            the keys of the dict specify in which columns (same name), a
+            comboBox should be used, the corresponding value gives the
+            possible choices of the comboBox
+        subtables : dict of lists
+            the keys of the dict specify in which columns (same name),
+            an additional AddRemoveTable should be contained
+        growsize : bool, default True
+            Whether to increase the MaximumSize of the Widget when more
+            data is contained
+        checkstrings : int, list of int, default None
+            Positions of the columns (if horizontal) that are to be
+            checked for validity, if None, none are
+        askdelete : bool, default False
+            Whether to have a PopUp make sure, that the user wants to
+            delete the selected column
+        """
+        super().__init__(parent)
+        self.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.customContextMenuRequested.connect(self.context_menu)
+        layout = QGridLayout()
+        layout.setContentsMargins(0,0,0,0)
+        self.setLayout(layout)
+        self.askdelete = askdelete
+        self.checkables = checkables if not type(checkables) is int else [checkables]
+        if checkstrings is None:
+            checkstrings = []
+        self.checkstrings = checkstrings if not type(checkstrings) is int else [checkstrings]
+        self.horizontal = horizontal
+        self.orderBy = orderBy
+        self.comboBoxes = {} if comboBoxes is None else comboBoxes
+        self.subtables = {} if subtables is None else subtables
+        self.growsize = growsize
+        self.fixedsize = fixedsize
+        self.boxes = []
+        self.tables = []
+        if headerLabels is None and tableData is not None:
+            headerLabels = tableData.keys()
+        elif tableData is None and headerLabels is not None:
+            tableData = {}
+        elif tableData is None and headerLabels is None:
+            raise Exception('Cannot create a table without Data Format (AddRemoveTable)')
+        if isinstance(tableData, dict):
+            tableData = pd.DataFrame(tableData)
+        for label in headerLabels:
+            if label not in tableData:
+                tableData.insert(headerLabels.index(label), label, ['']*len(tableData))
+        self.tableData = tableData
+        if editables is None:
+            editables = range(len(headerLabels))
+        self.editables = editables if not isinstance(editables, int) else [editables]
+        if enableds is None:
+            enableds = range(len(headerLabels))
+        self.enableds = enableds if not isinstance(enableds, int) else [enableds]
+
+        self.addButton = QPushButton(addLabel)
+        self.removeButton = QPushButton(removeLabel)
+        self.table = QTableView()
+        self.table_model = QStandardItemModel()
+        self.table.setModel(self.table_model)
+        mover = 0
+        if len(title):
+            label = QLabel(title)
+            layout.addWidget(label, 0, 0)
+            font = QFont()
+            font.setBold(True)
+            label.setStyleSheet('font-size: 9pt')
+            label.setFont(font)
+            mover = 1
+        layout.addWidget(self.addButton, 0, 0+mover)
+        layout.addWidget(self.removeButton, 0, 1+mover)
+        layout.addWidget(self.table, 1, 0, 1, 2+mover)
+
+        self.headerLabels = headerLabels
+        if horizontal:
+            self.table.verticalHeader().hide()
+            if len(headerLabels):
+                self.table_model.setHorizontalHeaderLabels(headerLabels)
+                self.table_model.setColumnCount(len(headerLabels))
             else:
-                self.loop_steps.insert(position, loop_step)
+                self.table_model.setColumnCount(1)
+                self.table.horizontalHeader().hide()
         else:
-            loop_step.parent_step = parent_step_name
-            self.loop_step_dict[parent_step_name].add_child(loop_step, position)
-        if model is not None:
-            loop_step.append_to_model(model)
-        self.loop_step_dict.update({loop_step.full_name: loop_step})
-
-    def add_loop_step_rec(self, loop_step, model=None, parent_step_name=None, position=-1):
-        """Recursively adds the loop_step and all its children to the
-        protocol. Steps are added to the list if they have no parent,
-        otherwise to the parent. All are added to the dictionary.
+            self.table.horizontalHeader().hide()
+            if len(headerLabels):
+                self.table_model.setVerticalHeaderLabels(headerLabels)
+                self.table_model.setRowCount(len(headerLabels))
+            else:
+                self.table_model.setRowCount(1)
+                self.table.verticalHeader().hide()
 
-        Parameters
-        ----------
-        loop_step :
-            
-        model :
-             (Default value = None)
-        parent_step_name :
-             (Default value = None)
-        position :
-             (Default value = -1)
+        self.addButton.clicked.connect(lambda x: self.add())
+        self.removeButton.clicked.connect(self.remove)
+        self.table.clicked.connect(self.table.resizeColumnsToContents)
+        self.table.clicked.connect(self.table.resizeRowsToContents)
+        self.load_table_data()
+        self.table.resizeColumnsToContents()
+        self.table.resizeRowsToContents()
+        self.update_max_hight()
+        self.table_model.itemChanged.connect(self.check_string)
 
-        Returns
-        -------
+    def update_max_hight(self):
+        """ """
+        if self.growsize:
+            self.setMaximumHeight(90 + self.table_model.rowCount()*100)
+            self.sizechange.emit()
+        elif self.fixedsize:
+            self.setMaximumHeight(100)
+            self.setMaximumWidth(200)
+        elif not self.horizontal:
+            self.setMaximumHeight(30 * len(self.headerLabels) + 30)
 
+    def change_table_data(self, tableData):
         """
-        if parent_step_name is None:
-            self.add_loop_step(loop_step, model=model, parent_step_name=parent_step_name, position=position)
-        else:
-            if model is not None:
-                loop_step.append_to_model(model, parent=parent_step_name)
-            if loop_step not in self.loop_step_dict[parent_step_name].children:
-                self.loop_step_dict[parent_step_name].add_child(loop_step, position)
-            self.loop_step_dict.update({loop_step.full_name: loop_step})
-        # if loop_step.has_children:
-        for child in loop_step.children:
-            self.add_loop_step_rec(child, parent_step_name=loop_step.full_name, model=model)
-
-    def remove_loop_step(self, loop_step_name):
-        """Removes the step with the given name from the sequence-list
-        (or parent) and from the dictionary.
 
         Parameters
         ----------
-        loop_step_name :
+        tableData :
             
 
         Returns
         -------
 
         """
-        step = self.loop_step_dict.pop(loop_step_name)
-        if step.parent_step is not None:
-            self.loop_step_dict[step.parent_step].remove_child(step)
+        if isinstance(tableData, dict):
+            tableData = pd.DataFrame(tableData)
+        self.tableData = tableData
+        self.load_table_data()
+
+    def load_table_data(self):
+        """Putting the `tableData` into the table."""
+        if self.horizontal:
+            while self.table_model.rowCount():
+                self.table_model.removeRow(0)
         else:
-            self.loop_steps.remove(step)
-
+            while self.table_model.columnCount():
+                self.table_model.removeColumn(0)
+        data = np.array(self.tableData)
+        for dat in data:
+            self.add(dat)
 
-    def load_loop_steps(self, loop_steps, model=None):
-        """Takes a list of loop_steps, creates them (with the input data
-        of each step) and adds them to the specified model.
+    def context_menu(self, pos):
+        """Generates the right-click-menu.
+        There are entries for inserting (replace) and appending the
+        variables, channels, functions and operators.
 
         Parameters
         ----------
-        loop_steps :
+        pos :
             
-        model :
-             (Default value = None)
 
         Returns
         -------
 
         """
-        for step in loop_steps:
-            loop_step = self.make_step(step)
-            self.add_loop_step_rec(loop_step, model=model)
-
-    def make_step(self, step_info):
-        """Creates the step specified with step_info (including the
-        children), 'step_type' gives which subclass of Loop_Step shall
-        be created.
+        menu = QMenu()
+        # putting the returned actions somewhere is necessary, otherwise
+        # there will be none inside the single menus
+        (channel_menu, variable_menu, function_menu), _ =\
+            variables_handling.get_menus(self.insert_variable)
+        menu.addMenu(variable_menu)
+        menu.addMenu(channel_menu)
+        menu.addMenu(function_menu)
+        # menu.addMenu(operator_menu)
+        menu.addSeparator()
+        (channel_menu2, variable_menu2, operator_menu2, function_menu2), __ =\
+            variables_handling.get_menus(self.append_variable, 'Append')
+        menu.addMenu(variable_menu2)
+        menu.addMenu(channel_menu2)
+        menu.addMenu(function_menu2)
+        menu.addMenu(operator_menu2)
+        menu.exec_(self.mapToGlobal(pos))
 
-        Parameters
-        ----------
-        step_info :
-            
-
-        Returns
-        -------
-
-        """
-        # children = None
-        # if step_info['has_children']:
-        children = []
-        if 'children' in step_info:
-            for child in step_info['children']:
-                child_step = self.make_step(child)
-                child_step.parent_step = step_info['full_name']
-                children.append(child_step)
-        st = make_step_of_type.make_step(step_info['step_type'], step_info, children)
-        st.full_name = step_info['full_name']
-        return st
-
-    def rearrange_loop_steps(self, step_list):
-        """Takes a list of loopsteps, each entry consisting of a tuple
-        of the loopstep name and its children, which is recursively the
-        same kind of list. Re-populates the loop_step_dict and then puts
-        the loop_steps in the correct order.
+    def append_variable(self, val):
+        """Used for the single actions of the context menu.
 
         Parameters
         ----------
-        step_list :
+        val :
             
 
         Returns
         -------
 
         """
-        self.loop_step_dict = {}
-        for step in self.loop_steps:
-            update_all_children(self.loop_step_dict, step)
-        self.loop_steps = []
-        for step, children in step_list:
-            self.loop_step_dict[step].children = []
-            append_all_children(children, self.loop_step_dict[step], self.loop_step_dict)
-            self.loop_steps.append(self.loop_step_dict[step])
-
-    def get_plan_string(self):
-        """Get the string for the protocol-plan, including the loopsteps."""
-        variables_handling.current_protocol = self
-        plan_string = f'\n\n\ndef {self.name.replace(" ","_")}_plan_inner(devs, eva=None, stream_name="primary"):\n'
-        prot_vars = dict(variables_handling.protocol_variables)
-        if 'StartTime' in prot_vars:
-            prot_vars.pop('StartTime')
-            prot_vars.pop('ElapsedTime')
-        if prot_vars:
-            plan_string += '\tglobal '
-            for i, var in enumerate(prot_vars.keys()):
-                if i > 0:
-                    plan_string += ', '
-                plan_string += var
-            plan_string += '\n'
-        for step in self.loop_steps:
-            plan_string += step.get_protocol_string(n_tabs=1)
-        plan_string += f'\n\n\ndef {self.name.replace(" ","_")}_plan(devs, md=None, runEngine=None, stream_name="primary"):\n'
-        plan_string += '\teva = Evaluator(namespace=namespace)\n'
-        plan_string += '\trunEngine.subscribe(eva)\n'
-        plan_string += '\tyield from bps.open_run(md=md)\n'
-        plan_string += f'\tyield from {self.name.replace(" ", "_")}_plan_inner(devs, eva, stream_name)\n'
-        plan_string += '\tyield from helper_functions.get_fit_results(all_fits, namespace, True)\n'
-        plan_string += '\tyield from bps.close_run()\n'
-        return plan_string
-
-    def get_short_string(self):
-        """ """
-        short_string = ''
-        for step in self.loop_steps:
-            short_string += step.get_protocol_short_string()
-        return short_string
-
-    def get_add_main_string(self):
-        """ """
-        add_main_string = 'def steps_add_main(RE, devs):\n'
-        add_main_string += '\treturner = {}\n'
-        for step in self.loop_steps:
-            add_main_string += step.get_add_main_string()
-        add_main_string += '\treturn returner\n\n\n'
-        return add_main_string
-
-    def get_total_steps(self):
-        """ """
-        total = 0
-        for step in self.loop_steps:
-            step.update_time_weight()
-            total += step.time_weight
-        return total
-
-    def get_outer_string(self):
-        """ """
-        outer_string = ''
-        for step in self.loop_steps:
-            outer_string += step.get_outer_string()
-        return outer_string
-
-    def get_used_devices(self):
-        """Get a list of all devices needed by any loopstep."""
-        devices = []
-        for step in self.loop_steps:
-            step.update_used_devices()
-            devices += step.used_devices
-        adds = []
-        for dev in devices:
-            adds += variables_handling.devices[dev].get_necessary_devices()
-        devices += adds
-        devices = list(set(devices))
-        devices = sorted(devices, key=lambda x: x in adds, reverse=True)
-        return devices
-
-def append_all_children(child_list, step, step_dict):
-    """Takes a list of the kind specified in rearrange_loop_steps, does
-    the same as the other function, but recursively for all the
-    (grand-)children.
-
-    Parameters
-    ----------
-    child_list :
-        
-    step :
-        
-    step_dict :
-        
-
-    Returns
-    -------
+        ind = self.table.selectedIndexes()[0]
+        item = self.table_model.itemFromIndex(ind)
+        text = item.text()
+        item.setText(f'{text}{val}')
 
-    """
-    for child, grandchildren in child_list:
-        child_step = step_dict[child]
-        child_step.children = []
-        append_all_children(grandchildren, child_step, step_dict)
-        child_step.parent_step = step.full_name
-        step.children.append(child_step)
-
-def update_all_children(step_dict, step):
-    """Similar to append_all_children, but only updating the step_dict
-    with all the children.
-
-    Parameters
-    ----------
-    step_dict :
-        
-    step :
-        
-
-    Returns
-    -------
-
-    """
-    step_dict.update({step.full_name: step})
-    # if step.has_children:
-    for child in step.children:
-        update_all_children(step_dict, child)
-
-
-class General_Protocol_Settings(Ui_Protocol_Settings, QWidget):
-    """Widget for the configuration of the general protocol settings.
-    Here plots may be defined and variables added to the protocol.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-
-    """
-    name_changed = Signal()
-
-    def __init__(self, parent=None, protocol=Measurement_Protocol()):
-        super(General_Protocol_Settings, self).__init__(parent)
-        self.setupUi(self)
-        self.protocol = protocol
-        self.lineEdit_filename.setText(self.protocol.filename)
-        self.lineEdit_protocol_name.setText(self.protocol.name)
-
-        self.variable_model = QStandardItemModel()
-        self.variable_model.setHorizontalHeaderLabels(['Name', 'Value',
-                                                       'Data-Type'])
-        self.tableView_variables.setModel(self.variable_model)
-        self.load_variables()
-
-        self.pushButton_add_variable.clicked.connect(lambda x: self.add_variable())
-        self.pushButton_remove_variable.clicked.connect(self.remove_variable)
-
-        self.variable_model.itemChanged.connect(self.check_variable)
-
-        self.plot_widge = Plot_Button_Overview(self, self.protocol.plots)
-
-        cols = ['Channel', 'NeXus-path']
-        comboBoxes = {'Channel': list(variables_handling.channels.keys())}
-        self.table_channel_NX_paths = AddRemoveTable(headerLabels=cols,
-                                                     title='Channel-NeXus-Path',
-                                                     comboBoxes=comboBoxes,
-                                                     tableData=self.protocol.channel_metadata)
-
-        cols = ['Configuration', 'NeXus-path']
-        configs = []
-        for dev in variables_handling.devices:
-            device = variables_handling.devices[dev]
-            allconf = []
-            allconf += list(device.get_passive_config().keys())
-            allconf += list(device.get_config().keys())
-            for key in allconf:
-                configs.append(f'{device.name}_{key}')
-        comboBoxes = {'Configuration': configs}
-        self.table_config_NX_paths = AddRemoveTable(headerLabels=cols,
-                                                    title='Config-NeXus-Path',
-                                                    comboBoxes=comboBoxes,
-                                                    tableData=self.protocol.config_metadata)
-
-        cols = ['Name', 'NeXus-path', 'Value']
-        self.table_metadata = AddRemoveTable(headerLabels=cols,
-                                             title='NeXus-Metadata',
-                                             tableData=self.protocol.metadata)
-
-        self.checkBox_NeXus = QCheckBox('Use NeXus-output')
-        self.checkBox_NeXus.clicked.connect(self.enable_nexus)
-        self.checkBox_NeXus.setChecked(self.protocol.use_nexus)
-        self.lineEdit_protocol_name.textChanged.connect(self.name_change)
-        self.name_change()
-
-        self.textEdit_desc = QTextEdit(parent=self)
-        self.textEdit_desc.setPlaceholderText('Enter your description here.')
-        if self.protocol.description:
-            self.textEdit_desc.setText(self.protocol.description)
-        self.checkBox_csv_exp.setChecked(self.protocol.export_csv)
-        self.checkBox_json_exp.setChecked(self.protocol.export_json)
-
-        self.layout().addWidget(self.textEdit_desc, 5, 0, 1, 4)
-        self.layout().addWidget(self.plot_widge, 6, 0, 1, 4)
-        self.layout().addWidget(self.checkBox_NeXus, 7, 0, 1, 4)
-        self.layout().addWidget(self.table_channel_NX_paths, 9, 0, 1, 4)
-        self.layout().addWidget(self.table_config_NX_paths, 10, 0, 1, 4)
-        self.layout().addWidget(self.table_metadata, 11, 0, 1, 4)
-
-        self.checkBox_NeXus.setHidden(True)
-        self.enable_nexus()
-
-
-
-    def enable_nexus(self):
-        """When the checkBox_NeXus is clicked, enables / disables the
-        other widgets for the nexus-definition.
+    def insert_variable(self, val):
+        """Used for the single actions of the context menu.
 
         Parameters
         ----------
+        val :
+            
 
         Returns
         -------
 
         """
-        nx = self.checkBox_NeXus.isChecked()
-        self.table_channel_NX_paths.setHidden(not nx)
-        self.table_metadata.setHidden(not nx)
-        self.table_config_NX_paths.setHidden(not nx)
+        ind = self.table.selectedIndexes()[0]
+        item = self.table_model.itemFromIndex(ind)
+        item.setText(f'{val}')
 
-
-    def get_unique_name(self, name='name'):
-        """Checks whether name already exists in the variables of the
-        protocol and returns a unique name (with added _i).
-
-        Parameters
-        ----------
-        name :
-             (Default value = 'name')
-
-        Returns
-        -------
-
-        """
-        i = 1
-        while name in self.protocol.variables:
-            if '_' not in name:
-                name += f'_{i}'
-            else:
-                name = f'{name.split("_")[0]}_{i}'
-            i += 1
-        return name
-
-    def add_variable(self):
-        """Add a variable to the list, given a unique name, then updates
-        the protocol.
+    def check_string(self, item):
+        """If an element is part of the checkstrings, the item becomes
+        green if valid, red otherwise and white if empty.
 
         Parameters
         ----------
+        item :
+            
 
         Returns
         -------
 
         """
-        self.append_variable(self.get_unique_name('name'))
-        self.update_variables()
+        ind = item.index()
+        pos = ind.column() if self.horizontal else ind.row()
+        if pos not in self.checkstrings or item.text() == '':
+            color = variables_handling.get_color('white')
+        elif variables_handling.check_eval(item.text()):
+            color = variables_handling.get_color('green')
+        else:
+            color = variables_handling.get_color('red')
+        self.table_model.setData(self.table_model.indexFromItem(item), QBrush(color), Qt.BackgroundRole)
 
-    def append_variable(self, name='name', value='value'):
-        """Append the variable with name and value to the item_model,
-        also add an item that shows the datatype of the value.
+    def add(self, vals=None):
+        """Add the `vals` to the table as a new line. Checks are done
+        for each part, whether there should be a comboBox etc.
 
         Parameters
         ----------
-        name :
-             (Default value = 'name')
-        value :
-             (Default value = 'value')
+        vals :
+             (Default value = None)
 
         Returns
         -------
 
         """
-        name_item = QStandardItem(name)
-        value_item = QStandardItem(value)
-        type_item = QStandardItem(variables_handling.check_data_type(value))
-        type_item.setEditable(False)
-        self.variable_model.appendRow([name_item, value_item, type_item])
+        if vals is None:
+            vals = [''] * len(self.headerLabels) if len(self.headerLabels) else ''
+        items = []
+        box_indexes = []
+        boxes = []
+        table_indexes = []
+        tables = []
+        for i, name in enumerate(self.headerLabels):
+            item = QStandardItem()
+            if name in self.comboBoxes:
+                box = QComboBox()
+                for text in self.comboBoxes[name]:
+                    box.addItem(text)
+                self.boxes.append(box)
+                box_indexes.append(i)
+                boxes.append(box)
+                if vals[i] in self.comboBoxes[name]:
+                    box.setCurrentText(vals[i])
+            elif name in self.subtables:
+                if type(vals[i]) is not list:
+                    vals[i] = []
+                checksting = 0 if i in self.checkstrings else None
+                table = AddRemoveTable(horizontal=self.horizontal,
+                                       headerLabels=[], tableData=vals[i],
+                                       growsize=False, checkstrings=checksting,
+                                       fixedsize=True)
+                self.tables.append(table)
+                table_indexes.append(i)
+                tables.append(table)
+                if vals[i] in self.subtables[name]:
+                    table.setCurrentText(vals[i])
+            else:
+                item = QStandardItem(str(vals[i]))
+            item.setEditable(i in self.editables)
+            item.setEnabled(i in self.enableds)
+            item.setCheckable(i in self.checkables)
+            items.append(item)
+        if len(self.headerLabels) == 0:
+            if self.comboBoxes:
+                box = QComboBox()
+                box.addItems(self.comboBoxes)
+                self.boxes.append(box)
+                box_indexes.append(0)
+                boxes.append(box)
+                if vals in self.comboBoxes:
+                    box.setCurrentText(vals)
+            item = QStandardItem(str(vals))
+            items.append(item)
+        if self.horizontal:
+            self.table_model.appendRow(items)
+            for j, i in enumerate(box_indexes):
+                index = self.table_model.index(self.table_model.rowCount()-1, i)
+                self.table.setIndexWidget(index, boxes[j])
+            for j, i in enumerate(table_indexes):
+                index = self.table_model.index(self.table_model.rowCount()-1, i)
+                self.table.setIndexWidget(index, tables[j])
+        else:
+            self.table_model.appendColumn(items)
+            for j, i in enumerate(box_indexes):
+                index = self.table_model.index(i, self.table_model.columnCount()-1)
+                self.table.setIndexWidget(index, boxes[j])
+            for j, i in enumerate(table_indexes):
+                index = self.table_model.index(i, self.table_model.columnCount()-1)
+                self.table.setIndexWidget(index, tables[j])
+        for item in items:
+            self.check_string(item)
+        self.table.resizeColumnsToContents()
+        self.table.resizeRowsToContents()
+        self.update_max_hight()
+        if self.horizontal:
+            self.added.emit(items[0].row())
+        else:
+            self.added.emit(items[0].column())
 
-    def remove_variable(self):
-        """Removes the selected variable."""
+    def remove(self):
+        """ """
         try:
-            index = self.tableView_variables.selectedIndexes()[0]
+            index = self.table.selectedIndexes()[0]
         except IndexError:
             raise Exception('You need to select a row first!')
-        if index.row() >= 0:
-            self.variable_model.removeRow(index.row())
-            self.update_variables()
-
-    def update_step_config(self):
-        """Updates all the protocol settings."""
-        self.protocol.filename = self.lineEdit_filename.text()
-        self.protocol.name = self.lineEdit_protocol_name.text()
-        self.protocol.description = self.textEdit_desc.toPlainText()
-        self.protocol.plots = self.plot_widge.plot_data
-        self.protocol.metadata = self.table_metadata.update_table_data()
-        self.protocol.channel_metadata = self.table_channel_NX_paths.update_table_data()
-        self.protocol.config_metadata = self.table_config_NX_paths.update_table_data()
-        self.protocol.export_csv = self.checkBox_csv_exp.isChecked()
-        self.protocol.export_json = self.checkBox_json_exp.isChecked()
-        self.update_variables()
-        self.protocol.use_nexus = self.checkBox_NeXus.isChecked()
-
-    def load_variables(self):
-        """Called when starting, loads the variables from the protocol
-        into the table.
+        if self.askdelete:
+            entry = self.table_model.itemFromIndex(index).text()
+            remove_dialog = QMessageBox.question(self, 'Remove entry?',
+                                                 f'Are you sure you want to remove the entry {entry}?',
+                                                 QMessageBox.Yes | QMessageBox.No)
+            if remove_dialog != QMessageBox.Yes:
+                return
+        row = index.row()
+        col = index.column()
+        if self.horizontal and row >= 0:
+            self.table_model.removeRow(row)
+            if not self.headerLabels and self.comboBoxes:
+                self.boxes.pop(row)
+            self.removed.emit(row)
+        elif not self.horizontal and col >= 0:
+            self.table_model.removeColumn(col)
+            if not self.headerLabels and self.comboBoxes:
+                self.boxes.pop(col)
+            self.removed.emit(col)
+        self.update_table_data()
+        self.update_max_hight()
+
+    def update_table_data(self):
+        """Reading all the data of the table, putting it as dict into
+        `self.tableData` and returning it.
 
         Parameters
         ----------
 
         Returns
         -------
 
         """
-        for var in sorted(self.protocol.variables):
-            self.append_variable(var, str(self.protocol.variables[var]))
+        self.tableData = {}
+        for i, lab in enumerate(self.headerLabels):
+            vals = []
+            self.tableData.update({lab: vals})
+            if self.horizontal:
+                for j in range(self.table_model.rowCount()):
+                    ind = self.table_model.index(j, i)
+                    if lab in self.comboBoxes:
+                        vals.append(self.table.indexWidget(ind).currentText())
+                    elif lab in self.subtables:
+                        tab = self.table.indexWidget(ind)
+                        tab.update_table_data()
+                        vals.append(tab.tableData)
+                    elif i in self.checkables:
+                        vals.append(self.table_model.item(j, i).checkState() != Qt.CheckState.Unchecked)
+                    else:
+                        try:
+                            vals.append(int(self.table_model.item(j, i).text()))
+                        except:
+                            try:
+                                vals.append(float(self.table_model.item(j, i).text()))
+                            except:
+                                vals.append(self.table_model.item(j, i).text())
+            else:
+                for j in range(self.table_model.columnCount()):
+                    ind = self.table_model.index(i, j)
+                    if lab in self.comboBoxes:
+                        vals.append(self.table.indexWidget(ind).currentText())
+                    elif lab in self.subtables:
+                        tab = self.table.indexWidget(ind)
+                        tab.update_table_data()
+                        vals.append(tab.tableData)
+                    else:
+                        try:
+                            vals.append(float(self.table_model.item(i, j).text()))
+                        except:
+                            vals.append(self.table_model.item(i, j).text())
+        if len(self.headerLabels) == 0:
+            self.tableData = []
+            if self.comboBoxes:
+                for box in self.boxes:
+                    self.tableData.append(box.currentText())
+            elif self.horizontal:
+                for j in range(self.table_model.rowCount()):
+                    try:
+                        self.tableData.append(float(self.table_model.item(j, 0).text()))
+                    except:
+                        self.tableData.append(self.table_model.item(j, 0).text())
+            else:
+                for j in range(self.table_model.columnCount()):
+                    try:
+                        self.tableData.append(float(self.table_model.item(0,j).text()))
+                    except:
+                        self.tableData.append(self.table_model.item(0,j).text())
+        return self.tableData
+
+
+class AddRemoveDialoge(QDialog):
+    """A QDialog providing an AddRemoveTable."""
+
+    def __init__(self, addLabel='+', removeLabel='-', horizontal=True,
+                 editables=None, checkables=(), headerLabels=None, orderBy=None,
+                 parent=None, tableData=None, title='', comboBoxes=None,
+                 subtables=None, checkstrings=None, askdelete=False):
+        super().__init__(parent)
+        self.setWindowFlags(self.windowFlags() | Qt.WindowMaximizeButtonHint)
+        self.buttonBox = QDialogButtonBox(self)
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
+        self.buttonBox.setObjectName("buttonBox")
+
+        self.buttonBox.rejected.connect(self.reject)
+        self.buttonBox.accepted.connect(self.accept)
+
+        self.table = AddRemoveTable(addLabel=addLabel, removeLabel=removeLabel, horizontal=horizontal, editables=editables, checkables=checkables, headerLabels=headerLabels, orderBy=orderBy, parent=self, tableData=tableData, title=title, comboBoxes=comboBoxes, subtables=subtables, growsize=False, checkstrings=checkstrings, askdelete=askdelete)
+
+        layout = QGridLayout()
+        self.setLayout(layout)
+        layout.addWidget(self.table, 0, 0)
+        layout.addWidget(self.buttonBox, 1, 0)
+        self.setWindowTitle(title)
+        self.table.sizechange.connect(self.adjustSize)
+        self.adjustSize()
+        self.setMinimumWidth(len(headerLabels) * 70)
 
-    def check_variable(self):
-        """If name of variable changed: check whether the variable is
-        unique, if not change its name and raise an error.
-        If value changed: re-evaluate the data-type.
-        Update the protocol afterwards.
+    def get_data(self):
+        """ """
+        return self.table.update_table_data()
+
+    def keyPressEvent(self, a0: QKeyEvent) -> None:
+        """Overwrites the keyPressEvent of the QDialog so that it does
+        not close when pressing Enter/Return.
 
         Parameters
         ----------
+        a0: QKeyEvent :
+            
 
         Returns
         -------
 
         """
-        ind = self.tableView_variables.selectedIndexes()
-        if ind:
-            ind = ind[0]
-        else:
+        if a0.key() == Qt.Key_Enter or a0.key() == Qt.Key_Return:
             return
-        item = self.variable_model.itemFromIndex(ind)
-        if ind.column() == 0:
-            variables_handling.check_variable_name(item.text(), parent=self)
-        if ind.column() == 0 and item.text() in self.protocol.variables:
-            new_name = self.get_unique_name(item.text())
-            item.setText(new_name)
-            raise Exception('Variable names must be unique!')
-        if ind.column() == 1:
-            d_type = variables_handling.check_data_type(item.text())
-            self.variable_model.item(ind.row(), 2).setText(d_type)
-        self.update_variables()
-
-    def update_variables(self):
-        """Taking all the variables from the list into the protocol."""
-        self.protocol.variables = {}
-        for i in range(self.variable_model.rowCount()):
-            name = self.variable_model.item(i, 0).text()
-            value = variables_handling.get_data(self.variable_model.item(i, 1).text())
-            self.protocol.variables.update({name: value})
-
-    def name_change(self):
-        """ """
-        name = self.lineEdit_protocol_name.text()
-        self.label_title.setText(f'{name} - General Configuration')
-        self.protocol.name = name
-        self.name_changed.emit()
+        super().keyPressEvent(a0)
```

### Comparing `nomad_camels-0.1.4/nomad_camels/manual_controls/get_manual_controls.py` & `nomad_camels-0.1.5/nomad_camels/manual_controls/get_manual_controls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+"""This package provides access to all classes of Manual_Control that
+can be used by CAMELS, including device specific ones."""
+
+
 from PySide6.QtWidgets import QDialog, QGridLayout, QDialogButtonBox, QComboBox, QLabel
 from PySide6.QtCore import Qt
 
 from nomad_camels.utility import variables_handling
 from nomad_camels.manual_controls.stage_control import stage_control
 
 manual_controls = {'Stage_Control': [stage_control.Stage_Control,
                                      stage_control.Stage_Control_Config]}
 
 
 class New_Manual_Control_Dialog(QDialog):
-    """ """
+    """A dialog that provides the user with a selection of available manual
+    controls."""
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         layout = QGridLayout()
         self.setLayout(layout)
 
         self.setWindowTitle('New Manual Control - NOMAD-CAMELS')
 
@@ -37,44 +42,52 @@
         label = QLabel('What kind of manual control do you want to add?')
         layout.addWidget(label, 0, 0)
         layout.addWidget(self.selection_box, 1, 0)
         layout.addWidget(self.buttonBox, 2, 0)
 
 
     def accept(self):
-        """ """
+        """Writes the control that was selected into `self.selected_control`."""
         name = self.selection_box.currentText()
         if name in self.std_controls:
             self.selected_control = self.std_controls[name]
         else:
             self.selected_control = self.instr_controls[name]
         super().accept()
 
 
 
 def get_instrument_controls():
-    """ """
+    """Goes through all configured instruments and checks them for manual
+    controls. If there are any, they will be added to a dictionary.
+
+    Returns
+    -------
+    controls : dict{'<name>': (Manual_Control, Manual_Control_Config)}
+        Dictionary with the manual controls and there config widgets.
+    """
     controls = {}
     for name, instr in sorted(variables_handling.devices.items(),
                               key=lambda x: x[0].lower()):
         adds = instr.get_controls()
         controls.update(adds)
     return controls
 
 def get_control_by_type_name(name):
     """
+    Returns a tuple/list of the specified control's class / config-class.
 
     Parameters
     ----------
-    name :
-        
+    name : str
+        Name of the manual control (could be CAMELS-main or instrument specific)
 
     Returns
     -------
-
+    tuple(Manual_Control, Manual_Control_Config)
     """
     if name in manual_controls:
         return manual_controls[name]
     instr_controls = get_instrument_controls()
     if name in instr_controls:
         return instr_controls[name]
     raise Exception(f'Manual Control of type {name} is not defined!')
```

### Comparing `nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/stage_control.py` & `nomad_camels-0.1.5/nomad_camels/manual_controls/stage_control/stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/ui_stage_control.py` & `nomad_camels-0.1.5/nomad_camels/manual_controls/stage_control/ui_stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/tests/protocol_test.py` & `nomad_camels-0.1.5/nomad_camels/tests/protocol_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import importlib
 import os.path
 import sys
 import databroker
+import pytest
+
+from PySide6.QtCore import Qt, QItemSelectionModel
+from PySide6.QtWidgets import QMessageBox
+
 from nomad_camels.frontpanels import protocol_config
 from nomad_camels.bluesky_handling import make_catalog
 from nomad_camels.frontpanels import instrument_installer
 from nomad_camels.utility import variables_handling
 from nomad_camels.utility.treeView_functions import getItemIndex
-from PySide6.QtCore import Qt, QItemSelectionModel
 
 
-def test_change_dev_config(qtbot, tmp_path):
-    """
 
-    Parameters
-    ----------
-    qtbot :
-        
-    tmp_path :
-        
+@pytest.fixture(autouse=True)
+def mock_message_box(monkeypatch):
+    """If a messagebox, e.g. asking whether to discard all changes to the
+    protocol, pops up, it is automatically accepted"""
+    def mock_question(*args, **kwargs):
+        return QMessageBox.Yes
+    monkeypatch.setattr(QMessageBox, 'question', mock_question)
 
-    Returns
-    -------
 
-    """
+def test_change_dev_config(qtbot, tmp_path):
+    """Opens the config for "change device config" tries to configure it for the
+    demo instrument and tries to run a protocol with this step."""
     ensure_demo_in_devices()
     from nomad_camels.loop_steps import change_device_config
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'Change Device Config')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
@@ -40,27 +43,16 @@
     prot.name = 'test_change_dev_config_protocol'
     assert 'Change Device Config (Change_Device_Config)' in prot.loop_step_dict
     assert prot.loop_steps[0].device == 'demo_instrument'
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_for_loop(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for a "For Loop" tries to configure it looping over a
+    wait-step and tries to run a protocol with this step."""
     # ensure_demo_in_devices()
     from nomad_camels.loop_steps import for_while_loops
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'For Loop')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
@@ -87,27 +79,16 @@
     assert 'For Loop (For_Loop)' in prot.loop_step_dict
     assert prot.loop_steps[0].has_children
     assert prot.loop_steps[0].children[0].full_name == 'Wait (Wait)'
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_gradient_descent(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "Gradient Descent" tries to configure it for the
+    demo instrument and tries to run a protocol with this step."""
     ensure_demo_in_devices()
     from nomad_camels.loop_steps import gradient_descent
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'Gradient Descent')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
@@ -131,27 +112,16 @@
     prot.loop_steps[0].read_channels.append('demo_instrument_detectorY')
     prot.name = 'test_gradient_descent_protocol'
     assert 'Gradient Descent (Gradient_Descent)' in prot.loop_step_dict
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_if_and_set_variables(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "If" tries to configure to run the correct way if
+    the variables have the correct value, which is done by a "Set Variables" step."""
     from nomad_camels.loop_steps import set_variables
     conf = protocol_config.Protocol_Config()
     prot = conf.protocol
     qtbot.addWidget(conf)
     qtbot.mouseClick(conf.general_settings.pushButton_add_variable,
                      Qt.MouseButton.LeftButton)
     conf.general_settings.variable_model.item(0, 0).setText('condition')
@@ -184,27 +154,16 @@
     run_test_protocol(tmp_path, prot)
 
 def test_nd_sweep():
     """ """
     pass
 
 def test_read_channels(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "Read Channels" tries to configure it for the
+    demo instrument and tries to run a protocol with this step."""
     ensure_demo_in_devices()
     from nomad_camels.loop_steps import read_channels
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'Read Channels')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
@@ -223,27 +182,16 @@
     run_test_protocol(tmp_path, prot)
 
 def test_run_subprotocol():
     """ """
     pass
 
 def test_set_channels(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "Set Channels" tries to configure it for the
+    demo instrument and tries to run a protocol with this step."""
     ensure_demo_in_devices()
     from nomad_camels.loop_steps import set_channels
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'Set Channels')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
@@ -259,42 +207,31 @@
     prot.name = 'test_set_channels_protocol'
     assert 'Set Channels (Set_Channels)' in prot.loop_step_dict
     assert prot.loop_steps[0].channels_values == {'Channels': ['demo_instrument_motorX'], 'Values': ['1']}
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_simple_sweep_with_plot_and_fit(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "Simple Sweep" tries to configure it for the
+    demo instrument. Further it adds a plot and a fit to the sweep and tries to
+    run a protocol with this step."""
     ensure_demo_in_devices()
     from nomad_camels.loop_steps import simple_sweep
     from nomad_camels.frontpanels import plot_definer
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'Simple Sweep')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
     assert isinstance(conf_widge,
                       simple_sweep.Simple_Sweep_Config)
     conf_widge.sweep_widget.lineEdit_start.setText('-10')
     conf_widge.sweep_widget.lineEdit_stop.setText('10')
     conf_widge.sweep_widget.lineEdit_n_points.setText('21')
     conf_widge.comboBox_sweep_channel.setCurrentText('demo_instrument_motorY')
-    conf_widge.checkBox_use_own_plots.setChecked(True)
 
     table = conf_widge.read_table.tableWidget_channels
     row = get_row_from_channel_table('demo_instrument_detectorY', table)
     table.item(row, 0).setCheckState(Qt.CheckState.Checked)
     row = get_row_from_channel_table('demo_instrument_motorY', table)
     table.item(row, 0).setCheckState(Qt.CheckState.Checked)
 
@@ -311,27 +248,17 @@
     prot = conf.protocol
     prot.name = 'test_simple_sweep_protocol'
     assert 'Simple Sweep (Simple_Sweep)' in prot.loop_step_dict
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_trigger_and_read_channels(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "Read Channels" tries to configure it with a split
+    triggering of the channels, then configures the trigger-step and tries to
+    run a protocol with these steps."""
     ensure_demo_in_devices()
     from nomad_camels.loop_steps import read_channels
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     prot = conf.protocol
     variables_handling.current_protocol = prot
     action = get_action_from_name(conf.add_actions, 'Read Channels')
@@ -364,27 +291,17 @@
     assert 'Trigger Channels (Trigger_Channels)' in prot.loop_step_dict
     assert prot.loop_steps[0].read_step == 'Read Channels (Read_Channels)'
 
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_while_loop(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for a "While Loop" and tries to configure it with the
+    condition being `While_Loop_Count < 5`. Into the loop, a wait-step is added.
+    Tries to run a protocol with this step."""
     from nomad_camels.loop_steps import for_while_loops
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'While Loop')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
     assert isinstance(conf_widge,
@@ -408,27 +325,16 @@
     assert 'While Loop (While_Loop)' in prot.loop_step_dict
     assert prot.loop_steps[0].has_children
     assert prot.loop_steps[0].children[0].full_name == 'Wait (Wait)'
     catalog_maker(tmp_path)
     run_test_protocol(tmp_path, prot)
 
 def test_wait(qtbot, tmp_path):
-    """
-
-    Parameters
-    ----------
-    qtbot :
-
-    tmp_path :
-
-
-    Returns
-    -------
-
-    """
+    """Opens the config for "Wait" tries to configure it to a wait time of
+    1.0 second and tries to run a protocol with this step."""
     from nomad_camels.loop_steps import wait_loop_step
     conf = protocol_config.Protocol_Config()
     qtbot.addWidget(conf)
     action = get_action_from_name(conf.add_actions, 'Wait')
     action.trigger()
     conf_widge = conf.loop_step_configuration_widget
     assert isinstance(conf_widge,
```

### Comparing `nomad_camels-0.1.4/nomad_camels/tests/startup_test.py` & `nomad_camels-0.1.5/nomad_camels/tests/startup_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,12 @@
 def test_startup(qtbot, capfd):
     """Simply try to start and run CAMELS.
     By default, the autosave is enabled, so if it works correctly and closes,
-    the statement should be printed
-
-    Parameters
-    ----------
-    qtbot :
-        
-    capfd :
-        
-
-    Returns
-    -------
-
-    """
-    import sys
+    the statement "current state saved!" should be printed"""
+    # import sys
     import nomad_camels.MainApp_v2
     from nomad_camels.utility import exception_hook
     # sys.excepthook = exception_hook.exception_hook
     main_window = nomad_camels.MainApp_v2.MainWindow()
 
     def close_save_message():
         """ """
```

### Comparing `nomad_camels-0.1.4/nomad_camels/tools/EPICS_driver_builder.py` & `nomad_camels-0.1.5/nomad_camels/tools/EPICS_driver_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
             if configs['Datatype'][i] == 'str':
                 class_string += f'\t\tself.config["{name}"] = ""\n'
             elif configs['Datatype'][i] == 'float':
                 class_string += f'\t\tself.config["{name}"] = 0\n'
             elif configs['Datatype'][i] == 'bool':
                 class_string += f'\t\tself.config["{name}"] = False\n'
         class_string += '\n\nclass subclass_config(device_class.Simple_Config):\n'
-        class_string += '\tdef __init__(self, parent=None, data="", settings_dict=None, config_dict=None, ioc_dict=None, additional_info=None):\n'
-        class_string += f'\t\tsuper().__init__(parent, "{dev_name}", data, settings_dict, config_dict, ioc_dict, additional_info)\n'
+        class_string += '\tdef __init__(self, parent=None, data="", settings_dict=None, config_dict=None, additional_info=None):\n'
+        class_string += f'\t\tsuper().__init__(parent, "{dev_name}", data, settings_dict, config_dict, additional_info)\n'
         class_string += '\t\tself.comboBox_connection_type.addItem("EPICS")\n'
         class_string += '\t\tself.load_settings()\n'
 
         ophyd_string = 'from ophyd import Component as Cpt\n\n'
         ophyd_string += 'from ophyd import Device, EpicsSignal, EpicsSignalRO\n\n'
         ophyd_string += f'class {dev_name}_Ophyd(Device):\n'
         for i, name in enumerate(inputs['PV-Name']):
```

### Comparing `nomad_camels-0.1.4/nomad_camels/tools/VISA_builder.py` & `nomad_camels-0.1.5/nomad_camels/tools/VISA_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/tools/VISA_driver_builder.py` & `nomad_camels-0.1.5/nomad_camels/tools/VISA_driver_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
         try:
             self.setWindowIcon(QIcon(resource_filename('nomad_camels', 'graphics/camels_icon.png')))
         except:
             pass
         self.setWindowTitle('NOMAD-CAMELS - VISA-driver-builder')
 
-        label_in = QLabel('Input Channels')
-        label_out = QLabel('Output Channels')
+        label_in = QLabel('Read Channels')
+        label_out = QLabel('Set Channels')
         label_config = QLabel('Config Channels')
-        label_config_in = QLabel('Config Channels - Input Only')
+        label_config_in = QLabel('Config Channels - Read Only')
         label_in.setStyleSheet("font-weight: bold")
         label_out.setStyleSheet("font-weight: bold")
         label_config.setStyleSheet("font-weight: bold")
         label_config_in.setStyleSheet("font-weight: bold")
         label_info = QLabel('The values "Write-Format-String", "Return-Parser" and "Query-String" can be left empty, if you want to use a custom function for those!')
         label_info.setStyleSheet("font-weight: bold")
 
@@ -113,16 +113,16 @@
             if configs['Input-Type'][i] == 'str':
                 class_string += f'\t\tself.config["{name}"] = ""\n'
             elif configs['Input-Type'][i] == 'float':
                 class_string += f'\t\tself.config["{name}"] = 0\n'
             elif configs['Input-Type'][i] == 'bool':
                 class_string += f'\t\tself.config["{name}"] = False\n'
         class_string += '\n\nclass subclass_config(device_class.Simple_Config):\n'
-        class_string += '\tdef __init__(self, parent=None, data="", settings_dict=None, config_dict=None, ioc_dict=None, additional_info=None):\n'
-        class_string += f'\t\tsuper().__init__(parent, "{dev_name}", data, settings_dict, config_dict, ioc_dict, additional_info)\n'
+        class_string += '\tdef __init__(self, parent=None, data="", settings_dict=None, config_dict=None, additional_info=None):\n'
+        class_string += f'\t\tsuper().__init__(parent, "{dev_name}", data, settings_dict, config_dict, additional_info)\n'
         class_string += '\t\tself.comboBox_connection_type.addItem("Local VISA")\n'
         class_string += '\t\tself.load_settings()\n'
 
         ophyd_string = 'from ophyd import Component as Cpt\n\n'
         ophyd_string += 'from nomad_camels.bluesky_handling.visa_signal import VISA_Signal, VISA_Signal_RO, VISA_Device\n\n'
         ophyd_string += f'class {ophyd_name}(VISA_Device):\n'
         open_queries = []
```

### Comparing `nomad_camels-0.1.4/nomad_camels/tools/databroker_exporter.py` & `nomad_camels-0.1.5/nomad_camels/tools/databroker_exporter.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/ui_widgets/channels_check_table.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/channels_check_table.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/ui_widgets/console_redirect.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/console_redirect.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/ui_widgets/drag_drop_tree_view.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/drag_drop_tree_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/ui_widgets/options_run_button.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/options_run_button.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/ui_widgets/path_button_edit.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/path_button_edit.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/ui_widgets/variable_tool_tip_box.py` & `nomad_camels-0.1.5/nomad_camels/ui_widgets/variable_tool_tip_box.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/databroker_export.py` & `nomad_camels-0.1.5/nomad_camels/utility/databroker_export.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/exception_hook.py` & `nomad_camels-0.1.5/nomad_camels/utility/exception_hook.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-import os.path
 from traceback import print_tb
 from PySide6.QtWidgets import QMessageBox
 from PySide6.QtCore import QUrl
 
 from PySide6.QtMultimedia import QSoundEffect
 
 import logging
 
-from nomad_camels.utility.load_save_functions import appdata_path
-
 from bluesky.utils import RunEngineInterrupted
 
 from nomad_camels.utility import variables_handling
 from pkg_resources import resource_filename
 
-if not os.path.isfile(f'{appdata_path}/logging.log'):
-    with open(f'{appdata_path}/logging.log', 'w', encoding='utf-8'):
-        pass
-logging.basicConfig(filename=f'{appdata_path}/logging.log', level=logging.DEBUG)
+# imported, so that it is run once, before the logging in
+# `exception_hook` is connected
+from nomad_camels.utility import logging_settings
+
+
 
 
 class ErrorMessage(QMessageBox):
-    """A popUp-box describing the Error."""
+    """A popUp-box describing an Error.
+
+    Parameters
+    ----------
+    msg : str
+        the error message
+    info_text : str
+        A longer text, explaining the error (usually traceback)
+    parent : QWidget
+        The parent widget of this Messagebox
+    """
     def __init__(self, msg, info_text='', parent=None):
         super().__init__(parent)
         self.setWindowTitle('ERROR')
         self.setIcon(QMessageBox.Warning)
         self.setStandardButtons(QMessageBox.Ok)
         self.setText(msg)
         print(msg)
         print(info_text)
         if info_text:
             self.setInformativeText(info_text)
 
 
 def exception_hook(*exc_info):
-    """Use to overwrite sys.excepthook, so that an exception does not
-        terminate the program, but simply shows a Message with the exception.
+    """Used to overwrite sys.excepthook, so that an exception does not
+    terminate the program, but simply shows a Message with the exception.
+    If the Exception is a KeyboardInterrupt, it does nothing, so that the
+    interrupt may actually stop the program execution.
 
     Parameters
     ----------
-    *exc_info :
-        
-
-    Returns
-    -------
-
+    *exc_info : tuple(class, Exception, traceback)
+        The information for the exception.
     """
     if issubclass(exc_info[0], KeyboardInterrupt):
         return
     elif issubclass(exc_info[0], RunEngineInterrupted):
         return
-    logging.exception(str(exc_info))
+    logging.exception(f'{exc_info[1]} - {print_tb(exc_info[2])}')
     if variables_handling.preferences['play_camel_on_error']:
         effect = QSoundEffect()
         effect.setSource(QUrl.fromLocalFile(resource_filename('nomad_camels','graphics/Camel-Groan-2-QuickSounds.com.wav')))
         effect.play()
     ErrorMessage(exc_info[0].__name__, str(exc_info[1]) + '\n' + str(print_tb(exc_info[2]))).exec()
```

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/number_formatting.py` & `nomad_camels-0.1.5/nomad_camels/utility/number_formatting.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 preferences = {}
 
 def format_number(value):
     """Format a number-string the way it is specified in the preferences.
 
     Parameters
     ----------
-    value :
-        
+    value : float, int
+        The number that should be displayed as string.
 
     Returns
     -------
-
+    str
+        The formatted string of the number.
     """
     if isinstance(value, int):
         return str(value)
     if 'number_format' not in preferences or 'n_decimals' not in preferences:
         return str(f'{value:.2f}')
     if preferences['number_format'] == 'plain':
         return f'{value:.{preferences["n_decimals"]}f}'
```

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/qthreads.py` & `nomad_camels-0.1.5/nomad_camels/utility/qthreads.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+CURRENTLY DEPRECATED MODULE, NOTHING IS USED
+This module contains various threads that may be run from the main UI."""
+
 import signal
 import os
 import time
 
 import numpy as np
 
 from PySide6.QtCore import QThread, Signal
@@ -9,15 +13,17 @@
 import subprocess
 
 from nomad_camels.utility import variables_handling
 
 
 
 class Run_Protocol(QThread):
-    """Runs the given protocol with a file at the given path."""
+    """
+    DEPRECATED
+    Runs the given protocol with a file at the given path."""
     sig_step = Signal(int)
     info_step = Signal(str)
     protocol_done = Signal()
 
     def __init__(self):
         super().__init__()
         self.protocol = None
@@ -139,15 +145,17 @@
             raise Exception('Exiting the shell is not allowed!')
         if self.popen is not None:
             self.popen.stdin.write(bytes(f'{msg}\n', 'utf-8'))
             self.popen.stdin.flush()
             self.info_step.emit(f'{msg}\n')
 
 class Run_Protocol_test(QThread):
-    """Runs the given protocol with a file at the given path."""
+    """
+    DEPRECATED
+    Runs the given protocol with a file at the given path."""
     sig_step = Signal(int)
     info_step = Signal(str)
     protocol_done = Signal()
 
     def __init__(self, RE, main_fun):
         super().__init__()
         self.protocol = None
@@ -278,15 +286,15 @@
 
 
 
 
 
 
 class Manual_Device_Thread(QThread):
-    """ """
+    """DEPRECATED"""
     def __init__(self, device, ophyd_class):
         super().__init__()
         self.device = ophyd_class(f'{device.custom_name}:',
                                   name=f'manual_{device.custom_name}',
                                   **device.get_settings())
         self.device.wait_for_connection()
         self.device.configure(device.get_config())
```

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/theme_changing.py` & `nomad_camels-0.1.5/nomad_camels/utility/theme_changing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""This module is used to change the UI-theme of CAMELS. It provides some
+default color palettes `light_palette` and `dark_palette`."""
+
 from PySide6.QtWidgets import QApplication, QMainWindow, QStyleFactory
 from PySide6.QtGui import QPalette, QColor, QColorConstants
 from qt_material import apply_stylesheet
 
 
 light_palette = QPalette(QColor(225, 225, 225), QColor(238, 238, 238))
 light_palette.setColor(QPalette.Highlight, QColor(42, 130, 218))
@@ -22,39 +25,41 @@
 dark_palette.setColor(QPalette.HighlightedText, QColorConstants.Black)
 
 def change_theme(theme, main_app=None, material_theme=None, dark_mode=False):
     """
 
     Parameters
     ----------
-    theme :
-        
-    main_app :
-         (Default value = None)
-    material_theme :
-         (Default value = None)
-    dark_mode :
-         (Default value = False)
-
-    Returns
-    -------
-
+    theme : str
+        The name of the used theme. Possible values are the themes from
+        QStyleFactory and "qt-material".
+    main_app : QMainWindow
+        (Default value = None)
+        The main UI-window. If it is None, it is looked for with
+        `QApplication.instance()`.
+    material_theme : str
+        (Default value = None)
+        If `theme=="qt-material"`, the qt-material color palette is chosen with
+        this theme name.
+    dark_mode : bool
+        (Default value = False)
+        If True, the color palettes are switched to dark mode.
     """
     if main_app is None:
         main_app = QApplication.instance()
         if main_app is None:
             raise RuntimeError("MainApp not found.")
     if theme in QStyleFactory.keys():
         main_app.setStyleSheet('')
         palette = None
         if dark_mode:
             palette = dark_palette
         else:
             palette = light_palette
-        if theme == 'windowsvista':# in QStyleFactory.keys():
+        if theme == 'windowsvista':
             main_app.setStyle(QStyleFactory.create('windowsvista'))
         main_app.setPalette(palette)
         main_app.setStyle(QStyleFactory.create(theme))
         if palette:
             main_app.setPalette(palette)
     elif theme == 'qt-material':
         if not isinstance(material_theme, str):
```

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/treeView_functions.py` & `nomad_camels-0.1.5/nomad_camels/utility/treeView_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/nomad_camels/utility/variables_handling.py` & `nomad_camels-0.1.5/nomad_camels/utility/variables_handling.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,57 @@
+"""This module helps to synchronize information between different modules. To
+this aim, it holds several variables that may be read from different places.
+Furthermore, some functions to work with those variables are provided.
+
+Attributes
+----------
+    preset : str
+        The name of the currently used preset of CAMELS.
+    device_driver_path : str, path
+        The path, where to find local drivers.
+    meas_files_path : str, path
+        The path, where to write the measurement files, i.e. data.
+    CAMELS_path : str, path
+        The path to the current installation of CAMELS.
+    preferences : dict
+        The currently used preferences.
+    protocols : dict{"<protocol_name>": protocol}
+        The available protocols.
+    protocol_variables : dict{"<name>": <value>}
+        The variables provided by the currently viewed protocol.
+    channels : dict{"<name>": channel}
+        All available channels provided by the configured instruments.
+    loop_step_variables : dict{"<name>": <value>}
+        The variables provided by the steps of the currently viewed protocol.
+    devices : dict
+        All configured instruments/devices.
+    current_protocol = Measurement_Protocol
+        The protocol, that is currently being used.
+    dark_mode : bool
+        Whether dark-mode is currently active.
+    copied_step : Loop_Step
+        The last step, that was copied.
+    read_channel_sets : list[set]
+        Sets of the different channel-compositions for read-channels. Used to distinguish different reads with different channels for bluesky
+    read_channel_names : list[str]
+        Names of the different read-channel steps in use. Used to distinguish the different reads.
+    evaluation_functions_names : dict
+        Used to provide the right-click menu to use mathematical functions.
+    operator_names : dict
+        Used to provide the right-click menu to use mathematical operators.
+"""
+
 from ast import literal_eval, parse
 from PySide6.QtWidgets import QMenu
 from PySide6.QtGui import QColor, QAction
 
 import numpy as np
-# from nomad_camels.utility import simpleeval
 from nomad_camels.bluesky_handling import evaluation_helper
 from nomad_camels.ui_widgets.warn_popup import WarnPopup
 
-# from bluesky_widgets.models import utils
 
 preset = ''
 device_driver_path = ''
 meas_files_path = ''
 CAMELS_path = ''
 
 preferences = {}
@@ -25,42 +65,14 @@
 dark_mode = False
 
 copied_step = None
 
 read_channel_sets = []
 read_channel_names = []
 
-
-def get_output_channels():
-    """ """
-    outputs = []
-    for channel in channels:
-        if channels[channel].output:
-            outputs.append(channel)
-    return outputs
-
-# evaluation_functions = simpleeval.DEFAULT_FUNCTIONS.copy()
-# evaluation_functions.update({'exp': np.exp,
-#                              'log': np.log,
-#                              'sqrt': np.sqrt,
-#                              'round': round,
-#                              'sin': np.sin,
-#                              'cos': np.cos,
-#                              'sinh': np.sinh,
-#                              'cosh': np.cosh,
-#                              'sinc': np.sinc,
-#                              'tan': np.tan,
-#                              'arctan': np.arctan,
-#                              'arcsin': np.arcsin,
-#                              'arccos': np.arccos,
-#                              'arcsinh': np.arcsinh,
-#                              'arccosh': np.arccosh,
-#                              'arctanh': np.arctanh})
-
-
 evaluation_functions_names = {
     'randint()': 'randint(x) - random integer below x',
     'rand()': 'rand() - random float between 0 and 1',
     'round()': 'round(x) - round number to nearest integer',
     'exp()': 'exp(x) - exponential function of x',
     'sqrt()': 'sqrt(x) - square root of x',
     'log()': 'ln(x) - natural logarithm of x',
@@ -92,28 +104,39 @@
     '<=': 'less or equal',
     '>=': 'greater or equal',
     'and': 'logical AND',
     'or': 'logical OR',
     'not': 'logical negation'
 }
 
+
+def get_output_channels():
+    """Goes through all channels and returns a list of the names of those, that
+    are outputs."""
+    outputs = []
+    for channel in channels:
+        if channels[channel].output:
+            outputs.append(channel)
+    return outputs
+
 def get_color(color='', string=False):
     """Returns the respective QColor or rgb-code(if `string`) for
     `color`, taking dark-mode into account.
 
     Parameters
     ----------
-    color :
-         (Default value = '')
-    string :
-         (Default value = False)
-
-    Returns
-    -------
-
+    color : str
+        (Default value = '')
+        The name of the color asked for. Possible values are "red" / "r",
+        "strong_red", "green" / "g", "dark_green", "grey" / "gray", "blue" / "b"
+        "black" (white if `dark_mode`), "orange". Otherwise white (or black, if
+        `dark_mode`) is returned.
+    string : bool
+        (Default value = False)
+        If True, only the string of the rgb will be returned, not the QColor.
     """
     if color == 'red' or color == 'r':
         rgb = (255, 180, 180)
         if dark_mode:
             rgb = (75, 0, 0)
     elif color == 'strong_red':
         rgb = (230, 0, 0)
@@ -145,110 +168,93 @@
 
 def get_menus(connect_function, pretext='Insert'):
     """Providing QMenus with the `connect_function` for each action,
     containing all the variables, channels, functions and operators.
 
     Parameters
     ----------
-    connect_function :
-        
-    pretext :
-         (Default value = 'Insert')
+    connect_function : callable
+        The function that should be executed when the action is clicked. It gets
+        the variable's name as a value.
+    pretext : str
+        (Default value = 'Insert')
+        This string will be written in front of the menus.
 
     Returns
     -------
-
+    menus : list[QMenu]
+        the created menus
+    actions : list[list[QAction]]
+        lists of the individual actions in the menus
     """
     variable_menu = QMenu(f'{pretext} Variable')
     channel_menu = QMenu(f'{pretext} Channel-Value')
     function_menu = QMenu(f'{pretext} Function')
     operator_menu = QMenu(f'{pretext} Operator')
     channel_actions = []
     operator_actions = []
     actions = []
     function_actions = []
     add_actions_from_dict(channels, channel_actions, connect_function)
-    # for channel in sorted(channels, key=lambda x: x.lower()):
-    #     action = QAction(channel)
-    #     action.triggered.connect(lambda state=None, x=channel: connect_function(x))
-    #     channel_actions.append(action)
     add_actions_from_dict(protocol_variables, actions, connect_function)
-    # for variable in sorted(protocol_variables, key=lambda x: x.lower()):
-    #     action = QAction(variable)
-    #     action.triggered.connect(lambda state=None, x=variable: connect_function(x))
-    #     actions.append(action)
     add_actions_from_dict(loop_step_variables, actions, connect_function)
     add_actions_from_dict({'StartTime': 1, 'ElapsedTime': 1}, actions,
                           connect_function)
-    # for variable in sorted(loop_step_variables, key=lambda x: x.lower()):
-    #     action = QAction(variable)
-    #     action.triggered.connect(lambda state=None, x=variable: connect_function(x))
-    #     actions.append(action)
     add_actions_from_dict(operator_names, operator_actions, connect_function)
-    # for op in operator_names:
-    #     action = QAction(f'{op}\t{operator_names[op]}')
-    #     action.triggered.connect(lambda state=None, x=op: connect_function(x))
-    #     operator_actions.append(action)
     add_actions_from_dict(evaluation_functions_names, function_actions,
                           connect_function)
-    # for foo in sorted(evaluation_functions_names, key=lambda x: x.lower()):
-    #     action = QAction(evaluation_functions_names[foo])
-    #     action.triggered.connect(lambda state=None, x=foo: connect_function(x))
-    #     function_actions.append(action)
     channel_menu.addActions(channel_actions)
     variable_menu.addActions(actions)
     operator_menu.addActions(operator_actions)
     function_menu.addActions(function_actions)
     if pretext == 'Insert':
         menus = [channel_menu, variable_menu, function_menu]
         actions = [channel_actions, actions, function_actions]
     else:
         menus = [channel_menu, variable_menu, operator_menu, function_menu]
         actions = [channel_actions, actions, operator_actions, function_actions]
     return menus, actions
 
 def add_actions_from_dict(dictionary, actions, connect_function, add_string=''):
     """
+    The values of `dictionary` are handed to the `connect_function` when
+    clicking on the respective action named with the keys of the dictionary. The
+    created actions are added to `actions`.
 
     Parameters
     ----------
-    dictionary :
-        
-    actions :
-        
-    connect_function :
-        
-    add_string :
-         (Default value = '')
-
-    Returns
-    -------
-
+    dictionary : dict
+        the keys become the names of the actions, the values are handed to the
+        `connect_function`
+    actions : list
+        the created actions will be added to this list
+    connect_function : callable
+        this function is called, when one of the actions is clicked
+    add_string : str
+        (Default value = '')
+        added in front of the values of the dictionary for the connect_function
     """
     for var in sorted(dictionary, key=lambda x: x.lower()):
         if isinstance(dictionary[var], dict):
             add_actions_from_dict(dictionary[var], actions, connect_function,
                                   f'{var}:')
         else:
             addvar = f'{add_string}{var}'
             action = QAction(addvar)
             action.triggered.connect(lambda state=None, x=addvar: connect_function(x))
             actions.append(action)
 
 def check_eval(s):
-    """Checks, whether the string `s` can be evaluated.
+    """Checks, whether the string `s` can be evaluated. Returns True if it is
+    possible, otherwise False.
 
     Parameters
     ----------
-    s :
-        
-
-    Returns
-    -------
-
+    s : str
+        the string that should be checked
     """
     try:
         namespace = dict(evaluation_helper.base_namespace)
         namespace.update(protocol_variables)
         namespace.update(loop_step_variables)
         for channel in channels:
             namespace.update({channel: 1})
@@ -256,46 +262,42 @@
         evaluation_helper.get_eval(s, namespace)
         return True
     except Exception:
         return False
 
 def get_eval(s):
     """
+    Evaluates the string `s` with the namespace of `protocol_variables` and
+    `loop_step_variables` in addition to `evaluation_helper.base_namespace`.
+    Returns the evaluated value.
 
     Parameters
     ----------
-    s :
-        
-
-    Returns
-    -------
-
+    s : str
+        the string that should be evaluated
     """
     try:
         namespace = dict(evaluation_helper.base_namespace)
         namespace.update(protocol_variables)
         namespace.update(loop_step_variables)
         for channel in channels:
             namespace.update({channel: 1})
         return evaluation_helper.get_eval(s, namespace)
     except:
         return np.nan
 
 
 def get_data(s):
-    """Returns the evaluated data of s.
+    """Used instead of `get_eval` when there is no specific namespace. It simply
+    uses `ast.literal_eval` and if it does not work, the string `s` is returned.
 
     Parameters
     ----------
-    s :
-        
-
-    Returns
-    -------
-
+    s : str
+        the string to be evaluated
     """
     if not s:
         return ''
     try:
         lit = literal_eval(s)
     except ValueError:
         return s
@@ -304,52 +306,57 @@
     return lit
 
 def check_data_type(s):
     """Returns the datatype of the string-evaluation of s.
 
     Parameters
     ----------
-    s :
-        
-
-    Returns
-    -------
-
+    s : str
+        the string that should be checked
     """
     if not isinstance(s, str):
         return str(type(s))
     if not s:
         return ''
     try:
         lit = literal_eval(s)
     except ValueError:
         return 'String'
     except SyntaxError:
         return 'String'
     return str(type(lit))
 
 def get_write_from_data_type(s):
-    """
-
-    Parameters
-    ----------
-    s :
-        
-
-    Returns
-    -------
-
-    """
+    """Used for writing longer strings. Since the strings should stay strings in
+    the written files, if the evaluated datatype of `s` is str, quatation marks
+    will be added around the value, otherwise nothing is done."""
     t = check_data_type(s)
     if t == 'String':
         return f'"{s}"'
     return s
 
 
 def check_variable_name(name, raise_not_warn=False, parent=None):
+    """Checks whether `name` is a valid name for a variable. It checks, whether
+    the name mirrors a builtin function or keyword. If not, it is tried with ast
+    to parse the statement `<name> = None`, i.e. whether it works as a variable
+    name. If anything fails, either an exception is raised (if `raise_not_warn`)
+    or a `WarnPopup` is called.
+
+    Parameters
+    ----------
+    name : str
+        the name that should be checked
+    raise_not_warn : bool
+        (Default value = False)
+        if True, an exception is raised if a check fails, otherwise a WarnPopup
+    parent : QWidget
+        (Default value = None)
+        the parent widget for a possibly called WarnPopup
+    """
     try:
         built_check = name in vars(__builtins__)
     except:
         built_check = name in __builtins__
     if built_check:
         text = f'The name "{name}" is a python builtin function! Please use another name.'
         if raise_not_warn:
@@ -361,9 +368,7 @@
     except (ValueError, SyntaxError, TypeError):
         text = f'The name "{name}" is not a valid name! Remove e.g. spaces or special characters.'
         if raise_not_warn:
             raise Exception(text)
         WarnPopup(parent, text, 'Invalid Name')
         return False
     return True
-
-
```

### Comparing `nomad_camels-0.1.4/nomad_camels.egg-info/PKG-INFO` & `nomad_camels-0.1.5/nomad_camels.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad-camels
-Version: 0.1.4
+Version: 0.1.5
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
@@ -27,16 +27,20 @@
 
 ## Documentation
 
 For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 # Changelog
 
+## 0.1.5
+Fixed the 'Update CAMELS' tool.\
+Renamed input and output to read and set in the 'Update CAMELS' tool.\
+Small fix to the VISA device builder.
 
 ## 0.1.4
-Added a timeout setting to all VISA instruments. 
+Added a timeout setting to all VISA instruments. Setting the timeout determines how long the instrument waits after sending a command before raising a timeout exception
 
 ## 0.1.3
 First stable and working release
 
 ## 0.1.0 to 0.1.2 
 &#9888; Broken releases due to minor bugs that were fixed in 0.1.3
```

### Comparing `nomad_camels-0.1.4/nomad_camels.egg-info/SOURCES.txt` & `nomad_camels-0.1.5/nomad_camels.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 nomad_camels/utility/__init__.py
 nomad_camels/utility/databroker_export.py
 nomad_camels/utility/device_handling.py
 nomad_camels/utility/exception_hook.py
 nomad_camels/utility/fit_variable_renaming.py
 nomad_camels/utility/load_save_functions.py
 nomad_camels/utility/load_save_helper_functions.py
+nomad_camels/utility/logging_settings.py
 nomad_camels/utility/number_formatting.py
 nomad_camels/utility/plot_placement.py
 nomad_camels/utility/qthreads.py
 nomad_camels/utility/theme_changing.py
 nomad_camels/utility/tqdm_progress_bar.py
 nomad_camels/utility/treeView_functions.py
 nomad_camels/utility/update_camels.py
```

### Comparing `nomad_camels-0.1.4/nomad_camels.egg-info/requires.txt` & `nomad_camels-0.1.5/nomad_camels.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.4/pyproject.toml` & `nomad_camels-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
```

### Comparing `nomad_camels-0.1.4/requirements.txt` & `nomad_camels-0.1.5/requirements.txt`

 * *Files identical despite different names*

