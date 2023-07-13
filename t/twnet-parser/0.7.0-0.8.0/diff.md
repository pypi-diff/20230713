# Comparing `tmp/twnet_parser-0.7.0.tar.gz` & `tmp/twnet_parser-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twnet_parser-0.7.0.tar", last modified: Fri May 19 07:47:26 2023, max compression
+gzip compressed data, was "twnet_parser-0.8.0.tar", last modified: Thu Jul 13 11:02:21 2023, max compression
```

## Comparing `twnet_parser-0.7.0.tar` & `twnet_parser-0.8.0.tar`

### file list

```diff
@@ -1,152 +1,246 @@
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.7.0/LICENSE.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6415 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5682 2023-05-13 14:22:02.000000 twnet_parser-0.7.0/README.md
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/examples/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/examples/download_map/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     4656 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/examples/download_map/download_map.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/examples/print_pcap_files/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      681 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/examples/print_pcap_files/print_pcap_files.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.7.0/pyproject.toml
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/scripts/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)    46929 2023-05-19 07:45:51.000000 twnet_parser-0.7.0/scripts/generate_messages.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/setup.cfg
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/tests/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.7.0/tests/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.7.0/tests/control_packets7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)    14284 2023-04-30 11:05:38.000000 twnet_parser-0.7.0/tests/ctrl_packets_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-05-09 13:53:12.000000 twnet_parser-0.7.0/tests/int_packer_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.7.0/tests/invalid_packet_header7_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/tests/msg7/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.7.0/tests/msg7/sv_tune_params_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.7.0/tests/packet_header6_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9816 2023-05-09 18:37:49.000000 twnet_parser-0.7.0/tests/packet_header7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.7.0/tests/packet_invalid_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.7.0/tests/packet_with_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.7.0/tests/repack_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7972 2023-05-10 09:03:48.000000 twnet_parser-0.7.0/tests/unpacker_state_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/twnet_parser/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1717 2023-05-07 12:05:43.000000 twnet_parser-0.7.0/twnet_parser/chunk_header.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      278 2023-05-09 10:04:55.000000 twnet_parser-0.7.0/twnet_parser/connless_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       98 2023-05-09 15:59:50.000000 twnet_parser-0.7.0/twnet_parser/constants.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      302 2023-05-09 09:32:18.000000 twnet_parser-0.7.0/twnet_parser/ctrl_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2807 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/enum7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/twnet_parser/external/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/external/huffman.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      322 2023-05-10 09:59:05.000000 twnet_parser-0.7.0/twnet_parser/master_server.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/message_parser.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/twnet_parser/messages7/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.119950 twnet_parser-0.7.0/twnet_parser/messages7/connless/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      882 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/count.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_check.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_error.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      641 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_ok.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      651 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_response.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      903 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/heartbeat.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2810 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      997 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/list.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/request_count.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/request_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      644 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/connless/request_list.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.119950 twnet_parser-0.7.0/twnet_parser/messages7/control/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      448 2023-05-09 09:39:14.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/accept.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      946 2023-05-09 09:39:20.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/close.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      732 2023-05-09 09:39:30.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/connect.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      455 2023-05-09 09:39:40.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/keep_alive.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      839 2023-05-09 09:39:50.000000 twnet_parser-0.7.0/twnet_parser/messages7/control/token.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.123283 twnet_parser-0.7.0/twnet_parser/messages7/game/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1523 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_call_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1221 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_command.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      779 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_kill.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      794 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_ready_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1403 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_say.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1301 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1087 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1875 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2322 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_start_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1007 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/cl_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1426 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1382 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_leave.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1039 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_broadcast.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1576 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_chat.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1019 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_checkpoint.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1382 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_drop.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2987 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1416 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1067 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1266 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1093 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_extra_projectile.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1732 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1479 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_kill_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1029 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_motd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1695 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_race_finish.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      796 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_ready_to_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1907 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_server_settings.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2032 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1566 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7704 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_tune_params.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      805 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_clear_options.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1094 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      808 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1100 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1758 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_set.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1411 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_status.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1106 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/game/sv_weapon_pickup.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.123283 twnet_parser-0.7.0/twnet_parser/messages7/system/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      783 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/con_ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/enter_game.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1422 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1555 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/input.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1230 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/input_timing.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1906 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/map_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      968 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1035 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1035 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      775 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/ping.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/ping_reply.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1040 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      791 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_off.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      789 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_on.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1013 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1315 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1025 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_line.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      777 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      797 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/request_map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      974 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/server_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2021 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/snap.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1175 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/snap_empty.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1658 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/messages7/system/snap_single.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2304 2023-05-12 15:10:15.000000 twnet_parser-0.7.0/twnet_parser/msg7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.123283 twnet_parser-0.7.0/twnet_parser/msg_matcher/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2525 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/connless7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-05-19 07:45:11.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/control7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/game7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-05-19 07:45:53.000000 twnet_parser-0.7.0/twnet_parser/msg_matcher/system7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      348 2023-05-09 09:36:25.000000 twnet_parser-0.7.0/twnet_parser/net_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6333 2023-05-10 10:14:10.000000 twnet_parser-0.7.0/twnet_parser/packer.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)    10665 2023-05-10 10:30:42.000000 twnet_parser-0.7.0/twnet_parser/packet.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.7.0/twnet_parser/pretty_print.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      742 2023-05-19 07:17:02.000000 twnet_parser-0.7.0/twnet_parser/snapshot7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.116617 twnet_parser-0.7.0/twnet_parser.egg-info/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6415 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5026 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/SOURCES.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/dependency_links.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-05-19 07:47:26.000000 twnet_parser-0.7.0/twnet_parser.egg-info/top_level.txt
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.113284 twnet_parser-0.7.0/venv/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-19 07:47:26.126617 twnet_parser-0.7.0/venv/bin/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2html.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2man.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-05-07 10:41:18.000000 twnet_parser-0.7.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.639378 twnet_parser-0.8.0/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/LICENSE.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7403 2023-07-13 11:02:21.639378 twnet_parser-0.8.0/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6670 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/README.md
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/examples/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/examples/07/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/examples/07/download_map/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     4656 2023-06-25 09:37:03.000000 twnet_parser-0.8.0/examples/07/download_map/download_map.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/examples/07/flood/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     5118 2023-07-13 09:17:46.000000 twnet_parser-0.8.0/examples/07/flood/flood.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/examples/07/print_pcap_files/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      681 2023-05-18 06:41:21.000000 twnet_parser-0.8.0/examples/07/print_pcap_files/print_pcap_files.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/pyproject.toml
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-07-13 11:02:21.639378 twnet_parser-0.8.0/setup.cfg
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.615378 twnet_parser-0.8.0/twnet_parser/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1717 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/chunk_header.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      278 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/connless_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       98 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/constants.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      302 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/ctrl_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      851 2023-07-13 10:29:57.000000 twnet_parser-0.8.0/twnet_parser/ddnet_uuid.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1949 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/enum6.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2840 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/enum7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.615378 twnet_parser-0.8.0/twnet_parser/external/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/external/huffman.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      584 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/huffman.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      322 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/master_server.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1094 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/message_parser.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/twnet_parser/messages6/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.615378 twnet_parser-0.8.0/twnet_parser/messages6/connless/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      882 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/count.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_check.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_error.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      641 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_ok.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      651 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_response.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      903 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/heartbeat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2522 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      997 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/list.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/request_count.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/request_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      644 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/connless/request_list.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.619378 twnet_parser-0.8.0/twnet_parser/messages6/control/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      448 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/control/accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      921 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/control/close.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      870 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/control/connect.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      726 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/control/connect_accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      455 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/control/keep_alive.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      839 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/control/token.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.619378 twnet_parser-0.8.0/twnet_parser/messages6/game/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1365 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_call_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2038 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_change_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      779 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_kill.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1205 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_say.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1073 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_set_spectator_mode.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1087 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_set_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2036 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_start_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1007 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/cl_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1039 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_broadcast.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1363 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_chat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1266 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1188 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_extra_projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1479 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_kill_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1029 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_motd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      796 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_ready_to_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1114 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_sound_global.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7903 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      805 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_clear_options.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1094 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_option_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1437 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_option_list_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1100 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_option_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1399 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_set.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1411 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1106 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/game/sv_weapon_pickup.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.623378 twnet_parser-0.8.0/twnet_parser/messages6/system/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      783 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/con_ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/enter_game.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1260 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1687 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1229 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/input_timing.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1290 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/map_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1627 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      775 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/ping.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/ping_reply.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1474 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/rcon_auth.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1385 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/rcon_auth_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1013 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/rcon_cmd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1315 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/rcon_cmd_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1031 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/rcon_cmd_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/rcon_line.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      777 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1030 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/request_map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2021 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/snap.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1175 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/snap_empty.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1658 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages6/system/snap_single.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.611379 twnet_parser-0.8.0/twnet_parser/messages7/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.623378 twnet_parser-0.8.0/twnet_parser/messages7/connless/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      882 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/count.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/forward_check.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/forward_error.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      641 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/forward_ok.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      651 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/forward_response.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      903 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/heartbeat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2810 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      997 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/list.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      645 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/request_count.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/request_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      644 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/connless/request_list.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.623378 twnet_parser-0.8.0/twnet_parser/messages7/control/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      448 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/messages7/control/accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      921 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/messages7/control/close.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      732 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/messages7/control/connect.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      455 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/messages7/control/keep_alive.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      839 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/messages7/control/token.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.627378 twnet_parser-0.8.0/twnet_parser/messages7/game/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1523 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_call_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1221 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_command.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      779 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_kill.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      794 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_ready_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1403 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_say.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1301 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1087 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_set_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1875 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2322 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_start_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1007 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/cl_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1426 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/de_client_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1382 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/de_client_leave.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1039 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_broadcast.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1576 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_chat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1019 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_checkpoint.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1382 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_client_drop.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2987 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1416 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_command_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1067 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_command_info_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1266 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1188 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_extra_projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1732 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_game_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1479 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_kill_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1029 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_motd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1695 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_race_finish.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      796 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_ready_to_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1907 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_server_settings.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2032 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1566 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7704 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      805 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_clear_options.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1094 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_option_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      808 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1100 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_option_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1758 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_set.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1411 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1106 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/game/sv_weapon_pickup.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.631378 twnet_parser-0.8.0/twnet_parser/messages7/system/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      783 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/con_ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/enter_game.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1520 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1687 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1230 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/input_timing.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1906 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/map_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      968 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1035 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/maplist_entry_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1035 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/maplist_entry_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      775 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/ping.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      786 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/ping_reply.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1040 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_auth.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      791 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_auth_off.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      789 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_auth_on.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1013 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_cmd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1315 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_cmd_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1025 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_cmd_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_line.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      777 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      797 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/request_map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      974 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/server_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2021 2023-05-15 08:55:36.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/snap.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1175 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/snap_empty.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1658 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/messages7/system/snap_single.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1953 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/msg6.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2337 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/msg7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.631378 twnet_parser-0.8.0/twnet_parser/msg_matcher/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2525 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/connless6.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2525 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/connless7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1133 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/control6.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/control7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5234 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/game6.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7872 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/game7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4023 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/system6.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4779 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/msg_matcher/system7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      348 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/net_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6665 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/packer.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)    17319 2023-06-25 09:37:08.000000 twnet_parser-0.8.0/twnet_parser/packet.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-05-13 07:34:38.000000 twnet_parser-0.8.0/twnet_parser/pretty_print.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.635378 twnet_parser-0.8.0/twnet_parser/snap6/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1791 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/character.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2782 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/character_core.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2030 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      852 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/common.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      762 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/damage_ind.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      773 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/death.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      528 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/explosion.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      979 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/flag.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1370 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/game_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2003 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      529 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/hammer_hit.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1295 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/laser.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1130 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/pickup.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1410 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/player_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2168 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/player_input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1500 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      854 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/sound_global.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      852 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/sound_world.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      520 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/spawn.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1039 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap6/spectator_info.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.635378 twnet_parser-0.8.0/twnet_parser/snap7/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1835 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/character.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2782 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/character_core.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      852 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/common.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1409 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/damage.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2885 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/de_client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1476 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/de_game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1018 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/de_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      773 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/death.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      528 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/explosion.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      979 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/flag.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1231 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/game_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1429 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/game_data_flag.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1131 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/game_data_race.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      990 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/game_data_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      529 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/hammer_hit.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1295 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/laser.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1056 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/pickup.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1106 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/player_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      823 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/player_info_race.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2213 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/player_input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1500 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      852 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/sound_world.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      520 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/spawn.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1267 2023-07-13 10:36:10.000000 twnet_parser-0.8.0/twnet_parser/snap7/spectator_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      742 2023-05-15 08:55:38.000000 twnet_parser-0.8.0/twnet_parser/snapshot7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-07-13 11:02:21.615378 twnet_parser-0.8.0/twnet_parser.egg-info/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7403 2023-07-13 11:02:21.000000 twnet_parser-0.8.0/twnet_parser.egg-info/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     8857 2023-07-13 11:02:21.000000 twnet_parser-0.8.0/twnet_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-07-13 11:02:21.000000 twnet_parser-0.8.0/twnet_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-07-13 11:02:21.000000 twnet_parser-0.8.0/twnet_parser.egg-info/top_level.txt
```

### Comparing `twnet_parser-0.7.0/LICENSE.txt` & `twnet_parser-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/PKG-INFO` & `twnet_parser-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: twnet_parser
-Version: 0.7.0
-Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
-Home-page: https://gitlab.com/teeworlds-network/twnet_parser
-Author: ChillerDragon
-Author-email: chillerdragon@gmail.com
-License: BSD-2.0
-Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
-Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 
 # THIS LIBRARY IS IN EARLY DEVELOPMENT
 
 ## Do not get bamboozled by the mature looking readme!
 ## This project is not in a very usable state yet. It is in very early development!
 ## APIs might change and many essential features are missing!
