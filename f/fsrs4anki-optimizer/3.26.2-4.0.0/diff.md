# Comparing `tmp/fsrs4anki_optimizer-3.26.2.tar.gz` & `tmp/fsrs4anki_optimizer-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.26.2.tar", last modified: Mon Jul 10 11:35:13 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.0.0.tar", last modified: Thu Jul 13 07:55:59 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.26.2.tar` & `fsrs4anki_optimizer-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45685 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 11:35:13.000000 fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 11:35:13.618971 fsrs4anki_optimizer-3.26.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 11:35:03.000000 fsrs4anki_optimizer-3.26.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49386 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 07:55:59.000000 fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:55:59.283603 fsrs4anki_optimizer-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 07:55:49.000000 fsrs4anki_optimizer-4.0.0/setup.py
```

### Comparing `fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.26.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.0.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,82 @@
 import zipfile
 import sqlite3
 import time
 import pandas as pd
 import numpy as np
 import os
 import math
-from typing import List, Optional
+from typing import List, Optional, Dict
 from datetime import timedelta, datetime
 import statsmodels.api as sm
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import torch
 from torch import nn
 from torch import Tensor
 from torch.utils.data import Dataset, DataLoader, Sampler
 from torch.nn.utils.rnn import pad_sequence, pack_padded_sequence, pad_packed_sequence
 from sklearn.model_selection import StratifiedGroupKFold
 from sklearn.metrics import mean_squared_error, r2_score
+from scipy.optimize import curve_fit
 from itertools import accumulate
 from tqdm.auto import tqdm
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 
+def power_forgetting_curve(t, s):
+    return (1 + t / (9 * s)) ** -1
+
+def next_interval(s, r):
+    return np.maximum(1, np.round(9 * s * (1/r - 1)))
+
 class FSRS(nn.Module):
     def __init__(self, w: List[float]):
         super(FSRS, self).__init__()
         self.w = nn.Parameter(torch.tensor(w, dtype=torch.float32))
 
-    def stability_after_success(self, state: Tensor, new_d: Tensor, r: Tensor) -> Tensor:
-        new_s = state[:,0] * (1 + torch.exp(self.w[6]) *
+    def stability_after_success(self, state: Tensor, new_d: Tensor, r: Tensor, rating: Tensor) -> Tensor:
+        hard_penalty = torch.where(rating == 2, self.w[15], 1)
+        easy_bonus = torch.where(rating == 4, self.w[16], 1)
+        new_s = state[:,0] * (1 + torch.exp(self.w[8]) *
                         (11 - new_d) *
-                        torch.pow(state[:,0], self.w[7]) *
-                        (torch.exp((1 - r) * self.w[8]) - 1))
+                        torch.pow(state[:,0], -self.w[9]) *
+                        (torch.exp((1 - r) * self.w[10]) - 1) * 
+                        hard_penalty * 
+                        easy_bonus)
         return new_s
 
     def stability_after_failure(self, state: Tensor, new_d: Tensor, r: Tensor) -> Tensor:
-        new_s = self.w[9] * torch.pow(new_d, self.w[10]) * torch.pow(
-            state[:,0], self.w[11]) * torch.exp((1 - r) * self.w[12])
-        return new_s.clamp(max=state[:,0])
+        new_s = self.w[11] * \
+                torch.pow(new_d, -self.w[12]) * \
+                (torch.pow(state[:,0] + 1, self.w[13]) - 1) * \
+                torch.exp((1 - r) * self.w[14])
+        return new_s
 
     def step(self, X: Tensor, state: Tensor) -> Tensor:
         '''
         :param X: shape[batch_size, 2], X[:,0] is elapsed time, X[:,1] is rating
         :param state: shape[batch_size, 2], state[:,0] is stability, state[:,1] is difficulty
         :return state:
         '''
         if torch.equal(state, torch.zeros_like(state)):
+            keys = torch.tensor([1, 2, 3, 4])
+            keys = keys.view(1, -1).expand(X[:,1].long().size(0), -1)
+            index = (X[:,1].long().unsqueeze(1) == keys).nonzero(as_tuple=True)
             # first learn, init memory states
-            new_s = self.w[0] + self.w[1] * (X[:,1] - 1)
-            new_d = self.w[2] + self.w[3] * (X[:,1] - 3)
+            new_s = self.w[index[1]]
+            new_d = self.w[4] - self.w[5] * (X[:,1] - 3)
             new_d = new_d.clamp(1, 10)
         else:
