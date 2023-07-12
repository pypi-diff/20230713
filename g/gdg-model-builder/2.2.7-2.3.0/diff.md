# Comparing `tmp/gdg-model-builder-2.2.7.tar.gz` & `tmp/gdg-model-builder-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdg-model-builder-2.2.7.tar", max compression
+gzip compressed data, was "gdg-model-builder-2.3.0.tar", max compression
```

## Comparing `gdg-model-builder-2.2.7.tar` & `gdg-model-builder-2.3.0.tar`

### file list

```diff
@@ -1,95 +1,44 @@
--rw-r--r--   0        0        0      471 2023-03-28 18:00:55.259623 gdg-model-builder-2.2.7/gdg_model_builder/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.420190 gdg-model-builder-2.2.7/gdg_model_builder/completion_stream/__init__.py
--rw-r--r--   0        0        0      478 2023-03-28 16:14:48.420579 gdg-model-builder-2.2.7/gdg_model_builder/completion_stream/completion_stream.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.420642 gdg-model-builder-2.2.7/gdg_model_builder/completion_stream/providers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.420728 gdg-model-builder-2.2.7/gdg_model_builder/completion_stream/providers/redis/__init__.py
--rw-r--r--   0        0        0      106 2023-03-28 16:14:48.421004 gdg-model-builder-2.2.7/gdg_model_builder/completion_stream/providers/redis/redis_completion_stream.py
--rw-r--r--   0        0        0     2030 2023-03-28 16:14:48.421459 gdg-model-builder-2.2.7/gdg_model_builder/completion_stream/sc_stream/sc_stream.py
--rw-r--r--   0        0        0      561 2023-01-24 01:17:21.265520 gdg-model-builder-2.2.7/gdg_model_builder/context/bounds/bounds.py
--rw-r--r--   0        0        0      232 2023-01-24 01:17:21.265637 gdg-model-builder-2.2.7/gdg_model_builder/context/bounds/execution/execution.py
--rw-r--r--   0        0        0      218 2023-01-24 01:17:21.265749 gdg-model-builder-2.2.7/gdg_model_builder/context/bounds/session/session.py
--rw-r--r--   0        0        0      197 2023-01-24 01:17:21.265867 gdg-model-builder-2.2.7/gdg_model_builder/context/bounds/user/user.py
--rw-r--r--   0        0        0     2313 2023-03-28 16:14:48.421838 gdg-model-builder-2.2.7/gdg_model_builder/context/context/context.py
--rw-r--r--   0        0        0      346 2023-01-24 01:17:21.266134 gdg-model-builder-2.2.7/gdg_model_builder/context/execution/execution.py
--rw-r--r--   0        0        0      537 2023-01-24 01:17:21.266261 gdg-model-builder-2.2.7/gdg_model_builder/context/session/session.py
--rw-r--r--   0        0        0      468 2023-01-24 01:17:21.266380 gdg-model-builder-2.2.7/gdg_model_builder/context/user/user.py
--rw-r--r--   0        0        0      701 2023-01-24 01:17:21.266502 gdg-model-builder-2.2.7/gdg_model_builder/environment/environment.py
--rw-r--r--   0        0        0       35 2023-01-24 01:17:21.266617 gdg-model-builder-2.2.7/gdg_model_builder/event/__init__.py
--rw-r--r--   0        0        0     2506 2023-01-24 01:17:21.266706 gdg-model-builder-2.2.7/gdg_model_builder/event/event.py
--rw-r--r--   0        0        0     1132 2023-01-24 01:17:21.266795 gdg-model-builder-2.2.7/gdg_model_builder/event/event__test.py
--rw-r--r--   0        0        0      191 2023-02-19 17:51:49.470950 gdg-model-builder-2.2.7/gdg_model_builder/event/event_builder.py
--rw-r--r--   0        0        0        0 2023-01-24 01:17:21.266874 gdg-model-builder-2.2.7/gdg_model_builder/libutil/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 01:17:21.266972 gdg-model-builder-2.2.7/gdg_model_builder/libutil/np/__init__.py
--rw-r--r--   0        0        0      358 2023-01-24 01:17:21.267076 gdg-model-builder-2.2.7/gdg_model_builder/libutil/np/hash.py
--rw-r--r--   0        0        0        0 2023-01-24 01:17:21.267158 gdg-model-builder-2.2.7/gdg_model_builder/libutil/sync/__init__.py
--rw-r--r--   0        0        0      756 2023-01-24 01:17:21.267260 gdg-model-builder-2.2.7/gdg_model_builder/libutil/sync/deasync.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.421923 gdg-model-builder-2.2.7/gdg_model_builder/lock/__init__.py
--rw-r--r--   0        0        0      279 2023-03-28 16:14:48.422215 gdg-model-builder-2.2.7/gdg_model_builder/lock/lock.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.422278 gdg-model-builder-2.2.7/gdg_model_builder/lock/rem_lock/__init__.py
--rw-r--r--   0        0        0      992 2023-03-28 16:14:48.422550 gdg-model-builder-2.2.7/gdg_model_builder/lock/rem_lock/rem_lock.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.422603 gdg-model-builder-2.2.7/gdg_model_builder/lock/rem_lock/rem_lock__test.py
--rw-r--r--   0        0        0      113 2023-03-28 16:14:48.422912 gdg-model-builder-2.2.7/gdg_model_builder/model/__init__.py
--rw-r--r--   0        0        0      938 2023-01-24 01:17:21.267719 gdg-model-builder-2.2.7/gdg_model_builder/model/model__test.py
--rw-r--r--   0        0        0     3694 2023-03-28 16:14:48.423167 gdg-model-builder-2.2.7/gdg_model_builder/model/modellike.py
--rw-r--r--   0        0        0       85 2023-03-28 16:14:48.423399 gdg-model-builder-2.2.7/gdg_model_builder/model/redis_model/__init__.py
--rw-r--r--   0        0        0     2497 2023-03-28 16:14:48.423645 gdg-model-builder-2.2.7/gdg_model_builder/model/redis_model/cron.py
--rw-r--r--   0        0        0    21462 2023-03-28 16:14:48.424119 gdg-model-builder-2.2.7/gdg_model_builder/model/redis_model/model.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.424192 gdg-model-builder-2.2.7/gdg_model_builder/model/redis_model/runtime.py
--rw-r--r--   0        0        0        0 2023-01-24 01:17:21.267807 gdg-model-builder-2.2.7/gdg_model_builder/model_builder_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 01:17:21.267977 gdg-model-builder-2.2.7/gdg_model_builder/model_builder_cli/assets/docker/local.dockerfile
--rw-r--r--   0        0        0     1041 2023-01-24 01:17:21.268136 gdg-model-builder-2.2.7/gdg_model_builder/modifiers/state.py
--rw-r--r--   0        0        0        0 2023-03-16 06:55:05.526941 gdg-model-builder-2.2.7/gdg_model_builder/sdk/__init__.py
--rw-r--r--   0        0        0      364 2023-03-29 16:30:20.159713 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/__init__.py
--rw-r--r--   0        0        0     3011 2023-03-28 17:31:28.593127 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/get_games_by_date.py
--rw-r--r--   0        0        0     2244 2023-03-28 20:25:58.015623 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/get_games_with_lineups_by_date.py
--rw-r--r--   0        0        0     1311 2023-03-29 16:35:33.100656 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/get_games_with_weather_by_date.py
--rw-r--r--   0        0        0     2000 2023-03-29 16:23:21.774294 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/get_stadium.py
--rw-r--r--   0        0        0     2443 2023-03-28 17:31:37.865928 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/lineups_by_date.py
--rw-r--r--   0        0        0      764 2023-03-28 21:55:41.991131 gdg-model-builder-2.2.7/gdg_model_builder/sdk/mlb/weather_at_ballpark.py
--rw-r--r--   0        0        0      193 2023-03-16 06:55:05.528572 gdg-model-builder-2.2.7/gdg_model_builder/sdk/ncaab/__init__.py
--rw-r--r--   0        0        0     4827 2023-03-16 06:55:05.531264 gdg-model-builder-2.2.7/gdg_model_builder/sdk/ncaab/game_stats_by_date.py
--rw-r--r--   0        0        0     4671 2023-03-28 16:49:16.448800 gdg-model-builder-2.2.7/gdg_model_builder/sdk/ncaab/games_by_date.py
--rw-r--r--   0        0        0     2251 2023-03-16 06:55:05.531708 gdg-model-builder-2.2.7/gdg_model_builder/sdk/ncaab/team.py
--rw-r--r--   0        0        0     4200 2023-03-16 06:55:05.531915 gdg-model-builder-2.2.7/gdg_model_builder/sdk/ncaab/team_stats_by_season.py
--rw-r--r--   0        0        0       19 2023-03-16 06:55:05.532124 gdg-model-builder-2.2.7/gdg_model_builder/sdk/spiodirect.py
--rw-r--r--   0        0        0        0 2023-03-28 20:40:46.673826 gdg-model-builder-2.2.7/gdg_model_builder/sdk/weather/__init__.py
--rw-r--r--   0        0        0     2088 2023-03-28 21:47:42.780751 gdg-model-builder-2.2.7/gdg_model_builder/sdk/weather/forecast_at.py
--rw-r--r--   0        0        0     1322 2023-03-28 21:09:34.761124 gdg-model-builder-2.2.7/gdg_model_builder/sdk/weather/weather_at.py
--rw-r--r--   0        0        0       34 2023-02-06 23:53:29.777865 gdg-model-builder-2.2.7/gdg_model_builder/serializer/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.424291 gdg-model-builder-2.2.7/gdg_model_builder/serializer/model_serializer/__init__.py
--rw-r--r--   0        0        0     1814 2023-03-28 16:14:48.424568 gdg-model-builder-2.2.7/gdg_model_builder/serializer/model_serializer/model_serializer.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.424636 gdg-model-builder-2.2.7/gdg_model_builder/serializer/providers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.424721 gdg-model-builder-2.2.7/gdg_model_builder/serializer/providers/redis/__init__.py
--rw-r--r--   0        0        0     4280 2023-03-28 16:14:48.425027 gdg-model-builder-2.2.7/gdg_model_builder/serializer/providers/redis/redis_model_serializer.py
--rw-r--r--   0        0        0     3107 2023-03-28 16:14:48.425346 gdg-model-builder-2.2.7/gdg_model_builder/serializer/providers/redis/redis_model_serializer__test.py
--rw-r--r--   0        0        0      256 2023-03-28 16:14:48.425627 gdg-model-builder-2.2.7/gdg_model_builder/serializer/providers/redis/redis_staged_model_serializer.py
--rw-r--r--   0        0        0     2681 2023-03-28 16:14:48.425948 gdg-model-builder-2.2.7/gdg_model_builder/serializer/serializer.py
--rw-r--r--   0        0        0        0 2023-02-06 23:50:29.675951 gdg-model-builder-2.2.7/gdg_model_builder/structs/__init__.py
--rw-r--r--   0        0        0       21 2023-02-06 23:56:14.589972 gdg-model-builder-2.2.7/gdg_model_builder/structs/entry.py
--rw-r--r--   0        0        0       19 2023-02-06 23:56:36.647114 gdg-model-builder-2.2.7/gdg_model_builder/structs/set.py
--rw-r--r--   0        0        0      713 2023-03-28 16:14:48.426268 gdg-model-builder-2.2.7/gdg_model_builder/structs/table.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.426340 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.426477 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/cbq_listener/__init__.py
--rw-r--r--   0        0        0      636 2023-03-28 16:14:48.426728 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/cbq_listener/cbq_listener.py
--rw-r--r--   0        0        0      739 2023-03-28 16:14:48.426959 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/listener.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.427089 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/providers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.427213 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/serialized_listener/__init__.py
--rw-r--r--   0        0        0      410 2023-03-28 16:14:48.427438 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/serialized_listener/serialized_listener.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.427540 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/sleepy_listener/__init__.py
--rw-r--r--   0        0        0      332 2023-03-28 16:14:48.427753 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/sleepy_listener/sleepy_listener.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.427861 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/std_listener/__init__.py
--rw-r--r--   0        0        0      536 2023-03-28 16:14:48.428089 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/std_listener/std_listener.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.428137 gdg-model-builder-2.2.7/gdg_model_builder/task/listener/std_listener/std_listener__test.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.428213 gdg-model-builder-2.2.7/gdg_model_builder/task/tasker/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.428295 gdg-model-builder-2.2.7/gdg_model_builder/task/tasker/serialized_tasker/__init__.py
--rw-r--r--   0        0        0      837 2023-03-28 16:14:48.428539 gdg-model-builder-2.2.7/gdg_model_builder/task/tasker/serialized_tasker/serialized_tasker.py
--rw-r--r--   0        0        0     3010 2023-03-28 16:14:48.428786 gdg-model-builder-2.2.7/gdg_model_builder/task/tasker/tasker.py
--rw-r--r--   0        0        0        0 2023-03-16 06:55:05.493369 gdg-model-builder-2.2.7/gdg_model_builder/util/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 06:55:05.494848 gdg-model-builder-2.2.7/gdg_model_builder/util/lru/__init__.py
--rw-r--r--   0        0        0      712 2023-03-16 06:55:05.496291 gdg-model-builder-2.2.7/gdg_model_builder/util/lru/lru.py
--rw-r--r--   0        0        0      691 2023-03-16 06:55:05.496567 gdg-model-builder-2.2.7/gdg_model_builder/util/lru/lru__test.py
--rw-r--r--   0        0        0        0 2023-03-28 16:14:48.428848 gdg-model-builder-2.2.7/gdg_model_builder/watcher/__init__.py
--rw-r--r--   0        0        0      176 2023-03-28 16:17:25.378658 gdg-model-builder-2.2.7/gdg_model_builder/watcher/watcher.py
--rw-r--r--   0        0        0      504 2023-03-29 16:35:38.871935 gdg-model-builder-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     2532 2023-03-29 16:35:44.096783 gdg-model-builder-2.2.7/setup.py
--rw-r--r--   0        0        0      653 2023-03-29 16:35:44.096965 gdg-model-builder-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-07-12 18:27:06.089370 gdg-model-builder-2.3.0/gdg_model_builder/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-12 18:25:10.054832 gdg-model-builder-2.3.0/gdg_model_builder/clock/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-06 21:09:17.755431 gdg-model-builder-2.3.0/gdg_model_builder/clock/clock.py
+-rw-r--r--   0        0        0     2119 2023-07-12 20:38:57.871644 gdg-model-builder-2.3.0/gdg_model_builder/clock/predicates.py
+-rw-r--r--   0        0        0      696 2023-07-12 20:25:47.029578 gdg-model-builder-2.3.0/gdg_model_builder/clock/predicates__test.py
+-rw-r--r--   0        0        0      963 2023-07-12 20:39:41.499684 gdg-model-builder-2.3.0/gdg_model_builder/clock/retro_clock.py
+-rw-r--r--   0        0        0      718 2023-05-18 02:32:58.577557 gdg-model-builder-2.3.0/gdg_model_builder/clock/retro_clock__test.py
+-rw-r--r--   0        0        0     1108 2023-07-12 20:39:59.420701 gdg-model-builder-2.3.0/gdg_model_builder/clock/weakref_clock.py
+-rw-r--r--   0        0        0       80 2023-05-18 02:36:11.035940 gdg-model-builder-2.3.0/gdg_model_builder/collection/__init__.py
+-rw-r--r--   0        0        0     1533 2023-05-18 03:25:47.715642 gdg-model-builder-2.3.0/gdg_model_builder/collection/collection.py
+-rw-r--r--   0        0        0     2626 2023-05-18 03:32:05.987825 gdg-model-builder-2.3.0/gdg_model_builder/collection/redis_collection.py
+-rw-r--r--   0        0        0      741 2023-05-18 03:26:33.990249 gdg-model-builder-2.3.0/gdg_model_builder/collection/redis_collection__test.py
+-rw-r--r--   0        0        0       48 2023-07-12 21:46:46.162124 gdg-model-builder-2.3.0/gdg_model_builder/data/__init__.py
+-rw-r--r--   0        0        0      876 2023-07-12 21:44:31.812554 gdg-model-builder-2.3.0/gdg_model_builder/data/bufferized.py
+-rw-r--r--   0        0        0       66 2023-05-17 02:28:13.464600 gdg-model-builder-2.3.0/gdg_model_builder/model/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-12 21:05:42.796002 gdg-model-builder-2.3.0/gdg_model_builder/model/model.py
+-rw-r--r--   0        0        0     5794 2023-07-12 21:54:16.304555 gdg-model-builder-2.3.0/gdg_model_builder/model/standard_model.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:36:40.213943 gdg-model-builder-2.3.0/gdg_model_builder/schedule/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-07 16:57:11.034804 gdg-model-builder-2.3.0/gdg_model_builder/schedule/multiplexed_schedule.py
+-rw-r--r--   0        0        0     2082 2023-05-16 22:49:36.754876 gdg-model-builder-2.3.0/gdg_model_builder/schedule/redis_multiplexed_schedule.py
+-rw-r--r--   0        0        0     4645 2023-05-18 02:33:23.327530 gdg-model-builder-2.3.0/gdg_model_builder/schedule/redis_multiplexed_schedule__test.py
+-rw-r--r--   0        0        0     9894 2023-05-16 23:53:46.567370 gdg-model-builder-2.3.0/gdg_model_builder/schedule/redis_schedule.py
+-rw-r--r--   0        0        0    10739 2023-05-18 02:33:41.608103 gdg-model-builder-2.3.0/gdg_model_builder/schedule/redis_schedule__test.py
+-rw-r--r--   0        0        0      552 2023-05-07 16:07:05.676140 gdg-model-builder-2.3.0/gdg_model_builder/schedule/schedule.py
+-rw-r--r--   0        0        0      537 2023-05-07 15:31:34.120565 gdg-model-builder-2.3.0/gdg_model_builder/schedule/weakref_schedule.py
+-rw-r--r--   0        0        0      159 2023-05-18 03:46:54.580736 gdg-model-builder-2.3.0/gdg_model_builder/shape/__init__.py
+-rw-r--r--   0        0        0      221 2023-07-12 18:43:27.870552 gdg-model-builder-2.3.0/gdg_model_builder/shape/pydantic_event.py
+-rw-r--r--   0        0        0        0 2023-05-06 16:30:45.994017 gdg-model-builder-2.3.0/gdg_model_builder/shape/pydantic_event__test.py
+-rw-r--r--   0        0        0     1348 2023-05-18 01:29:45.025960 gdg-model-builder-2.3.0/gdg_model_builder/shape/pydantic_shape.py
+-rw-r--r--   0        0        0      983 2023-05-18 00:04:34.419433 gdg-model-builder-2.3.0/gdg_model_builder/shape/pydantic_shape__test.py
+-rw-r--r--   0        0        0      665 2023-07-12 21:41:53.590502 gdg-model-builder-2.3.0/gdg_model_builder/shape/shape.py
+-rw-r--r--   0        0        0       24 2023-05-06 22:11:03.134396 gdg-model-builder-2.3.0/gdg_model_builder/state/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-31 23:22:20.499464 gdg-model-builder-2.3.0/gdg_model_builder/state/redis_state.py
+-rw-r--r--   0        0        0      417 2023-05-17 02:17:56.848203 gdg-model-builder-2.3.0/gdg_model_builder/state/state.py
+-rw-r--r--   0        0        0       26 2023-07-12 21:40:55.684272 gdg-model-builder-2.3.0/gdg_model_builder/util/__init__.py
+-rw-r--r--   0        0        0      755 2023-04-24 23:49:21.801047 gdg-model-builder-2.3.0/gdg_model_builder/util/deasync.py
+-rw-r--r--   0        0        0       22 2023-07-12 21:40:44.721480 gdg-model-builder-2.3.0/gdg_model_builder/util/symbol.py
+-rw-r--r--   0        0        0      110 2023-07-12 17:32:04.331263 gdg-model-builder-2.3.0/gdg_model_builder/watcher/__init__.py
+-rw-r--r--   0        0        0     3228 2023-07-12 20:41:12.291100 gdg-model-builder-2.3.0/gdg_model_builder/watcher/redis_watcher.py
+-rw-r--r--   0        0        0     2774 2023-07-12 20:41:02.416786 gdg-model-builder-2.3.0/gdg_model_builder/watcher/redis_watcher__test.py
+-rw-r--r--   0        0        0     1701 2023-07-12 17:48:51.904997 gdg-model-builder-2.3.0/gdg_model_builder/watcher/watcher.py
+-rw-r--r--   0        0        0      565 2023-07-12 22:46:10.950079 gdg-model-builder-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1146 2023-07-12 22:46:15.785097 gdg-model-builder-2.3.0/setup.py
+-rw-r--r--   0        0        0      779 2023-07-12 22:46:15.785246 gdg-model-builder-2.3.0/PKG-INFO
```

### Comparing `gdg-model-builder-2.2.7/gdg_model_builder/libutil/sync/deasync.py` & `gdg-model-builder-2.3.0/gdg_model_builder/util/deasync.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 C = TypeVar("C", bound=Callable)
 
 class DeasyncCallable(Callable):
     bypass : Callable
 
 def deasync(f : A)->C:
     """Transforms an async method into a synchronous one.
-
     :param f: is the method.
     :type f: A is a AsyncCallable
     :return: the synchronous equivalent of the method.
     :rtype: C is the Callable equivalent of the AsyncCallable.
     """
     def wrapper(*args, **kwargs):
         coro = asyncio.coroutine(f)
