# Comparing `tmp/mms_monthly_cli-0.1.0.tar.gz` & `tmp/mms_monthly_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_monthly_cli-0.1.0.tar", max compression
+gzip compressed data, was "mms_monthly_cli-0.2.0.tar", max compression
```

## Comparing `mms_monthly_cli-0.1.0.tar` & `mms_monthly_cli-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    35150 2023-07-11 10:17:32.238486 mms_monthly_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0      916 2023-07-11 10:18:11.051323 mms_monthly_cli-0.1.0/README.md
--rw-r--r--   0        0        0     2177 2023-07-11 10:06:56.125696 mms_monthly_cli-0.1.0/mms_monthly_cli/cli.py
--rw-r--r--   0        0        0    11491 2023-07-11 08:34:42.398872 mms_monthly_cli-0.1.0/mms_monthly_cli/mms_monthly.py
--rw-r--r--   0        0        0      730 2023-07-11 10:02:22.906772 mms_monthly_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 mms_monthly_cli-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35150 2023-07-11 10:17:32.238486 mms_monthly_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6058 2023-07-13 05:56:46.657469 mms_monthly_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     2652 2023-07-13 05:56:46.657469 mms_monthly_cli-0.2.0/mms_monthly_cli/cli.py
+-rw-r--r--   0        0        0    12705 2023-07-13 05:56:46.657469 mms_monthly_cli-0.2.0/mms_monthly_cli/mms_monthly.py
+-rw-r--r--   0        0        0      730 2023-07-13 05:56:21.629262 mms_monthly_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6923 1970-01-01 00:00:00.000000 mms_monthly_cli-0.2.0/PKG-INFO
```

### Comparing `mms_monthly_cli-0.1.0/LICENSE` & `mms_monthly_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_monthly_cli-0.1.0/mms_monthly_cli/cli.py` & `mms_monthly_cli-0.2.0/mms_monthly_cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 
 import typer
 from rich import print
 from typing_extensions import Annotated
 
 from .mms_monthly import (
+    _validate_data_dir,
     get_and_unzip_table_csv,
     get_available_tables,
     get_years_and_months,
 )
 
 app = typer.Typer(
     no_args_is_help=True,
@@ -41,32 +42,49 @@
     """
     Displays years and the months within them for which data is available
     """
     print(get_years_and_months())
 
 
 @app.command(no_args_is_help=True)
-def available_tables(year: int, month: int):
+def available_tables(
+    year: int,
+    month: int,
+    data_dir: Annotated[
+        str,
+        typer.Argument(
+            help=("NEMWeb data directory to look at. Default is `DATA`."),
+        ),
+    ] = "DATA",
+):
     """
     Displays available tables for a period (i.e. supplied month and year)
     """
-    print(get_available_tables(year, month))
+    _validate_data_dir(year, month, data_dir)
+    print(get_available_tables(year, month, data_dir))
 
 
 @app.command(no_args_is_help=True)
 def get_table(
     year: int,
     month: int,
     table: str,
     cache: Annotated[
         Path,
         typer.Argument(
             help="Directory to save data to. If it does not exist, it will be created"
         ),
     ],
+    data_dir: Annotated[
+        str,
+        typer.Argument(
+            help=("NEMWeb data directory to look at. Default is `DATA`."),
+        ),
+    ] = "DATA",
 ):
     """
     Download and unzip monthly data zip file to get data table CSV in cache.
     To see available periods, use the `available_periods` command
     To see available tables for a given period, use the `available_tables` command
     """
-    get_and_unzip_table_csv(year, month, table, cache)
+    _validate_data_dir(year, month, data_dir)
+    get_and_unzip_table_csv(year, month, data_dir, table, cache)
```

### Comparing `mms_monthly_cli-0.1.0/mms_monthly_cli/mms_monthly.py` & `mms_monthly_cli-0.2.0/mms_monthly_cli/mms_monthly.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,31 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 import shutil
 from pathlib import Path
 from re import match
-from typing import Dict, List
+from typing import Dict, List, Union
 from zipfile import BadZipFile, ZipFile
 
 import requests
 from bs4 import BeautifulSoup
 from tqdm.auto import tqdm
 from user_agent import generate_user_agent
 
 logger = logging.getLogger(__name__)
 
 # Data
 
 MMSDM_ARCHIVE_URL = "http://www.nemweb.com.au/Data_Archive/Wholesale_Electricity/MMSDM/"
 """Wholesale electricity data archive base URL"""
 
+# Decorator function to
+
 # Functions to handle requests and scraped soup
 
 
 def _build_nemweb_get_header(useragent: str) -> Dict[str, str]:
     """Builds request header for GET requests from NEMWeb
 
     Args:
@@ -101,29 +103,32 @@
         else:
             logging.info("Relaunching request")
             useragent = generate_user_agent()
     soup = BeautifulSoup(r.content, "html.parser")
     return soup
 
 
-def _get_all_links_from_soup(year: int, month) -> List[str]:
+def _get_all_links_from_soup(
+    year: int, month: int, data_dir: Union[str, None]
+) -> List[str]:
     """Gets all links from scraped Data Archive year-month URL
     Args:
         year: Year
         month: Month
+        data_dir : Directory within monthly archives, or None
     Returns:
         All scraped links
     """
     available_years_and_months = get_years_and_months()
     if (
         year not in available_years_and_months.keys()
         or month not in available_years_and_months[year]
     ):
         raise ValueError(f"Monthly Data Archive does not have data for {month}/{year}")
-    url = _construct_yearmonth_url(year, month)
+    url = _construct_yearmonth_url(year, month, data_dir)
     soup = _rerequest_to_obtain_soup(url)
     links = [link.get("href") for link in soup.find_all("a")]
     return links
 
 
 # Functions to construct filenames and URLs
 
@@ -140,43 +145,46 @@
     """
     (stryear, strmonth) = (str(year), str(month).rjust(2, "0"))
     prefix = f"PUBLIC_DVD_{table}"
     fn = prefix + f"_{stryear}{strmonth}010000"
     return fn
 
 
-def _construct_yearmonth_url(year: int, month: int) -> str:
+def _construct_yearmonth_url(year: int, month: int, data_dir: Union[str, None]) -> str:
     """Constructs URL that points to a MMSDM Historical Data Archive zip file
 
     Args:
         year: Year
         month: Month
+        data_dir : Directory within monthly archives, or None
     Returns:
         URL to zip file
     """
     url = (
         MMSDM_ARCHIVE_URL
         + f"{year}/MMSDM_{year}_"
         + f'{str(month).rjust(2, "0")}/MMSDM_Historical_Data_SQLLoader/'
-        + "DATA/"
     )
+    if data_dir is not None:
+        url += data_dir + "/"
     return url
 
 
-def _construct_table_url(year: int, month: int, table: str) -> str:
+def _construct_table_url(year: int, month: int, data_dir: str, table: str) -> str:
     """Constructs URL that points to a MMSDM Historical Data Archive zip file
 
     Args:
         year: Year
         month: Month
+        data_dir : Directory within monthly archives
         table: Table of interest
     Returns:
         URL to zip file
     """
-    data_url = _construct_yearmonth_url(year, month)
+    data_url = _construct_yearmonth_url(year, month, data_dir)
     fn = _construct_filename(year, month, table)
     url = data_url + fn + ".zip"
     return url
 
 
 # Functions to obtain table properties
 
@@ -190,36 +198,59 @@
         File size in bytes
     """
     h = requests.head(url, headers=_build_nemweb_get_header(generate_user_agent()))
     total_length = int(h.headers.get("Content-Length", 0))
     return total_length
 
 
-def _get_table_names(year: int, month: int, regex: str) -> List[str]:
+def _get_table_names(year: int, month: int, data_dir: str, regex: str) -> List[str]:
     """Returns table names from MMSDM Historical Data Archive page
 
     For a year and month in the MMSDM Historical Data Archive, returns a list of
     table names (obtained via captured regex group)
 
     Args:
         year: Year
         month: Month
+        data_dir : Directory within monthly archives
         regex: Regular expression pattern, with one group capture
     Returns:
         List of table names
     """
     names = []
-    links = _get_all_links_from_soup(year, month)
+    links = _get_all_links_from_soup(year, month, data_dir)
     for link in links:
         if mo := match(regex, link):
             name = mo.group(1).lstrip("_")
             names.append(name)
     return list(set(names))
 
 
+# Validator functions
+
+
+def _validate_data_dir(year: int, month: int, data_dir: str) -> None:
+    """Validates user `data_dir` specification
+
+    Args:
+        year: Year
+        month: Month
+        data_dir : Directory within monthly archives
+    Errors:
+        ValueError: If `data_dir` does not exist
+    """
+    links = _get_all_links_from_soup(year, month, None)
+    links = [Path(link).name for link in links]
+    if data_dir not in links:
+        raise ValueError(
+            f"{data_dir} not in Monthly Data Archive for {year} {month}. "
+            + f"Possible dirs: {links}"
+        )
+
+
 # Main functions to find available data, or to obtain data
 
 
 def get_years_and_months() -> Dict[int, List[int]]:
     """Years and months with data on NEMWeb MMSDM Historical Data Archive
     Returns:
         Months mapped to each year. Data is available for each of these months.
@@ -259,86 +290,87 @@
         else:
             year = int(findyear.group(1))
             months = _get_months(MMSDM_ARCHIVE_URL + f"{year}/")
             yearmonths[year] = months
     return yearmonths
 
 
-def get_available_tables(
-    year: int,
-    month: int,
-) -> List[str]:
+def get_available_tables(year: int, month: int, data_dir: str) -> List[str]:
     """Tables that can be requested from MMSDM Historical Data Archive for a
        particular month and year.
     Args:
         year: Year
         month: Month
+        data_dir : Directory within monthly archives
 
     Returns:
         List of tables associated with that forecast type for that period
     """
     table_regex = ".*/PUBLIC_DVD_([A-Z_0-9]*)_[0-9]*.zip"
-    names = _get_table_names(year, month, table_regex)
+    names = _get_table_names(year, month, data_dir, table_regex)
     return sorted(names)
 
 
-def get_table_names_and_sizes(year: int, month: int) -> Dict:
+def get_table_names_and_sizes(year: int, month: int, data_dir: str) -> Dict:
     """Returns table names and sizes from MMSDM Historical Data Archive page
 
     For a year and month in the MMSDM Historical Data Archive, returns a list of
     tuples each consisting of:
     - A table name (obtained via captured regex group)
     - The size of the associated zip file
 
     Args:
         year: Year
         month: Month
-        regex: Regular expression pattern, with one group capture
+        data_dir : Directory within monthly archives
     Returns:
         Tuple of table names and file sizes
     """
     regex = ".*/PUBLIC_DVD_([A-Z_0-9]*)_[0-9]*.zip"
     names_and_sizes = []
-    links = _get_all_links_from_soup(year, month)
+    links = _get_all_links_from_soup(year, month, data_dir)
     for link in links:
         if mo := match(regex, link):
             name = mo.group(1).lstrip("_")
-            table_url = _construct_table_url(year, month, name)
+            table_url = _construct_table_url(year, month, data_dir, name)
             size = _get_filesize(table_url)
             names_and_sizes.append((name, size))
     names_and_size = list(set(names_and_sizes))
     name_size_dict = {}
     for name, size in names_and_size:
         name_size_dict[name] = size
     return name_size_dict
 
 
-def get_and_unzip_table_csv(year: int, month: int, table: str, cache: Path) -> None:
+def get_and_unzip_table_csv(
+    year: int, month: int, data_dir: str, table: str, cache: Path
+) -> None:
     """Unzipped (single) csv file downloaded from `url` to `cache`
 
     This function:
 
     1. Downloads zip file in chunks to limit memory use and enable progress bar
     2. Validates that the zip contains a single file that has the same name as the zip
 
     Args:
         year: Year
         month: Month
+        data_dir : Directory within monthly archives
         table: Table name
         cache: Path to save zip.
     Returns:
         None. Extracts csv to `cache`
     """
-    available_tables = get_available_tables(year, month)
+    available_tables = get_available_tables(year, month, data_dir)
     if table not in available_tables:
         raise ValueError(f"Table not in available tables for {month}/{year}")
     if not (cache_path := Path(cache)).exists():
         cache_path.mkdir(parents=True)
     header = _build_nemweb_get_header(generate_user_agent())
-    url = _construct_table_url(year, month, table)
+    url = _construct_table_url(year, month, data_dir, table)
     file_name = Path(url).name
     file_path = cache / Path(file_name)
     with requests.get(url, headers=header, stream=True) as resp:
         total_length = int(resp.headers.get("Content-Length", 0))
         resp.raise_for_status()
         with tqdm.wrapattr(resp.raw, "read", desc=file_name, total=total_length) as raw:
             with open(file_path, "wb") as fout:
```

### Comparing `mms_monthly_cli-0.1.0/pyproject.toml` & `mms_monthly_cli-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms-monthly-cli"
-version = "0.1.0"
+version = "0.2.0"
 description = "A package and CLI utility to check for available data and download tables from AEMO's Monthly Data Archive"
 authors = ["prakaa <abiprakash007@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "mms_monthly_cli"}]
 
 [tool.poetry.scripts]
```

