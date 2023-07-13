# Comparing `tmp/tej-tool-api-1.0.2.tar.gz` & `tmp/tej-tool-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tej-tool-api-1.0.2.tar", last modified: Mon Jul 10 09:24:30 2023, max compression
+gzip compressed data, was "tej-tool-api-1.0.3.tar", last modified: Thu Jul 13 09:35:58 2023, max compression
```

## Comparing `tej-tool-api-1.0.2.tar` & `tej-tool-api-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/
--rw-rw-rw-   0        0        0     5553 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5143 2023-06-08 06:00:16.000000 tej-tool-api-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.468400 tej-tool-api-1.0.2/TejTOolAPI/
--rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.2/TejTOolAPI/Error.py
--rw-rw-rw-   0        0        0    17148 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/Map_Dask_API.py
--rw-rw-rw-   0        0        0    11098 2023-07-07 05:58:29.000000 tej-tool-api-1.0.2/TejTOolAPI/TejToolAPI.py
--rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/exchange_calendar.py
--rw-rw-rw-   0        0        0     1381 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/parameters.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.468400 tej-tool-api-1.0.2/TejTOolAPI/tables/
--rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/tables/columns_group.xlsx
--rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.2/TejTOolAPI/tables/mktboard.csv
--rw-rw-rw-   0        0        0       42 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1490 2023-07-04 07:26:09.000000 tej-tool-api-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/tej_tool_api.egg-info/
--rw-rw-rw-   0        0        0     5553 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 09:35:58.877329 tej-tool-api-1.0.3/
+-rw-rw-rw-   0        0        0     5564 2023-07-13 09:35:58.877329 tej-tool-api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5154 2023-07-11 07:37:31.000000 tej-tool-api-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 09:35:58.861704 tej-tool-api-1.0.3/TejTOolAPI/
+-rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.3/TejTOolAPI/Error.py
+-rw-rw-rw-   0        0        0    17841 2023-07-13 08:57:10.000000 tej-tool-api-1.0.3/TejTOolAPI/Map_Dask_API.py
+-rw-rw-rw-   0        0        0    11025 2023-07-12 03:01:58.000000 tej-tool-api-1.0.3/TejTOolAPI/TejToolAPI.py
+-rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.3/TejTOolAPI/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.3/TejTOolAPI/exchange_calendar.py
+-rw-rw-rw-   0        0        0     1488 2023-07-12 03:01:58.000000 tej-tool-api-1.0.3/TejTOolAPI/parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:35:58.861704 tej-tool-api-1.0.3/TejTOolAPI/tables/
+-rw-rw-rw-   0        0        0    60467 2023-07-12 03:01:58.000000 tej-tool-api-1.0.3/TejTOolAPI/tables/TQ_Analytics_資料欄位查詢 (4).xlsx
+-rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.3/TejTOolAPI/tables/columns_group.xlsx
+-rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.3/TejTOolAPI/tables/mktboard.csv
+-rw-rw-rw-   0        0        0      165 2023-07-12 03:01:58.000000 tej-tool-api-1.0.3/TejTOolAPI/tables/~$columns_group.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:35:58.877329 tej-tool-api-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2023-07-11 07:38:59.000000 tej-tool-api-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:35:58.877329 tej-tool-api-1.0.3/tej_tool_api.egg-info/
+-rw-rw-rw-   0        0        0     5564 2023-07-13 09:35:58.000000 tej-tool-api-1.0.3/tej_tool_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-07-13 09:35:58.000000 tej-tool-api-1.0.3/tej_tool_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:35:58.000000 tej-tool-api-1.0.3/tej_tool_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 09:35:58.000000 tej-tool-api-1.0.3/tej_tool_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-13 09:35:58.000000 tej-tool-api-1.0.3/tej_tool_api.egg-info/top_level.txt
```

### Comparing `tej-tool-api-1.0.2/PKG-INFO` & `tej-tool-api-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
@@ -16,38 +16,44 @@
 ### 安裝套件
 ```python
 pip install tej-tool-api
 ```
 
 ### 匯入套件
 ```python
-from TejToolAPI.TejToolAPI import *
+import os
+os.environ['TEJAPI_KEY'] = "YOURAPIKEY"
+import TejToolAPI
 ```
 ### get_history_data - 獲取歷史資料<br>
 
 ```python
-from TejToolAPI.TejToolAPI import *
+import TejToolAPI
 tejapi.ApiConfig.api_key = "YOURAPIKEY"
 tejapi.ApiConfig.ignoretz = True
 list_of_Stocks = ['2330','2303','2454', '2882', '2881']
 # 撈取歷史資料
-data = get_history_data(ticker=list_of_Stocks,columns= ['稅前淨利成長率', '單月營收成長率%'], transfer_to_chinese=False)
+data = TejToolAPI.get_history_data(
+ticker=list_of_Stocks,
+columns= ['稅前淨利成長率', '單月營收成長率%'], 
+transfer_to_chinese=False
+)
 ```
 目前資料庫僅支援台灣市場。<br>
