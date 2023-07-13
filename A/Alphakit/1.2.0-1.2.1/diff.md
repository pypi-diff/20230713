# Comparing `tmp/Alphakit-1.2.0.tar.gz` & `tmp/Alphakit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Alphakit-1.2.0.tar", last modified: Wed Jul  5 02:50:23 2023, max compression
+gzip compressed data, was "dist/Alphakit-1.2.1.tar", last modified: Thu Jul 13 06:29:33 2023, max compression
```

## Comparing `Alphakit-1.2.0.tar` & `Alphakit-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/Alphakit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-05 02:50:23.000000 Alphakit-1.2.0/Alphakit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-07-05 02:50:23.000000 Alphakit-1.2.0/Alphakit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 02:50:23.000000 Alphakit-1.2.0/Alphakit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-05 02:50:23.000000 Alphakit-1.2.0/Alphakit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 02:50:23.000000 Alphakit-1.2.0/Alphakit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-05 02:25:31.000000 Alphakit-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-05 02:49:36.000000 Alphakit-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-05 02:50:23.000000 Alphakit-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-05 02:25:31.000000 Alphakit-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/alphakit/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-05 02:49:54.000000 Alphakit-1.2.0/alphakit/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117998 2023-07-05 02:41:55.000000 Alphakit-1.2.0/alphakit/const.c
--rw-r--r--   0 root         (0) root         (0)      702 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/const.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/alphakit/data/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)   774588 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/data/calculator.c
--rw-r--r--   0 root         (0) root         (0)     7937 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/data/calculator.pyx
--rw-r--r--   0 root         (0) root         (0)   162253 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/data/processing.c
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/data/processing.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/alphakit/factor/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/factor/__init__.py
--rw-r--r--   0 root         (0) root         (0)   279924 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/factor/analysis.c
--rw-r--r--   0 root         (0) root         (0)     2827 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/factor/analysis.pyx
--rw-r--r--   0 root         (0) root         (0)   359516 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/factor/metrics.c
--rw-r--r--   0 root         (0) root         (0)     4194 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/factor/metrics.pyx
--rw-r--r--   0 root         (0) root         (0)   299502 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/factor/processing.c
--rw-r--r--   0 root         (0) root         (0)     4718 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/factor/processing.pyx
--rw-r--r--   0 root         (0) root         (0)   212245 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/factor/transform.c
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/factor/transform.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/alphakit/portfolio/
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)   147280 2023-07-05 02:41:56.000000 Alphakit-1.2.0/alphakit/portfolio/combine.c
--rw-r--r--   0 root         (0) root         (0)      480 2023-07-05 02:26:44.000000 Alphakit-1.2.0/alphakit/portfolio/combine.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:50:23.000000 Alphakit-1.2.0/requirements/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-05 02:25:31.000000 Alphakit-1.2.0/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 02:50:23.000000 Alphakit-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3356 2023-07-05 02:40:32.000000 Alphakit-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      764 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-13 05:13:18.000000 Alphakit-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-13 06:29:33.000000 Alphakit-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-05 02:25:31.000000 Alphakit-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-13 06:28:35.000000 Alphakit-1.2.1/alphakit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117998 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/const.c
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/const.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/data/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 02:26:44.000000 Alphakit-1.2.1/alphakit/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   774588 2023-07-13 06:26:18.000000 Alphakit-1.2.1/alphakit/data/calculator.c
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/data/calculator.pyx
+-rw-r--r--   0 root         (0) root         (0)   162253 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/data/processing.c
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/data/processing.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/factor/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-05 02:26:44.000000 Alphakit-1.2.1/alphakit/factor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   287606 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/analysis.c
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/analysis.pyx
+-rw-r--r--   0 root         (0) root         (0)   361294 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/metrics.c
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/metrics.pyx
+-rw-r--r--   0 root         (0) root         (0)   299502 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/processing.c
+-rw-r--r--   0 root         (0) root         (0)     4718 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/processing.pyx
+-rw-r--r--   0 root         (0) root         (0)   212245 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/transform.c
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/transform.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/portfolio/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 02:26:44.000000 Alphakit-1.2.1/alphakit/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   147280 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/portfolio/combine.c
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/portfolio/combine.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/requirements/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-05 02:25:31.000000 Alphakit-1.2.1/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 06:29:33.000000 Alphakit-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-07-13 05:13:18.000000 Alphakit-1.2.1/setup.py
```

### Comparing `Alphakit-1.2.0/Alphakit.egg-info/SOURCES.txt` & `Alphakit-1.2.1/Alphakit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./README.md
 Alphakit.egg-info/PKG-INFO
 Alphakit.egg-info/SOURCES.txt
 Alphakit.egg-info/dependency_links.txt
```

### Comparing `Alphakit-1.2.0/alphakit/const.c` & `Alphakit-1.2.1/alphakit/const.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/const.pyx` & `Alphakit-1.2.1/alphakit/const.pyx`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 ]
 BARRA_COUNTRY = ['COUNTRY']
 BRAAR_RISKFACTOR = [
     'BETA', 'MOMENTUM', 'SIZE', 'EARNYILD', 'RESVOL', 'GROWTH', 'BTOP',
     'LEVERAGE', 'LIQUIDTY', 'SIZENL'
 ]
 BARRA_ALL = BARRA_INDUSTRY + BARRA_COUNTRY + BRAAR_RISKFACTOR
-BARRA_SIZEIND = BARRA_INDUSTRY + BARRA_COUNTRY + ['SIZE', 'SIZENL']
+BARRA_SIZEIND = BARRA_INDUSTRY + BARRA_COUNTRY + ['SIZE', 'SIZENL']
```

### Comparing `Alphakit-1.2.0/alphakit/data/calculator.c` & `Alphakit-1.2.1/alphakit/data/calculator.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/data/calculator.pyx` & `Alphakit-1.2.1/alphakit/data/calculator.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/data/processing.c` & `Alphakit-1.2.1/alphakit/data/processing.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/data/processing.pyx` & `Alphakit-1.2.1/alphakit/data/processing.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/factor/analysis.c` & `Alphakit-1.2.1/alphakit/factor/analysis.c`

 * *Files 2% similar despite different names*

