# Comparing `tmp/quantflow-0.2.1.tar.gz` & `tmp/quantflow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantflow-0.2.1.tar", max compression
+gzip compressed data, was "quantflow-0.2.2.tar", max compression
```

## Comparing `quantflow-0.2.1.tar` & `quantflow-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,37 @@
--rw-r--r--   0        0        0     1461 2023-07-07 14:53:44.773527 quantflow-0.2.1/LICENSE
--rw-r--r--   0        0        0     1779 2023-07-07 14:53:44.777526 quantflow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/data/__init__.py
--rw-r--r--   0        0        0     2840 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/data/client.py
--rw-r--r--   0        0        0     5329 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/data/fmp.py
--rw-r--r--   0        0        0      146 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/data/utils.py
--rw-r--r--   0        0        0        0 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/options/__init__.py
--rw-r--r--   0        0        0     1675 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/options/bs.py
--rw-r--r--   0        0        0     1021 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/options/inputs.py
--rw-r--r--   0        0        0    16213 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/options/surface.py
--rw-r--r--   0        0        0        0 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/py.typed
--rw-r--r--   0        0        0        0 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/__init__.py
--rwxr-xr-x   0        0        0     9896 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/base.py
--rwxr-xr-x   0        0        0    11076 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/cached.py
--rwxr-xr-x   0        0        0     4744 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/cir.py
--rwxr-xr-x   0        0        0     5131 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/combined.py
--rwxr-xr-x   0        0        0     3174 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/copula.py
--rwxr-xr-x   0        0        0     3302 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/derived.py
--rwxr-xr-x   0        0        0     1867 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/dsp.py
--rw-r--r--   0        0        0     1879 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/heston.py
--rwxr-xr-x   0        0        0     3180 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/ou.py
--rwxr-xr-x   0        0        0     7683 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/poisson.py
--rwxr-xr-x   0        0        0     3648 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/weibull.py
--rw-r--r--   0        0        0     1719 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/sp/weiner.py
--rw-r--r--   0        0        0        0 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/utils/__init__.py
--rw-r--r--   0        0        0      894 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/utils/bins.py
--rwxr-xr-x   0        0        0      496 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/utils/functions.py
--rw-r--r--   0        0        0     1265 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/utils/interest_rates.py
--rw-r--r--   0        0        0       48 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/utils/kalman.py
--rw-r--r--   0        0        0     3979 2023-07-07 14:53:44.777526 quantflow-0.2.1/quantflow/utils/marginal.py
--rw-r--r--   0        0        0      221 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/numbers.py
--rwxr-xr-x   0        0        0     1438 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/paths.py
--rw-r--r--   0        0        0      825 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/plot.py
--rw-r--r--   0        0        0     1097 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/text.py
--rw-r--r--   0        0        0     3642 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/transforms.py
--rw-r--r--   0        0        0      622 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/types.py
--rw-r--r--   0        0        0     2091 2023-07-07 14:53:44.781527 quantflow-0.2.1/quantflow/utils/volatility.py
--rw-r--r--   0        0        0      920 2023-07-07 14:53:44.781527 quantflow-0.2.1/readme.md
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 quantflow-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-07-13 08:54:47.392163 quantflow-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1813 2023-07-13 08:54:47.396163 quantflow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/data/__init__.py
+-rw-r--r--   0        0        0     2840 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/data/client.py
+-rw-r--r--   0        0        0     5374 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/data/fmp.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/__init__.py
+-rw-r--r--   0        0        0     2032 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/bs.py
+-rw-r--r--   0        0        0     7301 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/calibration.py
+-rw-r--r--   0        0        0     1021 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/inputs.py
+-rw-r--r--   0        0        0     4389 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/pricer.py
+-rw-r--r--   0        0        0    19846 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/options/surface.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/py.typed
+-rw-r--r--   0        0        0        0 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/__init__.py
+-rwxr-xr-x   0        0        0     4580 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/base.py
+-rw-r--r--   0        0        0     2448 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/bns.py
+-rwxr-xr-x   0        0        0     5500 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/cir.py
+-rwxr-xr-x   0        0        0     2054 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/dsp.py
+-rw-r--r--   0        0        0     2576 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/heston.py
+-rwxr-xr-x   0        0        0     4771 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/ou.py
+-rwxr-xr-x   0        0        0     5921 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/poisson.py
+-rw-r--r--   0        0        0     1531 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/weiner.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/__init__.py
+-rw-r--r--   0        0        0      894 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/bins.py
+-rw-r--r--   0        0        0      252 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/dates.py
+-rw-r--r--   0        0        0      975 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/distributions.py
+-rwxr-xr-x   0        0        0      496 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/functions.py
+-rw-r--r--   0        0        0     1265 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/interest_rates.py
+-rw-r--r--   0        0        0     9347 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/marginal.py
+-rw-r--r--   0        0        0      370 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/numbers.py
+-rwxr-xr-x   0        0        0     2698 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/paths.py
+-rw-r--r--   0        0        0     3411 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/plot.py
+-rw-r--r--   0        0        0     4884 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/transforms.py
+-rw-r--r--   0        0        0      721 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/types.py
+-rw-r--r--   0        0        0     2091 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/volatility.py
+-rw-r--r--   0        0        0     1179 2023-07-13 08:54:47.400163 quantflow-0.2.2/readme.md
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 quantflow-0.2.2/PKG-INFO
```

### Comparing `quantflow-0.2.1/LICENSE` & `quantflow-0.2.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Quantmind
+Copyright (c) 2023 Quantmind
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `quantflow-0.2.1/pyproject.toml` & `quantflow-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantflow"
-version = "0.2.1"
+version = "0.2.2"
 description = "quantitative analysis"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD-3-Clause"
 readme = "readme.md"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/quantmind/quantflow"
@@ -21,37 +21,40 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.4.0"
 ghp-import = "^2.0.2"
 ruff = "^0.0.277"
+pytest-asyncio = "^0.21.1"
 
 [tool.poetry.extras]
 data = ["aiohttp"]
 
 [tool.poetry.group.book]
 optional = true
 
 [tool.poetry.group.book.dependencies]
 jupyter-book = "^0.15.1"
 nbconvert = "^6.4.5"
 jupytext = "^1.13.8"
 plotly = "^5.7.0"
 jupyterlab = "^4.0.2"
+sympy = "^1.12"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.jupytext]
 formats = "ipynb,myst"
 
 [tool.pytest.ini_options]
+asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.isort]
 profile = "black"
 
@@ -64,28 +67,27 @@
 path = "quantflow/__init__.py"
 
 [tool.mypy]
 # strict = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 warn_no_return = true
-exclude = [
-    "quantflow/sp/cached.py",
-    "quantflow/sp/combined.py",
-    "quantflow/sp/derived.py"
-]
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
 module = "IPython.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "pandas.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = "plotly.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 module = "scipy.*"
 ignore_missing_imports = true
```

