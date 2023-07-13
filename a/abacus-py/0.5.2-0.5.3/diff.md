# Comparing `tmp/abacus_py-0.5.2.tar.gz` & `tmp/abacus_py-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abacus_py-0.5.2.tar", max compression
+gzip compressed data, was "abacus_py-0.5.3.tar", max compression
```

## Comparing `abacus_py-0.5.2.tar` & `abacus_py-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1083 2023-07-02 14:22:37.926844 abacus_py-0.5.2/abacus/__init__.py
--rw-r--r--   0        0        0     2072 2023-07-09 11:53:45.981139 abacus_py-0.5.2/abacus/accounting_types.py
--rw-r--r--   0        0        0     4229 2023-07-01 14:16:18.359232 abacus_py-0.5.2/abacus/accounts.py
--rw-r--r--   0        0        0     5332 2023-07-09 11:53:45.981139 abacus_py-0.5.2/abacus/book.py
--rw-r--r--   0        0        0    14775 2023-07-13 06:46:53.332075 abacus_py-0.5.2/abacus/bx.py
--rw-r--r--   0        0        0     5681 2023-07-09 11:53:45.981139 abacus_py-0.5.2/abacus/chart.py
--rw-r--r--   0        0        0     2953 2023-06-18 14:34:57.659155 abacus_py-0.5.2/abacus/closing.py
--rw-r--r--   0        0        0     5026 2023-07-01 14:16:18.381634 abacus_py-0.5.2/abacus/ledger.py
--rw-r--r--   0        0        0     1978 2023-07-08 15:35:17.258226 abacus_py-0.5.2/abacus/reports.py
--rw-r--r--   0        0        0      885 2023-06-04 06:28:14.876039 abacus_py-0.5.2/abacus/shortcodes.py
--rw-r--r--   0        0        0     6550 2023-07-08 15:35:16.001265 abacus_py-0.5.2/abacus/tables.py
--rw-r--r--   0        0        0    35823 2023-05-28 16:48:33.004211 abacus_py-0.5.2/LICENSE
--rw-r--r--   0        0        0     1018 2023-07-13 06:57:56.304842 abacus_py-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     8509 2023-07-09 11:53:45.975129 abacus_py-0.5.2/README.md
--rw-r--r--   0        0        0     9091 1970-01-01 00:00:00.000000 abacus_py-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-02 14:22:37.926844 abacus_py-0.5.3/abacus/__init__.py
+-rw-r--r--   0        0        0     2072 2023-07-09 11:53:45.981139 abacus_py-0.5.3/abacus/accounting_types.py
+-rw-r--r--   0        0        0     4229 2023-07-01 14:16:18.359232 abacus_py-0.5.3/abacus/accounts.py
+-rw-r--r--   0        0        0     5332 2023-07-09 11:53:45.981139 abacus_py-0.5.3/abacus/book.py
+-rw-r--r--   0        0        0    14901 2023-07-13 07:21:57.203751 abacus_py-0.5.3/abacus/bx.py
+-rw-r--r--   0        0        0     5681 2023-07-09 11:53:45.981139 abacus_py-0.5.3/abacus/chart.py
+-rw-r--r--   0        0        0     2953 2023-06-18 14:34:57.659155 abacus_py-0.5.3/abacus/closing.py
+-rw-r--r--   0        0        0     5026 2023-07-01 14:16:18.381634 abacus_py-0.5.3/abacus/ledger.py
+-rw-r--r--   0        0        0     1978 2023-07-08 15:35:17.258226 abacus_py-0.5.3/abacus/reports.py
+-rw-r--r--   0        0        0      885 2023-06-04 06:28:14.876039 abacus_py-0.5.3/abacus/shortcodes.py
+-rw-r--r--   0        0        0     6550 2023-07-08 15:35:16.001265 abacus_py-0.5.3/abacus/tables.py
+-rw-r--r--   0        0        0    35823 2023-05-28 16:48:33.004211 abacus_py-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1018 2023-07-13 21:06:32.279459 abacus_py-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     8915 2023-07-13 21:04:00.043462 abacus_py-0.5.3/README.md
+-rw-r--r--   0        0        0     9752 1970-01-01 00:00:00.000000 abacus_py-0.5.3/PKG-INFO
```

### Comparing `abacus_py-0.5.2/abacus/__init__.py` & `abacus_py-0.5.3/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/accounting_types.py` & `abacus_py-0.5.3/abacus/accounting_types.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/accounts.py` & `abacus_py-0.5.3/abacus/accounts.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/book.py` & `abacus_py-0.5.3/abacus/book.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/bx.py` & `abacus_py-0.5.3/abacus/bx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Double entry accounting manager.
 
 Usage:
+  bx chart start [-f | --force] [--chart-file <chart-file>]
   bx chart set --asset <account_name> [--title <title>] [--code <code>] 
   bx chart set --expense <account_name> [--title <title>] [--code <code>]
   bx chart set --capital <account_name> [--title <title>] [--code <code>]
   bx chart set --retained-earnings <account_name>
   bx chart set --liability <account_name> [--title <title>] [--code <code>]
   bx chart set --income <account_name> [--title <title>] [--code <code>]
   bx chart offset <account_name> <contra_account_names>...
   bx chart title <account_name> <title>
   bx chart set-title <account_name> <title>
   bx chart set-code <account_name> <code>
   bx chart show [--json]
   bx operation set <name> --debit <dr_account> --credit <cr_account> [--describe <text>] [--requires <matched_name>]
-  bx operation show
+  bx operation show [<name>]
+  bx ledger start [--file <balances_file>] [--dry-run]
   bx post operation (<operations> <amounts>)... 
   bx post operation -t <title> (<operations> <amounts>)... 
   bx post operation --title <title> --name <operation> --amount <amount> 
   bx post entry --debit <dr> --credit <cr> --amount <amount> [--adjust] [--after-close]
   bx post entry -t <title> --debit <dr> --credit <cr> --amount <amount> [--adjust] [--after-close]
   bx ledger close
   bx ledger list (--start | --business | --adjust | --close | --after-close | --all) [--json]
```

### Comparing `abacus_py-0.5.2/abacus/chart.py` & `abacus_py-0.5.3/abacus/chart.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/closing.py` & `abacus_py-0.5.3/abacus/closing.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/ledger.py` & `abacus_py-0.5.3/abacus/ledger.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/reports.py` & `abacus_py-0.5.3/abacus/reports.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/shortcodes.py` & `abacus_py-0.5.3/abacus/shortcodes.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/abacus/tables.py` & `abacus_py-0.5.3/abacus/tables.py`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/LICENSE` & `abacus_py-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `abacus_py-0.5.2/pyproject.toml` & `abacus_py-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.ruff]
 ignore=['E501', 'E741']
 extend-exclude=["minimal.py"]
 
 [tool.poetry]
 name = "abacus-py"
-version = "0.5.2"
+version = "0.5.3"
 description = "A minimal, yet valid double-entry accounting system in Python."
 authors = ["Evgeniy Pogrebnyak <e.pogrebnyak@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "abacus"}
 ]