```diff
@@ -1023,14 +1023,20 @@
 #define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
 #endif
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
@@ -1272,14 +1278,15 @@
 static const char __pyx_k_outpnl[] = "outpnl";
 static const char __pyx_k_pandas[] = "pandas";
 static const char __pyx_k_pnlplt[] = "pnlplt";
 static const char __pyx_k_usecol[] = "usecol";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_weighT[] = "weighT";
 static const char __pyx_k_weight[] = "weight";
+static const char __pyx_k_checkna[] = "checkna";
 static const char __pyx_k_columns[] = "columns";
 static const char __pyx_k_figsize[] = "figsize";
 static const char __pyx_k_gretplt[] = "gretplt";
 static const char __pyx_k_inplace[] = "inplace";
 static const char __pyx_k_outpnl1[] = "outpnl1";
 static const char __pyx_k_outpnl2[] = "outpnl2";
 static const char __pyx_k_outpnl3[] = "outpnl3";
@@ -1344,14 +1351,15 @@
 static PyObject *__pyx_n_s_ax1;
 static PyObject *__pyx_n_s_ax2;
 static PyObject *__pyx_n_s_ax3;
 static PyObject *__pyx_n_s_ax4;
 static PyObject *__pyx_n_s_axis;
 static PyObject *__pyx_n_s_bins;
 static PyObject *__pyx_n_s_block;
+static PyObject *__pyx_n_s_checkna;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_color;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_concat;
 static PyObject *__pyx_n_s_cumsum;
 static PyObject *__pyx_kp_s_datetime64_ns;
@@ -1437,15 +1445,15 @@
 static PyObject *__pyx_n_s_unstack;
 static PyObject *__pyx_n_s_usecol;
 static PyObject *__pyx_n_s_values;
 static PyObject *__pyx_n_s_weighT;
 static PyObject *__pyx_n_s_weight;
 static PyObject *__pyx_n_s_weightB;
 static PyObject *__pyx_pf_8alphakit_6factor_8analysis_factor_plot(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_gret, PyObject *__pyx_v_outpnl, PyObject *__pyx_v_savepath); /* proto */
-static PyObject *__pyx_pf_8alphakit_6factor_8analysis_2factor_one(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_freq, PyObject *__pyx_v_hold, PyObject *__pyx_v_group, PyObject *__pyx_v_skip, PyObject *__pyx_v_savepath); /* proto */
+static PyObject *__pyx_pf_8alphakit_6factor_8analysis_2factor_one(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_freq, PyObject *__pyx_v_hold, PyObject *__pyx_v_group, PyObject *__pyx_v_skip, PyObject *__pyx_v_checkna, PyObject *__pyx_v_savepath); /* proto */
 static PyObject *__pyx_float_0_2;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_3;
 static PyObject *__pyx_int_9;
 static PyObject *__pyx_int_10;
 static PyObject *__pyx_int_16;
@@ -1880,16 +1888,16 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
     /* "alphakit/factor/analysis.pyx":23
  *         ax2.legend(loc='lower left')
  * 
  *         ax4 = plt.subplot(224)             # <<<<<<<<<<<<<<
- *         gnline = gret['GN'].mean()
- *         gret.drop('GN', axis=1, inplace=True)
+ *         gnline = None
+ *         if 'GN' in gret.columns:
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_plt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_subplot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
@@ -1909,87 +1917,120 @@
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_ax4 = __pyx_t_2;
     __pyx_t_2 = 0;
 
     /* "alphakit/factor/analysis.pyx":24
  * 
  *         ax4 = plt.subplot(224)
- *         gnline = gret['GN'].mean()             # <<<<<<<<<<<<<<
- *         gret.drop('GN', axis=1, inplace=True)
- *         gretplt = pd.DataFrame(gret.mean())
+ *         gnline = None             # <<<<<<<<<<<<<<
+ *         if 'GN' in gret.columns:
+ *             gnline = gret['GN'].mean()
  */
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gret, __pyx_n_s_GN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mean); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_v_gnline = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __Pyx_INCREF(Py_None);
+    __pyx_v_gnline = Py_None;
 
     /* "alphakit/factor/analysis.pyx":25
  *         ax4 = plt.subplot(224)
- *         gnline = gret['GN'].mean()
- *         gret.drop('GN', axis=1, inplace=True)             # <<<<<<<<<<<<<<
- *         gretplt = pd.DataFrame(gret.mean())
- *         gretplt['level'] = 0
+ *         gnline = None
+ *         if 'GN' in gret.columns:             # <<<<<<<<<<<<<<
+ *             gnline = gret['GN'].mean()
+ *             gret.drop('GN', axis=1, inplace=True)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_drop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_columns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_GN, __pyx_t_2, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 25, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_5 = (__pyx_t_4 != 0);
+    if (__pyx_t_5) {
 
-    /* "alphakit/factor/analysis.pyx":26
- *         gnline = gret['GN'].mean()
- *         gret.drop('GN', axis=1, inplace=True)
+      /* "alphakit/factor/analysis.pyx":26
+ *         gnline = None
+ *         if 'GN' in gret.columns:
+ *             gnline = gret['GN'].mean()             # <<<<<<<<<<<<<<
+ *             gret.drop('GN', axis=1, inplace=True)
+ *         gretplt = pd.DataFrame(gret.mean())
+ */
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gret, __pyx_n_s_GN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mean); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+        }
+      }
+      __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF_SET(__pyx_v_gnline, __pyx_t_2);
+      __pyx_t_2 = 0;
+
+      /* "alphakit/factor/analysis.pyx":27
+ *         if 'GN' in gret.columns:
+ *             gnline = gret['GN'].mean()
+ *             gret.drop('GN', axis=1, inplace=True)             # <<<<<<<<<<<<<<
+ *         gretplt = pd.DataFrame(gret.mean())
+ *         gretplt['level'] = 0
+ */
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_drop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+      /* "alphakit/factor/analysis.pyx":25
+ *         ax4 = plt.subplot(224)
+ *         gnline = None
+ *         if 'GN' in gret.columns:             # <<<<<<<<<<<<<<
+ *             gnline = gret['GN'].mean()
+ *             gret.drop('GN', axis=1, inplace=True)
+ */
+    }
+
+    /* "alphakit/factor/analysis.pyx":28
+ *             gnline = gret['GN'].mean()
+ *             gret.drop('GN', axis=1, inplace=True)
  *         gretplt = pd.DataFrame(gret.mean())             # <<<<<<<<<<<<<<
  *         gretplt['level'] = 0
  *         ax4.plot(gretplt, marker='.')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_mean); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_mean); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -1997,290 +2038,310 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_gretplt = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "alphakit/factor/analysis.pyx":27
- *         gret.drop('GN', axis=1, inplace=True)
+    /* "alphakit/factor/analysis.pyx":29
+ *             gret.drop('GN', axis=1, inplace=True)
  *         gretplt = pd.DataFrame(gret.mean())
  *         gretplt['level'] = 0             # <<<<<<<<<<<<<<
  *         ax4.plot(gretplt, marker='.')
- *         po = abs(gretplt[0] - gnline).reset_index(drop=True)
+ *         if gnline is not None:
  */
-    if (unlikely(PyObject_SetItem(__pyx_v_gretplt, __pyx_n_s_level, __pyx_int_0) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_gretplt, __pyx_n_s_level, __pyx_int_0) < 0)) __PYX_ERR(0, 29, __pyx_L1_error)
 
-    /* "alphakit/factor/analysis.pyx":28
+    /* "alphakit/factor/analysis.pyx":30
  *         gretplt = pd.DataFrame(gret.mean())
  *         gretplt['level'] = 0
  *         ax4.plot(gretplt, marker='.')             # <<<<<<<<<<<<<<
- *         po = abs(gretplt[0] - gnline).reset_index(drop=True)
- *         po1 = po.nsmallest(1).index[0]
+ *         if gnline is not None:
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_plot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_plot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_gretplt);
     __Pyx_GIVEREF(__pyx_v_gretplt);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_gretplt);
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_marker, __pyx_kp_s__4) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_marker, __pyx_kp_s__4) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "alphakit/factor/analysis.pyx":29
+    /* "alphakit/factor/analysis.pyx":31
  *         gretplt['level'] = 0
  *         ax4.plot(gretplt, marker='.')
- *         po = abs(gretplt[0] - gnline).reset_index(drop=True)             # <<<<<<<<<<<<<<
- *         po1 = po.nsmallest(1).index[0]
- *         if not np.isnan(gnline):
- */
-    __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_gretplt, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PyNumber_Subtract(__pyx_t_6, __pyx_v_gnline); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_drop, Py_True) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_v_po = __pyx_t_2;
-    __pyx_t_2 = 0;
-
-    /* "alphakit/factor/analysis.pyx":30
- *         ax4.plot(gretplt, marker='.')
- *         po = abs(gretplt[0] - gnline).reset_index(drop=True)
- *         po1 = po.nsmallest(1).index[0]             # <<<<<<<<<<<<<<
- *         if not np.isnan(gnline):
- *             ax4.scatter(po1, gnline, s=150, marker='*', color='green')
- */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_po, __pyx_n_s_nsmallest); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_1);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_int_1) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_int_1);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_v_po1 = __pyx_t_2;
-    __pyx_t_2 = 0;
-
-    /* "alphakit/factor/analysis.pyx":31
- *         po = abs(gretplt[0] - gnline).reset_index(drop=True)
- *         po1 = po.nsmallest(1).index[0]
- *         if not np.isnan(gnline):             # <<<<<<<<<<<<<<
- *             ax4.scatter(po1, gnline, s=150, marker='*', color='green')
- *             ax4.text(po1 + 0.2, gnline, 'GN')
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isnan); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_v_gnline) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_gnline);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 31, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = ((!__pyx_t_4) != 0);
-    if (__pyx_t_5) {
+ *         if gnline is not None:             # <<<<<<<<<<<<<<
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)
+ *             po1 = po.nsmallest(1).index[0]
+ */
+    __pyx_t_5 = (__pyx_v_gnline != Py_None);
+    __pyx_t_4 = (__pyx_t_5 != 0);
+    if (__pyx_t_4) {
 
       /* "alphakit/factor/analysis.pyx":32
- *         po1 = po.nsmallest(1).index[0]
- *         if not np.isnan(gnline):
- *             ax4.scatter(po1, gnline, s=150, marker='*', color='green')             # <<<<<<<<<<<<<<
- *             ax4.text(po1 + 0.2, gnline, 'GN')
- *         group = len(gretplt) - 1
+ *         ax4.plot(gretplt, marker='.')
+ *         if gnline is not None:
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)             # <<<<<<<<<<<<<<
+ *             po1 = po.nsmallest(1).index[0]
+ *             if not np.isnan(gnline):
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_scatter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_gretplt, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_1 = PyNumber_Subtract(__pyx_t_6, __pyx_v_gnline); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_INCREF(__pyx_v_po1);
-      __Pyx_GIVEREF(__pyx_v_po1);
-      PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_po1);
-      __Pyx_INCREF(__pyx_v_gnline);
-      __Pyx_GIVEREF(__pyx_v_gnline);
-      PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_gnline);
-      __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_s, __pyx_int_150) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_marker, __pyx_kp_s__5) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_color, __pyx_n_s_green) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_drop, Py_True) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_v_po = __pyx_t_2;
+      __pyx_t_2 = 0;
 
       /* "alphakit/factor/analysis.pyx":33
- *         if not np.isnan(gnline):
- *             ax4.scatter(po1, gnline, s=150, marker='*', color='green')
- *             ax4.text(po1 + 0.2, gnline, 'GN')             # <<<<<<<<<<<<<<
- *         group = len(gretplt) - 1
- *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
+ *         if gnline is not None:
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)
+ *             po1 = po.nsmallest(1).index[0]             # <<<<<<<<<<<<<<
+ *             if not np.isnan(gnline):
+ *                 ax4.scatter(po1, gnline, s=150, marker='*', color='green')
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_text); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 33, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_po, __pyx_n_s_nsmallest); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 33, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyFloat_AddObjC(__pyx_v_po1, __pyx_float_0_2, 0.2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = NULL;
-      __pyx_t_8 = 0;
+      __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_2)) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
-          __pyx_t_8 = 1;
         }
       }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_6)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_1, __pyx_v_gnline, __pyx_n_s_GN};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_1, __pyx_v_gnline, __pyx_n_s_GN};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 33, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        if (__pyx_t_2) {
-          __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
+      __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_int_1) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_int_1);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_v_po1 = __pyx_t_2;
+      __pyx_t_2 = 0;
+
+      /* "alphakit/factor/analysis.pyx":34
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)
+ *             po1 = po.nsmallest(1).index[0]
+ *             if not np.isnan(gnline):             # <<<<<<<<<<<<<<
+ *                 ax4.scatter(po1, gnline, s=150, marker='*', color='green')
+ *                 ax4.text(po1 + 0.2, gnline, 'GN')
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isnan); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
         }
-        __Pyx_GIVEREF(__pyx_t_1);
-        PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_1);
+      }
+      __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_v_gnline) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_gnline);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 34, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_5 = ((!__pyx_t_4) != 0);
+      if (__pyx_t_5) {
+
+        /* "alphakit/factor/analysis.pyx":35
+ *             po1 = po.nsmallest(1).index[0]
+ *             if not np.isnan(gnline):
+ *                 ax4.scatter(po1, gnline, s=150, marker='*', color='green')             # <<<<<<<<<<<<<<
+ *                 ax4.text(po1 + 0.2, gnline, 'GN')
+ *         group = len(gretplt) - 1
+ */
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_scatter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_INCREF(__pyx_v_po1);
+        __Pyx_GIVEREF(__pyx_v_po1);
+        PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_po1);
         __Pyx_INCREF(__pyx_v_gnline);
         __Pyx_GIVEREF(__pyx_v_gnline);
-        PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_gnline);
-        __Pyx_INCREF(__pyx_n_s_GN);
-        __Pyx_GIVEREF(__pyx_n_s_GN);
-        PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_n_s_GN);
-        __pyx_t_1 = 0;
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+        PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_gnline);
+        __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_s, __pyx_int_150) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_marker, __pyx_kp_s__5) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_color, __pyx_n_s_green) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+        /* "alphakit/factor/analysis.pyx":36
+ *             if not np.isnan(gnline):
+ *                 ax4.scatter(po1, gnline, s=150, marker='*', color='green')
+ *                 ax4.text(po1 + 0.2, gnline, 'GN')             # <<<<<<<<<<<<<<
+ *         group = len(gretplt) - 1
+ *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
+ */
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_text); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_1 = __Pyx_PyFloat_AddObjC(__pyx_v_po1, __pyx_float_0_2, 0.2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_2 = NULL;
+        __pyx_t_8 = 0;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
+          if (likely(__pyx_t_2)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+            __Pyx_INCREF(__pyx_t_2);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_6, function);
+            __pyx_t_8 = 1;
+          }
+        }
+        #if CYTHON_FAST_PYCALL
+        if (PyFunction_Check(__pyx_t_6)) {
+          PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_1, __pyx_v_gnline, __pyx_n_s_GN};
+          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        } else
+        #endif
+        #if CYTHON_FAST_PYCCALL
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
+          PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_1, __pyx_v_gnline, __pyx_n_s_GN};
+          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        } else
+        #endif
+        {
+          __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 36, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          if (__pyx_t_2) {
+            __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
+          }
+          __Pyx_GIVEREF(__pyx_t_1);
+          PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_1);
+          __Pyx_INCREF(__pyx_v_gnline);
+          __Pyx_GIVEREF(__pyx_v_gnline);
+          PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_gnline);
+          __Pyx_INCREF(__pyx_n_s_GN);
+          __Pyx_GIVEREF(__pyx_n_s_GN);
+          PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_n_s_GN);
+          __pyx_t_1 = 0;
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+        /* "alphakit/factor/analysis.pyx":34
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)
+ *             po1 = po.nsmallest(1).index[0]
+ *             if not np.isnan(gnline):             # <<<<<<<<<<<<<<
+ *                 ax4.scatter(po1, gnline, s=150, marker='*', color='green')
+ *                 ax4.text(po1 + 0.2, gnline, 'GN')
+ */
       }
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
       /* "alphakit/factor/analysis.pyx":31
- *         po = abs(gretplt[0] - gnline).reset_index(drop=True)
- *         po1 = po.nsmallest(1).index[0]
- *         if not np.isnan(gnline):             # <<<<<<<<<<<<<<
- *             ax4.scatter(po1, gnline, s=150, marker='*', color='green')
- *             ax4.text(po1 + 0.2, gnline, 'GN')
+ *         gretplt['level'] = 0
+ *         ax4.plot(gretplt, marker='.')
+ *         if gnline is not None:             # <<<<<<<<<<<<<<
+ *             po = abs(gretplt[0] - gnline).reset_index(drop=True)
+ *             po1 = po.nsmallest(1).index[0]
  */
     }
 
-    /* "alphakit/factor/analysis.pyx":34
- *             ax4.scatter(po1, gnline, s=150, marker='*', color='green')
- *             ax4.text(po1 + 0.2, gnline, 'GN')
+    /* "alphakit/factor/analysis.pyx":37
+ *                 ax4.scatter(po1, gnline, s=150, marker='*', color='green')
+ *                 ax4.text(po1 + 0.2, gnline, 'GN')
  *         group = len(gretplt) - 1             # <<<<<<<<<<<<<<
  *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
  *     if outpnl is not None:
  */
-    __pyx_t_9 = PyObject_Length(__pyx_v_gretplt); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v_gretplt); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 37, __pyx_L1_error)
     __pyx_v_group = (__pyx_t_9 - 1);
 
-    /* "alphakit/factor/analysis.pyx":35
- *             ax4.text(po1 + 0.2, gnline, 'GN')
+    /* "alphakit/factor/analysis.pyx":38
+ *                 ax4.text(po1 + 0.2, gnline, 'GN')
  *         group = len(gretplt) - 1
  *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))             # <<<<<<<<<<<<<<
  *     if outpnl is not None:
  *         ax3 = plt.subplot(223)
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_set_xticks); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax4, __pyx_n_s_set_xticks); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_linspace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_linspace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_group); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_group); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_group); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_group); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_2);
     __pyx_t_7 = 0;
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_endpoint, Py_True) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_endpoint, Py_True) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
@@ -2290,312 +2351,312 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_2, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "alphakit/factor/analysis.pyx":16
  *         ax1 = plt.subplot(221)
  *         values = ax1.hist(invar.unstack(), bins=100)
  *     if gret is not None:             # <<<<<<<<<<<<<<
  *         ax2 = plt.subplot(222)
  *         df_factor_plt = gret.cumsum()
  */
   }
 
-  /* "alphakit/factor/analysis.pyx":36
+  /* "alphakit/factor/analysis.pyx":39
  *         group = len(gretplt) - 1
  *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
  *     if outpnl is not None:             # <<<<<<<<<<<<<<
  *         ax3 = plt.subplot(223)
  *         pnlplt = outpnl.cumsum()
  */
   __pyx_t_5 = (__pyx_v_outpnl != Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "alphakit/factor/analysis.pyx":37
+    /* "alphakit/factor/analysis.pyx":40
  *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
  *     if outpnl is not None:
  *         ax3 = plt.subplot(223)             # <<<<<<<<<<<<<<
  *         pnlplt = outpnl.cumsum()
  *         pnlplt.index = pnlplt.index.astype('datetime64[ns]')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_plt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_plt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_subplot); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_subplot); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_int_223) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_int_223);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_ax3 = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "alphakit/factor/analysis.pyx":38
+    /* "alphakit/factor/analysis.pyx":41
  *     if outpnl is not None:
  *         ax3 = plt.subplot(223)
  *         pnlplt = outpnl.cumsum()             # <<<<<<<<<<<<<<
  *         pnlplt.index = pnlplt.index.astype('datetime64[ns]')
  *         ax3.plot(pnlplt)
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_outpnl, __pyx_n_s_cumsum); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_outpnl, __pyx_n_s_cumsum); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_pnlplt = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "alphakit/factor/analysis.pyx":39
+    /* "alphakit/factor/analysis.pyx":42
  *         ax3 = plt.subplot(223)
  *         pnlplt = outpnl.cumsum()
  *         pnlplt.index = pnlplt.index.astype('datetime64[ns]')             # <<<<<<<<<<<<<<
  *         ax3.plot(pnlplt)
  *     if savepath != '':
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pnlplt, __pyx_n_s_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pnlplt, __pyx_n_s_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_kp_s_datetime64_ns) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_s_datetime64_ns);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pnlplt, __pyx_n_s_index, __pyx_t_3) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pnlplt, __pyx_n_s_index, __pyx_t_3) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "alphakit/factor/analysis.pyx":40
+    /* "alphakit/factor/analysis.pyx":43
  *         pnlplt = outpnl.cumsum()
  *         pnlplt.index = pnlplt.index.astype('datetime64[ns]')
  *         ax3.plot(pnlplt)             # <<<<<<<<<<<<<<
  *     if savepath != '':
  *         plt.savefig(savepath)
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax3, __pyx_n_s_plot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax3, __pyx_n_s_plot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_v_pnlplt) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_pnlplt);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "alphakit/factor/analysis.pyx":36
+    /* "alphakit/factor/analysis.pyx":39
  *         group = len(gretplt) - 1
  *         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
  *     if outpnl is not None:             # <<<<<<<<<<<<<<
  *         ax3 = plt.subplot(223)
  *         pnlplt = outpnl.cumsum()
  */
   }
 
-  /* "alphakit/factor/analysis.pyx":41
+  /* "alphakit/factor/analysis.pyx":44
  *         pnlplt.index = pnlplt.index.astype('datetime64[ns]')
  *         ax3.plot(pnlplt)
  *     if savepath != '':             # <<<<<<<<<<<<<<
  *         plt.savefig(savepath)
  *         plt.show(block=False)
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_savepath, __pyx_kp_s_, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_savepath, __pyx_kp_s_, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 44, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "alphakit/factor/analysis.pyx":42
+    /* "alphakit/factor/analysis.pyx":45
  *         ax3.plot(pnlplt)
  *     if savepath != '':
  *         plt.savefig(savepath)             # <<<<<<<<<<<<<<
  *         plt.show(block=False)
  *         plt.pause(3)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_plt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_plt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_savefig); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_savefig); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_v_savepath) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_savepath);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "alphakit/factor/analysis.pyx":43
+    /* "alphakit/factor/analysis.pyx":46
  *     if savepath != '':
  *         plt.savefig(savepath)
  *         plt.show(block=False)             # <<<<<<<<<<<<<<
  *         plt.pause(3)
  *         plt.close('all')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_plt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_plt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_show); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_show); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_block, Py_False) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 43, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_block, Py_False) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "alphakit/factor/analysis.pyx":44
+    /* "alphakit/factor/analysis.pyx":47
  *         plt.savefig(savepath)
  *         plt.show(block=False)
  *         plt.pause(3)             # <<<<<<<<<<<<<<
  *         plt.close('all')
  *     else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_plt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_plt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_pause); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_pause); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_6 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_int_3) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_int_3);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "alphakit/factor/analysis.pyx":45
+    /* "alphakit/factor/analysis.pyx":48
  *         plt.show(block=False)
  *         plt.pause(3)
  *         plt.close('all')             # <<<<<<<<<<<<<<
  *     else:
  *         plt.show(block=True)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_plt); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_plt); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_n_s_all) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_all);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "alphakit/factor/analysis.pyx":41
+    /* "alphakit/factor/analysis.pyx":44
  *         pnlplt.index = pnlplt.index.astype('datetime64[ns]')
  *         ax3.plot(pnlplt)
  *     if savepath != '':             # <<<<<<<<<<<<<<
  *         plt.savefig(savepath)
  *         plt.show(block=False)
  */
-    goto __pyx_L7;
+    goto __pyx_L9;
   }
 
-  /* "alphakit/factor/analysis.pyx":47
+  /* "alphakit/factor/analysis.pyx":50
  *         plt.close('all')
  *     else:
  *         plt.show(block=True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_plt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_plt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_show); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_show); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_block, Py_True) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 47, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_block, Py_True) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
-  __pyx_L7:;
+  __pyx_L9:;
 
   /* "alphakit/factor/analysis.pyx":10
  * 
  * 
  * def factor_plot(dummy, invar=None, gret=None, outpnl=None, savepath=''):             # <<<<<<<<<<<<<<
  *     plt.figure(figsize=(16, 9))
  *     if invar is not None:
@@ -2627,53 +2688,65 @@
   __Pyx_XDECREF(__pyx_v_pnlplt);
   __Pyx_XDECREF(__pyx_v_invar);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "alphakit/factor/analysis.pyx":50
+/* "alphakit/factor/analysis.pyx":53
  * 
  * 
- * def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):             # <<<<<<<<<<<<<<
- *     invar = dummy * invar
- *     disp = factor_stat(dummy, invar)
+ * def factor_one(dummy,             # <<<<<<<<<<<<<<
+ *                invar,
+ *                ret_f1d,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8alphakit_6factor_8analysis_3factor_one(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8alphakit_6factor_8analysis_2factor_one[] = "factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath='')";
+static char __pyx_doc_8alphakit_6factor_8analysis_2factor_one[] = "factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, checkna=True, savepath='')";
 static PyMethodDef __pyx_mdef_8alphakit_6factor_8analysis_3factor_one = {"factor_one", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8alphakit_6factor_8analysis_3factor_one, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8alphakit_6factor_8analysis_2factor_one};
 static PyObject *__pyx_pw_8alphakit_6factor_8analysis_3factor_one(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_dummy = 0;
   PyObject *__pyx_v_invar = 0;
   PyObject *__pyx_v_ret_f1d = 0;
   PyObject *__pyx_v_freq = 0;
   PyObject *__pyx_v_hold = 0;
   PyObject *__pyx_v_group = 0;
   PyObject *__pyx_v_skip = 0;
+  PyObject *__pyx_v_checkna = 0;
   PyObject *__pyx_v_savepath = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("factor_one (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dummy,&__pyx_n_s_invar,&__pyx_n_s_ret_f1d,&__pyx_n_s_freq,&__pyx_n_s_hold,&__pyx_n_s_group,&__pyx_n_s_skip,&__pyx_n_s_savepath,0};
-    PyObject* values[8] = {0,0,0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dummy,&__pyx_n_s_invar,&__pyx_n_s_ret_f1d,&__pyx_n_s_freq,&__pyx_n_s_hold,&__pyx_n_s_group,&__pyx_n_s_skip,&__pyx_n_s_checkna,&__pyx_n_s_savepath,0};
+    PyObject* values[9] = {0,0,0,0,0,0,0,0,0};
     values[3] = ((PyObject *)__pyx_int_252);
     values[4] = ((PyObject *)__pyx_int_1);
     values[5] = ((PyObject *)__pyx_int_10);
     values[6] = ((PyObject *)__pyx_int_0);
-    values[7] = ((PyObject *)__pyx_kp_s_);
+
+    /* "alphakit/factor/analysis.pyx":60
+ *                group=10,
+ *                skip=0,
+ *                checkna=True,             # <<<<<<<<<<<<<<
+ *                savepath=''):
+ *     invar = dummy * invar
+ */
+    values[7] = ((PyObject *)Py_True);
+    values[8] = ((PyObject *)__pyx_kp_s_);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
@@ -2694,21 +2767,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dummy)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_invar)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("factor_one", 0, 3, 8, 1); __PYX_ERR(0, 50, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("factor_one", 0, 3, 9, 1); __PYX_ERR(0, 53, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ret_f1d)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("factor_one", 0, 3, 8, 2); __PYX_ERR(0, 50, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("factor_one", 0, 3, 9, 2); __PYX_ERR(0, 53, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_freq);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -2729,23 +2802,31 @@
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_skip);
           if (value) { values[6] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_savepath);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_checkna);
           if (value) { values[7] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_savepath);
+          if (value) { values[8] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "factor_one") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "factor_one") < 0)) __PYX_ERR(0, 53, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
@@ -2762,32 +2843,41 @@
     __pyx_v_dummy = values[0];
     __pyx_v_invar = values[1];
     __pyx_v_ret_f1d = values[2];
     __pyx_v_freq = values[3];
     __pyx_v_hold = values[4];
     __pyx_v_group = values[5];
     __pyx_v_skip = values[6];
-    __pyx_v_savepath = values[7];
+    __pyx_v_checkna = values[7];
+    __pyx_v_savepath = values[8];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("factor_one", 0, 3, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("factor_one", 0, 3, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 53, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("alphakit.factor.analysis.factor_one", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8alphakit_6factor_8analysis_2factor_one(__pyx_self, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_freq, __pyx_v_hold, __pyx_v_group, __pyx_v_skip, __pyx_v_savepath);
+  __pyx_r = __pyx_pf_8alphakit_6factor_8analysis_2factor_one(__pyx_self, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_freq, __pyx_v_hold, __pyx_v_group, __pyx_v_skip, __pyx_v_checkna, __pyx_v_savepath);
+
+  /* "alphakit/factor/analysis.pyx":53
+ * 
+ * 
+ * def factor_one(dummy,             # <<<<<<<<<<<<<<
+ *                invar,
+ *                ret_f1d,
+ */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8alphakit_6factor_8analysis_2factor_one(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_freq, PyObject *__pyx_v_hold, PyObject *__pyx_v_group, PyObject *__pyx_v_skip, PyObject *__pyx_v_savepath) {
+static PyObject *__pyx_pf_8alphakit_6factor_8analysis_2factor_one(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_freq, PyObject *__pyx_v_hold, PyObject *__pyx_v_group, PyObject *__pyx_v_skip, PyObject *__pyx_v_checkna, PyObject *__pyx_v_savepath) {
   PyObject *__pyx_v_disp = NULL;
   PyObject *__pyx_v_invar_score = NULL;
   PyObject *__pyx_v_weighT = NULL;
   PyObject *__pyx_v_weightB = NULL;
   PyObject *__pyx_v_weight = NULL;
   PyObject *__pyx_v_stockNum = NULL;
   PyObject *__pyx_v_outpnl1 = NULL;
@@ -2817,34 +2907,34 @@
   PyObject *(*__pyx_t_8)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factor_one", 0);
   __Pyx_INCREF(__pyx_v_invar);
 
-  /* "alphakit/factor/analysis.pyx":51
- * 
- * def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):
+  /* "alphakit/factor/analysis.pyx":62
+ *                checkna=True,
+ *                savepath=''):
  *     invar = dummy * invar             # <<<<<<<<<<<<<<
  *     disp = factor_stat(dummy, invar)
  *     invar_score = factor_score_sig(invar)
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_v_dummy, __pyx_v_invar); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_v_dummy, __pyx_v_invar); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_invar, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":52
- * def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):
+  /* "alphakit/factor/analysis.pyx":63
+ *                savepath=''):
  *     invar = dummy * invar
  *     disp = factor_stat(dummy, invar)             # <<<<<<<<<<<<<<
  *     invar_score = factor_score_sig(invar)
  *     weighT, weightB, weight, stockNum = factorToWeight(invar_score, hold)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_factor_stat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_factor_stat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -2853,82 +2943,82 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_dummy, __pyx_v_invar};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_dummy, __pyx_v_invar};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dummy);
     __Pyx_GIVEREF(__pyx_v_dummy);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_dummy);
     __Pyx_INCREF(__pyx_v_invar);
     __Pyx_GIVEREF(__pyx_v_invar);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_invar);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_disp = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":53
+  /* "alphakit/factor/analysis.pyx":64
  *     invar = dummy * invar
  *     disp = factor_stat(dummy, invar)
  *     invar_score = factor_score_sig(invar)             # <<<<<<<<<<<<<<
  *     weighT, weightB, weight, stockNum = factorToWeight(invar_score, hold)
  *     disp['TopNum'] = stockNum['TOP'].mean()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_factor_score_sig); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_factor_score_sig); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_invar) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_invar);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_invar_score = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":54
+  /* "alphakit/factor/analysis.pyx":65
  *     disp = factor_stat(dummy, invar)
  *     invar_score = factor_score_sig(invar)
  *     weighT, weightB, weight, stockNum = factorToWeight(invar_score, hold)             # <<<<<<<<<<<<<<
  *     disp['TopNum'] = stockNum['TOP'].mean()
  *     disp['BotNum'] = stockNum['BOT'].mean()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_factorToWeight); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_factorToWeight); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -2937,51 +3027,51 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_invar_score, __pyx_v_hold};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_invar_score, __pyx_v_hold};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_3 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_invar_score);
     __Pyx_GIVEREF(__pyx_v_invar_score);
     PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_4, __pyx_v_invar_score);
     __Pyx_INCREF(__pyx_v_hold);
     __Pyx_GIVEREF(__pyx_v_hold);
     PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_4, __pyx_v_hold);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 4)) {
       if (size > 4) __Pyx_RaiseTooManyValuesError(4);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 54, __pyx_L1_error)
+      __PYX_ERR(0, 65, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 2); 
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 3); 
@@ -2996,151 +3086,175 @@
     __Pyx_INCREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_t_6);
     #else
     {
       Py_ssize_t i;
       PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_3,&__pyx_t_5,&__pyx_t_6};
       for (i=0; i < 4; i++) {
-        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 54, __pyx_L1_error)
+        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 65, __pyx_L1_error)
         __Pyx_GOTREF(item);
         *(temps[i]) = item;
       }
     }
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
     PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_3,&__pyx_t_5,&__pyx_t_6};
-    __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
     for (index=0; index < 4; index++) {
       PyObject* item = __pyx_t_8(__pyx_t_7); if (unlikely(!item)) goto __pyx_L3_unpacking_failed;
       __Pyx_GOTREF(item);
       *(temps[index]) = item;
     }
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 4) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 4) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 54, __pyx_L1_error)
+    __PYX_ERR(0, 65, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_weighT = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_weightB = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_weight = __pyx_t_5;
   __pyx_t_5 = 0;
   __pyx_v_stockNum = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "alphakit/factor/analysis.pyx":55
+  /* "alphakit/factor/analysis.pyx":66
  *     invar_score = factor_score_sig(invar)
  *     weighT, weightB, weight, stockNum = factorToWeight(invar_score, hold)
  *     disp['TopNum'] = stockNum['TOP'].mean()             # <<<<<<<<<<<<<<
  *     disp['BotNum'] = stockNum['BOT'].mean()
- *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy, weighT, ret_f1d, skip, type='all')
+ *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy,
  */
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_stockNum, __pyx_n_s_TOP); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_stockNum, __pyx_n_s_TOP); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_disp, __pyx_n_s_TopNum, __pyx_t_1) < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_disp, __pyx_n_s_TopNum, __pyx_t_1) < 0)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":56
+  /* "alphakit/factor/analysis.pyx":67
  *     weighT, weightB, weight, stockNum = factorToWeight(invar_score, hold)
  *     disp['TopNum'] = stockNum['TOP'].mean()
  *     disp['BotNum'] = stockNum['BOT'].mean()             # <<<<<<<<<<<<<<
- *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy, weighT, ret_f1d, skip, type='all')
- *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy, weightB, ret_f1d, skip, type='all')
+ *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy,
+ *                                                 weighT,
  */
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_stockNum, __pyx_n_s_BOT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_stockNum, __pyx_n_s_BOT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_mean); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_mean); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_disp, __pyx_n_s_BotNum, __pyx_t_1) < 0)) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_disp, __pyx_n_s_BotNum, __pyx_t_1) < 0)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":57
+  /* "alphakit/factor/analysis.pyx":68
  *     disp['TopNum'] = stockNum['TOP'].mean()
  *     disp['BotNum'] = stockNum['BOT'].mean()
- *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy, weighT, ret_f1d, skip, type='all')             # <<<<<<<<<<<<<<
- *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy, weightB, ret_f1d, skip, type='all')
- *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy, weight, ret_f1d, skip, type='all')
+ *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy,             # <<<<<<<<<<<<<<
+ *                                                 weighT,
+ *                                                 ret_f1d,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_factor_pnl); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_factor_pnl); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":71
+ *                                                 weighT,
+ *                                                 ret_f1d,
+ *                                                 skip,             # <<<<<<<<<<<<<<
+ *                                                 type='all')
+ *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy,
+ */
+  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_dummy);
   __Pyx_GIVEREF(__pyx_v_dummy);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_dummy);
   __Pyx_INCREF(__pyx_v_weighT);
   __Pyx_GIVEREF(__pyx_v_weighT);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_weighT);
   __Pyx_INCREF(__pyx_v_ret_f1d);
   __Pyx_GIVEREF(__pyx_v_ret_f1d);
   PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_v_ret_f1d);
   __Pyx_INCREF(__pyx_v_skip);
   __Pyx_GIVEREF(__pyx_v_skip);
   PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_v_skip);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":72
+ *                                                 ret_f1d,
+ *                                                 skip,
+ *                                                 type='all')             # <<<<<<<<<<<<<<
+ *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy,
+ *                                                 weightB,
+ */
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_type, __pyx_n_s_all) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_type, __pyx_n_s_all) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":68
+ *     disp['TopNum'] = stockNum['TOP'].mean()
+ *     disp['BotNum'] = stockNum['BOT'].mean()
+ *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy,             # <<<<<<<<<<<<<<
+ *                                                 weighT,
+ *                                                 ret_f1d,
+ */
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 57, __pyx_L1_error)
+      __PYX_ERR(0, 68, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -3148,90 +3262,114 @@
       __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_1 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_t_1);
     #else
-    __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext;
     index = 0; __pyx_t_5 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_5)) goto __pyx_L5_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_5);
     index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_6);
     index = 2; __pyx_t_1 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_1)) goto __pyx_L5_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_1);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 3) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 3) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L6_unpacking_done;
     __pyx_L5_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 57, __pyx_L1_error)
+    __PYX_ERR(0, 68, __pyx_L1_error)
     __pyx_L6_unpacking_done:;
   }
   __pyx_v_outpnl1 = __pyx_t_5;
   __pyx_t_5 = 0;
   __pyx_v_turnover1 = __pyx_t_6;
   __pyx_t_6 = 0;
   __pyx_v_ic_series1 = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":58
- *     disp['BotNum'] = stockNum['BOT'].mean()
- *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy, weighT, ret_f1d, skip, type='all')
- *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy, weightB, ret_f1d, skip, type='all')             # <<<<<<<<<<<<<<
- *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy, weight, ret_f1d, skip, type='all')
- *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
+  /* "alphakit/factor/analysis.pyx":73
+ *                                                 skip,
+ *                                                 type='all')
+ *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy,             # <<<<<<<<<<<<<<
+ *                                                 weightB,
+ *                                                 ret_f1d,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_factor_pnl); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_factor_pnl); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":76
+ *                                                 weightB,
+ *                                                 ret_f1d,
+ *                                                 skip,             # <<<<<<<<<<<<<<
+ *                                                 type='all')
+ *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy,
+ */
+  __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_dummy);
   __Pyx_GIVEREF(__pyx_v_dummy);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dummy);
   __Pyx_INCREF(__pyx_v_weightB);
   __Pyx_GIVEREF(__pyx_v_weightB);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_weightB);
   __Pyx_INCREF(__pyx_v_ret_f1d);
   __Pyx_GIVEREF(__pyx_v_ret_f1d);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_ret_f1d);
   __Pyx_INCREF(__pyx_v_skip);
   __Pyx_GIVEREF(__pyx_v_skip);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_v_skip);
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":77
+ *                                                 ret_f1d,
+ *                                                 skip,
+ *                                                 type='all')             # <<<<<<<<<<<<<<
+ *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy,
+ *                                                 weight,
+ */
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_type, __pyx_n_s_all) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_type, __pyx_n_s_all) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":73
+ *                                                 skip,
+ *                                                 type='all')
+ *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy,             # <<<<<<<<<<<<<<
+ *                                                 weightB,
+ *                                                 ret_f1d,
+ */
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
     PyObject* sequence = __pyx_t_5;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 58, __pyx_L1_error)
+      __PYX_ERR(0, 73, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -3239,90 +3377,114 @@
       __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext;
     index = 0; __pyx_t_6 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_6)) goto __pyx_L7_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_6);
     index = 1; __pyx_t_1 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_1)) goto __pyx_L7_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_1);
     index = 2; __pyx_t_3 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L7_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 3) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 3) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L8_unpacking_done;
     __pyx_L7_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 58, __pyx_L1_error)
+    __PYX_ERR(0, 73, __pyx_L1_error)
     __pyx_L8_unpacking_done:;
   }
   __pyx_v_outpnl2 = __pyx_t_6;
   __pyx_t_6 = 0;
   __pyx_v_turnover2 = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_ic_series2 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "alphakit/factor/analysis.pyx":59
- *     outpnl1, turnover1, ic_series1 = factor_pnl(dummy, weighT, ret_f1d, skip, type='all')
- *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy, weightB, ret_f1d, skip, type='all')
- *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy, weight, ret_f1d, skip, type='all')             # <<<<<<<<<<<<<<
- *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
- *     outpnl.columns = ['TOP', 'BOT', 'TMB']
+  /* "alphakit/factor/analysis.pyx":78
+ *                                                 skip,
+ *                                                 type='all')
+ *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy,             # <<<<<<<<<<<<<<
+ *                                                 weight,
+ *                                                 ret_f1d,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_factor_pnl); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_factor_pnl); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":81
+ *                                                 weight,
+ *                                                 ret_f1d,
+ *                                                 skip,             # <<<<<<<<<<<<<<
+ *                                                 type='all')
+ *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
+ */
+  __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_dummy);
   __Pyx_GIVEREF(__pyx_v_dummy);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_dummy);
   __Pyx_INCREF(__pyx_v_weight);
   __Pyx_GIVEREF(__pyx_v_weight);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_weight);
   __Pyx_INCREF(__pyx_v_ret_f1d);
   __Pyx_GIVEREF(__pyx_v_ret_f1d);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_ret_f1d);
   __Pyx_INCREF(__pyx_v_skip);
   __Pyx_GIVEREF(__pyx_v_skip);
   PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_v_skip);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":82
+ *                                                 ret_f1d,
+ *                                                 skip,
+ *                                                 type='all')             # <<<<<<<<<<<<<<
+ *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
+ *     outpnl.columns = ['TOP', 'BOT', 'TMB']
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_type, __pyx_n_s_all) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_type, __pyx_n_s_all) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":78
+ *                                                 skip,
+ *                                                 type='all')
+ *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy,             # <<<<<<<<<<<<<<
+ *                                                 weight,
+ *                                                 ret_f1d,
+ */
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_6))) || (PyList_CheckExact(__pyx_t_6))) {
     PyObject* sequence = __pyx_t_6;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 59, __pyx_L1_error)
+      __PYX_ERR(0, 78, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -3330,317 +3492,349 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_5 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_2 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_2 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext;
     index = 0; __pyx_t_1 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_1)) goto __pyx_L9_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_1);
     index = 1; __pyx_t_3 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L9_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_5 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_5)) goto __pyx_L9_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_5);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 3) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 3) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L10_unpacking_done;
     __pyx_L9_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 59, __pyx_L1_error)
+    __PYX_ERR(0, 78, __pyx_L1_error)
     __pyx_L10_unpacking_done:;
   }
   __pyx_v_outpnl3 = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_turnover3 = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_ic_series3 = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "alphakit/factor/analysis.pyx":60
- *     outpnl2, turnover2, ic_series2 = factor_pnl(dummy, weightB, ret_f1d, skip, type='all')
- *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy, weight, ret_f1d, skip, type='all')
+  /* "alphakit/factor/analysis.pyx":83
+ *                                                 skip,
+ *                                                 type='all')
  *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)             # <<<<<<<<<<<<<<
  *     outpnl.columns = ['TOP', 'BOT', 'TMB']
  *     turnover = pd.concat([turnover1, turnover2, turnover3], axis=1)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_concat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_concat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyList_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_outpnl1);
   __Pyx_GIVEREF(__pyx_v_outpnl1);
   PyList_SET_ITEM(__pyx_t_6, 0, __pyx_v_outpnl1);
   __Pyx_INCREF(__pyx_v_outpnl2);
   __Pyx_GIVEREF(__pyx_v_outpnl2);
   PyList_SET_ITEM(__pyx_t_6, 1, __pyx_v_outpnl2);
   __Pyx_INCREF(__pyx_v_outpnl3);
   __Pyx_GIVEREF(__pyx_v_outpnl3);
   PyList_SET_ITEM(__pyx_t_6, 2, __pyx_v_outpnl3);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_outpnl = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":61
- *     outpnl3, turnover3, ic_series3 = factor_pnl(dummy, weight, ret_f1d, skip, type='all')
+  /* "alphakit/factor/analysis.pyx":84
+ *                                                 type='all')
  *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
  *     outpnl.columns = ['TOP', 'BOT', 'TMB']             # <<<<<<<<<<<<<<
  *     turnover = pd.concat([turnover1, turnover2, turnover3], axis=1)
  *     turnover.columns = ['TOP', 'BOT', 'TMB']
  */
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_TOP);
   __Pyx_GIVEREF(__pyx_n_s_TOP);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_TOP);
   __Pyx_INCREF(__pyx_n_s_BOT);
   __Pyx_GIVEREF(__pyx_n_s_BOT);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_BOT);
   __Pyx_INCREF(__pyx_n_s_TMB);
   __Pyx_GIVEREF(__pyx_n_s_TMB);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_TMB);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_outpnl, __pyx_n_s_columns, __pyx_t_1) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_outpnl, __pyx_n_s_columns, __pyx_t_1) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":62
+  /* "alphakit/factor/analysis.pyx":85
  *     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
  *     outpnl.columns = ['TOP', 'BOT', 'TMB']
  *     turnover = pd.concat([turnover1, turnover2, turnover3], axis=1)             # <<<<<<<<<<<<<<
  *     turnover.columns = ['TOP', 'BOT', 'TMB']
  *     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_concat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_concat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_turnover1);
   __Pyx_GIVEREF(__pyx_v_turnover1);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_turnover1);
   __Pyx_INCREF(__pyx_v_turnover2);
   __Pyx_GIVEREF(__pyx_v_turnover2);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_turnover2);
   __Pyx_INCREF(__pyx_v_turnover3);
   __Pyx_GIVEREF(__pyx_v_turnover3);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_v_turnover3);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_turnover = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "alphakit/factor/analysis.pyx":63
+  /* "alphakit/factor/analysis.pyx":86
  *     outpnl.columns = ['TOP', 'BOT', 'TMB']
  *     turnover = pd.concat([turnover1, turnover2, turnover3], axis=1)
  *     turnover.columns = ['TOP', 'BOT', 'TMB']             # <<<<<<<<<<<<<<
  *     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)
  *     ic_series.columns = ['TOP', 'BOT', 'TMB']
  */
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_TOP);
   __Pyx_GIVEREF(__pyx_n_s_TOP);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_TOP);
   __Pyx_INCREF(__pyx_n_s_BOT);
   __Pyx_GIVEREF(__pyx_n_s_BOT);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_BOT);
   __Pyx_INCREF(__pyx_n_s_TMB);
   __Pyx_GIVEREF(__pyx_n_s_TMB);
   PyList_SET_ITEM(__pyx_t_5, 2, __pyx_n_s_TMB);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_turnover, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_turnover, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "alphakit/factor/analysis.pyx":64
+  /* "alphakit/factor/analysis.pyx":87
  *     turnover = pd.concat([turnover1, turnover2, turnover3], axis=1)
  *     turnover.columns = ['TOP', 'BOT', 'TMB']
  *     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)             # <<<<<<<<<<<<<<
  *     ic_series.columns = ['TOP', 'BOT', 'TMB']
- *     pnlstat = pnl_metrics(freq, outpnl, turnover, ic_series, usecol=['TOP', 'BOT', 'TMB'])
+ *     pnlstat = pnl_metrics(freq,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_concat); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_concat); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_ic_series1);
   __Pyx_GIVEREF(__pyx_v_ic_series1);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_v_ic_series1);
   __Pyx_INCREF(__pyx_v_ic_series2);
   __Pyx_GIVEREF(__pyx_v_ic_series2);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_v_ic_series2);
   __Pyx_INCREF(__pyx_v_ic_series3);
   __Pyx_GIVEREF(__pyx_v_ic_series3);
   PyList_SET_ITEM(__pyx_t_5, 2, __pyx_v_ic_series3);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_ic_series = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "alphakit/factor/analysis.pyx":65
+  /* "alphakit/factor/analysis.pyx":88
  *     turnover.columns = ['TOP', 'BOT', 'TMB']
  *     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)
  *     ic_series.columns = ['TOP', 'BOT', 'TMB']             # <<<<<<<<<<<<<<
- *     pnlstat = pnl_metrics(freq, outpnl, turnover, ic_series, usecol=['TOP', 'BOT', 'TMB'])
- *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip)
+ *     pnlstat = pnl_metrics(freq,
+ *                           outpnl,
  */
-  __pyx_t_6 = PyList_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_n_s_TOP);
   __Pyx_GIVEREF(__pyx_n_s_TOP);
   PyList_SET_ITEM(__pyx_t_6, 0, __pyx_n_s_TOP);
   __Pyx_INCREF(__pyx_n_s_BOT);
   __Pyx_GIVEREF(__pyx_n_s_BOT);
   PyList_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_BOT);
   __Pyx_INCREF(__pyx_n_s_TMB);
   __Pyx_GIVEREF(__pyx_n_s_TMB);
   PyList_SET_ITEM(__pyx_t_6, 2, __pyx_n_s_TMB);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_ic_series, __pyx_n_s_columns, __pyx_t_6) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_ic_series, __pyx_n_s_columns, __pyx_t_6) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "alphakit/factor/analysis.pyx":66
+  /* "alphakit/factor/analysis.pyx":89
  *     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)
  *     ic_series.columns = ['TOP', 'BOT', 'TMB']
- *     pnlstat = pnl_metrics(freq, outpnl, turnover, ic_series, usecol=['TOP', 'BOT', 'TMB'])             # <<<<<<<<<<<<<<
- *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip)
- *     factor_plot(dummy, invar, gret, outpnl, savepath)
+ *     pnlstat = pnl_metrics(freq,             # <<<<<<<<<<<<<<
+ *                           outpnl,
+ *                           turnover,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pnl_metrics); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pnl_metrics); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":92
+ *                           outpnl,
+ *                           turnover,
+ *                           ic_series,             # <<<<<<<<<<<<<<
+ *                           usecol=['TOP', 'BOT', 'TMB'])
+ *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,
+ */
+  __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_freq);
   __Pyx_GIVEREF(__pyx_v_freq);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_freq);
   __Pyx_INCREF(__pyx_v_outpnl);
   __Pyx_GIVEREF(__pyx_v_outpnl);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_outpnl);
   __Pyx_INCREF(__pyx_v_turnover);
   __Pyx_GIVEREF(__pyx_v_turnover);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_turnover);
   __Pyx_INCREF(__pyx_v_ic_series);
   __Pyx_GIVEREF(__pyx_v_ic_series);
   PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_v_ic_series);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":93
+ *                           turnover,
+ *                           ic_series,
+ *                           usecol=['TOP', 'BOT', 'TMB'])             # <<<<<<<<<<<<<<
+ *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,
+ *                                    checkna)
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_TOP);
   __Pyx_GIVEREF(__pyx_n_s_TOP);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_TOP);
   __Pyx_INCREF(__pyx_n_s_BOT);
   __Pyx_GIVEREF(__pyx_n_s_BOT);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_BOT);
   __Pyx_INCREF(__pyx_n_s_TMB);
   __Pyx_GIVEREF(__pyx_n_s_TMB);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_TMB);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_usecol, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_usecol, __pyx_t_1) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+
+  /* "alphakit/factor/analysis.pyx":89
+ *     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)
+ *     ic_series.columns = ['TOP', 'BOT', 'TMB']
+ *     pnlstat = pnl_metrics(freq,             # <<<<<<<<<<<<<<
+ *                           outpnl,
+ *                           turnover,
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_pnlstat = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":67
- *     ic_series.columns = ['TOP', 'BOT', 'TMB']
- *     pnlstat = pnl_metrics(freq, outpnl, turnover, ic_series, usecol=['TOP', 'BOT', 'TMB'])
- *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip)             # <<<<<<<<<<<<<<
+  /* "alphakit/factor/analysis.pyx":94
+ *                           ic_series,
+ *                           usecol=['TOP', 'BOT', 'TMB'])
+ *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,             # <<<<<<<<<<<<<<
+ *                                    checkna)
  *     factor_plot(dummy, invar, gret, outpnl, savepath)
- *     return disp, outpnl, pnlstat, gret_stat
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_factor_group); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_factor_group); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+
+  /* "alphakit/factor/analysis.pyx":95
+ *                           usecol=['TOP', 'BOT', 'TMB'])
+ *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,
+ *                                    checkna)             # <<<<<<<<<<<<<<
+ *     factor_plot(dummy, invar, gret, outpnl, savepath)
+ *     return disp, outpnl, pnlstat, gret_stat
+ */
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[7] = {__pyx_t_5, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 6+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+    PyObject *__pyx_temp[8] = {__pyx_t_5, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip, __pyx_v_checkna};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 7+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[7] = {__pyx_t_5, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 6+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+    PyObject *__pyx_temp[8] = {__pyx_t_5, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip, __pyx_v_checkna};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 7+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(6+__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(7+__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dummy);
     __Pyx_GIVEREF(__pyx_v_dummy);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_4, __pyx_v_dummy);
@@ -3655,77 +3849,88 @@
     PyTuple_SET_ITEM(__pyx_t_6, 3+__pyx_t_4, __pyx_v_group);
     __Pyx_INCREF(__pyx_v_hold);
     __Pyx_GIVEREF(__pyx_v_hold);
     PyTuple_SET_ITEM(__pyx_t_6, 4+__pyx_t_4, __pyx_v_hold);
     __Pyx_INCREF(__pyx_v_skip);
     __Pyx_GIVEREF(__pyx_v_skip);
     PyTuple_SET_ITEM(__pyx_t_6, 5+__pyx_t_4, __pyx_v_skip);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __Pyx_INCREF(__pyx_v_checkna);
+    __Pyx_GIVEREF(__pyx_v_checkna);
+    PyTuple_SET_ITEM(__pyx_t_6, 6+__pyx_t_4, __pyx_v_checkna);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 67, __pyx_L1_error)
+      __PYX_ERR(0, 94, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_6);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext;
     index = 0; __pyx_t_3 = __pyx_t_8(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L11_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_5); if (unlikely(!__pyx_t_6)) goto __pyx_L11_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_6);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_5), 2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_5), 2) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L12_unpacking_done;
     __pyx_L11_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 67, __pyx_L1_error)
+    __PYX_ERR(0, 94, __pyx_L1_error)
     __pyx_L12_unpacking_done:;
   }
+
+  /* "alphakit/factor/analysis.pyx":94
+ *                           ic_series,
+ *                           usecol=['TOP', 'BOT', 'TMB'])
+ *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,             # <<<<<<<<<<<<<<
+ *                                    checkna)
+ *     factor_plot(dummy, invar, gret, outpnl, savepath)
+ */
   __pyx_v_gret = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_gret_stat = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "alphakit/factor/analysis.pyx":68
- *     pnlstat = pnl_metrics(freq, outpnl, turnover, ic_series, usecol=['TOP', 'BOT', 'TMB'])
- *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip)
+  /* "alphakit/factor/analysis.pyx":96
+ *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,
+ *                                    checkna)
  *     factor_plot(dummy, invar, gret, outpnl, savepath)             # <<<<<<<<<<<<<<
  *     return disp, outpnl, pnlstat, gret_stat
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_factor_plot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_factor_plot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -3734,29 +3939,29 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[6] = {__pyx_t_3, __pyx_v_dummy, __pyx_v_invar, __pyx_v_gret, __pyx_v_outpnl, __pyx_v_savepath};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_4, 5+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_4, 5+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[6] = {__pyx_t_3, __pyx_v_dummy, __pyx_v_invar, __pyx_v_gret, __pyx_v_outpnl, __pyx_v_savepath};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_4, 5+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_4, 5+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(5+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(5+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dummy);
     __Pyx_GIVEREF(__pyx_v_dummy);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_dummy);
@@ -3768,28 +3973,28 @@
     PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_gret);
     __Pyx_INCREF(__pyx_v_outpnl);
     __Pyx_GIVEREF(__pyx_v_outpnl);
     PyTuple_SET_ITEM(__pyx_t_5, 3+__pyx_t_4, __pyx_v_outpnl);
     __Pyx_INCREF(__pyx_v_savepath);
     __Pyx_GIVEREF(__pyx_v_savepath);
     PyTuple_SET_ITEM(__pyx_t_5, 4+__pyx_t_4, __pyx_v_savepath);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "alphakit/factor/analysis.pyx":69
- *     gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip)
+  /* "alphakit/factor/analysis.pyx":97
+ *                                    checkna)
  *     factor_plot(dummy, invar, gret, outpnl, savepath)
  *     return disp, outpnl, pnlstat, gret_stat             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_disp);
   __Pyx_GIVEREF(__pyx_v_disp);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_disp);
   __Pyx_INCREF(__pyx_v_outpnl);
   __Pyx_GIVEREF(__pyx_v_outpnl);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_outpnl);
@@ -3799,20 +4004,20 @@
   __Pyx_INCREF(__pyx_v_gret_stat);
   __Pyx_GIVEREF(__pyx_v_gret_stat);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_v_gret_stat);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "alphakit/factor/analysis.pyx":50
+  /* "alphakit/factor/analysis.pyx":53
  * 
  * 
- * def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):             # <<<<<<<<<<<<<<
- *     invar = dummy * invar
- *     disp = factor_stat(dummy, invar)
+ * def factor_one(dummy,             # <<<<<<<<<<<<<<
+ *                invar,
+ *                ret_f1d,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -4048,14 +4253,15 @@
   {&__pyx_n_s_ax1, __pyx_k_ax1, sizeof(__pyx_k_ax1), 0, 0, 1, 1},
   {&__pyx_n_s_ax2, __pyx_k_ax2, sizeof(__pyx_k_ax2), 0, 0, 1, 1},
   {&__pyx_n_s_ax3, __pyx_k_ax3, sizeof(__pyx_k_ax3), 0, 0, 1, 1},
   {&__pyx_n_s_ax4, __pyx_k_ax4, sizeof(__pyx_k_ax4), 0, 0, 1, 1},
   {&__pyx_n_s_axis, __pyx_k_axis, sizeof(__pyx_k_axis), 0, 0, 1, 1},
   {&__pyx_n_s_bins, __pyx_k_bins, sizeof(__pyx_k_bins), 0, 0, 1, 1},
   {&__pyx_n_s_block, __pyx_k_block, sizeof(__pyx_k_block), 0, 0, 1, 1},
+  {&__pyx_n_s_checkna, __pyx_k_checkna, sizeof(__pyx_k_checkna), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_color, __pyx_k_color, sizeof(__pyx_k_color), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_concat, __pyx_k_concat, sizeof(__pyx_k_concat), 0, 0, 1, 1},
   {&__pyx_n_s_cumsum, __pyx_k_cumsum, sizeof(__pyx_k_cumsum), 0, 0, 1, 1},
   {&__pyx_kp_s_datetime64_ns, __pyx_k_datetime64_ns, sizeof(__pyx_k_datetime64_ns), 0, 0, 1, 0},
@@ -4161,22 +4367,22 @@
  *     if invar is not None:
  *         invar = invar * dummy
  */
   __pyx_tuple__2 = PyTuple_Pack(2, __pyx_int_16, __pyx_int_9); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "alphakit/factor/analysis.pyx":25
- *         ax4 = plt.subplot(224)
- *         gnline = gret['GN'].mean()
- *         gret.drop('GN', axis=1, inplace=True)             # <<<<<<<<<<<<<<
+  /* "alphakit/factor/analysis.pyx":27
+ *         if 'GN' in gret.columns:
+ *             gnline = gret['GN'].mean()
+ *             gret.drop('GN', axis=1, inplace=True)             # <<<<<<<<<<<<<<
  *         gretplt = pd.DataFrame(gret.mean())
  *         gretplt['level'] = 0
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_GN); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_GN); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "alphakit/factor/analysis.pyx":10
  * 
  * 
  * def factor_plot(dummy, invar=None, gret=None, outpnl=None, savepath=''):             # <<<<<<<<<<<<<<
@@ -4184,25 +4390,25 @@
  *     if invar is not None:
  */
   __pyx_tuple__6 = PyTuple_Pack(17, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_gret, __pyx_n_s_outpnl, __pyx_n_s_savepath, __pyx_n_s_ax1, __pyx_n_s_values, __pyx_n_s_ax2, __pyx_n_s_df_factor_plt, __pyx_n_s_ax4, __pyx_n_s_gnline, __pyx_n_s_gretplt, __pyx_n_s_po, __pyx_n_s_po1, __pyx_n_s_group, __pyx_n_s_ax3, __pyx_n_s_pnlplt); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
   __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(5, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_analysis_pyx, __pyx_n_s_factor_plot, 10, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 10, __pyx_L1_error)
 
-  /* "alphakit/factor/analysis.pyx":50
+  /* "alphakit/factor/analysis.pyx":53
  * 
  * 
- * def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):             # <<<<<<<<<<<<<<
- *     invar = dummy * invar
- *     disp = factor_stat(dummy, invar)
+ * def factor_one(dummy,             # <<<<<<<<<<<<<<
+ *                invar,
+ *                ret_f1d,
  */
-  __pyx_tuple__8 = PyTuple_Pack(29, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_ret_f1d, __pyx_n_s_freq, __pyx_n_s_hold, __pyx_n_s_group, __pyx_n_s_skip, __pyx_n_s_savepath, __pyx_n_s_disp, __pyx_n_s_invar_score, __pyx_n_s_weighT, __pyx_n_s_weightB, __pyx_n_s_weight, __pyx_n_s_stockNum, __pyx_n_s_outpnl1, __pyx_n_s_turnover1, __pyx_n_s_ic_series1, __pyx_n_s_outpnl2, __pyx_n_s_turnover2, __pyx_n_s_ic_series2, __pyx_n_s_outpnl3, __pyx_n_s_turnover3, __pyx_n_s_ic_series3, __pyx_n_s_outpnl, __pyx_n_s_turnover, __pyx_n_s_ic_series, __pyx_n_s_pnlstat, __pyx_n_s_gret, __pyx_n_s_gret_stat); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(30, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_ret_f1d, __pyx_n_s_freq, __pyx_n_s_hold, __pyx_n_s_group, __pyx_n_s_skip, __pyx_n_s_checkna, __pyx_n_s_savepath, __pyx_n_s_disp, __pyx_n_s_invar_score, __pyx_n_s_weighT, __pyx_n_s_weightB, __pyx_n_s_weight, __pyx_n_s_stockNum, __pyx_n_s_outpnl1, __pyx_n_s_turnover1, __pyx_n_s_ic_series1, __pyx_n_s_outpnl2, __pyx_n_s_turnover2, __pyx_n_s_ic_series2, __pyx_n_s_outpnl3, __pyx_n_s_turnover3, __pyx_n_s_ic_series3, __pyx_n_s_outpnl, __pyx_n_s_turnover, __pyx_n_s_ic_series, __pyx_n_s_pnlstat, __pyx_n_s_gret, __pyx_n_s_gret_stat); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(8, 0, 29, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_analysis_pyx, __pyx_n_s_factor_one, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(9, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_analysis_pyx, __pyx_n_s_factor_one, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4579,24 +4785,24 @@
  *     if invar is not None:
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_8analysis_1factor_plot, NULL, __pyx_n_s_alphakit_factor_analysis); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_factor_plot, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "alphakit/factor/analysis.pyx":50
+  /* "alphakit/factor/analysis.pyx":53
  * 
  * 
- * def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):             # <<<<<<<<<<<<<<
- *     invar = dummy * invar
- *     disp = factor_stat(dummy, invar)
+ * def factor_one(dummy,             # <<<<<<<<<<<<<<
+ *                invar,
+ *                ret_f1d,
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_8analysis_3factor_one, NULL, __pyx_n_s_alphakit_factor_analysis); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_8analysis_3factor_one, NULL, __pyx_n_s_alphakit_factor_analysis); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_factor_one, __pyx_t_2) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_factor_one, __pyx_t_2) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "alphakit/factor/analysis.pyx":1
  * # -*- coding: utf-8 -*-             # <<<<<<<<<<<<<<
  * import numpy as np
  * import pandas as pd
  */
```

