# Comparing `tmp/ltchiptool-4.2.2.tar.gz` & `tmp/ltchiptool-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool-4.2.2.tar", max compression
+gzip compressed data, was "ltchiptool-4.2.3.tar", max compression
```

## Comparing `ltchiptool-4.2.2.tar` & `ltchiptool-4.2.3.tar`

### file list

```diff
@@ -1,119 +1,122 @@
--rw-r--r--   0        0        0     1076 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/LICENSE
--rw-r--r--   0        0        0     2384 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/README.md
--rw-r--r--   0        0        0      376 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/__init__.py
--rw-r--r--   0        0        0     2769 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/__main__.py
--rw-r--r--   0        0        0      908 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/compile/elf2bin.py
--rw-r--r--   0        0        0      881 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/compile/link2bin.py
--rw-r--r--   0        0        0      502 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/flash/__main__.py
--rw-r--r--   0        0        0     1724 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/flash/_utils.py
--rw-r--r--   0        0        0     1610 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/flash/file.py
--rw-r--r--   0        0        0     3192 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/flash/read.py
--rw-r--r--   0        0        0     2442 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/flash/split.py
--rw-r--r--   0        0        0     7188 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/flash/write.py
--rw-r--r--   0        0        0     2331 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/list.py
--rw-r--r--   0        0        0     3833 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/plugin/manage.py
--rw-r--r--   0        0        0     1022 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/plugin/run.py
--rw-r--r--   0        0        0      423 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/commands/soc.py
--rw-r--r--   0        0        0     2022 2023-06-18 16:03:21.620300 ltchiptool-4.2.2/ltchiptool/families.json
--rw-r--r--   0        0        0      127 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/__main__.py
--rw-r--r--   0        0        0     5990 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/colors.json
--rw-r--r--   0        0        0     3964 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/colors.py
--rw-r--r--   0        0        0     9477 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/ltchiptool-192x192.png
--rw-r--r--   0        0        0    15406 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/ltchiptool.ico
--rw-r--r--   0        0        0    17134 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/ltchiptool.wxui
--rw-r--r--   0        0        0    21898 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/ltchiptool.xrc
--rw-r--r--   0        0        0    10596 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/main.py
--rw-r--r--   0        0        0       48 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/panels/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/panels/about.py
--rw-r--r--   0        0        0     5807 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/panels/base.py
--rw-r--r--   0        0        0    17297 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/panels/flash.py
--rw-r--r--   0        0        0     6885 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/panels/log.py
--rw-r--r--   0        0        0    12398 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/panels/plugins.py
--rw-r--r--   0        0        0     1405 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/utils.py
--rw-r--r--   0        0        0       47 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/work/__init__.py
--rw-r--r--   0        0        0      950 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/work/base.py
--rw-r--r--   0        0        0     6041 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/work/flash.py
--rw-r--r--   0        0        0      798 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/work/plugins.py
--rw-r--r--   0        0        0     2528 2023-06-18 16:03:04.531902 ltchiptool-4.2.2/ltchiptool/gui/work/ports.py
--rw-r--r--   0        0        0      263 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/models/__init__.py
--rw-r--r--   0        0        0     3144 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/models/board.py
--rw-r--r--   0        0        0      155 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/models/enums.py
--rw-r--r--   0        0        0     5966 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/models/family.py
--rw-r--r--   0        0        0     3199 2023-06-18 16:03:21.620300 ltchiptool-4.2.2/ltchiptool/platform.json
--rw-r--r--   0        0        0      185 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/__init__.py
--rw-r--r--   0        0        0      111 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz/__init__.py
--rw-r--r--   0        0        0     6198 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz/binary.py
--rw-r--r--   0        0        0     6959 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz/flash.py
--rw-r--r--   0        0        0      721 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz/main.py
--rw-r--r--   0        0        0       48 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz/util/__init__.py
--rw-r--r--   0        0        0    18071 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz/util/rtltool.py
--rw-r--r--   0        0        0      114 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/__init__.py
--rw-r--r--   0        0        0     7749 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/binary.py
--rw-r--r--   0        0        0     4791 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/flash.py
--rw-r--r--   0        0        0      648 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/main.py
--rw-r--r--   0        0        0     7691 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/parse_partition.py
--rw-r--r--   0        0        0       49 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/__init__.py
--rw-r--r--   0        0        0    17029 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/ambz2tool.py
--rw-r--r--   0        0        0       48 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/__init__.py
--rw-r--r--   0        0        0     1993 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/config.py
--rw-r--r--   0        0        0     1036 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/enums.py
--rw-r--r--   0        0        0     3188 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/headers.py
--rw-r--r--   0        0        0     5129 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/images.py
--rw-r--r--   0        0        0     4642 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/partitions.py
--rw-r--r--   0        0        0      619 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/utils.py
--rw-r--r--   0        0        0      111 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/__init__.py
--rw-r--r--   0        0        0     9025 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/binary.py
--rw-r--r--   0        0        0     8305 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/bkpackager.py
--rw-r--r--   0        0        0     6855 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/flash.py
--rw-r--r--   0        0        0      723 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/main.py
--rw-r--r--   0        0        0      317 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/__init__.py
--rw-r--r--   0        0        0     7069 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/binary.py
--rw-r--r--   0        0        0     6175 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/crypto.py
--rw-r--r--   0        0        0      515 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/models.py
--rw-r--r--   0        0        0     2940 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/rbl.py
--rw-r--r--   0        0        0     2843 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/common.py
--rw-r--r--   0        0        0     6513 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/soc/interface.py
--rw-r--r--   0        0        0       48 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/bitint.py
--rw-r--r--   0        0        0     3393 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/cli.py
--rw-r--r--   0        0        0     5642 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/crc16.py
--rw-r--r--   0        0        0     2277 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/crypto.py
--rw-r--r--   0        0        0     4441 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/curve25519.py
--rw-r--r--   0        0        0     6631 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/detection.py
--rw-r--r--   0        0        0     1987 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/dict.py
--rw-r--r--   0        0        0      252 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/env.py
--rw-r--r--   0        0        0     2661 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/fileio.py
--rw-r--r--   0        0        0     1746 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/flash.py
--rw-r--r--   0        0        0     3296 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/fwbinary.py
--rw-r--r--   0        0        0     6105 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/intbin.py
--rw-r--r--   0        0        0     5164 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/logging.py
--rw-r--r--   0        0        0     6332 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/lpm.py
--rw-r--r--   0        0        0     7308 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/lvm.py
--rw-r--r--   0        0        0     2670 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/misc.py
--rw-r--r--   0        0        0     1878 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/obj.py
--rw-r--r--   0        0        0      866 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/slice.py
--rw-r--r--   0        0        0     5747 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/streams.py
--rw-r--r--   0        0        0     1612 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/util/toolchain.py
--rw-r--r--   0        0        0      772 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltchiptool/version.py
--rw-r--r--   0        0        0      154 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltctplugin/base/__init__.py
--rw-r--r--   0        0        0     4431 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/ltctplugin/base/base.py
--rw-r--r--   0        0        0     1360 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/__init__.py
--rw-r--r--   0        0        0      251 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/binpatch/__init__.py
--rw-r--r--   0        0        0      471 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/binpatch/apply.py
--rw-r--r--   0        0        0     1027 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/binpatch/bindiff.py
--rw-r--r--   0        0        0     1666 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/binpatch/diff32.py
--rw-r--r--   0        0        0     4306 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/cli.py
--rw-r--r--   0        0        0      360 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/block.py
--rw-r--r--   0        0        0     5803 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/context.py
--rw-r--r--   0        0        0     2210 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/enums.py
--rw-r--r--   0        0        0     1256 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/flags.py
--rw-r--r--   0        0        0     3311 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/image.py
--rw-r--r--   0        0        0      772 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/partition.py
--rw-r--r--   0        0        0     4552 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/models/uf2.py
--rw-r--r--   0        0        0      124 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/upload/__init__.py
--rw-r--r--   0        0        0     4846 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/upload/esphome.py
--rw-r--r--   0        0        0     7219 2023-06-18 16:03:04.535902 ltchiptool-4.2.2/uf2tool/writer.py
--rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 ltchiptool-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/LICENSE
+-rw-r--r--   0        0        0     2384 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/README.md
+-rw-r--r--   0        0        0      376 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/__init__.py
+-rw-r--r--   0        0        0     2769 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/__main__.py
+-rw-r--r--   0        0        0      908 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/compile/elf2bin.py
+-rw-r--r--   0        0        0      881 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/compile/link2bin.py
+-rw-r--r--   0        0        0      502 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/flash/__main__.py
+-rw-r--r--   0        0        0     1724 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/flash/_utils.py
+-rw-r--r--   0        0        0     1610 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/flash/file.py
+-rw-r--r--   0        0        0     3192 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/flash/read.py
+-rw-r--r--   0        0        0     2442 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/flash/split.py
+-rw-r--r--   0        0        0     7188 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/flash/write.py
+-rw-r--r--   0        0        0     2331 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/list.py
+-rw-r--r--   0        0        0     3833 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/plugin/manage.py
+-rw-r--r--   0        0        0     1022 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/plugin/run.py
+-rw-r--r--   0        0        0      423 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/commands/soc.py
+-rw-r--r--   0        0        0     2262 2023-07-13 14:49:21.377052 ltchiptool-4.2.3/ltchiptool/families.json
+-rw-r--r--   0        0        0      127 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/__init__.py
+-rw-r--r--   0        0        0     1514 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/__main__.py
+-rw-r--r--   0        0        0     1350 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/base/frame.py
+-rw-r--r--   0        0        0     4363 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/base/panel.py
+-rw-r--r--   0        0        0     1750 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/base/window.py
+-rw-r--r--   0        0        0     5990 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/colors.json
+-rw-r--r--   0        0        0     3964 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/colors.py
+-rw-r--r--   0        0        0     9477 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/ltchiptool-192x192.png
+-rw-r--r--   0        0        0    15406 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/ltchiptool.ico
+-rw-r--r--   0        0        0    17134 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/ltchiptool.wxui
+-rw-r--r--   0        0        0    21898 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/ltchiptool.xrc
+-rw-r--r--   0        0        0    11053 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/main.py
+-rw-r--r--   0        0        0       48 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/panels/__init__.py
+-rw-r--r--   0        0        0     2038 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/panels/about.py
+-rw-r--r--   0        0        0      129 2023-07-13 14:48:51.355997 ltchiptool-4.2.3/ltchiptool/gui/panels/base.py
+-rw-r--r--   0        0        0    17297 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/panels/flash.py
+-rw-r--r--   0        0        0     6885 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/panels/log.py
+-rw-r--r--   0        0        0    12398 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/panels/plugins.py
+-rw-r--r--   0        0        0     1405 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/utils.py
+-rw-r--r--   0        0        0       47 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/work/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/work/base.py
+-rw-r--r--   0        0        0     6041 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/work/flash.py
+-rw-r--r--   0        0        0      798 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/work/plugins.py
+-rw-r--r--   0        0        0     2528 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/gui/work/ports.py
+-rw-r--r--   0        0        0      263 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/models/__init__.py
+-rw-r--r--   0        0        0     3144 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/models/board.py
+-rw-r--r--   0        0        0      155 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/models/enums.py
+-rw-r--r--   0        0        0     5966 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/models/family.py
+-rw-r--r--   0        0        0     3199 2023-07-13 14:49:21.377052 ltchiptool-4.2.3/ltchiptool/platform.json
+-rw-r--r--   0        0        0      185 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz/__init__.py
+-rw-r--r--   0        0        0     6198 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz/binary.py
+-rw-r--r--   0        0        0     6959 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz/flash.py
+-rw-r--r--   0        0        0      721 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz/main.py
+-rw-r--r--   0        0        0       48 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz/util/__init__.py
+-rw-r--r--   0        0        0    18071 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz/util/rtltool.py
+-rw-r--r--   0        0        0      114 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/__init__.py
+-rw-r--r--   0        0        0     8159 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/binary.py
+-rw-r--r--   0        0        0     4791 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/flash.py
+-rw-r--r--   0        0        0      648 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/main.py
+-rw-r--r--   0        0        0     7691 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/parse_partition.py
+-rw-r--r--   0        0        0       49 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/__init__.py
+-rw-r--r--   0        0        0    17029 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/ambz2tool.py
+-rw-r--r--   0        0        0       48 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/config.py
+-rw-r--r--   0        0        0     1036 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/enums.py
+-rw-r--r--   0        0        0     3188 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/headers.py
+-rw-r--r--   0        0        0     5129 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/images.py
+-rw-r--r--   0        0        0     4642 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/partitions.py
+-rw-r--r--   0        0        0      619 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/utils.py
+-rw-r--r--   0        0        0      111 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/__init__.py
+-rw-r--r--   0        0        0     9025 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/binary.py
+-rw-r--r--   0        0        0     8305 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/bkpackager.py
+-rw-r--r--   0        0        0     6855 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/flash.py
+-rw-r--r--   0        0        0      723 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/main.py
+-rw-r--r--   0        0        0      317 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/__init__.py
+-rw-r--r--   0        0        0     7069 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/binary.py
+-rw-r--r--   0        0        0     6175 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/crypto.py
+-rw-r--r--   0        0        0      515 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/models.py
+-rw-r--r--   0        0        0     2940 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/rbl.py
+-rw-r--r--   0        0        0     2843 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/common.py
+-rw-r--r--   0        0        0     6513 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/soc/interface.py
+-rw-r--r--   0        0        0       48 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/__init__.py
+-rw-r--r--   0        0        0     2408 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/bitint.py
+-rw-r--r--   0        0        0     3393 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/cli.py
+-rw-r--r--   0        0        0     5642 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/crc16.py
+-rw-r--r--   0        0        0     2277 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/crypto.py
+-rw-r--r--   0        0        0     4441 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/curve25519.py
+-rw-r--r--   0        0        0     6631 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/detection.py
+-rw-r--r--   0        0        0     1987 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/dict.py
+-rw-r--r--   0        0        0      252 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/env.py
+-rw-r--r--   0        0        0     2661 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/fileio.py
+-rw-r--r--   0        0        0     1746 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/flash.py
+-rw-r--r--   0        0        0     3296 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/fwbinary.py
+-rw-r--r--   0        0        0     6105 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/intbin.py
+-rw-r--r--   0        0        0     5164 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/logging.py
+-rw-r--r--   0        0        0     6332 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/lpm.py
+-rw-r--r--   0        0        0     7308 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/lvm.py
+-rw-r--r--   0        0        0     2670 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/misc.py
+-rw-r--r--   0        0        0     1878 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/obj.py
+-rw-r--r--   0        0        0      866 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/slice.py
+-rw-r--r--   0        0        0     5747 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/streams.py
+-rw-r--r--   0        0        0     1612 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/util/toolchain.py
+-rw-r--r--   0        0        0      772 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltchiptool/version.py
+-rw-r--r--   0        0        0      154 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltctplugin/base/__init__.py
+-rw-r--r--   0        0        0     4431 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/ltctplugin/base/base.py
+-rw-r--r--   0        0        0     1360 2023-07-13 14:48:51.359997 ltchiptool-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/__init__.py
+-rw-r--r--   0        0        0      251 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/binpatch/__init__.py
+-rw-r--r--   0        0        0      471 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/binpatch/apply.py
+-rw-r--r--   0        0        0     1027 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/binpatch/bindiff.py
+-rw-r--r--   0        0        0     1666 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/binpatch/diff32.py
+-rw-r--r--   0        0        0     4306 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/cli.py
+-rw-r--r--   0        0        0      360 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/__init__.py
+-rw-r--r--   0        0        0     4805 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/block.py
+-rw-r--r--   0        0        0     5803 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/context.py
+-rw-r--r--   0        0        0     2210 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/enums.py
+-rw-r--r--   0        0        0     1256 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/flags.py
+-rw-r--r--   0        0        0     3311 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/image.py
+-rw-r--r--   0        0        0      772 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/partition.py
+-rw-r--r--   0        0        0     4552 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/models/uf2.py
+-rw-r--r--   0        0        0      124 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/upload/__init__.py
+-rw-r--r--   0        0        0     4846 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/upload/esphome.py
+-rw-r--r--   0        0        0     7219 2023-07-13 14:48:51.363997 ltchiptool-4.2.3/uf2tool/writer.py
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 ltchiptool-4.2.3/PKG-INFO
```

### Comparing `ltchiptool-4.2.2/LICENSE` & `ltchiptool-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/README.md` & `ltchiptool-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/__main__.py` & `ltchiptool-4.2.3/ltchiptool/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/compile/elf2bin.py` & `ltchiptool-4.2.3/ltchiptool/commands/compile/elf2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/compile/link2bin.py` & `ltchiptool-4.2.3/ltchiptool/commands/compile/link2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/flash/_utils.py` & `ltchiptool-4.2.3/ltchiptool/commands/flash/_utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/flash/file.py` & `ltchiptool-4.2.3/ltchiptool/commands/flash/file.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/flash/read.py` & `ltchiptool-4.2.3/ltchiptool/commands/flash/read.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/flash/split.py` & `ltchiptool-4.2.3/ltchiptool/commands/flash/split.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/flash/write.py` & `ltchiptool-4.2.3/ltchiptool/commands/flash/write.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/list.py` & `ltchiptool-4.2.3/ltchiptool/commands/list.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/plugin/manage.py` & `ltchiptool-4.2.3/ltchiptool/commands/plugin/manage.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/commands/plugin/run.py` & `ltchiptool-4.2.3/ltchiptool/commands/plugin/run.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/families.json` & `ltchiptool-4.2.3/ltchiptool/families.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'beken-7231'": "OrderedDict([('parent', 'beken-72xx-gen1'), ('code', 'bk7231'), ('description', "*

 * *                 "'Beken 7231')])",*

 * * "'beken-7231q'": "OrderedDict([('parent', 'beken-7231'), ('code', 'bk7231q'), ('description', "*

 * *                  "'Beken 7231Q'), ('id', '0xAFE81D49'), ('short_name', 'BK7231Q')])",*

 * * "'beken-7231t'": "OrderedDict([('parent', 'beken-7231'), ('code', 'bk7231t'), ('description', "*

 * *                  "'Beken 7231T'), ('id', '0x675A40B0'), ('short_name', 'BK7231T')])",*

 * * 'delete […]*

```diff
@@ -1,22 +1,34 @@
 {
     "$schema": "./families.schema.json",
+    "beken-7231": {
+        "code": "bk7231",
+        "description": "Beken 7231",
+        "parent": "beken-72xx-gen1"
+    },
     "beken-7231n": {
         "code": "bk7231n",
         "description": "Beken 7231N",
         "id": "0x7B3EF230",
         "parent": "beken-72xx-gen1",
         "short_name": "BK7231N"
     },
-    "beken-7231u": {
-        "code": "bk7231u",
-        "description": "Beken 7231U/7231T",
+    "beken-7231q": {
+        "code": "bk7231q",
+        "description": "Beken 7231Q",
+        "id": "0xAFE81D49",
+        "parent": "beken-7231",
+        "short_name": "BK7231Q"
+    },
+    "beken-7231t": {
+        "code": "bk7231t",
+        "description": "Beken 7231T",
         "id": "0x675A40B0",
-        "parent": "beken-72xx-gen1",
-        "short_name": "BK7231U"
+        "parent": "beken-7231",
+        "short_name": "BK7231T"
     },
     "beken-7251": {
         "code": "bk7251",
         "description": "Beken 7251/7252",
         "id": "0x6A82CC42",
         "parent": "beken-72xx-gen1",
         "short_name": "BK7251"
```

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/__main__.py` & `ltchiptool-4.2.3/ltchiptool/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/colors.json` & `ltchiptool-4.2.3/ltchiptool/gui/colors.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/colors.py` & `ltchiptool-4.2.3/ltchiptool/gui/colors.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/ltchiptool-192x192.png` & `ltchiptool-4.2.3/ltchiptool/gui/ltchiptool-192x192.png`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/ltchiptool.ico` & `ltchiptool-4.2.3/ltchiptool/gui/ltchiptool.ico`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/ltchiptool.wxui` & `ltchiptool-4.2.3/ltchiptool/gui/ltchiptool.wxui`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/ltchiptool.xrc` & `ltchiptool-4.2.3/ltchiptool/gui/ltchiptool.xrc`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/main.py` & `ltchiptool-4.2.3/ltchiptool/gui/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 from click import get_app_dir
 
 from ltchiptool.util.fileio import readjson, writejson
 from ltchiptool.util.logging import LoggingHandler, verbose
 from ltchiptool.util.lpm import LPM
 from ltchiptool.util.lvm import LVM
 
+from .base.frame import BaseFrame
+from .base.panel import BasePanel
+from .base.window import BaseWindow
 from .colors import ColorPalette
-from .panels.base import BasePanel
 from .panels.log import LogPanel
 from .utils import load_xrc_file, on_event, with_event, with_target
 
 
 # noinspection PyPep8Naming
 class MainFrame(wx.Frame):
+    Windows: dict[str, BaseWindow]
     Panels: dict[str, BasePanel]
     Menus: dict[str, wx.Menu]
     MenuItems: dict[str, dict[str, wx.MenuItem]]
     init_params: dict
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
@@ -57,15 +60,15 @@
         self.config_file = join(get_app_dir("ltchiptool"), "gui.json")
         if isfile(old_config):
             # migrate old config to new filename
             if isfile(self.config_file):
                 unlink(self.config_file)
             rename(old_config, self.config_file)
         self.loaded = False
-        self.Panels = {}
+        self.Windows = self.Panels = {}
         self.init_params = {}
 
         # main window layout
         self.Sizer = wx.BoxSizer(wx.VERTICAL)
         self.Splitter = wx.SplitterWindow(self, style=wx.SP_3D | wx.SP_LIVE_UPDATE)
         # build splitter panes
         self.Notebook = wx.Notebook(parent=self.Splitter)
@@ -73,15 +76,15 @@
         self.Log = LogPanel(parent=self.Splitter, frame=self)
         # initialize the splitter
         self.Splitter.SetMinimumPaneSize(150)
         self.Splitter.SetSashGravity(0.7)
         self.Splitter.SplitHorizontally(self.Notebook, self.Log, sashPosition=-300)
         self.Sizer.Add(self.Splitter, proportion=1, flag=wx.EXPAND)
         self.SetSizer(self.Sizer)
-        self.Panels["log"] = self.Log
+        self.Windows["log"] = self.Log
 
         # list all built-in panels
         from .panels.about import AboutPanel
         from .panels.flash import FlashPanel
         from .panels.plugins import PluginsPanel
 
         windows = [
@@ -107,15 +110,18 @@
                 if not cls:
                     continue
                 if name.startswith("plugin."):
                     # mark as loaded after trying to build any plugin
                     self.loaded = True
                 if issubclass(cls, BasePanel):
                     panel = cls(parent=self.Notebook, frame=self)
-                    self.Panels[name] = panel
+                    self.Windows[name] = panel
+                elif issubclass(cls, BaseFrame):
+                    frame = cls(parent=self, frame=self)
+                    self.Windows[name] = frame
                 else:
                     warning(f"Unknown GUI element: {cls}")
 
             self.loaded = True
         except Exception as e:
             LoggingHandler.get().emit_exception(e, msg=f"Couldn't build {name}")
             if not self.loaded:
@@ -189,22 +195,22 @@
         for i in range(self.Notebook.GetPageCount()):
             if panel == self.Notebook.GetPage(i):
                 self.Notebook.SetSelection(i)
                 return
 
     @property
     def NotebookPageName(self) -> str:
-        for name, panel in self.Panels.items():
+        for name, panel in self.Windows.items():
             if panel == self.Notebook.GetCurrentPage():
                 return name
 
     @NotebookPageName.setter
     def NotebookPageName(self, name: str):
-        panel = self.Panels.get(name, None)
-        if panel:
+        panel = self.Windows.get(name, None)
+        if isinstance(panel, BasePanel):
             self.NotebookPagePanel = panel
 
     def UpdateMenus(self) -> None:
         self.MenuBar: wx.MenuBar = self.GetMenuBar()
         self.Menus = {}
         self.MenuItems = {}
         for menu, label in self.MenuBar.GetMenus():
@@ -230,32 +236,34 @@
             caption="Error",
             style=wx.ICON_ERROR,
         )
 
     def OnShow(self, *_):
         settings = self._settings
         self.SetSettings(**settings.get("main", {}))
-        for name, panel in self.Panels.items():
-            panel.SetSettings(**settings.get(name, {}))
-            panel.SetInitParams(**self.init_params)
+        for name, window in self.Windows.items():
+            window.SetSettings(**settings.get(name, {}))
+            window.SetInitParams(**self.init_params)
         if settings:
             info(f"Loaded settings from {self.config_file}")
-        for name, panel in self.Panels.items():
-            panel.OnShow()
+        for name, window in self.Windows.items():
+            window.OnShow()
 
     def OnClose(self, *_):
         if not self.loaded:
             # avoid writing partial settings in case of loading failure
             self.Destroy()
             return
         settings = self._settings
         settings["main"] = self.GetSettings()
-        for name, panel in self.Panels.items():
-            panel.OnClose()
-            settings[name] = panel.GetSettings() or {}
+        for name, window in self.Windows.items():
+            window.OnClose()
+            window_settings = window.GetSettings() or {}
+            if window_settings:
+                settings[name] = window_settings
         self._settings = settings
         info(f"Saved settings to {self.config_file}")
         self.Destroy()
 
     @with_target
     def OnMenu(self, event: wx.CommandEvent, target: wx.Menu):
         if not isinstance(target, wx.Menu):
@@ -273,20 +281,21 @@
                 self.Close(True)
 
             case ("Colors", _):
                 self.palette = label
 
             case ("Debug", "Print settings"):
                 debug(f"Main settings: {self.GetSettings()}")
-                for name, panel in self.Panels.items():
-                    debug(f"Panel '{name}' settings: {panel.GetSettings()}")
+                for name, window in self.Windows.items():
+                    debug(f"Window '{name}' settings: {window.GetSettings()}")
 
             case _:
-                for panel in self.Panels.values():
-                    panel.OnMenu(title, label, checked)
+                for panel in self.Windows.values():
+                    if isinstance(panel, BasePanel):
+                        panel.OnMenu(title, label, checked)
 
     @with_event
     def OnPageChanging(self, event: wx.BookCtrlEvent):
         panel = self.NotebookPagePanel
         if not panel:
             return
         verbose(f"Deactivating page: {type(panel)}")
@@ -307,9 +316,9 @@
 
     @palette.setter
     def palette(self, value: str) -> None:
         old = ColorPalette.get()
         new = ColorPalette.set(ColorPalette(value))
         item = self.MenuItems["Colors"][new.title]
         item.Check(True)
-        for panel in self.Panels.values():
-            panel.OnPaletteChanged(old, new)
+        for window in self.Windows.values():
+            window.OnPaletteChanged(old, new)
```

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/panels/about.py` & `ltchiptool-4.2.3/ltchiptool/gui/panels/about.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/panels/flash.py` & `ltchiptool-4.2.3/ltchiptool/gui/panels/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/panels/log.py` & `ltchiptool-4.2.3/ltchiptool/gui/panels/log.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/panels/plugins.py` & `ltchiptool-4.2.3/ltchiptool/gui/panels/plugins.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/utils.py` & `ltchiptool-4.2.3/ltchiptool/gui/utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/work/base.py` & `ltchiptool-4.2.3/ltchiptool/gui/work/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/work/flash.py` & `ltchiptool-4.2.3/ltchiptool/gui/work/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/work/plugins.py` & `ltchiptool-4.2.3/ltchiptool/gui/work/plugins.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/gui/work/ports.py` & `ltchiptool-4.2.3/ltchiptool/gui/work/ports.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/models/board.py` & `ltchiptool-4.2.3/ltchiptool/models/board.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/models/family.py` & `ltchiptool-4.2.3/ltchiptool/models/family.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/platform.json` & `ltchiptool-4.2.3/ltchiptool/platform.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -107,9 +107,9 @@
         }
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/kuba2k2/platformio-libretiny"
     },
     "title": "LibreTiny",
-    "version": "1.0.2"
+    "version": "1.1.0"
 }
```

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz/binary.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz/flash.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz/main.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz/util/rtltool.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz/util/rtltool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/binary.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/binary.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         )
 
     def elf2bin(self, input: str, ota_idx: int) -> List[FirmwareBinary]:
         result: Dict[str, Optional[int]] = {}
         # read AmbZ2 image config
         config = ImageConfig(**self.board["image"])
         # find partition offsets
+        ptab_offset, _, ptab_end = self.board.region("part_table")
         boot_offset, _, boot_end = self.board.region("boot")
         ota1_offset, _, ota1_end = self.board.region("ota1")
 
         # find bootloader image
         input_boot = chname(input, "bootloader.axf")
         if not isfile(input_boot):
             raise FileNotFoundError("Bootloader image not found")
@@ -105,14 +106,20 @@
             location=input,
             name="firmware_is",
             offset=ota1_offset,
             title="Application Image",
             description="Firmware partition image for direct flashing",
             public=True,
         )
+        out_ptab = FirmwareBinary(
+            location=input,
+            name="part_table",
+            offset=ptab_offset,
+            title="Partition Table",
+        )
         out_boot = FirmwareBinary(
             location=input,
             name="bootloader",
             offset=boot_offset,
             title="Bootloader Image",
         )
         # print graph element
@@ -191,14 +198,18 @@
             firmware=firmware,
         )
 
         # write all parts to files
         data = flash.pack(hash_key=config.keys.hash_keys["part_table"])
         with output.write() as f:
             f.write(data)