-Tool API 可獲取 PIT 資料庫的所有欄位，共計超過 600 個指標，具體指標內容參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) 。<br>
+Tool API 可獲取 PIT 資料庫的所有欄位，共計超過 600 個指標，具體指標內容參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) 。<br>
 財務數據是根據發布日（announcement date）來mapping，非發布日的財務數據會使用當下可獲得最新的資料為準進行填值。ex: 2330 在 2010-02-01 時所能獲得最新的財務資料為 2009Q3 的財務資料，則 2010-01-01 會以 2009Q3 的資料進行填補。惟公司2009Q4自結財報早於 2010-02-01 發布時，且 include_self_acc = 'Y'，這時 2010-02-01 的財務數據使用自結財務數據。<br>
 <br>
 
 **參數:**
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
 | ticker     | Required    | list      | 股票代碼，ex: ['2330', '2881', '2882'] |
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 | start      | Optional    | date/str  | 起始日，ex: '2008-01-01' (預設值為 '2013-01-01')，目前版本尚未支援timezone的設定 |
 | end        | Optional    | date/str  | 結束日，ex: '2008-01-01' (預設值為今日 datetime.now())，目前版本尚未支援timezone的設定|
 | transfer_to_chinese | Optional | boolean | 欄位轉換成中文，若 transfer_to_chinese=True，則欄位顯示為中文名稱，transfer_to_chinese=False，則欄位顯示為英文名稱。(預設為 False)|
 | fin_type   | Optional    | list      | 會計科目類型 -> 單季:Q、累計:A、移動四季:TTM，ex: 撈取單季和累積，fin_type=['Q','A']。(預設為 ['Q','A','TTM']) |
 | include_self_acc | Optional | string | 財務是否包含公司自結損益，include_self_acc='Y'，表示財務資料包含自結損益，否則僅有財簽資料 (預設為 'N') |
 | npartitions | Optional    | int       | 多核心執行，可以指定執行所要使用的核心數量，ex: npartitions=6，代表使用6個核心來運行程式 (預設為當前 CPU 可使用之核心數) |
 
@@ -59,20 +65,19 @@
 get_internal_code(['稅前淨利成長率', 'Gross_Profit_Loss_from_Operations'])
 
 ```
 ```html
 output: ['r404', 'gm']
 ```
 <br>
-
 **參數:**
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 
 
 ### search_columns <br>
 若想從內部編碼反向取得 columns 所對應之中英文欄位則可利用 search_columns 這個function <br>
 
 ```python
 search_columns(['r404'])
@@ -87,30 +92,29 @@
 
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 
 ### search_table <br>
 ```python
 search_table(['r404'])
 ```
 
 | COLUMNS | TABLE_NAMES | 
 |---------|-----------------|
 | r404    | fin_self_acc    |
 | r404    | fin_auditor    |
 
 <br>
