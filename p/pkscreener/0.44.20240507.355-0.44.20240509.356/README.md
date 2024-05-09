# Comparing `tmp/pkscreener-0.44.20240507.355.tar.gz` & `tmp/pkscreener-0.44.20240509.356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240507.355.tar", last modified: Tue May  7 21:22:13 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240509.356.tar", last modified: Thu May  9 00:37:06 2024, max compression
```

## Comparing `pkscreener-0.44.20240507.355.tar` & `pkscreener-0.44.20240509.356.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 21:22:13.225366 pkscreener-0.44.20240507.355/
--rw-rw-rw-   0        0        0     1086 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-07 21:22:13.225938 pkscreener-0.44.20240507.355/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 21:22:13.200464 pkscreener-0.44.20240507.355/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 21:22:13.225366 pkscreener-0.44.20240507.355/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26895 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    10741 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30557 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23429 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119820 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52163 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82527 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-07 21:22:05.000000 pkscreener-0.44.20240507.355/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   127567 2024-05-07 21:17:45.000000 pkscreener-0.44.20240507.355/pkscreener/globals.py
--rw-rw-rw-   0        0        0      872 2024-05-07 21:17:46.000000 pkscreener-0.44.20240507.355/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    49807 2024-05-07 21:17:46.000000 pkscreener-0.44.20240507.355/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    28594 2024-05-07 21:17:46.000000 pkscreener-0.44.20240507.355/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-07 21:22:13.208218 pkscreener-0.44.20240507.355/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-07 21:22:13.000000 pkscreener-0.44.20240507.355/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-07 21:22:13.000000 pkscreener-0.44.20240507.355/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 21:22:13.000000 pkscreener-0.44.20240507.355/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-07 21:22:13.000000 pkscreener-0.44.20240507.355/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-07 21:22:13.000000 pkscreener-0.44.20240507.355/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-07 21:22:13.000000 pkscreener-0.44.20240507.355/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-07 21:22:13.226505 pkscreener-0.44.20240507.355/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-07 21:17:46.000000 pkscreener-0.44.20240507.355/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 00:37:06.301699 pkscreener-0.44.20240509.356/
+-rw-rw-rw-   0        0        0     1086 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-09 00:37:06.301699 pkscreener-0.44.20240509.356/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 00:37:06.286081 pkscreener-0.44.20240509.356/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 00:37:06.301699 pkscreener-0.44.20240509.356/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26895 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    10741 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30554 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23429 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21859 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119820 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    53283 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82527 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-09 00:36:59.000000 pkscreener-0.44.20240509.356/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   127581 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      872 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    49802 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    28594 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-09 00:37:06.301699 pkscreener-0.44.20240509.356/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-09 00:37:06.000000 pkscreener-0.44.20240509.356/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-09 00:37:06.000000 pkscreener-0.44.20240509.356/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 00:37:06.000000 pkscreener-0.44.20240509.356/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-09 00:37:06.000000 pkscreener-0.44.20240509.356/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 00:37:06.000000 pkscreener-0.44.20240509.356/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-09 00:37:06.000000 pkscreener-0.44.20240509.356/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-09 00:37:06.301699 pkscreener-0.44.20240509.356/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-09 00:33:26.000000 pkscreener-0.44.20240509.356/setup.py
```

### Comparing `pkscreener-0.44.20240507.355/LICENSE` & `pkscreener-0.44.20240509.356/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/LICENSE-Others` & `pkscreener-0.44.20240509.356/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/PKG-INFO` & `pkscreener-0.44.20240509.356/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240507.355
+Version: 0.44.20240509.356
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.355.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240509.356.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240507.355/README.md` & `pkscreener-0.44.20240509.356/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener/__init__.py` & `pkscreener-0.44.20240509.356/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     "22": "View Stock Performance         ",
     "23": "Breaking out now               ",
     "24": "Higher Highs,Lows & Close (SuperTrend)",
     "25": "Lower Highs,Lows (Watch for Rev.)",
     "26": "Stocks with stock-split/bonus/dividends",
     "27": "ATR Cross                      ",
     "28": "Bullish Higher Opens           ",
