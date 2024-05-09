# Comparing `tmp/mptradelib-0.3.9.tar.gz` & `tmp/mptradelib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.9.tar", max compression
+gzip compressed data, was "mptradelib-0.4.0.tar", max compression
```

## Comparing `mptradelib-0.3.9.tar` & `mptradelib-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.9/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.9/mptradelib/__init__.py
--rw-r--r--   0        0        0     4662 2024-05-05 15:13:06.736697 mptradelib-0.3.9/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.9/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5853 2024-05-05 15:12:34.719178 mptradelib-0.3.9/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.9/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.9/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.9/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2338 2024-05-04 09:41:29.250845 mptradelib-0.3.9/mptradelib/cli/new.py
--rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.9/mptradelib/feed.py
--rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.9/mptradelib/livetrade.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.9/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.9/mptradelib/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.3.9/mptradelib/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.9/mptradelib/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.9/mptradelib/test_renko.py
--rw-r--r--   0        0        0     2767 2024-05-04 12:41:24.598195 mptradelib-0.3.9/mptradelib/utils.py
--rw-r--r--   0        0        0      829 2024-05-05 17:14:03.977551 mptradelib-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.4.0/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4685 2024-05-09 18:07:27.997364 mptradelib-0.4.0/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.4.0/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.4.0/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.4.0/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.4.0/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.4.0/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.4.0/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.4.0/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.4.0/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.4.0/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.4.0/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.4.0/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.4.0/mptradelib/livetrade.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.4.0/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.4.0/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.4.0/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     5502 2024-05-06 16:15:40.095142 mptradelib-0.4.0/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.4.0/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      829 2024-05-09 18:31:59.599239 mptradelib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.4.0/PKG-INFO
```

### Comparing `mptradelib-0.3.9/README.md` & `mptradelib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.9/mptradelib/backtest.py` & `mptradelib-0.4.0/mptradelib/backtest.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,34 +3,16 @@
 import numpy as np
 from dataclasses import dataclass, asdict
 from typing import Callable
 from tqdm import tqdm
 from hyperopt import fmin, tpe, hp, STATUS_OK
 from hyperopt.pyll import scope
 from retry import retry
-
-position = None
-orders = []
-
-@dataclass
-class Order:
-    entry_time: dt.datetime
-    entry_price: float
-    sl: float
-    tp: float
-    direction: int
-    exit_time: dt.datetime = None
-    exit_price: float = None
-    profit: float = None
-
-    def set_profit(self):
-        if self.direction == 1:
-            self.profit = self.exit_price - self.entry_price
-        else:
-            self.profit = self.entry_price - self.exit_price
+import multiprocessing as mp
+from .broker.broker import Order
 
 class Backtest:
     params: dict = {
         "sl": None,
         "tp": None
     }
 
@@ -106,15 +88,15 @@
             elif isinstance(v.step, float):
                 space[k] = hp.quniform(k, v.start, v.stop, v.step)
             else:
                 raise ValueError(f"step of {k} can not be {type(v.step)}")
         return space
 
     @retry(tries=10)
-    def _optimizer(self, **kwargs):
+    def _optimizer(self, kwargs):
         space = self._define_space(kwargs)
         
         def objective(params):
             r = self.run(**params)
             return {'loss': -np.sum(r[0].profit), 'status': STATUS_OK}
         
         best = fmin(
@@ -124,19 +106,28 @@
             max_evals=100,
             show_progressbar=False
         )
         p = {k: int(v) for k, v in best.items()}
         r = self.run(**p)
         return best, np.sum(r[0].profit)
     
-    def optimize(self, runs=5, **kwargs):
+    def optimize(self, runs=5, show_progress=False, **kwargs):
         results = []
-        for _ in tqdm(range(runs)):
-            r = self._optimizer(**kwargs)
-            results.append(r)
+        l = tqdm(range(runs)) if show_progress else range(runs)
+
+        params = [kwargs] * runs
+        if show_progress:
+            with tqdm(total=len(params)) as pbar:
+                with mp.Pool(mp.cpu_count()) as p:
+                    for r in p.imap(self._optimizer, params):
+                        results.append(r)
+                        pbar.update()
+        else:
+            with mp.Pool(mp.cpu_count()) as p:
+                results = p.map(self._optimizer, params)
 
         max_profit = 0
         result = None
         for r in results:
             if r[1] > max_profit:
                 max_profit = r[1]
                 result = r
```

### Comparing `mptradelib-0.3.9/mptradelib/broker/session.py` & `mptradelib-0.4.0/mptradelib/broker/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import struct
 import time
 from urllib.parse import urlparse, parse_qs
 import requests
 import os
 from retry import retry
-from mptradelib.shoonya import NorenApi
+from .shoonya import NorenApi
 import pyotp
 
 
 class BaseSession:
     def init_client(self):
         raise NotImplementedError
