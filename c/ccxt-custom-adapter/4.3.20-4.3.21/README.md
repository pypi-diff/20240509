# Comparing `tmp/ccxt-custom-adapter-4.3.20.tar.gz` & `tmp/ccxt-custom-adapter-4.3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccxt-custom-adapter-4.3.20.tar", last modified: Thu May  9 09:50:14 2024, max compression
+gzip compressed data, was "ccxt-custom-adapter-4.3.21.tar", last modified: Thu May  9 09:59:25 2024, max compression
```

## Comparing `ccxt-custom-adapter-4.3.20.tar` & `ccxt-custom-adapter-4.3.21.tar`

### file list

```diff
@@ -1,573 +1,573 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:14.143308 ccxt-custom-adapter-4.3.20/
--rw-rw-rw-   0        0        0     1068 2024-05-09 09:45:33.000000 ccxt-custom-adapter-4.3.20/LICENSE.txt
--rw-rw-rw-   0        0        0      101 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/MANIFEST.in
--rw-rw-rw-   0        0        0   112518 2024-05-09 09:50:14.140293 ccxt-custom-adapter-4.3.20/PKG-INFO
--rw-rw-rw-   0        0        0   102253 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.344546 ccxt-custom-adapter-4.3.20/ccxt/
--rw-rw-rw-   0        0        0    15834 2024-05-09 09:45:07.000000 ccxt-custom-adapter-4.3.20/ccxt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.499586 ccxt-custom-adapter-4.3.20/ccxt/abstract/
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/__init__.py
--rw-rw-rw-   0        0        0     1448 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/ace.py
--rw-rw-rw-   0        0        0    10382 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/alpaca.py
--rw-rw-rw-   0        0        0    11394 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/ascendex.py
--rw-rw-rw-   0        0        0    15601 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bequant.py
--rw-rw-rw-   0        0        0     4895 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bigone.py
--rw-rw-rw-   0        0        0    92016 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/binance.py
--rw-rw-rw-   0        0        0    92016 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/binancecoinm.py
--rw-rw-rw-   0        0        0    98736 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/binanceus.py
--rw-rw-rw-   0        0        0    92016 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/binanceusdm.py
--rw-rw-rw-   0        0        0    16032 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bingx.py
--rw-rw-rw-   0        0        0     2830 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bit2c.py
--rw-rw-rw-   0        0        0     2735 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitbank.py
--rw-rw-rw-   0        0        0     5820 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitbay.py
--rw-rw-rw-   0        0        0     4082 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitbns.py
--rw-rw-rw-   0        0        0    15601 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitcoincom.py
--rw-rw-rw-   0        0        0     7605 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitfinex.py
--rw-rw-rw-   0        0        0    19194 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitfinex2.py
--rw-rw-rw-   0        0        0     3576 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitflyer.py
--rw-rw-rw-   0        0        0    89841 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitget.py
--rw-rw-rw-   0        0        0     3443 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bithumb.py
--rw-rw-rw-   0        0        0    14031 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitmart.py
--rw-rw-rw-   0        0        0    10774 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitmex.py
--rw-rw-rw-   0        0        0     3295 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitopro.py
--rw-rw-rw-   0        0        0     3859 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitpanda.py
--rw-rw-rw-   0        0        0     9379 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitrue.py
--rw-rw-rw-   0        0        0     4025 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitso.py
--rw-rw-rw-   0        0        0    27930 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitstamp.py
--rw-rw-rw-   0        0        0     3478 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitteam.py
--rw-rw-rw-   0        0        0     2357 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bitvavo.py
--rw-rw-rw-   0        0        0     2024 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bl3p.py
--rw-rw-rw-   0        0        0     2638 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/blockchaincom.py
--rw-rw-rw-   0        0        0     4217 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/blofin.py
--rw-rw-rw-   0        0        0     1380 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/btcalpha.py
--rw-rw-rw-   0        0        0      849 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/btcbox.py
--rw-rw-rw-   0        0        0     3690 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/btcmarkets.py
--rw-rw-rw-   0        0        0     1777 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/btcturk.py
--rw-rw-rw-   0        0        0    48773 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/bybit.py
--rw-rw-rw-   0        0        0     3311 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/cex.py
--rw-rw-rw-   0        0        0    15507 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinbase.py
--rw-rw-rw-   0        0        0     4770 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinbaseinternational.py
--rw-rw-rw-   0        0        0     7162 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinbasepro.py
--rw-rw-rw-   0        0        0     3417 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coincheck.py
--rw-rw-rw-   0        0        0    34678 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinex.py
--rw-rw-rw-   0        0        0     6538 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinlist.py
--rw-rw-rw-   0        0        0     6842 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinmate.py
--rw-rw-rw-   0        0        0     3975 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinmetro.py
--rw-rw-rw-   0        0        0     8291 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinone.py
--rw-rw-rw-   0        0        0     8007 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinsph.py
--rw-rw-rw-   0        0        0     2707 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/coinspot.py
--rw-rw-rw-   0        0        0    18475 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/cryptocom.py
--rw-rw-rw-   0        0        0     7563 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/currencycom.py
--rw-rw-rw-   0        0        0     5107 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/delta.py
--rw-rw-rw-   0        0        0    15499 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/deribit.py
--rw-rw-rw-   0        0        0    11452 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/digifinex.py
--rw-rw-rw-   0        0        0     6177 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/exmo.py
--rw-rw-rw-   0        0        0    15601 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/fmfwio.py
--rw-rw-rw-   0        0        0    41994 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/gate.py
--rw-rw-rw-   0        0        0    41994 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/gateio.py
--rw-rw-rw-   0        0        0     6915 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/gemini.py
--rw-rw-rw-   0        0        0    15601 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/hitbtc.py
--rw-rw-rw-   0        0        0    15601 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/hitbtc3.py
--rw-rw-rw-   0        0        0     2906 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/hollaex.py
--rw-rw-rw-   0        0        0    99311 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/htx.py
--rw-rw-rw-   0        0        0    99311 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/huobi.py
--rw-rw-rw-   0        0        0    14331 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/huobijp.py
--rw-rw-rw-   0        0        0      240 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/hyperliquid.py
--rw-rw-rw-   0        0        0     1743 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/idax.py
--rw-rw-rw-   0        0        0     2129 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/idex.py
--rw-rw-rw-   0        0        0     4165 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/independentreserve.py
--rw-rw-rw-   0        0        0     2488 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/indodax.py
--rw-rw-rw-   0        0        0     5877 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/kraken.py
--rw-rw-rw-   0        0        0     3537 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/krakenfutures.py
--rw-rw-rw-   0        0        0    25491 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/kucoin.py
--rw-rw-rw-   0        0        0    28204 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/kucoinfutures.py
--rw-rw-rw-   0        0        0    24579 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/kuna.py
--rw-rw-rw-   0        0        0     7168 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/latoken.py
--rw-rw-rw-   0        0        0     8675 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/lbank.py
--rw-rw-rw-   0        0        0     3619 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/luno.py
--rw-rw-rw-   0        0        0     2960 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/lykke.py
--rw-rw-rw-   0        0        0     2357 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/mercado.py
--rw-rw-rw-   0        0        0    25902 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/mexc.py
--rw-rw-rw-   0        0        0    11878 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/ndax.py
--rw-rw-rw-   0        0        0     3093 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/novadax.py
--rw-rw-rw-   0        0        0     1721 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/oceanex.py
--rw-rw-rw-   0        0        0     9414 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/okcoin.py
--rw-rw-rw-   0        0        0    45891 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/okx.py
--rw-rw-rw-   0        0        0     3859 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/onetrading.py
--rw-rw-rw-   0        0        0     2054 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/p2b.py
--rw-rw-rw-   0        0        0     2843 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/paymium.py
--rw-rw-rw-   0        0        0    15203 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/phemex.py
--rw-rw-rw-   0        0        0     8073 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/poloniex.py
--rw-rw-rw-   0        0        0     5219 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/poloniexfutures.py
--rw-rw-rw-   0        0        0     1969 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/probit.py
--rw-rw-rw-   0        0        0     5875 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/timex.py
--rw-rw-rw-   0        0        0     4094 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/tokocrypto.py
--rw-rw-rw-   0        0        0     1372 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/tradeogre.py
--rw-rw-rw-   0        0        0     3576 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/upbit.py
--rw-rw-rw-   0        0        0    19631 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/wavesexchange.py
--rw-rw-rw-   0        0        0     2782 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/wazirx.py
--rw-rw-rw-   0        0        0    10977 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/whitebit.py
--rw-rw-rw-   0        0        0    10368 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/woo.py
--rw-rw-rw-   0        0        0     1339 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/yobit.py
--rw-rw-rw-   0        0        0     3935 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/zaif.py
--rw-rw-rw-   0        0        0     5820 2024-05-09 09:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/abstract/zonda.py
--rw-rw-rw-   0        0        0    41656 2024-05-09 07:22:32.000000 ccxt-custom-adapter-4.3.20/ccxt/ace.py
--rw-rw-rw-   0        0        0    47215 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/alpaca.py
--rw-rw-rw-   0        0        0   151413 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.20/ccxt/ascendex.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.692201 ccxt-custom-adapter-4.3.20/ccxt/async_support/
--rw-rw-rw-   0        0        0    15597 2024-05-09 09:45:07.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/__init__.py
--rw-rw-rw-   0        0        0    41880 2024-05-09 07:22:32.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/ace.py
--rw-rw-rw-   0        0        0    47427 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/alpaca.py
--rw-rw-rw-   0        0        0   152201 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/ascendex.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.700740 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/
--rw-rw-rw-   0        0        0       67 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/__init__.py
--rw-rw-rw-   0        0        0   107440 2024-05-09 09:46:30.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/exchange.py
--rw-rw-rw-   0        0        0     1847 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/throttler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.719206 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/
--rw-rw-rw-   0        0        0     1791 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/__init__.py
--rw-rw-rw-   0        0        0     5751 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-rw-   0        0        0     8100 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/cache.py
--rw-rw-rw-   0        0        0     7289 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/client.py
--rw-rw-rw-   0        0        0     3864 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/fast_client.py
--rw-rw-rw-   0        0        0     1499 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/functions.py
--rw-rw-rw-   0        0        0     2067 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/future.py
--rw-rw-rw-   0        0        0     2894 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/order_book.py
--rw-rw-rw-   0        0        0     6478 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-rw-   0        0        0     1188 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bequant.py
--rw-rw-rw-   0        0        0    92628 2024-05-09 07:22:36.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bigone.py
--rw-rw-rw-   0        0        0   619727 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/binance.py
--rw-rw-rw-   0        0        0     1683 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/binancecoinm.py
--rw-rw-rw-   0        0        0     9177 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/binanceus.py
--rw-rw-rw-   0        0        0     2518 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/binanceusdm.py
--rw-rw-rw-   0        0        0   185788 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bingx.py
--rw-rw-rw-   0        0        0    37119 2024-05-09 07:23:14.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bit2c.py
--rw-rw-rw-   0        0        0    42105 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitbank.py
--rw-rw-rw-   0        0        0      492 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitbay.py
--rw-rw-rw-   0        0        0    48391 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitbns.py
--rw-rw-rw-   0        0        0      516 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitcoincom.py
--rw-rw-rw-   0        0        0    72683 2024-05-09 07:23:17.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitfinex.py
--rw-rw-rw-   0        0        0   159158 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitfinex2.py
--rw-rw-rw-   0        0        0    41705 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitflyer.py
--rw-rw-rw-   0        0        0   423998 2024-05-09 07:23:57.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitget.py
--rw-rw-rw-   0        0        0    45764 2024-05-09 07:23:59.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bithumb.py
--rw-rw-rw-   0        0        0   199986 2024-05-09 07:24:11.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitmart.py
--rw-rw-rw-   0        0        0   127015 2024-05-09 07:24:17.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitmex.py
--rw-rw-rw-   0        0        0    68926 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitopro.py
--rw-rw-rw-   0        0        0      485 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitpanda.py
--rw-rw-rw-   0        0        0   136842 2024-05-09 07:24:28.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitrue.py
--rw-rw-rw-   0        0        0    71271 2024-05-09 07:24:31.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitso.py
--rw-rw-rw-   0        0        0    92723 2024-05-09 07:24:39.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitstamp.py
--rw-rw-rw-   0        0        0   102358 2024-05-09 07:24:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitteam.py
--rw-rw-rw-   0        0        0    92011 2024-05-09 07:24:49.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bitvavo.py
--rw-rw-rw-   0        0        0    20611 2024-05-09 07:24:50.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bl3p.py
--rw-rw-rw-   0        0        0    49191 2024-05-09 07:24:52.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/blockchaincom.py
--rw-rw-rw-   0        0        0    99798 2024-05-09 07:24:57.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/blofin.py
--rw-rw-rw-   0        0        0    36979 2024-05-09 07:24:58.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/btcalpha.py
--rw-rw-rw-   0        0        0    23686 2024-05-09 07:24:59.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/btcbox.py
--rw-rw-rw-   0        0        0    51834 2024-05-09 07:25:01.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/btcmarkets.py
--rw-rw-rw-   0        0        0    36875 2024-05-09 07:25:02.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/btcturk.py
--rw-rw-rw-   0        0        0   412729 2024-05-09 07:25:35.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/bybit.py
--rw-rw-rw-   0        0        0    70280 2024-05-09 07:25:37.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/cex.py
--rw-rw-rw-   0        0        0   213099 2024-05-09 07:25:49.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinbase.py
--rw-rw-rw-   0        0        0    87794 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinbaseinternational.py
--rw-rw-rw-   0        0        0    79177 2024-05-09 07:25:53.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinbasepro.py
--rw-rw-rw-   0        0        0    35870 2024-05-09 07:25:56.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coincheck.py
--rw-rw-rw-   0        0        0   260942 2024-05-09 07:26:08.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinex.py
--rw-rw-rw-   0        0        0   103557 2024-05-09 07:26:14.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinlist.py
--rw-rw-rw-   0        0        0    46212 2024-05-09 07:26:16.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinmate.py
--rw-rw-rw-   0        0        0    81020 2024-05-09 07:26:20.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinmetro.py
--rw-rw-rw-   0        0        0    47138 2024-05-09 07:26:23.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinone.py
--rw-rw-rw-   0        0        0    91066 2024-05-09 07:26:29.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinsph.py
--rw-rw-rw-   0        0        0    23766 2024-05-09 07:26:30.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/coinspot.py
--rw-rw-rw-   0        0        0   130329 2024-05-09 07:26:38.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/cryptocom.py
--rw-rw-rw-   0        0        0    87220 2024-05-09 07:26:42.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/currencycom.py
--rw-rw-rw-   0        0        0   151065 2024-05-09 07:26:48.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/delta.py
--rw-rw-rw-   0        0        0   161268 2024-05-09 07:26:59.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/deribit.py
--rw-rw-rw-   0        0        0   168940 2024-05-09 07:27:06.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/digifinex.py
--rw-rw-rw-   0        0        0   115081 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/exmo.py
--rw-rw-rw-   0        0        0     1250 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/fmfwio.py
--rw-rw-rw-   0        0        0   321459 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/gate.py
--rw-rw-rw-   0        0        0      459 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/gateio.py
--rw-rw-rw-   0        0        0    81171 2024-05-09 07:27:36.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/gemini.py
--rw-rw-rw-   0        0        0   154049 2024-05-09 07:27:45.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/hitbtc.py
--rw-rw-rw-   0        0        0      469 2024-05-09 07:27:46.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/hitbtc3.py
--rw-rw-rw-   0        0        0    76379 2024-05-09 07:27:48.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/hollaex.py
--rw-rw-rw-   0        0        0   422790 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/htx.py
--rw-rw-rw-   0        0        0      452 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/huobi.py
--rw-rw-rw-   0        0        0    88468 2024-05-09 07:28:56.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/huobijp.py
--rw-rw-rw-   0        0        0   100359 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/hyperliquid.py
--rw-rw-rw-   0        0        0    23564 2024-05-09 09:46:28.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/idax.py
--rw-rw-rw-   0        0        0    73474 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/idex.py
--rw-rw-rw-   0        0        0    32435 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/independentreserve.py
--rw-rw-rw-   0        0        0    52229 2024-05-09 07:43:24.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/indodax.py
--rw-rw-rw-   0        0        0   126051 2024-05-09 07:43:27.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/kraken.py
--rw-rw-rw-   0        0        0   117284 2024-05-09 07:43:30.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/krakenfutures.py
--rw-rw-rw-   0        0        0   218775 2024-05-09 07:43:38.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/kucoin.py
--rw-rw-rw-   0        0        0   124930 2024-05-09 07:43:39.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/kucoinfutures.py
--rw-rw-rw-   0        0        0    96407 2024-05-09 07:43:41.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/kuna.py
--rw-rw-rw-   0        0        0    79533 2024-05-09 07:43:42.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/latoken.py
--rw-rw-rw-   0        0        0   115887 2024-05-09 07:43:44.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/lbank.py
--rw-rw-rw-   0        0        0    46225 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/luno.py
--rw-rw-rw-   0        0        0    51384 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/lykke.py
--rw-rw-rw-   0        0        0    35581 2024-05-09 07:43:46.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/mercado.py
--rw-rw-rw-   0        0        0   241953 2024-05-09 07:43:52.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/mexc.py
--rw-rw-rw-   0        0        0   109125 2024-05-09 07:43:58.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/ndax.py
--rw-rw-rw-   0        0        0    64673 2024-05-09 07:44:00.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/novadax.py
--rw-rw-rw-   0        0        0    38180 2024-05-09 07:44:01.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/oceanex.py
--rw-rw-rw-   0        0        0   151640 2024-05-09 07:44:14.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/okcoin.py
--rw-rw-rw-   0        0        0   377624 2024-05-09 07:44:50.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/okx.py
--rw-rw-rw-   0        0        0    88565 2024-05-09 07:44:52.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/onetrading.py
--rw-rw-rw-   0        0        0    54455 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/p2b.py
--rw-rw-rw-   0        0        0    24397 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/paymium.py
--rw-rw-rw-   0        0        0   219662 2024-05-09 07:45:07.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/phemex.py
--rw-rw-rw-   0        0        0   102516 2024-05-09 07:45:11.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/poloniex.py
--rw-rw-rw-   0        0        0    78185 2024-05-09 07:45:14.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/poloniexfutures.py
--rw-rw-rw-   0        0        0    76771 2024-05-09 07:45:18.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/probit.py
--rw-rw-rw-   0        0        0    71649 2024-05-09 07:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/timex.py
--rw-rw-rw-   0        0        0   123375 2024-05-09 07:45:36.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/tokocrypto.py
--rw-rw-rw-   0        0        0    24094 2024-05-09 07:45:37.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/tradeogre.py
--rw-rw-rw-   0        0        0    82093 2024-05-09 07:45:41.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/upbit.py
--rw-rw-rw-   0        0        0   114153 2024-05-09 07:45:49.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/wavesexchange.py
--rw-rw-rw-   0        0        0    51644 2024-05-09 07:45:52.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/wazirx.py
--rw-rw-rw-   0        0        0   114999 2024-05-09 07:45:59.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/whitebit.py
--rw-rw-rw-   0        0        0   140261 2024-05-09 07:46:04.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/woo.py
--rw-rw-rw-   0        0        0    53506 2024-05-09 07:46:07.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/yobit.py
--rw-rw-rw-   0        0        0    28161 2024-05-09 07:46:09.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/zaif.py
--rw-rw-rw-   0        0        0    80877 2024-05-09 07:46:14.000000 ccxt-custom-adapter-4.3.20/ccxt/async_support/zonda.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.731414 ccxt-custom-adapter-4.3.20/ccxt/base/
--rw-rw-rw-   0        0        0     1320 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/base/__init__.py
--rw-rw-rw-   0        0        0     6634 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/base/decimal_to_precision.py
--rw-rw-rw-   0        0        0     4264 2024-05-09 09:46:30.000000 ccxt-custom-adapter-4.3.20/ccxt/base/errors.py
--rw-rw-rw-   0        0        0   276091 2024-05-09 09:46:30.000000 ccxt-custom-adapter-4.3.20/ccxt/base/exchange.py
--rw-rw-rw-   0        0        0     8565 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/base/precise.py
--rw-rw-rw-   0        0        0     8495 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/base/types.py
--rw-rw-rw-   0        0        0     1174 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.20/ccxt/bequant.py
--rw-rw-rw-   0        0        0    92174 2024-05-09 07:22:36.000000 ccxt-custom-adapter-4.3.20/ccxt/bigone.py
--rw-rw-rw-   0        0        0   617029 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.20/ccxt/binance.py
--rw-rw-rw-   0        0        0     1645 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.20/ccxt/binancecoinm.py
--rw-rw-rw-   0        0        0     9163 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.20/ccxt/binanceus.py
--rw-rw-rw-   0        0        0     2480 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.20/ccxt/binanceusdm.py
--rw-rw-rw-   0        0        0   184752 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/bingx.py
--rw-rw-rw-   0        0        0    36907 2024-05-09 07:23:14.000000 ccxt-custom-adapter-4.3.20/ccxt/bit2c.py
--rw-rw-rw-   0        0        0    41845 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.20/ccxt/bitbank.py
--rw-rw-rw-   0        0        0      478 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.20/ccxt/bitbay.py
--rw-rw-rw-   0        0        0    48137 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.20/ccxt/bitbns.py
--rw-rw-rw-   0        0        0      502 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.20/ccxt/bitcoincom.py
--rw-rw-rw-   0        0        0    72243 2024-05-09 07:23:17.000000 ccxt-custom-adapter-4.3.20/ccxt/bitfinex.py
--rw-rw-rw-   0        0        0   158424 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.20/ccxt/bitfinex2.py
--rw-rw-rw-   0        0        0    41397 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.20/ccxt/bitflyer.py
--rw-rw-rw-   0        0        0   422374 2024-05-09 07:23:57.000000 ccxt-custom-adapter-4.3.20/ccxt/bitget.py
--rw-rw-rw-   0        0        0    45534 2024-05-09 07:23:59.000000 ccxt-custom-adapter-4.3.20/ccxt/bithumb.py
--rw-rw-rw-   0        0        0   199066 2024-05-09 07:24:11.000000 ccxt-custom-adapter-4.3.20/ccxt/bitmart.py
--rw-rw-rw-   0        0        0   126437 2024-05-09 07:24:17.000000 ccxt-custom-adapter-4.3.20/ccxt/bitmex.py
--rw-rw-rw-   0        0        0    68522 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.20/ccxt/bitopro.py
--rw-rw-rw-   0        0        0      471 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.20/ccxt/bitpanda.py
--rw-rw-rw-   0        0        0   136184 2024-05-09 07:24:28.000000 ccxt-custom-adapter-4.3.20/ccxt/bitrue.py
--rw-rw-rw-   0        0        0    70885 2024-05-09 07:24:31.000000 ccxt-custom-adapter-4.3.20/ccxt/bitso.py
--rw-rw-rw-   0        0        0    92223 2024-05-09 07:24:39.000000 ccxt-custom-adapter-4.3.20/ccxt/bitstamp.py
--rw-rw-rw-   0        0        0   102026 2024-05-09 07:24:44.000000 ccxt-custom-adapter-4.3.20/ccxt/bitteam.py
--rw-rw-rw-   0        0        0    91577 2024-05-09 07:24:49.000000 ccxt-custom-adapter-4.3.20/ccxt/bitvavo.py
--rw-rw-rw-   0        0        0    20483 2024-05-09 07:24:50.000000 ccxt-custom-adapter-4.3.20/ccxt/bl3p.py
--rw-rw-rw-   0        0        0    48799 2024-05-09 07:24:52.000000 ccxt-custom-adapter-4.3.20/ccxt/blockchaincom.py
--rw-rw-rw-   0        0        0    99214 2024-05-09 07:24:57.000000 ccxt-custom-adapter-4.3.20/ccxt/blofin.py
--rw-rw-rw-   0        0        0    36701 2024-05-09 07:24:58.000000 ccxt-custom-adapter-4.3.20/ccxt/btcalpha.py
--rw-rw-rw-   0        0        0    23492 2024-05-09 07:24:59.000000 ccxt-custom-adapter-4.3.20/ccxt/btcbox.py
--rw-rw-rw-   0        0        0    51484 2024-05-09 07:25:01.000000 ccxt-custom-adapter-4.3.20/ccxt/btcmarkets.py
--rw-rw-rw-   0        0        0    36657 2024-05-09 07:25:02.000000 ccxt-custom-adapter-4.3.20/ccxt/btcturk.py
--rw-rw-rw-   0        0        0   410949 2024-05-09 07:25:35.000000 ccxt-custom-adapter-4.3.20/ccxt/bybit.py
--rw-rw-rw-   0        0        0    69930 2024-05-09 07:25:37.000000 ccxt-custom-adapter-4.3.20/ccxt/cex.py
--rw-rw-rw-   0        0        0   211993 2024-05-09 07:25:49.000000 ccxt-custom-adapter-4.3.20/ccxt/coinbase.py
--rw-rw-rw-   0        0        0    87240 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/coinbaseinternational.py
--rw-rw-rw-   0        0        0    78671 2024-05-09 07:25:53.000000 ccxt-custom-adapter-4.3.20/ccxt/coinbasepro.py
--rw-rw-rw-   0        0        0    35664 2024-05-09 07:25:56.000000 ccxt-custom-adapter-4.3.20/ccxt/coincheck.py
--rw-rw-rw-   0        0        0   259648 2024-05-09 07:26:08.000000 ccxt-custom-adapter-4.3.20/ccxt/coinex.py
--rw-rw-rw-   0        0        0   103069 2024-05-09 07:26:14.000000 ccxt-custom-adapter-4.3.20/ccxt/coinlist.py
--rw-rw-rw-   0        0        0    45946 2024-05-09 07:26:16.000000 ccxt-custom-adapter-4.3.20/ccxt/coinmate.py
--rw-rw-rw-   0        0        0    80700 2024-05-09 07:26:20.000000 ccxt-custom-adapter-4.3.20/ccxt/coinmetro.py
--rw-rw-rw-   0        0        0    46896 2024-05-09 07:26:23.000000 ccxt-custom-adapter-4.3.20/ccxt/coinone.py
--rw-rw-rw-   0        0        0    90632 2024-05-09 07:26:29.000000 ccxt-custom-adapter-4.3.20/ccxt/coinsph.py
--rw-rw-rw-   0        0        0    23614 2024-05-09 07:26:30.000000 ccxt-custom-adapter-4.3.20/ccxt/coinspot.py
--rw-rw-rw-   0        0        0   129757 2024-05-09 07:26:38.000000 ccxt-custom-adapter-4.3.20/ccxt/cryptocom.py
--rw-rw-rw-   0        0        0    86798 2024-05-09 07:26:42.000000 ccxt-custom-adapter-4.3.20/ccxt/currencycom.py
--rw-rw-rw-   0        0        0   150457 2024-05-09 07:26:48.000000 ccxt-custom-adapter-4.3.20/ccxt/delta.py
--rw-rw-rw-   0        0        0   160492 2024-05-09 07:26:59.000000 ccxt-custom-adapter-4.3.20/ccxt/deribit.py
--rw-rw-rw-   0        0        0   167970 2024-05-09 07:27:06.000000 ccxt-custom-adapter-4.3.20/ccxt/digifinex.py
--rw-rw-rw-   0        0        0   114449 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.20/ccxt/exmo.py
--rw-rw-rw-   0        0        0     1236 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.20/ccxt/fmfwio.py
--rw-rw-rw-   0        0        0   319781 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.20/ccxt/gate.py
--rw-rw-rw-   0        0        0      445 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.20/ccxt/gateio.py
--rw-rw-rw-   0        0        0    80658 2024-05-09 07:27:36.000000 ccxt-custom-adapter-4.3.20/ccxt/gemini.py
--rw-rw-rw-   0        0        0   153003 2024-05-09 07:27:45.000000 ccxt-custom-adapter-4.3.20/ccxt/hitbtc.py
--rw-rw-rw-   0        0        0      455 2024-05-09 07:27:46.000000 ccxt-custom-adapter-4.3.20/ccxt/hitbtc3.py
--rw-rw-rw-   0        0        0    75945 2024-05-09 07:27:48.000000 ccxt-custom-adapter-4.3.20/ccxt/hollaex.py
--rw-rw-rw-   0        0        0   420434 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.20/ccxt/htx.py
--rw-rw-rw-   0        0        0      438 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.20/ccxt/huobi.py
--rw-rw-rw-   0        0        0    87968 2024-05-09 07:28:56.000000 ccxt-custom-adapter-4.3.20/ccxt/huobijp.py
--rw-rw-rw-   0        0        0    99839 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/hyperliquid.py
--rw-rw-rw-   0        0        0    23278 2024-05-09 09:46:28.000000 ccxt-custom-adapter-4.3.20/ccxt/idax.py
--rw-rw-rw-   0        0        0    72998 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.20/ccxt/idex.py
--rw-rw-rw-   0        0        0    32175 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.20/ccxt/independentreserve.py
--rw-rw-rw-   0        0        0    51921 2024-05-09 07:43:24.000000 ccxt-custom-adapter-4.3.20/ccxt/indodax.py
--rw-rw-rw-   0        0        0   125449 2024-05-09 07:43:27.000000 ccxt-custom-adapter-4.3.20/ccxt/kraken.py
--rw-rw-rw-   0        0        0   116796 2024-05-09 07:43:30.000000 ccxt-custom-adapter-4.3.20/ccxt/krakenfutures.py
--rw-rw-rw-   0        0        0   217703 2024-05-09 07:43:38.000000 ccxt-custom-adapter-4.3.20/ccxt/kucoin.py
--rw-rw-rw-   0        0        0   124292 2024-05-09 07:43:39.000000 ccxt-custom-adapter-4.3.20/ccxt/kucoinfutures.py
--rw-rw-rw-   0        0        0    95991 2024-05-09 07:43:41.000000 ccxt-custom-adapter-4.3.20/ccxt/kuna.py
--rw-rw-rw-   0        0        0    79057 2024-05-09 07:43:42.000000 ccxt-custom-adapter-4.3.20/ccxt/latoken.py
--rw-rw-rw-   0        0        0   115175 2024-05-09 07:43:44.000000 ccxt-custom-adapter-4.3.20/ccxt/lbank.py
--rw-rw-rw-   0        0        0    45887 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.20/ccxt/luno.py
--rw-rw-rw-   0        0        0    51070 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.20/ccxt/lykke.py
--rw-rw-rw-   0        0        0    35339 2024-05-09 07:43:46.000000 ccxt-custom-adapter-4.3.20/ccxt/mercado.py
--rw-rw-rw-   0        0        0   240775 2024-05-09 07:43:52.000000 ccxt-custom-adapter-4.3.20/ccxt/mexc.py
--rw-rw-rw-   0        0        0   108601 2024-05-09 07:43:58.000000 ccxt-custom-adapter-4.3.20/ccxt/ndax.py
--rw-rw-rw-   0        0        0    64305 2024-05-09 07:44:00.000000 ccxt-custom-adapter-4.3.20/ccxt/novadax.py
--rw-rw-rw-   0        0        0    37860 2024-05-09 07:44:01.000000 ccxt-custom-adapter-4.3.20/ccxt/oceanex.py
--rw-rw-rw-   0        0        0   151116 2024-05-09 07:44:14.000000 ccxt-custom-adapter-4.3.20/ccxt/okcoin.py
--rw-rw-rw-   0        0        0   376037 2024-05-09 07:44:50.000000 ccxt-custom-adapter-4.3.20/ccxt/okx.py
--rw-rw-rw-   0        0        0    88113 2024-05-09 07:44:52.000000 ccxt-custom-adapter-4.3.20/ccxt/onetrading.py
--rw-rw-rw-   0        0        0    54213 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.20/ccxt/p2b.py
--rw-rw-rw-   0        0        0    24209 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.20/ccxt/paymium.py
--rw-rw-rw-   0        0        0   218850 2024-05-09 07:45:07.000000 ccxt-custom-adapter-4.3.20/ccxt/phemex.py
--rw-rw-rw-   0        0        0   101968 2024-05-09 07:45:11.000000 ccxt-custom-adapter-4.3.20/ccxt/poloniex.py
--rw-rw-rw-   0        0        0    77799 2024-05-09 07:45:14.000000 ccxt-custom-adapter-4.3.20/ccxt/poloniexfutures.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.838449 ccxt-custom-adapter-4.3.20/ccxt/pro/
--rw-rw-rw-   0        0        0     6999 2024-05-09 09:45:07.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/__init__.py
--rw-rw-rw-   0        0        0    27167 2024-05-09 08:11:45.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/alpaca.py
--rw-rw-rw-   0        0        0    35432 2024-05-09 08:11:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/ascendex.py
--rw-rw-rw-   0        0        0     1351 2024-05-09 08:11:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bequant.py
--rw-rw-rw-   0        0        0   152488 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/binance.py
--rw-rw-rw-   0        0        0      976 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/binancecoinm.py
--rw-rw-rw-   0        0        0     2321 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/binanceus.py
--rw-rw-rw-   0        0        0     1357 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/binanceusdm.py
--rw-rw-rw-   0        0        0    42110 2024-05-09 08:11:49.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bingx.py
--rw-rw-rw-   0        0        0     1181 2024-05-09 08:11:49.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitcoincom.py
--rw-rw-rw-   0        0        0    24826 2024-05-09 08:11:49.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitfinex.py
--rw-rw-rw-   0        0        0    42834 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitfinex2.py
--rw-rw-rw-   0        0        0    72217 2024-05-09 08:11:50.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitget.py
--rw-rw-rw-   0        0        0    16799 2024-05-09 08:11:50.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bithumb.py
--rw-rw-rw-   0        0        0    62382 2024-05-09 08:11:51.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitmart.py
--rw-rw-rw-   0        0        0    68956 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitmex.py
--rw-rw-rw-   0        0        0    18724 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitopro.py
--rw-rw-rw-   0        0        0      415 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitpanda.py
--rw-rw-rw-   0        0        0    16448 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitrue.py
--rw-rw-rw-   0        0        0    20886 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitstamp.py
--rw-rw-rw-   0        0        0    56145 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bitvavo.py
--rw-rw-rw-   0        0        0    29560 2024-05-09 08:11:53.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/blockchaincom.py
--rw-rw-rw-   0        0        0    85098 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/bybit.py
--rw-rw-rw-   0        0        0    58380 2024-05-09 08:11:53.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/cex.py
--rw-rw-rw-   0        0        0    29324 2024-05-09 08:11:54.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/coinbase.py
--rw-rw-rw-   0        0        0    25428 2024-05-09 08:11:54.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/coinbaseinternational.py
--rw-rw-rw-   0        0        0    38945 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/coinbasepro.py
--rw-rw-rw-   0        0        0     7789 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/coincheck.py
--rw-rw-rw-   0        0        0    45042 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/coinex.py
--rw-rw-rw-   0        0        0    15652 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/coinone.py
--rw-rw-rw-   0        0        0    42643 2024-05-09 08:11:56.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/cryptocom.py
--rw-rw-rw-   0        0        0    22355 2024-05-09 08:11:56.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/currencycom.py
--rw-rw-rw-   0        0        0    41035 2024-05-09 08:11:57.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/deribit.py
--rw-rw-rw-   0        0        0    24527 2024-05-09 08:11:57.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/exmo.py
--rw-rw-rw-   0        0        0    52489 2024-05-09 08:11:58.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/gate.py
--rw-rw-rw-   0        0        0      391 2024-05-09 08:11:58.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/gateio.py
--rw-rw-rw-   0        0        0    36641 2024-05-09 08:11:58.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/gemini.py
--rw-rw-rw-   0        0        0    56284 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/hitbtc.py
--rw-rw-rw-   0        0        0    21957 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/hollaex.py
--rw-rw-rw-   0        0        0    95869 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/htx.py
--rw-rw-rw-   0        0        0      385 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/huobi.py
--rw-rw-rw-   0        0        0    23174 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/huobijp.py
--rw-rw-rw-   0        0        0    20791 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/hyperliquid.py
--rw-rw-rw-   0        0        0    28282 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/idex.py
--rw-rw-rw-   0        0        0    11179 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/independentreserve.py
--rw-rw-rw-   0        0        0    60764 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/kraken.py
--rw-rw-rw-   0        0        0    63917 2024-05-09 08:12:00.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/krakenfutures.py
--rw-rw-rw-   0        0        0    50705 2024-05-09 08:12:01.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/kucoin.py
--rw-rw-rw-   0        0        0    46006 2024-05-09 08:12:02.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/kucoinfutures.py
--rw-rw-rw-   0        0        0    35105 2024-05-09 08:12:02.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/lbank.py
--rw-rw-rw-   0        0        0    12348 2024-05-09 08:12:02.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/luno.py
--rw-rw-rw-   0        0        0    43183 2024-05-09 08:12:03.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/mexc.py
--rw-rw-rw-   0        0        0    22643 2024-05-09 08:12:03.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/ndax.py
--rw-rw-rw-   0        0        0    30385 2024-05-09 08:12:03.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/okcoin.py
--rw-rw-rw-   0        0        0    69412 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/okx.py
--rw-rw-rw-   0        0        0    54634 2024-05-09 08:12:04.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/onetrading.py
--rw-rw-rw-   0        0        0    17877 2024-05-09 08:12:04.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/p2b.py
--rw-rw-rw-   0        0        0    61032 2024-05-09 08:12:05.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/phemex.py
--rw-rw-rw-   0        0        0    51235 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/poloniex.py
--rw-rw-rw-   0        0        0    41652 2024-05-09 08:12:05.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/poloniexfutures.py
--rw-rw-rw-   0        0        0    22822 2024-05-09 08:12:06.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/probit.py
--rw-rw-rw-   0        0        0     9654 2024-05-09 08:12:06.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/upbit.py
--rw-rw-rw-   0        0        0    30043 2024-05-09 08:12:06.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/wazirx.py
--rw-rw-rw-   0        0        0    35021 2024-05-09 08:12:07.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/whitebit.py
--rw-rw-rw-   0        0        0    42372 2024-05-09 08:12:07.000000 ccxt-custom-adapter-4.3.20/ccxt/pro/woo.py
--rw-rw-rw-   0        0        0    76379 2024-05-09 07:45:18.000000 ccxt-custom-adapter-4.3.20/ccxt/probit.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.840862 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/
--rw-rw-rw-   0        0        0       84 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.855764 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/
--rw-rw-rw-   0        0        0      594 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-rw-   0        0        0    18461 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-rw-   0        0        0     1886 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-rw-   0        0        0     6942 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-rw-   0        0        0    11336 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-rw-   0        0        0     5517 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-rw-   0        0        0    14201 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-rw-   0        0        0    13468 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-rw-   0        0        0     2572 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-rw-   0        0        0    10037 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.858191 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/
--rw-rw-rw-   0        0        0      171 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.876950 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/
--rw-rw-rw-   0        0        0      276 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-rw-   0        0        0      490 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-rw-   0        0        0     4861 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-rw-   0        0        0     6871 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-rw-   0        0        0       51 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-rw-   0        0        0    16828 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-rw-   0        0        0    20162 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-rw-   0        0        0     2941 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-rw-   0        0        0    12358 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-rw-   0        0        0      387 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-rw-   0        0        0    19329 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.880469 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-rw-   0        0        0       65 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-rw-   0        0        0     5742 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.886151 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-rw-   0        0        0     2097 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-rw-   0        0        0      426 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-rw-   0        0        0      436 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.891267 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/
--rw-rw-rw-   0        0        0       48 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.896985 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-rw-   0        0        0       80 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-rw-   0        0        0     7126 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-rw-   0        0        0      982 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-rw-   0        0        0    10588 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.903047 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-rw-   0        0        0       60 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-rw-   0        0        0     1687 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-rw-   0        0        0     1768 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.922626 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/
--rw-rw-rw-   0        0        0      913 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-rw-   0        0        0       85 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-rw-   0        0        0      191 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-rw-   0        0        0       71 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-rw-   0        0        0      117 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-rw-   0        0        0      458 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-rw-   0        0        0      173 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-rw-   0        0        0      546 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-rw-   0        0        0    20845 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.962714 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/
--rw-rw-rw-   0        0        0     2162 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-rw-   0        0        0     4364 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-rw-   0        0        0     4342 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-rw-   0        0        0     5498 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-rw-   0        0        0     3021 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.964713 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-rw-   0        0        0     6398 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-rw-   0        0        0      499 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-rw-   0        0        0     3997 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-rw-   0        0        0      199 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-rw-   0        0        0      110 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-rw-   0        0        0     2100 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-rw-   0        0        0     1826 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-rw-   0        0        0     4137 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-rw-   0        0        0     5155 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-rw-   0        0        0      842 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-rw-   0        0        0     1190 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-rw-   0        0        0     1001 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-rw-   0        0        0     1074 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.969224 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-rw-   0        0        0      325 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-rw-   0        0        0      189 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-rw-   0        0        0     1757 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.972358 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/keccak/
--rw-rw-rw-   0        0        0       45 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-rw-   0        0        0     6934 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.981438 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/
--rw-rw-rw-   0        0        0     1077 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     5629 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-rw-   0        0        0    33175 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:13.996639 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/
--rw-rw-rw-   0        0        0      385 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-rw-   0        0        0     3603 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-rw-   0        0        0    16864 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-rw-   0        0        0    19190 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-rw-   0        0        0    13084 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-rw-   0        0        0     1087 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:14.015646 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/
--rw-rw-rw-   0        0        0      374 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-rw-   0        0        0    20555 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-rw-   0        0        0    18447 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/_version.py
--rw-rw-rw-   0        0        0      997 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:14.023079 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/curried/
--rw-rw-rw-   0        0        0     2226 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-rw-   0        0        0      344 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-rw-   0        0        0      525 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-rw-   0        0        0     8955 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-rw-   0        0        0    29821 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-rw-   0        0        0    27612 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-rw-   0        0        0     1256 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-rw-   0        0        0      139 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:14.029128 ccxt-custom-adapter-4.3.20/ccxt/test/
--rw-rw-rw-   0        0        0      141 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:14.098028 ccxt-custom-adapter-4.3.20/ccxt/test/base/
--rw-rw-rw-   0        0        0     1889 2024-05-09 09:46:31.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/__init__.py
--rw-rw-rw-   0        0        0      978 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_account.py
--rw-rw-rw-   0        0        0     2931 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_balance.py
--rw-rw-rw-   0        0        0     1808 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_borrow_interest.py
--rw-rw-rw-   0        0        0     1500 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_borrow_rate.py
--rw-rw-rw-   0        0        0     1177 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_calculate_fee.py
--rw-rw-rw-   0        0        0     7702 2024-05-09 09:46:30.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_crypto.py
--rw-rw-rw-   0        0        0     4472 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_currency.py
--rw-rw-rw-   0        0        0     5634 2024-05-09 09:46:30.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_datetime.py
--rw-rw-rw-   0        0        0    20934 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-rw-   0        0        0     1402 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_deep_extend.py
--rw-rw-rw-   0        0        0     2452 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-rw-   0        0        0     3592 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-rw-   0        0        0     1351 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_funding_rate_history.py
--rw-rw-rw-   0        0        0     1332 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_last_price.py
--rw-rw-rw-   0        0        0     2289 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ledger_entry.py
--rw-rw-rw-   0        0        0     2154 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ledger_item.py
--rw-rw-rw-   0        0        0     1656 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_leverage_tier.py
--rw-rw-rw-   0        0        0      869 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_margin_mode.py
--rw-rw-rw-   0        0        0     1730 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_margin_modification.py
--rw-rw-rw-   0        0        0    11632 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_market.py
--rw-rw-rw-   0        0        0    22083 2024-05-09 09:46:30.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_number.py
--rw-rw-rw-   0        0        0     2036 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ohlcv.py
--rw-rw-rw-   0        0        0     1547 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_open_interest.py
--rw-rw-rw-   0        0        0     3964 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_order.py
--rw-rw-rw-   0        0        0     3949 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_order_book.py
--rw-rw-rw-   0        0        0     3884 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_position.py
--rw-rw-rw-   0        0        0    19998 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_shared_methods.py
--rw-rw-rw-   0        0        0      722 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_status.py
--rw-rw-rw-   0        0        0     3123 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_throttle.py
--rw-rw-rw-   0        0        0     5810 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ticker.py
--rw-rw-rw-   0        0        0     2336 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_trade.py
--rw-rw-rw-   0        0        0     1066 2024-05-09 09:47:11.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_trading_fee.py
--rw-rw-rw-   0        0        0     1434 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/ccxt/test/base/test_transaction.py
--rw-rw-rw-   0        0        0    78755 2024-05-09 09:46:31.000000 ccxt-custom-adapter-4.3.20/ccxt/test/test_async.py
--rw-rw-rw-   0        0        0    77736 2024-05-09 09:46:31.000000 ccxt-custom-adapter-4.3.20/ccxt/test/test_sync.py
--rw-rw-rw-   0        0        0    71287 2024-05-09 07:45:23.000000 ccxt-custom-adapter-4.3.20/ccxt/timex.py
--rw-rw-rw-   0        0        0   123013 2024-05-09 07:45:36.000000 ccxt-custom-adapter-4.3.20/ccxt/tokocrypto.py
--rw-rw-rw-   0        0        0    23900 2024-05-09 07:45:37.000000 ccxt-custom-adapter-4.3.20/ccxt/tradeogre.py
--rw-rw-rw-   0        0        0    81611 2024-05-09 07:45:41.000000 ccxt-custom-adapter-4.3.20/ccxt/upbit.py
--rw-rw-rw-   0        0        0   113603 2024-05-09 07:45:49.000000 ccxt-custom-adapter-4.3.20/ccxt/wavesexchange.py
--rw-rw-rw-   0        0        0    51342 2024-05-09 07:45:52.000000 ccxt-custom-adapter-4.3.20/ccxt/wazirx.py
--rw-rw-rw-   0        0        0   114379 2024-05-09 07:45:59.000000 ccxt-custom-adapter-4.3.20/ccxt/whitebit.py
--rw-rw-rw-   0        0        0   139371 2024-05-09 07:46:04.000000 ccxt-custom-adapter-4.3.20/ccxt/woo.py
--rw-rw-rw-   0        0        0    53222 2024-05-09 07:46:07.000000 ccxt-custom-adapter-4.3.20/ccxt/yobit.py
--rw-rw-rw-   0        0        0    27979 2024-05-09 07:46:09.000000 ccxt-custom-adapter-4.3.20/ccxt/zaif.py
--rw-rw-rw-   0        0        0    80563 2024-05-09 07:46:14.000000 ccxt-custom-adapter-4.3.20/ccxt/zonda.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:50:14.132767 ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/
--rw-rw-rw-   0        0        0   112518 2024-05-09 09:50:13.000000 ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    15832 2024-05-09 09:50:13.000000 ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 09:50:13.000000 ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2024-05-09 09:50:13.000000 ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-09 09:50:13.000000 ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12577 2024-05-09 09:50:09.000000 ccxt-custom-adapter-4.3.20/package.json
--rw-rw-rw-   0        0        0      226 2024-05-09 09:50:14.145306 ccxt-custom-adapter-4.3.20/setup.cfg
--rw-rw-rw-   0        0        0     3071 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.601998 ccxt-custom-adapter-4.3.21/
+-rw-rw-rw-   0        0        0     1068 2024-05-09 09:55:53.000000 ccxt-custom-adapter-4.3.21/LICENSE.txt
+-rw-rw-rw-   0        0        0      101 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/MANIFEST.in
+-rw-rw-rw-   0        0        0   112518 2024-05-09 09:59:25.600999 ccxt-custom-adapter-4.3.21/PKG-INFO
+-rw-rw-rw-   0        0        0   102253 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:24.814106 ccxt-custom-adapter-4.3.21/ccxt/
+-rw-rw-rw-   0        0        0    15834 2024-05-09 09:55:27.000000 ccxt-custom-adapter-4.3.21/ccxt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:24.971476 ccxt-custom-adapter-4.3.21/ccxt/abstract/
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/__init__.py
+-rw-rw-rw-   0        0        0     1448 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/ace.py
+-rw-rw-rw-   0        0        0    10382 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/alpaca.py
+-rw-rw-rw-   0        0        0    11394 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/ascendex.py
+-rw-rw-rw-   0        0        0    15601 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bequant.py
+-rw-rw-rw-   0        0        0     4895 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bigone.py
+-rw-rw-rw-   0        0        0    92016 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/binance.py
+-rw-rw-rw-   0        0        0    92016 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/binancecoinm.py
+-rw-rw-rw-   0        0        0    98736 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/binanceus.py
+-rw-rw-rw-   0        0        0    92016 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/binanceusdm.py
+-rw-rw-rw-   0        0        0    16032 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bingx.py
+-rw-rw-rw-   0        0        0     2830 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bit2c.py
+-rw-rw-rw-   0        0        0     2735 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitbank.py
+-rw-rw-rw-   0        0        0     5820 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitbay.py
+-rw-rw-rw-   0        0        0     4082 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitbns.py
+-rw-rw-rw-   0        0        0    15601 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitcoincom.py
+-rw-rw-rw-   0        0        0     7605 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitfinex.py
+-rw-rw-rw-   0        0        0    19194 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitfinex2.py
+-rw-rw-rw-   0        0        0     3576 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitflyer.py
+-rw-rw-rw-   0        0        0    89841 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitget.py
+-rw-rw-rw-   0        0        0     3443 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bithumb.py
+-rw-rw-rw-   0        0        0    14031 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitmart.py
+-rw-rw-rw-   0        0        0    10774 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitmex.py
+-rw-rw-rw-   0        0        0     3295 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitopro.py
+-rw-rw-rw-   0        0        0     3859 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitpanda.py
+-rw-rw-rw-   0        0        0     9379 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitrue.py
+-rw-rw-rw-   0        0        0     4025 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitso.py
+-rw-rw-rw-   0        0        0    27930 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitstamp.py
+-rw-rw-rw-   0        0        0     3478 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitteam.py
+-rw-rw-rw-   0        0        0     2357 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bitvavo.py
+-rw-rw-rw-   0        0        0     2024 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bl3p.py
+-rw-rw-rw-   0        0        0     2638 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/blockchaincom.py
+-rw-rw-rw-   0        0        0     4217 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/blofin.py
+-rw-rw-rw-   0        0        0     1380 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/btcalpha.py
+-rw-rw-rw-   0        0        0      849 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/btcbox.py
+-rw-rw-rw-   0        0        0     3690 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/btcmarkets.py
+-rw-rw-rw-   0        0        0     1777 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/btcturk.py
+-rw-rw-rw-   0        0        0    48773 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/bybit.py
+-rw-rw-rw-   0        0        0     3311 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/cex.py
+-rw-rw-rw-   0        0        0    15507 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinbase.py
+-rw-rw-rw-   0        0        0     4770 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinbaseinternational.py
+-rw-rw-rw-   0        0        0     7162 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinbasepro.py
+-rw-rw-rw-   0        0        0     3417 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coincheck.py
+-rw-rw-rw-   0        0        0    34678 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinex.py
+-rw-rw-rw-   0        0        0     6538 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinlist.py
+-rw-rw-rw-   0        0        0     6842 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinmate.py
+-rw-rw-rw-   0        0        0     3975 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinmetro.py
+-rw-rw-rw-   0        0        0     8291 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinone.py
+-rw-rw-rw-   0        0        0     8007 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinsph.py
+-rw-rw-rw-   0        0        0     2707 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/coinspot.py
+-rw-rw-rw-   0        0        0    18475 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/cryptocom.py
+-rw-rw-rw-   0        0        0     7563 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/currencycom.py
+-rw-rw-rw-   0        0        0     5107 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/delta.py
+-rw-rw-rw-   0        0        0    15499 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/deribit.py
+-rw-rw-rw-   0        0        0    11452 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/digifinex.py
+-rw-rw-rw-   0        0        0     6177 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/exmo.py
+-rw-rw-rw-   0        0        0    15601 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/fmfwio.py
+-rw-rw-rw-   0        0        0    41994 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/gate.py
+-rw-rw-rw-   0        0        0    41994 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/gateio.py
+-rw-rw-rw-   0        0        0     6915 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/gemini.py
+-rw-rw-rw-   0        0        0    15601 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/hitbtc.py
+-rw-rw-rw-   0        0        0    15601 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/hitbtc3.py
+-rw-rw-rw-   0        0        0     2906 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/hollaex.py
+-rw-rw-rw-   0        0        0    99311 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/htx.py
+-rw-rw-rw-   0        0        0    99311 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/huobi.py
+-rw-rw-rw-   0        0        0    14331 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/huobijp.py
+-rw-rw-rw-   0        0        0      240 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/hyperliquid.py
+-rw-rw-rw-   0        0        0     1743 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/idax.py
+-rw-rw-rw-   0        0        0     2129 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/idex.py
+-rw-rw-rw-   0        0        0     4165 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/independentreserve.py
+-rw-rw-rw-   0        0        0     2488 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/indodax.py
+-rw-rw-rw-   0        0        0     5877 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/kraken.py
+-rw-rw-rw-   0        0        0     3537 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/krakenfutures.py
+-rw-rw-rw-   0        0        0    25491 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/kucoin.py
+-rw-rw-rw-   0        0        0    28204 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/kucoinfutures.py
+-rw-rw-rw-   0        0        0    24579 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/kuna.py
+-rw-rw-rw-   0        0        0     7168 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/latoken.py
+-rw-rw-rw-   0        0        0     8675 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/lbank.py
+-rw-rw-rw-   0        0        0     3619 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/luno.py
+-rw-rw-rw-   0        0        0     2960 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/lykke.py
+-rw-rw-rw-   0        0        0     2357 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/mercado.py
+-rw-rw-rw-   0        0        0    25902 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/mexc.py
+-rw-rw-rw-   0        0        0    11878 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/ndax.py
+-rw-rw-rw-   0        0        0     3093 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/novadax.py
+-rw-rw-rw-   0        0        0     1721 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/oceanex.py
+-rw-rw-rw-   0        0        0     9414 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/okcoin.py
+-rw-rw-rw-   0        0        0    45891 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/okx.py
+-rw-rw-rw-   0        0        0     3859 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/onetrading.py
+-rw-rw-rw-   0        0        0     2054 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/p2b.py
+-rw-rw-rw-   0        0        0     2843 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/paymium.py
+-rw-rw-rw-   0        0        0    15203 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/phemex.py
+-rw-rw-rw-   0        0        0     8073 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/poloniex.py
+-rw-rw-rw-   0        0        0     5219 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/poloniexfutures.py
+-rw-rw-rw-   0        0        0     1969 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/probit.py
+-rw-rw-rw-   0        0        0     5875 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/timex.py
+-rw-rw-rw-   0        0        0     4094 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/tokocrypto.py
+-rw-rw-rw-   0        0        0     1372 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/tradeogre.py
+-rw-rw-rw-   0        0        0     3576 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/upbit.py
+-rw-rw-rw-   0        0        0    19631 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/wavesexchange.py
+-rw-rw-rw-   0        0        0     2782 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/wazirx.py
+-rw-rw-rw-   0        0        0    10977 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/whitebit.py
+-rw-rw-rw-   0        0        0    10368 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/woo.py
+-rw-rw-rw-   0        0        0     1339 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/yobit.py
+-rw-rw-rw-   0        0        0     3935 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/zaif.py
+-rw-rw-rw-   0        0        0     5820 2024-05-09 09:55:43.000000 ccxt-custom-adapter-4.3.21/ccxt/abstract/zonda.py
+-rw-rw-rw-   0        0        0    41656 2024-05-09 07:22:32.000000 ccxt-custom-adapter-4.3.21/ccxt/ace.py
+-rw-rw-rw-   0        0        0    47215 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/alpaca.py
+-rw-rw-rw-   0        0        0   151413 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.21/ccxt/ascendex.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.158303 ccxt-custom-adapter-4.3.21/ccxt/async_support/
+-rw-rw-rw-   0        0        0    15597 2024-05-09 09:55:27.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/__init__.py
+-rw-rw-rw-   0        0        0    41880 2024-05-09 07:22:32.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/ace.py
+-rw-rw-rw-   0        0        0    47427 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/alpaca.py
+-rw-rw-rw-   0        0        0   152201 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/ascendex.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.162917 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/
+-rw-rw-rw-   0        0        0       67 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/__init__.py
+-rw-rw-rw-   0        0        0   107440 2024-05-09 09:56:45.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/exchange.py
+-rw-rw-rw-   0        0        0     1847 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/throttler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.181165 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/
+-rw-rw-rw-   0        0        0     1791 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/__init__.py
+-rw-rw-rw-   0        0        0     5751 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-rw-   0        0        0     8100 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/cache.py
+-rw-rw-rw-   0        0        0     7289 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/client.py
+-rw-rw-rw-   0        0        0     3864 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-rw-   0        0        0     1499 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/functions.py
+-rw-rw-rw-   0        0        0     2067 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/future.py
+-rw-rw-rw-   0        0        0     2894 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/order_book.py
+-rw-rw-rw-   0        0        0     6478 2024-05-03 06:32:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-rw-   0        0        0     1188 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bequant.py
+-rw-rw-rw-   0        0        0    92628 2024-05-09 07:22:36.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bigone.py
+-rw-rw-rw-   0        0        0   619727 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/binance.py
+-rw-rw-rw-   0        0        0     1683 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/binancecoinm.py
+-rw-rw-rw-   0        0        0     9177 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/binanceus.py
+-rw-rw-rw-   0        0        0     2518 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/binanceusdm.py
+-rw-rw-rw-   0        0        0   185788 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bingx.py
+-rw-rw-rw-   0        0        0    37119 2024-05-09 07:23:14.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bit2c.py
+-rw-rw-rw-   0        0        0    42105 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitbank.py
+-rw-rw-rw-   0        0        0      492 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitbay.py
+-rw-rw-rw-   0        0        0    48391 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitbns.py
+-rw-rw-rw-   0        0        0      516 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitcoincom.py
+-rw-rw-rw-   0        0        0    72683 2024-05-09 07:23:17.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitfinex.py
+-rw-rw-rw-   0        0        0   159158 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitfinex2.py
+-rw-rw-rw-   0        0        0    41705 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitflyer.py
+-rw-rw-rw-   0        0        0   423998 2024-05-09 07:23:57.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitget.py
+-rw-rw-rw-   0        0        0    45764 2024-05-09 07:23:59.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bithumb.py
+-rw-rw-rw-   0        0        0   199986 2024-05-09 07:24:11.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitmart.py
+-rw-rw-rw-   0        0        0   127015 2024-05-09 07:24:17.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitmex.py
+-rw-rw-rw-   0        0        0    68926 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitopro.py
+-rw-rw-rw-   0        0        0      485 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitpanda.py
+-rw-rw-rw-   0        0        0   136842 2024-05-09 07:24:28.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitrue.py
+-rw-rw-rw-   0        0        0    71271 2024-05-09 07:24:31.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitso.py
+-rw-rw-rw-   0        0        0    92723 2024-05-09 07:24:39.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitstamp.py
+-rw-rw-rw-   0        0        0   102358 2024-05-09 07:24:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitteam.py
+-rw-rw-rw-   0        0        0    92011 2024-05-09 07:24:49.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bitvavo.py
+-rw-rw-rw-   0        0        0    20611 2024-05-09 07:24:50.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bl3p.py
+-rw-rw-rw-   0        0        0    49191 2024-05-09 07:24:52.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/blockchaincom.py
+-rw-rw-rw-   0        0        0    99798 2024-05-09 07:24:57.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/blofin.py
+-rw-rw-rw-   0        0        0    36979 2024-05-09 07:24:58.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/btcalpha.py
+-rw-rw-rw-   0        0        0    23686 2024-05-09 07:24:59.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/btcbox.py
+-rw-rw-rw-   0        0        0    51834 2024-05-09 07:25:01.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/btcmarkets.py
+-rw-rw-rw-   0        0        0    36875 2024-05-09 07:25:02.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/btcturk.py
+-rw-rw-rw-   0        0        0   412729 2024-05-09 07:25:35.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/bybit.py
+-rw-rw-rw-   0        0        0    70280 2024-05-09 07:25:37.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/cex.py
+-rw-rw-rw-   0        0        0   213099 2024-05-09 07:25:49.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinbase.py
+-rw-rw-rw-   0        0        0    87794 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinbaseinternational.py
+-rw-rw-rw-   0        0        0    79177 2024-05-09 07:25:53.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinbasepro.py
+-rw-rw-rw-   0        0        0    35870 2024-05-09 07:25:56.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coincheck.py
+-rw-rw-rw-   0        0        0   260942 2024-05-09 07:26:08.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinex.py
+-rw-rw-rw-   0        0        0   103557 2024-05-09 07:26:14.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinlist.py
+-rw-rw-rw-   0        0        0    46212 2024-05-09 07:26:16.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinmate.py
+-rw-rw-rw-   0        0        0    81020 2024-05-09 07:26:20.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinmetro.py
+-rw-rw-rw-   0        0        0    47138 2024-05-09 07:26:23.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinone.py
+-rw-rw-rw-   0        0        0    91066 2024-05-09 07:26:29.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinsph.py
+-rw-rw-rw-   0        0        0    23766 2024-05-09 07:26:30.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/coinspot.py
+-rw-rw-rw-   0        0        0   130329 2024-05-09 07:26:38.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/cryptocom.py
+-rw-rw-rw-   0        0        0    87220 2024-05-09 07:26:42.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/currencycom.py
+-rw-rw-rw-   0        0        0   151065 2024-05-09 07:26:48.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/delta.py
+-rw-rw-rw-   0        0        0   161268 2024-05-09 07:26:59.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/deribit.py
+-rw-rw-rw-   0        0        0   168940 2024-05-09 07:27:06.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/digifinex.py
+-rw-rw-rw-   0        0        0   115081 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/exmo.py
+-rw-rw-rw-   0        0        0     1250 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/fmfwio.py
+-rw-rw-rw-   0        0        0   321459 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/gate.py
+-rw-rw-rw-   0        0        0      459 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/gateio.py
+-rw-rw-rw-   0        0        0    81171 2024-05-09 07:27:36.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/gemini.py
+-rw-rw-rw-   0        0        0   154049 2024-05-09 07:27:45.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/hitbtc.py
+-rw-rw-rw-   0        0        0      469 2024-05-09 07:27:46.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/hitbtc3.py
+-rw-rw-rw-   0        0        0    76379 2024-05-09 07:27:48.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/hollaex.py
+-rw-rw-rw-   0        0        0   422790 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/htx.py
+-rw-rw-rw-   0        0        0      452 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/huobi.py
+-rw-rw-rw-   0        0        0    88468 2024-05-09 07:28:56.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/huobijp.py
+-rw-rw-rw-   0        0        0   100359 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/hyperliquid.py
+-rw-rw-rw-   0        0        0    23625 2024-05-09 09:56:43.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/idax.py
+-rw-rw-rw-   0        0        0    73474 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/idex.py
+-rw-rw-rw-   0        0        0    32435 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/independentreserve.py
+-rw-rw-rw-   0        0        0    52229 2024-05-09 07:43:24.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/indodax.py
+-rw-rw-rw-   0        0        0   126051 2024-05-09 07:43:27.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/kraken.py
+-rw-rw-rw-   0        0        0   117284 2024-05-09 07:43:30.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/krakenfutures.py
+-rw-rw-rw-   0        0        0   218775 2024-05-09 07:43:38.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/kucoin.py
+-rw-rw-rw-   0        0        0   124930 2024-05-09 07:43:39.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/kucoinfutures.py
+-rw-rw-rw-   0        0        0    96407 2024-05-09 07:43:41.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/kuna.py
+-rw-rw-rw-   0        0        0    79533 2024-05-09 07:43:42.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/latoken.py
+-rw-rw-rw-   0        0        0   115887 2024-05-09 07:43:44.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/lbank.py
+-rw-rw-rw-   0        0        0    46225 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/luno.py
+-rw-rw-rw-   0        0        0    51384 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/lykke.py
+-rw-rw-rw-   0        0        0    35581 2024-05-09 07:43:46.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/mercado.py
+-rw-rw-rw-   0        0        0   241953 2024-05-09 07:43:52.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/mexc.py
+-rw-rw-rw-   0        0        0   109125 2024-05-09 07:43:58.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/ndax.py
+-rw-rw-rw-   0        0        0    64673 2024-05-09 07:44:00.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/novadax.py
+-rw-rw-rw-   0        0        0    38180 2024-05-09 07:44:01.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/oceanex.py
+-rw-rw-rw-   0        0        0   151640 2024-05-09 07:44:14.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/okcoin.py
+-rw-rw-rw-   0        0        0   377624 2024-05-09 07:44:50.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/okx.py
+-rw-rw-rw-   0        0        0    88565 2024-05-09 07:44:52.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/onetrading.py
+-rw-rw-rw-   0        0        0    54455 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/p2b.py
+-rw-rw-rw-   0        0        0    24397 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/paymium.py
+-rw-rw-rw-   0        0        0   219662 2024-05-09 07:45:07.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/phemex.py
+-rw-rw-rw-   0        0        0   102516 2024-05-09 07:45:11.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/poloniex.py
+-rw-rw-rw-   0        0        0    78185 2024-05-09 07:45:14.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/poloniexfutures.py
+-rw-rw-rw-   0        0        0    76771 2024-05-09 07:45:18.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/probit.py
+-rw-rw-rw-   0        0        0    71649 2024-05-09 07:45:23.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/timex.py
+-rw-rw-rw-   0        0        0   123375 2024-05-09 07:45:36.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/tokocrypto.py
+-rw-rw-rw-   0        0        0    24094 2024-05-09 07:45:37.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/tradeogre.py
+-rw-rw-rw-   0        0        0    82093 2024-05-09 07:45:41.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/upbit.py
+-rw-rw-rw-   0        0        0   114153 2024-05-09 07:45:49.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/wavesexchange.py
+-rw-rw-rw-   0        0        0    51644 2024-05-09 07:45:52.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/wazirx.py
+-rw-rw-rw-   0        0        0   114999 2024-05-09 07:45:59.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/whitebit.py
+-rw-rw-rw-   0        0        0   140261 2024-05-09 07:46:04.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/woo.py
+-rw-rw-rw-   0        0        0    53506 2024-05-09 07:46:07.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/yobit.py
+-rw-rw-rw-   0        0        0    28161 2024-05-09 07:46:09.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/zaif.py
+-rw-rw-rw-   0        0        0    80877 2024-05-09 07:46:14.000000 ccxt-custom-adapter-4.3.21/ccxt/async_support/zonda.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.193160 ccxt-custom-adapter-4.3.21/ccxt/base/
+-rw-rw-rw-   0        0        0     1320 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/base/__init__.py
+-rw-rw-rw-   0        0        0     6634 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/base/decimal_to_precision.py
+-rw-rw-rw-   0        0        0     4264 2024-05-09 09:56:45.000000 ccxt-custom-adapter-4.3.21/ccxt/base/errors.py
+-rw-rw-rw-   0        0        0   276091 2024-05-09 09:56:45.000000 ccxt-custom-adapter-4.3.21/ccxt/base/exchange.py
+-rw-rw-rw-   0        0        0     8565 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/base/precise.py
+-rw-rw-rw-   0        0        0     8495 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/base/types.py
+-rw-rw-rw-   0        0        0     1174 2024-05-09 07:22:35.000000 ccxt-custom-adapter-4.3.21/ccxt/bequant.py
+-rw-rw-rw-   0        0        0    92174 2024-05-09 07:22:36.000000 ccxt-custom-adapter-4.3.21/ccxt/bigone.py
+-rw-rw-rw-   0        0        0   617029 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.21/ccxt/binance.py
+-rw-rw-rw-   0        0        0     1645 2024-05-09 07:23:11.000000 ccxt-custom-adapter-4.3.21/ccxt/binancecoinm.py
+-rw-rw-rw-   0        0        0     9163 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.21/ccxt/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2024-05-09 07:23:12.000000 ccxt-custom-adapter-4.3.21/ccxt/binanceusdm.py
+-rw-rw-rw-   0        0        0   184752 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/bingx.py
+-rw-rw-rw-   0        0        0    36907 2024-05-09 07:23:14.000000 ccxt-custom-adapter-4.3.21/ccxt/bit2c.py
+-rw-rw-rw-   0        0        0    41845 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.21/ccxt/bitbank.py
+-rw-rw-rw-   0        0        0      478 2024-05-09 07:23:15.000000 ccxt-custom-adapter-4.3.21/ccxt/bitbay.py
+-rw-rw-rw-   0        0        0    48137 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.21/ccxt/bitbns.py
+-rw-rw-rw-   0        0        0      502 2024-05-09 07:23:16.000000 ccxt-custom-adapter-4.3.21/ccxt/bitcoincom.py
+-rw-rw-rw-   0        0        0    72243 2024-05-09 07:23:17.000000 ccxt-custom-adapter-4.3.21/ccxt/bitfinex.py
+-rw-rw-rw-   0        0        0   158424 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.21/ccxt/bitfinex2.py
+-rw-rw-rw-   0        0        0    41397 2024-05-09 07:23:21.000000 ccxt-custom-adapter-4.3.21/ccxt/bitflyer.py
+-rw-rw-rw-   0        0        0   422374 2024-05-09 07:23:57.000000 ccxt-custom-adapter-4.3.21/ccxt/bitget.py
+-rw-rw-rw-   0        0        0    45534 2024-05-09 07:23:59.000000 ccxt-custom-adapter-4.3.21/ccxt/bithumb.py
+-rw-rw-rw-   0        0        0   199066 2024-05-09 07:24:11.000000 ccxt-custom-adapter-4.3.21/ccxt/bitmart.py
+-rw-rw-rw-   0        0        0   126437 2024-05-09 07:24:17.000000 ccxt-custom-adapter-4.3.21/ccxt/bitmex.py
+-rw-rw-rw-   0        0        0    68522 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.21/ccxt/bitopro.py
+-rw-rw-rw-   0        0        0      471 2024-05-09 07:24:20.000000 ccxt-custom-adapter-4.3.21/ccxt/bitpanda.py
+-rw-rw-rw-   0        0        0   136184 2024-05-09 07:24:28.000000 ccxt-custom-adapter-4.3.21/ccxt/bitrue.py
+-rw-rw-rw-   0        0        0    70885 2024-05-09 07:24:31.000000 ccxt-custom-adapter-4.3.21/ccxt/bitso.py
+-rw-rw-rw-   0        0        0    92223 2024-05-09 07:24:39.000000 ccxt-custom-adapter-4.3.21/ccxt/bitstamp.py
+-rw-rw-rw-   0        0        0   102026 2024-05-09 07:24:44.000000 ccxt-custom-adapter-4.3.21/ccxt/bitteam.py
+-rw-rw-rw-   0        0        0    91577 2024-05-09 07:24:49.000000 ccxt-custom-adapter-4.3.21/ccxt/bitvavo.py
+-rw-rw-rw-   0        0        0    20483 2024-05-09 07:24:50.000000 ccxt-custom-adapter-4.3.21/ccxt/bl3p.py
+-rw-rw-rw-   0        0        0    48799 2024-05-09 07:24:52.000000 ccxt-custom-adapter-4.3.21/ccxt/blockchaincom.py
+-rw-rw-rw-   0        0        0    99214 2024-05-09 07:24:57.000000 ccxt-custom-adapter-4.3.21/ccxt/blofin.py
+-rw-rw-rw-   0        0        0    36701 2024-05-09 07:24:58.000000 ccxt-custom-adapter-4.3.21/ccxt/btcalpha.py
+-rw-rw-rw-   0        0        0    23492 2024-05-09 07:24:59.000000 ccxt-custom-adapter-4.3.21/ccxt/btcbox.py
+-rw-rw-rw-   0        0        0    51484 2024-05-09 07:25:01.000000 ccxt-custom-adapter-4.3.21/ccxt/btcmarkets.py
+-rw-rw-rw-   0        0        0    36657 2024-05-09 07:25:02.000000 ccxt-custom-adapter-4.3.21/ccxt/btcturk.py
+-rw-rw-rw-   0        0        0   410949 2024-05-09 07:25:35.000000 ccxt-custom-adapter-4.3.21/ccxt/bybit.py
+-rw-rw-rw-   0        0        0    69930 2024-05-09 07:25:37.000000 ccxt-custom-adapter-4.3.21/ccxt/cex.py
+-rw-rw-rw-   0        0        0   211993 2024-05-09 07:25:49.000000 ccxt-custom-adapter-4.3.21/ccxt/coinbase.py
+-rw-rw-rw-   0        0        0    87240 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/coinbaseinternational.py
+-rw-rw-rw-   0        0        0    78671 2024-05-09 07:25:53.000000 ccxt-custom-adapter-4.3.21/ccxt/coinbasepro.py
+-rw-rw-rw-   0        0        0    35664 2024-05-09 07:25:56.000000 ccxt-custom-adapter-4.3.21/ccxt/coincheck.py
+-rw-rw-rw-   0        0        0   259648 2024-05-09 07:26:08.000000 ccxt-custom-adapter-4.3.21/ccxt/coinex.py
+-rw-rw-rw-   0        0        0   103069 2024-05-09 07:26:14.000000 ccxt-custom-adapter-4.3.21/ccxt/coinlist.py
+-rw-rw-rw-   0        0        0    45946 2024-05-09 07:26:16.000000 ccxt-custom-adapter-4.3.21/ccxt/coinmate.py
+-rw-rw-rw-   0        0        0    80700 2024-05-09 07:26:20.000000 ccxt-custom-adapter-4.3.21/ccxt/coinmetro.py
+-rw-rw-rw-   0        0        0    46896 2024-05-09 07:26:23.000000 ccxt-custom-adapter-4.3.21/ccxt/coinone.py
+-rw-rw-rw-   0        0        0    90632 2024-05-09 07:26:29.000000 ccxt-custom-adapter-4.3.21/ccxt/coinsph.py
+-rw-rw-rw-   0        0        0    23614 2024-05-09 07:26:30.000000 ccxt-custom-adapter-4.3.21/ccxt/coinspot.py
+-rw-rw-rw-   0        0        0   129757 2024-05-09 07:26:38.000000 ccxt-custom-adapter-4.3.21/ccxt/cryptocom.py
+-rw-rw-rw-   0        0        0    86798 2024-05-09 07:26:42.000000 ccxt-custom-adapter-4.3.21/ccxt/currencycom.py
+-rw-rw-rw-   0        0        0   150457 2024-05-09 07:26:48.000000 ccxt-custom-adapter-4.3.21/ccxt/delta.py
+-rw-rw-rw-   0        0        0   160492 2024-05-09 07:26:59.000000 ccxt-custom-adapter-4.3.21/ccxt/deribit.py
+-rw-rw-rw-   0        0        0   167970 2024-05-09 07:27:06.000000 ccxt-custom-adapter-4.3.21/ccxt/digifinex.py
+-rw-rw-rw-   0        0        0   114449 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.21/ccxt/exmo.py
+-rw-rw-rw-   0        0        0     1236 2024-05-09 07:27:10.000000 ccxt-custom-adapter-4.3.21/ccxt/fmfwio.py
+-rw-rw-rw-   0        0        0   319781 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.21/ccxt/gate.py
+-rw-rw-rw-   0        0        0      445 2024-05-09 07:27:31.000000 ccxt-custom-adapter-4.3.21/ccxt/gateio.py
+-rw-rw-rw-   0        0        0    80658 2024-05-09 07:27:36.000000 ccxt-custom-adapter-4.3.21/ccxt/gemini.py
+-rw-rw-rw-   0        0        0   153003 2024-05-09 07:27:45.000000 ccxt-custom-adapter-4.3.21/ccxt/hitbtc.py
+-rw-rw-rw-   0        0        0      455 2024-05-09 07:27:46.000000 ccxt-custom-adapter-4.3.21/ccxt/hitbtc3.py
+-rw-rw-rw-   0        0        0    75945 2024-05-09 07:27:48.000000 ccxt-custom-adapter-4.3.21/ccxt/hollaex.py
+-rw-rw-rw-   0        0        0   420434 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.21/ccxt/htx.py
+-rw-rw-rw-   0        0        0      438 2024-05-09 07:28:52.000000 ccxt-custom-adapter-4.3.21/ccxt/huobi.py
+-rw-rw-rw-   0        0        0    87968 2024-05-09 07:28:56.000000 ccxt-custom-adapter-4.3.21/ccxt/huobijp.py
+-rw-rw-rw-   0        0        0    99839 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/hyperliquid.py
+-rw-rw-rw-   0        0        0    23339 2024-05-09 09:56:43.000000 ccxt-custom-adapter-4.3.21/ccxt/idax.py
+-rw-rw-rw-   0        0        0    72998 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.21/ccxt/idex.py
+-rw-rw-rw-   0        0        0    32175 2024-05-09 07:43:23.000000 ccxt-custom-adapter-4.3.21/ccxt/independentreserve.py
+-rw-rw-rw-   0        0        0    51921 2024-05-09 07:43:24.000000 ccxt-custom-adapter-4.3.21/ccxt/indodax.py
+-rw-rw-rw-   0        0        0   125449 2024-05-09 07:43:27.000000 ccxt-custom-adapter-4.3.21/ccxt/kraken.py
+-rw-rw-rw-   0        0        0   116796 2024-05-09 07:43:30.000000 ccxt-custom-adapter-4.3.21/ccxt/krakenfutures.py
+-rw-rw-rw-   0        0        0   217703 2024-05-09 07:43:38.000000 ccxt-custom-adapter-4.3.21/ccxt/kucoin.py
+-rw-rw-rw-   0        0        0   124292 2024-05-09 07:43:39.000000 ccxt-custom-adapter-4.3.21/ccxt/kucoinfutures.py
+-rw-rw-rw-   0        0        0    95991 2024-05-09 07:43:41.000000 ccxt-custom-adapter-4.3.21/ccxt/kuna.py
+-rw-rw-rw-   0        0        0    79057 2024-05-09 07:43:42.000000 ccxt-custom-adapter-4.3.21/ccxt/latoken.py
+-rw-rw-rw-   0        0        0   115175 2024-05-09 07:43:44.000000 ccxt-custom-adapter-4.3.21/ccxt/lbank.py
+-rw-rw-rw-   0        0        0    45887 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.21/ccxt/luno.py
+-rw-rw-rw-   0        0        0    51070 2024-05-09 07:43:45.000000 ccxt-custom-adapter-4.3.21/ccxt/lykke.py
+-rw-rw-rw-   0        0        0    35339 2024-05-09 07:43:46.000000 ccxt-custom-adapter-4.3.21/ccxt/mercado.py
+-rw-rw-rw-   0        0        0   240775 2024-05-09 07:43:52.000000 ccxt-custom-adapter-4.3.21/ccxt/mexc.py
+-rw-rw-rw-   0        0        0   108601 2024-05-09 07:43:58.000000 ccxt-custom-adapter-4.3.21/ccxt/ndax.py
+-rw-rw-rw-   0        0        0    64305 2024-05-09 07:44:00.000000 ccxt-custom-adapter-4.3.21/ccxt/novadax.py
+-rw-rw-rw-   0        0        0    37860 2024-05-09 07:44:01.000000 ccxt-custom-adapter-4.3.21/ccxt/oceanex.py
+-rw-rw-rw-   0        0        0   151116 2024-05-09 07:44:14.000000 ccxt-custom-adapter-4.3.21/ccxt/okcoin.py
+-rw-rw-rw-   0        0        0   376037 2024-05-09 07:44:50.000000 ccxt-custom-adapter-4.3.21/ccxt/okx.py
+-rw-rw-rw-   0        0        0    88113 2024-05-09 07:44:52.000000 ccxt-custom-adapter-4.3.21/ccxt/onetrading.py
+-rw-rw-rw-   0        0        0    54213 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.21/ccxt/p2b.py
+-rw-rw-rw-   0        0        0    24209 2024-05-09 07:44:53.000000 ccxt-custom-adapter-4.3.21/ccxt/paymium.py
+-rw-rw-rw-   0        0        0   218850 2024-05-09 07:45:07.000000 ccxt-custom-adapter-4.3.21/ccxt/phemex.py
+-rw-rw-rw-   0        0        0   101968 2024-05-09 07:45:11.000000 ccxt-custom-adapter-4.3.21/ccxt/poloniex.py
+-rw-rw-rw-   0        0        0    77799 2024-05-09 07:45:14.000000 ccxt-custom-adapter-4.3.21/ccxt/poloniexfutures.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.307471 ccxt-custom-adapter-4.3.21/ccxt/pro/
+-rw-rw-rw-   0        0        0     6999 2024-05-09 09:55:27.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/__init__.py
+-rw-rw-rw-   0        0        0    27167 2024-05-09 08:11:45.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/alpaca.py
+-rw-rw-rw-   0        0        0    35432 2024-05-09 08:11:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/ascendex.py
+-rw-rw-rw-   0        0        0     1351 2024-05-09 08:11:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bequant.py
+-rw-rw-rw-   0        0        0   152488 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/binance.py
+-rw-rw-rw-   0        0        0      976 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/binancecoinm.py
+-rw-rw-rw-   0        0        0     2321 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/binanceus.py
+-rw-rw-rw-   0        0        0     1357 2024-05-09 08:11:48.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/binanceusdm.py
+-rw-rw-rw-   0        0        0    42110 2024-05-09 08:11:49.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bingx.py
+-rw-rw-rw-   0        0        0     1181 2024-05-09 08:11:49.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitcoincom.py
+-rw-rw-rw-   0        0        0    24826 2024-05-09 08:11:49.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitfinex.py
+-rw-rw-rw-   0        0        0    42834 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitfinex2.py
+-rw-rw-rw-   0        0        0    72217 2024-05-09 08:11:50.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitget.py
+-rw-rw-rw-   0        0        0    16799 2024-05-09 08:11:50.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bithumb.py
+-rw-rw-rw-   0        0        0    62382 2024-05-09 08:11:51.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitmart.py
+-rw-rw-rw-   0        0        0    68956 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitmex.py
+-rw-rw-rw-   0        0        0    18724 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitopro.py
+-rw-rw-rw-   0        0        0      415 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitpanda.py
+-rw-rw-rw-   0        0        0    16448 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitrue.py
+-rw-rw-rw-   0        0        0    20886 2024-05-09 08:11:52.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitstamp.py
+-rw-rw-rw-   0        0        0    56145 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bitvavo.py
+-rw-rw-rw-   0        0        0    29560 2024-05-09 08:11:53.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/blockchaincom.py
+-rw-rw-rw-   0        0        0    85098 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/bybit.py
+-rw-rw-rw-   0        0        0    58380 2024-05-09 08:11:53.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/cex.py
+-rw-rw-rw-   0        0        0    29324 2024-05-09 08:11:54.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/coinbase.py
+-rw-rw-rw-   0        0        0    25428 2024-05-09 08:11:54.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/coinbaseinternational.py
+-rw-rw-rw-   0        0        0    38945 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/coinbasepro.py
+-rw-rw-rw-   0        0        0     7789 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/coincheck.py
+-rw-rw-rw-   0        0        0    45042 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/coinex.py
+-rw-rw-rw-   0        0        0    15652 2024-05-09 08:11:55.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/coinone.py
+-rw-rw-rw-   0        0        0    42643 2024-05-09 08:11:56.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/cryptocom.py
+-rw-rw-rw-   0        0        0    22355 2024-05-09 08:11:56.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/currencycom.py
+-rw-rw-rw-   0        0        0    41035 2024-05-09 08:11:57.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/deribit.py
+-rw-rw-rw-   0        0        0    24527 2024-05-09 08:11:57.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/exmo.py
+-rw-rw-rw-   0        0        0    52489 2024-05-09 08:11:58.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/gate.py
+-rw-rw-rw-   0        0        0      391 2024-05-09 08:11:58.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/gateio.py
+-rw-rw-rw-   0        0        0    36641 2024-05-09 08:11:58.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/gemini.py
+-rw-rw-rw-   0        0        0    56284 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/hitbtc.py
+-rw-rw-rw-   0        0        0    21957 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/hollaex.py
+-rw-rw-rw-   0        0        0    95869 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/htx.py
+-rw-rw-rw-   0        0        0      385 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/huobi.py
+-rw-rw-rw-   0        0        0    23174 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/huobijp.py
+-rw-rw-rw-   0        0        0    20791 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/hyperliquid.py
+-rw-rw-rw-   0        0        0    28282 2024-05-09 08:11:59.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/idex.py
+-rw-rw-rw-   0        0        0    11179 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/independentreserve.py
+-rw-rw-rw-   0        0        0    60764 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/kraken.py
+-rw-rw-rw-   0        0        0    63917 2024-05-09 08:12:00.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/krakenfutures.py
+-rw-rw-rw-   0        0        0    50705 2024-05-09 08:12:01.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/kucoin.py
+-rw-rw-rw-   0        0        0    46006 2024-05-09 08:12:02.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/kucoinfutures.py
+-rw-rw-rw-   0        0        0    35105 2024-05-09 08:12:02.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/lbank.py
+-rw-rw-rw-   0        0        0    12348 2024-05-09 08:12:02.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/luno.py
+-rw-rw-rw-   0        0        0    43183 2024-05-09 08:12:03.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/mexc.py
+-rw-rw-rw-   0        0        0    22643 2024-05-09 08:12:03.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/ndax.py
+-rw-rw-rw-   0        0        0    30385 2024-05-09 08:12:03.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/okcoin.py
+-rw-rw-rw-   0        0        0    69412 2024-05-08 04:04:46.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/okx.py
+-rw-rw-rw-   0        0        0    54634 2024-05-09 08:12:04.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/onetrading.py
+-rw-rw-rw-   0        0        0    17877 2024-05-09 08:12:04.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/p2b.py
+-rw-rw-rw-   0        0        0    61032 2024-05-09 08:12:05.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/phemex.py
+-rw-rw-rw-   0        0        0    51235 2024-05-05 05:05:27.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/poloniex.py
+-rw-rw-rw-   0        0        0    41652 2024-05-09 08:12:05.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/poloniexfutures.py
+-rw-rw-rw-   0        0        0    22822 2024-05-09 08:12:06.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/probit.py
+-rw-rw-rw-   0        0        0     9654 2024-05-09 08:12:06.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/upbit.py
+-rw-rw-rw-   0        0        0    30043 2024-05-09 08:12:06.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/wazirx.py
+-rw-rw-rw-   0        0        0    35021 2024-05-09 08:12:07.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/whitebit.py
+-rw-rw-rw-   0        0        0    42372 2024-05-09 08:12:07.000000 ccxt-custom-adapter-4.3.21/ccxt/pro/woo.py
+-rw-rw-rw-   0        0        0    76379 2024-05-09 07:45:18.000000 ccxt-custom-adapter-4.3.21/ccxt/probit.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.308560 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/
+-rw-rw-rw-   0        0        0       84 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.334433 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/
+-rw-rw-rw-   0        0        0      594 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-rw-   0        0        0    18461 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-rw-   0        0        0     1886 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-rw-   0        0        0     6942 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-rw-   0        0        0    11336 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-rw-   0        0        0     5517 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-rw-   0        0        0    14201 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-rw-   0        0        0    13468 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-rw-   0        0        0     2572 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-rw-   0        0        0    10037 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.336446 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/
+-rw-rw-rw-   0        0        0      171 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.363036 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-rw-   0        0        0      276 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-rw-   0        0        0      490 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-rw-   0        0        0     4861 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-rw-   0        0        0     6871 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-rw-   0        0        0       51 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-rw-   0        0        0    16828 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-rw-   0        0        0    20162 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-rw-   0        0        0     2941 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-rw-   0        0        0    12358 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-rw-   0        0        0      387 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-rw-   0        0        0    19329 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.367789 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-rw-   0        0        0       65 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-rw-   0        0        0     5742 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.375057 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2097 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-rw-   0        0        0      426 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-rw-   0        0        0      436 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.379893 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/
+-rw-rw-rw-   0        0        0       48 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.385432 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-rw-   0        0        0       80 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-rw-   0        0        0     7126 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-rw-   0        0        0      982 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-rw-   0        0        0    10588 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.392020 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-rw-   0        0        0       60 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-rw-   0        0        0     1687 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-rw-   0        0        0     1768 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.407842 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-rw-   0        0        0      913 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-rw-   0        0        0       85 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-rw-   0        0        0      191 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-rw-   0        0        0       71 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-rw-   0        0        0      117 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-rw-   0        0        0      458 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-rw-   0        0        0      173 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-rw-   0        0        0      546 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-rw-   0        0        0    20845 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.440778 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-rw-   0        0        0     2162 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-rw-   0        0        0     4364 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-rw-   0        0        0     4342 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-rw-   0        0        0     5498 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-rw-   0        0        0     3021 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.442796 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-rw-   0        0        0     6398 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-rw-   0        0        0     3997 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-rw-   0        0        0      199 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-rw-   0        0        0      110 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-rw-   0        0        0     2100 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-rw-   0        0        0     1826 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-rw-   0        0        0     4137 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-rw-   0        0        0     5155 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-rw-   0        0        0      842 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-rw-   0        0        0     1190 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-rw-   0        0        0     1001 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-rw-   0        0        0     1074 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.446174 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-rw-   0        0        0      325 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-rw-   0        0        0      189 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-rw-   0        0        0     1757 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.450612 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/keccak/
+-rw-rw-rw-   0        0        0       45 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-rw-   0        0        0     6934 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.457866 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/
+-rw-rw-rw-   0        0        0     1077 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     5629 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-rw-   0        0        0    33175 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.470454 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/
+-rw-rw-rw-   0        0        0      385 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-rw-   0        0        0     3603 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-rw-   0        0        0    16864 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-rw-   0        0        0    19190 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-rw-   0        0        0    13084 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-rw-   0        0        0     1087 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.487749 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/
+-rw-rw-rw-   0        0        0      374 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-rw-   0        0        0    20555 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-rw-   0        0        0    18447 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-rw-   0        0        0      997 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.494023 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/curried/
+-rw-rw-rw-   0        0        0     2226 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-rw-   0        0        0      525 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-rw-   0        0        0     8955 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-rw-   0        0        0    29821 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-rw-   0        0        0    27612 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-rw-   0        0        0     1256 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-rw-   0        0        0      139 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.500477 ccxt-custom-adapter-4.3.21/ccxt/test/
+-rw-rw-rw-   0        0        0      141 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.581680 ccxt-custom-adapter-4.3.21/ccxt/test/base/
+-rw-rw-rw-   0        0        0     1889 2024-05-09 09:56:46.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/__init__.py
+-rw-rw-rw-   0        0        0      978 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_account.py
+-rw-rw-rw-   0        0        0     2931 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_balance.py
+-rw-rw-rw-   0        0        0     1808 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_borrow_interest.py
+-rw-rw-rw-   0        0        0     1500 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_borrow_rate.py
+-rw-rw-rw-   0        0        0     1177 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_calculate_fee.py
+-rw-rw-rw-   0        0        0     7702 2024-05-09 09:56:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_crypto.py
+-rw-rw-rw-   0        0        0     4472 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_currency.py
+-rw-rw-rw-   0        0        0     5634 2024-05-09 09:56:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_datetime.py
+-rw-rw-rw-   0        0        0    20934 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-rw-   0        0        0     1402 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_deep_extend.py
+-rw-rw-rw-   0        0        0     2452 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-rw-   0        0        0     3592 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-rw-   0        0        0     1351 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-rw-   0        0        0     1332 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_last_price.py
+-rw-rw-rw-   0        0        0     2289 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ledger_entry.py
+-rw-rw-rw-   0        0        0     2154 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ledger_item.py
+-rw-rw-rw-   0        0        0     1656 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_leverage_tier.py
+-rw-rw-rw-   0        0        0      869 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_margin_mode.py
+-rw-rw-rw-   0        0        0     1730 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_margin_modification.py
+-rw-rw-rw-   0        0        0    11632 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_market.py
+-rw-rw-rw-   0        0        0    22083 2024-05-09 09:56:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_number.py
+-rw-rw-rw-   0        0        0     2036 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ohlcv.py
+-rw-rw-rw-   0        0        0     1547 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_open_interest.py
+-rw-rw-rw-   0        0        0     3964 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_order.py
+-rw-rw-rw-   0        0        0     3949 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_order_book.py
+-rw-rw-rw-   0        0        0     3884 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_position.py
+-rw-rw-rw-   0        0        0    19998 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_shared_methods.py
+-rw-rw-rw-   0        0        0      722 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_status.py
+-rw-rw-rw-   0        0        0     3123 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_throttle.py
+-rw-rw-rw-   0        0        0     5810 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ticker.py
+-rw-rw-rw-   0        0        0     2336 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_trade.py
+-rw-rw-rw-   0        0        0     1066 2024-05-09 09:57:18.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_trading_fee.py
+-rw-rw-rw-   0        0        0     1434 2024-05-03 06:32:45.000000 ccxt-custom-adapter-4.3.21/ccxt/test/base/test_transaction.py
+-rw-rw-rw-   0        0        0    78755 2024-05-09 09:56:46.000000 ccxt-custom-adapter-4.3.21/ccxt/test/test_async.py
+-rw-rw-rw-   0        0        0    77736 2024-05-09 09:56:46.000000 ccxt-custom-adapter-4.3.21/ccxt/test/test_sync.py
+-rw-rw-rw-   0        0        0    71287 2024-05-09 07:45:23.000000 ccxt-custom-adapter-4.3.21/ccxt/timex.py
+-rw-rw-rw-   0        0        0   123013 2024-05-09 07:45:36.000000 ccxt-custom-adapter-4.3.21/ccxt/tokocrypto.py
+-rw-rw-rw-   0        0        0    23900 2024-05-09 07:45:37.000000 ccxt-custom-adapter-4.3.21/ccxt/tradeogre.py
+-rw-rw-rw-   0        0        0    81611 2024-05-09 07:45:41.000000 ccxt-custom-adapter-4.3.21/ccxt/upbit.py
+-rw-rw-rw-   0        0        0   113603 2024-05-09 07:45:49.000000 ccxt-custom-adapter-4.3.21/ccxt/wavesexchange.py
+-rw-rw-rw-   0        0        0    51342 2024-05-09 07:45:52.000000 ccxt-custom-adapter-4.3.21/ccxt/wazirx.py
+-rw-rw-rw-   0        0        0   114379 2024-05-09 07:45:59.000000 ccxt-custom-adapter-4.3.21/ccxt/whitebit.py
+-rw-rw-rw-   0        0        0   139371 2024-05-09 07:46:04.000000 ccxt-custom-adapter-4.3.21/ccxt/woo.py
+-rw-rw-rw-   0        0        0    53222 2024-05-09 07:46:07.000000 ccxt-custom-adapter-4.3.21/ccxt/yobit.py
+-rw-rw-rw-   0        0        0    27979 2024-05-09 07:46:09.000000 ccxt-custom-adapter-4.3.21/ccxt/zaif.py
+-rw-rw-rw-   0        0        0    80563 2024-05-09 07:46:14.000000 ccxt-custom-adapter-4.3.21/ccxt/zonda.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:59:25.596985 ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/
+-rw-rw-rw-   0        0        0   112518 2024-05-09 09:59:24.000000 ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    15832 2024-05-09 09:59:24.000000 ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 09:59:24.000000 ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2024-05-09 09:59:24.000000 ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-09 09:59:24.000000 ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12577 2024-05-09 09:59:00.000000 ccxt-custom-adapter-4.3.21/package.json
+-rw-rw-rw-   0        0        0      226 2024-05-09 09:59:25.603001 ccxt-custom-adapter-4.3.21/setup.cfg
+-rw-rw-rw-   0        0        0     3071 2024-05-09 09:58:59.000000 ccxt-custom-adapter-4.3.21/setup.py
```

### Comparing `ccxt-custom-adapter-4.3.20/LICENSE.txt` & `ccxt-custom-adapter-4.3.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/PKG-INFO` & `ccxt-custom-adapter-4.3.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt-custom-adapter
-Version: 4.3.20
+Version: 4.3.21
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
```

### Comparing `ccxt-custom-adapter-4.3.20/README.rst` & `ccxt-custom-adapter-4.3.21/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/ace.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/alpaca.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/ascendex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bequant.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bigone.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/binance.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/binancecoinm.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/binanceus.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/binanceusdm.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bingx.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bit2c.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitbay.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitbns.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitcoincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitfinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitfinex2.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitflyer.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitget.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bithumb.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitmart.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitmex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitopro.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitpanda.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitrue.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitso.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitstamp.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitteam.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bitvavo.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bl3p.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/blockchaincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/blofin.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/btcalpha.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/btcbox.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/btcmarkets.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/btcturk.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/bybit.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/cex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinbase.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinbaseinternational.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinbasepro.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coincheck.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinlist.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinmate.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinmetro.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinone.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinsph.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/coinspot.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/cryptocom.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/currencycom.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/delta.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/deribit.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/digifinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/exmo.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/fmfwio.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/gate.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/gateio.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/gemini.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/hitbtc.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/hitbtc3.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/hollaex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/htx.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/huobi.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/huobijp.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/idax.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/idax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/idex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/independentreserve.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/indodax.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/kraken.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/krakenfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/kucoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/kucoinfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/kuna.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/latoken.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/lbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/luno.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/lykke.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/mercado.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/mexc.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/ndax.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/novadax.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/oceanex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/okcoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/okx.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/onetrading.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/p2b.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/paymium.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/phemex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/poloniex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/poloniexfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/probit.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/timex.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/tokocrypto.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/tradeogre.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/upbit.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/wavesexchange.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/wazirx.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/whitebit.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/woo.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/yobit.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/zaif.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/abstract/zonda.py` & `ccxt-custom-adapter-4.3.21/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/ace.py` & `ccxt-custom-adapter-4.3.21/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/alpaca.py` & `ccxt-custom-adapter-4.3.21/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/ascendex.py` & `ccxt-custom-adapter-4.3.21/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/ace.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/alpaca.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/ascendex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/exchange.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/exchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/throttler.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/cache.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/client.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/fast_client.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/functions.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/future.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/order_book.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bequant.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bigone.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/binance.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/binancecoinm.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/binanceus.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/binanceusdm.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bingx.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bit2c.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitbns.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitcoincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitfinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitfinex2.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitflyer.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitget.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bithumb.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitmart.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitmex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitopro.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitrue.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitso.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitstamp.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitteam.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bitvavo.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bl3p.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/blockchaincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/blofin.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/btcalpha.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/btcbox.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/btcmarkets.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/btcturk.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/bybit.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/cex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinbase.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinbaseinternational.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinbasepro.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coincheck.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinlist.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinmate.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinmetro.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinone.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinsph.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/coinspot.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/cryptocom.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/currencycom.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/delta.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/deribit.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/digifinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/exmo.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/fmfwio.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/gate.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/gemini.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/hitbtc.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/hollaex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/htx.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/huobijp.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/hyperliquid.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/idax.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/idax.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,14 +430,16 @@
         # Will modify it when support for futures and margins are being implemented
         if api == 'sapiPrivate':
             paramsString = self.json(params)
             bodyString = self.json(body)
             timestamp = self.milliseconds()
             hashData = self.number_to_string(timestamp) + method + path + '?' + paramsString + bodyString
             signature = self.hmac(self.encode(hashData), self.encode(self.secret), hashlib.sha256)
