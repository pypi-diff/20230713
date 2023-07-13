# Comparing `tmp/iv_tools-0.0.1.tar.gz` & `tmp/iv_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iv_tools-0.0.1.tar", last modified: Wed Jul 12 15:37:33 2023, max compression
+gzip compressed data, was "iv_tools-0.0.2.tar", last modified: Thu Jul 13 08:51:24 2023, max compression
```

## Comparing `iv_tools-0.0.1.tar` & `iv_tools-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:37:33.257307 iv_tools-0.0.1/
--rw-rw-rw-   0        0        0      506 2023-07-12 15:37:33.256311 iv_tools-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 15:37:33.243343 iv_tools-0.0.1/iv_tools/
--rw-rw-rw-   0        0        0      116 2023-07-12 14:35:18.000000 iv_tools-0.0.1/iv_tools/__init__.py
--rw-rw-rw-   0        0        0    18078 2023-07-12 14:11:55.000000 iv_tools-0.0.1/iv_tools/iv_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:37:33.255319 iv_tools-0.0.1/iv_tools.egg-info/
--rw-rw-rw-   0        0        0      506 2023-07-12 15:37:33.000000 iv_tools-0.0.1/iv_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-12 15:37:33.000000 iv_tools-0.0.1/iv_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:37:33.000000 iv_tools-0.0.1/iv_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 15:37:33.000000 iv_tools-0.0.1/iv_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:37:33.257307 iv_tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-12 15:35:24.000000 iv_tools-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:51:24.836063 iv_tools-0.0.2/
+-rw-rw-rw-   0        0        0      511 2023-07-13 08:51:24.835066 iv_tools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-07-13 08:22:18.000000 iv_tools-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 08:51:24.825093 iv_tools-0.0.2/iv_tools/
+-rw-rw-rw-   0        0        0      116 2023-07-12 14:35:18.000000 iv_tools-0.0.2/iv_tools/__init__.py
+-rw-rw-rw-   0        0        0    20652 2023-07-13 08:17:54.000000 iv_tools-0.0.2/iv_tools/iv_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:51:24.834070 iv_tools-0.0.2/iv_tools.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 08:51:24.000000 iv_tools-0.0.2/iv_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 08:51:24.836063 iv_tools-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-13 08:51:13.000000 iv_tools-0.0.2/setup.py
```

### Comparing `iv_tools-0.0.1/iv_tools/iv_tools.py` & `iv_tools-0.0.2/iv_tools/iv_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,45 @@
 """
 Created on Wed Jul 12 07:47:19 2023
 
 @author: varun
 """
 
 """
-def iv_solver(index = True, method = ['ensemble', 'straddle', 'put'], front_back = ['front', 'back'], next_contract_skip = 3, interpolate = False, interpolate_term = 0, index_opt = 'weekly')
 
 
 
 """
     
 import pandas as pd
 import numpy as np
 import datetime as dt
+from py_vollib.black_scholes import black_scholes as bs
+from py_vollib.black_scholes.greeks.analytical import vega, delta
 
-
+def implied_vol(S0, K, T, r, market_price, flag = 'c', tol = 0.00001):
+    
+    max_iter = 200 # max iterations
+    vol_old = 0.3 #initial guess
+    
+    for k in range(max_iter):
+        bs_price = bs(flag, S0, K, T, r, vol_old)
+        Cprime = vega(flag, S0, K, T, r, vol_old)*100
+        C = bs_price - market_price
+    
+        vol_new = vol_old - C/Cprime
+        new_bs_price = bs(flag, S0, K, T, r, vol_new)
+        
+        if (abs(vol_old-vol_new) < tol) or (abs(new_bs_price-market_price) < tol):
+            break
+        
+        vol_old = vol_new
+        
+    implied_vol = vol_new
+    return implied_vol         
 
 def straddle_iv_finder(straddle_price, spot, dte):
     """
     Returns implied volatility using the straddle approximation formula.
 
     Parameters
     ----------
@@ -37,14 +57,28 @@
         Returns annualized implied volatility
 
     """
     
     sigma = (1.25*straddle_price)/(spot*np.sqrt(dte/365))
     return sigma
 