### Comparing `Alphakit-1.2.0/alphakit/factor/analysis.pyx` & `Alphakit-1.2.1/alphakit/factor/analysis.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -17,24 +17,27 @@
         ax2 = plt.subplot(222)
         df_factor_plt = gret.cumsum()
         df_factor_plt.index = df_factor_plt.index.astype('datetime64[ns]')
         ax2.plot(df_factor_plt, label=gret.columns)
         ax2.legend(loc='lower left')
 
         ax4 = plt.subplot(224)
-        gnline = gret['GN'].mean()
-        gret.drop('GN', axis=1, inplace=True)
+        gnline = None
+        if 'GN' in gret.columns:
+            gnline = gret['GN'].mean()
+            gret.drop('GN', axis=1, inplace=True)
         gretplt = pd.DataFrame(gret.mean())
         gretplt['level'] = 0
         ax4.plot(gretplt, marker='.')
-        po = abs(gretplt[0] - gnline).reset_index(drop=True)
-        po1 = po.nsmallest(1).index[0]
-        if not np.isnan(gnline):
-            ax4.scatter(po1, gnline, s=150, marker='*', color='green')
-            ax4.text(po1 + 0.2, gnline, 'GN')
+        if gnline is not None:
+            po = abs(gretplt[0] - gnline).reset_index(drop=True)
+            po1 = po.nsmallest(1).index[0]
+            if not np.isnan(gnline):
+                ax4.scatter(po1, gnline, s=150, marker='*', color='green')
+                ax4.text(po1 + 0.2, gnline, 'GN')
         group = len(gretplt) - 1
         ax4.set_xticks(np.linspace(0, group, group, endpoint=True))
     if outpnl is not None:
         ax3 = plt.subplot(223)
         pnlplt = outpnl.cumsum()
         pnlplt.index = pnlplt.index.astype('datetime64[ns]')
         ax3.plot(pnlplt)