+        with out_ptab.write() as f:
+            ptab = data[ptab_offset:ptab_end].rstrip(b"\xFF")
+            ptab = pad_data(ptab, 0x20, 0xFF)
+            f.write(ptab)
         with out_boot.write() as f:
             boot = data[boot_offset:boot_end].rstrip(b"\xFF")
             boot = pad_data(boot, 0x20, 0xFF)
             f.write(boot)
         with out_ota1.write() as f:
             ota1 = data[ota1_offset:ota1_end]
             f.write(ota1)
```

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/flash.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/main.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/parse_partition.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/parse_partition.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/ambz2tool.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/ambz2tool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/config.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/config.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/enums.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/headers.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/headers.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/images.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/images.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/partitions.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/partitions.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/ambz2/util/models/utils.py` & `ltchiptool-4.2.3/ltchiptool/soc/ambz2/util/models/utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/binary.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/bkpackager.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/bkpackager.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/flash.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/main.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/binary.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/crypto.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/models.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/models.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/bk72xx/util/rbl.py` & `ltchiptool-4.2.3/ltchiptool/soc/bk72xx/util/rbl.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/common.py` & `ltchiptool-4.2.3/ltchiptool/soc/common.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/soc/interface.py` & `ltchiptool-4.2.3/ltchiptool/soc/interface.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/bitint.py` & `ltchiptool-4.2.3/ltchiptool/util/bitint.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/cli.py` & `ltchiptool-4.2.3/ltchiptool/util/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/crc16.py` & `ltchiptool-4.2.3/ltchiptool/util/crc16.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/crypto.py` & `ltchiptool-4.2.3/ltchiptool/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/curve25519.py` & `ltchiptool-4.2.3/ltchiptool/util/curve25519.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/detection.py` & `ltchiptool-4.2.3/ltchiptool/util/detection.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/dict.py` & `ltchiptool-4.2.3/ltchiptool/util/dict.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/fileio.py` & `ltchiptool-4.2.3/ltchiptool/util/fileio.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/flash.py` & `ltchiptool-4.2.3/ltchiptool/util/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/fwbinary.py` & `ltchiptool-4.2.3/ltchiptool/util/fwbinary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/intbin.py` & `ltchiptool-4.2.3/ltchiptool/util/intbin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/logging.py` & `ltchiptool-4.2.3/ltchiptool/util/logging.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/lpm.py` & `ltchiptool-4.2.3/ltchiptool/util/lpm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/lvm.py` & `ltchiptool-4.2.3/ltchiptool/util/lvm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/misc.py` & `ltchiptool-4.2.3/ltchiptool/util/misc.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/obj.py` & `ltchiptool-4.2.3/ltchiptool/util/obj.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/slice.py` & `ltchiptool-4.2.3/ltchiptool/util/slice.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/streams.py` & `ltchiptool-4.2.3/ltchiptool/util/streams.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/util/toolchain.py` & `ltchiptool-4.2.3/ltchiptool/util/toolchain.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltchiptool/version.py` & `ltchiptool-4.2.3/ltchiptool/version.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/ltctplugin/base/base.py` & `ltchiptool-4.2.3/ltctplugin/base/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/pyproject.toml` & `ltchiptool-4.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ltchiptool"
-version = "4.2.2"
+version = "4.2.3"
 description = "Universal flashing and binary manipulation tool for IoT chips"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 packages = [
     { include = "ltchiptool" },
     { include = "ltctplugin/base" },
     { include = "uf2tool" },
```