```

### Comparing `mptradelib-0.3.9/mptradelib/broker/ticker.py` & `mptradelib-0.4.0/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.9/mptradelib/cli/new.py` & `mptradelib-0.4.0/mptradelib/cli/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logging.addLevelName(logging.INFO, 'info')
 
 libpath = os.path.abspath(os.path.join(sys.executable, f"../../lib/python{'.'.join(sys.version.split('.')[:2])}/site-packages/mptradelib"))
 if not os.path.exists(libpath):
     libpath = os.path.join(os.path.abspath('.'), "mptradelib")
 
 env = Environment(
-    loader=FileSystemLoader(os.path.join(libpath, "templates/strategy/")),
+    loader=FileSystemLoader(os.path.join(libpath, "cli/templates/strategy/")),
     extensions=['jinja2_strcase.StrcaseExtension']
 )
 
 @click.group
 def commands():
     pass
```

### Comparing `mptradelib-0.3.9/mptradelib/livetrade.py` & `mptradelib-0.4.0/mptradelib/livetrade.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from .feed import Datas, Tick, Series
 from .broker.broker import BaseBroker
-import pydantic
+import pydantic as pyd
 import copy
 
-class BaseStrategy(pydantic.BaseModel):
+class BaseStrategy(pyd.BaseModel):
+    model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
+
+    b: BaseBroker = pyd.Field(..., alias='broker')
     def next(self, symbol: str, data: Series) -> None:
         raise NotImplementedError
 
 class LiveTrade:
     _datas: Datas = None
     _s: BaseStrategy
-    b: BaseBroker
     _p: dict = {}
 
-    def __init__(self, s: BaseStrategy.__class__) -> None:
-        self._s = s()
+    def __init__(self, s: BaseStrategy.__class__, broker: BaseBroker) -> None:
+        if broker is None:
+            raise ValueError('broker not provided')
+        self._s = s(broker=broker)
 
     def set_datas(self, d: Datas):
         self._datas = d
 
-    def set_broker(self, b: BaseBroker):
-        self.b = b
-
     def _next(self, t: Tick):
+        self._s.b.notify_tick(t)
         params = self._p.get(t.symbol, {})
         for k, v in params.items():
             setattr(self._s, k, v)
         self._s.next(t.symbol, self._datas[t.symbol])
 
     def _process_params(self, kwargs):
         multisym_params_flag = True
@@ -50,15 +52,13 @@
         if not multisym_params_flag and not default_params_flag:
             raise ValueError("invalid strategy params provided")
 
     def run(self, **kwargs):
         if self._datas is None:
             raise ValueError("'datas' not found")
         
-        if not self.b:
-            raise ValueError('broker not found')
-        
         self._p = self._process_params(kwargs)
 
         self._datas.run("ticks", self._next)
-        while True:
-            pass
+        if self._datas.is_live:
+            while True:
+                pass
```

### Comparing `mptradelib-0.3.9/mptradelib/shoonya.py` & `mptradelib-0.4.0/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.9/mptradelib/templates/strategy/__init__.py.jinja` & `mptradelib-0.4.0/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -5,35 +5,28 @@
 import redis
 import requests
 import os
 from retry import retry
 from .livetrade import {{ strategy_name | to_camel }}
 
 
-@retry(tries=10, delay=2)
-def subscribe(symbols):
-    subs = {
-        "symbols": symbols
-    }
-    result = requests.post(os.getenv("SUBSCRIPTION_ENDPOINT"), data=subs)
-    if result.status_code != 200:
-        raise Exception("unable to subscribe to symbols")
-
-def run(symbols: list, timeframe: int, params: dict):
+def run(symbols: list, timeframe: int, params: dict, live: True):
     r = redis.Redis(
         host=os.getenv('REDIS_HOST'),
         port=os.getenv('REDIS_PORT'),
         decode_responses=True # <-- this will ensure that binary data is decoded
     )
 
     h = Historical(FyersSession())
-    datas = Datas(r, h).resample(timeframe)
-    datas.load(symbols=symbols)
-
-    sb = ShoonyaBroker(ShoonyaSession())
+    datas = Datas(symbols, r, h, live=live).resample(timeframe)
+    datas.load()
 
-    subscribe(symbols)
+    broker = None
+    if live:
+        broker = ShoonyaBroker(ShoonyaSession())
+    else:
+        broker = MockBroker()
     
-    l = LiveTrade(Popo)
+    l = LiveTrade({{ strategy_name | to_camel }}, broker=broker)
     l.set_datas(datas)
-    l.set_broker(sb)
-    l.run(**params)
+    l.run(**params)
+    return broker.orders()
```

### Comparing `mptradelib-0.3.9/mptradelib/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.4.0/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.9/mptradelib/templates/strategy/livetrade.py.jinja` & `mptradelib-0.4.0/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.9/mptradelib/test_renko.py` & `mptradelib-0.4.0/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.9/pyproject.toml` & `mptradelib-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.3.9/PKG-INFO` & `mptradelib-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