+
+def find_synthetic_forward(symbol, opt_bhav, monthly_fut, expiry_date_str, dte):  
+    """
+    Identifies the strike with the greatest OI and uses put-call parity to find the implied forward
+    """
+    strike_diff = 50 if symbol == 'NIFTY' else 100
+    strike = int(round((monthly_fut+1)/strike_diff))*strike_diff
+    opt_bhav = opt_bhav[(opt_bhav['EXPIRY_DT'] == expiry_date_str)&(opt_bhav['STRIKE_PR'] == strike)]
+    ce_price = opt_bhav[opt_bhav['OPTION_TYP']=='CE']['SETTLE_PR'].iloc[0]
+    pe_price = opt_bhav[opt_bhav['OPTION_TYP']=='PE']['SETTLE_PR'].iloc[0]
+    tte_years = dte/365
+    forward = (np.exp(-(0.07)*tte_years)*strike) + ce_price - pe_price
+    return forward
+    
 def find_liquid_strike(opt_bhav, expiry_date_str, strike_series, initial_guess, straddle=True, opt_type = 'p'):
     opt_type = (opt_type+'e').upper()
    
     final_price = np.nan
     if straddle:
         initial_straddle = opt_bhav[(opt_bhav['STRIKE_PR']==initial_guess)&(opt_bhav['EXPIRY_DT']==expiry_date_str)]
         if ((initial_straddle[['OPEN','HIGH','LOW']]==0).sum().sum()<1)&((initial_straddle['CHG_IN_OI']==0).sum() == 0): # filter for illiquidity
