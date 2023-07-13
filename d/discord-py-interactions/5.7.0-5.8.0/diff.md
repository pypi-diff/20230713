# Comparing `tmp/discord-py-interactions-5.7.0.tar.gz` & `tmp/discord-py-interactions-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-5.7.0.tar", last modified: Mon Jun 19 07:12:48 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.8.0.tar", last modified: Thu Jul 13 19:03:24 2023, max compression
```

## Comparing `discord-py-interactions-5.7.0.tar` & `discord-py-interactions-5.8.0.tar`

### file list

```diff
@@ -1,192 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.223792 discord-py-interactions-5.7.0/discord_py_interactions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-19 07:12:48.000000 discord-py-interactions-5.7.0/discord_py_interactions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-19 07:12:48.000000 discord-py-interactions-5.7.0/discord_py_interactions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:12:48.000000 discord-py-interactions-5.7.0/discord_py_interactions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-19 07:12:48.000000 discord-py-interactions-5.7.0/discord_py_interactions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 07:12:48.000000 discord-py-interactions-5.7.0/discord_py_interactions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.223792 discord-py-interactions-5.7.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.223792 discord-py-interactions-5.7.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.223792 discord-py-interactions-5.7.0/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24007 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.227792 discord-py-interactions-5.7.0/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.227792 discord-py-interactions-5.7.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.231792 discord-py-interactions-5.7.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.235792 discord-py-interactions-5.7.0/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.235792 discord-py-interactions-5.7.0/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.235792 discord-py-interactions-5.7.0/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.239792 discord-py-interactions-5.7.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    92213 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.239792 discord-py-interactions-5.7.0/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.243792 discord-py-interactions-5.7.0/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.243792 discord-py-interactions-5.7.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.243792 discord-py-interactions-5.7.0/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/debug_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.247792 discord-py-interactions-5.7.0/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.247792 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.247792 discord-py-interactions-5.7.0/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.255792 discord-py-interactions-5.7.0/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   103562 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    96261 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    38399 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55760 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    36003 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/interactions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-19 07:12:48.267792 discord-py-interactions-5.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-19 07:12:38.000000 discord-py-interactions-5.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:48.263792 discord-py-interactions-5.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 07:12:24.000000 discord-py-interactions-5.7.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23953 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92213 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23266 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/hybrid_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.484833 discord-py-interactions-5.8.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.484833 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.484833 discord-py-interactions-5.8.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.488834 discord-py-interactions-5.8.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103722 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31037 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96356 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38408 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.492833 discord-py-interactions-5.8.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.492833 discord-py-interactions-5.8.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55760 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.492833 discord-py-interactions-5.8.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-13 19:03:17.000000 discord-py-interactions-5.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/utils.py
```

### Comparing `discord-py-interactions-5.7.0/LICENSE` & `discord-py-interactions-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/PKG-INFO` & `discord-py-interactions-5.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.7.0
+Version: 5.8.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.7.0/README.md` & `discord-py-interactions-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/discord_py_interactions.egg-info/PKG-INFO` & `discord-py-interactions-5.8.0/discord_py_interactions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.7.0
+Version: 5.8.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.7.0/discord_py_interactions.egg-info/SOURCES.txt` & `discord-py-interactions-5.8.0/discord_py_interactions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 interactions/ext/paginators.py
 interactions/ext/sentry.py
 interactions/ext/debug_extension/__init__.py
 interactions/ext/debug_extension/debug_application_cmd.py
 interactions/ext/debug_extension/debug_exec.py
 interactions/ext/debug_extension/debug_exts.py
 interactions/ext/debug_extension/utils.py
+interactions/ext/hybrid_commands/__init__.py
+interactions/ext/hybrid_commands/context.py
+interactions/ext/hybrid_commands/hybrid_slash.py
+interactions/ext/hybrid_commands/manager.py
 interactions/ext/mypy/__init__.py
 interactions/ext/prefixed_commands/__init__.py
 interactions/ext/prefixed_commands/command.py
 interactions/ext/prefixed_commands/context.py
 interactions/ext/prefixed_commands/help.py
 interactions/ext/prefixed_commands/manager.py
 interactions/ext/prefixed_commands/utils.py
