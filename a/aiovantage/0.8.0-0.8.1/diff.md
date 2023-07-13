# Comparing `tmp/aiovantage-0.8.0.tar.gz` & `tmp/aiovantage-0.8.1.tar.gz`

## Comparing `aiovantage-0.8.0.tar` & `aiovantage-0.8.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.pylintrc
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aiovantage-0.8.0/TODO
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.vscode/settings.json
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/dump_system.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/load_groups/monitor_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/masters/dump_masters.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/masters/monitor_masters.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/connection.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/discovery.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/errors.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/events.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/query.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/requests.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/close_filter.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_object.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/introspection/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/login/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/login/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/area.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind_base.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind_group.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind_group_base.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/button.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/child_device.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/child_object.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/custom_device.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dc_power_profile.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dimmer.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/eq_ux.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/gmem.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/keypad.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/light_sensor.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/load.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/load_group.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/location_object.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/master.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/module.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/module_gen2.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/omni_sensor.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/pwm_power_profile.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/qis_blind.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/qube_blind.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/relay_blind.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/rgb_load_base.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/sensor.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_rs_485_group_child.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_rs_485_shade_child.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_urtsi_2_group_child.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_urtsi_2_shade_child.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/station_bus.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/station_object.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/system_object.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/task.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/temperature.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/vantage_ddg_color_load.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/vantage_dg_color_load.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/vantage_dmx_dali_gateway.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/modules.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.0/LICENSE
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 aiovantage-0.8.0/README.md
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 aiovantage-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 aiovantage-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.pylintrc
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 aiovantage-0.8.1/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.vscode/settings.json
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/dump_system.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/load_groups/monitor_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/masters/dump_masters.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/masters/monitor_masters.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/connection.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/discovery.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/events.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/requests.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/close_filter.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_object.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/introspection/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/login/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/login/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/area.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind_base.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind_group.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind_group_base.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/button.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/child_device.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/child_object.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/custom_device.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dc_power_profile.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dimmer.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/eq_ux.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/gmem.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/keypad.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/light_sensor.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/load.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/load_group.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/location_object.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/master.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/module.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/module_gen2.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/omni_sensor.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/pwm_power_profile.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/qis_blind.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/qube_blind.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/relay_blind.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/rgb_load_base.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/sensor.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_rs_485_group_child.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_rs_485_shade_child.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_urtsi_2_group_child.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_urtsi_2_shade_child.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/station_bus.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/station_object.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/system_object.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/task.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/temperature.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/vantage_ddg_color_load.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/vantage_dg_color_load.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/vantage_dmx_dali_gateway.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.1/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 aiovantage-0.8.1/README.md
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 aiovantage-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 aiovantage-0.8.1/PKG-INFO
```

### Comparing `aiovantage-0.8.0/.pre-commit-config.yaml` & `aiovantage-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/CONTRIBUTING.md` & `aiovantage-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.8.1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.8.1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/dump_system.py` & `aiovantage-0.8.1/examples/dump_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,24 @@
     """Print text indented by the given number of levels."""
     indent = indent_level * "    "
     print(f"{indent}{text}")
 
 
 def load_state(load: Load) -> str:
     """Return a string describing the state of a load."""
-    if not load.level:
+    if load.level is None:
+        return ""
+
+    if load.level == 0:
         return colorize("(OFF)", RED)
-    elif load.level == 100:
+
+    if load.level == 100:
         return colorize("(ON)", GREEN)
-    else:
-        return colorize(f"({load.level}%)", GREEN)
+
+    return colorize(f"({load.level}%)", GREEN)
 
 
 def print_area(vantage: Vantage, area: Optional[Area], indent: int = 0) -> None:
     """Recursively print an area and all its children."""
     if area is None:
         return