@@ -43,27 +46,52 @@
         plt.show(block=False)
         plt.pause(3)
         plt.close('all')
     else:
         plt.show(block=True)
 
 
-def factor_one(dummy, invar, ret_f1d, freq=252, hold=1, group=10, skip=0, savepath=''):
+def factor_one(dummy,
+               invar,
+               ret_f1d,
+               freq=252,
+               hold=1,
+               group=10,
+               skip=0,
+               checkna=True,
+               savepath=''):
     invar = dummy * invar
     disp = factor_stat(dummy, invar)
     invar_score = factor_score_sig(invar)
     weighT, weightB, weight, stockNum = factorToWeight(invar_score, hold)
     disp['TopNum'] = stockNum['TOP'].mean()
     disp['BotNum'] = stockNum['BOT'].mean()
-    outpnl1, turnover1, ic_series1 = factor_pnl(dummy, weighT, ret_f1d, skip, type='all')
-    outpnl2, turnover2, ic_series2 = factor_pnl(dummy, weightB, ret_f1d, skip, type='all')
-    outpnl3, turnover3, ic_series3 = factor_pnl(dummy, weight, ret_f1d, skip, type='all')
+    outpnl1, turnover1, ic_series1 = factor_pnl(dummy,
+                                                weighT,
+                                                ret_f1d,
+                                                skip,
+                                                type='all')
+    outpnl2, turnover2, ic_series2 = factor_pnl(dummy,
+                                                weightB,
+                                                ret_f1d,
+                                                skip,
+                                                type='all')
+    outpnl3, turnover3, ic_series3 = factor_pnl(dummy,
+                                                weight,
+                                                ret_f1d,
+                                                skip,
+                                                type='all')
     outpnl = pd.concat([outpnl1, outpnl2, outpnl3], axis=1)
     outpnl.columns = ['TOP', 'BOT', 'TMB']
     turnover = pd.concat([turnover1, turnover2, turnover3], axis=1)
     turnover.columns = ['TOP', 'BOT', 'TMB']
     ic_series = pd.concat([ic_series1, ic_series2, ic_series3], axis=1)
     ic_series.columns = ['TOP', 'BOT', 'TMB']