```

### Comparing `discord-py-interactions-5.7.0/discord_py_interactions.egg-info/requires.txt` & `discord-py-interactions-5.8.0/discord_py_interactions.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 mkdocs-autorefs
 mkdocs-awesome-pages-plugin
 mkdocs-material
 mkdocstrings-python
 mkdocs-minify-plugin
 mkdocs-git-committers-plugin-2
 mkdocs-git-revision-date-localized-plugin
+griffe==0.25
 pre-commit
 
 [dev:sys_platform != "win32"]
 uvloop
 
 [docs]
 PyNaCl<1.6,>=1.5.0
@@ -58,14 +59,15 @@
 mkdocs-autorefs
 mkdocs-awesome-pages-plugin
 mkdocs-material
 mkdocstrings-python
 mkdocs-minify-plugin
 mkdocs-git-committers-plugin-2
 mkdocs-git-revision-date-localized-plugin
+griffe==0.25
 
 [docs:sys_platform != "win32"]
 uvloop
 
 [jurigged]
 jurigged
```

### Comparing `discord-py-interactions-5.7.0/interactions/__init__.py` & `discord-py-interactions-5.8.0/interactions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     GuildCategoryConverter,
     GuildChannel,
     GuildChannelConverter,
     GuildConverter,
     GuildForum,
     GuildForumPost,
     GuildIntegration,
+    GuildMedia,
     GuildNews,
     GuildNewsConverter,
     GuildNewsThread,
     GuildNewsThreadConverter,
     GuildPreview,
     GuildPrivateThread,
     GuildPrivateThreadConverter,
@@ -472,14 +473,15 @@
     "GuildCategoryConverter",
     "GuildChannel",
     "GuildChannelConverter",
     "GuildConverter",
     "GuildForum",
     "GuildForumPost",
     "GuildIntegration",
+    "GuildMedia",
     "GuildNews",
     "GuildNewsConverter",
     "GuildNewsThread",
     "GuildNewsThreadConverter",
     "GuildPreview",
     "GuildPrivateThread",
     "GuildPrivateThreadConverter",
```

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/__init__.py` & `discord-py-interactions-5.8.0/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/base.py` & `discord-py-interactions-5.8.0/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/discord.py` & `discord-py-interactions-5.8.0/interactions/api/events/discord.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 These are events dispatched by Discord. This is intended as a reference so you know what data to expect for each event.
 
-??? Hint "Example Usage:"
-    The event classes outlined here are in `CamelCase` to comply with Class naming convention, however the event names
-    are actually in `lower_case_with_underscores` so your listeners should be named as following:
+???+ hint "Example Usage"
+    To listen to an event, use the `listen` decorator:
 
     ```python
-    @listen()
-    def on_ready():
-        # ready events pass no data, so dont have params
-        print("Im ready!")
-
-    @listen()
-    def on_guild_join(event):
-        # guild_create events pass a guild object, expect a single param
-        print(f"{event.guild.name} created")
+    from interactions import listen
+    from interactions.api.events import ChannelCreate  # or any other event
+
+    @listen(ChannelCreate)
+    async def an_event_handler(event: ChannelCreate):
+        print(f"Channel created with name: {event.channel.name}")
     ```
+
+    For more information, including other ways to listen to events, see [the events guide](/interactions.py/Guides/10 Events).
+
 !!! warning
     While all of these events are documented, not all of them are used, currently.
 
 """
 
 from typing import TYPE_CHECKING, List, Sequence, Union, Optional
```

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/internal.py` & `discord-py-interactions-5.8.0/interactions/api/events/internal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 These are events dispatched by the client. This is intended as a reference so you know what data to expect for each event.
 