### Comparing `quantflow-0.2.1/quantflow/data/client.py` & `quantflow-0.2.2/quantflow/data/client.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.1/quantflow/data/fmp.py` & `quantflow-0.2.2/quantflow/data/fmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 from datetime import date, timedelta
 from typing import Any, cast
 
 import pandas as pd
 
 from .client import HttpClient, compact
-from .utils import isoformat
+from ..utils.dates import isoformat
 
 
 class FMP(HttpClient):
-    url: str = "https://financialmodelingprep.com/api"
-
     def __init__(
         self,
+        *,
+        url: str = "https://financialmodelingprep.com/api",
         key: str = "",
     ) -> None:
+        self.url = url
         self.key = key or os.environ.get("FMP_API_KEY")
 
     async def stocks(self, **kw: Any) -> list[dict]:
         return await self.get_path("v3/stock/list", **kw)
 
     async def etfs(self, **kw: Any) -> list[dict]:
         return await self.get_path("v3/etf/list", **kw)
```

### Comparing `quantflow-0.2.1/quantflow/options/inputs.py` & `quantflow-0.2.2/quantflow/options/inputs.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.1/quantflow/options/surface.py` & `quantflow-0.2.2/quantflow/options/surface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
 
+import enum
 from dataclasses import dataclass, field
-from datetime import datetime, timezone
+from datetime import datetime, timedelta
 from decimal import Decimal
 from typing import Any, Generic, Iterator, NamedTuple, Protocol, TypeVar
 
 import numpy as np
 import pandas as pd
 
 from quantflow.utils import plot
 from quantflow.utils.interest_rates import rate_from_spot_and_forward
 