+            if headers is None:
+                headers = {}
             headers['X-API-KEY'] = self.apiKey
             headers['X-API-SIGN'] = signature
             headers['X-API-TS'] = timestamp
         url += '/' + path
         if params is not None:
             url = url + '?' + self.urlencode(params)
         obj = {
```

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/idex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/independentreserve.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/indodax.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/kraken.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/krakenfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/kucoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/kucoinfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/kuna.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/latoken.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/lbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/luno.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/lykke.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/mercado.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/mexc.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/ndax.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/novadax.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/oceanex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/okcoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/okx.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/onetrading.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/p2b.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/paymium.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/phemex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/poloniex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/poloniexfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/probit.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/timex.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/tokocrypto.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/tradeogre.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/upbit.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/wavesexchange.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/wazirx.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/whitebit.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/woo.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/yobit.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/zaif.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/async_support/zonda.py` & `ccxt-custom-adapter-4.3.21/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/base/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/base/decimal_to_precision.py` & `ccxt-custom-adapter-4.3.21/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/base/errors.py` & `ccxt-custom-adapter-4.3.21/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/base/exchange.py` & `ccxt-custom-adapter-4.3.21/ccxt/base/exchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/base/precise.py` & `ccxt-custom-adapter-4.3.21/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/base/types.py` & `ccxt-custom-adapter-4.3.21/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bequant.py` & `ccxt-custom-adapter-4.3.21/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bigone.py` & `ccxt-custom-adapter-4.3.21/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/binance.py` & `ccxt-custom-adapter-4.3.21/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/binancecoinm.py` & `ccxt-custom-adapter-4.3.21/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/binanceus.py` & `ccxt-custom-adapter-4.3.21/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/binanceusdm.py` & `ccxt-custom-adapter-4.3.21/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bingx.py` & `ccxt-custom-adapter-4.3.21/ccxt/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bit2c.py` & `ccxt-custom-adapter-4.3.21/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitbns.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitfinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitfinex2.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitflyer.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitget.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bithumb.py` & `ccxt-custom-adapter-4.3.21/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitmart.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitmex.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitopro.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitrue.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitso.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitstamp.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitteam.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bitvavo.py` & `ccxt-custom-adapter-4.3.21/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bl3p.py` & `ccxt-custom-adapter-4.3.21/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/blockchaincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/blofin.py` & `ccxt-custom-adapter-4.3.21/ccxt/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/btcalpha.py` & `ccxt-custom-adapter-4.3.21/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/btcbox.py` & `ccxt-custom-adapter-4.3.21/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/btcmarkets.py` & `ccxt-custom-adapter-4.3.21/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/btcturk.py` & `ccxt-custom-adapter-4.3.21/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/bybit.py` & `ccxt-custom-adapter-4.3.21/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/cex.py` & `ccxt-custom-adapter-4.3.21/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinbase.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinbaseinternational.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinbasepro.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coincheck.py` & `ccxt-custom-adapter-4.3.21/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinlist.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinmate.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinmetro.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinone.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinsph.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/coinspot.py` & `ccxt-custom-adapter-4.3.21/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/cryptocom.py` & `ccxt-custom-adapter-4.3.21/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/currencycom.py` & `ccxt-custom-adapter-4.3.21/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/delta.py` & `ccxt-custom-adapter-4.3.21/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/deribit.py` & `ccxt-custom-adapter-4.3.21/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/digifinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/exmo.py` & `ccxt-custom-adapter-4.3.21/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/fmfwio.py` & `ccxt-custom-adapter-4.3.21/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/gate.py` & `ccxt-custom-adapter-4.3.21/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/gemini.py` & `ccxt-custom-adapter-4.3.21/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/hitbtc.py` & `ccxt-custom-adapter-4.3.21/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/hollaex.py` & `ccxt-custom-adapter-4.3.21/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/htx.py` & `ccxt-custom-adapter-4.3.21/ccxt/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/huobijp.py` & `ccxt-custom-adapter-4.3.21/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/hyperliquid.py` & `ccxt-custom-adapter-4.3.21/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/idax.py` & `ccxt-custom-adapter-4.3.21/ccxt/idax.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,16 @@
         # Will modify it when support for futures and margins are being implemented
         if api == 'sapiPrivate':
             paramsString = self.json(params)
             bodyString = self.json(body)
             timestamp = self.milliseconds()
             hashData = self.number_to_string(timestamp) + method + path + '?' + paramsString + bodyString
             signature = self.hmac(self.encode(hashData), self.encode(self.secret), hashlib.sha256)
+            if headers is None:
+                headers = {}
             headers['X-API-KEY'] = self.apiKey
             headers['X-API-SIGN'] = signature
             headers['X-API-TS'] = timestamp
         url += '/' + path
         if params is not None:
             url = url + '?' + self.urlencode(params)
         obj = {
```

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/idex.py` & `ccxt-custom-adapter-4.3.21/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/independentreserve.py` & `ccxt-custom-adapter-4.3.21/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/indodax.py` & `ccxt-custom-adapter-4.3.21/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/kraken.py` & `ccxt-custom-adapter-4.3.21/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/krakenfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/kucoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/kucoinfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/kuna.py` & `ccxt-custom-adapter-4.3.21/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/latoken.py` & `ccxt-custom-adapter-4.3.21/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/lbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/luno.py` & `ccxt-custom-adapter-4.3.21/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/lykke.py` & `ccxt-custom-adapter-4.3.21/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/mercado.py` & `ccxt-custom-adapter-4.3.21/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/mexc.py` & `ccxt-custom-adapter-4.3.21/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/ndax.py` & `ccxt-custom-adapter-4.3.21/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/novadax.py` & `ccxt-custom-adapter-4.3.21/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/oceanex.py` & `ccxt-custom-adapter-4.3.21/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/okcoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/okx.py` & `ccxt-custom-adapter-4.3.21/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/onetrading.py` & `ccxt-custom-adapter-4.3.21/ccxt/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/p2b.py` & `ccxt-custom-adapter-4.3.21/ccxt/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/paymium.py` & `ccxt-custom-adapter-4.3.21/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/phemex.py` & `ccxt-custom-adapter-4.3.21/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/poloniex.py` & `ccxt-custom-adapter-4.3.21/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/poloniexfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/alpaca.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/ascendex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bequant.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/binance.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/binancecoinm.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/binanceus.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/binanceusdm.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bingx.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitcoincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitfinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitfinex2.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitget.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bithumb.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitmart.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitmex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitopro.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitrue.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitstamp.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bitvavo.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/blockchaincom.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/bybit.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/cex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/coinbase.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/coinbaseinternational.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/coinbasepro.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/coincheck.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/coinex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/coinone.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/cryptocom.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/currencycom.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/deribit.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/exmo.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/gate.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/gemini.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/hitbtc.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/hollaex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/htx.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/huobijp.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/hyperliquid.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/idex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/independentreserve.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/kraken.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/krakenfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/kucoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/kucoinfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/lbank.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/luno.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/mexc.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/ndax.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/okcoin.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/okx.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/onetrading.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/p2b.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/phemex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/poloniex.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/poloniexfutures.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/probit.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/upbit.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/wazirx.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/whitebit.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/pro/woo.py` & `ccxt-custom-adapter-4.3.21/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/probit.py` & `ccxt-custom-adapter-4.3.21/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/_version.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-custom-adapter-4.3.21/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/__init__.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_account.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_balance.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_borrow_interest.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_borrow_rate.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_calculate_fee.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_crypto.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_currency.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_datetime.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_deep_extend.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_funding_rate_history.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_last_price.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ledger_entry.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ledger_item.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_leverage_tier.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_margin_mode.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_margin_modification.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_market.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_number.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ohlcv.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_open_interest.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_order.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_order_book.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_position.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_shared_methods.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_status.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_throttle.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_ticker.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_trade.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_trading_fee.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/base/test_transaction.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/test_async.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/test/test_sync.py` & `ccxt-custom-adapter-4.3.21/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/timex.py` & `ccxt-custom-adapter-4.3.21/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/tokocrypto.py` & `ccxt-custom-adapter-4.3.21/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/tradeogre.py` & `ccxt-custom-adapter-4.3.21/ccxt/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/upbit.py` & `ccxt-custom-adapter-4.3.21/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/wavesexchange.py` & `ccxt-custom-adapter-4.3.21/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/wazirx.py` & `ccxt-custom-adapter-4.3.21/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/whitebit.py` & `ccxt-custom-adapter-4.3.21/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/woo.py` & `ccxt-custom-adapter-4.3.21/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/yobit.py` & `ccxt-custom-adapter-4.3.21/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/zaif.py` & `ccxt-custom-adapter-4.3.21/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt/zonda.py` & `ccxt-custom-adapter-4.3.21/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/PKG-INFO` & `ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt-custom-adapter
-Version: 4.3.20
+Version: 4.3.21
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
```

### Comparing `ccxt-custom-adapter-4.3.20/ccxt_custom_adapter.egg-info/SOURCES.txt` & `ccxt-custom-adapter-4.3.21/ccxt_custom_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-custom-adapter-4.3.20/package.json` & `ccxt-custom-adapter-4.3.21/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'4.3.21'"}*

```diff
@@ -268,9 +268,9 @@
         "update-links": "node build/update-links",
         "validate-types": "tsx build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.3.20"
+    "version": "4.3.21"
 }
```

### Comparing `ccxt-custom-adapter-4.3.20/setup.py` & `ccxt-custom-adapter-4.3.21/setup.py`

 * *Files identical despite different names*
