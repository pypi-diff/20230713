# Comparing `tmp/zaber_motion-4.2.2.tar.gz` & `tmp/zaber_motion-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-4.2.2.tar", last modified: Fri Jul  7 21:09:10 2023, max compression
+gzip compressed data, was "zaber_motion-4.2.3.tar", last modified: Thu Jul 13 19:49:58 2023, max compression
```

## Comparing `zaber_motion-4.2.2.tar` & `zaber_motion-4.2.3.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.530451 zaber_motion-4.2.2/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-07 21:09:10.530519 zaber_motion-4.2.2/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-07-07 21:09:10.530771 zaber_motion-4.2.2/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.508238 zaber_motion-4.2.2/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.510114 zaber_motion-4.2.2/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.517373 zaber_motion-4.2.2/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/io_port_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      268 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope_data_source.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)    26067 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/process.py
--rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/process_controller.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/process_controller_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/process_controller_source.py
--rw-r--r--   0 zaber      (501) staff       (20)      281 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/process_controller_source_sensor.py
--rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/pvt_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      256 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/pvt_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/pvt_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      247 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/pvt_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/pvt_sequence.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.518957 zaber_motion-4.2.2/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1535 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.528429 zaber_motion-4.2.2/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_pvt_point.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      326 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      285 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.529610 zaber_motion-4.2.2/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.529839 zaber_motion-4.2.2/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.530227 zaber_motion-4.2.2/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    67598 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   206262 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     9021 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-07-07 21:08:21.000000 zaber_motion-4.2.2/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-07 21:09:10.510685 zaber_motion-4.2.2/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-07 21:09:10.000000 zaber_motion-4.2.2/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-07-07 21:09:10.000000 zaber_motion-4.2.2/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-07-07 21:09:10.000000 zaber_motion-4.2.2/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-07-07 21:09:10.000000 zaber_motion-4.2.2/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-07 21:09:10.000000 zaber_motion-4.2.2/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.776574 zaber_motion-4.2.3/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-13 19:49:58.776638 zaber_motion-4.2.3/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-07-13 19:49:58.776887 zaber_motion-4.2.3/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.754929 zaber_motion-4.2.3/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.756739 zaber_motion-4.2.3/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.763767 zaber_motion-4.2.3/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/io_port_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      268 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_data_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26067 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)      281 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller_source_sensor.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    23693 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.765272 zaber_motion-4.2.3/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1940 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1535 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.774569 zaber_motion-4.2.3/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      396 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.775728 zaber_motion-4.2.3/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.775969 zaber_motion-4.2.3/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.776346 zaber_motion-4.2.3/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    67598 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   206262 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     9340 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.757292 zaber_motion-4.2.3/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-4.2.2/LICENSE.txt` & `zaber_motion-4.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/PKG-INFO` & `zaber_motion-4.2.3/zaber_motion.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zaber_motion
-Version: 4.2.2
+Name: zaber-motion
+Version: 4.2.3
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.2/setup.py` & `zaber_motion-4.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='4.2.2',
+    version='4.2.3',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.8',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==4.2.2;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==4.2.2;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==4.2.2;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==4.2.3;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==4.2.3;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==4.2.3;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-4.2.2/test/test_integration.py` & `zaber_motion-4.2.3/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/__init__.py` & `zaber_motion-4.2.3/zaber_motion/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/__init__.py` & `zaber_motion-4.2.3/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/alert_event.py` & `zaber_motion-4.2.3/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/all_axes.py` & `zaber_motion-4.2.3/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/axis.py` & `zaber_motion-4.2.3/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/axis_identity.py` & `zaber_motion-4.2.3/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/axis_settings.py` & `zaber_motion-4.2.3/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/connection.py` & `zaber_motion-4.2.3/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-4.2.3/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/device.py` & `zaber_motion-4.2.3/zaber_motion/ascii/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/device_identity.py` & `zaber_motion-4.2.3/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/device_io.py` & `zaber_motion-4.2.3/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/device_io_info.py` & `zaber_motion-4.2.3/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/device_settings.py` & `zaber_motion-4.2.3/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/lockstep.py` & `zaber_motion-4.2.3/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-4.2.3/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/paramset_info.py` & `zaber_motion-4.2.3/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-4.2.3/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/process.py` & `zaber_motion-4.2.3/zaber_motion/ascii/process.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/process_controller.py` & `zaber_motion-4.2.3/zaber_motion/ascii/process_controller.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/process_controller_source.py` & `zaber_motion-4.2.3/zaber_motion/ascii/process_controller_source.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-4.2.3/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-4.2.3/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-4.2.3/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/response.py` & `zaber_motion-4.2.3/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-4.2.3/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-4.2.3/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/setting_constants.py` & `zaber_motion-4.2.3/zaber_motion/ascii/setting_constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,49 @@
 
     """
     Accel.
     """
     ACCEL = "accel"
 
     """
+    Brake Closing Duration.
+    """
+    BRAKE_CLOSING_DURATION = "brake.closing.duration"
+
+    """
+    Brake Mode.
+    """
+    BRAKE_MODE = "brake.mode"
+
+    """
+    Brake Opening Duration.
+    """
+    BRAKE_OPENING_DURATION = "brake.opening.duration"
+
+    """
+    Brake State.
+    """
+    BRAKE_STATE = "brake.state"
+
+    """
+    Brake Voltage Excitation.
+    """
+    BRAKE_VOLTAGE_EXCITATION = "brake.voltage.excitation"
+
+    """
+    Brake Voltage Hold.
+    """
+    BRAKE_VOLTAGE_HOLD = "brake.voltage.hold"
+
+    """
+    Brake Voltage Hold Delay.
+    """
+    BRAKE_VOLTAGE_HOLD_DELAY = "brake.voltage.hold.delay"
+
+    """
     Calibration Type.
     """
     CALIBRATION_TYPE = "calibration.type"
 
     """
     Cloop Continuous Enable.
     """