-    pnlstat = pnl_metrics(freq, outpnl, turnover, ic_series, usecol=['TOP', 'BOT', 'TMB'])
-    gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip)
+    pnlstat = pnl_metrics(freq,
+                          outpnl,
+                          turnover,
+                          ic_series,
+                          usecol=['TOP', 'BOT', 'TMB'])
+    gret, gret_stat = factor_group(dummy, invar, ret_f1d, group, hold, skip,
+                                   checkna)
     factor_plot(dummy, invar, gret, outpnl, savepath)
     return disp, outpnl, pnlstat, gret_stat
```

### Comparing `Alphakit-1.2.0/alphakit/factor/metrics.c` & `Alphakit-1.2.1/alphakit/factor/metrics.c`

 * *Files 2% similar despite different names*

```diff
@@ -1358,15 +1358,14 @@
 static const char __pyx_k_stack[] = "stack";
 static const char __pyx_k_zeror[] = "zeror";
 static const char __pyx_k_Series[] = "Series";
 static const char __pyx_k_astype[] = "astype";
 static const char __pyx_k_calmar[] = "calmar";
 static const char __pyx_k_concat[] = "concat";
 static const char __pyx_k_cumsum[] = "cumsum";
-static const char __pyx_k_dropna[] = "dropna";
 static const char __pyx_k_er_fnd[] = "er_fnd";
 static const char __pyx_k_factor[] = "factor";
 static const char __pyx_k_gnline[] = "gnline";
 static const char __pyx_k_icmean[] = "icmean";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_median[] = "median";
 static const char __pyx_k_method[] = "method";
