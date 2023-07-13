# Comparing `tmp/fsrs4anki_optimizer-4.0.0.tar.gz` & `tmp/fsrs4anki_optimizer-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.0.0.tar", last modified: Thu Jul 13 07:55:59 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.0.1.tar", last modified: Thu Jul 13 16:01:56 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.0.0.tar` & `fsrs4anki_optimizer-4.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49386 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49531 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/setup.py
```

### Comparing `fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,14 @@
                 (df['id'] <= time.time() * 1000)].copy()
         
         df_set_due_date = df[(df['type'] == 4) & (df['ivl'] > 0)]
         df.drop(df_set_due_date.index, inplace=True)
 
         df['create_date'] = pd.to_datetime(df['cid'] // 1000, unit='s')
         df['create_date'] = df['create_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
-        df.drop(df[df['create_date'].dt.year < 2006].index, inplace=True)
         df['review_date'] = pd.to_datetime(df['id'] // 1000, unit='s')
         df['review_date'] = df['review_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
         df.drop(df[df['review_date'].dt.year < 2006].index, inplace=True)
         df.sort_values(by=['cid', 'id'], inplace=True, ignore_index=True)
 
         df['is_learn_start'] = (df['type'] == 0) & (df['type'].shift() != 0)
         df['sequence_group'] = df['is_learn_start'].cumsum()
@@ -484,14 +483,15 @@
             group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
             if group.empty:
                 continue
             delta_t = group['delta_t']
             recall = group['y']['mean']
             count = group['y']['count']
             if sum(count) < 100:
+                print(f'Not enough data for first rating {first_rating}. Expected at least 100, got {sum(count)}.')
                 continue
             params, covs = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (3650)))
             rating_stability[int(first_rating)] = params[0]
             rating_count[int(first_rating)] = sum(count)
             print('Weighted fit parameters:', params)
             print('Number of reviews:', sum(count))
             predict_recall = power_forgetting_curve(delta_t, *params)
@@ -507,19 +507,21 @@
             plt.xlim(0, 30)
             plt.xlabel('Interval')
             plt.ylabel('Recall')
             plt.title('Forgetting curve for first rating ' + first_rating)
             plt.show()
 
         print(rating_stability)
+        if len(rating_stability) < 2:
+            raise Exception("Not enough data for pretraining!")
 
         def S0_rating_curve(rating, a, b, c):
             return np.exp(a + b * rating) + c
 
-        params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, 0), (15, 7, 30)))
+        params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, -5), (15, 7, 30)))
         print('Weighted fit parameters:', params)
         predict_stability = S0_rating_curve(np.array(list(rating_stability.keys())), *params)
         print("Fit stability:", predict_stability)
         print(f'RMSE: {mean_squared_error(list(rating_stability.values()), predict_stability, sample_weight=list(rating_count.values()), squared=False):.4f}')
         plt.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
         plt.plot(list(rating_stability.keys()), predict_stability, label='Weighted fit')
         plt.legend(loc='upper right', fancybox=True, shadow=False)
```