-
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
```

### Comparing `tej-tool-api-1.0.2/README.md` & `tej-tool-api-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,38 +2,44 @@
 ### 安裝套件
 ```python
 pip install tej-tool-api
 ```
 
 ### 匯入套件
 ```python
-from TejToolAPI.TejToolAPI import *
+import os
+os.environ['TEJAPI_KEY'] = "YOURAPIKEY"
+import TejToolAPI
 ```
 ### get_history_data - 獲取歷史資料<br>
 
 ```python
-from TejToolAPI.TejToolAPI import *
+import TejToolAPI
 tejapi.ApiConfig.api_key = "YOURAPIKEY"
 tejapi.ApiConfig.ignoretz = True
 list_of_Stocks = ['2330','2303','2454', '2882', '2881']
 # 撈取歷史資料
-data = get_history_data(ticker=list_of_Stocks,columns= ['稅前淨利成長率', '單月營收成長率%'], transfer_to_chinese=False)
+data = TejToolAPI.get_history_data(
+ticker=list_of_Stocks,
+columns= ['稅前淨利成長率', '單月營收成長率%'], 
+transfer_to_chinese=False
+)
 ```
 目前資料庫僅支援台灣市場。<br>
-Tool API 可獲取 PIT 資料庫的所有欄位，共計超過 600 個指標，具體指標內容參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) 。<br>
+Tool API 可獲取 PIT 資料庫的所有欄位，共計超過 600 個指標，具體指標內容參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) 。<br>
 財務數據是根據發布日（announcement date）來mapping，非發布日的財務數據會使用當下可獲得最新的資料為準進行填值。ex: 2330 在 2010-02-01 時所能獲得最新的財務資料為 2009Q3 的財務資料，則 2010-01-01 會以 2009Q3 的資料進行填補。惟公司2009Q4自結財報早於 2010-02-01 發布時，且 include_self_acc = 'Y'，這時 2010-02-01 的財務數據使用自結財務數據。<br>
 <br>
 
 **參數:**
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
 | ticker     | Required    | list      | 股票代碼，ex: ['2330', '2881', '2882'] |
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 | start      | Optional    | date/str  | 起始日，ex: '2008-01-01' (預設值為 '2013-01-01')，目前版本尚未支援timezone的設定 |
 | end        | Optional    | date/str  | 結束日，ex: '2008-01-01' (預設值為今日 datetime.now())，目前版本尚未支援timezone的設定|
 | transfer_to_chinese | Optional | boolean | 欄位轉換成中文，若 transfer_to_chinese=True，則欄位顯示為中文名稱，transfer_to_chinese=False，則欄位顯示為英文名稱。(預設為 False)|
 | fin_type   | Optional    | list      | 會計科目類型 -> 單季:Q、累計:A、移動四季:TTM，ex: 撈取單季和累積，fin_type=['Q','A']。(預設為 ['Q','A','TTM']) |
 | include_self_acc | Optional | string | 財務是否包含公司自結損益，include_self_acc='Y'，表示財務資料包含自結損益，否則僅有財簽資料 (預設為 'N') |
 | npartitions | Optional    | int       | 多核心執行，可以指定執行所要使用的核心數量，ex: npartitions=6，代表使用6個核心來運行程式 (預設為當前 CPU 可使用之核心數) |
 
@@ -45,20 +51,19 @@
 get_internal_code(['稅前淨利成長率', 'Gross_Profit_Loss_from_Operations'])
 
 ```
 ```html
 output: ['r404', 'gm']
 ```
 <br>
-
 **參數:**
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 
 
 ### search_columns <br>
 若想從內部編碼反向取得 columns 所對應之中英文欄位則可利用 search_columns 這個function <br>
 
 ```python
 search_columns(['r404'])
@@ -73,30 +78,29 @@
 
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 
 ### search_table <br>
 ```python
 search_table(['r404'])
 ```
 
 | COLUMNS | TABLE_NAMES | 
 |---------|-----------------|
 | r404    | fin_self_acc    |
 | r404    | fin_auditor    |
 
 <br>