@@ -1378,17 +1377,17 @@
 static const char __pyx_k_pandas[] = "pandas";
 static const char __pyx_k_rmaxdd[] = "rmaxdd";
 static const char __pyx_k_test_2[] = "__test__";
 static const char __pyx_k_ticker[] = "ticker";
 static const char __pyx_k_usecol[] = "usecol";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_weight[] = "weight";
+static const char __pyx_k_checkna[] = "checkna";
 static const char __pyx_k_columns[] = "columns";
 static const char __pyx_k_groupby[] = "groupby";
-static const char __pyx_k_inplace[] = "inplace";
 static const char __pyx_k_nanmean[] = "nanmean";
 static const char __pyx_k_ret_f1d[] = "ret_f1d";
 static const char __pyx_k_rolling[] = "rolling";
 static const char __pyx_k_unstack[] = "unstack";
 static const char __pyx_k_corrwith[] = "corrwith";
 static const char __pyx_k_megedata[] = "megedata";
 static const char __pyx_k_nanframe[] = "nanframe";
@@ -1424,22 +1423,22 @@
 static PyObject *__pyx_n_s_Series;
 static PyObject *__pyx_n_s_all;
 static PyObject *__pyx_n_s_alphakit_factor_metrics;
 static PyObject *__pyx_kp_s_alphakit_factor_metrics_pyx;
 static PyObject *__pyx_n_s_astype;
 static PyObject *__pyx_n_s_axis;
 static PyObject *__pyx_n_s_calmar;
+static PyObject *__pyx_n_s_checkna;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_concat;
 static PyObject *__pyx_n_s_corrwith;
 static PyObject *__pyx_n_s_count;
 static PyObject *__pyx_n_s_cumsum;
 static PyObject *__pyx_n_s_disp;
-static PyObject *__pyx_n_s_dropna;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dummy;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_er_fnd;
 static PyObject *__pyx_n_s_exp;
 static PyObject *__pyx_n_s_expanding;
@@ -1461,15 +1460,14 @@
 static PyObject *__pyx_n_s_ic;
 static PyObject *__pyx_n_s_ic_series;
 static PyObject *__pyx_n_s_icir;
 static PyObject *__pyx_n_s_icmean;
 static PyObject *__pyx_n_s_idx;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_index;
-static PyObject *__pyx_n_s_inplace;
 static PyObject *__pyx_n_s_int;
 static PyObject *__pyx_n_s_invar;
 static PyObject *__pyx_n_s_isna;
 static PyObject *__pyx_n_s_level;
 static PyObject *__pyx_n_s_loc;
 static PyObject *__pyx_n_s_log;
 static PyObject *__pyx_n_s_main;
@@ -1540,15 +1538,15 @@
 static PyObject *__pyx_n_s_weight;
 static PyObject *__pyx_n_s_win;
 static PyObject *__pyx_n_s_zeror;
 static PyObject *__pyx_pf_8alphakit_6factor_7metrics_factor_stat(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar); /* proto */
 static PyObject *__pyx_pf_8alphakit_6factor_7metrics_2factor_pnl(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_weight, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_skip, PyObject *__pyx_v_type); /* proto */
 static PyObject *__pyx_pf_8alphakit_6factor_7metrics_4pnl_metrics(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_freq, PyObject *__pyx_v_outpnl, PyObject *__pyx_v_turnover, PyObject *__pyx_v_ic_series, PyObject *__pyx_v_usecol); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_8alphakit_6factor_7metrics_6factor_group(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_group, PyObject *__pyx_v_hold, PyObject *__pyx_v_skip); /* proto */