```

### Comparing `gdg-model-builder-2.2.7/gdg_model_builder/model/model__test.py` & `gdg-model-builder-2.3.0/gdg_model_builder/clock/retro_clock.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-import unittest
-import time
-from fastapi import FastAPI
-from libutil.sync.deasync import deasync
+from .clock import Clock
+from typing import Callable, Awaitable
+from datetime import datetime
+from .weakref_clock import WeakrefClock
 
-def timeit(method):
-    def timed(*args, **kw):
-        ts = time.time()
-        result = method(*args, **kw)
-        te = time.time()
-        if 'log_time' in kw:
-            name = kw.get('log_name', method.__name__.upper())
-            kw['log_time'][name] = int((te - ts) * 1000)
-        else:
-            print('%r  %2.2f ms' % (method.__name__, (te - ts) * 1000))
-        return result
-    return timed
+class RetroClock(WeakrefClock):
+    
+    step : int
+    retrodating : bool
+    internal_time : int
+    
+    def __init__(
+        self, *, 
+        step : int = 1000,
+        start : int = int(datetime.now().timestamp() * 1000) - (1000) # second ago
+    ) -> None:
+        super().__init__()
+        self.step = step
+        self.internal_time = start
+        self.retrodating = True
+    
+    def now(self)->int:
+        
+        return int(datetime.now().timestamp() * 1000) if self.retrodating else self.internal_time
  