-??? Hint "Example Usage:"
-    The event classes outlined here are in `CamelCase` to comply with Class naming convention, however the event names
-    are actually in `lower_case_with_underscores` so your listeners should be named as following:
+???+ hint "Example Usage"
+    To listen to an event, use the `listen` decorator:
 
     ```python
-    @listen()
-    def on_ready():
-        # ready events pass no data, so dont have params
-        print("Im ready!")
-
-    @listen()
-    def on_guild_join(event):
-        # guild_create events pass a guild object, expect a single param
-        print(f"{event.guild.name} created")
+    from interactions import listen
+    from interactions.api.events import ChannelCreate  # or any other event
+
+    @listen(ChannelCreate)
+    async def an_event_handler(event: ChannelCreate):
+        print(f"Channel created with name: {event.channel.name}")
     ```
+
+    For more information, including other ways to listen to events, see [the events guide](/interactions.py/Guides/10 Events).
+
 !!! warning
     While all of these events are documented, not all of them are used, currently.
 
 """
 import re
 import typing
 from typing import Any, Optional, TYPE_CHECKING, Type
```

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/__init__.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/_template.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/auto_mod.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/auto_mod.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __all__ = ("AutoModEvents",)
 
 
 class AutoModEvents(EventMixinTemplate):
     @Processor.define()
     async def _raw_auto_moderation_action_execution(self, event: "RawGatewayEvent") -> None:
         action = AutoModerationAction.from_dict(event.data.copy(), self)
-        channel = self.get_channel(event.data["channel_id"])
+        channel = self.get_channel(event.data.get("channel_id"))
         guild = self.get_guild(event.data["guild_id"])
         self.dispatch(events.AutoModExec(action, channel, guild))
 
     @Processor.define()
     async def raw_auto_moderation_rule_create(self, event: "RawGatewayEvent") -> None:
         rule = AutoModRule.from_dict(event.data, self)
         guild = self.get_guild(event.data["guild_id"])
```

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/channel_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/guild_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/integrations.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/member_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/message_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/reaction_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/role_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/stage_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/thread_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/user_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/events/processors/voice_events.py` & `discord-py-interactions-5.8.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/gateway/gateway.py` & `discord-py-interactions-5.8.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/gateway/state.py` & `discord-py-interactions-5.8.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/gateway/websocket.py` & `discord-py-interactions-5.8.0/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_client.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/__init__.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/bot.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/channels.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/emojis.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/guild.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/interactions.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/members.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/messages.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/reactions.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/scheduled_events.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/stickers.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/threads.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/users.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/http_requests/webhooks.py` & `discord-py-interactions-5.8.0/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/http/route.py` & `discord-py-interactions-5.8.0/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/audio.py` & `discord-py-interactions-5.8.0/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/audio_writer.py` & `discord-py-interactions-5.8.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/encryption.py` & `discord-py-interactions-5.8.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/opus.py` & `discord-py-interactions-5.8.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/player.py` & `discord-py-interactions-5.8.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/recorder.py` & `discord-py-interactions-5.8.0/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/api/voice/voice_gateway.py` & `discord-py-interactions-5.8.0/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/bin/opus-x64.dll` & `discord-py-interactions-5.8.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/bin/opus-x86.dll` & `discord-py-interactions-5.8.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/__init__.py` & `discord-py-interactions-5.8.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/auto_shard_client.py` & `discord-py-interactions-5.8.0/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/client.py` & `discord-py-interactions-5.8.0/interactions/client/client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/const.py` & `discord-py-interactions-5.8.0/interactions/client/const.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/errors.py` & `discord-py-interactions-5.8.0/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/mixins/modal.py` & `discord-py-interactions-5.8.0/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/mixins/send.py` & `discord-py-interactions-5.8.0/interactions/client/mixins/send.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,9 +107,12 @@
             **kwargs,
         )
 
         message_data = await self._send_http_request(message_payload, files=files or file)
         if message_data:
             message = self.client.cache.place_message_data(message_data)
             if delete_after:
-                await message.delete(delay=delete_after)
+                if kwargs.get("pass_self_into_delete"):  # hack to pass in interaction/hybrid context
+                    await message.delete(delay=delete_after, context=self)
+                else:
+                    await message.delete(delay=delete_after)
             return message
```

### Comparing `discord-py-interactions-5.7.0/interactions/client/mixins/serialization.py` & `discord-py-interactions-5.8.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/smart_cache.py` & `discord-py-interactions-5.8.0/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/__init__.py` & `discord-py-interactions-5.8.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/attr_converters.py` & `discord-py-interactions-5.8.0/interactions/client/utils/attr_converters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import typing
+import interactions
 from datetime import datetime
 from typing import Callable, Union, Any
 
 from interactions.client.const import MISSING
 from interactions.models.discord.timestamp import Timestamp
 
 __all__ = ("timestamp_converter", "list_converter", "optional")
@@ -16,21 +17,26 @@
     Args:
         value: The time value to convert
 
     Returns:
         A Timestamp object
 
     """