-from .bs import black_price, implied_black_volatility_full_result
+from ..utils.dates import utcnow
+from ..utils.numbers import Number, sigfig, to_decimal
+from .bs import black_price, implied_black_volatility
 from .inputs import (
     ForwardInput,
     OptionInput,
     OptionSidesInput,
     SpotInput,
     VolSecurityType,
     VolSurfaceInput,
@@ -35,14 +38,25 @@
 
 
 def time_to_maturity(maturity: datetime, ref_date: datetime) -> float:
     delta = maturity - ref_date
     return (delta.days + delta.seconds / 86400) / 365
 
 
+class OptionSelection(enum.Enum):
+    """Option selection method"""
+
+    best = enum.auto()
+    """Select the best bid/ask options - the ones which are otm"""
+    call = enum.auto()
+    """Select the call options"""
+    put = enum.auto()
+    """Select the put options"""
+
+
 @dataclass
 class Price(Generic[S]):
     security: S
     bid: Decimal
     ask: Decimal
 
     @property
@@ -85,14 +99,38 @@
     ttm: float = 0
     """Time to maturity in years"""
     side: str = "bid"
     """Side of the market"""
     converged: bool = True
     """Flag indicating if implied vol calculation converged"""
 
+    @classmethod
+    def create(
+        cls,
+        strike: Number,
+        *,
+        price: Number = ZERO,
+        implied_vol: float = INITIAL_VOL,
+        forward: Number | None = None,
+        ref_date: datetime | None = None,
+        maturity: datetime | None = None,
+        call: bool = True,
+    ) -> OptionPrice:
+        ref_date = ref_date or utcnow()
+        maturity = maturity or ref_date + timedelta(days=365)
+        return cls(
+            price=to_decimal(price),
+            strike=to_decimal(strike),
+            forward=to_decimal(forward or strike),
+            implied_vol=implied_vol,
+            call=call,
+            maturity=maturity,
+            ttm=time_to_maturity(maturity, ref_date),
+        )
+
     @property
     def moneyness(self) -> float:
         return float(np.log(float(self.strike / self.forward)))
 
     @property
     def price_bp(self) -> Decimal:
         return self.price * 10000
@@ -108,32 +146,73 @@
         else:
             return max(self.strike - self.forward, ZERO) / self.forward
 
     @property
     def price_time(self) -> Decimal:
         return self.price - self.price_intrinsic
 
-    def can_price(self, converged: bool) -> bool:
-        if self.price_time > ZERO:
-            return self.converged if converged else True
+    @property
+    def call_price(self) -> Decimal:
+        """call price
+
+        use put-call parity to calculate the call price if a put
+        """
+        if self.call:
+            return self.price
+        else:
+            return self.price + 1 - self.strike / self.forward
+
+    @property
+    def put_price(self) -> Decimal:
+        """put price
+
+        use put-call parity to calculate the put price if a call
+        """
+        if self.call:
+            return self.price - 1 + self.strike / self.forward
+        else:
+            return self.price
+
+    def can_price(self, converged: bool, select: OptionSelection) -> bool:
+        if self.price_time > ZERO and not np.isnan(self.implied_vol):
+            if not self.converged and converged is True:
+                return False
+            if select == OptionSelection.best:
+                return self.price_intrinsic == ZERO
+            return True
         return False
 
     def inputs(self) -> OptionInput:
         return OptionInput(
             strike=self.strike,
             price=self.price,
             maturity=self.maturity,
             call=self.call,
         )
 
+    def calculate_price(self) -> OptionPrice:
+        self.price = Decimal(
+            sigfig(
+                black_price(
+                    np.asarray(self.moneyness),
+                    self.implied_vol,
+                    self.ttm,
+                    1 if self.call else -1,
+                ).sum(),
+                8,
+            )
+        )
+        return self
+
     def _asdict(self) -> dict[str, Any]:
         return dict(
             strike=float(self.strike),
             forward=float(self.forward),
             moneyness=self.moneyness,
+            moneyness_ttm=self.moneyness / np.sqrt(self.ttm),
             ttm=self.ttm,
             implied_vol=self.implied_vol,
             price=float(self.price),
             price_bp=float(self.price_bp),
             forward_price=float(self.forward_price),
             call=self.call,
             side=self.side,
@@ -142,35 +221,38 @@
 
 class OptionArrays(NamedTuple):
     options: list[OptionPrice]
     moneyness: np.ndarray
     price: np.ndarray
     ttm: np.ndarray
     implied_vol: np.ndarray
+    call_put: np.ndarray
 
 
 @dataclass
 class OptionPrices(Generic[S]):
     security: S
     bid: OptionPrice
     ask: OptionPrice
 
     def prices(
         self,
         forward: Decimal,
         ttm: float,
-        initial_vol: float,
+        *,
+        select: OptionSelection = OptionSelection.best,
+        initial_vol: float = INITIAL_VOL,
         converged: bool = True,
     ) -> Iterator[OptionPrice]:
         for o in (self.bid, self.ask):
             o.forward = forward
             o.ttm = ttm
             if not o.implied_vol:
                 o.implied_vol = initial_vol
-            if o.can_price(converged):
+            if o.can_price(converged, select):
                 yield o
 
     def inputs(self) -> OptionSidesInput:
         return OptionSidesInput(
             bid=self.bid.inputs(),
             ask=self.ask.inputs(),
         )
@@ -182,56 +264,73 @@
     call: OptionPrices[S] | None = None
     put: OptionPrices[S] | None = None
 
     def option_prices(
         self,
         forward: Decimal,
         ttm: float,
-        call: bool = True,
+        *,
+        select: OptionSelection = OptionSelection.best,
         initial_vol: float = INITIAL_VOL,
         converged: bool = True,
     ) -> Iterator[OptionPrice]:
-        if call and self.call:
-            yield from self.call.prices(forward, ttm, initial_vol, converged)
-        if not call and self.put:
-            yield from self.put.prices(forward, ttm, initial_vol, converged)
+        if select != OptionSelection.put and self.call:
+            yield from self.call.prices(
+                forward,
+                ttm,
+                select=select,
+                initial_vol=initial_vol,
+                converged=converged,
+            )
+        if select != OptionSelection.call and self.put:
+            yield from self.put.prices(
+                forward,
+                ttm,
+                select=select,
+                initial_vol=initial_vol,
+                converged=converged,
+            )
 
 
 @dataclass
 class VolCrossSection(Generic[S]):
     maturity: datetime
     forward: FwdPrice[S]
     """Forward price of the underlying asset at the time of the cross section"""
     strikes: tuple[Strike[S], ...]
     """Tuple of sorted strikes and their corresponding option prices"""
 
+    def ttm(self, ref_date: datetime) -> float:
+        return time_to_maturity(self.maturity, ref_date)
+
     def info_dict(self, ref_date: datetime, spot: SpotPrice[S]) -> dict:
         return dict(
             maturity=self.maturity,
-            ttm=time_to_maturity(self.maturity, ref_date),
+            ttm=self.ttm(ref_date),
             forward=self.forward.mid,
             basis=self.forward.mid - spot.mid,
             rate_percent=rate_from_spot_and_forward(
                 spot.mid, self.forward.mid, self.maturity - ref_date
             ).percent,
         )
 
     def option_prices(
         self,
         ref_date: datetime,
-        call: bool = True,
+        *,
+        select: OptionSelection = OptionSelection.best,
         initial_vol: float = INITIAL_VOL,
         converged: bool = True,
     ) -> Iterator[OptionPrice]:
         ttm = time_to_maturity(self.maturity, ref_date)
         for s in self.strikes:
             yield from s.option_prices(
                 self.forward.mid,
                 ttm,
-                call,
+                select=select,
                 initial_vol=initial_vol,
                 converged=converged,
             )
 
     def securities(self) -> Iterator[FwdPrice[S] | OptionPrices[S]]:
         """Return a list of all securities in the cross section"""
         yield self.forward
@@ -263,127 +362,151 @@
         return pd.DataFrame(
             cross.info_dict(self.ref_date, self.spot) for cross in self.maturities
         )
 
     def option_prices(
         self,
         *,
-        call: bool = True,
+        select: OptionSelection = OptionSelection.best,
         index: int | None = None,
         initial_vol: float = INITIAL_VOL,
         converged: bool = True,
     ) -> Iterator[OptionPrice]:
-        "Iterator over all option prices in the surface"
+        "Iterator over selected option prices in the surface"
         if index is not None:
             yield from self.maturities[index].option_prices(
-                self.ref_date, call=call, initial_vol=initial_vol, converged=converged
+                self.ref_date,
+                select=select,
+                initial_vol=initial_vol,
+                converged=converged,
             )
         else:
             for maturity in self.maturities:
                 yield from maturity.option_prices(
                     self.ref_date,
-                    call=call,
+                    select=select,
                     initial_vol=initial_vol,
                     converged=converged,
                 )
 
     def option_list(
         self,
         *,
-        call: bool = True,
+        select: OptionSelection = OptionSelection.best,
         index: int | None = None,
         converged: bool = True,
     ) -> list[OptionPrice]:
         "List of all option prices in the surface"
-        return list(self.option_prices(call=call, index=index, converged=converged))
+        return list(self.option_prices(select=select, index=index, converged=converged))
 
     def bs(
         self,
         *,
-        call: bool = True,
+        select: OptionSelection = OptionSelection.best,
         index: int | None = None,
         initial_vol: float = INITIAL_VOL,
     ) -> list[OptionPrice]:
         """calculate Black-Scholes implied volatilities for all options
         in the surface"""
         d = self.as_array(
-            call=call, index=index, initial_vol=initial_vol, converged=False
+            select=select, index=index, initial_vol=initial_vol, converged=False
         )
-        result = implied_black_volatility_full_result(
+        result = implied_black_volatility(
             k=d.moneyness,
             price=d.price,
             ttm=d.ttm,
             initial_sigma=d.implied_vol,
+            call_put=d.call_put,
         )
         for option, implied_vol, converged in zip(
             d.options, result.root, result.converged
         ):
             option.implied_vol = float(implied_vol)
             option.converged = converged
         return d.options
 
     def calc_bs_prices(
-        self, *, call: bool = True, index: int | None = None
+        self,
+        *,
+        select: OptionSelection = OptionSelection.best,
+        index: int | None = None,
     ) -> np.ndarray:
         """calculate Black-Scholes prices for all options in the surface"""
-        d = self.as_array(call=call, index=index)
-        return black_price(k=d.moneyness, sigma=d.implied_vol, ttm=d.ttm)
+        d = self.as_array(select=select, index=index)
+        return black_price(k=d.moneyness, sigma=d.implied_vol, ttm=d.ttm, s=d.call_put)
 
     def options_df(
         self,
         *,
-        call: bool = True,
+        select: OptionSelection = OptionSelection.best,
         index: int | None = None,
         initial_vol: float = INITIAL_VOL,
         converged: bool = True,
     ) -> pd.DataFrame:
         """Time frame of Black-Scholes call input data"""
         data = self.option_prices(
-            call=call, index=index, initial_vol=initial_vol, converged=converged
+            select=select, index=index, initial_vol=initial_vol, converged=converged
         )
         return pd.DataFrame([d._asdict() for d in data])
 
     def as_array(
         self,
         *,
-        call: bool = True,
+        select: OptionSelection = OptionSelection.best,
         index: int | None = None,
         initial_vol: float = INITIAL_VOL,
         converged: bool = True,
     ) -> OptionArrays:
         """Organize option prices in a numpy arrays for black volatility calculation"""
         options = list(
             self.option_prices(
-                call=call, index=index, initial_vol=initial_vol, converged=converged
+                select=select, index=index, initial_vol=initial_vol, converged=converged
             )
         )
         moneyness = []
         ttm = []
         price = []
         vol = []
+        call_put = []
         for option in options:
             moneyness.append(float(option.moneyness))
             price.append(float(option.price))
             ttm.append(float(option.ttm))
             vol.append(float(option.implied_vol))
+            call_put.append(1 if option.call else -1)
         return OptionArrays(
             options=options,
             moneyness=np.array(moneyness),
             price=np.array(price),
             ttm=np.array(ttm),
             implied_vol=np.array(vol),
+            call_put=np.array(call_put),
         )
 
     def plot(
-        self, *, index: int | None = None, call: bool = True, **kwargs: Any
+        self,
+        *,
+        index: int | None = None,
+        select: OptionSelection = OptionSelection.best,
+        **kwargs: Any,
     ) -> Any:
         """Plot the volatility surface"""
-        df = self.options_df(index=index, call=call)
+        df = self.options_df(index=index, select=select)
         return plot.plot_vol_surface(df, **kwargs)
 
+    def plot3d(
+        self,
+        *,
+        select: OptionSelection = OptionSelection.best,
+        **kwargs: Any,
+    ) -> Any:
+        """Plot the volatility surface"""
+        df = self.options_df(select=select)
+        return plot.plot_vol_surface_3d(df, **kwargs)
+
 
 @dataclass
 class VolCrossSectionLoader(Generic[S]):
     maturity: datetime
     forward: FwdPrice[S] | None = None
     """Forward price of the underlying asset at the time of the cross section"""
     strikes: dict[Decimal, Strike[S]] = field(default_factory=dict)
@@ -477,15 +600,15 @@
         if not self.spot or self.spot.mid == ZERO:
             raise ValueError("No spot price provided")
         maturities = []
         for maturity in sorted(self.maturities):
             if section := self.maturities[maturity].cross_section():
                 maturities.append(section)
         return VolSurface(
-            ref_date=ref_date or datetime.utcnow().replace(tzinfo=timezone.utc),
+            ref_date=ref_date or utcnow(),
             spot=self.spot,
             maturities=tuple(maturities),
         )
 
 
 class VolSurfaceLoader(GenericVolSurfaceLoader[VolSecurityType]):
     def add(self, input: VolSurfaceInput[Any]) -> None:
```

### Comparing `quantflow-0.2.1/quantflow/sp/cir.py` & `quantflow-0.2.2/quantflow/sp/cir.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import enum
 
 import numpy as np
-from numpy.random import normal
 from pydantic import Field
 from scipy import special
+from scipy.optimize import Bounds
 
 from quantflow.utils.types import Vector
 
-from .base import Im, IntensityProcess
+from ..utils.paths import Paths
+from .base import Im, IntensityProcess, StochasticProcess1DMarginal
 
 
 class SamplingAlgorithm(str, enum.Enum):
     euler = "euler"
+    milstein = "milstein"
     implicit = "implicit"
 
 
 class CIR(IntensityProcess):
     r"""The Cox–Ingersoll–Ross (CIR) model is a mean-reverting square-root diffusion
     process.
 
@@ -34,110 +36,129 @@
     :param kappa: Mean reversion speed :math:`\kappa`
     :param sigma: Volatility parameter :math:`\sigma`
     :param theta: Long term mean rate :math:`\theta`
     """
     sigma: float = Field(default=1.0, gt=0, description="Volatility")
     theta: float = Field(default=1.0, gt=0, description="Mean rate")
     sample_algo: SamplingAlgorithm = Field(
-        default=SamplingAlgorithm.implicit, description="Sampling algorithm", repr=False
+        default=SamplingAlgorithm.implicit, description="Sampling algorithm"
     )
 
     @property
     def is_positive(self) -> bool:
-        return self.kappa * self.theta >= 0.5 * self.sigma * self.sigma
+        return self.kappa * self.theta >= 0.5 * self.sigma2
 
-    def pdf(self, t: float, x: Vector) -> Vector:
-        k = self.kappa
-        s2 = self.sigma * self.sigma
-        ekt = np.exp(-k * t)
-        c = 2 * k / (1 - ekt) / s2
-        q = 2 * k * self.theta / s2 - 1
-        u = c * ekt * self.rate
-        v = c * x
-        return (
-            c
-            * np.exp(-v - u)
-            * np.power(v / u, 0.5 * q)
-            * special.iv(q, 2 * np.sqrt(u * v))
-        )
-
-    def mean(self, t: float) -> float:
-        ekt = np.exp(-self.kappa * t)
-        return self.rate * ekt + self.theta * (1 - ekt)
+    @property
+    def sigma2(self) -> float:
+        return self.sigma * self.sigma
 
-    def std(self, t: float) -> float:
-        kappa = self.kappa
-        ekt = np.exp(-kappa * t)
-        return np.sqrt(
-            self.sigma
-            * self.sigma
-            * (1 - ekt)
-            * (self.rate * ekt + 0.5 * self.theta * (1 - ekt))
-            / kappa
-        )
+    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
+        return CIRMarginal(process=self, t=t)
 
-    def sample(self, n: int, t: float = 1, steps: int = 0) -> np.ndarray:
-        if self.sample_algo == SamplingAlgorithm.euler:
-            return self.sample_euler(n, t, steps)
-        else:
-            return self.sample_implicit(n, t, steps)
+    def sample(
+        self, paths: int, time_horizon: float = 1, time_steps: int = 100
+    ) -> Paths:
+        draws = Paths.normal_draws(paths, time_horizon, time_steps)
+        return self.sample_from_draws(draws)
+
+    def sample_from_draws(self, paths: Paths, *args: Paths) -> Paths:
+        match self.sample_algo:
+            case SamplingAlgorithm.euler:
+                return self.sample_euler(paths)
+            case SamplingAlgorithm.milstein:
+                return self.sample_euler(paths, 0.25)
+            case SamplingAlgorithm.implicit:
+                return self.sample_implicit(paths)
 
-    def sample_euler(self, n: int, t: float = 1, steps: int = 0) -> np.ndarray:
-        size, dt = self.sample_dt(t, steps)
+    def sample_euler(self, draws: Paths, ic: float = 0.0) -> Paths:
         kappa = self.kappa
         theta = self.theta
+        dt = draws.dt
         sdt = self.sigma * np.sqrt(dt)
-        paths = np.zeros((size + 1, n))
+        sdt2 = sdt * sdt
+        paths = np.zeros(draws.data.shape)
         paths[0, :] = self.rate
-        for p in range(n):
-            w = normal(scale=sdt, size=size)
-            for i in range(size):
-                x = paths[i, p]
-                dx = kappa * (theta - x) * dt + np.sqrt(x) * w[i]
-                paths[i + 1, p] = x + dx
-        return paths
+        for t in range(draws.time_steps):
+            w = sdt * draws.data[t, :]
+            x = paths[t, :]
+            xplus = np.clip(x, 0, None)
+            dx = kappa * (theta - xplus) * dt + np.sqrt(xplus) * w + ic * (w * w - sdt2)
+            paths[t + 1, :] = x + dx
+        return Paths(t=draws.t, data=paths)
 
-    def sample_implicit(self, n: int, t: float = 1, steps: int = 0) -> np.ndarray:
+    def sample_implicit(self, draws: Paths) -> Paths:
         """Use an implicit scheme to preserve positivity of the process."""
-        size, dt = self.sample_dt(t, steps)
         kappa = self.kappa
         theta = self.theta
-        sigma = self.sigma
-        kdt2 = 2 * (kappa * dt + 1)
-        kts = (kappa * theta - 0.5 * sigma * sigma) * dt
+        dt = draws.dt
+        kdt2 = 2 * (1 + kappa * dt)
+        kts = (kappa * theta - 0.5 * self.sigma2) * dt
         sdt = self.sigma * np.sqrt(dt)
-        paths = np.zeros((size + 1, n))
+        paths = np.zeros(draws.data.shape)
         paths[0, :] = self.rate
-        for p in range(n):
-            w = normal(scale=sdt, size=size)
-            for i in range(size):
-                x = paths[i, p]
-                sw = w[i]
-                xs = (sw + np.sqrt(sw * sw + 2 * (x + kts) * kdt2)) / kdt2
-                paths[i + 1, p] = xs * xs
-        return paths
+        for t in range(draws.time_steps):
+            w = sdt * draws.data[t, :]
+            x = paths[t, :]
+            w2p = np.clip(w * w + 2 * (x + kts) * kdt2, 0, None)
+            xs = (w + np.sqrt(w2p)) / kdt2
+            paths[t + 1, :] = xs * xs
+        return Paths(t=draws.t, data=paths)
 
-    def characteristic(self, t: float, u: Vector) -> Vector:
+    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
         iu = Im * u
         sigma = self.sigma
         kappa = self.kappa
         kt = kappa * t
         ekt = np.exp(kt)
         sigma2 = sigma * sigma
         s2u = iu * sigma2
         c = s2u + (2 * kappa - s2u) * ekt
         b = 2 * kappa * iu / c
         a = 2 * kappa * self.theta * (kt + np.log(2 * kappa / c)) / sigma2
-        return np.exp(a + b * self.rate)
+        return -a - b * self.rate
 
-    def cumulative_characteristic(self, t: float, u: Vector) -> Vector:
+    def cumulative_characteristic(self, t: Vector, u: Vector) -> Vector:
         iu = Im * u
         sigma = self.sigma
         kappa = self.kappa
         sigma2 = sigma * sigma
         gamma = np.sqrt(kappa * kappa - 2 * iu * sigma2)
         egt = np.exp(gamma * t)
         c = (gamma + kappa) * (1 - egt) - 2 * gamma
         d = 2 * gamma * np.exp(0.5 * (gamma + kappa) * t)
         a = 2 * self.theta * kappa * np.log(-d / c) / sigma2
         b = 2 * iu * (1 - egt) / c
         return np.exp(a + b * self.rate)
+
+    def domain_range(self) -> Bounds:
+        return Bounds(0, np.inf)
+
+
+class CIRMarginal(StochasticProcess1DMarginal[CIR]):
+    def mean(self) -> Vector:
+        ekt = np.exp(-self.process.kappa * self.t)
+        return self.process.rate * ekt + self.process.theta * (1 - ekt)
+
+    def variance(self) -> Vector:
+        kappa = self.process.kappa
+        ekt = np.exp(-kappa * self.t)
+        return (
+            self.process.sigma2
+            * (1 - ekt)
+            * (self.process.rate * ekt + 0.5 * self.process.theta * (1 - ekt))
+            / kappa
+        )
+
+    def pdf(self, x: Vector) -> Vector:
+        k = self.process.kappa
+        s2 = self.process.sigma2
+        ekt = np.exp(-k * self.t)
+        c = 2 * k / (1 - ekt) / s2
+        q = 2 * k * self.process.theta / s2 - 1
+        u = c * ekt * self.process.rate
+        v = c * x
+        return (
+            c
+            * np.exp(-v - u)
+            * np.power(v / u, 0.5 * q)
+            * special.iv(q, 2 * np.sqrt(u * v))
+        )
```

### Comparing `quantflow-0.2.1/quantflow/sp/dsp.py` & `quantflow-0.2.2/quantflow/sp/dsp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+import math
 from typing import List
 
 import numpy as np
 from pydantic import Field
 
 from ..utils.types import Vector, as_array
-from .base import CountingProcess1D, Im
-from .cir import IntensityProcess
-from .poisson import PoissonProcess
+from .base import Im
+from .cir import CIR, IntensityProcess
+from .poisson import PoissonBase, PoissonProcess, poisson_arrivals
 
 
-class DSP(CountingProcess1D):
+class DSP(PoissonBase):
     r"""
     Doubly Stochastic Poisson process.
 
     It's a process where the inter-arrival time is exponentially distributed
     with rate :math:`\lambda_t`
 
     :param intensity: the stochastic intensity of the Poisson
     """
-    intensity: IntensityProcess = Field(
-        default_factory=IntensityProcess, description="intensity process"
+    intensity: IntensityProcess = Field(  # type ignore
+        default_factory=CIR, description="intensity process"
     )
     poisson: PoissonProcess = Field(default_factory=PoissonProcess, exclude=True)
 
     def pdf(self, t: float, n: Vector = 0) -> Vector:
         """PDF of the number of events at time t.
 
         It is obtained via inverse Fourier transform of the characteristic function
@@ -40,17 +41,21 @@
     def cdf(self, t: float, n: Vector) -> Vector:
         """CDF of the number of events at time t.
 
         It is obtained form cumulative summation of :class:`pdf`
         """
         return np.cumsum(self.pdf(t, n))
 
-    def characteristic_exponent(self, u: Vector) -> Vector:
-        return self.poisson.characteristic_exponent(u)
+    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
+        return self.poisson.characteristic_exponent(t, u)
 
-    def characteristic(self, t: float, u: Vector) -> Vector:
-        phi = self.characteristic_exponent(u)
+    def characteristic(self, t: Vector, u: Vector) -> Vector:
+        phi = self.characteristic_exponent(t, u)
         return self.intensity.cumulative_characteristic(t, -Im * phi)
 
     def arrivals(self, t: float = 1) -> List[float]:
-        paths = self.intensity.paths(1, t).integrate()
-        return self.poisson.arrivals(paths.data[-1, 0])
+        paths = self.intensity.sample(1, t, math.ceil(100 * t)).integrate()
+        intensity = paths.data[-1, 0]
+        return poisson_arrivals(intensity, t)
+
+    def sample_jumps(self, n: int) -> np.ndarray:
+        return self.poisson.sample_jumps(n)
```

### Comparing `quantflow-0.2.1/quantflow/sp/ou.py` & `quantflow-0.2.2/quantflow/sp/bns.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,66 @@
 from __future__ import annotations
 
 import numpy as np
 from pydantic import Field
+from scipy.special import xlogy
 
+from ..utils.paths import Paths
 from ..utils.types import Vector
-from .base import Im, IntensityProcess
-from .poisson import ExponentialPoissonProcess
+from .base import Im, StochasticProcess1D
+from .ou import GammaOU
 
 
-class OU(IntensityProcess):
-    r"""Non-Gaussian Ornstein-Uhlenbeck process
+class BNS(StochasticProcess1D):
+    """Barndorff-Nielson--Shephard (BNS) stochastic volatility model"""
 
-    The process :math:`x_t` that satisfies the following stochastic
-    differential equation:
-
-    .. math::
-        dx_t =-\kappa x_t dt + d j_t
-    """
-    a: float = Field(default=1, ge=0, description="Jump intensity")
-    decay: float = Field(default=0, gt=0, description="Jump size exponential decay")
+    variance_process: GammaOU = Field(
+        default_factory=GammaOU, description="Variance process"
+    )
+    rho: float = Field(default=0, ge=-1, le=1, description="Correlation")
 
     @classmethod
-    def create(
-        cls, rate: float = 1, kappa: float = 1, a: float = 1, decay: float | None = None
-    ) -> OU:
-        return cls(rate=rate, kappa=kappa, a=a, decay=decay or a / rate)
-
-    @property
-    def jump_process(self) -> ExponentialPoissonProcess:
-        return ExponentialPoissonProcess(rate=self.kappa * self.a, decay=self.decay)
-
-    def cdf(self, t: float, n: Vector) -> Vector:
-        raise NotImplementedError
-
-    def characteristic(self, t: float, u: Vector) -> Vector:
-        kappa = self.kappa
-        b = self.decay
-        iu = Im * u
-        kt = kappa * t
-        ekt = np.exp(-kt)
-        c1 = iu * ekt
-        c0 = self.a * (np.log((b / ekt - iu) / (b - iu)) - kt)
-        return np.exp(c0 + c1 * self.rate)
-
-    def cumulative_characteristic(self, t: float, u: Vector) -> Vector:
-        kappa = self.kappa
-        b = self.decay
-        iu = Im * u
-        iuk = iu / kappa
-        ekt = np.exp(-kappa * t)
-        c1 = iuk * (1 - ekt)
-        c0 = self.a * (b * np.log(b / (iuk + (b - iuk) / ekt)) / (iuk - b) - kappa * t)
-        return np.exp(c0 + c1 * self.rate)
-
-    def sample(self, n: int, t: float = 1, steps: int = 0) -> np.ndarray:
-        size, dt = self.sample_dt(t, steps)
-        jump_process = self.jump_process
-        paths = np.zeros((size + 1, n))
-        paths[0, :] = self.rate
-        for p in range(n):
-            arrivals = jump_process.arrivals(t)
-            jumps = jump_process.jumps(len(arrivals))
-            pp = paths[:, p]
-            i = 1
-            for arrival, jump in zip(arrivals, jumps):
-                while i * dt < arrival:
-                    i = self._advance(i, pp, dt)
-                if i <= size:
-                    i = self._advance(i, pp, dt, arrival, jump)
-            while i <= size:
-                i = self._advance(i, pp, dt)
-        return paths
-
-    def _advance(
-        self, i: int, pp: np.ndarray, dt: float, arrival: float = 0, jump: float = 0
-    ) -> int:
-        x = pp[i - 1]
-        kappa = self.kappa
-        t0 = i * dt
-        t1 = t0 + dt
-        a = arrival or t1
-        pp[i] = x - kappa * x * (a - t0) - kappa * (x + jump) * (t1 - a) + jump
-        return i + 1
-
-
-class OU2(OU):
-    def cumulative_characteristic(self, t: float, u: Vector) -> Vector:
-        """Formula from a paper"""
-        kappa = self.kappa
-        b = self.decay
-        iu = Im * u
-        iuk = iu / kappa
-        ekt = np.exp(-kappa * t)
-        c1 = iuk * (1 - ekt)
-        c0 = self.a * (b * np.log(b / (b - c1)) - iu * t) / (iuk - b)
-        return np.exp(c0 + c1 * self.rate)
+    def create(cls, vol: float, kappa: float, decay: float, rho: float) -> BNS:
+        return cls(
+            variance_process=GammaOU.create(rate=vol * vol, kappa=kappa, decay=decay),
+            rho=rho,
+        )
+
+    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
+        return -self._zeta(t, 0.5 * Im * u * u, self.rho * u)
+
+    def sample(self, n: int, time_horizon: float = 1, time_steps: int = 100) -> Paths:
+        return self.sample_from_draws(Paths.normal_draws(n, time_horizon, time_steps))
+
+    def sample_from_draws(self, path_dw: Paths, *args: Paths) -> Paths:
+        if args:
+            args[0]
+        else:
+            # generate the background driving process samples if not provided
+            path_dz = self.variance_process.bdlp.sample(
+                path_dw.samples, path_dw.t, path_dw.time_steps
+            )
+        dt = path_dw.dt
+        # sample the activity rate process
+        v = self.variance_process.sample_from_draws(path_dz)
+        # create the time-changed Brownian motion
+        dw = path_dw.data * np.sqrt(v.data * dt)
+        paths = np.zeros(dw.shape)
+        paths[1:] = np.cumsum(dw[:-1], axis=0) + path_dz.data
+        return Paths(t=path_dw.t, data=paths)
+
+    # Internal characteristics function methods (see docs)
+
+    def _zeta(self, t: Vector, a: Vector, b: Vector) -> Vector:
+        k = self.variance_process.kappa
+        c = a * (1 - np.exp(-k * t)) / k
+        g = (a + b) / self.variance_process.beta
+        return Im * c * self.variance_process.rate - self.variance_process.intensity * (
+            self._i(b + c, g) - self._i(b, g)
+        )
+
+    def _i(self, x: Vector, g: Vector) -> Vector:
+        k = self.variance_process.kappa
+        beta = self.variance_process.beta
+        l1 = xlogy(k - Im * g, x + Im * beta)
+        l2 = xlogy(g / (g + Im * k) / k, beta * g / k - x)
+        return l1 + l2
```

### Comparing `quantflow-0.2.1/quantflow/utils/bins.py` & `quantflow-0.2.2/quantflow/utils/bins.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.1/quantflow/utils/interest_rates.py` & `quantflow-0.2.2/quantflow/utils/interest_rates.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.1/quantflow/utils/marginal.py` & `quantflow-0.2.2/quantflow/sp/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,139 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import Optional, cast
+from typing import Generic, TypeVar
 
 import numpy as np
-import pandas as pd
+from pydantic import BaseModel, ConfigDict, Field
 from scipy.optimize import Bounds
 
-from .transforms import Transform, grid
-from .types import Vector
-
+from quantflow.utils.marginal import Marginal1D, default_bounds
+from quantflow.utils.numbers import sigfig
+from quantflow.utils.paths import Paths
+from quantflow.utils.transforms import lower_bound, upper_bound
+from quantflow.utils.types import FloatArray, Vector
+
+Im = complex(0, 1)
 
-def default_bounds() -> Bounds:
-    return Bounds(-np.inf, np.inf)
 
+class StochasticProcess(BaseModel, ABC):
+    """
+    Base class for stochastic processes in continuous time
+    """
 
-class Marginal1D(ABC):
-    def mean(self) -> float:
-        """Expected value at a time horizon"""
-        return self.mean_from_characteristic()
-
-    def std(self) -> float:
-        """Standard deviation at a time horizon"""
-        return np.sqrt(self.variance())
-
-    def variance(self) -> float:
-        """Variance at a time horizon"""
-        return self.variance_from_characteristic()
-
-    def mean_from_characteristic(self) -> float:
-        """Calculate mean as first derivative of characteristic function at 0"""
-        d = 0.001
-        m = -0.5 * 1j * (self.characteristic(d) - self.characteristic(-d)) / d
-        return cast(complex, m).real
-
-    def variance_from_characteristic(self) -> float:
-        """Calculate variance as second derivative of characteristic function at 0"""
-        d = 0.001
-        c1 = self.characteristic(d)
-        c0 = self.characteristic(0)
-        c2 = self.characteristic(-d)
-        m = -0.5 * 1j * (c1 - c2) / d
-        s = -(c1 - 2 * c0 + c2) / (d * d) - m * m
-        return cast(float, s.real)
+    @abstractmethod
+    def sample_from_draws(self, path: Paths, *args: Paths) -> Paths:
+        """Sample a path from the process given a set of draws"""
 
-    def pdf(self, n: Vector) -> Vector:
+    @abstractmethod
+    def sample(
+        self, paths: int, time_horizon: float = 1, time_steps: int = 100
+    ) -> Paths:
+        """Generate random paths from the process.
+
+        :param paths: Number of paths
+        :param time_horizon: time horizon
+        :param time_steps: number of time steps to arrive at horizon
         """
-        Computes the probability density (or mass) function of the process.
 
-        It has a base implementation that computes the pdf from the
-        :class:`cdf` method, but a subclass should overload this method if a
-        more optimized way of computing it is available.
+    @abstractmethod
+    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
+        """Characteristic exponent at time `t` for a given input parameter"""
+
+    def characteristic(self, t: Vector, u: Vector) -> Vector:
+        r"""Characteristic function at time `t` for a given input parameter
+
+        The characteristic function represents the Fourier transform of the
+        probability density function
+
+        .. math::
+            \phi = {\mathbb E} \left[e^{i u x_t}\right]
 
         :param t: time horizon
-        :param n: Location in the stochastic process domain space. If a numpy array,
-            the output should have the same shape as the input.
+        :param u: characteristic function input parameter
         """
-        return self.cdf(n) - self.cdf(n - 1)
+        return np.exp(-self.characteristic_exponent(t, u))
 
-    def frequency_space(self, N: int, max_frequency: float = 10.0) -> np.ndarray:
-        return max_frequency * grid(N) / N
+    def convexity_correction(self, t: Vector) -> Vector:
+        """Convexity correction for the process"""
+        return -self.characteristic_exponent(t, complex(0, -1)).real
 
-    def pdf_from_characteristic(
-        self,
-        N: int,
-        max_frequency: float = 10.0,
-        delta_x: float | None = None,
-        simpson_rule: bool = False,
-    ) -> pd.DataFrame:
-        """
-        Compute the probability density function from the characteristic function.
-        """
-        t = Transform(N, max_frequency, self.domain_range(), simpson_rule)
-        psi = cast(np.ndarray, self.characteristic(t.freq))
-        return pd.DataFrame(t(psi, delta_x))
-
-    def call_option(
-        self,
-        N: int,
-        max_frequency: float = 10.0,
-        delta_x: Optional[float] = None,
-        alpha: float = 0.5,
-        simpson_rule: bool = False,
-    ) -> pd.DataFrame:
-        t = Transform(N, max_frequency, self.domain_range(), simpson_rule)
-        phi = cast(np.ndarray, self.call_option_transform(t.freq - 1j * alpha))
-        result = t(phi, delta_x)
-        x = result["x"]
-        y = result["y"]
-        return pd.DataFrame(dict(x=x, y=y * np.exp(-alpha * x)))
-
-    def call_option_transform(self, u: Vector) -> Vector:
-        """Call option transfrom"""
-        uj = 1j * u
-        return self.characteristic_corrected(u - 1j) / (uj * uj + uj)
-
-    def characteristic_corrected(self, u: Vector) -> Vector:
-        convexity = np.log(self.characteristic(-1j))
-        return self.characteristic(u) * np.exp(-1j * u * convexity)
+
+class StochasticProcess1D(StochasticProcess):
+    """
+    Base class for 1D stochastic process in continuous time
+    """
+
+    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
+        return StochasticProcess1DMarginal(process=self, t=t)
 
     def domain_range(self) -> Bounds:
         return default_bounds()
 
-    def cdf(self, n: Vector) -> Vector:
-        """
-        Compute the cumulative distribution function of the process.
+    def max_frequency(self, std: float) -> float:
+        """Maximum frequency when calculating characteristic functions"""
+        return np.sqrt(40 / std / std)
+
+    def support(self, mean: float, std: float, points: int) -> FloatArray:
+        """Support of the process at time `t`"""
+        bounds = self.domain_range()
+        start = float(sigfig(lower_bound(bounds.lb, mean - std)))
+        end = float(sigfig(upper_bound(bounds.ub, mean + std)))
+        return np.linspace(start, end, points)
+
+
+P = TypeVar("P", bound=StochasticProcess1D)
 
-        :param t: time horizon
-        :param n: Location in the stochastic process domain space. If a numpy array,
-            the output should have the same shape as the input.
-        """
-        raise NotImplementedError
+
+class StochasticProcess1DMarginal(Marginal1D, Generic[P]):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+    process: P
+    t: Vector
+
+    def std_norm(self) -> Vector:
+        """Standard deviation at a time horizon normalized by the time"""
+        return np.sqrt(self.variance() / self.t)
+
+    def characteristic(self, u: Vector) -> Vector:
+        return self.process.characteristic(self.t, u)
+
+    def domain_range(self) -> Bounds:
+        return self.process.domain_range()
+
+    def max_frequency(self) -> float:
+        return self.process.max_frequency(np.min(self.std()))
+
+    def support(self, points: int = 100, *, std_mult: float = 4) -> FloatArray:
+        return self.process.support(
+            np.max(self.mean()), std_mult * np.max(self.std()), points
+        )
+
+    def option_alpha(self) -> float:
+        """Option alpha parameter for integrability of call option transform"""
+        return max(8 * np.max(np.exp(-2 * self.t)), 0.5)
+
+
+class IntensityProcess(StochasticProcess1D):
+    """Base class for mean reverting 1D processes which can be used
+    as stochastic intensity
+    """
+
+    rate: float = Field(default=1.0, gt=0, description="Instantaneous initial rate")
+    kappa: float = Field(default=1.0, gt=0, description="Mean reversion speed")
 
     @abstractmethod
-    def characteristic(self, n: Vector) -> Vector:
-        """
-        Compute the characteristic function on support points `n`.
+    def cumulative_characteristic(self, t: Vector, u: Vector) -> Vector:
+        r"""The characteristic function of the cumulative process:
+
+        .. math::
+            \phi = {\mathbb E} \left[e^{i u \int_0^t x_s ds}\right]
+
+        :param t: time horizon
+        :param u: frequency
         """
+
+    def domain_range(self) -> Bounds:
+        return Bounds(0, np.inf)
+
+    def ekt(self, t: Vector) -> Vector:
+        return np.exp(-self.kappa * t)
```

### Comparing `quantflow-0.2.1/quantflow/utils/paths.py` & `quantflow-0.2.2/quantflow/utils/paths.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any
 
 import numpy as np
 import pandas as pd
+from numpy.random import normal
 from pydantic import BaseModel, ConfigDict, Field
 from scipy.integrate import cumtrapz
 
 from . import plot
 
 
 class Paths(BaseModel):
@@ -15,43 +16,82 @@
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
     t: float = Field(description="time horizon")
     data: np.ndarray = Field(description="paths")
 
     @property
     def dt(self) -> float:
-        return self.t / self.steps
+        return self.t / self.time_steps
 
     @property
     def samples(self) -> int:
         return self.data.shape[1]
 
     @property
-    def steps(self) -> int:
+    def time_steps(self) -> int:
         return self.data.shape[0] - 1
 
     @property
     def time(self) -> np.ndarray:
-        return np.linspace(0.0, self.t, num=self.steps + 1)
+        return np.linspace(0.0, self.t, num=self.time_steps + 1)
 
     @property
     def df(self) -> pd.DataFrame:
-        return pd.DataFrame(self.data)
+        return pd.DataFrame(self.data, index=self.time)
 
     @property
     def xs(self) -> list[np.ndarray]:
         """Time as list of list (for visualization tools)"""
         return self.samples * [self.time]
 
     @property
     def ys(self) -> list[list[float]]:
         """Paths as list of list (for visualization tools)"""
         return self.data.transpose().tolist()
 
+    def mean(self) -> np.ndarray:
+        """Mean of paths"""
+        return np.mean(self.data, axis=1)
+
+    def std(self) -> np.ndarray:
+        """Standard deviation of paths"""
+        return np.std(self.data, axis=1)
+
+    def var(self) -> np.ndarray:
+        """Variance of paths"""
+        return np.var(self.data, axis=1)
+
     def integrate(self) -> Paths:
         """Integrate paths"""
         return self.__class__(
             t=self.t, data=cumtrapz(self.data, dx=self.dt, axis=0, initial=0)
         )
 
-    def plot(self) -> Any:
-        return plot.plot_lines(self.data)
+    def plot(self, **kwargs: Any) -> Any:
+        return plot.plot_lines(self.df, **kwargs)
+
+    @classmethod
+    def normal_draws(
+        cls,
+        paths: int,
+        time_horizon: float,
+        time_steps: int = 1000,
+        antithetic_variates: bool = True,
+    ) -> Paths:
+        """Generate normal draws
+
+        paths: number of paths
+        time_horizon: time horizon
+        time_steps: number of time steps to arrive at horizon
+        """
+        time_horizon / time_steps
+        odd = 0
+        if antithetic_variates:
+            odd = paths % 2
+            paths = paths // 2
+        data = normal(size=(time_steps + 1, paths))
+        if antithetic_variates:
+            data = np.concatenate((data, -data), axis=1)
+            if odd:
+                extra_data = normal(size=(time_steps + 1, odd))
+                data = np.concatenate((data, extra_data), axis=1)
+        return cls(t=time_horizon, data=data)
```

### Comparing `quantflow-0.2.1/quantflow/utils/types.py` & `quantflow-0.2.2/quantflow/utils/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from decimal import Decimal
 from typing import Optional, Union
 
 import numpy as np
+import numpy.typing as npt
 
 Number = Decimal
 Numbers = Union[int, float, np.number]
 NumberType = Union[float, int, str, Number]
 Vector = Union[int, float, complex, np.ndarray]
+FloatArray = npt.NDArray[np.float_]
+FloatArrayLike = FloatArray | float
 
 
 def as_number(num: Optional[NumberType] = None) -> Number:
     return Number(0 if num is None else str(num))
 
 
 def as_float(num: Optional[NumberType] = None) -> float:
```

### Comparing `quantflow-0.2.1/quantflow/utils/volatility.py` & `quantflow-0.2.2/quantflow/utils/volatility.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.1/PKG-INFO` & `quantflow-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: quantitative analysis
 License: BSD-3-Clause
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,16 @@
 
 ## Installation
 
 ```bash
 pip install quantflow
 ```
 
+![btcvol](https://github.com/quantmind/quantflow/assets/144320/88ed85d1-c3c5-489c-ac07-21b036593214)
+
 
 ## Modules
 
-* [quantflow.data](./quantflow/data) data APIs (requires `quantflow[data]`)
-* [quantflow.options](./quantflow/options) option pricing
-* [quantflow.sp](./quantflow/sp) stochastic process primitives
+* [quantflow.data](https://github.com/quantmind/quantflow/tree/main/quantflow/data) data APIs (requires `quantflow[data]`)
+* [quantflow.options](https://github.com/quantmind/quantflow/tree/main/quantflow/options) option pricing and calibration
+* [quantflow.sp](https://github.com/quantmind/quantflow/tree/main/quantflow/sp) stochastic process primitives
```