@@ -46,14 +81,19 @@
 
     """
     Cloop Recovery Enable.
     """
     CLOOP_RECOVERY_ENABLE = "cloop.recovery.enable"
 
     """
+    Cloop Servo Effort.
+    """
+    CLOOP_SERVO_EFFORT = "cloop.servo.effort"
+
+    """
     Cloop Servo Enable.
     """
     CLOOP_SERVO_ENABLE = "cloop.servo.enable"
 
     """
     Cloop Settle Period.
     """
@@ -256,24 +296,34 @@
 
     """
     Driver Dir.
     """
     DRIVER_DIR = "driver.dir"
 
     """
+    Driver Enable Mode.
+    """
+    DRIVER_ENABLE_MODE = "driver.enable.mode"
+
+    """
     Driver Enabled.
     """
     DRIVER_ENABLED = "driver.enabled"
 
     """
     Driver I 2 T Measured.
     """
     DRIVER_I_2_T_MEASURED = "driver.i2t.measured"
 
     """
+    Driver Overdrive State.
+    """
+    DRIVER_OVERDRIVE_STATE = "driver.overdrive.state"
+
+    """
     Driver Temperature.
     """
     DRIVER_TEMPERATURE = "driver.temperature"
 
     """
     Encoder 1 Count.
     """
@@ -1176,14 +1226,19 @@
 
     """
     Pos.
     """
     POS = "pos"
 
     """
+    Pvt Numseqs.
+    """
+    PVT_NUMSEQS = "pvt.numseqs"
+
+    """
     Resolution.
     """
     RESOLUTION = "resolution"
 
     """
     Scope Channel Size.
     """
@@ -1251,14 +1306,19 @@
 
     """
     System Temperature.
     """
     SYSTEM_TEMPERATURE = "system.temperature"
 
     """
+    System Uptime.
+    """
+    SYSTEM_UPTIME = "system.uptime"
+
+    """
     System Voltage.
     """
     SYSTEM_VOLTAGE = "system.voltage"
 
     """
     Trigger Numactions.
     """
