# Comparing `tmp/temporian-0.1.1.tar.gz` & `tmp/temporian-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporian-0.1.1.tar", max compression
+gzip compressed data, was "temporian-0.1.2.tar", max compression
```

## Comparing `temporian-0.1.1.tar` & `temporian-0.1.2.tar`

### file list

```diff
@@ -1,260 +1,282 @@
--rw-r--r--   0        0        0    11358 2023-06-15 08:27:36.155324 temporian-0.1.1/LICENSE
--rw-r--r--   0        0        0     3395 2023-06-15 08:27:36.155475 temporian-0.1.1/README.md
--rw-r--r--   0        0        0     3633 2023-06-15 08:27:36.157936 temporian-0.1.1/config/build.py
--rw-r--r--   0        0        0     2603 2023-06-15 08:27:36.203976 temporian-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      865 2023-06-15 08:27:36.204946 temporian-0.1.1/temporian/BUILD
--rw-r--r--   0        0        0     2460 2023-06-15 08:27:36.205527 temporian-0.1.1/temporian/__init__.py
--rw-r--r--   0        0        0      943 2023-06-15 08:27:36.206059 temporian-0.1.1/temporian/core/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.206303 temporian-0.1.1/temporian/core/__init__.py
--rw-r--r--   0        0        0      853 2023-06-15 08:27:36.207495 temporian-0.1.1/temporian/core/data/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.207694 temporian-0.1.1/temporian/core/data/__init__.py
--rw-r--r--   0        0        0      469 2023-06-15 08:27:36.208019 temporian-0.1.1/temporian/core/data/dtypes/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.208495 temporian-0.1.1/temporian/core/data/dtypes/__init__.py
--rw-r--r--   0        0        0      919 2023-06-15 08:27:36.208980 temporian-0.1.1/temporian/core/data/dtypes/api_symbols.py
--rw-r--r--   0        0        0     2866 2023-06-15 08:27:36.209371 temporian-0.1.1/temporian/core/data/dtypes/dtype.py
--rw-r--r--   0        0        0     2780 2023-06-15 08:27:36.209684 temporian-0.1.1/temporian/core/data/duration.py
--rw-r--r--   0        0        0     6233 2023-06-15 08:27:36.209992 temporian-0.1.1/temporian/core/data/duration_utils.py
--rw-r--r--   0        0        0    21120 2023-06-15 08:27:36.210392 temporian-0.1.1/temporian/core/data/node.py
--rw-r--r--   0        0        0     3874 2023-06-15 08:27:36.210927 temporian-0.1.1/temporian/core/data/schema.py
--rw-r--r--   0        0        0      382 2023-06-15 08:27:36.211208 temporian-0.1.1/temporian/core/data/test/BUILD
--rw-r--r--   0        0        0     1326 2023-06-15 08:27:36.211483 temporian-0.1.1/temporian/core/data/test/node_test.py
--rw-r--r--   0        0        0     9858 2023-06-15 08:27:36.212196 temporian-0.1.1/temporian/core/evaluation.py
--rw-r--r--   0        0        0    10229 2023-06-15 08:27:36.212502 temporian-0.1.1/temporian/core/graph.py
--rw-r--r--   0        0        0     1325 2023-06-15 08:27:36.212703 temporian-0.1.1/temporian/core/operator_lib.py
--rw-r--r--   0        0        0     6032 2023-06-15 08:27:36.213173 temporian-0.1.1/temporian/core/operators/BUILD
--rw-r--r--   0        0        0      594 2023-06-15 08:27:36.213357 temporian-0.1.1/temporian/core/operators/__init__.py
--rw-r--r--   0        0        0     6849 2023-06-15 08:27:36.213899 temporian-0.1.1/temporian/core/operators/add_index.py
--rw-r--r--   0        0        0     2003 2023-06-15 08:27:36.214155 temporian-0.1.1/temporian/core/operators/api_symbols.py
--rw-r--r--   0        0        0    10868 2023-06-15 08:27:36.214492 temporian-0.1.1/temporian/core/operators/base.py
--rw-r--r--   0        0        0     2012 2023-06-15 08:27:36.214748 temporian-0.1.1/temporian/core/operators/begin.py
--rw-r--r--   0        0        0     1659 2023-06-15 08:27:36.215082 temporian-0.1.1/temporian/core/operators/binary/BUILD
--rw-r--r--   0        0        0      771 2023-06-15 08:27:36.215326 temporian-0.1.1/temporian/core/operators/binary/__init__.py
--rw-r--r--   0        0        0     1623 2023-06-15 08:27:36.215825 temporian-0.1.1/temporian/core/operators/binary/api_symbols.py
--rw-r--r--   0        0        0     6545 2023-06-15 08:27:36.216178 temporian-0.1.1/temporian/core/operators/binary/arithmetic.py
--rw-r--r--   0        0        0     4072 2023-06-15 08:27:36.216464 temporian-0.1.1/temporian/core/operators/binary/base.py
--rw-r--r--   0        0        0     4164 2023-06-15 08:27:36.216998 temporian-0.1.1/temporian/core/operators/binary/logical.py
--rw-r--r--   0        0        0     6286 2023-06-15 08:27:36.217315 temporian-0.1.1/temporian/core/operators/binary/relational.py
--rw-r--r--   0        0        0     2687 2023-06-15 08:27:36.217644 temporian-0.1.1/temporian/core/operators/calendar/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.217781 temporian-0.1.1/temporian/core/operators/calendar/__init__.py
--rw-r--r--   0        0        0     1257 2023-06-15 08:27:36.217967 temporian-0.1.1/temporian/core/operators/calendar/api_symbols.py
--rw-r--r--   0        0        0     2363 2023-06-15 08:27:36.218207 temporian-0.1.1/temporian/core/operators/calendar/base.py
--rw-r--r--   0        0        0     1715 2023-06-15 08:27:36.218611 temporian-0.1.1/temporian/core/operators/calendar/day_of_month.py
--rw-r--r--   0        0        0     1723 2023-06-15 08:27:36.218871 temporian-0.1.1/temporian/core/operators/calendar/day_of_week.py
--rw-r--r--   0        0        0     1707 2023-06-15 08:27:36.219183 temporian-0.1.1/temporian/core/operators/calendar/day_of_year.py
--rw-r--r--   0        0        0     1650 2023-06-15 08:27:36.219416 temporian-0.1.1/temporian/core/operators/calendar/hour.py
--rw-r--r--   0        0        0     1683 2023-06-15 08:27:36.220283 temporian-0.1.1/temporian/core/operators/calendar/iso_week.py
--rw-r--r--   0        0        0     1673 2023-06-15 08:27:36.220559 temporian-0.1.1/temporian/core/operators/calendar/minute.py
--rw-r--r--   0        0        0     1756 2023-06-15 08:27:36.220816 temporian-0.1.1/temporian/core/operators/calendar/month.py
--rw-r--r--   0        0        0     1670 2023-06-15 08:27:36.221009 temporian-0.1.1/temporian/core/operators/calendar/second.py
--rw-r--r--   0        0        0     1595 2023-06-15 08:27:36.221429 temporian-0.1.1/temporian/core/operators/calendar/year.py
--rw-r--r--   0        0        0    10818 2023-06-15 08:27:36.221832 temporian-0.1.1/temporian/core/operators/cast.py
--rw-r--r--   0        0        0     7062 2023-06-15 08:27:36.222095 temporian-0.1.1/temporian/core/operators/drop_index.py
--rw-r--r--   0        0        0     1997 2023-06-15 08:27:36.222445 temporian-0.1.1/temporian/core/operators/end.py
--rw-r--r--   0        0        0     3432 2023-06-15 08:27:36.222692 temporian-0.1.1/temporian/core/operators/filter.py
--rw-r--r--   0        0        0     4828 2023-06-15 08:27:36.222911 temporian-0.1.1/temporian/core/operators/glue.py
--rw-r--r--   0        0        0     2779 2023-06-15 08:27:36.223389 temporian-0.1.1/temporian/core/operators/lag.py
--rw-r--r--   0        0        0     3120 2023-06-15 08:27:36.223708 temporian-0.1.1/temporian/core/operators/leak.py
--rw-r--r--   0        0        0     2846 2023-06-15 08:27:36.224235 temporian-0.1.1/temporian/core/operators/prefix.py
--rw-r--r--   0        0        0     4622 2023-06-15 08:27:36.224516 temporian-0.1.1/temporian/core/operators/propagate.py
--rw-r--r--   0        0        0     6067 2023-06-15 08:27:36.224711 temporian-0.1.1/temporian/core/operators/rename.py
--rw-r--r--   0        0        0     3155 2023-06-15 08:27:36.225460 temporian-0.1.1/temporian/core/operators/resample.py
--rw-r--r--   0        0        0     1382 2023-06-15 08:27:36.225954 temporian-0.1.1/temporian/core/operators/scalar/BUILD
--rw-r--r--   0        0        0      776 2023-06-15 08:27:36.226160 temporian-0.1.1/temporian/core/operators/scalar/__init__.py
--rw-r--r--   0        0        0     1656 2023-06-15 08:27:36.226341 temporian-0.1.1/temporian/core/operators/scalar/api_symbols.py
--rw-r--r--   0        0        0     9495 2023-06-15 08:27:36.226770 temporian-0.1.1/temporian/core/operators/scalar/arithmetic_scalar.py
--rw-r--r--   0        0        0     4937 2023-06-15 08:27:36.227019 temporian-0.1.1/temporian/core/operators/scalar/base.py
--rw-r--r--   0        0        0     5828 2023-06-15 08:27:36.227477 temporian-0.1.1/temporian/core/operators/scalar/relational_scalar.py
--rw-r--r--   0        0        0     3766 2023-06-15 08:27:36.227736 temporian-0.1.1/temporian/core/operators/select.py
--rw-r--r--   0        0        0     3918 2023-06-15 08:27:36.228214 temporian-0.1.1/temporian/core/operators/since_last.py
--rw-r--r--   0        0        0      421 2023-06-15 08:27:36.228842 temporian-0.1.1/temporian/core/operators/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.228973 temporian-0.1.1/temporian/core/operators/test/__init__.py
--rw-r--r--   0        0        0     2671 2023-06-15 08:27:36.229211 temporian-0.1.1/temporian/core/operators/test/propagate_test.py
--rw-r--r--   0        0        0     3590 2023-06-15 08:27:36.229483 temporian-0.1.1/temporian/core/operators/tick.py
--rw-r--r--   0        0        0      566 2023-06-15 08:27:36.229817 temporian-0.1.1/temporian/core/operators/unary/BUILD
--rw-r--r--   0        0        0      600 2023-06-15 08:27:36.230034 temporian-0.1.1/temporian/core/operators/unary/__init__.py
--rw-r--r--   0        0        0      883 2023-06-15 08:27:36.230536 temporian-0.1.1/temporian/core/operators/unary/api_symbols.py
--rw-r--r--   0        0        0     7050 2023-06-15 08:27:36.230808 temporian-0.1.1/temporian/core/operators/unary/unary.py
--rw-r--r--   0        0        0     2338 2023-06-15 08:27:36.231356 temporian-0.1.1/temporian/core/operators/unique_timestamps.py
--rw-r--r--   0        0        0     3055 2023-06-15 08:27:36.231686 temporian-0.1.1/temporian/core/operators/window/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.231824 temporian-0.1.1/temporian/core/operators/window/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-15 08:27:36.231980 temporian-0.1.1/temporian/core/operators/window/api_symbols.py
--rw-r--r--   0        0        0     3381 2023-06-15 08:27:36.232381 temporian-0.1.1/temporian/core/operators/window/base.py
--rw-r--r--   0        0        0     2473 2023-06-15 08:27:36.232855 temporian-0.1.1/temporian/core/operators/window/moving_count.py
--rw-r--r--   0        0        0     2443 2023-06-15 08:27:36.233078 temporian-0.1.1/temporian/core/operators/window/moving_max.py
--rw-r--r--   0        0        0     2461 2023-06-15 08:27:36.233586 temporian-0.1.1/temporian/core/operators/window/moving_min.py
--rw-r--r--   0        0        0     2690 2023-06-15 08:27:36.233874 temporian-0.1.1/temporian/core/operators/window/moving_standard_deviation.py
--rw-r--r--   0        0        0     3089 2023-06-15 08:27:36.234145 temporian-0.1.1/temporian/core/operators/window/moving_sum.py
--rw-r--r--   0        0        0     2672 2023-06-15 08:27:36.234617 temporian-0.1.1/temporian/core/operators/window/simple_moving_average.py
--rw-r--r--   0        0        0      919 2023-06-15 08:27:36.234813 temporian-0.1.1/temporian/core/schedule.py
--rw-r--r--   0        0        0      833 2023-06-15 08:27:36.235357 temporian-0.1.1/temporian/core/serialization/BUILD
--rw-r--r--   0        0        0      614 2023-06-15 08:27:36.235662 temporian-0.1.1/temporian/core/serialization/__init__.py
--rw-r--r--   0        0        0      722 2023-06-15 08:27:36.235842 temporian-0.1.1/temporian/core/serialization/api_symbols.py
--rw-r--r--   0        0        0    14739 2023-06-15 08:27:36.236008 temporian-0.1.1/temporian/core/serialization/serialize.py
--rw-r--r--   0        0        0     2486 2023-06-15 08:27:36.236367 temporian-0.1.1/temporian/core/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.236751 temporian-0.1.1/temporian/core/test/__init__.py
--rw-r--r--   0        0        0     5783 2023-06-15 08:27:36.236982 temporian-0.1.1/temporian/core/test/evaluation_test.py
--rw-r--r--   0        0        0     6399 2023-06-15 08:27:36.237195 temporian-0.1.1/temporian/core/test/graph_test.py
--rw-r--r--   0        0        0    17489 2023-06-15 08:27:36.237475 temporian-0.1.1/temporian/core/test/magic_methods_test.py
--rw-r--r--   0        0        0     2428 2023-06-15 08:27:36.237678 temporian-0.1.1/temporian/core/test/operator_test.py
--rw-r--r--   0        0        0     3080 2023-06-15 08:27:36.237872 temporian-0.1.1/temporian/core/test/registered_operators_test.py
--rw-r--r--   0        0        0     7171 2023-06-15 08:27:36.238030 temporian-0.1.1/temporian/core/test/serialization_test.py
--rw-r--r--   0        0        0     7746 2023-06-15 08:27:36.238497 temporian-0.1.1/temporian/core/test/utils.py
--rw-r--r--   0        0        0      212 2023-06-15 08:27:36.238935 temporian-0.1.1/temporian/implementation/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.239073 temporian-0.1.1/temporian/implementation/__init__.py
--rw-r--r--   0        0        0      735 2023-06-15 08:27:36.239639 temporian-0.1.1/temporian/implementation/numpy/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.239727 temporian-0.1.1/temporian/implementation/numpy/__init__.py
--rw-r--r--   0        0        0     1039 2023-06-15 08:27:36.239961 temporian-0.1.1/temporian/implementation/numpy/data/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.240097 temporian-0.1.1/temporian/implementation/numpy/data/__init__.py
--rw-r--r--   0        0        0    16630 2023-06-15 08:27:36.240300 temporian-0.1.1/temporian/implementation/numpy/data/event_set.py
--rw-r--r--   0        0        0     6765 2023-06-15 08:27:36.240483 temporian-0.1.1/temporian/implementation/numpy/data/io.py
--rw-r--r--   0        0        0     9069 2023-06-15 08:27:36.240646 temporian-0.1.1/temporian/implementation/numpy/data/plotter.py
--rw-r--r--   0        0        0     7765 2023-06-15 08:27:36.240866 temporian-0.1.1/temporian/implementation/numpy/data/plotter_bokeh.py
--rw-r--r--   0        0        0     6186 2023-06-15 08:27:36.241229 temporian-0.1.1/temporian/implementation/numpy/data/plotter_matplotlib.py
--rw-r--r--   0        0        0     1047 2023-06-15 08:27:36.241444 temporian-0.1.1/temporian/implementation/numpy/data/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.241787 temporian-0.1.1/temporian/implementation/numpy/data/test/__init__.py
--rw-r--r--   0        0        0     1652 2023-06-15 08:27:36.241936 temporian-0.1.1/temporian/implementation/numpy/data/test/event_set_test.py
--rw-r--r--   0        0        0     4129 2023-06-15 08:27:36.242110 temporian-0.1.1/temporian/implementation/numpy/data/test/io_test.py
--rw-r--r--   0        0        0     1796 2023-06-15 08:27:36.242476 temporian-0.1.1/temporian/implementation/numpy/data/test/plotter_test.py
--rw-r--r--   0        0        0     3683 2023-06-15 08:27:36.242873 temporian-0.1.1/temporian/implementation/numpy/evaluation.py
--rw-r--r--   0        0        0     1655 2023-06-15 08:27:36.243356 temporian-0.1.1/temporian/implementation/numpy/implementation_lib.py
--rw-r--r--   0        0        0     8229 2023-06-15 08:27:36.243623 temporian-0.1.1/temporian/implementation/numpy/operators/BUILD
--rw-r--r--   0        0        0     3268 2023-06-15 08:27:36.243786 temporian-0.1.1/temporian/implementation/numpy/operators/__init__.py
--rw-r--r--   0        0        0     2683 2023-06-15 08:27:36.244189 temporian-0.1.1/temporian/implementation/numpy/operators/add_index.py
--rw-r--r--   0        0        0     7361 2023-06-15 08:27:36.244420 temporian-0.1.1/temporian/implementation/numpy/operators/base.py
--rw-r--r--   0        0        0     2066 2023-06-15 08:27:36.244639 temporian-0.1.1/temporian/implementation/numpy/operators/begin.py
--rw-r--r--   0        0        0     1444 2023-06-15 08:27:36.244888 temporian-0.1.1/temporian/implementation/numpy/operators/binary/BUILD
--rw-r--r--   0        0        0      772 2023-06-15 08:27:36.245141 temporian-0.1.1/temporian/implementation/numpy/operators/binary/__init__.py
--rw-r--r--   0        0        0     5119 2023-06-15 08:27:36.245495 temporian-0.1.1/temporian/implementation/numpy/operators/binary/arithmetic.py
--rw-r--r--   0        0        0     3170 2023-06-15 08:27:36.245641 temporian-0.1.1/temporian/implementation/numpy/operators/binary/base.py
--rw-r--r--   0        0        0     2457 2023-06-15 08:27:36.245788 temporian-0.1.1/temporian/implementation/numpy/operators/binary/logical.py
--rw-r--r--   0        0        0     3735 2023-06-15 08:27:36.246165 temporian-0.1.1/temporian/implementation/numpy/operators/binary/relational.py
--rw-r--r--   0        0        0     2726 2023-06-15 08:27:36.246647 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.246763 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/__init__.py
--rw-r--r--   0        0        0     2618 2023-06-15 08:27:36.247006 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/base.py
--rw-r--r--   0        0        0     1363 2023-06-15 08:27:36.247270 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/day_of_month.py
--rw-r--r--   0        0        0     1362 2023-06-15 08:27:36.247642 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/day_of_week.py
--rw-r--r--   0        0        0     1372 2023-06-15 08:27:36.247861 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/day_of_year.py
--rw-r--r--   0        0        0     1318 2023-06-15 08:27:36.248698 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/hour.py
--rw-r--r--   0        0        0     1353 2023-06-15 08:27:36.249000 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/iso_week.py
--rw-r--r--   0        0        0     1334 2023-06-15 08:27:36.250389 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/minute.py
--rw-r--r--   0        0        0     1326 2023-06-15 08:27:36.250628 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/month.py
--rw-r--r--   0        0        0     1334 2023-06-15 08:27:36.250861 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/second.py
--rw-r--r--   0        0        0     1318 2023-06-15 08:27:36.251132 temporian-0.1.1/temporian/implementation/numpy/operators/calendar/year.py
--rw-r--r--   0        0        0     4075 2023-06-15 08:27:36.251887 temporian-0.1.1/temporian/implementation/numpy/operators/cast.py
--rw-r--r--   0        0        0     3971 2023-06-15 08:27:36.252244 temporian-0.1.1/temporian/implementation/numpy/operators/drop_index.py
--rw-r--r--   0        0        0     2049 2023-06-15 08:27:36.252539 temporian-0.1.1/temporian/implementation/numpy/operators/end.py
--rw-r--r--   0        0        0     1531 2023-06-15 08:27:36.253113 temporian-0.1.1/temporian/implementation/numpy/operators/filter.py
--rw-r--r--   0        0        0     2250 2023-06-15 08:27:36.253344 temporian-0.1.1/temporian/implementation/numpy/operators/glue.py
--rw-r--r--   0        0        0     1842 2023-06-15 08:27:36.253519 temporian-0.1.1/temporian/implementation/numpy/operators/lag.py
--rw-r--r--   0        0        0     1957 2023-06-15 08:27:36.253802 temporian-0.1.1/temporian/implementation/numpy/operators/leak.py
--rw-r--r--   0        0        0     1551 2023-06-15 08:27:36.253948 temporian-0.1.1/temporian/implementation/numpy/operators/prefix.py
--rw-r--r--   0        0        0     2113 2023-06-15 08:27:36.254464 temporian-0.1.1/temporian/implementation/numpy/operators/propagate.py
--rw-r--r--   0        0        0     1766 2023-06-15 08:27:36.254629 temporian-0.1.1/temporian/implementation/numpy/operators/rename.py
--rw-r--r--   0        0        0     3990 2023-06-15 08:27:36.254790 temporian-0.1.1/temporian/implementation/numpy/operators/resample.py
--rw-r--r--   0        0        0     1155 2023-06-15 08:27:36.255014 temporian-0.1.1/temporian/implementation/numpy/operators/scalar/BUILD
--rw-r--r--   0        0        0      692 2023-06-15 08:27:36.255165 temporian-0.1.1/temporian/implementation/numpy/operators/scalar/__init__.py
--rw-r--r--   0        0        0     4182 2023-06-15 08:27:36.255365 temporian-0.1.1/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py
--rw-r--r--   0        0        0     2155 2023-06-15 08:27:36.255834 temporian-0.1.1/temporian/implementation/numpy/operators/scalar/base.py
--rw-r--r--   0        0        0     3125 2023-06-15 08:27:36.256040 temporian-0.1.1/temporian/implementation/numpy/operators/scalar/relational_scalar.py
--rw-r--r--   0        0        0     2245 2023-06-15 08:27:36.256437 temporian-0.1.1/temporian/implementation/numpy/operators/select.py
--rw-r--r--   0        0        0     2645 2023-06-15 08:27:36.256848 temporian-0.1.1/temporian/implementation/numpy/operators/since_last.py
--rw-r--r--   0        0        0    19769 2023-06-15 08:27:36.257331 temporian-0.1.1/temporian/implementation/numpy/operators/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.257453 temporian-0.1.1/temporian/implementation/numpy/operators/test/__init__.py
--rw-r--r--   0        0        0     6666 2023-06-15 08:27:36.257674 temporian-0.1.1/temporian/implementation/numpy/operators/test/add_index_test.py
--rw-r--r--   0        0        0    11587 2023-06-15 08:27:36.257928 temporian-0.1.1/temporian/implementation/numpy/operators/test/arithmetic_multi_index_test.py
--rw-r--r--   0        0        0    16938 2023-06-15 08:27:36.258218 temporian-0.1.1/temporian/implementation/numpy/operators/test/arithmetic_scalar_test.py
--rw-r--r--   0        0        0     9123 2023-06-15 08:27:36.258582 temporian-0.1.1/temporian/implementation/numpy/operators/test/arithmetic_test.py
--rw-r--r--   0        0        0     1594 2023-06-15 08:27:36.259089 temporian-0.1.1/temporian/implementation/numpy/operators/test/begin_test.py
--rw-r--r--   0        0        0     4726 2023-06-15 08:27:36.259280 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_day_of_month_test.py
--rw-r--r--   0        0        0     2559 2023-06-15 08:27:36.259537 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_day_of_week_test.py
--rw-r--r--   0        0        0     2688 2023-06-15 08:27:36.259771 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_day_of_year_test.py
--rw-r--r--   0        0        0     2429 2023-06-15 08:27:36.260179 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_hour_test.py
--rw-r--r--   0        0        0     3165 2023-06-15 08:27:36.260637 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_iso_week_test.py
--rw-r--r--   0        0        0     2560 2023-06-15 08:27:36.260844 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_minute_test.py
--rw-r--r--   0        0        0     2551 2023-06-15 08:27:36.261099 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_month_test.py
--rw-r--r--   0        0        0     2486 2023-06-15 08:27:36.261263 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_second_test.py
--rw-r--r--   0        0        0     2557 2023-06-15 08:27:36.261682 temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_year_test.py
--rw-r--r--   0        0        0    10110 2023-06-15 08:27:36.262108 temporian-0.1.1/temporian/implementation/numpy/operators/test/cast_test.py
--rw-r--r--   0        0        0     7852 2023-06-15 08:27:36.262319 temporian-0.1.1/temporian/implementation/numpy/operators/test/drop_index_test.py
--rw-r--r--   0        0        0     1580 2023-06-15 08:27:36.262892 temporian-0.1.1/temporian/implementation/numpy/operators/test/end_test.py
--rw-r--r--   0        0        0     2913 2023-06-15 08:27:36.263084 temporian-0.1.1/temporian/implementation/numpy/operators/test/filter_test.py
--rw-r--r--   0        0        0     4312 2023-06-15 08:27:36.263598 temporian-0.1.1/temporian/implementation/numpy/operators/test/glue_test.py
--rw-r--r--   0        0        0     1707 2023-06-15 08:27:36.264180 temporian-0.1.1/temporian/implementation/numpy/operators/test/lag_test.py
--rw-r--r--   0        0        0     1770 2023-06-15 08:27:36.264454 temporian-0.1.1/temporian/implementation/numpy/operators/test/leak_test.py
--rw-r--r--   0        0        0     3694 2023-06-15 08:27:36.264976 temporian-0.1.1/temporian/implementation/numpy/operators/test/logical_test.py
--rw-r--r--   0        0        0     7859 2023-06-15 08:27:36.265142 temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_count_test.py
--rw-r--r--   0        0        0     3109 2023-06-15 08:27:36.265797 temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_max_test.py
--rw-r--r--   0        0        0     3093 2023-06-15 08:27:36.266076 temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_min_test.py
--rw-r--r--   0        0        0     8171 2023-06-15 08:27:36.266565 temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_standard_deviation_test.py
--rw-r--r--   0        0        0     9618 2023-06-15 08:27:36.267003 temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_sum_test.py
--rw-r--r--   0        0        0     2121 2023-06-15 08:27:36.267206 temporian-0.1.1/temporian/implementation/numpy/operators/test/prefix_test.py
--rw-r--r--   0        0        0     2365 2023-06-15 08:27:36.267866 temporian-0.1.1/temporian/implementation/numpy/operators/test/propagate_test.py
--rw-r--r--   0        0        0     7212 2023-06-15 08:27:36.268072 temporian-0.1.1/temporian/implementation/numpy/operators/test/relational_scalar_test.py
--rw-r--r--   0        0        0     7711 2023-06-15 08:27:36.268731 temporian-0.1.1/temporian/implementation/numpy/operators/test/relational_test.py
--rw-r--r--   0        0        0    10515 2023-06-15 08:27:36.268984 temporian-0.1.1/temporian/implementation/numpy/operators/test/rename_test.py
--rw-r--r--   0        0        0     2630 2023-06-15 08:27:36.269522 temporian-0.1.1/temporian/implementation/numpy/operators/test/resample_test.py
--rw-r--r--   0        0        0     5068 2023-06-15 08:27:36.269745 temporian-0.1.1/temporian/implementation/numpy/operators/test/select_test.py
--rw-r--r--   0        0        0     9448 2023-06-15 08:27:36.270244 temporian-0.1.1/temporian/implementation/numpy/operators/test/simple_moving_average_test.py
--rw-r--r--   0        0        0     2930 2023-06-15 08:27:36.270489 temporian-0.1.1/temporian/implementation/numpy/operators/test/since_last_test.py
--rw-r--r--   0        0        0     1751 2023-06-15 08:27:36.270856 temporian-0.1.1/temporian/implementation/numpy/operators/test/test_util.py
--rw-r--r--   0        0        0     3372 2023-06-15 08:27:36.271084 temporian-0.1.1/temporian/implementation/numpy/operators/test/tick_test.py
--rw-r--r--   0        0        0     7661 2023-06-15 08:27:36.271465 temporian-0.1.1/temporian/implementation/numpy/operators/test/unary_test.py
--rw-r--r--   0        0        0     1841 2023-06-15 08:27:36.271679 temporian-0.1.1/temporian/implementation/numpy/operators/test/unique_timestamps_test.py
--rw-r--r--   0        0        0     2568 2023-06-15 08:27:36.272178 temporian-0.1.1/temporian/implementation/numpy/operators/tick.py
--rw-r--r--   0        0        0     2778 2023-06-15 08:27:36.272379 temporian-0.1.1/temporian/implementation/numpy/operators/unary.py
--rw-r--r--   0        0        0     1937 2023-06-15 08:27:36.272872 temporian-0.1.1/temporian/implementation/numpy/operators/unique_timestamps.py
--rw-r--r--   0        0        0     2521 2023-06-15 08:27:36.273365 temporian-0.1.1/temporian/implementation/numpy/operators/window/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.273482 temporian-0.1.1/temporian/implementation/numpy/operators/window/__init__.py
--rw-r--r--   0        0        0     3319 2023-06-15 08:27:36.273707 temporian-0.1.1/temporian/implementation/numpy/operators/window/base.py
--rw-r--r--   0        0        0     1217 2023-06-15 08:27:36.273960 temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_count.py
--rw-r--r--   0        0        0     1203 2023-06-15 08:27:36.274187 temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_max.py
--rw-r--r--   0        0        0     1203 2023-06-15 08:27:36.274655 temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_min.py
--rw-r--r--   0        0        0     1304 2023-06-15 08:27:36.274918 temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_standard_deviation.py
--rw-r--r--   0        0        0     1203 2023-06-15 08:27:36.275399 temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_sum.py
--rw-r--r--   0        0        0     1276 2023-06-15 08:27:36.275607 temporian-0.1.1/temporian/implementation/numpy/operators/window/simple_moving_average.py
--rw-r--r--   0        0        0      429 2023-06-15 08:27:36.276278 temporian-0.1.1/temporian/implementation/numpy/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.276396 temporian-0.1.1/temporian/implementation/numpy/test/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-15 08:27:36.276505 temporian-0.1.1/temporian/implementation/numpy/test/registered_operators_test.py
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.276856 temporian-0.1.1/temporian/implementation/numpy/utils.py
--rw-r--r--   0        0        0       92 2023-06-15 08:27:36.277103 temporian-0.1.1/temporian/implementation/numpy_cc/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.277241 temporian-0.1.1/temporian/implementation/numpy_cc/__init__.py
--rw-r--r--   0        0        0      730 2023-06-15 08:27:36.277391 temporian-0.1.1/temporian/implementation/numpy_cc/operators/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.277590 temporian-0.1.1/temporian/implementation/numpy_cc/operators/__init__.py
--rw-r--r--   0        0        0      425 2023-06-15 08:27:36.277945 temporian-0.1.1/temporian/implementation/numpy_cc/operators/pyinit.cc
--rw-r--r--   0        0        0     1581 2023-06-15 08:27:36.278486 temporian-0.1.1/temporian/implementation/numpy_cc/operators/resample.cc
--rw-r--r--   0        0        0      105 2023-06-15 08:27:36.278722 temporian-0.1.1/temporian/implementation/numpy_cc/operators/resample.h
--rw-r--r--   0        0        0     1496 2023-06-15 08:27:36.278993 temporian-0.1.1/temporian/implementation/numpy_cc/operators/since_last.cc
--rw-r--r--   0        0        0      107 2023-06-15 08:27:36.279199 temporian-0.1.1/temporian/implementation/numpy_cc/operators/since_last.h
--rw-r--r--   0        0        0    14829 2023-06-15 08:27:36.279588 temporian-0.1.1/temporian/implementation/numpy_cc/operators/window.cc
--rw-r--r--   0        0        0      103 2023-06-15 08:27:36.279835 temporian-0.1.1/temporian/implementation/numpy_cc/operators/window.h
--rw-r--r--   0        0        0      922 2023-06-15 08:27:36.280154 temporian-0.1.1/temporian/io/BUILD
--rw-r--r--   0        0        0      607 2023-06-15 08:27:36.280415 temporian-0.1.1/temporian/io/__init__.py
--rw-r--r--   0        0        0      771 2023-06-15 08:27:36.280575 temporian-0.1.1/temporian/io/api_symbols.py
--rw-r--r--   0        0        0     2066 2023-06-15 08:27:36.280921 temporian-0.1.1/temporian/io/csv.py
--rw-r--r--   0        0        0     4244 2023-06-15 08:27:36.281319 temporian-0.1.1/temporian/io/pandas.py
--rw-r--r--   0        0        0      410 2023-06-15 08:27:36.281931 temporian-0.1.1/temporian/io/test/BUILD
--rw-r--r--   0        0        0    17524 2023-06-15 08:27:36.282142 temporian-0.1.1/temporian/io/test/pandas_test.py
--rw-r--r--   0        0        0      257 2023-06-15 08:27:36.282344 temporian-0.1.1/temporian/proto/BUILD
--rw-r--r--   0        0        0      576 2023-06-15 08:27:36.282649 temporian-0.1.1/temporian/proto/__init__.py
--rw-r--r--   0        0        0     4754 2023-06-15 08:27:36.282950 temporian-0.1.1/temporian/proto/core.proto
--rw-r--r--   0        0        0     1055 2023-06-15 08:27:36.283213 temporian-0.1.1/temporian/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.283375 temporian-0.1.1/temporian/test/__init__.py
--rw-r--r--   0        0        0     5156 2023-06-15 08:27:36.283524 temporian-0.1.1/temporian/test/api_test.py
--rw-r--r--   0        0        0     3332 2023-06-15 08:27:36.283856 temporian-0.1.1/temporian/test/docstring_test.py
--rw-r--r--   0        0        0     1863 2023-06-15 08:27:36.284469 temporian-0.1.1/temporian/test/io_test.py
--rw-r--r--   0        0        0     4492 2023-06-15 08:27:36.284783 temporian-0.1.1/temporian/test/prototype_test_numpy.py
--rw-r--r--   0        0        0      151 2023-06-15 08:27:36.285112 temporian-0.1.1/temporian/test/test_data/BUILD
--rw-r--r--   0        0        0       78 2023-06-15 08:27:36.285604 temporian-0.1.1/temporian/test/test_data/io/input.csv
--rw-r--r--   0        0        0      100 2023-06-15 08:27:36.285800 temporian-0.1.1/temporian/test/test_data/prototype/left_event.csv
--rw-r--r--   0        0        0      124 2023-06-15 08:27:36.286235 temporian-0.1.1/temporian/test/test_data/prototype/output_event.csv
--rw-r--r--   0        0        0       99 2023-06-15 08:27:36.286507 temporian-0.1.1/temporian/test/test_data/prototype/right_event.csv
--rw-r--r--   0        0        0      448 2023-06-15 08:27:36.286862 temporian-0.1.1/temporian/utils/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.287162 temporian-0.1.1/temporian/utils/__init__.py
--rw-r--r--   0        0        0     1615 2023-06-15 08:27:36.287385 temporian-0.1.1/temporian/utils/compile.bzl
--rw-r--r--   0        0        0       70 2023-06-15 08:27:36.287559 temporian-0.1.1/temporian/utils/config.py
--rw-r--r--   0        0        0      587 2023-06-15 08:27:36.287696 temporian-0.1.1/temporian/utils/string.py
--rw-r--r--   0        0        0      323 2023-06-15 08:27:36.288260 temporian-0.1.1/temporian/utils/test/BUILD
--rw-r--r--   0        0        0        0 2023-06-15 08:27:36.288348 temporian-0.1.1/temporian/utils/test/__init__.py
--rw-r--r--   0        0        0     1089 2023-06-15 08:27:36.288525 temporian-0.1.1/temporian/utils/test/string_test.py
--rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 temporian-0.1.1/setup.py
--rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 temporian-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-13 12:55:43.426290 temporian-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3304 2023-07-13 12:55:43.426430 temporian-0.1.2/README.md
+-rw-r--r--   0        0        0     3627 2023-07-13 12:55:43.428844 temporian-0.1.2/config/build.py
+-rw-r--r--   0        0        0     2769 2023-07-13 12:55:43.481702 temporian-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2906 2023-07-13 12:55:43.482010 temporian-0.1.2/temporian/BUILD
+-rw-r--r--   0        0        0     7271 2023-07-13 12:55:43.482166 temporian-0.1.2/temporian/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-13 12:55:43.482419 temporian-0.1.2/temporian/beam/BUILD
+-rw-r--r--   0        0        0     1349 2023-07-13 12:55:43.482560 temporian-0.1.2/temporian/beam/__init__.py
+-rw-r--r--   0        0        0     5170 2023-07-13 12:55:43.482707 temporian-0.1.2/temporian/beam/evaluation.py
+-rw-r--r--   0        0        0     1837 2023-07-13 12:55:43.482829 temporian-0.1.2/temporian/beam/implementation_lib.py
+-rw-r--r--   0        0        0    11407 2023-07-13 12:55:43.482999 temporian-0.1.2/temporian/beam/io.py
+-rw-r--r--   0        0        0     1160 2023-07-13 12:55:43.483434 temporian-0.1.2/temporian/beam/operators/BUILD
+-rw-r--r--   0        0        0      867 2023-07-13 12:55:43.483750 temporian-0.1.2/temporian/beam/operators/__init__.py
+-rw-r--r--   0        0        0     5590 2023-07-13 12:55:43.483968 temporian-0.1.2/temporian/beam/operators/add_index.py
+-rw-r--r--   0        0        0     1184 2023-07-13 12:55:43.484418 temporian-0.1.2/temporian/beam/operators/base.py
+-rw-r--r--   0        0        0     1830 2023-07-13 12:55:43.484562 temporian-0.1.2/temporian/beam/operators/select.py
+-rw-r--r--   0        0        0      691 2023-07-13 12:55:43.484737 temporian-0.1.2/temporian/beam/operators/test/BUILD
+-rw-r--r--   0        0        0     2252 2023-07-13 12:55:43.485088 temporian-0.1.2/temporian/beam/operators/test/add_index_test.py
+-rw-r--r--   0        0        0     2205 2023-07-13 12:55:43.485231 temporian-0.1.2/temporian/beam/operators/test/select_test.py
+-rw-r--r--   0        0        0      573 2023-07-13 12:55:43.485539 temporian-0.1.2/temporian/beam/operators/window/BUILD
+-rw-r--r--   0        0        0     1976 2023-07-13 12:55:43.485697 temporian-0.1.2/temporian/beam/operators/window/moving_sum.py
+-rw-r--r--   0        0        0      404 2023-07-13 12:55:43.486200 temporian-0.1.2/temporian/beam/operators/window/test/BUILD
+-rw-r--r--   0        0        0     1649 2023-07-13 12:55:43.486371 temporian-0.1.2/temporian/beam/operators/window/test/moving_sum_test.py
+-rw-r--r--   0        0        0     1285 2023-07-13 12:55:43.486810 temporian-0.1.2/temporian/beam/test/BUILD
+-rw-r--r--   0        0        0     1713 2023-07-13 12:55:43.486954 temporian-0.1.2/temporian/beam/test/evaluation_test.py
+-rw-r--r--   0        0        0     3762 2023-07-13 12:55:43.487341 temporian-0.1.2/temporian/beam/test/io_test.py
+-rw-r--r--   0        0        0     2789 2023-07-13 12:55:43.487556 temporian-0.1.2/temporian/beam/test/utils.py
+-rw-r--r--   0        0        0     1763 2023-07-13 12:55:43.487985 temporian-0.1.2/temporian/core/BUILD
+-rw-r--r--   0        0        0      576 2023-07-13 12:55:43.488133 temporian-0.1.2/temporian/core/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-13 12:55:43.488348 temporian-0.1.2/temporian/core/compilation.py
+-rw-r--r--   0        0        0      912 2023-07-13 12:55:43.488617 temporian-0.1.2/temporian/core/data/BUILD
+-rw-r--r--   0        0        0      576 2023-07-13 12:55:43.488747 temporian-0.1.2/temporian/core/data/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-13 12:55:43.489117 temporian-0.1.2/temporian/core/data/dtype.py
+-rw-r--r--   0        0        0     6026 2023-07-13 12:55:43.489346 temporian-0.1.2/temporian/core/data/duration.py
+-rw-r--r--   0        0        0     6378 2023-07-13 12:55:43.489566 temporian-0.1.2/temporian/core/data/duration_utils.py
+-rw-r--r--   0        0        0    11449 2023-07-13 12:55:43.489822 temporian-0.1.2/temporian/core/data/node.py
+-rw-r--r--   0        0        0     3905 2023-07-13 12:55:43.490056 temporian-0.1.2/temporian/core/data/schema.py
+-rw-r--r--   0        0        0      382 2023-07-13 12:55:43.490399 temporian-0.1.2/temporian/core/data/test/BUILD
+-rw-r--r--   0        0        0     1968 2023-07-13 12:55:43.490598 temporian-0.1.2/temporian/core/data/test/node_test.py
+-rw-r--r--   0        0        0    14622 2023-07-13 12:55:43.490837 temporian-0.1.2/temporian/core/evaluation.py
+-rw-r--r--   0        0        0    12130 2023-07-13 12:55:43.491064 temporian-0.1.2/temporian/core/graph.py
+-rw-r--r--   0        0        0    11770 2023-07-13 12:55:43.491328 temporian-0.1.2/temporian/core/mixins.py
+-rw-r--r--   0        0        0     1325 2023-07-13 12:55:43.491639 temporian-0.1.2/temporian/core/operator_lib.py
+-rw-r--r--   0        0        0     7222 2023-07-13 12:55:43.491908 temporian-0.1.2/temporian/core/operators/BUILD
+-rw-r--r--   0        0        0      594 2023-07-13 12:55:43.492066 temporian-0.1.2/temporian/core/operators/__init__.py
+-rw-r--r--   0        0        0     9598 2023-07-13 12:55:43.492602 temporian-0.1.2/temporian/core/operators/add_index.py
+-rw-r--r--   0        0        0    12445 2023-07-13 12:55:43.492931 temporian-0.1.2/temporian/core/operators/base.py
+-rw-r--r--   0        0        0     2521 2023-07-13 12:55:43.493380 temporian-0.1.2/temporian/core/operators/begin.py
+-rw-r--r--   0        0        0     1606 2023-07-13 12:55:43.493581 temporian-0.1.2/temporian/core/operators/binary/BUILD
+-rw-r--r--   0        0        0     1373 2023-07-13 12:55:43.493950 temporian-0.1.2/temporian/core/operators/binary/__init__.py
+-rw-r--r--   0        0        0    16492 2023-07-13 12:55:43.494332 temporian-0.1.2/temporian/core/operators/binary/arithmetic.py
+-rw-r--r--   0        0        0     4067 2023-07-13 12:55:43.494651 temporian-0.1.2/temporian/core/operators/binary/base.py
+-rw-r--r--   0        0        0     6551 2023-07-13 12:55:43.495054 temporian-0.1.2/temporian/core/operators/binary/logical.py
+-rw-r--r--   0        0        0    10650 2023-07-13 12:55:43.495191 temporian-0.1.2/temporian/core/operators/binary/relational.py
+-rw-r--r--   0        0        0     2898 2023-07-13 12:55:43.495621 temporian-0.1.2/temporian/core/operators/calendar/BUILD
+-rw-r--r--   0        0        0     1284 2023-07-13 12:55:43.495768 temporian-0.1.2/temporian/core/operators/calendar/__init__.py
+-rw-r--r--   0        0        0     2372 2023-07-13 12:55:43.496180 temporian-0.1.2/temporian/core/operators/calendar/base.py
+-rw-r--r--   0        0        0     2216 2023-07-13 12:55:43.496378 temporian-0.1.2/temporian/core/operators/calendar/day_of_month.py
+-rw-r--r--   0        0        0     2220 2023-07-13 12:55:43.496590 temporian-0.1.2/temporian/core/operators/calendar/day_of_week.py
+-rw-r--r--   0        0        0     2208 2023-07-13 12:55:43.496777 temporian-0.1.2/temporian/core/operators/calendar/day_of_year.py
+-rw-r--r--   0        0        0     2159 2023-07-13 12:55:43.496908 temporian-0.1.2/temporian/core/operators/calendar/hour.py
+-rw-r--r--   0        0        0     2245 2023-07-13 12:55:43.497074 temporian-0.1.2/temporian/core/operators/calendar/iso_week.py
+-rw-r--r--   0        0        0     2223 2023-07-13 12:55:43.497208 temporian-0.1.2/temporian/core/operators/calendar/minute.py
+-rw-r--r--   0        0        0     2269 2023-07-13 12:55:43.497631 temporian-0.1.2/temporian/core/operators/calendar/month.py
+-rw-r--r--   0        0        0     2224 2023-07-13 12:55:43.497775 temporian-0.1.2/temporian/core/operators/calendar/second.py
+-rw-r--r--   0        0        0     2117 2023-07-13 12:55:43.498148 temporian-0.1.2/temporian/core/operators/calendar/year.py
+-rw-r--r--   0        0        0    11395 2023-07-13 12:55:43.498511 temporian-0.1.2/temporian/core/operators/cast.py
+-rw-r--r--   0        0        0     7941 2023-07-13 12:55:43.498710 temporian-0.1.2/temporian/core/operators/drop_index.py
+-rw-r--r--   0        0        0     2499 2023-07-13 12:55:43.499111 temporian-0.1.2/temporian/core/operators/end.py
+-rw-r--r--   0        0        0     2679 2023-07-13 12:55:43.499369 temporian-0.1.2/temporian/core/operators/enumerate.py
+-rw-r--r--   0        0        0     4142 2023-07-13 12:55:43.499520 temporian-0.1.2/temporian/core/operators/filter.py
+-rw-r--r--   0        0        0     6282 2023-07-13 12:55:43.499957 temporian-0.1.2/temporian/core/operators/glue.py
+-rw-r--r--   0        0        0     7362 2023-07-13 12:55:43.500098 temporian-0.1.2/temporian/core/operators/join.py
+-rw-r--r--   0        0        0     3142 2023-07-13 12:55:43.500312 temporian-0.1.2/temporian/core/operators/lag.py
+-rw-r--r--   0        0        0     3522 2023-07-13 12:55:43.500510 temporian-0.1.2/temporian/core/operators/leak.py
+-rw-r--r--   0        0        0     3182 2023-07-13 12:55:43.500729 temporian-0.1.2/temporian/core/operators/prefix.py
+-rw-r--r--   0        0        0     6139 2023-07-13 12:55:43.500884 temporian-0.1.2/temporian/core/operators/propagate.py
+-rw-r--r--   0        0        0     7050 2023-07-13 12:55:43.501203 temporian-0.1.2/temporian/core/operators/rename.py
+-rw-r--r--   0        0        0     3111 2023-07-13 12:55:43.501575 temporian-0.1.2/temporian/core/operators/resample.py
+-rw-r--r--   0        0        0     1240 2023-07-13 12:55:43.501760 temporian-0.1.2/temporian/core/operators/scalar/BUILD
+-rw-r--r--   0        0        0     1378 2023-07-13 12:55:43.502068 temporian-0.1.2/temporian/core/operators/scalar/__init__.py
+-rw-r--r--   0        0        0    14450 2023-07-13 12:55:43.502402 temporian-0.1.2/temporian/core/operators/scalar/arithmetic_scalar.py
+-rw-r--r--   0        0        0     5105 2023-07-13 12:55:43.502547 temporian-0.1.2/temporian/core/operators/scalar/base.py
+-rw-r--r--   0        0        0     9555 2023-07-13 12:55:43.502919 temporian-0.1.2/temporian/core/operators/scalar/relational_scalar.py
+-rw-r--r--   0        0        0     4775 2023-07-13 12:55:43.503171 temporian-0.1.2/temporian/core/operators/select.py
+-rw-r--r--   0        0        0     3633 2023-07-13 12:55:43.503387 temporian-0.1.2/temporian/core/operators/since_last.py
+-rw-r--r--   0        0        0      703 2023-07-13 12:55:43.503825 temporian-0.1.2/temporian/core/operators/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.503918 temporian-0.1.2/temporian/core/operators/test/__init__.py
+-rw-r--r--   0        0        0     2697 2023-07-13 12:55:43.504042 temporian-0.1.2/temporian/core/operators/test/join_test.py
+-rw-r--r--   0        0        0     2722 2023-07-13 12:55:43.504436 temporian-0.1.2/temporian/core/operators/test/propagate_test.py
+-rw-r--r--   0        0        0     3902 2023-07-13 12:55:43.504650 temporian-0.1.2/temporian/core/operators/tick.py
+-rw-r--r--   0        0        0     3421 2023-07-13 12:55:43.504877 temporian-0.1.2/temporian/core/operators/timestamps.py
+-rw-r--r--   0        0        0     9760 2023-07-13 12:55:43.505059 temporian-0.1.2/temporian/core/operators/unary.py
+-rw-r--r--   0        0        0     2607 2023-07-13 12:55:43.505373 temporian-0.1.2/temporian/core/operators/unique_timestamps.py
+-rw-r--r--   0        0        0     3104 2023-07-13 12:55:43.505634 temporian-0.1.2/temporian/core/operators/window/BUILD
+-rw-r--r--   0        0        0     1192 2023-07-13 12:55:43.505870 temporian-0.1.2/temporian/core/operators/window/__init__.py
+-rw-r--r--   0        0        0     3398 2023-07-13 12:55:43.506103 temporian-0.1.2/temporian/core/operators/window/base.py
+-rw-r--r--   0        0        0     4284 2023-07-13 12:55:43.506294 temporian-0.1.2/temporian/core/operators/window/moving_count.py
+-rw-r--r--   0        0        0     3075 2023-07-13 12:55:43.506581 temporian-0.1.2/temporian/core/operators/window/moving_max.py
+-rw-r--r--   0        0        0     3122 2023-07-13 12:55:43.506771 temporian-0.1.2/temporian/core/operators/window/moving_min.py
+-rw-r--r--   0        0        0     3357 2023-07-13 12:55:43.507000 temporian-0.1.2/temporian/core/operators/window/moving_standard_deviation.py
+-rw-r--r--   0        0        0     4164 2023-07-13 12:55:43.507187 temporian-0.1.2/temporian/core/operators/window/moving_sum.py
+-rw-r--r--   0        0        0     3333 2023-07-13 12:55:43.507387 temporian-0.1.2/temporian/core/operators/window/simple_moving_average.py
+-rw-r--r--   0        0        0     1099 2023-07-13 12:55:43.507683 temporian-0.1.2/temporian/core/schedule.py
+-rw-r--r--   0        0        0    22379 2023-07-13 12:55:43.507944 temporian-0.1.2/temporian/core/serialization.py
+-rw-r--r--   0        0        0     2855 2023-07-13 12:55:43.508201 temporian-0.1.2/temporian/core/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.508343 temporian-0.1.2/temporian/core/test/__init__.py
+-rw-r--r--   0        0        0     5353 2023-07-13 12:55:43.508531 temporian-0.1.2/temporian/core/test/compilation_test.py
+-rw-r--r--   0        0        0     7511 2023-07-13 12:55:43.508692 temporian-0.1.2/temporian/core/test/evaluation_test.py
+-rw-r--r--   0        0        0     8004 2023-07-13 12:55:43.509067 temporian-0.1.2/temporian/core/test/graph_test.py
+-rw-r--r--   0        0        0    23290 2023-07-13 12:55:43.509251 temporian-0.1.2/temporian/core/test/magic_methods_test.py
+-rw-r--r--   0        0        0     2428 2023-07-13 12:55:43.509414 temporian-0.1.2/temporian/core/test/operator_test.py
+-rw-r--r--   0        0        0     3159 2023-07-13 12:55:43.509818 temporian-0.1.2/temporian/core/test/registered_operators_test.py
+-rw-r--r--   0        0        0    17955 2023-07-13 12:55:43.510073 temporian-0.1.2/temporian/core/test/serialization_test.py
+-rw-r--r--   0        0        0     7787 2023-07-13 12:55:43.510303 temporian-0.1.2/temporian/core/test/utils.py
+-rw-r--r--   0        0        0      211 2023-07-13 12:55:43.510611 temporian-0.1.2/temporian/implementation/BUILD
+-rw-r--r--   0        0        0      576 2023-07-13 12:55:43.510802 temporian-0.1.2/temporian/implementation/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-13 12:55:43.511086 temporian-0.1.2/temporian/implementation/numpy/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.511170 temporian-0.1.2/temporian/implementation/numpy/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-13 12:55:43.511326 temporian-0.1.2/temporian/implementation/numpy/data/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.511415 temporian-0.1.2/temporian/implementation/numpy/data/__init__.py
+-rw-r--r--   0        0        0    18226 2023-07-13 12:55:43.511584 temporian-0.1.2/temporian/implementation/numpy/data/event_set.py
+-rw-r--r--   0        0        0     6676 2023-07-13 12:55:43.511757 temporian-0.1.2/temporian/implementation/numpy/data/io.py
+-rw-r--r--   0        0        0     9985 2023-07-13 12:55:43.512130 temporian-0.1.2/temporian/implementation/numpy/data/plotter.py
+-rw-r--r--   0        0        0     7773 2023-07-13 12:55:43.512426 temporian-0.1.2/temporian/implementation/numpy/data/plotter_bokeh.py
+-rw-r--r--   0        0        0     6174 2023-07-13 12:55:43.512658 temporian-0.1.2/temporian/implementation/numpy/data/plotter_matplotlib.py
+-rw-r--r--   0        0        0     1040 2023-07-13 12:55:43.512905 temporian-0.1.2/temporian/implementation/numpy/data/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.513052 temporian-0.1.2/temporian/implementation/numpy/data/test/__init__.py
+-rw-r--r--   0        0        0     2786 2023-07-13 12:55:43.513162 temporian-0.1.2/temporian/implementation/numpy/data/test/event_set_test.py
+-rw-r--r--   0        0        0     4115 2023-07-13 12:55:43.513367 temporian-0.1.2/temporian/implementation/numpy/data/test/io_test.py
+-rw-r--r--   0        0        0     2536 2023-07-13 12:55:43.513627 temporian-0.1.2/temporian/implementation/numpy/data/test/plotter_test.py
+-rw-r--r--   0        0        0     3750 2023-07-13 12:55:43.513958 temporian-0.1.2/temporian/implementation/numpy/evaluation.py
+-rw-r--r--   0        0        0     1655 2023-07-13 12:55:43.514147 temporian-0.1.2/temporian/implementation/numpy/implementation_lib.py
+-rw-r--r--   0        0        0     9228 2023-07-13 12:55:43.514547 temporian-0.1.2/temporian/implementation/numpy/operators/BUILD
+-rw-r--r--   0        0        0     3453 2023-07-13 12:55:43.514695 temporian-0.1.2/temporian/implementation/numpy/operators/__init__.py
+-rw-r--r--   0        0        0     2651 2023-07-13 12:55:43.515087 temporian-0.1.2/temporian/implementation/numpy/operators/add_index.py
+-rw-r--r--   0        0        0     7627 2023-07-13 12:55:43.515248 temporian-0.1.2/temporian/implementation/numpy/operators/base.py
+-rw-r--r--   0        0        0     2175 2023-07-13 12:55:43.515628 temporian-0.1.2/temporian/implementation/numpy/operators/begin.py
+-rw-r--r--   0        0        0     1554 2023-07-13 12:55:43.515878 temporian-0.1.2/temporian/implementation/numpy/operators/binary/BUILD
+-rw-r--r--   0        0        0      772 2023-07-13 12:55:43.516073 temporian-0.1.2/temporian/implementation/numpy/operators/binary/__init__.py
+-rw-r--r--   0        0        0     5429 2023-07-13 12:55:43.516291 temporian-0.1.2/temporian/implementation/numpy/operators/binary/arithmetic.py
+-rw-r--r--   0        0        0     3478 2023-07-13 12:55:43.516533 temporian-0.1.2/temporian/implementation/numpy/operators/binary/base.py
+-rw-r--r--   0        0        0     2619 2023-07-13 12:55:43.516755 temporian-0.1.2/temporian/implementation/numpy/operators/binary/logical.py
+-rw-r--r--   0        0        0     4280 2023-07-13 12:55:43.516968 temporian-0.1.2/temporian/implementation/numpy/operators/binary/relational.py
+-rw-r--r--   0        0        0     2726 2023-07-13 12:55:43.517224 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.517371 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/__init__.py
+-rw-r--r--   0        0        0     2682 2023-07-13 12:55:43.517499 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/base.py
+-rw-r--r--   0        0        0     1363 2023-07-13 12:55:43.517708 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/day_of_month.py
+-rw-r--r--   0        0        0     1362 2023-07-13 12:55:43.518067 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/day_of_week.py
+-rw-r--r--   0        0        0     1372 2023-07-13 12:55:43.518203 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/day_of_year.py
+-rw-r--r--   0        0        0     1318 2023-07-13 12:55:43.518665 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/hour.py
+-rw-r--r--   0        0        0     1353 2023-07-13 12:55:43.518865 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/iso_week.py
+-rw-r--r--   0        0        0     1334 2023-07-13 12:55:43.519075 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/minute.py
+-rw-r--r--   0        0        0     1326 2023-07-13 12:55:43.519387 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/month.py
+-rw-r--r--   0        0        0     1334 2023-07-13 12:55:43.519529 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/second.py
+-rw-r--r--   0        0        0     1318 2023-07-13 12:55:43.519850 temporian-0.1.2/temporian/implementation/numpy/operators/calendar/year.py
+-rw-r--r--   0        0        0     4179 2023-07-13 12:55:43.520205 temporian-0.1.2/temporian/implementation/numpy/operators/cast.py
+-rw-r--r--   0        0        0     3955 2023-07-13 12:55:43.520413 temporian-0.1.2/temporian/implementation/numpy/operators/drop_index.py
+-rw-r--r--   0        0        0     2158 2023-07-13 12:55:43.520612 temporian-0.1.2/temporian/implementation/numpy/operators/end.py
+-rw-r--r--   0        0        0     1978 2023-07-13 12:55:43.520812 temporian-0.1.2/temporian/implementation/numpy/operators/enumerate.py
+-rw-r--r--   0        0        0     1639 2023-07-13 12:55:43.521075 temporian-0.1.2/temporian/implementation/numpy/operators/filter.py
+-rw-r--r--   0        0        0     2360 2023-07-13 12:55:43.521377 temporian-0.1.2/temporian/implementation/numpy/operators/glue.py
+-rw-r--r--   0        0        0     4528 2023-07-13 12:55:43.521579 temporian-0.1.2/temporian/implementation/numpy/operators/join.py
+-rw-r--r--   0        0        0     1951 2023-07-13 12:55:43.521781 temporian-0.1.2/temporian/implementation/numpy/operators/lag.py
+-rw-r--r--   0        0        0     2070 2023-07-13 12:55:43.522097 temporian-0.1.2/temporian/implementation/numpy/operators/leak.py
+-rw-r--r--   0        0        0     1551 2023-07-13 12:55:43.522248 temporian-0.1.2/temporian/implementation/numpy/operators/prefix.py
+-rw-r--r--   0        0        0     2114 2023-07-13 12:55:43.522625 temporian-0.1.2/temporian/implementation/numpy/operators/propagate.py
+-rw-r--r--   0        0        0     1756 2023-07-13 12:55:43.522832 temporian-0.1.2/temporian/implementation/numpy/operators/rename.py
+-rw-r--r--   0        0        0     4099 2023-07-13 12:55:43.523180 temporian-0.1.2/temporian/implementation/numpy/operators/resample.py
+-rw-r--r--   0        0        0     1272 2023-07-13 12:55:43.523423 temporian-0.1.2/temporian/implementation/numpy/operators/scalar/BUILD
+-rw-r--r--   0        0        0      692 2023-07-13 12:55:43.523568 temporian-0.1.2/temporian/implementation/numpy/operators/scalar/__init__.py
+-rw-r--r--   0        0        0     4499 2023-07-13 12:55:43.523953 temporian-0.1.2/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py
+-rw-r--r--   0        0        0     2591 2023-07-13 12:55:43.524096 temporian-0.1.2/temporian/implementation/numpy/operators/scalar/base.py
+-rw-r--r--   0        0        0     3613 2023-07-13 12:55:43.524460 temporian-0.1.2/temporian/implementation/numpy/operators/scalar/relational_scalar.py
+-rw-r--r--   0        0        0     2355 2023-07-13 12:55:43.524772 temporian-0.1.2/temporian/implementation/numpy/operators/select.py
+-rw-r--r--   0        0        0     2950 2023-07-13 12:55:43.524896 temporian-0.1.2/temporian/implementation/numpy/operators/since_last.py
+-rw-r--r--   0        0        0    21122 2023-07-13 12:55:43.525351 temporian-0.1.2/temporian/implementation/numpy/operators/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.525547 temporian-0.1.2/temporian/implementation/numpy/operators/test/__init__.py
+-rw-r--r--   0        0        0     6616 2023-07-13 12:55:43.525758 temporian-0.1.2/temporian/implementation/numpy/operators/test/add_index_test.py
+-rw-r--r--   0        0        0    11552 2023-07-13 12:55:43.525994 temporian-0.1.2/temporian/implementation/numpy/operators/test/arithmetic_multi_index_test.py
+-rw-r--r--   0        0        0    16866 2023-07-13 12:55:43.526221 temporian-0.1.2/temporian/implementation/numpy/operators/test/arithmetic_scalar_test.py
+-rw-r--r--   0        0        0     9083 2023-07-13 12:55:43.526469 temporian-0.1.2/temporian/implementation/numpy/operators/test/arithmetic_test.py
+-rw-r--r--   0        0        0     1580 2023-07-13 12:55:43.526676 temporian-0.1.2/temporian/implementation/numpy/operators/test/begin_test.py
+-rw-r--r--   0        0        0     4715 2023-07-13 12:55:43.527000 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_day_of_month_test.py
+-rw-r--r--   0        0        0     2559 2023-07-13 12:55:43.527211 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_day_of_week_test.py
+-rw-r--r--   0        0        0     2688 2023-07-13 12:55:43.527402 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_day_of_year_test.py
+-rw-r--r--   0        0        0     2429 2023-07-13 12:55:43.527561 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_hour_test.py
+-rw-r--r--   0        0        0     3165 2023-07-13 12:55:43.527894 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_iso_week_test.py
+-rw-r--r--   0        0        0     2560 2023-07-13 12:55:43.528037 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_minute_test.py
+-rw-r--r--   0        0        0     2551 2023-07-13 12:55:43.528449 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_month_test.py
+-rw-r--r--   0        0        0     2486 2023-07-13 12:55:43.528601 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_second_test.py
+-rw-r--r--   0        0        0     2557 2023-07-13 12:55:43.528963 temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_year_test.py
+-rw-r--r--   0        0        0    10396 2023-07-13 12:55:43.529291 temporian-0.1.2/temporian/implementation/numpy/operators/test/cast_test.py
+-rw-r--r--   0        0        0     7784 2023-07-13 12:55:43.529489 temporian-0.1.2/temporian/implementation/numpy/operators/test/drop_index_test.py
+-rw-r--r--   0        0        0     1566 2023-07-13 12:55:43.529699 temporian-0.1.2/temporian/implementation/numpy/operators/test/end_test.py
+-rw-r--r--   0        0        0     1975 2023-07-13 12:55:43.529895 temporian-0.1.2/temporian/implementation/numpy/operators/test/enumerate_test.py
+-rw-r--r--   0        0        0     2892 2023-07-13 12:55:43.530212 temporian-0.1.2/temporian/implementation/numpy/operators/test/filter_test.py
+-rw-r--r--   0        0        0     4285 2023-07-13 12:55:43.530364 temporian-0.1.2/temporian/implementation/numpy/operators/test/glue_test.py
+-rw-r--r--   0        0        0     3026 2023-07-13 12:55:43.530755 temporian-0.1.2/temporian/implementation/numpy/operators/test/join_test.py
+-rw-r--r--   0        0        0     1693 2023-07-13 12:55:43.531081 temporian-0.1.2/temporian/implementation/numpy/operators/test/lag_test.py
+-rw-r--r--   0        0        0     1756 2023-07-13 12:55:43.531275 temporian-0.1.2/temporian/implementation/numpy/operators/test/leak_test.py
+-rw-r--r--   0        0        0     3699 2023-07-13 12:55:43.531556 temporian-0.1.2/temporian/implementation/numpy/operators/test/logical_test.py
+-rw-r--r--   0        0        0     7851 2023-07-13 12:55:43.531708 temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_count_test.py
+-rw-r--r--   0        0        0     3109 2023-07-13 12:55:43.532078 temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_max_test.py
+-rw-r--r--   0        0        0     3093 2023-07-13 12:55:43.532238 temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_min_test.py
+-rw-r--r--   0        0        0     8162 2023-07-13 12:55:43.532467 temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_standard_deviation_test.py
+-rw-r--r--   0        0        0     9602 2023-07-13 12:55:43.532779 temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_sum_test.py
+-rw-r--r--   0        0        0     2113 2023-07-13 12:55:43.532942 temporian-0.1.2/temporian/implementation/numpy/operators/test/prefix_test.py
+-rw-r--r--   0        0        0     2353 2023-07-13 12:55:43.533274 temporian-0.1.2/temporian/implementation/numpy/operators/test/propagate_test.py
+-rw-r--r--   0        0        0     8633 2023-07-13 12:55:43.533572 temporian-0.1.2/temporian/implementation/numpy/operators/test/relational_scalar_test.py
+-rw-r--r--   0        0        0     9459 2023-07-13 12:55:43.533764 temporian-0.1.2/temporian/implementation/numpy/operators/test/relational_test.py
+-rw-r--r--   0        0        0    10493 2023-07-13 12:55:43.534114 temporian-0.1.2/temporian/implementation/numpy/operators/test/rename_test.py
+-rw-r--r--   0        0        0     2618 2023-07-13 12:55:43.534270 temporian-0.1.2/temporian/implementation/numpy/operators/test/resample_test.py
+-rw-r--r--   0        0        0     5033 2023-07-13 12:55:43.534630 temporian-0.1.2/temporian/implementation/numpy/operators/test/select_test.py
+-rw-r--r--   0        0        0     9440 2023-07-13 12:55:43.534783 temporian-0.1.2/temporian/implementation/numpy/operators/test/simple_moving_average_test.py
+-rw-r--r--   0        0        0     2922 2023-07-13 12:55:43.535180 temporian-0.1.2/temporian/implementation/numpy/operators/test/since_last_test.py
+-rw-r--r--   0        0        0     1880 2023-07-13 12:55:43.535389 temporian-0.1.2/temporian/implementation/numpy/operators/test/test_util.py
+-rw-r--r--   0        0        0     3372 2023-07-13 12:55:43.535724 temporian-0.1.2/temporian/implementation/numpy/operators/test/tick_test.py
+-rw-r--r--   0        0        0     2935 2023-07-13 12:55:43.535894 temporian-0.1.2/temporian/implementation/numpy/operators/test/timestamps_test.py
+-rw-r--r--   0        0        0     7646 2023-07-13 12:55:43.536267 temporian-0.1.2/temporian/implementation/numpy/operators/test/unary_test.py
+-rw-r--r--   0        0        0     1833 2023-07-13 12:55:43.536404 temporian-0.1.2/temporian/implementation/numpy/operators/test/unique_timestamps_test.py
+-rw-r--r--   0        0        0     2677 2023-07-13 12:55:43.536807 temporian-0.1.2/temporian/implementation/numpy/operators/tick.py
+-rw-r--r--   0        0        0     1955 2023-07-13 12:55:43.537009 temporian-0.1.2/temporian/implementation/numpy/operators/timestamps.py
+-rw-r--r--   0        0        0     2895 2023-07-13 12:55:43.537211 temporian-0.1.2/temporian/implementation/numpy/operators/unary.py
+-rw-r--r--   0        0        0     1937 2023-07-13 12:55:43.537424 temporian-0.1.2/temporian/implementation/numpy/operators/unique_timestamps.py
+-rw-r--r--   0        0        0     2521 2023-07-13 12:55:43.537803 temporian-0.1.2/temporian/implementation/numpy/operators/window/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.537889 temporian-0.1.2/temporian/implementation/numpy/operators/window/__init__.py
+-rw-r--r--   0        0        0     3783 2023-07-13 12:55:43.538038 temporian-0.1.2/temporian/implementation/numpy/operators/window/base.py
+-rw-r--r--   0        0        0     1217 2023-07-13 12:55:43.538168 temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_count.py
+-rw-r--r--   0        0        0     1203 2023-07-13 12:55:43.538540 temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_max.py
+-rw-r--r--   0        0        0     1203 2023-07-13 12:55:43.538683 temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_min.py
+-rw-r--r--   0        0        0     1304 2023-07-13 12:55:43.539039 temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_standard_deviation.py
+-rw-r--r--   0        0        0     1203 2023-07-13 12:55:43.539436 temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_sum.py
+-rw-r--r--   0        0        0     1276 2023-07-13 12:55:43.539632 temporian-0.1.2/temporian/implementation/numpy/operators/window/simple_moving_average.py
+-rw-r--r--   0        0        0      429 2023-07-13 12:55:43.539884 temporian-0.1.2/temporian/implementation/numpy/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.540068 temporian-0.1.2/temporian/implementation/numpy/test/__init__.py
+-rw-r--r--   0        0        0     3236 2023-07-13 12:55:43.540168 temporian-0.1.2/temporian/implementation/numpy/test/registered_operators_test.py
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.540308 temporian-0.1.2/temporian/implementation/numpy/utils.py
+-rw-r--r--   0        0        0       92 2023-07-13 12:55:43.540457 temporian-0.1.2/temporian/implementation/numpy_cc/BUILD
+-rw-r--r--   0        0        0      576 2023-07-13 12:55:43.540677 temporian-0.1.2/temporian/implementation/numpy_cc/__init__.py
+-rw-r--r--   0        0        0      839 2023-07-13 12:55:43.540983 temporian-0.1.2/temporian/implementation/numpy_cc/operators/BUILD
+-rw-r--r--   0        0        0      576 2023-07-13 12:55:43.541175 temporian-0.1.2/temporian/implementation/numpy_cc/operators/__init__.py
+-rw-r--r--   0        0        0     2952 2023-07-13 12:55:43.541483 temporian-0.1.2/temporian/implementation/numpy_cc/operators/join.cc
+-rw-r--r--   0        0        0       97 2023-07-13 12:55:43.541676 temporian-0.1.2/temporian/implementation/numpy_cc/operators/join.h
+-rw-r--r--   0        0        0      505 2023-07-13 12:55:43.541875 temporian-0.1.2/temporian/implementation/numpy_cc/operators/pyinit.cc
+-rw-r--r--   0        0        0     1581 2023-07-13 12:55:43.542092 temporian-0.1.2/temporian/implementation/numpy_cc/operators/resample.cc
+-rw-r--r--   0        0        0      105 2023-07-13 12:55:43.542405 temporian-0.1.2/temporian/implementation/numpy_cc/operators/resample.h
+-rw-r--r--   0        0        0     1496 2023-07-13 12:55:43.542539 temporian-0.1.2/temporian/implementation/numpy_cc/operators/since_last.cc
+-rw-r--r--   0        0        0      107 2023-07-13 12:55:43.542951 temporian-0.1.2/temporian/implementation/numpy_cc/operators/since_last.h
+-rw-r--r--   0        0        0    14829 2023-07-13 12:55:43.543299 temporian-0.1.2/temporian/implementation/numpy_cc/operators/window.cc
+-rw-r--r--   0        0        0      103 2023-07-13 12:55:43.543425 temporian-0.1.2/temporian/implementation/numpy_cc/operators/window.h
+-rw-r--r--   0        0        0      729 2023-07-13 12:55:43.543660 temporian-0.1.2/temporian/io/BUILD
+-rw-r--r--   0        0        0      769 2023-07-13 12:55:43.543808 temporian-0.1.2/temporian/io/__init__.py
+-rw-r--r--   0        0        0     3036 2023-07-13 12:55:43.544173 temporian-0.1.2/temporian/io/csv.py
+-rw-r--r--   0        0        0     5825 2023-07-13 12:55:43.544392 temporian-0.1.2/temporian/io/pandas.py
+-rw-r--r--   0        0        0      410 2023-07-13 12:55:43.544635 temporian-0.1.2/temporian/io/test/BUILD
+-rw-r--r--   0        0        0    16553 2023-07-13 12:55:43.544868 temporian-0.1.2/temporian/io/test/pandas_test.py
+-rw-r--r--   0        0        0      257 2023-07-13 12:55:43.545176 temporian-0.1.2/temporian/proto/BUILD
+-rw-r--r--   0        0        0      576 2023-07-13 12:55:43.545399 temporian-0.1.2/temporian/proto/__init__.py
+-rw-r--r--   0        0        0     4859 2023-07-13 12:55:43.545690 temporian-0.1.2/temporian/proto/core.proto
+-rw-r--r--   0        0        0     1462 2023-07-13 12:55:43.545949 temporian-0.1.2/temporian/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.546096 temporian-0.1.2/temporian/test/__init__.py
+-rw-r--r--   0        0        0     4461 2023-07-13 12:55:43.546251 temporian-0.1.2/temporian/test/api_beam_test.py
+-rw-r--r--   0        0        0     6291 2023-07-13 12:55:43.546462 temporian-0.1.2/temporian/test/api_test.py
+-rw-r--r--   0        0        0     3848 2023-07-13 12:55:43.546830 temporian-0.1.2/temporian/test/docstring_test.py
+-rw-r--r--   0        0        0     1789 2023-07-13 12:55:43.547042 temporian-0.1.2/temporian/test/io_test.py
+-rw-r--r--   0        0        0     4408 2023-07-13 12:55:43.547340 temporian-0.1.2/temporian/test/prototype_test_numpy.py
+-rw-r--r--   0        0        0      151 2023-07-13 12:55:43.547531 temporian-0.1.2/temporian/test/test_data/BUILD
+-rw-r--r--   0        0        0       78 2023-07-13 12:55:43.547707 temporian-0.1.2/temporian/test/test_data/io/input.csv
+-rw-r--r--   0        0        0      100 2023-07-13 12:55:43.547915 temporian-0.1.2/temporian/test/test_data/prototype/left_event.csv
+-rw-r--r--   0        0        0      124 2023-07-13 12:55:43.548284 temporian-0.1.2/temporian/test/test_data/prototype/output_event.csv
+-rw-r--r--   0        0        0       99 2023-07-13 12:55:43.548417 temporian-0.1.2/temporian/test/test_data/prototype/right_event.csv
+-rw-r--r--   0        0        0      448 2023-07-13 12:55:43.548901 temporian-0.1.2/temporian/utils/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.548988 temporian-0.1.2/temporian/utils/__init__.py
+-rw-r--r--   0        0        0     1615 2023-07-13 12:55:43.549109 temporian-0.1.2/temporian/utils/compile.bzl
+-rw-r--r--   0        0        0       70 2023-07-13 12:55:43.549239 temporian-0.1.2/temporian/utils/config.py
+-rw-r--r--   0        0        0      587 2023-07-13 12:55:43.549681 temporian-0.1.2/temporian/utils/string.py
+-rw-r--r--   0        0        0      323 2023-07-13 12:55:43.549859 temporian-0.1.2/temporian/utils/test/BUILD
+-rw-r--r--   0        0        0        0 2023-07-13 12:55:43.550182 temporian-0.1.2/temporian/utils/test/__init__.py
+-rw-r--r--   0        0        0     1089 2023-07-13 12:55:43.550291 temporian-0.1.2/temporian/utils/test/string_test.py
+-rw-r--r--   0        0        0     5923 1970-01-01 00:00:00.000000 temporian-0.1.2/setup.py
+-rw-r--r--   0        0        0     5216 1970-01-01 00:00:00.000000 temporian-0.1.2/PKG-INFO
```

### Comparing `temporian-0.1.1/LICENSE` & `temporian-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/README.md` & `temporian-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,81 @@
-<img src="https://github.com/google/temporian/blob/main/docs/src/assets/banner.png?raw=true" width="100%" alt="Temporian logo">
+<img src="docs/src/assets/banner.png" width="100%" alt="Temporian logo">
 
-![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg) ![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg) [![docs](https://readthedocs.org/projects/temporian/badge/?version=latest)](https://temporian.readthedocs.io/en/latest/?badge=latest)
+[![pypi](https://img.shields.io/pypi/v/temporian?color=blue)](https://pypi.org/project/temporian/)
+[![docs](https://readthedocs.org/projects/temporian/badge/?version=stable)](https://temporian.readthedocs.io/en/stable/?badge=stable)
+![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg)
+![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg)
+![publish](https://github.com/google/temporian/actions/workflows/publish.yaml/badge.svg)
 
-**Temporian** is a Python package for **feature engineering of temporal data**, focusing on **preventing common modeling errors** and providing a **simple and powerful API**, a first-class **iterative development** experience, and **efficient and well-tested implementations** of common and not-so-common temporal data preprocessing functions.
+**Temporian** is a Python library for **feature engineering** 🛠 and **data augmentation** ⚡ of **temporal data** 📈 (e.g. time-series, transactions) in **machine learning applications** 🤖.
+
+> **Warning**
+> Temporian development is in alpha.
+
+## Key features
+
+- Temporian operates natively on **multivariate** and **multi-index time-series** and **time-sequences** data. With Temporian, all temporal data processing is unified.
+
+- Temporian favors **iterative** and **interactive** development in Colab, where users can **easily visualize intermediate results** 📊 each step of the way.
+
+- Temporian introduces a novel mechanism to **prevent unwanted future leakage** and **training/serving skew** 😰. Temporian programs always return the same result in batch and in streaming mode.
+
+- Temporian programs can run seamlessly **in-process** in Python, on **large datasets using [Apache Beam](https://beam.apache.org/)** ☁️, and in **streaming for continuous** data ingestion.
+
+- Temporian's core is implemented **in C++** and **highly optimized** 🔥, so large amounts of data can be handled in-process. In some cases, Temporian can provide a speed-up in the order of 1000x compared to other libraries.
 
 ## Installation
 
-Temporian is available on PyPI. To install it, run:
+Temporian is available on [PyPI](https://pypi.org/project/temporian/). To install it, run:
 
 ```shell
 pip install temporian
 ```
 
-## Getting Started
+## Minimal example
+
+Consider the following dataset.
+
+```shell
+$ head sales.csv
+timestamp,store,price,count
+2022-01-01 00:00:00+00:00,CA,27.42,61.9
+2022-01-01 00:00:00+00:00,TX,98.55,18.02
+2022-01-02 00:00:00+00:00,CA,32.74,14.93
+2022-01-02 00:00:00+00:00,TX,48.69,83.99
+...
+```
 
-This is how a minimal end-to-end example looks like:
+We compute the weekly sales per store as follows.
 
 ```python
 import temporian as tp
 
-# Load data and create input node.
-evset = tp.from_csv("temporal_data.csv", timestamp_column="date")
-source = evset.node()
-
-# Apply operators to create a processing graph.
-sma = tp.simple_moving_average(source, window_length=tp.duration.days(7))
-
-# Run the graph.
-result_evset = sma.evaluate({source: evset})
-
-# Show output.
-print(result_evset)
-result_evset.plot()
-```
+input_data = tp.from_csv("sales.csv")
 
-This is an example `temporal_data.csv` to use with the code above:
-
-```
-date,feature_1,feature_2
-2023-01-01,10.0,3.0
-2023-01-02,20.0,4.0
-2023-02-01,30.0,5.0
-```
+# Define a Temporian program
+input_node = input_data.node()
+per_store = tp.set_index(input_node, "store")
+weekly_sum = tp.moving_sum(per_store["price"], window_length=tp.duration.days(7))
 
-Check the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to try it out!
+# Execute Temporian program
+output_data = weekly_sum.run({input_node: input_data})
 
-## Key features
+# Plot the result
+output_data.plot()
+```
 
-These are what set Temporian apart.
+![](docs/src/assets/frontpage_plot.png)
 
-- **Simple and powerful API**: Temporian exports high level operations making processing complex programs short and ready to read.
-- **Flexible data model**: Temporian models temporal data as a sequence of events, supporting non-uniform sampling timestamps seamlessly.
-- **Prevents modeling errors**: Temporian programs are guaranteed not to have future leakage unless explicitly specified, ensuring that models are not trained on future data.
-- **Iterative development**: Temporian can be used to develop preprocessing pipelines in Colab or local notebooks, allowing users to visualize results each step of the way to identify and correct errors early on.
-- **Efficient and well-tested implementations**: Temporian contains efficient and well-tested implementations of a variety of temporal data processing functions. For instance, our implementation of window operators is **x2000** faster than the same function implemented with NumPy.
-- **Wide range of preprocessing functions**: Temporian contains a wide range of preprocessing functions, including moving window operations, lagging, calendar features, arithmetic operations, index manipulation and propagation, resampling, and more. For a full list of the available operators, see the [operators documentation](https://temporian.readthedocs.io/en/stable/reference/).
+Check the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to try it out!
 
 ## Documentation
 
-The official documentation is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/).
+The documentation 📚 is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/). The [3 minutes to Temporian ⏰️](https://temporian.readthedocs.io/en/stable/3_minutes/) is the best way to start.
 
 ## Contributing
 
 Contributions to Temporian are welcome! Check out the [contributing guide](CONTRIBUTING.md) to get started.
 
 ## Credits
 
-This project is a collaboration between Google and [Tryolabs](https://tryolabs.com/).
+Temporian is developed in collaboration between Google and [Tryolabs](https://tryolabs.com/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `temporian-0.1.1/config/build.py` & `temporian-0.1.2/config/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def _build_cc_extensions(self):
         return True
 
     # Add the "bazel_build" command as the first sub-command of "build". Each
     # sub_command of "build" (e.g. "build_py", "build_ext", etc.) is executed
     # sequentially when running a "build" command, if the second item in the tuple
-    # (predicate method) is evaluated to true.
+    # (predicate method) is run to true.
     sub_commands = [
         ("bazel_build", _build_cc_extensions)
     ] + build.build.sub_commands
 
 
 class _BazelBuildCommand(setuptools.Command):
     """Build C++ extensions and public protos with Bazel.
```

### Comparing `temporian-0.1.1/pyproject.toml` & `temporian-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "temporian"
-version = "0.1.1"
+version = "0.1.2"
 description = "Temporian is a Python package for feature engineering of temporal data, focusing on preventing common modeling errors and providing a simple and powerful API, a first-class iterative development experience, and efficient and well-tested implementations of common and not-so-common temporal data preprocessing functions."
 authors = [
     "Mathieu Guillame-Bert, Braulio Ríos, Guillermo Etchebarne, Ian Spektor, Richard Stotz <gbm@google.com>",
 ]
 maintainers = ["Mathieu Guillame-Bert <gbm@google.com>"]
 repository = "https://github.com/google/temporian"
 classifiers = [
@@ -34,49 +34,56 @@
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 absl-py = "^1.3.0"
 protobuf = "^4.21.12"
 pandas = "^1.5.2"
 matplotlib = "^3.7.1"
+apache-beam = {version = "^2.48.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
 toml = "^0.10.2"
-pylint = "^2.15.10"
+pylint = "^2.14.0"
 memory-profiler = "^0.61.0"
 # scalene = "^1.5.20" # FIXME: scalene doesn't support Python 3.11
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1.5"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-jupyter = "^0.24.1"
 bokeh = "^3.1.0"
 ipykernel = "^6.22.0"
 griffe = "0.26.0"
 jupyterlab = "^4.0.0"
 mkdocs-exclude-search = "^0.6.5"
+apache-beam = "^2.48.0"
 pillow = "^9.5.0"
 cairosvg = "^2.7.0"
+colorama = "^0.4.6"
+
+[tool.poetry.extras]
+beam = ["apache-beam"]
 
 [tool.black]
 line-length = 80
 preview = true
 
 [tool.pylint]
 max-line-length = 80
 disable = [
     "redefined-builtin",
     "missing-class-docstring",
     "missing-function-docstring",
     "fixme",
     "invalid-name",
+    "no-name-in-module",
 ]
 
 [tool.pyright]
 include = ["temporian"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=67.6.0"]
```

### Comparing `temporian-0.1.1/temporian/BUILD` & `temporian-0.1.2/temporian/core/operators/binary/BUILD`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,71 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "temporian",
+    name = "binary",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core:evaluation",
-        "//temporian/core:graph",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:duration",
+        ":arithmetic",
+        ":logical",
+        ":relational",
+    ],
+)
+
+py_library(
+    name = "base",
+    srcs = ["base.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:api_symbols",
-        "//temporian/core/operators:api_symbols",
         "//temporian/core/operators:base",
-        "//temporian/core/serialization:api_symbols",
-        "//temporian/implementation/numpy/data:event_set",
-        "//temporian/implementation/numpy/data:io",
-        "//temporian/implementation/numpy/data:plotter",
-        "//temporian/io:api_symbols",
+        "//temporian/proto:core_py_proto",
+    ],
+)
+
+py_library(
+    name = "arithmetic",
+    srcs = ["arithmetic.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":base",
+        "//temporian/core:compilation",
+        "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+    ],
+)
+
+py_library(
+    name = "logical",
+    srcs = ["logical.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":base",
+        "//temporian/core:compilation",
+        "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+    ],
+)
+
+py_library(
+    name = "relational",
+    srcs = ["relational.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":base",
+        "//temporian/core:compilation",
+        "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+        "//temporian/core/operators/scalar:relational_scalar",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/__init__.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,69 +8,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Temporian."""
+"""Imports all the packages containing operator implementations."""
 
-# NOTE: The API reference documentation reads this file and expects a single
-# import per line. Do not import several symbols from the same module in a
-# single line. Do not allow import to break lines.
-
-# NOTE: If you need to import something here that isn't part of the public API,
-# and therefore shouldn't show up in the documentation, import it with a private
-# name:
-# from temporian.module import submodule as _submodule
-
-# NOTE: Wildcard imports (*) are treated and parsed as part of root-level
-# imports, so same rules apply to modules imported with a wildcard.
-# Also:
-# - Wildcard imports are only allowed from modules explicitly called api_symbols
-# - Modules imported with wildcards are shown as subfolders in the docs, with
-# the folder's name being the api_symbols.py file's parent's name.
-
-# pylint: disable=wrong-import-position
+# pylint: disable=unused-import
 # pylint: disable=line-too-long
-
-__version__ = "0.0.1"
-
-# Register the ops definitions and implementations.
-from temporian.core.operator_lib import registered_operators as _ops
-from temporian.implementation.numpy import operators as _impls
-
-
-# Actual API
-# ==========
-
-# Nodes and related
-from temporian.core.data.node import Node
-from temporian.core.data.node import input_node
-
-# Dtypes
-from temporian.core.data.dtypes.api_symbols import *
-
-# Schema
-from temporian.core.data.schema import Schema
-
-# Durations
-from temporian.core.data import duration
-
-# Event set
-from temporian.implementation.numpy.data.event_set import EventSet
-from temporian.implementation.numpy.data.io import event_set
-
-# Graph serialization
-from temporian.core.serialization.api_symbols import *
-
-# Graph execution
-from temporian.core.evaluation import evaluate
-
-# Operators
-from temporian.core.operators.api_symbols import *
-
-# IO
-from temporian.io.api_symbols import *
-
-# Plotting
-from temporian.implementation.numpy.data.plotter import plot
+# fmt: off
+from temporian.implementation.numpy.operators import cast
+from temporian.implementation.numpy.operators import drop_index
+from temporian.implementation.numpy.operators import filter
+from temporian.implementation.numpy.operators import glue
+from temporian.implementation.numpy.operators import join
+from temporian.implementation.numpy.operators import unary
+from temporian.implementation.numpy.operators import lag
+from temporian.implementation.numpy.operators import leak
+from temporian.implementation.numpy.operators import prefix
+from temporian.implementation.numpy.operators import propagate
+from temporian.implementation.numpy.operators import select
+from temporian.implementation.numpy.operators import add_index
+from temporian.implementation.numpy.operators import resample
+from temporian.implementation.numpy.operators import rename
+from temporian.implementation.numpy.operators.binary import arithmetic
+from temporian.implementation.numpy.operators.binary import relational
+from temporian.implementation.numpy.operators.binary import logical
+
+from temporian.implementation.numpy.operators.scalar import arithmetic_scalar
+from temporian.implementation.numpy.operators.scalar import relational_scalar
+
+from temporian.implementation.numpy.operators.window import simple_moving_average
+from temporian.implementation.numpy.operators.window import moving_standard_deviation
+from temporian.implementation.numpy.operators.window import moving_sum
+from temporian.implementation.numpy.operators.window import moving_count
+from temporian.implementation.numpy.operators.window import moving_min
+from temporian.implementation.numpy.operators.window import moving_max
+from temporian.implementation.numpy.operators.calendar import day_of_month
+from temporian.implementation.numpy.operators.calendar import day_of_week
+from temporian.implementation.numpy.operators.calendar import day_of_year
+from temporian.implementation.numpy.operators.calendar import year
+from temporian.implementation.numpy.operators.calendar import month
+from temporian.implementation.numpy.operators.calendar import iso_week
+from temporian.implementation.numpy.operators.calendar import hour
+from temporian.implementation.numpy.operators.calendar import minute
+from temporian.implementation.numpy.operators.calendar import second
+from temporian.implementation.numpy.operators import since_last
+from temporian.implementation.numpy.operators import unique_timestamps
+from temporian.implementation.numpy.operators import begin
+from temporian.implementation.numpy.operators import end
+from temporian.implementation.numpy.operators import tick
+from temporian.implementation.numpy.operators import timestamps
+from temporian.implementation.numpy.operators import enumerate
```

### Comparing `temporian-0.1.1/temporian/core/BUILD` & `temporian-0.1.2/temporian/beam/operators/BUILD`

 * *Files 16% similar despite different names*

```diff
@@ -3,45 +3,53 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "evaluation",
-    srcs = ["evaluation.py"],
+    name = "base",
+    srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        ":graph",
-        ":schedule",
-        "//temporian/core/data:node",
+        "//temporian/beam:io",
         "//temporian/core/operators:base",
-        "//temporian/implementation/numpy:evaluation",
-        "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
-    name = "operator_lib",
-    srcs = ["operator_lib.py"],
+    name = "operators",
+    srcs = ["__init__.py"],
     srcs_version = "PY3",
+    deps = [
+        ":add_index",
+        ":select",
+        "//temporian/beam/operators/window:moving_sum",
+    ],
 )
 
 py_library(
-    name = "schedule",
-    srcs = ["schedule.py"],
+    name = "select",
+    srcs = ["select.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/core/operators:base",
+        # already_there/apache_beam
+        "//temporian/beam:io",
+        "//temporian/beam/operators:base",
+        "//temporian/core/operators:select",
+        "//temporian/beam:implementation_lib",
     ],
 )
 
 py_library(
-    name = "graph",
-    srcs = ["graph.py"],
+    name = "add_index",
+    srcs = ["add_index.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/core/operators:base",
+        # already_there/apache_beam
+        # already_there/numpy
+        "//temporian/beam:implementation_lib",
+        "//temporian/beam:io",
+        "//temporian/beam/operators:base",
+        "//temporian/core/operators:add_index",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/__init__.py` & `temporian-0.1.2/temporian/core/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/core/data/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/BUILD`

 * *Files 22% similar despite different names*

```diff
@@ -3,49 +3,36 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "data",
+    name = "numpy",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
 )
 
 py_library(
-    name = "node",
-    srcs = ["node.py"],
+    name = "evaluation",
+    srcs = ["evaluation.py"],
     srcs_version = "PY3",
     deps = [
-        ":schema",
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/utils:string",
+        ":implementation_lib",
+        "//temporian/core:schedule",
+        "//temporian/core/data:node",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy/operators",
     ],
 )
 
 py_library(
-    name = "schema",
-    srcs = ["schema.py"],
+    name = "utils",
+    srcs = ["utils.py"],
     srcs_version = "PY3",
-    deps = [
-        "//temporian/core/data/dtypes:dtype",
-    ],
-)
-
-py_library(
-    name = "duration",
-    srcs = ["duration.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":duration_utils",
-    ],
 )
 
 py_library(
-    name = "duration_utils",
-    srcs = ["duration_utils.py"],
+    name = "implementation_lib",
+    srcs = ["implementation_lib.py"],
     srcs_version = "PY3",
-    deps = [
-        # already_there/numpy
-    ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/data/__init__.py` & `temporian-0.1.2/temporian/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/core/data/dtypes/__init__.py` & `temporian-0.1.2/temporian/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/core/data/dtypes/dtype.py` & `temporian-0.1.2/temporian/core/data/dtype.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,30 +39,30 @@
     def is_float(self) -> bool:
         return self in (DType.FLOAT64, DType.FLOAT32)
 
     @property
     def is_integer(self) -> bool:
         return self in (DType.INT64, DType.INT32)
 
-    def missing_value(self) -> Union[float, int, str]:
+    def missing_value(self) -> Union[float, int, bytes]:
         """
         Returns missing value for specific dtype.
 
         Returns:
             The default missing value for the given data type.
         """
 
         if self.is_float:
             return math.nan
 
         if self.is_integer:
             return 0
 
         if self == DType.STRING:
-            return ""
+            return b""
 
         raise ValueError(f"Non-implemented type {self}")
 
     @classmethod
     def from_python_type(cls, python_type: type) -> "DType":
         """
         Returns DType from python type.
@@ -82,14 +82,17 @@
 
         if python_type is int:
             return DType.INT64
 
         if python_type is str:
             return DType.STRING
 
+        if python_type is bytes:
+            return DType.STRING
+
         if python_type is bool:
             return DType.BOOLEAN
 
         raise ValueError(f"Non-implemented type {python_type}")
 
 
 # The dtype of indexes.
@@ -104,13 +107,28 @@
         raise ValueError(
             f"Trying to create an index with dtype={dtype}. The dtype of an"
             " index can only be int32, int64 or string."
         )
 
 
 # API dtypes definition
+
 float32 = DType.FLOAT32
+"""32-bit floating point number."""
+
 float64 = DType.FLOAT64
+"""64-bit floating point number."""
+
 int32 = DType.INT32
+"""32-bit integer."""
+
 int64 = DType.INT64
+"""64-bit integer."""
+
 bool_ = DType.BOOLEAN
-str_ = DType.STRING
+"""Boolean value."""
+
+bytes_ = DType.STRING
+"""String value (stored as bytes)."""
+
+str_ = bytes_
+"""String value (stored as bytes)."""
```

### Comparing `temporian-0.1.1/temporian/core/data/duration_utils.py` & `temporian-0.1.2/temporian/core/data/duration_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,20 +20,30 @@
 """
 import datetime
 from enum import Enum
 from typing import Union
 
 import numpy as np
 
+from temporian.core.data.duration import (
+    Duration,
+    weeks,
+    days,
+    hours,
+    minutes,
+    seconds,
+    milliseconds,
+)
+
+
 # Unit for durations
 #
 # NormalizedDuration is used by internal code that handle duration.
-# Duration is a duration provided by the user though the API.
+# Duration (defined in ./duration.py) is a duration provided by the user though the API.
 NormalizedDuration = float
-Duration = Union[float, int]
 
 Timestamp = Union[np.datetime64, datetime.datetime, int, float]
 NormalizedTimestamp = float
 
 
 def normalize_duration(x: Duration) -> NormalizedDuration:
     if isinstance(x, (int, float)) and x > 0:
```

### Comparing `temporian-0.1.1/temporian/core/data/schema.py` & `temporian-0.1.2/temporian/core/data/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Schema and related classes."""
 
 from __future__ import annotations
 
 from typing import List, Tuple, Dict, Union
 
 from dataclasses import dataclass
-from temporian.core.data.dtypes.dtype import DType, IndexDType
+from temporian.core.data.dtype import DType, IndexDType
 
 
 @dataclass
 class FeatureSchema:
     name: str
     dtype: DType
 
@@ -37,18 +37,21 @@
     dtype: IndexDType
 
     def __repr__(self) -> str:
         return f"({self.name!r}, {self.dtype})"
 
 
 class Schema:
-    """A schema defines the type of data in an event set.
+    """A schema defines the type of data in an
+    [`EventSetNode`][temporian.EventSetNode] or
+    [`EventSet`][temporian.EventSet].
 
     A schema does not contain any actual data.
-    A schema can be shared by multiple nodes.
+
+    A schema can be shared by multiple EventSetNodes.
 
     Attributes:
         features: List of feature names and types.
         indexes: List of index names and types.
         is_unix_timestamp: Whether values correspond to Unix timestamps.
     """
 
@@ -105,20 +108,18 @@
         r = (
             f"features: {self._features}\n"
             f"indexes: {self._indexes}\n"
             f"is_unix_timestamp: {self._is_unix_timestamp}\n"
         )
         return r
 
-    def check_compatible_index(
-        self, other: Schema, label: str = "input and sampling"
-    ):
+    def check_compatible_index(self, other: Schema):
         if self.indexes != other.indexes:
             raise ValueError(
-                f"The index of {label} don't match. {self.indexes} !="
+                f"Arguments don't have the same index. {self.indexes} !="
                 f" {other.indexes}"
             )
 
 
 def _normalize_feature(x):
     if isinstance(x, FeatureSchema):
         return x
```

### Comparing `temporian-0.1.1/temporian/core/data/test/node_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/begin_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,31 +8,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 from absl.testing import absltest
 
-import temporian as tp
-from temporian.core.test import utils
-from temporian.implementation.numpy.data.event_set import EventSet
-
-
-class NodeTest(absltest.TestCase):
-    def test_evaluate_input(self):
-        node = utils.create_source_node()
-        evset = utils.create_input_event_set()
-        result = node.evaluate({node: evset})
-        self.assertIsInstance(result, EventSet)
-        self.assertTrue(result is evset)
-
-    def test_evaluate_single_operator(self):
-        evset = utils.create_input_event_set()
-        result = tp.simple_moving_average(evset.node(), 10)
-        result = result.evaluate(evset)
-        self.assertIsInstance(result, EventSet)
+from temporian.core.operators.begin import BeginOperator
+from temporian.implementation.numpy.data.io import event_set
+from temporian.implementation.numpy.operators.begin import (
+    BeginNumpyImplementation,
+)
+
+
+class BeginOperatorTest(absltest.TestCase):
+    def setUp(self):
+        pass
+
+    def test_base(self):
+        evset = event_set(
+            timestamps=[1, 2, 3, 4],
+            features={
+                "a": [5, 6, 7, 8],
+                "b": ["A", "A", "B", "B"],
+            },
+            indexes=["b"],
+        )
+        node = evset.node()
+
+        expected_output = event_set(
+            timestamps=[1, 3],
+            features={"b": ["A", "B"]},
+            indexes=["b"],
+        )
+
+        # Run op
+        op = BeginOperator(input=node)
+        instance = BeginNumpyImplementation(op)
+        output = instance.call(input=evset)["output"]
+
+        self.assertEqual(output, expected_output)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/core/graph.py` & `temporian-0.1.2/temporian/core/graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,105 +10,109 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Graph class definition and inference logic."""
 
+from __future__ import annotations
+from copy import deepcopy
 from typing import List, Set, Dict, Union, Optional
 
-from temporian.core.data.node import Node, Feature, Sampling
+from temporian.core.data.node import EventSetNode, Feature, Sampling
 from temporian.core.operators import base
 
-NamedNodes = Union[Dict[str, Node], List[Node], Set[Node], Node]
+NamedEventSetNodes = Union[
+    Dict[str, EventSetNode], List[EventSetNode], Set[EventSetNode], EventSetNode
+]
 
 
 class Graph:
     """A set of operators, nodes, features and samplings."""
 
     def __init__(self):
         self._operators: Set[base.Operator] = set()
         self._features: Set[Feature] = set()
-        self._nodes: Set[Node] = set()
+        self._nodes: Set[EventSetNode] = set()
         self._samplings: Set[Sampling] = set()
-        self._inputs: Set[Node] = set()
-        self._outputs: Set[Node] = set()
-        self._named_inputs: Optional[Dict[str, Node]] = None
-        self._named_outputs: Optional[Dict[str, Node]] = None
+        self._inputs: Set[EventSetNode] = set()
+        self._outputs: Set[EventSetNode] = set()
+        self._named_inputs: Optional[Dict[str, EventSetNode]] = None
+        self._named_outputs: Optional[Dict[str, EventSetNode]] = None
 
     @property
     def samplings(self) -> Set[Sampling]:
         return self._samplings
 
     @property
     def features(self) -> Set[Feature]:
         return self._features
 
     @property
     def operators(self) -> Set[base.Operator]:
         return self._operators
 
     @property
-    def nodes(self) -> Set[Node]:
+    def nodes(self) -> Set[EventSetNode]:
         return self._nodes
 
     @property
-    def inputs(self) -> Set[Node]:
+    def inputs(self) -> Set[EventSetNode]:
         return self._inputs
 
     @property
-    def outputs(self) -> Set[Node]:
+    def outputs(self) -> Set[EventSetNode]:
         return self._outputs
 
     @property
-    def named_inputs(self) -> Optional[Dict[str, Node]]:
+    def named_inputs(self) -> Optional[Dict[str, EventSetNode]]:
         return self._named_inputs
 
     @property
-    def named_outputs(self) -> Optional[Dict[str, Node]]:
+    def named_outputs(self) -> Optional[Dict[str, EventSetNode]]:
         return self._named_outputs
 
     @named_inputs.setter
-    def named_inputs(self, named_inputs: Optional[Dict[str, Node]]):
+    def named_inputs(self, named_inputs: Optional[Dict[str, EventSetNode]]):
         self._named_inputs = named_inputs
 
     @named_outputs.setter
-    def named_outputs(self, named_outputs: Optional[Dict[str, Node]]):
+    def named_outputs(self, named_outputs: Optional[Dict[str, EventSetNode]]):
         self._named_outputs = named_outputs
 
     def add_operator(self, operator: base.Operator) -> None:
         self._operators.add(operator)
 
     def add_sampling(self, sampling: Sampling) -> None:
         self._samplings.add(sampling)
 
     def add_feature(self, feature: Feature) -> None:
         self._features.add(feature)
 
-    def add_node(self, node: Node) -> None:
+    def add_node(self, node: EventSetNode) -> None:
         self._nodes.add(node)
 
     def input_features(self) -> Set[Feature]:
         return {
             feature for node in self.inputs for feature in node.feature_nodes
         }
 
-    def set_input_node_names(self, names: Dict[str, Node]):
+    def set_input_node_names(self, names: Dict[str, EventSetNode]):
         if self._inputs is not None:
             named_nodes = set(names.values())
             if named_nodes != self._inputs:
                 raise ValueError(
                     "All the input nodes and only the input nodes should be"
                     f" renamed. Input nodes: {self._inputs}. Renamed nodes:"
                     f" {names}"
                 )
 
         self._named_inputs = names
 
-    def set_output_node_names(self, names: Dict[str, Node]):
+    def set_output_node_names(self, names: Dict[str, EventSetNode]):
         if self._outputs is not None:
             named_nodes = set(names.values())
             if named_nodes != self._outputs:
                 raise ValueError(
                     "All the input nodes and only the input nodes should be"
                     f" renamed. Input nodes: {self._outputs}. Renamed nodes:"
                     f" {names}"
@@ -128,15 +132,15 @@
             for e in elements:
                 s += f"\t{e}\n"
             s += "\n"
 
         p("Operators", self.operators)
         p("Features", self.features)
         p("Samplings", self.samplings)
-        p("Nodes", self.nodes)
+        p("EventSetNodes", self.nodes)
 
         def p2(title, dictionary):
             nonlocal s
             s += f"{title} ({len(dictionary)}):\n"
             for k, v in dictionary.items():
                 s += f"\t{k}:{v}\n"
             s += "\n"
@@ -155,25 +159,65 @@
 
         if self.named_outputs is not None:
             p2("Named output", self.named_outputs)
         else:
             p3("Output", self.outputs)
         return s
 
+    def apply_on_inputs(
+        self, named_inputs: Dict[str, EventSetNode]
+    ) -> Dict[str, EventSetNode]:
+        """Applies the operators in this graph to new inputs.
+
+        Note that the objects in the modified graph are very inconsistent, but
+        that's okay since we won't use it anymore. When running it or save it
+        the graph will be re-inferred.
+
+        Args:
+            named_inputs: The new inputs to the graph.
+
+        Returns:
+            The graph's named outputs.
+        """
+
+        # Avoid messing with the objects in the received graph
+        # Else each time we apply the graph on inputs it changes
+        # Might be possible to optimize by copying only what's necessary
+        g = deepcopy(self)
+
+        assert g.named_inputs is not None
+        assert g.named_outputs is not None
+
+        for name, new_node in named_inputs.items():
+            if name not in g.named_inputs:
+                raise ValueError(
+                    f"Input node {name} is not in the graph's inputs. Inputs:"
+                    f" {g.named_inputs}"
+                )
+            old_node = g.named_inputs[name]
+            # Replace node as input in all operators that depend on it
+            # TODO: create and maintain a mapping from named_input to operator
+            # to make this more efficient
+            for operator in g.operators:
+                for name, inp in operator.inputs.items():
+                    if inp is old_node:
+                        operator.inputs[name] = new_node
+        return g.named_outputs
+
 
 def infer_graph_named_nodes(
-    inputs: Optional[NamedNodes], outputs: NamedNodes
+    inputs: Optional[NamedEventSetNodes], outputs: NamedEventSetNodes
 ) -> Graph:
     """Extracts the nodes in between the output and input nodes.
 
     Unlike infer_graph, infer_graph_named_nodes requires for the input and
     output nodes to be named.
     """
 
-    normalized_inputs: Optional[Dict[str, Node]] = None
+    normalized_inputs: Optional[Dict[str, EventSetNode]] = None
     input_nodes = None
     if inputs is not None:
         normalized_inputs = normalize_named_nodes(inputs)
         input_nodes = set(normalized_inputs.values())
 
     normalized_outputs = normalize_named_nodes(outputs)
     output_nodes = set(normalized_outputs.values())
@@ -183,15 +227,17 @@
         normalized_inputs = normalize_named_nodes(list(g.inputs))
 
     g.set_input_node_names(normalized_inputs)
     g.set_output_node_names(normalized_outputs)
     return g
 
 
-def infer_graph(inputs: Optional[Set[Node]], outputs: Set[Node]) -> Graph:
+def infer_graph(
+    inputs: Optional[Set[EventSetNode]], outputs: Set[EventSetNode]
+) -> Graph:
     """Extracts the nodes in between the output and input nodes.
 
     If inputs is set, fails if outputs cannot be computed from `inputs`.
     If inputs is not set, infers the required set of inputs.
 
     Args:
         inputs: Set of available input nodes. If None, inputs are inferred.
@@ -228,23 +274,23 @@
     # else:
     #     input_set = inputs if isinstance(inputs, set) else
     #         set(inputs.values())
 
     graph = Graph()
     graph.outputs.update(outputs)
 
-    # The next nodes to process. Nodes are processed from the outputs to
+    # The next nodes to process. EventSetNodes are processed from the outputs to
     # the inputs.
-    pending_nodes: Set[Node] = outputs.copy()
+    pending_nodes: Set[EventSetNode] = outputs.copy()
 
     # Features already processed.
-    done_nodes: Set[Node] = set()
+    done_nodes: Set[EventSetNode] = set()
 
     # List of the missing nodes. Used to create an error message.
-    missing_nodes: Set[Node] = set()
+    missing_nodes: Set[EventSetNode] = set()
 
     while pending_nodes:
         # Select a node to process.
         node = next(iter(pending_nodes))
         pending_nodes.remove(node)
         assert node not in done_nodes
 
@@ -291,20 +337,20 @@
         graph.add_sampling(e.sampling_node)
         for f in e.feature_nodes:
             graph.add_feature(f)
 
     return graph
 
 
-def normalize_named_nodes(src: NamedNodes) -> Dict[str, Node]:
+def normalize_named_nodes(src: NamedEventSetNodes) -> Dict[str, EventSetNode]:
     """Normalizes a node or list of nodes into a dictionary of nodes."""
 
     save_src = src
 
-    if isinstance(src, Node):
+    if isinstance(src, EventSetNode):
         # Will be further processed after.
         src = [src]
 
     if isinstance(src, set):
         src = list(src)
 
     if isinstance(src, list):
```

### Comparing `temporian-0.1.1/temporian/core/operator_lib.py` & `temporian-0.1.2/temporian/core/operator_lib.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/core/operators/__init__.py` & `temporian-0.1.2/temporian/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/core/operators/add_index.py` & `temporian-0.1.2/temporian/core/operators/drop_index.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,210 +8,241 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Set index operator class and public API function definition."""
+"""Drop index operator class and public API function definition."""
 
-from typing import List, Union
+from typing import List, Optional, Union
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.data.schema import FeatureSchema, IndexSchema
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
-from temporian.core.operators.drop_index import drop_index
 
 
-class AddIndexOperator(Operator):
+class DropIndexOperator(Operator):
     def __init__(
         self,
-        input: Node,
-        index_to_add: List[str],
+        input: EventSetNode,
+        indexes: List[str],
+        keep: bool,
     ) -> None:
         super().__init__()
 
-        self._output_feature_schemas = self._get_output_feature_schemas(
-            input, index_to_add
-        )
-        self._output_indexes = self._get_output_indexes(input, index_to_add)
-        self._index_to_add = index_to_add
+        # `indexes`` is the list of indexes in `input` to drop. If
+        # `keep` is true, those indexes will be converted into features.
+        self._indexes = indexes
+        self._keep = keep
 
         self.add_input("input", input)
+        self.add_attribute("indexes", indexes)
+        self.add_attribute("keep", keep)
+
+        self._output_feature_schemas = self._get_output_feature_schemas(
+            input, indexes, keep
+        )
 
-        self.add_attribute("index_to_add", index_to_add)
+        self._output_indexes = [
+            index_level
+            for index_level in input.schema.indexes
+            if index_level.name not in indexes
+        ]
 
         self.add_output(
             "output",
             create_node_new_features_new_sampling(
                 features=self._output_feature_schemas,
                 indexes=self._output_indexes,
                 is_unix_timestamp=input.schema.is_unix_timestamp,
                 creator=self,
             ),
         )
         self.check()
 
     def _get_output_feature_schemas(
-        self, input: Node, index_to_add: List[str]
+        self, input: EventSetNode, indexes: List[str], keep: bool
     ) -> List[FeatureSchema]:
-        return [
-            feature
-            for feature in input.schema.features
-            if feature.name not in index_to_add
-        ]
+        if not keep:
+            return input.schema.features
 
-    def _get_output_indexes(
-        self, input: Node, index_to_add: List[str]
-    ) -> List[IndexSchema]:
         index_dict = input.schema.index_name_to_dtype()
         feature_dict = input.schema.feature_name_to_dtype()
 
-        new_indexes: List[IndexSchema] = []
-        for index_name in index_to_add:
-            if index_name not in feature_dict:
-                raise ValueError(
-                    f"Add index {index_name} is not part of the features."
-                )
+        new_features: List[FeatureSchema] = []
+        for index in indexes:
+            if index not in index_dict:
+                raise ValueError(f"{index} is not an index in input.")
 
-            if index_name in index_dict:
+            if index in feature_dict:
                 raise ValueError(
-                    f"Add index {index_name} is already part of the index."
+                    f"{index} already exists in input's features. If you"
+                    " want to drop the index, specify `keep=False`."
                 )
 
-            new_indexes.append(
-                IndexSchema(name=index_name, dtype=feature_dict[index_name])
+            new_features.append(
+                FeatureSchema(name=index, dtype=index_dict[index])
             )
-        # Note: The new index is added after the existing index items.
-        return input.schema.indexes + new_indexes
 
-    @classmethod
-    def build_op_definition(cls) -> pb.OperatorDef:
-        return pb.OperatorDef(
-            key="ADD_INDEX",
-            attributes=[
-                pb.OperatorDef.Attribute(
-                    key="index_to_add",
-                    type=pb.OperatorDef.Attribute.Type.LIST_STRING,
-                ),
-            ],
-            inputs=[pb.OperatorDef.Input(key="input")],
-            outputs=[pb.OperatorDef.Output(key="output")],
-        )
+        # Note: The new features are added after the existing features.
+        return input.schema.features + new_features
 
     @property
     def output_feature_schemas(self) -> List[FeatureSchema]:
         return self._output_feature_schemas
 
     @property
     def output_indexes(self) -> List[IndexSchema]:
         return self._output_indexes
 
     @property
-    def index_to_add(self) -> List[str]:
-        return self._index_to_add
-
-
-operator_lib.register_operator(AddIndexOperator)
+    def indexes(self) -> List[str]:
+        return self._indexes
 
+    @property
+    def keep(self) -> bool:
+        return self._keep
 
-def _normalize_index_to_add(
-    index_names: Union[str, List[str]],
-) -> List[str]:
-    if isinstance(index_names, str):
-        return [index_names]
+    @classmethod
+    def build_op_definition(cls) -> pb.OperatorDef:
+        return pb.OperatorDef(
+            key="DROP_INDEX",
+            attributes=[
+                pb.OperatorDef.Attribute(
+                    key="indexes",
+                    type=pb.OperatorDef.Attribute.Type.LIST_STRING,
+                ),
+                pb.OperatorDef.Attribute(
+                    key="keep",
+                    type=pb.OperatorDef.Attribute.Type.BOOL,
+                ),
+            ],
+            inputs=[pb.OperatorDef.Input(key="input")],
+            outputs=[pb.OperatorDef.Output(key="output")],
+        )
 
-    if len(index_names) == 0:
-        raise ValueError("Cannot specify empty list as `index_names` argument.")
 
-    return index_names
+operator_lib.register_operator(DropIndexOperator)
 
 
-def _normalize_index_to_set(
-    index_names: Union[str, List[str]],
+def _normalize_indexes(
+    input: EventSetNode,
+    indexes: Optional[Union[List[str], str]],
 ) -> List[str]:
-    if isinstance(index_names, str):
-        return [index_names]
-
-    if len(index_names) == 0:
-        raise ValueError("Cannot specify empty list as `index_names` argument.")
-
-    return index_names
-
-
-def add_index(input: Node, index_to_add: Union[str, List[str]]) -> Node:
-    """Adds one or more features as index in a node.
-
-    Examples:
-        Given an input `Node` with index names ['A', 'B', 'C'] and features
-        names ['X', 'Y', 'Z']:
-
-        3. `add_index(input, feature_names=['X', 'Y'])`
-           Output `Node` will have index names ['A', 'B', 'C', 'X', 'Y'] and
-           features names ['Z'].
-
-    Args:
-        input: Input `Node` object for which the index is to be set or
-            updated.
-        index_to_add: List of feature names (strings) that should be used as
-            the new index. These feature names should already exist in `input`.
-
-    Returns:
-         New `Node` with the updated index.
-
-    Raises:
-        KeyError: If any of the specified `index_to_add` are not found in
-            `input`.
-    """
-
-    index_to_add = _normalize_index_to_add(index_to_add)
-    return AddIndexOperator(input, index_to_add).outputs["output"]
-
-
-def set_index(input: Node, index: Union[str, List[str]]) -> Node:
-    """Replaces the index in a node.
+    if indexes is None:
+        # Drop all the indexes
+        return input.schema.index_names()
+
+    if isinstance(indexes, str):
+        indexes = [indexes]
+
+    if len(indexes) == 0:
+        raise ValueError("Cannot specify empty list as `indexes` argument.")
+
+    # Check that requested indexes exist
+    index_dict = input.schema.index_name_to_dtype()
+    for index in indexes:
+        if index not in index_dict:
+            raise KeyError(
+                f"{index} is not an index in {input.schema.indexes}."
+            )
 
-    "set_index" is implemented as drop_index + add_index.
+    return indexes
 
-    Examples:
-        Given an input `Node` with index names ['A', 'B', 'C'] and features
-        names ['X', 'Y', 'Z']:
 
-        1. `set_index(input, index=['X'])`
-           Output `Node` will have index names ['X'] and features names
-           ['A', 'B', 'C', 'Y', 'Z'].
+@compile
+def drop_index(
+    input: EventSetNode,
+    indexes: Optional[Union[str, List[str]]] = None,
+    keep: bool = True,
+) -> EventSetNode:
+    """Removes indexes from an [`EventSetNode`][temporian.EventSetNode].
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2, 1, 0, 1, 1],
+        ...     features={
+        ...         "f1": [1, 1, 1, 2, 2, 2],
+        ...         "f2": [1, 1, 2, 1, 1, 2],
+        ...         "f3": [1, 1, 1, 1, 1, 1]
+        ...     },
+        ...     indexes=["f1", "f2"]
+        ... )
+
+        >>> # Both f1 and f2 are indices
+        >>> a
+        indexes: [('f1', int64), ('f2', int64)]
+        features: [('f3', int64)]
+        events:
+            f1=2 f2=1 (2 events):
+                timestamps: [0. 1.]
+                'f3': [1 1]
+            f1=1 f2=1 (2 events):
+                timestamps: [1. 2.]
+                'f3': [1 1]
+            f1=1 f2=2 (1 events):
+                timestamps: [1.]
+                'f3': [1]
+            f1=2 f2=2 (1 events):
+                timestamps: [1.]
+                'f3': [1]
+        ...
+
+        >>> # Drop "f2", remove it from features
+        >>> b = tp.drop_index(a, "f2", keep=False)
+        >>> b
+        indexes: [('f1', int64)]
+        features: [('f3', int64)]
+        events:
+            f1=2 (3 events):
+                timestamps: [0. 1. 1.]
+                'f3': [1 1 1]
+            f1=1 (3 events):
+                timestamps: [1. 1. 2.]
+                'f3': [1 1 1]
+        ...
+
+        >>> # Drop both indices, keep them as features
+        >>> b = tp.drop_index(a, ["f2", "f1"])
+        >>> b
+        indexes: []
+        features: [('f3', int64), ('f2', int64), ('f1', int64)]
+        events:
+            (6 events):
+                timestamps: [0. 1. 1. 1. 1. 2.]
+                'f3': [1 1 1 1 1 1]
+                'f2': [2 2 1 1 2 1]
+                'f1': [1 1 1 2 2 1]
+        ...
 
-        2. `set_index(input, index=['X', 'Y'])`
-           Output `Node` will have index names ['X', 'Y'] and
-           features names ['A', 'B', 'C', 'Z'].
+        ```
 
     Args:
-        input: Input `Node` object for which the index is to be set or
-            updated.
-        index: List of index / feature names (strings) used as
-            the new index. These feature names should be either index or
-            features in `input`.
+        input: EventSetNode from which the specified indexes should be removed.
+        indexes: Index column(s) to be removed from `input`. This can be a
+            single column name (`str`) or a list of column names (`List[str]`).
+            If not specified or set to `None`, all indexes in `input` will
+            be removed. Defaults to `None`.
+        keep: Flag indicating whether the removed indexes should be kept
+            as features in the output `EventSetNode`. Defaults to `True`.
 
     Returns:
-        New `Node` with the updated index.
+        New `EventSetNode` with the specified indexes removed. If `keep` is set to
+        `True`, the removed indexes will be included as features in it.
 
     Raises:
-        KeyError: If any of the specified `index_to_add` are not found in
-            `input`.
+        ValueError: If an empty list is provided as the `index_names` argument.
+        KeyError: If any of the specified `index_names` are missing from
+            `input`'s index.
+        ValueError: If a feature name coming from the indexes already exists in
+            `input`, and the `keep` flag is set to `True`.
     """
-
-    new_index = _normalize_index_to_set(index)
-
-    # Note
-    # The set_index is implemented as a drop_index + add_index.
-    # The implementation could be improved (simpoler, faster) with a new
-    # operator to re-order the index items.
-
-    if len(input.schema.indexes) != 0:
-        input = drop_index(input)
-
-    if len(new_index) != 0:
-        input = add_index(input, new_index)
-
-    return input
+    indexes = _normalize_indexes(input, indexes)
+    return DropIndexOperator(input, indexes, keep).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/base.py` & `temporian-0.1.2/temporian/core/operators/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,27 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base operator class and auxiliary classes definition."""
 
+from __future__ import annotations
 from abc import ABC
-from typing import Dict, List, Tuple, Union, Any
-from temporian.core.data.dtypes.dtype import DType
+from copy import deepcopy
+from typing import Dict, List, Tuple, TypeVar, Union, Any
+from temporian.core.data.dtype import DType
 
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
+from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.proto import core_pb2 as pb
 
 
 # Valid types for operator attributes
 AttributeType = Union[
-    str, int, float, bool, List[str], Dict[str, str], List[DType]
+    str, int, float, bool, bytes, List[str], Dict[str, str], List[DType]
 ]
 
+# Generic type for defining the input/output types of operators.
+EventSetOrNode = TypeVar("EventSetOrNode", EventSet, EventSetNode)
+
 
 class OperatorExceptionDecorator:
     """Adds details about an operator to exceptions raised in a block.
 
     Usage example:
       with OperatorExceptionDecorator(operator):
         raise ValueError("Something is wrong")
@@ -62,60 +68,75 @@
                 exc_val.args += (message,)
         return False
 
 
 class Operator(ABC):
     """Interface definition and common logic for operators."""
 
+    _next_internal_id: int = 0
+
     def __init__(self):
-        self._inputs: Dict[str, Node] = {}
-        self._outputs: Dict[str, Node] = {}
+        self._inputs: Dict[str, EventSetNode] = {}
+        self._outputs: Dict[str, EventSetNode] = {}
         self._attributes: Dict[str, AttributeType] = {}
         self._definition: pb.OperatorDef = self.build_op_definition()
         self._attr_types: Dict[str, type] = {
             attr.key: attr.type for attr in self._definition.attributes
         }
 
+        # Id of the operator object such that an operator A instantiated before
+        # an operator B will have a smaller _internal_ordered_id.
+        #
+        # _internal_ordered_id is used to ensure the deterministic graph
+        # evaluation.
+        self._internal_ordered_id = Operator.next_internal_id()
+
+    @classmethod
+    def next_internal_id(cls) -> int:
+        id = cls._next_internal_id
+        cls._next_internal_id += 1
+        return id
+
     def __repr__(self):
         return (
-            f"Operator(key={self.definition().key!r}, id={id(self)!r},"
-            f" attributes={self.attributes!r})"
+            f"Operator(key={self.definition().key!r},"
+            f" id={self._internal_ordered_id}, attributes={self.attributes!r})"
         )
 
     @property
     def attributes(self) -> Dict[str, AttributeType]:
         return self._attributes
 
     @property
-    def inputs(self) -> Dict[str, Node]:
+    def inputs(self) -> Dict[str, EventSetNode]:
         return self._inputs
 
     @property
-    def outputs(self) -> Dict[str, Node]:
+    def outputs(self) -> Dict[str, EventSetNode]:
         return self._outputs
 
     @attributes.setter
     def attributes(self, attributes: Dict[str, AttributeType]):
         self._attributes = attributes
 
     @inputs.setter
-    def inputs(self, inputs: Dict[str, Node]):
+    def inputs(self, inputs: Dict[str, EventSetNode]):
         self._inputs = inputs
 
     @outputs.setter
-    def outputs(self, outputs: Dict[str, Node]):
+    def outputs(self, outputs: Dict[str, EventSetNode]):
         self._outputs = outputs
 
-    def add_input(self, key: str, node: Node) -> None:
+    def add_input(self, key: str, node: EventSetNode) -> None:
         with OperatorExceptionDecorator(self):
             if key in self.inputs:
                 raise ValueError(f'Already existing input "{key}".')
             self.inputs[key] = node
 
-    def add_output(self, key: str, node: Node) -> None:
+    def add_output(self, key: str, node: EventSetNode) -> None:
         with OperatorExceptionDecorator(self):
             if key in self.outputs:
                 raise ValueError(f'Already existing output "{key}".')
             self.outputs[key] = node
 
     def add_attribute(self, key: str, value: AttributeType) -> None:
         with OperatorExceptionDecorator(self):
@@ -156,14 +177,16 @@
             # Check that expected attributes are present and have correct type
             for expected_attr in definition.attributes:
                 # From definition
                 def_key = expected_attr.key
                 def_type = expected_attr.type
 
                 if def_key not in self._attributes:
+                    if expected_attr.is_optional:
+                        continue
                     raise ValueError(f'Missing attr. "{expected_attr.key}".')
 
                 # Check that the value type is as defined for this attribute
                 attr_value = self._attributes[def_key]
                 self.check_attribute_type(attr_value, def_type)
 
             # Check that no unexpected attributes are present
@@ -227,14 +250,18 @@
 
         # Check exact matching between attr type (except ANY) and value type
         if (
             attr_type == pb.OperatorDef.Attribute.Type.STRING
             and not isinstance(value, str)
         ):
             raise ValueError(f"Attribute {value=} mismatch: string expected")
+        if attr_type == pb.OperatorDef.Attribute.Type.BYTES and not isinstance(
+            value, bytes
+        ):
+            raise ValueError(f"Attribute {value=} mismatch: string expected")
         if (
             attr_type == pb.OperatorDef.Attribute.Type.INTEGER_64
             and not isinstance(value, int)
         ):
             raise ValueError(f"Attribute {value=} mismatch: integer expected")
         if (
             attr_type == pb.OperatorDef.Attribute.Type.FLOAT_64
@@ -267,14 +294,15 @@
                 f"Attribute {value=} type mismatch: list[DType] expected"
             )
 
         # Special case: ANY attribute type, still needs to be a valid type
         if (
             attr_type == pb.OperatorDef.Attribute.Type.ANY
             and not isinstance(value, str)
+            and not isinstance(value, bytes)
             and not isinstance(value, bool)
             and not isinstance(value, int)
             and not isinstance(value, float)
             and not is_list_str(value)
             and not is_dict_str(value)
             and not is_list_dtype(value)
         ):
@@ -299,7 +327,18 @@
         if (
             attr_type == pb.OperatorDef.Attribute.Type.BOOL
             and isinstance(value, int)
             and value in [0, 1]
         ):
             return bool(value)
         return value
+
+    def __deepcopy__(self, memo) -> Operator:
+        """Custom deepcopy implementation to avoid having repeated internal
+        ordered op ids."""
+        cls = self.__class__
+        op = cls.__new__(cls)
+        memo[id(self)] = op
+        for k, v in self.__dict__.items():
+            setattr(op, k, deepcopy(v, memo))
+        op._internal_ordered_id = Operator.next_internal_id()
+        return op
```

### Comparing `temporian-0.1.1/temporian/core/operators/begin.py` & `temporian-0.1.2/temporian/core/operators/unique_timestamps.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Begin operator class and public API function definitions."""
+
+"""Unique timestamps operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
-class BeginOperator(Operator):
-    def __init__(self, input: Node):
+class UniqueTimestamps(Operator):
+    def __init__(self, input: EventSetNode):
         super().__init__()
 
         self.add_input("input", input)
 
         self.add_output(
             "output",
             create_node_new_features_new_sampling(
@@ -36,33 +41,45 @@
             ),
         )
         self.check()
 
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="BEGIN",
+            key="UNIQUE_TIMESTAMPS",
             attributes=[],
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
-operator_lib.register_operator(BeginOperator)
+operator_lib.register_operator(UniqueTimestamps)
 
 
-def begin(input: Node) -> Node:
-    """Generates a single timestamp at the beginning of the input.
+@compile
+def unique_timestamps(input: EventSetNode) -> EventSetNode:
+    """Removes events with duplicated timestamps from an EventSetNode.
+
+    Returns a feature-less node where each timestamps from `input` only appears
+    once. If the input is indexed, the unique operation is applied independently
+    for each index.
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(timestamps=[5, 9, 9, 16], features={'f': [1,2,3,4]})
+        >>> b = tp.unique_timestamps(a)
+        >>> b
+        indexes: []
+        features: []
+        events:
+             (3 events):
+                timestamps: [ 5. 9. 16.]
+        ...
 
     Args:
-        input: Guide input
-
-    Example:
-        Input
-            timestamps: [1, 5, 10]
-        Output
-            timestamps: [1]
+        input: EventSetNode, possibly with features, to process.
 
     Returns:
-        A feature-less node with a single timestamp.
+        EventSetNode without features with unique timestamps in `input`.
     """
-    return BeginOperator(input=input).outputs["output"]
+
+    return UniqueTimestamps(input=input).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/binary/BUILD` & `temporian-0.1.2/temporian/core/operators/scalar/BUILD`

 * *Files 12% similar despite different names*

```diff
@@ -3,79 +3,55 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "binary",
+    name = "scalar",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
     deps = [
-        ":api_symbols",
-        ":arithmetic",
-        ":logical",
-        ":relational",
-    ],
-)
-
-py_library(
-    name = "api_symbols",
-    srcs = ["api_symbols.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":arithmetic",
-        ":logical",
-        ":relational",
+        ":arithmetic_scalar",
+        ":relational_scalar",
     ],
 )
 
 py_library(
     name = "base",
     srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
         "//temporian/core/operators:base",
         "//temporian/proto:core_py_proto",
     ],
 )
 
 py_library(
-    name = "arithmetic",
-    srcs = ["arithmetic.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
-        "//temporian/core/data/dtypes:dtype",
-    ],
-)
-
-py_library(
-    name = "logical",
-    srcs = ["logical.py"],
+    name = "arithmetic_scalar",
+    srcs = ["arithmetic_scalar.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
+        "//temporian/core:compilation",
         "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
     ],
 )
 
 py_library(
-    name = "relational",
-    srcs = ["relational.py"],
+    name = "relational_scalar",
+    srcs = ["relational_scalar.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
+        "//temporian/core:compilation",
         "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/operators/binary/base.py` & `temporian-0.1.2/temporian/core/operators/binary/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base binary operators class definition."""
 
 from abc import abstractmethod
 
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class BaseBinaryOperator(Operator):
     """Base for common code of binary operators (between two events)."""
 
     def __init__(
         self,
-        input_1: Node,
-        input_2: Node,
+        input_1: EventSetNode,
+        input_2: EventSetNode,
     ):
         super().__init__()
 
         # inputs
         self.add_input("input_1", input_1)
         self.add_input("input_2", input_2)
 
@@ -54,15 +54,15 @@
         # check that features have same dtype
         for feature_idx, (feature_1, feature_2) in enumerate(
             zip(input_1.schema.features, input_2.schema.features)
         ):
             if feature_1.dtype != feature_2.dtype:
                 raise ValueError(
                     "The operator is applied feature-wise, and "
-                    "corresponding features (with the same index) should have "
+                    "corresponding features should have "
                     "the same dtype. However the dtypes of the "
                     f" {feature_idx}-th features don't match. Left argument ="
                     f" {feature_1}, right argument = {feature_2}."
                 )
 
         # outputs
         output_features = [  # pylint: disable=g-complex-comprehension
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/BUILD`

 * *Files 18% similar despite different names*

```diff
@@ -6,139 +6,119 @@
 # Libraries
 # =========
 
 py_library(
     name = "calendar",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
-    deps = [
-        ":api_symbols",
-    ],
-)
-
-py_library(
-    name = "api_symbols",
-    srcs = ["api_symbols.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":day_of_month",
-        ":day_of_week",
-        ":day_of_year",
-        ":hour",
-        ":iso_week",
-        ":minute",
-        ":month",
-        ":second",
-        ":year",
-    ],
 )
 
 py_library(
     name = "base",
     srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/core/operators:base",
-        "//temporian/proto:core_py_proto",
+        # already_there/numpy
+        "//temporian/core/operators/calendar:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy/operators:base",
     ],
 )
 
 py_library(
     name = "day_of_month",
     srcs = ["day_of_month.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:day_of_month",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "day_of_week",
     srcs = ["day_of_week.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:day_of_week",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "day_of_year",
     srcs = ["day_of_year.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:day_of_year",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "hour",
     srcs = ["hour.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:hour",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "iso_week",
     srcs = ["iso_week.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:iso_week",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "minute",
     srcs = ["minute.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:minute",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "month",
     srcs = ["month.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:month",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "second",
     srcs = ["second.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:second",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
     name = "year",
     srcs = ["year.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
+        "//temporian/core/operators/calendar:year",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/api_symbols.py` & `temporian-0.1.2/temporian/core/operators/calendar/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Calendar operators."""
+
 # pylint: disable=unused-import
 
 from temporian.core.operators.calendar.day_of_month import calendar_day_of_month
 from temporian.core.operators.calendar.day_of_week import calendar_day_of_week
 from temporian.core.operators.calendar.day_of_year import calendar_day_of_year
 from temporian.core.operators.calendar.hour import calendar_hour
 from temporian.core.operators.calendar.iso_week import calendar_iso_week
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/base.py` & `temporian-0.1.2/temporian/core/operators/calendar/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base calendar operator class definition."""
 
 from abc import ABC, abstractmethod
 
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_existing_sampling,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class BaseCalendarOperator(Operator, ABC):
     """Interface definition and common logic for calendar operators."""
 
-    def __init__(self, sampling: Node):
+    def __init__(self, sampling: EventSetNode):
         super().__init__()
 
         if not sampling.schema.is_unix_timestamp:
             raise ValueError(
                 "Calendar operators can only be applied on nodes with unix"
                 " timestamps as sampling. This can be specified with"
                 " `is_unix_timestamp=True` when manually creating a sampling."
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/day_of_month.py` & `temporian-0.1.2/temporian/core/operators/calendar/iso_week.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,43 +8,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Calendar day of month operator class and public API function definitions."""
+"""Calendar ISO week operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
-class CalendarDayOfMonthOperator(BaseCalendarOperator):
+class CalendarISOWeekOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
-        return "CALENDAR_DAY_OF_MONTH"
+        return "CALENDAR_ISO_WEEK"
 
     @classmethod
     def output_feature_name(cls) -> str:
-        return "calendar_day_of_month"
+        return "calendar_iso_week"
 
 
-operator_lib.register_operator(CalendarDayOfMonthOperator)
+operator_lib.register_operator(CalendarISOWeekOperator)
 
 
-def calendar_day_of_month(sampling: Node) -> Node:
-    """Obtains the day of month the timestamps in a node's sampling are in.
-
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
-
-    Output feature contains numbers between 1 and 31.
+@compile
+def calendar_iso_week(sampling: EventSetNode) -> EventSetNode:
+    """Obtains the ISO week the timestamps in a node's sampling are in.
+
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
+
+    Output feature contains numbers between 1 and 53.
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    # Note: 2023-01-01 is Sunday in the same week as 2022-12-31
+        ...    timestamps=["2022-12-31", "2023-01-01", "2023-01-02", "2023-12-20"],
+        ... )
+        >>> b = tp.calendar_iso_week(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_iso_week', int32)]
+        events:
+            (4 events):
+                timestamps: [...]
+                'calendar_iso_week': [52 52 1 51]
+        ...
 
+        ```
     Args:
-        sampling: Node to get the days of month from.
+        sampling: EventSetNode to get the ISO weeks from.
 
     Returns:
-        Single feature with the day each timestamp in `sampling` belongs to.
+        Single feature with the week each timestamp in `sampling` belongs to.
     """
-    return CalendarDayOfMonthOperator(sampling).outputs["output"]
+    return CalendarISOWeekOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/day_of_week.py` & `temporian-0.1.2/temporian/core/operators/calendar/day_of_week.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Calendar day of week operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
 class CalendarDayOfWeekOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
         return "CALENDAR_DAY_OF_WEEK"
@@ -28,23 +29,40 @@
     def output_feature_name(cls) -> str:
         return "calendar_day_of_week"
 
 
 operator_lib.register_operator(CalendarDayOfWeekOperator)
 
 
-def calendar_day_of_week(sampling: Node) -> Node:
+@compile
+def calendar_day_of_week(sampling: EventSetNode) -> EventSetNode:
     """Obtains the day of the week the timestamps in a node's sampling are in.
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
 
     Output feature contains numbers from 0 (Monday) to 6 (Sunday).
 
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    timestamps=["2023-06-19", "2023-06-21", "2023-06-25", "2023-07-03"],
+        ... )
+        >>> b = tp.calendar_day_of_week(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_day_of_week', int32)]
+        events:
+            (4 events):
+                timestamps: [...]
+                'calendar_day_of_week': [0  2  6  0]
+        ...
+
+        ```
+
     Args:
-        sampling: Node to get the days of week from.
+        sampling: EventSetNode to get the days of week from.
 
     Returns:
         Single feature with the day each timestamp in `sampling` belongs to.
     """
     return CalendarDayOfWeekOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/day_of_year.py` & `temporian-0.1.2/temporian/core/operators/calendar/day_of_year.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Calendar day of year operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
 class CalendarDayOfYearOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
         return "CALENDAR_DAY_OF_YEAR"
@@ -28,23 +29,40 @@
     def output_feature_name(cls) -> str:
         return "calendar_day_of_year"
 
 
 operator_lib.register_operator(CalendarDayOfYearOperator)
 
 
-def calendar_day_of_year(sampling: Node) -> Node:
+@compile
+def calendar_day_of_year(sampling: EventSetNode) -> EventSetNode:
     """Obtains the day of year the timestamps in a node's sampling are in.
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
 
     Output feature contains numbers between 1 and 366.
 
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    timestamps=["2020-01-01", "2021-06-01", "2022-12-31", "2024-12-31"],
+        ... )
+        >>> b = tp.calendar_day_of_year(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_day_of_year', int32)]
+        events:
+            (4 events):
+                timestamps: [...]
+                'calendar_day_of_year': [ 1 152 365 366]
+        ...
+
+        ```
+
     Args:
-        sampling: Node to get the days of year from.
+        sampling: EventSetNode to get the days of year from.
 
     Returns:
         Single feature with the day each timestamp in `sampling` belongs to.
     """
     return CalendarDayOfYearOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/hour.py` & `temporian-0.1.2/temporian/core/operators/calendar/hour.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Calendar hour operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
 class CalendarHourOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
         return "CALENDAR_HOUR"
@@ -28,23 +29,41 @@
     def output_feature_name(cls) -> str:
         return "calendar_hour"
 
 
 operator_lib.register_operator(CalendarHourOperator)
 
 
-def calendar_hour(sampling: Node) -> Node:
+@compile
+def calendar_hour(sampling: EventSetNode) -> EventSetNode:
     """Obtains the hour the timestamps in a node's sampling are in.
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
 
     Output feature contains numbers between 0 and 23.
 
+    Usage example:
+        ```python
+        >>> from datetime import datetime
+        >>> a = tp.event_set(
+        ...    timestamps=[datetime(2020,1,1,18,30), datetime(2020,1,1,23,59)],
+        ... )
+        >>> b = tp.calendar_hour(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_hour', int32)]
+        events:
+            (2 events):
+                timestamps: [...]
+                'calendar_hour': [18 23]
+        ...
+
+        ```
+
     Args:
-        sampling: Node to get the hours from.
+        sampling: EventSetNode to get the hours from.
 
     Returns:
         Single feature with the hour each timestamp in `sampling` belongs to.
     """
     return CalendarHourOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/iso_week.py` & `temporian-0.1.2/temporian/core/operators/calendar/minute.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,43 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Calendar ISO week operator class and public API function definitions."""
+"""Calendar minute operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
-class CalendarISOWeekOperator(BaseCalendarOperator):
+class CalendarMinuteOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
-        return "CALENDAR_ISO_WEEK"
+        return "CALENDAR_MINUTE"
 
     @classmethod
     def output_feature_name(cls) -> str:
-        return "calendar_iso_week"
+        return "calendar_minute"
 
 
-operator_lib.register_operator(CalendarISOWeekOperator)
+operator_lib.register_operator(CalendarMinuteOperator)
 
 
-def calendar_iso_week(sampling: Node) -> Node:
-    """Obtains the ISO week the timestamps in a node's sampling are in.
+@compile
+def calendar_minute(sampling: EventSetNode) -> EventSetNode:
+    """Obtain the minute the timestamps in a node's sampling are in.
+
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
+
+    Output feature contains numbers between
+    0 and 59.
+
+    Usage example:
+        ```python
+        >>> from datetime import datetime
+        >>> a = tp.event_set(
+        ...    timestamps=[datetime(2020,1,1,18,30), datetime(2020,1,1,23,59)],
+        ...    name='random_hours'
+        ... )
+        >>> b = tp.calendar_minute(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_minute', int32)]
+        events:
+            (2 events):
+                timestamps: [...]
+                'calendar_minute': [30 59]
+        ...
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
-
-    Output feature contains numbers between 1 and 53.
+        ```
 
     Args:
-        sampling: Node to get the ISO weeks from.
+        sampling: EventSetNode to get the minutes from.
 
     Returns:
-        Single feature with the week each timestamp in `sampling` belongs to.
+        Single feature with the minute each timestamp in `sampling` belongs to.
     """
-    return CalendarISOWeekOperator(sampling).outputs["output"]
+    return CalendarMinuteOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/minute.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/hour.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,44 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Calendar minute operator class and public API function definitions."""
+from typing import Any
+from datetime import datetime
 
-from temporian.core import operator_lib
-from temporian.core.data.node import Node
-from temporian.core.operators.calendar.base import BaseCalendarOperator
+from temporian.core.operators.calendar.hour import (
+    CalendarHourOperator,
+)
+from temporian.implementation.numpy import implementation_lib
+from temporian.implementation.numpy.operators.calendar.base import (
+    BaseCalendarNumpyImplementation,
+)
 
 
-class CalendarMinuteOperator(BaseCalendarOperator):
-    @classmethod
-    def operator_def_key(cls) -> str:
-        return "CALENDAR_MINUTE"
+class CalendarHourNumpyImplementation(BaseCalendarNumpyImplementation):
+    """Numpy implementation of the calendar_hour operator."""
 
-    @classmethod
-    def output_feature_name(cls) -> str:
-        return "calendar_minute"
+    def __init__(self, operator: CalendarHourOperator) -> None:
+        super().__init__(operator)
 
+    def _get_value_from_datetime(self, dt: datetime) -> Any:
+        return dt.hour
 
-operator_lib.register_operator(CalendarMinuteOperator)
 
-
-def calendar_minute(sampling: Node) -> Node:
-    """Obtain the minute the timestamps in a node's sampling are in.
-
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
-
-    Output feature contains numbers between
-    0 and 59.
-
-    Args:
-        sampling: Node to get the minutes from.
-
-    Returns:
-        Single feature with the minute each timestamp in `sampling` belongs to.
-    """
-    return CalendarMinuteOperator(sampling).outputs["output"]
+implementation_lib.register_operator_implementation(
+    CalendarHourOperator, CalendarHourNumpyImplementation
+)
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/month.py` & `temporian-0.1.2/temporian/core/operators/calendar/month.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Calendar month operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
 class CalendarMonthOperator(BaseCalendarOperator):
     """
     Calendar operator to obtain the month each timestamp belongs to.
     """
@@ -32,24 +33,42 @@
     def output_feature_name(cls) -> str:
         return "calendar_month"
 
 
 operator_lib.register_operator(CalendarMonthOperator)
 
 
-def calendar_month(sampling: Node) -> Node:
+@compile
+def calendar_month(sampling: EventSetNode) -> EventSetNode:
     """Obtains the month the timestamps in a node's sampling are in.
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
 
     Output feature contains numbers between
     1 and 12.
 
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    timestamps=["2023-02-04", "2023-02-20", "2023-03-01", "2023-05-07"],
+        ...    name='special_events'
+        ... )
+        >>> b = tp.calendar_month(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_month', int32)]
+        events:
+            (4 events):
+                timestamps: [...]
+                'calendar_month': [2 2 3 5]
+        ...
+
+        ```
+
     Args:
-        sampling: Node with unix timestamp sampling.
+        sampling: EventSetNode with unix timestamp sampling.
 
     Returns:
         Single feature with the month each timestamp in `sampling` belongs to.
     """
     return CalendarMonthOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/second.py` & `temporian-0.1.2/temporian/core/operators/calendar/second.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Calendar second operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
 class CalendarSecondOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
         return "CALENDAR_SECOND"
@@ -28,23 +29,42 @@
     def output_feature_name(cls) -> str:
         return "calendar_second"
 
 
 operator_lib.register_operator(CalendarSecondOperator)
 
 
-def calendar_second(sampling: Node) -> Node:
+@compile
+def calendar_second(sampling: EventSetNode) -> EventSetNode:
     """Obtains the second the timestamps in a node's sampling are in.
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
 
     Output feature contains numbers between 0 and 59.
 
+    Usage example:
+        ```python
+        >>> from datetime import datetime
+        >>> a = tp.event_set(
+        ...    timestamps=[datetime(2020,1,1,18,30,55), datetime(2020,1,1,23,59,0)],
+        ...    name='random_hours'
+        ... )
+        >>> b = tp.calendar_second(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_second', int32)]
+        events:
+            (2 events):
+                timestamps: [...]
+                'calendar_second': [55 0]
+        ...
+
+        ```
+
     Args:
-        sampling: Node to get the seconds from.
+        sampling: EventSetNode to get the seconds from.
 
     Returns:
         Single feature with the second each timestamp in `sampling` belongs to.
     """
     return CalendarSecondOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/calendar/year.py` & `temporian-0.1.2/temporian/core/operators/calendar/year.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Calendar year operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
 class CalendarYearOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
         return "CALENDAR_YEAR"
@@ -28,21 +29,39 @@
     def output_feature_name(cls) -> str:
         return "calendar_year"
 
 
 operator_lib.register_operator(CalendarYearOperator)
 
 
-def calendar_year(sampling: Node) -> Node:
+@compile
+def calendar_year(sampling: EventSetNode) -> EventSetNode:
     """Obtains the year the timestamps in a node's sampling are in.
 
-    Features in the input node are ignored, only the timestamps in
-    `Node.sampling` are used and they must be unix timestamps
-    (check  `Node.sampling.is_unix_timestamp`).
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    timestamps=["2021-02-04", "2022-02-20", "2023-03-01", "2023-05-07"],
+        ...    name='random_moments'
+        ... )
+        >>> b = tp.calendar_year(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_year', int32)]
+        events:
+            (4 events):
+                timestamps: [...]
+                'calendar_year': [2021 2022 2023 2023]
+        ...
+
+        ```
 
     Args:
-        sampling: Node to get the years from.
+        sampling: EventSetNode to get the years from.
 
     Returns:
         Single feature with the year each timestamp in `sampling` belongs to.
     """
     return CalendarYearOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/cast.py` & `temporian-0.1.2/temporian/core/operators/cast.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 # limitations under the License.
 
 """Cast operator class and public API function definition."""
 
 from typing import Union, Dict, Optional, List, Any, Type
 from temporian.core.data.schema import Schema, FeatureSchema
 
-from temporian.core.data.dtypes.dtype import DType
+
 from temporian.core import operator_lib
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     Feature,
     create_node_with_new_reference,
 )
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 TypeOrDType = Union[DType, Type[float], Type[int], Type[str], Type[bool]]
 
 
-def _normalize_dtype(x: Any) -> TypeOrDType:
+def _normalize_dtype(x: Any) -> DType:
     if isinstance(x, DType):
         return x
     if x == int:
         return DType.INT64
     if x == float:
         return DType.FLOAT64
     if x == str:
@@ -43,15 +45,15 @@
         return DType.BOOLEAN
     raise ValueError(f"Cannot normalize {x!r} as a DType.")
 
 
 class CastOperator(Operator):
     def __init__(
         self,
-        input: Node,
+        input: EventSetNode,
         check_overflow: bool,
         dtype: Optional[DType] = None,
         dtype_to_dtype: Optional[Dict[DType, DType]] = None,
         feature_name_to_dtype: Optional[Dict[str, DType]] = None,
         dtypes: Optional[List[DType]] = None,
     ):
         """Constructor.
@@ -151,15 +153,15 @@
 
     @property
     def is_noop(self) -> bool:
         return self._is_noop
 
     def _build_dtypes(
         self,
-        input: Node,
+        input: EventSetNode,
         dtype: Optional[DType] = None,
         dtype_to_dtype: Optional[Dict[DType, DType]] = None,
         feature_name_to_dtype: Optional[Dict[str, DType]] = None,
     ) -> List[DType]:
         if dtype is not None:
             return [dtype] * len(input.schema.features)
 
@@ -195,61 +197,90 @@
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
 operator_lib.register_operator(CastOperator)
 
 
+@compile
 def cast(
-    input: Node,
+    input: EventSetNode,
     target: Union[
         TypeOrDType,
         Dict[str, TypeOrDType],
         Dict[TypeOrDType, TypeOrDType],
     ],
     check_overflow: bool = True,
-) -> Node:
+) -> EventSetNode:
     """Casts the dtype of features to the dtype(s) specified in `target`.
 
     Features not impacted by cast are kept.
 
-    Examples:
-        Given an input `Node` with features 'A' (`INT64`), 'B'
-        (`INT64`), 'C' (`FLOAT64`) and 'D' (`STRING`):
-
-        1. `cast(input, target=dtype.INT32)`
-           Try to convert all features to `INT32`, or raise `ValueError` if some
-           string value in 'D' is invalid, or any column value is out of range
-           for `INT32`.
-
-        2. `cast(input, target={dtype.INT64: dtype.INT32,
-                dtype.STRING: dtype.FLOAT32})`
-            Convert features 'A' and 'B' to `INT32`, 'D' to `FLOAT32`, leave 'C'
-            unchanged.
-
-        3. `cast(input, target={'A': dtype.FLOAT32, 'B': dtype.INT32})`
-            Convert 'A' to `FLOAT32` and 'B' to `INT32`.
-
-        4. `cast(input, target={'A': dtype.FLOAT32,
-                dtype.FLOAT64: dtype.INT32})`
-            Raises ValueError: don't mix dtype and feature name keys
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2],
+        ...     features={"A": [0, 2], "B": ['a', 'b'], "C": [5.0, 5.5]},
+        ... )
+
+        >>> # Cast all input features to the same dtype
+        >>> b = tp.cast(a[["A", "C"]], tp.float32)
+        >>> b
+        indexes: []
+        features: [('A', float32), ('C', float32)]
+        events:
+            (2 events):
+                timestamps: [1. 2.]
+                'A': [0. 2.]
+                'C': [5.  5.5]
+        ...
+
+
+        >>> # Cast by feature name
+        >>> b = tp.cast(a, {'A': bool, 'C': int})
+        >>> b
+        indexes: []
+        features: [('A', bool_), ('B', str_), ('C', int64)]
+        events:
+            (2 events):
+                timestamps: [1. 2.]
+                'A': [False  True]
+                'B': [b'a' b'b']
+                'C': [5  5]
+        ...
+
+        >>> # Map original_dtype -> target_dtype
+        >>> b = tp.cast(a, {float: int, int: float})
+        >>> b
+        indexes: []
+        features: [('A', float64), ('B', str_), ('C', int64)]
+        events:
+            (2 events):
+                timestamps: [1. 2.]
+                'A': [0. 2.]
+                'B': [b'a' b'b']
+                'C': [5  5]
+        ...
+
+        ```
 
     Args:
-        input: Input `Node` object to cast the columns from.
+        input: Input `EventSetNode` object to cast the columns from.
         target: Single dtype or a map. Providing a single dtype will cast all
             columns to it. The mapping keys can be either feature names or the
             original dtypes (and not both types mixed), and the values are the
             target dtypes for them. All dtypes must be temporian types (see
             `dtype.py`).
         check_overflow: Flag to check overflow when casting to a dtype with a
             shorter range (e.g: `INT64`->`INT32`). Note that this check adds
             some computation overhead. Defaults to `True`.
 
     Returns:
-        New `Node` (or the same if no features actually changed dtype), with
+        New `EventSetNode` (or the same if no features actually changed dtype), with
         the same feature names as the input one, but with the new dtypes as
         specified in `target`.
 
     Raises:
         ValueError: If `check_overflow=True` and some value is out of the range
             of the `target` dtype.
         ValueError: If trying to cast a non-numeric string to numeric dtype.
@@ -262,16 +293,20 @@
     dtype: Optional[DType] = None
     feature_name_to_dtype: Optional[Dict[str, DType]] = None
     dtype_to_dtype: Optional[Dict[DType, DType]] = None
 
     # Further type verifications are done in the operator
     if isinstance(target, dict):
         keys_are_strs = all(isinstance(v, str) for v in target.keys())
-        keys_are_dtypes = all(isinstance(v, DType) for v in target.keys())
-        values_are_dtypes = all(isinstance(v, DType) for v in target.values())
+        keys_are_dtypes = all(
+            isinstance(v, (DType, type)) for v in target.keys()
+        )
+        values_are_dtypes = all(
+            isinstance(v, (DType, type)) for v in target.values()
+        )
 
         if keys_are_strs and values_are_dtypes:
             feature_name_to_dtype = {
                 key: _normalize_dtype(value) for key, value in target.items()
             }
 
             input_feature_names = input.schema.feature_names()
```

### Comparing `temporian-0.1.1/temporian/core/operators/end.py` & `temporian-0.1.2/temporian/core/operators/begin.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""End operator class and public API function definitions."""
+"""Begin operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
-class EndOperator(Operator):
-    def __init__(self, input: Node):
+class BeginOperator(Operator):
+    def __init__(self, input: EventSetNode):
         super().__init__()
 
         self.add_input("input", input)
 
         self.add_output(
             "output",
             create_node_new_features_new_sampling(
@@ -37,34 +40,50 @@
             ),
         )
         self.check()
 
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="END",
+            key="BEGIN",
             attributes=[],
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
-operator_lib.register_operator(EndOperator)
+operator_lib.register_operator(BeginOperator)
+
 
+@compile
+def begin(input: EventSetNode) -> EventSetNode:
+    """Generates a single timestamp at the beginning of the input, per index.
+
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[5, 6, 7, -1],
+        ...     features={"f": [50, 60, 70, -10], "idx": [1, 1, 1, 2]},
+        ...     indexes=["idx"]
+        ... )
+
+        >>> a_ini = tp.begin(a)
+        >>> a_ini
+        indexes: [('idx', int64)]
+        features: []
+        events:
+            idx=2 (1 events):
+                timestamps: [-1.]
+            idx=1 (1 events):
+                timestamps: [5.]
+        ...
 
-def end(input: Node) -> Node:
-    """Generates a single timestamp at the end of the input.
+        ```
 
     Args:
         input: Guide input
 
-    Example:
-        Input
-            timestamps: [1, 5, 10]
-        Output
-            timestamps: [10]
-
     Returns:
         A feature-less node with a single timestamp.
     """
-
-    return EndOperator(input=input).outputs["output"]
+    return BeginOperator(input=input).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/filter.py` & `temporian-0.1.2/temporian/core/operators/filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 # limitations under the License.
 
 """Filter operator class and public API function definition."""
 
 from typing import Optional
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class FilterOperator(Operator):
-    def __init__(self, input: Node, condition: Node):
+    def __init__(self, input: EventSetNode, condition: EventSetNode):
         super().__init__()
 
         # check that condition is a single feature
         if len(condition.schema.features) != 1:
             raise ValueError(
                 "Condition must be a single feature. Got"
                 f" {condition.schema} instead."
@@ -72,37 +76,59 @@
         )
 
 
 operator_lib.register_operator(FilterOperator)
 
 
 # pylint: disable=redefined-builtin
+@compile
 def filter(
-    input: Node,
-    condition: Optional[Node] = None,
-) -> Node:
-    """Filters out timestamps in a node for which a condition is false.
+    input: EventSetNode,
+    condition: Optional[EventSetNode] = None,
+) -> EventSetNode:
+    """Filters out events in an EventSetNode for which a condition is false.
 
     Each timestamp in `input` is only kept if the corresponding value for that
     timestamp in `condition` is `True`.
 
-    `input` and `condition` must have the same sampling.
+    `input` and `condition` must have the same sampling, and `condition` must
+    have one single feature, of boolean type.
 
     filter(x) is equivalent to filter(x,x). filter(x) can be used to convert
-    a boolean mask into a timestamps. For example:
-        Input:
-            timestamps: 1 2 3
-            value: True False True
-        Output:
-            timestamps: 1 3
-            value: True True
+    a boolean mask into a timestamps.
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 5, 6],
+        ...     features={"f1": [0, 10, 50, 60], "f2": [50, 100, 500, 600]},
+        ... )
+
+        >>> # Example boolean condition
+        >>> condition = a["f1"] > 20
+        >>> condition
+        indexes: ...
+                timestamps: [0. 1. 5. 6.]
+                'f1': [False False  True  True]
+        ...
+
+        >>> # Filter only True timestamps
+        >>> filtered = tp.filter(a, condition)
+        >>> filtered
+        indexes: ...
+                timestamps: [5. 6.]
+                'f1': [50 60]
+                'f2': [500 600]
+        ...
+
+        ```
 
     Args:
-        input: Node to filter.
-        condition: Node with a single boolean feature condition.
+        input: EventSetNode to filter.
+        condition: EventSetNode with a single boolean feature condition.
 
     Returns:
         Filtered input.
     """
 
     if condition is None:
         condition = input
```

### Comparing `temporian-0.1.1/temporian/core/operators/glue.py` & `temporian-0.1.2/temporian/core/operators/select.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,142 +8,148 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Glue operator class and public API function definition."""
+"""Select operator class and public API function definition."""
+
+from typing import List, Union
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_with_new_reference
-from temporian.core.data.schema import Schema
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_with_new_reference,
+)
 from temporian.core.operators.base import Operator
+from temporian.core.data.schema import Schema
 from temporian.proto import core_pb2 as pb
 
-# Maximum number of arguments taken by the glue operator
-MAX_NUM_ARGUMENTS = 30
 
-
-class GlueOperator(Operator):
-    def __init__(
-        self,
-        **inputs: Node,
-    ):
+class SelectOperator(Operator):
+    def __init__(self, input: EventSetNode, feature_names: List[str]):
         super().__init__()
 
-        # Note: Support for dictionaries of nodes is required for
-        # serialization.
-
-        if len(inputs) < 2:
-            raise ValueError("At least two arguments should be provided")
+        self._feature_names = feature_names
+        self.add_attribute("feature_names", feature_names)
+        self.add_input("input", input)
 
-        if len(inputs) >= MAX_NUM_ARGUMENTS:
-            raise ValueError(
-                f"Too many (>{MAX_NUM_ARGUMENTS}) arguments provided"
-            )
-
-        # inputs
+        # outputs
         output_features = []
         output_feature_schemas = []
-        feature_names = set()
-        first_sampling_node = None
-
-        for key, input in inputs.items():
-            self.add_input(key, input)
-
-            output_features.extend(input.feature_nodes)
-            output_feature_schemas.extend(input.schema.features)
+        input_feature_names = input.schema.feature_names()
 
-            for f in input.schema.features:
-                if f.name in feature_names:
-                    raise ValueError(
-                        f'Feature "{f.name}" is defined in multiple input'
-                        " nodes to glue. Consider using prefix() or rename()."
-                    )
-                feature_names.add(f.name)
-
-            if first_sampling_node is None:
-                first_sampling_node = input
-            else:
-                input.check_same_sampling(first_sampling_node)
-
-        assert first_sampling_node is not None
+        for feature_name in feature_names:
+            if feature_name not in input_feature_names:
+                raise IndexError(
+                    f"Selected features {feature_name!r} is not part of the"
+                    f" available features {input_feature_names!r}."
+                )
+            feature_idx = input_feature_names.index(feature_name)
+            output_features.append(input.feature_nodes[feature_idx])
+            output_feature_schemas.append(input.schema.features[feature_idx])
 
         self.add_output(
             "output",
             create_node_with_new_reference(
                 schema=Schema(
                     features=output_feature_schemas,
-                    indexes=first_sampling_node.schema.indexes,
-                    is_unix_timestamp=first_sampling_node.schema.is_unix_timestamp,
+                    indexes=input.schema.indexes,
+                    is_unix_timestamp=input.schema.is_unix_timestamp,
                 ),
-                sampling=first_sampling_node.sampling_node,
+                sampling=input.sampling_node,
                 features=output_features,
                 creator=self,
             ),
         )
         self.check()
 
+    @property
+    def feature_names(self) -> List[str]:
+        return self._feature_names
+
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="GLUE",
-            # TODO: Add support to array of nodes arguments.
-            inputs=[
-                pb.OperatorDef.Input(key=f"input_{idx}", is_optional=idx >= 2)
-                for idx in range(MAX_NUM_ARGUMENTS)
+            key="SELECT",
+            attributes=[
+                pb.OperatorDef.Attribute(
+                    key="feature_names",
+                    type=pb.OperatorDef.Attribute.Type.LIST_STRING,
+                    is_optional=False,
+                ),
             ],
+            inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
-operator_lib.register_operator(GlueOperator)
-
-
-def glue(
-    *inputs: Node,
-) -> Node:
-    """Concatenates together nodes with the same sampling.
+operator_lib.register_operator(SelectOperator)
 
-    Example:
 
-        ```python
-        >>> a = tp.input_node(features=[("A1", tp.str_), ("A2", tp.int32)])
-        >>> b = tp.input_node(features=[("B", tp.float64)], same_sampling_as=a)
-        >>> c = tp.input_node(features=[("C", tp.float64)], same_sampling_as=a)
-        >>> output = tp.glue(a, b, c)
-        >>> output.features
-        [('A1', str_), ('A2', int32), ('B', float64), ('C', float64)]
-
-        ```
+@compile
+def select(
+    input: EventSetNode,
+    feature_names: Union[str, List[str]],
+) -> EventSetNode:
+    """Selects a subset of features from an EventSetNode.
 
-    To concatenate nodes with different samplings, use
-    [`tp.resample()`][temporian.resample] first.
-
-    Example:
+    Args:
+        input: EventSetNode to select features from.
+        feature_names: Name or list of names of the features to select from the
+            input.
 
+    Usage example:
         ```python
-        >>> a = tp.input_node(features=[("A", tp.str_)])
-        >>> b = tp.input_node(features=[("B", tp.float64)])
-        >>> c = tp.input_node(features=[("C", tp.float64)])
-        >>> output = tp.glue(a,
-        ...                  tp.resample(b, sampling=a),
-        ...                  tp.resample(c, sampling=a)
-        ...          )
-        >>> output.features
-        [('A', str_), ('B', float64), ('C', float64)]
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2],
+        ...     features={"A": [1, 2], "B": ['s', 'm'], "C": [5.0, 5.5]},
+        ... )
+
+        >>> # Select single feature
+        >>> b = tp.select(a, 'B')
+        >>> # Equivalent
+        >>> b = a['B']
+        >>> b
+        indexes: []
+        features: [('B', str_)]
+        events:
+            (2 events):
+                timestamps: [1. 2.]
+                'B': [b's' b'm']
+        ...
+
+        >>> # Select multiple features
+        >>> bc = tp.select(a, ['B', 'C'])
+        >>> # Equivalent
+        >>> bc = a[['B', 'C']]
+        >>> bc
+        indexes: []
+        features: [('B', str_), ('C', float64)]
+        events:
+            (2 events):
+                timestamps: [1. 2.]
+                'B': [b's' b'm']
+                'C': [5.  5.5]
+        ...
 
         ```
 
-    Args:
-        *inputs: Nodes to concatenate.
 
     Returns:
-        Concatenated nodes.
+        EventSetNode containing only the selected features.
     """
-    if len(inputs) == 1:
-        return inputs[0]
+    if isinstance(feature_names, list) and all(
+        isinstance(f, str) for f in feature_names
+    ):
+        pass
+    elif isinstance(feature_names, str):
+        feature_names = [feature_names]
+    else:
+        raise TypeError(
+            "Unexpected type for feature_names. Expect str or list of"
+            f" str. Got '{feature_names}' instead."
+        )
 
-    # Note: The node should be called "input_{idx}" with idx in [0, MAX_NUM_ARGUMENTS).
-    inputs_dict = {f"input_{idx}": input for idx, input in enumerate(inputs)}
-    return GlueOperator(**inputs_dict).outputs["output"]
+    return SelectOperator(input, feature_names).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/lag.py` & `temporian-0.1.2/temporian/core/operators/window/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,93 +8,104 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Lag operator class and public API function definitions."""
+"""Base calendar operator class definition."""
 
-from temporian.core import operator_lib
-from temporian.core.data.duration_utils import (
-    Duration,
-    NormalizedDuration,
-    normalize_duration,
+from abc import ABC, abstractmethod
+from typing import Optional
+
+
+from temporian.core.data.duration_utils import NormalizedDuration
+from temporian.core.data.dtype import DType
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_existing_sampling,
 )
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
-class LagOperator(Operator):
+class BaseWindowOperator(Operator, ABC):
+    """Interface definition and common logic for window operators."""
+
     def __init__(
         self,
-        input: Node,
-        duration: NormalizedDuration,
+        input: EventSetNode,
+        window_length: NormalizedDuration,
+        sampling: Optional[EventSetNode] = None,
     ):
         super().__init__()
 
-        self._duration = duration
+        self._window_length = window_length
+        self.add_attribute("window_length", window_length)
+
+        self._has_sampling = sampling is not None
+        if self._has_sampling:
+            assert sampling is not None
+
+            self.add_input("sampling", sampling)
+            effective_sampling_node = sampling
+
+            input.schema.check_compatible_index(sampling.schema)
+
+        else:
+            effective_sampling_node = input
 
         self.add_input("input", input)
-        self.add_attribute("duration", duration)
+
+        feature_schemas = [  # pylint: disable=g-complex-comprehension
+            FeatureSchema(
+                name=f.name,
+                dtype=self.get_feature_dtype(f),
+            )
+            for f in input.schema.features
+        ]
 
         self.add_output(
             "output",
-            create_node_new_features_new_sampling(
-                features=input.schema.features,
-                indexes=input.schema.indexes,
-                is_unix_timestamp=input.schema.is_unix_timestamp,
+            create_node_new_features_existing_sampling(
+                features=feature_schemas,
+                sampling_node=effective_sampling_node,
                 creator=self,
             ),
         )
+
         self.check()
 
     @property
-    def duration(self) -> Duration:
-        return self._duration
+    def window_length(self) -> NormalizedDuration:
+        return self._window_length
+
+    @property
+    def has_sampling(self) -> bool:
+        return self._has_sampling
 
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="LAG",
+            key=cls.operator_def_key(),
             attributes=[
                 pb.OperatorDef.Attribute(
-                    key="duration",
+                    key="window_length",
                     type=pb.OperatorDef.Attribute.Type.FLOAT_64,
-                    is_optional=False,
                 ),
             ],
-            inputs=[pb.OperatorDef.Input(key="input")],
+            inputs=[
+                pb.OperatorDef.Input(key="input"),
+                pb.OperatorDef.Input(key="sampling", is_optional=True),
+            ],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
-
-operator_lib.register_operator(LagOperator)
-
-
-def lag(input: Node, duration: Duration) -> Node:
-    """Adds a delay to the timestamps.
-
-    In other words, shifts the timestamp values forwards in time.
-
-    Example:
-        Input
-            timestamps: [1, 5, 10]
-            duration: 2
-        Output
-            timestamps: [3, 8, 13]
-
-    Args:
-        input: Node to lag.
-        duration: Duration to lag by.
-
-    Returns:
-        Lagged node.
-    """
-
-    normalized_duration = normalize_duration(duration)
-
-    return LagOperator(
-        input=input,
-        duration=normalized_duration,
-    ).outputs["output"]
+    @classmethod
+    @abstractmethod
+    def operator_def_key(cls) -> str:
+        """Gets the key of the operator definition."""
+
+    @abstractmethod
+    def get_feature_dtype(self, feature: FeatureSchema) -> DType:
+        """Gets the dtype of the output feature."""
```

### Comparing `temporian-0.1.1/temporian/core/operators/leak.py` & `temporian-0.1.2/temporian/core/operators/leak.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Lag operator class and public API function definitions."""
 
 
 from temporian.core import operator_lib
+from temporian.core.compilation import compile
 from temporian.core.data.duration_utils import (
     Duration,
     NormalizedDuration,
     normalize_duration,
 )
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class LeakOperator(Operator):
     def __init__(
         self,
-        input: Node,
+        input: EventSetNode,
         duration: NormalizedDuration,
     ):
         super().__init__()
 
         self._duration = duration
 
         self.add_input("input", input)
@@ -69,32 +73,43 @@
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
 operator_lib.register_operator(LeakOperator)
 
 
-def leak(input: Node, duration: Duration) -> Node:
-    """Move timestamps in the past.
+@compile
+def leak(input: EventSetNode, duration: Duration) -> EventSetNode:
+    """Subtracts a duration from an EventSetNode's timestamps.
 
     In other words, shifts the timestamp values backward in time.
 
     Note that this operator moves future data into the past, and should be used
     with caution to prevent unwanted future leakage. For instance, this op
     should generally not be used to compute the input features of a model.
 
-    Example:
-        Input
-            timestamps: [1, 5, 10]
-            duration: 2
-        Output
-            timestamps: [-1, 2, 7]
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 5, 6],
+        ...     features={"value": [0, 1, 5, 6]},
+        ... )
+
+        >>> b = tp.leak(a, tp.duration.seconds(2))
+        >>> b
+        indexes: ...
+            (4 events):
+                timestamps: [-2. -1. 3. 4.]
+                'value': [0 1 5 6]
+        ...
+
+        ```
 
     Args:
-        input: Node to leak.
+        input: EventSetNode to leak.
         duration: Duration to leak by.
 
     Returns:
         Leaked node.
     """
 
     normalized_duration = normalize_duration(duration)
```

### Comparing `temporian-0.1.1/temporian/core/operators/propagate.py` & `temporian-0.1.2/temporian/core/operators/propagate.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 # limitations under the License.
 
 """Propagate operator class and public API function definition."""
 
 
 from typing import List
 from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.operators.base import Operator
 from temporian.core.operators.resample import Resample
 from temporian.proto import core_pb2 as pb
 
 
 class Propagate(Operator):
     def __init__(
         self,
-        input: Node,
-        sampling: Node,
+        input: EventSetNode,
+        sampling: EventSetNode,
     ):
         super().__init__()
 
         self.add_input("input", input)
         self.add_input("sampling", sampling)
 
         self._index_mapping: List[int] = []
@@ -41,19 +45,19 @@
 
         for index in input.schema.indexes:
             try:
                 sampling_idx = sampling_index_name.index(index.name)
                 self._index_mapping.append(sampling_idx)
             except ValueError as exc:
                 raise ValueError(
-                    "The index of input should be contained in the index of"
+                    "The indexes of input should be contained in the indexes of"
                     f' sampling. Index "{index.name}" from input is not'
-                    " available in sampling. input.index="
+                    " available in sampling. input.indexes="
                     f" {input.schema.indexes},"
-                    f" sampling.index={sampling.schema.indexes}."
+                    f" sampling.indexes={sampling.schema.indexes}."
                 ) from exc
             if sampling_index_dtypes[sampling_idx] != index.dtype:
                 raise ValueError(
                     f'The index "{index.name}" is found both in the input and'
                     " sampling argument. However, the dtype is different."
                     f" {index.dtype} != {sampling_index_dtypes[sampling_idx]}"
                 )
@@ -89,45 +93,80 @@
 
 
 operator_lib.register_operator(Propagate)
 
 
 # TODO: Do we want for "propagate" to take a list of feature names
 # (like add_index) instead?
-def propagate(input: Node, sampling: Node, resample: bool = False) -> Node:
+@compile
+def propagate(
+    input: EventSetNode, sampling: EventSetNode, resample: bool = False
+) -> EventSetNode:
     """Propagates feature values over a sub index.
 
-    Given `input` and `sampling` where `input` has a super index of
-    `sampling` (e.g., the index of `input` is `["x"]`, and the index of
-    `sampling` is `["x","y"]`), duplicates the features of `input` over the
-    index of `sampling`.
-
-    Example:
-
-        Inputs:
-            input:
-                feature_1: ...
-                feature_2: ...
-                index: ["x"]
-            sampling:
-                index: ["x", "y"]
-
-        Output:
-            feature_1: ...
-            feature_2: ...
-            index: ["x", "y"]
+    Given `input` and `sampling` where `input`'s indexes are a superset of
+    `sampling`'s (e.g., the indexes of `input` are `["x"]`, and the indexes of
+    `sampling` are `["x","y"]`), duplicates the features of `input` over the
+    indexes of `sampling`.
+
+    Example use case:
+        ```python
+        >>> products = tp.event_set(
+        ...     timestamps=[1, 2, 3, 1, 2, 3],
+        ...     features={
+        ...         "product": [1, 1, 1, 2, 2, 2],
+        ...         "sales": [100., 200., 500., 1000., 2000., 5000.]
+        ...     },
+        ...     indexes=["product"],
+        ... )
+        >>> store = tp.event_set(
+        ...     timestamps=[1, 2, 3, 4, 5],
+        ...     features={
+        ...         "sales": [10000., 20000., 30000., 5000., 1000.]
+        ...     },
+        ... )
+
+        >>> # First attempt: divide to calculate fraction of total store sales
+        >>> products / store
+        Traceback (most recent call last):
+            ...
+        ValueError: Arguments don't have the same index. ...
+
+        >>> # Second attempt: propagate index
+        >>> store_prop = tp.propagate(store, products)
+        >>> products / store_prop
+        Traceback (most recent call last):
+            ...
+        ValueError: Arguments should have the same sampling. ...
+
+        >>> # Third attempt: propagate + resample
+        >>> store_resample = tp.propagate(store, products, resample=True)
+        >>> div = products / store_resample
+        >>> div
+        indexes: [('product', int64)]
+        features: [('div_sales_sales', float64)]
+        events:
+            product=1 (3 events):
+                timestamps: [1. 2. 3.]
+                'div_sales_sales': [0.01   0.01   0.0167]
+            product=2 (3 events):
+                timestamps: [1. 2. 3.]
+                'div_sales_sales': [0.1    0.1    0.1667]
+        ...
+
+        ```
 
     Args:
-        input: Node to propagate.
+        input: EventSetNode to propagate.
         sampling: Index to propagate over.
         resample: If true, apply a [`tp.resample()`][temporian.resample] before
             propagating, for the output to have the same sampling as `sampling`.
 
     Returns:
-        Node propagated over `sampling`'s index.
+        EventSetNode propagated over `sampling`'s index.
     """
 
     result = Propagate(
         input=input,
         sampling=sampling,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/rename.py` & `temporian-0.1.2/temporian/core/operators/rename.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,52 +12,53 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Rename operator."""
 from typing import Dict, Optional, Union
 
 from temporian.core import operator_lib
+from temporian.core.compilation import compile
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_new_sampling,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.data.schema import Schema
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class RenameOperator(Operator):
     """Rename operator."""
 
     def __init__(
         self,
-        input: Node,
+        input: EventSetNode,
         features: Dict[str, str],
-        index: Dict[str, str],
+        indexes: Dict[str, str],
     ):
         super().__init__()
 
         self.add_attribute("features", features)
-        self.add_attribute("index", index)
+        self.add_attribute("indexes", indexes)
 
         self._features = features
-        self._index = index
+        self._indexes = indexes
 
         self.add_input("input", input)
 
         new_indexes = [
-            (index.get(i.name, i.name), i.dtype) for i in input.schema.indexes
+            (indexes.get(i.name, i.name), i.dtype) for i in input.schema.indexes
         ]
         new_feature_schemas = [
             (features.get(f.name, f.name), f.dtype)
             for f in input.schema.features
         ]
 
-        if index:
+        if indexes:
             self.add_output(
                 "output",
                 create_node_new_features_new_sampling(
                     features=new_feature_schemas,
                     indexes=new_indexes,
                     is_unix_timestamp=input.schema.is_unix_timestamp,
                     creator=self,
@@ -77,27 +78,27 @@
 
     @property
     def features(self) -> Dict[str, str]:
         return self._features
 
     @property
     def index(self) -> Dict[str, str]:
-        return self._index
+        return self._indexes
 
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
             key="RENAME",
             attributes=[
                 pb.OperatorDef.Attribute(
                     key="features",
                     type=pb.OperatorDef.Attribute.Type.MAP_STR_STR,
                 ),
                 pb.OperatorDef.Attribute(
-                    key="index",
+                    key="indexes",
                     type=pb.OperatorDef.Attribute.Type.MAP_STR_STR,
                 ),
             ],
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
@@ -112,15 +113,15 @@
     if features is None:
         return {}
 
     if isinstance(features, str):
         if len(schema.features) != 1:
             raise ValueError(
                 "Cannot apply rename operator with a single rename string when "
-                "the event set contains multiple features. Pass a dictionary "
+                "the EventSet contains multiple features. Pass a dictionary "
                 "of rename strings instead."
             )
         features = {schema.features[0].name: features}
 
     feature_dict = schema.feature_name_to_dtype()
 
     if len(features) != len(set(features.values())):
@@ -141,15 +142,15 @@
     if indexes is None:
         return {}
 
     if isinstance(indexes, str):
         if len(schema.indexes) != 1:
             raise ValueError(
                 "Cannot apply rename operator with a single rename string when "
-                "the event set contains multiple indexes. Pass a dictionary "
+                "the EventSet contains multiple indexes. Pass a dictionary "
                 "of rename strings instead."
             )
         indexes = {schema.indexes[0].name: indexes}
 
     indexes_dict = schema.index_name_to_dtype()
 
     if len(indexes) != len(set(indexes.values())):
@@ -159,37 +160,71 @@
         if dst == "":
             raise ValueError("Cannot rename to an empty string")
         if src not in indexes_dict:
             raise KeyError(f"The index {src!r} does not exist.")
     return indexes
 
 
+@compile
 def rename(
-    input: Node,
+    input: EventSetNode,
     features: Optional[Union[str, Dict[str, str]]] = None,
-    index: Optional[Union[str, Dict[str, str]]] = None,
-) -> Node:
-    """Renames a node's features and index.
+    indexes: Optional[Union[str, Dict[str, str]]] = None,
+) -> EventSetNode:
+    """Renames an EventSetNode's features and index.
 
     If the input has a single feature, then the `features` can be a
     single string with the new name.
 
     If the input has multiple features, then `features` must be a mapping
     with the old names as keys and the new names as values.
 
-    The index renaming follows the same criteria, accepting a single string or
-    a mapping for multiple index levels.
+    The indexes renaming follows the same criteria, accepting a single string or
+    a mapping for multiple indexes.
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    timestamps=[0, 1],
+        ...    features={"f1": [0, 2], "f2": [5, 6]}
+        ... )
+        >>> b = 5 * a
+
+        >>> # Rename single feature
+        >>> b_1 = tp.rename(b["f1"], "f1_result")
+        >>> b_1
+        indexes: []
+        features: [('f1_result', int64)]
+        events:
+             (2 events):
+                timestamps: [0. 1.]
+                'f1_result': [ 0 10]
+        ...
+
+        >>> # Rename multiple features
+        >>> b_rename = tp.rename(b, {"f1": "5xf1", "f2": "5xf2"})
+        >>> b_rename
+        indexes: []
+        features: [('5xf1', int64), ('5xf2', int64)]
+        events:
+             (2 events):
+                timestamps: [0. 1.]
+                '5xf1': [ 0 10]
+                '5xf2': [25 30]
+        ...
+
+        ```
 
     Args:
-        input: Node to rename.
+        input: EventSetNode to rename.
 
         features: New feature name or mapping from old names to new names.
-        index: New index name or mapping from old names to new names.
+        indexes: New index name or mapping from old names to new names.
 
     Returns:
-        Node with renamed features and index.
+        EventSetNode with renamed features and index.
     """
 
     features = _normalize_rename_features(input.schema, features)
-    index = _normalize_rename_indexes(input.schema, index)
+    indexes = _normalize_rename_indexes(input.schema, indexes)
 
-    return RenameOperator(input, features, index).outputs["output"]
+    return RenameOperator(input, features, indexes).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/resample.py` & `temporian-0.1.2/temporian/core/operators/resample.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Resample operator class and public API function definition."""
 
 from temporian.core import operator_lib
+from temporian.core.compilation import compile
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class Resample(Operator):
     def __init__(
         self,
-        input: Node,
-        sampling: Node,
+        input: EventSetNode,
+        sampling: EventSetNode,
     ):
         super().__init__()
 
         self.add_input("input", input)
         self.add_input("sampling", sampling)
 
         input.schema.check_compatible_index(sampling.schema)
@@ -58,46 +59,45 @@
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
 operator_lib.register_operator(Resample)
 
 
+@compile
 def resample(
-    input: Node,
-    sampling: Node,
-) -> Node:
-    """Resamples a node at each timestamp of a sampling.
+    input: EventSetNode,
+    sampling: EventSetNode,
+) -> EventSetNode:
+    """Resamples an EventSetNode at each timestamp of another EventSetNode.
 
     If a timestamp in `sampling` does not have a corresponding timestamp in
     `input`, the last timestamp in `input` is used instead. If this timestamp
     is anterior to an value in `input`, the value is replaced by
     `dtype.MissingValue(...)`.
 
     Example:
 
         ```python
-        >>> evset = tp.event_set(
+        >>> a = tp.event_set(
         ...     timestamps=[1, 5, 8, 9],
         ...     features={"f1": [1.0, 2.0, 3.0, 4.0]}
         ... )
-        >>> sampling = tp.event_set(timestamps=[-1, 1, 6, 10])
-        >>> input_node = evset.node()
-        >>> sampling_node = sampling.node()
-        >>> out_node = tp.resample(input_node, sampling=sampling_node)
-        >>> out_node.evaluate({input_node: evset, sampling_node: sampling})
+        >>> b = tp.event_set(timestamps=[-1, 1, 6, 10])
+        >>> c = tp.resample(a, sampling=b)
+        >>> c
         indexes: ...
                 timestamps: [-1.  1.  6. 10.]
                 'f1': [nan  1.  2.  4.]
         ...
 
         ```
 
     Args:
-        input: Node to sample.
-        sampling: Node to use the sampling of.
+        input: EventSetNode to sample.
+        sampling: EventSetNode to use the sampling of.
 
     Returns:
         Resampled node, with same sampling as `sampling`.
     """
 
     return Resample(input=input, sampling=sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/scalar/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/operators/binary/BUILD`

 * *Files 19% similar despite different names*

```diff
@@ -3,64 +3,68 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "scalar",
+    name = "binary",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
     deps = [
-        "api_symbols",
-        ":arithmetic_scalar",
-        ":relational_scalar",
+        ":arithmetic",
+        ":logical",
+        ":relational",
     ],
 )
 
 py_library(
-    name = "api_symbols",
-    srcs = ["api_symbols.py"],
+    name = "base",
+    srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        ":arithmetic_scalar",
-        ":relational_scalar",
+        # already_there/numpy
+        "//temporian/core/data:dtype",
+        "//temporian/core/operators/binary:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy/operators:base",
     ],
 )
 
 py_library(
-    name = "base",
-    srcs = ["base.py"],
+    name = "arithmetic",
+    srcs = ["arithmetic.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/core/operators:base",
-        "//temporian/proto:core_py_proto",
+        ":base",
+        # already_there/numpy
+        "//temporian/core/data:dtype",
+        "//temporian/core/operators/binary",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "arithmetic_scalar",
-    srcs = ["arithmetic_scalar.py"],
+    name = "relational",
+    srcs = ["relational.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
-        "//temporian/core/data/dtypes:dtype",
+        # already_there/numpy
+        "//temporian/core/data:dtype",
+        "//temporian/core/operators/binary",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "relational_scalar",
-    srcs = ["relational_scalar.py"],
+    name = "logical",
+    srcs = ["logical.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
+        # already_there/numpy
+        "//temporian/core/data:dtype",
+        "//temporian/core/operators/binary",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/operators/scalar/base.py` & `temporian-0.1.2/temporian/core/operators/scalar/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,48 +12,53 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base scalar operator class definition."""
 
 from typing import Union, List
 
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class BaseScalarOperator(Operator):
     """Interface definition and common code for scalar operators."""
 
     DEF_KEY = ""
 
     def __init__(
         self,
-        input: Node,
-        value: Union[float, int, str, bool],
+        input: EventSetNode,
+        value: Union[float, int, str, bytes, bool],
         is_value_first: bool = False,  # useful for non-commutative operators
     ):
         super().__init__()
 
+        if isinstance(value, str):
+            value = value.encode()
+
         self.value = value
         self.is_value_first = is_value_first
 
         # inputs
         self.add_input("input", input)
 
         self.add_attribute("value", value)
         self.add_attribute("is_value_first", is_value_first)
 
-        if not isinstance(input, Node):
-            raise TypeError(f"Input must be of type Node but got {type(input)}")
+        if not isinstance(input, EventSetNode):
+            raise TypeError(
+                f"Input must be of type EventSetNode but got {type(input)}"
+            )
 
         # check that every dtype of input feature is equal to value dtype
         value_dtype = DType.from_python_type(type(value))
 
         # check that value dtype is in self.dtypes_to_check
         if value_dtype not in self.supported_value_dtypes:
             raise ValueError(
@@ -63,14 +68,15 @@
 
         # Check that the feature dtype doesn't need an upcast to operate with
         # this value type
         self.map_vtype_dtype = {
             float: [DType.FLOAT32, DType.FLOAT64],
             int: [DType.INT32, DType.INT64, DType.FLOAT32, DType.FLOAT64],
             str: [DType.STRING],
+            bytes: [DType.STRING],
             bool: [
                 DType.BOOLEAN,
                 DType.INT32,
                 DType.INT64,
                 DType.FLOAT32,
                 DType.FLOAT64,
             ],
```

### Comparing `temporian-0.1.1/temporian/core/operators/since_last.py` & `temporian-0.1.2/temporian/core/operators/since_last.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,40 +13,39 @@
 # limitations under the License.
 
 """Resample operator class and public API function definition."""
 
 from typing import Optional
 
 from temporian.core import operator_lib
+from temporian.core.compilation import compile
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 
 
 class SinceLast(Operator):
     def __init__(
         self,
-        input: Node,
-        sampling: Optional[Node] = None,
+        input: EventSetNode,
+        sampling: Optional[EventSetNode] = None,
     ):
         super().__init__()
 
         self.add_input("input", input)
 
         if sampling is not None:
             self.add_input("sampling", sampling)
             self._has_sampling = True
             effective_sampling_node = sampling
-            input.schema.check_compatible_index(
-                sampling.schema, "input and sampling"
-            )
+            input.schema.check_compatible_index(sampling.schema)
 
         else:
             effective_sampling_node = input
             self._has_sampling = False
 
         self.add_output(
             "output",
@@ -74,46 +73,42 @@
     def has_sampling(self) -> bool:
         return self._has_sampling
 
 
 operator_lib.register_operator(SinceLast)
 
 
+@compile
 def since_last(
-    input: Node,
-    sampling: Optional[Node] = None,
-) -> Node:
-    """Amount of time since the last distinct timestamp.
+    input: EventSetNode,
+    sampling: Optional[EventSetNode] = None,
+) -> EventSetNode:
+    """Computes the amount of time since the last distinct timestamp.
 
     Example 1:
         ```python
-        >>> t_evset = tp.event_set(timestamps=[1, 5, 8, 8, 9])
-        >>> t_node = t_evset.node()
-        >>> since_node = tp.since_last(t_node)
-        >>> since_node.evaluate({t_node: t_evset})
+        >>> a = tp.event_set(timestamps=[1, 5, 8, 8, 9])
+        >>> b = tp.since_last(a)
+        >>> b
         indexes: ...
                 timestamps: [1. 5. 8. 8. 9.]
                 'since_last': [nan  4.  3.  0.  1.]
         ...
 
         ```
 
     Example 2:
         ```python
-        >>> since_evset = tp.event_set(timestamps=[2, 5, 7])
-        >>> sampling_evset = tp.event_set(timestamps=[1, 4, 6, 10])
-        >>> since_node = since_evset.node()
-        >>> sampling_node = sampling_evset.node()
+        >>> a = tp.event_set(timestamps=[2, 5, 7])
+        >>> b = tp.event_set(timestamps=[1, 4, 6, 10])
 
         >>> # Time elapsed between each sampling event
-        >>> # and the latest previous event in since_evset
-        >>> result = tp.since_last(since_node, sampling_node)
-        >>> result.evaluate({since_node: since_evset,
-        ...     sampling_node: sampling_evset}
-        ... )
+        >>> # and the latest previous event in a
+        >>> c = tp.since_last(a, sampling=b)
+        >>> c
         indexes: ...
                 timestamps: [ 1. 4. 6. 10.]
                 'since_last': [nan  2.  1.  3.]
         ...
 
         ```
```

### Comparing `temporian-0.1.1/temporian/core/operators/test/propagate_test.py` & `temporian-0.1.2/temporian/core/operators/test/propagate_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from absl.testing import absltest
 
 from temporian.core.data.node import input_node
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.operators.propagate import propagate
 
 
 class PropagateOperatorTest(absltest.TestCase):
     def setUp(self):
         pass
 
@@ -51,15 +51,18 @@
         sampling = input_node(
             [],
             indexes=[("x", DType.STRING), ("y", DType.STRING)],
             is_unix_timestamp=False,
         )
         with self.assertRaisesRegex(
             ValueError,
-            "The index of input should be contained in the index of sampling",
+            (
+                "The indexes of input should be contained in the indexes of"
+                " sampling"
+            ),
         ):
             _ = propagate(input=node, sampling=sampling)
 
     def test_error_wrong_index_type(self):
         node = input_node(
             [
                 ("a", DType.FLOAT64),
```

### Comparing `temporian-0.1.1/temporian/core/operators/tick.py` & `temporian-0.1.2/temporian/core/operators/tick.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,26 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Tick operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 from temporian.core.data.duration_utils import (
     Duration,
     NormalizedDuration,
     normalize_duration,
 )
 
 
 class Tick(Operator):
-    def __init__(self, input: Node, interval: NormalizedDuration, align: bool):
+    def __init__(
+        self, input: EventSetNode, interval: NormalizedDuration, align: bool
+    ):
         super().__init__()
 
         self._interval = interval
         self._align = align
 
         self.add_input("input", input)
         self.add_attribute("interval", interval)
@@ -76,43 +82,50 @@
         )
 
 
 operator_lib.register_operator(Tick)
 
 
 # TODO: Add support for begin/end arguments.
-def tick(input: Node, interval: Duration, align: bool = True) -> Node:
+@compile
+def tick(
+    input: EventSetNode, interval: Duration, align: bool = True
+) -> EventSetNode:
     """Generates timestamps at regular intervals in the range of a guide.
 
+    Example with align:
+        ```python
+        >>> a = tp.event_set(timestamps=[5, 9, 16])
+        >>> b = tp.tick(a, interval=tp.duration.seconds(3), align=True)
+        >>> b
+        indexes: ...
+                timestamps: [ 6. 9. 12. 15.]
+        ...
+
+        ```
+
+    Example without align:
+        ```python
+        >>> a = tp.event_set(timestamps=[5, 9, 16])
+        >>> b = tp.tick(a, interval=tp.duration.seconds(3), align=False)
+        >>> b
+        indexes: ...
+                timestamps: [ 5. 8. 11. 14.]
+        ...
+
+        ```
+
     Args:
         input: Guide node. The start and end time boundaries to generate the new
             timestamps are defined by the range of timestamps in `input`.
         interval: Tick interval.
         align: If false, the first tick is generated at the first timestamp
             (similar to [`tp.begin()`][temporian.begin]). If true (default),
             ticks are generated on timestamps that are multiple of `interval`.
 
-    Example #1:
-        Input
-            events: [1, 5.5, 5.6, 8.6]
-        Argument
-            interval: 4
-            align: false
-        Output
-            timestamp: 1, 5
-
-    Example #2:
-        Input
-            events: [1, 5.5, 5.6, 8.6]
-        Argument
-            interval: 4
-            align: true
-        Output
-            timestamp: 4, 8
-
     Returns:
         A feature-less node with regular timestamps.
     """
 
     return Tick(
         input=input, interval=normalize_duration(interval), align=align
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/unary/__init__.py` & `temporian-0.1.2/temporian/implementation/numpy_cc/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""Unary operators."""
```

### Comparing `temporian-0.1.1/temporian/core/operators/unary/api_symbols.py` & `temporian-0.1.2/temporian/core/operators/window/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Window operators."""
+
 # pylint: disable=unused-import
+# pylint: disable=line-too-long
+# fmt: off
 
-from temporian.core.operators.unary.unary import abs
-from temporian.core.operators.unary.unary import log
-from temporian.core.operators.unary.unary import invert
-from temporian.core.operators.unary.unary import isnan
-from temporian.core.operators.unary.unary import notnan
+from temporian.core.operators.window.simple_moving_average import simple_moving_average
+from temporian.core.operators.window.moving_standard_deviation import moving_standard_deviation
+from temporian.core.operators.window.moving_sum import cumsum
+from temporian.core.operators.window.moving_sum import moving_sum
+from temporian.core.operators.window.moving_count import moving_count
+from temporian.core.operators.window.moving_min import moving_min
+from temporian.core.operators.window.moving_max import moving_max
```

### Comparing `temporian-0.1.1/temporian/core/operators/unary/unary.py` & `temporian-0.1.2/temporian/core/operators/unary.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,33 +14,36 @@
 
 """Unary operators (e.g: ~, isnan, abs) and public API definitions."""
 
 from abc import abstractmethod
 from typing import List
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.operators.base import Operator
 from temporian.proto import core_pb2 as pb
 
 
 class BaseUnaryOperator(Operator):
     def __init__(
         self,
-        input: Node,
+        input: EventSetNode,
     ):
         super().__init__()
 
         # Check input
-        if not isinstance(input, Node):
-            raise TypeError(f"Input must be of type Node but got {type(input)}")
+        if not isinstance(input, EventSetNode):
+            raise TypeError(
+                f"Input must be of type EventSetNode but got {type(input)}"
+            )
 
         for feature in input.schema.features:
             if feature.dtype not in self.allowed_dtypes():
                 raise ValueError(
                     "DTypes supported by the operator:"
                     f" {self.allowed_dtypes()}. Got feature {feature.name} with"
                     f" dtype {feature.dtype}."
@@ -181,97 +184,209 @@
 operator_lib.register_operator(InvertOperator)
 operator_lib.register_operator(IsNanOperator)
 operator_lib.register_operator(NotNanOperator)
 operator_lib.register_operator(AbsOperator)
 operator_lib.register_operator(LogOperator)
 
 
+@compile
 def invert(
-    input: Node,
-) -> Node:
+    input: EventSetNode,
+) -> EventSetNode:
     """Inverts a boolean node (~node).
 
     Swaps False<->True element-wise.
     Does not work on integers, they should be cast to BOOLEAN beforehand.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2],
+        ...     features={"M": [1, 5], "N": [1.0, 5.5]},
+        ... )
+        >>> # Boolean node
+        >>> b = a < 2
+        >>> b
+        indexes: ...
+                'M': [ True False]
+                'N': [ True False]
+        ...
+
+        >>> # Inverted node
+        >>> c = ~b
+        >>> c
+        indexes: ...
+                'M': [False True]
+                'N': [False True]
+        ...
+
+        ```
+
     Args:
-        input: Node to invert.
+        input: EventSetNode to invert.
 
     Returns:
         Negated node.
     """
     return InvertOperator(
         input=input,
     ).outputs["output"]
 
 
+@compile
 def isnan(
-    input: Node,
-) -> Node:
+    input: EventSetNode,
+) -> EventSetNode:
     """Returns boolean features, `True` in the NaN elements of the input.
 
     Note that for `int` and `bool` this will
     always be `False` since those types don't support NaNs.
     It only makes actual sense to use on `float` (or `tp.float32`) features.
 
+    See also [`tp.notnan()`][temporian.notnan].
+
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2, 3],
+        ...     features={"M":[np.nan, 5., np.nan], "N":  [-1, 0, 5]},
+        ... )
+        >>> b = tp.isnan(a)
+        >>> b
+        indexes: ...
+                'M': [ True False True]
+                'N': [False False False]
+        ...
+
+        >>> # Count nans
+        >>> tp.cumsum(tp.cast(b["M"], int))
+        indexes: ...
+                timestamps: [1. 2. 3.]
+                'M': [1 1 2]
+        ...
+
+        ```
+
     Args:
-        input: Node to check for NaNs.
+        input: EventSetNode to check for NaNs.
 
     Returns:
-        Node with `bool` features.
+        EventSetNode with `bool` features.
     """
     return IsNanOperator(
         input=input,
     ).outputs["output"]
 
 
+@compile
 def notnan(
-    input: Node,
-) -> Node:
+    input: EventSetNode,
+) -> EventSetNode:
     """Opposite of `isnan()`, being `True` in the elements that are not NaN.
 
     Equivalent to `invert(isnan())`. Note that for `int` and `bool` this will
     always be `True` since those types don't support NaNs.
     It only makes actual sense to use on `float` (or `tp.float32`) features.
 
+
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2, 3],
+        ...     features={"M":[np.nan, 5., np.nan], "N":  [-1, 0, 5]},
+        ... )
+        >>> b = tp.isnan(a)
+        >>> b
+        indexes: ...
+                'M': [ True False True]
+                'N': [False False False]
+        ...
+
+        >>> # Filter only not nan rows
+        >>> not_nans = ~b["M"]
+        >>> not_nans
+        indexes: ...
+                'M': [False True False]
+        ...
+
+        >>> tp.filter(a, not_nans)
+        indexes: ...
+                'M': [5.]
+                'N': [0]
+        ...
+
+        ```
+
     Args:
-        input: Node to check for NaNs.
+        input: EventSetNode to check for NaNs.
 
     Returns:
-        Node with `bool` features.
+        EventSetNode with `bool` features.
     """
     return NotNanOperator(
         input=input,
     ).outputs["output"]
 
 
+@compile
 def abs(
-    input: Node,
-) -> Node:
+    input: EventSetNode,
+) -> EventSetNode:
     """Gets the absolute value of the input features.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2, 3],
+        ...     features={"M":[np.nan, -1., 2.], "N":  [-1, -3, 5]},
+        ... )
+        >>> b = tp.abs(a)
+        >>> b
+        indexes: ...
+                'M': [nan 1. 2.]
+                'N': [1 3 5]
+        ...
+
+        ```
+
     Args:
-        input: Node calculate absolute value.
+        input: EventSetNode calculate absolute value.
 
     Returns:
-        Node with positive valued features.
+        EventSetNode with positive valued features.
     """
     return AbsOperator(
         input=input,
     ).outputs["output"]
 
 
+@compile
 def log(
-    input: Node,
-) -> Node:
+    input: EventSetNode,
+) -> EventSetNode:
     """Calculates the natural logarithm of the features. Can only be used
     on floating point feature types.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[1, 2, 3, 4, 5],
+        ...     features={"M": [np.e, 1., 2., 10., -1.]},
+        ... )
+        >>> b = tp.log(a)
+        >>> b
+        indexes: ...
+                timestamps: [1. 2. 3. 4. 5.]
+                'M': [1. 0. 0.6931 2.3026 nan]
+        ...
+
+        ```
+
     Args:
-        input: Node to calculate natural logarithm.
+        input: EventSetNode to calculate natural logarithm.
 
     Returns:
-        Node with logarithm of input features.
+        EventSetNode with logarithm of input features.
     """
     return LogOperator(
         input=input,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/unique_timestamps.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/end_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,70 +9,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Unique timestamps operator class and public API function definitions."""
+from absl.testing import absltest
 
-from temporian.core import operator_lib
-from temporian.core.data.node import Node, create_node_new_features_new_sampling
-from temporian.core.operators.base import Operator
-from temporian.proto import core_pb2 as pb
-
-
-class UniqueTimestamps(Operator):
-    def __init__(self, input: Node):
-        super().__init__()
-
-        self.add_input("input", input)
-
-        self.add_output(
-            "output",
-            create_node_new_features_new_sampling(
-                features=[],
-                indexes=input.schema.indexes,
-                is_unix_timestamp=input.schema.is_unix_timestamp,
-                creator=self,
-            ),
+from temporian.core.operators.end import EndOperator
+from temporian.implementation.numpy.data.io import event_set
+from temporian.implementation.numpy.operators.end import (
+    EndNumpyImplementation,
+)
+
+
+class EndOperatorTest(absltest.TestCase):
+    def setUp(self):
+        pass
+
+    def test_base(self):
+        evset = event_set(
+            timestamps=[1, 2, 3, 4],
+            features={
+                "a": [5, 6, 7, 8],
+                "b": ["A", "A", "B", "B"],
+            },
+            indexes=["b"],
         )
-        self.check()
+        node = evset.node()
 
-    @classmethod
-    def build_op_definition(cls) -> pb.OperatorDef:
-        return pb.OperatorDef(
-            key="UNIQUE_TIMESTAMPS",
-            attributes=[],
-            inputs=[pb.OperatorDef.Input(key="input")],
-            outputs=[pb.OperatorDef.Output(key="output")],
+        expected_output = event_set(
+            timestamps=[2, 4],
+            features={"b": ["A", "B"]},
+            indexes=["b"],
         )
 
+        # Run op
+        op = EndOperator(input=node)
+        instance = EndNumpyImplementation(op)
+        output = instance.call(input=evset)["output"]
 
-operator_lib.register_operator(UniqueTimestamps)
+        self.assertEqual(output, expected_output)
 
 
-def unique_timestamps(input: Node) -> Node:
-    """Removes duplicated timestamps.
-
-    Returns a feature-less node where each timestamps from `input` only appears
-    once. If the input is indexed, the unique operation is applied independently
-    for each index.
-
-    Example:
-
-        Inputs:
-            input:
-                feature_1: ['a', 'b', 'c', 'd']
-                timestamps: [1, 2, 2, 4]
-
-        Output:
-            timestamps: [1, 2, 4]
-
-    Args:
-        input: Node, possibly with features, to process.
-
-    Returns:
-        Node without features with unique timestamps in `input`.
-    """
-
-    return UniqueTimestamps(input=input).outputs["output"]
+if __name__ == "__main__":
+    absltest.main()
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/BUILD`

 * *Files 16% similar despite different names*

```diff
@@ -6,124 +6,92 @@
 # Libraries
 # =========
 
 py_library(
     name = "window",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
-    deps = [
-        ":api_symbols",
-    ],
-)
-
-py_library(
-    name = "api_symbols",
-    srcs = ["api_symbols.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":moving_count",
-        ":moving_max",
-        ":moving_min",
-        ":moving_standard_deviation",
-        ":moving_sum",
-        ":simple_moving_average",
-    ],
 )
 
 py_library(
     name = "base",
     srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/core/operators:base",
-        "//temporian/proto:core_py_proto",
+        # already_there/numpy
+        "//temporian/core/operators/window:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy/operators:base",
     ],
 )
 
 py_library(
     name = "simple_moving_average",
     srcs = ["simple_moving_average.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/operators/window:simple_moving_average",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
     name = "moving_standard_deviation",
     srcs = ["moving_standard_deviation.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/operators/window:moving_standard_deviation",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
     name = "moving_sum",
     srcs = ["moving_sum.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        # already_there/numpy
-        "//temporian/core:operator_lib",
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
+        "//temporian/core/operators/window:moving_sum",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
     name = "moving_count",
     srcs = ["moving_count.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/operators/window:moving_count",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "moving_min",
-    srcs = ["moving_min.py"],
+    name = "moving_max",
+    srcs = ["moving_max.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/operators/window:moving_max",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "moving_max",
-    srcs = ["moving_max.py"],
+    name = "moving_min",
+    srcs = ["moving_min.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:duration_utils",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/operators/window:moving_min",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/api_symbols.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_max.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,18 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint: disable=unused-import
-# pylint: disable=line-too-long
-# fmt: off
-
-from temporian.core.operators.window.simple_moving_average import simple_moving_average
-from temporian.core.operators.window.moving_standard_deviation import moving_standard_deviation
-from temporian.core.operators.window.moving_sum import cumsum
-from temporian.core.operators.window.moving_sum import moving_sum
-from temporian.core.operators.window.moving_count import moving_count
-from temporian.core.operators.window.moving_min import moving_min
-from temporian.core.operators.window.moving_max import moving_max
+
+from temporian.core.operators.window.moving_max import (
+    MovingMaxOperator,
+)
+from temporian.implementation.numpy import implementation_lib
+from temporian.implementation.numpy.operators.window.base import (
+    BaseWindowNumpyImplementation,
+)
+from temporian.implementation.numpy_cc.operators import operators_cc
+
+
+class MovingMaxNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the moving max operator."""
+
+    def _implementation(self):
+        return operators_cc.moving_max
+
+
+implementation_lib.register_operator_implementation(
+    MovingMaxOperator, MovingMaxNumpyImplementation
+)
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/base.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,104 +8,100 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Base calendar operator class definition."""
+from abc import abstractmethod
+from typing import Dict, Optional, List, Any
 
-from abc import ABC, abstractmethod
-from typing import Optional
+import numpy as np
 
+from temporian.core.operators.window.base import BaseWindowOperator
+from temporian.implementation.numpy.data.event_set import IndexData
+from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.implementation.numpy.operators.base import OperatorImplementation
 
-from temporian.core.data.duration_utils import NormalizedDuration
-from temporian.core.data.dtypes.dtype import DType
-from temporian.core.data.node import (
-    Node,
-    create_node_new_features_existing_sampling,
-)
-from temporian.core.data.schema import FeatureSchema
-from temporian.core.operators.base import Operator
-from temporian.proto import core_pb2 as pb
 
+class BaseWindowNumpyImplementation(OperatorImplementation):
+    """Interface definition and common logic for numpy implementation of
+    window operators."""
 
-class BaseWindowOperator(Operator, ABC):
-    """Interface definition and common logic for window operators."""
+    def __init__(self, operator: BaseWindowOperator) -> None:
+        super().__init__(operator)
+        assert isinstance(operator, BaseWindowOperator)
 
-    def __init__(
+    def __call__(
         self,
-        input: Node,
-        window_length: NormalizedDuration,
-        sampling: Optional[Node] = None,
-    ):
-        super().__init__()
-
-        self._window_length = window_length
-        self.add_attribute("window_length", window_length)
-
-        self._has_sampling = sampling is not None
-        if self._has_sampling:
-            assert sampling is not None
-
-            self.add_input("sampling", sampling)
-            effective_sampling_node = sampling
-
-            input.schema.check_compatible_index(sampling.schema)
-
-        else:
-            effective_sampling_node = input
-
-        self.add_input("input", input)
-
-        feature_schemas = [  # pylint: disable=g-complex-comprehension
-            FeatureSchema(
-                name=f.name,
-                dtype=self.get_feature_dtype(f),
+        input: EventSet,
+        sampling: Optional[EventSet] = None,
+    ) -> Dict[str, EventSet]:
+        assert isinstance(self.operator, BaseWindowOperator)
+
+        # if no sampling is provided, apply operator to the evset's own
+        # timestamps
+        if sampling is None:
+            sampling = input
+
+        # create destination evset
+        output_schema = self.operator.outputs["output"].schema
+        dst_evset = EventSet(data={}, schema=output_schema)
+        # For each index
+        for index_key, index_data in input.data.items():
+            dst_features = []
+            dst_timestamps = sampling.data[index_key].timestamps
+            dst_index_data = IndexData(
+                features=dst_features,
+                timestamps=dst_timestamps,
+                schema=None,
+            )
+            self._compute(
+                src_timestamps=index_data.timestamps,
+                src_features=index_data.features,
+                sampling_timestamps=dst_timestamps,
+                dst_features=dst_features,
+            )
+            dst_index_data.check_schema(output_schema)
+            dst_evset.set_index_value(
+                index_key, dst_index_data, normalize=False
             )
-            for f in input.schema.features
-        ]
 
-        self.add_output(
-            "output",
-            create_node_new_features_existing_sampling(
-                features=feature_schemas,
-                sampling_node=effective_sampling_node,
-                creator=self,
-            ),
-        )
-
-        self.check()
-
-    @property
-    def window_length(self) -> NormalizedDuration:
-        return self._window_length
-
-    @property
-    def has_sampling(self) -> bool:
-        return self._has_sampling
-
-    @classmethod
-    def build_op_definition(cls) -> pb.OperatorDef:
-        return pb.OperatorDef(
-            key=cls.operator_def_key(),
-            attributes=[
-                pb.OperatorDef.Attribute(
-                    key="window_length",
-                    type=pb.OperatorDef.Attribute.Type.FLOAT_64,
-                ),
-            ],
-            inputs=[
-                pb.OperatorDef.Input(key="input"),
-                pb.OperatorDef.Input(key="sampling", is_optional=True),
-            ],
-            outputs=[pb.OperatorDef.Output(key="output")],
-        )
+        return {"output": dst_evset}
 
-    @classmethod
     @abstractmethod
-    def operator_def_key(cls) -> str:
-        """Gets the key of the operator definition."""
+    def _implementation(self) -> Any:
+        pass
 
-    @abstractmethod
-    def get_feature_dtype(self, feature: FeatureSchema) -> DType:
-        """Gets the dtype of the output feature."""
+    def _compute(
+        self,
+        src_timestamps: np.ndarray,
+        src_features: List[np.ndarray],
+        sampling_timestamps: np.ndarray,
+        dst_features: List[np.ndarray],
+    ) -> None:
+        assert isinstance(self.operator, BaseWindowOperator)
+
+        implementation = self._implementation()
+        for src_ts in src_features:
+            kwargs = {
+                "evset_timestamps": src_timestamps,
+                "evset_values": src_ts,
+                "window_length": self.operator.window_length,
+            }
+            if self.operator.has_sampling:
+                kwargs["sampling_timestamps"] = sampling_timestamps
+            dst_feature = implementation(**kwargs)
+            dst_features.append(dst_feature)
+
+    def apply_feature_wise(
+        self,
+        src_timestamps: np.ndarray,
+        src_feature: np.ndarray,
+    ) -> np.ndarray:
+        implementation = self._implementation()
+        kwargs = {
+            "evset_timestamps": src_timestamps,
+            "evset_values": src_feature,
+            "window_length": self.operator.window_length,
+        }
+        return implementation(**kwargs)
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/moving_count.py` & `temporian-0.1.2/temporian/core/operators/window/moving_max.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,57 +13,79 @@
 # limitations under the License.
 
 """Moving count operator class and public API function definition."""
 
 from typing import Optional
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
 from temporian.core.data.duration_utils import Duration, normalize_duration
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.window.base import BaseWindowOperator
 
 
-class MovingCountOperator(BaseWindowOperator):
+class MovingMaxOperator(BaseWindowOperator):
     @classmethod
     def operator_def_key(cls) -> str:
-        return "MOVING_COUNT"
+        return "MOVING_MAX"
 
     def get_feature_dtype(self, feature: FeatureSchema) -> DType:
-        return DType.INT32
+        return feature.dtype
 
 
-operator_lib.register_operator(MovingCountOperator)
+operator_lib.register_operator(MovingMaxOperator)
 
 
-def moving_count(
-    input: Node,
+@compile
+def moving_max(
+    input: EventSetNode,
     window_length: Duration,
-    sampling: Optional[Node] = None,
-) -> Node:
-    """Computes the number of values in a sliding window over the node.
-
-    For each t in sampling, and for each feature independently, returns at time
-    t the number of non-nan values for the feature in the window
-    [t - window_length, t].
+    sampling: Optional[EventSetNode] = None,
+) -> EventSetNode:
+    """Computes the maximum in a sliding window over the node.
+
+    For each t in sampling, and for each index and feature independently,
+    returns at time t the max of non-nan values for the feature in the window
+    (t - window_length, t].
 
     If `sampling` is provided samples the moving window's value at each
     timestamp in `sampling`, else samples it at each timestamp in `input`.
 
     If the window does not contain any values (e.g., all the values are missing,
     or the window does not contain any sampling), outputs missing values.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 2, 5, 6, 7],
+        ...     features={"value": [np.nan, 1, 5, 1, 15, 20]},
+        ... )
+
+        >>> b = tp.moving_max(a, tp.duration.seconds(4))
+        >>> b
+        indexes: ...
+            (6 events):
+                timestamps: [0. 1. 2. 5. 6. 7.]
+                'value': [nan 1. 5. 5. 15. 20.]
+        ...
+
+        ```
+
+    See [`tp.moving_count()`](../moving_count) for examples with external
+    sampling and indices.
+
     Args:
-        input: Node for which to count the number of values in each feature.
+        input: EventSetNode for which to count the number of values in each feature.
         window_length: Sliding window's length.
         sampling: Timestamps to sample the sliding window's value at. If not
             provided, timestamps in `input` are used.
 
     Returns:
-        Node containing the non-nan count of each feature in `input`.
+        EventSetNode containing the max of each feature in `input`.
     """
-    return MovingCountOperator(
+    return MovingMaxOperator(
         input=input,
         window_length=normalize_duration(window_length),
         sampling=sampling,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/moving_max.py` & `temporian-0.1.2/temporian/core/operators/window/simple_moving_average.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,62 +8,91 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Moving count operator class and public API function definition."""
+"""Simple moving average operator class and public API function definition.."""
 
 from typing import Optional
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
 from temporian.core.data.duration_utils import Duration, normalize_duration
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.window.base import BaseWindowOperator
 
 
-class MovingMaxOperator(BaseWindowOperator):
+class SimpleMovingAverageOperator(BaseWindowOperator):
+    """
+    Window operator to compute the simple moving average.
+    """
+
     @classmethod
     def operator_def_key(cls) -> str:
-        return "MOVING_MAX"
+        return "SIMPLE_MOVING_AVERAGE"
 
     def get_feature_dtype(self, feature: FeatureSchema) -> DType:
-        return feature.dtype
+        return (
+            DType.FLOAT32 if feature.dtype == DType.FLOAT32 else DType.FLOAT64
+        )
 
 
-operator_lib.register_operator(MovingMaxOperator)
+operator_lib.register_operator(SimpleMovingAverageOperator)
 
 
-def moving_max(
-    input: Node,
+@compile
+def simple_moving_average(
+    input: EventSetNode,
     window_length: Duration,
-    sampling: Optional[Node] = None,
-) -> Node:
-    """Computes the maximum in a sliding window over the node.
+    sampling: Optional[EventSetNode] = None,
+) -> EventSetNode:
+    """Computes the average of values in a sliding window over the node.
 
     For each t in sampling, and for each feature independently, returns at time
-    t the max of non-nan values for the feature in the window
-    [t - window_length, t].
+    t the average value of the feature in the window (t - window_length, t].
 
     If `sampling` is provided samples the moving window's value at each
     timestamp in `sampling`, else samples it at each timestamp in `input`.
 
+    Missing values (such as NaNs) are ignored.
+
     If the window does not contain any values (e.g., all the values are missing,
     or the window does not contain any sampling), outputs missing values.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 2, 5, 6, 7],
+        ...     features={"value": [np.nan, 1, 5, 10, 15, 20]},
+        ... )
+
+        >>> b = tp.simple_moving_average(a, tp.duration.seconds(4))
+        >>> b
+        indexes: ...
+            (6 events):
+                timestamps: [0. 1. 2. 5. 6. 7.]
+                'value': [ nan 1.  3. 7.5  12.5  15. ]
+        ...
+
+        ```
+
+    See [`tp.moving_count()`](../moving_count) for examples of moving window
+    operations with external sampling and indices.
+
     Args:
-        input: Node for which to count the number of values in each feature.
+        input: Features to average.
         window_length: Sliding window's length.
         sampling: Timestamps to sample the sliding window's value at. If not
             provided, timestamps in `input` are used.
 
     Returns:
-        Node containing the max of each feature in `input`.
+        EventSetNode containing the moving average of each feature in `input`.
     """
-    return MovingMaxOperator(
+    return SimpleMovingAverageOperator(
         input=input,
         window_length=normalize_duration(window_length),
         sampling=sampling,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/moving_min.py` & `temporian-0.1.2/temporian/core/operators/window/moving_min.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # limitations under the License.
 
 """Moving count operator class and public API function definition."""
 
 from typing import Optional
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
 from temporian.core.data.duration_utils import Duration, normalize_duration
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.window.base import BaseWindowOperator
 
 
 class MovingMinOperator(BaseWindowOperator):
     @classmethod
     def operator_def_key(cls) -> str:
@@ -32,38 +33,59 @@
     def get_feature_dtype(self, feature: FeatureSchema) -> DType:
         return feature.dtype
 
 
 operator_lib.register_operator(MovingMinOperator)
 
 
+@compile
 def moving_min(
-    input: Node,
+    input: EventSetNode,
     window_length: Duration,
-    sampling: Optional[Node] = None,
-) -> Node:
+    sampling: Optional[EventSetNode] = None,
+) -> EventSetNode:
     """Computes the minimum of values in a sliding window over the node.
 
-    For each t in sampling, and for each feature independently, returns at time
-    t the minimum of non-nan values for the feature in the window
-    [t - window_length, t].
+    For each t in sampling, and for each index and feature independently,
+    returns at time t the minimum of non-nan values for the feature in the window
+    (t - window_length, t].
 
     If `sampling` is provided samples the moving window's value at each
     timestamp in `sampling`, else samples it at each timestamp in `input`.
 
     If the window does not contain any values (e.g., all the values are missing,
     or the window does not contain any sampling), outputs missing values.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 2, 5, 6, 7],
+        ...     features={"value": [np.nan, 1, 5, 10, 15, 20]},
+        ... )
+
+        >>> b = tp.moving_min(a, tp.duration.seconds(4))
+        >>> b
+        indexes: ...
+            (6 events):
+                timestamps: [0. 1. 2. 5. 6. 7.]
+                'value': [nan 1. 1. 5. 10. 10.]
+        ...
+
+        ```
+
+    See [`tp.moving_count()`](../moving_count) for examples of moving window
+    operations with external sampling and indices.
+
     Args:
-        input: Node for which to count the number of values in each feature.
+        input: EventSetNode for which to count the number of values in each feature.
         window_length: Sliding window's length.
         sampling: Timestamps to sample the sliding window's value at. If not
             provided, timestamps in `input` are used.
 
     Returns:
-        Node containing the minimum of each feature in `input`.
+        EventSetNode containing the minimum of each feature in `input`.
     """
     return MovingMinOperator(
         input=input,
         window_length=normalize_duration(window_length),
         sampling=sampling,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/moving_standard_deviation.py` & `temporian-0.1.2/temporian/core/operators/window/moving_standard_deviation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Moving standard deviation operator class and public API function definition."""
 from typing import Optional
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
 from temporian.core.data.duration_utils import Duration, normalize_duration
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.core.data.schema import FeatureSchema
 from temporian.core.operators.window.base import BaseWindowOperator
 
 
 class MovingStandardDeviationOperator(BaseWindowOperator):
     @classmethod
     def operator_def_key(cls) -> str:
@@ -33,42 +34,63 @@
             DType.FLOAT32 if feature.dtype == DType.FLOAT32 else DType.FLOAT64
         )
 
 
 operator_lib.register_operator(MovingStandardDeviationOperator)
 
 
+@compile
 def moving_standard_deviation(
-    input: Node,
+    input: EventSetNode,
     window_length: Duration,
-    sampling: Optional[Node] = None,
-) -> Node:
+    sampling: Optional[EventSetNode] = None,
+) -> EventSetNode:
     """Computes the standard deviation of values in a sliding window over the
     node.
 
     For each t in sampling, and for each feature independently, returns at time
     t the standard deviation for the feature in the window
-    [t - window_length, t].
+    (t - window_length, t].
 
     If `sampling` is provided samples the moving window's value at each
     timestamp in `sampling`, else samples it at each timestamp in `input`.
 
     Missing values (such as NaNs) are ignored.
 
     If the window does not contain any values (e.g., all the values are missing,
     or the window does not contain any sampling), outputs missing values.
 
+    Example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 2, 5, 6, 7],
+        ...     features={"value": [np.nan, 1, 5, 10, 15, 20]},
+        ... )
+
+        >>> b = tp.moving_standard_deviation(a, tp.duration.seconds(4))
+        >>> b
+        indexes: ...
+            (6 events):
+                timestamps: [0. 1. 2. 5. 6. 7.]
+                'value': [ nan 0.  2.  2.5  2.5  4.0825]
+        ...
+
+        ```
+
+    See [`tp.moving_count()`](../moving_count) for examples of moving window
+    operations with external sampling and indices.
+
     Args:
         input: Features to compute the standard deviation for.
         window_length: Sliding window's length.
         sampling: Timestamps to sample the sliding window's value at. If not
             provided, timestamps in `input` are used.
 
     Returns:
-        Node containing the moving standard deviation of each feature in
+        EventSetNode containing the moving standard deviation of each feature in
         `input`.
     """
     return MovingStandardDeviationOperator(
         input=input,
         window_length=normalize_duration(window_length),
         sampling=sampling,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/moving_sum.py` & `temporian-0.1.2/temporian/core/operators/calendar/day_of_month.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,90 +8,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Moving Sum operator class and public API function definition.."""
-
-from typing import Optional
-
-import numpy as np
+"""Calendar day of month operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.duration_utils import Duration, normalize_duration
-from temporian.core.data.node import Node
-from temporian.core.data.schema import FeatureSchema
-from temporian.core.operators.window.base import BaseWindowOperator
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.compilation import compile
+from temporian.core.data.node import EventSetNode
+from temporian.core.operators.calendar.base import BaseCalendarOperator
 
 
-class MovingSumOperator(BaseWindowOperator):
+class CalendarDayOfMonthOperator(BaseCalendarOperator):
     @classmethod
     def operator_def_key(cls) -> str:
-        return "MOVING_SUM"
-
-    def get_feature_dtype(self, feature: FeatureSchema) -> DType:
-        return feature.dtype
-
-
-operator_lib.register_operator(MovingSumOperator)
-
-
-def moving_sum(
-    input: Node,
-    window_length: Duration,
-    sampling: Optional[Node] = None,
-) -> Node:
-    """Computes the sum of values in a sliding window over the node.
-
-    For each t in sampling, and for each feature independently, returns at time
-    t the sum of the feature in the window [t - window_length, t].
+        return "CALENDAR_DAY_OF_MONTH"
 
-    If `sampling` is provided samples the moving window's value at each
-    timestamp in `sampling`, else samples it at each timestamp in `input`.
-
-    Missing values (such as NaNs) are ignored.
-
-    If the window does not contain any values (e.g., all the values are missing,
-    or the window does not contain any sampling), outputs missing values.
-
-    Args:
-        input: Features to sum.
-        window_length: Sliding window's length.
-        sampling: Timestamps to sample the sliding window's value at. If not
-            provided, timestamps in `input` are used.
-
-    Returns:
-        Node containing the moving sum of each feature in `input`.
-    """
-    return MovingSumOperator(
-        input=input,
-        window_length=normalize_duration(window_length),
-        sampling=sampling,
-    ).outputs["output"]
+    @classmethod
+    def output_feature_name(cls) -> str:
+        return "calendar_day_of_month"
 
 
-def cumsum(
-    input: Node,
-) -> Node:
-    """Cumulative Sum.
+operator_lib.register_operator(CalendarDayOfMonthOperator)
 
-    Foreach timestamp, calculate the sum of the feature from the beginning.
-    It's a shorthand for `moving_sum(event, window_length=np.inf)`.
 
-    Missing values are ignored.
+@compile
+def calendar_day_of_month(sampling: EventSetNode) -> EventSetNode:
+    """Obtains the day of month the timestamps in a node's sampling are in.
+
+    Features in the input node are ignored, only the timestamps are used and
+    they must be unix timestamps (`is_unix_timestamp=True`).
+
+    Output feature contains numbers between 1 and 31.
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...    timestamps=["2023-02-04", "2023-02-20", "2023-03-01", "2023-05-07"],
+        ... )
+        >>> b = tp.calendar_day_of_month(a)
+        >>> b
+        indexes: ...
+        features: [('calendar_day_of_month', int32)]
+        events:
+            (4 events):
+                timestamps: [...]
+                'calendar_day_of_month': [ 4 20  1  7]
+        ...
 
-    While the feature does not have any values (e.g., missing initial values),
-    outputs missing values.
+        ```
 
     Args:
-        input: The node with features to accumulate.
+        sampling: EventSetNode to get the days of month from.
 
     Returns:
-        A node containing the cumulative sum of each feature in `node`.
+        Single feature with the day each timestamp in `sampling` belongs to.
     """
-    return MovingSumOperator(
-        input=input,
-        window_length=normalize_duration(np.inf),
-    ).outputs["output"]
+    return CalendarDayOfMonthOperator(sampling).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/operators/window/simple_moving_average.py` & `temporian-0.1.2/temporian/core/operators/lag.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,69 +8,108 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Simple moving average operator class and public API function definition.."""
-
-from typing import Optional
+"""Lag operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.data.dtypes.dtype import DType
-from temporian.core.data.duration_utils import Duration, normalize_duration
-from temporian.core.data.node import Node
-from temporian.core.data.schema import FeatureSchema
-from temporian.core.operators.window.base import BaseWindowOperator
-
+from temporian.core.compilation import compile
+from temporian.core.data.duration_utils import (
+    Duration,
+    NormalizedDuration,
+    normalize_duration,
+)
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
+from temporian.core.operators.base import Operator
+from temporian.proto import core_pb2 as pb
+
+
+class LagOperator(Operator):
+    def __init__(
+        self,
+        input: EventSetNode,
+        duration: NormalizedDuration,
+    ):
+        super().__init__()
+
+        self._duration = duration
+
+        self.add_input("input", input)
+        self.add_attribute("duration", duration)
+
+        self.add_output(
+            "output",
+            create_node_new_features_new_sampling(
+                features=input.schema.features,
+                indexes=input.schema.indexes,
+                is_unix_timestamp=input.schema.is_unix_timestamp,
+                creator=self,
+            ),
+        )
+        self.check()
 
-class SimpleMovingAverageOperator(BaseWindowOperator):
-    """
-    Window operator to compute the simple moving average.
-    """
+    @property
+    def duration(self) -> Duration:
+        return self._duration
 
     @classmethod
-    def operator_def_key(cls) -> str:
-        return "SIMPLE_MOVING_AVERAGE"
-
-    def get_feature_dtype(self, feature: FeatureSchema) -> DType:
-        return (
-            DType.FLOAT32 if feature.dtype == DType.FLOAT32 else DType.FLOAT64
+    def build_op_definition(cls) -> pb.OperatorDef:
+        return pb.OperatorDef(
+            key="LAG",
+            attributes=[
+                pb.OperatorDef.Attribute(
+                    key="duration",
+                    type=pb.OperatorDef.Attribute.Type.FLOAT_64,
+                    is_optional=False,
+                ),
+            ],
+            inputs=[pb.OperatorDef.Input(key="input")],
+            outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
-operator_lib.register_operator(SimpleMovingAverageOperator)
+operator_lib.register_operator(LagOperator)
 
 
-def simple_moving_average(
-    input: Node,
-    window_length: Duration,
-    sampling: Optional[Node] = None,
-) -> Node:
-    """Computes the average of values in a sliding window over the node.
+@compile
+def lag(input: EventSetNode, duration: Duration) -> EventSetNode:
+    """Adds a delay to an EventSetNode's timestamps.
+
+    In other words, shifts the timestamp values forwards in time.
+
+    Usage example:
+        ```python
+        >>> a = tp.event_set(
+        ...     timestamps=[0, 1, 5, 6],
+        ...     features={"value": [0, 1, 5, 6]},
+        ... )
+
+        >>> b = tp.lag(a, tp.duration.seconds(2))
+        >>> b
+        indexes: ...
+            (4 events):
+                timestamps: [2. 3. 7. 8.]
+                'value': [0 1 5 6]
+        ...
 
-    For each t in sampling, and for each feature independently, returns at time
-    t the average value of the feature in the window [t - window_length, t].
-
-    If `sampling` is provided samples the moving window's value at each
-    timestamp in `sampling`, else samples it at each timestamp in `input`.
-
-    Missing values (such as NaNs) are ignored.
-
-    If the window does not contain any values (e.g., all the values are missing,
-    or the window does not contain any sampling), outputs missing values.
+        ```
 
     Args:
-        input: Features to average.
-        window_length: Sliding window's length.
-        sampling: Timestamps to sample the sliding window's value at. If not
-            provided, timestamps in `input` are used.
+        input: node to lag.
+        duration: Duration to lag by.
 
     Returns:
-        Node containing the moving average of each feature in `input`.
+        Lagged node.
     """
-    return SimpleMovingAverageOperator(
+
+    normalized_duration = normalize_duration(duration)
+
+    return LagOperator(
         input=input,
-        window_length=normalize_duration(window_length),
-        sampling=sampling,
+        duration=normalized_duration,
     ).outputs["output"]
```

### Comparing `temporian-0.1.1/temporian/core/schedule.py` & `temporian-0.1.2/temporian/core/schedule.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass, field
 from typing import List, Set
 
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.core.operators.base import Operator
 
 
 @dataclass
+class ScheduleStep:
+    op: Operator
+
+    # List of nodes that will not be used anymore after "op" is executed.
+    released_nodes: List[EventSetNode]
+
+
+@dataclass
 class Schedule:
-    ordered_operators: List[Operator] = field(default_factory=list)
-    input_nodes: Set[Node] = field(default_factory=set)
+    steps: List[ScheduleStep] = field(default_factory=list)
+    input_nodes: Set[EventSetNode] = field(default_factory=set)
```

### Comparing `temporian-0.1.1/temporian/core/serialization/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/operators/scalar/BUILD`

 * *Files 22% similar despite different names*

```diff
@@ -3,39 +3,54 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "serialization",
+    name = "scalar",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
     deps = [
-        ":api_symbols",
+        ":arithmetic_scalar",
+        ":relational_scalar",
     ],
 )
 
 py_library(
-    name = "api_symbols",
-    srcs = ["api_symbols.py"],
+    name = "base",
+    srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        ":serialize",
+        # already_there/numpy
+        "//temporian/core/data:dtype",
+        "//temporian/core/operators/scalar:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy/operators:base",
     ],
 )
 
 py_library(
-    name = "serialize",
-    srcs = ["serialize.py"],
+    name = "arithmetic_scalar",
+    srcs = ["arithmetic_scalar.py"],
     srcs_version = "PY3",
     deps = [
-        # already_there/google/protobuf
-        "//temporian/core:graph",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/operators:base",
-        "//temporian/proto:core_py_proto",
+        ":base",
+        # already_there/numpy
+        "//temporian/core/data:dtype",
+        "//temporian/core/operators/scalar",
+        "//temporian/implementation/numpy:implementation_lib",
+    ],
+)
+
+py_library(
+    name = "relational_scalar",
+    srcs = ["relational_scalar.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":base",
+        "//temporian/core/data:dtype",
+        # already_there/numpy
+        "//temporian/core/operators/scalar",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/serialization/api_symbols.py` & `temporian-0.1.2/temporian/beam/operators/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint: disable=unused-import
+"""Imports all the packages containing operator implementations."""
 
-from temporian.core.serialization.serialize import load
-from temporian.core.serialization.serialize import save
+# pylint: disable=unused-import
+# pylint: disable=line-too-long
+# fmt: off
+from temporian.beam.operators.window import moving_sum
+from temporian.beam.operators import select
+from temporian.beam.operators import add_index
```

### Comparing `temporian-0.1.1/temporian/core/test/BUILD` & `temporian-0.1.2/temporian/core/test/BUILD`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 py_library(
     name = "utils",
     srcs = ["utils.py"],
     srcs_version = "PY3",
     deps = [
         "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
-        "//temporian/core/data/dtypes:dtype",
         "//temporian/core/operators:base",
         "//temporian/implementation/numpy/data:event_set",
         "//temporian/implementation/numpy/data:io",
         "//temporian/proto:core_py_proto",
     ],
 )
 
@@ -22,22 +22,25 @@
 # =====
 
 py_test(
     name = "magic_methods_test",
     srcs = ["magic_methods_test.py"],
     srcs_version = "PY3",
     deps = [
+        # already_there/absl/testing:parameterized
         # already_there/absl/testing:absltest
         ":utils",
         "//temporian/core/data:node",
         "//temporian/core/operators:base",
-        "//temporian/core/operators/unary",
+        "//temporian/core/operators:unary",
         "//temporian/core/operators/binary",
         "//temporian/core/operators/scalar",
         "//temporian/proto:core_py_proto",
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_test(
     name = "operator_test",
     srcs = ["operator_test.py"],
     srcs_version = "PY3",
@@ -66,35 +69,47 @@
     srcs_version = "PY3",
     deps = [
         ":utils",
         # already_there/absl/logging
         # already_there/absl/testing:absltest
         "//temporian",
         "//temporian/core:graph",
-        "//temporian/core/serialization:serialize",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core:serialization",
+        "//temporian/core/data:dtype",
         "//temporian/implementation/numpy/data:io",
     ],
 )
 
 py_test(
     name = "evaluation_test",
     srcs = ["evaluation_test.py"],
     srcs_version = "PY3",
     deps = [
         ":utils",
         # already_there/absl/testing:absltest
         "//temporian/core:evaluation",
         "//temporian/implementation/numpy/data:event_set",
+        "//temporian",
     ],
 )
 
 py_test(
     name = "registered_operators_test",
     srcs = ["registered_operators_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         "//temporian/core:operator_lib",
-        "//temporian/core/operators:api_symbols",
+        "//temporian",
+    ],
+)
+
+py_test(
+    name = "compilation_test",
+    srcs = ["compilation_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        "//temporian/core:operator_lib",
+        "//temporian",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/core/test/graph_test.py` & `temporian-0.1.2/temporian/core/test/graph_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from temporian.core.test import utils
 
 
 class GraphTest(absltest.TestCase):
     def test_infer_graph_no_names(self):
         """Lists all the objects in a graph."""
 
-        i1 = utils.create_source_node()
+        i1 = utils.create_input_node()
         o2 = utils.OpI1O1(i1)
-        i3 = utils.create_source_node()
+        i3 = utils.create_input_node()
         o4 = utils.OpI2O1(o2.outputs["output"], i3)
         o5 = utils.OpI1O2(o4.outputs["output"])
         output_1 = o5.outputs["output_1"]
         output_2 = o4.outputs["output"]
 
         g = graph.infer_graph({i1, i3}, {output_1, output_2})
 
@@ -53,17 +53,17 @@
         g.set_output_node_names(
             {"io_output_1": output_1, "io_output_2": output_2}
         )
 
     def test_infer_graph_with_names(self):
         """Lists all the objects in a graph."""
 
-        i1 = utils.create_source_node()
+        i1 = utils.create_input_node()
         o2 = utils.OpI1O1(i1)
-        i3 = utils.create_source_node()
+        i3 = utils.create_input_node()
         o4 = utils.OpI2O1(o2.outputs["output"], i3)
         o5 = utils.OpI1O2(o4.outputs["output"])
         output_1 = o5.outputs["output_1"]
         output_2 = o4.outputs["output"]
 
         g = graph.infer_graph_named_nodes(
             {"io_input_1": i1, "io_input_2": i3},
@@ -80,17 +80,17 @@
         g.set_output_node_names(
             {"io_output_1": output_1, "io_output_2": output_2}
         )
 
     def test_infer_graph_with_node_names(self):
         """Lists all the objects in a graph."""
 
-        i1 = utils.create_source_node("io_input_1")
+        i1 = utils.create_input_node("io_input_1")
         o2 = utils.OpI1O1(i1)
-        i3 = utils.create_source_node("io_input_2")
+        i3 = utils.create_input_node("io_input_2")
         o4 = utils.OpI2O1(o2.outputs["output"], i3)
         o5 = utils.OpI1O2(o4.outputs["output"])
         output_1 = o5.outputs["output_1"]
         output_2 = o4.outputs["output"]
         output_1.name = "io_output_1"
         output_2.name = "io_output_2"
 
@@ -106,29 +106,29 @@
         g.set_output_node_names(
             {"io_output_1": output_1, "io_output_2": output_2}
         )
 
     def test_infer_graph_noop(self):
         """With an opt that just passes features."""
 
-        a = utils.create_source_node()
+        a = utils.create_input_node()
         b = utils.OpI1O1NotCreator(a)
         c = utils.OpI1O1(b.outputs["output"])
 
         g = graph.infer_graph({a}, {c.outputs["output"]})
 
         self.assertLen(g.operators, 2)
         self.assertLen(g.samplings, 2)
         self.assertLen(g.nodes, 3)
         self.assertLen(g.features, 4)
 
     def test_infer_graph_input_is_not_feature_creator(self):
         """When the user input is not the feature creator."""
 
-        a = utils.create_source_node()
+        a = utils.create_input_node()
         b = utils.OpI1O1NotCreator(a)
         c = utils.OpI1O1(b.outputs["output"])
 
         g = graph.infer_graph(
             {b.outputs["output"]},
             {c.outputs["output"]},
         )
@@ -137,27 +137,27 @@
         self.assertLen(g.samplings, 2)
         self.assertLen(g.nodes, 2)
         self.assertLen(g.features, 4)
 
     def test_infer_graph_missing_input(self):
         """The input is missing."""
 
-        i = utils.create_source_node("missing_node")
+        i = utils.create_input_node("missing_node")
         o2 = utils.OpI1O1(i)
 
         with self.assertRaisesRegex(ValueError, " but not provided as input"):
             graph.infer_graph(set(), {o2.outputs["output"]})
 
     def test_infer_graph_automatic_input(self):
         """Infer automatically the input."""
 
-        i1 = utils.create_source_node()
+        i1 = utils.create_input_node()
         i1.name = "io_input_1"
         o2 = utils.OpI1O1(i1)
-        i3 = utils.create_source_node()
+        i3 = utils.create_input_node()
         i3.name = "io_input_2"
         o4 = utils.OpI2O1(o2.outputs["output"], i3)
         o5 = utils.OpI1O2(o4.outputs["output"])
 
         g = graph.infer_graph(
             None,
             {o5.outputs["output_1"], o4.outputs["output"]},
@@ -167,20 +167,60 @@
         self.assertLen(g.samplings, 3)
         self.assertLen(g.nodes, 6)
         self.assertLen(g.features, 10)
 
     def test_automatic_input_equality_graph(self):
         """Automated inference when the input is the same as the output."""
 
-        i1 = utils.create_source_node()
+        i1 = utils.create_input_node()
         g = graph.infer_graph(None, {i1})
 
         self.assertLen(g.operators, 0)
         self.assertLen(g.nodes, 1)
         self.assertLen(g.samplings, 1)
         self.assertLen(g.inputs, 1)
         self.assertLen(g.outputs, 1)
         self.assertEqual(g.inputs, g.outputs)
 
+    def test_apply_on_inputs(self):
+        """Ensures applying a graph on inputs works and doesn't cause repeated
+        ordered internal op ids when infer_graph is called again on the outputs.
+        """
+        i1 = utils.create_input_node("io_input_1")
+        o2 = utils.OpI1O1(i1)
+        i3 = utils.create_input_node("io_input_2")
+        o4 = utils.OpI2O1(o2.outputs["output"], i3)
+        o5 = utils.OpI1O2(o4.outputs["output"])
+
+        output_1 = o5.outputs["output_1"]
+        output_2 = o4.outputs["output"]
+        output_1.name = "io_output_1"
+        output_2.name = "io_output_2"
+
+        g = graph.infer_graph_named_nodes([i1, i3], [output_1, output_2])
+
+        # Apply same graph again to its own outputs
+        outputs = g.apply_on_inputs(
+            {"io_input_1": output_1, "io_input_2": output_2}
+        )
+        new_output_1 = outputs["io_output_1"]
+        new_output_2 = outputs["io_output_2"]
+        new_g = graph.infer_graph_named_nodes(
+            [i1, i3], [new_output_1, new_output_2]
+        )
+
+        self.assertLen(new_g.operators, 6)
+        self.assertLen(new_g.nodes, 10)  # 6 in the original graph + 4
+        # 2 in inputs + 2 * OpI101 which creates a new one
+        self.assertLen(new_g.samplings, 4)
+        # 4 in inputs + 2 created by each operator
+        self.assertLen(new_g.features, 16)
+
+        self.assertSetEqual(new_g.inputs, {i1, i3})
+        self.assertSetEqual(new_g.outputs, {new_output_1, new_output_2})
+
+        internal_ids = [op._internal_ordered_id for op in new_g.operators]
+        self.assertEqual(len(internal_ids), len(set(internal_ids)))
+
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/core/test/operator_test.py` & `temporian-0.1.2/temporian/core/test/operator_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/core/test/registered_operators_test.py` & `temporian-0.1.2/temporian/core/test/registered_operators_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # limitations under the License.
 
 """Checks that the expected operators are registered."""
 
 from absl.testing import absltest
 
 from temporian.core import operator_lib
-from temporian.core.operators import api_symbols
+
+import temporian  # Load and register all operators
 
 
 class RegisteredOperatorsTest(absltest.TestCase):
     def test_base(self):
         # Note: The operators are stored alphabetically.
         expected_operators = [
             "ABS",
@@ -40,26 +41,28 @@
             "CALENDAR_SECOND",
             "CALENDAR_YEAR",
             "CAST",
             "DIVISION",
             "DIVISION_SCALAR",
             "DROP_INDEX",
             "END",
+            "ENUMERATE",
             "EQUAL",
             "EQUAL_SCALAR",
             "FILTER",
             "FLOORDIV",
             "FLOORDIV_SCALAR",
             "GLUE",
             "GREATER",
             "GREATER_EQUAL",
             "GREATER_EQUAL_SCALAR",
             "GREATER_SCALAR",
             "INVERT",
             "IS_NAN",
+            "JOIN",
             "LAG",
             "LEAK",
             "LESS",
             "LESS_EQUAL",
             "LESS_EQUAL_SCALAR",
             "LESS_SCALAR",
             "LOG",
@@ -84,14 +87,15 @@
             "RESAMPLE",
             "SELECT",
             "SIMPLE_MOVING_AVERAGE",
             "SINCE_LAST",
             "SUBTRACTION",
             "SUBTRACTION_SCALAR",
             "TICK",
+            "TIMESTAMPS",
             "UNIQUE_TIMESTAMPS",
             "XOR",
         ]
 
         self.assertEqual(
             expected_operators, sorted(list(set(expected_operators)))
         )
```

### Comparing `temporian-0.1.1/temporian/core/test/utils.py` & `temporian-0.1.2/temporian/core/test/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for unit testing."""
 from typing import Dict, List, Optional
 
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import (
-    Node,
+    EventSetNode,
     input_node,
     create_node_with_new_reference,
     create_node_new_features_new_sampling,
     create_node_new_features_existing_sampling,
 )
 from temporian.core.operators import base
 from temporian.proto import core_pb2 as pb
@@ -15,15 +15,15 @@
 from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.implementation.numpy.data.io import event_set
 
 # The name of the operator is defined by the number of inputs and outputs.
 # For example "OpI1O2" has 1 input and 2 outputs.
 
 
-def create_source_node(name: Optional[str] = None):
+def create_input_node(name: Optional[str] = None):
     return input_node(
         features=[
             ("f1", DType.FLOAT64),
             ("f2", DType.FLOAT64),
         ],
         indexes=[("x", DType.INT64), ("y", DType.STRING)],
         name=name,
@@ -35,29 +35,29 @@
         timestamps=[0, 2, 4, 6],
         features={
             "x": [10, 20, 30, 40],
             "y": ["a", "b", "c", "d"],
             "f1": [1.0, 2.0, 3.0, 4.0],
             "f2": [5.0, 6.0, 7.0, 8.0],
         },
-        index_features=["x", "y"],
+        indexes=["x", "y"],
         name=name,
     )
 
 
 class OpI1O1(base.Operator):
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
             key="OpI1O1",
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
-    def __init__(self, input: Node):
+    def __init__(self, input: EventSetNode):
         super().__init__()
 
         self.add_input("input", input)
         self.add_output(
             "output",
             create_node_new_features_new_sampling(
                 features=[
@@ -82,15 +82,15 @@
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
             key="OpI1O1NotCreator",
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
-    def __init__(self, input: Node):
+    def __init__(self, input: EventSetNode):
         super().__init__()
         self.add_input("input", input)
         self.add_output(
             "output",
             create_node_with_new_reference(
                 schema=input.schema,
                 features=input.feature_nodes,
@@ -112,15 +112,15 @@
             inputs=[
                 pb.OperatorDef.Input(key="input_1"),
                 pb.OperatorDef.Input(key="input_2"),
             ],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
-    def __init__(self, input_1: Node, input_2: Node):
+    def __init__(self, input_1: EventSetNode, input_2: EventSetNode):
         super().__init__()
         self.add_input("input_1", input_1)
         self.add_input("input_2", input_2)
         self.add_output(
             "output",
             create_node_new_features_existing_sampling(
                 features=[
@@ -147,15 +147,15 @@
             ],
             outputs=[
                 pb.OperatorDef.Output(key="output_1"),
                 pb.OperatorDef.Output(key="output_2"),
             ],
         )
 
-    def __init__(self, input: Node):
+    def __init__(self, input: EventSetNode):
         super().__init__()
         self.add_input("input", input)
         self.add_output(
             "output_1",
             create_node_new_features_existing_sampling(
                 features=[("f1", DType.INT32)],
                 sampling_node=input,
@@ -217,15 +217,15 @@
                     type=pb.OperatorDef.Attribute.Type.LIST_DTYPE,
                 ),
             ],
         )
 
     def __init__(
         self,
-        input: Node,
+        input: EventSetNode,
         attr_int: int,
         attr_str: str,
         attr_list: List[str],
         attr_float: float,
         attr_bool: bool,
         attr_map: Dict[str, str],
         attr_list_dtypes: List[DType],
```

### Comparing `temporian-0.1.1/temporian/implementation/__init__.py` & `temporian-0.1.2/temporian/implementation/numpy_cc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/BUILD` & `temporian-0.1.2/temporian/beam/operators/test/BUILD`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 package(
     default_visibility = ["//visibility:public"],
     licenses = ["notice"],
 )
 
-# Libraries
-# =========
-
-py_library(
-    name = "numpy",
-    srcs = ["__init__.py"],
-    srcs_version = "PY3",
-)
-
-py_library(
-    name = "evaluation",
-    srcs = ["evaluation.py"],
+py_test(
+    name = "select_test",
+    srcs = ["select_test.py"],
     srcs_version = "PY3",
     deps = [
-        ":implementation_lib",
-        "//temporian/core:schedule",
-        "//temporian/core/data:node",
-        "//temporian/implementation/numpy/data:event_set",
-        "//temporian/implementation/numpy/operators",
+        # already_there/absl/testing:absltest
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/beam/test:utils",
+        "//temporian/core/operators:select",
     ],
 )
 
-py_library(
-    name = "utils",
-    srcs = ["utils.py"],
-    srcs_version = "PY3",
-)
-
-py_library(
-    name = "implementation_lib",
-    srcs = ["implementation_lib.py"],
+py_test(
+    name = "add_index_test",
+    srcs = ["add_index_test.py"],
     srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/beam/test:utils",
+        "//temporian/core/operators:add_index",
+    ],
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/data/BUILD`

 * *Files 14% similar despite different names*

```diff
@@ -14,39 +14,44 @@
 
 py_library(
     name = "event_set",
     srcs = ["event_set.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/numpy
-        # already_there/pandas
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/utils:string",
+        "//temporian/core:mixins",
     ],
 )
 
 py_library(
     name = "io",
     srcs = ["io.py"],
     srcs_version = "PY3",
     deps = [
-        ":event_set",
         # already_there/numpy
-        # already_there/pandas
+        ":event_set",
         "//temporian/core:evaluation",
         "//temporian/core/data:schema",
         "//temporian/core/operators:add_index",
     ],
 )
 
 py_library(
     name = "plotter",
     srcs = [
         "plotter.py",
         "plotter_bokeh.py",
         "plotter_matplotlib.py",
     ],
     srcs_version = "PY3",
-    deps = [":event_set"],
+    deps = [
+        ":event_set",
+        # already_there/numpy
+        # already_there/matplotlib
+        # already_there/bokeh
+        "//temporian/core/data:duration_utils",
+    ],
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/event_set.py` & `temporian-0.1.2/temporian/implementation/numpy/data/event_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,65 +9,85 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
+
+import logging
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Tuple
-import math
+from typing import Any, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 import datetime
 import sys
 
 import numpy as np
 
-from temporian.core.data.dtypes.dtype import DType
-from temporian.core.data.node import Node, create_node_with_new_reference
+from temporian.core.data.dtype import DType
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_with_new_reference,
+)
 from temporian.core.data.schema import Schema
+from temporian.core.mixins import EventSetOperationsMixin
 from temporian.utils import string
 
-# Maximum of printed index when calling repr(evset)
+if TYPE_CHECKING:
+    from temporian.core.operators.base import Operator
+
+# Maximum of printed index groups when calling repr(evset)
 MAX_NUM_PRINTED_INDEX = 5
 
 # Maximum of printed features when calling repr(evset)
 MAX_NUM_PRINTED_FEATURES = 10
 
-_PYTHON_DTYPE_MAPPING = {
-    str: DType.STRING,
-    # TODO: fix this, int doesn't have to be INT64 necessarily
-    int: DType.INT64,
-    np.int64: DType.INT64,
-}
-
 # Mapping of temporian types to and from numpy types.
 #
 # Remarks:
 #   - np.object_ is not automatically converted into DType.STRING.
-#   - Strings are always represented internally as np.str_ for features and str
-#     for index values.
+#   - Strings are always represented internally as np.bytes_ for features and
+#       bytes for index groups.
 _DTYPE_MAPPING = {
     np.float64: DType.FLOAT64,
     np.float32: DType.FLOAT32,
     np.int64: DType.INT64,
     np.int32: DType.INT32,
     np.str_: DType.STRING,
-    np.string_: DType.STRING,
+    np.bytes_: DType.STRING,
     np.bool_: DType.BOOLEAN,
     np.datetime64: DType.INT64,
 }
 _DTYPE_REVERSE_MAPPING = {
     DType.FLOAT64: np.float64,
     DType.FLOAT32: np.float32,
     DType.INT64: np.int64,
     DType.INT32: np.int32,
-    DType.STRING: np.str_,
+    DType.STRING: np.bytes_,
     DType.BOOLEAN: np.bool_,
 }
 
+IndexItemType = Union[int, str, bytes]
+IndexType = Tuple[IndexItemType, ...]
+
+
+def normalize_index_item(x: IndexItemType) -> IndexItemType:
+    if isinstance(x, str):
+        return x.encode()
+    return x
+
+
+def normalize_index_key(
+    index: Optional[Union[IndexItemType, IndexType]]
+) -> Optional[Union[IndexItemType, IndexType]]:
+    if index is None:
+        return None
+    if isinstance(index, tuple):
+        return tuple([normalize_index_item(x) for x in index])
+    return normalize_index_item(index)
+
 
 def is_supported_numpy_dtype(numpy_dtype) -> bool:
     return numpy_dtype in _DTYPE_MAPPING
 
 
 def numpy_dtype_to_tp_dtype(feature_name: str, numpy_dtype) -> DType:
     """Converts a numpy dtype into a temporian dtype."""
@@ -92,14 +112,15 @@
 
 def tp_dtype_to_np_dtype(dtype: DType) -> Any:
     return _DTYPE_REVERSE_MAPPING[dtype]
 
 
 def normalize_features(
     feature_values: Any,
+    name: str,
 ) -> np.ndarray:
     """Normalizes a list of feature values to temporian format.
 
     Keep this function in sync with the documentation of "io.event_set".
 
     `normalize_features` should match `_DTYPE_MAPPING`.
     """
@@ -108,45 +129,43 @@
         if feature_values.dtype == "object":
             feature_values = feature_values.fillna("")
         feature_values = feature_values.to_numpy(copy=True)
 
     if not isinstance(feature_values, np.ndarray):
         # The data is not a np.array
 
-        all_str = all(
-            (
-                isinstance(x, (str, bytes)) or x is math.nan or x is np.nan
-                for x in feature_values
-            )
-        )
+        # Looks for an indication of a string or non-string array.
+        is_string = False
+        for x in feature_values:
+            if isinstance(x, (str, bytes)):
+                is_string = True
+                break
+            if isinstance(x, (int, bool, float)):
+                is_string = False
+                break
 
-        if all_str:
+        if is_string:
             # All the values are python strings.
-            feature_values = [
-                "" if x is math.nan or x is np.nan else x
-                for x in feature_values
-            ]
-            feature_values = np.array(feature_values, dtype=np.str_)
+            feature_values = np.array(feature_values, dtype=np.bytes_)
         else:
             feature_values = np.array(feature_values)
 
     if feature_values.dtype.type == np.string_:
-        feature_values = feature_values.astype(np.str_)
+        feature_values = feature_values.astype(np.bytes_)
 
-    # TODO: This is slow. Speed-up.
-    if feature_values.dtype.type == np.object_ and all(
-        isinstance(x, str) or x is math.nan or x is np.nan
-        for x in feature_values
-    ):
-        # This is a np.array of python string.
-        # TODO: This is slow. Speed-up.
-        feature_values = np.array(
-            ["" if x is math.nan or x is np.nan else x for x in feature_values],
-            dtype=np.str_,
+    if feature_values.dtype.type == np.object_:
+        logging.warning(
+            (
+                'Feature "%s" is an array of numpy.object_ and was casted to'
+                " numpy.string_ (Note: numpy.string_ is equivalent to"
+                " numpy.bytes_)."
+            ),
+            name,
         )
+        feature_values = feature_values.astype(np.bytes_)
 
     if feature_values.dtype.type == np.datetime64:
         feature_values = feature_values.astype("datetime64[s]").astype(np.int64)
 
     return feature_values
 
 
@@ -173,15 +192,15 @@
     if values.dtype.type == np.float64:
         # Check NaN
         if np.isnan(values).any():
             raise ValueError("Timestamps contains NaN values.")
 
         return values, False
 
-    if values.dtype.type in [np.str_, np.string_]:
+    if values.dtype.type in [np.str_, np.bytes_]:
         values = values.astype("datetime64[ns]")
 
     if values.dtype.type == np.object_:
         if all(isinstance(x, str) for x in values) or all(
             isinstance(x, datetime.datetime) for x in values
         ):
             # values is a date. Cast to unix epoch in float64 seconds.
@@ -212,26 +231,26 @@
         " list of supported timestamp types. Instead, got"
         f" {object_description}."
     )
 
 
 @dataclass
 class IndexData:
-    """Features and timestamps data for a single index item.
+    """Features and timestamps data for a single index group.
 
     Note: The `schema` constructor argument is only used for checking. If
     `schema=None`, no checking is done. Checking can be done manually with
     `index_data.check_schema(...)`.
 
     Attributes:
         features: List of one-dimensional NumPy arrays representing the
             features.
         timestamps: One-dimensional NumPy array representing the timestamps.
 
-    Example usage:
+    Usage example:
         ```
         >>> features = [np.array([1, 2, 3]), np.array([4, 5, 6])]
         >>> timestamps = np.array([0, 1, 2])
         >>> index_data = IndexData(features, timestamps)
         >>> len(index_data)
         3
 
@@ -304,17 +323,14 @@
         if not isinstance(other, IndexData):
             return False
 
         if not np.array_equal(self.timestamps, other.timestamps):
             return False
 
         for f1, f2 in zip(self.features, other.features):
-            if f1.dtype != f2.dtype:
-                return False
-
             if f1.dtype.kind == "f":
                 if not np.allclose(f1, f2, equal_nan=True):
                     return False
             else:
                 if not np.array_equal(f1, f2):
                     return False
 
@@ -322,97 +338,96 @@
 
     def __len__(self) -> int:
         """Number of events / timestamps."""
 
         return len(self.timestamps)
 
 
-class EventSet:
+class EventSet(EventSetOperationsMixin):
     """Actual temporal data.
 
-    Use [`tp.event_set()`][temporian.event_set] to create an event set manually,
-    or [`tp.from_pandas()`][temporian.from_pandas] to create an event set from a
+    Use [`tp.event_set()`][temporian.event_set] to create an EventSet manually,
+    or [`tp.from_pandas()`][temporian.from_pandas] to create an EventSet from a
     pandas DataFrame.
     """
 
     def __init__(
         self,
-        data: Dict[Tuple, IndexData],
+        data: Dict[IndexType, IndexData],
         schema: Schema,
         name: Optional[str] = None,
     ) -> None:
         self._data = data
         self._schema = schema
         self._name = name
 
-        # Node created when "self.node()" is called.
-        self._internal_node: Optional[Node] = None
+        # EventSetNode created when "self.node()" is called.
+        self._internal_node: Optional[EventSetNode] = None
 
     @property
-    def data(self) -> Dict[Tuple, IndexData]:
+    def data(self) -> Dict[IndexType, IndexData]:
         return self._data
 
     @property
     def schema(self) -> Schema:
         return self._schema
 
     @property
     def name(self) -> Optional[str]:
         return self._name
 
     @name.setter
     def name(self, name: Optional[str]) -> None:
         self._name = name
 
-    def get_arbitrary_index_value(self) -> Optional[Tuple]:
-        """Gets an arbitrary index value.
+    def get_arbitrary_index_key(self) -> Optional[IndexType]:
+        """Gets an arbitrary index key.
 
-        If the event set is empty, return None.
+        If the EventSet is empty, return None.
         """
 
         if self._data:
             return next(iter(self._data.keys()))
         return None
 
     def get_arbitrary_index_data(self) -> Optional[IndexData]:
-        """Gets an arbitrary index data.
+        """Gets data from an arbitrary index key.
 
-        If the event set is empty, return None.
+        If the EventSet is empty, return None.
         """
 
         if self._data:
             return next(iter(self._data.values()))
         return None
 
-    def node(self, force_new_node: bool = False) -> Node:
-        """Creates a node able to consume the the event set.
+    def node(self, force_new_node: bool = False) -> EventSetNode:
+        """Creates an [`EventSetNode`][temporian.EventSetNode] able to consume the the EventSet.
 
         If called multiple times with `force_new_node=False` (default), the same
         node is returned.
 
         Usage example:
+            ```python
+            >>> my_evset = tp.event_set(
+            ...     timestamps=[1, 2, 3, 4],
+            ...     features={
+            ...         "feature_1": [0.5, 0.6, np.nan, 0.9],
+            ...         "feature_2": ["red", "blue", "red", "blue"],
+            ...     },
+            ... )
+            >>> my_node = my_evset.node()
 
-        ```python
-        >>> my_evset = tp.event_set(
-        ...     timestamps=[1, 2, 3, 4],
-        ...     features={
-        ...         "feature_1": [0.5, 0.6, np.nan, 0.9],
-        ...         "feature_2": ["red", "blue", "red", "blue"],
-        ...     },
-        ... )
-        >>> my_node = my_evset.node()
-
-        ```
+            ```
 
         Args:
             force_new_node: If false (default), return the same node each time
                 `node` is called. If true, a new node is created each time.
 
         Returns:
-            A node able to consume the content of the event set.
+            A EventSetNode able to consume the content of the EventSet.
         """
 
         if self._internal_node is not None and not force_new_node:
             # "node" was already called. Return the cached node.
             return self._internal_node
 
         self._internal_node = create_node_with_new_reference(
@@ -460,19 +475,39 @@
             f"indexes: {self.schema.indexes}\n"
             f"features: {self.schema.features}\n"
             "events:\n"
             f"{data_repr}\n"
             f"memory usage: {string.pretty_num_bytes(self.memory_usage())}\n"
         )
 
-    def __getitem__(self, index: Tuple) -> IndexData:
-        return self.data[index]
+    def get_index_value(
+        self, index_key: Tuple, normalize: bool = True
+    ) -> IndexData:
+        """Gets the value for a specified index key.
+
+        The index key must be a tuple of values corresponding to the indexes
+        of the EventSet.
+        """
+
+        if normalize:
+            index_key = normalize_index_key(index_key)
+        return self.data[index_key]
+
+    def set_index_value(
+        self, index_key: Tuple, value: IndexData, normalize: bool = True
+    ) -> None:
+        """Sets the value for a specified index key.
+
+        The index key must be a tuple of values corresponding to the indexes
+        of the EventSet.
+        """
 
-    def __setitem__(self, index: Tuple, value: IndexData) -> None:
-        self.data[index] = value
+        if normalize:
+            index_key = normalize_index_key(index_key)
+        self.data[index_key] = value
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, EventSet):
             return False
 
         if self._name != other._name:
             return False
@@ -482,15 +517,15 @@
 
         if self._data != other._data:
             return False
 
         return True
 
     def plot(self, *args, **wargs) -> Any:
-        """Plots the event set. See [`tp.plot()`][temporian.plot] for details.
+        """Plots the EventSet. See [`tp.plot()`][temporian.plot] for details.
 
         Example usage:
 
             ```python
             >>> evset = tp.event_set(timestamps=[1, 2, 3], features={"f1": [0, 42, 10]})
             >>> evset.plot()
 
@@ -508,13 +543,26 @@
                 index_data.timestamps
             )
             for feature in index_data.features:
                 size += sys.getsizeof(feature)
         return size
 
     def memory_usage(self) -> int:
-        """Gets the approximated memory usage of the event set in bytes.
+        """Gets the approximated memory usage of the EventSet in bytes.
 
         Takes into account garbage collector overhead.
         """
 
         return sys.getsizeof(self)
+
+    def check_same_sampling(self, other: EventSet):
+        """Checks if two EventSets have the same sampling."""
+        self.node().check_same_sampling(other.node())
+
+    @property
+    def creator(self) -> Optional[Operator]:
+        """Creator.
+
+        The creator is the operator that outputted this EventSet. Manually
+        created EventSets have a `None` creator.
+        """
+        return self.node()._creator
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/io.py` & `temporian-0.1.2/temporian/implementation/numpy/data/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,66 +6,67 @@
 from temporian.implementation.numpy.data.event_set import (
     EventSet,
     IndexData,
     numpy_array_to_tp_dtype,
     normalize_timestamps,
     normalize_features,
 )
-from temporian.core.evaluation import evaluate
+from temporian.core.evaluation import run
 from temporian.core.operators.add_index import add_index
 from temporian.core.data.schema import Schema
 
 # Array of values as feed by the user.
 DataArray = Union[List[Any], np.ndarray, "pandas.Series"]
 
 
 # Note: Keep the documentation about supported types in sync with
 # "normalize_timestamp" and "normalize_features".
 def event_set(
     timestamps: DataArray,
     features: Optional[Dict[str, DataArray]] = None,
-    index_features: Optional[List[str]] = None,
+    indexes: Optional[List[str]] = None,
     name: Optional[str] = None,
     is_unix_timestamp: Optional[bool] = None,
     same_sampling_as: Optional[EventSet] = None,
 ) -> EventSet:
-    """Creates an event set from arrays (list, numpy, pandas).
+    """Creates an [`EventSet`][temporian.EventSet] from arrays (lists, NumPy
+    arrays, Pandas Series.)
 
     Usage examples:
 
         ```python
-        >>> # Creates an event set with 4 timestamps and 3 features.
+        >>> # Creates an EventSet with 4 timestamps and 3 features.
         >>> evset = tp.event_set(
         ...     timestamps=[1, 2, 3, 4],
         ...     features={
         ...         "feature_1": [0.5, 0.6, np.nan, 0.9],
         ...         "feature_2": ["red", "blue", "red", "blue"],
         ...         "feature_3": [10, -1, 5, 5],
         ...     },
         ... )
 
-        >>> # Creates an event set with an index.
+        >>> # Creates an EventSet with an index.
         >>> evset = tp.event_set(
         ...     timestamps=[1, 2, 3, 4],
         ...     features={
         ...         "feature_1": [0.5, 0.6, np.nan, 0.9],
         ...         "feature_2": ["red", "blue", "red", "blue"],
         ...     },
-        ...     index_features=["feature_2"],
+        ...     indexes=["feature_2"],
         ... )
 
-        >>> # Create an evet set with datetimes.
+        >>> # Create an EventSet with datetimes.
         >>> from datetime import datetime
         >>> evset = tp.event_set(
         ...     timestamps=[datetime(2015, 1, 1), datetime(2015, 1, 2)],
         ...     features={
         ...         "feature_1": [0.5, 0.6],
         ...         "feature_2": ["red", "blue"],
         ...     },
-        ...     index_features=["feature_2"],
+        ...     indexes=["feature_2"],
         ... )
 
         ```
 
     Supported values for `timestamps`:
 
     - List of int, float, str, bytes and datetime.
@@ -85,37 +86,38 @@
     Date / datetime features are converted to int64 unix times.
     NaN for float-like features are interpreted as missing values.
 
     Args:
         timestamps: Array of timestamps values.
         features: Dictionary of feature names to feature values. Feature
             and timestamp arrays must be of the same length.
-        index_features: Names of the features to use as index. If empty
+        indexes: Names of the features to use as indexes. If empty
             (default), the data is not indexed. Only integer and string features
-            can be used as index.
-        name: Optional name of the event set. Used for debugging, and
+            can be used as indexes.
+        name: Optional name of the EventSet. Used for debugging, and
             graph serialization.
         is_unix_timestamp: Whether the timestamps correspond to unix time. Unix
             times are required for calendar operators. If `None` (default),
             timestamps are interpreted as unix times if the `timestamps`
             argument is an array of date or date-like object.
-        same_sampling_as: If set, the new event set is cheched and tagged as
+        same_sampling_as: If set, the new EventSet is cheched and tagged as
             having the same sampling as `same_sampling_as`. Some operators,
             such as [`tp.filter()`][temporian.filter], require their inputs to
             have the same sampling.
 
     Returns:
-        An event set.
+        An EventSet.
     """
 
     if features is None:
         features = {}
 
     features = {
-        name: normalize_features(value) for name, value in features.items()
+        name: normalize_features(value, name)
+        for name, value in features.items()
     }
 
     # Convert timestamps to expected type.
     timestamps, auto_is_unix_timestamp = normalize_timestamps(timestamps)
 
     if not np.all(timestamps[:-1] <= timestamps[1:]):
         order = np.argsort(timestamps, kind="mergesort")
@@ -145,42 +147,39 @@
         schema=schema,
     )
     evset = EventSet(
         schema=schema,
         data={(): index_data},
     )
 
-    if index_features:
+    if indexes:
         # Index the data
         input_node = evset.node()
-        output_node = add_index(input_node, index_to_add=index_features)
-        evset = evaluate(output_node, {input_node: evset})
+        output_node = add_index(input_node, indexes=indexes)
+        evset = run(output_node, {input_node: evset})
         assert isinstance(evset, EventSet)
 
     evset.name = name
 
     if same_sampling_as is not None:
-        evset.schema.check_compatible_index(
-            same_sampling_as.schema,
-            label="the new event set and `same_sampling_as`",
-        )
+        evset.schema.check_compatible_index(same_sampling_as.schema)
 
         if evset.data.keys() != same_sampling_as.data.keys():
             raise ValueError(
-                "The new event set and `same_sampling_as` have the same index,"
-                " but different index values. Both should have the same index"
-                " keys to have the same sampling."
+                "The new EventSet and `same_sampling_as` have the same"
+                " indexes, but different index keys. They should have the"
+                " same index keys to have the same sampling."
             )
 
         for key, same_sampling_as_value in same_sampling_as.data.items():
             if not np.all(
                 evset.data[key].timestamps == same_sampling_as_value.timestamps
             ):
                 raise ValueError(
-                    "The new event set and `same_sampling_as` have different"
+                    "The new EventSet and `same_sampling_as` have different"
                     f" timestamps values for the index={key!r}. The timestamps"
                     " should be equal for both to have the same sampling."
                 )
 
             # Discard the new timestamps arrays.
             evset.data[key].timestamps = same_sampling_as_value.timestamps
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/plotter.py` & `temporian-0.1.2/temporian/implementation/numpy/data/plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 
 from typing import NamedTuple, Optional, Union, List, Any, Set
 from enum import Enum
 
 import numpy as np
 
 from temporian.core.data import duration_utils
-from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.implementation.numpy.data.event_set import (
+    EventSet,
+    normalize_index_key,
+    IndexItemType,
+    IndexType,
+)
 
 
 class Style(Enum):
     """Plotting style."""
 
     # Determine the style according to the data.
     auto = "auto"
@@ -48,35 +53,60 @@
     max_num_plots: int
     style: Style
     interactive: bool
 
 
 def plot(
     evsets: Union[List[EventSet], EventSet],
-    indexes: Optional[Union[Any, tuple, List[tuple]]] = None,
+    indexes: Optional[
+        Union[IndexItemType, IndexType, List[IndexItemType], List[IndexType]]
+    ] = None,
     features: Optional[Union[str, List[str], Set[str]]] = None,
     width_px: int = 1024,
     height_per_plot_px: int = 150,
     max_points: Optional[int] = None,
     min_time: Optional[duration_utils.Timestamp] = None,
     max_time: Optional[duration_utils.Timestamp] = None,
     max_num_plots: int = 20,
     style: Union[Style, str] = Style.auto,
     return_fig: bool = False,
     interactive: bool = False,
     backend: Optional[str] = None,
 ):
-    """Plots event sets.
+    """Plots [`EventSets`][temporian.EventSet].
+
+    This method can also be called from
+    [`EventSet.plot()`][temporian.EventSet.plot] with the same args (except
+    `evsets`).
+
+    Examples:
+        ```python
+        >>> evset = tp.event_set(timestamps=[1, 2, 4],
+        ...     features={"f1": [0, 42, 10], "f2": [10, -10, 20]})
+
+        # Default
+        >>> tp.plot(evset)
+
+        # Lines instead of markers, only f2, limit x-axis to t=2
+        >>> tp.plot(evset, style="line", features="f2", max_time=2)
+
+        # Access figure and axes
+        >>> fig = tp.plot(evset, return_fig=True)
+        >>> fig.tight_layout(pad=3.0)
+        >>> _ = fig.axes[0].set_ylim([-50, 50])
+
+        ```
 
     Args:
-        evsets: Single or list of event sets to plot.
-        indexes: The index or list of indexes to plot. If index=None, plots all
-            the available indexes. Indexes should be provided as single value
-            (e.g. string) or tuple of values. Example: index="a", index=("a",),
-            index=("a", "b",), index=["a", "b"], index=[("a", "b"), ("a", "c")].
+        evsets: Single or list of EventSets to plot.
+        indexes: The index keys or list of indexes keys to plot. If
+            indexes=None, plots all the available indexes. Indexes should be
+            provided as single value (e.g. string) or tuple of values. Example:
+            indexes="a", indexes=("a",), indexes=("a", "b",),
+            indexes=["a", "b"], indexes=[("a", "b"), ("a", "c")].
         features: Feature names of the event(s) to plot. Use
             'evset.feature_names' for the list of available names.
             If a feature doesn't exist in an event, it's silently skipped.
             If None, plots all features of all events.
         width_px: Width of the figure in pixel.
         height_per_plot_px: Height of each sub-plot (one per feature) in pixel.
         max_points: Maximum number of points to plot.
@@ -115,19 +145,21 @@
         # e.g. indexes=["a", ("b",)]
         indexes = [v if isinstance(v, tuple) else (v,) for v in indexes]
 
     else:
         # e.g. indexes="a"
         indexes = [(indexes,)]
 
+    indexes = [normalize_index_key(x) for x in indexes]
+
     for index in indexes:
         if not isinstance(index, tuple):
             raise ValueError(
-                "An index should be a tuple or a list of tuples. Instead"
-                f' receives "indexes={original_indexes}"'
+                "Indexes should be tuples or lists of tuples. Instead"
+                f' received "indexes={original_indexes}"'
             )
 
     if isinstance(style, str):
         style = Style[style]
     assert isinstance(style, Style)
 
     if features is None:
@@ -193,19 +225,19 @@
     """Computes the number of sub-plots."""
 
     num_plots = 0
     for index in indexes:
         for evset in evsets:
             if index not in evset.data:
                 raise ValueError(
-                    f"Index '{index}' does not exist in event set. Check the"
-                    " available indexes with 'evset.index' and provide one of"
-                    " those index to the 'index' argument of 'plot'."
-                    ' Alternatively, set "index=None" to select a random'
-                    f" index value (e.g., {evset.get_arbitrary_index_value()}."
+                    f"Index key '{index}' does not exist in the EventSet. Check"
+                    " the available indexes with 'evset.indexes' and provide"
+                    " one of those to the 'indexes' argument of 'plot'."
+                    " Alternatively, set 'indexes=None' to select a random"
+                    f" index key (e.g., {evset.get_arbitrary_index_key()}."
                 )
             candidate_features = set(evset.schema.feature_names())
             num_features = len(candidate_features.intersection(features))
             if num_features == 0:
                 # We plot the sampling
                 num_features = 1
             num_plots += num_features
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/plotter_bokeh.py` & `temporian-0.1.2/temporian/implementation/numpy/data/plotter_bokeh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Bokeh plotting backend."""
 
 import datetime
 from typing import Optional, List, Any, Set
 
 import numpy as np
 
-from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.implementation.numpy.data.event_set import EventSet, IndexType
 from temporian.implementation.numpy.data.plotter import (
     Options,
     Style,
     is_uniform,
     get_num_plots,
     auto_style,
 )
 
 
 def plot_bokeh(
     evsets: List[EventSet],
-    indexes: List[tuple],
+    indexes: List[IndexType],
     features: Set[str],
     options: Options,
 ):
     from bokeh.io import output_notebook, show
     from bokeh.layouts import gridplot
     from bokeh.models import CustomJS
     from bokeh.palettes import Dark2_5 as colors
@@ -33,25 +33,25 @@
     # Actual plotting
     plot_idx = 0
     for index in indexes:
         if plot_idx >= num_plots:
             # Too much plots are displayed already.
             break
 
-        # Note: Don't display the tuple parenthesis is the index contain a
-        # single dimension.
-        title = str(index[0] if len(index) == 1 else index)
-
         # Index of the next color to use in the plot.
         color_idx = 0
 
         for evset in evsets:
             if plot_idx >= num_plots:
                 break
 
+            title = " ".join(
+                [f"{k}={v}" for k, v in zip(evset.schema.index_names(), index)]
+            )
+
             evset_features = evset.schema.feature_names()
             display_features = [f for f in evset_features if f in features]
 
             xs = evset.data[index].timestamps
             uniform = is_uniform(xs)
 
             plot_mask = np.full(len(xs), True)
@@ -202,16 +202,17 @@
 
     fig_args = {}
     if is_unix_timestamp:
         fig_args["x_axis_type"] = "datetime"
     if title:
         fig_args["title"] = title
 
-    is_string = ys.dtype.type is np.str_ or ys.dtype.type is np.string_
+    is_string = ys.dtype.type is np.str_ or ys.dtype.type is np.bytes_
     if is_string:
+        ys = ys.astype(np.str_)
         unique_ys_values = list(set(ys))
         fig_args["y_range"] = unique_ys_values
     else:
         unique_ys_values = None
 
     fig = figure(
         width=options.width_px,
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/plotter_matplotlib.py` & `temporian-0.1.2/temporian/implementation/numpy/data/plotter_matplotlib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Matplotlib plotting backend."""
 
 import datetime
 from typing import Optional, List, Set
 
 import numpy as np
 
-from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.implementation.numpy.data.event_set import EventSet, IndexType
 from temporian.implementation.numpy.data.plotter import (
     Options,
     Style,
     is_uniform,
     get_num_plots,
     auto_style,
 )
 
 
 def plot_matplotlib(
     evsets: List[EventSet],
-    indexes: List[tuple],
+    indexes: List[IndexType],
     features: Set[str],
     options: Options,
 ):
     import matplotlib.pyplot as plt
     from matplotlib.cm import get_cmap
 
     colors = get_cmap("tab10").colors
@@ -42,25 +42,25 @@
     # Actual plotting
     plot_idx = 0
     for index in indexes:
         if plot_idx >= num_plots:
             # Too much plots are displayed already.
             break
 
-        # Note: Don't display the tuple parenthesis is the index contain a
-        # single dimension.
-        title = str(index[0] if len(index) == 1 else index)
-
         # Index of the next color to use in the plot.
         color_idx = 0
 
         for evset in evsets:
             if plot_idx >= num_plots:
                 break
 
+            title = " ".join(
+                [f"{k}={v}" for k, v in zip(evset.schema.index_names(), index)]
+            )
+
             evset_features = evset.schema.feature_names()
             display_features = [f for f in evset_features if f in features]
 
             xs = evset.data[index].timestamps
             uniform = is_uniform(xs)
 
             plot_mask = np.full(len(xs), True)
@@ -190,8 +190,8 @@
     ax.set_ylabel(name, size=8)
     ax.yaxis.set_tick_params(labelsize=8)
     ax.yaxis.set_major_locator(ticker.MaxNLocator(5))
     ax.yaxis.set_minor_locator(ticker.NullLocator())
 
     ax.grid(lw=0.4, ls="--", axis="x")
     if title:
-        ax.set_title(title)
+        ax.set_title(title, fontsize=8)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/test/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/data/test/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
     name = "io_test",
     srcs = ["io_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:schema",
         "//temporian/implementation/numpy/data:event_set",
         "//temporian/implementation/numpy/data:io",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/test/event_set_test.py` & `temporian-0.1.2/temporian/implementation/numpy/data/test/event_set_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,82 @@
+import numpy as np
 from absl.testing import absltest
 
-from temporian.implementation.numpy.data.io import event_set
+from temporian.implementation.numpy.data.io import event_set, IndexData
 
 # TODO: Rename file to "event_set_test" and rename the following class to EventSetTest.
 
 
 class EventTest(absltest.TestCase):
     def setUp(self):
-        self._evset = event_set(
+        self.evset = event_set(
             timestamps=[0.1, 0.2, 0.3, 0.4, 0.5],
             features={
                 "a": [1, 2, 3, 7, 8],
                 "b": [4, 5, 6, 9, 10],
                 "x": [1, 1, 1, 2, 2],
                 "y": ["hello", "hello", "hello", "world", "world"],
             },
-            index_features=["x", "y"],
+            indexes=["x", "y"],
         )
 
+    def test_get_index_value(self):
+        index_data = self.evset.get_index_value((2, b"world"), normalize=False)
+        self.assertTrue(isinstance(index_data, IndexData))
+        self.assertTrue(
+            (np.array(index_data.features) == [[7, 8], [9, 10]]).all()
+        )
+        self.assertTrue((abs(index_data.timestamps - [0.4, 0.5]) < 1e-6).all())
+
+    def test_get_index_value_normalized(self):
+        index_data = self.evset.get_index_value((2, "world"))
+        self.assertTrue(isinstance(index_data, IndexData))
+        self.assertTrue(
+            (np.array(index_data.features) == [[7, 8], [9, 10]]).all()
+        )
+        self.assertTrue((abs(index_data.timestamps - [0.4, 0.5]) < 1e-6).all())
+
+    def test_set_index_value(self):
+        value = self.evset.get_index_value((1, b"hello"))
+        modified = IndexData(
+            timestamps=value.timestamps,
+            features=[f + 1 for f in value.features],
+        )
+        self.evset.set_index_value((2, b"world"), modified)
+        self.assertEqual(self.evset.get_index_value((2, b"world")), modified)
+
     def test_data_access(self):
         self.assertEqual(
-            repr(self._evset.schema.features), "[('a', int64), ('b', int64)]"
+            repr(self.evset.schema.features), "[('a', int64), ('b', int64)]"
         )
         self.assertEqual(
-            repr(self._evset.schema.indexes), "[('x', int64), ('y', str_)]"
+            repr(self.evset.schema.indexes), "[('x', int64), ('y', str_)]"
         )
 
     def test_repr(self):
-        print(self._evset)
+        print(self.evset)
         self.assertEqual(
-            repr(self._evset),
+            repr(self.evset),
             """indexes: [('x', int64), ('y', str_)]
 features: [('a', int64), ('b', int64)]
 events:
-    x=1 y=hello (3 events):
+    x=1 y=b'hello' (3 events):
         timestamps: [0.1 0.2 0.3]
         'a': [1 2 3]
         'b': [4 5 6]
-    x=2 y=world (2 events):
+    x=2 y=b'world' (2 events):
         timestamps: [0.4 0.5]
         'a': [7 8]
         'b': [ 9 10]
 memory usage: 1.2 kB
 """,
         )
 
     def test_memory_usage(self):
-        memory_usage = self._evset.memory_usage()
+        memory_usage = self.evset.memory_usage()
         print("memory_usage:", memory_usage)
 
         self.assertLessEqual(memory_usage, 1200 + 500)
         self.assertGreaterEqual(memory_usage, 1200 - 500)
 
 
 if __name__ == "__main__":
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/test/io_test.py` & `temporian-0.1.2/temporian/implementation/numpy/data/test/io_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 from numpy.testing import assert_array_equal
 from datetime import datetime
 
 from temporian.implementation.numpy.data.io import event_set
 from temporian.implementation.numpy.data.event_set import IndexData, EventSet
 from temporian.core.data.schema import Schema
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 
 
 class IOTest(absltest.TestCase):
     def test_event_set(self):
         # a
         evset = event_set(
             timestamps=[1, 2, 3, 4],
@@ -22,15 +22,15 @@
                 "feature_1": [0.5, 0.6, math.nan, 0.9],
                 "feature_2": ["red", "blue", "red", "blue"],
                 "feature_3": [10, -1, 5, 5],
                 "feature_4": ["a", "b", math.nan, "c"],
                 "feature_5": pd.Series(["d", "e", math.nan, "f"]),
                 "feature_6": pd.Series([1, 2, 3, 4]),
             },
-            index_features=["feature_2"],
+            indexes=["feature_2"],
         )
 
         expected_schema = Schema(
             features=[
                 ("feature_1", DType.FLOAT64),
                 ("feature_3", DType.INT64),
                 ("feature_4", DType.STRING),
@@ -38,43 +38,43 @@
                 ("feature_6", DType.INT64),
             ],
             indexes=[("feature_2", DType.STRING)],
             is_unix_timestamp=False,
         )
         expected_evset = EventSet(
             data={
-                ("red",): IndexData(
+                (b"red",): IndexData(
                     features=[
                         np.array([0.5, math.nan]),
                         np.array([10, 5]),
-                        np.array(["a", ""]),
-                        np.array(["d", ""]),
+                        np.array([b"a", b"nan"]),
+                        np.array([b"d", b""]),
                         np.array([1, 3]),
                     ],
                     timestamps=np.array([1.0, 3.0], dtype=np.float64),
                     schema=expected_schema,
                 ),
-                ("blue",): IndexData(
+                (b"blue",): IndexData(
                     features=[
                         np.array([0.6, 0.9]),
                         np.array([-1, 5]),
-                        np.array(["b", "c"]),
-                        np.array(["e", "f"]),
+                        np.array([b"b", b"c"]),
+                        np.array([b"e", b"f"]),
                         np.array([2, 4]),
                     ],
                     timestamps=np.array([2.0, 4.0], dtype=np.float64),
                     schema=expected_schema,
                 ),
             },
             schema=expected_schema,
         )
 
         print("evset:\n", evset)
         print("expected_evset:\n", expected_evset)
-        self.assertEqual(repr(evset), repr(expected_evset))
+        self.assertEqual(evset, expected_evset)
 
     def test_timestamps_non_unix_time(self):
         for timestamps in [
             [2],
             [2.0],
             np.array([2], dtype=np.int32),
             np.array([2], dtype=np.int64),
@@ -95,15 +95,15 @@
             # Python
             [datetime(1970, 1, 2)],
             ["1970-01-02"],
             [b"1970-01-02"],
             # Numpy
             [np.datetime64("1970-01-02")],
             np.array(["1970-01-02"], dtype=np.str_),
-            np.array(["1970-01-02"], dtype=np.string_),
+            np.array(["1970-01-02"], dtype=np.bytes_),
             np.array(["1970-01-02"], dtype=np.object_),
             # Pandas
             pd.Series([pd.Timestamp("1970-01-02")]),
             pd.Series(["1970-01-02"]),
         ]:
             logging.info("Testing: %s (%s)", timestamps, type(timestamps))
             evset = event_set(timestamps)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/data/test/plotter_test.py` & `temporian-0.1.2/temporian/implementation/numpy/data/test/plotter_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             timestamps=[0.1, 0.2, 0.3, 0.4, 0.5],
             features={
                 "a": [1, 2, 3, 7, 8],
                 "b": [4, 5, 6, 9, 10],
                 "c": ["X", "Y", "X", "X", "Z"],
                 "x": [1, 1, 1, 2, 2],
             },
-            index_features=["x"],
+            indexes=["x"],
         )
 
         _ = plotter.plot(
             evset, indexes=None, interactive=interactive, return_fig=True
         )
         _ = plotter.plot(
             evset, indexes=1, interactive=interactive, return_fig=True
@@ -43,14 +43,37 @@
         _ = plotter.plot(
             evset,
             indexes=[(1,), (2,)],
             interactive=interactive,
             return_fig=True,
         )
 
+    def test_index_str(self):
+        try:
+            import IPython.display
+        except ImportError:
+            # IPython is not installed / supported
+            return
+
+        evset = event_set(
+            timestamps=[0.1, 0.2, 0.3],
+            features={
+                "a": [1, 2, 3],
+                "b": [4, 5, 6],
+                "c": ["X", "Y", "X"],
+                "x": [1, 1, 1],
+            },
+            indexes=["c"],
+        )
+
+        _ = plotter.plot(evset, indexes="X", return_fig=True)
+        _ = plotter.plot(evset, indexes=b"X", return_fig=True)
+        _ = plotter.plot(evset, indexes=["X", "Y"], return_fig=True)
+        _ = plotter.plot(evset, indexes=[("X",), ("Y",)], return_fig=True)
+
     def test_is_uniform(self):
         self.assertTrue(plotter.is_uniform([]))
         self.assertTrue(plotter.is_uniform([1]))
         self.assertTrue(plotter.is_uniform([1, 2, 3]))
         self.assertFalse(plotter.is_uniform([1, 2, 2.5]))
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/evaluation.py` & `temporian-0.1.2/temporian/implementation/numpy/evaluation.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,74 +13,72 @@
 # limitations under the License.
 
 import sys
 import time
 
 from typing import Dict
 
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.core.schedule import Schedule
 
 # Loads all the numpy operator implementations
 from temporian.implementation.numpy import operators as _impls
 
 
-def evaluate_schedule(
-    inputs: Dict[Node, EventSet],
+def run_schedule(
+    inputs: Dict[EventSetNode, EventSet],
     schedule: Schedule,
     verbose: int,
     check_execution: bool,
-) -> Dict[Node, EventSet]:
-    """Evaluates a schedule on a dictionary of input event sets.
+) -> Dict[EventSetNode, EventSet]:
+    """Evaluates a schedule on a dictionary of input
+    [`EventSets`][temporian.EventSet].
 
     Args:
-        inputs: Mapping of nodes to materialized EventSets.
+        inputs: Mapping of EventSetNodes to materialized EventSets.
         schedule: Sequence of operators to apply on the data.
         verbose: If >0, prints details about the execution on the standard error
             output. The larger the number, the more information is displayed.
         check_execution: If `True`, data of the intermediate results of the
             operators is checked against its expected structure and raises if
             it differs.
     """
     data = {**inputs}
 
-    num_operators = len(schedule.ordered_operators)
-    for operator_idx, operator in enumerate(schedule.ordered_operators):
-        operator_def = operator.definition()
+    num_steps = len(schedule.steps)
+    for step_idx, step in enumerate(schedule.steps):
+        operator_def = step.op.definition()
 
         # Get implementation
         implementation_cls = implementation_lib.get_implementation_class(
             operator_def.key
         )
 
         # Instantiate implementation
-        implementation = implementation_cls(operator)
+        implementation = implementation_cls(step.op)
 
         if verbose == 1:
             print(
-                (
-                    f"    {operator_idx+1} / {num_operators}:"
-                    f" {operator.operator_key()}"
-                ),
+                f"    {step_idx+1} / {num_steps}: {step.op.operator_key()}",
                 file=sys.stderr,
                 end="",
             )
         elif verbose >= 2:
             print("=============================", file=sys.stderr)
             print(
-                f"{operator_idx+1} / {num_operators}: Run {operator}",
+                f"{step_idx+1} / {num_steps}: Run {step.op}",
                 file=sys.stderr,
             )
 
         # Construct operator inputs
         operator_inputs = {
             input_key: data[input_node]
-            for input_key, input_node in operator.inputs.items()
+            for input_key, input_node in step.op.inputs.items()
         }
 
         if verbose >= 2:
             print(f"Inputs:\n{operator_inputs}\n", file=sys.stderr)
 
         # Compute output
         begin_time = time.perf_counter()
@@ -93,13 +91,18 @@
         if verbose == 1:
             print(f" [{end_time - begin_time:.5f} s]", file=sys.stderr)
         elif verbose >= 2:
             print(f"Outputs:\n{operator_outputs}\n", file=sys.stderr)
             print(f"Duration: {end_time - begin_time} s", file=sys.stderr)
 
         # materialize data in output nodes
-        for output_key, output_node in operator.outputs.items():
-            data[output_node] = operator_outputs[output_key]
+        for output_key, output_node in step.op.outputs.items():
+            output_evset = operator_outputs[output_key]
+            output_evset._internal_node = output_node
+            data[output_node] = output_evset
+
+        # Release unused memory
+        for node in step.released_nodes:
+            assert node in data
+            del data[node]
 
-    # TODO: Only return the required data.
-    # TODO: Un-allocate not used anymore object.
     return data
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/implementation_lib.py` & `temporian-0.1.2/temporian/implementation/numpy/implementation_lib.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/operators/BUILD`

 * *Files 14% similar despite different names*

```diff
@@ -12,25 +12,28 @@
     srcs_version = "PY3",
     deps = [
         ":add_index",
         ":begin",
         ":cast",
         ":drop_index",
         ":end",
+        ":enumerate",
         ":filter",
         ":glue",
+        ":join",
         ":lag",
         ":leak",
         ":prefix",
         ":propagate",
         ":rename",
         ":resample",
         ":select",
         ":since_last",
         ":tick",
+        ":timestamps",
         ":unary",
         ":unique_timestamps",
         "//temporian/implementation/numpy/operators/binary:arithmetic",
         "//temporian/implementation/numpy/operators/binary:logical",
         "//temporian/implementation/numpy/operators/binary:relational",
         "//temporian/implementation/numpy/operators/calendar:day_of_month",
         "//temporian/implementation/numpy/operators/calendar:day_of_week",
@@ -52,15 +55,22 @@
     ],
 )
 
 py_library(
     name = "base",
     srcs = ["base.py"],
     srcs_version = "PY3",
-    deps = ["//temporian/utils:config"],
+    deps = [
+        # already_there/numpy
+        "//temporian/utils:config",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/core/data:schema",
+        "//temporian/core/data:node",
+        "//temporian/core/operators:base",
+    ],
 )
 
 py_library(
     name = "filter",
     srcs = ["filter.py"],
     srcs_version = "PY3",
     deps = [
@@ -182,15 +192,15 @@
 
 py_library(
     name = "resample",
     srcs = ["resample.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/data:duration_utils",
+        # already_there/numpy
         "//temporian/core/operators:resample",
         "//temporian/implementation/numpy:implementation_lib",
         "//temporian/implementation/numpy/data:event_set",
         "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
@@ -211,29 +221,29 @@
 py_library(
     name = "cast",
     srcs = ["cast.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
         # already_there/numpy
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/operators:cast",
         "//temporian/implementation/numpy:implementation_lib",
         "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
     name = "unary",
     srcs = ["unary.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
         # already_there/numpy
-        "//temporian/core/operators/unary",
+        "//temporian/core/operators:unary",
         "//temporian/implementation/numpy:implementation_lib",
         "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
     name = "unique_timestamps",
@@ -251,44 +261,77 @@
 py_library(
     name = "begin",
     srcs = ["begin.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/numpy
         ":base",
-        "//temporian/core/data:duration_utils",
         "//temporian/core/operators:begin",
         "//temporian/implementation/numpy:implementation_lib",
-        "//temporian/implementation/numpy:utils",
         "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
     name = "end",
     srcs = ["end.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/numpy
         ":base",
-        "//temporian/core/data:duration_utils",
         "//temporian/core/operators:end",
         "//temporian/implementation/numpy:implementation_lib",
-        "//temporian/implementation/numpy:utils",
         "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
     name = "tick",
     srcs = ["tick.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/numpy
         ":base",
-        "//temporian/core/data:duration",
         "//temporian/core/operators:tick",
         "//temporian/implementation/numpy:implementation_lib",
-        "//temporian/implementation/numpy:utils",
+        "//temporian/implementation/numpy/data:event_set",
+    ],
+)
+
+py_library(
+    name = "join",
+    srcs = ["join.py"],
+    deps = [
+        # already_there/numpy
+        ":base",
+        "//temporian/core/operators:join",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
+    ],
+)
+
+py_library(
+    name = "timestamps",
+    srcs = ["timestamps.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/numpy
+        ":base",
+        "//temporian/core/operators:timestamps",
+        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy/data:event_set",
+    ],
+)
+
+py_library(
+    name = "enumerate",
+    srcs = ["enumerate.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/numpy
+        ":base",
+        "//temporian/core/operators:enumerate",
+        "//temporian/implementation/numpy:implementation_lib",
         "//temporian/implementation/numpy/data:event_set",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/add_index.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/add_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,42 +16,41 @@
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, AddIndexOperator)
         output_node = self.operator.outputs["output"]
 
         # Idx of input features added to index.
         src_feature_names = input.schema.feature_names()
         new_index_idxs = [
-            src_feature_names.index(f_name)
-            for f_name in self.operator.index_to_add
+            src_feature_names.index(f_name) for f_name in self.operator.indexes
         ]
 
         # Idx of input features not added to index.
         kept_feature_idxs = [
             idx
             for idx, f_name in enumerate(src_feature_names)
-            if f_name not in self.operator.index_to_add
+            if f_name not in self.operator.indexes
         ]
 
         dst_data = {}
         for src_index, src_data in input.data.items():
-            # Maps, for each new index value, the indices of the events in
+            # Maps, for each new index key, the indices of the events in
             # src_data.
             #
             # TODO: Do more efficiently. E.g. with numpy masks.
 
             new_index_to_value_idxs = defaultdict(list)
             # TODO: This is slow. Speed-up.
             for event_idx, new_index in enumerate(
                 zip(*[src_data.features[f_idx] for f_idx in new_index_idxs])
             ):
                 new_index = tuple(new_index)
                 new_index_to_value_idxs[new_index].append(event_idx)
 
             for new_index, example_idxs in new_index_to_value_idxs.items():
-                # Note: The new index is added after the existing index items.
+                # Note: The new indexes added after the existing ones.
                 dst_index = src_index + new_index
                 assert isinstance(dst_index, tuple)
 
                 dst_data[dst_index] = IndexData(
                     features=[
                         src_data.features[f_idx][example_idxs]
                         for f_idx in kept_feature_idxs
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/base.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Tuple
 
 from temporian.utils import config
-from temporian.core.data.node import Node
+from temporian.core.data.node import EventSetNode
 from temporian.core.data.schema import Schema
 from temporian.core.operators.base import Operator
 from temporian.core.operators.base import OperatorExceptionDecorator
 from temporian.implementation.numpy.data.event_set import (
     EventSet,
     numpy_array_to_tp_dtype,
 )
+import numpy as np
 
 
 class OperatorImplementation(ABC):
     def __init__(self, operator: Operator):
         assert operator is not None
         self._operator = operator
         # TODO: Check operator type
@@ -33,35 +34,44 @@
     @abstractmethod
     def __call__(self, **inputs: EventSet) -> Dict[str, EventSet]:
         """Applies the operator to its inputs."""
 
     def output_schema(self, key: str) -> Schema:
         return self._operator.outputs[key].schema
 
+    def apply_feature_wise(
+        self,
+        src_timestamps: np.ndarray,
+        src_feature: np.ndarray,
+    ) -> np.ndarray:
+        """Executes the op on a single feature. Optionally implemented."""
+
+        raise NotImplementedError()
+
 
 def _check_value_to_schema(
     values: Dict[str, EventSet],
-    nodes: Dict[str, Node],
+    nodes: Dict[str, EventSetNode],
     label: str,
 ) -> None:
-    """Checks if event sets are matching the expected schema."""
+    """Checks if EventSets are matching the expected schema."""
 
     for key, node in nodes.items():
         value = values[key]
 
         if value.schema != node.schema:
             raise RuntimeError(
-                "Unexpected event set schema.\n"
-                f"event set schema =\n{value.schema}\n"
+                "Unexpected EventSet set schema.\n"
+                f"actual schema =\n{value.schema}\n"
                 f"expected schema =\n{node.schema}"
             )
 
-        index_value = value.get_arbitrary_index_value()
-        if index_value is not None:
-            index_data = value.data[index_value]
+        index_key = value.get_arbitrary_index_key()
+        if index_key is not None:
+            index_data = value.data[index_key]
 
             if len(index_data.features) != len(value.schema.features):
                 raise RuntimeError(
                     "Invalid internal number of input features for argument"
                     f" {label!r}.\nexpected ="
                     f" {len(value.schema.features)}\neffective ="
                     f" {len(index_data.features)}.\n\nSchema:\n{value.schema}"
@@ -150,38 +160,38 @@
                         f" generated during the op execution ({input} vs"
                         f" {output}). Reason: {reason}"
                     )
 
 
 def _is_same_sampling(evset_1: EventSet, evset_2: EventSet) -> Tuple[bool, str]:
     if evset_1.schema.indexes != evset_2.schema.indexes:
-        return (False, "Different index names")
+        return (False, "Different indexes")
 
-    # Number of index values where to ensure that the numpy array containing
+    # Number of index keys to ensure that the numpy array containing
     # timestamps is the same for both evset_1 and evset_2.
     num_checks = 1 if config.DEBUG_MODE else len(evset_1.data)
 
     for i, (index_key, index_data_1) in enumerate(evset_1.data.items()):
         if i >= num_checks:
             break
 
         if index_key not in evset_2.data:
             return (
                 False,
                 (
-                    f"Index {index_key} missing from one of the two event sets."
+                    f"Index {index_key} missing from one of the two EventSets."
                     f" When comparing {evset_1} with {evset_2}"
                 ),
             )
         index_data_2 = evset_2.data[index_key]
         if index_data_1.timestamps is not index_data_2.timestamps:
             return (
                 False,
                 (
-                    f"Timestamps for index value {index_key} have two different"
+                    f"Timestamps for index key {index_key} have two different"
                     " allocated np.arrays."
                 ),
             )
 
     if config.DEBUG_MODE:
         # Compare index keys.
         # TODO: is there a way to avoid checking all keys here (keys might come
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/begin.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/begin.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,29 +30,33 @@
         assert isinstance(operator, BeginOperator)
         super().__init__(operator)
 
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, BeginOperator)
         output_schema = self.output_schema("output")
 
-        # create output event set
+        # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
 
-        # fill output event set data
+        # fill output EventSet data
         for index_key, index_data in input.data.items():
             if len(index_data.timestamps) == 0:
                 dst_timestamps = np.array([], dtype=np.float64)
             else:
                 dst_timestamps = np.array(
                     [index_data.timestamps[0]], dtype=np.float64
                 )
-            output_evset[index_key] = IndexData(
-                [],
-                dst_timestamps,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [],
+                    dst_timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     BeginOperator, BeginNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/binary/BUILD` & `temporian-0.1.2/temporian/core/BUILD`

 * *Files 25% similar despite different names*

```diff
@@ -3,65 +3,79 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "binary",
-    srcs = ["__init__.py"],
+    name = "evaluation",
+    srcs = ["evaluation.py"],
     srcs_version = "PY3",
     deps = [
-        ":arithmetic",
-        ":logical",
-        ":relational",
+        ":graph",
+        ":schedule",
+        "//temporian/core/data:node",
+        "//temporian/core/operators:base",
+        "//temporian/core/operators:leak",
+        "//temporian/implementation/numpy:evaluation",
+        "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
-    name = "base",
-    srcs = ["base.py"],
+    name = "operator_lib",
+    srcs = ["operator_lib.py"],
+    srcs_version = "PY3",
+)
+
+py_library(
+    name = "schedule",
+    srcs = ["schedule.py"],
     srcs_version = "PY3",
     deps = [
-        # already_there/numpy
-        "//temporian/core/operators/binary:base",
-        "//temporian/implementation/numpy/data:event_set",
-        "//temporian/implementation/numpy/operators:base",
+        "//temporian/core/data:node",
+        "//temporian/core/operators:base",
     ],
 )
 
 py_library(
-    name = "arithmetic",
-    srcs = ["arithmetic.py"],
+    name = "graph",
+    srcs = ["graph.py"],
     srcs_version = "PY3",
     deps = [
-        ":base",
-        # already_there/numpy
-        "//temporian/core/data/dtypes:dtype",
-        "//temporian/core/operators/binary",
-        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/core/data:node",
+        "//temporian/core/operators:base",
     ],
 )
 
 py_library(
-    name = "relational",
-    srcs = ["relational.py"],
+    name = "serialization",
+    srcs = ["serialization.py"],
     srcs_version = "PY3",
     deps = [
-        ":base",
-        # already_there/numpy
-        "//temporian/core/operators/binary",
-        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/core:graph",
+        "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+        "//temporian/core/operators:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/proto:core_py_proto",
     ],
 )
 
 py_library(
-    name = "logical",
-    srcs = ["logical.py"],
+    name = "compilation",
+    srcs = ["compilation.py"],
     srcs_version = "PY3",
     deps = [
-        ":base",
-        # already_there/numpy
-        "//temporian/core/operators/binary",
-        "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/core/data:node",
+        "//temporian/implementation/numpy/data:event_set",
     ],
 )
+
+py_library(
+    name = "mixins",
+    srcs = ["mixins.py"],
+    srcs_version = "PY3",
+    deps = [],
+)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/binary/__init__.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/binary/arithmetic.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/binary/arithmetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,78 +9,91 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
 
+from temporian.core.data.dtype import DType
 from temporian.core.operators.binary import (
     AddOperator,
     SubtractOperator,
     MultiplyOperator,
     DivideOperator,
     FloorDivOperator,
     ModuloOperator,
     PowerOperator,
 )
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.binary.base import (
     BaseBinaryNumpyImplementation,
 )
 
 
 class AddNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of add operator."""
 
     def __init__(self, operator: AddOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, AddOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return evset_1_feature + evset_2_feature
 
 
 class SubtractNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the subtract operator."""
 
     def __init__(self, operator: SubtractOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, SubtractOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return evset_1_feature - evset_2_feature
 
 
 class MultiplyNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the multiply operator."""
 
     def __init__(self, operator: MultiplyOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, MultiplyOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return evset_1_feature * evset_2_feature
 
 
 class DivideNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the divide operator."""
 
     def __init__(self, operator: DivideOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, DivideOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         if evset_1_feature.dtype in [DType.INT32, DType.INT64]:
             raise ValueError(
                 "Cannot use the divide operator on feature "
                 f"{evset_1_feature} of type {evset_1_feature.dtype.type}. "
                 "Cast to a floating point type or use "
                 "floordiv operator (//) instead, on these integer types."
@@ -92,41 +105,50 @@
     """Numpy implementation of the floordiv operator."""
 
     def __init__(self, operator: FloorDivOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, FloorDivOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return evset_1_feature // evset_2_feature
 
 
 class ModuloNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the modulo operator."""
 
     def __init__(self, operator: ModuloOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, ModuloOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return evset_1_feature % evset_2_feature
 
 
 class PowerNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the power operator."""
 
     def __init__(self, operator: PowerOperator) -> None:
         super().__init__(operator)
         assert isinstance(operator, PowerOperator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return evset_1_feature**evset_2_feature
 
 
 implementation_lib.register_operator_implementation(
     AddOperator, AddNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/binary/base.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/scalar/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,80 +7,69 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Dict
-from abc import abstractmethod
+from typing import Dict, Union
+from abc import ABC, abstractmethod
 
 import numpy as np
 
-from temporian.core.operators.binary.base import BaseBinaryOperator
-from temporian.implementation.numpy.data.event_set import IndexData
-from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.core.data.dtype import DType
+from temporian.core.operators.scalar.base import (
+    BaseScalarOperator,
+)
+from temporian.implementation.numpy.data.event_set import EventSet, IndexData
 from temporian.implementation.numpy.operators.base import OperatorImplementation
 
 
-class BaseBinaryNumpyImplementation(OperatorImplementation):
-    def __init__(self, operator: BaseBinaryOperator) -> None:
+class BaseScalarNumpyImplementation(OperatorImplementation, ABC):
+    def __init__(self, operator: BaseScalarOperator) -> None:
         super().__init__(operator)
-        assert isinstance(operator, BaseBinaryOperator)
 
     @abstractmethod
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         """Performs the arithmetic operation corresponding to the subclass."""
 
-    def __call__(
-        self, input_1: EventSet, input_2: EventSet
-    ) -> Dict[str, EventSet]:
-        """Applies the corresponding arithmetic operation between two event
-        sets.
+    def __call__(self, input: EventSet) -> Dict[str, EventSet]:
+        """Applies the corresponding arithmetic operation between an EventSet
+        and a scalar.
 
         Args:
-            input_1: First event set.
-            input_2: Second event set.
+            input: Event set to perform the operation to.
 
         Returns:
             Result of the operation.
-
-        Raises:
-            ValueError: If sampling of both event sets is not equal.
         """
-        assert isinstance(self.operator, BaseBinaryOperator)
-        output_schema = self.output_schema("output")
 
-        if len(input_1.schema.features) != len(input_2.schema.features):
-            raise ValueError(
-                "Both event sets must have the same number of features."
-            )
-        num_features = len(input_1.schema.features)
+        assert isinstance(self.operator, BaseScalarOperator)
+        output_schema = self.output_schema("output")
 
-        # create destination event set
         dst_evset = EventSet(data={}, schema=output_schema)
-
-        assert len(input_1.data) == len(input_2.data)
-
-        for index_key, index_data in input_1.data.items():
-            # iterate over index key features
-            input_1_features = index_data.features
-            input_2_features = input_2[index_key].features
-            dst_features = []
-
-            for feature_idx in range(num_features):
-                input_1_feature = input_1_features[feature_idx]
-                input_2_feature = input_2_features[feature_idx]
-                assert input_1_feature.dtype.type == input_2_feature.dtype.type
-
-                result = self._do_operation(input_1_feature, input_2_feature)
-                dst_features.append(result)
-
-            dst_evset[index_key] = IndexData(
-                features=dst_features,
-                timestamps=index_data.timestamps,
-                schema=output_schema,
+        for index_key, index_data in input.data.items():
+            dst_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [
+                        self._do_operation(
+                            feature,
+                            self.operator.value,
+                            input.schema.features[feature_idx].dtype,
+                        )
+                        for feature_idx, feature in enumerate(
+                            index_data.features
+                        )
+                    ],
+                    index_data.timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": dst_evset}
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/binary/logical.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/binary/logical.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
+
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy.operators.binary.base import (
     BaseBinaryNumpyImplementation,
 )
 from temporian.core.operators.binary import (
     LogicalAndOperator,
     LogicalOrOperator,
     LogicalXorOperator,
@@ -26,39 +28,48 @@
 class LogicalAndNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the logical AND operator."""
 
     def __init__(self, operator: LogicalAndOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.logical_and(evset_1_feature.data, evset_2_feature.data)
 
 
 class LogicalOrNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the logical OR operator."""
 
     def __init__(self, operator: LogicalOrOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.logical_or(evset_1_feature.data, evset_2_feature.data)
 
 
 class LogicalXorNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the logical XOR operator."""
 
     def __init__(self, operator: LogicalXorOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.logical_xor(evset_1_feature.data, evset_2_feature.data)
 
 
 implementation_lib.register_operator_implementation(
     LogicalAndOperator, LogicalAndNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/binary/relational.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/binary/relational.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
+
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy.operators.binary.base import (
     BaseBinaryNumpyImplementation,
 )
 from temporian.core.operators.binary import (
     EqualOperator,
     NotEqualOperator,
     GreaterOperator,
@@ -29,66 +31,90 @@
 class EqualNumpyImplementation(BaseBinaryNumpyImplementation):
     """Numpy implementation of the equal operator."""
 
     def __init__(self, operator: EqualOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
-    ) -> np.ndarray:
-        # returns False on both NaNs
-        return np.equal(evset_1_feature.data, evset_2_feature.data)
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
+    ) -> np.ndarray:
+        if dtype == DType.STRING:
+            return np.char.equal(evset_1_feature.data, evset_2_feature.data)
+        else:
+            # returns False on both NaNs
+            return np.equal(evset_1_feature.data, evset_2_feature.data)
 
 
 class NotEqualNumpyImplementation(BaseBinaryNumpyImplementation):
     def __init__(self, operator: EqualOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
-    ) -> np.ndarray:
-        return np.not_equal(evset_1_feature.data, evset_2_feature.data)
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
+    ) -> np.ndarray:
+        if dtype == DType.STRING:
+            return np.char.not_equal(evset_1_feature.data, evset_2_feature.data)
+        else:
+            return np.not_equal(evset_1_feature.data, evset_2_feature.data)
 
 
 class GreaterNumpyImplementation(BaseBinaryNumpyImplementation):
     def __init__(self, operator: EqualOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.greater(evset_1_feature.data, evset_2_feature.data)
 
 
 class GreaterEqualNumpyImplementation(BaseBinaryNumpyImplementation):
     def __init__(self, operator: EqualOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.greater_equal(evset_1_feature.data, evset_2_feature.data)
 
 
 class LessNumpyImplementation(BaseBinaryNumpyImplementation):
     def __init__(self, operator: EqualOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.less(evset_1_feature.data, evset_2_feature.data)
 
 
 class LessEqualNumpyImplementation(BaseBinaryNumpyImplementation):
     def __init__(self, operator: EqualOperator) -> None:
         super().__init__(operator)
 
     def _do_operation(
-        self, evset_1_feature: np.ndarray, evset_2_feature: np.ndarray
+        self,
+        evset_1_feature: np.ndarray,
+        evset_2_feature: np.ndarray,
+        dtype: DType,
     ) -> np.ndarray:
         return np.less_equal(evset_1_feature.data, evset_2_feature.data)
 
 
 implementation_lib.register_operator_implementation(
     EqualOperator, EqualNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/BUILD` & `temporian-0.1.2/temporian/beam/BUILD`

 * *Files 24% similar despite different names*

```diff
@@ -3,122 +3,48 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "calendar",
+    name = "beam",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
-)
-
-py_library(
-    name = "base",
-    srcs = ["base.py"],
-    srcs_version = "PY3",
-    deps = [
-        # already_there/numpy
-        "//temporian/core/operators/calendar:base",
-        "//temporian/implementation/numpy/data:event_set",
-        "//temporian/implementation/numpy/operators:base",
-    ],
-)
-
-py_library(
-    name = "day_of_month",
-    srcs = ["day_of_month.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:day_of_month",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "day_of_week",
-    srcs = ["day_of_week.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:day_of_week",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "day_of_year",
-    srcs = ["day_of_year.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:day_of_year",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "hour",
-    srcs = ["hour.py"],
-    srcs_version = "PY3",
     deps = [
-        ":base",
-        "//temporian/core/operators/calendar:hour",
-        "//temporian/implementation/numpy:implementation_lib",
+        ":evaluation",
+        ":io",
     ],
 )
 
 py_library(
-    name = "iso_week",
-    srcs = ["iso_week.py"],
+    name = "io",
+    srcs = ["io.py"],
     srcs_version = "PY3",
     deps = [
-        ":base",
-        "//temporian/core/operators/calendar:iso_week",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "minute",
-    srcs = ["minute.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:minute",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "month",
-    srcs = ["month.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:month",
-        "//temporian/implementation/numpy:implementation_lib",
+        # already_there/apache_beam
+        # already_there/numpy
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
     ],
 )
 
 py_library(
-    name = "second",
-    srcs = ["second.py"],
+    name = "evaluation",
+    srcs = ["evaluation.py"],
     srcs_version = "PY3",
     deps = [
-        ":base",
-        "//temporian/core/operators/calendar:second",
-        "//temporian/implementation/numpy:implementation_lib",
+        # already_there/apache_beam
+        "//temporian/core:evaluation",
+        "//temporian/beam:io",
+        ":implementation_lib",
+        "//temporian/beam/operators",
+        "//temporian/core/data:node",
     ],
 )
 
 py_library(
-    name = "year",
-    srcs = ["year.py"],
+    name = "implementation_lib",
+    srcs = ["implementation_lib.py"],
     srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:year",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/base.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,30 +31,32 @@
         super().__init__(operator)
         assert isinstance(operator, BaseCalendarOperator)
 
     def __call__(self, sampling: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, BaseCalendarOperator)
         output_schema = self.output_schema("output")
 
-        # create destination event set
+        # create destination EventSet
         dst_evset = EventSet(data={}, schema=output_schema)
         for index_key, index_data in sampling.data.items():
             value = np.array(
                 [
                     self._get_value_from_datetime(
                         datetime.fromtimestamp(ts, tz=timezone.utc)
                     )
                     for ts in index_data.timestamps
                 ]
             ).astype(
                 np.int32
             )  # TODO: parametrize output dtype
 
-            dst_evset[index_key] = IndexData(
-                [value], index_data.timestamps, schema=output_schema
+            dst_evset.set_index_value(
+                index_key,
+                IndexData([value], index_data.timestamps, schema=output_schema),
+                normalize=False,
             )
 
         return {"output": dst_evset}
 
     @abstractmethod
     def _get_value_from_datetime(self, dt: datetime) -> Any:
         """Gets the value of the datetime object that corresponds to each
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/day_of_month.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/day_of_month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/day_of_week.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/day_of_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/day_of_year.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/day_of_year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/hour.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/month.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 from datetime import datetime
 
-from temporian.core.operators.calendar.hour import (
-    CalendarHourOperator,
+from temporian.core.operators.calendar.month import (
+    CalendarMonthOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.calendar.base import (
     BaseCalendarNumpyImplementation,
 )
 
 
-class CalendarHourNumpyImplementation(BaseCalendarNumpyImplementation):
-    """Numpy implementation of the calendar_hour operator."""
+class CalendarMonthNumpyImplementation(BaseCalendarNumpyImplementation):
+    """Numpy implementation of the calendar_month operator."""
 
-    def __init__(self, operator: CalendarHourOperator) -> None:
+    def __init__(self, operator: CalendarMonthOperator) -> None:
         super().__init__(operator)
 
     def _get_value_from_datetime(self, dt: datetime) -> Any:
-        return dt.hour
+        return dt.month
 
 
 implementation_lib.register_operator_implementation(
-    CalendarHourOperator, CalendarHourNumpyImplementation
+    CalendarMonthOperator, CalendarMonthNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/iso_week.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/iso_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/minute.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/minute.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/month.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/year.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 from datetime import datetime
 
-from temporian.core.operators.calendar.month import (
-    CalendarMonthOperator,
+from temporian.core.operators.calendar.year import (
+    CalendarYearOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.calendar.base import (
     BaseCalendarNumpyImplementation,
 )
 
 
-class CalendarMonthNumpyImplementation(BaseCalendarNumpyImplementation):
-    """Numpy implementation of the calendar_month operator."""
+class CalendarYearNumpyImplementation(BaseCalendarNumpyImplementation):
+    """Numpy implementation of the calendar_year operator."""
 
-    def __init__(self, operator: CalendarMonthOperator) -> None:
+    def __init__(self, operator: CalendarYearOperator) -> None:
         super().__init__(operator)
 
     def _get_value_from_datetime(self, dt: datetime) -> Any:
-        return dt.month
+        return dt.year
 
 
 implementation_lib.register_operator_implementation(
-    CalendarMonthOperator, CalendarMonthNumpyImplementation
+    CalendarYearOperator, CalendarYearNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/second.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/calendar/second.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/calendar/year.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_count.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,32 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any
-from datetime import datetime
 
-from temporian.core.operators.calendar.year import (
-    CalendarYearOperator,
+from temporian.core.operators.window.moving_count import (
+    MovingCountOperator,
 )
 from temporian.implementation.numpy import implementation_lib
-from temporian.implementation.numpy.operators.calendar.base import (
-    BaseCalendarNumpyImplementation,
+from temporian.implementation.numpy.operators.window.base import (
+    BaseWindowNumpyImplementation,
 )
+from temporian.implementation.numpy_cc.operators import operators_cc
 
 
-class CalendarYearNumpyImplementation(BaseCalendarNumpyImplementation):
-    """Numpy implementation of the calendar_year operator."""
+class MovingCountNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the moving count operator."""
 
-    def __init__(self, operator: CalendarYearOperator) -> None:
-        super().__init__(operator)
-
-    def _get_value_from_datetime(self, dt: datetime) -> Any:
-        return dt.year
+    def _implementation(self):
+        return operators_cc.moving_count
 
 
 implementation_lib.register_operator_implementation(
-    CalendarYearOperator, CalendarYearNumpyImplementation
+    MovingCountOperator, MovingCountNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/cast.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/cast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Tuple, List, Optional, Any
 
 import numpy as np
 
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.operators.cast import CastOperator
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.data.event_set import (
     EventSet,
     IndexData,
     tp_dtype_to_np_dtype,
 )
@@ -103,18 +103,22 @@
                         src_schema.dtype,
                         dst_schema.dtype,
                         src_schema.name,
                         min_max,
                     )
                 dst_features.append(src_values.astype(np_dtype))
 
-            output_evset[index_key] = IndexData(
-                features=dst_features,
-                timestamps=index_data.timestamps,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    features=dst_features,
+                    timestamps=index_data.timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     CastOperator, CastNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/drop_index.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/drop_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,37 +27,37 @@
 
         src_index_names = input.schema.index_names()
 
         # Idx in src_index_names of the indexes to keep in the output.
         final_index_idxs = [
             idx
             for idx, f_name in enumerate(src_index_names)
-            if f_name not in self.operator.index_to_drop
+            if f_name not in self.operator.indexes
         ]
         # Idx in src_index_names of the indexes to remove in the output.
         final_nonindex_idxs = [
             idx
             for idx, f_name in enumerate(src_index_names)
-            if f_name in self.operator.index_to_drop
+            if f_name in self.operator.indexes
         ]
         # Non-aggregated (i.e., in separate containers) event data indexed by
         # the destination index.
         dst_index_groups: Dict[tuple, DstIndexGroup] = defaultdict(
             DstIndexGroup
         )
         # Compute "dst_index_groups".
         for src_index_key, src_index_data in input.data.items():
             new_features_data = []
             if self.operator.keep:
                 # Convert the dropped indexes into features
                 num_timestamps = len(src_index_data.timestamps)
                 for idx in final_nonindex_idxs:
-                    index_value = src_index_key[idx]
+                    index_key = src_index_key[idx]
                     new_feature_data = np.full(
-                        shape=num_timestamps, fill_value=index_value
+                        shape=num_timestamps, fill_value=index_key
                     )
                     new_features_data.append(new_feature_data)
 
             dst_index_key = tuple((src_index_key[i] for i in final_index_idxs))
             dst_index_group = dst_index_groups[dst_index_key]
             dst_index_group.timestamps.append(src_index_data.timestamps)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/end.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/end.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,29 +30,33 @@
         assert isinstance(operator, EndOperator)
         super().__init__(operator)
 
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, EndOperator)
         output_schema = self.output_schema("output")
 
-        # create output event set
+        # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
 
-        # fill output event set data
+        # fill output EventSet data
         for index_key, index_data in input.data.items():
             if len(index_data.timestamps) == 0:
                 dst_timestamps = np.array([], dtype=np.float64)
             else:
                 dst_timestamps = np.array(
                     [index_data.timestamps[-1]], dtype=np.float64
                 )
-            output_evset[index_key] = IndexData(
-                [],
-                dst_timestamps,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [],
+                    dst_timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     EndOperator, EndNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/filter.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,28 @@
         output_schema = self.output_schema("output")
 
         output_evset = EventSet(data={}, schema=output_schema)
         for condition_index, condition_data in condition.data.items():
             # get boolean mask from condition
             mask = condition_data.features[0]
 
-            src_event = input[condition_index]
+            src_event = input.data[condition_index]
 
             filtered_timestamps = src_event.timestamps[mask]
 
             filtered_features = [
                 feature_data[mask] for feature_data in src_event.features
             ]
 
-            output_evset[condition_index] = IndexData(
-                filtered_features, filtered_timestamps, schema=output_schema
+            output_evset.set_index_value(
+                condition_index,
+                IndexData(
+                    filtered_features, filtered_timestamps, schema=output_schema
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     FilterOperator, FilterNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/glue.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/glue.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,27 +38,31 @@
 
         # convert input evest dict to list of evsets
         evsets: List[EventSet] = list(
             list(zip(*sorted(list(inputs.items()))))[1]
         )
         if len(evsets) < 2:
             raise ValueError(
-                f"Glue operator cannot be called on a {len(evsets)} event sets."
+                f"Glue operator cannot be called on a {len(evsets)} EventSets."
             )
 
         dst_evset = EventSet(data={}, schema=output_schema)
         for index_key, index_data in evsets[0].data.items():
             features = []
             for evset in evsets:
                 features.extend(evset.data[index_key].features)
 
-            dst_evset[index_key] = IndexData(
-                timestamps=index_data.timestamps,
-                features=features,
-                schema=output_schema,
+            dst_evset.set_index_value(
+                index_key,
+                IndexData(
+                    timestamps=index_data.timestamps,
+                    features=features,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": dst_evset}
 
 
 implementation_lib.register_operator_implementation(
     GlueOperator, GlueNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/lag.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/lag.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,23 +28,27 @@
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, LagOperator)
         output_schema = self.output_schema("output")
 
         # gather operator attributes
         duration = self.operator.duration
 
-        # create output event set
+        # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
 
-        # fill output event set data
+        # fill output EventSet data
         for index_key, index_data in input.data.items():
-            output_evset[index_key] = IndexData(
-                index_data.features,
-                index_data.timestamps + duration,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    index_data.features,
+                    index_data.timestamps + duration,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     LagOperator, LagNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/leak.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/leak.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,26 @@
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, LeakOperator)
         output_schema = self.output_schema("output")
 
         # gather operator attributes
         duration = self.operator.duration
 
-        # create output event set
+        # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
-        # fill output event set data
+        # fill output EventSet data
         for index_key, index_data in input.data.items():
-            output_evset[index_key] = IndexData(
-                index_data.features,
-                index_data.timestamps - duration,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    index_data.features,
+                    index_data.timestamps - duration,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     LeakOperator, LeakNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/prefix.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/prefix.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/propagate.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/propagate.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ) -> Dict[str, EventSet]:
         assert isinstance(self.operator, Propagate)
         output_schema = self.output_schema("output")
 
         dst_data = {}
 
         for sampling_index in sampling.data:
-            # Compute the event set index
+            # Compute the EventSet's index
             src_index = tuple(
                 [sampling_index[i] for i in self.operator.index_mapping]
             )
 
             # Find the source data
             if src_index not in input.data:
                 # TODO: Add option to skip non matched indexes.
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/rename.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/rename.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
         # rename index
         new_index_names = [
             index.get(index_name, index_name)
             for index_name in input.schema.index_names()
         ]
 
-        # check that after renaming everything there are no common values
-        # between index names and feature names
+        # check that after renaming everything there are no common names
+        # between indexes and features
         if set(new_feature_names).intersection(set(new_index_names)):
             raise ValueError(
                 "Index names and feature names must be unique. Got"
                 f" {new_feature_names} and {new_index_names}."
             )
 
         # create output evset
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/resample.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/resample.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,23 +45,27 @@
         output_missing_and_np_dtypes = [
             (
                 f.dtype.missing_value(),
                 tp_dtype_to_np_dtype(f.dtype),
             )
             for f in output_schema.features
         ]
-        # create output event set
+        # create output EventSet
         dst_evset = EventSet(data={}, schema=output_schema)
         # iterate over destination sampling
         for index_key, index_data in sampling.data.items():
-            # intialize destination index data
+            # initialize destination index data
             dst_mts = []
 
             index_data = IndexData(dst_mts, index_data.timestamps, schema=None)
-            dst_evset[index_key] = index_data
+            dst_evset.set_index_value(
+                index_key,
+                index_data,
+                normalize=False,
+            )
 
             if index_key not in input.data:
                 # No matching events to sample from
                 for (
                     output_missing_value,
                     output_np_dtype,
                 ) in output_missing_and_np_dtypes:
@@ -71,16 +75,16 @@
                             fill_value=output_missing_value,
                             dtype=output_np_dtype,
                         )
                     )
                 index_data.check_schema(output_schema)
                 continue
 
-            src_mts = input[index_key].features
-            src_timestamps = input[index_key].timestamps
+            src_mts = input.data[index_key].features
+            src_timestamps = input.data[index_key].timestamps
             (
                 sampling_idxs,
                 first_valid_idx,
             ) = operators_cc.build_sampling_idxs(
                 src_timestamps, index_data.timestamps
             )
             # For each feature
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/scalar/__init__.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union
 
 import numpy as np
 
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy.operators.scalar.base import (
     BaseScalarNumpyImplementation,
 )
 from temporian.core.operators.scalar import (
     AddScalarOperator,
     SubtractScalarOperator,
     MultiplyScalarOperator,
@@ -30,80 +31,101 @@
 from temporian.implementation.numpy import implementation_lib
 
 
 class AddScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the add scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         return feature + value
 
 
 class SubtractScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the subtract scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         if self._operator.is_value_first:
             return value - feature
 
         return feature - value
 
 
 class MultiplyScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the multiply scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         return feature * value
 
 
 class DivideScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the divide scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         if self._operator.is_value_first:
             return value / feature
 
         return feature / value
 
 
 class FloorDivideScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the floordiv scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         if self._operator.is_value_first:
             return value // feature
 
         return feature // value
 
 
 class ModuloScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the modulo scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         if self._operator.is_value_first:
             return value % feature
         return feature % value
 
 
 class PowerScalarNumpyImplementation(BaseScalarNumpyImplementation):
     """Numpy implementation of the power scalar operator."""
 
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         if self._operator.is_value_first:
             return value**feature
         return feature**value
 
 
 implementation_lib.register_operator_implementation(
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/scalar/base.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/enumerate.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,55 +7,52 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Dict, Union
-from abc import ABC, abstractmethod
 
+
+"""Implementation for the Enumerate operator."""
+
+
+from typing import Dict
 import numpy as np
 
-from temporian.core.operators.scalar.base import (
-    BaseScalarOperator,
-)
-from temporian.implementation.numpy.data.event_set import EventSet, IndexData
+from temporian.implementation.numpy.data.event_set import IndexData, EventSet
+from temporian.core.operators.enumerate import Enumerate
+from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.base import OperatorImplementation
 
 
-class BaseScalarNumpyImplementation(OperatorImplementation, ABC):
-    def __init__(self, operator: BaseScalarOperator) -> None:
+class EnumerateNumpyImplementation(OperatorImplementation):
+    def __init__(self, operator: Enumerate) -> None:
+        assert isinstance(operator, Enumerate)
         super().__init__(operator)
 
-    @abstractmethod
-    def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
-    ) -> np.ndarray:
-        """Performs the arithmetic operation corresponding to the subclass."""
-
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
-        """Applies the corresponding arithmetic operation between an event set
-        and a scalar.
-
-        Args:
-            input: Event set to perform the operation to.
+        assert isinstance(self.operator, Enumerate)
 
-        Returns:
-            Result of the operation.
-        """
-
-        assert isinstance(self.operator, BaseScalarOperator)
         output_schema = self.output_schema("output")
 
-        dst_evset = EventSet(data={}, schema=output_schema)
+        # Create output EventSet
+        output_evset = EventSet(data={}, schema=output_schema)
+
+        # Fill output EventSet's data
         for index_key, index_data in input.data.items():
-            dst_evset[index_key] = IndexData(
-                [
-                    self._do_operation(feature, self.operator.value)
-                    for feature in index_data.features
-                ],
-                index_data.timestamps,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [np.arange(len(index_data.timestamps), dtype=np.int64)],
+                    index_data.timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
-        return {"output": dst_evset}
+        return {"output": output_evset}
+
+
+implementation_lib.register_operator_implementation(
+    Enumerate, EnumerateNumpyImplementation
+)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/scalar/relational_scalar.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/scalar/relational_scalar.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union
 
 import numpy as np
 
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy.operators.scalar.base import (
     BaseScalarNumpyImplementation,
 )
 from temporian.core.operators.scalar import (
     EqualScalarOperator,
     NotEqualScalarOperator,
     GreaterEqualScalarOperator,
@@ -27,51 +28,75 @@
     LessScalarOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 
 
 class EqualScalarNumpyImplementation(BaseScalarNumpyImplementation):
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
-    ) -> np.ndarray:
-        # Returns False if both NaNs
-        return np.equal(feature, value)
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
+    ) -> np.ndarray:
+        if dtype == DType.STRING:
+            return np.char.equal(feature, value)
+        else:
+            # Returns False if both NaNs
+            return np.equal(feature, value)
 
 
 class NotEqualScalarNumpyImplementation(BaseScalarNumpyImplementation):
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
-    ) -> np.ndarray:
-        return np.not_equal(feature, value)
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
+    ) -> np.ndarray:
+        if dtype == DType.STRING:
+            return np.char.not_equal(feature, value)
+        else:
+            return np.not_equal(feature, value)
 
 
 class GreaterEqualScalarNumpyImplementation(BaseScalarNumpyImplementation):
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         return np.greater_equal(feature, value)
 
 
 class LessEqualScalarNumpyImplementation(BaseScalarNumpyImplementation):
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         return np.less_equal(feature, value)
 
 
 class GreaterScalarNumpyImplementation(BaseScalarNumpyImplementation):
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         return np.greater(feature, value)
 
 
 class LessScalarNumpyImplementation(BaseScalarNumpyImplementation):
     def _do_operation(
-        self, feature: np.ndarray, value: Union[float, int, str, bool]
+        self,
+        feature: np.ndarray,
+        value: Union[float, int, str, bool],
+        dtype: DType,
     ) -> np.ndarray:
         return np.less(feature, value)
 
 
 implementation_lib.register_operator_implementation(
     EqualScalarOperator, EqualScalarNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/select.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/select.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,22 +38,26 @@
 
         # get feature indexes to be selected
         src_feature_names = input.schema.feature_names()
         feature_idxs = [
             src_feature_names.index(feature_name)
             for feature_name in feature_names
         ]
-        # create output event set
+        # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
         # select feature index key-wise
         for index_key, index_data in input.data.items():
-            output_evset[index_key] = IndexData(
-                [index_data.features[idx] for idx in feature_idxs],
-                index_data.timestamps,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [index_data.features[idx] for idx in feature_idxs],
+                    index_data.timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     SelectOperator, SelectNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/since_last.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/since_last.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,35 +34,45 @@
         self, input: EventSet, sampling: Optional[EventSet] = None
     ) -> Dict[str, EventSet]:
         assert isinstance(self.operator, SinceLast)
 
         assert self.operator.has_sampling == (sampling is not None)
 
         output_schema = self.output_schema("output")
-        output_event = EventSet(data={}, schema=output_schema)
+        output_evset = EventSet(data={}, schema=output_schema)
 
         for index_key, index_data in input.data.items():
             if sampling is not None:
                 sampling_timestamps = sampling.data[index_key].timestamps
                 feature_values = operators_cc.since_last(
                     index_data.timestamps, sampling_timestamps
                 )
-                output_event[index_key] = IndexData(
-                    [feature_values], sampling_timestamps, schema=output_schema
+                output_evset.set_index_value(
+                    index_key,
+                    IndexData(
+                        [feature_values],
+                        sampling_timestamps,
+                        schema=output_schema,
+                    ),
+                    normalize=False,
                 )
             else:
                 # TODO: Avoid memory copy.
                 feature_values = np.concatenate(
                     [[np.nan], np.diff(index_data.timestamps)]
                 )
-                output_event[index_key] = IndexData(
-                    [feature_values],
-                    index_data.timestamps,
-                    schema=output_schema,
+                output_evset.set_index_value(
+                    index_key,
+                    IndexData(
+                        [feature_values],
+                        index_data.timestamps,
+                        schema=output_schema,
+                    ),
+                    normalize=False,
                 )
 
-        return {"output": output_event}
+        return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     SinceLast, SinceLastNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/BUILD` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/BUILD`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 )
 
 py_library(
     name = "test_util",
     srcs = ["test_util.py"],
     srcs_version = "PY3",
     deps = [
+        "//temporian/core:serialization",
         "//temporian/core/operators:base",
-        "//temporian/core/serialization:serialize",
         "//temporian/implementation/numpy/data:event_set",
         "//temporian/implementation/numpy/operators:base",
     ],
 )
 
 # Tests
 # =====
@@ -25,14 +25,15 @@
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         "//temporian/core/operators/binary",
         "//temporian/implementation/numpy/data:io",
         "//temporian/io:pandas",
         "//temporian/implementation/numpy/operators/binary",
+        ":test_util",
     ],
 )
 
 py_test(
     name = "relational_test",
     srcs = ["relational_test.py"],
     srcs_version = "PY3",
@@ -40,44 +41,46 @@
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         "//temporian/io:pandas",
         "//temporian/core/operators/binary",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/binary",
+        ":test_util",
     ],
 )
 
 py_test(
     name = "logical_test",
     srcs = ["logical_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         "//temporian/io:pandas",
         "//temporian/core/operators/binary",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/binary",
+        ":test_util",
     ],
 )
 
 py_test(
     name = "arithmetic_scalar_test",
     srcs = ["arithmetic_scalar_test.py"],
     srcs_version = "PY3",
     deps = [
-        ":test_util",
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         "//temporian/io:pandas",
         "//temporian/core/operators/scalar",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/scalar",
+        ":test_util",
     ],
 )
 
 py_test(
     name = "relational_scalar_test",
     srcs = ["relational_scalar_test.py"],
     srcs_version = "PY3",
@@ -85,48 +88,49 @@
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         "//temporian/io:pandas",
         "//temporian/core/operators/scalar",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/scalar",
+        ":test_util",
     ],
 )
 
 py_test(
     name = "arithmetic_multi_index_test",
     srcs = ["arithmetic_multi_index_test.py"],
     srcs_version = "PY3",
     deps = [
-        ":test_util",
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         # absl/testing:absltest dep,
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/io:pandas",
         "//temporian/core/operators/binary",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/binary",
+        ":test_util",
     ],
 )
 
 py_test(
     name = "cast_test",
     srcs = ["cast_test.py"],
     srcs_version = "PY3",
     deps = [
         ":test_util",
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         "//temporian/io:pandas",
         "//temporian/core:evaluation",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/operators:cast",
         "//temporian/implementation/numpy/data:event_set",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:cast",
     ],
 )
@@ -147,15 +151,15 @@
 py_test(
     name = "glue_test",
     srcs = ["glue_test.py"],
     srcs_version = "PY3",
     deps = [
         ":test_util",
         # already_there/absl/testing:absltest
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/operators:glue",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:glue",
     ],
 )
 
@@ -165,15 +169,15 @@
     srcs_version = "PY3",
     deps = [
         ":test_util",
         # already_there/absl/testing:absltest
         # already_there/numpy
         # already_there/pandas
         "//temporian/io:pandas",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:unary",
     ],
 )
 
 py_test(
@@ -417,15 +421,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators/window:simple_moving_average",
         "//temporian/implementation/numpy:evaluation",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/window:simple_moving_average",
     ],
@@ -437,15 +441,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators/window:moving_standard_deviation",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/window:moving_standard_deviation",
     ],
 )
@@ -456,15 +460,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators/window:moving_sum",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/window:moving_sum",
     ],
 )
@@ -475,15 +479,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators/window:moving_count",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/window:moving_count",
     ],
 )
@@ -494,15 +498,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators/window:moving_min",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/window:moving_min",
     ],
 )
@@ -513,15 +517,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators/window:moving_max",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators/window:moving_max",
     ],
 )
@@ -532,15 +536,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators:propagate",
         "//temporian/implementation/numpy:evaluation",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:propagate",
     ],
@@ -552,15 +556,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators:resample",
         "//temporian/implementation/numpy:evaluation",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:resample",
     ],
@@ -572,15 +576,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators:prefix",
         "//temporian/implementation/numpy:evaluation",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:prefix",
     ],
@@ -607,15 +611,15 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/pandas
         # already_there/numpy
         "//temporian/io:pandas",
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators:since_last",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/operators:since_last",
     ],
 )
@@ -624,15 +628,15 @@
     name = "begin_test",
     srcs = ["begin_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         ":test_util",
         "//temporian/implementation/numpy/data:io",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators:begin",
         "//temporian/implementation/numpy/operators:begin",
     ],
 )
 
@@ -640,30 +644,78 @@
     name = "end_test",
     srcs = ["end_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         ":test_util",
         "//temporian/implementation/numpy/data:io",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/core/operators:end",
         "//temporian/implementation/numpy/operators:end",
     ],
 )
 
 py_test(
     name = "tick_test",
     srcs = ["tick_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         ":test_util",
-        "//temporian/core/data/dtypes:dtype",
+        "//temporian/core/data:dtype",
         "//temporian/core/data:node",
         "//temporian/core/data:schema",
         "//temporian/implementation/numpy/data:io",
         "//temporian/core/operators:tick",
         "//temporian/implementation/numpy/operators:tick",
     ],
 )
+
+py_test(
+    name = "join_test",
+    srcs = ["join_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        ":test_util",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/core/operators:join",
+        "//temporian/implementation/numpy/operators:join",
+    ],
+)
+
+py_test(
+    name = "timestamps_test",
+    srcs = ["timestamps_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        ":test_util",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/core/operators:timestamps",
+        "//temporian/implementation/numpy/operators:timestamps",
+    ],
+)
+
+py_test(
+    name = "enumerate_test",
+    srcs = ["enumerate_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        ":test_util",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/core/operators:enumerate",
+        "//temporian/implementation/numpy/operators:enumerate",
+    ],
+)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/add_index_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/add_index_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     set_index,
 )
 from temporian.implementation.numpy.data.io import event_set
 from temporian.implementation.numpy.operators.add_index import (
     AddIndexNumpyImplementation,
 )
 from temporian.io.pandas import from_pandas
-from temporian.core.evaluation import evaluate
+from temporian.core.evaluation import run
 from temporian.implementation.numpy.operators.test.test_util import (
     assertEqualEventSet,
 )
 
 
 class AddIndexNumpyImplementationTest(absltest.TestCase):
     def setUp(self) -> None:
@@ -35,15 +35,15 @@
                     "state_id",
                     "store_id",
                     "item_id",
                     "timestamp",
                     "sales",
                 ],
             ),
-            index_names=["state_id"],
+            indexes=["state_id"],
         )
 
         self.input_node = self.input_evset.node()
 
     def test_add_index_single(self) -> None:
         expected_evset = from_pandas(
             pd.DataFrame(
@@ -61,15 +61,15 @@
                     "state_id",
                     "store_id",
                     "item_id",
                     "timestamp",
                     "sales",
                 ],
             ),
-            index_names=["state_id", "store_id"],
+            indexes=["state_id", "store_id"],
         )
         output = add_index(self.input_node, "store_id")
         operator_impl = AddIndexNumpyImplementation(output.creator)
         output_evset = operator_impl.call(input=self.input_evset)["output"]
 
         assertEqualEventSet(self, output_evset, expected_evset)
 
@@ -90,15 +90,15 @@
                     "state_id",
                     "store_id",
                     "item_id",
                     "timestamp",
                     "sales",
                 ],
             ),
-            index_names=["state_id", "store_id", "item_id"],
+            indexes=["state_id", "store_id", "item_id"],
         )
         output = add_index(self.input_node, ["store_id", "item_id"])
         # instance operator implementation
         operator_impl = AddIndexNumpyImplementation(output.creator)
 
         # call operator
         output_evset = operator_impl.call(input=self.input_evset)["output"]
@@ -123,18 +123,18 @@
                     "store_id",
                     "item_id",
                     "timestamp",
                     "sales",
                     "state_id",
                 ],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         output = set_index(self.input_node, ["store_id"])
-        output_evset = evaluate(
+        output_evset = run(
             output, {self.input_node: self.input_evset}, check_execution=True
         )
 
         assertEqualEventSet(self, output_evset, expected_evset)
 
     def test_set_index_multiple(self) -> None:
         expected_evset = from_pandas(
@@ -153,43 +153,43 @@
                     "store_id",
                     "item_id",
                     "timestamp",
                     "sales",
                     "state_id",
                 ],
             ),
-            index_names=["store_id", "item_id"],
+            indexes=["store_id", "item_id"],
         )
         output = set_index(
             self.input_node,
             ["store_id", "item_id"],
         )
-        output_evset = evaluate(
+        output_evset = run(
             output, {self.input_node: self.input_evset}, check_execution=True
         )
 
         assertEqualEventSet(self, output_evset, expected_evset)
 
     def test_set_index_multiple_change_order(self) -> None:
         common = {"features": {"a": [], "b": [], "c": []}, "timestamps": []}
 
-        evset_abc = event_set(**common, index_features=["a", "b", "c"])
-        evset_acb = event_set(**common, index_features=["a", "c", "b"])
-        evset_cba = event_set(**common, index_features=["c", "b", "a"])
-        evset_cab = event_set(**common, index_features=["c", "a", "b"])
+        evset_abc = event_set(**common, indexes=["a", "b", "c"])
+        evset_acb = event_set(**common, indexes=["a", "c", "b"])
+        evset_cba = event_set(**common, indexes=["c", "b", "a"])
+        evset_cab = event_set(**common, indexes=["c", "a", "b"])
 
-        def run(src_evset, new_index, expected_evset):
+        def my_run(src_evset, new_index, expected_evset):
             output = set_index(src_evset.node(), new_index)
-            output_evset = evaluate(
+            output_evset = run(
                 output, {src_evset.node(): src_evset}, check_execution=True
             )
             assertEqualEventSet(self, output_evset, expected_evset)
 
-        run(evset_abc, ["a", "b", "c"], evset_abc)
-        run(evset_abc, ["a", "c", "b"], evset_acb)
-        run(evset_abc, ["c", "b", "a"], evset_cba)
-        run(evset_abc, ["c", "a", "b"], evset_cab)
-        run(evset_cba, ["a", "b", "c"], evset_abc)
+        my_run(evset_abc, ["a", "b", "c"], evset_abc)
+        my_run(evset_abc, ["a", "c", "b"], evset_acb)
+        my_run(evset_abc, ["c", "b", "a"], evset_cba)
+        my_run(evset_abc, ["c", "a", "b"], evset_cab)
+        my_run(evset_cba, ["a", "b", "c"], evset_abc)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/arithmetic_multi_index_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/arithmetic_multi_index_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import pandas as pd
 from absl.testing import absltest
 
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.core.data.node import input_node
 from temporian.core.operators.binary import (
     AddOperator,
     SubtractOperator,
     MultiplyOperator,
     DivideOperator,
     FloorDivOperator,
@@ -71,15 +71,15 @@
                     "timestamp",
                     "sales",
                     "revenue",
                 ],
             ).astype(
                 {"revenue": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         self.evset_2 = from_pandas(
             pd.DataFrame(
                 data=[
                     [GOOGLE_SHOP, BOOK_ID, 1.0, 3, -8.0],
                     [TRYOLABS_SHOP, MATE_ID, 0.0, 4.5, 5],
@@ -96,15 +96,15 @@
                     "timestamp",
                     "costs",
                     "sales",
                 ],
             ).astype(
                 {"sales": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
 
         # Expected result after addition
         self.expected_evset_add = from_pandas(
             pd.DataFrame(
                 [
@@ -123,15 +123,15 @@
                     "timestamp",
                     "add_sales_costs",
                     "add_revenue_sales",
                 ],
             ).astype(
                 {"add_revenue_sales": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
         # Expected result after subtraction
         self.expected_evset_subtract = from_pandas(
             pd.DataFrame(
                 [
                     [TRYOLABS_SHOP, MATE_ID, 0.0, -18.5, -4],
                     [TRYOLABS_SHOP, MATE_ID, 1.0, 20.5, -1],
@@ -148,15 +148,15 @@
                     "timestamp",
                     "sub_sales_costs",
                     "sub_revenue_sales",
                 ],
             ).astype(
                 {"sub_revenue_sales": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
         # Expected result after multiplication
         self.expected_evset_multiply = from_pandas(
             pd.DataFrame(
                 [
                     [TRYOLABS_SHOP, MATE_ID, 0.0, -63, 5],
                     [TRYOLABS_SHOP, MATE_ID, 1.0, -82.5, 6],
@@ -173,15 +173,15 @@
                     "timestamp",
                     "mult_sales_costs",
                     "mult_revenue_sales",
                 ],
             ).astype(
                 {"mult_revenue_sales": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
         # Expected result after division
         self.expected_evset_divide = from_pandas(
             pd.DataFrame(
                 [
                     [TRYOLABS_SHOP, MATE_ID, 0.0, -14 / 4.5, 0.2],
                     [TRYOLABS_SHOP, MATE_ID, 1.0, -15 / 5.5, 2 / 3],
@@ -198,15 +198,15 @@
                     "timestamp",
                     "div_sales_costs",
                     "div_revenue_sales",
                 ],
             ).astype(
                 {"div_revenue_sales": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         # Expected result after floor division
         self.expected_evset_floordiv = from_pandas(
             pd.DataFrame(
                 [
                     [TRYOLABS_SHOP, MATE_ID, 0.0, -4.0, 0],
@@ -224,15 +224,15 @@
                     "timestamp",
                     "floordiv_sales_costs",
                     "floordiv_revenue_sales",
                 ],
             ).astype(
                 {"floordiv_revenue_sales": np.float32}  # Default is float64
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         self.node_1 = input_node(
             [("sales", DType.FLOAT64), ("revenue", DType.FLOAT32)],
             indexes=[("store_id", DType.INT64), ("product_id", DType.INT64)],
         )
         self.node_2 = input_node(
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/arithmetic_scalar_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/arithmetic_scalar_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 12.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 30.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         self.node = self.evset.node()
 
     def test_correct_add(self) -> None:
         """Test correct sum operator."""
 
@@ -74,15 +74,15 @@
                     [0, 2.0, 10.0],
                     [0, 3.0, 22.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 40.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = AddScalarOperator(
             input=self.node,
             value=value,
         )
         operator.outputs["output"].check_same_sampling(self.node)
@@ -104,15 +104,15 @@
                     [0, 2.0, -10.0],
                     [0, 3.0, 2.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 20.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = SubtractScalarOperator(
             input=self.node,
             value=value,
         )
 
@@ -135,15 +135,15 @@
                     [0, 2.0, 10.0],
                     [0, 3.0, -2.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, -20.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = SubtractScalarOperator(
             input=self.node,
             value=value,
             is_value_first=True,
         )
@@ -166,15 +166,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 120.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 300.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = MultiplyScalarOperator(
             input=self.node,
             value=value,
         )
 
@@ -195,15 +195,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 1.2],
                     [0, 4.0, np.nan],
                     [0, 5.0, 3.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = DivideScalarOperator(
             input=self.node,
             value=value,
         )
 
@@ -224,15 +224,15 @@
                     [0, 2.0, np.inf],
                     [0, 3.0, 10.0 / 12.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 1.0 / 3.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = DivideScalarOperator(
             input=self.node,
             value=value,
             is_value_first=True,
         )
@@ -255,15 +255,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 1.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 3.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = FloorDivScalarOperator(
             input=self.node,
             value=value,
         )
 
@@ -284,15 +284,15 @@
                     [0, 2.0, np.inf],
                     [0, 3.0, 10.0 // 12.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 1.0 // 3.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = FloorDivScalarOperator(
             input=self.node,
             value=value,
             is_value_first=True,
         )
@@ -314,15 +314,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 5.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 2.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = ModuloScalarOperator(
             input=self.node,
             value=value,
         )
 
@@ -343,15 +343,15 @@
                     [0, 2.0, np.nan],
                     [0, 3.0, 1.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 25.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = ModuloScalarOperator(
             input=self.node, value=value, is_value_first=True
         )
 
         impl = ModuloScalarNumpyImplementation(operator)
@@ -371,15 +371,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 144.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 900.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = PowerScalarOperator(
             input=self.node,
             value=value,
         )
 
@@ -400,15 +400,15 @@
                     [0, 2.0, 1.0],
                     [0, 3.0, 4096.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 2**30],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = PowerScalarOperator(
             input=self.node, value=value, is_value_first=True
         )
 
         impl = PowerScalarNumpyImplementation(operator)
@@ -427,15 +427,15 @@
                     [0, 203, 2.0, 0.0],
                     [1, 83, 3.0, 12.0],
                     [1, 21, 4.0, np.nan],
                     [2, 310, 5.0, 30.0],
                 ],
                 columns=["store_id", "product_id", "timestamp", "sales"],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         value = 10.0
 
         output_evset = from_pandas(
             pd.DataFrame(
                 [
@@ -448,15 +448,15 @@
                 columns=[
                     "store_id",
                     "product_id",
                     "timestamp",
                     "sales",
                 ],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         node = evset.node()
 
         operator = AddScalarOperator(
             input=node,
             value=value,
@@ -482,15 +482,15 @@
                     [0, 2.0, 0],
                     [0, 3.0, 12],
                     [0, 4.0, -10],
                     [0, 5.0, 30],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         node = event_data.node()
 
         with self.assertRaises(ValueError):
             _ = AddScalarOperator(
                 input=node,
@@ -518,15 +518,15 @@
                     [0, 2.0, 0, 3.0],
                     [0, 3.0, 12, 2.1],
                     [0, 4.0, -10, 3.3],
                     [0, 5.0, 30, 9],
                 ],
                 columns=["store_id", "timestamp", "sales", "revenue"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         node = evset.node()
 
         value = 10
 
         output_evset = from_pandas(
@@ -541,15 +541,15 @@
                 columns=[
                     "store_id",
                     "timestamp",
                     "sales",
                     "revenue",
                 ],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = AddScalarOperator(
             input=node,
             value=value,
         )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/arithmetic_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/arithmetic_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,42 +49,42 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, 12.0],
                     [0, 4.0, np.nan],
                     [0, 5.0, 30.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         self.evset_2 = from_pandas(
             pd.DataFrame(
                 [
                     [0, 1.0, 0.0],
                     [0, 2.0, 20.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, 6.0],
                     [0, 5.0, 10.0],
                 ],
                 columns=["store_id", "timestamp", "costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         self.evset_3 = from_pandas(
             pd.DataFrame(
                 [
                     [0, 1.0, 0.0],
                     [0, 2.0, 20.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, 0.0],
                     [0, 5.0, 7.0],
                 ],
                 columns=["store_id", "timestamp", "costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         self.node_1 = self.evset_1.node()
         self.node_2 = self.evset_2.node()
         self.node_3 = self.evset_3.node()
 
     def test_correct_sum(self) -> None:
@@ -97,15 +97,15 @@
                     [0, 2.0, 20.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, np.nan],
                     [0, 5.0, 40.0],
                 ],
                 columns=["store_id", "timestamp", "add_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = AddOperator(
             input_1=self.node_1,
             input_2=self.node_2,
         )
         operator.outputs["output"].check_same_sampling(self.node_1)
@@ -127,15 +127,15 @@
                     [0, 2.0, -20.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, np.nan],
                     [0, 5.0, 20.0],
                 ],
                 columns=["store_id", "timestamp", "sub_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = SubtractOperator(
             input_1=self.node_1,
             input_2=self.node_2,
         )
 
@@ -155,15 +155,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, np.nan],
                     [0, 5.0, 300.0],
                 ],
                 columns=["store_id", "timestamp", "mult_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = MultiplyOperator(
             input_1=self.node_1,
             input_2=self.node_2,
         )
 
@@ -184,15 +184,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, np.nan],
                     [0, 5.0, 3.0],
                 ],
                 columns=["store_id", "timestamp", "div_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = DivideOperator(
             input_1=self.node_1,
             input_2=self.node_2,
         )
 
@@ -215,15 +215,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, np.nan],
                     [0, 5.0, 4.0],
                 ],
                 columns=["store_id", "timestamp", "floordiv_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = FloorDivOperator(
             input_1=self.node_1,
             input_2=self.node_3,
         )
 
@@ -246,15 +246,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, np.nan],
                     [0, 5.0, 2.0],
                 ],
                 columns=["store_id", "timestamp", "mod_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = ModuloOperator(
             input_1=self.node_1,
             input_2=self.node_3,
         )
 
@@ -277,15 +277,15 @@
                     [0, 2.0, 0.0],
                     [0, 3.0, np.nan],
                     [0, 4.0, 1.0],
                     [0, 5.0, 30**7],
                 ],
                 columns=["store_id", "timestamp", "pow_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = PowerOperator(
             input_1=self.node_1,
             input_2=self.node_3,
         )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/begin_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/lag_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,48 +8,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 from absl.testing import absltest
 
-from temporian.core.operators.begin import BeginOperator
+from temporian.core.operators.lag import LagOperator
+from temporian.implementation.numpy.operators.lag import LagNumpyImplementation
 from temporian.implementation.numpy.data.io import event_set
-from temporian.implementation.numpy.operators.begin import (
-    BeginNumpyImplementation,
+from temporian.implementation.numpy.operators.test.test_util import (
+    assertEqualEventSet,
+    testOperatorAndImp,
 )
 
 
-class BeginOperatorTest(absltest.TestCase):
-    def setUp(self):
-        pass
-
-    def test_base(self):
-        evset = event_set(
+class LagNumpyImplementationTest(absltest.TestCase):
+    def test_base(self) -> None:
+        input_data = event_set(
             timestamps=[1, 2, 3, 4],
-            features={
-                "a": [5, 6, 7, 8],
-                "b": ["A", "A", "B", "B"],
-            },
-            index_features=["b"],
+            features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
+            indexes=["y"],
         )
-        node = evset.node()
-
-        expected_output = event_set(
-            timestamps=[1, 3],
-            features={"b": ["A", "B"]},
-            index_features=["b"],
+        expected_result = event_set(
+            timestamps=[1 + 2, 2 + 2, 3 + 2, 4 + 2],
+            features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
+            indexes=["y"],
         )
-
-        # Run op
-        op = BeginOperator(input=node)
-        instance = BeginNumpyImplementation(op)
-        output = instance.call(input=evset)["output"]
-
-        self.assertEqual(output, expected_output)
+        op = LagOperator(input=input_data.node(), duration=2)
+        imp = LagNumpyImplementation(op)
+        testOperatorAndImp(self, op, imp)
+        filtered_evset = imp.call(input=input_data)["output"]
+        assertEqualEventSet(self, filtered_evset, expected_result)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_day_of_month_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_day_of_month_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                     [pd.to_datetime("2023-03-14 00:00:01", utc=True), 1],
                     [pd.to_datetime("2023-03-14 00:00:01", utc=True), 2],
                     [pd.to_datetime("2023-03-14 23:59:59", utc=True), 1],
                     [pd.to_datetime("2023-03-15 12:00:00", utc=True), 2],
                 ],
                 columns=["timestamp", "id"],
             ),
-            index_names=["id"],
+            indexes=["id"],
         )
 
         output_evset = event_set(
             timestamps=np.concatenate(
                 [
                     input_evset.data[(1,)].timestamps,
                     input_evset.data[(2,)].timestamps,
@@ -92,15 +92,15 @@
             ),
             features={
                 "calendar_day_of_month": np.array([1, 14, 14, 14, 15]).astype(
                     np.int32
                 ),
                 "id": [1, 1, 1, 2, 2],
             },
-            index_features=["id"],
+            indexes=["id"],
             is_unix_timestamp=True,
         )
         operator = CalendarDayOfMonthOperator(input_evset.node())
         operator.outputs["output"].check_same_sampling(input_evset.node())
 
         impl = CalendarDayOfMonthNumpyImplementation(operator)
         output = impl.call(sampling=input_evset)["output"]
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_day_of_week_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_day_of_week_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_day_of_year_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_day_of_year_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_hour_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_hour_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_iso_week_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_iso_week_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_minute_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_minute_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_month_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_month_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_second_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_second_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/calendar_year_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/calendar_year_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/cast_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/cast_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 from absl.testing import absltest
 
 from temporian.core.data.node import input_node
 from temporian.implementation.numpy.operators.cast import (
     CastNumpyImplementation,
 )
 from temporian.core.operators.cast import CastOperator, cast
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.io.pandas import from_pandas
 from temporian.implementation.numpy.data.io import event_set
 from temporian.implementation.numpy.operators.test.test_util import (
     assertEqualEventSet,
     testOperatorAndImp,
 )
-from temporian.core.evaluation import evaluate
+from temporian.core.evaluation import run
 
 
 class CastNumpyImplementationTest(absltest.TestCase):
     """Test numpy implementation of all arithmetic operators,
     but using a two-level index and disordered rows."""
 
     def setUp(self):
@@ -69,20 +69,20 @@
                     # The following are just tricky column names :)
                     "f_float_64",
                     "f_int_64",
                     "f_str",
                     "f_boolean",
                 ],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         self.input_node = self.input_evset.node()
 
-        # Expected event set when applying some downcast operations
+        # Expected EventSet when applying some downcast operations
         self.expected_evset_1 = from_pandas(
             pd.DataFrame(
                 data=[
                     # Note: astype() below will truncate above/below numbers
                     [TRYO_SHOP, MATE_ID, 0.0, -14.0, abv_i32, 1.2, 1],
                     [TRYO_SHOP, MATE_ID, 1.0, 15.0, 0, 2, 1],
                     [TRYO_SHOP, MATE_ID, 2.0, 16, 3, 0, 1],
@@ -99,15 +99,15 @@
                     "f_float_64",
                     "f_int_64",
                     "f_str",
                     "f_boolean",
                 ],
                 # Even more tricky: these columns won't match their type
             ).astype({"f_float_64": np.float32, "f_int_64": np.int32}),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         # Expected when converting everything to float32
         self.expected_evset_2 = from_pandas(
             pd.DataFrame(
                 data=[
                     # Note: astype() below will truncate above/below numbers
@@ -133,15 +133,15 @@
                 {
                     "f_float_64": np.float32,
                     "f_int_64": np.float32,
                     "f_str": np.float32,
                     "f_boolean": np.float32,
                 }
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
     def test_cast_manual(self) -> None:
         node = input_node([("x", DType.FLOAT32), ("y", DType.FLOAT32)])
         op = CastOperator(node, check_overflow=True, dtype=DType.INT64)
         imp = CastNumpyImplementation(op)
         testOperatorAndImp(self, op, imp)
@@ -157,15 +157,15 @@
                 "f_str": DType.FLOAT64,
                 "f_boolean": DType.INT64,
             },
             check_overflow=False,
         )
         output_node.check_same_sampling(self.input_node)
 
-        output_evset = evaluate(
+        output_evset = run(
             output_node,
             {self.input_node: self.input_evset},
             check_execution=True,
         )
         assert isinstance(output_evset, EventSet)
         assertEqualEventSet(self, output_evset, self.expected_evset_1)
 
@@ -179,15 +179,15 @@
                 DType.INT64: DType.INT32,
                 DType.STRING: DType.FLOAT64,
                 DType.BOOLEAN: DType.INT64,
                 DType.INT32: DType.INT64,  # This one should have no effect
             },
             check_overflow=False,
         )
-        output_evset = evaluate(
+        output_evset = run(
             output_node,
             {self.input_node: self.input_evset},
             check_execution=True,
         )
         assert isinstance(output_evset, EventSet)
         assertEqualEventSet(self, output_evset, self.expected_evset_1)
 
@@ -195,15 +195,15 @@
         """Test correct casting everything to float32, no overflow check."""
 
         output_node = cast(
             self.input_node,
             target=DType.FLOAT32,
             check_overflow=False,
         )
-        output_evset = evaluate(
+        output_evset = run(
             output_node,
             {self.input_node: self.input_evset},
             check_execution=True,
         )
         assert isinstance(output_evset, EventSet)
         assertEqualEventSet(self, output_evset, self.expected_evset_2)
 
@@ -228,15 +228,15 @@
         output_node = cast(
             self.input_node,
             target={DType.INT64: DType.INT32},
             check_overflow=True,
         )
 
         with self.assertRaisesRegex(ValueError, "Overflow"):
-            _ = evaluate(
+            _ = run(
                 output_node,
                 {self.input_node: self.input_evset},
                 check_execution=True,
             )
 
     def test_overflow_float64_float32(self) -> None:
         """Test overflow check for float32, coming from float64."""
@@ -244,15 +244,15 @@
         output_node = cast(
             self.input_node,
             target={DType.FLOAT64: DType.FLOAT32},
             check_overflow=True,
         )
 
         with self.assertRaisesRegex(ValueError, "Overflow"):
-            _ = evaluate(
+            _ = run(
                 output_node,
                 {self.input_node: self.input_evset},
                 check_execution=True,
             )
 
     def test_no_overflow_boolean(self) -> None:
         """Test that no overflow error is raised when
@@ -260,21 +260,31 @@
 
         output_node = cast(
             self.input_node,
             target={"f_int_64": DType.BOOLEAN, "f_float_64": DType.BOOLEAN},
             check_overflow=True,
         )
 
-        _ = evaluate(
+        _ = run(
             output_node,
             {self.input_node: self.input_evset},
             check_execution=True,
         )
 
     def test_python_types(self):
         input_data = event_set(timestamps=[1, 2], features={"a": [1, 2]})
+
+        # All features
         output_node = cast(input_data.node(), float)
         self.assertEqual(output_node.features[0].dtype, DType.FLOAT64)
 
+        # Map type->type
+        output_node = cast(input_data.node(), {int: float})
+        self.assertEqual(output_node.features[0].dtype, DType.FLOAT64)
+
+        # Map feature->type
+        output_node = cast(input_data.node(), {"a": float})
+        self.assertEqual(output_node.features[0].dtype, DType.FLOAT64)
+
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/drop_index_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/drop_index_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     [0, 2, 0.2, 14.0],
                     [1, 2, 0.3, 15.0],
                     [1, 2, 0.4, 16.0],
                     [1, 3, 0.3, 17.0],
                 ],
                 columns=["store_id", "item_id", "timestamp", "sales"],
             ),
-            index_names=["store_id", "item_id"],
+            indexes=["store_id", "item_id"],
         )
         self.input_node = self.input_evset.node()
 
     def test_drop_all(self) -> None:
         expected_output = from_pandas(
             pd.DataFrame(
                 [
@@ -58,19 +58,19 @@
                     [0.4, 16.0, 1, 2],
                     [0.4, 10.0, 0, 1],
                     [0.5, 11.0, 0, 1],
                     [0.6, 12.0, 0, 1],
                 ],
                 columns=["timestamp", "sales", "store_id", "item_id"],
             ),
-            index_names=[],
+            indexes=[],
         )
 
         operator = DropIndexOperator(
-            self.input_node, index_to_drop=["store_id", "item_id"], keep=True
+            self.input_node, indexes=["store_id", "item_id"], keep=True
         )
         operator_impl = DropIndexNumpyImplementation(operator)
         testOperatorAndImp(self, operator, operator_impl)
         output = operator_impl.call(input=self.input_evset)["output"]
         assertEqualEventSet(self, output, expected_output)
 
     def test_drop_item_id(self) -> None:
@@ -85,19 +85,19 @@
                     [0, 0.4, 10.0, 1],
                     [1, 0.4, 16.0, 2],
                     [0, 0.5, 11.0, 1],
                     [0, 0.6, 12.0, 1],
                 ],
                 columns=["store_id", "timestamp", "sales", "item_id"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = DropIndexOperator(
-            self.input_node, index_to_drop=["item_id"], keep=True
+            self.input_node, indexes=["item_id"], keep=True
         )
         operator_impl = DropIndexNumpyImplementation(operator)
         testOperatorAndImp(self, operator, operator_impl)
         output = operator_impl.call(input=self.input_evset)["output"]
         assertEqualEventSet(self, output, expected_output)
 
     def test_drop_store_id(self) -> None:
@@ -111,19 +111,19 @@
                     [1, 0.4, 10.0, 0],
                     [2, 0.4, 16.0, 1],
                     [1, 0.5, 11.0, 0],
                     [1, 0.6, 12.0, 0],
                 ],
                 columns=["item_id", "timestamp", "sales", "store_id"],
             ),
-            index_names=["item_id"],
+            indexes=["item_id"],
         )
 
         operator = DropIndexOperator(
-            self.input_node, index_to_drop=["store_id"], keep=True
+            self.input_node, indexes=["store_id"], keep=True
         )
 
         operator_impl = DropIndexNumpyImplementation(operator)
         testOperatorAndImp(self, operator, operator_impl)
         output = operator_impl.call(input=self.input_evset)["output"]
         assertEqualEventSet(self, output, expected_output)
 
@@ -139,19 +139,19 @@
                     [0, 0.4, 10.0],
                     [1, 0.4, 16.0],
                     [0, 0.5, 11.0],
                     [0, 0.6, 12.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = DropIndexOperator(
-            self.input_node, index_to_drop=["item_id"], keep=False
+            self.input_node, indexes=["item_id"], keep=False
         )
 
         operator_impl = DropIndexNumpyImplementation(operator)
         testOperatorAndImp(self, operator, operator_impl)
         output = operator_impl.call(input=self.input_evset)["output"]
         assertEqualEventSet(self, output, expected_output)
 
@@ -167,19 +167,19 @@
                     [1, 0.4, 10.0],
                     [2, 0.4, 16.0],
                     [1, 0.5, 11.0],
                     [1, 0.6, 12.0],
                 ],
                 columns=["item_id", "timestamp", "sales"],
             ),
-            index_names=["item_id"],
+            indexes=["item_id"],
         )
 
         operator = DropIndexOperator(
-            self.input_node, index_to_drop=["store_id"], keep=False
+            self.input_node, indexes=["store_id"], keep=False
         )
         operator_impl = DropIndexNumpyImplementation(operator)
         testOperatorAndImp(self, operator, operator_impl)
         output = operator_impl.call(input=self.input_evset)["output"]
         assertEqualEventSet(self, output, expected_output)
 
     def test_str_index(self):
@@ -189,33 +189,33 @@
                     "timestamp": [1, 2, 2, 3],
                     "a": [1, 2, 3, 4],
                     "d": ["D1", "D2", "D3", "D4"],
                     "b": ["B1", "B1", "B2", "B2"],
                     "c": ["C1", "C2", "C1", "C2"],
                 }
             ),
-            index_names=["b", "c"],
+            indexes=["b", "c"],
         )
         node = evset.node()
 
         expected_output = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 2, 2, 3],
                     "a": [1, 2, 3, 4],
                     "d": ["D1", "D2", "D3", "D4"],
                     "b": ["B1", "B1", "B2", "B2"],
                     "c": ["C1", "C2", "C1", "C2"],
                 }
             ),
-            index_names=["c"],
+            indexes=["c"],
         )
 
         # Run op
-        operator = DropIndexOperator(input=node, index_to_drop=["b"], keep=True)
+        operator = DropIndexOperator(input=node, indexes=["b"], keep=True)
         operator_impl = DropIndexNumpyImplementation(operator)
         testOperatorAndImp(self, operator, operator_impl)
         output = operator_impl.call(input=evset)["output"]
         assertEqualEventSet(self, output, expected_output)
 
 
 if __name__ == "__main__":
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/end_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/enumerate_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,45 +11,55 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from absl.testing import absltest
 
-from temporian.core.operators.end import EndOperator
+import numpy as np
+from temporian.core.operators.enumerate import Enumerate
 from temporian.implementation.numpy.data.io import event_set
-from temporian.implementation.numpy.operators.end import (
-    EndNumpyImplementation,
+from temporian.implementation.numpy.operators.enumerate import (
+    EnumerateNumpyImplementation,
+)
+from temporian.implementation.numpy.operators.test.test_util import (
+    assertEqualEventSet,
+    testOperatorAndImp,
 )
 
 
-class EndOperatorTest(absltest.TestCase):
+class EnumerateOperatorTest(absltest.TestCase):
     def setUp(self):
         pass
 
     def test_base(self):
         evset = event_set(
-            timestamps=[1, 2, 3, 4],
+            timestamps=[1, 2, 3, 4, 0, 1],
             features={
-                "a": [5, 6, 7, 8],
-                "b": ["A", "A", "B", "B"],
+                "a": [1.0, 2.0, 3.0, 4.0, 0.0, 1.0],
+                "b": [5, 6, 7, 8, 1, 2],
+                "c": ["A", "A", "A", "A", "B", "B"],
             },
-            index_features=["b"],
+            indexes=["c"],
         )
         node = evset.node()
 
         expected_output = event_set(
-            timestamps=[2, 4],
-            features={"b": ["A", "B"]},
-            index_features=["b"],
+            timestamps=[1, 2, 3, 4, 0, 1],
+            features={
+                "enumerate": [0, 1, 2, 3, 0, 1],
+                "c": ["A", "A", "A", "A", "B", "B"],
+            },
+            indexes=["c"],
         )
 
         # Run op
-        op = EndOperator(input=node)
-        instance = EndNumpyImplementation(op)
+        op = Enumerate(input=node)
+        instance = EnumerateNumpyImplementation(op)
+        testOperatorAndImp(self, op, instance)
         output = instance.call(input=evset)["output"]
 
-        self.assertEqual(output, expected_output)
+        assertEqualEventSet(self, output, expected_output)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/filter_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/filter_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,26 +50,26 @@
         ]
         assertEqualEventSet(self, filtered_evset, expected_result)
 
     def test_index(self) -> None:
         input_data = event_set(
             timestamps=[1, 2, 3, 4],
             features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
-            index_features=["y"],
+            indexes=["y"],
         )
         input_condition = event_set(
             timestamps=[1, 2, 3, 4],
             features={"c": [True, True, True, False], "y": [1, 1, 2, 2]},
-            index_features=["y"],
+            indexes=["y"],
             same_sampling_as=input_data,
         )
         expected_result = event_set(
             timestamps=[1, 2, 3],
             features={"x": [4, 5, 6], "y": [1, 1, 2]},
-            index_features=["y"],
+            indexes=["y"],
         )
         operator = FilterOperator(
             input=input_data.node(), condition=input_condition.node()
         )
         impl = FilterNumpyImplementation(operator)
         testOperatorAndImp(self, operator, impl)
         filtered_evset = impl.call(input=input_data, condition=input_condition)[
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/glue_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/glue_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from absl.testing import absltest
 
 from temporian.core.operators.glue import GlueOperator
 from temporian.core.data.node import input_node
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.implementation.numpy.operators.glue import (
     GlueNumpyImplementation,
 )
 from temporian.implementation.numpy.data.io import event_set
 from temporian.implementation.numpy.operators.test.test_util import (
     assertEqualEventSet,
     testOperatorAndImp,
@@ -36,48 +36,48 @@
     def test_manual_nodes(self):
         evset_1 = event_set(
             timestamps=[1, 1, 2, 3, 4],
             features={
                 "user_id": ["user_1", "user_1", "user_1", "user_1", "user_2"],
                 "feature_1": [10, 11, 12, 13, 14],
             },
-            index_features=["user_id"],
+            indexes=["user_id"],
         )
 
         evset_2 = event_set(
             timestamps=[1, 1, 2, 3, 4],
             features={
                 "user_id": ["user_1", "user_1", "user_1", "user_1", "user_2"],
                 "feature_2": [20, 21, 22, 23, 24],
                 "feature_3": [30, 31, 32, 33, 34],
             },
-            index_features=["user_id"],
+            indexes=["user_id"],
             same_sampling_as=evset_1,
         )
 
         evset_3 = event_set(
             timestamps=[1, 1, 2, 3, 4],
             features={
                 "user_id": ["user_1", "user_1", "user_1", "user_1", "user_2"],
                 "feature_4": [40, 41, 42, 43, 44],
             },
-            index_features=["user_id"],
+            indexes=["user_id"],
             same_sampling_as=evset_1,
         )
 
         expected_evset = event_set(
             timestamps=[1, 1, 2, 3, 4],
             features={
                 "user_id": ["user_1", "user_1", "user_1", "user_1", "user_2"],
                 "feature_1": [10, 11, 12, 13, 14],
                 "feature_2": [20, 21, 22, 23, 24],
                 "feature_3": [30, 31, 32, 33, 34],
                 "feature_4": [40, 41, 42, 43, 44],
             },
-            index_features=["user_id"],
+            indexes=["user_id"],
         )
 
         operator = GlueOperator(
             input_0=evset_1.node(),
             input_1=evset_2.node(),
             input_2=evset_3.node(),
         )
@@ -104,15 +104,15 @@
                 features=[("b", DType.FLOAT64)], indexes=[("x", DType.STRING)]
             )
             _ = GlueOperator(input_0=n1, input_1=n2)
 
     def test_duplicate_feature(self):
         with self.assertRaisesRegex(
             ValueError,
-            'Feature "a" is defined in multiple input nodes',
+            'Feature "a" is defined in multiple input EventSetNodes',
         ):
             n1 = input_node(
                 features=[("a", DType.FLOAT64)], indexes=[("x", DType.STRING)]
             )
             n2 = input_node(
                 features=[("a", DType.FLOAT64)], same_sampling_as=n1
             )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/lag_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/unique_timestamps_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,39 +8,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 from absl.testing import absltest
 
-from temporian.core.operators.lag import LagOperator
-from temporian.implementation.numpy.operators.lag import LagNumpyImplementation
-from temporian.implementation.numpy.data.io import event_set
-from temporian.implementation.numpy.operators.test.test_util import (
-    assertEqualEventSet,
-    testOperatorAndImp,
+import pandas as pd
+from temporian.core.operators.unique_timestamps import UniqueTimestamps
+from temporian.implementation.numpy.operators.unique_timestamps import (
+    UniqueTimestampsNumpyImplementation,
 )
+from temporian.io.pandas import from_pandas
 
 
-class LagNumpyImplementationTest(absltest.TestCase):
-    def test_base(self) -> None:
-        input_data = event_set(
-            timestamps=[1, 2, 3, 4],
-            features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
-            index_features=["y"],
+class UniqueTimestampsOperatorTest(absltest.TestCase):
+    def setUp(self):
+        pass
+
+    def test_base(self):
+        evset = from_pandas(
+            pd.DataFrame(
+                {
+                    "timestamp": [1, 2, 2, 2, 3, 3, 3, 4],
+                    "a": [1, 2, 3, 4, 5, 6, 7, 8],
+                    "c": [1, 1, 1, 1, 1, 2, 2, 2],
+                }
+            ),
+            indexes=["c"],
         )
-        expected_result = event_set(
-            timestamps=[1 + 2, 2 + 2, 3 + 2, 4 + 2],
-            features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
-            index_features=["y"],
+        node = evset.node()
+
+        expected_output = from_pandas(
+            pd.DataFrame(
+                {
+                    "timestamp": [1, 2, 3, 3, 4],
+                    "c": [1, 1, 1, 2, 2],
+                }
+            ),
+            indexes=["c"],
         )
-        op = LagOperator(input=input_data.node(), duration=2)
-        imp = LagNumpyImplementation(op)
-        testOperatorAndImp(self, op, imp)
-        filtered_evset = imp.call(input=input_data)["output"]
-        assertEqualEventSet(self, filtered_evset, expected_result)
+
+        # Run op
+        op = UniqueTimestamps(input=node)
+        instance = UniqueTimestampsNumpyImplementation(op)
+        output = instance.call(input=evset)["output"]
+
+        self.assertEqual(output, expected_output)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/leak_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/leak_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 
 
 class LagNumpyImplementationTest(absltest.TestCase):
     def test_base(self) -> None:
         input_data = event_set(
             timestamps=[1, 2, 3, 4],
             features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
-            index_features=["y"],
+            indexes=["y"],
         )
         expected_result = event_set(
             timestamps=[1 - 2, 2 - 2, 3 - 2, 4 - 2],
             features={"x": [4, 5, 6, 7], "y": [1, 1, 2, 2]},
-            index_features=["y"],
+            indexes=["y"],
         )
         op = LeakOperator(input=input_data.node(), duration=2)
         imp = LeakNumpyImplementation(op)
         testOperatorAndImp(self, op, imp)
         filtered_evset = imp.call(input=input_data)["output"]
         assertEqualEventSet(self, filtered_evset, expected_result)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/logical_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/logical_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         )
         self.node_1 = self.evset_1.node()
         self.node_2 = self.evset_2.node()
 
         # FIXME: This should not be necessary
         self.node_2._sampling = self.node_1._sampling
         for index, data in self.evset_1.data.items():
-            self.evset_2[index].timestamps = data.timestamps
+            self.evset_2.data[index].timestamps = data.timestamps
 
     def test_correct_and(self) -> None:
         """Test correct AND operator."""
         output_evset = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 2, 3, 4],
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_count_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_count_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                     ["X2", "Y1", 15.0, 3.1],
                     ["X2", "Y2", 16.0, 1.2],
                     ["X2", "Y2", 17.0, 2.2],
                     ["X2", "Y2", 18.0, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         op = MovingCountOperator(
             input=evset.node(),
             window_length=5,
             sampling=None,
         )
@@ -138,15 +138,15 @@
                     ["X2", "Y1", 3, 3.1],
                     ["X2", "Y2", 1, 1.2],
                     ["X2", "Y2", 2, 2.2],
                     ["X2", "Y2", 3, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ).astype({"a": np.int32}),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         self.assertEqual(output["output"], expected_output)
 
     def test_with_sampling(self):
         """Event sets with user provided sampling."""
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_max_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_max_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_min_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_min_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_standard_deviation_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_standard_deviation_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 columns=["a", "b", "timestamp"],
             )
         )
 
         self.assertEqual(repr(output), repr({"output": expected_output}))
 
     def test_with_index(self):
-        """Indexed event sets."""
+        """Indexed EventSets."""
 
         input_data = from_pandas(
             pd.DataFrame(
                 [
                     ["X1", "Y1", 10.0, 1],
                     ["X1", "Y1", 11.0, 2],
                     ["X1", "Y1", 12.0, 3],
@@ -109,15 +109,15 @@
                     ["X2", "Y1", 15.0, 3.1],
                     ["X2", "Y2", 16.0, 1.2],
                     ["X2", "Y2", 17.0, 2.2],
                     ["X2", "Y2", 18.0, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         op = MovingStandardDeviationOperator(
             input=input_data.node(),
             window_length=5.0,
             sampling=None,
         )
@@ -137,15 +137,15 @@
                     ["X2", "Y1", math.sqrt(2 / 3), 3.1],
                     ["X2", "Y2", 0, 1.2],
                     ["X2", "Y2", 0.5, 2.2],
                     ["X2", "Y2", math.sqrt(2 / 3), 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         self.assertEqual(repr(output), repr({"output": expected_output}))
 
     def test_with_sampling(self):
         """Event sets with user provided sampling."""
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/moving_sum_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/moving_sum_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                     ["X2", "Y1", 15.0, 3.1],
                     ["X2", "Y2", 16.0, 1.2],
                     ["X2", "Y2", 17.0, 2.2],
                     ["X2", "Y2", 18.0, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         op = MovingSumOperator(
             input=evset.node(),
             window_length=5.0,
             sampling=None,
         )
@@ -138,15 +138,15 @@
                     ["X2", "Y1", 42.0, 3.1],
                     ["X2", "Y2", 16.0, 1.2],
                     ["X2", "Y2", 33.0, 2.2],
                     ["X2", "Y2", 51.0, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         self.assertEqual(output["output"], expected_output)
 
     def test_with_sampling(self):
         """Event sets with user provided sampling."""
 
@@ -280,15 +280,15 @@
                     ["X2", "Y1", 15.0, 0, 3.1],
                     ["X2", "Y2", 16.0, 5, 1.2],
                     ["X2", "Y2", 17.0, 3, 2.2],
                     ["X2", "Y2", 18.0, -1, 3.2],
                 ],
                 columns=["x", "y", "a", "b", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         op = MovingSumOperator(
             input=input_data.node(),
             window_length=np.inf,
             sampling=None,
         )
@@ -308,15 +308,15 @@
                     ["X2", "Y1", 42.0, -11, 3.1],
                     ["X2", "Y2", 16.0, 5, 1.2],
                     ["X2", "Y2", 33.0, 8, 2.2],
                     ["X2", "Y2", 51.0, 7, 3.2],
                 ],
                 columns=["x", "y", "a", "b", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         self.assertEqual(output["output"], expected_output)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/prefix_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/prefix_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,28 +35,28 @@
                 {
                     "timestamp": [1, 2, 3],
                     "a": [1.0, 2.0, 3.0],
                     "b": [5, 6, 7],
                     "x": [1, 1, 2],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
         node = evset.node()
 
         expected_output = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 2, 3],
                     "hello_a": [1.0, 2.0, 3.0],
                     "hello_b": [5, 6, 7],
                     "x": [1, 1, 2],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
 
         # Run op
         op = Prefix("hello_", input=node)
         op.outputs["output"].check_same_sampling(node)
 
         instance = PrefixNumpyImplementation(op)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/propagate_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/propagate_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,40 +32,40 @@
             pd.DataFrame(
                 {
                     "timestamp": [1, 2, 3],
                     "a": [1, 2, 3],
                     "x": [1, 1, 2],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
         node = evset.node()
 
         sampling_evset = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 1, 1, 1],
                     "x": [1, 1, 2, 2],
                     "y": [1, 2, 1, 2],
                 }
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
         sampling_node = sampling_evset.node()
 
         expected_output = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 2, 1, 2, 3, 3],
                     "a": [1, 2, 1, 2, 3, 3],
                     "x": [1, 1, 1, 1, 2, 2],
                     "y": [1, 1, 2, 2, 1, 2],
                 }
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
         # Run op
         op = Propagate(input=node, sampling=sampling_node)
         self.assertEqual(op.list_matching_io_samplings(), [])
 
         instance = PropagateNumpyImplementation(op)
         output = instance.call(input=evset, sampling=sampling_evset)["output"]
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/relational_scalar_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/relational_scalar_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import pandas as pd
 from absl.testing import absltest
 
+from temporian.implementation.numpy.data.io import event_set
 from temporian.core.operators.scalar import (
     EqualScalarOperator,
     NotEqualScalarOperator,
     GreaterScalarOperator,
     LessScalarOperator,
     GreaterEqualScalarOperator,
     LessEqualScalarOperator,
@@ -29,14 +30,18 @@
     NotEqualScalarNumpyImplementation,
     GreaterScalarNumpyImplementation,
     LessScalarNumpyImplementation,
     GreaterEqualScalarNumpyImplementation,
     LessEqualScalarNumpyImplementation,
 )
 from temporian.io.pandas import from_pandas
+from temporian.implementation.numpy.operators.test.test_util import (
+    assertEqualEventSet,
+    testOperatorAndImp,
+)
 
 
 class ArithmeticScalarNumpyImplementationTest(absltest.TestCase):
     """Test numpy implementation of all arithmetic operators:
     addition, subtraction, division and multiplication"""
 
     def setUp(self):
@@ -47,15 +52,15 @@
                     [0, 2.0, 0.0],
                     [1, 3.0, 12.0],
                     [1, 4.0, np.nan],
                     [1, 5.0, 30.0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         self.node = self.evset.node()
 
     def test_correct_equal(self) -> None:
         """Test correct equal operator."""
         value = 12.0
@@ -67,29 +72,67 @@
                     [0, 2.0, False],
                     [1, 3.0, True],
                     [1, 4.0, False],
                     [1, 5.0, False],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = EqualScalarOperator(
             input=self.node,
             value=value,
         )
         operator.outputs["output"].check_same_sampling(self.node)
 
         impl = EqualScalarNumpyImplementation(operator)
 
         operator_output = impl.call(input=self.evset)
 
         self.assertEqual(output_evset, operator_output["output"])
 
+    def test_equal_str(self) -> None:
+        timestamps = [1, 2, 3, 4]
+        evset = event_set(
+            timestamps=timestamps,
+            features={"a": ["A", "A", "B", "B"]},
+        )
+        node = evset.node()
+
+        expected_output = event_set(
+            timestamps=timestamps,
+            features={"a": [True, True, False, False]},
+        )
+
+        op = EqualScalarOperator(node, "A")
+        instance = EqualScalarNumpyImplementation(op)
+        testOperatorAndImp(self, op, instance)
+        output = instance.call(input=evset)["output"]
+        assertEqualEventSet(self, output, expected_output)
+
+    def test_notequal_str(self) -> None:
+        timestamps = [1, 2, 3, 4]
+        evset = event_set(
+            timestamps=timestamps,
+            features={"a": ["A", "A", "B", "B"]},
+        )
+        node = evset.node()
+
+        expected_output = event_set(
+            timestamps=timestamps,
+            features={"a": [False, False, True, True]},
+        )
+
+        op = NotEqualScalarOperator(node, "A")
+        instance = NotEqualScalarNumpyImplementation(op)
+        testOperatorAndImp(self, op, instance)
+        output = instance.call(input=evset)["output"]
+        assertEqualEventSet(self, output, expected_output)
+
     def test_equal_nan(self) -> None:
         """Test equal operator against a nan value."""
         value = np.nan
 
         output_evset = from_pandas(
             pd.DataFrame(
                 [
@@ -97,15 +140,15 @@
                     [0, 2.0, False],
                     [1, 3.0, False],
                     [1, 4.0, False],
                     [1, 5.0, False],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         operator = EqualScalarOperator(
             input=self.node,
             value=value,
         )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/relational_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/relational_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import pandas as pd
 from absl.testing import absltest
 
+from temporian.implementation.numpy.data.io import event_set
 from temporian.core.operators.binary import (
     EqualOperator,
     NotEqualOperator,
     GreaterEqualOperator,
     GreaterOperator,
     LessEqualOperator,
     LessOperator,
@@ -29,14 +30,18 @@
     NotEqualNumpyImplementation,
     GreaterEqualNumpyImplementation,
     GreaterNumpyImplementation,
     LessEqualNumpyImplementation,
     LessNumpyImplementation,
 )
 from temporian.io.pandas import from_pandas
+from temporian.implementation.numpy.operators.test.test_util import (
+    assertEqualEventSet,
+    testOperatorAndImp,
+)
 
 
 class ArithmeticNumpyImplementationTest(absltest.TestCase):
     """Test numpy implementation of all arithmetic operators:
     addition, subtraction, division and multiplication"""
 
     def setUp(self):
@@ -48,38 +53,38 @@
                     [1, 3.0, 12.0],
                     [1, 4.0, np.nan],
                     [2, 5.0, -30.0],
                     [2, 6.0, 0],
                 ],
                 columns=["store_id", "timestamp", "sales"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
 
         self.evset_2 = from_pandas(
             pd.DataFrame(
                 [
                     [0, 1.0, 10.0],
                     [0, 2.0, -1.0],
                     [1, 3.0, 12.000000001],
                     [1, 4.0, np.nan],
                     [2, 5.0, -30.0],
                     [2, 6.0, np.nan],
                 ],
                 columns=["store_id", "timestamp", "costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         self.node_1 = self.evset_1.node()
         self.node_2 = self.evset_2.node()
 
         # FIXME: This should not be necessary
         self.node_2._sampling = self.node_1._sampling
         for index, data in self.evset_1.data.items():
-            self.evset_2[index].timestamps = data.timestamps
+            self.evset_2.data[index].timestamps = data.timestamps
 
     def test_correct_equal(self) -> None:
         """Test correct equal operator."""
         output_evset = from_pandas(
             pd.DataFrame(
                 [
                     [0, 1.0, True],
@@ -87,40 +92,86 @@
                     [1, 3.0, False],
                     [1, 4.0, False],  # nan == nan is False
                     [2, 5.0, True],
                     [2, 6.0, False],
                 ],
                 columns=["store_id", "timestamp", "eq_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         operator = EqualOperator(input_1=self.node_1, input_2=self.node_2)
         operator.outputs["output"].check_same_sampling(self.node_1)
         operator.outputs["output"].check_same_sampling(self.node_2)
 
         operator_output = EqualNumpyImplementation(operator).call(
             input_1=self.evset_1, input_2=self.evset_2
         )
         self.assertEqual(output_evset, operator_output["output"])
 
+    def test_equal_str(self) -> None:
+        timestamps = [1, 2, 3, 4]
+        evset_1 = event_set(
+            timestamps=timestamps,
+            features={"a": ["A", "A", "B", "B"]},
+        )
+        evset_2 = event_set(
+            timestamps=timestamps,
+            features={"b": ["A", "B", "A", "B"]},
+            same_sampling_as=evset_1,
+        )
+
+        expected_output = event_set(
+            timestamps=timestamps,
+            features={"eq_a_b": [True, False, False, True]},
+        )
+
+        op = EqualOperator(evset_1.node(), evset_2.node())
+        instance = EqualNumpyImplementation(op)
+        testOperatorAndImp(self, op, instance)
+        output = instance.call(input_1=evset_1, input_2=evset_2)["output"]
+        assertEqualEventSet(self, output, expected_output)
+
+    def test_notequal_str(self) -> None:
+        timestamps = [1, 2, 3, 4]
+        evset_1 = event_set(
+            timestamps=timestamps,
+            features={"a": ["A", "A", "B", "B"]},
+        )
+        evset_2 = event_set(
+            timestamps=timestamps,
+            features={"b": ["A", "B", "A", "B"]},
+            same_sampling_as=evset_1,
+        )
+
+        expected_output = event_set(
+            timestamps=timestamps,
+            features={"ne_a_b": [False, True, True, False]},
+        )
+
+        op = NotEqualOperator(evset_1.node(), evset_2.node())
+        instance = NotEqualNumpyImplementation(op)
+        testOperatorAndImp(self, op, instance)
+        output = instance.call(input_1=evset_1, input_2=evset_2)["output"]
+        assertEqualEventSet(self, output, expected_output)
+
     def test_correct_not_equal(self) -> None:
         """Test correct not-equal operator."""
         output_evset = from_pandas(
             pd.DataFrame(
                 [
                     [0, 1.0, False],
                     [0, 2.0, True],
                     [1, 3.0, True],
                     [1, 4.0, True],  # nan != nan is True
                     [2, 5.0, False],
                     [2, 6.0, True],
                 ],
                 columns=["store_id", "timestamp", "ne_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         operator = NotEqualOperator(input_1=self.node_1, input_2=self.node_2)
         operator_output = NotEqualNumpyImplementation(operator).call(
             input_1=self.evset_1, input_2=self.evset_2
         )
         self.assertEqual(output_evset, operator_output["output"])
 
@@ -133,15 +184,15 @@
                     [1, 3.0, False],
                     [1, 4.0, False],  # nan > nan is always False
                     [2, 5.0, False],
                     [2, 6.0, False],  # any comparison to nan is False
                 ],
                 columns=["store_id", "timestamp", "gt_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         operator = GreaterOperator(input_1=self.node_1, input_2=self.node_2)
         operator_output = GreaterNumpyImplementation(operator).call(
             input_1=self.evset_1, input_2=self.evset_2
         )
         self.assertEqual(output_evset, operator_output["output"])
 
@@ -154,15 +205,15 @@
                     [1, 3.0, False],
                     [1, 4.0, False],  # nan >= nan is always False
                     [2, 5.0, True],
                     [2, 6.0, False],  # any comparison to nan is False
                 ],
                 columns=["store_id", "timestamp", "ge_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         op = GreaterEqualOperator(input_1=self.node_1, input_2=self.node_2)
         operator_output = GreaterEqualNumpyImplementation(op).call(
             input_1=self.evset_1, input_2=self.evset_2
         )
         self.assertEqual(output_evset, operator_output["output"])
 
@@ -175,15 +226,15 @@
                     [1, 3.0, True],
                     [1, 4.0, False],  # nan < nan is always False
                     [2, 5.0, False],
                     [2, 6.0, False],  # any comparison to nan is False
                 ],
                 columns=["store_id", "timestamp", "lt_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         op = LessOperator(input_1=self.node_1, input_2=self.node_2)
         operator_output = LessNumpyImplementation(op).call(
             input_1=self.evset_1, input_2=self.evset_2
         )
         self.assertEqual(output_evset, operator_output["output"])
 
@@ -196,15 +247,15 @@
                     [1, 3.0, True],
                     [1, 4.0, False],  # nan <= nan is always False
                     [2, 5.0, True],
                     [2, 6.0, False],  # any comparison to nan is False
                 ],
                 columns=["store_id", "timestamp", "le_sales_costs"],
             ),
-            index_names=["store_id"],
+            indexes=["store_id"],
         )
         op = LessEqualOperator(input_1=self.node_1, input_2=self.node_2)
         operator_output = LessEqualNumpyImplementation(op).call(
             input_1=self.evset_1, input_2=self.evset_2
         )
         self.assertEqual(output_evset, operator_output["output"])
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/rename_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/rename_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,26 @@
             [
                 ["A", 1.0, 10.0, -1.0, 0.0],
                 ["A", 2.0, np.nan, -2.0, 32.0],
             ],
             columns=["store_id", "timestamp", "sales", "costs", "weather"],
         )
 
-        self.input_evset = from_pandas(self.df, index_names=["store_id"])
+        self.input_evset = from_pandas(self.df, indexes=["store_id"])
         self.input_node = self.input_evset.node()
 
         df = pd.DataFrame(
             [
                 ["A", 1.0, "X", -1.0, 0.0],
                 ["A", 2.0, "Y", -2.0, 32.0],
             ],
             columns=["store_id", "timestamp", "sales", "costs", "weather"],
         )
 
-        self_input_evset_2 = from_pandas(df, index_names=["store_id", "sales"])
+        self_input_evset_2 = from_pandas(df, indexes=["store_id", "sales"])
         self.input_node_2 = self_input_evset_2.node()
 
     def test_rename_single_feature_with_str(self) -> None:
         """Test renaming single feature with str."""
         df = pd.DataFrame(
             [
                 [1.0, 10.0],
@@ -115,15 +115,15 @@
             [
                 ["A", 1.0, 10.0, -1.0, 0.0],
                 ["A", 2.0, np.nan, -2.0, 32.0],
             ],
             columns=["store_id", "timestamp", "new_sales", "costs", "profit"],
         )
 
-        expected_evset = from_pandas(new_df, index_names=["store_id"])
+        expected_evset = from_pandas(new_df, indexes=["store_id"])
 
         output = rename(
             input=self.input_node,
             features={"sales": "new_sales", "weather": "profit"},
         )
         impl = RenameNumpyImplementation(output.creator)
         renamed_evset = impl.call(input=self.input_evset)["output"]
@@ -136,19 +136,19 @@
             [
                 ["A", 1.0, 10.0, -1.0, 0.0],
                 ["A", 2.0, np.nan, -2.0, 32.0],
             ],
             columns=["product_id", "timestamp", "sales", "costs", "weather"],
         )
 
-        expected_evset = from_pandas(new_df, index_names=["product_id"])
+        expected_evset = from_pandas(new_df, indexes=["product_id"])
 
         output = rename(
             input=self.input_node,
-            index="product_id",
+            indexes="product_id",
         )
         impl = RenameNumpyImplementation(output.creator)
         renamed_evset = impl.call(input=self.input_evset)["output"]
 
         self.assertEqual(renamed_evset, expected_evset)
 
     def test_rename_single_index_with_dict(self) -> None:
@@ -157,19 +157,19 @@
             [
                 ["A", 1.0, 10.0, -1.0, 0.0],
                 ["A", 2.0, np.nan, -2.0, 32.0],
             ],
             columns=["product_id", "timestamp", "sales", "costs", "weather"],
         )
 
-        expected_evset = from_pandas(new_df, index_names=["product_id"])
+        expected_evset = from_pandas(new_df, indexes=["product_id"])
 
         output = rename(
             input=self.input_node,
-            index={"store_id": "product_id"},
+            indexes={"store_id": "product_id"},
         )
         impl = RenameNumpyImplementation(output.creator)
         renamed_evset = impl.call(input=self.input_evset)["output"]
 
         self.assertEqual(renamed_evset, expected_evset)
 
     def test_rename_multiple_indexes(self) -> None:
@@ -179,31 +179,31 @@
             [
                 ["A", 1.0, 10.0, -1, 0.0],
                 ["A", 2.0, np.nan, -2, 32.0],
             ],
             columns=["store_id", "timestamp", "sales", "costs", "weather"],
         )
 
-        self.input_evset = from_pandas(df, index_names=["store_id", "costs"])
+        self.input_evset = from_pandas(df, indexes=["store_id", "costs"])
 
         self.input_node = self.input_evset.node()
 
         new_df = pd.DataFrame(
             [
                 ["A", 1.0, 10.0, -1, 0.0],
                 ["A", 2.0, np.nan, -2, 32.0],
             ],
             columns=["product_id", "timestamp", "sales", "roi", "weather"],
         )
 
-        expected_evset = from_pandas(new_df, index_names=["product_id", "roi"])
+        expected_evset = from_pandas(new_df, indexes=["product_id", "roi"])
 
         output = rename(
             input=self.input_node,
-            index={"store_id": "product_id", "costs": "roi"},
+            indexes={"store_id": "product_id", "costs": "roi"},
         )
         impl = RenameNumpyImplementation(output.creator)
         renamed_evset = impl.call(input=self.input_evset)["output"]
 
         self.assertEqual(renamed_evset, expected_evset)
 
     def test_rename_feature_with_empty_str(self) -> None:
@@ -243,50 +243,50 @@
                 input=self.input_node,
                 features={"sales": "new_sales", "costs": "new_sales"},
             )
 
     def test_rename_index_with_empty_str(self) -> None:
         """Test renaming index with empty string."""
         with self.assertRaises(ValueError):
-            rename(input=self.input_node, index={"sales": ""})
+            rename(input=self.input_node, indexes={"sales": ""})
 
     def test_rename_index_with_empty_str_without_dict(self) -> None:
         """Test renaming index with empty string."""
         df = pd.DataFrame(
             [
                 [1.0, "A"],
                 [2.0, "A"],
             ],
             columns=["timestamp", "sales"],
         )
 
-        self.input_node = from_pandas(df, index_names=["sales"]).node()
+        self.input_node = from_pandas(df, indexes=["sales"]).node()
 
         with self.assertRaises(ValueError):
-            rename(self.input_node, index="")
+            rename(self.input_node, indexes="")
 
     def test_rename_index_with_non_existent_index(self) -> None:
         """Test renaming index with non existent index."""
         with self.assertRaises(KeyError):
-            rename(input=self.input_node, index={"sales_1": "costs"})
+            rename(input=self.input_node, indexes={"sales_1": "costs"})
 
-    def test_rename_index_with_duplicated_new_index_names(self) -> None:
+    def test_rename_index_with_duplicated_new_indexes(self) -> None:
         """Test renaming index with duplicated new names."""
         with self.assertRaises(ValueError):
             rename(
                 input=self.input_node,
-                index={"store_id": "new_sales", "sales": "new_sales"},
+                indexes={"store_id": "new_sales", "sales": "new_sales"},
             )
 
     def test_rename_feature_and_index_with_same_name(self) -> None:
         """Test renaming feature and index with same name."""
 
         output = rename(
             input=self.input_node,
-            index={"store_id": "sales"},
+            indexes={"store_id": "sales"},
         )
         impl = RenameNumpyImplementation(output.creator)
 
         with self.assertRaises(ValueError):
             impl.call(input=self.input_evset)["output"]
 
     def test_rename_feature_and_index_inverting_name(self) -> None:
@@ -295,20 +295,20 @@
             [
                 ["A", 1.0, 10.0, -1.0, 0.0],
                 ["A", 2.0, np.nan, -2.0, 32.0],
             ],
             columns=["sales", "timestamp", "store_id", "costs", "weather"],
         )
 
-        expected_evset = from_pandas(new_df, index_names=["sales"])
+        expected_evset = from_pandas(new_df, indexes=["sales"])
 
         output = rename(
             input=self.input_node,
             features={"sales": "store_id"},
-            index={"store_id": "sales"},
+            indexes={"store_id": "sales"},
         )
         impl = RenameNumpyImplementation(output.creator)
         renamed_evset = impl.call(input=self.input_evset)["output"]
 
         self.assertEqual(renamed_evset, expected_evset)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/resample_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/resample_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,38 +35,38 @@
                     "timestamp": [1, 5, 8, 9, 1, 1],
                     "a": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0],
                     "b": [5, 6, 7, 8, 9, 10],
                     "c": ["A", "B", "C", "D", "E", "F"],
                     "x": [1, 1, 1, 1, 2, 2],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
 
         sampling_evset = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [-1, 1, 6, 10, 2, 2, 1],
                     "x": [1, 1, 1, 1, 2, 2, 3],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
 
         expected_output = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [-1, 1, 6, 10, 2, 2, 1],
                     "a": [math.nan, 1.0, 2.0, 4.0, 6.0, 6.0, math.nan],
                     "b": [0, 5, 6, 8, 10, 10, 0],
                     "c": ["", "A", "B", "D", "F", "F", ""],
                     "x": [1, 1, 1, 1, 2, 2, 3],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
 
         # Run op
         op = Resample(input=evset.node(), sampling=sampling_evset.node())
         op.outputs["output"].check_same_sampling(sampling_evset.node())
         instance = ResampleNumpyImplementation(op)
         output = instance.call(input=evset, sampling=sampling_evset)["output"]
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/select_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/select_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from absl.testing import absltest
 
 import numpy as np
 import pandas as pd
 
-from temporian.core.evaluation import evaluate
+from temporian.core.evaluation import run
 from temporian.core.operators.select import SelectOperator
 from temporian.implementation.numpy.operators import select
 from temporian.io.pandas import from_pandas
 
 
 class SelectOperatorTest(absltest.TestCase):
     """Select operator test."""
@@ -41,15 +41,15 @@
                 [self.C, 6.0, 15.0, -6.0, np.nan],
             ],
             columns=["store_id", "timestamp", "sales", "costs", "weather"],
         )
 
         self.features = ["sales", "costs", "weather"]
 
-        self.input_evset = from_pandas(df, index_names=["store_id"])
+        self.input_evset = from_pandas(df, indexes=["store_id"])
         self.input_node = self.input_evset.node()
 
     def test_select_one_feature(self) -> None:
         """Test correct select operator for one feature selection."""
         new_df = pd.DataFrame(
             [
                 [self.A, 1.0, 10.0],
@@ -66,15 +66,15 @@
             input=self.input_node, feature_names=["sales"]
         )
         operator.outputs["output"].check_same_sampling(self.input_node)
 
         impl = select.SelectNumpyImplementation(operator)
         output_evset = impl.call(input=self.input_evset)["output"]
 
-        expected_evset = from_pandas(new_df, index_names=["store_id"])
+        expected_evset = from_pandas(new_df, indexes=["store_id"])
 
         self.assertTrue(output_evset == expected_evset)
 
     def test_select_multiple_features(self) -> None:
         """Test correct select operator for multiple features selection."""
         new_df = pd.DataFrame(
             [
@@ -90,15 +90,15 @@
 
         operator = SelectOperator(
             input=self.input_node, feature_names=["sales", "costs"]
         )
         impl = select.SelectNumpyImplementation(operator)
         output_evset = impl.call(input=self.input_evset)["output"]
 
-        expected_evset = from_pandas(new_df, index_names=["store_id"])
+        expected_evset = from_pandas(new_df, indexes=["store_id"])
 
         self.assertTrue(output_evset == expected_evset)
 
     def test_select_with_core(self) -> None:
         """Test correct select operator with core."""
         new_df = pd.DataFrame(
             [
@@ -107,17 +107,17 @@
                 [self.B, 3.0, 12.0],
                 [self.B, 4.0, 13.0],
                 [self.C, 5.0, 14.0],
                 [self.C, 6.0, 15.0],
             ],
             columns=["store_id", "timestamp", "sales"],
         )
-        expected_evset = from_pandas(new_df, index_names=["store_id"])
+        expected_evset = from_pandas(new_df, indexes=["store_id"])
 
-        output_evset = evaluate(
+        output_evset = run(
             self.input_node["sales"],
             input={
                 self.input_node: self.input_evset,
             },
         )
 
         self.assertEqual(expected_evset, output_evset)
@@ -131,17 +131,17 @@
                 [self.B, 3.0, 12.0, -3.0],
                 [self.B, 4.0, 13.0, -4.0],
                 [self.C, 5.0, 14.0, np.nan],
                 [self.C, 6.0, 15.0, -6.0],
             ],
             columns=["store_id", "timestamp", "sales", "costs"],
         )
-        expected_evset = from_pandas(new_df, index_names=["store_id"])
+        expected_evset = from_pandas(new_df, indexes=["store_id"])
 
-        output_evset = evaluate(
+        output_evset = run(
             self.input_node[["sales", "costs"]],
             input={
                 self.input_node: self.input_evset,
             },
         )
 
         self.assertEqual(expected_evset, output_evset)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/simple_moving_average_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/simple_moving_average_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                     ["X2", "Y1", 15.0, 3.1],
                     ["X2", "Y2", 16.0, 1.2],
                     ["X2", "Y2", 17.0, 2.2],
                     ["X2", "Y2", 18.0, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         op = SimpleMovingAverageOperator(
             input=evset.node(),
             window_length=5.0,
             sampling=None,
         )
@@ -182,15 +182,15 @@
                     ["X2", "Y1", 14.0, 3.1],
                     ["X2", "Y2", 16.0, 1.2],
                     ["X2", "Y2", 16.5, 2.2],
                     ["X2", "Y2", 17.0, 3.2],
                 ],
                 columns=["x", "y", "a", "timestamp"],
             ),
-            index_names=["x", "y"],
+            indexes=["x", "y"],
         )
 
         self.assertEqual(output["output"], expected_output)
 
     def test_with_sampling(self):
         """Event sets with user provided sampling."""
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/since_last_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/since_last_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,27 +34,27 @@
         event_data = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 5, 8, 9, 1, 1, 2],
                     "x": [1, 1, 1, 1, 2, 2, 2],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
         event = event_data.node()
 
         expected_output = from_pandas(
             pd.DataFrame(
                 {
                     "timestamp": [1, 5, 8, 9, 1, 1, 2],
                     "x": [1, 1, 1, 1, 2, 2, 2],
                     "since_last": [nan, 4, 3, 1, nan, 0, 1],
                 }
             ),
-            index_names=["x"],
+            indexes=["x"],
         )
 
         # Run op
         op = SinceLast(input=event)
         op.outputs["output"].check_same_sampling(event)
 
         instance = SinceLastNumpyImplementation(op)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/test_util.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/test_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,42 +11,47 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.implementation.numpy.operators.base import OperatorImplementation
 from temporian.core.operators.base import Operator
-from temporian.core.serialization import serialize
+from temporian.core import serialization
 
 
 def assertEqualEventSet(self, real: EventSet, expected: EventSet):
     """Asserts the equality between real and expected.
 
     Prints a nice message in case of error.
     """
 
     self.assertEqual(
         real,
         expected,
-        f"\nREAL:\n{real}\nEXPECTED:\n{expected}",
+        (
+            "\n==========\nREAL:\n==========\n"
+            f"{real}"
+            "\n==========\nEXPECTED:\n==========\n"
+            f"{expected}"
+        ),
     )
 
 
 def testOperatorAndImp(self, op: Operator, imp: OperatorImplementation):
     """Tests an operator and its implementation.
 
     Currently test:
       - Serialization / unserialization of the operator.
     """
 
     # TODO: Add tests related to the implementation.
     del imp
 
-    serialized_op = serialize._serialize_operator(op)
+    serialized_op = serialization._serialize_operator(op)
 
     nodes = {}
     for node in op.inputs.values():
-        nodes[serialize._identifier(node)] = node
+        nodes[serialization._identifier(node)] = node
     for node in op.outputs.values():
-        nodes[serialize._identifier(node)] = node
+        nodes[serialization._identifier(node)] = node
 
-    _ = serialize._unserialize_operator(serialized_op, nodes)
+    _ = serialization._unserialize_operator(serialized_op, nodes)
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/tick_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/tick_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/test/unary_test.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/test/unary_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     NotNanNumpyImplementation,
     InvertOperator,
     AbsOperator,
     LogOperator,
     IsNanOperator,
     NotNanOperator,
 )
-from temporian.core.data.dtypes.dtype import DType
+from temporian.core.data.dtype import DType
 from temporian.io.pandas import from_pandas
 from temporian.implementation.numpy.operators.test.test_util import (
     assertEqualEventSet,
 )
 
 
 class UnaryNumpyImplementationTest(absltest.TestCase):
@@ -65,15 +65,15 @@
                     "store_id",
                     "product_id",
                     "timestamp",
                     "boolean_1",
                     "boolean_2",
                 ],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         # Expected event set after invert
         # 2 index columns, 2 boolean features
         self.expected_evset = from_pandas(
             pd.DataFrame(
                 data=[
@@ -90,15 +90,15 @@
                     "store_id",
                     "product_id",
                     "timestamp",
                     "boolean_1",
                     "boolean_2",
                 ],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         self.input_node = input_node(
             [("boolean_1", DType.BOOLEAN), ("boolean_2", DType.BOOLEAN)],
             indexes=[("store_id", DType.INT64), ("product_id", DType.INT64)],
         )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/tick.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/tick.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         super().__init__(operator)
 
     def __call__(self, input: EventSet) -> Dict[str, EventSet]:
         assert isinstance(self.operator, Tick)
 
         output_schema = self.output_schema("output")
 
-        # create output event set
+        # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
 
-        # fill output event set data
+        # fill output EventSet data
         for index_key, index_data in input.data.items():
             if len(index_data.timestamps) == 0:
                 dst_timestamps = np.array([], dtype=np.float64)
             else:
                 begin = index_data.timestamps[0]
                 end = index_data.timestamps[-1]
 
@@ -60,18 +60,22 @@
                 dst_timestamps = np.arange(
                     begin,
                     np.nextafter(end, math.inf),
                     self.operator.interval,
                     dtype=np.float64,
                 )
 
-            output_evset[index_key] = IndexData(
-                [],
-                dst_timestamps,
-                schema=output_schema,
+            output_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [],
+                    dst_timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": output_evset}
 
 
 implementation_lib.register_operator_implementation(
     Tick, TickNumpyImplementation
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/unary.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/unary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 from typing import Dict
 
 import numpy as np
 
-from temporian.core.operators.unary.unary import (
+from temporian.core.operators.unary import (
     BaseUnaryOperator,
     AbsOperator,
     InvertOperator,
     NotNanOperator,
     IsNanOperator,
     LogOperator,
 )
@@ -26,21 +26,25 @@
 
         output_schema = self.output_schema("output")
         dst_evset = EventSet(
             data={},
             schema=output_schema,
         )
         for index_key, index_data in input.data.items():
-            dst_evset[index_key] = IndexData(
-                [
-                    self._do_operation(feature)
-                    for feature in index_data.features
-                ],
-                index_data.timestamps,
-                schema=output_schema,
+            dst_evset.set_index_value(
+                index_key,
+                IndexData(
+                    [
+                        self._do_operation(feature)
+                        for feature in index_data.features
+                    ],
+                    index_data.timestamps,
+                    schema=output_schema,
+                ),
+                normalize=False,
             )
 
         return {"output": dst_evset}
 
     @abstractmethod
     def _do_operation(self, feature: np.ndarray) -> np.ndarray:
         """
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/unique_timestamps.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/unique_timestamps.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_count.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_min.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from temporian.core.operators.window.moving_count import (
-    MovingCountOperator,
+from temporian.core.operators.window.moving_min import (
+    MovingMinOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.window.base import (
     BaseWindowNumpyImplementation,
 )
 from temporian.implementation.numpy_cc.operators import operators_cc
 
 
-class MovingCountNumpyImplementation(BaseWindowNumpyImplementation):
-    """Numpy implementation of the moving count operator."""
+class MovingMinNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the moving min operator."""
 
     def _implementation(self):
-        return operators_cc.moving_count
+        return operators_cc.moving_min
 
 
 implementation_lib.register_operator_implementation(
-    MovingCountOperator, MovingCountNumpyImplementation
+    MovingMinOperator, MovingMinNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_max.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_sum.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from temporian.core.operators.window.moving_max import (
-    MovingMaxOperator,
+from temporian.core.operators.window.moving_sum import (
+    MovingSumOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.window.base import (
     BaseWindowNumpyImplementation,
 )
 from temporian.implementation.numpy_cc.operators import operators_cc
 
 
-class MovingMaxNumpyImplementation(BaseWindowNumpyImplementation):
-    """Numpy implementation of the moving max operator."""
+class MovingSumNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the moving sum operator."""
 
     def _implementation(self):
-        return operators_cc.moving_max
+        return operators_cc.moving_sum
 
 
 implementation_lib.register_operator_implementation(
-    MovingMaxOperator, MovingMaxNumpyImplementation
+    MovingSumOperator, MovingSumNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_min.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/moving_standard_deviation.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from temporian.core.operators.window.moving_min import (
-    MovingMinOperator,
+from temporian.core.operators.window.moving_standard_deviation import (
+    MovingStandardDeviationOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.window.base import (
     BaseWindowNumpyImplementation,
 )
 from temporian.implementation.numpy_cc.operators import operators_cc
 
 
-class MovingMinNumpyImplementation(BaseWindowNumpyImplementation):
-    """Numpy implementation of the moving min operator."""
+class MovingStandardDeviationNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the moving standard deviation operator."""
 
     def _implementation(self):
-        return operators_cc.moving_min
+        return operators_cc.moving_standard_deviation
 
 
 implementation_lib.register_operator_implementation(
-    MovingMinOperator, MovingMinNumpyImplementation
+    MovingStandardDeviationOperator, MovingStandardDeviationNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/operators/window/moving_standard_deviation.py` & `temporian-0.1.2/temporian/implementation/numpy/operators/window/simple_moving_average.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from temporian.core.operators.window.moving_standard_deviation import (
-    MovingStandardDeviationOperator,
+from temporian.core.operators.window.simple_moving_average import (
+    SimpleMovingAverageOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.window.base import (
     BaseWindowNumpyImplementation,
 )
 from temporian.implementation.numpy_cc.operators import operators_cc
 
 
-class MovingStandardDeviationNumpyImplementation(BaseWindowNumpyImplementation):
-    """Numpy implementation of the moving standard deviation operator."""
+class SimpleMovingAverageNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the simple moving average operator."""
 
     def _implementation(self):
-        return operators_cc.moving_standard_deviation
+        return operators_cc.simple_moving_average
 
 
 implementation_lib.register_operator_implementation(
-    MovingStandardDeviationOperator, MovingStandardDeviationNumpyImplementation
+    SimpleMovingAverageOperator, SimpleMovingAverageNumpyImplementation
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy/test/registered_operators_test.py` & `temporian-0.1.2/temporian/implementation/numpy/test/registered_operators_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,26 +39,28 @@
             "CALENDAR_SECOND",
             "CALENDAR_YEAR",
             "CAST",
             "DIVISION",
             "DIVISION_SCALAR",
             "DROP_INDEX",
             "END",
+            "ENUMERATE",
             "EQUAL",
             "EQUAL_SCALAR",
             "FILTER",
             "FLOORDIV",
             "FLOORDIV_SCALAR",
             "GLUE",
             "GREATER",
             "GREATER_EQUAL",
             "GREATER_EQUAL_SCALAR",
             "GREATER_SCALAR",
             "INVERT",
             "IS_NAN",
+            "JOIN",
             "LAG",
             "LEAK",
             "LESS",
             "LESS_EQUAL",
             "LESS_EQUAL_SCALAR",
             "LESS_SCALAR",
             "LOG",
@@ -83,14 +85,15 @@
             "RESAMPLE",
             "SELECT",
             "SIMPLE_MOVING_AVERAGE",
             "SINCE_LAST",
             "SUBTRACTION",
             "SUBTRACTION_SCALAR",
             "TICK",
+            "TIMESTAMPS",
             "UNIQUE_TIMESTAMPS",
             "XOR",
         ]
 
         self.assertEqual(
             expected_implementations,
             sorted(list(set(expected_implementations))),
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy_cc/__init__.py` & `temporian-0.1.2/temporian/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy_cc/operators/BUILD` & `temporian-0.1.2/temporian/implementation/numpy_cc/operators/BUILD`

 * *Files 13% similar despite different names*

```diff
@@ -19,21 +19,28 @@
 
 pybind_library(
     name = "resample",
     srcs = ["resample.cc"],
     hdrs = ["resample.h"],
 )
 
+pybind_library(
+    name = "join",
+    srcs = ["join.cc"],
+    hdrs = ["join.h"],
+)
+
 pybind_extension(
     name = "operators_cc",
     srcs = ["pyinit.cc"],
     deps = [
         ":resample",
         ":since_last",
         ":window",
+        ":join",
     ],
 )
 
 py_library(
     name = "operators_cc",
     data = [":operators_cc.so"],
 )
```

### Comparing `temporian-0.1.1/temporian/implementation/numpy_cc/operators/resample.cc` & `temporian-0.1.2/temporian/implementation/numpy_cc/operators/resample.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy_cc/operators/since_last.cc` & `temporian-0.1.2/temporian/implementation/numpy_cc/operators/since_last.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/implementation/numpy_cc/operators/window.cc` & `temporian-0.1.2/temporian/implementation/numpy_cc/operators/window.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/io/BUILD` & `temporian-0.1.2/temporian/beam/test/BUILD`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 package(
     default_visibility = ["//visibility:public"],
     licenses = ["notice"],
 )
 
-# Libraries
-# =========
+# Tests
+# =====
 
-py_library(
-    name = "io",
-    srcs = ["__init__.py"],
+py_test(
+    name = "io_test",
+    srcs = ["io_test.py"],
+    data = ["//temporian/test/test_data"],
     srcs_version = "PY3",
     deps = [
-        ":api_symbols",
-        ":csv",
-        ":pandas",
+        # already_there/absl/testing:absltest
+        "//temporian/beam:io",
+        "//temporian/core/data:node",
+        "//temporian/core/data:dtype",
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/io:csv",
     ],
 )
 
-py_library(
-    name = "api_symbols",
-    srcs = ["api_symbols.py"],
+py_test(
+    name = "evaluation_test",
+    srcs = ["evaluation_test.py"],
     srcs_version = "PY3",
     deps = [
-        ":csv",
-        ":pandas",
+        # already_there/absl/testing:absltest
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/beam/test:utils",
+        "//temporian/core/operators:select",
+        "//temporian/core/operators/window:moving_sum",
     ],
 )
 
-py_library(
-    name = "csv",
-    srcs = ["csv.py"],
-    srcs_version = "PY3",
-    deps = [
-        # already_there/pandas
-        ":pandas",
-        "//temporian/implementation/numpy/data:event_set",
-    ],
-)
+# Libraries
+# =========
 
 py_library(
-    name = "pandas",
-    srcs = ["pandas.py"],
+    name = "utils",
+    srcs = ["utils.py"],
     srcs_version = "PY3",
     deps = [
-        # already_there/pandas
-        # already_there/numpy
+        # already_there/apache_beam
+        "//temporian/beam:io",
+        "//temporian/beam:evaluation",
+        "//temporian/io:csv",
+        "//temporian/core/data:node",
         "//temporian/implementation/numpy/data:event_set",
-        "//temporian/implementation/numpy/data:io",
+        "//temporian/implementation/numpy/operators/test:test_util",
     ],
 )
```

### Comparing `temporian-0.1.1/temporian/io/api_symbols.py` & `temporian-0.1.2/temporian/io/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint: disable=unused-import
+"""Input/output functions."""
 
 from temporian.io.csv import to_csv
 from temporian.io.csv import from_csv
 
 from temporian.io.pandas import to_pandas
 from temporian.io.pandas import from_pandas
```

### Comparing `temporian-0.1.1/temporian/io/csv.py` & `temporian-0.1.2/temporian/io/csv.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,62 +8,90 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utility for reading an event set from disk."""
+"""Utilities for reading and saving EventSets from/to disk."""
 
 from typing import List, Optional
 from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.io.pandas import from_pandas, to_pandas
 
 
 def from_csv(
     path: str,
-    timestamp_column: str,
-    index_names: Optional[List[str]] = None,
+    timestamps: str = "timestamp",
+    indexes: Optional[List[str]] = None,
     sep: str = ",",
 ) -> EventSet:
-    """Reads an EventSet from a file.
+    """Reads an [`EventSet`][temporian.EventSet] from a CSV file.
+
+    Example:
+        ```python
+        >>> # Example CSV
+        >>> temp_file = tmp_dir / "temporal_data.csv"
+        >>> _ = open(temp_file, "w").write(
+        ...     "date,feature_1,feature_2\\n"
+        ...     "2023-01-01,10.0,3.0\\n"
+        ...     "2023-01-02,20.0,4.0\\n"
+        ...     "2023-02-01,30.0,5.0"
+        ... )
+        >>> # Load CSV
+        >>> evset = tp.from_csv(temp_file, timestamps="date")
+        >>> evset
+        indexes: []
+        features: [('feature_1', float64), ('feature_2', float64)]
+        events:
+            (3 events):
+                timestamps: [1.6725e+09 1.6726e+09 1.6752e+09]
+                'feature_1': [10. 20. 30.]
+                'feature_2': [3. 4. 5.]
+        ...
+
+        ```
 
     Args:
         path: Path to the file.
-        timestamp_column: Name of the column to be used as timestamps for the
-            event set.
-        index_names: Names of the columns to be used as index for the event set.
-            If None, a flat event set will be created.
+        timestamps: Name of the column to be used as timestamps for the
+            EventSet.
+        indexes: Names of the columns to be used as indexes for the EventSet.
+            If None, a flat EventSet will be created.
         sep: Separator to use.
 
-
     Returns:
         EventSet read from file.
-
     """
 
     import pandas as pd
 
-    if index_names is None:
-        index_names = []
+    if indexes is None:
+        indexes = []
 
     df = pd.read_csv(path, sep=sep)
-    return from_pandas(
-        df, index_names=index_names, timestamp_column=timestamp_column
-    )
+    return from_pandas(df, indexes=indexes, timestamps=timestamps)
 
 
 def to_csv(
     evset: EventSet,
     path: str,
     sep: str = ",",
     na_rep: Optional[str] = None,
     columns: Optional[List[str]] = None,
 ):
-    """Saves an EventSet to a file.
+    """Saves an [`EventSet`][temporian.EventSet] to a CSV file.
+
+    Example:
+        ```python
+        >>> output_path = tmp_dir / "output_data.csv"
+        >>> evset = tp.event_set(timestamps=[1,], features={"f1": [0.1]})
+        >>> tp.to_csv(evset, output_path)
+
+        ```
 
     Args:
         evset: EventSet to save.
         path: Path to the file.
         sep: Separator to use.
         na_rep: Representation to use for missing values.
         columns: Columns to save. If `None`, saves all columns.
```

### Comparing `temporian-0.1.1/temporian/io/pandas.py` & `temporian-0.1.2/temporian/io/pandas.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,94 +8,129 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utility for reading an event set from disk."""
+"""Utilities for converting EventSets to pandas DataFrames and viceversa."""
 
 import numpy as np
 
 from typing import List, Optional
 from temporian.implementation.numpy.data.event_set import EventSet
 from temporian.implementation.numpy.data.io import event_set
+from temporian.core.data.dtype import DType
 
 
 # TODO: Rename argument `index_names` to `index_features`.
 def from_pandas(
     df: "pandas.DataFrame",
-    index_names: Optional[List[str]] = None,
-    timestamp_column: str = "timestamp",
+    indexes: Optional[List[str]] = None,
+    timestamps: str = "timestamp",
     name: Optional[str] = None,
     same_sampling_as: Optional[EventSet] = None,
 ) -> EventSet:
-    """Converts a Pandas DataFrame into an EventSet.
+    """Converts a Pandas DataFrame into an [`EventSet`][temporian.EventSet].
 
-    The column `timestamp_column` (default to "timestamp") contains the
-    timestamps. Columns `index_names` (default to `None`, equivalent to `[]`),
-    contains the index. The remaining columns are converted into features.
+    The column `timestamps` (defaults to "timestamp") contains the
+    timestamps. Columns `indexes` (default to `None`, equivalent to `[]`),
+    contains the indexes. The remaining columns are converted into features.
 
     See [`tp.event_set()`][temporian.event_set] for the list of supported
     timestamp and feature types.
 
     Usage example:
-
         ```python
         >>> df = pd.DataFrame(
         ...     data=[
         ...         [1.0, 5, "A"],
         ...         [2.0, 6, "A"],
         ...         [3.0, 7, "B"],
         ...     ],
         ...     columns=["timestamp", "feature_1", "feature_2"],
         ... )
-        >>> evset = tp.from_pandas(df, index_names=["feature_2"])
+        >>> evset = tp.from_pandas(df, indexes=["feature_2"])
 
         ```
 
     Args:
         df: A non indexed Pandas dataframe.
-        index_names: Names of the features to use as index. If empty
-            (default), the data is not indexed. Only integer and string features
-            can be used as index.
-        timestamp_column: Name of the column containing the timestamps. See
+        indexes: Names of the columns to use as indexes. If empty
+            (default), the data is not indexed. Only integer and string columns
+            can be used as indexes.
+        timestamps: Name of the column containing the timestamps. See
             [`tp.event_set()`][temporian.event_set] for the list of supported
             timestamp types.
-        name: Optional name of the event set. Used for debugging, and
+        name: Optional name of the EventSet. Used for debugging, and
             graph serialization.
-        same_sampling_as: If set, the new event set is cheched and tagged as
+        same_sampling_as: If set, the new EventSet is cheched and tagged as
             having the same sampling as `same_sampling_as`. Some operators,
             such as [`tp.filter()`][temporian.filter], require their inputs to
             have the same sampling.
 
     Returns:
-        An event set.
+        An EventSet.
 
     Raises:
-        ValueError: If `index_names` or `timestamp_column` are not in `df`'s
+        ValueError: If `indexes` or `timestamps` are not in `df`'s
             columns.
         ValueError: If a column has an unsupported dtype.
     """
 
-    feature_dict = df.drop(columns=timestamp_column).to_dict("series")
+    feature_dict = df.drop(columns=timestamps).to_dict("series")
 
     return event_set(
-        timestamps=df[timestamp_column].to_numpy(copy=True),
+        timestamps=df[timestamps].to_numpy(copy=True),
         features={k: v.to_numpy(copy=True) for k, v in feature_dict.items()},
-        index_features=index_names,
+        indexes=indexes,
         name=name,
         same_sampling_as=same_sampling_as,
     )
 
 
 def to_pandas(
-    evset: EventSet,
+    evset: EventSet, tp_string_to_pd_string: bool = True
 ) -> "pandas.DataFrame":
-    """Converts an EventSet to a pandas DataFrame.
+    """Converts an [`EventSet`][temporian.EventSet] to a pandas DataFrame.
+
+    Usage example:
+        ```python
+        >>> from datetime import datetime
+
+        >>> evset = tp.event_set(
+        ...     timestamps=[datetime(2015, 1, 1), datetime(2015, 1, 2)],
+        ...     features={
+        ...         "feature_1": [0.5, 0.6],
+        ...         "my_index": ["red", "red"],
+        ...     },
+        ...     indexes=["my_index"],
+        ... )
+
+        # Indices are not set as dataframe's indices and dates are unix timestamps
+        >>> df = tp.to_pandas(evset)
+        >>> df
+        my_index   feature_1     timestamp
+        0       red        0.5  1.420070e+09
+        1       red        0.6  1.420157e+09
+
+        # Set index/date manually in pandas
+        >>> df["timestamp"] = pd.to_datetime(df["timestamp"], unit='s')
+        >>> df.set_index("my_index")
+                    feature_1  timestamp
+        my_index
+        red         0.5     2015-01-01
+        red         0.6     2015-01-02
+
+        ```
+
+    Args:
+        evset: Input event set.
+        tp_string_to_pd_string: If true, cast Temporian strings (equivalent to
+            np.string_ or np.bytes) to Pandas strings (equivalent to np.str_).
 
     Returns:
         DataFrame created from EventSet.
     """
 
     import pandas as pd
 
@@ -118,8 +153,17 @@
 
         # Indexes
         num_timestamps = len(data.timestamps)
         for index_name, index_item in zip(index_names, index):
             dst[index_name].append(np.repeat(index_item, num_timestamps))
 
     dst = {k: np.concatenate(v) for k, v in dst.items()}
+
+    if tp_string_to_pd_string:
+        for feature in evset.schema.features:
+            if feature.dtype == DType.STRING:
+                dst[feature.name] = dst[feature.name].astype(str)
+        for index in evset.schema.indexes:
+            if index.dtype == DType.STRING:
+                dst[index.name] = dst[index.name].astype(str)
+
     return pd.DataFrame(dst)
```

### Comparing `temporian-0.1.1/temporian/io/test/pandas_test.py` & `temporian-0.1.2/temporian/io/test/pandas_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,20 +34,18 @@
         )
         expected_evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
         )
 
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
         self.assertEqual(evset, expected_evset)
 
     def test_timestamp_order(self) -> None:
         df = pd.DataFrame(
             [
                 [1.0, 100.0],
@@ -65,49 +63,32 @@
 
         self.assertEqual(evset, expected_evset)
 
     def test_string_column(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, "740"],
-                [666964, 2.0, "B"],
+                [666964, 2.0, np.nan],
                 [574016, 3.0, ""],
             ],
             columns=["product_id", "timestamp", "costs"],
         )
         expected_evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
-                "costs": ["740", "B", ""],
+                "costs": ["740", "nan", ""],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
         )
 
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
         self.assertEqual(evset, expected_evset)
 
-    def test_mixed_types_in_string_column(self) -> None:
-        df = pd.DataFrame(
-            [
-                [666964, 1.0, "740", "A"],
-                [666964, 2.0, "400", 101],
-                [574016, 3.0, np.nan, "B"],
-            ],
-            columns=["product_id", "timestamp", "costs", "sales"],
-        )
-        # not allowed
-        with self.assertRaises(ValueError):
-            from_pandas(
-                df, index_names=["product_id"], timestamp_column="timestamp"
-            )
-
     def test_multiple_string_formats(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, "740", "A", "D"],
                 [666964, 2.0, "400", "B", "E"],
                 [574016, 3.0, "200", "C", "F"],
             ],
@@ -126,19 +107,17 @@
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "str_0": ["740", "400", "200"],
                 "str_1": ["A", "B", "C"],
                 "str_2": ["D", "E", "F"],
             },
-            index_features=["product_id"],
-        )
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
+            indexes=["product_id"],
         )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
         self.assertEqual(evset, expected_evset)
 
     def test_string_in_index(self):
         evset = from_pandas(
             pd.DataFrame(
                 [
@@ -150,15 +129,15 @@
                     ["X2", "Y1", 3.1, 15.0],
                     ["X2", "Y2", 1.2, 16.0],
                     ["X2", "Y2", 2.2, 17.0],
                     ["X2", "Y2", 3.2, 18.0],
                 ],
                 columns=["index_x", "index_y", "timestamp", "costs"],
             ),
-            index_names=["index_x", "index_y"],
+            indexes=["index_x", "index_y"],
         )
         expected_evset = event_set(
             timestamps=[1.0, 2.0, 3.0, 1.1, 2.1, 3.1, 1.2, 2.2, 3.2],
             features={
                 "costs": [10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0, 18.0],
                 "index_x": [
                     "X1",
@@ -179,15 +158,15 @@
                     "Y1",
                     "Y1",
                     "Y2",
                     "Y2",
                     "Y2",
                 ],
             },
-            index_features=["index_x", "index_y"],
+            indexes=["index_x", "index_y"],
         )
         self.assertEqual(evset, expected_evset)
 
     def test_missing_values(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, 740.0],
@@ -199,20 +178,18 @@
 
         expected_evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, np.nan, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
         )
 
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
         self.assertEqual(evset, expected_evset)
         self.assertFalse(evset.schema.is_unix_timestamp)
 
     def test_npdatetime64_index(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, np.datetime64("2022-01-01"), 740.0],
@@ -223,20 +200,18 @@
         )
         expected_evset = event_set(
             timestamps=[1640995200, 1641081600, 1641168000],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
             is_unix_timestamp=True,
         )
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
         # validate
         self.assertEqual(evset, expected_evset)
         self.assertTrue(evset.schema.is_unix_timestamp)
 
     def test_pdTimestamp_index(self) -> None:
         df = pd.DataFrame(
             [
@@ -248,20 +223,18 @@
         )
         expected_evset = event_set(
             timestamps=[1640995200, 1641081600, 1641168000],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
             is_unix_timestamp=True,
         )
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
         # validate
         self.assertEqual(evset, expected_evset)
         self.assertTrue(evset.schema.is_unix_timestamp)
 
     def test_string_timestamp(self) -> None:
         df = pd.DataFrame(
             [
@@ -274,21 +247,19 @@
 
         expected_evset = event_set(
             timestamps=[1640995200, 1641081600, 1641168000],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
             is_unix_timestamp=True,
         )
 
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
         # validate
         self.assertEqual(evset, expected_evset)
         self.assertTrue(evset.schema.is_unix_timestamp)
 
     def test_datetime_index(self) -> None:
         df = pd.DataFrame(
@@ -313,85 +284,75 @@
         )
         expected_evset = event_set(
             timestamps=[1640995200, 1641081600, 1641168000],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
             is_unix_timestamp=True,
         )
 
-        evset = from_pandas(
-            df, index_names=["product_id"], timestamp_column="timestamp"
-        )
+        evset = from_pandas(df, indexes=["product_id"], timestamps="timestamp")
         self.assertEqual(evset, expected_evset)
         self.assertTrue(evset.schema.is_unix_timestamp)
 
     def test_invalid_boolean_timestamp_type(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, False, 740.0],
                 [666964, True, 508.0],
                 [574016, False, 573.0],
             ],
             columns=["product_id", "timestamp", "costs"],
         )
 
         with self.assertRaises(ValueError):
-            from_pandas(
-                df, index_names=["product_id"], timestamp_column="timestamp"
-            )
+            from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
     def test_invalid_string_timestamp_type(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, "A", 740.0],
                 [666964, "B", 508.0],
                 [574016, 1.0, 573.0],
             ],
             columns=["product_id", "timestamp", "costs"],
         )
 
         with self.assertRaises(ValueError):
-            from_pandas(
-                df, index_names=["product_id"], timestamp_column="timestamp"
-            )
+            from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
-    def test_timestamp_column_with_missing_values(self) -> None:
+    def test_timestamps_with_missing_values(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, 740.0],
                 [666964, 2.0, 508.0],
                 [574016, 3.0, 573.0],
                 [574016, None, 573.0],
             ],
             columns=["product_id", "timestamp", "costs"],
         )
 
         with self.assertRaises(ValueError):
-            from_pandas(
-                df, index_names=["product_id"], timestamp_column="timestamp"
-            )
+            from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
-    def test_timestamp_column_with_non_supported_object(self) -> None:
+    def test_timestamps_with_non_supported_object(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, 740.0],
                 [666964, 2.0, 508.0],
                 [574016, 3.0, 573.0],
                 [574016, object(), 573.0],
             ],
             columns=["product_id", "timestamp", "costs"],
         )
 
         with self.assertRaises(ValueError):
-            from_pandas(
-                df, index_names=["product_id"], timestamp_column="timestamp"
-            )
+            from_pandas(df, indexes=["product_id"], timestamps="timestamp")
 
     def test_no_index(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, 740.0],
                 [666964, 2.0, 508.0],
                 [574016, 3.0, 573.0],
@@ -401,15 +362,15 @@
         expected_evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
         )
-        evset = from_pandas(df, index_names=[], timestamp_column="timestamp")
+        evset = from_pandas(df, indexes=[], timestamps="timestamp")
         self.assertEqual(evset, expected_evset)
 
     def test_datetime_in_feature_column(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, np.datetime64("2022-01-01"), 740.0],
                 [666964, np.datetime64("2022-01-02"), 508.0],
@@ -424,15 +385,15 @@
                 "product_id": [666964, 666964, 574016],
                 "costs": np.array(
                     ["2022-01-01", "2022-01-02", "2022-01-03"],
                     dtype="datetime64[s]",
                 ).astype(np.int64),
             },
         )
-        evset = from_pandas(df, index_names=[], timestamp_column="timestamp")
+        evset = from_pandas(df, indexes=[], timestamps="timestamp")
 
         self.assertEqual(evset, expected_evset)
 
     def test_nan_in_string(self) -> None:
         evset = from_pandas(
             pd.DataFrame(
                 {
@@ -440,27 +401,31 @@
                     "x": ["a", math.nan, "b"],
                     "y": [1, 2, 3],
                 }
             )
         )
 
         expected_evset = event_set(
-            timestamps=[1, 2, 3], features={"x": ["a", "", "b"], "y": [1, 2, 3]}
+            timestamps=[1, 2, 3],
+            features={
+                "x": ["a", "nan", "b"],
+                "y": [1, 2, 3],
+            },
         )
 
         self.assertEqual(evset, expected_evset)
 
     def test_evset_to_df(self) -> None:
         evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
         )
 
         expected_df = pd.DataFrame(
             [
                 [666964, 740.0, 1.0],
                 [666964, 508.0, 2.0],
                 [574016, 573.0, 3.0],
@@ -496,15 +461,15 @@
         evset = event_set(
             timestamps=[1.0, 2.0, 3.0, 1.1, 2.1, 3.1, 1.2, 2.2, 3.2],
             features={
                 "sma_a": [10.0, 10.5, 11.0, 13.0, 13.5, 14.0, 16.0, 16.5, 17.0],
                 "x": ["X1", "X1", "X1", "X2", "X2", "X2", "X2", "X2", "X2"],
                 "y": ["Y1", "Y1", "Y1", "Y1", "Y1", "Y1", "Y2", "Y2", "Y2"],
             },
-            index_features=["x", "y"],
+            indexes=["x", "y"],
         )
         expected_df = pd.DataFrame(
             [
                 ["X1", "Y1", 10.0, 1.0],
                 ["X1", "Y1", 10.5, 2.0],
                 ["X1", "Y1", 11.0, 3.0],
                 ["X2", "Y1", 13.0, 1.1],
@@ -523,15 +488,15 @@
     def test_evset_to_df_string_feature(self) -> None:
         evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": ["740.0", "508.0", "573.0"],
             },
-            index_features=["product_id"],
+            indexes=["product_id"],
         )
         expected_df = pd.DataFrame(
             [
                 [666964, "740.0", 1.0],
                 [666964, "508.0", 2.0],
                 [574016, "573.0", 3.0],
             ],
```

### Comparing `temporian-0.1.1/temporian/proto/core.proto` & `temporian-0.1.2/temporian/proto/core.proto`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
  * limitations under the License.
  */
 
 syntax = "proto2";
 
 package temporian.proto;
 
-// A graph defines a set of processing operations and holds all Node,
+// A graph defines a set of processing operations and holds all EventSetNode,
 // Feature and Sampling instances.
 message Graph {
   repeated Operator operators = 1;
 
-  repeated Node nodes = 2;
+  repeated EventSetNode nodes = 2;
 
-  repeated Node.Feature features = 3;
+  repeated EventSetNode.Feature features = 3;
 
-  repeated Node.Sampling samplings = 4;
+  repeated EventSetNode.Sampling samplings = 4;
 
   repeated IOSignature inputs = 5;
 
   repeated IOSignature outputs = 6;
 }
 
 // The input or output of a graph.
@@ -44,23 +44,23 @@
   // Unique identifier of the operator instance.
   optional string id = 1;
 
   // Key of the operator definition.
   optional string operator_def_key = 2;
 
   // Input node ids by key.
-  repeated NodeArgument inputs = 3;
+  repeated EventSetNodeArgument inputs = 3;
 
   // Output node ids by key.
-  repeated NodeArgument outputs = 4;
+  repeated EventSetNodeArgument outputs = 4;
 
   // Constructor attributes.
   repeated Attribute attributes = 5;
 
-  message NodeArgument {
+  message EventSetNodeArgument {
     // Name of the argument.
     optional string key = 1;
 
     optional string node_id = 2;
   }
 
   message Attribute {
@@ -71,15 +71,15 @@
       int64 integer_64 = 2;
       string str = 3;
       double float_64 = 4;
       ListString list_str = 5;
       bool boolean = 6;
       MapStrStr map_str_str = 7;
       ListDType list_dtype = 8;
-
+      bytes bytes_ = 9;
     }
     message ListString{
       repeated string values = 1;
     }
     message MapStrStr{
       map<string, string> values = 1;
     }
@@ -97,15 +97,15 @@
   DTYPE_FLOAT32 = 3;
   DTYPE_INT32 = 4;
   DTYPE_BOOLEAN = 5;
   DTYPE_STRING = 6;
 }
 
 // Connections between operators
-message Node {
+message EventSetNode {
   // Identifier of the node. Should be unique across all the nodes of the
   // graph.
   optional string id = 1;
 
   // Identifier of the sampling ref.
   optional string sampling_id = 2;
 
@@ -201,10 +201,11 @@
       LIST_STRING=3;
       FLOAT_64 = 4;
       BOOL = 5;
       ANY = 6;
       MAP_STR_STR = 7;
       DTYPE = 8;
       LIST_DTYPE = 9;
+      BYTES = 10;
     }
   }
 }
```

### Comparing `temporian-0.1.1/temporian/test/BUILD` & `temporian-0.1.2/temporian/test/BUILD`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,35 @@
         # already_there/bokeh
         # already_there/matplotlib
         "//temporian",
     ],
 )
 
 py_test(
+    name = "api_beam_test",
+    srcs = ["api_beam_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/logging
+        # already_there/absl/testing:absltest
+        # already_there/bokeh
+        # already_there/matplotlib
+        "//temporian",
+        "//temporian/beam",
+    ],
+    data = ["//temporian/test/test_data"],
+)
+
+py_test(
     name = "docstring_test",
     srcs = ["docstring_test.py"],
     srcs_version = "PY3",
     deps = [
         "//temporian",
+        # already_there/absl/testing:absltest
     ],
 )
 
 py_test(
     name = "prototype_test_numpy",
     srcs = ["prototype_test_numpy.py"],
     data = ["//temporian/test/test_data"],
```

### Comparing `temporian-0.1.1/temporian/test/api_test.py` & `temporian-0.1.2/temporian/test/api_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,30 +40,69 @@
         h2 = tp.resample(input=h1, sampling=i2)
         h3 = i1 * 2.0 + 3.0 > 10.0
 
         result = tp.glue(tp.prefix("sma_", h2["f2"]), i2)
 
         result2 = tp.glue(tp.prefix("toto.", h3))
 
-        result_data, result2_data = tp.evaluate(
+        result_data, result2_data = tp.run(
             query=[result, result2],
             input={i1: evset_1, i2: evset_2},
             verbose=2,
         )
-        logging.info("results: %s", result_data)
-        logging.info("result2: %s", result2_data)
 
         with tempfile.TemporaryDirectory() as tempdir:
             result_data.plot(return_fig=True).savefig(
                 os.path.join(tempdir, "p1.png")
             )
             tp.plot([evset_1, evset_2], return_fig=True).savefig(
                 os.path.join(tempdir, "p2.png")
             )
 
+    def test_eager_mode(self):
+        evset_1 = tp.event_set(
+            timestamps=[0.0, 2.0, 4.0, 6.0],
+            features={
+                "f1": [1.0, 2.0, 3.0, 4.0],
+                "f2": [5.0, 6.0, 7.0, 8.0],
+            },
+        )
+
+        evset_2 = tp.event_set(timestamps=[1.0, 2.0, 2.0])
+
+        h1 = tp.simple_moving_average(input=evset_1, window_length=7)
+        h2 = tp.resample(input=h1, sampling=evset_2)
+
+        self.assertTrue(isinstance(h1, tp.EventSet))
+        self.assertTrue(isinstance(h2, tp.EventSet))
+
+        del h1
+
+        h3 = evset_1 * 2.0 + 3.0 > 10.0
+
+        result = tp.glue(tp.prefix("sma_", h2["f2"]), evset_2)
+
+        result2 = tp.glue(tp.prefix("toto.", h3))
+
+        self.assertTrue(isinstance(result, tp.EventSet))
+        self.assertTrue(isinstance(result2, tp.EventSet))
+
+    def test_eager_mixed_args(self):
+        evset = tp.event_set(timestamps=[0.0])
+
+        with self.assertRaises(ValueError):
+            tp.simple_moving_average(
+                evset, window_length=7, sampling=evset.node()
+            )
+
+        with self.assertRaises(ValueError):
+            tp.simple_moving_average(
+                evset.node(), window_length=7, sampling=evset
+            )
+
     def test_pandas(self):
         evset = tp.event_set(
             timestamps=[0.0, 2.0, 4.0, 6.0],
             features={
                 "f1": [1.0, 2.0, 3.0, 4.0],
                 "f2": [5.0, 6.0, 7.0, 8.0],
             },
@@ -75,87 +114,86 @@
 
     def test_serialization(self):
         a = tp.input_node([("f1", tp.float32), ("f2", tp.float32)])
         b = tp.simple_moving_average(input=a, window_length=7)
 
         with tempfile.TemporaryDirectory() as tempdir:
             path = os.path.join(tempdir, "my_graph.tem")
-            tp.save(inputs={"a": a}, outputs={"b": b}, path=path)
+            tp.save_graph(inputs={"a": a}, outputs={"b": b}, path=path)
 
-            inputs, outputs = tp.load(path=path)
+            inputs, outputs = tp.load_graph(path=path)
 
         self.assertSetEqual(set(inputs.keys()), {"a"})
         self.assertSetEqual(set(outputs.keys()), {"b"})
 
     def test_serialization_single_node(self):
         a = tp.input_node(
             [("f1", tp.float32), ("f2", tp.float32)], name="my_source_node"
         )
         b = tp.simple_moving_average(input=a, window_length=7)
         b.name = "my_output_node"
 
         with tempfile.TemporaryDirectory() as tempdir:
             path = os.path.join(tempdir, "my_graph.tem")
-            tp.save(
+            tp.save_graph(
                 inputs=a,
                 outputs=b,
                 path=path,
             )
 
-            inputs, outputs = tp.load(path=path)
+            inputs, outputs = tp.load_graph(path=path)
 
         self.assertSetEqual(set(inputs.keys()), {"my_source_node"})
         self.assertSetEqual(set(outputs.keys()), {"my_output_node"})
 
     def test_serialization_squeeze_loading_results(self):
         a = tp.input_node(
             [("f1", tp.float32), ("f2", tp.float32)],
             name="my_source_node",
         )
         b = tp.simple_moving_average(input=a, window_length=7)
         b.name = "my_output_node"
 
         with tempfile.TemporaryDirectory() as tempdir:
             path = os.path.join(tempdir, "my_graph.tem")
-            tp.save(
+            tp.save_graph(
                 inputs=a,
                 outputs=b,
                 path=path,
             )
 
-            i, o = tp.load(path=path, squeeze=True)
+            i, o = tp.load_graph(path=path, squeeze=True)
 
         self.assertEqual(i.name, "my_source_node")
         self.assertEqual(o.name, "my_output_node")
 
     def test_serialization_infer_inputs(self):
         a = tp.input_node(
             [("f1", tp.float32), ("f2", tp.float32)],
             name="my_source_node",
         )
         b = tp.simple_moving_average(input=a, window_length=7)
         b.name = "my_output_node"
 
         with tempfile.TemporaryDirectory() as tempdir:
             path = os.path.join(tempdir, "my_graph.tem")
-            tp.save(inputs=None, outputs=b, path=path)
+            tp.save_graph(inputs=None, outputs=b, path=path)
 
-            i, o = tp.load(path=path, squeeze=True)
+            i, o = tp.load_graph(path=path, squeeze=True)
 
         self.assertEqual(i.name, "my_source_node")
         self.assertEqual(o.name, "my_output_node")
 
     def test_event_set(self):
-        evset = tp.event_set(
+        tp.event_set(
             timestamps=[1, 2, 3, 4],
             features={
                 "feature_1": [0.5, 0.6, math.nan, 0.9],
                 "feature_2": ["red", "blue", "red", "blue"],
                 "feature_3": [10, -1, 5, 5],
             },
-            index_features=["feature_2"],
+            indexes=["feature_2"],
         )
-        print(evset)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/test/docstring_test.py` & `temporian-0.1.2/temporian/test/docstring_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import sys
 import doctest
 import inspect
 import traceback
+import tempfile
+from pathlib import Path
 
 from absl.testing import absltest
 
 import numpy as np
 import pandas as pd
 import temporian as tp
 
@@ -30,14 +32,17 @@
     >>> print("hello")
     hello
 
     """
 
     def test_docstrings(self):
         tested_modules = set()
+        tmp_dir_handle = tempfile.TemporaryDirectory()
+        tmp_dir = Path(tmp_dir_handle.name)
+
         for api_object in tp.__dict__.values():
             if inspect.ismodule(api_object):
                 module = api_object
             else:
                 module = inspect.getmodule(api_object)
                 if module is None:
                     continue
@@ -45,52 +50,60 @@
             # Avoid testing twice
             module_name = module.__name__
             if "temporian" not in module_name or module_name in tested_modules:
                 continue
 
             tested_modules.add(module.__name__)
             try:
-                # Run with np.pd,tp + module globals as exec context
+                # Run with np,pd,tp + tmp_dir + module globals as exec context
                 _, test_count = doctest.testmod(
                     module,
-                    globs={"np": np, "tp": tp, "pd": pd},
+                    globs={"np": np, "tp": tp, "pd": pd, "tmp_dir": tmp_dir},
                     extraglobs=module.__dict__,
                     # Use ... to match anything and ignore different whitespaces
                     optionflags=doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE,
                     raise_on_error=True,
                     verbose=False,
                 )
                 if test_count:
                     print(f"Tested {test_count} doc examples on: {module_name}")
                 else:
                     print(f"No examples in {module_name}")
 
             # Failure due to mismatch on expected result
             except doctest.DocTestFailure as e:
+                test = e.test
                 ex = e.example
+                lineno = test.lineno + ex.lineno
                 path = inspect.getfile(module)
                 # Re-raise as bazel assertion
                 self.assertEqual(
                     ex.want,
                     e.got,
                     (
-                        f"Docstring example failed on file {path}:{ex.lineno}\n"
+                        f"Docstring example starting at line {lineno} failed"
+                        f" on file {path}\n"
                         f">>> {ex.source}"
                     ),
                 )
 
             # Failure due to exception raised during code execution
             except doctest.UnexpectedException as e:
+                test = e.test
                 ex = e.example
+                lineno = test.lineno + ex.lineno
                 path = inspect.getfile(module)
                 print("\n\nTraceback:")
                 traceback.print_tb(e.exc_info[2], file=sys.stdout)
                 print("\n\n")
+                # pylint: disable=raise-missing-from
                 raise AssertionError(
-                    "Exception running docstring example on file"
-                    f" {path}:{ex.lineno}\n>>> {ex.source}{e.exc_info[0]}:"
+                    "Exception running docstring example starting at line "
+                    f"{lineno} on file {path}\n>>> {ex.source}{e.exc_info[0]}:"
                     f" {e.exc_info[1]}"
-                ) from e
+                )
+                # pylint: enable=raise-missing-from
+        tmp_dir_handle.cleanup()
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.1.1/temporian/test/prototype_test_numpy.py` & `temporian-0.1.2/temporian/test/prototype_test_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pandas as pd
 from absl.testing import absltest
-
-# Even if not used, ensure that all the necessary code is loaded.
 import temporian as tp
 
 
 class PrototypeTest(absltest.TestCase):
     def setUp(self) -> None:
         # store ids
         TRYOLABS_SHOP = 42
@@ -38,15 +36,15 @@
                     [GOOGLE_SHOP, BOOK_ID, 1.0, 7],
                     [GOOGLE_SHOP, BOOK_ID, 2.0, 8],
                     [GOOGLE_SHOP, PIXEL_ID, 0.0, 3],
                     [GOOGLE_SHOP, PIXEL_ID, 1.0, 4],
                 ],
                 columns=["store_id", "product_id", "timestamp", "sales"],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
         self.evset_2 = tp.from_pandas(
             pd.DataFrame(
                 data=[
                     [TRYOLABS_SHOP, MATE_ID, 0.0, -14],
                     [TRYOLABS_SHOP, MATE_ID, 1.0, -15],
@@ -55,15 +53,15 @@
                     [GOOGLE_SHOP, BOOK_ID, 1.0, -7],
                     [GOOGLE_SHOP, BOOK_ID, 2.0, -8],
                     [GOOGLE_SHOP, PIXEL_ID, 0.0, -3],
                     [GOOGLE_SHOP, PIXEL_ID, 1.0, -4],
                 ],
                 columns=["store_id", "product_id", "timestamp", "costs"],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
 
         # TODO: Remove the following line when "from_pandas" support creating
         # event set with shared sampling. Note that "evset_1" and
         # "evset_2" should have the same sampling in this tests.
 
@@ -88,29 +86,29 @@
                     "timestamp",
                     "sales",
                     "costs",
                     "lag[1s]_sales",
                     "negated_sales",
                 ],
             ),
-            index_names=["store_id", "product_id"],
+            indexes=["store_id", "product_id"],
         )
 
     def test_prototype(self) -> None:
         a = tp.glue(self.node_1, self.node_2)
         # create and glue sum feature
         # TODO: Restore when arithmetic operator is fixed.
         # b = tp.glue(a, self.node_1 + self.node_2)
         c = tp.prefix("lag[1s]_", tp.lag(self.node_1, duration=1))
         d = tp.glue(a, tp.resample(c, a))
         sub_sales = tp.prefix("negated_", -self.node_1["sales"])
         e = tp.glue(d, sub_sales)
         output_node = e
 
-        output_evset = tp.evaluate(
+        output_evset = tp.run(
             output_node,
             input={
                 self.node_1: self.evset_1,
                 self.node_2: self.evset_2,
             },
             check_execution=True,
             verbose=2,
```

### Comparing `temporian-0.1.1/temporian/utils/compile.bzl` & `temporian-0.1.2/temporian/utils/compile.bzl`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/utils/string.py` & `temporian-0.1.2/temporian/utils/string.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/temporian/utils/test/string_test.py` & `temporian-0.1.2/temporian/utils/test/string_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.1.1/setup.py` & `temporian-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['temporian',
+ 'temporian.beam',
+ 'temporian.beam.operators',
+ 'temporian.beam.operators.test',
+ 'temporian.beam.operators.window',
+ 'temporian.beam.operators.window.test',
+ 'temporian.beam.test',
  'temporian.core',
  'temporian.core.data',
- 'temporian.core.data.dtypes',
  'temporian.core.data.test',
  'temporian.core.operators',
  'temporian.core.operators.binary',
  'temporian.core.operators.calendar',
  'temporian.core.operators.scalar',
  'temporian.core.operators.test',
- 'temporian.core.operators.unary',
  'temporian.core.operators.window',
- 'temporian.core.serialization',
  'temporian.core.test',
  'temporian.implementation',
  'temporian.implementation.numpy',
  'temporian.implementation.numpy.data',
  'temporian.implementation.numpy.data.test',
  'temporian.implementation.numpy.operators',
  'temporian.implementation.numpy.operators.binary',
@@ -42,26 +45,30 @@
 
 install_requires = \
 ['absl-py>=1.3.0,<2.0.0',
  'matplotlib>=3.7.1,<4.0.0',
  'pandas>=1.5.2,<2.0.0',
  'protobuf>=4.21.12,<5.0.0']
 
+extras_require = \
+{'beam': ['apache-beam>=2.48.0,<3.0.0']}
+
 setup_kwargs = {
     'name': 'temporian',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Temporian is a Python package for feature engineering of temporal data, focusing on preventing common modeling errors and providing a simple and powerful API, a first-class iterative development experience, and efficient and well-tested implementations of common and not-so-common temporal data preprocessing functions.',
-    'long_description': '<img src="https://github.com/google/temporian/blob/main/docs/src/assets/banner.png?raw=true" width="100%" alt="Temporian logo">\n\n![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg) ![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg) [![docs](https://readthedocs.org/projects/temporian/badge/?version=latest)](https://temporian.readthedocs.io/en/latest/?badge=latest)\n\n**Temporian** is a Python package for **feature engineering of temporal data**, focusing on **preventing common modeling errors** and providing a **simple and powerful API**, a first-class **iterative development** experience, and **efficient and well-tested implementations** of common and not-so-common temporal data preprocessing functions.\n\n## Installation\n\nTemporian is available on PyPI. To install it, run:\n\n```shell\npip install temporian\n```\n\n## Getting Started\n\nThis is how a minimal end-to-end example looks like:\n\n```python\nimport temporian as tp\n\n# Load data and create input node.\nevset = tp.from_csv("temporal_data.csv", timestamp_column="date")\nsource = evset.node()\n\n# Apply operators to create a processing graph.\nsma = tp.simple_moving_average(source, window_length=tp.duration.days(7))\n\n# Run the graph.\nresult_evset = sma.evaluate({source: evset})\n\n# Show output.\nprint(result_evset)\nresult_evset.plot()\n```\n\nThis is an example `temporal_data.csv` to use with the code above:\n\n```\ndate,feature_1,feature_2\n2023-01-01,10.0,3.0\n2023-01-02,20.0,4.0\n2023-02-01,30.0,5.0\n```\n\nCheck the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to try it out!\n\n## Key features\n\nThese are what set Temporian apart.\n\n- **Simple and powerful API**: Temporian exports high level operations making processing complex programs short and ready to read.\n- **Flexible data model**: Temporian models temporal data as a sequence of events, supporting non-uniform sampling timestamps seamlessly.\n- **Prevents modeling errors**: Temporian programs are guaranteed not to have future leakage unless explicitly specified, ensuring that models are not trained on future data.\n- **Iterative development**: Temporian can be used to develop preprocessing pipelines in Colab or local notebooks, allowing users to visualize results each step of the way to identify and correct errors early on.\n- **Efficient and well-tested implementations**: Temporian contains efficient and well-tested implementations of a variety of temporal data processing functions. For instance, our implementation of window operators is **x2000** faster than the same function implemented with NumPy.\n- **Wide range of preprocessing functions**: Temporian contains a wide range of preprocessing functions, including moving window operations, lagging, calendar features, arithmetic operations, index manipulation and propagation, resampling, and more. For a full list of the available operators, see the [operators documentation](https://temporian.readthedocs.io/en/stable/reference/).\n\n## Documentation\n\nThe official documentation is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/).\n\n## Contributing\n\nContributions to Temporian are welcome! Check out the [contributing guide](CONTRIBUTING.md) to get started.\n\n## Credits\n\nThis project is a collaboration between Google and [Tryolabs](https://tryolabs.com/).\n',
+    'long_description': '<img src="docs/src/assets/banner.png" width="100%" alt="Temporian logo">\n\n[![pypi](https://img.shields.io/pypi/v/temporian?color=blue)](https://pypi.org/project/temporian/)\n[![docs](https://readthedocs.org/projects/temporian/badge/?version=stable)](https://temporian.readthedocs.io/en/stable/?badge=stable)\n![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg)\n![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg)\n![publish](https://github.com/google/temporian/actions/workflows/publish.yaml/badge.svg)\n\n**Temporian** is a Python library for **feature engineering** 🛠 and **data augmentation** ⚡ of **temporal data** 📈 (e.g. time-series, transactions) in **machine learning applications** 🤖.\n\n> **Warning**\n> Temporian development is in alpha.\n\n## Key features\n\n- Temporian operates natively on **multivariate** and **multi-index time-series** and **time-sequences** data. With Temporian, all temporal data processing is unified.\n\n- Temporian favors **iterative** and **interactive** development in Colab, where users can **easily visualize intermediate results** 📊 each step of the way.\n\n- Temporian introduces a novel mechanism to **prevent unwanted future leakage** and **training/serving skew** 😰. Temporian programs always return the same result in batch and in streaming mode.\n\n- Temporian programs can run seamlessly **in-process** in Python, on **large datasets using [Apache Beam](https://beam.apache.org/)** ☁️, and in **streaming for continuous** data ingestion.\n\n- Temporian\'s core is implemented **in C++** and **highly optimized** 🔥, so large amounts of data can be handled in-process. In some cases, Temporian can provide a speed-up in the order of 1000x compared to other libraries.\n\n## Installation\n\nTemporian is available on [PyPI](https://pypi.org/project/temporian/). To install it, run:\n\n```shell\npip install temporian\n```\n\n## Minimal example\n\nConsider the following dataset.\n\n```shell\n$ head sales.csv\ntimestamp,store,price,count\n2022-01-01 00:00:00+00:00,CA,27.42,61.9\n2022-01-01 00:00:00+00:00,TX,98.55,18.02\n2022-01-02 00:00:00+00:00,CA,32.74,14.93\n2022-01-02 00:00:00+00:00,TX,48.69,83.99\n...\n```\n\nWe compute the weekly sales per store as follows.\n\n```python\nimport temporian as tp\n\ninput_data = tp.from_csv("sales.csv")\n\n# Define a Temporian program\ninput_node = input_data.node()\nper_store = tp.set_index(input_node, "store")\nweekly_sum = tp.moving_sum(per_store["price"], window_length=tp.duration.days(7))\n\n# Execute Temporian program\noutput_data = weekly_sum.run({input_node: input_data})\n\n# Plot the result\noutput_data.plot()\n```\n\n![](docs/src/assets/frontpage_plot.png)\n\nCheck the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to try it out!\n\n## Documentation\n\nThe documentation 📚 is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/). The [3 minutes to Temporian ⏰️](https://temporian.readthedocs.io/en/stable/3_minutes/) is the best way to start.\n\n## Contributing\n\nContributions to Temporian are welcome! Check out the [contributing guide](CONTRIBUTING.md) to get started.\n\n## Credits\n\nTemporian is developed in collaboration between Google and [Tryolabs](https://tryolabs.com/).\n',
     'author': 'Mathieu Guillame-Bert, Braulio Ríos, Guillermo Etchebarne, Ian Spektor, Richard Stotz',
     'author_email': 'gbm@google.com',
     'maintainer': 'Mathieu Guillame-Bert',
     'maintainer_email': 'gbm@google.com',
     'url': 'https://github.com/google/temporian',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8,<3.12',
 }
 from config.build import *
 build(setup_kwargs)
 
 setup(**setup_kwargs)
```

### Comparing `temporian-0.1.1/PKG-INFO` & `temporian-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temporian
-Version: 0.1.1
+Version: 0.1.2
 Summary: Temporian is a Python package for feature engineering of temporal data, focusing on preventing common modeling errors and providing a simple and powerful API, a first-class iterative development experience, and efficient and well-tested implementations of common and not-so-common temporal data preprocessing functions.
 Home-page: https://github.com/google/temporian
 License: Apache 2.0
 Author: Mathieu Guillame-Bert, Braulio Ríos, Guillermo Etchebarne, Ian Spektor, Richard Stotz
 Author-email: gbm@google.com
 Maintainer: Mathieu Guillame-Bert
 Maintainer-email: gbm@google.com
@@ -22,84 +22,98 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: beam
 Requires-Dist: absl-py (>=1.3.0,<2.0.0)
+Requires-Dist: apache-beam (>=2.48.0,<3.0.0) ; extra == "beam"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: protobuf (>=4.21.12,<5.0.0)
 Project-URL: Repository, https://github.com/google/temporian
 Description-Content-Type: text/markdown
 
-<img src="https://github.com/google/temporian/blob/main/docs/src/assets/banner.png?raw=true" width="100%" alt="Temporian logo">
+<img src="docs/src/assets/banner.png" width="100%" alt="Temporian logo">
 
-![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg) ![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg) [![docs](https://readthedocs.org/projects/temporian/badge/?version=latest)](https://temporian.readthedocs.io/en/latest/?badge=latest)
+[![pypi](https://img.shields.io/pypi/v/temporian?color=blue)](https://pypi.org/project/temporian/)
+[![docs](https://readthedocs.org/projects/temporian/badge/?version=stable)](https://temporian.readthedocs.io/en/stable/?badge=stable)
+![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg)
+![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg)
+![publish](https://github.com/google/temporian/actions/workflows/publish.yaml/badge.svg)
 
-**Temporian** is a Python package for **feature engineering of temporal data**, focusing on **preventing common modeling errors** and providing a **simple and powerful API**, a first-class **iterative development** experience, and **efficient and well-tested implementations** of common and not-so-common temporal data preprocessing functions.
+**Temporian** is a Python library for **feature engineering** 🛠 and **data augmentation** ⚡ of **temporal data** 📈 (e.g. time-series, transactions) in **machine learning applications** 🤖.
+
+> **Warning**
+> Temporian development is in alpha.
+
+## Key features
+
+- Temporian operates natively on **multivariate** and **multi-index time-series** and **time-sequences** data. With Temporian, all temporal data processing is unified.
+
+- Temporian favors **iterative** and **interactive** development in Colab, where users can **easily visualize intermediate results** 📊 each step of the way.
+
+- Temporian introduces a novel mechanism to **prevent unwanted future leakage** and **training/serving skew** 😰. Temporian programs always return the same result in batch and in streaming mode.
+
+- Temporian programs can run seamlessly **in-process** in Python, on **large datasets using [Apache Beam](https://beam.apache.org/)** ☁️, and in **streaming for continuous** data ingestion.
+
+- Temporian's core is implemented **in C++** and **highly optimized** 🔥, so large amounts of data can be handled in-process. In some cases, Temporian can provide a speed-up in the order of 1000x compared to other libraries.
 
 ## Installation
 
-Temporian is available on PyPI. To install it, run:
+Temporian is available on [PyPI](https://pypi.org/project/temporian/). To install it, run:
 
 ```shell
 pip install temporian
 ```
 
-## Getting Started
+## Minimal example
+
+Consider the following dataset.
+
+```shell
+$ head sales.csv
+timestamp,store,price,count
+2022-01-01 00:00:00+00:00,CA,27.42,61.9
+2022-01-01 00:00:00+00:00,TX,98.55,18.02
+2022-01-02 00:00:00+00:00,CA,32.74,14.93
+2022-01-02 00:00:00+00:00,TX,48.69,83.99
+...
+```
 
-This is how a minimal end-to-end example looks like:
+We compute the weekly sales per store as follows.
 
 ```python
 import temporian as tp
 
-# Load data and create input node.
-evset = tp.from_csv("temporal_data.csv", timestamp_column="date")
-source = evset.node()
-
-# Apply operators to create a processing graph.
-sma = tp.simple_moving_average(source, window_length=tp.duration.days(7))
-
-# Run the graph.
-result_evset = sma.evaluate({source: evset})
-
-# Show output.
-print(result_evset)
-result_evset.plot()
-```
+input_data = tp.from_csv("sales.csv")
 
-This is an example `temporal_data.csv` to use with the code above:
-
-```
-date,feature_1,feature_2
-2023-01-01,10.0,3.0
-2023-01-02,20.0,4.0
-2023-02-01,30.0,5.0
-```
+# Define a Temporian program
+input_node = input_data.node()
+per_store = tp.set_index(input_node, "store")
+weekly_sum = tp.moving_sum(per_store["price"], window_length=tp.duration.days(7))
 
-Check the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to try it out!
+# Execute Temporian program
+output_data = weekly_sum.run({input_node: input_data})
 
-## Key features
+# Plot the result
+output_data.plot()
+```
 
-These are what set Temporian apart.
+![](docs/src/assets/frontpage_plot.png)
 
-- **Simple and powerful API**: Temporian exports high level operations making processing complex programs short and ready to read.
-- **Flexible data model**: Temporian models temporal data as a sequence of events, supporting non-uniform sampling timestamps seamlessly.
-- **Prevents modeling errors**: Temporian programs are guaranteed not to have future leakage unless explicitly specified, ensuring that models are not trained on future data.
-- **Iterative development**: Temporian can be used to develop preprocessing pipelines in Colab or local notebooks, allowing users to visualize results each step of the way to identify and correct errors early on.
-- **Efficient and well-tested implementations**: Temporian contains efficient and well-tested implementations of a variety of temporal data processing functions. For instance, our implementation of window operators is **x2000** faster than the same function implemented with NumPy.
-- **Wide range of preprocessing functions**: Temporian contains a wide range of preprocessing functions, including moving window operations, lagging, calendar features, arithmetic operations, index manipulation and propagation, resampling, and more. For a full list of the available operators, see the [operators documentation](https://temporian.readthedocs.io/en/stable/reference/).
+Check the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to try it out!
 
 ## Documentation
 
-The official documentation is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/).
+The documentation 📚 is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/). The [3 minutes to Temporian ⏰️](https://temporian.readthedocs.io/en/stable/3_minutes/) is the best way to start.
 
 ## Contributing
 
 Contributions to Temporian are welcome! Check out the [contributing guide](CONTRIBUTING.md) to get started.
 
 ## Credits
 
-This project is a collaboration between Google and [Tryolabs](https://tryolabs.com/).
+Temporian is developed in collaboration between Google and [Tryolabs](https://tryolabs.com/).
```