-            r = torch.exp(np.log(0.9) * X[:,0] / state[:,0])
-            new_d = state[:,1] + self.w[4] * (X[:,1] - 3)
-            new_d = self.mean_reversion(self.w[2], new_d)
+            r = power_forgetting_curve(X[:,0], state[:,0])
+            new_d = state[:,1] - self.w[6] * (X[:,1] - 3)
+            new_d = self.mean_reversion(self.w[4], new_d)
             new_d = new_d.clamp(1, 10)
             condition = X[:,1] > 1
-            new_s = torch.where(condition, self.stability_after_success(state, new_d, r), self.stability_after_failure(state, new_d, r))
+            new_s = torch.where(condition, self.stability_after_success(state, new_d, r, X[:,1]), self.stability_after_failure(state, new_d, r))
         new_s = new_s.clamp(0.1, 36500)
         return torch.stack([new_s, new_d], dim=1)
 
     def forward(self, inputs: Tensor, state: Optional[Tensor]=None) -> Tensor:
         '''
         :param inputs: shape[seq_len, batch_size, 2]
         '''
@@ -69,36 +85,36 @@
         outputs = []
         for X in inputs:
             state = self.step(X, state)
             outputs.append(state)
         return torch.stack(outputs), state
 
     def mean_reversion(self, init: Tensor, current: Tensor) -> Tensor:
-        return self.w[5] * init + (1-self.w[5]) * current
+        return self.w[7] * init + (1-self.w[7]) * current
 
 class WeightClipper:
     def __init__(self, frequency: int=1):
         self.frequency = frequency
 
     def __call__(self, module):
         if hasattr(module, 'w'):
             w = module.w.data
-            w[0] = w[0].clamp(0.1, 10)
-            w[1] = w[1].clamp(0.1, 5)
-            w[2] = w[2].clamp(1, 10)
-            w[3] = w[3].clamp(-5, -0.1)
-            w[4] = w[4].clamp(-5, -0.1)
-            w[5] = w[5].clamp(0.05, 0.5)
-            w[6] = w[6].clamp(0, 2)
-            w[7] = w[7].clamp(-0.8, -0.15)
-            w[8] = w[8].clamp(0.01, 1.5)
-            w[9] = w[9].clamp(0.5, 5)
-            w[10] = w[10].clamp(-2, -0.01)
-            w[11] = w[11].clamp(0.01, 0.9)
-            w[12] = w[12].clamp(0.01, 2)
+            w[4] = w[4].clamp(1, 10)
+            w[5] = w[5].clamp(0.1, 5)
+            w[6] = w[6].clamp(0.1, 5)
+            w[7] = w[7].clamp(0, 0.5)
+            w[8] = w[8].clamp(0, 2)
+            w[9] = w[9].clamp(0.1, 0.8)
+            w[10] = w[10].clamp(0.01, 1.5)
+            w[11] = w[11].clamp(0.5, 5)
+            w[12] = w[12].clamp(0.01, 0.2)
+            w[13] = w[13].clamp(0.01, 0.9)
+            w[14] = w[14].clamp(0.01, 2)
+            w[15] = w[15].clamp(0, 1)
+            w[16] = w[16].clamp(1, 10)
             module.w.data = w
 
 def lineToTensor(line: str) -> Tensor:
     ivl = line[0].split(',')
     response = line[1].split(',')
     tensor = torch.zeros(len(response), 2)
     for li, response in enumerate(response):
@@ -169,15 +185,15 @@
         self.batch_size = batch_size
         self.build_dataset(train_set, test_set)
         self.n_epoch = n_epoch
         self.batch_nums = self.next_train_data_loader.batch_sampler.batch_nums
         self.scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(self.optimizer, T_max=self.batch_nums * n_epoch)
         self.avg_train_losses = []
         self.avg_eval_losses = []
-        self.loss_fn = nn.BCELoss(reduction='sum')
+        self.loss_fn = nn.BCELoss(reduction='none')
 
     def build_dataset(self, train_set: pd.DataFrame, test_set: pd.DataFrame):
         pre_train_set = train_set[train_set['i'] == 2]
         self.pre_train_set = RevlogDataset(pre_train_set)
         sampler = RevlogSampler(self.pre_train_set, batch_size=self.batch_size)
         self.pre_train_data_loader = DataLoader(self.pre_train_set, batch_sampler=sampler, collate_fn=collate_fn)
 
@@ -192,41 +208,15 @@
 
         self.test_set = RevlogDataset(test_set)
         sampler = RevlogSampler(self.test_set, batch_size=self.batch_size)
         self.test_data_loader = DataLoader(self.test_set, batch_sampler=sampler, collate_fn=collate_fn)
         print("dataset built")
 
     def train(self, verbose: bool=True):
-        # pretrain
         best_loss = np.inf