```

### Comparing `aiovantage-0.8.0/examples/monitor_all.py` & `aiovantage-0.8.1/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.8.1/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.8.1/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/areas/dump_areas.py` & `aiovantage-0.8.1/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.8.1/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/blinds/dump_blinds.py` & `aiovantage-0.8.1/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.8.1/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/buttons/dump_buttons.py` & `aiovantage-0.8.1/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.8.1/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/command_client/event_log.py` & `aiovantage-0.8.1/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/command_client/status_load.py` & `aiovantage-0.8.1/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/config_client/dump_objects.py` & `aiovantage-0.8.1/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/config_client/get_version.py` & `aiovantage-0.8.1/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.8.1/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.8.1/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/gmem/dump_gmem.py` & `aiovantage-0.8.1/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.8.1/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/gmem/set_gmem.py` & `aiovantage-0.8.1/examples/gmem/set_gmem.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and value of each GMem
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Look up the object by id
         try:
             gmem_id = int(args.id)
             gmem = await vantage.gmem.aget(gmem_id)
             if gmem is None:
                 print(f"GMem object with id '{gmem_id}' does not exist")
```

### Comparing `aiovantage-0.8.0/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.8.1/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.8.1/examples/light_sensors/monitor_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.8.1/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/load_groups/monitor_load_groups.py` & `aiovantage-0.8.1/examples/load_groups/monitor_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/loads/control_load.py` & `aiovantage-0.8.1/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/loads/dump_loads.py` & `aiovantage-0.8.1/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/loads/monitor_loads.py` & `aiovantage-0.8.1/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/loads/poll_on_loads.py` & `aiovantage-0.8.1/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/loads/toggle_load.py` & `aiovantage-0.8.1/examples/loads/toggle_load.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and value of each GMem
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Look up the load
         try:
             load_id = int(args.id)
         except ValueError:
             print("Invalid load id")
             return
 
         load = await vantage.loads.aget(load_id)
         if load is None:
             print("Load not found")
             return
 
+        # Toggle the load
         print(f"Toggling {load.name} (id = {load.id})")
         if load.is_on:
             await vantage.loads.turn_off(load.id)
         else:
             await vantage.loads.turn_on(load.id)
```

### Comparing `aiovantage-0.8.0/examples/masters/dump_masters.py` & `aiovantage-0.8.1/examples/masters/dump_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/masters/monitor_masters.py` & `aiovantage-0.8.1/examples/masters/monitor_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.8.1/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.8.1/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.8.1/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.8.1/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/stations/dump_stations.py` & `aiovantage-0.8.1/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/stations/jingle_bells.py` & `aiovantage-0.8.1/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/tasks/dump_tasks.py` & `aiovantage-0.8.1/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/tasks/run_task.py` & `aiovantage-0.8.1/examples/tasks/run_task.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,26 +18,28 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and value of each GMem
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Look up the task
         try:
             task_id = int(args.id)
         except ValueError:
             print("Invalid task id")
             return
 
         task = await vantage.tasks.aget(task_id)
         if task is None:
             print("Task not found")
             return
 
+        # Run the task
         print(f"{task.name} (id = {task.id})")
         await vantage.tasks.start(task.id)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.8.0/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.8.1/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.8.1/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/__init__.py` & `aiovantage-0.8.1/src/aiovantage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,37 +71,31 @@
 
         self._event_stream = EventStream(
             host, username, password, ssl=use_ssl, port=command_port
         )
 
         # Set up controllers
         self._controllers: Set[BaseController[Any]] = set()