```

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-4.2.3/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/storage.py` & `zaber_motion-4.2.3/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/stream.py` & `zaber_motion-4.2.3/zaber_motion/ascii/stream.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-4.2.3/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-4.2.3/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/transport.py` & `zaber_motion-4.2.3/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-4.2.3/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/warning_flags.py` & `zaber_motion-4.2.3/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/ascii/warnings.py` & `zaber_motion-4.2.3/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/__init__.py` & `zaber_motion-4.2.3/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/binary_settings.py` & `zaber_motion-4.2.3/zaber_motion/binary/binary_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ANALOG_OUTPUT_COUNT = 5
     AUTO_HOME_DISABLED_MODE = 6
     AUTO_REPLY_DISABLED_MODE = 7
     AXIS_DEVICE_NUMBER = 8
     AXIS_INVERSION = 9
     AXIS_VELOCITY_PROFILE = 10
     AXIS_VELOCITY_SCALE = 11
-    BAUD_RATE = 12
+    BAUDRATE = 12
     CALIBRATED_ENCODER_COUNT = 13
     CALIBRATION_ERROR = 14
     CALIBRATION_TYPE = 15
     CLOSED_LOOP_MODE = 16
     CURRENT_POSITION = 17
     CYCLE_DISTANCE = 18
     DECELERATION_ONLY = 19
```

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/command_code.py` & `zaber_motion-4.2.3/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/connection.py` & `zaber_motion-4.2.3/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/device.py` & `zaber_motion-4.2.3/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/device_identity.py` & `zaber_motion-4.2.3/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/device_settings.py` & `zaber_motion-4.2.3/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/error_code.py` & `zaber_motion-4.2.3/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/message.py` & `zaber_motion-4.2.3/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/reply_only_event.py` & `zaber_motion-4.2.3/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-4.2.3/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/bindings.py` & `zaber_motion-4.2.3/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/call.py` & `zaber_motion-4.2.3/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/convert_exception.py` & `zaber_motion-4.2.3/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/events.py` & `zaber_motion-4.2.3/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/__init__.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/firmware_version.py` & `zaber_motion-4.2.3/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/__init__.py` & `zaber_motion-4.2.3/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/axis_definition.py` & `zaber_motion-4.2.3/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-4.2.3/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-4.2.3/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/device_definition.py` & `zaber_motion-4.2.3/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/offline_translator.py` & `zaber_motion-4.2.3/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/translate_message.py` & `zaber_motion-4.2.3/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/translate_result.py` & `zaber_motion-4.2.3/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/translator.py` & `zaber_motion-4.2.3/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/gcode/translator_config.py` & `zaber_motion-4.2.3/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/library.py` & `zaber_motion-4.2.3/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/measurement.py` & `zaber_motion-4.2.3/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-4.2.3/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.pyi`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/serialization.py` & `zaber_motion-4.2.3/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/tools.py` & `zaber_motion-4.2.3/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.2/zaber_motion/units.py` & `zaber_motion-4.2.3/zaber_motion/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,19 @@
     INDUCTANCE_MICROHENRIES = 'Inductance:microhenries'
     INDUCTANCE_NANOHENRIES = 'Inductance:nanohenries'
 
     VOLTAGE_CONSTANT_VOLT_SECONDS_PER_RADIAN = 'Voltage Constant:volt seconds per radian'
     VOLTAGE_CONSTANT_MILLIVOLT_SECONDS_PER_RADIAN = 'Voltage Constant:millivolt seconds per radian'
     VOLTAGE_CONSTANT_MICROVOLT_SECONDS_PER_RADIAN = 'Voltage Constant:microvolt seconds per radian'
 
+    ABSOLUTE_TEMPERATURE_DEGREES_CELSIUS = 'Absolute Temperature:degrees Celsius'
+    ABSOLUTE_TEMPERATURE_KELVINS = 'Absolute Temperature:kelvins'
+    ABSOLUTE_TEMPERATURE_DEGREES_FAHRENHEIT = 'Absolute Temperature:degrees Fahrenheit'
+    ABSOLUTE_TEMPERATURE_DEGREES_RANKINE = 'Absolute Temperature:degrees Rankine'
+
 
 UnitsAndLiterals = Union[Units, Literal["m", "cm", "mm", "µm", "um", "nm", "in", "m/s", "cm/s", "mm/s", "µm/s", "um/s", "nm/s", "in/s", "m/s²", "m/s^2", "cm/s²", "cm/s^2", "mm/s²", "mm/s^2", "µm/s²", "um/s^2", "nm/s²", "nm/s^2", "in/s²", "in/s^2", "°", "deg", "rad", "°/s", "deg/s", "rad/s", "°/s²", "deg/s^2", "rad/s²", "rad/s^2", "%", "s", "ms", "µs", "us"]]
 LengthUnits = Union[Units, Literal["m", "cm", "mm", "µm", "um", "nm", "in", "°", "deg", "rad"]]
 VelocityUnits = Union[Units, Literal["m/s", "cm/s", "mm/s", "µm/s", "um/s", "nm/s", "in/s", "°/s", "deg/s", "rad/s"]]
 AccelerationUnits = Union[Units, Literal["m/s²", "m/s^2", "cm/s²", "cm/s^2", "mm/s²", "mm/s^2", "µm/s²", "um/s^2", "nm/s²", "nm/s^2", "in/s²", "in/s^2", "°/s²", "deg/s^2", "rad/s²", "rad/s^2"]]
 TimeUnits = Union[Units, Literal["s", "ms", "µs", "us"]]
```

### Comparing `zaber_motion-4.2.2/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-4.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zaber-motion
-Version: 4.2.2
+Name: zaber_motion
+Version: 4.2.3
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.2/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-4.2.3/zaber_motion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