-    # "27": "Intraday Momentum Build-up      ",
+    "29": "Intraday Bid/Ask Build-up      ",
     # "28": "Extremely bullish daily close      ",
     # "29": "Rising RSI                      ",
     # "30": "RSI entering bullish territory",
     "42": "Show Last Screened Results",
     "M": "Back to the Top/Main menu",
     "Z": "Exit (Ctrl + C)",
 }
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PKScanRunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 from PKDevTools.classes.multiprocessing_logging import LogQueueReader
 from PKDevTools.classes.SuppressOutput import SuppressOutput
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.OutputControls import OutputControls
-# from PKDevTools.classes.PKJoinableQueue import PKJoinableQueue
-
+from PKNSETools.PKIntraDay import Intra_Day
 import pkscreener.classes.Fetcher as Fetcher
 import pkscreener.classes.ScreeningStatistics as ScreeningStatistics
 import pkscreener.classes.Utility as Utility
 
 class PKScanRunner:
     configManager = tools()
     configManager.getConfig(parser)
@@ -247,23 +246,27 @@
 
     def refreshDatabase(consumers,stockDictPrimary,stockDictSecondary):
         for worker in consumers:
             worker.objectDictionaryPrimary = stockDictPrimary
             worker.objectDictionarySecondary = stockDictSecondary
             worker.refreshDatabase = True
             
-    def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers,logging_queue):
+    def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, executeOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers,logging_queue):
         if tasks_queue is None or results_queue is None or consumers is None:
-            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(menuOption,keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items)
+            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(menuOption,keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items,executeOption)
             try:
                 if logging_queue is not None:
                     log_queue_reader = LogQueueReader(logging_queue)
                     log_queue_reader.start()
             except:
                 pass
+        # if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
+        #     intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
+        #     for consumer in consumers:
+        #         consumer.intradayNSEFetcher = intradayFetcher
         # else:
         #     # Restart the workers because the run method may have exited from a previous run
         #     PKScanRunner.startWorkers(consumers)
         PKScanRunner.tasks_queue = tasks_queue
         PKScanRunner.results_queue = results_queue
         PKScanRunner.consumers = consumers
         screenResults, saveResults, backtest_df = scanningCb(
@@ -285,15 +288,15 @@
         if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options) and not userPassedArgs.options.upper().startswith("C"):
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
-    def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
+    def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items, executeOption):
         tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
         sec_cache_file = cache_file if "intraday_" in cache_file else f"intraday_{cache_file}"
         consumers = [
                     PKMultiProcessorClient(
                         StockScreener().screenStocks,
@@ -316,14 +319,18 @@
                         None,
                         None
                         # (cache_file if (exists and menuOption in ["C"]) else None),
                         # (sec_cache_file if (exists and menuOption in ["C"]) else None),
                     )
                     for _ in range(totalConsumers)
                 ]
+        if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
+            intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
+            for consumer in consumers:
+                consumer.intradayNSEFetcher = intradayFetcher
         PKScanRunner.startWorkers(consumers)
         return tasks_queue,results_queue,consumers,logging_queue
 
     def startWorkers(consumers):
         try:
             from pytest_cov.embed import cleanup_on_signal, cleanup_on_sigterm
         except ImportError:
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/StockScreener.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,29 @@
                 intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.objectDictionarySecondary, configManager, fetcher, "1d","1m", testData,exchangeName)
                 
             if data is not None:
                 if len(data) == 0 or len(data) < backtestDuration:
                     raise StockDataEmptyException(f"Data length:{len(data)}")
             else:
                 raise StockDataEmptyException(f"Data is None: {data}")
+            
+            bidGreaterThanAsk = False
+            bidAskRatio = 0
+            if executeOption == 29:
+                hostRef.intradayNSEFetcher.symbol = stock.upper()
+                priceData = hostRef.intradayNSEFetcher.price_order_info()
+                totalBid = priceData["BidQty"].iloc[0]
+                totalAsk = priceData["AskQty"].iloc[0]
+                if totalBid > totalAsk and \
+                    priceData["LTP"].iloc[0] < float(priceData["UprCP"].iloc[0]) and \
+                    priceData["LTP"].iloc[0] > float(priceData["LwrCP"].iloc[0]):
+                    bidGreaterThanAsk = True
+                    bidAskRatio = round(totalBid/totalAsk,1) if totalAsk > 0 else 0
+                else:
+                    raise ScreeningStatistics.EligibilityConditionNotMet("Bid/Ask Eligibility Not met.")
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
             fullData, processedData, data = self.getCleanedDataForDuration(backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data)
             if "RUNNER" not in os.environ.keys() and backtestDuration == 0 and configManager.calculatersiintraday:
                 if (intraday_data is not None and not intraday_data.empty):
                     intraday_fullData, intraday_processedData = screener.preprocessData(
                         intraday_data, daysToLookback=configManager.effectiveDaysToLookback
                     )