-    if isinstance(value, str):
-        return Timestamp.fromisoformat(value)
-    if isinstance(value, (float, int)):
-        return Timestamp.fromtimestamp(float(value))
-    if isinstance(value, datetime):
-        return Timestamp.fromdatetime(value)
-    raise TypeError("Timestamp must be one of: datetime, int, float, ISO8601 str")
+    try:
+        if isinstance(value, str):
+            return Timestamp.fromisoformat(value)
+        if isinstance(value, (float, int)):
+            return Timestamp.fromtimestamp(float(value))
+        if isinstance(value, datetime):
+            return Timestamp.fromdatetime(value)
+        raise TypeError("Timestamp must be one of: datetime, int, float, ISO8601 str")
+    except ValueError as e:
+        interactions.const.get_logger().warning("Failed to convert timestamp", exc_info=e)
+        # Should only happen if the timestamp is something stupid like 269533-01-01T00:00 - in which case we just return MISSING
+        return MISSING
 
 
 def list_converter(converter) -> Callable[[list], list]:
     """Converts a list of values to a list of converted values"""
 
     def convert_action(value: Union[list, Any]) -> list:
         if not isinstance(value, list):
```

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/attr_utils.py` & `discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/attr_utils.pyi` & `discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/cache.py` & `discord-py-interactions-5.8.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/deserialise_app_cmds.py` & `discord-py-interactions-5.8.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/formatting.py` & `discord-py-interactions-5.8.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/input_utils.py` & `discord-py-interactions-5.8.0/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/misc_utils.py` & `discord-py-interactions-5.8.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/serializer.py` & `discord-py-interactions-5.8.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/client/utils/text_utils.py` & `discord-py-interactions-5.8.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/console.py` & `discord-py-interactions-5.8.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/debug_extension/__init__.py` & `discord-py-interactions-5.8.0/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/debug_extension/debug_application_cmd.py` & `discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/debug_extension/debug_exec.py` & `discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/debug_extension/debug_exts.py` & `discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/debug_extension/utils.py` & `discord-py-interactions-5.8.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/jurigged.py` & `discord-py-interactions-5.8.0/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/mypy/__init__.py` & `discord-py-interactions-5.8.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/paginators.py` & `discord-py-interactions-5.8.0/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/__init__.py` & `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/command.py` & `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/context.py` & `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/help.py` & `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/manager.py` & `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/prefixed_commands/utils.py` & `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/ext/sentry.py` & `discord-py-interactions-5.8.0/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/__init__.py` & `discord-py-interactions-5.8.0/interactions/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     Guild,
     GuildBan,
     GuildCategory,
     GuildChannel,
     GuildForum,
     GuildForumPost,
     GuildIntegration,
+    GuildMedia,
     GuildNews,
     GuildNewsThread,
     GuildPreview,
     GuildPrivateThread,
     GuildPublicThread,
     GuildStageVoice,
     GuildTemplate,
@@ -407,14 +408,15 @@
     "GuildCategoryConverter",
     "GuildChannel",
     "GuildChannelConverter",
     "GuildConverter",
     "GuildForum",
     "GuildForumPost",
     "GuildIntegration",
+    "GuildMedia",
     "GuildNews",
     "GuildNewsConverter",
     "GuildNewsThread",
     "GuildNewsThreadConverter",
     "GuildPreview",
     "GuildPrivateThread",
     "GuildPrivateThreadConverter",
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/__init__.py` & `discord-py-interactions-5.8.0/interactions/models/discord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     DM,
     DMChannel,
     DMGroup,
     GuildCategory,
     GuildChannel,
     GuildForum,
     GuildForumPost,
+    GuildMedia,
     GuildNews,
     GuildNewsThread,
     GuildPrivateThread,
     GuildPublicThread,
     GuildStageVoice,
     GuildText,
     GuildVoice,
@@ -230,14 +231,15 @@
     "Guild",
     "GuildBan",
     "GuildCategory",
     "GuildChannel",
     "GuildForum",
     "GuildForumPost",
     "GuildIntegration",
+    "GuildMedia",
     "GuildNews",
     "GuildNewsThread",
     "GuildPreview",
     "GuildPrivateThread",
     "GuildPublicThread",
     "GuildStageVoice",
     "GuildTemplate",
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/activity.py` & `discord-py-interactions-5.8.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/app_perms.py` & `discord-py-interactions-5.8.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/application.py` & `discord-py-interactions-5.8.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/asset.py` & `discord-py-interactions-5.8.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/auto_mod.py` & `discord-py-interactions-5.8.0/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/base.py` & `discord-py-interactions-5.8.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/channel.py` & `discord-py-interactions-5.8.0/interactions/models/discord/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2636,14 +2636,19 @@
         Args:
             tag_id: The ID of the tag to delete
         """
         data = await self._client.http.delete_tag(self.id, tag_id)
         self._client.cache.place_channel_data(data)
 
 
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class GuildMedia(GuildForum):
+    ...
+
+
 def process_permission_overwrites(
     overwrites: Union[dict, PermissionOverwrite, List[Union[dict, PermissionOverwrite]]]
 ) -> List[dict]:
     """
     Processes a permission overwrite lists into format for sending to discord.
 
     Args:
@@ -2690,14 +2695,15 @@
 TYPE_GUILD_CHANNEL = Union[
     GuildCategory,
     GuildNews,
     GuildText,
     GuildVoice,
     GuildStageVoice,
     GuildForum,
+    GuildMedia,
     GuildPublicThread,
     GuildForumPost,
     GuildPrivateThread,
 ]
 
 
 TYPE_THREAD_CHANNEL = Union[GuildNewsThread, GuildPublicThread, GuildForumPost, GuildPrivateThread]
@@ -2727,8 +2733,9 @@
     ChannelType.GUILD_CATEGORY: GuildCategory,
     ChannelType.GUILD_PUBLIC_THREAD: GuildPublicThread,
     ChannelType.GUILD_PRIVATE_THREAD: GuildPrivateThread,
     ChannelType.GUILD_NEWS_THREAD: GuildNewsThread,
     ChannelType.DM: DM,
     ChannelType.GROUP_DM: DMGroup,
     ChannelType.GUILD_FORUM: GuildForum,
+    ChannelType.GUILD_MEDIA: GuildMedia,
 }
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/color.py` & `discord-py-interactions-5.8.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/components.py` & `discord-py-interactions-5.8.0/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/embed.py` & `discord-py-interactions-5.8.0/interactions/models/discord/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,20 @@
     type: EmbedType = attrs.field(
         repr=False,
         default=EmbedType.RICH,
         converter=c_optional(EmbedType),
         metadata=no_export_meta,
     )
 
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
+        if image_data := data.pop("image", None):
+            data["images"] = [image_data]
+        return data
+
     @property
     def image(self) -> Optional[EmbedAttachment]:
         """
         The image of the embed.
 
         Raises:
             ValueError: If there are multiple images in the embed.
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/emoji.py` & `discord-py-interactions-5.8.0/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/enums.py` & `discord-py-interactions-5.8.0/interactions/models/discord/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,14 +607,16 @@
     """Temporary sub-channel within a GUILD_TEXT channel"""
     GUILD_PRIVATE_THREAD = 12
     """Temporary sub-channel within a GUILD_TEXT channel that is only viewable by those invited and those with the MANAGE_THREADS permission"""
     GUILD_STAGE_VOICE = 13
     """Voice channel for hosting events with an audience"""
     GUILD_FORUM = 15
     """A Forum channel"""
+    GUILD_MEDIA = 16
+    """Channel that can only contain threads, similar to `GUILD_FORUM` channels"""
 
     @property
     def guild(self) -> bool:
         """Whether this channel is a guild channel."""
         return self.value not in {1, 3}
 
     @property
@@ -790,14 +792,16 @@
 
 
 class ChannelFlags(DiscordIntFlag):
     PINNED = 1 << 1
     """ Thread is pinned to the top of its parent forum channel """
     CLYDE_THREAD = 1 << 8
     """This thread was created by Clyde"""
+    HIDE_MEDIA_DOWNLOAD_OPTIONS = 1 << 15
+    """when set hides the embedded media download options. Available only for media channels"""
 
     # Special members
     NONE = 0
 
 
 class VideoQualityMode(CursedIntEnum):
     """Video quality settings."""
@@ -964,14 +968,15 @@
     APPLICATION_COMMAND_PERMISSION_UPDATE = 121
     AUTO_MODERATION_RULE_CREATE = 140
     AUTO_MODERATION_RULE_UPDATE = 141
     AUTO_MODERATION_RULE_DELETE = 142
     AUTO_MODERATION_BLOCK_MESSAGE = 143
     AUTO_MODERATION_FLAG_TO_CHANNEL = 144
     AUTO_MODERATION_USER_COMMUNICATION_DISABLED = 145
+    AUTO_MODERATION_QUARANTINE = 146
     CREATOR_MONETIZATION_REQUEST_CREATED = 150
     CREATOR_MONETIZATION_TERMS_ACCEPTED = 151
     ROLE_PROMPT_CREATE = 160
     ROLE_PROMPT_UPDATE = 161
     ROLE_PROMPT_DELETE = 162
     ON_BOARDING_QUESTION_CREATE = 163
     ON_BOARDING_QUESTION_UPDATE = 164
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/file.py` & `discord-py-interactions-5.8.0/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/guild.py` & `discord-py-interactions-5.8.0/interactions/models/discord/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,16 @@
     def threads(self) -> List["models.TYPE_THREAD_CHANNEL"]:
         """Returns a list of threads associated with this guild."""
         return [self._client.cache.get_channel(t_id) for t_id in self._thread_ids]
 
     @property
     def members(self) -> List["models.Member"]:
         """Returns a list of all members within this guild."""
-        return [self._client.cache.get_member(self.id, m_id) for m_id in self._member_ids]
+        members = (self._client.cache.get_member(self.id, m_id) for m_id in self._member_ids)
+        return [m for m in members if m]
 
     @property
     def premium_subscribers(self) -> List["models.Member"]:
         """Returns a list of all premium subscribers"""
         return [member for member in self.members if member.premium]
 
     @property
@@ -364,15 +365,15 @@
     def humans(self) -> List["models.Member"]:
         """Returns a list of all humans within this guild"""
         return [member for member in self.members if not member.bot]
 
     @property
     def roles(self) -> List["models.Role"]:
         """Returns a list of roles associated with this guild."""
-        return sorted([self._client.cache.get_role(r_id) for r_id in self._role_ids], reverse=True)
+        return sorted((r for r_id in self._role_ids if (r := self._client.cache.get_role(r_id))), reverse=True)
 
     @property
     def me(self) -> "models.Member":
         """Returns this bots member object within this guild."""
         return self._client.cache.get_member(self.id, self._client.user.id)
 
     @property
@@ -1471,15 +1472,15 @@
         if name:
             payload["name"] = name
 
         if permissions is not MISSING and permissions is not None:
             payload["permissions"] = str(int(permissions))
 
         if colour := colour or color:
-            payload["color"] = colour.value
+            payload["color"] = colour if isinstance(colour, int) else colour.value
 
         if hoist:
             payload["hoist"] = True
 
         if mentionable:
             payload["mentionable"] = True
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/invite.py` & `discord-py-interactions-5.8.0/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/message.py` & `discord-py-interactions-5.8.0/interactions/models/discord/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,17 +183,18 @@
 
     @classmethod
     def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
         user_data = data["user"]
         data["user_id"] = client.cache.place_user_data(user_data).id
         return data
 
-    async def user(self) -> "models.User":
+    @property
+    def user(self) -> "models.User":
         """Get the user associated with this interaction."""
-        return await self.get_user(self._user_id)
+        return self.client.get_user(self._user_id)
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=False)
 class AllowedMentions(DictSerializationMixin):
     """
     The allowed mention field allows for more granular control over mentions without various hacks to the message content.
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/modal.py` & `discord-py-interactions-5.8.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/reaction.py` & `discord-py-interactions-5.8.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/role.py` & `discord-py-interactions-5.8.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/scheduled_event.py` & `discord-py-interactions-5.8.0/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/snowflake.py` & `discord-py-interactions-5.8.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/stage_instance.py` & `discord-py-interactions-5.8.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/sticker.py` & `discord-py-interactions-5.8.0/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/team.py` & `discord-py-interactions-5.8.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/thread.py` & `discord-py-interactions-5.8.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/timestamp.py` & `discord-py-interactions-5.8.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/user.py` & `discord-py-interactions-5.8.0/interactions/models/discord/user.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/user.pyi` & `discord-py-interactions-5.8.0/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/voice_state.py` & `discord-py-interactions-5.8.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/discord/webhooks.py` & `discord-py-interactions-5.8.0/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/__init__.py` & `discord-py-interactions-5.8.0/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/active_voice_state.py` & `discord-py-interactions-5.8.0/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/annotations/slash.py` & `discord-py-interactions-5.8.0/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/application_commands.py` & `discord-py-interactions-5.8.0/interactions/models/internal/application_commands.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/auto_defer.py` & `discord-py-interactions-5.8.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/callback.py` & `discord-py-interactions-5.8.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/checks.py` & `discord-py-interactions-5.8.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/command.py` & `discord-py-interactions-5.8.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/context.py` & `discord-py-interactions-5.8.0/interactions/models/internal/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,16 +233,14 @@
 
 class BaseInteractionContext(BaseContext):
     token: str
     """The interaction token."""
     id: Snowflake
     """The interaction ID."""
 
-    app_permissions: Permissions
-    """The permissions available to this interaction"""
     locale: str
     """The selected locale of the invoking user (https://discord.com/developers/docs/reference#locales)"""
     guild_locale: str
     """The selected locale of the invoking user's guild (https://discord.com/developers/docs/reference#locales)"""
     resolved: Resolved
     """The resolved data for this interaction."""
 
@@ -257,14 +255,16 @@
     _context_type: int
     """The context type of the interaction."""
     command_id: Snowflake
     """The command ID of the interaction."""
     _command_name: str
     """The command name of the interaction."""
 
+    permission_map: dict[Snowflake, Permissions]
+
     args: list[typing.Any]
     """The arguments passed to the interaction."""
     kwargs: dict[str, typing.Any]
     """The keyword arguments passed to the interaction."""
 
     def __init__(self, client: "interactions.Client") -> None:
         super().__init__(client)
@@ -273,15 +273,15 @@
         self.ephemeral = False
 
     @classmethod
     def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
         instance = cls(client=client)
         instance.token = payload["token"]
         instance.id = Snowflake(payload["id"])
-        instance.app_permissions = Permissions(payload.get("app_permissions", 0))
+        instance.permission_map = {client.app.id: Permissions(payload.get("app_permissions", 0))}
         instance.locale = payload["locale"]
         instance.guild_locale = payload.get("guild_locale", instance.locale)
         instance._context_type = payload.get("type", 0)
         instance.resolved = Resolved.from_dict(client, payload["data"].get("resolved", {}), payload.get("guild_id"))
 
         instance.channel_id = Snowflake(payload["channel_id"])
         if member := payload.get("member"):
@@ -300,17 +300,32 @@
 
         if payload["type"] in (InteractionType.APPLICATION_COMMAND, InteractionType.AUTOCOMPLETE):
             instance.command_id = Snowflake(payload["data"]["id"])
             instance._command_name = payload["data"]["name"]
 
         instance.process_options(payload)
 
+        if member := payload.get("member"):
+            instance.permission_map[Snowflake(member["id"])] = Permissions(member["permissions"])
+
         return instance
 
     @property
+    def app_permissions(self) -> Permissions:
+        """The permissions available to this interaction"""
+        return self.permission_map.get(self.client.app.id, Permissions(0))
+
+    @property
+    def author_permissions(self) -> Permissions:
+        """The permissions available to the author of this interaction"""
+        if self.guild_id:
+            return self.permission_map.get(self.author_id, Permissions(0))
+        return Permissions(0)
+
+    @property
     def command(self) -> InteractionCommand:
         return self.client._interaction_lookup[self._command_name]
 
     @property
     def expires_at(self) -> typing.Optional[datetime.datetime]:
         """The time at which the interaction expires."""
         if self.responded:
@@ -519,14 +534,15 @@
             allowed_mentions=allowed_mentions,
             reply_to=reply_to,
             files=files,
             file=file,
             tts=tts,
             flags=flags,
             delete_after=delete_after,
+            pass_self_into_delete=True,
             **kwargs,
         )
 
     respond = send
 
     async def delete(self, message: "Snowflake_Type") -> None:
         """
```

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/converters.py` & `discord-py-interactions-5.8.0/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/cooldowns.py` & `discord-py-interactions-5.8.0/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/extension.py` & `discord-py-interactions-5.8.0/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/listener.py` & `discord-py-interactions-5.8.0/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/localisation.py` & `discord-py-interactions-5.8.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/protocols.py` & `discord-py-interactions-5.8.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/tasks/task.py` & `discord-py-interactions-5.8.0/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/tasks/triggers.py` & `discord-py-interactions-5.8.0/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/internal/wait.py` & `discord-py-interactions-5.8.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/misc/context_manager.py` & `discord-py-interactions-5.8.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/interactions/models/misc/iterator.py` & `discord-py-interactions-5.8.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/pyproject.toml` & `discord-py-interactions-5.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.7.0"
+version = "5.8.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `discord-py-interactions-5.7.0/setup.py` & `discord-py-interactions-5.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "mkdocs-autorefs",
     "mkdocs-awesome-pages-plugin",
     "mkdocs-material",
     "mkdocstrings-python",
     "mkdocs-minify-plugin",
     "mkdocs-git-committers-plugin-2",
     "mkdocs-git-revision-date-localized-plugin",
+    "griffe==0.25",
 ]
 extras_require["tests"] = [
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "python-dotenv",
     "typeguard",
```

### Comparing `discord-py-interactions-5.7.0/tests/consts.py` & `discord-py-interactions-5.8.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/tests/test_bot.py` & `discord-py-interactions-5.8.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/tests/test_cache.py` & `discord-py-interactions-5.8.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/tests/test_contexts.py` & `discord-py-interactions-5.8.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/tests/test_cooldowns.py` & `discord-py-interactions-5.8.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/tests/test_emoji.py` & `discord-py-interactions-5.8.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.7.0/tests/utils.py` & `discord-py-interactions-5.8.0/tests/utils.py`

 * *Files identical despite different names*