```

### Comparing `abacus_py-0.5.2/README.md` & `abacus_py-0.5.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,255 +1,304 @@
-# abacus
-
-[![pytest](https://github.com/epogrebnyak/abacus/actions/workflows/.pytest.yml/badge.svg)](https://github.com/epogrebnyak/abacus/actions/workflows/.pytest.yml)
-
-A minimal, yet valid double-entry accounting system, provided as a Python package and a command line tool.
-
-Using `abacus` you can define a chart of accounts, create a general ledger, post
-entries, close accounts at period end and produce trial balance, balance sheet and income statement.
-
-## Documentation
-
-<https://epogrebnyak.github.io/abacus/>
-
-## Quotes about `abacus`
-
-[![Reddit Discussion](https://img.shields.io/badge/Reddit-%23FF4500.svg?style=for-the-badge&logo=Reddit&logoColor=white)](https://www.reddit.com/r/Accounting/comments/136rrit/wrote_an_accounting_demo_in_python/)
-
-> I think it's a great idea to mock-up a mini GL ERP to really get a foundational understanding of how the accounting in ERP works!
-
-> I teach accounting information systems... I'd be tempted to use abacus as a way of simply showing the structure of a simple AIS.
-
-> Hey, what a cool job, thanks much. Do you plan to make a possibility for RAS accounting?
-
-## Install
-
-```
-pip install git+https://github.com/epogrebnyak/abacus.git
-```
-
-This will install both `abacus` package and the `bx` command line tool.
-
-## Minimal example
-
-A freshly created trading Klondike Trading Company (KTC) has recorded the following transactions.
-
-|     | Transaction Title                         |        Debit        |       Credit        | Amount |
-| --- | ----------------------------------------- | :-----------------: | :-----------------: | -----: |
-| 1   | Shareholders paid up capital contribution |        Cash         |       Equity        |   1000 |
-| 2   | Purchased goods for resale                |      Inventory      |        Cash         |    800 |
-| 3   | Invoiced client on sales contract         | Accounts Receivable |       Revenue       |    465 |
-| 4   | Provided discount to client               |      Discounts      | Accounts Receivable |     65 |
-| 5   | Recorded cost of sales                    |        COGS         |      Inventory      |    200 |
-| 6   | Paid salary to contract manager           |    SG&A Expenses    |        Cash         |    100 |
-| 7   | Accepted payment on sales contract        |        Cash         | Accounts Receivable |    360 |
-
-After closing accounts the company announced, but has not paid dividend.
-
-|     | Transaction Title                   |       Debit       |    Credit    | Amount |
-| --- | ----------------------------------- | :---------------: | :----------: | -----: |
-| \*  | Accrued dividend after announcement | Retained Earnings | Dividend Due |     50 |
-
-### 1. Chart
-
-Define a chart of accounts of five types (assets, equity, liabilities, income and expenses),
-specify retained earnings account name and, optionally, add contra accounts.
-
-```python
-from abacus import Chart
-
-chart = Chart(
-    assets=["cash", "ar", "goods"],
-    expenses=["cogs", "sga"],
-    equity=["equity"],
-    liabilities=["dividend_due"],
-    income=["sales"])
-chart = chart.set_retained_earnings("re").offset("sales", ["discounts"])
-```
-
-### 2. Ledger
-
-Create a general ledger based on the chart of accounts,
-post entries and close accounts at accounting period end.
-
-```python
-book = (chart.book()
-  .post(debit="cash", credit="equity", amount=1000)
-  .post(debit="goods", credit="cash", amount=800)
-  .post(debit="ar", credit="sales", amount=465)
-  .post(debit="discounts", credit="ar", amount=65)
-  .post(debit="cogs", credit="goods", amount=200)
-  .post(debit="sga", credit="cash", amount=100)
-  .post(debit="cash", credit="ar", amount=360)
-  .close()
-  .after_close(debit="re", credit="dividend_due", amount=50)
-)
-```
-
-### 3. Reports
-
-Make trail balance, income statement and balance sheet and save or print them to screen
-with verbose account names and rich text formatting.
-
-```python
-from abacus import RichViewer, PlainTextViewer
-
-income_statement = book.income_statement()
-balance_sheet = book.balance_sheet()
-rename_dict = {
-    "re": "Retained earnings",
-    "ar": "Accounts receivable",
-    "goods": "Inventory (goods for sale)",
-    "cogs": "Cost of goods sold",
-    "sga": "Selling, general and adm. expenses",
-}
-
-tv = PlainTextViewer(rename_dict)
-tv.print(balance_sheet)
-tv.print(income_statement)
-
-rv = RichViewer(rename_dict, width=80)
-rv.print(balance_sheet)
-rv.print(income_statement)
-```
-
-The output should look similar to text and a screenshot below.
-
-```
-Assets                        1100  Capital              1050
-- Cash                        460   - Equity             1000
-- Accounts receivable         40    - Retained earnings    50
-- Inventory (goods for sale)  600   Liabilities            50
-                                    - Dividend due         50
-Total                         1100  Total                1100
-
-Income                                400
-- Sales                               400
-Expenses                              300
-- Cost of goods sold                  200
-- Selling, general and adm. expenses  100
-Profit                                100
-```
-
-<details>
-<summary> Screenshot (outdated).
-</summary>
-
-![](https://user-images.githubusercontent.com/9265326/249445794-7def0fc2-934b-49fa-a3ad-9137072a2900.png)
-
-</details>
-
-<details>
-<summary> Details about correctness checks and end balances.
-</summary>
-
-### Check values
-
-As a reminder `assert` statement in Python will raise exception if provided wrong comparison.
-These checks will execute and this way we will know the code in README is up to date and correct.
-
-```python
-from abacus import IncomeStatement, BalanceSheet
-
-print(income_statement)
-assert income_statement == IncomeStatement(
-    income={'sales': 400},
-    expenses={'cogs': 200, 'sga': 100}
-)
-print(balance_sheet)
-assert balance_sheet == BalanceSheet(
-  assets={'cash': 460, 'ar': 40, 'goods': 600},
-  capital={'equity': 1000, 're': 50},
-  liabilities={'dividend_due': 50}
-)
-```
-
-### End balances
-
-You can use end balances from current period to initialize ledger at the start of next accounting period.
-
-```python
-end_balances = book.nonzero_balances()
-print(end_balances)
-next_book = chart.book(starting_balances=end_balances)
-```
-
-</details>
-
-## Command line
-
-Similar operations with chart, ledger and reports can be performed on the command line.
-
-### Create chart of accounts
-
-```bash
-bx erase --chart
-bx chart set --asset cash
-bx chart set --asset ar --title "Accounts receivable"
-bx chart set --asset goods --title "Inventory (good for sale)"
-bx chart set --capital equity
-bx chart set --retained-earnings re
-bx chart set --liability dividend_due
-bx chart set --income sales
-bx chart set --expense cogs --title "Cost of sales"
-bx chart set --expense sga --title "Selling expenses"
-bx chart offset sales discounts
-bx chart show
-```
-
-### Post entries to ledger and close
-
-```bash
-bx erase --ledger
-bx ledger start
-bx post entry --debit cash      --credit equity --amount 1000
-bx post entry --debit goods     --credit cash   --amount 800
-bx post entry --debit ar        --credit sales  --amount 465
-bx post entry --debit discounts --credit ar     --amount 65
-bx post entry --debit cogs      --credit goods  --amount 200
-bx post entry --debit sga       --credit cash   --amount 100
-bx post entry --debit cash      --credit ar     --amount 360
-bx ledger close
-bx post entry --debit re --credit dividend_due --amount 50 --after-close
-```
-
-### Report
-
-```bash
-bx report --balance-sheet
-bx report --income-statement
-```
-
-### Account information
-
-```bash
-bx account cash
-bx account ar
-bx account goods
-bx account sales
-bx accounts
-```
-
-You can save end balances to a file and initialize next period ledger.
-
-```bash
-bx accounts --json > end_balances.json
-```
-
-`assert` command will complain if account balance is not equal to provided value.
-This is useful for testing.
-
-```bash
-bx assert cash 460
-```
-
-## Feedback
-
-Anything missing in `abacus`?
-Got a good use case for `abacus` or used `abacus` for teaching?
-
-Feel free to contact `abacus` author
-in [issues](https://github.com/epogrebnyak/abacus/issues),
-on [reddit](https://www.reddit.com/user/iamevpo)
-or via [Telegram](https://t.me/epoepo).
-
-Your feedback is highly appreciated and helps steering development of `abacus`.
+Metadata-Version: 2.1
+Name: abacus-py
+Version: 0.5.3
+Summary: A minimal, yet valid double-entry accounting system in Python.
+Author: Evgeniy Pogrebnyak
+Author-email: e.pogrebnyak@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: types-docopt (>=0.6.11.3,<0.7.0.0)
+Description-Content-Type: text/markdown
+
+# abacus
+
+[![pytest](https://github.com/epogrebnyak/abacus/actions/workflows/.pytest.yml/badge.svg)](https://github.com/epogrebnyak/abacus/actions/workflows/.pytest.yml)
+![PyPI](https://img.shields.io/pypi/v/abacus-py?color=blue)
+
+A minimal, yet valid double-entry accounting system, provided as `abacus-py` Python package and `bx` command line tool.
+
+Using `abacus` you can define a chart of accounts, create a general ledger, post entries,
+close accounts properly at accounting period end and produce trial balance, balance sheet and income statement.
+
+The very minimal example of using `abacus` at command line is the following:
+
+```bash
+pip install abacus-py
+mkdir abacus_demo && cd abacus_demo
+bx erase --chart
+bx chart set --asset cash
+bx chart set --capital equity
+bx chart set --retained-earnings re
+bx ledger start
+bx post entry --title "Initial investment" --debit cash --credit equity --amount 5000
+bx ledger close
+bx report --balance-sheet
+```
+
+<!-- TODO: add corresponding Python code -->
+
+## Documentation
+
+<https://epogrebnyak.github.io/abacus/>
+
+## Quotes about `abacus`
+
+[![Reddit Discussion](https://img.shields.io/badge/Reddit-%23FF4500.svg?style=for-the-badge&logo=Reddit&logoColor=white)](https://www.reddit.com/r/Accounting/comments/136rrit/wrote_an_accounting_demo_in_python/)
+
+> I think it's a great idea to mock-up a mini GL ERP to really get a foundational understanding of how the accounting in ERP works!
+
+> I teach accounting information systems... I'd be tempted to use abacus as a way of simply showing the structure of a simple AIS.
+
+> Hey, what a cool job, thanks much. Do you plan to make a possibility for RAS accounting?
+
+## Install
+
+```
+pip install abacus-py
+```
+
+For latest version install from github:
+
+```
+pip install git+https://github.com/epogrebnyak/abacus.git
+```
+
+This will install both `abacus-py` package and the `bx` command line tool.
+
+`abacus-py` requires Python 3.10 or higher.
+
+## Minimal example
+
+A freshly created trading Klondike Trading Company (KTC) has recorded the following transactions.
+
+|     | Transaction Title                         |        Debit        |       Credit        | Amount |
+| --- | ----------------------------------------- | :-----------------: | :-----------------: | -----: |
+| 1   | Shareholders paid up capital contribution |        Cash         |       Equity        |   1000 |
+| 2   | Purchased goods for resale                |      Inventory      |        Cash         |    800 |
+| 3   | Invoiced client on sales contract         | Accounts Receivable |       Revenue       |    465 |
+| 4   | Provided discount to client               |      Discounts      | Accounts Receivable |     65 |
+| 5   | Recorded cost of sales                    |        COGS         |      Inventory      |    200 |
+| 6   | Paid salary to contract manager           |    SG&A Expenses    |        Cash         |    100 |
+| 7   | Accepted payment on sales contract        |        Cash         | Accounts Receivable |    360 |
+
+After closing accounts the company announced, but has not paid dividend.
+
+|     | Transaction Title                   |       Debit       |    Credit    | Amount |
+| --- | ----------------------------------- | :---------------: | :----------: | -----: |
+| \*  | Accrued dividend after announcement | Retained Earnings | Dividend Due |     50 |
+
+### 1. Chart
+
+Define a chart of accounts of five types (assets, equity, liabilities, income and expenses),
+specify retained earnings account name and, optionally, add contra accounts.
+
+```python
+from abacus import Chart
+
+chart = Chart(
+    assets=["cash", "ar", "goods"],
+    expenses=["cogs", "sga"],
+    equity=["equity"],
+    liabilities=["dividend_due"],
+    income=["sales"])
+chart = chart.set_retained_earnings("re").offset("sales", ["discounts"])
+```
+
+### 2. Ledger
+
+Create a general ledger based on the chart of accounts,
+post entries and close accounts at accounting period end.
+
+```python
+book = (chart.book()
+  .post(debit="cash", credit="equity", amount=1000)
+  .post(debit="goods", credit="cash", amount=800)
+  .post(debit="ar", credit="sales", amount=465)
+  .post(debit="discounts", credit="ar", amount=65)
+  .post(debit="cogs", credit="goods", amount=200)
+  .post(debit="sga", credit="cash", amount=100)
+  .post(debit="cash", credit="ar", amount=360)
+  .close()
+  .after_close(debit="re", credit="dividend_due", amount=50)
+)
+```
+
+### 3. Reports
+
+Make trail balance, income statement and balance sheet and save or print them to screen
+with verbose account names and rich text formatting.
+
+```python
+from abacus import RichViewer, PlainTextViewer
+
+income_statement = book.income_statement()
+balance_sheet = book.balance_sheet()
+rename_dict = {
+    "re": "Retained earnings",
+    "ar": "Accounts receivable",
+    "goods": "Inventory (goods for sale)",
+    "cogs": "Cost of goods sold",
+    "sga": "Selling, general and adm. expenses",
+}
+
+tv = PlainTextViewer(rename_dict)
+tv.print(balance_sheet)
+tv.print(income_statement)
+
+rv = RichViewer(rename_dict, width=80)
+rv.print(balance_sheet)
+rv.print(income_statement)
+```
+
+The output should look similar to text and a screenshot below.
+
+```
+Assets                        1100  Capital              1050
+- Cash                        460   - Equity             1000
+- Accounts receivable         40    - Retained earnings    50
+- Inventory (goods for sale)  600   Liabilities            50
+                                    - Dividend due         50
+Total                         1100  Total                1100
+
+Income                                400
+- Sales                               400
+Expenses                              300
+- Cost of goods sold                  200
+- Selling, general and adm. expenses  100
+Profit                                100
+```
+
+<details>
+<summary> Screenshot (outdated).
+</summary>
+
+![](https://user-images.githubusercontent.com/9265326/249445794-7def0fc2-934b-49fa-a3ad-9137072a2900.png)
+
+</details>
+
+<details>
+<summary> Details about correctness checks and end balances.
+</summary>
+
+### Check values
+
+As a reminder `assert` statement in Python will raise exception if provided wrong comparison.
+These checks will execute and this way we will know the code in README is up to date and correct.
+
+```python
+from abacus import IncomeStatement, BalanceSheet
+
+print(income_statement)
+assert income_statement == IncomeStatement(
+    income={'sales': 400},
+    expenses={'cogs': 200, 'sga': 100}
+)
+print(balance_sheet)
+assert balance_sheet == BalanceSheet(
+  assets={'cash': 460, 'ar': 40, 'goods': 600},
+  capital={'equity': 1000, 're': 50},
+  liabilities={'dividend_due': 50}
+)
+```
+
+### End balances
+
+You can use end balances from current period to initialize ledger at the start of next accounting period.
+
+```python
+end_balances = book.nonzero_balances()
+print(end_balances)
+next_book = chart.book(starting_balances=end_balances)
+```
+
+</details>
+
+## Command line
+
+Similar operations with chart, ledger and reports can be performed on the command line.
+
+### Create chart of accounts
+
+```bash
+bx erase --chart
+bx chart set --asset cash
+bx chart set --asset ar --title "Accounts receivable"
+bx chart set --asset goods --title "Inventory (good for sale)"
+bx chart set --capital equity
+bx chart set --retained-earnings re
+bx chart set --liability dividend_due
+bx chart set --income sales
+bx chart set --expense cogs --title "Cost of sales"
+bx chart set --expense sga --title "Selling expenses"
+bx chart offset sales discounts
+bx chart show
+```
+
+### Post entries to ledger and close
+
+```bash
+bx erase --ledger
+bx ledger start
+bx post entry --debit cash      --credit equity --amount 1000
+bx post entry --debit goods     --credit cash   --amount 800
+bx post entry --debit ar        --credit sales  --amount 465
+bx post entry --debit discounts --credit ar     --amount 65
+bx post entry --debit cogs      --credit goods  --amount 200
+bx post entry --debit sga       --credit cash   --amount 100
+bx post entry --debit cash      --credit ar     --amount 360
+bx ledger close
+bx post entry --debit re --credit dividend_due --amount 50 --after-close
+```
+
+### Report
+
+```bash
+bx report --balance-sheet
+bx report --income-statement
+```
+
+### Account information
+
+```bash
+bx account cash
+bx account ar
+bx account goods
+bx account sales
+bx accounts
+```
+
+You can save end balances to a file and initialize next period ledger.
+
+```bash
+bx accounts --json > end_balances.json
+```
+
+`assert` command will complain if account balance is not equal to provided value.
+This is useful for testing.
+
+```bash
+bx assert cash 460
+```
+
+## Feedback
+
+Anything missing in `abacus`?
+Got a good use case for `abacus` or used `abacus` for teaching?
+
+Feel free to contact `abacus` author
+in [issues](https://github.com/epogrebnyak/abacus/issues),
+on [reddit](https://www.reddit.com/user/iamevpo)
+or via [Telegram](https://t.me/epoepo).
+
+Your feedback is highly appreciated and helps steering development of `abacus`.
+
```

### Comparing `abacus_py-0.5.2/PKG-INFO` & `abacus_py-0.5.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-Metadata-Version: 2.1
-Name: abacus-py
-Version: 0.5.2
-Summary: A minimal, yet valid double-entry accounting system in Python.
-Author: Evgeniy Pogrebnyak
-Author-email: e.pogrebnyak@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: rich (>=13.3.5,<14.0.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
-Requires-Dist: types-docopt (>=0.6.11.3,<0.7.0.0)
-Description-Content-Type: text/markdown
-
 # abacus
 
 [![pytest](https://github.com/epogrebnyak/abacus/actions/workflows/.pytest.yml/badge.svg)](https://github.com/epogrebnyak/abacus/actions/workflows/.pytest.yml)
+![PyPI](https://img.shields.io/pypi/v/abacus-py?color=blue)
+
+A minimal, yet valid double-entry accounting system, provided as `abacus-py` Python package and `bx` command line tool.
 
-A minimal, yet valid double-entry accounting system, provided as a Python package and a command line tool.
+Using `abacus` you can define a chart of accounts, create a general ledger, post entries,
+close accounts properly at accounting period end and produce trial balance, balance sheet and income statement.
 
-Using `abacus` you can define a chart of accounts, create a general ledger, post
-entries, close accounts at period end and produce trial balance, balance sheet and income statement.
+The very minimal example of using `abacus` at command line is the following:
+
+```bash
+pip install abacus-py
+mkdir abacus_demo && cd abacus_demo
+bx erase --chart
+bx chart set --asset cash
+bx chart set --capital equity
+bx chart set --retained-earnings re
+bx ledger start
+bx post entry --title "Initial investment" --debit cash --credit equity --amount 5000
+bx ledger close
+bx report --balance-sheet
+```
+
+<!-- TODO: add corresponding Python code -->
 
 ## Documentation
 
 <https://epogrebnyak.github.io/abacus/>
 
 ## Quotes about `abacus`
 
@@ -42,18 +38,26 @@
 > I teach accounting information systems... I'd be tempted to use abacus as a way of simply showing the structure of a simple AIS.
 
 > Hey, what a cool job, thanks much. Do you plan to make a possibility for RAS accounting?
 
 ## Install
 
 ```
+pip install abacus-py
+```
+
+For latest version install from github:
+
+```
 pip install git+https://github.com/epogrebnyak/abacus.git
 ```
 
-This will install both `abacus` package and the `bx` command line tool.
+This will install both `abacus-py` package and the `bx` command line tool.
+
+`abacus-py` requires Python 3.10 or higher.
 
 ## Minimal example
 
 A freshly created trading Klondike Trading Company (KTC) has recorded the following transactions.
 
 |     | Transaction Title                         |        Debit        |       Credit        | Amount |
 | --- | ----------------------------------------- | :-----------------: | :-----------------: | -----: |
@@ -271,8 +275,7 @@
 
 Feel free to contact `abacus` author
 in [issues](https://github.com/epogrebnyak/abacus/issues),
 on [reddit](https://www.reddit.com/user/iamevpo)
 or via [Telegram](https://t.me/epoepo).
 
 Your feedback is highly appreciated and helps steering development of `abacus`.
-
```