@@ -170,15 +185,16 @@
                 raise StockDataEmptyException("Empty processedData")
             
             with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
                 self.updateStock(stock, screeningDictionary, saveDictionary, executeOption, exchangeName)
                 
                 self.performBasicLTPChecks(executeOption, screeningDictionary, saveDictionary, fullData, configManager, screener, exchangeName)
                 hasMinVolumeRatio = self.performBasicVolumeChecks(executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener)
-                
+                if (bidGreaterThanAsk and not hasMinVolumeRatio) or (bidGreaterThanAsk and bidAskRatio < 2):
+                    raise ScreeningStatistics.EligibilityConditionNotMet("Bid/Ask Eligibility Not met.")
                 isConfluence = False
                 isInsideBar = 0
                 isMaReversal = 0
                 isIpoBase = False
                 isMaSupport = False
                 isLorentzian = False
                 isVCP = False
@@ -485,14 +501,15 @@
                         or (executeOption == 11 and isShortTermBullish)
                         or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25,27,28] and isValidityCheckMet)
                         or (executeOption == 21 and (mfiStake > 0 and reversalOption in [3,5]))
                         or (executeOption == 21 and (mfiStake < 0 and reversalOption in [6,7]))
                         or (executeOption == 21 and (fairValueDiff > 0 and reversalOption in [8]))
                         or (executeOption == 21 and (fairValueDiff < 0 and reversalOption in [9]))
                         or (executeOption == 26)
+                        or (executeOption == 29) and bidGreaterThanAsk
                     ):
                         isNotMonitoringDashboard = userArgs.monitor is None
                         # Now screen for common ones to improve performance
                         if isNotMonitoringDashboard and not (executeOption == 6 and reversalOption == 7):
                             if sys.version_info >= (3, 11):
                                 with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
                                     screener.validateLorentzian(
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/classes/keys.py` & `pkscreener-0.44.20240509.356/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/courbd.ttf` & `pkscreener-0.44.20240509.356/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/globals.py` & `pkscreener-0.44.20240509.356/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1083,19 +1083,19 @@
             df = df[
                 df["Stock"].astype(str).str.contains("BSE:") == False
             ]
             listStockCodes.extend(list(df["Stock"]))
     if executeOption == 42:
         Utility.tools.getLastScreenedResults(defaultAnswer)
         return None, None
-    if executeOption >= 29 and executeOption <= 41:
+    if executeOption >= 30 and executeOption <= 41:
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
-            + "\n[+] Error: Option 29 to 41 Not implemented yet! Press <Enter> to continue."
+            + "\n[+] Error: Option 30 to 41 Not implemented yet! Press <Enter> to continue."
             + colorText.END
         )
         input("Press <Enter> to continue...")
         return None, None
     if (
         not str(indexOption).isnumeric() and indexOption in ["W", "E", "M", "N", "Z"]
     ) or (
@@ -1239,15 +1239,15 @@
                 fillerPlaceHolder = fillerPlaceHolder + 1
                 actualHistoricalDuration = samplingDuration - fillerPlaceHolder
                 if actualHistoricalDuration >= 0:
                     progressbar()
         sys.stdout.write(f"\x1b[1A") # Replace the download progress bar and start writing on the same line
         if not keyboardInterruptEventFired:
             global tasks_queue, results_queue, consumers, logging_queue
-            screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers,logging_queue=logging_queue)
+            screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption,executeOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers,logging_queue=logging_queue)
             if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options and not userPassedArgs.options.upper().startswith("C")):
                 tasks_queue = None
                 results_queue = None
                 consumers = None
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDictPrimary,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240509.356/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240509.356/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,22 +109,22 @@
 TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI"]
 TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "D", "I", "E", "U", "L", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
 SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_19_TO_25 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","22","26","27","28","29","30","42","M","Z"]
-SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","30","42","M","Z"]
 SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27","28"]
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
 INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
-UNSUPPORTED_COMMAND_MENUS =["22","29","30","42","M","Z"]
-SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28"]
+UNSUPPORTED_COMMAND_MENUS =["22","30","42","M","Z"]
+SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29"]
 
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0) -> int:
     """Send message on `/start`."""
     updateCarrier = None
     if update is None:
         return
     else:
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240509.356/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240509.356/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240507.355
+Version: 0.44.20240509.356
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240507.355.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240509.356.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.353/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240507.355/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240507.355/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240509.356/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240507.355/setup.py` & `pkscreener-0.44.20240509.356/setup.py`

 * *Files identical despite different names*