@@ -100,54 +134,74 @@
 
     Returns
     -------
     iv : FLOAT
     
 
     """
-    
-    iv_near = iv_near/100
-    iv_far = iv_far/100
+
     tte_near = dte_near/365
     tte_far = dte_far/365
-    tte_thirty = term/365
+    tte_term = term/365
 
-    iv = 100*np.sqrt((((tte_near*(iv_near**2))*((tte_far - tte_thirty)/(tte_far - tte_near)))+((tte_far*(iv_far**2))*((tte_thirty - tte_near)/(tte_far - tte_near))))*(365/30))
+    iv = np.sqrt((((tte_near*(iv_near**2))*((tte_far - tte_term)/(tte_far - tte_near)))+((tte_far*(iv_far**2))*((tte_term - tte_near)/(tte_far - tte_near))))*(365/term))
     return iv
 
 
 
 
-def retrieve_iv(symbol, date, index = True, method = 'straddle', front_back = 'interpolate', next_contract_skip = 3, interpolate_term = 0):
+def retrieve_iv(symbol, date, index = True, method = 'straddle', front_back = 'interpolate', next_contract_skip = 1, interpolate_term = 5, index_opt = 'weekly'):
     call_put_dict = {'put': 'p', 'call': 'c'}
     final_iv = np.nan
     try:
         date_str  = date.strftime('%Y-%m-%d')
         bhav = pd.read_csv(rf'C:\Users\varun\Documents\Raw Data\Bhavcopies\Bhavcopy_fno_{date_str}.csv')
         bhav = bhav[bhav['SYMBOL']==symbol]
         
         if index:   # filtering depending on index or single stock   
             fut_bhav = bhav[bhav['INSTRUMENT']=='FUTIDX']
             opt_bhav = bhav[bhav['INSTRUMENT']=='OPTIDX']
+            
+            weekly_expiry_dates_str = pd.Series(opt_bhav['EXPIRY_DT'].unique()).sort_values()
+            weekly_expiry_dates= weekly_expiry_dates_str.apply(lambda x: dt.datetime.strptime(x, '%Y-%m-%d'))
+            monthly_expiry_dates_str = pd.Series(fut_bhav['EXPIRY_DT'].unique()).sort_values()
+            monthly_expiry_dates = monthly_expiry_dates_str.apply(lambda x: dt.datetime.strptime(x, '%Y-%m-%d'))
+            
         else:
             fut_bhav = bhav[bhav['INSTRUMENT']=='FUTSTK']
             opt_bhav = bhav[bhav['INSTRUMENT']=='OPTSTK']
                     
+
         front_fut = fut_bhav['SETTLE_PR'].iloc[0]
         back_fut = fut_bhav['SETTLE_PR'].iloc[1]
-                    
+        
+        
         front_expiry_date_str = fut_bhav['EXPIRY_DT'].iloc[0]
         front_expiry_date = dt.datetime.strptime(front_expiry_date_str, '%Y-%m-%d')
         back_expiry_date_str = fut_bhav['EXPIRY_DT'].iloc[1]
         back_expiry_date = dt.datetime.strptime(back_expiry_date_str, '%Y-%m-%d')
                             
         front_dte = (front_expiry_date - date).days
         back_dte = (back_expiry_date - date).days
         
+        # modifications for index options
         
+        if ((index) & (index_opt == 'weekly')):
+            front_expiry_date_str = weekly_expiry_dates_str.iloc[0]
+            front_expiry_date = weekly_expiry_dates.iloc[0]
+            back_expiry_date_str = weekly_expiry_dates_str.iloc[1]
+            back_expiry_date = weekly_expiry_dates.iloc[1]
+                                
+            front_dte = (front_expiry_date - date).days
+            back_dte = (back_expiry_date - date).days
+            
+            front_fut = find_synthetic_forward(symbol, opt_bhav, front_fut, front_expiry_date_str, front_dte)
+            back_fut = find_synthetic_forward(symbol, opt_bhav, front_fut, back_expiry_date_str, back_dte)
+                    
+                
         if front_back == 'front':
             if front_dte <= next_contract_skip: # This is rolling to the next contract
                 front_expiry_date_str = back_expiry_date_str
                 front_expiry_date = back_expiry_date
                 front_dte = back_dte
                 front_fut = back_fut
                 
@@ -160,36 +214,40 @@
                 front_month_straddle = find_liquid_strike(opt_bhav, front_expiry_date_str, front_strike_diff, front_closest_strike, straddle = True)
                 final_iv = straddle_iv_finder(front_month_straddle, front_fut, front_dte)
             elif method == 'put':
                 front_pe_price = find_liquid_strike(opt_bhav, front_expiry_date_str, front_strike_diff, front_closest_strike, straddle = False)
                 final_iv = implied_vol(front_fut, front_closest_strike, front_dte/365, 0.07, front_pe_price, 'p')
             elif method == 'call':
                 front_ce_price = find_liquid_strike(opt_bhav, front_expiry_date_str, front_strike_diff, front_closest_strike, straddle = False, opt_type = 'c')
-                final_iv = implied_vol(front_fut, front_closest_strike, front_dte/365, 0.07, front_pe_price, 'c')
+                final_iv = implied_vol(front_fut, front_closest_strike, front_dte/365, 0.07, front_ce_price, 'c')
         
             else:
                 front_month_straddle = find_liquid_strike(opt_bhav, front_expiry_date_str, front_strike_diff, front_closest_strike, straddle = True)
                 front_straddle_iv = straddle_iv_finder(front_month_straddle, front_fut, front_dte)
                 front_pe_price = find_liquid_strike(opt_bhav, front_expiry_date_str, front_strike_diff, front_closest_strike, straddle = False)
                 front_pe_iv = implied_vol(front_fut, front_closest_strike, front_dte/365, 0.07, front_pe_price, 'p')
                 front_ce_price = find_liquid_strike(opt_bhav, front_expiry_date_str, front_strike_diff, front_closest_strike, straddle = False, opt_type = 'c')
-                front_ce_iv = implied_vol(front_fut, front_closest_strike, front_dte/365, 0.07, front_pe_price, 'c')
+                front_ce_iv = implied_vol(front_fut, front_closest_strike, front_dte/365, 0.07, front_ce_price, 'c')
                 
                 final_iv = (front_ce_iv+ front_pe_iv + front_straddle_iv)/3
         
             
             return final_iv
        
         elif front_back == 'back':
             if back_dte <= next_contract_skip: # This is rolling to the next contract
                 back_expiry_date_str = fut_bhav['EXPIRY_DT'].iloc[2]
                 back_expiry_date = dt.datetime.strptime(back_expiry_date_str, '%Y-%m-%d')
                 back_dte = (back_expiry_date - date).days
                 back_fut = fut_bhav['SETTLE_PR'].iloc[2]
                 
+                if ((index) & (index_opt == 'weekly')):
+                    back_expiry_date_str = weekly_expiry_dates_str.iloc[2]
+                    back_expiry_date = weekly_expiry_dates.iloc[2]
+                
             strike_list = pd.Series(opt_bhav[opt_bhav['EXPIRY_DT']==back_expiry_date_str]['STRIKE_PR'].unique())
             back_strike_diff = abs(strike_list - back_fut) # finding the closest strikes to the forward
             back_strike_diff.index = strike_list
             back_closest_strike = back_strike_diff[back_strike_diff == back_strike_diff.min()].index[0]
             
             if method == 'straddle':
                 back_month_straddle = find_liquid_strike(opt_bhav, back_expiry_date_str, back_strike_diff, back_closest_strike, straddle = True)
@@ -311,9 +369,7 @@
                 
                 final_iv = (interpolated_straddle_iv + interpolated_call_iv + interpolated_put_iv)/3
                 
             return final_iv
     except Exception as e:
         return final_iv
         print(f'error {e} for {date} for {symbol}')
-
-retrieve_iv('RELIANCE', dt.datetime(2023,7,10), False, front_back = 'back', method = 'put')
```

### Comparing `iv_tools-0.0.1/setup.py` & `iv_tools-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 @author: varun
 """
 
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
-DESCRIPTION = 'FFF'
-LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
+VERSION = '0.0.2'
+DESCRIPTION = 'IV Tools'
+LONG_DESCRIPTION = 'Implied Volatility Tools'
 
 # Setting up
 setup(
     name="iv_tools",
     version=VERSION,
     author="varun",
     author_email="varunsrikanth91@gmail.com",
```