@@ -44,24 +27,24 @@
     print(msg.message_name) # => close
 ```
 
 ## Features
 
 | Feature                      | 0.7                | 0.6                |
 | ---------------------------- | ------------------ | ------------------ |
-| Deserialize packet headers   | :heavy_check_mark: |                    |
-| Deserialize chunk headers    | :heavy_check_mark: |                    |
-| Deserialize messages         | 85%                |                    |
+| Deserialize packet headers   | :heavy_check_mark: | :heavy_check_mark: |
+| Deserialize chunk headers    | :heavy_check_mark: | :heavy_check_mark: |
+| Deserialize messages         | 90%                | 90%                |
 | Deserialize snapshots        |                    |                    |
-| Deserialize connless packets | :heavy_check_mark: |                    |
-| Serialize packet headers     | :heavy_check_mark: |                    |
-| Serialize chunk headers      | :heavy_check_mark: |                    |
-| Serialize messages           | 85%                |                    |
+| Deserialize connless packets | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize packet headers     | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize chunk headers      | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize messages           | 90%                | 90%                |
 | Serialize snapshots          |                    |                    |
-| Serialize connless packets   | :heavy_check_mark: |                    |
+| Serialize connless packets   | :heavy_check_mark: | :heavy_check_mark: |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
@@ -138,22 +121,46 @@
 msg.value = 'test'
 msg.reason = ''
 msg.force = False
 packet.messages.append(msg)
 packet.pack() # => b'\x02~\x06H\x1f\x93\xd7\x00\x00\x80\x01option\x00test\x00\x00\x00'
 ```
 