+static PyObject *__pyx_pf_8alphakit_6factor_7metrics_6factor_group(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_group, PyObject *__pyx_v_hold, PyObject *__pyx_v_skip, PyObject *__pyx_v_checkna); /* proto */
 static PyObject *__pyx_float_0_5;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
@@ -3549,45 +3547,49 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "alphakit/factor/metrics.pyx":71
  * 
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):             # <<<<<<<<<<<<<<
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
  *         print('skip must >=0')
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8alphakit_6factor_7metrics_7factor_group(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8alphakit_6factor_7metrics_6factor_group[] = "factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0)";
+static char __pyx_doc_8alphakit_6factor_7metrics_6factor_group[] = "factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True)";
 static PyMethodDef __pyx_mdef_8alphakit_6factor_7metrics_7factor_group = {"factor_group", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8alphakit_6factor_7metrics_7factor_group, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8alphakit_6factor_7metrics_6factor_group};
 static PyObject *__pyx_pw_8alphakit_6factor_7metrics_7factor_group(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_dummy = 0;
   PyObject *__pyx_v_invar = 0;
   PyObject *__pyx_v_ret_f1d = 0;
   PyObject *__pyx_v_group = 0;
   PyObject *__pyx_v_hold = 0;
   PyObject *__pyx_v_skip = 0;
+  PyObject *__pyx_v_checkna = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("factor_group (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dummy,&__pyx_n_s_invar,&__pyx_n_s_ret_f1d,&__pyx_n_s_group,&__pyx_n_s_hold,&__pyx_n_s_skip,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dummy,&__pyx_n_s_invar,&__pyx_n_s_ret_f1d,&__pyx_n_s_group,&__pyx_n_s_hold,&__pyx_n_s_skip,&__pyx_n_s_checkna,0};
+    PyObject* values[7] = {0,0,0,0,0,0,0};
     values[4] = ((PyObject *)__pyx_int_1);
     values[5] = ((PyObject *)__pyx_int_0);
+    values[6] = ((PyObject *)Py_True);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -3604,46 +3606,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dummy)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_invar)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 6, 1); __PYX_ERR(0, 71, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 7, 1); __PYX_ERR(0, 71, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ret_f1d)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 6, 2); __PYX_ERR(0, 71, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 7, 2); __PYX_ERR(0, 71, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_group)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 6, 3); __PYX_ERR(0, 71, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 7, 3); __PYX_ERR(0, 71, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hold);
           if (value) { values[4] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_skip);
           if (value) { values[5] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_checkna);
+          if (value) { values[6] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "factor_group") < 0)) __PYX_ERR(0, 71, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -3654,31 +3664,32 @@
     }
     __pyx_v_dummy = values[0];
     __pyx_v_invar = values[1];
     __pyx_v_ret_f1d = values[2];
     __pyx_v_group = values[3];
     __pyx_v_hold = values[4];
     __pyx_v_skip = values[5];
+    __pyx_v_checkna = values[6];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 71, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("factor_group", 0, 4, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 71, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("alphakit.factor.metrics.factor_group", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8alphakit_6factor_7metrics_6factor_group(__pyx_self, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip);
+  __pyx_r = __pyx_pf_8alphakit_6factor_7metrics_6factor_group(__pyx_self, __pyx_v_dummy, __pyx_v_invar, __pyx_v_ret_f1d, __pyx_v_group, __pyx_v_hold, __pyx_v_skip, __pyx_v_checkna);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "alphakit/factor/metrics.pyx":93
+/* "alphakit/factor/metrics.pyx":94
  *     megedata.index.names = ['tradingday', 'ticker']
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))             # <<<<<<<<<<<<<<
  *     if not nanframe.empty:
  *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  */
 
@@ -3702,20 +3713,20 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_x, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_x, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_n_s_G, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_n_s_G, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
@@ -3729,20 +3740,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "alphakit/factor/metrics.pyx":71
  * 
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):             # <<<<<<<<<<<<<<
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
  *         print('skip must >=0')
  */
 
-static PyObject *__pyx_pf_8alphakit_6factor_7metrics_6factor_group(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_group, PyObject *__pyx_v_hold, PyObject *__pyx_v_skip) {
+static PyObject *__pyx_pf_8alphakit_6factor_7metrics_6factor_group(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dummy, PyObject *__pyx_v_invar, PyObject *__pyx_v_ret_f1d, PyObject *__pyx_v_group, PyObject *__pyx_v_hold, PyObject *__pyx_v_skip, PyObject *__pyx_v_checkna) {
   PyObject *__pyx_v_ret_f1d_skip = NULL;
   PyObject *__pyx_v_ret_mkt_fnd = NULL;
   PyObject *__pyx_v_er_fnd = NULL;
   PyObject *__pyx_v_megedata = NULL;
   PyObject *__pyx_v_nanframe = NULL;
   PyObject *__pyx_v_gret = NULL;
   PyObject *__pyx_v_gnline = NULL;
@@ -3765,26 +3776,26 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factor_group", 0);
   __Pyx_INCREF(__pyx_v_invar);
   __Pyx_INCREF(__pyx_v_ret_f1d);
 
   /* "alphakit/factor/metrics.pyx":72
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):
  *     if skip < 0:             # <<<<<<<<<<<<<<
  *         print('skip must >=0')
  *         return None
  */
   __pyx_t_1 = PyObject_RichCompare(__pyx_v_skip, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "alphakit/factor/metrics.pyx":73
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):
  *     if skip < 0:
  *         print('skip must >=0')             # <<<<<<<<<<<<<<
  *         return None
  *     invar = invar * dummy
  */
     if (__Pyx_PrintOne(0, __pyx_kp_s_skip_must_0) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
 
@@ -3797,15 +3808,15 @@
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
     /* "alphakit/factor/metrics.pyx":72
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):
  *     if skip < 0:             # <<<<<<<<<<<<<<
  *         print('skip must >=0')
  *         return None
  */
   }
 
   /* "alphakit/factor/metrics.pyx":75
@@ -4087,15 +4098,15 @@
   __pyx_t_4 = 0;
 
   /* "alphakit/factor/metrics.pyx":84
  *     megedata = np.exp(
  *         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)             # <<<<<<<<<<<<<<
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']
- *     nanframe = megedata.loc[(megedata.factor.isna()) & (~megedata.dummy.isna())]
+ *     megedata = megedata.loc[megedata.dummy == 1]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_concat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_invar, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L1_error)
@@ -4159,16 +4170,16 @@
   __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "alphakit/factor/metrics.pyx":85
  *         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']             # <<<<<<<<<<<<<<
- *     nanframe = megedata.loc[(megedata.factor.isna()) & (~megedata.dummy.isna())]
- *     megedata.dropna(inplace=True)
+ *     megedata = megedata.loc[megedata.dummy == 1]
+ *     nanframe = megedata.loc[megedata.factor.isna()]
  */
   __pyx_t_4 = PyList_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_er_fnd);
   __Pyx_GIVEREF(__pyx_n_s_er_fnd);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_er_fnd);
   __Pyx_INCREF(__pyx_n_s_factor);
@@ -4179,243 +4190,258 @@
   PyList_SET_ITEM(__pyx_t_4, 2, __pyx_n_s_dummy);
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_megedata, __pyx_n_s_columns, __pyx_t_4) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "alphakit/factor/metrics.pyx":86
  *     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
  *     megedata.columns = ['er_fnd', 'factor', 'dummy']
- *     nanframe = megedata.loc[(megedata.factor.isna()) & (~megedata.dummy.isna())]             # <<<<<<<<<<<<<<
- *     megedata.dropna(inplace=True)
- *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
+ *     megedata = megedata.loc[megedata.dummy == 1]             # <<<<<<<<<<<<<<
+ *     nanframe = megedata.loc[megedata.factor.isna()]
+ *     megedata = megedata.loc[~megedata.factor.isna()]
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_dummy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_8 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_isna); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = NULL;
+  __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "alphakit/factor/metrics.pyx":87
+ *     megedata.columns = ['er_fnd', 'factor', 'dummy']
+ *     megedata = megedata.loc[megedata.dummy == 1]
+ *     nanframe = megedata.loc[megedata.factor.isna()]             # <<<<<<<<<<<<<<
+ *     megedata = megedata.loc[~megedata.factor.isna()]
+ *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_isna); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_8)) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_dummy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_isna); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Invert(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_And(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_nanframe = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_v_nanframe = __pyx_t_5;
+  __pyx_t_5 = 0;
 
-  /* "alphakit/factor/metrics.pyx":87
- *     megedata.columns = ['er_fnd', 'factor', 'dummy']
- *     nanframe = megedata.loc[(megedata.factor.isna()) & (~megedata.dummy.isna())]
- *     megedata.dropna(inplace=True)             # <<<<<<<<<<<<<<
+  /* "alphakit/factor/metrics.pyx":88
+ *     megedata = megedata.loc[megedata.dummy == 1]
+ *     nanframe = megedata.loc[megedata.factor.isna()]
+ *     megedata = megedata.loc[~megedata.factor.isna()]             # <<<<<<<<<<<<<<
  *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_dropna); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_inplace, Py_True) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_isna); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_8 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyNumber_Invert(__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(__pyx_v_megedata, __pyx_t_8);
+  __pyx_t_8 = 0;
 
-  /* "alphakit/factor/metrics.pyx":88
- *     nanframe = megedata.loc[(megedata.factor.isna()) & (~megedata.dummy.isna())]
- *     megedata.dropna(inplace=True)
+  /* "alphakit/factor/metrics.pyx":89
+ *     nanframe = megedata.loc[megedata.factor.isna()]
+ *     megedata = megedata.loc[~megedata.factor.isna()]
  *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)             # <<<<<<<<<<<<<<
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  */
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_factor); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_groupby); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_groupby); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_group_keys, Py_False) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_group_keys, Py_False) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_rank); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_rank); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pct, Py_True) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_5) < 0)) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_pct, Py_True) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_4) < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "alphakit/factor/metrics.pyx":89
- *     megedata.dropna(inplace=True)
+  /* "alphakit/factor/metrics.pyx":90
+ *     megedata = megedata.loc[~megedata.factor.isna()]
  *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1             # <<<<<<<<<<<<<<
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  *     megedata.index.names = ['tradingday', 'ticker']
  */
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_3, __pyx_v_group); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_8 = PyNumber_Multiply(__pyx_t_5, __pyx_v_group); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_astype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_s_int) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_int);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_n_s_int) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_int);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_5) < 0)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_megedata, __pyx_n_s_quantile, __pyx_t_3) < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "alphakit/factor/metrics.pyx":90
+  /* "alphakit/factor/metrics.pyx":91
  *     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group             # <<<<<<<<<<<<<<
  *     megedata.index.names = ['tradingday', 'ticker']
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_loc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_group, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_megedata, __pyx_n_s_quantile); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_5, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_v_group, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_quantile);
   __Pyx_GIVEREF(__pyx_n_s_quantile);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_s_quantile);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_n_s_quantile);
   __pyx_t_1 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_t_4, __pyx_v_group) < 0)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(PyObject_SetItem(__pyx_t_5, __pyx_t_8, __pyx_v_group) < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "alphakit/factor/metrics.pyx":91
+  /* "alphakit/factor/metrics.pyx":92
  *     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  *     megedata.index.names = ['tradingday', 'ticker']             # <<<<<<<<<<<<<<
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
  */
-  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
-  PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_tradingday);
+  PyList_SET_ITEM(__pyx_t_8, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_ticker);
   __Pyx_GIVEREF(__pyx_n_s_ticker);