### Comparing `ltchiptool-4.2.2/uf2tool/binpatch/bindiff.py` & `ltchiptool-4.2.3/uf2tool/binpatch/bindiff.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/binpatch/diff32.py` & `ltchiptool-4.2.3/uf2tool/binpatch/diff32.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/cli.py` & `ltchiptool-4.2.3/uf2tool/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/block.py` & `ltchiptool-4.2.3/uf2tool/models/block.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/context.py` & `ltchiptool-4.2.3/uf2tool/models/context.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/enums.py` & `ltchiptool-4.2.3/uf2tool/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/flags.py` & `ltchiptool-4.2.3/uf2tool/models/flags.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/image.py` & `ltchiptool-4.2.3/uf2tool/models/image.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/partition.py` & `ltchiptool-4.2.3/uf2tool/models/partition.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/models/uf2.py` & `ltchiptool-4.2.3/uf2tool/models/uf2.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/upload/esphome.py` & `ltchiptool-4.2.3/uf2tool/upload/esphome.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/uf2tool/writer.py` & `ltchiptool-4.2.3/uf2tool/writer.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.2/PKG-INFO` & `ltchiptool-4.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltchiptool
-Version: 4.2.2
+Version: 4.2.3
 Summary: Universal flashing and binary manipulation tool for IoT chips
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