-
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
```

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/Map_Dask_API.py` & `tej-tool-api-1.0.3/TejTOolAPI/Map_Dask_API.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-# import os
 import tejapi
-# tejapi.ApiConfig.ignoretz = True
-# tejapi.ApiConfig.page_limit=10000
-# tejapi.ApiConfig.api_base = os.environ.get('TEJAPI_BASE')
-# tejapi.ApiConfig.api_key = os.environ.get('TEJAPI_KEY')
-
 import pandas as pd
 import datetime
 import numpy as np
 import dask.dataframe as dd
 import dask
 import gc
 from . import parameters as para
@@ -40,17 +34,14 @@
             return pd.DataFrame({'coid': pd.Series(dtype='object'),
                                   'mdate': pd.Series(dtype='datetime64[ns]'),
                                   'key3': pd.Series(dtype='object'),
                                   'no': pd.Series(dtype='object'),
                                   'annd':pd.Series(dtype='datetime64[ns]')
                                     })
 
-        # select certain fin_type
-        # data_sets = get_certain_fin_type(data_sets, fin_type)
-
         # parallel fin_type to columns 
         data_sets = fin_pivot(data_sets, remain_keys=['coid', 'mdate', 'no', 'annd'])
 
         return data_sets
     
     # Define the meta of the dataframe
     meta = get_data(table = table, tickers = '2330', columns = columns, start = start, end =end, fin_type= fin_type)
@@ -61,14 +52,17 @@
     # Submit jobs to the parallel cores
     data_sets = dd.from_delayed([dask.delayed(get_data)(table=table, tickers = tickers[(i-1)*npartitions:i*npartitions]+['2330'], columns = columns, start = start, end = end, fin_type = fin_type) for i in range(1, ticker_partitions)], meta = meta)
     
     # If ticker smaller than defaulted partitions, then transform it into defaulted partitions
     if data_sets.npartitions < npartitions:
         data_sets = data_sets.repartition(npartitions=npartitions)
     
+    if '2330' not in tickers:
+        data_sets = data_sets.loc[~(data_sets['coid']=='2330'),:]
+    
     data_sets = data_sets.drop_duplicates(subset=['coid', 'annd'], keep = 'last')
 
     return data_sets
 
 
 def get_most_recent_date(data, sort_keys, subset, keep_mothod):
     # sort data order by mdate(accural date) and annd_s(announce date)
@@ -93,14 +87,20 @@
     def get_data(table, tickers, columns, start, end):
         data = tejapi.get(table,
                         coid = tickers,
                         paginate = True,
                         chinese_column_name=False,
                         mdate = {'gte':start,'lte':end},
                         opts = {'columns':columns, 'sort':{'coid.asc', 'mdate.asc'}})
+        # 
+        if len(data) < 1:
+            return pd.DataFrame({'coid': pd.Series(dtype='object'),
+                                  'mdate': pd.Series(dtype='datetime64[ns]')
+                                    })
+        
         return data
     
     # Define the meta of the dataframe
     meta = get_data(table = table, tickers = '2330', columns=columns, start = start, end =end)
 
     # Calculate the number of tickers in each partition.
     ticker_partitions = get_partition_group(tickers=tickers, npartitions=npartitions)
@@ -109,14 +109,17 @@
     data_sets = dd.from_delayed([dask.delayed(get_data)(table, tickers[(i-1)*npartitions:i*npartitions]+['2330'], columns, start, end) for i in range(1, ticker_partitions)], meta = meta)
     
     # If ticker smaller than defaulted partitions, then transform it into defaulted partitions
     if data_sets.npartitions < npartitions:
         data_sets = data_sets.repartition(npartitions=npartitions)
 
     data_sets = data_sets.drop_duplicates(subset=['coid', 'mdate'], keep = 'last')
+    
+    if '2330' not in tickers:
+        data_sets = data_sets.loc[~(data_sets['coid']=='2330'),:]
 
     return data_sets
 
 def get_alternative_data(table, tickers=[], columns = [], **kwargs):
     start = kwargs.get('start', para.default_start)
     end = kwargs.get('end', para.default_end)
     # transfer_to_chinese = False
@@ -158,20 +161,15 @@
     dict_map = {uni_dates[i]:result[i] for i in range(len(result))}
 
     # Adjust non-trading announce date to next trading date.
     data_sets[annd] = data_sets[annd].map(dict_map)
     
     data_sets = data_sets.drop(columns=['mdate'])
 
-    if table == 'TWN/APISALE':
-        # data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates', 'coid'], right_on=['annd_s', 'coid'])
-        data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates'], right_on=['annd_s'])
-    else:
-        # data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates', 'coid'], right_on=['edate1', 'coid'])
-        data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates'], right_on=['edate1'])
+    data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates'], right_on=[annd])
 
     del days
     gc.collect()
 
     data_sets = data_sets.groupby('coid', group_keys = False).apply(fillna_multicolumns)
 
     return data_sets
@@ -198,15 +196,15 @@
                             key3 = fin_type, 
                             paginate = True,
                             chinese_column_name=False,
                             mdate = {'gte':start,'lte':end},
                             opts= {'columns':columns, 'sort':{'coid.asc', 'mdate.asc', 'key3.asc', 'no.asc'}, 'pivot':True})
         
         columns.append('annd')
-
+        # print(fin_type)
         if len(data_sets) < 1:
             return pd.DataFrame({'coid': pd.Series(dtype='object'),
                                 'mdate': pd.Series(dtype='datetime64[ns]'),
                                 'key3': pd.Series(dtype='object'),
                                 'no': pd.Series(dtype='object')
                                     })
         
@@ -234,35 +232,32 @@
             
             # Select columns again
             data_sets = data_sets.loc[:,selected_columns]
 
         # Parallel fin_type (key3) to columns 
         data_sets = fin_pivot(data_sets, remain_keys=['coid','mdate','no','annd'])
         
-        # Cut off the duplicate rows
-        # data_sets = data_sets.sort_values(['coid','mdate', 'annd'])
-        # data_sets = data_sets.drop_duplicates(subset=['coid','annd'], keep = 'last')
-        
         return data_sets
-        
-        # except: 
-        #     print(tickers, columns)
+
     
     # Define the meta of the dataframe
     meta = _get_data(table = table, tickers = '2330', columns = columns, start = start, end =end, fin_type= fin_type)
 
     # 
     ticker_partitions = get_partition_group(tickers=tickers, npartitions=npartitions)
     
     # Submit jobs to the parallel cores
     data_sets = dd.from_delayed([dask.delayed(_get_data)(table=table, tickers = tickers[(i-1)*npartitions:i*npartitions]+['2330'], columns = columns, start = start, end = end, fin_type = fin_type) for i in range(1, ticker_partitions)], meta = meta)
     
     # If ticker smaller than defaulted partitions, then transform it into defaulted partitions
     if data_sets.npartitions < npartitions:
         data_sets = data_sets.repartition(npartitions=npartitions)
+    
+    if '2330' not in tickers:
+        data_sets = data_sets.loc[~(data_sets['coid']=='2330'),:]
 
     data_sets = data_sets.drop_duplicates(subset=['coid','annd'], keep = 'last')
 
     return data_sets
 
 
 def get_announce_date(tickers, **kwargs):
@@ -274,41 +269,79 @@
                     coid = tickers,
                     paginate = True,
                     key3 = fin_type,
                     chinese_column_name=False, 
                     mdate = {'gte':start, 'lte':end},
                     opts = {'sort':{'coid.asc', 'mdate.asc', 'key3.asc', 'no.asc','annd.asc'}})
 
+    
+    data = parallize_annd_process(data)
+    # Keep the last row when there are multiple rows with the same keys
+    # The last row represents the data with the greatest mdate
+    # data = data.drop_duplicates(subset=['coid', 'key3','annd'], keep='last')
+    data['ver'] = data['mdate'].astype(str) + '-' + data['no']
+    data = data.groupby(['coid', 'key3','annd'], as_index=False).max()
+    data = data.groupby(['coid','key3']).apply(lambda x: np.fmax.accumulate(x, axis=0))
+    data = parallelize_ver_process(data)
+    data.drop(columns = 'ver')
+
+    return data
+
+def parallize_annd_process(data):
+    # annd
     # 創建一個向量化的函數
     vectorized_annd_adjusted = np.vectorize(annd_adjusted)
 
     # 所有不同的發布日
     uni_dates = pd.to_datetime(data['annd'].unique())
 
     # 傳入 ExchangeCalendar 物件
     result = vectorized_annd_adjusted(para.exc, uni_dates)
 
     # Create a mapping dictionary
     dict_map = {uni_dates[i]:result[i] for i in range(len(result))}
 
-    # Adjust non-trading announce date to next trading date.
     data['annd'] = data['annd'].map(dict_map)
+    
+    return data
 
-    # Keep the last row when there are multiple rows with the same keys
-    # The last row represents the data with the greatest mdate
-    data = data.drop_duplicates(subset=['coid', 'key3','annd'], keep='last')
+def parallelize_ver_process(data):
+    def parallel_process(func, data):
+        vectorized = np.vectorize(func)
+        uni_dates = data['ver'].unique()
+        result = vectorized(uni_dates)
+        dict_map = {uni_dates[i]:result[i] for i in range(len(result))}
+        return dict_map
+    
+    # mdate
+    mdate_dict = parallel_process(split_mdate, data)
+    data['mdate'] = data['ver'].map(mdate_dict)
+
+    # no
+    no_dict = parallel_process(split_no, data)
+    data['no'] = data['ver'].map(no_dict)
 
     return data
 
+
 def annd_adjusted(ExchangeCalendar, date):
         if ExchangeCalendar.is_session(date):
             return date
         
         return ExchangeCalendar.next_open(date)
 
+def split_mdate(string:str):
+    mdate = string.split('-')[:2]
+    mdate = pd.to_datetime('-'.join(mdate))
+    return mdate
+
+def split_no(string:str):
+    no = string.split('-')[-1]
+    return no
+
 def fin_pivot(df, remain_keys):
     # for loop execute pviot function
     uni = df['key3'].dropna().unique()
     data = pivot(df, remain_keys, uni[0])
 
     for i in range(1, len(uni)):
         temp = pivot(df, remain_keys, uni[i])
```

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/TejToolAPI.py` & `tej-tool-api-1.0.3/TejTOolAPI/TejToolAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import tejapi
-# tejapi.ApiConfig.ignoretz = True
-# tejapi.ApiConfig.page_limit=10000
 import dask.dataframe as dd
 import pandas as pd
 import gc
 from . import parameters as para
 from . import Map_Dask_API as dask_api
 import dask