-  PyList_SET_ITEM(__pyx_t_4, 1, __pyx_n_s_ticker);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_3, __pyx_n_s_names, __pyx_t_4) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyList_SET_ITEM(__pyx_t_8, 1, __pyx_n_s_ticker);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_names, __pyx_t_8) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "alphakit/factor/metrics.pyx":92
+  /* "alphakit/factor/metrics.pyx":93
  *     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
  *     megedata.index.names = ['tradingday', 'ticker']
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)             # <<<<<<<<<<<<<<
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
  *     if not nanframe.empty:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_megedata, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_10 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_groupby); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_groupby); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_n_s_tradingday);
   __Pyx_GIVEREF(__pyx_n_s_tradingday);
   PyList_SET_ITEM(__pyx_t_10, 0, __pyx_n_s_tradingday);
   __Pyx_INCREF(__pyx_n_s_quantile);
   __Pyx_GIVEREF(__pyx_n_s_quantile);
   PyList_SET_ITEM(__pyx_t_10, 1, __pyx_n_s_quantile);
@@ -4425,281 +4451,300 @@
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
-  __pyx_t_8 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
+  __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_8, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_mean); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
+  __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_unstack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unstack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_8);
+  __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_8, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_gret = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_v_gret = __pyx_t_5;
+  __pyx_t_5 = 0;
 
-  /* "alphakit/factor/metrics.pyx":93
+  /* "alphakit/factor/metrics.pyx":94
  *     megedata.index.names = ['tradingday', 'ticker']
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))             # <<<<<<<<<<<<<<
  *     if not nanframe.empty:
  *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Series); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Series); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8alphakit_6factor_7metrics_12factor_group_lambda, 0, __pyx_n_s_factor_group_locals_lambda, NULL, __pyx_n_s_alphakit_factor_metrics, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8alphakit_6factor_7metrics_12factor_group_lambda, 0, __pyx_n_s_factor_group_locals_lambda, NULL, __pyx_n_s_alphakit_factor_metrics, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_4, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_shape); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_8, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_0);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_int_0);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
   __pyx_t_1 = 0;
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_gret, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_gret, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "alphakit/factor/metrics.pyx":94
+  /* "alphakit/factor/metrics.pyx":95
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
  *     if not nanframe.empty:             # <<<<<<<<<<<<<<
  *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  *     else:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_11 = ((!__pyx_t_2) != 0);
   if (__pyx_t_11) {
 
-    /* "alphakit/factor/metrics.pyx":95
+    /* "alphakit/factor/metrics.pyx":96
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
  *     if not nanframe.empty:
  *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()             # <<<<<<<<<<<<<<
  *     else:
  *         gnline = np.nan
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_groupby); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_nanframe, __pyx_n_s_groupby); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_er_fnd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mean); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_mean); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_v_gnline = __pyx_t_3;
-    __pyx_t_3 = 0;
+    __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_v_gnline = __pyx_t_5;
+    __pyx_t_5 = 0;
 
-    /* "alphakit/factor/metrics.pyx":94
+    /* "alphakit/factor/metrics.pyx":95
  *     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
  *     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
  *     if not nanframe.empty:             # <<<<<<<<<<<<<<
  *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "alphakit/factor/metrics.pyx":97
+  /* "alphakit/factor/metrics.pyx":98
  *         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
  *     else:
  *         gnline = np.nan             # <<<<<<<<<<<<<<
- *     gret['GN'] = gnline
- *     gret_stat = gret.mean()
+ *     if checkna:
+ *         gret['GN'] = gnline
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_gnline = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nan); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_v_gnline = __pyx_t_8;
+    __pyx_t_8 = 0;
   }
   __pyx_L4:;
 
-  /* "alphakit/factor/metrics.pyx":98
+  /* "alphakit/factor/metrics.pyx":99
  *     else:
  *         gnline = np.nan
- *     gret['GN'] = gnline             # <<<<<<<<<<<<<<
+ *     if checkna:             # <<<<<<<<<<<<<<
+ *         gret['GN'] = gnline
+ *     gret_stat = gret.mean()
+ */
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_checkna); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (__pyx_t_11) {
+
+    /* "alphakit/factor/metrics.pyx":100
+ *         gnline = np.nan
+ *     if checkna:
+ *         gret['GN'] = gnline             # <<<<<<<<<<<<<<
  *     gret_stat = gret.mean()
  *     return gret, gret_stat
  */
-  if (unlikely(PyObject_SetItem(__pyx_v_gret, __pyx_n_s_GN, __pyx_v_gnline) < 0)) __PYX_ERR(0, 98, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_gret, __pyx_n_s_GN, __pyx_v_gnline) < 0)) __PYX_ERR(0, 100, __pyx_L1_error)
 
-  /* "alphakit/factor/metrics.pyx":99
+    /* "alphakit/factor/metrics.pyx":99
+ *     else:
  *         gnline = np.nan
- *     gret['GN'] = gnline
+ *     if checkna:             # <<<<<<<<<<<<<<
+ *         gret['GN'] = gnline
+ *     gret_stat = gret.mean()
+ */
+  }
+
+  /* "alphakit/factor/metrics.pyx":101
+ *     if checkna:
+ *         gret['GN'] = gnline
  *     gret_stat = gret.mean()             # <<<<<<<<<<<<<<
  *     return gret, gret_stat
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_gret, __pyx_n_s_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_gret_stat = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_v_gret_stat = __pyx_t_8;
+  __pyx_t_8 = 0;
 
-  /* "alphakit/factor/metrics.pyx":100
- *     gret['GN'] = gnline
+  /* "alphakit/factor/metrics.pyx":102
+ *         gret['GN'] = gnline
  *     gret_stat = gret.mean()
  *     return gret, gret_stat             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_v_gret);
   __Pyx_GIVEREF(__pyx_v_gret);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_gret);
+  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_gret);
   __Pyx_INCREF(__pyx_v_gret_stat);
   __Pyx_GIVEREF(__pyx_v_gret_stat);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_gret_stat);
-  __pyx_r = __pyx_t_4;
-  __pyx_t_4 = 0;
+  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_gret_stat);
+  __pyx_r = __pyx_t_8;
+  __pyx_t_8 = 0;
   goto __pyx_L0;
 
   /* "alphakit/factor/metrics.pyx":71
  * 
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):             # <<<<<<<<<<<<<<
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
  *         print('skip must >=0')
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -4781,22 +4826,22 @@
   {&__pyx_n_s_Series, __pyx_k_Series, sizeof(__pyx_k_Series), 0, 0, 1, 1},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
   {&__pyx_n_s_alphakit_factor_metrics, __pyx_k_alphakit_factor_metrics, sizeof(__pyx_k_alphakit_factor_metrics), 0, 0, 1, 1},
   {&__pyx_kp_s_alphakit_factor_metrics_pyx, __pyx_k_alphakit_factor_metrics_pyx, sizeof(__pyx_k_alphakit_factor_metrics_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_astype, __pyx_k_astype, sizeof(__pyx_k_astype), 0, 0, 1, 1},
   {&__pyx_n_s_axis, __pyx_k_axis, sizeof(__pyx_k_axis), 0, 0, 1, 1},
   {&__pyx_n_s_calmar, __pyx_k_calmar, sizeof(__pyx_k_calmar), 0, 0, 1, 1},
+  {&__pyx_n_s_checkna, __pyx_k_checkna, sizeof(__pyx_k_checkna), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_concat, __pyx_k_concat, sizeof(__pyx_k_concat), 0, 0, 1, 1},
   {&__pyx_n_s_corrwith, __pyx_k_corrwith, sizeof(__pyx_k_corrwith), 0, 0, 1, 1},
   {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
   {&__pyx_n_s_cumsum, __pyx_k_cumsum, sizeof(__pyx_k_cumsum), 0, 0, 1, 1},
   {&__pyx_n_s_disp, __pyx_k_disp, sizeof(__pyx_k_disp), 0, 0, 1, 1},
-  {&__pyx_n_s_dropna, __pyx_k_dropna, sizeof(__pyx_k_dropna), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dummy, __pyx_k_dummy, sizeof(__pyx_k_dummy), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_er_fnd, __pyx_k_er_fnd, sizeof(__pyx_k_er_fnd), 0, 0, 1, 1},
   {&__pyx_n_s_exp, __pyx_k_exp, sizeof(__pyx_k_exp), 0, 0, 1, 1},
   {&__pyx_n_s_expanding, __pyx_k_expanding, sizeof(__pyx_k_expanding), 0, 0, 1, 1},
@@ -4818,15 +4863,14 @@
   {&__pyx_n_s_ic, __pyx_k_ic, sizeof(__pyx_k_ic), 0, 0, 1, 1},
   {&__pyx_n_s_ic_series, __pyx_k_ic_series, sizeof(__pyx_k_ic_series), 0, 0, 1, 1},
   {&__pyx_n_s_icir, __pyx_k_icir, sizeof(__pyx_k_icir), 0, 0, 1, 1},
   {&__pyx_n_s_icmean, __pyx_k_icmean, sizeof(__pyx_k_icmean), 0, 0, 1, 1},
   {&__pyx_n_s_idx, __pyx_k_idx, sizeof(__pyx_k_idx), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
-  {&__pyx_n_s_inplace, __pyx_k_inplace, sizeof(__pyx_k_inplace), 0, 0, 1, 1},
   {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
   {&__pyx_n_s_invar, __pyx_k_invar, sizeof(__pyx_k_invar), 0, 0, 1, 1},
   {&__pyx_n_s_isna, __pyx_k_isna, sizeof(__pyx_k_isna), 0, 0, 1, 1},
   {&__pyx_n_s_level, __pyx_k_level, sizeof(__pyx_k_level), 0, 0, 1, 1},
   {&__pyx_n_s_loc, __pyx_k_loc, sizeof(__pyx_k_loc), 0, 0, 1, 1},
   {&__pyx_n_s_log, __pyx_k_log, sizeof(__pyx_k_log), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
@@ -4896,16 +4940,16 @@
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_weight, __pyx_k_weight, sizeof(__pyx_k_weight), 0, 0, 1, 1},
   {&__pyx_n_s_win, __pyx_k_win, sizeof(__pyx_k_win), 0, 0, 1, 1},
   {&__pyx_n_s_zeror, __pyx_k_zeror, sizeof(__pyx_k_zeror), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 93, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 94, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -4946,22 +4990,22 @@
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
   __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(5, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_metrics_pyx, __pyx_n_s_pnl_metrics, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 40, __pyx_L1_error)
 
   /* "alphakit/factor/metrics.pyx":71
  * 
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):             # <<<<<<<<<<<<<<
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
  *         print('skip must >=0')
  */
-  __pyx_tuple__7 = PyTuple_Pack(14, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_ret_f1d, __pyx_n_s_group, __pyx_n_s_hold, __pyx_n_s_skip, __pyx_n_s_ret_f1d_skip, __pyx_n_s_ret_mkt_fnd, __pyx_n_s_er_fnd, __pyx_n_s_megedata, __pyx_n_s_nanframe, __pyx_n_s_gret, __pyx_n_s_gnline, __pyx_n_s_gret_stat); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(15, __pyx_n_s_dummy, __pyx_n_s_invar, __pyx_n_s_ret_f1d, __pyx_n_s_group, __pyx_n_s_hold, __pyx_n_s_skip, __pyx_n_s_checkna, __pyx_n_s_ret_f1d_skip, __pyx_n_s_ret_mkt_fnd, __pyx_n_s_er_fnd, __pyx_n_s_megedata, __pyx_n_s_nanframe, __pyx_n_s_gret, __pyx_n_s_gnline, __pyx_n_s_gret_stat); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(6, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_metrics_pyx, __pyx_n_s_factor_group, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(7, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_alphakit_factor_metrics_pyx, __pyx_n_s_factor_group, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5299,15 +5343,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pnl_metrics, __pyx_t_1) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "alphakit/factor/metrics.pyx":71
  * 
  * 
- * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):             # <<<<<<<<<<<<<<
+ * def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):             # <<<<<<<<<<<<<<
  *     if skip < 0:
  *         print('skip must >=0')
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8alphakit_6factor_7metrics_7factor_group, NULL, __pyx_n_s_alphakit_factor_metrics); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_factor_group, __pyx_t_1) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `Alphakit-1.2.0/alphakit/factor/metrics.pyx` & `Alphakit-1.2.1/alphakit/factor/metrics.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -64,37 +64,39 @@
             ic_series = ic_series[usecol]
         icmean = ic_series.mean()
         disp.loc['ic'] = icmean
         disp.loc['icir'] = icmean / ic_series.std()
     return disp
 
 
-def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0):
+def factor_group(dummy, invar, ret_f1d, group, hold=1, skip=0, checkna=True):
     if skip < 0:
         print('skip must >=0')
         return None
     invar = invar * dummy
     ret_f1d = ret_f1d * dummy
     ret_f1d_skip = ret_f1d.shift(-skip)
     ret_f1d_skip = np.exp(ret_f1d_skip) - 1
     ret_mkt_fnd = (ret_f1d_skip * dummy).mean(axis=1)
     er_fnd = ret_f1d_skip.sub(ret_mkt_fnd, axis='rows')
     # 分层画图
     megedata = np.exp(
         np.log(er_fnd + 1).rolling(hold, min_periods=1).sum().shift(-(hold - 1)).stack() / hold) - 1
     megedata = pd.concat([megedata, invar.stack(), dummy.stack()], axis=1)
     megedata.columns = ['er_fnd', 'factor', 'dummy']
-    nanframe = megedata.loc[(megedata.factor.isna()) & (~megedata.dummy.isna())]
-    megedata.dropna(inplace=True)
+    megedata = megedata.loc[megedata.dummy == 1]
+    nanframe = megedata.loc[megedata.factor.isna()]
+    megedata = megedata.loc[~megedata.factor.isna()]
     megedata["quantile"] = megedata["factor"].groupby(level=0, group_keys=False).rank(pct=True)
     megedata["quantile"] = (megedata["quantile"] * group).astype('int') + 1
     megedata.loc[megedata['quantile'] == group + 1, 'quantile'] = group
     megedata.index.names = ['tradingday', 'ticker']
     gret = np.log(megedata.reset_index().groupby(['tradingday', 'quantile'])['er_fnd'].mean().unstack() + 1)
     gret.columns = pd.Series(map(lambda x: 'G' + str(x + 1), range(0, gret.shape[1])))
     if not nanframe.empty:
         gnline = nanframe.groupby(axis=0, level=0).er_fnd.mean()
     else:
         gnline = np.nan
-    gret['GN'] = gnline
+    if checkna:
+        gret['GN'] = gnline
     gret_stat = gret.mean()
     return gret, gret_stat
```

### Comparing `Alphakit-1.2.0/alphakit/factor/processing.c` & `Alphakit-1.2.1/alphakit/factor/processing.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/factor/processing.pyx` & `Alphakit-1.2.1/alphakit/factor/processing.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/factor/transform.c` & `Alphakit-1.2.1/alphakit/factor/transform.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/factor/transform.pyx` & `Alphakit-1.2.1/alphakit/factor/transform.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/alphakit/portfolio/combine.c` & `Alphakit-1.2.1/alphakit/portfolio/combine.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.0/setup.py` & `Alphakit-1.2.1/setup.py`

 * *Files identical despite different names*