-
-        def _create_controller(controller_cls: Type[ControllerT]) -> ControllerT:
-            controller = controller_cls(self)
-            self._controllers.add(controller)
-            return controller
-
-        self._anemo_sensors = _create_controller(AnemoSensorsController)
-        self._areas = _create_controller(AreasController)
-        self._blind_groups = _create_controller(BlindGroupsController)
-        self._blinds = _create_controller(BlindsController)
-        self._buttons = _create_controller(ButtonsController)
-        self._dry_contacts = _create_controller(DryContactsController)
-        self._gmem = _create_controller(GMemController)
-        self._light_sensors = _create_controller(LightSensorsController)
-        self._load_groups = _create_controller(LoadGroupsController)
-        self._loads = _create_controller(LoadsController)
-        self._masters = _create_controller(MastersController)
-        self._modules = _create_controller(ModulesController)
-        self._rgb_loads = _create_controller(RGBLoadsController)
-        self._omni_sensors = _create_controller(OmniSensorsController)
-        self._stations = _create_controller(StationsController)
-        self._tasks = _create_controller(TasksController)
-        self._temperature_sensors = _create_controller(TemperatureSensorsController)
+        self._anemo_sensors = self._add_controller(AnemoSensorsController)
+        self._areas = self._add_controller(AreasController)
+        self._blind_groups = self._add_controller(BlindGroupsController)
+        self._blinds = self._add_controller(BlindsController)
+        self._buttons = self._add_controller(ButtonsController)
+        self._dry_contacts = self._add_controller(DryContactsController)
+        self._gmem = self._add_controller(GMemController)
+        self._light_sensors = self._add_controller(LightSensorsController)
+        self._load_groups = self._add_controller(LoadGroupsController)
+        self._loads = self._add_controller(LoadsController)
+        self._masters = self._add_controller(MastersController)
+        self._modules = self._add_controller(ModulesController)
+        self._rgb_loads = self._add_controller(RGBLoadsController)
+        self._omni_sensors = self._add_controller(OmniSensorsController)
+        self._stations = self._add_controller(StationsController)
+        self._tasks = self._add_controller(TasksController)
+        self._temperature_sensors = self._add_controller(TemperatureSensorsController)
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
         return self
 
     async def __aexit__(
         self,
@@ -162,15 +156,15 @@
     @property
     def dry_contacts(self) -> DryContactsController:
         """Return the DryContacts controller for managing dry contacts."""
         return self._dry_contacts
 
     @property
     def gmem(self) -> GMemController:
-        """Return the GMem controller for managing global memory."""
+        """Return the GMem controller for managing variables."""
         return self._gmem
 
     @property
     def light_sensors(self) -> LightSensorsController:
         """Return the LightSensors controller for managing light sensors."""
         return self._light_sensors
 
@@ -187,20 +181,20 @@
     @property
     def masters(self) -> MastersController:
         """Return the Masters controller for managing Vantage Controllers."""
         return self._masters
 
     @property
     def modules(self) -> ModulesController:
-        """Return the Modules controller for managing modules."""
+        """Return the Modules controller for managing dimmer modules."""
         return self._modules
 
     @property
     def omni_sensors(self) -> OmniSensorsController:
-        """Return the OmniSensors controller for managing generic sensors."""
+        """Return the OmniSensors controller for managing omni sensors."""
         return self._omni_sensors
 
     @property
     def rgb_loads(self) -> RGBLoadsController:
         """Return the RGBLoads controller for managing RGB loads."""
         return self._rgb_loads
 
@@ -268,7 +262,13 @@
 
     async def _handle_event(self, event: Event) -> None:
         # Handle events from the event stream.
         if event["type"] == EventType.RECONNECTED:
             for controller in self._controllers:
                 if controller.initialized:
                     await controller.fetch_full_state()
+
+    def _add_controller(self, controller_cls: Type[ControllerT]) -> ControllerT:
+        # Add a controller to the known controllers.
+        controller = controller_cls(self)
+        self._controllers.add(controller)
+        return controller
```

### Comparing `aiovantage-0.8.0/src/aiovantage/connection.py` & `aiovantage-0.8.1/src/aiovantage/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/discovery.py` & `aiovantage-0.8.1/src/aiovantage/discovery.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/errors.py` & `aiovantage-0.8.1/src/aiovantage/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/query.py` & `aiovantage-0.8.1/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/README.md` & `aiovantage-0.8.1/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.8.1/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/commands.py` & `aiovantage-0.8.1/src/aiovantage/command_client/commands.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/events.py` & `aiovantage-0.8.1/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/utils.py` & `aiovantage-0.8.1/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/README.md` & `aiovantage-0.8.1/src/aiovantage/config_client/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 The ACI service is an XML-based RPC service that Design Center uses to communicate
 with Vantage InFusion Controllers. There are a number of "interfaces" exposed, each
 with one or more "methods".
 
 The `ConfigClient` class handles connecting to the ACI service, authenticating, and the
 serialization/deserialization of XML requests and responses.
 
-Various pre-defined method classes are available in [`methods`](methods) to help with
+Various pre-defined classes are available in [`interfaces`](interfaces) to help with
 creating XML serialized requests, but it is also possible to make raw XML requests to
 a particular interface.
 
 Since a common use case for interacting with the ACI service is to lookup system
 objects, this module also provides models to help with deserializing many of these
-object types, available in [`objects`](objects).
+object types, available in [`models`](models).
 
 Additionally, a few helper functions for fetching objects are provided by
 [`requests.py`](requests.py).
 
 ## Examples
 
 ### Lookup objects by type, using a helper
```

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.8.1/src/aiovantage/config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/requests.py` & `aiovantage-0.8.1/src/aiovantage/config_client/requests.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/types.py` & `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py` & `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_object.py` & `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/open_filter.py` & `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/introspection/get_version.py` & `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/login/login.py` & `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/__init__.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/blind_base.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/blind_base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/button.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/child_object.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/child_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/gmem.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/load.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/load_group.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/load_group.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/master.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/master.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/omni_sensor.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/omni_sensor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 """OmniSensor object."""
 
 from dataclasses import dataclass, field
 from decimal import Decimal
+from enum import Enum
 from typing import Union
 
 from .child_object import ChildObject
 from .sensor import Sensor
 
 
+class ConversionType(Enum):
+    """OmniSensor type conversion information."""
+
+    FIXED = "fixed"
+    INT = "int"
+
+
 @dataclass
 class Formula:
-    """OmniSensor type conversion information."""
+    """OmniSensor conversion formula information."""
 
-    return_type: str = field(
+    return_type: ConversionType = field(
         metadata={
             "name": "ReturnType",
             "type": "Attribute",
         }
     )
 
-    level_type: str = field(
+    level_type: ConversionType = field(
         metadata={
             "name": "LevelType",
             "type": "Attribute",
         }
     )
 
+    value: str
+
 
 @dataclass
 class GetMethodType:
-    """Omnisensor method information."""
+    """Omnisensor get method information."""
 
     formula: Formula = field(
         metadata={
             "name": "Formula",
         }
     )
```

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/power_profile.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/power_profile.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/rgb_load_base.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/rgb_load_base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/config_client/models/system_object.py` & `aiovantage-0.8.1/src/aiovantage/config_client/models/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/__init__.py` & `aiovantage-0.8.1/src/aiovantage/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.8.1/src/aiovantage/controllers/anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/base.py` & `aiovantage-0.8.1/src/aiovantage/controllers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     """Which status methods this controller handles from the Enhanced Log."""
 
     def __init__(self, vantage: "Vantage") -> None:
         """Initialize a controller.
 
         Args:
             vantage: The Vantage instance.
-            init_callback: A callback to call when the controller is initialized.
         """
         self._vantage = vantage
         self._items: Dict[int, T] = {}
         self._logger = logging.getLogger(__package__)
         self._subscribed_to_state_changes = False
         self._subscriptions: List[EventSubscription[T]] = []
         self._id_subscriptions: Dict[int, List[EventSubscription[T]]] = {}
@@ -118,15 +117,19 @@
     def parse_object_update(
         self, _vid: int, _status: str, _args: Sequence[str]
     ) -> State:
         """Parse updates from the event stream for an object, should be overridden by subclasses."""
         return None
 
     async def initialize(self, fetch_state: bool = True) -> None:
-        """Populate objects and fetch their initial state."""
+        """Populate objects and fetch their initial state.
+
+        Args:
+            fetch_state: Whether to also fetch the state of each object.
+        """
         prev_ids = set(self._items.keys())
         cur_ids = set()
 
         # Fetch all objects managed by this controller
         async for obj in get_objects(self.config_client, types=self.vantage_types):
             if obj.id not in prev_ids:
                 # This is a new object, add it to the controller
```

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.8.1/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.8.1/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.8.1/src/aiovantage/controllers/light_sensors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-"""Controller holding and managing Vantage buttons."""
+"""Controller holding and managing Vantage light sensors."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
-from aiovantage.command_client.interfaces import ButtonInterface
-from aiovantage.models import Button
+from aiovantage.command_client.interfaces import LightSensorInterface
+from aiovantage.models import LightSensor
 
 from .base import BaseController, State
 
 
-class ButtonsController(BaseController[Button], ButtonInterface):
-    """Controller holding and managing Vantage buttons."""
+class LightSensorsController(BaseController[LightSensor], LightSensorInterface):
+    """Controller holding and managing Vantage light sensors."""
 
-    vantage_types = ("Button",)
+    vantage_types = ("LightSensor",)
     """The Vantage object types that this controller will fetch."""
 
-    status_types = ("BTN",)
-    """Which Vantage 'STATUS' types this controller handles, if any."""
+    enhanced_log_status_methods = ("LightSensor.GetLevel",)
+    """Which status methods this controller handles from the Enhanced Log."""
+
+    @override
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of a light sensor."""
+        return {
+            "level": await LightSensorInterface.get_level(self, vid),
+        }
 
     @override
     def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
-        """Handle state changes for a button."""
-        if status != "BTN":
+        """Handle state changes for a light sensor."""
+        if status != "LightSensor.GetLevel":
             return None
 
         return {
-            "pressed": ButtonInterface.parse_btn_status(args),
+            "level": LightSensorInterface.parse_get_level_status(args),
         }
```

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.8.1/src/aiovantage/controllers/buttons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-"""Controller holding and managing Vantage dry contacts."""
+"""Controller holding and managing Vantage buttons."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import ButtonInterface
-from aiovantage.models import DryContact
+from aiovantage.models import Button
 
 from .base import BaseController, State
 
 
-class DryContactsController(BaseController[DryContact], ButtonInterface):
-    """Controller holding and managing Vantage dry contacts."""
+class ButtonsController(BaseController[Button], ButtonInterface):
+    """Controller holding and managing Vantage buttons."""
 
-    vantage_types = ("DryContact",)
+    vantage_types = ("Button",)
     """The Vantage object types that this controller will fetch."""
 
     status_types = ("BTN",)
     """Which Vantage 'STATUS' types this controller handles, if any."""
 
     @override
+    async def fetch_object_state(self, _vid: int) -> State:
+        """Fetch the state properties of a dry contact."""
+        return {
+            # Buttons are momentary, so default to not pressed to avoid a lookup
+            "pressed": False,
+        }
+
+    @override
     def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
-        """Handle state changes for a dry contact."""
+        """Handle state changes for a button."""
         if status != "BTN":
             return None
 
         return {
-            "triggered": ButtonInterface.parse_btn_status(args),
+            "pressed": ButtonInterface.parse_btn_status(args),
         }
```

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/gmem.py` & `aiovantage-0.8.1/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.8.1/src/aiovantage/controllers/load_groups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-"""Controller holding and managing Vantage light sensors."""
+"""Controller holding and managing Vantage load groups."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
-from aiovantage.command_client.interfaces import LightSensorInterface
-from aiovantage.models import LightSensor
+from aiovantage.command_client.interfaces.load import LoadInterface
+from aiovantage.models import Load, LoadGroup
+from aiovantage.query import QuerySet
 
 from .base import BaseController, State
 
 
-class LightSensorsController(BaseController[LightSensor], LightSensorInterface):
-    """Controller holding and managing Vantage light sensors."""
+class LoadGroupsController(BaseController[LoadGroup], LoadInterface):
+    """Controller holding and managing Vantage load groups."""
 
-    vantage_types = ("LightSensor",)
+    vantage_types = ("LoadGroup",)
     """The Vantage object types that this controller will fetch."""
 
-    enhanced_log_status_methods = ("LightSensor.GetLevel",)
-    """Which status methods this controller handles from the Enhanced Log."""
+    status_types = ("LOAD",)
+    """Which Vantage 'STATUS' types this controller handles, if any."""
 
     @override
     async def fetch_object_state(self, vid: int) -> State:
-        """Fetch the state properties of a light sensor."""
+        """Fetch the state properties of a load."""
         return {
-            "level": await LightSensorInterface.get_level(self, vid),
+            "level": await LoadInterface.get_level(self, vid),
         }
 
     @override
     def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
-        """Handle state changes for a light sensor."""
-        if status != "LightSensor.GetLevel":
+        """Handle state changes for a load."""
+        if status != "LOAD":
             return None
 
         return {
-            "level": LightSensorInterface.parse_get_level_status(args),
+            "level": LoadInterface.parse_load_status(args),
         }
+
+    def loads(self, vid: int) -> QuerySet[Load]:
+        """Return a queryset of all loads in this load group."""
+        load_group = self[vid]
+
+        return self._vantage.loads.filter(lambda load: load.id in load_group.load_ids)
```

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.8.1/src/aiovantage/controllers/dry_contacts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-"""Controller holding and managing Vantage load groups."""
+"""Controller holding and managing Vantage dry contacts."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
-from aiovantage.command_client.interfaces.load import LoadInterface
-from aiovantage.models import Load, LoadGroup
-from aiovantage.query import QuerySet
+from aiovantage.command_client.interfaces import ButtonInterface
+from aiovantage.models import DryContact
 
 from .base import BaseController, State
 
 
-class LoadGroupsController(BaseController[LoadGroup], LoadInterface):
-    """Controller holding and managing Vantage load groups."""
+class DryContactsController(BaseController[DryContact], ButtonInterface):
+    """Controller holding and managing Vantage dry contacts."""
 
-    vantage_types = ("LoadGroup",)
+    vantage_types = ("DryContact",)
     """The Vantage object types that this controller will fetch."""
 
-    status_types = ("LOAD",)
+    status_types = ("BTN",)
     """Which Vantage 'STATUS' types this controller handles, if any."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> State:
-        """Fetch the state properties of a load."""
+    async def fetch_object_state(self, _vid: int) -> State:
+        """Fetch the state properties of a dry contact."""
         return {
-            "level": await LoadInterface.get_level(self, vid),
+            # Dry contacts are momentary, so default to not pressed to avoid a lookup
+            "triggered": False,
         }
 
     @override
     def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
-        """Handle state changes for a load."""
-        if status != "LOAD":
+        """Handle state changes for a dry contact."""
+        if status != "BTN":
             return None
 
         return {
-            "level": LoadInterface.parse_load_status(args),
+            "triggered": ButtonInterface.parse_btn_status(args),
         }
-
-    def loads(self, vid: int) -> QuerySet[Load]:
-        """Return a queryset of all loads in this load group."""
-        load_group = self[vid]
-
-        return self._vantage.loads.filter(lambda load: load.id in load_group.load_ids)
```

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.8.1/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/masters.py` & `aiovantage-0.8.1/src/aiovantage/controllers/masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.8.1/src/aiovantage/controllers/omni_sensors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage omni sensors."""
 
 from decimal import Decimal
 from typing import Sequence, Union
 
 from typing_extensions import override
 
-from aiovantage.models import OmniSensor
+from aiovantage.config_client.models.omni_sensor import ConversionType, OmniSensor
 
 from .base import BaseController, State
 
 
 class OmniSensorsController(BaseController[OmniSensor]):
     """Controller holding and managing Vantage omni sensors."""
 
@@ -52,24 +52,24 @@
         method = omni_sensor.get.method if cached else omni_sensor.get.method_hw
 
         # INVOKE <id> <method>
         # -> R:INVOKE <id> <value> <method>
         response = await self.command_client.command("INVOKE", vid, method)
 
         # Convert the level to the correct type
-        if omni_sensor.get.formula.return_type == "fixed":
+        if omni_sensor.get.formula.return_type == ConversionType.FIXED:
             level = Decimal(response.args[1])
-            if omni_sensor.get.formula.level_type == "int":
+            if omni_sensor.get.formula.level_type == ConversionType.INT:
                 return int(level)
 
             return level
 
-        if omni_sensor.get.formula.return_type == "int":
+        if omni_sensor.get.formula.return_type == ConversionType.INT:
             level = Decimal(response.args[1]) / 1000
-            if omni_sensor.get.formula.level_type == "int":
+            if omni_sensor.get.formula.level_type == ConversionType.INT:
                 return int(level)
 
             return level
 
         raise ValueError(f"Unknown return type {omni_sensor.get.formula.return_type}")
 
     @classmethod
@@ -78,11 +78,11 @@
     ) -> Union[int, Decimal]:
         """Parse an OmniSensor 'GetLevel' event, eg. 'PowerSensor.GetPower'."""
         # ELLOG STATUS ON
         # -> EL: <id> <method> <value>
         # STATUS ADD <id>
         # -> S:STATUS <id> <method> <value>
         level = Decimal(args[0]) / 1000
-        if omni_sensor.get.formula.level_type == "int":
+        if omni_sensor.get.formula.level_type == ConversionType.INT:
             return int(level)
 
         return level
```

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.8.1/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.8.1/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.8.1/src/aiovantage/controllers/temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/LICENSE` & `aiovantage-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/README.md` & `aiovantage-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/pyproject.toml` & `aiovantage-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.0/PKG-INFO` & `aiovantage-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.8.0
+Version: 0.8.1
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
```