-        weighted_loss, w = self.eval()
-        if weighted_loss < best_loss:
-            best_loss = weighted_loss
-            best_w = w
-
-        pbar = tqdm(desc="pre-train", colour="red", total=len(self.pre_train_data_loader) * self.n_epoch)
-        for k in range(self.n_epoch):
-            for i, batch in enumerate(self.pre_train_data_loader):
-                self.model.train()
-                self.optimizer.zero_grad()
-                sequences, delta_ts, labels, seq_lens = batch
-                real_batch_size = seq_lens.shape[0]
-                outputs, _ = self.model(sequences)
-                stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
-                retentions = torch.exp(np.log(0.9) * delta_ts / stabilities)
-                loss = self.loss_fn(retentions, labels)
-                loss.backward()
-                self.optimizer.step()
-                self.model.apply(self.clipper)
-                pbar.update(n=real_batch_size)
-
-        pbar.close()
-        for name, param in self.model.named_parameters():
-            tqdm.write(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
-
         epoch_len = len(self.next_train_data_loader)
         pbar = tqdm(desc="train", colour="red", total=epoch_len*self.n_epoch)
         print_len = max(self.batch_nums*self.n_epoch // 10, 1)
         for k in range(self.n_epoch):
             weighted_loss, w = self.eval()
             if weighted_loss < best_loss:
                 best_loss = weighted_loss
@@ -235,19 +225,19 @@
             for i, batch in enumerate(self.next_train_data_loader):
                 self.model.train()
                 self.optimizer.zero_grad()
                 sequences, delta_ts, labels, seq_lens = batch
                 real_batch_size = seq_lens.shape[0]
                 outputs, _ = self.model(sequences)
                 stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
-                retentions = torch.exp(np.log(0.9) * delta_ts / stabilities)
-                loss = self.loss_fn(retentions, labels)
+                retentions = power_forgetting_curve(delta_ts, stabilities)
+                loss = self.loss_fn(retentions, labels).sum()
                 loss.backward()
                 for param in self.model.parameters():
-                    param.grad[:2] = torch.zeros(2)
+                    param.grad[:4] = torch.zeros(4)
                 self.optimizer.step()
                 self.scheduler.step()
                 self.model.apply(self.clipper)
                 pbar.update(real_batch_size)
 
                 if verbose and (k * self.batch_nums + i + 1) % print_len == 0:
                     tqdm.write(f"iteration: {k * epoch_len + (i + 1) * self.batch_size}")
@@ -265,25 +255,25 @@
     def eval(self):
         self.model.eval()
         with torch.no_grad():
             sequences, delta_ts, labels, seq_lens = self.train_set.x_train, self.train_set.t_train, self.train_set.y_train, self.train_set.seq_len
             real_batch_size = seq_lens.shape[0]
             outputs, _ = self.model(sequences.transpose(0, 1))
             stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
-            retentions = torch.exp(np.log(0.9) * delta_ts / stabilities)
-            tran_loss = self.loss_fn(retentions, labels)/len(self.train_set)
+            retentions = power_forgetting_curve(delta_ts, stabilities)
+            tran_loss = self.loss_fn(retentions, labels).mean()
             self.avg_train_losses.append(tran_loss)
             tqdm.write(f"Loss in trainset: {tran_loss:.4f}")
 
             sequences, delta_ts, labels, seq_lens = self.test_set.x_train, self.test_set.t_train, self.test_set.y_train, self.test_set.seq_len
             real_batch_size = seq_lens.shape[0]
             outputs, _ = self.model(sequences.transpose(0, 1))
             stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
-            retentions = torch.exp(np.log(0.9) * delta_ts / stabilities)
-            test_loss = self.loss_fn(retentions, labels)/len(self.test_set)
+            retentions = power_forgetting_curve(delta_ts, stabilities)
+            test_loss = self.loss_fn(retentions, labels).mean()
             self.avg_eval_losses.append(test_loss)
             tqdm.write(f"Loss in testset: {test_loss:.4f}")
 
             w = list(map(lambda x: round(float(x), 4), dict(self.model.named_parameters())['w'].data))
 
             weighted_loss = (tran_loss * len(self.train_set) + test_loss * len(self.test_set)) / (len(self.train_set) + len(self.test_set))
 
@@ -345,31 +335,33 @@
         cur = con.cursor()
         res = cur.execute(f"""
         SELECT *
         FROM revlog
         WHERE cid IN (
             SELECT id
             FROM cards
-            {"WHERE queue != -1" if filter_out_suspended_cards else ""}
+            WHERE queue != 0
+            {"AND queue != -1" if filter_out_suspended_cards else ""}
         )
         """
         )
         revlog = res.fetchall()
         if len(revlog) == 0:
             raise Exception("No review log found!")
         df = pd.DataFrame(revlog)
-        df.columns = ['id', 'cid', 'usn', 'r', 'ivl', 'last_lvl', 'factor', 'time', 'type']
+        df.columns = ['id', 'cid', 'usn', 'r', 'ivl', 'last_ivl', 'factor', 'time', 'type']
         df = df[(df['cid'] <= time.time() * 1000) &
                 (df['id'] <= time.time() * 1000)].copy()
         
         df_set_due_date = df[(df['type'] == 4) & (df['ivl'] > 0)]
         df.drop(df_set_due_date.index, inplace=True)
 
         df['create_date'] = pd.to_datetime(df['cid'] // 1000, unit='s')
         df['create_date'] = df['create_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
+        df.drop(df[df['create_date'].dt.year < 2006].index, inplace=True)
         df['review_date'] = pd.to_datetime(df['id'] // 1000, unit='s')
         df['review_date'] = df['review_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
         df.drop(df[df['review_date'].dt.year < 2006].index, inplace=True)
         df.sort_values(by=['cid', 'id'], inplace=True, ignore_index=True)
 
         df['is_learn_start'] = (df['type'] == 0) & (df['type'].shift() != 0)
         df['sequence_group'] = df['is_learn_start'].cumsum()
@@ -409,19 +401,22 @@
         r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
         df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
         print("Trainset saved.")
 
+        S0_dataset = df[df['i'] == 2]
+        self.S0_dataset_group = S0_dataset.groupby(by=['r_history', 'delta_t'], group_keys=False).agg({'y': ['mean', 'count']}).reset_index()
+
         df['retention'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['y'].transform('mean')
         df['total_cnt'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['id'].transform('count')
         print("Retention calculated.")
 
-        df = df.drop(columns=['id', 'cid', 'usn', 'ivl', 'last_lvl', 'factor', 'time', 'type', 'create_date', 'review_date', 'real_days', 'r', 't_history', 'y'])
+        df = df.drop(columns=['id', 'cid', 'usn', 'ivl', 'last_ivl', 'factor', 'time', 'type', 'create_date', 'review_date', 'real_days', 'r', 't_history', 'y'])
         df.drop_duplicates(inplace=True)
         df['retention'] = df['retention'].map(lambda x: max(min(0.99, x), 0.01))
 
         def cal_stability(group: pd.DataFrame) -> pd.DataFrame:
             group_cnt = sum(group['total_cnt'])
             if group_cnt < 10:
                 return pd.DataFrame()
@@ -458,15 +453,15 @@
             print("Analysis saved!")
             caption = "1:again, 2:hard, 3:good, 4:easy\n"
             analysis = df[df['r_history'].str.contains(r'^[1-4][^124]*$', regex=True)][['r_history', 'avg_interval', 'avg_retention', 'stability', 'factor', 'group_cnt']].to_string(index=False)
             return caption + analysis
 
     def define_model(self):
         """Step 3"""
-        self.init_w = [1, 1, 5, -0.5, -0.5, 0.2, 1.4, -0.2, 0.8, 2, -0.2, 0.2, 1]
+        self.init_w = [1, 2, 3, 4, 5, 0.5, 0.5, 0.2, 1.4, 0.2, 0.8, 2, 0.2, 0.2, 1, 0.5, 2]
         '''
         w[0]: initial_stability_for_again_answer
         w[1]: initial_stability_step_per_rating
         w[2]: initial_difficulty_for_good_answer
         w[3]: initial_difficulty_step_per_rating
         w[4]: next_difficulty_step_per_rating
         w[5]: next_difficulty_reversion_to_mean_speed (used to avoid ease hell)
@@ -477,28 +472,101 @@
         w[10]: next_stability_difficulty_decay_after_success
         w[11]: next_stability_stability_gain_after_failure
         w[12]: next_stability_retrievability_gain_after_failure
         For more details about the parameters, please see: 
         https://github.com/open-spaced-repetition/fsrs4anki/wiki/Free-Spaced-Repetition-Scheduler
         '''
 
-    def train(self, lr: float = 4e-2, n_epoch: int = 3, n_splits: int = 3, batch_size: int = 512, verbose: bool = True):
+    def pretrain(self):
+        rating_stability = {}
+        rating_count = {}
+
+        for first_rating in ("1", "2", "3", "4"):
+            group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
+            if group.empty:
+                continue
+            delta_t = group['delta_t']
+            recall = group['y']['mean']
+            count = group['y']['count']
+            if sum(count) < 100:
+                continue
+            params, covs = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (3650)))
+            rating_stability[int(first_rating)] = params[0]
+            rating_count[int(first_rating)] = sum(count)
+            print('Weighted fit parameters:', params)
+            print('Number of reviews:', sum(count))
+            predict_recall = power_forgetting_curve(delta_t, *params)
+            print(f'RMSE: {mean_squared_error(recall, predict_recall, sample_weight=count, squared=False):.4f}')
+
+            plt.plot(delta_t, recall, label='Exact')
+            plt.plot(np.linspace(0, 30), power_forgetting_curve(np.linspace(0, 30), *params), label='Weighted fit')
+            count_percent = np.array([x/sum(count) for x in count])
+            plt.scatter(delta_t, recall, s=count_percent * 1000, alpha=0.5)
+            plt.legend(loc='upper right', fancybox=True, shadow=False)
+            plt.grid(True)
+            plt.ylim(0, 1)
+            plt.xlim(0, 30)
+            plt.xlabel('Interval')
+            plt.ylabel('Recall')
+            plt.title('Forgetting curve for first rating ' + first_rating)
+            plt.show()
+
+        print(rating_stability)
+
+        def S0_rating_curve(rating, a, b, c):
+            return np.exp(a + b * rating) + c
+
+        params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, 0), (15, 7, 30)))
+        print('Weighted fit parameters:', params)
+        predict_stability = S0_rating_curve(np.array(list(rating_stability.keys())), *params)
+        print("Fit stability:", predict_stability)
+        print(f'RMSE: {mean_squared_error(list(rating_stability.values()), predict_stability, sample_weight=list(rating_count.values()), squared=False):.4f}')
+        plt.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
+        plt.plot(list(rating_stability.keys()), predict_stability, label='Weighted fit')
+        plt.legend(loc='upper right', fancybox=True, shadow=False)
+        plt.grid(True)
+        plt.xlabel('First rating')
+        plt.ylabel('Stability')
+        plt.title('Stability for first rating')
+        plt.show()
+
+        for rating in (1, 2, 3, 4):
+            again_extrap = max(min(S0_rating_curve(1, *params), 3650), 0.1)
+            # if there isn't enough data to calculate the value for "Again" exactly
+            if 1 not in rating_stability:
+                # then check if there exists an exact value for "Hard"
+                if 2 in rating_stability:
+                    # if it exists, then check whether the extrapolation breaks monotonicity
+                    # Again > Hard is possible, but we should allow it only for exact values, otherwise we should assume monotonicity
+                    if again_extrap > rating_stability[2]:
+                        # if it does, then replace the missing "Again" value with the exact "Hard" value
+                        rating_stability[1] = rating_stability[2]
+                    else:
+                        # if it doesn't break monotonicity, then use the extrapolated value
+                        rating_stability[1] = again_extrap
+                # if an exact value for "Hard" doesn't exist, then just use the extrapolation, there's nothing else we can do
+                else:
+                    rating_stability[1] = again_extrap
+            elif rating not in rating_stability:
+                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 3650), 0.1)
+
+        rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
+        for rating, stability in rating_stability.items():
+            self.init_w[rating-1] = stability
+        
+
+    def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
         """Step 4"""
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         if self.dataset.empty:
             raise ValueError('Training data is inadequate.')
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
         print("Tensorized!")
-        
-        n_pre_train_groups = len(self.dataset[self.dataset['i'] == 2]['group'].unique())
-        if n_pre_train_groups < n_splits:
-            print("Not enough groups for pre-training. Splitting into {} folds.".format(n_pre_train_groups))
-            n_splits = n_pre_train_groups
 
         w = []
         plots = []
         if n_splits > 1:
             sgkf = StratifiedGroupKFold(n_splits=n_splits)
             for train_index, test_index in sgkf.split(self.dataset, self.dataset['i'], self.dataset['group']):
                 print("TRAIN:", len(train_index), "TEST:",  len(test_index))
@@ -528,40 +596,34 @@
             d_history = "0"
             r_history = f"{first_rating}"  # the first rating of the new card
             # print("stability, difficulty, lapses")
             for i in range(10):
                 states = my_collection.predict(t_history, r_history)
                 # print('{0:9.2f} {1:11.2f} {2:7.0f}'.format(
                     # *list(map(lambda x: round(float(x), 4), states))))
-                next_t = max(round(float(np.log(requestRetention)/np.log(0.9) * states[0])), 1)
+                next_t = next_interval(states[0], requestRetention)                
                 difficulty = round(float(states[1]), 1)
                 t_history += f',{int(next_t)}'
                 d_history += f',{difficulty}'
                 r_history += f",3"
             preview_text += f"rating history: {r_history}\n"
             preview_text += "interval history: " + ",".join([f"{ivl}d" if ivl < 30 else f"{ivl / 30:.1f}m" if ivl < 365 else f"{ivl / 365:.1f}y" for ivl in map(int, t_history.split(','))]) + "\n"
             preview_text += f"difficulty history: {d_history}\n"
         return preview_text
 
-    def preview_sequence(self, test_rating_sequence: str, requestRetention: float, easyBonus: float, hardInterval: float):
+    def preview_sequence(self, test_rating_sequence: str, requestRetention: float):
         my_collection = Collection(self.w)
 
         t_history = "0"
         d_history = "0"
         for i in range(len(test_rating_sequence.split(','))):
-            rating = test_rating_sequence[2*i]
-            last_t = int(t_history.split(',')[-1])
             r_history = test_rating_sequence[:2*i+1]
             states = my_collection.predict(t_history, r_history)
             print(states)
-            next_t = max(1,round(float(np.log(requestRetention)/np.log(0.9) * states[0])))
-            if rating == '4':
-                next_t = round(next_t * easyBonus)
-            elif rating == '2':
-                next_t = round(last_t * hardInterval)
+            next_t = next_interval(states[0], requestRetention)
             t_history += f',{int(next_t)}'
             difficulty = round(float(states[1]), 1)
             d_history += f',{difficulty}'
         preview_text = f"rating history: {test_rating_sequence}\n"
         preview_text += f"interval history: {t_history}\n"
         preview_text += f"difficulty history: {d_history}"
         return preview_text
@@ -621,47 +683,44 @@
 
         print(f"average time for failed cards: {f_time}s")
         print(f"average time for recalled cards: {r_time}s")
 
         def stability2index(stability):
             return (np.log(stability) / np.log(base)).round().astype(int) + index_offset
 
-        def init_stability(d):
-            return max(((d - self.w[2]) / self.w[3] + 2) * self.w[1] + self.w[0], np.power(base, -index_offset))
-
         def cal_next_recall_stability(s, r, d, response):
             if response == 1:
-                return s * (1 + np.exp(self.w[6]) * (11 - d) * np.power(s, self.w[7]) * (np.exp((1 - r) * self.w[8]) - 1))
+                return s * (1 + np.exp(self.w[8]) * (11 - d) * np.power(s, -self.w[9]) * (np.exp((1 - r) * self.w[10]) - 1))
             else:
-                return np.minimum(self.w[9] * np.power(d, self.w[10]) * np.power(s, self.w[11]) * np.exp((1 - r) * self.w[12]), s)
+                return np.minimum(self.w[11] * np.power(d, -self.w[12]) * (np.power(s + 1, self.w[13]) - 1) * np.exp((1 - r) * self.w[14]), s)
 
         terminal_stability = minimum_stability
         for _ in range(128):
             terminal_stability = cal_next_recall_stability(terminal_stability, 0.96, d_range, 1)
         index_len = stability2index(terminal_stability)
         stability_list = np.array([np.power(base, i - index_offset) for i in range(index_len)])
         print(f"terminal stability: {stability_list.max(): .2f}")
         df = pd.DataFrame(columns=["retention", "difficulty", "time"])
 
         for percentage in tqdm(range(96, 66, -2), desc="find optimal retention"):
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
             time_list[:,:-1] = max_time
             for d in range(d_range, 0, -1):
-                s0 = init_stability(d)
+                s0 = 1
                 s0_index = stability2index(s0)
                 diff = max_time
                 iteration = 0
                 while diff > 1 and iteration < 2e5:
                     iteration += 1
                     total_time = time_list[d - 1].sum()
                     s_indices = np.arange(index_len - 2, -1, -1)
                     stabilities = stability_list[s_indices]
-                    intervals = np.maximum(1, np.round(stabilities * np.log(recall) / np.log(0.9)))
-                    p_recalls = np.power(0.9, intervals / stabilities)
+                    intervals = next_interval(stabilities, recall)
+                    p_recalls = power_forgetting_curve(intervals, stabilities)
                     recall_s = cal_next_recall_stability(stabilities, p_recalls, d, 1)
                     forget_d = np.minimum(d + d_offset, 10)
                     forget_s = cal_next_recall_stability(stabilities, p_recalls, forget_d, 0)
                     recall_s_indices = np.minimum(stability2index(recall_s), index_len - 1)
                     forget_s_indices = np.clip(stability2index(forget_s), 0, index_len - 1)
                     recall_times = time_list[d - 1][recall_s_indices] + r_time
                     forget_times = time_list[forget_d - 1][forget_s_indices] + f_time
@@ -698,44 +757,49 @@
         return (fig, )
     
     def evaluate(self):
         my_collection = Collection(self.init_w)
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         self.dataset['stability'] = stabilities
         self.dataset['difficulty'] = difficulties
-        self.dataset['p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['stability'])
+        self.dataset['p'] = power_forgetting_curve(self.dataset['delta_t'], self.dataset['stability'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['p']) if row['y'] == 1 else - np.log(1 - row['p']), axis=1)
         loss_before = self.dataset['log_loss'].mean()
 
         my_collection = Collection(self.w)
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         self.dataset['stability'] = stabilities
         self.dataset['difficulty'] = difficulties
-        self.dataset['p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['stability'])
+        self.dataset['p'] = power_forgetting_curve(self.dataset['delta_t'], self.dataset['stability'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['p']) if row['y'] == 1 else - np.log(1 - row['p']), axis=1)
         loss_after = self.dataset['log_loss'].mean()
 
         tmp = self.dataset.copy()
         tmp['stability'] = tmp['stability'].map(lambda x: round(x, 2))
         tmp['difficulty'] = tmp['difficulty'].map(lambda x: round(x, 2))
         tmp['p'] = tmp['p'].map(lambda x: round(x, 2))
         tmp['log_loss'] = tmp['log_loss'].map(lambda x: round(x, 2))
         tmp.rename(columns={"r": "grade", "p": "retrievability"}, inplace=True)
         tmp[['id', 'cid', 'review_date', 'r_history', 't_history', 'delta_t', 'grade', 'stability', 'difficulty', 'retrievability', 'log_loss']].to_csv("./evaluation.tsv", sep='\t', index=False)
         del tmp
         return loss_before, loss_after
 
     def calibration_graph(self):
-        fig1 = plot_brier(self.dataset['p'], self.dataset['y'], bins=40)
+        fig1 = plt.figure()
+        plot_brier(self.dataset['p'], self.dataset['y'], bins=40, ax=fig1.add_subplot(111))
+        fig2 = plt.figure(figsize=(16, 12))
+        for last_rating in ("1","2","3","4"):
+            print(f"\nLast rating: {last_rating}")
+            plot_brier(self.dataset[self.dataset['r_history'].str.endswith(last_rating)]['p'], self.dataset[self.dataset['r_history'].str.endswith(last_rating)]['y'], bins=40, ax=fig2.add_subplot(2, 2, int(last_rating)), title=f"Last rating: {last_rating}")
 
         def to_percent(temp, position):
             return '%1.0f' % (100 * temp) + '%'
 
-        fig2 = plt.figure()
-        ax1 = fig2.add_subplot(111)
+        fig3 = plt.figure()
+        ax1 = fig3.add_subplot(111)
         ax2 = ax1.twinx()
         lns = []
 
         stability_calibration = pd.DataFrame(columns=['stability', 'predicted_retention', 'actual_retention'])
         stability_calibration = self.dataset[['stability', 'p', 'y']].copy()
         stability_calibration['bin'] = stability_calibration['stability'].map(lambda x: math.pow(1.2, math.floor(math.log(x, 1.2))))
         stability_group = stability_calibration.groupby('bin').count()
@@ -757,16 +821,16 @@
 
         labs = [l.get_label() for l in lns]
         ax2.legend(lns, labs, loc='lower right')
         ax2.grid(linestyle='--')
         ax2.yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
         ax2.xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
 
-        fig3 = plt.figure()
-        ax1 = fig3.add_subplot(111)
+        fig4 = plt.figure()
+        ax1 = fig4.add_subplot(111)
         ax2 = ax1.twinx()
         lns = []
 
         difficulty_calibration = pd.DataFrame(columns=['difficulty', 'predicted_retention', 'actual_retention'])
         difficulty_calibration = self.dataset[['difficulty', 'p', 'y']].copy()
         difficulty_calibration['bin'] = difficulty_calibration['difficulty'].map(round)
         difficulty_group = difficulty_calibration.groupby('bin').count()
@@ -787,15 +851,15 @@
 
         labs = [l.get_label() for l in lns]
         ax2.legend(lns, labs, loc='lower right')
         ax2.grid(linestyle='--')
         ax2.yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
         ax2.xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
 
-        return fig1, fig2, fig3
+        return fig1, fig2, fig3, fig4
 
     def bw_matrix(self):
         B_W_Metric_raw = self.dataset[['difficulty', 'stability', 'p', 'y']].copy()
         B_W_Metric_raw['s_bin'] = B_W_Metric_raw['stability'].map(lambda x: round(math.pow(1.4, math.floor(math.log(x, 1.4))), 2))
         B_W_Metric_raw['d_bin'] = B_W_Metric_raw['difficulty'].map(lambda x: int(round(x)))
         B_W_Metric = B_W_Metric_raw.groupby(by=['s_bin', 'd_bin']).agg('mean').reset_index()
         B_W_Metric_count = B_W_Metric_raw.groupby(by=['s_bin', 'd_bin']).agg('count').reset_index()
@@ -807,15 +871,16 @@
 
     def compare_with_sm2(self):
         self.dataset['sm2_ivl'] = self.dataset['tensor'].map(sm2)
         self.dataset['sm2_p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['sm2_ivl'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['sm2_p']) if row['y'] == 1 else - np.log(1 - row['sm2_p']), axis=1)
         print(f"Loss of SM-2: {self.dataset['log_loss'].mean():.4f}")
         cross_comparison = self.dataset[['sm2_p', 'p', 'y']].copy()
-        fig1 = plot_brier(cross_comparison['sm2_p'], cross_comparison['y'], bins=40)
+        fig1 = plt.figure()
+        plot_brier(cross_comparison['sm2_p'], cross_comparison['y'], bins=40, ax=fig1.add_subplot(111))
 
         fig2 = plt.figure(figsize=(6, 6))
         ax = fig2.gca()
 
         cross_comparison['SM2_B-W'] = cross_comparison['sm2_p'] - cross_comparison['y']
         cross_comparison['SM2_bin'] = cross_comparison['sm2_p'].map(lambda x: round(x, 1))
         cross_comparison['FSRS_B-W'] = cross_comparison['p'] - cross_comparison['y']
@@ -869,45 +934,44 @@
             "bin_count": bins,
             "bin_counts": list(counts),
             "bin_prediction_means": list(prediction_means),
             "bin_correct_means": list(correct_means),
         }
     }
 
-def plot_brier(predictions, real, bins=20):
+def plot_brier(predictions, real, bins=20, ax=None, title=None):
     brier = load_brier(predictions, real, bins=bins)
     bin_prediction_means = brier['detail']['bin_prediction_means']
     bin_correct_means = brier['detail']['bin_correct_means']
     bin_counts = brier['detail']['bin_counts']
     r2 = r2_score(bin_correct_means, bin_prediction_means, sample_weight=bin_counts)
     rmse = np.sqrt(mean_squared_error(bin_correct_means, bin_prediction_means, sample_weight=bin_counts))
     print(f"R-squared: {r2:.4f}")
     print(f"RMSE: {rmse:.4f}")
-    fig = plt.figure()
-    ax1 = fig.add_subplot(111)
-    ax1.set_xlim([0, 1])
-    ax1.set_ylim([0, 1])
-    ax1.grid(True)
+    ax.set_xlim([0, 1])
+    ax.set_ylim([0, 1])
+    ax.grid(True)
     fit_wls = sm.WLS(bin_correct_means, sm.add_constant(bin_prediction_means), weights=bin_counts).fit()
     print(fit_wls.params)
     y_regression = [fit_wls.params[0] + fit_wls.params[1]*x for x in bin_prediction_means]
-    ax1.plot(bin_prediction_means, y_regression, label='Weighted Least Squares Regression', color="green")
-    ax1.plot(bin_prediction_means, bin_correct_means, label='Actual Calibration', color="#1f77b4")
-    ax1.plot((0, 1), (0, 1), label='Perfect Calibration', color="#ff7f0e")
+    ax.plot(bin_prediction_means, y_regression, label='Weighted Least Squares Regression', color="green")
+    ax.plot(bin_prediction_means, bin_correct_means, label='Actual Calibration', color="#1f77b4")
+    ax.plot((0, 1), (0, 1), label='Perfect Calibration', color="#ff7f0e")
     bin_count = brier['detail']['bin_count']
     counts = np.array(bin_counts)
     bins = (np.arange(bin_count) + 0.5) / bin_count
-    ax1.legend(loc='upper center')
-    ax1.set_xlabel('Predicted R')
-    ax1.set_ylabel('Actual R')
-    ax2 = ax1.twinx()
+    ax.legend(loc='upper center')
+    ax.set_xlabel('Predicted R')
+    ax.set_ylabel('Actual R')
+    ax2 = ax.twinx()
     ax2.set_ylabel('Number of reviews')
     ax2.bar(bins, counts, width=(0.8 / bin_count), ec='k', lw=.2, alpha=0.5, label='Number of reviews')
     ax2.legend(loc='lower center')
-    return fig
+    if title:
+        ax.set_title(title)
 
 def sm2(history):
     ivl = 0
     ef = 2.5
     reps = 0
     for delta_t, rating in history:
         delta_t = delta_t.item()
```

