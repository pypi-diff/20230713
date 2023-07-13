# Comparing `tmp/hpcom-0.1.7.tar.gz` & `tmp/hpcom-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpcom-0.1.7.tar", last modified: Tue Jul 11 13:30:16 2023, max compression
+gzip compressed data, was "hpcom-0.1.8.tar", last modified: Thu Jul 13 15:39:56 2023, max compression
```

## Comparing `hpcom-0.1.7.tar` & `hpcom-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:30:16.055776 hpcom-0.1.7/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    35137 2022-11-10 15:49:50.000000 hpcom-0.1.7/LICENSE
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-11 13:30:16.055776 hpcom-0.1.7/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1080 2023-04-30 12:37:52.000000 hpcom-0.1.7/README.md
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:30:16.055776 hpcom-0.1.7/hpcom/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      239 2022-12-14 10:00:50.000000 hpcom-0.1.7/hpcom/__init__.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    47603 2023-07-11 13:29:01.000000 hpcom-0.1.7/hpcom/channel.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      434 2022-11-11 14:09:01.000000 hpcom-0.1.7/hpcom/decorators.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    13393 2022-11-23 13:08:09.000000 hpcom-0.1.7/hpcom/hpcom_old.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     4996 2023-04-13 16:56:44.000000 hpcom-0.1.7/hpcom/metrics.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     7485 2022-11-23 13:22:15.000000 hpcom-0.1.7/hpcom/modulation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      452 2023-04-12 17:22:11.000000 hpcom-0.1.7/hpcom/plot.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    23931 2023-07-11 13:29:01.000000 hpcom-0.1.7/hpcom/signal.py
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:30:16.055776 hpcom-0.1.7/hpcom.egg-info/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-11 13:30:16.000000 hpcom-0.1.7/hpcom.egg-info/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      425 2023-07-11 13:30:16.000000 hpcom-0.1.7/hpcom.egg-info/SOURCES.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-11 13:30:16.000000 hpcom-0.1.7/hpcom.egg-info/dependency_links.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        6 2023-07-11 13:30:16.000000 hpcom-0.1.7/hpcom.egg-info/top_level.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      707 2023-07-11 13:29:53.000000 hpcom-0.1.7/pyproject.toml
--rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-11 13:30:16.055776 hpcom-0.1.7/setup.cfg
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-11 13:30:16.055776 hpcom-0.1.7/tests/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2216 2023-07-06 13:53:07.000000 hpcom-0.1.7/tests/test_back_to_back.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1910 2023-01-18 15:52:29.000000 hpcom-0.1.7/tests/test_channel_model.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      719 2022-12-14 10:08:52.000000 hpcom-0.1.7/tests/test_generation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1730 2023-06-21 12:18:51.000000 hpcom-0.1.7/tests/test_ofdm_generation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2421 2022-12-14 11:09:37.000000 hpcom-0.1.7/tests/test_propagation.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.868414 hpcom-0.1.8/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    35137 2022-11-10 15:49:50.000000 hpcom-0.1.8/LICENSE
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-13 15:39:56.868414 hpcom-0.1.8/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1080 2023-04-30 12:37:52.000000 hpcom-0.1.8/README.md
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.864414 hpcom-0.1.8/hpcom/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      239 2022-12-14 10:00:50.000000 hpcom-0.1.8/hpcom/__init__.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    58698 2023-07-13 15:38:19.000000 hpcom-0.1.8/hpcom/channel.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      434 2022-11-11 14:09:01.000000 hpcom-0.1.8/hpcom/decorators.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    13393 2022-11-23 13:08:09.000000 hpcom-0.1.8/hpcom/hpcom_old.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     4996 2023-04-13 16:56:44.000000 hpcom-0.1.8/hpcom/metrics.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     7485 2022-11-23 13:22:15.000000 hpcom-0.1.8/hpcom/modulation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      452 2023-04-12 17:22:11.000000 hpcom-0.1.8/hpcom/plot.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    23931 2023-07-11 13:29:01.000000 hpcom-0.1.8/hpcom/signal.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.864414 hpcom-0.1.8/hpcom.egg-info/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      425 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        6 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/top_level.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      707 2023-07-13 15:38:19.000000 hpcom-0.1.8/pyproject.toml
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-13 15:39:56.868414 hpcom-0.1.8/setup.cfg
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.864414 hpcom-0.1.8/tests/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2216 2023-07-06 13:53:07.000000 hpcom-0.1.8/tests/test_back_to_back.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1910 2023-01-18 15:52:29.000000 hpcom-0.1.8/tests/test_channel_model.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      719 2022-12-14 10:08:52.000000 hpcom-0.1.8/tests/test_generation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1730 2023-06-21 12:18:51.000000 hpcom-0.1.8/tests/test_ofdm_generation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2421 2022-12-14 11:09:37.000000 hpcom-0.1.8/tests/test_propagation.py
```

### Comparing `hpcom-0.1.7/LICENSE` & `hpcom-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/PKG-INFO` & `hpcom-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcom
-Version: 0.1.7
+Version: 0.1.8
 Summary: High performance optical communication library
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpcom-0.1.7/README.md` & `hpcom-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/hpcom/channel.py` & `hpcom-0.1.8/hpcom/channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -980,8 +980,255 @@
         'points_y_found': points_y_found,
         'ber_x': ber_x,
         'ber_y': ber_y,
         'q_x': q_x,
         'q_y': q_y
     }
 