```

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/__init__.py` & `tej-tool-api-1.0.3/TejTOolAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/exchange_calendar.py` & `tej-tool-api-1.0.3/TejTOolAPI/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/parameters.py` & `tej-tool-api-1.0.3/TejTOolAPI/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import pandas as pd
 import datetime
 import multiprocessing as mp
 import os
 from .exchange_calendar import ExchangeCalendar
 
 # Initialize exchange calendar
-exc = ExchangeCalendar()
+try:
+    exc = ExchangeCalendar()
+except:
+    raise ValueError('請設定 TEJAPI_KEY ： os.environ["TEJAPI_KEY"] = "your_key"')
 
 # current directory
 module_dir = os.path.dirname(os.path.abspath(__file__))
 xlsx_path = os.path.join(module_dir,'tables','columns_group.xlsx')
 
 # get number of cpu
 npartitions_local = mp.cpu_count()
```

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/tables/columns_group.xlsx` & `tej-tool-api-1.0.3/TejTOolAPI/tables/columns_group.xlsx`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.2/TejTOolAPI/tables/mktboard.csv` & `tej-tool-api-1.0.3/TejTOolAPI/tables/mktboard.csv`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.2/setup.py` & `tej-tool-api-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 long_description = (this_directionary/"README.md").read_text(encoding='utf-8')
 setup(
     name='tej-tool-api',
     description='Package to fetch a large quantity of data from tejapi.',
     keywords=['tej', 'big data', 'data', 'financial', 'economic','stock','TEJ',],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.2',
+    version='1.0.3',
     author='tej',
     author_email='tej@tej.com.tw',
     maintainer='tej api Development Team',
     maintainer_email='tej@tej.com',
     url='https://api.tej.com.tw',
     license='MIT',
     install_requires=install_requires,
```

### Comparing `tej-tool-api-1.0.2/tej_tool_api.egg-info/PKG-INFO` & `tej-tool-api-1.0.3/tej_tool_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
@@ -16,38 +16,44 @@
 ### 安裝套件
 ```python
 pip install tej-tool-api
 ```
 
 ### 匯入套件
 ```python
-from TejToolAPI.TejToolAPI import *
+import os
+os.environ['TEJAPI_KEY'] = "YOURAPIKEY"
+import TejToolAPI
 ```
 ### get_history_data - 獲取歷史資料<br>
 
 ```python
-from TejToolAPI.TejToolAPI import *
+import TejToolAPI
 tejapi.ApiConfig.api_key = "YOURAPIKEY"
 tejapi.ApiConfig.ignoretz = True
 list_of_Stocks = ['2330','2303','2454', '2882', '2881']
 # 撈取歷史資料
-data = get_history_data(ticker=list_of_Stocks,columns= ['稅前淨利成長率', '單月營收成長率%'], transfer_to_chinese=False)
+data = TejToolAPI.get_history_data(
+ticker=list_of_Stocks,
+columns= ['稅前淨利成長率', '單月營收成長率%'], 
+transfer_to_chinese=False
+)
 ```
 目前資料庫僅支援台灣市場。<br>
-Tool API 可獲取 PIT 資料庫的所有欄位，共計超過 600 個指標，具體指標內容參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) 。<br>
+Tool API 可獲取 PIT 資料庫的所有欄位，共計超過 600 個指標，具體指標內容參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) 。<br>
 財務數據是根據發布日（announcement date）來mapping，非發布日的財務數據會使用當下可獲得最新的資料為準進行填值。ex: 2330 在 2010-02-01 時所能獲得最新的財務資料為 2009Q3 的財務資料，則 2010-01-01 會以 2009Q3 的資料進行填補。惟公司2009Q4自結財報早於 2010-02-01 發布時，且 include_self_acc = 'Y'，這時 2010-02-01 的財務數據使用自結財務數據。<br>
 <br>
 
 **參數:**
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
 | ticker     | Required    | list      | 股票代碼，ex: ['2330', '2881', '2882'] |
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 | start      | Optional    | date/str  | 起始日，ex: '2008-01-01' (預設值為 '2013-01-01')，目前版本尚未支援timezone的設定 |
 | end        | Optional    | date/str  | 結束日，ex: '2008-01-01' (預設值為今日 datetime.now())，目前版本尚未支援timezone的設定|
 | transfer_to_chinese | Optional | boolean | 欄位轉換成中文，若 transfer_to_chinese=True，則欄位顯示為中文名稱，transfer_to_chinese=False，則欄位顯示為英文名稱。(預設為 False)|
 | fin_type   | Optional    | list      | 會計科目類型 -> 單季:Q、累計:A、移動四季:TTM，ex: 撈取單季和累積，fin_type=['Q','A']。(預設為 ['Q','A','TTM']) |
 | include_self_acc | Optional | string | 財務是否包含公司自結損益，include_self_acc='Y'，表示財務資料包含自結損益，否則僅有財簽資料 (預設為 'N') |
 | npartitions | Optional    | int       | 多核心執行，可以指定執行所要使用的核心數量，ex: npartitions=6，代表使用6個核心來運行程式 (預設為當前 CPU 可使用之核心數) |
 
@@ -59,20 +65,19 @@
 get_internal_code(['稅前淨利成長率', 'Gross_Profit_Loss_from_Operations'])
 
 ```
 ```html
 output: ['r404', 'gm']
 ```
 <br>
-
 **參數:**
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 
 
 ### search_columns <br>
 若想從內部編碼反向取得 columns 所對應之中英文欄位則可利用 search_columns 這個function <br>
 
 ```python
 search_columns(['r404'])
@@ -87,30 +92,29 @@
 
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
 
 ### search_table <br>
 ```python
 search_table(['r404'])
 ```
 
 | COLUMNS | TABLE_NAMES | 
 |---------|-----------------|
 | r404    | fin_self_acc    |
 | r404    | fin_auditor    |
 
 <br>
-
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
-| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](https://api.tej.com.tw/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
+| columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
```