+## Zero dependencies by default
+
+Running ``pip install twnet_parser`` will not install any additional packages.
+
+But there is an optional dependency for huffman compression.
+By default twnet_parser is using the huffman compression code from the [TeeAI](https://github.com/edg-l/TeeAI)
+project which is written in pure python.
+If you have [libtw2-huffman](https://pypi.org/project/libtw2-huffman/) installed it will use that one instead.
+Because it is faster since it is written in rust and has better error handling.
+But since it is so much overhead it is not installed by default to keep twnet_parser light weight.
+
+
+You can install it by running ``pip install libtw2-huffman``
+or by running ``pip install -r requirements/optional.txt``
+
+
+You can also check which huffman backend is currently active with these lines of code
+
+```python
+import twnet_parser.huffman
+print(twnet_parser.huffman.backend_name()) # => rust-libtw2 or python-TeeAI
+```
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
 pip install -r requirements/dev.txt
+pre-commit install --hook-type commit-msg
 ```
 
 ## tests and linting
 
 ```bash
 # dev dependencies
 pip install -r requirements/dev.txt
```

### Comparing `twnet_parser-0.7.0/README.md` & `twnet_parser-0.8.0/twnet_parser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: twnet-parser
+Version: 0.8.0
+Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
+Home-page: https://gitlab.com/teeworlds-network/twnet_parser
+Author: ChillerDragon
+Author-email: chillerdragon@gmail.com
+License: BSD-2.0
+Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
+Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 
 # THIS LIBRARY IS IN EARLY DEVELOPMENT
 
 ## Do not get bamboozled by the mature looking readme!
 ## This project is not in a very usable state yet. It is in very early development!
 ## APIs might change and many essential features are missing!
@@ -27,24 +44,24 @@
     print(msg.message_name) # => close
 ```
 
 ## Features
 
 | Feature                      | 0.7                | 0.6                |
 | ---------------------------- | ------------------ | ------------------ |
-| Deserialize packet headers   | :heavy_check_mark: |                    |
-| Deserialize chunk headers    | :heavy_check_mark: |                    |
-| Deserialize messages         | 85%                |                    |
+| Deserialize packet headers   | :heavy_check_mark: | :heavy_check_mark: |
+| Deserialize chunk headers    | :heavy_check_mark: | :heavy_check_mark: |
+| Deserialize messages         | 90%                | 90%                |
 | Deserialize snapshots        |                    |                    |
-| Deserialize connless packets | :heavy_check_mark: |                    |
-| Serialize packet headers     | :heavy_check_mark: |                    |
-| Serialize chunk headers      | :heavy_check_mark: |                    |
-| Serialize messages           | 85%                |                    |
+| Deserialize connless packets | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize packet headers     | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize chunk headers      | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize messages           | 90%                | 90%                |
 | Serialize snapshots          |                    |                    |
-| Serialize connless packets   | :heavy_check_mark: |                    |
+| Serialize connless packets   | :heavy_check_mark: | :heavy_check_mark: |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
@@ -121,22 +138,46 @@
 msg.value = 'test'
 msg.reason = ''
 msg.force = False
 packet.messages.append(msg)
 packet.pack() # => b'\x02~\x06H\x1f\x93\xd7\x00\x00\x80\x01option\x00test\x00\x00\x00'
 ```
 
+## Zero dependencies by default
+
+Running ``pip install twnet_parser`` will not install any additional packages.
+
+But there is an optional dependency for huffman compression.
+By default twnet_parser is using the huffman compression code from the [TeeAI](https://github.com/edg-l/TeeAI)
+project which is written in pure python.
+If you have [libtw2-huffman](https://pypi.org/project/libtw2-huffman/) installed it will use that one instead.
+Because it is faster since it is written in rust and has better error handling.
+But since it is so much overhead it is not installed by default to keep twnet_parser light weight.
+
+
+You can install it by running ``pip install libtw2-huffman``
+or by running ``pip install -r requirements/optional.txt``
+
+
+You can also check which huffman backend is currently active with these lines of code
+
+```python
+import twnet_parser.huffman
+print(twnet_parser.huffman.backend_name()) # => rust-libtw2 or python-TeeAI
+```
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
 pip install -r requirements/dev.txt
+pre-commit install --hook-type commit-msg
 ```
 
 ## tests and linting
 
 ```bash
 # dev dependencies
 pip install -r requirements/dev.txt
```

### Comparing `twnet_parser-0.7.0/examples/download_map/download_map.py` & `twnet_parser-0.8.0/examples/07/download_map/download_map.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/examples/print_pcap_files/print_pcap_files.py` & `twnet_parser-0.8.0/examples/07/print_pcap_files/print_pcap_files.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/setup.cfg` & `twnet_parser-0.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twnet_parser
-version = 0.7.0
+version = 0.8.0
 author = ChillerDragon
 author_email = chillerdragon@gmail.com
 description = A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/teeworlds-network/twnet_parser
 license = BSD-2.0
```

### Comparing `twnet_parser-0.7.0/twnet_parser/chunk_header.py` & `twnet_parser-0.8.0/twnet_parser/chunk_header.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/enum7.py` & `twnet_parser-0.8.0/twnet_parser/enum7.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=duplicate-code
 from enum import Enum
 
 class Pickup(Enum):
     HEALTH: int = 0
     ARMOR: int = 1
     GRENADE: int = 2
     SHOTGUN: int = 3
```

### Comparing `twnet_parser-0.7.0/twnet_parser/external/huffman.py` & `twnet_parser-0.8.0/twnet_parser/external/huffman.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/message_parser.py` & `twnet_parser-0.8.0/twnet_parser/message_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,34 @@
+from typing import Literal
+
 from twnet_parser.net_message import NetMessage
 
 from twnet_parser.msg_matcher.game7 import match_game7
 from twnet_parser.msg_matcher.system7 import match_system7
 
+from twnet_parser.msg_matcher.game6 import match_game6
+from twnet_parser.msg_matcher.system6 import match_system6
+
 # could also be named ChunkParser
 class MessageParser():
     # the first byte of data has to be the
     # first byte of a message PAYLOAD
     # NOT the whole packet with packet header
     # and NOT the whole message with chunk header
-    def parse_game_message(self, msg_id: int, data: bytes) -> NetMessage:
+    def parse_game_message(
+            self,
+            version: Literal['0.6', '0.7'],
+            msg_id: int,
+            data: bytes
+    ) -> NetMessage:
+        if version == '0.6':
+            return match_game6(msg_id, data)
         return match_game7(msg_id, data)
-    def parse_sys_message(self, msg_id: int, data: bytes) -> NetMessage:
+    def parse_sys_message(
+            self,
+            version: Literal['0.6', '0.7'],
+            msg_id: int,
+            data: bytes
+    ) -> NetMessage:
+        if version == '0.6':
+            return match_system6(msg_id, data)
         return match_system7(msg_id, data)
```

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/count.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/count.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_check.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_check.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_error.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_error.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_ok.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_ok.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/forward_response.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/forward_response.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/heartbeat.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/heartbeat.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/info.py` & `twnet_parser-0.8.0/twnet_parser/messages7/connless/info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/list.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/list.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/request_count.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/request_count.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/request_info.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/request_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/connless/request_list.py` & `twnet_parser-0.8.0/twnet_parser/messages6/connless/request_list.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/control/close.py` & `twnet_parser-0.8.0/twnet_parser/messages6/control/close.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,14 @@
         self.reason: Optional[str] = reason
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes, we_are_a_client: bool = True) -> bool:
         unpacker = Unpacker(data)
-        self.reason = unpacker.get_str() # TODO: this is an optional field
+        self.reason = unpacker.get_optional_str()
         return True
 
     def pack(self, we_are_a_client: bool = True) -> bytes:
         if self.reason:
             return pack_str(self.reason)
         return b''
```

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/control/connect.py` & `twnet_parser-0.8.0/twnet_parser/messages7/control/connect.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/control/token.py` & `twnet_parser-0.8.0/twnet_parser/messages6/control/token.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_call_vote.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_call_vote.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_command.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_command.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_emoticon.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_emoticon.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_kill.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_kill.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_ready_change.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_ready_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_say.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_say.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_spectator_mode.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_set_spectator_mode.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_set_team.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_set_team.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_skin_change.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_skin_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_start_info.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_start_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/cl_vote.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/cl_vote.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_enter.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/de_client_enter.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/de_client_leave.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/de_client_leave.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_broadcast.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_broadcast.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_chat.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_chat.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_checkpoint.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_checkpoint.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_drop.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_client_drop.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_client_info.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_client_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_command_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_command_info_remove.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_command_info_remove.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_emoticon.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_emoticon.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_extra_projectile.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/cl_set_spectator_mode.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 from typing import Literal
 
-class MsgSvExtraProjectile(PrettyPrint):
+class MsgClSetSpectatorMode(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            projectile: int = 0
+            spectator_id: int = 0
     ) -> None:
         self.message_type: Literal['system', 'game'] = 'game'
-        self.message_name: str = 'sv_extra_projectile'
+        self.message_name: str = 'cl_set_spectator_mode'
         self.system_message: bool = False
-        self.message_id: int = 7
+        self.message_id: int = 19
         self.header: ChunkHeader = chunk_header
 
-        self.projectile: int = projectile
+        self.spectator_id: int = spectator_id
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.projectile = unpacker.get_int() # TODO: this is a snapshot object
+        self.spectator_id = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.projectile)
+        return pack_int(self.spectator_id)
```

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_info.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_game_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_game_msg.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_game_msg.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_kill_msg.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_kill_msg.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_motd.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_motd.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_race_finish.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_race_finish.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_ready_to_enter.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_ready_to_enter.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_server_settings.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_server_settings.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_skin_change.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_skin_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_team.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_team.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_tune_params.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_tune_params.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_clear_options.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_clear_options.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_add.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_option_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_list_add.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_option_list_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_option_remove.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_option_remove.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_set.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_vote_set.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_vote_status.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_vote_status.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/game/sv_weapon_pickup.py` & `twnet_parser-0.8.0/twnet_parser/messages7/game/sv_weapon_pickup.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/con_ready.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/con_ready.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/enter_game.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/enter_game.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/info.py` & `twnet_parser-0.8.0/twnet_parser/messages6/game/sv_chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 from typing import Literal
 
-class MsgInfo(PrettyPrint):
+class MsgSvChat(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            version: str = '0.7 802f1be60a05665f',
-            password: str = '',
-            client_version: int = 1797
+            team: bool = False,
+            client_id: int = 0,
+            message: str = 'default'
     ) -> None:
-        self.message_type: Literal['system', 'game'] = 'system'
-        self.message_name: str = 'info'
-        self.system_message: bool = True
-        self.message_id: int = 1
+        self.message_type: Literal['system', 'game'] = 'game'
+        self.message_name: str = 'sv_chat'
+        self.system_message: bool = False
+        self.message_id: int = 3
         self.header: ChunkHeader = chunk_header
 
-        self.version: str = version
-        self.password: str = password
-        self.client_version: int = client_version
+        self.team: bool = team
+        self.client_id: int = client_id
+        self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.version = unpacker.get_str()
-        self.password = unpacker.get_str() # TODO: optionals
-        self.client_version = unpacker.get_int() # TODO: optionals
+        self.team = unpacker.get_int() == 1
+        self.client_id = unpacker.get_int()
+        self.message = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.version) + \
-            pack_str(self.password) + \
-            pack_int(self.client_version)
+        return pack_int(self.team) + \
+            pack_int(self.client_id) + \
+            pack_str(self.message)
```

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/input.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
-from typing import Literal
+from typing import Literal, Optional
+from twnet_parser.snap7.player_input import ObjPlayerInput
 
 class MsgInput(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
             ack_snapshot: int = 0,
             intended_tick: int = 0,
             input_size: int = 0,
-            input: int = 0
+            input: Optional[ObjPlayerInput] = None
     ) -> None:
         self.message_type: Literal['system', 'game'] = 'system'
         self.message_name: str = 'input'
         self.system_message: bool = True
         self.message_id: int = 20
         self.header: ChunkHeader = chunk_header
 
         self.ack_snapshot: int = ack_snapshot
         self.intended_tick: int = intended_tick
         self.input_size: int = input_size
-        self.input: int = input
+        if not input:
+            input = ObjPlayerInput()
+        self.input: ObjPlayerInput = input
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.ack_snapshot = unpacker.get_int()
         self.intended_tick = unpacker.get_int()
         self.input_size = unpacker.get_int()
-        self.input = unpacker.get_int() # TODO: this is a snapshot object
+        self.input.unpack(unpacker.get_raw())
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.ack_snapshot) + \
             pack_int(self.intended_tick) + \
             pack_int(self.input_size) + \
-            pack_int(self.input)
+            self.input.pack()
```

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/input_timing.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/input_timing.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/map_change.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/map_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/map_data.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/map_data.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_add.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/maplist_entry_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/maplist_entry_rem.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/maplist_entry_rem.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/ping.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/ping.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/ping_reply.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/ping_reply.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_auth.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_off.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_auth_off.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_auth_on.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_auth_on.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_cmd.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_add.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_cmd_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_cmd_rem.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_cmd_rem.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/rcon_line.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/rcon_line.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/ready.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/ready.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/request_map_data.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/request_map_data.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/server_info.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/server_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/snap.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/snap.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/snap_empty.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/snap_empty.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/messages7/system/snap_single.py` & `twnet_parser-0.8.0/twnet_parser/messages7/system/snap_single.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/msg7.py` & `twnet_parser-0.8.0/twnet_parser/msg7.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # connless
+# pylint: disable=duplicate-code
 
 CONNLESS_HEARTBEAT = b'\xff\xff\xff\xffbea2'
 CONNLESS_REQUEST_LIST = b'\xff\xff\xff\xffreq2'
 CONNLESS_LIST = b'\xff\xff\xff\xfflis2'
 CONNLESS_REQUEST_COUNT = b'\xff\xff\xff\xffcou2'
 CONNLESS_COUNT = b'\xff\xff\xff\xffsiz2'
 CONNLESS_REQUEST_INFO = b'\xff\xff\xff\xffgie3'
```

### Comparing `twnet_parser-0.7.0/twnet_parser/msg_matcher/connless7.py` & `twnet_parser-0.8.0/twnet_parser/msg_matcher/connless7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/msg_matcher/control7.py` & `twnet_parser-0.8.0/twnet_parser/msg_matcher/control7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser/msg_matcher/game7.py` & `twnet_parser-0.8.0/twnet_parser/msg_matcher/game7.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # generated by scripts/generate_messages.py
 from typing import Optional
 
 import twnet_parser.msg7
 from twnet_parser.net_message import NetMessage
+from twnet_parser.ddnet_uuid import MsgDDNetUuid
 
 import twnet_parser.messages7.game.sv_motd as \
        game7_sv_motd
 import twnet_parser.messages7.game.sv_broadcast as \
        game7_sv_broadcast
 import twnet_parser.messages7.game.sv_chat as \
        game7_sv_chat
@@ -161,12 +162,16 @@
     elif msg_id == twnet_parser.msg7.SV_COMMAND_INFO:
         msg = game7_sv_command_info.MsgSvCommandInfo()
     elif msg_id == twnet_parser.msg7.SV_COMMAND_INFO_REMOVE:
         msg = game7_sv_command_info_remove.MsgSvCommandInfoRemove()
     elif msg_id == twnet_parser.msg7.CL_COMMAND:
         msg = game7_cl_command.MsgClCommand()
 
+    # msg_id 0 is used by ddnet uuid messages
+    # do not crash on those
     if msg is None:
-        raise ValueError(f"Error: unknown game message id={msg_id} data={data[0]}")
+        if msg_id != 0:
+            raise ValueError(f"Error: unknown game message id={msg_id} data={data[0]}")
+        msg = MsgDDNetUuid()
 
     msg.unpack(data)
     return msg
```

### Comparing `twnet_parser-0.7.0/twnet_parser/msg_matcher/system7.py` & `twnet_parser-0.8.0/twnet_parser/msg_matcher/system7.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # generated by scripts/generate_messages.py
 from typing import Optional
 
 import twnet_parser.msg7
 from twnet_parser.net_message import NetMessage
+from twnet_parser.ddnet_uuid import MsgDDNetUuid
 
 import twnet_parser.messages7.system.info as \
        system7_info
 import twnet_parser.messages7.system.map_change as \
        system7_map_change
 import twnet_parser.messages7.system.map_data as \
        system7_map_data
@@ -101,12 +102,16 @@
     elif msg_id == twnet_parser.msg7.PING_REPLY:
         msg = system7_ping_reply.MsgPingReply()
     elif msg_id == twnet_parser.msg7.MAPLIST_ENTRY_ADD:
         msg = system7_maplist_entry_add.MsgMaplistEntryAdd()
     elif msg_id == twnet_parser.msg7.MAPLIST_ENTRY_REM:
         msg = system7_maplist_entry_rem.MsgMaplistEntryRem()
 
+    # msg_id 0 is used by ddnet uuid messages
+    # do not crash on those
     if msg is None:
-        raise ValueError(f"Error: unknown system message id={msg_id} data={data[0]}")
+        if msg_id != 0:
+            raise ValueError(f"Error: unknown system message id={msg_id} data={data[0]}")
+        msg = MsgDDNetUuid()
 
     msg.unpack(data)
     return msg
```

### Comparing `twnet_parser-0.7.0/twnet_parser/packer.py` & `twnet_parser-0.8.0/twnet_parser/packer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-from typing import Final, Literal
+from typing import Final, Literal, Optional
 
 from twnet_parser.master_server import MastersrvAddr
 
 # Before chaning the current packer code to extend it
 # Consider having two packers
 #
 # One being this one. That is simple and fast.
@@ -67,14 +67,19 @@
     def get_be_uint16(self) -> int:
         left = self.byte()
         self.idx += 1
         right = self.byte()
         self.idx += 1
         return left << 8 | right
 
+    def get_optional_int(self) -> Optional[int]:
+        if self.idx >= len(self._data):
+            return None
+        return self.get_int()
+
     def get_int(self) -> int:
         sign = (self.byte() >> 6) & 1
         res = self.byte() & 0x3F
         # fake loop should only loop once
         # its the poor mans goto hack
         while True:
             if (self.byte() & 0x80) == 0:
@@ -98,14 +103,19 @@
             res |= (self.byte() & 0x7F) << (6 + 7 + 7 + 7)
             break
 
         self.idx += 1
         res ^= -sign
         return res
 
+    def get_optional_str(self, sanitize: int = SANITIZE) -> Optional[str]:
+        if self.idx >= len(self._data):
+            return None
+        return self.get_str(sanitize)
+
     # TODO: optimize performance
     #       I am highly confident iterating byte by byte is very
     #       expensive in python
     #       and something common as byte filtering has to have
     #       a fast alternative
     #
     #       If there is nothing from the python standard
```

### Comparing `twnet_parser-0.7.0/twnet_parser/packet.py` & `twnet_parser-0.8.0/twnet_parser/packet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 #!/usr/bin/env python
 
-from typing import Union, cast, Optional
+from typing import Union, cast, Optional, Literal
 
 from twnet_parser.packer import Unpacker, pack_int
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.message_parser import MessageParser
 from twnet_parser.net_message import NetMessage
 from twnet_parser.ctrl_message import CtrlMessage
 from twnet_parser.connless_message import ConnlessMessage
 from twnet_parser.chunk_header import ChunkHeader, ChunkFlags
 from twnet_parser.msg_matcher.control7 import match_control7
 from twnet_parser.msg_matcher.connless7 import match_connless7
+from twnet_parser.msg_matcher.control6 import match_control6
+from twnet_parser.msg_matcher.connless6 import match_connless6
 from twnet_parser.constants import NET_MAX_SEQUENCE, NET_PACKETVERSION
 
-from twnet_parser.external.huffman import huffman
+import twnet_parser.huffman
 
 # TODO: what is a nice pythonic way of storing those?
 #       also does some version:: namespace thing make sense?
 PACKETFLAG7_CONTROL = 1
 PACKETFLAG7_RESEND = 2
 PACKETFLAG7_COMPRESSION = 4
 PACKETFLAG7_CONNLESS = 8
 
+PACKETFLAG6_UNUSED = 1
+PACKETFLAG6_TOKEN = 2
+PACKETFLAG6_CONTROL = 4
+PACKETFLAG6_CONNLESS = 8
+PACKETFLAG6_RESEND = 16
+PACKETFLAG6_COMPRESSION = 32
+
 CHUNKFLAG7_VITAL = 1
 CHUNKFLAG7_RESEND = 2
 
 PACKET_HEADER7_SIZE = 7
 CONNLESS_PACKET_HEADER7_SIZE = 9
+CONNLESS_PACKET_HEADER6_SIZE = 6
 
 class PacketFlags7(PrettyPrint):
     def __init__(self) -> None:
         self.control: Optional[bool] = None
         self.resend: Optional[bool] = None
         self.compression: Optional[bool] = None
         self.connless: Optional[bool] = None
@@ -39,14 +49,87 @@
     def __init__(self) -> None:
         self.token: Optional[bool] = None
         self.control: Optional[bool] = None
         self.resend: Optional[bool] = None
         self.compression: Optional[bool] = None
         self.connless: Optional[bool] = None
 
+class PacketHeader6(PrettyPrint):
+    def __init__(
+            self,
+            flags: Optional[PacketFlags6] = None,
+            ack: int = 0,
+            token: bytes = b'\xff\xff\xff\xff',
+            num_chunks: Optional[int] = None
+    ) -> None:
+        """
+        If num_chunks is not set it will count
+        the messages it was given when
+        the pack() method is called
+        """
+        if not flags:
+            flags = PacketFlags6()
+        self.flags: PacketFlags6 = flags
+        self.ack: int = ack % NET_MAX_SEQUENCE
+        self.token: bytes = token
+        self.num_chunks: Optional[int] = num_chunks
+
+        # connless only
+        self.connless_version: int = NET_PACKETVERSION
+        self.response_token: bytes = b'\xff\xff\xff\xff'
+
+    def pack(self) -> bytes:
+        """
+        Generate 7 byte teeworlds 0.6.5 packet header
+        based on the current instance variable
+        values.
+
+        The layout is as follows
+        6bit flags, 2bit ack
+        8bit ack
+        8bit chunks
+        32bit token
+
+        ffffffaa
+        aaaaaaaa
+        NNNNNNNN
+        TTTTTTTT
+        TTTTTTTT
+        TTTTTTTT
+        TTTTTTTT
+        """
+        flags = 0
+        if self.flags.token is None:
+            # do not automatically set the token flag
+            # if the token field has the empty token value
+            if self.token != b'\xff\xff\xff\xff':
+                self.flags.token = True
+        if self.flags.token:
+            flags |= PACKETFLAG6_TOKEN
+        if self.flags.control:
+            flags |= PACKETFLAG6_CONTROL
+        if self.flags.connless:
+            flags |= PACKETFLAG6_CONNLESS
+        if self.flags.resend:
+            flags |= PACKETFLAG6_RESEND
+        if self.flags.compression:
+            flags |= PACKETFLAG6_COMPRESSION
+        if self.num_chunks is None:
+            self.num_chunks = 0
+        if self.flags.connless:
+            return b'\xff\xff\xff\xff\xff\xff'
+        packed = bytes([ \
+            ((flags << 2)&0xfc) | ((self.ack>>8)&0x03), \
+            self.ack&0xff, \
+            self.num_chunks \
+        ])
+        if self.flags.token:
+            packed += self.token
+        return packed
+
 class PacketHeader(PrettyPrint):
     def __init__(
             self,
             flags: Optional[PacketFlags7] = None,
             ack: int = 0,
             token: bytes = b'\xff\xff\xff\xff',
             num_chunks: Optional[int] = None
@@ -105,21 +188,31 @@
         return bytes([ \
             ((flags << 2)&0xfc) | ((self.ack>>8)&0x03), \
             self.ack&0xff, \
             self.num_chunks \
         ]) + self.token
 
 class TwPacket(PrettyPrint):
-    def __init__(self) -> None:
-        self.version: str = 'unknown'
+    def __init__(self, version: Literal['0.6', '0.7']= '0.7') -> None:
+        self._version: Literal['0.6', '0.7'] = version
         self.payload_raw: bytes = b''
         self.payload_decompressed: bytes = b''
-        self.header: PacketHeader = PacketHeader()
+        self.header: Union[PacketHeader, PacketHeader6]
+        if self.version == '0.6':
+            self.header = PacketHeader6()
+        elif self.version == '0.7':
+            self.header = PacketHeader()
+        else:
+            raise ValueError(f"Error: invalid packet version '{self.version}'")
         self.messages: list[Union[CtrlMessage, NetMessage, ConnlessMessage]] = []
 
+    @property
+    def version(self) -> Literal['0.6', '0.7']:
+        return self._version
+
     def pack(self, we_are_a_client = True) -> bytes:
         payload: bytes = b''
         msg: Union[CtrlMessage, NetMessage, ConnlessMessage]
         is_control: bool = False
         is_connless: bool = False
         for msg in self.messages:
             if msg.message_type == 'connless':
@@ -150,16 +243,69 @@
                 self.header.num_chunks = len(self.messages)
         if is_control:
             if self.header.flags.control is None:
                 self.header.flags.control = True
         if is_connless:
             if self.header.flags.connless is None:
                 self.header.flags.connless = True
+        if self.header.flags.compression:
+            payload = twnet_parser.huffman.compress(payload)
         return self.header.pack() + payload
 
+class PacketHeaderParser6():
+    def parse_flags6(self, data: bytes) -> PacketFlags6:
+        # FFFF FFaa
+        flag_bits = data[0] >> 2
+        flags = PacketFlags6()
+        flags.token = (flag_bits & PACKETFLAG6_TOKEN) != 0
+        flags.control = (flag_bits & PACKETFLAG6_CONTROL) != 0
+        flags.connless = (flag_bits & PACKETFLAG6_CONNLESS) != 0
+        flags.resend = (flag_bits & PACKETFLAG6_RESEND) != 0
+        flags.compression = (flag_bits & PACKETFLAG6_COMPRESSION) != 0
+        if flags.connless:
+            # conless packets send FF
+            # as the flag byte
+            # but setting the connless bit basically means
+            # all other flags are false implicitly
+            flags.token = False
+            flags.control = False
+            flags.resend = False
+            flags.compression = False
+        return flags
+
+    def parse_ack(self, header_bytes: bytes) -> int:
+        # ffAA AAAA AAAA
+        return ((header_bytes[0] & 0x3) << 8) | header_bytes[1]
+
+    def parse_num_chunks(self, header_bytes: bytes) -> int:
+        # TODO: not sure if this is correct
+        return header_bytes[2]
+
+    def parse_token(self, header_bytes: bytes) -> bytes:
+        return header_bytes[3:7]
+
+    def parse_header(self, data: bytes) -> PacketHeader6:
+        header = PacketHeader6()
+        # bits 1..5
+        header.flags = self.parse_flags6(data)
+        if header.flags.connless:
+            # TODO: do not hardcode version field
+            #       but actually read the bits
+            header.connless_version = NET_PACKETVERSION
+            header.token = data[1:5]
+            header.response_token = data[5:9]
+        else:
+            # bits 6..16
+            header.ack = self.parse_ack(data)
+            # bits 17..25
+            header.num_chunks = self.parse_num_chunks(data)
+            # bits 16..57
+            header.token = self.parse_token(data)
+        return header
+
 class PacketHeaderParser7():
     def parse_flags7(self, data: bytes) -> PacketFlags7:
         # FFFF FFaa
         flag_bits = (data[0] & 0xfc) >> 2
         flags = PacketFlags7()
         flags.control = (flag_bits & PACKETFLAG7_CONTROL) != 0
         flags.resend = (flag_bits & PACKETFLAG7_RESEND) != 0
@@ -215,14 +361,17 @@
         header.size = ((data[0] & 0x3F) << 6) | (data[1] & 0x3F)
         if header.flags.vital:
             # ffss ssss  XXss ssss
             header.seq = ((data[1] & 0xC0) << 2) | data[2]
         return header
 
 class PacketParser():
+    def __init__(self) -> None:
+        self.version: Literal['0.6', '0.7'] = '0.7'
+
     # the first byte of data has to be the
     # first byte of a message chunk
     # NOT the whole packet with packet header
     def get_messages(self, data: bytes) -> list[NetMessage]:
         messages: list[NetMessage] = []
         i = 0
         while i < len(data):
@@ -246,47 +395,78 @@
         unpacker = Unpacker(data[i:])
         msg_id: int = unpacker.get_int()
         i += 1
         sys: bool = (msg_id & 1) == 1
         msg_id >>= 1
         msg: NetMessage
         if sys:
-            msg = MessageParser().parse_sys_message(msg_id, unpacker.get_raw())
+            msg = MessageParser().parse_sys_message(self.version, msg_id, unpacker.get_raw())
         else:
-            msg = MessageParser().parse_game_message(msg_id, unpacker.get_raw())
+            msg = MessageParser().parse_game_message(self.version, msg_id, unpacker.get_raw())
         msg.header = chunk_header
         return msg
 
+    def parse6(self, data: bytes, client: bool) -> TwPacket:
+        pck = TwPacket(version = '0.6')
+        self.version = '0.6'
+        # TODO: what is the most performant way in python to do this?
+        #       heap allocating a PacketHeaderParser7 just to bundle a bunch of
+        #       methods that do not share state seems like a waste of performance
+        #       would this be nicer with class methods?
+        pck.header = PacketHeaderParser6().parse_header(data)
+        header_size = PACKET_HEADER7_SIZE
+        if pck.header.flags.connless:
+            header_size = CONNLESS_PACKET_HEADER6_SIZE
+        elif not pck.header.flags.token:
+            header_size = 3
+        pck.payload_raw = data[header_size:]
+        pck.payload_decompressed = pck.payload_raw
+        if pck.header.flags.control:
+            ctrl_msg: CtrlMessage = match_control6(data[header_size], data[header_size+1:], client)
+            pck.messages.append(ctrl_msg)
+            return pck
+        if pck.header.flags.connless:
+            connless_msg: ConnlessMessage = match_connless6(data[header_size:14], data[14:])
+            pck.messages.append(connless_msg)
+            return pck
+        if pck.header.flags.compression:
+            payload = bytearray(pck.payload_raw)
+            pck.payload_decompressed = twnet_parser.huffman.decompress(payload)
+        pck.messages = cast(
+                list[Union[CtrlMessage, NetMessage, ConnlessMessage]],
+                self.get_messages(pck.payload_decompressed))
+        return pck
+
     def parse7(self, data: bytes, client: bool) -> TwPacket:
-        pck = TwPacket()
-        pck.version = '0.7'
+        pck = TwPacket(version = '0.7')
+        self.version = '0.7'
         # TODO: what is the most performant way in python to do this?
         #       heap allocating a PacketHeaderParser7 just to bundle a bunch of
         #       methods that do not share state seems like a waste of performance
         #       would this be nicer with class methods?
         pck.header = PacketHeaderParser7().parse_header(data)
         header_size = PACKET_HEADER7_SIZE
         if pck.header.flags.connless:
             header_size = CONNLESS_PACKET_HEADER7_SIZE
         pck.payload_raw = data[header_size:]
         pck.payload_decompressed = pck.payload_raw
         if pck.header.flags.control:
-            ctrl_msg: CtrlMessage = match_control7(data[7], data[8:], client)
+            ctrl_msg: CtrlMessage = match_control7(data[header_size], data[8:], client)
             pck.messages.append(ctrl_msg)
             return pck
         if pck.header.flags.connless:
-            connless_msg: ConnlessMessage = match_connless7(data[9:17], data[17:])
+            connless_msg: ConnlessMessage = match_connless7(data[header_size:17], data[17:])
             pck.messages.append(connless_msg)
             return pck
         if pck.header.flags.compression:
             payload = bytearray(pck.payload_raw)
-            pck.payload_decompressed = huffman.decompress(payload)
+            pck.payload_decompressed = twnet_parser.huffman.decompress(payload)
         pck.messages = cast(
                 list[Union[CtrlMessage, NetMessage, ConnlessMessage]],
                 self.get_messages(pck.payload_decompressed))
         return pck
 
-def parse6(data: bytes) -> TwPacket:
-    raise NotImplementedError()
+def parse6(data: bytes, we_are_a_client: bool = True) -> TwPacket:
+    return PacketParser().parse6(data, we_are_a_client)
 
 def parse7(data: bytes, we_are_a_client: bool = True) -> TwPacket:
     return PacketParser().parse7(data, we_are_a_client)
```

### Comparing `twnet_parser-0.7.0/twnet_parser/snapshot7.py` & `twnet_parser-0.8.0/twnet_parser/snapshot7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.7.0/twnet_parser.egg-info/PKG-INFO` & `twnet_parser-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: twnet-parser
-Version: 0.7.0
+Name: twnet_parser
+Version: 0.8.0
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -44,24 +44,24 @@
     print(msg.message_name) # => close
 ```
 
 ## Features
 
 | Feature                      | 0.7                | 0.6                |
 | ---------------------------- | ------------------ | ------------------ |
-| Deserialize packet headers   | :heavy_check_mark: |                    |
-| Deserialize chunk headers    | :heavy_check_mark: |                    |
-| Deserialize messages         | 85%                |                    |
+| Deserialize packet headers   | :heavy_check_mark: | :heavy_check_mark: |
+| Deserialize chunk headers    | :heavy_check_mark: | :heavy_check_mark: |
+| Deserialize messages         | 90%                | 90%                |
 | Deserialize snapshots        |                    |                    |
-| Deserialize connless packets | :heavy_check_mark: |                    |
-| Serialize packet headers     | :heavy_check_mark: |                    |
-| Serialize chunk headers      | :heavy_check_mark: |                    |
-| Serialize messages           | 85%                |                    |
+| Deserialize connless packets | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize packet headers     | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize chunk headers      | :heavy_check_mark: | :heavy_check_mark: |
+| Serialize messages           | 90%                | 90%                |
 | Serialize snapshots          |                    |                    |
-| Serialize connless packets   | :heavy_check_mark: |                    |
+| Serialize connless packets   | :heavy_check_mark: | :heavy_check_mark: |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
@@ -138,22 +138,46 @@
 msg.value = 'test'
 msg.reason = ''
 msg.force = False
 packet.messages.append(msg)
 packet.pack() # => b'\x02~\x06H\x1f\x93\xd7\x00\x00\x80\x01option\x00test\x00\x00\x00'
 ```
 
+## Zero dependencies by default
+
+Running ``pip install twnet_parser`` will not install any additional packages.
+
+But there is an optional dependency for huffman compression.
+By default twnet_parser is using the huffman compression code from the [TeeAI](https://github.com/edg-l/TeeAI)
+project which is written in pure python.
+If you have [libtw2-huffman](https://pypi.org/project/libtw2-huffman/) installed it will use that one instead.
+Because it is faster since it is written in rust and has better error handling.
+But since it is so much overhead it is not installed by default to keep twnet_parser light weight.
+
+
+You can install it by running ``pip install libtw2-huffman``
+or by running ``pip install -r requirements/optional.txt``
+
+
+You can also check which huffman backend is currently active with these lines of code
+
+```python
+import twnet_parser.huffman
+print(twnet_parser.huffman.backend_name()) # => rust-libtw2 or python-TeeAI
+```
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
 pip install -r requirements/dev.txt
+pre-commit install --hook-type commit-msg
 ```
 
 ## tests and linting
 
 ```bash
 # dev dependencies
 pip install -r requirements/dev.txt
```