-class MYTestCase(unittest.TestCase):
-    """Checks that the get_image_colors methods work appropriately.
-    """
-
-    @deasync
-    async def test_can_create_callable(self):
-        """Experimenting with fast api
-        """
-        app = FastAPI()
-        async def add(a : int, b : int)->int:
-            return a + b
-
-        @app.post(add.__name__)
-        async def inner(a : int, b : int)->int:
-            return a + b
-    
+    async def tick(self):
+        await super().tick()
+        if self.retrodating is True:
+            pass
+        else:
+            pass
+        
+        self.internal_time += self.step
+        if self.internal_time > int(datetime.now().timestamp() * 1000):
+            self.retrodating = False
+
```

### Comparing `gdg-model-builder-2.2.7/PKG-INFO` & `gdg-model-builder-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: gdg-model-builder
-Version: 2.2.7
+Version: 2.3.0
 Summary: 
 License: MIT
 Author: Liam Monninger
 Author-email: l.mak.monninger@gmail.com
 Requires-Python: >3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: cattrs (>=22.1.0,<23.0.0)
 Requires-Dist: checksumdir (>=1.2.0,<2.0.0)
+Requires-Dist: dask (>=2023.3.2,<2024.0.0)
 Requires-Dist: fastapi[all] (>=0.78.0,<0.79.0)
+Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
-Requires-Dist: polars (>=0.16.2,<0.17.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pottery (>=3.0.0,<4.0.0)
 Requires-Dist: pycron (>=3.0.0,<4.0.0)
 Requires-Dist: redis (>=4.3.4,<5.0.0)
```