+    return result
+
+
+def transceiver_line_model(channel, wdm, bits=None, points=None, verbose=0, dbp=False, ft_filter_values_tx=None):
+    """
+        Simulates a full optical transmission line, including generation of a wavelength division multiplexed (WDM)
+        signal with multiple WDM channels, propagation through a specified channel, and detection at the receiver.
+
+        Args:
+            channel: object, channel through which the WDM signal is passed
+            wdm: dict, contains information about the WDM signal
+            bits: tuple, number of bits in the x (and y) component of the signal (optional)
+            points: tuple, points of the x (and y) component of the signal (optional)
+            channels_type: str: 'all' -- calculate metrics for all channels, 'middle' -- calculate only for middle (optional)
+            verbose: int: level of system messages. 0 -- nothing, 1 -- +metrics, 2 -- +time, 3 -- +everything (optional)
+            dbp: bool: flag to dbp algorithm. Only True if you calculate DBP for already received points (optional)
+            optimise: 'not' -- no optimisation, 'ber_x' -- optimise BER for x, 'evm_x' -- optimise EVM for x (optional)
+            ft_filter_values_tx:
+            ft_filter_values_rx:
+
+        Returns:
+            dict: containing the points and BER and Q-value of the signal in the x and y component
+
+            - 'points_x' -- an array of the points of the x component of the signal after processing
+            - 'points_orig_x' -- an array of the original points of the x component of the signal
+            - 'points_x_shifted' -- an array of the points of the x component of the signal after shifting
+            - 'points_x_found' -- an array of the nearest constellation points of the x component of the signal
+            - 'points_y' -- an array of the points of the y component of the signal after processing
+            - 'points_orig_y' -- an array of the original points of the y component of the signal
+            - 'points_y_shifted' -- an array of the points of the y component of the signal after shifting
+            - 'points_y_found' -- an array of the nearest constellation points of the y component of the signal
+            - 'ber_x' -- the bit error rate of the x component of the signal
+            - 'ber_y' -- the bit error rate of the y component of the signal
+            - 'q_x' -- the Q-value of the x component of the signal
+            - 'q_y' -- the Q-value of the y component of the signal
+
+        """
+
+    dt = 1. / wdm['sample_freq']
+
+    signal_x, signal_y, wdm_info = generate_wdm(wdm, bits=bits, points=points, ft_filter_values=ft_filter_values_tx)
+
+    points_x_orig = wdm_info['points_x']
+    points_y_orig = wdm_info['points_y']
+
+    ft_filter_values_x = wdm_info['ft_filter_values_x']
+    ft_filter_values_y = wdm_info['ft_filter_values_y']
+
+    np_signal = len(signal_x)
+
+    e_signal_x = get_energy(signal_x, dt * np_signal)
+    e_signal_y = get_energy(signal_y, dt * np_signal)
+    p_signal_x = get_average_power(signal_x, dt)
+    p_signal_y = get_average_power(signal_y, dt)
+    p_signal_correct = dbm_to_mw(wdm['p_ave_dbm']) / 1000 / wdm['n_polarisations'] * wdm['n_channels']
+    print("Average signal power (x / y): "
+          "%1.7f / %1.7f (has to be close to %1.7f)" % (p_signal_x, p_signal_y, p_signal_correct)) if verbose >= 3 else ...
+
+    # TODO: reconsider dbp logic
+    start_time = datetime.now()
+    if not dbp:
+        signal_x, signal_y = propagate_manakov(channel, signal_x, signal_y, wdm['sample_freq'])
+    else:
+        print('DBP')
+        channel_back = channel.copy()
+        channel_back['z_span'] = -channel['z_span']
+
+        # [propagate_manakov_backward] is the proper function for backpropagation
+        # which properly handle attenuation of the signal
+        # if you still wand to use [propagate_manakov] then you have to set alpha = -alpha for channel parameters
+        signal_x, signal_y = propagate_manakov_backward(channel_back, signal_x, signal_y, wdm['sample_freq'])
+    print("propagation took", (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
+
+    e_signal_x_prop = get_energy(signal_x, dt * np_signal)
+    e_signal_y_prop = get_energy(signal_y, dt * np_signal)
+
+    if verbose >= 3:
+        print("Signal energy before propagation (x / y):", e_signal_x, e_signal_y)
+        print("Signal energy after propagation (x / y):", e_signal_x_prop, e_signal_y_prop)
+        print("Signal energy difference (x / y):",
+              np.absolute(e_signal_x - e_signal_x_prop),
+              np.absolute(e_signal_y - e_signal_y_prop))
+
+    if not dbp:
+        signal_x, signal_y = dispersion_compensation_manakov(channel, signal_x, signal_y, 1. / wdm['sample_freq'])
+
+    result = {
+        'signal': [signal_x, signal_y],
+        'points_orig': [points_x_orig, points_y_orig],
+        'ft_filter_values': [ft_filter_values_x, ft_filter_values_y]
+        }
+
+    return result
+
+
+def receiver_model(wdm, signal, points_orig, ft_filter_values_rx,
+                   channels_type='all', verbose=0, optimise='not'):
+
+    signal_x = signal[0]
+    signal_y = signal[1]
+
+    samples_x = receiver_wdm(signal_x, ft_filter_values_rx[0], wdm)
+    samples_y = receiver_wdm(signal_y, ft_filter_values_rx[1], wdm)
+
+    points_x_orig = points_orig[0]
+    points_y_orig = points_orig[1]
+
+    # TODO: make CDC after receiver
+    # for k in range(wdm['n_channels']):
+    #     samples_x[k], samples_y[k] = dispersion_compensation(channel, samples_x[k], samples_y[k], wdm['downsampling_rate'] / wdm['sample_freq'])
+
+    # print(np.shape(samples_x))
+
+    sample_step = int(wdm['upsampling'] / wdm['downsampling_rate'])
+
+    # TODO: rewrite this part. Use one for and inside check if channel_type is 'all' or 'middle' and store only one
+    if channels_type == 'all':
+
+        points_x = []
+        points_y = []
+
+        points_x_shifted = []
+        points_y_shifted = []
+
+        for k in range(wdm['n_channels']):
+
+            points_x.append(get_points_wdm(samples_x[k], wdm))
+            points_y.append(get_points_wdm(samples_y[k], wdm))
+
+            nl_shift_x = nonlinear_shift(points_x[k], points_x_orig[k])
+            points_x_shifted.append(points_x[k] * nl_shift_x)
+
+            nl_shift_y = nonlinear_shift(points_y[k], points_y_orig[k])
+            points_y_shifted.append(points_y[k] * nl_shift_y)
+
+        mod_type = get_modulation_type_from_order(wdm['m_order'])
+        scale_constellation = get_scale_coef_constellation(mod_type) / np.sqrt(wdm['p_ave'] / wdm['n_polarisations'])
+
+        points_x_found = []
+        points_y_found = []
+
+        ber_x = []
+        ber_y = []
+        q_x = []
+        q_y = []
+        evm_x = []
+        evm_y = []
+
+        for k in range(wdm['n_channels']):
+            print('WDM channel', k) if verbose >= 1 else ...
+
+            start_time = datetime.now()
+            points_x_found.append(get_nearest_constellation_points_unscaled(points_x_shifted[k], mod_type))
+            points_y_found.append(get_nearest_constellation_points_unscaled(points_y_shifted[k], mod_type))
+            print("search x and y points took",
+                  (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
+
+            start_time = datetime.now()
+            ber_x.append(get_ber_by_points(points_x_orig[k] * scale_constellation, points_x_found[k], mod_type))
+            ber_y.append(get_ber_by_points(points_y_orig[k] * scale_constellation, points_y_found[k], mod_type))
+            print("ber for x and y took",
+                  (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
+
+            q_x.append(np.sqrt(2) * sp.special.erfcinv(2 * ber_x[k][0]))
+            q_y.append(np.sqrt(2) * sp.special.erfcinv(2 * ber_y[k][0]))
+
+            evm_x.append(get_evm(points_x_orig[k] * scale_constellation, points_x_shifted[k] * scale_constellation))
+            evm_y.append(get_evm(points_y_orig[k] * scale_constellation, points_y_shifted[k] * scale_constellation))
+
+            print("BER (x / y):", ber_x[k], ber_y[k]) if verbose >= 1 else ...
+            print(r'Q^2-factor (x / y):', q_x[k], q_y[k]) if verbose >= 1 else ...
+
+    elif channels_type == 'middle':
+
+        k = (wdm['n_channels'] - 1) // 2
+
+        samples_x_temp = samples_x[k]
+        samples_y_temp = samples_y[k]
+
+        points_x = samples_x_temp[::sample_step].numpy()
+        points_y = samples_y_temp[::sample_step].numpy()
+
+        nl_shift_x = nonlinear_shift(points_x, points_x_orig[k])
+        points_x_shifted = points_x * nl_shift_x
+
+        nl_shift_y = nonlinear_shift(points_y, points_y_orig[k])
+        points_y_shifted = points_y * nl_shift_y
+
+        mod_type = get_modulation_type_from_order(wdm['m_order'])
+        scale_constellation = get_scale_coef_constellation(mod_type) / np.sqrt(wdm['p_ave'] / wdm['n_polarisations'])
+
+        start_time = datetime.now()
+        points_x_found = get_nearest_constellation_points_unscaled(points_x_shifted, mod_type)
+        points_y_found = get_nearest_constellation_points_unscaled(points_y_shifted, mod_type)
+        print("search x and y points took",
+              (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
+
+        start_time = datetime.now()
+        ber_x = get_ber_by_points(points_x_orig[k] * scale_constellation, points_x_found, mod_type)
+        ber_y = get_ber_by_points(points_y_orig[k] * scale_constellation, points_y_found, mod_type)
+        print("ber for x and y took",
+              (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
+
+        q_x = np.sqrt(2) * sp.special.erfcinv(2 * ber_x[0])
+        q_y = np.sqrt(2) * sp.special.erfcinv(2 * ber_y[0])
+
+        evm_x = get_evm(points_x_orig[k] * scale_constellation, points_x_shifted[k] * scale_constellation)
+        evm_y = get_evm(points_y_orig[k] * scale_constellation, points_y_shifted[k] * scale_constellation)
+
+        print("BER (x / y):", ber_x, ber_y) if verbose >= 1 else ...
+        print(r'Q^2-factor (x / y):', q_x, q_y) if verbose >= 1 else ...
+
+    else:
+        print('Error[full_line_model_wdm]: no such type of channels_type variable')
+
+
+    if optimise == 'not':
+
+        result = {
+            'points_x': points_x,
+            'points_x_orig': points_x_orig,
+            'points_x_shifted': points_x_shifted,
+            'points_x_found': points_x_found,
+            'points_y': points_y,
+            'points_y_orig': points_y_orig,
+            'points_y_shifted': points_y_shifted,
+            'points_y_found': points_y_found,
+            'ber_x': ber_x,
+            'ber_y': ber_y,
+            'q_x': q_x,
+            'q_y': q_y,
+            'evm_x': evm_x,
+            'evm_y': evm_y
+        }
+
+    elif optimise == 'ber_x':
+        return ber_x
+    elif optimise == 'ber_y':
+        return ber_y
+    elif optimise == 'evm_x':
+        return evm_x
+    elif optimise == 'evm_y':
+        return evm_y
+    else:
+        print('Error[full_line_model_wdm]: no such type of optimise variable')
+        return None
+
     return result
```

### Comparing `hpcom-0.1.7/hpcom/hpcom_old.py` & `hpcom-0.1.8/hpcom/hpcom_old.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/hpcom/metrics.py` & `hpcom-0.1.8/hpcom/metrics.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/hpcom/modulation.py` & `hpcom-0.1.8/hpcom/modulation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/hpcom/signal.py` & `hpcom-0.1.8/hpcom/signal.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/hpcom.egg-info/PKG-INFO` & `hpcom-0.1.8/hpcom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcom
-Version: 0.1.7
+Version: 0.1.8
 Summary: High performance optical communication library
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpcom-0.1.7/pyproject.toml` & `hpcom-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hpcom"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Egor Sedov", email="e.sedov@g.nsu.ru" },
 ]
 description = "High performance optical communication library"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hpcom-0.1.7/tests/test_back_to_back.py` & `hpcom-0.1.8/tests/test_back_to_back.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/tests/test_channel_model.py` & `hpcom-0.1.8/tests/test_channel_model.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/tests/test_generation.py` & `hpcom-0.1.8/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/tests/test_ofdm_generation.py` & `hpcom-0.1.8/tests/test_ofdm_generation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.7/tests/test_propagation.py` & `hpcom-0.1.8/tests/test_propagation.py`

 * *Files identical despite different names*

