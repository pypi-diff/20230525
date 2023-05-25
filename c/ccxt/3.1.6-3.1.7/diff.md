# Comparing `tmp/ccxt-3.1.6.tar.gz` & `tmp/ccxt-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-3.1.6.tar", last modified: Tue May 23 09:17:11 2023, max compression
+gzip compressed data, was "dist/ccxt-3.1.7.tar", last modified: Wed May 24 21:45:12 2023, max compression
```

## Comparing `ccxt-3.1.6.tar` & `ccxt-3.1.7.tar`

### file list

```diff
@@ -1,490 +1,490 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.477289 ccxt-3.1.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-05-23 09:17:03.000000 ccxt-3.1.6/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-23 08:51:40.000000 ccxt-3.1.6/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   113435 2023-05-23 09:17:11.477289 ccxt-3.1.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-05-23 08:51:40.000000 ccxt-3.1.6/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.389280 ccxt-3.1.6/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15625 2023-05-23 09:17:02.000000 ccxt-3.1.6/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.413283 ccxt-3.1.6/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11071 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31631 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8653 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22372 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5594 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72593 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9017 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14890 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7452 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28044 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28044 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6840 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21746 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10639 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/stex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7689 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27028 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-23 08:52:55.000000 ccxt-3.1.6/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41329 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33161 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   129270 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.449286 ccxt-3.1.6/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15428 2023-05-23 09:17:02.000000 ccxt-3.1.6/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41553 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33307 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   129884 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.449286 ccxt-3.1.6/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128826 2023-05-23 09:17:02.000000 ccxt-3.1.6/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.453287 ccxt-3.1.6/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62726 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   386604 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35688 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46227 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69752 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111979 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38049 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218411 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42790 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   132120 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   120028 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63629 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87785 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88471 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68835 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82612 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17931 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93903 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77171 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74597 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16351 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47548 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35438 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111410 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48897 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22323 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35602 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45959 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/buda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   399030 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65248 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125226 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74293 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34414 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   192757 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39252 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39709 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34679 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81496 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18912 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108780 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80003 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84440 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119560 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152866 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89266 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   222625 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69449 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62675 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117197 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69616 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   364171 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87087 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67772 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30046 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42709 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35208 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/itbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101946 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82024 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160977 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101796 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37998 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70399 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33953 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98405 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40781 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48763 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34881 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   210272 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106630 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62006 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37393 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   178258 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   268618 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24075 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   192389 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90796 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76966 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70124 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47585 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118368 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/stex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42655 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65784 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119594 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75965 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103947 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35792 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92648 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95037 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   197847 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51652 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28959 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   184533 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74326 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.453287 ccxt-3.1.6/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-05-23 09:00:40.000000 ccxt-3.1.6/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   169914 2023-05-23 09:17:02.000000 ccxt-3.1.6/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62340 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   385358 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35482 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39008 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45973 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69312 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111509 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37741 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28316 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   217537 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42572 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131482 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119564 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63261 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87333 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88097 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68449 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82190 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17785 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93397 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76761 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74167 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16241 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35160 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22489 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   110784 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48547 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22177 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35384 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45591 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/buda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   397142 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64922 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   124582 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73787 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34208 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191859 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38956 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39461 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34455 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81092 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18778 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108248 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79611 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84060 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119018 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152160 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88724 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   221799 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69001 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62241 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116511 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69194 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   362643 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86605 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67332 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29810 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42437 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34960 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/itbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101404 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81722 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160363 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101326 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37750 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70007 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33717 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97857 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40473 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48461 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34639 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   209226 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106106 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61638 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37055 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   177794 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   267588 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23887 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191805 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90296 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76598 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.469288 ccxt-3.1.6/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6359 2023-05-23 09:17:02.000000 ccxt-3.1.6/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26668 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34553 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77193 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42069 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46154 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24486 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55606 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12557 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54349 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16235 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20784 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36705 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31535 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31132 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60508 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44892 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30072 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40632 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22975 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22087 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34004 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24397 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41825 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21786 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85533 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23052 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28068 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11059 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44317 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52058 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34128 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27781 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41880 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30234 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35657 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    59782 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40520 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22635 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29862 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34279 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25030 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/pro/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69774 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47325 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/ripio.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.469288 ccxt-3.1.6/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.469288 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.469288 ccxt-3.1.6/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/static_dependencies/keccak/keccak.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117868 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/stex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.469288 ccxt-3.1.6/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.477289 ccxt-3.1.6/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-05-23 09:00:41.000000 ccxt-3.1.6/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      980 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2585 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1797 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-05-23 09:00:40.000000 ccxt-3.1.6/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2023-05-23 09:00:40.000000 ccxt-3.1.6/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1340 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2369 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11190 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22033 2023-05-23 09:00:40.000000 ccxt-3.1.6/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3225 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3985 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16118 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5658 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2023-05-23 09:01:49.000000 ccxt-3.1.6/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26934 2023-05-23 09:00:41.000000 ccxt-3.1.6/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26530 2023-05-23 09:00:41.000000 ccxt-3.1.6/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42407 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65452 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119250 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75531 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103453 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35544 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92196 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    94453 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   196728 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51368 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28777 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   183857 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74036 2023-05-23 08:51:40.000000 ccxt-3.1.6/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-23 09:17:11.389280 ccxt-3.1.6/ccxt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)   113435 2023-05-23 09:17:11.000000 ccxt-3.1.6/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11715 2023-05-23 09:17:11.000000 ccxt-3.1.6/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-23 09:17:11.000000 ccxt-3.1.6/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-05-23 09:17:11.000000 ccxt-3.1.6/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-05-23 09:17:11.000000 ccxt-3.1.6/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8568 2023-05-23 09:17:03.000000 ccxt-3.1.6/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-05-23 09:17:11.481289 ccxt-3.1.6/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-05-23 08:51:40.000000 ccxt-3.1.6/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.939150 ccxt-3.1.7/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-05-24 21:45:05.000000 ccxt-3.1.7/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-24 21:19:12.000000 ccxt-3.1.7/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113435 2023-05-24 21:45:12.943151 ccxt-3.1.7/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-05-24 21:19:12.000000 ccxt-3.1.7/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.851142 ccxt-3.1.7/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15625 2023-05-24 21:45:04.000000 ccxt-3.1.7/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.879145 ccxt-3.1.7/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11071 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69166 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31631 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8653 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22372 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5594 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72593 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9017 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14890 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7452 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28044 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28044 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6840 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21746 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10639 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/stex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7689 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27028 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-24 21:20:30.000000 ccxt-3.1.7/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41329 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33161 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129270 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.915148 ccxt-3.1.7/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15428 2023-05-24 21:45:04.000000 ccxt-3.1.7/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41553 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33307 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129884 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.915148 ccxt-3.1.7/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128826 2023-05-24 21:45:04.000000 ccxt-3.1.7/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.919148 ccxt-3.1.7/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62726 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   386604 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35688 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46227 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69752 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111979 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38049 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218411 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42790 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   132120 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   120028 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63629 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87785 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88471 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68835 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82612 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17931 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93903 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77171 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74597 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16351 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47548 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35438 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111410 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48897 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22323 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35602 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45959 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/buda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   399274 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65248 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125226 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74293 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34414 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   192757 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39252 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39709 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34679 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81496 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18912 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108780 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80003 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84440 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119560 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152866 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89266 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   222625 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69449 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62675 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117197 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69616 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   364171 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87087 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67772 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30046 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42709 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35208 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/itbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101946 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82024 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160977 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101796 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37998 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70399 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33953 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98405 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40781 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48763 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34881 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   210856 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106630 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62006 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37393 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178258 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   268618 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24075 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   193380 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90796 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76966 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70124 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47585 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118368 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/stex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42655 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65784 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119594 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75965 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103947 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35792 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92648 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95037 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   197847 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51652 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28959 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   184533 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74326 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.919148 ccxt-3.1.7/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-05-24 21:28:14.000000 ccxt-3.1.7/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   169914 2023-05-24 21:45:04.000000 ccxt-3.1.7/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62340 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   385358 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35482 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39008 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45973 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69312 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111509 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37741 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28316 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217537 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42572 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131482 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119564 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63261 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87333 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88097 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68449 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82190 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17785 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93397 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76761 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74167 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16241 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35160 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22489 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110784 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48547 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22177 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35384 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45591 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/buda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   397386 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64922 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   124582 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73787 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34208 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191859 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38956 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39461 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34455 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81092 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18778 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108248 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79611 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84060 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119018 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152160 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88724 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   221799 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69001 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62241 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116511 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69194 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   362643 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86605 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67332 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29810 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42437 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34960 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/itbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101404 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81722 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160363 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101326 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37750 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70007 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33717 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97857 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40473 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48461 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34639 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   209810 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106106 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61638 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37055 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   177794 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   267588 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23887 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   192790 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90296 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76598 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.931150 ccxt-3.1.7/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6359 2023-05-24 21:45:04.000000 ccxt-3.1.7/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26668 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34553 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77193 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42069 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46154 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24486 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55606 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12557 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54349 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16235 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20784 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36705 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31535 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31132 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60508 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44892 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30072 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40632 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22975 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22087 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34004 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24397 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41825 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21786 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85533 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23052 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28068 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11059 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44317 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52058 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34128 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27781 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41882 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30234 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35657 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59782 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40520 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22635 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29862 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34279 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25030 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/pro/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69774 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47325 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/ripio.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.931150 ccxt-3.1.7/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.935150 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.935150 ccxt-3.1.7/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/static_dependencies/keccak/keccak.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117868 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/stex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.935150 ccxt-3.1.7/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.939150 ccxt-3.1.7/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-05-24 21:28:15.000000 ccxt-3.1.7/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      980 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2585 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1797 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-05-24 21:28:15.000000 ccxt-3.1.7/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2023-05-24 21:28:15.000000 ccxt-3.1.7/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1340 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2369 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11190 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22033 2023-05-24 21:28:15.000000 ccxt-3.1.7/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3225 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3985 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16118 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      783 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5658 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2023-05-24 21:29:25.000000 ccxt-3.1.7/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26934 2023-05-24 21:28:15.000000 ccxt-3.1.7/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26530 2023-05-24 21:28:15.000000 ccxt-3.1.7/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42407 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65452 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119250 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75531 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103453 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35544 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92196 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94453 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   196728 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51368 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28777 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   183857 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74036 2023-05-24 21:19:12.000000 ccxt-3.1.7/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-24 21:45:12.855142 ccxt-3.1.7/ccxt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113435 2023-05-24 21:45:12.000000 ccxt-3.1.7/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11715 2023-05-24 21:45:12.000000 ccxt-3.1.7/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-24 21:45:12.000000 ccxt-3.1.7/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-05-24 21:45:12.000000 ccxt-3.1.7/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-05-24 21:45:12.000000 ccxt-3.1.7/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8568 2023-05-24 21:45:04.000000 ccxt-3.1.7/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-05-24 21:45:12.943151 ccxt-3.1.7/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-05-24 21:19:12.000000 ccxt-3.1.7/setup.py
```

### Comparing `ccxt-3.1.6/LICENSE.txt` & `ccxt-3.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/PKG-INFO` & `ccxt-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 3.1.6
+Version: 3.1.7
 Summary: A JavaScript / Python / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -228,21 +228,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.1.6/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@3.1.6/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.1.7/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@3.1.7/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.1.6/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.1.7/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-3.1.6/README.rst` & `ccxt-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/__init__.py` & `ccxt-3.1.7/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-3.1.6/ccxt/abstract/ace.py` & `ccxt-3.1.7/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/alpaca.py` & `ccxt-3.1.7/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/ascendex.py` & `ccxt-3.1.7/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bequant.py` & `ccxt-3.1.7/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bigone.py` & `ccxt-3.1.7/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/binance.py` & `ccxt-3.1.7/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/binancecoinm.py` & `ccxt-3.1.7/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/binanceus.py` & `ccxt-3.1.7/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/binanceusdm.py` & `ccxt-3.1.7/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bit2c.py` & `ccxt-3.1.7/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitbank.py` & `ccxt-3.1.7/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitbay.py` & `ccxt-3.1.7/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitbns.py` & `ccxt-3.1.7/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitcoincom.py` & `ccxt-3.1.7/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitfinex.py` & `ccxt-3.1.7/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitfinex2.py` & `ccxt-3.1.7/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitflyer.py` & `ccxt-3.1.7/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitforex.py` & `ccxt-3.1.7/ccxt/abstract/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitget.py` & `ccxt-3.1.7/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bithumb.py` & `ccxt-3.1.7/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitmart.py` & `ccxt-3.1.7/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitmex.py` & `ccxt-3.1.7/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitopro.py` & `ccxt-3.1.7/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitpanda.py` & `ccxt-3.1.7/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitrue.py` & `ccxt-3.1.7/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitso.py` & `ccxt-3.1.7/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitstamp.py` & `ccxt-3.1.7/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitstamp1.py` & `ccxt-3.1.7/ccxt/abstract/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bittrex.py` & `ccxt-3.1.7/ccxt/abstract/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bitvavo.py` & `ccxt-3.1.7/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bkex.py` & `ccxt-3.1.7/ccxt/abstract/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bl3p.py` & `ccxt-3.1.7/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/blockchaincom.py` & `ccxt-3.1.7/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/btcalpha.py` & `ccxt-3.1.7/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/btcbox.py` & `ccxt-3.1.7/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/btcex.py` & `ccxt-3.1.7/ccxt/abstract/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/btcmarkets.py` & `ccxt-3.1.7/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/btctradeua.py` & `ccxt-3.1.7/ccxt/abstract/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/btcturk.py` & `ccxt-3.1.7/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/bybit.py` & `ccxt-3.1.7/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/cex.py` & `ccxt-3.1.7/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinbase.py` & `ccxt-3.1.7/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinbaseprime.py` & `ccxt-3.1.7/ccxt/abstract/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinbasepro.py` & `ccxt-3.1.7/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coincheck.py` & `ccxt-3.1.7/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinex.py` & `ccxt-3.1.7/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinfalcon.py` & `ccxt-3.1.7/ccxt/abstract/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinmate.py` & `ccxt-3.1.7/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinone.py` & `ccxt-3.1.7/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinsph.py` & `ccxt-3.1.7/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/coinspot.py` & `ccxt-3.1.7/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/cryptocom.py` & `ccxt-3.1.7/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/currencycom.py` & `ccxt-3.1.7/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/delta.py` & `ccxt-3.1.7/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/deribit.py` & `ccxt-3.1.7/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/digifinex.py` & `ccxt-3.1.7/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/exmo.py` & `ccxt-3.1.7/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/fmfwio.py` & `ccxt-3.1.7/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/gate.py` & `ccxt-3.1.7/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/gateio.py` & `ccxt-3.1.7/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/gemini.py` & `ccxt-3.1.7/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/hitbtc.py` & `ccxt-3.1.7/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/hitbtc3.py` & `ccxt-3.1.7/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/hollaex.py` & `ccxt-3.1.7/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/huobi.py` & `ccxt-3.1.7/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/huobijp.py` & `ccxt-3.1.7/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/huobipro.py` & `ccxt-3.1.7/ccxt/abstract/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/idex.py` & `ccxt-3.1.7/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/independentreserve.py` & `ccxt-3.1.7/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/indodax.py` & `ccxt-3.1.7/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/kraken.py` & `ccxt-3.1.7/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/krakenfutures.py` & `ccxt-3.1.7/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/kucoin.py` & `ccxt-3.1.7/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/kucoinfutures.py` & `ccxt-3.1.7/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/kuna.py` & `ccxt-3.1.7/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/latoken.py` & `ccxt-3.1.7/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/lbank.py` & `ccxt-3.1.7/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/lbank2.py` & `ccxt-3.1.7/ccxt/abstract/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/luno.py` & `ccxt-3.1.7/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/lykke.py` & `ccxt-3.1.7/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/mercado.py` & `ccxt-3.1.7/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/mexc.py` & `ccxt-3.1.7/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/mexc3.py` & `ccxt-3.1.7/ccxt/abstract/mexc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/ndax.py` & `ccxt-3.1.7/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/novadax.py` & `ccxt-3.1.7/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/oceanex.py` & `ccxt-3.1.7/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/okcoin.py` & `ccxt-3.1.7/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/okex.py` & `ccxt-3.1.7/ccxt/abstract/okex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/okex5.py` & `ccxt-3.1.7/ccxt/abstract/okex5.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/okx.py` & `ccxt-3.1.7/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/paymium.py` & `ccxt-3.1.7/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/phemex.py` & `ccxt-3.1.7/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/poloniex.py` & `ccxt-3.1.7/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/poloniexfutures.py` & `ccxt-3.1.7/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/probit.py` & `ccxt-3.1.7/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/stex.py` & `ccxt-3.1.7/ccxt/abstract/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/tidex.py` & `ccxt-3.1.7/ccxt/abstract/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/timex.py` & `ccxt-3.1.7/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/tokocrypto.py` & `ccxt-3.1.7/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/upbit.py` & `ccxt-3.1.7/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/wavesexchange.py` & `ccxt-3.1.7/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/wazirx.py` & `ccxt-3.1.7/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/whitebit.py` & `ccxt-3.1.7/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/woo.py` & `ccxt-3.1.7/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/xt.py` & `ccxt-3.1.7/ccxt/abstract/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/yobit.py` & `ccxt-3.1.7/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/zaif.py` & `ccxt-3.1.7/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/abstract/zonda.py` & `ccxt-3.1.7/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/ace.py` & `ccxt-3.1.7/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/alpaca.py` & `ccxt-3.1.7/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/ascendex.py` & `ccxt-3.1.7/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/__init__.py` & `ccxt-3.1.7/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-3.1.6/ccxt/async_support/ace.py` & `ccxt-3.1.7/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/alpaca.py` & `ccxt-3.1.7/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/ascendex.py` & `ccxt-3.1.7/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/exchange.py` & `ccxt-3.1.7/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-3.1.6/ccxt/async_support/base/throttler.py` & `ccxt-3.1.7/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/__init__.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/cache.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/client.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/fast_client.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/functions.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/order_book.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-3.1.7/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bequant.py` & `ccxt-3.1.7/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bigone.py` & `ccxt-3.1.7/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/binance.py` & `ccxt-3.1.7/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/binancecoinm.py` & `ccxt-3.1.7/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/binanceus.py` & `ccxt-3.1.7/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/binanceusdm.py` & `ccxt-3.1.7/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bit2c.py` & `ccxt-3.1.7/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitbank.py` & `ccxt-3.1.7/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitbns.py` & `ccxt-3.1.7/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitfinex.py` & `ccxt-3.1.7/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitfinex2.py` & `ccxt-3.1.7/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitflyer.py` & `ccxt-3.1.7/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitforex.py` & `ccxt-3.1.7/ccxt/async_support/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitget.py` & `ccxt-3.1.7/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bithumb.py` & `ccxt-3.1.7/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitmart.py` & `ccxt-3.1.7/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitmex.py` & `ccxt-3.1.7/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitopro.py` & `ccxt-3.1.7/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitpanda.py` & `ccxt-3.1.7/ccxt/async_support/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitrue.py` & `ccxt-3.1.7/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitso.py` & `ccxt-3.1.7/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitstamp.py` & `ccxt-3.1.7/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitstamp1.py` & `ccxt-3.1.7/ccxt/async_support/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bittrex.py` & `ccxt-3.1.7/ccxt/async_support/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bitvavo.py` & `ccxt-3.1.7/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bkex.py` & `ccxt-3.1.7/ccxt/async_support/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bl3p.py` & `ccxt-3.1.7/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/blockchaincom.py` & `ccxt-3.1.7/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/btcalpha.py` & `ccxt-3.1.7/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/btcbox.py` & `ccxt-3.1.7/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/btcex.py` & `ccxt-3.1.7/ccxt/async_support/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/btcmarkets.py` & `ccxt-3.1.7/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/btctradeua.py` & `ccxt-3.1.7/ccxt/async_support/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/btcturk.py` & `ccxt-3.1.7/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/buda.py` & `ccxt-3.1.7/ccxt/async_support/buda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/bybit.py` & `ccxt-3.1.7/ccxt/async_support/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -22788,2153 +22788,2168 @@
 00059030: 2020 2020 2020 2020 2274 696d 6522 3a20          "time": 
 00059040: 3136 3732 3035 3335 3438 3537 390a 2020  1672053548579.  
 00059050: 2020 2020 2020 2320 2020 2020 7d0a 2020        #     }.  
 00059060: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
 00059070: 7265 7375 6c74 203d 2073 656c 662e 7361  result = self.sa
 00059080: 6665 5f76 616c 7565 2872 6573 706f 6e73  fe_value(respons
 00059090: 652c 2027 7265 7375 6c74 272c 207b 7d29  e, 'result', {})
-000590a0: 0a20 2020 2020 2020 2069 6420 3d20 7365  .        id = se
-000590b0: 6c66 2e73 6166 655f 7374 7269 6e67 2872  lf.safe_string(r
-000590c0: 6573 756c 742c 2027 7379 6d62 6f6c 2729  esult, 'symbol')
-000590d0: 0a20 2020 2020 2020 206d 6172 6b65 7420  .        market 
-000590e0: 3d20 7365 6c66 2e73 6166 655f 6d61 726b  = self.safe_mark
-000590f0: 6574 2869 642c 206d 6172 6b65 742c 204e  et(id, market, N
-00059100: 6f6e 652c 2027 636f 6e74 7261 6374 2729  one, 'contract')
-00059110: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00059120: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-00059130: 7265 7375 6c74 2c20 276c 6973 7427 2c20  result, 'list', 
-00059140: 5b5d 290a 2020 2020 2020 2020 7265 7475  []).        retu
-00059150: 726e 2073 656c 662e 7061 7273 655f 6f70  rn self.parse_op
-00059160: 656e 5f69 6e74 6572 6573 7473 2864 6174  en_interests(dat
-00059170: 612c 206d 6172 6b65 742c 2073 696e 6365  a, market, since
-00059180: 2c20 6c69 6d69 7429 0a0a 2020 2020 6173  , limit)..    as
-00059190: 796e 6320 6465 6620 6665 7463 685f 6f70  ync def fetch_op
-000591a0: 656e 5f69 6e74 6572 6573 7428 7365 6c66  en_interest(self
-000591b0: 2c20 7379 6d62 6f6c 3a20 7374 722c 2070  , symbol: str, p
-000591c0: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
-000591d0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-000591e0: 6574 7269 6576 6573 2074 6865 206f 7065  etrieves the ope
-000591f0: 6e20 696e 7465 7265 7374 206f 6620 6120  n interest of a 
-00059200: 6465 7269 7661 7469 7665 2074 7261 6469  derivative tradi
-00059210: 6e67 2070 6169 720a 2020 2020 2020 2020  ng pair.        
-00059220: 7365 6520 6874 7470 733a 2f2f 6279 6269  see https://bybi
-00059230: 742d 6578 6368 616e 6765 2e67 6974 6875  t-exchange.githu
-00059240: 622e 696f 2f64 6f63 732f 7635 2f6d 6172  b.io/docs/v5/mar
-00059250: 6b65 742f 6f70 656e 2d69 6e74 6572 6573  ket/open-interes
-00059260: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-00059270: 2073 7472 2073 796d 626f 6c3a 2055 6e69   str symbol: Uni
-00059280: 6669 6564 2043 4358 5420 6d61 726b 6574  fied CCXT market
-00059290: 2073 796d 626f 6c0a 2020 2020 2020 2020   symbol.        
-000592a0: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
-000592b0: 6d73 3a20 6578 6368 616e 6765 2073 7065  ms: exchange spe
-000592c0: 6369 6669 6320 7061 7261 6d65 7465 7273  cific parameters
-000592d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000592e0: 7374 727c 4e6f 6e65 2070 6172 616d 735b  str|None params[
-000592f0: 2769 6e74 6572 7661 6c27 5d3a 2035 6d2c  'interval']: 5m,
-00059300: 2031 356d 2c20 3330 6d2c 2031 682c 2034   15m, 30m, 1h, 4
-00059310: 682c 2031 640a 2020 2020 2020 2020 3a70  h, 1d.        :p
-00059320: 6172 616d 2073 7472 7c4e 6f6e 6520 7061  aram str|None pa
-00059330: 7261 6d73 5b27 6361 7465 676f 7279 275d  rams['category']
-00059340: 3a20 226c 696e 6561 7222 206f 7220 2269  : "linear" or "i
-00059350: 6e76 6572 7365 220a 2020 2020 2020 2020  nverse".        
-00059360: 3a72 6574 7572 6e73 2064 6963 747d 2061  :returns dict} a
-00059370: 6e20 6f70 656e 2069 6e74 6572 6573 7420  n open interest 
-00059380: 7374 7275 6374 7572 657b 406c 696e 6b20  structure{@link 
-00059390: 6874 7470 733a 2f2f 646f 6373 2e63 6378  https://docs.ccx
-000593a0: 742e 636f 6d2f 232f 3f69 643d 696e 7465  t.com/#/?id=inte
-000593b0: 7265 7374 2d68 6973 746f 7279 2d73 7472  rest-history-str
-000593c0: 7563 7475 7265 3a0a 2020 2020 2020 2020  ucture:.        
-000593d0: 2222 220a 2020 2020 2020 2020 6177 6169  """.        awai
-000593e0: 7420 7365 6c66 2e6c 6f61 645f 6d61 726b  t self.load_mark
-000593f0: 6574 7328 290a 2020 2020 2020 2020 6d61  ets().        ma
-00059400: 726b 6574 203d 2073 656c 662e 6d61 726b  rket = self.mark
-00059410: 6574 2873 796d 626f 6c29 0a20 2020 2020  et(symbol).     
-00059420: 2020 2069 6620 6e6f 7420 6d61 726b 6574     if not market
-00059430: 5b27 636f 6e74 7261 6374 275d 3a0a 2020  ['contract']:.  
-00059440: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00059450: 4261 6452 6571 7565 7374 2873 656c 662e  BadRequest(self.
-00059460: 6964 202b 2027 2066 6574 6368 4f70 656e  id + ' fetchOpen
-00059470: 496e 7465 7265 7374 2829 2073 7570 706f  Interest() suppo
-00059480: 7274 7320 636f 6e74 7261 6374 206d 6172  rts contract mar
-00059490: 6b65 7473 206f 6e6c 7927 290a 2020 2020  kets only').    
-000594a0: 2020 2020 7469 6d65 6672 616d 6520 3d20      timeframe = 
-000594b0: 7365 6c66 2e73 6166 655f 7374 7269 6e67  self.safe_string
-000594c0: 2870 6172 616d 732c 2027 696e 7465 7276  (params, 'interv
-000594d0: 616c 272c 2027 3168 2729 0a20 2020 2020  al', '1h').     
-000594e0: 2020 2069 6e74 6572 7661 6c73 203d 2073     intervals = s
-000594f0: 656c 662e 7361 6665 5f76 616c 7565 2873  elf.safe_value(s
-00059500: 656c 662e 6f70 7469 6f6e 732c 2027 696e  elf.options, 'in
-00059510: 7465 7276 616c 7327 290a 2020 2020 2020  tervals').      
-00059520: 2020 696e 7465 7276 616c 203d 2073 656c    interval = sel
-00059530: 662e 7361 6665 5f73 7472 696e 6728 696e  f.safe_string(in
-00059540: 7465 7276 616c 732c 2074 696d 6566 7261  tervals, timefra
-00059550: 6d65 2920 2023 2035 6d69 6e2c 3135 6d69  me)  # 5min,15mi
-00059560: 6e2c 3330 6d69 6e2c 3168 2c34 682c 3164  n,30min,1h,4h,1d
-00059570: 0a20 2020 2020 2020 2069 6620 696e 7465  .        if inte
-00059580: 7276 616c 2069 7320 4e6f 6e65 3a0a 2020  rval is None:.  
-00059590: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000595a0: 4261 6452 6571 7565 7374 2873 656c 662e  BadRequest(self.
-000595b0: 6964 202b 2027 2066 6574 6368 4f70 656e  id + ' fetchOpen
-000595c0: 496e 7465 7265 7374 2829 2063 616e 6e6f  Interest() canno
-000595d0: 7420 7573 6520 7468 6520 2720 2b20 7469  t use the ' + ti
-000595e0: 6d65 6672 616d 6520 2b20 2720 7469 6d65  meframe + ' time
-000595f0: 6672 616d 6527 290a 2020 2020 2020 2020  frame').        
-00059600: 7375 6254 7970 6520 3d20 276c 696e 6561  subType = 'linea
-00059610: 7227 2069 6620 6d61 726b 6574 5b27 6c69  r' if market['li
-00059620: 6e65 6172 275d 2065 6c73 6520 2769 6e76  near'] else 'inv
-00059630: 6572 7365 270a 2020 2020 2020 2020 6361  erse'.        ca
-00059640: 7465 676f 7279 203d 2073 656c 662e 7361  tegory = self.sa
-00059650: 6665 5f73 7472 696e 6728 7061 7261 6d73  fe_string(params
-00059660: 2c20 2763 6174 6567 6f72 7927 2c20 7375  , 'category', su
-00059670: 6254 7970 6529 0a20 2020 2020 2020 2072  bType).        r
-00059680: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
-00059690: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
-000596a0: 206d 6172 6b65 745b 2769 6427 5d2c 0a20   market['id'],. 
-000596b0: 2020 2020 2020 2020 2020 2027 696e 7465             'inte
-000596c0: 7276 616c 5469 6d65 273a 2069 6e74 6572  rvalTime': inter
-000596d0: 7661 6c2c 0a20 2020 2020 2020 2020 2020  val,.           
-000596e0: 2027 6361 7465 676f 7279 273a 2063 6174   'category': cat
-000596f0: 6567 6f72 792c 0a20 2020 2020 2020 207d  egory,.        }
-00059700: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00059710: 6520 3d20 6177 6169 7420 7365 6c66 2e70  e = await self.p
-00059720: 7562 6c69 6347 6574 5635 4d61 726b 6574  ublicGetV5Market
-00059730: 4f70 656e 496e 7465 7265 7374 2873 656c  OpenInterest(sel
-00059740: 662e 6578 7465 6e64 2872 6571 7565 7374  f.extend(request
-00059750: 2c20 7061 7261 6d73 2929 0a20 2020 2020  , params)).     
-00059760: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-00059770: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
-00059780: 2020 2020 2020 2022 7265 7443 6f64 6522         "retCode"
-00059790: 3a20 302c 0a20 2020 2020 2020 2023 2020  : 0,.        #  
-000597a0: 2020 2020 2020 2022 7265 744d 7367 223a         "retMsg":
-000597b0: 2022 4f4b 222c 0a20 2020 2020 2020 2023   "OK",.        #
-000597c0: 2020 2020 2020 2020 2022 7265 7375 6c74           "result
-000597d0: 223a 207b 0a20 2020 2020 2020 2023 2020  ": {.        #  
-000597e0: 2020 2020 2020 2020 2020 2022 7379 6d62             "symb
-000597f0: 6f6c 223a 2022 4254 4355 5344 222c 0a20  ol": "BTCUSD",. 
-00059800: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00059810: 2020 2020 2022 6361 7465 676f 7279 223a       "category":
-00059820: 2022 696e 7665 7273 6522 2c0a 2020 2020   "inverse",.    
-00059830: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00059840: 2020 226c 6973 7422 3a20 5b0a 2020 2020    "list": [.    
-00059850: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00059860: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00059870: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-00059880: 2020 2020 2020 226f 7065 6e49 6e74 6572        "openInter
-00059890: 6573 7422 3a20 2234 3631 3133 3433 3834  est": "461134384
-000598a0: 2e30 3030 3030 3030 3022 2c0a 2020 2020  .00000000",.    
-000598b0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-000598c0: 2020 2020 2020 2020 2020 2274 696d 6573            "times
-000598d0: 7461 6d70 223a 2022 3136 3639 3537 3134  tamp": "16695714
-000598e0: 3030 3030 3022 0a20 2020 2020 2020 2023  00000".        #
-000598f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00059900: 207d 2c0a 2020 2020 2020 2020 2320 2020   },.        #   
-00059910: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+000590a0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000590b0: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
+000590c0: 7265 7375 6c74 2c20 276c 6973 7427 2c20  result, 'list', 
+000590d0: 5b5d 290a 2020 2020 2020 2020 7061 6769  []).        pagi
+000590e0: 6e61 7469 6f6e 4375 7273 6f72 203d 2073  nationCursor = s
+000590f0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+00059100: 7265 7375 6c74 2c20 276e 6578 7450 6167  result, 'nextPag
+00059110: 6543 7572 736f 7227 290a 2020 2020 2020  eCursor').      
+00059120: 2020 6966 2028 7061 6769 6e61 7469 6f6e    if (pagination
+00059130: 4375 7273 6f72 2069 7320 6e6f 7420 4e6f  Cursor is not No
+00059140: 6e65 2920 616e 6420 286c 656e 2864 6174  ne) and (len(dat
+00059150: 6129 203e 2030 293a 0a20 2020 2020 2020  a) > 0):.       
+00059160: 2020 2020 2066 6972 7374 203d 2064 6174       first = dat
+00059170: 615b 305d 0a20 2020 2020 2020 2020 2020  a[0].           
+00059180: 2066 6972 7374 5b27 6e65 7874 5061 6765   first['nextPage
+00059190: 4375 7273 6f72 275d 203d 2070 6167 696e  Cursor'] = pagin
+000591a0: 6174 696f 6e43 7572 736f 720a 2020 2020  ationCursor.    
+000591b0: 2020 2020 2020 2020 6461 7461 5b30 5d20          data[0] 
+000591c0: 3d20 6669 7273 740a 2020 2020 2020 2020  = first.        
+000591d0: 6964 203d 2073 656c 662e 7361 6665 5f73  id = self.safe_s
+000591e0: 7472 696e 6728 7265 7375 6c74 2c20 2773  tring(result, 's
+000591f0: 796d 626f 6c27 290a 2020 2020 2020 2020  ymbol').        
+00059200: 6d61 726b 6574 203d 2073 656c 662e 7361  market = self.sa
+00059210: 6665 5f6d 6172 6b65 7428 6964 2c20 6d61  fe_market(id, ma
+00059220: 726b 6574 2c20 4e6f 6e65 2c20 2763 6f6e  rket, None, 'con
+00059230: 7472 6163 7427 290a 2020 2020 2020 2020  tract').        
+00059240: 7265 7475 726e 2073 656c 662e 7061 7273  return self.pars
+00059250: 655f 6f70 656e 5f69 6e74 6572 6573 7473  e_open_interests
+00059260: 2864 6174 612c 206d 6172 6b65 742c 2073  (data, market, s
+00059270: 696e 6365 2c20 6c69 6d69 7429 0a0a 2020  ince, limit)..  
+00059280: 2020 6173 796e 6320 6465 6620 6665 7463    async def fetc
+00059290: 685f 6f70 656e 5f69 6e74 6572 6573 7428  h_open_interest(
+000592a0: 7365 6c66 2c20 7379 6d62 6f6c 3a20 7374  self, symbol: st
+000592b0: 722c 2070 6172 616d 733d 7b7d 293a 0a20  r, params={}):. 
+000592c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000592d0: 2020 2052 6574 7269 6576 6573 2074 6865     Retrieves the
+000592e0: 206f 7065 6e20 696e 7465 7265 7374 206f   open interest o
+000592f0: 6620 6120 6465 7269 7661 7469 7665 2074  f a derivative t
+00059300: 7261 6469 6e67 2070 6169 720a 2020 2020  rading pair.    
+00059310: 2020 2020 7365 6520 6874 7470 733a 2f2f      see https://
+00059320: 6279 6269 742d 6578 6368 616e 6765 2e67  bybit-exchange.g
+00059330: 6974 6875 622e 696f 2f64 6f63 732f 7635  ithub.io/docs/v5
+00059340: 2f6d 6172 6b65 742f 6f70 656e 2d69 6e74  /market/open-int
+00059350: 6572 6573 740a 2020 2020 2020 2020 3a70  erest.        :p
+00059360: 6172 616d 2073 7472 2073 796d 626f 6c3a  aram str symbol:
+00059370: 2055 6e69 6669 6564 2043 4358 5420 6d61   Unified CCXT ma
+00059380: 726b 6574 2073 796d 626f 6c0a 2020 2020  rket symbol.    
+00059390: 2020 2020 3a70 6172 616d 2064 6963 7420      :param dict 
+000593a0: 7061 7261 6d73 3a20 6578 6368 616e 6765  params: exchange
+000593b0: 2073 7065 6369 6669 6320 7061 7261 6d65   specific parame
+000593c0: 7465 7273 0a20 2020 2020 2020 203a 7061  ters.        :pa
+000593d0: 7261 6d20 7374 727c 4e6f 6e65 2070 6172  ram str|None par
+000593e0: 616d 735b 2769 6e74 6572 7661 6c27 5d3a  ams['interval']:
+000593f0: 2035 6d2c 2031 356d 2c20 3330 6d2c 2031   5m, 15m, 30m, 1
+00059400: 682c 2034 682c 2031 640a 2020 2020 2020  h, 4h, 1d.      
+00059410: 2020 3a70 6172 616d 2073 7472 7c4e 6f6e    :param str|Non
+00059420: 6520 7061 7261 6d73 5b27 6361 7465 676f  e params['catego
+00059430: 7279 275d 3a20 226c 696e 6561 7222 206f  ry']: "linear" o
+00059440: 7220 2269 6e76 6572 7365 220a 2020 2020  r "inverse".    
+00059450: 2020 2020 3a72 6574 7572 6e73 2064 6963      :returns dic
+00059460: 747d 2061 6e20 6f70 656e 2069 6e74 6572  t} an open inter
+00059470: 6573 7420 7374 7275 6374 7572 657b 406c  est structure{@l
+00059480: 696e 6b20 6874 7470 733a 2f2f 646f 6373  ink https://docs
+00059490: 2e63 6378 742e 636f 6d2f 232f 3f69 643d  .ccxt.com/#/?id=
+000594a0: 696e 7465 7265 7374 2d68 6973 746f 7279  interest-history
+000594b0: 2d73 7472 7563 7475 7265 3a0a 2020 2020  -structure:.    
+000594c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000594d0: 6177 6169 7420 7365 6c66 2e6c 6f61 645f  await self.load_
+000594e0: 6d61 726b 6574 7328 290a 2020 2020 2020  markets().      
+000594f0: 2020 6d61 726b 6574 203d 2073 656c 662e    market = self.
+00059500: 6d61 726b 6574 2873 796d 626f 6c29 0a20  market(symbol). 
+00059510: 2020 2020 2020 2069 6620 6e6f 7420 6d61         if not ma
+00059520: 726b 6574 5b27 636f 6e74 7261 6374 275d  rket['contract']
+00059530: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00059540: 6973 6520 4261 6452 6571 7565 7374 2873  ise BadRequest(s
+00059550: 656c 662e 6964 202b 2027 2066 6574 6368  elf.id + ' fetch
+00059560: 4f70 656e 496e 7465 7265 7374 2829 2073  OpenInterest() s
+00059570: 7570 706f 7274 7320 636f 6e74 7261 6374  upports contract
+00059580: 206d 6172 6b65 7473 206f 6e6c 7927 290a   markets only').
+00059590: 2020 2020 2020 2020 7469 6d65 6672 616d          timefram
+000595a0: 6520 3d20 7365 6c66 2e73 6166 655f 7374  e = self.safe_st
+000595b0: 7269 6e67 2870 6172 616d 732c 2027 696e  ring(params, 'in
+000595c0: 7465 7276 616c 272c 2027 3168 2729 0a20  terval', '1h'). 
+000595d0: 2020 2020 2020 2069 6e74 6572 7661 6c73         intervals
+000595e0: 203d 2073 656c 662e 7361 6665 5f76 616c   = self.safe_val
+000595f0: 7565 2873 656c 662e 6f70 7469 6f6e 732c  ue(self.options,
+00059600: 2027 696e 7465 7276 616c 7327 290a 2020   'intervals').  
+00059610: 2020 2020 2020 696e 7465 7276 616c 203d        interval =
+00059620: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
+00059630: 6728 696e 7465 7276 616c 732c 2074 696d  g(intervals, tim
+00059640: 6566 7261 6d65 2920 2023 2035 6d69 6e2c  eframe)  # 5min,
+00059650: 3135 6d69 6e2c 3330 6d69 6e2c 3168 2c34  15min,30min,1h,4
+00059660: 682c 3164 0a20 2020 2020 2020 2069 6620  h,1d.        if 
+00059670: 696e 7465 7276 616c 2069 7320 4e6f 6e65  interval is None
+00059680: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00059690: 6973 6520 4261 6452 6571 7565 7374 2873  ise BadRequest(s
+000596a0: 656c 662e 6964 202b 2027 2066 6574 6368  elf.id + ' fetch
+000596b0: 4f70 656e 496e 7465 7265 7374 2829 2063  OpenInterest() c
+000596c0: 616e 6e6f 7420 7573 6520 7468 6520 2720  annot use the ' 
+000596d0: 2b20 7469 6d65 6672 616d 6520 2b20 2720  + timeframe + ' 
+000596e0: 7469 6d65 6672 616d 6527 290a 2020 2020  timeframe').    
+000596f0: 2020 2020 7375 6254 7970 6520 3d20 276c      subType = 'l
+00059700: 696e 6561 7227 2069 6620 6d61 726b 6574  inear' if market
+00059710: 5b27 6c69 6e65 6172 275d 2065 6c73 6520  ['linear'] else 
+00059720: 2769 6e76 6572 7365 270a 2020 2020 2020  'inverse'.      
+00059730: 2020 6361 7465 676f 7279 203d 2073 656c    category = sel
+00059740: 662e 7361 6665 5f73 7472 696e 6728 7061  f.safe_string(pa
+00059750: 7261 6d73 2c20 2763 6174 6567 6f72 7927  rams, 'category'
+00059760: 2c20 7375 6254 7970 6529 0a20 2020 2020  , subType).     
+00059770: 2020 2072 6571 7565 7374 203d 207b 0a20     request = {. 
+00059780: 2020 2020 2020 2020 2020 2027 7379 6d62             'symb
+00059790: 6f6c 273a 206d 6172 6b65 745b 2769 6427  ol': market['id'
+000597a0: 5d2c 0a20 2020 2020 2020 2020 2020 2027  ],.            '
+000597b0: 696e 7465 7276 616c 5469 6d65 273a 2069  intervalTime': i
+000597c0: 6e74 6572 7661 6c2c 0a20 2020 2020 2020  nterval,.       
+000597d0: 2020 2020 2027 6361 7465 676f 7279 273a       'category':
+000597e0: 2063 6174 6567 6f72 792c 0a20 2020 2020   category,.     
+000597f0: 2020 207d 0a20 2020 2020 2020 2072 6573     }.        res
+00059800: 706f 6e73 6520 3d20 6177 6169 7420 7365  ponse = await se
+00059810: 6c66 2e70 7562 6c69 6347 6574 5635 4d61  lf.publicGetV5Ma
+00059820: 726b 6574 4f70 656e 496e 7465 7265 7374  rketOpenInterest
+00059830: 2873 656c 662e 6578 7465 6e64 2872 6571  (self.extend(req
+00059840: 7565 7374 2c20 7061 7261 6d73 2929 0a20  uest, params)). 
+00059850: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+00059860: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
+00059870: 2023 2020 2020 2020 2020 2022 7265 7443   #         "retC
+00059880: 6f64 6522 3a20 302c 0a20 2020 2020 2020  ode": 0,.       
+00059890: 2023 2020 2020 2020 2020 2022 7265 744d   #         "retM
+000598a0: 7367 223a 2022 4f4b 222c 0a20 2020 2020  sg": "OK",.     
+000598b0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+000598c0: 7375 6c74 223a 207b 0a20 2020 2020 2020  sult": {.       
+000598d0: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
+000598e0: 7379 6d62 6f6c 223a 2022 4254 4355 5344  symbol": "BTCUSD
+000598f0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+00059900: 2020 2020 2020 2020 2022 6361 7465 676f           "catego
+00059910: 7279 223a 2022 696e 7665 7273 6522 2c0a  ry": "inverse",.
 00059920: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00059930: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-00059940: 7065 6e49 6e74 6572 6573 7422 3a20 2234  penInterest": "4
-00059950: 3631 3133 3432 3932 2e30 3030 3030 3030  61134292.0000000
-00059960: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-00059970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00059980: 2020 2274 696d 6573 7461 6d70 223a 2022    "timestamp": "
-00059990: 3136 3639 3537 3131 3030 3030 3022 0a20  1669571100000". 
-000599a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-000599b0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000599c0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-000599d0: 205d 2c0a 2020 2020 2020 2020 2320 2020   ],.        #   
-000599e0: 2020 2020 2020 2020 2020 226e 6578 7450            "nextP
-000599f0: 6167 6543 7572 736f 7222 3a20 2222 0a20  ageCursor": "". 
-00059a00: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00059a10: 207d 2c0a 2020 2020 2020 2020 2320 2020   },.        #   
-00059a20: 2020 2020 2020 2272 6574 4578 7449 6e66        "retExtInf
-00059a30: 6f22 3a20 7b7d 2c0a 2020 2020 2020 2020  o": {},.        
-00059a40: 2320 2020 2020 2020 2020 2274 696d 6522  #         "time"
-00059a50: 3a20 3136 3732 3035 3335 3438 3537 390a  : 1672053548579.
-00059a60: 2020 2020 2020 2020 2320 2020 2020 7d0a          #     }.
-00059a70: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-00059a80: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00059a90: 7361 6665 5f76 616c 7565 2872 6573 706f  safe_value(respo
-00059aa0: 6e73 652c 2027 7265 7375 6c74 272c 207b  nse, 'result', {
-00059ab0: 7d29 0a20 2020 2020 2020 2069 6420 3d20  }).        id = 
-00059ac0: 7365 6c66 2e73 6166 655f 7374 7269 6e67  self.safe_string
-00059ad0: 2872 6573 756c 742c 2027 7379 6d62 6f6c  (result, 'symbol
-00059ae0: 2729 0a20 2020 2020 2020 206d 6172 6b65  ').        marke
-00059af0: 7420 3d20 7365 6c66 2e73 6166 655f 6d61  t = self.safe_ma
-00059b00: 726b 6574 2869 642c 206d 6172 6b65 742c  rket(id, market,
-00059b10: 204e 6f6e 652c 2027 636f 6e74 7261 6374   None, 'contract
-00059b20: 2729 0a20 2020 2020 2020 2064 6174 6120  ').        data 
-00059b30: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
-00059b40: 6528 7265 7375 6c74 2c20 276c 6973 7427  e(result, 'list'
-00059b50: 2c20 5b5d 290a 2020 2020 2020 2020 7265  , []).        re
-00059b60: 7475 726e 2073 656c 662e 7061 7273 655f  turn self.parse_
-00059b70: 6f70 656e 5f69 6e74 6572 6573 7428 6461  open_interest(da
-00059b80: 7461 5b30 5d2c 206d 6172 6b65 7429 0a0a  ta[0], market)..
-00059b90: 2020 2020 6173 796e 6320 6465 6620 6665      async def fe
-00059ba0: 7463 685f 6f70 656e 5f69 6e74 6572 6573  tch_open_interes
-00059bb0: 745f 6869 7374 6f72 7928 7365 6c66 2c20  t_history(self, 
-00059bc0: 7379 6d62 6f6c 3a20 7374 722c 2074 696d  symbol: str, tim
-00059bd0: 6566 7261 6d65 3d27 3168 272c 2073 696e  eframe='1h', sin
-00059be0: 6365 3a20 4f70 7469 6f6e 616c 5b69 6e74  ce: Optional[int
-00059bf0: 5d20 3d20 4e6f 6e65 2c20 6c69 6d69 743a  ] = None, limit:
-00059c00: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00059c10: 204e 6f6e 652c 2070 6172 616d 733d 7b7d   None, params={}
-00059c20: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00059c30: 2020 2020 2020 2047 6574 7320 7468 6520         Gets the 
-00059c40: 746f 7461 6c20 616d 6f75 6e74 206f 6620  total amount of 
-00059c50: 756e 7365 7474 6c65 6420 636f 6e74 7261  unsettled contra
-00059c60: 6374 732e 2049 6e20 6f74 6865 7220 776f  cts. In other wo
-00059c70: 7264 732c 2074 6865 2074 6f74 616c 206e  rds, the total n
-00059c80: 756d 6265 7220 6f66 2063 6f6e 7472 6163  umber of contrac
-00059c90: 7473 2068 656c 6420 696e 206f 7065 6e20  ts held in open 
-00059ca0: 706f 7369 7469 6f6e 730a 2020 2020 2020  positions.      
-00059cb0: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
-00059cc0: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
-00059cd0: 6875 622e 696f 2f64 6f63 732f 7635 2f6d  hub.io/docs/v5/m
-00059ce0: 6172 6b65 742f 6f70 656e 2d69 6e74 6572  arket/open-inter
-00059cf0: 6573 740a 2020 2020 2020 2020 3a70 6172  est.        :par
-00059d00: 616d 2073 7472 2073 796d 626f 6c3a 2055  am str symbol: U
-00059d10: 6e69 6669 6564 206d 6172 6b65 7420 7379  nified market sy
-00059d20: 6d62 6f6c 0a20 2020 2020 2020 203a 7061  mbol.        :pa
-00059d30: 7261 6d20 7374 7220 7469 6d65 6672 616d  ram str timefram
-00059d40: 653a 2022 356d 222c 2031 356d 2c20 3330  e: "5m", 15m, 30
-00059d50: 6d2c 2031 682c 2034 682c 2031 640a 2020  m, 1h, 4h, 1d.  
-00059d60: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
-00059d70: 2073 696e 6365 3a20 4e6f 7420 7573 6564   since: Not used
-00059d80: 2062 7920 4279 6269 740a 2020 2020 2020   by Bybit.      
-00059d90: 2020 3a70 6172 616d 2069 6e74 206c 696d    :param int lim
-00059da0: 6974 3a20 5468 6520 6e75 6d62 6572 206f  it: The number o
-00059db0: 6620 6f70 656e 2069 6e74 6572 6573 7420  f open interest 
-00059dc0: 7374 7275 6374 7572 6573 2074 6f20 7265  structures to re
-00059dd0: 7475 726e 2e20 4d61 7820 3230 302c 2064  turn. Max 200, d
-00059de0: 6566 6175 6c74 2035 300a 2020 2020 2020  efault 50.      
-00059df0: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
-00059e00: 7261 6d73 3a20 4578 6368 616e 6765 2073  rams: Exchange s
-00059e10: 7065 6369 6669 6320 7061 7261 6d65 7465  pecific paramete
-00059e20: 7273 0a20 2020 2020 2020 203a 7265 7475  rs.        :retu
-00059e30: 726e 733a 2041 6e20 6172 7261 7920 6f66  rns: An array of
-00059e40: 206f 7065 6e20 696e 7465 7265 7374 2073   open interest s
-00059e50: 7472 7563 7475 7265 730a 2020 2020 2020  tructures.      
-00059e60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00059e70: 2074 696d 6566 7261 6d65 203d 3d20 2731   timeframe == '1
-00059e80: 6d27 3a0a 2020 2020 2020 2020 2020 2020  m':.            
-00059e90: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
-00059ea0: 2873 656c 662e 6964 202b 2027 6665 7463  (self.id + 'fetc
-00059eb0: 684f 7065 6e49 6e74 6572 6573 7448 6973  hOpenInterestHis
-00059ec0: 746f 7279 2063 616e 6e6f 7420 7573 6520  tory cannot use 
-00059ed0: 7468 6520 316d 2074 696d 6566 7261 6d65  the 1m timeframe
-00059ee0: 2729 0a20 2020 2020 2020 2061 7761 6974  ').        await
-00059ef0: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
-00059f00: 7473 2829 0a20 2020 2020 2020 206d 6172  ts().        mar
-00059f10: 6b65 7420 3d20 7365 6c66 2e6d 6172 6b65  ket = self.marke
-00059f20: 7428 7379 6d62 6f6c 290a 2020 2020 2020  t(symbol).      
-00059f30: 2020 6966 206d 6172 6b65 745b 2773 706f    if market['spo
-00059f40: 7427 5d20 6f72 206d 6172 6b65 745b 276f  t'] or market['o
-00059f50: 7074 696f 6e27 5d3a 0a20 2020 2020 2020  ption']:.       
-00059f60: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-00059f70: 7175 6573 7428 7365 6c66 2e69 6420 2b20  quest(self.id + 
-00059f80: 2720 6665 7463 684f 7065 6e49 6e74 6572  ' fetchOpenInter
-00059f90: 6573 7448 6973 746f 7279 2829 2073 796d  estHistory() sym
-00059fa0: 626f 6c20 646f 6573 206e 6f74 2073 7570  bol does not sup
-00059fb0: 706f 7274 206d 6172 6b65 7420 2720 2b20  port market ' + 
-00059fc0: 7379 6d62 6f6c 290a 2020 2020 2020 2020  symbol).        
-00059fd0: 7265 7175 6573 7420 3d20 7b0a 2020 2020  request = {.    
-00059fe0: 2020 2020 2020 2020 2773 796d 626f 6c27          'symbol'
-00059ff0: 3a20 6d61 726b 6574 5b27 6964 275d 2c0a  : market['id'],.
-0005a000: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0005a010: 2020 6966 206c 696d 6974 2069 7320 6e6f    if limit is no
-0005a020: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0005a030: 2020 2020 7265 7175 6573 745b 276c 696d      request['lim
-0005a040: 6974 275d 203d 206c 696d 6974 0a20 2020  it'] = limit.   
-0005a050: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-0005a060: 7420 7365 6c66 2e66 6574 6368 5f64 6572  t self.fetch_der
-0005a070: 6976 6174 6976 6573 5f6f 7065 6e5f 696e  ivatives_open_in
-0005a080: 7465 7265 7374 5f68 6973 746f 7279 2873  terest_history(s
-0005a090: 796d 626f 6c2c 2074 696d 6566 7261 6d65  ymbol, timeframe
-0005a0a0: 2c20 7369 6e63 652c 206c 696d 6974 2c20  , since, limit, 
-0005a0b0: 7061 7261 6d73 290a 0a20 2020 2064 6566  params)..    def
-0005a0c0: 2070 6172 7365 5f6f 7065 6e5f 696e 7465   parse_open_inte
-0005a0d0: 7265 7374 2873 656c 662c 2069 6e74 6572  rest(self, inter
-0005a0e0: 6573 742c 206d 6172 6b65 743d 4e6f 6e65  est, market=None
-0005a0f0: 293a 0a20 2020 2020 2020 2023 0a20 2020  ):.        #.   
-0005a100: 2020 2020 2023 2020 2020 7b0a 2020 2020       #    {.    
-0005a110: 2020 2020 2320 2020 2020 2020 2022 6f70      #        "op
-0005a120: 656e 496e 7465 7265 7374 223a 2036 3437  enInterest": 647
-0005a130: 3537 2e36 3234 3030 3030 302c 0a20 2020  57.62400000,.   
-0005a140: 2020 2020 2023 2020 2020 2020 2020 2274       #        "t
-0005a150: 696d 6573 7461 6d70 223a 2031 3636 3537  imestamp": 16657
-0005a160: 3834 3830 3030 3030 2c0a 2020 2020 2020  84800000,.      
-0005a170: 2020 2320 2020 207d 0a20 2020 2020 2020    #    }.       
-0005a180: 2023 0a20 2020 2020 2020 2074 696d 6573   #.        times
-0005a190: 7461 6d70 203d 2073 656c 662e 7361 6665  tamp = self.safe
-0005a1a0: 5f69 6e74 6567 6572 2869 6e74 6572 6573  _integer(interes
-0005a1b0: 742c 2027 7469 6d65 7374 616d 7027 290a  t, 'timestamp').
-0005a1c0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-0005a1d0: 7365 6c66 2e73 6166 655f 6e75 6d62 6572  self.safe_number
-0005a1e0: 5f32 2869 6e74 6572 6573 742c 2027 6f70  _2(interest, 'op
-0005a1f0: 656e 5f69 6e74 6572 6573 7427 2c20 276f  en_interest', 'o
-0005a200: 7065 6e49 6e74 6572 6573 7427 290a 2020  penInterest').  
-0005a210: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
-0005a220: 2020 2020 2020 2020 2020 2027 7379 6d62             'symb
-0005a230: 6f6c 273a 206d 6172 6b65 745b 2773 796d  ol': market['sym
-0005a240: 626f 6c27 5d2c 0a20 2020 2020 2020 2020  bol'],.         
-0005a250: 2020 2027 6f70 656e 496e 7465 7265 7374     'openInterest
-0005a260: 416d 6f75 6e74 273a 204e 6f6e 652c 0a20  Amount': None,. 
-0005a270: 2020 2020 2020 2020 2020 2027 6f70 656e             'open
-0005a280: 496e 7465 7265 7374 5661 6c75 6527 3a20  InterestValue': 
-0005a290: 7661 6c75 652c 0a20 2020 2020 2020 2020  value,.         
-0005a2a0: 2020 2027 7469 6d65 7374 616d 7027 3a20     'timestamp': 
-0005a2b0: 7469 6d65 7374 616d 702c 0a20 2020 2020  timestamp,.     
-0005a2c0: 2020 2020 2020 2027 6461 7465 7469 6d65         'datetime
-0005a2d0: 273a 2073 656c 662e 6973 6f38 3630 3128  ': self.iso8601(
-0005a2e0: 7469 6d65 7374 616d 7029 2c0a 2020 2020  timestamp),.    
-0005a2f0: 2020 2020 2020 2020 2769 6e66 6f27 3a20          'info': 
-0005a300: 696e 7465 7265 7374 2c0a 2020 2020 2020  interest,.      
-0005a310: 2020 7d0a 0a20 2020 2061 7379 6e63 2064    }..    async d
-0005a320: 6566 2066 6574 6368 5f62 6f72 726f 775f  ef fetch_borrow_
-0005a330: 7261 7465 2873 656c 662c 2063 6f64 653a  rate(self, code:
-0005a340: 2073 7472 2c20 7061 7261 6d73 3d7b 7d29   str, params={})
-0005a350: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0005a360: 2020 2020 2020 6665 7463 6820 7468 6520        fetch the 
-0005a370: 7261 7465 206f 6620 696e 7465 7265 7374  rate of interest
-0005a380: 2074 6f20 626f 7272 6f77 2061 2063 7572   to borrow a cur
-0005a390: 7265 6e63 7920 666f 7220 6d61 7267 696e  rency for margin
-0005a3a0: 2074 7261 6469 6e67 0a20 2020 2020 2020   trading.       
-0005a3b0: 2073 6565 2068 7474 7073 3a2f 2f62 7962   see https://byb
-0005a3c0: 6974 2d65 7863 6861 6e67 652e 6769 7468  it-exchange.gith
-0005a3d0: 7562 2e69 6f2f 646f 6373 2f73 706f 742f  ub.io/docs/spot/
-0005a3e0: 7633 2f23 742d 7175 6572 7969 6e74 6572  v3/#t-queryinter
-0005a3f0: 6573 7471 756f 7461 0a20 2020 2020 2020  estquota.       
-0005a400: 203a 7061 7261 6d20 7374 7220 636f 6465   :param str code
-0005a410: 3a20 756e 6966 6965 6420 6375 7272 656e  : unified curren
-0005a420: 6379 2063 6f64 650a 2020 2020 2020 2020  cy code.        
-0005a430: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
-0005a440: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
-0005a450: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
-0005a460: 2074 6865 2062 7962 6974 2061 7069 2065   the bybit api e
-0005a470: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
-0005a480: 3a72 6574 7572 6e73 2064 6963 743a 2061  :returns dict: a
-0005a490: 2060 626f 7272 6f77 2072 6174 6520 7374   `borrow rate st
-0005a4a0: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
-0005a4b0: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
-0005a4c0: 2f3f 6964 3d62 6f72 726f 772d 7261 7465  /?id=borrow-rate
-0005a4d0: 2d73 7472 7563 7475 7265 3e60 0a20 2020  -structure>`.   
-0005a4e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0005a4f0: 2061 7761 6974 2073 656c 662e 6c6f 6164   await self.load
-0005a500: 5f6d 6172 6b65 7473 2829 0a20 2020 2020  _markets().     
-0005a510: 2020 2063 7572 7265 6e63 7920 3d20 7365     currency = se
-0005a520: 6c66 2e63 7572 7265 6e63 7928 636f 6465  lf.currency(code
-0005a530: 290a 2020 2020 2020 2020 7265 7175 6573  ).        reques
-0005a540: 7420 3d20 7b0a 2020 2020 2020 2020 2020  t = {.          
-0005a550: 2020 2763 6f69 6e27 3a20 6375 7272 656e    'coin': curren
-0005a560: 6379 5b27 6964 275d 2c0a 2020 2020 2020  cy['id'],.      
-0005a570: 2020 7d0a 2020 2020 2020 2020 7265 7370    }.        resp
-0005a580: 6f6e 7365 203d 2061 7761 6974 2073 656c  onse = await sel
-0005a590: 662e 7072 6976 6174 6547 6574 5370 6f74  f.privateGetSpot
-0005a5a0: 5633 5072 6976 6174 6543 726f 7373 4d61  V3PrivateCrossMa
-0005a5b0: 7267 696e 4c6f 616e 496e 666f 2873 656c  rginLoanInfo(sel
-0005a5c0: 662e 6578 7465 6e64 2872 6571 7565 7374  f.extend(request
-0005a5d0: 2c20 7061 7261 6d73 2929 0a20 2020 2020  , params)).     
-0005a5e0: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-0005a5f0: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-0005a600: 2020 2020 2020 2272 6574 436f 6465 223a        "retCode":
-0005a610: 2022 3022 2c0a 2020 2020 2020 2020 2320   "0",.        # 
-0005a620: 2020 2020 2020 2020 2272 6574 4d73 6722          "retMsg"
-0005a630: 3a20 2273 7563 6365 7373 222c 0a20 2020  : "success",.   
-0005a640: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005a650: 7265 7375 6c74 223a 207b 0a20 2020 2020  result": {.     
-0005a660: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005a670: 2022 636f 696e 223a 2022 5553 4454 222c   "coin": "USDT",
-0005a680: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005a690: 2020 2020 2020 2022 696e 7465 7265 7374         "interest
-0005a6a0: 5261 7465 223a 2022 302e 3030 3031 3037  Rate": "0.000107
-0005a6b0: 3030 3030 3030 222c 0a20 2020 2020 2020  000000",.       
-0005a6c0: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
-0005a6d0: 6c6f 616e 4162 6c65 416d 6f75 6e74 223a  loanAbleAmount":
-0005a6e0: 2022 222c 0a20 2020 2020 2020 2023 2020   "",.        #  
-0005a6f0: 2020 2020 2020 2020 2020 2022 6d61 784c             "maxL
-0005a700: 6f61 6e41 6d6f 756e 7422 3a20 2237 3939  oanAmount": "799
-0005a710: 3939 2e39 3939 220a 2020 2020 2020 2020  99.999".        
-0005a720: 2320 2020 2020 2020 2020 7d2c 0a20 2020  #         },.   
-0005a730: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005a740: 7265 7445 7874 496e 666f 223a 206e 756c  retExtInfo": nul
-0005a750: 6c2c 0a20 2020 2020 2020 2023 2020 2020  l,.        #    
-0005a760: 2020 2020 2022 7469 6d65 223a 2022 3136       "time": "16
-0005a770: 3636 3733 3434 3930 3737 3822 0a20 2020  66734490778".   
-0005a780: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-0005a790: 2020 2020 2023 0a20 2020 2020 2020 2064       #.        d
-0005a7a0: 6174 6120 3d20 7365 6c66 2e73 6166 655f  ata = self.safe_
-0005a7b0: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
-0005a7c0: 2772 6573 756c 7427 2c20 7b7d 290a 2020  'result', {}).  
-0005a7d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0005a7e0: 662e 7061 7273 655f 626f 7272 6f77 5f72  f.parse_borrow_r
-0005a7f0: 6174 6528 6461 7461 2c20 6375 7272 656e  ate(data, curren
-0005a800: 6379 290a 0a20 2020 2064 6566 2070 6172  cy)..    def par
-0005a810: 7365 5f62 6f72 726f 775f 7261 7465 2873  se_borrow_rate(s
-0005a820: 656c 662c 2069 6e66 6f2c 2063 7572 7265  elf, info, curre
-0005a830: 6e63 793d 4e6f 6e65 293a 0a20 2020 2020  ncy=None):.     
-0005a840: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-0005a850: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
-0005a860: 2020 2020 2020 2022 636f 696e 223a 2022         "coin": "
-0005a870: 5553 4454 222c 0a20 2020 2020 2020 2023  USDT",.        #
-0005a880: 2020 2020 2020 2020 2022 696e 7465 7265           "intere
-0005a890: 7374 5261 7465 223a 2022 302e 3030 3031  stRate": "0.0001
-0005a8a0: 3037 3030 3030 3030 222c 0a20 2020 2020  07000000",.     
-0005a8b0: 2020 2023 2020 2020 2020 2020 2022 6c6f     #         "lo
-0005a8c0: 616e 4162 6c65 416d 6f75 6e74 223a 2022  anAbleAmount": "
-0005a8d0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005a8e0: 2020 2020 2022 6d61 784c 6f61 6e41 6d6f       "maxLoanAmo
-0005a8f0: 756e 7422 3a20 2237 3939 3939 2e39 3939  unt": "79999.999
-0005a900: 220a 2020 2020 2020 2020 2320 2020 2020  ".        #     
-0005a910: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
-0005a920: 2020 2020 7469 6d65 7374 616d 7020 3d20      timestamp = 
-0005a930: 7365 6c66 2e6d 696c 6c69 7365 636f 6e64  self.millisecond
-0005a940: 7328 290a 2020 2020 2020 2020 6375 7272  s().        curr
-0005a950: 656e 6379 4964 203d 2073 656c 662e 7361  encyId = self.sa
-0005a960: 6665 5f73 7472 696e 6728 696e 666f 2c20  fe_string(info, 
-0005a970: 2763 6f69 6e27 290a 2020 2020 2020 2020  'coin').        
-0005a980: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-0005a990: 2020 2020 2027 6375 7272 656e 6379 273a       'currency':
-0005a9a0: 2073 656c 662e 7361 6665 5f63 7572 7265   self.safe_curre
-0005a9b0: 6e63 795f 636f 6465 2863 7572 7265 6e63  ncy_code(currenc
-0005a9c0: 7949 642c 2063 7572 7265 6e63 7929 2c0a  yId, currency),.
-0005a9d0: 2020 2020 2020 2020 2020 2020 2772 6174              'rat
-0005a9e0: 6527 3a20 7365 6c66 2e73 6166 655f 6e75  e': self.safe_nu
-0005a9f0: 6d62 6572 2869 6e66 6f2c 2027 696e 7465  mber(info, 'inte
-0005aa00: 7265 7374 5261 7465 2729 2c0a 2020 2020  restRate'),.    
-0005aa10: 2020 2020 2020 2020 2770 6572 696f 6427          'period'
-0005aa20: 3a20 3836 3430 3030 3030 2c20 2023 2044  : 86400000,  # D
-0005aa30: 6169 6c79 0a20 2020 2020 2020 2020 2020  aily.           
-0005aa40: 2027 7469 6d65 7374 616d 7027 3a20 7469   'timestamp': ti
-0005aa50: 6d65 7374 616d 702c 0a20 2020 2020 2020  mestamp,.       
-0005aa60: 2020 2020 2027 6461 7465 7469 6d65 273a       'datetime':
-0005aa70: 2073 656c 662e 6973 6f38 3630 3128 7469   self.iso8601(ti
-0005aa80: 6d65 7374 616d 7029 2c0a 2020 2020 2020  mestamp),.      
-0005aa90: 2020 2020 2020 2769 6e66 6f27 3a20 696e        'info': in
-0005aaa0: 666f 2c0a 2020 2020 2020 2020 7d0a 0a20  fo,.        }.. 
-0005aab0: 2020 2061 7379 6e63 2064 6566 2066 6574     async def fet
-0005aac0: 6368 5f62 6f72 726f 775f 696e 7465 7265  ch_borrow_intere
-0005aad0: 7374 2873 656c 662c 2063 6f64 653a 204f  st(self, code: O
-0005aae0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0005aaf0: 6f6e 652c 2073 796d 626f 6c3a 204f 7074  one, symbol: Opt
-0005ab00: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0005ab10: 652c 2073 696e 6365 3a20 4f70 7469 6f6e  e, since: Option
-0005ab20: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
-0005ab30: 6c69 6d69 743a 204f 7074 696f 6e61 6c5b  limit: Optional[
-0005ab40: 696e 745d 203d 204e 6f6e 652c 2070 6172  int] = None, par
-0005ab50: 616d 733d 7b7d 293a 0a20 2020 2020 2020  ams={}):.       
-0005ab60: 2022 2222 0a20 2020 2020 2020 2066 6574   """.        fet
-0005ab70: 6368 2074 6865 2069 6e74 6572 6573 7420  ch the interest 
-0005ab80: 6f77 6564 2062 7920 7468 6520 7573 6572  owed by the user
-0005ab90: 2066 6f72 2062 6f72 726f 7769 6e67 2063   for borrowing c
-0005aba0: 7572 7265 6e63 7920 666f 7220 6d61 7267  urrency for marg
-0005abb0: 696e 2074 7261 6469 6e67 0a20 2020 2020  in trading.     
-0005abc0: 2020 203a 7061 7261 6d20 7374 727c 4e6f     :param str|No
-0005abd0: 6e65 2063 6f64 653a 2075 6e69 6669 6564  ne code: unified
-0005abe0: 2063 7572 7265 6e63 7920 636f 6465 0a20   currency code. 
-0005abf0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-0005ac00: 727c 4e6f 6e65 2073 796d 626f 6c3a 2075  r|None symbol: u
-0005ac10: 6e69 6669 6564 206d 6172 6b65 7420 7379  nified market sy
-0005ac20: 6d62 6f6c 2077 6865 6e20 6665 7463 6820  mbol when fetch 
-0005ac30: 696e 7465 7265 7374 2069 6e20 6973 6f6c  interest in isol
-0005ac40: 6174 6564 206d 6172 6b65 7473 0a20 2020  ated markets.   
-0005ac50: 2020 2020 203a 7061 7261 6d20 6e75 6d62       :param numb
-0005ac60: 6572 7c4e 6f6e 6520 7369 6e63 653a 2074  er|None since: t
-0005ac70: 6865 2065 6172 6c69 6573 7420 7469 6d65  he earliest time
-0005ac80: 2069 6e20 6d73 2074 6f20 6665 7463 6820   in ms to fetch 
-0005ac90: 626f 7272 726f 7720 696e 7465 7265 7374  borrrow interest
-0005aca0: 2066 6f72 0a20 2020 2020 2020 203a 7061   for.        :pa
-0005acb0: 7261 6d20 6e75 6d62 6572 7c4e 6f6e 6520  ram number|None 
-0005acc0: 6c69 6d69 743a 2074 6865 206d 6178 696d  limit: the maxim
-0005acd0: 756d 206e 756d 6265 7220 6f66 2073 7472  um number of str
-0005ace0: 7563 7475 7265 7320 746f 2072 6574 7269  uctures to retri
-0005acf0: 6576 650a 2020 2020 2020 2020 3a70 6172  eve.        :par
-0005ad00: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
-0005ad10: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
-0005ad20: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
-0005ad30: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
-0005ad40: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
-0005ad50: 7572 6e73 205b 6469 6374 5d3a 2061 206c  urns [dict]: a l
-0005ad60: 6973 7420 6f66 2060 626f 7272 6f77 2069  ist of `borrow i
-0005ad70: 6e74 6572 6573 7420 7374 7275 6374 7572  nterest structur
-0005ad80: 6573 203c 6874 7470 733a 2f2f 646f 6373  es <https://docs
-0005ad90: 2e63 6378 742e 636f 6d2f 232f 3f69 643d  .ccxt.com/#/?id=
-0005ada0: 626f 7272 6f77 2d69 6e74 6572 6573 742d  borrow-interest-
-0005adb0: 7374 7275 6374 7572 653e 600a 2020 2020  structure>`.    
-0005adc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0005add0: 6177 6169 7420 7365 6c66 2e6c 6f61 645f  await self.load_
-0005ade0: 6d61 726b 6574 7328 290a 2020 2020 2020  markets().      
-0005adf0: 2020 7265 7175 6573 7420 3d20 7b7d 0a20    request = {}. 
-0005ae00: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0005ae10: 3d20 6177 6169 7420 7365 6c66 2e70 7269  = await self.pri
-0005ae20: 7661 7465 4765 7453 706f 7456 3350 7269  vateGetSpotV3Pri
-0005ae30: 7661 7465 4372 6f73 734d 6172 6769 6e41  vateCrossMarginA
-0005ae40: 6363 6f75 6e74 2873 656c 662e 6578 7465  ccount(self.exte
-0005ae50: 6e64 2872 6571 7565 7374 2c20 7061 7261  nd(request, para
-0005ae60: 6d73 2929 0a20 2020 2020 2020 2023 0a20  ms)).        #. 
-0005ae70: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
-0005ae80: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005ae90: 2022 7265 745f 636f 6465 223a 2030 2c0a   "ret_code": 0,.
-0005aea0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005aeb0: 2020 2272 6574 5f6d 7367 223a 2022 222c    "ret_msg": "",
-0005aec0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005aed0: 2020 2022 6578 745f 636f 6465 223a 206e     "ext_code": n
-0005aee0: 756c 6c2c 0a20 2020 2020 2020 2023 2020  ull,.        #  
-0005aef0: 2020 2020 2020 2022 6578 745f 696e 666f         "ext_info
-0005af00: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
-0005af10: 2023 2020 2020 2020 2020 2022 7265 7375   #         "resu
-0005af20: 6c74 223a 207b 0a20 2020 2020 2020 2023  lt": {.        #
-0005af30: 2020 2020 2020 2020 2020 2020 2022 7374               "st
-0005af40: 6174 7573 223a 2022 3122 2c0a 2020 2020  atus": "1",.    
-0005af50: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005af60: 2020 2272 6973 6b52 6174 6522 3a20 2230    "riskRate": "0
-0005af70: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005af80: 2020 2020 2020 2020 2022 6163 6374 4261           "acctBa
-0005af90: 6c61 6e63 6553 756d 223a 2022 302e 3030  lanceSum": "0.00
-0005afa0: 3034 3836 3231 3338 3137 3638 3038 3537  0486213817680857
-0005afb0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005afc0: 2020 2020 2020 2020 2022 6465 6274 4261           "debtBa
-0005afd0: 6c61 6e63 6553 756d 223a 2022 3022 2c0a  lanceSum": "0",.
-0005afe0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005aff0: 2020 2020 2020 226c 6f61 6e41 6363 6f75        "loanAccou
-0005b000: 6e74 4c69 7374 223a 205b 0a20 2020 2020  ntList": [.     
-0005b010: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005b020: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0005b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005b040: 2020 2020 2022 746f 6b65 6e49 6422 3a20       "tokenId": 
-0005b050: 2242 5443 222c 0a20 2020 2020 2020 2023  "BTC",.        #
-0005b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005b070: 2020 2020 2022 746f 7461 6c22 3a20 2230       "total": "0
-0005b080: 2e30 3030 3438 3632 3122 2c0a 2020 2020  .00048621",.    
-0005b090: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005b0a0: 2020 2020 2020 2020 2020 226c 6f63 6b65            "locke
-0005b0b0: 6422 3a20 2230 222c 0a20 2020 2020 2020  d": "0",.       
-0005b0c0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0005b0d0: 2020 2020 2020 2022 6c6f 616e 223a 2022         "loan": "
-0005b0e0: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0005b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005b100: 2020 2269 6e74 6572 6573 7422 3a20 2230    "interest": "0
-0005b110: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005b130: 2022 6672 6565 223a 2022 302e 3030 3034   "free": "0.0004
-0005b140: 3836 3231 220a 2020 2020 2020 2020 2320  8621".        # 
-0005b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005b160: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
-0005b170: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-0005b180: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005b190: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0005b1a0: 2023 2020 2020 2020 2020 207d 0a20 2020   #         }.   
-0005b1b0: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-0005b1c0: 2020 2020 2023 0a20 2020 2020 2020 2064       #.        d
-0005b1d0: 6174 6120 3d20 7365 6c66 2e73 6166 655f  ata = self.safe_
-0005b1e0: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
-0005b1f0: 2772 6573 756c 7427 2c20 7b7d 290a 2020  'result', {}).  
-0005b200: 2020 2020 2020 726f 7773 203d 2073 656c        rows = sel
-0005b210: 662e 7361 6665 5f76 616c 7565 2864 6174  f.safe_value(dat
-0005b220: 612c 2027 6c6f 616e 4163 636f 756e 744c  a, 'loanAccountL
-0005b230: 6973 7427 2c20 5b5d 290a 2020 2020 2020  ist', []).      
-0005b240: 2020 696e 7465 7265 7374 203d 2073 656c    interest = sel
-0005b250: 662e 7061 7273 655f 626f 7272 6f77 5f69  f.parse_borrow_i
-0005b260: 6e74 6572 6573 7473 2872 6f77 732c 204e  nterests(rows, N
-0005b270: 6f6e 6529 0a20 2020 2020 2020 2072 6574  one).        ret
-0005b280: 7572 6e20 7365 6c66 2e66 696c 7465 725f  urn self.filter_
-0005b290: 6279 5f63 7572 7265 6e63 795f 7369 6e63  by_currency_sinc
-0005b2a0: 655f 6c69 6d69 7428 696e 7465 7265 7374  e_limit(interest
-0005b2b0: 2c20 636f 6465 2c20 7369 6e63 652c 206c  , code, since, l
-0005b2c0: 696d 6974 290a 0a20 2020 2064 6566 2070  imit)..    def p
-0005b2d0: 6172 7365 5f62 6f72 726f 775f 696e 7465  arse_borrow_inte
-0005b2e0: 7265 7374 2873 656c 662c 2069 6e66 6f2c  rest(self, info,
-0005b2f0: 206d 6172 6b65 743d 4e6f 6e65 293a 0a20   market=None):. 
-0005b300: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0005b310: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
-0005b320: 2023 2020 2020 2020 2020 2022 746f 6b65   #         "toke
-0005b330: 6e49 6422 3a20 2242 5443 222c 0a20 2020  nId": "BTC",.   
-0005b340: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005b350: 746f 7461 6c22 3a20 2230 2e30 3030 3438  total": "0.00048
-0005b360: 3632 3122 2c0a 2020 2020 2020 2020 2320  621",.        # 
-0005b370: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
-0005b380: 3a20 2230 222c 0a20 2020 2020 2020 2023  : "0",.        #
-0005b390: 2020 2020 2020 2020 2022 6c6f 616e 223a           "loan":
-0005b3a0: 2022 3022 2c0a 2020 2020 2020 2020 2320   "0",.        # 
-0005b3b0: 2020 2020 2020 2020 2269 6e74 6572 6573          "interes
-0005b3c0: 7422 3a20 2230 222c 0a20 2020 2020 2020  t": "0",.       
-0005b3d0: 2023 2020 2020 2020 2020 2022 6672 6565   #         "free
-0005b3e0: 223a 2022 302e 3030 3034 3836 3231 220a  ": "0.00048621".
-0005b3f0: 2020 2020 2020 2020 2320 2020 2020 7d2c          #     },
-0005b400: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005b410: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-0005b420: 2020 2020 2020 2020 2773 796d 626f 6c27          'symbol'
-0005b430: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
-0005b440: 2020 2020 276d 6172 6769 6e4d 6f64 6527      'marginMode'
-0005b450: 3a20 2763 726f 7373 272c 0a20 2020 2020  : 'cross',.     
-0005b460: 2020 2020 2020 2027 6375 7272 656e 6379         'currency
-0005b470: 273a 2073 656c 662e 7361 6665 5f63 7572  ': self.safe_cur
-0005b480: 7265 6e63 795f 636f 6465 2873 656c 662e  rency_code(self.
-0005b490: 7361 6665 5f73 7472 696e 6728 696e 666f  safe_string(info
-0005b4a0: 2c20 2774 6f6b 656e 4964 2729 292c 0a20  , 'tokenId')),. 
-0005b4b0: 2020 2020 2020 2020 2020 2027 696e 7465             'inte
-0005b4c0: 7265 7374 273a 2073 656c 662e 7361 6665  rest': self.safe
-0005b4d0: 5f6e 756d 6265 7228 696e 666f 2c20 2769  _number(info, 'i
-0005b4e0: 6e74 6572 6573 7427 292c 0a20 2020 2020  nterest'),.     
-0005b4f0: 2020 2020 2020 2027 696e 7465 7265 7374         'interest
-0005b500: 5261 7465 273a 204e 6f6e 652c 0a20 2020  Rate': None,.   
-0005b510: 2020 2020 2020 2020 2027 616d 6f75 6e74           'amount
-0005b520: 426f 7272 6f77 6564 273a 2073 656c 662e  Borrowed': self.
-0005b530: 7361 6665 5f6e 756d 6265 7228 696e 666f  safe_number(info
-0005b540: 2c20 276c 6f61 6e27 292c 0a20 2020 2020  , 'loan'),.     
-0005b550: 2020 2020 2020 2027 7469 6d65 7374 616d         'timestam
-0005b560: 7027 3a20 4e6f 6e65 2c0a 2020 2020 2020  p': None,.      
-0005b570: 2020 2020 2020 2764 6174 6574 696d 6527        'datetime'
-0005b580: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
-0005b590: 2020 2020 2769 6e66 6f27 3a20 696e 666f      'info': info
-0005b5a0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-0005b5b0: 2061 7379 6e63 2064 6566 2074 7261 6e73   async def trans
-0005b5c0: 6665 7228 7365 6c66 2c20 636f 6465 3a20  fer(self, code: 
-0005b5d0: 7374 722c 2061 6d6f 756e 742c 2066 726f  str, amount, fro
-0005b5e0: 6d41 6363 6f75 6e74 2c20 746f 4163 636f  mAccount, toAcco
-0005b5f0: 756e 742c 2070 6172 616d 733d 7b7d 293a  unt, params={}):
-0005b600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0005b610: 2020 2020 2074 7261 6e73 6665 7220 6375       transfer cu
-0005b620: 7272 656e 6379 2069 6e74 6572 6e61 6c6c  rrency internall
-0005b630: 7920 6265 7477 6565 6e20 7761 6c6c 6574  y between wallet
-0005b640: 7320 6f6e 2074 6865 2073 616d 6520 6163  s on the same ac
-0005b650: 636f 756e 740a 2020 2020 2020 2020 7365  count.        se
-0005b660: 6520 6874 7470 733a 2f2f 6279 6269 742d  e https://bybit-
-0005b670: 6578 6368 616e 6765 2e67 6974 6875 622e  exchange.github.
-0005b680: 696f 2f64 6f63 732f 6163 636f 756e 745f  io/docs/account_
-0005b690: 6173 7365 742f 2374 2d63 7265 6174 6569  asset/#t-createi
-0005b6a0: 6e74 6572 6e61 6c74 7261 6e73 6665 720a  nternaltransfer.
-0005b6b0: 2020 2020 2020 2020 7365 6520 6874 7470          see http
-0005b6c0: 733a 2f2f 6279 6269 742d 6578 6368 616e  s://bybit-exchan
-0005b6d0: 6765 2e67 6974 6875 622e 696f 2f64 6f63  ge.github.io/doc
-0005b6e0: 732f 6163 636f 756e 745f 6173 7365 742f  s/account_asset/
-0005b6f0: 7633 2f23 742d 6372 6561 7465 696e 7465  v3/#t-createinte
-0005b700: 726e 616c 7472 616e 7366 6572 0a20 2020  rnaltransfer.   
-0005b710: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
-0005b720: 636f 6465 3a20 756e 6966 6965 6420 6375  code: unified cu
-0005b730: 7272 656e 6379 2063 6f64 650a 2020 2020  rrency code.    
-0005b740: 2020 2020 3a70 6172 616d 2066 6c6f 6174      :param float
-0005b750: 2061 6d6f 756e 743a 2061 6d6f 756e 7420   amount: amount 
-0005b760: 746f 2074 7261 6e73 6665 720a 2020 2020  to transfer.    
-0005b770: 2020 2020 3a70 6172 616d 2073 7472 2066      :param str f
-0005b780: 726f 6d41 6363 6f75 6e74 3a20 6163 636f  romAccount: acco
-0005b790: 756e 7420 746f 2074 7261 6e73 6665 7220  unt to transfer 
-0005b7a0: 6672 6f6d 0a20 2020 2020 2020 203a 7061  from.        :pa
-0005b7b0: 7261 6d20 7374 7220 746f 4163 636f 756e  ram str toAccoun
-0005b7c0: 743a 2061 6363 6f75 6e74 2074 6f20 7472  t: account to tr
-0005b7d0: 616e 7366 6572 2074 6f0a 2020 2020 2020  ansfer to.      
-0005b7e0: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
-0005b7f0: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
-0005b800: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
-0005b810: 746f 2074 6865 2062 7962 6974 2061 7069  to the bybit api
-0005b820: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
-0005b830: 2020 3a70 6172 616d 2073 7472 2070 6172    :param str par
-0005b840: 616d 735b 2774 7261 6e73 6665 7249 6427  ams['transferId'
-0005b850: 5d3a 2055 5549 442c 2077 6869 6368 2069  ]: UUID, which i
-0005b860: 7320 756e 6971 7565 2061 6372 6f73 7320  s unique across 
-0005b870: 7468 6520 706c 6174 666f 726d 0a20 2020  the platform.   
-0005b880: 2020 2020 203a 7265 7475 726e 7320 6469       :returns di
-0005b890: 6374 3a20 6120 6074 7261 6e73 6665 7220  ct: a `transfer 
-0005b8a0: 7374 7275 6374 7572 6520 3c68 7474 7073  structure <https
-0005b8b0: 3a2f 2f64 6f63 732e 6363 7874 2e63 6f6d  ://docs.ccxt.com
-0005b8c0: 2f23 2f3f 6964 3d74 7261 6e73 6665 722d  /#/?id=transfer-
-0005b8d0: 7374 7275 6374 7572 653e 600a 2020 2020  structure>`.    
-0005b8e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0005b8f0: 6177 6169 7420 7365 6c66 2e6c 6f61 645f  await self.load_
-0005b900: 6d61 726b 6574 7328 290a 2020 2020 2020  markets().      
-0005b910: 2020 7472 616e 7366 6572 4964 203d 2073    transferId = s
-0005b920: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
-0005b930: 7061 7261 6d73 2c20 2774 7261 6e73 6665  params, 'transfe
-0005b940: 7249 6427 2c20 7365 6c66 2e75 7569 6428  rId', self.uuid(
-0005b950: 2929 0a20 2020 2020 2020 2061 6363 6f75  )).        accou
-0005b960: 6e74 5479 7065 7320 3d20 7365 6c66 2e73  ntTypes = self.s
-0005b970: 6166 655f 7661 6c75 6528 7365 6c66 2e6f  afe_value(self.o
-0005b980: 7074 696f 6e73 2c20 2761 6363 6f75 6e74  ptions, 'account
-0005b990: 7342 7954 7970 6527 2c20 7b7d 290a 2020  sByType', {}).  
-0005b9a0: 2020 2020 2020 6672 6f6d 4964 203d 2073        fromId = s
-0005b9b0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
-0005b9c0: 6163 636f 756e 7454 7970 6573 2c20 6672  accountTypes, fr
-0005b9d0: 6f6d 4163 636f 756e 742c 2066 726f 6d41  omAccount, fromA
-0005b9e0: 6363 6f75 6e74 290a 2020 2020 2020 2020  ccount).        
-0005b9f0: 746f 4964 203d 2073 656c 662e 7361 6665  toId = self.safe
-0005ba00: 5f73 7472 696e 6728 6163 636f 756e 7454  _string(accountT
-0005ba10: 7970 6573 2c20 746f 4163 636f 756e 742c  ypes, toAccount,
-0005ba20: 2074 6f41 6363 6f75 6e74 290a 2020 2020   toAccount).    
-0005ba30: 2020 2020 6375 7272 656e 6379 203d 2073      currency = s
-0005ba40: 656c 662e 6375 7272 656e 6379 2863 6f64  elf.currency(cod
-0005ba50: 6529 0a20 2020 2020 2020 2061 6d6f 756e  e).        amoun
-0005ba60: 7454 6f50 7265 6369 7369 6f6e 203d 2073  tToPrecision = s
-0005ba70: 656c 662e 6375 7272 656e 6379 5f74 6f5f  elf.currency_to_
-0005ba80: 7072 6563 6973 696f 6e28 636f 6465 2c20  precision(code, 
-0005ba90: 616d 6f75 6e74 290a 2020 2020 2020 2020  amount).        
-0005baa0: 6d65 7468 6f64 203d 204e 6f6e 650a 2020  method = None.  
-0005bab0: 2020 2020 2020 6d65 7468 6f64 2c20 7061        method, pa
-0005bac0: 7261 6d73 203d 2073 656c 662e 6861 6e64  rams = self.hand
-0005bad0: 6c65 5f6f 7074 696f 6e5f 616e 645f 7061  le_option_and_pa
-0005bae0: 7261 6d73 2870 6172 616d 732c 2027 7472  rams(params, 'tr
-0005baf0: 616e 7366 6572 272c 2027 6d65 7468 6f64  ansfer', 'method
-0005bb00: 272c 2027 7072 6976 6174 6550 6f73 7441  ', 'privatePostA
-0005bb10: 7373 6574 5631 5072 6976 6174 6554 7261  ssetV1PrivateTra
-0005bb20: 6e73 6665 7227 2920 2023 2076 3120 7072  nsfer')  # v1 pr
-0005bb30: 6566 6572 7265 6420 6174 6d2c 2062 6563  eferred atm, bec
-0005bb40: 6175 7365 2069 7420 7375 7070 6f72 7473  ause it supports
-0005bb50: 2066 756e 6469 6e67 0a20 2020 2020 2020   funding.       
-0005bb60: 2072 6571 7565 7374 203d 204e 6f6e 650a   request = None.
-0005bb70: 2020 2020 2020 2020 6966 206d 6574 686f          if metho
-0005bb80: 6420 3d3d 2027 7072 6976 6174 6550 6f73  d == 'privatePos
-0005bb90: 7441 7373 6574 5633 5072 6976 6174 6554  tAssetV3PrivateT
-0005bba0: 7261 6e73 6665 7249 6e74 6572 5472 616e  ransferInterTran
-0005bbb0: 7366 6572 2720 6f72 206d 6574 686f 6420  sfer' or method 
-0005bbc0: 3d3d 2027 7072 6976 6174 6550 6f73 7456  == 'privatePostV
-0005bbd0: 3541 7373 6574 5472 616e 7366 6572 496e  5AssetTransferIn
-0005bbe0: 7465 7254 7261 6e73 6665 7227 3a0a 2020  terTransfer':.  
-0005bbf0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0005bc00: 7420 3d20 7b0a 2020 2020 2020 2020 2020  t = {.          
-0005bc10: 2020 2020 2020 2774 7261 6e73 6665 7249        'transferI
-0005bc20: 6427 3a20 7472 616e 7366 6572 4964 2c0a  d': transferId,.
-0005bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005bc40: 2766 726f 6d41 6363 6f75 6e74 5479 7065  'fromAccountType
-0005bc50: 273a 2066 726f 6d49 642c 0a20 2020 2020  ': fromId,.     
-0005bc60: 2020 2020 2020 2020 2020 2027 746f 4163             'toAc
-0005bc70: 636f 756e 7454 7970 6527 3a20 746f 4964  countType': toId
-0005bc80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0005bc90: 2020 2763 6f69 6e27 3a20 6375 7272 656e    'coin': curren
-0005bca0: 6379 5b27 6964 275d 2c0a 2020 2020 2020  cy['id'],.      
-0005bcb0: 2020 2020 2020 2020 2020 2761 6d6f 756e            'amoun
-0005bcc0: 7427 3a20 616d 6f75 6e74 546f 5072 6563  t': amountToPrec
-0005bcd0: 6973 696f 6e2c 0a20 2020 2020 2020 2020  ision,.         
-0005bce0: 2020 207d 0a20 2020 2020 2020 2065 6c73     }.        els
-0005bcf0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0005bd00: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
-0005bd10: 2020 2020 2020 2020 2020 2027 7472 616e             'tran
-0005bd20: 7366 6572 5f69 6427 3a20 7472 616e 7366  sfer_id': transf
-0005bd30: 6572 4964 2c0a 2020 2020 2020 2020 2020  erId,.          
-0005bd40: 2020 2020 2020 2766 726f 6d5f 6163 636f        'from_acco
-0005bd50: 756e 745f 7479 7065 273a 2066 726f 6d49  unt_type': fromI
-0005bd60: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0005bd70: 2020 2027 746f 5f61 6363 6f75 6e74 5f74     'to_account_t
-0005bd80: 7970 6527 3a20 746f 4964 2c0a 2020 2020  ype': toId,.    
-0005bd90: 2020 2020 2020 2020 2020 2020 2763 6f69              'coi
-0005bda0: 6e27 3a20 6375 7272 656e 6379 5b27 6964  n': currency['id
-0005bdb0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-0005bdc0: 2020 2020 2761 6d6f 756e 7427 3a20 616d      'amount': am
-0005bdd0: 6f75 6e74 546f 5072 6563 6973 696f 6e2c  ountToPrecision,
-0005bde0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-0005bdf0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0005be00: 3d20 6177 6169 7420 6765 7461 7474 7228  = await getattr(
-0005be10: 7365 6c66 2c20 6d65 7468 6f64 2928 7365  self, method)(se
-0005be20: 6c66 2e65 7874 656e 6428 7265 7175 6573  lf.extend(reques
-0005be30: 742c 2070 6172 616d 7329 290a 2020 2020  t, params)).    
-0005be40: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
-0005be50: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0005be60: 2272 6574 436f 6465 223a 2030 2c0a 2020  "retCode": 0,.  
-0005be70: 2020 2020 2020 2320 2020 2020 2272 6574        #     "ret
-0005be80: 4d73 6722 3a20 2273 7563 6365 7373 222c  Msg": "success",
-0005be90: 0a20 2020 2020 2020 2023 2020 2020 2022  .        #     "
-0005bea0: 7265 7375 6c74 223a 207b 0a20 2020 2020  result": {.     
-0005beb0: 2020 2023 2020 2020 2020 2020 2022 7472     #         "tr
-0005bec0: 616e 7366 6572 4964 223a 2022 3432 3434  ansferId": "4244
-0005bed0: 6166 3434 2d66 3362 302d 3463 6636 2d61  af44-f3b0-4cf6-a
-0005bee0: 3734 332d 6235 3635 3630 6539 3837 6263  743-b56560e987bc
-0005bef0: 2220 2023 2074 7261 6e73 6665 725f 6964  "  # transfer_id
-0005bf00: 2069 6e20 7631 0a20 2020 2020 2020 2023   in v1.        #
-0005bf10: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-0005bf20: 2320 2020 2020 2272 6574 4578 7449 6e66  #     "retExtInf
-0005bf30: 6f22 3a20 7b7d 2c0a 2020 2020 2020 2020  o": {},.        
-0005bf40: 2320 2020 2020 2274 696d 6522 3a20 3136  #     "time": 16
-0005bf50: 3636 3837 3538 3537 3230 350a 2020 2020  66875857205.    
-0005bf60: 2020 2020 2320 7d0a 2020 2020 2020 2020      # }.        
-0005bf70: 230a 2020 2020 2020 2020 7469 6d65 7374  #.        timest
-0005bf80: 616d 7020 3d20 7365 6c66 2e73 6166 655f  amp = self.safe_
-0005bf90: 696e 7465 6765 725f 3228 7265 7370 6f6e  integer_2(respon
-0005bfa0: 7365 2c20 2774 696d 6527 2c20 2774 696d  se, 'time', 'tim
-0005bfb0: 655f 6e6f 7727 290a 2020 2020 2020 2020  e_now').        
-0005bfc0: 7472 616e 7366 6572 203d 2073 656c 662e  transfer = self.
-0005bfd0: 7361 6665 5f76 616c 7565 2872 6573 706f  safe_value(respo
-0005bfe0: 6e73 652c 2027 7265 7375 6c74 272c 207b  nse, 'result', {
-0005bff0: 7d29 0a20 2020 2020 2020 2073 7461 7475  }).        statu
-0005c000: 7352 6177 203d 2073 656c 662e 7361 6665  sRaw = self.safe
-0005c010: 5f73 7472 696e 675f 6e28 7265 7370 6f6e  _string_n(respon
-0005c020: 7365 2c20 5b27 7265 7443 6f64 6527 2c20  se, ['retCode', 
-0005c030: 2772 6574 4d73 6727 2c20 2772 6574 5f63  'retMsg', 'ret_c
-0005c040: 6f64 6527 2c20 2772 6574 5f6d 7367 275d  ode', 'ret_msg']
-0005c050: 290a 2020 2020 2020 2020 7374 6174 7573  ).        status
-0005c060: 203d 2073 656c 662e 7061 7273 655f 7472   = self.parse_tr
-0005c070: 616e 7366 6572 5f73 7461 7475 7328 7374  ansfer_status(st
-0005c080: 6174 7573 5261 7729 0a20 2020 2020 2020  atusRaw).       
-0005c090: 2072 6574 7572 6e20 7365 6c66 2e65 7874   return self.ext
-0005c0a0: 656e 6428 7365 6c66 2e70 6172 7365 5f74  end(self.parse_t
-0005c0b0: 7261 6e73 6665 7228 7472 616e 7366 6572  ransfer(transfer
-0005c0c0: 2c20 6375 7272 656e 6379 292c 207b 0a20  , currency), {. 
-0005c0d0: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
-0005c0e0: 7374 616d 7027 3a20 7469 6d65 7374 616d  stamp': timestam
-0005c0f0: 702c 0a20 2020 2020 2020 2020 2020 2027  p,.            '
-0005c100: 6461 7465 7469 6d65 273a 2073 656c 662e  datetime': self.
-0005c110: 6973 6f38 3630 3128 7469 6d65 7374 616d  iso8601(timestam
-0005c120: 7029 2c0a 2020 2020 2020 2020 2020 2020  p),.            
-0005c130: 2761 6d6f 756e 7427 3a20 7365 6c66 2e70  'amount': self.p
-0005c140: 6172 7365 5f6e 756d 6265 7228 616d 6f75  arse_number(amou
-0005c150: 6e74 546f 5072 6563 6973 696f 6e29 2c0a  ntToPrecision),.
-0005c160: 2020 2020 2020 2020 2020 2020 2766 726f              'fro
-0005c170: 6d41 6363 6f75 6e74 273a 2066 726f 6d41  mAccount': fromA
-0005c180: 6363 6f75 6e74 2c0a 2020 2020 2020 2020  ccount,.        
-0005c190: 2020 2020 2774 6f41 6363 6f75 6e74 273a      'toAccount':
-0005c1a0: 2074 6f41 6363 6f75 6e74 2c0a 2020 2020   toAccount,.    
-0005c1b0: 2020 2020 2020 2020 2773 7461 7475 7327          'status'
-0005c1c0: 3a20 7374 6174 7573 2c0a 2020 2020 2020  : status,.      
-0005c1d0: 2020 7d29 0a0a 2020 2020 6173 796e 6320    })..    async 
-0005c1e0: 6465 6620 6665 7463 685f 7472 616e 7366  def fetch_transf
-0005c1f0: 6572 7328 7365 6c66 2c20 636f 6465 3a20  ers(self, code: 
-0005c200: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0005c210: 4e6f 6e65 2c20 7369 6e63 653a 204f 7074  None, since: Opt
-0005c220: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0005c230: 652c 206c 696d 6974 3a20 4f70 7469 6f6e  e, limit: Option
-0005c240: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
-0005c250: 7061 7261 6d73 3d7b 7d29 3a0a 2020 2020  params={}):.    
-0005c260: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0005c270: 6665 7463 6820 6120 6869 7374 6f72 7920  fetch a history 
-0005c280: 6f66 2069 6e74 6572 6e61 6c20 7472 616e  of internal tran
-0005c290: 7366 6572 7320 6d61 6465 206f 6e20 616e  sfers made on an
-0005c2a0: 2061 6363 6f75 6e74 0a20 2020 2020 2020   account.       
-0005c2b0: 2073 6565 2068 7474 7073 3a2f 2f62 7962   see https://byb
-0005c2c0: 6974 2d65 7863 6861 6e67 652e 6769 7468  it-exchange.gith
-0005c2d0: 7562 2e69 6f2f 646f 6373 2f76 352f 6173  ub.io/docs/v5/as
-0005c2e0: 7365 742f 696e 7465 722d 7472 616e 7366  set/inter-transf
-0005c2f0: 6572 2d6c 6973 740a 2020 2020 2020 2020  er-list.        
-0005c300: 3a70 6172 616d 2073 7472 7c4e 6f6e 6520  :param str|None 
-0005c310: 636f 6465 3a20 756e 6966 6965 6420 6375  code: unified cu
-0005c320: 7272 656e 6379 2063 6f64 6520 6f66 2074  rrency code of t
-0005c330: 6865 2063 7572 7265 6e63 7920 7472 616e  he currency tran
-0005c340: 7366 6572 7265 640a 2020 2020 2020 2020  sferred.        
-0005c350: 3a70 6172 616d 2069 6e74 7c4e 6f6e 6520  :param int|None 
-0005c360: 7369 6e63 653a 2074 6865 2065 6172 6c69  since: the earli
-0005c370: 6573 7420 7469 6d65 2069 6e20 6d73 2074  est time in ms t
-0005c380: 6f20 6665 7463 6820 7472 616e 7366 6572  o fetch transfer
-0005c390: 7320 666f 720a 2020 2020 2020 2020 3a70  s for.        :p
-0005c3a0: 6172 616d 2069 6e74 7c4e 6f6e 6520 6c69  aram int|None li
-0005c3b0: 6d69 743a 2074 6865 206d 6178 696d 756d  mit: the maximum
-0005c3c0: 206e 756d 6265 7220 6f66 2020 7472 616e   number of  tran
-0005c3d0: 7366 6572 7320 7374 7275 6374 7572 6573  sfers structures
-0005c3e0: 2074 6f20 7265 7472 6965 7665 0a20 2020   to retrieve.   
-0005c3f0: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
-0005c400: 2070 6172 616d 733a 2065 7874 7261 2070   params: extra p
-0005c410: 6172 616d 6574 6572 7320 7370 6563 6966  arameters specif
-0005c420: 6963 2074 6f20 7468 6520 6279 6269 7420  ic to the bybit 
-0005c430: 6170 6920 656e 6470 6f69 6e74 0a20 2020  api endpoint.   
-0005c440: 2020 2020 203a 7265 7475 726e 7320 5b64       :returns [d
-0005c450: 6963 745d 3a20 6120 6c69 7374 206f 6620  ict]: a list of 
-0005c460: 6074 7261 6e73 6665 7220 7374 7275 6374  `transfer struct
-0005c470: 7572 6573 203c 6874 7470 733a 2f2f 646f  ures <https://do
-0005c480: 6373 2e63 6378 742e 636f 6d2f 232f 3f69  cs.ccxt.com/#/?i
-0005c490: 643d 7472 616e 7366 6572 2d73 7472 7563  d=transfer-struc
-0005c4a0: 7475 7265 3e60 0a20 2020 2020 2020 2022  ture>`.        "
-0005c4b0: 2222 0a20 2020 2020 2020 2061 7761 6974  "".        await
-0005c4c0: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
-0005c4d0: 7473 2829 0a20 2020 2020 2020 2063 7572  ts().        cur
-0005c4e0: 7265 6e63 7920 3d20 4e6f 6e65 0a20 2020  rency = None.   
-0005c4f0: 2020 2020 2072 6571 7565 7374 203d 207b       request = {
-0005c500: 7d0a 2020 2020 2020 2020 6966 2063 6f64  }.        if cod
-0005c510: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0005c520: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0005c530: 6e63 7920 3d20 7365 6c66 2e73 6166 655f  ncy = self.safe_
-0005c540: 6375 7272 656e 6379 5f63 6f64 6528 636f  currency_code(co
-0005c550: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
-0005c560: 7265 7175 6573 745b 2763 6f69 6e27 5d20  request['coin'] 
-0005c570: 3d20 6375 7272 656e 6379 0a20 2020 2020  = currency.     
-0005c580: 2020 2069 6620 7369 6e63 6520 6973 206e     if since is n
-0005c590: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0005c5a0: 2020 2020 2072 6571 7565 7374 5b27 7374       request['st
-0005c5b0: 6172 7454 696d 6527 5d20 3d20 7369 6e63  artTime'] = sinc
-0005c5c0: 650a 2020 2020 2020 2020 6966 206c 696d  e.        if lim
-0005c5d0: 6974 2069 7320 6e6f 7420 4e6f 6e65 3a0a  it is not None:.
-0005c5e0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0005c5f0: 6573 745b 276c 696d 6974 275d 203d 206c  est['limit'] = l
-0005c600: 696d 6974 0a20 2020 2020 2020 2072 6573  imit.        res
-0005c610: 706f 6e73 6520 3d20 6177 6169 7420 7365  ponse = await se
-0005c620: 6c66 2e70 7269 7661 7465 4765 7456 3541  lf.privateGetV5A
-0005c630: 7373 6574 5472 616e 7366 6572 5175 6572  ssetTransferQuer
-0005c640: 7949 6e74 6572 5472 616e 7366 6572 4c69  yInterTransferLi
-0005c650: 7374 2873 656c 662e 6578 7465 6e64 2872  st(self.extend(r
-0005c660: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
-0005c670: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005c680: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
-0005c690: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
-0005c6a0: 7443 6f64 6522 3a20 302c 0a20 2020 2020  tCode": 0,.     
-0005c6b0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
-0005c6c0: 744d 7367 223a 2022 7375 6363 6573 7322  tMsg": "success"
-0005c6d0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0005c6e0: 2020 2020 2272 6573 756c 7422 3a20 7b0a      "result": {.
-0005c6f0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005c700: 2020 2020 2020 226c 6973 7422 3a20 5b0a        "list": [.
-0005c710: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005c720: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-0005c730: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005c740: 2020 2020 2020 2020 2020 2274 7261 6e73            "trans
-0005c750: 6665 7249 6422 3a20 2273 656c 6654 7261  ferId": "selfTra
-0005c760: 6e73 6665 725f 6131 3039 3163 6337 2d39  nsfer_a1091cc7-9
-0005c770: 3336 342d 3462 3734 2d38 6465 312d 3138  364-4b74-8de1-18
-0005c780: 6630 3263 3666 3264 3563 222c 0a20 2020  f02c6f2d5c",.   
-0005c790: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0005c7a0: 2020 2020 2020 2020 2020 2022 636f 696e             "coin
-0005c7b0: 223a 2022 5553 4454 222c 0a20 2020 2020  ": "USDT",.     
-0005c7c0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005c7d0: 2020 2020 2020 2020 2022 616d 6f75 6e74           "amount
-0005c7e0: 223a 2022 3530 3030 222c 0a20 2020 2020  ": "5000",.     
-0005c7f0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005c800: 2020 2020 2020 2020 2022 6672 6f6d 4163           "fromAc
-0005c810: 636f 756e 7454 7970 6522 3a20 2253 504f  countType": "SPO
-0005c820: 5422 2c0a 2020 2020 2020 2020 2320 2020  T",.        #   
-0005c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005c840: 2020 2274 6f41 6363 6f75 6e74 5479 7065    "toAccountType
-0005c850: 223a 2022 554e 4946 4945 4422 2c0a 2020  ": "UNIFIED",.  
-0005c860: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005c870: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
-0005c880: 6573 7461 6d70 223a 2022 3136 3637 3238  estamp": "166728
-0005c890: 3332 3633 3030 3022 2c0a 2020 2020 2020  3263000",.      
-0005c8a0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005c8b0: 2020 2020 2020 2020 2273 7461 7475 7322          "status"
-0005c8c0: 3a20 2253 5543 4345 5353 220a 2020 2020  : "SUCCESS".    
-0005c8d0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005c8e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0005c8f0: 2320 2020 2020 2020 2020 2020 2020 5d2c  #             ],
-0005c900: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005c910: 2020 2020 2020 2022 6e65 7874 5061 6765         "nextPage
-0005c920: 4375 7273 6f72 223a 2022 6579 4a74 6157  Cursor": "eyJtaW
-0005c930: 354a 5243 4936 4d54 4d31 4f44 5132 4f43  5JRCI6MTM1ODQ2OC
-0005c940: 7769 6257 4634 5355 5169 4f6a 457a 4e54  wibWF4SUQiOjEzNT
-0005c950: 6730 4e6a 6839 220a 2020 2020 2020 2020  g0Njh9".        
-0005c960: 2320 2020 2020 2020 2020 7d2c 0a20 2020  #         },.   
-0005c970: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005c980: 7265 7445 7874 496e 666f 223a 207b 7d2c  retExtInfo": {},
-0005c990: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005c9a0: 2020 2022 7469 6d65 223a 2031 3637 3039     "time": 16709
-0005c9b0: 3838 3237 3136 3737 0a20 2020 2020 2020  88271677.       
-0005c9c0: 2023 2020 2020 207d 0a20 2020 2020 2020   #     }.       
-0005c9d0: 2023 0a20 2020 2020 2020 2064 6174 6120   #.        data 
-0005c9e0: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
-0005c9f0: 6528 7265 7370 6f6e 7365 2c20 2772 6573  e(response, 'res
-0005ca00: 756c 7427 2c20 7b7d 290a 2020 2020 2020  ult', {}).      
-0005ca10: 2020 7472 616e 7366 6572 7320 3d20 7365    transfers = se
-0005ca20: 6c66 2e73 6166 655f 7661 6c75 6528 6461  lf.safe_value(da
-0005ca30: 7461 2c20 276c 6973 7427 2c20 5b5d 290a  ta, 'list', []).
-0005ca40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0005ca50: 656c 662e 7061 7273 655f 7472 616e 7366  elf.parse_transf
-0005ca60: 6572 7328 7472 616e 7366 6572 732c 2063  ers(transfers, c
-0005ca70: 7572 7265 6e63 792c 2073 696e 6365 2c20  urrency, since, 
-0005ca80: 6c69 6d69 7429 0a0a 2020 2020 6173 796e  limit)..    asyn
-0005ca90: 6320 6465 6620 626f 7272 6f77 5f6d 6172  c def borrow_mar
-0005caa0: 6769 6e28 7365 6c66 2c20 636f 6465 3a20  gin(self, code: 
-0005cab0: 7374 722c 2061 6d6f 756e 742c 2073 796d  str, amount, sym
-0005cac0: 626f 6c3a 204f 7074 696f 6e61 6c5b 7374  bol: Optional[st
-0005cad0: 725d 203d 204e 6f6e 652c 2070 6172 616d  r] = None, param
-0005cae0: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
-0005caf0: 2222 0a20 2020 2020 2020 2063 7265 6174  "".        creat
-0005cb00: 6520 6120 6c6f 616e 2074 6f20 626f 7272  e a loan to borr
-0005cb10: 6f77 206d 6172 6769 6e0a 2020 2020 2020  ow margin.      
-0005cb20: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
-0005cb30: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
-0005cb40: 6875 622e 696f 2f64 6f63 732f 7370 6f74  hub.io/docs/spot
-0005cb50: 2f76 332f 2374 2d62 6f72 726f 776d 6172  /v3/#t-borrowmar
-0005cb60: 6769 6e6c 6f61 6e0a 2020 2020 2020 2020  ginloan.        
-0005cb70: 3a70 6172 616d 2073 7472 2063 6f64 653a  :param str code:
-0005cb80: 2075 6e69 6669 6564 2063 7572 7265 6e63   unified currenc
-0005cb90: 7920 636f 6465 206f 6620 7468 6520 6375  y code of the cu
-0005cba0: 7272 656e 6379 2074 6f20 626f 7272 6f77  rrency to borrow
-0005cbb0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0005cbc0: 666c 6f61 7420 616d 6f75 6e74 3a20 7468  float amount: th
-0005cbd0: 6520 616d 6f75 6e74 2074 6f20 626f 7272  e amount to borr
-0005cbe0: 6f77 0a20 2020 2020 2020 203a 7061 7261  ow.        :para
-0005cbf0: 6d20 7374 727c 4e6f 6e65 2073 796d 626f  m str|None symbo
-0005cc00: 6c3a 206e 6f74 2075 7365 6420 6279 2062  l: not used by b
-0005cc10: 7962 6974 2e62 6f72 726f 774d 6172 6769  ybit.borrowMargi
-0005cc20: 6e28 290a 2020 2020 2020 2020 3a70 6172  n().        :par
-0005cc30: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
-0005cc40: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
-0005cc50: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
-0005cc60: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
-0005cc70: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
-0005cc80: 7572 6e73 2064 6963 743a 2061 2060 6d61  urns dict: a `ma
-0005cc90: 7267 696e 206c 6f61 6e20 7374 7275 6374  rgin loan struct
-0005cca0: 7572 6520 3c68 7474 7073 3a2f 2f64 6f63  ure <https://doc
-0005ccb0: 732e 6363 7874 2e63 6f6d 2f23 2f3f 6964  s.ccxt.com/#/?id
-0005ccc0: 3d6d 6172 6769 6e2d 6c6f 616e 2d73 7472  =margin-loan-str
-0005ccd0: 7563 7475 7265 3e60 0a20 2020 2020 2020  ucture>`.       
-0005cce0: 2022 2222 0a20 2020 2020 2020 2061 7761   """.        awa
-0005ccf0: 6974 2073 656c 662e 6c6f 6164 5f6d 6172  it self.load_mar
-0005cd00: 6b65 7473 2829 0a20 2020 2020 2020 2063  kets().        c
-0005cd10: 7572 7265 6e63 7920 3d20 7365 6c66 2e63  urrency = self.c
-0005cd20: 7572 7265 6e63 7928 636f 6465 290a 2020  urrency(code).  
-0005cd30: 2020 2020 2020 6d61 7267 696e 4d6f 6465        marginMode
-0005cd40: 2c20 7175 6572 7920 3d20 7365 6c66 2e68  , query = self.h
-0005cd50: 616e 646c 655f 6d61 7267 696e 5f6d 6f64  andle_margin_mod
-0005cd60: 655f 616e 645f 7061 7261 6d73 2827 626f  e_and_params('bo
-0005cd70: 7272 6f77 4d61 7267 696e 272c 2070 6172  rrowMargin', par
-0005cd80: 616d 7329 0a20 2020 2020 2020 2069 6620  ams).        if 
-0005cd90: 6d61 7267 696e 4d6f 6465 203d 3d20 2769  marginMode == 'i
-0005cda0: 736f 6c61 7465 6427 3a0a 2020 2020 2020  solated':.      
-0005cdb0: 2020 2020 2020 7261 6973 6520 4e6f 7453        raise NotS
-0005cdc0: 7570 706f 7274 6564 2873 656c 662e 6964  upported(self.id
-0005cdd0: 202b 2027 2062 6f72 726f 774d 6172 6769   + ' borrowMargi
-0005cde0: 6e28 2920 6361 6e6e 6f74 2075 7365 2069  n() cannot use i
-0005cdf0: 736f 6c61 7465 6420 6d61 7267 696e 2729  solated margin')
-0005ce00: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0005ce10: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0005ce20: 2027 636f 696e 273a 2063 7572 7265 6e63   'coin': currenc
-0005ce30: 795b 2769 6427 5d2c 0a20 2020 2020 2020  y['id'],.       
-0005ce40: 2020 2020 2027 7174 7927 3a20 7365 6c66       'qty': self
-0005ce50: 2e63 7572 7265 6e63 795f 746f 5f70 7265  .currency_to_pre
-0005ce60: 6369 7369 6f6e 2863 6f64 652c 2061 6d6f  cision(code, amo
-0005ce70: 756e 7429 2c0a 2020 2020 2020 2020 7d0a  unt),.        }.
-0005ce80: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0005ce90: 203d 2061 7761 6974 2073 656c 662e 7072   = await self.pr
-0005cea0: 6976 6174 6550 6f73 7453 706f 7456 3350  ivatePostSpotV3P
-0005ceb0: 7269 7661 7465 4372 6f73 734d 6172 6769  rivateCrossMargi
-0005cec0: 6e4c 6f61 6e28 7365 6c66 2e65 7874 656e  nLoan(self.exten
-0005ced0: 6428 7265 7175 6573 742c 2071 7565 7279  d(request, query
-0005cee0: 2929 0a20 2020 2020 2020 2023 0a20 2020  )).        #.   
-0005cef0: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
-0005cf00: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005cf10: 7265 7443 6f64 6522 3a20 302c 0a20 2020  retCode": 0,.   
-0005cf20: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005cf30: 7265 744d 7367 223a 2022 7375 6363 6573  retMsg": "succes
-0005cf40: 7322 2c0a 2020 2020 2020 2020 2320 2020  s",.        #   
-0005cf50: 2020 2020 2020 2272 6573 756c 7422 3a20        "result": 
-0005cf60: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0005cf70: 2020 2020 2020 2020 2274 7261 6e73 6163          "transac
-0005cf80: 7449 6422 3a20 2231 3431 3433 220a 2020  tId": "14143".  
-0005cf90: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005cfa0: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
-0005cfb0: 2020 2020 2022 7265 7445 7874 496e 666f       "retExtInfo
-0005cfc0: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
-0005cfd0: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
-0005cfe0: 223a 2031 3636 3236 3137 3834 3839 3730  ": 1662617848970
-0005cff0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
-0005d000: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005d010: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0005d020: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
-0005d030: 6f6e 7365 2c20 2772 6573 756c 7427 2c20  onse, 'result', 
-0005d040: 7b7d 290a 2020 2020 2020 2020 7472 616e  {}).        tran
-0005d050: 7361 6374 696f 6e20 3d20 7365 6c66 2e70  saction = self.p
-0005d060: 6172 7365 5f6d 6172 6769 6e5f 6c6f 616e  arse_margin_loan
-0005d070: 2872 6573 756c 742c 2063 7572 7265 6e63  (result, currenc
-0005d080: 7929 0a20 2020 2020 2020 2072 6574 7572  y).        retur
-0005d090: 6e20 7365 6c66 2e65 7874 656e 6428 7472  n self.extend(tr
-0005d0a0: 616e 7361 6374 696f 6e2c 207b 0a20 2020  ansaction, {.   
-0005d0b0: 2020 2020 2020 2020 2027 7379 6d62 6f6c           'symbol
-0005d0c0: 273a 2073 796d 626f 6c2c 0a20 2020 2020  ': symbol,.     
-0005d0d0: 2020 2020 2020 2027 616d 6f75 6e74 273a         'amount':
-0005d0e0: 2061 6d6f 756e 742c 0a20 2020 2020 2020   amount,.       
-0005d0f0: 207d 290a 0a20 2020 2061 7379 6e63 2064   })..    async d
-0005d100: 6566 2072 6570 6179 5f6d 6172 6769 6e28  ef repay_margin(
-0005d110: 7365 6c66 2c20 636f 6465 3a20 7374 722c  self, code: str,
-0005d120: 2061 6d6f 756e 742c 2073 796d 626f 6c3a   amount, symbol:
-0005d130: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0005d140: 204e 6f6e 652c 2070 6172 616d 733d 7b7d   None, params={}
-0005d150: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0005d160: 2020 2020 2020 2072 6570 6179 2062 6f72         repay bor
-0005d170: 726f 7765 6420 6d61 7267 696e 2061 6e64  rowed margin and
-0005d180: 2069 6e74 6572 6573 740a 2020 2020 2020   interest.      
-0005d190: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
-0005d1a0: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
-0005d1b0: 6875 622e 696f 2f64 6f63 732f 7370 6f74  hub.io/docs/spot
-0005d1c0: 2f76 332f 2374 2d72 6570 6179 6d61 7267  /v3/#t-repaymarg
-0005d1d0: 696e 6c6f 616e 0a20 2020 2020 2020 203a  inloan.        :
-0005d1e0: 7061 7261 6d20 7374 7220 636f 6465 3a20  param str code: 
-0005d1f0: 756e 6966 6965 6420 6375 7272 656e 6379  unified currency
-0005d200: 2063 6f64 6520 6f66 2074 6865 2063 7572   code of the cur
-0005d210: 7265 6e63 7920 746f 2072 6570 6179 0a20  rency to repay. 
-0005d220: 2020 2020 2020 203a 7061 7261 6d20 666c         :param fl
-0005d230: 6f61 7420 616d 6f75 6e74 3a20 7468 6520  oat amount: the 
-0005d240: 616d 6f75 6e74 2074 6f20 7265 7061 790a  amount to repay.
-0005d250: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0005d260: 7472 7c4e 6f6e 6520 7379 6d62 6f6c 3a20  tr|None symbol: 
-0005d270: 6e6f 7420 7573 6564 2062 7920 6279 6269  not used by bybi
-0005d280: 742e 7265 7061 794d 6172 6769 6e28 290a  t.repayMargin().
-0005d290: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-0005d2a0: 6963 7420 7061 7261 6d73 3a20 6578 7472  ict params: extr
-0005d2b0: 6120 7061 7261 6d65 7465 7273 2073 7065  a parameters spe
-0005d2c0: 6369 6669 6320 746f 2074 6865 2062 7962  cific to the byb
-0005d2d0: 6974 2061 7069 2065 6e64 706f 696e 740a  it api endpoint.
-0005d2e0: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
-0005d2f0: 2064 6963 743a 2061 2060 6d61 7267 696e   dict: a `margin
-0005d300: 206c 6f61 6e20 7374 7275 6374 7572 6520   loan structure 
-0005d310: 3c68 7474 7073 3a2f 2f64 6f63 732e 6363  <https://docs.cc
-0005d320: 7874 2e63 6f6d 2f23 2f3f 6964 3d6d 6172  xt.com/#/?id=mar
-0005d330: 6769 6e2d 6c6f 616e 2d73 7472 7563 7475  gin-loan-structu
-0005d340: 7265 3e60 0a20 2020 2020 2020 2022 2222  re>`.        """
-0005d350: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-0005d360: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
-0005d370: 2829 0a20 2020 2020 2020 2063 7572 7265  ().        curre
-0005d380: 6e63 7920 3d20 7365 6c66 2e63 7572 7265  ncy = self.curre
-0005d390: 6e63 7928 636f 6465 290a 2020 2020 2020  ncy(code).      
-0005d3a0: 2020 6d61 7267 696e 4d6f 6465 2c20 7175    marginMode, qu
-0005d3b0: 6572 7920 3d20 7365 6c66 2e68 616e 646c  ery = self.handl
-0005d3c0: 655f 6d61 7267 696e 5f6d 6f64 655f 616e  e_margin_mode_an
-0005d3d0: 645f 7061 7261 6d73 2827 7265 7061 794d  d_params('repayM
-0005d3e0: 6172 6769 6e27 2c20 7061 7261 6d73 290a  argin', params).
-0005d3f0: 2020 2020 2020 2020 6966 206d 6172 6769          if margi
-0005d400: 6e4d 6f64 6520 3d3d 2027 6973 6f6c 6174  nMode == 'isolat
-0005d410: 6564 273a 0a20 2020 2020 2020 2020 2020  ed':.           
-0005d420: 2072 6169 7365 204e 6f74 5375 7070 6f72   raise NotSuppor
-0005d430: 7465 6428 7365 6c66 2e69 6420 2b20 2720  ted(self.id + ' 
-0005d440: 7265 7061 794d 6172 6769 6e28 2920 6361  repayMargin() ca
-0005d450: 6e6e 6f74 2075 7365 2069 736f 6c61 7465  nnot use isolate
-0005d460: 6420 6d61 7267 696e 2729 0a20 2020 2020  d margin').     
-0005d470: 2020 2072 6571 7565 7374 203d 207b 0a20     request = {. 
-0005d480: 2020 2020 2020 2020 2020 2027 636f 696e             'coin
-0005d490: 273a 2063 7572 7265 6e63 795b 2769 6427  ': currency['id'
-0005d4a0: 5d2c 0a20 2020 2020 2020 2020 2020 2027  ],.            '
-0005d4b0: 7174 7927 3a20 7365 6c66 2e6e 756d 6265  qty': self.numbe
-0005d4c0: 725f 746f 5f73 7472 696e 6728 616d 6f75  r_to_string(amou
-0005d4d0: 6e74 292c 0a20 2020 2020 2020 207d 0a20  nt),.        }. 
-0005d4e0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0005d4f0: 3d20 6177 6169 7420 7365 6c66 2e70 7269  = await self.pri
-0005d500: 7661 7465 506f 7374 5370 6f74 5633 5072  vatePostSpotV3Pr
-0005d510: 6976 6174 6543 726f 7373 4d61 7267 696e  ivateCrossMargin
-0005d520: 5265 7061 7928 7365 6c66 2e65 7874 656e  Repay(self.exten
-0005d530: 6428 7265 7175 6573 742c 2071 7565 7279  d(request, query
-0005d540: 2929 0a20 2020 2020 2020 2023 0a20 2020  )).        #.   
-0005d550: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
-0005d560: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005d570: 7265 7443 6f64 6522 3a20 302c 0a20 2020  retCode": 0,.   
-0005d580: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005d590: 7265 744d 7367 223a 2022 7375 6363 6573  retMsg": "succes
-0005d5a0: 7322 2c0a 2020 2020 2020 2020 2320 2020  s",.        #   
-0005d5b0: 2020 2020 2020 2272 6573 756c 7422 3a20        "result": 
-0005d5c0: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0005d5d0: 2020 2020 2020 2022 7265 7061 7949 6422         "repayId"
-0005d5e0: 3a20 2231 3231 3238 220a 2020 2020 2020  : "12128".      
-0005d5f0: 2020 2320 2020 2020 2020 2020 7d2c 0a20    #         },. 
-0005d600: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005d610: 2022 7265 7445 7874 496e 666f 223a 206e   "retExtInfo": n
-0005d620: 756c 6c2c 0a20 2020 2020 2020 2023 2020  ull,.        #  
-0005d630: 2020 2020 2020 2022 7469 6d65 223a 2031         "time": 1
-0005d640: 3636 3236 3138 3239 3834 3532 0a20 2020  662618298452.   
-0005d650: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-0005d660: 2020 2020 2023 0a20 2020 2020 2020 2072       #.        r
-0005d670: 6573 756c 7420 3d20 7365 6c66 2e73 6166  esult = self.saf
-0005d680: 655f 7661 6c75 6528 7265 7370 6f6e 7365  e_value(response
-0005d690: 2c20 2772 6573 756c 7427 2c20 7b7d 290a  , 'result', {}).
-0005d6a0: 2020 2020 2020 2020 7472 616e 7361 6374          transact
-0005d6b0: 696f 6e20 3d20 7365 6c66 2e70 6172 7365  ion = self.parse
-0005d6c0: 5f6d 6172 6769 6e5f 6c6f 616e 2872 6573  _margin_loan(res
-0005d6d0: 756c 742c 2063 7572 7265 6e63 7929 0a20  ult, currency). 
-0005d6e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0005d6f0: 6c66 2e65 7874 656e 6428 7472 616e 7361  lf.extend(transa
-0005d700: 6374 696f 6e2c 207b 0a20 2020 2020 2020  ction, {.       
-0005d710: 2020 2020 2027 7379 6d62 6f6c 273a 2073       'symbol': s
-0005d720: 796d 626f 6c2c 0a20 2020 2020 2020 2020  ymbol,.         
-0005d730: 2020 2027 616d 6f75 6e74 273a 2061 6d6f     'amount': amo
-0005d740: 756e 742c 0a20 2020 2020 2020 207d 290a  unt,.        }).
-0005d750: 0a20 2020 2064 6566 2070 6172 7365 5f6d  .    def parse_m
-0005d760: 6172 6769 6e5f 6c6f 616e 2873 656c 662c  argin_loan(self,
-0005d770: 2069 6e66 6f2c 2063 7572 7265 6e63 793d   info, currency=
-0005d780: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
-0005d790: 0a20 2020 2020 2020 2023 2062 6f72 726f  .        # borro
-0005d7a0: 774d 6172 6769 6e0a 2020 2020 2020 2020  wMargin.        
-0005d7b0: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
-0005d7c0: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0005d7d0: 2020 2020 2274 7261 6e73 6163 7449 6422      "transactId"
-0005d7e0: 3a20 2231 3431 3433 220a 2020 2020 2020  : "14143".      
-0005d7f0: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
-0005d800: 2020 230a 2020 2020 2020 2020 2320 7265    #.        # re
-0005d810: 7061 794d 6172 6769 6e0a 2020 2020 2020  payMargin.      
-0005d820: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
-0005d830: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-0005d840: 2020 2020 2020 2272 6570 6179 4964 223a        "repayId":
-0005d850: 2022 3132 3132 3822 0a20 2020 2020 2020   "12128".       
-0005d860: 2023 2020 2020 207d 0a20 2020 2020 2020   #     }.       
-0005d870: 2023 0a20 2020 2020 2020 2072 6574 7572   #.        retur
-0005d880: 6e20 7b0a 2020 2020 2020 2020 2020 2020  n {.            
-0005d890: 2769 6427 3a20 7365 6c66 2e73 6166 655f  'id': self.safe_
-0005d8a0: 7374 7269 6e67 5f32 2869 6e66 6f2c 2027  string_2(info, '
-0005d8b0: 7472 616e 7361 6374 4964 272c 2027 7265  transactId', 're
-0005d8c0: 7061 7949 6427 292c 0a20 2020 2020 2020  payId'),.       
-0005d8d0: 2020 2020 2027 6375 7272 656e 6379 273a       'currency':
-0005d8e0: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
-0005d8f0: 6728 6375 7272 656e 6379 2c20 2763 6f64  g(currency, 'cod
-0005d900: 6527 292c 0a20 2020 2020 2020 2020 2020  e'),.           
-0005d910: 2027 616d 6f75 6e74 273a 204e 6f6e 652c   'amount': None,
-0005d920: 0a20 2020 2020 2020 2020 2020 2027 7379  .            'sy
-0005d930: 6d62 6f6c 273a 204e 6f6e 652c 0a20 2020  mbol': None,.   
-0005d940: 2020 2020 2020 2020 2027 7469 6d65 7374           'timest
-0005d950: 616d 7027 3a20 4e6f 6e65 2c0a 2020 2020  amp': None,.    
-0005d960: 2020 2020 2020 2020 2764 6174 6574 696d          'datetim
-0005d970: 6527 3a20 4e6f 6e65 2c0a 2020 2020 2020  e': None,.      
-0005d980: 2020 2020 2020 2769 6e66 6f27 3a20 696e        'info': in
-0005d990: 666f 2c0a 2020 2020 2020 2020 7d0a 0a20  fo,.        }.. 
-0005d9a0: 2020 2064 6566 2070 6172 7365 5f74 7261     def parse_tra
-0005d9b0: 6e73 6665 725f 7374 6174 7573 2873 656c  nsfer_status(sel
-0005d9c0: 662c 2073 7461 7475 7329 3a0a 2020 2020  f, status):.    
-0005d9d0: 2020 2020 7374 6174 7573 6573 203d 207b      statuses = {
-0005d9e0: 0a20 2020 2020 2020 2020 2020 2027 3027  .            '0'
-0005d9f0: 3a20 276f 6b27 2c0a 2020 2020 2020 2020  : 'ok',.        
-0005da00: 2020 2020 274f 4b27 3a20 276f 6b27 2c0a      'OK': 'ok',.
-0005da10: 2020 2020 2020 2020 2020 2020 2753 5543              'SUC
-0005da20: 4345 5353 273a 2027 6f6b 272c 0a20 2020  CESS': 'ok',.   
-0005da30: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
-0005da40: 6574 7572 6e20 7365 6c66 2e73 6166 655f  eturn self.safe_
-0005da50: 7374 7269 6e67 2873 7461 7475 7365 732c  string(statuses,
-0005da60: 2073 7461 7475 732c 2073 7461 7475 7329   status, status)
-0005da70: 0a0a 2020 2020 6465 6620 7061 7273 655f  ..    def parse_
-0005da80: 7472 616e 7366 6572 2873 656c 662c 2074  transfer(self, t
-0005da90: 7261 6e73 6665 722c 2063 7572 7265 6e63  ransfer, currenc
-0005daa0: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0005dab0: 2023 0a20 2020 2020 2020 2023 2074 7261   #.        # tra
-0005dac0: 6e73 6665 720a 2020 2020 2020 2020 230a  nsfer.        #.
-0005dad0: 2020 2020 2020 2020 2320 2020 2020 7b0a          #     {.
-0005dae0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005daf0: 2020 2274 7261 6e73 6665 7249 6422 3a20    "transferId": 
-0005db00: 2232 3263 3262 6331 312d 6564 3562 2d34  "22c2bc11-ed5b-4
-0005db10: 3961 342d 3836 3437 2d63 3465 3066 3566  9a4-8647-c4e0f5f
-0005db20: 3666 3262 3222 2020 2320 7472 616e 7366  6f2b2"  # transf
-0005db30: 6572 5f69 6420 696e 2076 310a 2020 2020  er_id in v1.    
-0005db40: 2020 2020 2320 2020 2020 7d0a 2020 2020      #     }.    
-0005db50: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
-0005db60: 6665 7463 6854 7261 6e73 6665 7273 0a20  fetchTransfers. 
-0005db70: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0005db80: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
-0005db90: 2023 2020 2020 2020 2020 2022 7472 616e   #         "tran
-0005dba0: 7366 6572 4964 223a 2022 6539 6334 3231  sferId": "e9c421
-0005dbb0: 6334 2d62 3031 302d 3462 3136 2d61 6264  c4-b010-4b16-abd
-0005dbc0: 362d 3130 3631 3739 6632 3737 3032 222c  6-106179f27702",
-0005dbd0: 2020 2320 7472 616e 7366 6572 5f69 6420    # transfer_id 
-0005dbe0: 696e 2076 310a 2020 2020 2020 2020 2320  in v1.        # 
-0005dbf0: 2020 2020 2020 2020 2263 6f69 6e22 3a20          "coin": 
-0005dc00: 2255 5344 5422 2c0a 2020 2020 2020 2020  "USDT",.        
-0005dc10: 2320 2020 2020 2020 2020 2261 6d6f 756e  #         "amoun
-0005dc20: 7422 3a20 2238 222c 0a20 2020 2020 2020  t": "8",.       
-0005dc30: 2023 2020 2020 2020 2020 2022 6672 6f6d   #         "from
-0005dc40: 4163 636f 756e 7454 7970 6522 3a20 2246  AccountType": "F
-0005dc50: 554e 4422 2c20 2023 2066 726f 6d5f 6163  UND",  # from_ac
-0005dc60: 636f 756e 745f 7479 7065 2069 6e20 7631  count_type in v1
-0005dc70: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005dc80: 2020 2022 746f 4163 636f 756e 7454 7970     "toAccountTyp
-0005dc90: 6522 3a20 2253 504f 5422 2c20 2023 2074  e": "SPOT",  # t
-0005dca0: 6f5f 6163 636f 756e 745f 7479 7065 2069  o_account_type i
-0005dcb0: 6e20 7631 0a20 2020 2020 2020 2023 2020  n v1.        #  
-0005dcc0: 2020 2020 2020 2022 7469 6d65 7374 616d         "timestam
-0005dcd0: 7022 3a20 2231 3636 3638 3739 3432 3630  p": "16668794260
-0005dce0: 3030 222c 0a20 2020 2020 2020 2023 2020  00",.        #  
-0005dcf0: 2020 2020 2020 2022 7374 6174 7573 223a         "status":
-0005dd00: 2022 5355 4343 4553 5322 0a20 2020 2020   "SUCCESS".     
-0005dd10: 2020 2023 2020 2020 2020 7d0a 2020 2020     #      }.    
-0005dd20: 2020 2020 230a 2020 2020 2020 2020 6375      #.        cu
-0005dd30: 7272 656e 6379 4964 203d 2073 656c 662e  rrencyId = self.
-0005dd40: 7361 6665 5f73 7472 696e 6728 7472 616e  safe_string(tran
-0005dd50: 7366 6572 2c20 2763 6f69 6e27 290a 2020  sfer, 'coin').  
-0005dd60: 2020 2020 2020 7469 6d65 7374 616d 7020        timestamp 
-0005dd70: 3d20 7365 6c66 2e73 6166 655f 696e 7465  = self.safe_inte
-0005dd80: 6765 7228 7472 616e 7366 6572 2c20 2774  ger(transfer, 't
-0005dd90: 696d 6573 7461 6d70 2729 0a20 2020 2020  imestamp').     
-0005dda0: 2020 2066 726f 6d41 6363 6f75 6e74 4964     fromAccountId
-0005ddb0: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
-0005ddc0: 696e 675f 3228 7472 616e 7366 6572 2c20  ing_2(transfer, 
-0005ddd0: 2766 726f 6d41 6363 6f75 6e74 5479 7065  'fromAccountType
-0005dde0: 272c 2027 6672 6f6d 5f61 6363 6f75 6e74  ', 'from_account
-0005ddf0: 5f74 7970 6527 290a 2020 2020 2020 2020  _type').        
-0005de00: 746f 4163 636f 756e 7449 6420 3d20 7365  toAccountId = se
-0005de10: 6c66 2e73 6166 655f 7374 7269 6e67 5f32  lf.safe_string_2
-0005de20: 2874 7261 6e73 6665 722c 2027 746f 4163  (transfer, 'toAc
-0005de30: 636f 756e 7454 7970 6527 2c20 2774 6f5f  countType', 'to_
-0005de40: 6163 636f 756e 745f 7479 7065 2729 0a20  account_type'). 
-0005de50: 2020 2020 2020 2061 6363 6f75 6e74 4964         accountId
-0005de60: 7320 3d20 7365 6c66 2e73 6166 655f 7661  s = self.safe_va
-0005de70: 6c75 6528 7365 6c66 2e6f 7074 696f 6e73  lue(self.options
-0005de80: 2c20 2761 6363 6f75 6e74 7342 7949 6427  , 'accountsById'
-0005de90: 2c20 7b7d 290a 2020 2020 2020 2020 6672  , {}).        fr
-0005dea0: 6f6d 4163 636f 756e 7420 3d20 7365 6c66  omAccount = self
-0005deb0: 2e73 6166 655f 7374 7269 6e67 2861 6363  .safe_string(acc
-0005dec0: 6f75 6e74 4964 732c 2066 726f 6d41 6363  ountIds, fromAcc
-0005ded0: 6f75 6e74 4964 2c20 6672 6f6d 4163 636f  ountId, fromAcco
-0005dee0: 756e 7449 6429 0a20 2020 2020 2020 2074  untId).        t
-0005def0: 6f41 6363 6f75 6e74 203d 2073 656c 662e  oAccount = self.
-0005df00: 7361 6665 5f73 7472 696e 6728 6163 636f  safe_string(acco
-0005df10: 756e 7449 6473 2c20 746f 4163 636f 756e  untIds, toAccoun
-0005df20: 7449 642c 2074 6f41 6363 6f75 6e74 4964  tId, toAccountId
-0005df30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0005df40: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0005df50: 696e 666f 273a 2074 7261 6e73 6665 722c  info': transfer,
-0005df60: 0a20 2020 2020 2020 2020 2020 2027 6964  .            'id
-0005df70: 273a 2073 656c 662e 7361 6665 5f73 7472  ': self.safe_str
-0005df80: 696e 675f 3228 7472 616e 7366 6572 2c20  ing_2(transfer, 
-0005df90: 2774 7261 6e73 6665 7249 6427 2c20 2774  'transferId', 't
-0005dfa0: 7261 6e73 6665 725f 6964 2729 2c0a 2020  ransfer_id'),.  
-0005dfb0: 2020 2020 2020 2020 2020 2774 696d 6573            'times
-0005dfc0: 7461 6d70 273a 2074 696d 6573 7461 6d70  tamp': timestamp
-0005dfd0: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
-0005dfe0: 6174 6574 696d 6527 3a20 7365 6c66 2e69  atetime': self.i
-0005dff0: 736f 3836 3031 2874 696d 6573 7461 6d70  so8601(timestamp
-0005e000: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
-0005e010: 6375 7272 656e 6379 273a 2073 656c 662e  currency': self.
-0005e020: 7361 6665 5f63 7572 7265 6e63 795f 636f  safe_currency_co
-0005e030: 6465 2863 7572 7265 6e63 7949 642c 2063  de(currencyId, c
-0005e040: 7572 7265 6e63 7929 2c0a 2020 2020 2020  urrency),.      
-0005e050: 2020 2020 2020 2761 6d6f 756e 7427 3a20        'amount': 
-0005e060: 7365 6c66 2e73 6166 655f 6e75 6d62 6572  self.safe_number
-0005e070: 2874 7261 6e73 6665 722c 2027 616d 6f75  (transfer, 'amou
-0005e080: 6e74 2729 2c0a 2020 2020 2020 2020 2020  nt'),.          
-0005e090: 2020 2766 726f 6d41 6363 6f75 6e74 273a    'fromAccount':
-0005e0a0: 2066 726f 6d41 6363 6f75 6e74 2c0a 2020   fromAccount,.  
-0005e0b0: 2020 2020 2020 2020 2020 2774 6f41 6363            'toAcc
-0005e0c0: 6f75 6e74 273a 2074 6f41 6363 6f75 6e74  ount': toAccount
-0005e0d0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-0005e0e0: 7461 7475 7327 3a20 7365 6c66 2e70 6172  tatus': self.par
-0005e0f0: 7365 5f74 7261 6e73 6665 725f 7374 6174  se_transfer_stat
-0005e100: 7573 2873 656c 662e 7361 6665 5f73 7472  us(self.safe_str
-0005e110: 696e 6728 7472 616e 7366 6572 2c20 2773  ing(transfer, 's
-0005e120: 7461 7475 7327 2929 2c0a 2020 2020 2020  tatus')),.      
-0005e130: 2020 7d0a 0a20 2020 2061 7379 6e63 2064    }..    async d
-0005e140: 6566 2066 6574 6368 5f64 6572 6976 6174  ef fetch_derivat
-0005e150: 6976 6573 5f6d 6172 6b65 745f 6c65 7665  ives_market_leve
-0005e160: 7261 6765 5f74 6965 7273 2873 656c 662c  rage_tiers(self,
-0005e170: 2073 796d 626f 6c3a 2073 7472 2c20 7061   symbol: str, pa
-0005e180: 7261 6d73 3d7b 7d29 3a0a 2020 2020 2020  rams={}):.      
-0005e190: 2020 6177 6169 7420 7365 6c66 2e6c 6f61    await self.loa
-0005e1a0: 645f 6d61 726b 6574 7328 290a 2020 2020  d_markets().    
-0005e1b0: 2020 2020 6d61 726b 6574 203d 2073 656c      market = sel
-0005e1c0: 662e 6d61 726b 6574 2873 796d 626f 6c29  f.market(symbol)
-0005e1d0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0005e1e0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0005e1f0: 2027 7379 6d62 6f6c 273a 206d 6172 6b65   'symbol': marke
-0005e200: 745b 2769 6427 5d2c 0a20 2020 2020 2020  t['id'],.       
-0005e210: 207d 0a20 2020 2020 2020 2069 6620 6d61   }.        if ma
-0005e220: 726b 6574 5b27 6c69 6e65 6172 275d 3a0a  rket['linear']:.
-0005e230: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0005e240: 6573 745b 2763 6174 6567 6f72 7927 5d20  est['category'] 
-0005e250: 3d20 276c 696e 6561 7227 0a20 2020 2020  = 'linear'.     
-0005e260: 2020 2065 6c69 6620 6d61 726b 6574 5b27     elif market['
-0005e270: 696e 7665 7273 6527 5d3a 0a20 2020 2020  inverse']:.     
-0005e280: 2020 2020 2020 2072 6571 7565 7374 5b27         request['
-0005e290: 6361 7465 676f 7279 275d 203d 2027 696e  category'] = 'in
-0005e2a0: 7665 7273 6527 0a20 2020 2020 2020 2072  verse'.        r
-0005e2b0: 6573 706f 6e73 6520 3d20 6177 6169 7420  esponse = await 
-0005e2c0: 7365 6c66 2e70 7562 6c69 6347 6574 5635  self.publicGetV5
-0005e2d0: 4d61 726b 6574 5269 736b 4c69 6d69 7428  MarketRiskLimit(
-0005e2e0: 7365 6c66 2e65 7874 656e 6428 7265 7175  self.extend(requ
-0005e2f0: 6573 742c 2070 6172 616d 7329 290a 2020  est, params)).  
-0005e300: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-0005e310: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
-0005e320: 2320 2020 2020 2020 2020 2272 6574 436f  #         "retCo
-0005e330: 6465 223a 2030 2c0a 2020 2020 2020 2020  de": 0,.        
-0005e340: 2320 2020 2020 2020 2020 2272 6574 4d73  #         "retMs
-0005e350: 6722 3a20 224f 4b22 2c0a 2020 2020 2020  g": "OK",.      
-0005e360: 2020 2320 2020 2020 2020 2020 2272 6573    #         "res
-0005e370: 756c 7422 3a20 7b0a 2020 2020 2020 2020  ult": {.        
-0005e380: 2320 2020 2020 2020 2020 2020 2020 2263  #             "c
-0005e390: 6174 6567 6f72 7922 3a20 2269 6e76 6572  ategory": "inver
-0005e3a0: 7365 222c 0a20 2020 2020 2020 2023 2020  se",.        #  
-0005e3b0: 2020 2020 2020 2020 2020 2022 6c69 7374             "list
-0005e3c0: 223a 205b 0a20 2020 2020 2020 2023 2020  ": [.        #  
-0005e3d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0005e3e0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005e3f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0005e400: 6964 223a 2031 2c0a 2020 2020 2020 2020  id": 1,.        
-0005e410: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0005e420: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
-0005e430: 2242 5443 5553 4422 2c0a 2020 2020 2020  "BTCUSD",.      
-0005e440: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005e450: 2020 2020 2020 2020 2272 6973 6b4c 696d          "riskLim
-0005e460: 6974 5661 6c75 6522 3a20 2231 3530 222c  itValue": "150",
-0005e470: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005e480: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0005e490: 6d61 696e 7465 6e61 6e63 654d 6172 6769  maintenanceMargi
-0005e4a0: 6e22 3a20 2230 2e35 222c 0a20 2020 2020  n": "0.5",.     
-0005e4b0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005e4c0: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
-0005e4d0: 6c4d 6172 6769 6e22 3a20 2231 222c 0a20  lMargin": "1",. 
-0005e4e0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005e4f0: 2020 2020 2020 2020 2020 2020 2022 6973               "is
-0005e500: 4c6f 7765 7374 5269 736b 223a 2031 2c0a  LowestRisk": 1,.
-0005e510: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005e520: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0005e530: 6178 4c65 7665 7261 6765 223a 2022 3130  axLeverage": "10
-0005e540: 302e 3030 220a 2020 2020 2020 2020 2320  0.00".        # 
-0005e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005e560: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
-0005e570: 2020 2020 2020 2020 202e 2e2e 2e0a 2020           .....  
-0005e580: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005e590: 2020 2020 5d0a 2020 2020 2020 2020 2320      ].        # 
-0005e5a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-0005e5b0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
-0005e5c0: 7445 7874 496e 666f 223a 207b 7d2c 0a20  tExtInfo": {},. 
-0005e5d0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005e5e0: 2022 7469 6d65 223a 2031 3637 3230 3534   "time": 1672054
-0005e5f0: 3438 3830 3130 0a20 2020 2020 2020 2023  488010.        #
-0005e600: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0005e610: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0005e620: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
-0005e630: 6528 7265 7370 6f6e 7365 2c20 2772 6573  e(response, 'res
-0005e640: 756c 7427 290a 2020 2020 2020 2020 7469  ult').        ti
-0005e650: 6572 7320 3d20 7365 6c66 2e73 6166 655f  ers = self.safe_
-0005e660: 7661 6c75 6528 7265 7375 6c74 2c20 276c  value(result, 'l
-0005e670: 6973 7427 290a 2020 2020 2020 2020 7265  ist').        re
-0005e680: 7475 726e 2073 656c 662e 7061 7273 655f  turn self.parse_
-0005e690: 6d61 726b 6574 5f6c 6576 6572 6167 655f  market_leverage_
-0005e6a0: 7469 6572 7328 7469 6572 732c 206d 6172  tiers(tiers, mar
-0005e6b0: 6b65 7429 0a0a 2020 2020 6173 796e 6320  ket)..    async 
-0005e6c0: 6465 6620 6665 7463 685f 6d61 726b 6574  def fetch_market
-0005e6d0: 5f6c 6576 6572 6167 655f 7469 6572 7328  _leverage_tiers(
-0005e6e0: 7365 6c66 2c20 7379 6d62 6f6c 3a20 7374  self, symbol: st
-0005e6f0: 722c 2070 6172 616d 733d 7b7d 293a 0a20  r, params={}):. 
-0005e700: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0005e710: 2020 2072 6574 7269 6576 6520 696e 666f     retrieve info
-0005e720: 726d 6174 696f 6e20 6f6e 2074 6865 206d  rmation on the m
-0005e730: 6178 696d 756d 206c 6576 6572 6167 652c  aximum leverage,
-0005e740: 2061 6e64 206d 6169 6e74 656e 616e 6365   and maintenance
-0005e750: 206d 6172 6769 6e20 666f 7220 7472 6164   margin for trad
-0005e760: 6573 206f 6620 7661 7279 696e 6720 7472  es of varying tr
-0005e770: 6164 6520 7369 7a65 7320 666f 7220 6120  ade sizes for a 
-0005e780: 7369 6e67 6c65 206d 6172 6b65 740a 2020  single market.  
-0005e790: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
-0005e7a0: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
-0005e7b0: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
-0005e7c0: 7635 2f6d 6172 6b65 742f 7269 736b 2d6c  v5/market/risk-l
-0005e7d0: 696d 6974 0a20 2020 2020 2020 203a 7061  imit.        :pa
-0005e7e0: 7261 6d20 7374 7220 7379 6d62 6f6c 3a20  ram str symbol: 
-0005e7f0: 756e 6966 6965 6420 6d61 726b 6574 2073  unified market s
-0005e800: 796d 626f 6c0a 2020 2020 2020 2020 3a70  ymbol.        :p
-0005e810: 6172 616d 2064 6963 7420 7061 7261 6d73  aram dict params
-0005e820: 3a20 6578 7472 6120 7061 7261 6d65 7465  : extra paramete
-0005e830: 7273 2073 7065 6369 6669 6320 746f 2074  rs specific to t
-0005e840: 6865 2062 7962 6974 2061 7069 2065 6e64  he bybit api end
-0005e850: 706f 696e 740a 2020 2020 2020 2020 3a72  point.        :r
-0005e860: 6574 7572 6e73 2064 6963 743a 2061 2060  eturns dict: a `
-0005e870: 6c65 7665 7261 6765 2074 6965 7273 2073  leverage tiers s
-0005e880: 7472 7563 7475 7265 203c 6874 7470 733a  tructure <https:
-0005e890: 2f2f 646f 6373 2e63 6378 742e 636f 6d2f  //docs.ccxt.com/
-0005e8a0: 232f 3f69 643d 6c65 7665 7261 6765 2d74  #/?id=leverage-t
-0005e8b0: 6965 7273 2d73 7472 7563 7475 7265 3e60  iers-structure>`
-0005e8c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0005e8d0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-0005e8e0: 6c6f 6164 5f6d 6172 6b65 7473 2829 0a20  load_markets(). 
-0005e8f0: 2020 2020 2020 2072 6571 7565 7374 203d         request =
-0005e900: 207b 7d0a 2020 2020 2020 2020 6d61 726b   {}.        mark
-0005e910: 6574 203d 204e 6f6e 650a 2020 2020 2020  et = None.      
-0005e920: 2020 6d61 726b 6574 203d 2073 656c 662e    market = self.
-0005e930: 6d61 726b 6574 2873 796d 626f 6c29 0a20  market(symbol). 
-0005e940: 2020 2020 2020 2069 6620 6d61 726b 6574         if market
-0005e950: 5b27 7370 6f74 275d 206f 7220 6d61 726b  ['spot'] or mark
-0005e960: 6574 5b27 6f70 7469 6f6e 275d 3a0a 2020  et['option']:.  
-0005e970: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0005e980: 4261 6452 6571 7565 7374 2873 656c 662e  BadRequest(self.
-0005e990: 6964 202b 2027 2066 6574 6368 4d61 726b  id + ' fetchMark
-0005e9a0: 6574 4c65 7665 7261 6765 5469 6572 7328  etLeverageTiers(
-0005e9b0: 2920 7379 6d62 6f6c 2064 6f65 7320 6e6f  ) symbol does no
-0005e9c0: 7420 7375 7070 6f72 7420 6d61 726b 6574  t support market
-0005e9d0: 2027 202b 2073 796d 626f 6c29 0a20 2020   ' + symbol).   
-0005e9e0: 2020 2020 2072 6571 7565 7374 5b27 7379       request['sy
-0005e9f0: 6d62 6f6c 275d 203d 206d 6172 6b65 745b  mbol'] = market[
-0005ea00: 2769 6427 5d0a 2020 2020 2020 2020 7265  'id'].        re
-0005ea10: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-0005ea20: 6665 7463 685f 6465 7269 7661 7469 7665  fetch_derivative
-0005ea30: 735f 6d61 726b 6574 5f6c 6576 6572 6167  s_market_leverag
-0005ea40: 655f 7469 6572 7328 7379 6d62 6f6c 2c20  e_tiers(symbol, 
-0005ea50: 7061 7261 6d73 290a 0a20 2020 2064 6566  params)..    def
-0005ea60: 2070 6172 7365 5f6d 6172 6b65 745f 6c65   parse_market_le
-0005ea70: 7665 7261 6765 5f74 6965 7273 2873 656c  verage_tiers(sel
-0005ea80: 662c 2069 6e66 6f2c 206d 6172 6b65 743d  f, info, market=
-0005ea90: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
-0005eaa0: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
-0005eab0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005eac0: 2020 2022 6964 223a 2031 2c0a 2020 2020     "id": 1,.    
-0005ead0: 2020 2020 2320 2020 2020 2020 2020 2273      #         "s
-0005eae0: 796d 626f 6c22 3a20 2242 5443 5553 4422  ymbol": "BTCUSD"
-0005eaf0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0005eb00: 2020 2020 2272 6973 6b4c 696d 6974 5661      "riskLimitVa
-0005eb10: 6c75 6522 3a20 2231 3530 222c 0a20 2020  lue": "150",.   
-0005eb20: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005eb30: 6d61 696e 7465 6e61 6e63 654d 6172 6769  maintenanceMargi
-0005eb40: 6e22 3a20 2230 2e35 222c 0a20 2020 2020  n": "0.5",.     
-0005eb50: 2020 2023 2020 2020 2020 2020 2022 696e     #         "in
-0005eb60: 6974 6961 6c4d 6172 6769 6e22 3a20 2231  itialMargin": "1
-0005eb70: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005eb80: 2020 2020 2022 6973 4c6f 7765 7374 5269       "isLowestRi
-0005eb90: 736b 223a 2031 2c0a 2020 2020 2020 2020  sk": 1,.        
-0005eba0: 2320 2020 2020 2020 2020 226d 6178 4c65  #         "maxLe
-0005ebb0: 7665 7261 6765 223a 2022 3130 302e 3030  verage": "100.00
-0005ebc0: 220a 2020 2020 2020 2020 2320 2020 2020  ".        #     
-0005ebd0: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
-0005ebe0: 2020 2020 6d69 6e4e 6f74 696f 6e61 6c20      minNotional 
-0005ebf0: 3d20 300a 2020 2020 2020 2020 7469 6572  = 0.        tier
-0005ec00: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-0005ec10: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-0005ec20: 206c 656e 2869 6e66 6f29 293a 0a20 2020   len(info)):.   
-0005ec30: 2020 2020 2020 2020 2069 7465 6d20 3d20           item = 
-0005ec40: 696e 666f 5b69 5d0a 2020 2020 2020 2020  info[i].        
-0005ec50: 2020 2020 6d61 784e 6f74 696f 6e61 6c20      maxNotional 
-0005ec60: 3d20 7365 6c66 2e73 6166 655f 6e75 6d62  = self.safe_numb
-0005ec70: 6572 2869 7465 6d2c 2027 7269 736b 4c69  er(item, 'riskLi
-0005ec80: 6d69 7456 616c 7565 2729 0a20 2020 2020  mitValue').     
-0005ec90: 2020 2020 2020 2074 6965 7273 2e61 7070         tiers.app
-0005eca0: 656e 6428 7b0a 2020 2020 2020 2020 2020  end({.          
-0005ecb0: 2020 2020 2020 2774 6965 7227 3a20 7365        'tier': se
-0005ecc0: 6c66 2e73 756d 2869 2c20 3129 2c0a 2020  lf.sum(i, 1),.  
-0005ecd0: 2020 2020 2020 2020 2020 2020 2020 2763                'c
-0005ece0: 7572 7265 6e63 7927 3a20 6d61 726b 6574  urrency': market
-0005ecf0: 5b27 6261 7365 275d 2c0a 2020 2020 2020  ['base'],.      
-0005ed00: 2020 2020 2020 2020 2020 276d 696e 4e6f            'minNo
-0005ed10: 7469 6f6e 616c 273a 206d 696e 4e6f 7469  tional': minNoti
-0005ed20: 6f6e 616c 2c0a 2020 2020 2020 2020 2020  onal,.          
-0005ed30: 2020 2020 2020 276d 6178 4e6f 7469 6f6e        'maxNotion
-0005ed40: 616c 273a 206d 6178 4e6f 7469 6f6e 616c  al': maxNotional
-0005ed50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0005ed60: 2020 276d 6169 6e74 656e 616e 6365 4d61    'maintenanceMa
-0005ed70: 7267 696e 5261 7465 273a 2073 656c 662e  rginRate': self.
-0005ed80: 7361 6665 5f6e 756d 6265 7228 6974 656d  safe_number(item
-0005ed90: 2c20 276d 6169 6e74 656e 616e 6365 4d61  , 'maintenanceMa
-0005eda0: 7267 696e 2729 2c0a 2020 2020 2020 2020  rgin'),.        
-0005edb0: 2020 2020 2020 2020 276d 6178 4c65 7665          'maxLeve
-0005edc0: 7261 6765 273a 2073 656c 662e 7361 6665  rage': self.safe
-0005edd0: 5f6e 756d 6265 7228 6974 656d 2c20 276d  _number(item, 'm
-0005ede0: 6178 4c65 7665 7261 6765 2729 2c0a 2020  axLeverage'),.  
-0005edf0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
-0005ee00: 6e66 6f27 3a20 6974 656d 2c0a 2020 2020  nfo': item,.    
-0005ee10: 2020 2020 2020 2020 7d29 0a20 2020 2020          }).     
-0005ee20: 2020 2020 2020 206d 696e 4e6f 7469 6f6e         minNotion
-0005ee30: 616c 203d 206d 6178 4e6f 7469 6f6e 616c  al = maxNotional
-0005ee40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0005ee50: 7469 6572 730a 0a20 2020 2064 6566 2070  tiers..    def p
-0005ee60: 6172 7365 5f74 7261 6469 6e67 5f66 6565  arse_trading_fee
-0005ee70: 2873 656c 662c 2066 6565 2c20 6d61 726b  (self, fee, mark
-0005ee80: 6574 3d4e 6f6e 6529 3a0a 2020 2020 2020  et=None):.      
-0005ee90: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
-0005eea0: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-0005eeb0: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
-0005eec0: 2245 5448 5553 4454 222c 0a20 2020 2020  "ETHUSDT",.     
-0005eed0: 2020 2023 2020 2020 2020 2020 2022 6d61     #         "ma
-0005eee0: 6b65 7246 6565 5261 7465 223a 2030 2e30  kerFeeRate": 0.0
-0005eef0: 3031 2c0a 2020 2020 2020 2020 2320 2020  01,.        #   
-0005ef00: 2020 2020 2020 2274 616b 6572 4665 6552        "takerFeeR
-0005ef10: 6174 6522 3a20 302e 3030 310a 2020 2020  ate": 0.001.    
-0005ef20: 2020 2020 2320 2020 2020 7d0a 2020 2020      #     }.    
-0005ef30: 2020 2020 230a 2020 2020 2020 2020 6d61      #.        ma
-0005ef40: 726b 6574 4964 203d 2073 656c 662e 7361  rketId = self.sa
-0005ef50: 6665 5f73 7472 696e 6728 6665 652c 2027  fe_string(fee, '
-0005ef60: 7379 6d62 6f6c 2729 0a20 2020 2020 2020  symbol').       
-0005ef70: 2073 796d 626f 6c20 3d20 7365 6c66 2e73   symbol = self.s
-0005ef80: 6166 655f 7379 6d62 6f6c 286d 6172 6b65  afe_symbol(marke
-0005ef90: 7449 642c 204e 6f6e 652c 204e 6f6e 652c  tId, None, None,
-0005efa0: 2027 636f 6e74 7261 6374 2729 0a20 2020   'contract').   
-0005efb0: 2020 2020 2072 6574 7572 6e20 7b0a 2020       return {.  
-0005efc0: 2020 2020 2020 2020 2020 2769 6e66 6f27            'info'
-0005efd0: 3a20 6665 652c 0a20 2020 2020 2020 2020  : fee,.         
-0005efe0: 2020 2027 7379 6d62 6f6c 273a 2073 796d     'symbol': sym
-0005eff0: 626f 6c2c 0a20 2020 2020 2020 2020 2020  bol,.           
-0005f000: 2027 6d61 6b65 7227 3a20 7365 6c66 2e73   'maker': self.s
-0005f010: 6166 655f 6e75 6d62 6572 2866 6565 2c20  afe_number(fee, 
-0005f020: 276d 616b 6572 4665 6552 6174 6527 292c  'makerFeeRate'),
-0005f030: 0a20 2020 2020 2020 2020 2020 2027 7461  .            'ta
-0005f040: 6b65 7227 3a20 7365 6c66 2e73 6166 655f  ker': self.safe_
-0005f050: 6e75 6d62 6572 2866 6565 2c20 2774 616b  number(fee, 'tak
-0005f060: 6572 4665 6552 6174 6527 292c 0a20 2020  erFeeRate'),.   
-0005f070: 2020 2020 207d 0a0a 2020 2020 6173 796e       }..    asyn
-0005f080: 6320 6465 6620 6665 7463 685f 7472 6164  c def fetch_trad
-0005f090: 696e 675f 6665 6528 7365 6c66 2c20 7379  ing_fee(self, sy
-0005f0a0: 6d62 6f6c 3a20 7374 722c 2070 6172 616d  mbol: str, param
-0005f0b0: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
-0005f0c0: 2222 0a20 2020 2020 2020 2066 6574 6368  "".        fetch
-0005f0d0: 2074 6865 2074 7261 6469 6e67 2066 6565   the trading fee
-0005f0e0: 7320 666f 7220 6120 6d61 726b 6574 0a20  s for a market. 
-0005f0f0: 2020 2020 2020 2073 6565 2068 7474 7073         see https
-0005f100: 3a2f 2f62 7962 6974 2d65 7863 6861 6e67  ://bybit-exchang
-0005f110: 652e 6769 7468 7562 2e69 6f2f 646f 6373  e.github.io/docs
-0005f120: 2f76 352f 6163 636f 756e 742f 6665 652d  /v5/account/fee-
-0005f130: 7261 7465 0a20 2020 2020 2020 203a 7061  rate.        :pa
-0005f140: 7261 6d20 7374 7220 7379 6d62 6f6c 3a20  ram str symbol: 
-0005f150: 756e 6966 6965 6420 6d61 726b 6574 2073  unified market s
-0005f160: 796d 626f 6c0a 2020 2020 2020 2020 3a70  ymbol.        :p
-0005f170: 6172 616d 2064 6963 7420 7061 7261 6d73  aram dict params
-0005f180: 3a20 6578 7472 6120 7061 7261 6d65 7465  : extra paramete
-0005f190: 7273 2073 7065 6369 6669 6320 746f 2074  rs specific to t
-0005f1a0: 6865 2062 7962 6974 2061 7069 2065 6e64  he bybit api end
-0005f1b0: 706f 696e 740a 2020 2020 2020 2020 3a72  point.        :r
-0005f1c0: 6574 7572 6e73 2064 6963 743a 2061 2060  eturns dict: a `
-0005f1d0: 6665 6520 7374 7275 6374 7572 6520 3c68  fee structure <h
-0005f1e0: 7474 7073 3a2f 2f64 6f63 732e 6363 7874  ttps://docs.ccxt
-0005f1f0: 2e63 6f6d 2f23 2f3f 6964 3d66 6565 2d73  .com/#/?id=fee-s
-0005f200: 7472 7563 7475 7265 3e60 0a20 2020 2020  tructure>`.     
-0005f210: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-0005f220: 7761 6974 2073 656c 662e 6c6f 6164 5f6d  wait self.load_m
-0005f230: 6172 6b65 7473 2829 0a20 2020 2020 2020  arkets().       
-0005f240: 206d 6172 6b65 7420 3d20 7365 6c66 2e6d   market = self.m
-0005f250: 6172 6b65 7428 7379 6d62 6f6c 290a 2020  arket(symbol).  
-0005f260: 2020 2020 2020 6966 206d 6172 6b65 745b        if market[
-0005f270: 2773 706f 7427 5d3a 0a20 2020 2020 2020  'spot']:.       
-0005f280: 2020 2020 2072 6169 7365 204e 6f74 5375       raise NotSu
-0005f290: 7070 6f72 7465 6428 7365 6c66 2e69 6420  pported(self.id 
-0005f2a0: 2b20 2720 6665 7463 6854 7261 6469 6e67  + ' fetchTrading
-0005f2b0: 4665 6528 2920 6973 206e 6f74 2073 7570  Fee() is not sup
-0005f2c0: 706f 7274 6564 2066 6f72 2073 706f 7420  ported for spot 
-0005f2d0: 6d61 726b 6574 2729 0a20 2020 2020 2020  market').       
-0005f2e0: 2072 6571 7565 7374 203d 207b 0a20 2020   request = {.   
-0005f2f0: 2020 2020 2020 2020 2027 7379 6d62 6f6c           'symbol
-0005f300: 273a 206d 6172 6b65 745b 2769 6427 5d2c  ': market['id'],
-0005f310: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-0005f320: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
-0005f330: 6169 7420 7365 6c66 2e70 7269 7661 7465  ait self.private
-0005f340: 4765 7456 3541 6363 6f75 6e74 4665 6552  GetV5AccountFeeR
-0005f350: 6174 6528 7365 6c66 2e65 7874 656e 6428  ate(self.extend(
-0005f360: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
-0005f370: 290a 2020 2020 2020 2020 230a 2020 2020  ).        #.    
-0005f380: 2020 2020 2320 2020 2020 7b0a 2020 2020      #     {.    
-0005f390: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
-0005f3a0: 6574 436f 6465 223a 2030 2c0a 2020 2020  etCode": 0,.    
-0005f3b0: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
-0005f3c0: 6574 4d73 6722 3a20 224f 4b22 2c0a 2020  etMsg": "OK",.  
-0005f3d0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005f3e0: 2272 6573 756c 7422 3a20 7b0a 2020 2020  "result": {.    
-0005f3f0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005f400: 2020 226c 6973 7422 3a20 5b0a 2020 2020    "list": [.    
-0005f410: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005f420: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0005f430: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0005f440: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
-0005f450: 2245 5448 5553 4454 222c 0a20 2020 2020  "ETHUSDT",.     
-0005f460: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005f470: 2020 2020 2020 2020 2022 7461 6b65 7246           "takerF
-0005f480: 6565 5261 7465 223a 2022 302e 3030 3036  eeRate": "0.0006
-0005f490: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005f4b0: 2022 6d61 6b65 7246 6565 5261 7465 223a   "makerFeeRate":
-0005f4c0: 2022 302e 3030 3031 220a 2020 2020 2020   "0.0001".      
-0005f4d0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005f4e0: 2020 2020 7d0a 2020 2020 2020 2020 2320      }.        # 
-0005f4f0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-0005f500: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005f510: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
-0005f520: 2020 2020 2022 7265 7445 7874 496e 666f       "retExtInfo
-0005f530: 223a 207b 7d2c 0a20 2020 2020 2020 2023  ": {},.        #
-0005f540: 2020 2020 2020 2020 2022 7469 6d65 223a           "time":
-0005f550: 2031 3637 3633 3630 3431 3235 3736 0a20   1676360412576. 
-0005f560: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
-0005f570: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0005f580: 2072 6573 756c 7420 3d20 7365 6c66 2e73   result = self.s
-0005f590: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
-0005f5a0: 7365 2c20 2772 6573 756c 7427 2c20 7b7d  se, 'result', {}
-0005f5b0: 290a 2020 2020 2020 2020 6665 6573 203d  ).        fees =
-0005f5c0: 2073 656c 662e 7361 6665 5f76 616c 7565   self.safe_value
-0005f5d0: 2872 6573 756c 742c 2027 6c69 7374 272c  (result, 'list',
-0005f5e0: 205b 5d29 0a20 2020 2020 2020 2066 6972   []).        fir
-0005f5f0: 7374 203d 2073 656c 662e 7361 6665 5f76  st = self.safe_v
-0005f600: 616c 7565 2866 6565 732c 2030 2c20 7b7d  alue(fees, 0, {}
-0005f610: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0005f620: 2073 656c 662e 7061 7273 655f 7472 6164   self.parse_trad
-0005f630: 696e 675f 6665 6528 6669 7273 7429 0a0a  ing_fee(first)..
-0005f640: 2020 2020 6173 796e 6320 6465 6620 6665      async def fe
-0005f650: 7463 685f 7472 6164 696e 675f 6665 6573  tch_trading_fees
-0005f660: 2873 656c 662c 2070 6172 616d 733d 7b7d  (self, params={}
-0005f670: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0005f680: 2020 2020 2020 2066 6574 6368 2074 6865         fetch the
-0005f690: 2074 7261 6469 6e67 2066 6565 7320 666f   trading fees fo
-0005f6a0: 7220 6d75 6c74 6970 6c65 206d 6172 6b65  r multiple marke
-0005f6b0: 7473 0a20 2020 2020 2020 2073 6565 2068  ts.        see h
-0005f6c0: 7474 7073 3a2f 2f62 7962 6974 2d65 7863  ttps://bybit-exc
-0005f6d0: 6861 6e67 652e 6769 7468 7562 2e69 6f2f  hange.github.io/
-0005f6e0: 646f 6373 2f76 352f 6163 636f 756e 742f  docs/v5/account/
-0005f6f0: 6665 652d 7261 7465 0a20 2020 2020 2020  fee-rate.       
-0005f700: 203a 7061 7261 6d20 6469 6374 2070 6172   :param dict par
-0005f710: 616d 733a 2065 7874 7261 2070 6172 616d  ams: extra param
-0005f720: 6574 6572 7320 7370 6563 6966 6963 2074  eters specific t
-0005f730: 6f20 7468 6520 6279 6269 7420 6170 6920  o the bybit api 
-0005f740: 656e 6470 6f69 6e74 0a20 2020 2020 2020  endpoint.       
-0005f750: 203a 7265 7475 726e 7320 6469 6374 3a20   :returns dict: 
-0005f760: 6120 6469 6374 696f 6e61 7279 206f 6620  a dictionary of 
-0005f770: 6066 6565 2073 7472 7563 7475 7265 7320  `fee structures 
-0005f780: 3c68 7474 7073 3a2f 2f64 6f63 732e 6363  <https://docs.cc
-0005f790: 7874 2e63 6f6d 2f23 2f3f 6964 3d66 6565  xt.com/#/?id=fee
-0005f7a0: 2d73 7472 7563 7475 7265 3e60 2069 6e64  -structure>` ind
-0005f7b0: 6578 6564 2062 7920 6d61 726b 6574 2073  exed by market s
-0005f7c0: 796d 626f 6c73 0a20 2020 2020 2020 2022  ymbols.        "
-0005f7d0: 2222 0a20 2020 2020 2020 2061 7761 6974  "".        await
-0005f7e0: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
-0005f7f0: 7473 2829 0a20 2020 2020 2020 2074 7970  ts().        typ
-0005f800: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
-0005f810: 2074 7970 652c 2070 6172 616d 7320 3d20   type, params = 
-0005f820: 7365 6c66 2e68 616e 646c 655f 6f70 7469  self.handle_opti
-0005f830: 6f6e 5f61 6e64 5f70 6172 616d 7328 7061  on_and_params(pa
-0005f840: 7261 6d73 2c20 2766 6574 6368 5472 6164  rams, 'fetchTrad
-0005f850: 696e 6746 6565 7327 2c20 2774 7970 6527  ingFees', 'type'
-0005f860: 2c20 2766 7574 7572 6527 290a 2020 2020  , 'future').    
-0005f870: 2020 2020 6966 2074 7970 6520 3d3d 2027      if type == '
-0005f880: 7370 6f74 273a 0a20 2020 2020 2020 2020  spot':.         
-0005f890: 2020 2072 6169 7365 204e 6f74 5375 7070     raise NotSupp
-0005f8a0: 6f72 7465 6428 7365 6c66 2e69 6420 2b20  orted(self.id + 
-0005f8b0: 2720 6665 7463 6854 7261 6469 6e67 4665  ' fetchTradingFe
-0005f8c0: 6573 2829 2069 7320 6e6f 7420 7375 7070  es() is not supp
-0005f8d0: 6f72 7465 6420 666f 7220 7370 6f74 206d  orted for spot m
-0005f8e0: 6172 6b65 7427 290a 2020 2020 2020 2020  arket').        
-0005f8f0: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
-0005f900: 2073 656c 662e 7072 6976 6174 6547 6574   self.privateGet
-0005f910: 5635 4163 636f 756e 7446 6565 5261 7465  V5AccountFeeRate
-0005f920: 2870 6172 616d 7329 0a20 2020 2020 2020  (params).       
-0005f930: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-0005f940: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0005f950: 2020 2020 2022 7265 7443 6f64 6522 3a20       "retCode": 
-0005f960: 302c 0a20 2020 2020 2020 2023 2020 2020  0,.        #    
-0005f970: 2020 2020 2022 7265 744d 7367 223a 2022       "retMsg": "
-0005f980: 4f4b 222c 0a20 2020 2020 2020 2023 2020  OK",.        #  
-0005f990: 2020 2020 2020 2022 7265 7375 6c74 223a         "result":
-0005f9a0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0005f9b0: 2020 2020 2020 2020 2022 6c69 7374 223a           "list":
-0005f9c0: 205b 0a20 2020 2020 2020 2023 2020 2020   [.        #    
-0005f9d0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-0005f9e0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005f9f0: 2020 2020 2020 2020 2020 2020 2022 7379               "sy
-0005fa00: 6d62 6f6c 223a 2022 4554 4855 5344 5422  mbol": "ETHUSDT"
-0005fa10: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0005fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005fa30: 2274 616b 6572 4665 6552 6174 6522 3a20  "takerFeeRate": 
-0005fa40: 2230 2e30 3030 3622 2c0a 2020 2020 2020  "0.0006",.      
-0005fa50: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005fa60: 2020 2020 2020 2020 226d 616b 6572 4665          "makerFe
-0005fa70: 6552 6174 6522 3a20 2230 2e30 3030 3122  eRate": "0.0001"
-0005fa80: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005fa90: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0005faa0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0005fab0: 2020 205d 0a20 2020 2020 2020 2023 2020     ].        #  
-0005fac0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-0005fad0: 2020 2320 2020 2020 2020 2020 2272 6574    #         "ret
-0005fae0: 4578 7449 6e66 6f22 3a20 7b7d 2c0a 2020  ExtInfo": {},.  
-0005faf0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005fb00: 2274 696d 6522 3a20 3136 3736 3336 3034  "time": 16763604
-0005fb10: 3132 3537 360a 2020 2020 2020 2020 2320  12576.        # 
-0005fb20: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
-0005fb30: 2020 2020 2020 2020 6665 6573 203d 2073          fees = s
-0005fb40: 656c 662e 7361 6665 5f76 616c 7565 2872  elf.safe_value(r
-0005fb50: 6573 706f 6e73 652c 2027 7265 7375 6c74  esponse, 'result
-0005fb60: 272c 207b 7d29 0a20 2020 2020 2020 2066  ', {}).        f
-0005fb70: 6565 7320 3d20 7365 6c66 2e73 6166 655f  ees = self.safe_
-0005fb80: 7661 6c75 6528 6665 6573 2c20 276c 6973  value(fees, 'lis
-0005fb90: 7427 2c20 5b5d 290a 2020 2020 2020 2020  t', []).        
-0005fba0: 7265 7375 6c74 203d 207b 7d0a 2020 2020  result = {}.    
-0005fbb0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0005fbc0: 6765 2830 2c20 6c65 6e28 6665 6573 2929  ge(0, len(fees))
-0005fbd0: 3a0a 2020 2020 2020 2020 2020 2020 6665  :.            fe
-0005fbe0: 6520 3d20 7365 6c66 2e70 6172 7365 5f74  e = self.parse_t
-0005fbf0: 7261 6469 6e67 5f66 6565 2866 6565 735b  rading_fee(fees[
-0005fc00: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-0005fc10: 7379 6d62 6f6c 203d 2066 6565 5b27 7379  symbol = fee['sy
-0005fc20: 6d62 6f6c 275d 0a20 2020 2020 2020 2020  mbol'].         
-0005fc30: 2020 2072 6573 756c 745b 7379 6d62 6f6c     result[symbol
-0005fc40: 5d20 3d20 6665 650a 2020 2020 2020 2020  ] = fee.        
-0005fc50: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0005fc60: 2020 2064 6566 2073 6967 6e28 7365 6c66     def sign(self
-0005fc70: 2c20 7061 7468 2c20 6170 693d 2770 7562  , path, api='pub
-0005fc80: 6c69 6327 2c20 6d65 7468 6f64 3d27 4745  lic', method='GE
-0005fc90: 5427 2c20 7061 7261 6d73 3d7b 7d2c 2068  T', params={}, h
-0005fca0: 6561 6465 7273 3d4e 6f6e 652c 2062 6f64  eaders=None, bod
-0005fcb0: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0005fcc0: 2075 726c 203d 2073 656c 662e 696d 706c   url = self.impl
-0005fcd0: 6f64 655f 686f 7374 6e61 6d65 2873 656c  ode_hostname(sel
-0005fce0: 662e 7572 6c73 5b27 6170 6927 5d5b 6170  f.urls['api'][ap
-0005fcf0: 695d 2920 2b20 272f 2720 2b20 7061 7468  i]) + '/' + path
-0005fd00: 0a20 2020 2020 2020 2069 6620 6170 6920  .        if api 
-0005fd10: 3d3d 2027 7075 626c 6963 273a 0a20 2020  == 'public':.   
-0005fd20: 2020 2020 2020 2020 2069 6620 7061 7261           if para
-0005fd30: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-0005fd40: 2020 2020 7572 6c20 2b3d 2027 3f27 202b      url += '?' +
-0005fd50: 2073 656c 662e 7261 7765 6e63 6f64 6528   self.rawencode(
-0005fd60: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
-0005fd70: 656c 6966 2061 7069 203d 3d20 2770 7269  elif api == 'pri
-0005fd80: 7661 7465 273a 0a20 2020 2020 2020 2020  vate':.         
-0005fd90: 2020 2073 656c 662e 6368 6563 6b5f 7265     self.check_re
-0005fda0: 7175 6972 6564 5f63 7265 6465 6e74 6961  quired_credentia
-0005fdb0: 6c73 2829 0a20 2020 2020 2020 2020 2020  ls().           
-0005fdc0: 2069 734f 7065 6e61 7069 203d 2075 726c   isOpenapi = url
-0005fdd0: 2e66 696e 6428 276f 7065 6e61 7069 2729  .find('openapi')
-0005fde0: 203e 3d20 300a 2020 2020 2020 2020 2020   >= 0.          
-0005fdf0: 2020 6973 5633 556e 6966 6965 644d 6172    isV3UnifiedMar
-0005fe00: 6769 6e20 3d20 7572 6c2e 6669 6e64 2827  gin = url.find('
-0005fe10: 756e 6966 6965 642f 7633 2729 203e 3d20  unified/v3') >= 
-0005fe20: 300a 2020 2020 2020 2020 2020 2020 6973  0.            is
-0005fe30: 5633 436f 6e74 7261 6374 203d 2075 726c  V3Contract = url
-0005fe40: 2e66 696e 6428 2763 6f6e 7472 6163 742f  .find('contract/
-0005fe50: 7633 2729 203e 3d20 300a 2020 2020 2020  v3') >= 0.      
-0005fe60: 2020 2020 2020 6973 5635 556e 6966 6965        isV5Unifie
-0005fe70: 6441 6363 6f75 6e74 203d 2075 726c 2e66  dAccount = url.f
-0005fe80: 696e 6428 2776 3527 2920 3e3d 2030 0a20  ind('v5') >= 0. 
-0005fe90: 2020 2020 2020 2020 2020 2074 696d 6573             times
-0005fea0: 7461 6d70 203d 2073 7472 2873 656c 662e  tamp = str(self.
-0005feb0: 6e6f 6e63 6528 2929 0a20 2020 2020 2020  nonce()).       
-0005fec0: 2020 2020 2069 6620 6973 4f70 656e 6170       if isOpenap
-0005fed0: 693a 0a20 2020 2020 2020 2020 2020 2020  i:.             
-0005fee0: 2020 2069 6620 7061 7261 6d73 3a0a 2020     if params:.  
-0005fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005ff00: 2020 626f 6479 203d 2073 656c 662e 6a73    body = self.js
-0005ff10: 6f6e 2870 6172 616d 7329 0a20 2020 2020  on(params).     
-0005ff20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0005ff30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0005ff40: 2020 2020 2023 2073 656c 6620 6669 7820       # self fix 
-0005ff50: 666f 7220 5048 5020 6973 2072 6571 7569  for PHP is requi
-0005ff60: 7265 6420 6f74 6865 7277 6973 6520 6974  red otherwise it
-0005ff70: 2067 656e 6572 6174 6573 0a20 2020 2020   generates.     
-0005ff80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0005ff90: 2027 5b5d 2720 6f6e 2065 6d70 7479 2061   '[]' on empty a
-0005ffa0: 7272 6179 7320 6576 656e 2077 6865 6e20  rrays even when 
-0005ffb0: 666f 7263 6564 2074 6f20 7573 6520 6f62  forced to use ob
-0005ffc0: 6a65 6374 730a 2020 2020 2020 2020 2020  jects.          
-0005ffd0: 2020 2020 2020 2020 2020 626f 6479 203d            body =
-0005ffe0: 2027 7b7d 270a 2020 2020 2020 2020 2020   '{}'.          
-0005fff0: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-00060000: 7469 6d65 7374 616d 7020 2b20 7365 6c66  timestamp + self
-00060010: 2e61 7069 4b65 7920 2b20 626f 6479 0a20  .apiKey + body. 
-00060020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00060030: 6967 6e61 7475 7265 203d 2073 656c 662e  ignature = self.
-00060040: 686d 6163 2873 656c 662e 656e 636f 6465  hmac(self.encode
-00060050: 2870 6179 6c6f 6164 292c 2073 656c 662e  (payload), self.
-00060060: 656e 636f 6465 2873 656c 662e 7365 6372  encode(self.secr
-00060070: 6574 292c 2068 6173 686c 6962 2e73 6861  et), hashlib.sha
-00060080: 3235 362c 2027 6865 7827 290a 2020 2020  256, 'hex').    
-00060090: 2020 2020 2020 2020 2020 2020 6865 6164              head
-000600a0: 6572 7320 3d20 7b0a 2020 2020 2020 2020  ers = {.        
-000600b0: 2020 2020 2020 2020 2020 2020 2743 6f6e              'Con
-000600c0: 7465 6e74 2d54 7970 6527 3a20 2761 7070  tent-Type': 'app
-000600d0: 6c69 6361 7469 6f6e 2f6a 736f 6e27 2c0a  lication/json',.
-000600e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000600f0: 2020 2020 2758 2d42 4150 492d 4150 492d      'X-BAPI-API-
-00060100: 4b45 5927 3a20 7365 6c66 2e61 7069 4b65  KEY': self.apiKe
-00060110: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-00060120: 2020 2020 2020 2027 582d 4241 5049 2d54         'X-BAPI-T
-00060130: 494d 4553 5441 4d50 273a 2074 696d 6573  IMESTAMP': times
-00060140: 7461 6d70 2c0a 2020 2020 2020 2020 2020  tamp,.          
-00060150: 2020 2020 2020 2020 2020 2758 2d42 4150            'X-BAP
-00060160: 492d 5349 474e 273a 2073 6967 6e61 7475  I-SIGN': signatu
-00060170: 7265 2c0a 2020 2020 2020 2020 2020 2020  re,.            
-00060180: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00060190: 2020 656c 6966 2069 7356 3355 6e69 6669    elif isV3Unifi
-000601a0: 6564 4d61 7267 696e 206f 7220 6973 5633  edMargin or isV3
-000601b0: 436f 6e74 7261 6374 206f 7220 6973 5635  Contract or isV5
-000601c0: 556e 6966 6965 6441 6363 6f75 6e74 3a0a  UnifiedAccount:.
-000601d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000601e0: 6865 6164 6572 7320 3d20 7b0a 2020 2020  headers = {.    
-000601f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060200: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
-00060210: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
-00060220: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00060230: 2020 2020 2020 2020 2758 2d42 4150 492d          'X-BAPI-
-00060240: 4150 492d 4b45 5927 3a20 7365 6c66 2e61  API-KEY': self.a
-00060250: 7069 4b65 792c 0a20 2020 2020 2020 2020  piKey,.         
-00060260: 2020 2020 2020 2020 2020 2027 582d 4241             'X-BA
-00060270: 5049 2d54 494d 4553 5441 4d50 273a 2074  PI-TIMESTAMP': t
-00060280: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
-00060290: 2020 2020 2020 2020 2020 2020 2020 2758                'X
-000602a0: 2d42 4150 492d 5245 4356 2d57 494e 444f  -BAPI-RECV-WINDO
-000602b0: 5727 3a20 7374 7228 7365 6c66 2e6f 7074  W': str(self.opt
-000602c0: 696f 6e73 5b27 7265 6376 5769 6e64 6f77  ions['recvWindow
-000602d0: 275d 292c 0a20 2020 2020 2020 2020 2020  ']),.           
-000602e0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-000602f0: 2020 2020 2020 2069 6620 6973 5633 556e         if isV3Un
-00060300: 6966 6965 644d 6172 6769 6e20 6f72 2069  ifiedMargin or i
-00060310: 7356 3343 6f6e 7472 6163 743a 0a20 2020  sV3Contract:.   
-00060320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060330: 2068 6561 6465 7273 5b27 582d 4241 5049   headers['X-BAPI
-00060340: 2d53 4947 4e2d 5459 5045 275d 203d 2027  -SIGN-TYPE'] = '
-00060350: 3227 0a20 2020 2020 2020 2020 2020 2020  2'.             
-00060360: 2020 2071 7565 7279 203d 2073 656c 662e     query = self.
-00060370: 6578 7465 6e64 287b 7d2c 2070 6172 616d  extend({}, param
-00060380: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00060390: 2020 2071 7565 7279 456e 636f 6465 6420     queryEncoded 
-000603a0: 3d20 7365 6c66 2e72 6177 656e 636f 6465  = self.rawencode
-000603b0: 2871 7565 7279 290a 2020 2020 2020 2020  (query).        
-000603c0: 2020 2020 2020 2020 6175 7468 5f62 6173          auth_bas
-000603d0: 6520 3d20 7374 7228 7469 6d65 7374 616d  e = str(timestam
-000603e0: 7029 202b 2073 656c 662e 6170 694b 6579  p) + self.apiKey
-000603f0: 202b 2073 7472 2873 656c 662e 6f70 7469   + str(self.opti
-00060400: 6f6e 735b 2772 6563 7657 696e 646f 7727  ons['recvWindow'
-00060410: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00060420: 2020 2061 7574 6846 756c 6c20 3d20 4e6f     authFull = No
-00060430: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-00060440: 2020 2069 6620 6d65 7468 6f64 203d 3d20     if method == 
-00060450: 2750 4f53 5427 3a0a 2020 2020 2020 2020  'POST':.        
-00060460: 2020 2020 2020 2020 2020 2020 626f 6479              body
-00060470: 203d 2073 656c 662e 6a73 6f6e 2871 7565   = self.json(que
-00060480: 7279 290a 2020 2020 2020 2020 2020 2020  ry).            
-00060490: 2020 2020 2020 2020 6175 7468 4675 6c6c          authFull
-000604a0: 203d 2061 7574 685f 6261 7365 202b 2062   = auth_base + b
-000604b0: 6f64 790a 2020 2020 2020 2020 2020 2020  ody.            
-000604c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000604d0: 2020 2020 2020 2020 2020 2020 2020 6175                au
-000604e0: 7468 4675 6c6c 203d 2061 7574 685f 6261  thFull = auth_ba
-000604f0: 7365 202b 2071 7565 7279 456e 636f 6465  se + queryEncode
-00060500: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00060510: 2020 2020 2020 7572 6c20 2b3d 2027 3f27        url += '?'
-00060520: 202b 2073 656c 662e 7261 7765 6e63 6f64   + self.rawencod
-00060530: 6528 7175 6572 7929 0a20 2020 2020 2020  e(query).       
-00060540: 2020 2020 2020 2020 2073 6967 6e61 7475           signatu
-00060550: 7265 203d 204e 6f6e 650a 2020 2020 2020  re = None.      
-00060560: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00060570: 662e 7365 6372 6574 2e66 696e 6428 2750  f.secret.find('P
-00060580: 5249 5641 5445 204b 4559 2729 203e 202d  RIVATE KEY') > -
-00060590: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-000605a0: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-000605b0: 203d 2073 656c 662e 7273 6128 6175 7468   = self.rsa(auth
-000605c0: 4675 6c6c 2c20 7365 6c66 2e73 6563 7265  Full, self.secre
-000605d0: 742c 2027 7368 6132 3536 2729 0a20 2020  t, 'sha256').   
-000605e0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000605f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00060600: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-00060610: 203d 2073 656c 662e 686d 6163 2873 656c   = self.hmac(sel
-00060620: 662e 656e 636f 6465 2861 7574 6846 756c  f.encode(authFul
-00060630: 6c29 2c20 7365 6c66 2e65 6e63 6f64 6528  l), self.encode(
-00060640: 7365 6c66 2e73 6563 7265 7429 2c20 6861  self.secret), ha
-00060650: 7368 6c69 622e 7368 6132 3536 290a 2020  shlib.sha256).  
-00060660: 2020 2020 2020 2020 2020 2020 2020 6865                he
-00060670: 6164 6572 735b 2758 2d42 4150 492d 5349  aders['X-BAPI-SI
-00060680: 474e 275d 203d 2073 6967 6e61 7475 7265  GN'] = signature
-00060690: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000606a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000606b0: 2020 2071 7565 7279 203d 2073 656c 662e     query = self.
-000606c0: 6578 7465 6e64 2870 6172 616d 732c 207b  extend(params, {
+00059930: 2020 2020 2020 226c 6973 7422 3a20 5b0a        "list": [.
+00059940: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00059950: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00059960: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+00059970: 2020 2020 2020 2020 2020 226f 7065 6e49            "openI
+00059980: 6e74 6572 6573 7422 3a20 2234 3631 3133  nterest": "46113
+00059990: 3433 3834 2e30 3030 3030 3030 3022 2c0a  4384.00000000",.
+000599a0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+000599b0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000599c0: 696d 6573 7461 6d70 223a 2022 3136 3639  imestamp": "1669
+000599d0: 3537 3134 3030 3030 3022 0a20 2020 2020  571400000".     
+000599e0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+000599f0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00059a00: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00059a10: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
+00059a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00059a30: 2020 226f 7065 6e49 6e74 6572 6573 7422    "openInterest"
+00059a40: 3a20 2234 3631 3133 3432 3932 2e30 3030  : "461134292.000
+00059a50: 3030 3030 3022 2c0a 2020 2020 2020 2020  00000",.        
+00059a60: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00059a70: 2020 2020 2020 2274 696d 6573 7461 6d70        "timestamp
+00059a80: 223a 2022 3136 3639 3537 3131 3030 3030  ": "166957110000
+00059a90: 3022 0a20 2020 2020 2020 2023 2020 2020  0".        #    
+00059aa0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00059ab0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00059ac0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00059ad0: 2320 2020 2020 2020 2020 2020 2020 226e  #             "n
+00059ae0: 6578 7450 6167 6543 7572 736f 7222 3a20  extPageCursor": 
+00059af0: 2222 0a20 2020 2020 2020 2023 2020 2020  "".        #    
+00059b00: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00059b10: 2320 2020 2020 2020 2020 2272 6574 4578  #         "retEx
+00059b20: 7449 6e66 6f22 3a20 7b7d 2c0a 2020 2020  tInfo": {},.    
+00059b30: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
+00059b40: 696d 6522 3a20 3136 3732 3035 3335 3438  ime": 1672053548
+00059b50: 3537 390a 2020 2020 2020 2020 2320 2020  579.        #   
+00059b60: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
+00059b70: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00059b80: 656c 662e 7361 6665 5f76 616c 7565 2872  elf.safe_value(r
+00059b90: 6573 706f 6e73 652c 2027 7265 7375 6c74  esponse, 'result
+00059ba0: 272c 207b 7d29 0a20 2020 2020 2020 2069  ', {}).        i
+00059bb0: 6420 3d20 7365 6c66 2e73 6166 655f 7374  d = self.safe_st
+00059bc0: 7269 6e67 2872 6573 756c 742c 2027 7379  ring(result, 'sy
+00059bd0: 6d62 6f6c 2729 0a20 2020 2020 2020 206d  mbol').        m
+00059be0: 6172 6b65 7420 3d20 7365 6c66 2e73 6166  arket = self.saf
+00059bf0: 655f 6d61 726b 6574 2869 642c 206d 6172  e_market(id, mar
+00059c00: 6b65 742c 204e 6f6e 652c 2027 636f 6e74  ket, None, 'cont
+00059c10: 7261 6374 2729 0a20 2020 2020 2020 2064  ract').        d
+00059c20: 6174 6120 3d20 7365 6c66 2e73 6166 655f  ata = self.safe_
+00059c30: 7661 6c75 6528 7265 7375 6c74 2c20 276c  value(result, 'l
+00059c40: 6973 7427 2c20 5b5d 290a 2020 2020 2020  ist', []).      
+00059c50: 2020 7265 7475 726e 2073 656c 662e 7061    return self.pa
+00059c60: 7273 655f 6f70 656e 5f69 6e74 6572 6573  rse_open_interes
+00059c70: 7428 6461 7461 5b30 5d2c 206d 6172 6b65  t(data[0], marke
+00059c80: 7429 0a0a 2020 2020 6173 796e 6320 6465  t)..    async de
+00059c90: 6620 6665 7463 685f 6f70 656e 5f69 6e74  f fetch_open_int
+00059ca0: 6572 6573 745f 6869 7374 6f72 7928 7365  erest_history(se
+00059cb0: 6c66 2c20 7379 6d62 6f6c 3a20 7374 722c  lf, symbol: str,
+00059cc0: 2074 696d 6566 7261 6d65 3d27 3168 272c   timeframe='1h',
+00059cd0: 2073 696e 6365 3a20 4f70 7469 6f6e 616c   since: Optional
+00059ce0: 5b69 6e74 5d20 3d20 4e6f 6e65 2c20 6c69  [int] = None, li
+00059cf0: 6d69 743a 204f 7074 696f 6e61 6c5b 696e  mit: Optional[in
+00059d00: 745d 203d 204e 6f6e 652c 2070 6172 616d  t] = None, param
+00059d10: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
+00059d20: 2222 0a20 2020 2020 2020 2047 6574 7320  "".        Gets 
+00059d30: 7468 6520 746f 7461 6c20 616d 6f75 6e74  the total amount
+00059d40: 206f 6620 756e 7365 7474 6c65 6420 636f   of unsettled co
+00059d50: 6e74 7261 6374 732e 2049 6e20 6f74 6865  ntracts. In othe
+00059d60: 7220 776f 7264 732c 2074 6865 2074 6f74  r words, the tot
+00059d70: 616c 206e 756d 6265 7220 6f66 2063 6f6e  al number of con
+00059d80: 7472 6163 7473 2068 656c 6420 696e 206f  tracts held in o
+00059d90: 7065 6e20 706f 7369 7469 6f6e 730a 2020  pen positions.  
+00059da0: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
+00059db0: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
+00059dc0: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
+00059dd0: 7635 2f6d 6172 6b65 742f 6f70 656e 2d69  v5/market/open-i
+00059de0: 6e74 6572 6573 740a 2020 2020 2020 2020  nterest.        
+00059df0: 3a70 6172 616d 2073 7472 2073 796d 626f  :param str symbo
+00059e00: 6c3a 2055 6e69 6669 6564 206d 6172 6b65  l: Unified marke
+00059e10: 7420 7379 6d62 6f6c 0a20 2020 2020 2020  t symbol.       
+00059e20: 203a 7061 7261 6d20 7374 7220 7469 6d65   :param str time
+00059e30: 6672 616d 653a 2022 356d 222c 2031 356d  frame: "5m", 15m
+00059e40: 2c20 3330 6d2c 2031 682c 2034 682c 2031  , 30m, 1h, 4h, 1
+00059e50: 640a 2020 2020 2020 2020 3a70 6172 616d  d.        :param
+00059e60: 2069 6e74 2073 696e 6365 3a20 4e6f 7420   int since: Not 
+00059e70: 7573 6564 2062 7920 4279 6269 740a 2020  used by Bybit.  
+00059e80: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
+00059e90: 206c 696d 6974 3a20 5468 6520 6e75 6d62   limit: The numb
+00059ea0: 6572 206f 6620 6f70 656e 2069 6e74 6572  er of open inter
+00059eb0: 6573 7420 7374 7275 6374 7572 6573 2074  est structures t
+00059ec0: 6f20 7265 7475 726e 2e20 4d61 7820 3230  o return. Max 20
+00059ed0: 302c 2064 6566 6175 6c74 2035 300a 2020  0, default 50.  
+00059ee0: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+00059ef0: 7420 7061 7261 6d73 3a20 4578 6368 616e  t params: Exchan
+00059f00: 6765 2073 7065 6369 6669 6320 7061 7261  ge specific para
+00059f10: 6d65 7465 7273 0a20 2020 2020 2020 203a  meters.        :
+00059f20: 7265 7475 726e 733a 2041 6e20 6172 7261  returns: An arra
+00059f30: 7920 6f66 206f 7065 6e20 696e 7465 7265  y of open intere
+00059f40: 7374 2073 7472 7563 7475 7265 730a 2020  st structures.  
+00059f50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00059f60: 2020 6966 2074 696d 6566 7261 6d65 203d    if timeframe =
+00059f70: 3d20 2731 6d27 3a0a 2020 2020 2020 2020  = '1m':.        
+00059f80: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
+00059f90: 7565 7374 2873 656c 662e 6964 202b 2027  uest(self.id + '
+00059fa0: 6665 7463 684f 7065 6e49 6e74 6572 6573  fetchOpenInteres
+00059fb0: 7448 6973 746f 7279 2063 616e 6e6f 7420  tHistory cannot 
+00059fc0: 7573 6520 7468 6520 316d 2074 696d 6566  use the 1m timef
+00059fd0: 7261 6d65 2729 0a20 2020 2020 2020 2061  rame').        a
+00059fe0: 7761 6974 2073 656c 662e 6c6f 6164 5f6d  wait self.load_m
+00059ff0: 6172 6b65 7473 2829 0a20 2020 2020 2020  arkets().       
+0005a000: 206d 6172 6b65 7420 3d20 7365 6c66 2e6d   market = self.m
+0005a010: 6172 6b65 7428 7379 6d62 6f6c 290a 2020  arket(symbol).  
+0005a020: 2020 2020 2020 6966 206d 6172 6b65 745b        if market[
+0005a030: 2773 706f 7427 5d20 6f72 206d 6172 6b65  'spot'] or marke
+0005a040: 745b 276f 7074 696f 6e27 5d3a 0a20 2020  t['option']:.   
+0005a050: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+0005a060: 6164 5265 7175 6573 7428 7365 6c66 2e69  adRequest(self.i
+0005a070: 6420 2b20 2720 6665 7463 684f 7065 6e49  d + ' fetchOpenI
+0005a080: 6e74 6572 6573 7448 6973 746f 7279 2829  nterestHistory()
+0005a090: 2073 796d 626f 6c20 646f 6573 206e 6f74   symbol does not
+0005a0a0: 2073 7570 706f 7274 206d 6172 6b65 7420   support market 
+0005a0b0: 2720 2b20 7379 6d62 6f6c 290a 2020 2020  ' + symbol).    
+0005a0c0: 2020 2020 7265 7175 6573 7420 3d20 7b0a      request = {.
+0005a0d0: 2020 2020 2020 2020 2020 2020 2773 796d              'sym
+0005a0e0: 626f 6c27 3a20 6d61 726b 6574 5b27 6964  bol': market['id
+0005a0f0: 275d 2c0a 2020 2020 2020 2020 7d0a 2020  '],.        }.  
+0005a100: 2020 2020 2020 6966 206c 696d 6974 2069        if limit i
+0005a110: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0005a120: 2020 2020 2020 2020 7265 7175 6573 745b          request[
+0005a130: 276c 696d 6974 275d 203d 206c 696d 6974  'limit'] = limit
+0005a140: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0005a150: 6177 6169 7420 7365 6c66 2e66 6574 6368  await self.fetch
+0005a160: 5f64 6572 6976 6174 6976 6573 5f6f 7065  _derivatives_ope
+0005a170: 6e5f 696e 7465 7265 7374 5f68 6973 746f  n_interest_histo
+0005a180: 7279 2873 796d 626f 6c2c 2074 696d 6566  ry(symbol, timef
+0005a190: 7261 6d65 2c20 7369 6e63 652c 206c 696d  rame, since, lim
+0005a1a0: 6974 2c20 7061 7261 6d73 290a 0a20 2020  it, params)..   
+0005a1b0: 2064 6566 2070 6172 7365 5f6f 7065 6e5f   def parse_open_
+0005a1c0: 696e 7465 7265 7374 2873 656c 662c 2069  interest(self, i
+0005a1d0: 6e74 6572 6573 742c 206d 6172 6b65 743d  nterest, market=
+0005a1e0: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+0005a1f0: 0a20 2020 2020 2020 2023 2020 2020 7b0a  .        #    {.
+0005a200: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005a210: 2022 6f70 656e 496e 7465 7265 7374 223a   "openInterest":
+0005a220: 2036 3437 3537 2e36 3234 3030 3030 302c   64757.62400000,
+0005a230: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005a240: 2020 2274 696d 6573 7461 6d70 223a 2031    "timestamp": 1
+0005a250: 3636 3537 3834 3830 3030 3030 2c0a 2020  665784800000,.  
+0005a260: 2020 2020 2020 2320 2020 207d 0a20 2020        #    }.   
+0005a270: 2020 2020 2023 0a20 2020 2020 2020 2074       #.        t
+0005a280: 696d 6573 7461 6d70 203d 2073 656c 662e  imestamp = self.
+0005a290: 7361 6665 5f69 6e74 6567 6572 2869 6e74  safe_integer(int
+0005a2a0: 6572 6573 742c 2027 7469 6d65 7374 616d  erest, 'timestam
+0005a2b0: 7027 290a 2020 2020 2020 2020 7661 6c75  p').        valu
+0005a2c0: 6520 3d20 7365 6c66 2e73 6166 655f 6e75  e = self.safe_nu
+0005a2d0: 6d62 6572 5f32 2869 6e74 6572 6573 742c  mber_2(interest,
+0005a2e0: 2027 6f70 656e 5f69 6e74 6572 6573 7427   'open_interest'
+0005a2f0: 2c20 276f 7065 6e49 6e74 6572 6573 7427  , 'openInterest'
+0005a300: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0005a310: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0005a320: 7379 6d62 6f6c 273a 206d 6172 6b65 745b  symbol': market[
+0005a330: 2773 796d 626f 6c27 5d2c 0a20 2020 2020  'symbol'],.     
+0005a340: 2020 2020 2020 2027 6f70 656e 496e 7465         'openInte
+0005a350: 7265 7374 416d 6f75 6e74 273a 204e 6f6e  restAmount': Non
+0005a360: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+0005a370: 6f70 656e 496e 7465 7265 7374 5661 6c75  openInterestValu
+0005a380: 6527 3a20 7661 6c75 652c 0a20 2020 2020  e': value,.     
+0005a390: 2020 2020 2020 2027 7469 6d65 7374 616d         'timestam
+0005a3a0: 7027 3a20 7469 6d65 7374 616d 702c 0a20  p': timestamp,. 
+0005a3b0: 2020 2020 2020 2020 2020 2027 6461 7465             'date
+0005a3c0: 7469 6d65 273a 2073 656c 662e 6973 6f38  time': self.iso8
+0005a3d0: 3630 3128 7469 6d65 7374 616d 7029 2c0a  601(timestamp),.
+0005a3e0: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
+0005a3f0: 6f27 3a20 696e 7465 7265 7374 2c0a 2020  o': interest,.  
+0005a400: 2020 2020 2020 7d0a 0a20 2020 2061 7379        }..    asy
+0005a410: 6e63 2064 6566 2066 6574 6368 5f62 6f72  nc def fetch_bor
+0005a420: 726f 775f 7261 7465 2873 656c 662c 2063  row_rate(self, c
+0005a430: 6f64 653a 2073 7472 2c20 7061 7261 6d73  ode: str, params
+0005a440: 3d7b 7d29 3a0a 2020 2020 2020 2020 2222  ={}):.        ""
+0005a450: 220a 2020 2020 2020 2020 6665 7463 6820  ".        fetch 
+0005a460: 7468 6520 7261 7465 206f 6620 696e 7465  the rate of inte
+0005a470: 7265 7374 2074 6f20 626f 7272 6f77 2061  rest to borrow a
+0005a480: 2063 7572 7265 6e63 7920 666f 7220 6d61   currency for ma
+0005a490: 7267 696e 2074 7261 6469 6e67 0a20 2020  rgin trading.   
+0005a4a0: 2020 2020 2073 6565 2068 7474 7073 3a2f       see https:/
+0005a4b0: 2f62 7962 6974 2d65 7863 6861 6e67 652e  /bybit-exchange.
+0005a4c0: 6769 7468 7562 2e69 6f2f 646f 6373 2f73  github.io/docs/s
+0005a4d0: 706f 742f 7633 2f23 742d 7175 6572 7969  pot/v3/#t-queryi
+0005a4e0: 6e74 6572 6573 7471 756f 7461 0a20 2020  nterestquota.   
+0005a4f0: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+0005a500: 636f 6465 3a20 756e 6966 6965 6420 6375  code: unified cu
+0005a510: 7272 656e 6379 2063 6f64 650a 2020 2020  rrency code.    
+0005a520: 2020 2020 3a70 6172 616d 2064 6963 7420      :param dict 
+0005a530: 7061 7261 6d73 3a20 6578 7472 6120 7061  params: extra pa
+0005a540: 7261 6d65 7465 7273 2073 7065 6369 6669  rameters specifi
+0005a550: 6320 746f 2074 6865 2062 7962 6974 2061  c to the bybit a
+0005a560: 7069 2065 6e64 706f 696e 740a 2020 2020  pi endpoint.    
+0005a570: 2020 2020 3a72 6574 7572 6e73 2064 6963      :returns dic
+0005a580: 743a 2061 2060 626f 7272 6f77 2072 6174  t: a `borrow rat
+0005a590: 6520 7374 7275 6374 7572 6520 3c68 7474  e structure <htt
+0005a5a0: 7073 3a2f 2f64 6f63 732e 6363 7874 2e63  ps://docs.ccxt.c
+0005a5b0: 6f6d 2f23 2f3f 6964 3d62 6f72 726f 772d  om/#/?id=borrow-
+0005a5c0: 7261 7465 2d73 7472 7563 7475 7265 3e60  rate-structure>`
+0005a5d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0005a5e0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+0005a5f0: 6c6f 6164 5f6d 6172 6b65 7473 2829 0a20  load_markets(). 
+0005a600: 2020 2020 2020 2063 7572 7265 6e63 7920         currency 
+0005a610: 3d20 7365 6c66 2e63 7572 7265 6e63 7928  = self.currency(
+0005a620: 636f 6465 290a 2020 2020 2020 2020 7265  code).        re
+0005a630: 7175 6573 7420 3d20 7b0a 2020 2020 2020  quest = {.      
+0005a640: 2020 2020 2020 2763 6f69 6e27 3a20 6375        'coin': cu
+0005a650: 7272 656e 6379 5b27 6964 275d 2c0a 2020  rrency['id'],.  
+0005a660: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0005a670: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
+0005a680: 2073 656c 662e 7072 6976 6174 6547 6574   self.privateGet
+0005a690: 5370 6f74 5633 5072 6976 6174 6543 726f  SpotV3PrivateCro
+0005a6a0: 7373 4d61 7267 696e 4c6f 616e 496e 666f  ssMarginLoanInfo
+0005a6b0: 2873 656c 662e 6578 7465 6e64 2872 6571  (self.extend(req
+0005a6c0: 7565 7374 2c20 7061 7261 6d73 2929 0a20  uest, params)). 
+0005a6d0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0005a6e0: 2023 2020 2020 7b0a 2020 2020 2020 2020   #    {.        
+0005a6f0: 2320 2020 2020 2020 2020 2272 6574 436f  #         "retCo
+0005a700: 6465 223a 2022 3022 2c0a 2020 2020 2020  de": "0",.      
+0005a710: 2020 2320 2020 2020 2020 2020 2272 6574    #         "ret
+0005a720: 4d73 6722 3a20 2273 7563 6365 7373 222c  Msg": "success",
+0005a730: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005a740: 2020 2022 7265 7375 6c74 223a 207b 0a20     "result": {. 
+0005a750: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005a760: 2020 2020 2022 636f 696e 223a 2022 5553       "coin": "US
+0005a770: 4454 222c 0a20 2020 2020 2020 2023 2020  DT",.        #  
+0005a780: 2020 2020 2020 2020 2020 2022 696e 7465             "inte
+0005a790: 7265 7374 5261 7465 223a 2022 302e 3030  restRate": "0.00
+0005a7a0: 3031 3037 3030 3030 3030 222c 0a20 2020  0107000000",.   
+0005a7b0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0005a7c0: 2020 2022 6c6f 616e 4162 6c65 416d 6f75     "loanAbleAmou
+0005a7d0: 6e74 223a 2022 222c 0a20 2020 2020 2020  nt": "",.       
+0005a7e0: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
+0005a7f0: 6d61 784c 6f61 6e41 6d6f 756e 7422 3a20  maxLoanAmount": 
+0005a800: 2237 3939 3939 2e39 3939 220a 2020 2020  "79999.999".    
+0005a810: 2020 2020 2320 2020 2020 2020 2020 7d2c      #         },
+0005a820: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005a830: 2020 2022 7265 7445 7874 496e 666f 223a     "retExtInfo":
+0005a840: 206e 756c 6c2c 0a20 2020 2020 2020 2023   null,.        #
+0005a850: 2020 2020 2020 2020 2022 7469 6d65 223a           "time":
+0005a860: 2022 3136 3636 3733 3434 3930 3737 3822   "1666734490778"
+0005a870: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+0005a880: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005a890: 2020 2064 6174 6120 3d20 7365 6c66 2e73     data = self.s
+0005a8a0: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
+0005a8b0: 7365 2c20 2772 6573 756c 7427 2c20 7b7d  se, 'result', {}
+0005a8c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0005a8d0: 2073 656c 662e 7061 7273 655f 626f 7272   self.parse_borr
+0005a8e0: 6f77 5f72 6174 6528 6461 7461 2c20 6375  ow_rate(data, cu
+0005a8f0: 7272 656e 6379 290a 0a20 2020 2064 6566  rrency)..    def
+0005a900: 2070 6172 7365 5f62 6f72 726f 775f 7261   parse_borrow_ra
+0005a910: 7465 2873 656c 662c 2069 6e66 6f2c 2063  te(self, info, c
+0005a920: 7572 7265 6e63 793d 4e6f 6e65 293a 0a20  urrency=None):. 
+0005a930: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0005a940: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
+0005a950: 2023 2020 2020 2020 2020 2022 636f 696e   #         "coin
+0005a960: 223a 2022 5553 4454 222c 0a20 2020 2020  ": "USDT",.     
+0005a970: 2020 2023 2020 2020 2020 2020 2022 696e     #         "in
+0005a980: 7465 7265 7374 5261 7465 223a 2022 302e  terestRate": "0.
+0005a990: 3030 3031 3037 3030 3030 3030 222c 0a20  000107000000",. 
+0005a9a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005a9b0: 2022 6c6f 616e 4162 6c65 416d 6f75 6e74   "loanAbleAmount
+0005a9c0: 223a 2022 222c 0a20 2020 2020 2020 2023  ": "",.        #
+0005a9d0: 2020 2020 2020 2020 2022 6d61 784c 6f61           "maxLoa
+0005a9e0: 6e41 6d6f 756e 7422 3a20 2237 3939 3939  nAmount": "79999
+0005a9f0: 2e39 3939 220a 2020 2020 2020 2020 2320  .999".        # 
+0005aa00: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
+0005aa10: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+0005aa20: 7020 3d20 7365 6c66 2e6d 696c 6c69 7365  p = self.millise
+0005aa30: 636f 6e64 7328 290a 2020 2020 2020 2020  conds().        
+0005aa40: 6375 7272 656e 6379 4964 203d 2073 656c  currencyId = sel
+0005aa50: 662e 7361 6665 5f73 7472 696e 6728 696e  f.safe_string(in
+0005aa60: 666f 2c20 2763 6f69 6e27 290a 2020 2020  fo, 'coin').    
+0005aa70: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
+0005aa80: 2020 2020 2020 2020 2027 6375 7272 656e           'curren
+0005aa90: 6379 273a 2073 656c 662e 7361 6665 5f63  cy': self.safe_c
+0005aaa0: 7572 7265 6e63 795f 636f 6465 2863 7572  urrency_code(cur
+0005aab0: 7265 6e63 7949 642c 2063 7572 7265 6e63  rencyId, currenc
+0005aac0: 7929 2c0a 2020 2020 2020 2020 2020 2020  y),.            
+0005aad0: 2772 6174 6527 3a20 7365 6c66 2e73 6166  'rate': self.saf
+0005aae0: 655f 6e75 6d62 6572 2869 6e66 6f2c 2027  e_number(info, '
+0005aaf0: 696e 7465 7265 7374 5261 7465 2729 2c0a  interestRate'),.
+0005ab00: 2020 2020 2020 2020 2020 2020 2770 6572              'per
+0005ab10: 696f 6427 3a20 3836 3430 3030 3030 2c20  iod': 86400000, 
+0005ab20: 2023 2044 6169 6c79 0a20 2020 2020 2020   # Daily.       
+0005ab30: 2020 2020 2027 7469 6d65 7374 616d 7027       'timestamp'
+0005ab40: 3a20 7469 6d65 7374 616d 702c 0a20 2020  : timestamp,.   
+0005ab50: 2020 2020 2020 2020 2027 6461 7465 7469           'dateti
+0005ab60: 6d65 273a 2073 656c 662e 6973 6f38 3630  me': self.iso860
+0005ab70: 3128 7469 6d65 7374 616d 7029 2c0a 2020  1(timestamp),.  
+0005ab80: 2020 2020 2020 2020 2020 2769 6e66 6f27            'info'
+0005ab90: 3a20 696e 666f 2c0a 2020 2020 2020 2020  : info,.        
+0005aba0: 7d0a 0a20 2020 2061 7379 6e63 2064 6566  }..    async def
+0005abb0: 2066 6574 6368 5f62 6f72 726f 775f 696e   fetch_borrow_in
+0005abc0: 7465 7265 7374 2873 656c 662c 2063 6f64  terest(self, cod
+0005abd0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+0005abe0: 203d 204e 6f6e 652c 2073 796d 626f 6c3a   = None, symbol:
+0005abf0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0005ac00: 204e 6f6e 652c 2073 696e 6365 3a20 4f70   None, since: Op
+0005ac10: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0005ac20: 6e65 2c20 6c69 6d69 743a 204f 7074 696f  ne, limit: Optio
+0005ac30: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+0005ac40: 2070 6172 616d 733d 7b7d 293a 0a20 2020   params={}):.   
+0005ac50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0005ac60: 2066 6574 6368 2074 6865 2069 6e74 6572   fetch the inter
+0005ac70: 6573 7420 6f77 6564 2062 7920 7468 6520  est owed by the 
+0005ac80: 7573 6572 2066 6f72 2062 6f72 726f 7769  user for borrowi
+0005ac90: 6e67 2063 7572 7265 6e63 7920 666f 7220  ng currency for 
+0005aca0: 6d61 7267 696e 2074 7261 6469 6e67 0a20  margin trading. 
+0005acb0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
+0005acc0: 727c 4e6f 6e65 2063 6f64 653a 2075 6e69  r|None code: uni
+0005acd0: 6669 6564 2063 7572 7265 6e63 7920 636f  fied currency co
+0005ace0: 6465 0a20 2020 2020 2020 203a 7061 7261  de.        :para
+0005acf0: 6d20 7374 727c 4e6f 6e65 2073 796d 626f  m str|None symbo
+0005ad00: 6c3a 2075 6e69 6669 6564 206d 6172 6b65  l: unified marke
+0005ad10: 7420 7379 6d62 6f6c 2077 6865 6e20 6665  t symbol when fe
+0005ad20: 7463 6820 696e 7465 7265 7374 2069 6e20  tch interest in 
+0005ad30: 6973 6f6c 6174 6564 206d 6172 6b65 7473  isolated markets
+0005ad40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0005ad50: 6e75 6d62 6572 7c4e 6f6e 6520 7369 6e63  number|None sinc
+0005ad60: 653a 2074 6865 2065 6172 6c69 6573 7420  e: the earliest 
+0005ad70: 7469 6d65 2069 6e20 6d73 2074 6f20 6665  time in ms to fe
+0005ad80: 7463 6820 626f 7272 726f 7720 696e 7465  tch borrrow inte
+0005ad90: 7265 7374 2066 6f72 0a20 2020 2020 2020  rest for.       
+0005ada0: 203a 7061 7261 6d20 6e75 6d62 6572 7c4e   :param number|N
+0005adb0: 6f6e 6520 6c69 6d69 743a 2074 6865 206d  one limit: the m
+0005adc0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+0005add0: 2073 7472 7563 7475 7265 7320 746f 2072   structures to r
+0005ade0: 6574 7269 6576 650a 2020 2020 2020 2020  etrieve.        
+0005adf0: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
+0005ae00: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
+0005ae10: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
+0005ae20: 2074 6865 2062 7962 6974 2061 7069 2065   the bybit api e
+0005ae30: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
+0005ae40: 3a72 6574 7572 6e73 205b 6469 6374 5d3a  :returns [dict]:
+0005ae50: 2061 206c 6973 7420 6f66 2060 626f 7272   a list of `borr
+0005ae60: 6f77 2069 6e74 6572 6573 7420 7374 7275  ow interest stru
+0005ae70: 6374 7572 6573 203c 6874 7470 733a 2f2f  ctures <https://
+0005ae80: 646f 6373 2e63 6378 742e 636f 6d2f 232f  docs.ccxt.com/#/
+0005ae90: 3f69 643d 626f 7272 6f77 2d69 6e74 6572  ?id=borrow-inter
+0005aea0: 6573 742d 7374 7275 6374 7572 653e 600a  est-structure>`.
+0005aeb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0005aec0: 2020 2020 6177 6169 7420 7365 6c66 2e6c      await self.l
+0005aed0: 6f61 645f 6d61 726b 6574 7328 290a 2020  oad_markets().  
+0005aee0: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
+0005aef0: 7b7d 0a20 2020 2020 2020 2072 6573 706f  {}.        respo
+0005af00: 6e73 6520 3d20 6177 6169 7420 7365 6c66  nse = await self
+0005af10: 2e70 7269 7661 7465 4765 7453 706f 7456  .privateGetSpotV
+0005af20: 3350 7269 7661 7465 4372 6f73 734d 6172  3PrivateCrossMar
+0005af30: 6769 6e41 6363 6f75 6e74 2873 656c 662e  ginAccount(self.
+0005af40: 6578 7465 6e64 2872 6571 7565 7374 2c20  extend(request, 
+0005af50: 7061 7261 6d73 2929 0a20 2020 2020 2020  params)).       
+0005af60: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
+0005af70: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0005af80: 2020 2020 2022 7265 745f 636f 6465 223a       "ret_code":
+0005af90: 2030 2c0a 2020 2020 2020 2020 2320 2020   0,.        #   
+0005afa0: 2020 2020 2020 2272 6574 5f6d 7367 223a        "ret_msg":
+0005afb0: 2022 222c 0a20 2020 2020 2020 2023 2020   "",.        #  
+0005afc0: 2020 2020 2020 2022 6578 745f 636f 6465         "ext_code
+0005afd0: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
+0005afe0: 2023 2020 2020 2020 2020 2022 6578 745f   #         "ext_
+0005aff0: 696e 666f 223a 206e 756c 6c2c 0a20 2020  info": null,.   
+0005b000: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005b010: 7265 7375 6c74 223a 207b 0a20 2020 2020  result": {.     
+0005b020: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005b030: 2022 7374 6174 7573 223a 2022 3122 2c0a   "status": "1",.
+0005b040: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005b050: 2020 2020 2020 2272 6973 6b52 6174 6522        "riskRate"
+0005b060: 3a20 2230 222c 0a20 2020 2020 2020 2023  : "0",.        #
+0005b070: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
+0005b080: 6374 4261 6c61 6e63 6553 756d 223a 2022  ctBalanceSum": "
+0005b090: 302e 3030 3034 3836 3231 3338 3137 3638  0.00048621381768
+0005b0a0: 3038 3537 222c 0a20 2020 2020 2020 2023  0857",.        #
+0005b0b0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+0005b0c0: 6274 4261 6c61 6e63 6553 756d 223a 2022  btBalanceSum": "
+0005b0d0: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
+0005b0e0: 2020 2020 2020 2020 2020 226c 6f61 6e41            "loanA
+0005b0f0: 6363 6f75 6e74 4c69 7374 223a 205b 0a20  ccountList": [. 
+0005b100: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005b110: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0005b120: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005b130: 2020 2020 2020 2020 2022 746f 6b65 6e49           "tokenI
+0005b140: 6422 3a20 2242 5443 222c 0a20 2020 2020  d": "BTC",.     
+0005b150: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005b160: 2020 2020 2020 2020 2022 746f 7461 6c22           "total"
+0005b170: 3a20 2230 2e30 3030 3438 3632 3122 2c0a  : "0.00048621",.
+0005b180: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005b190: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+0005b1a0: 6f63 6b65 6422 3a20 2230 222c 0a20 2020  ocked": "0",.   
+0005b1b0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0005b1c0: 2020 2020 2020 2020 2020 2022 6c6f 616e             "loan
+0005b1d0: 223a 2022 3022 2c0a 2020 2020 2020 2020  ": "0",.        
+0005b1e0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0005b1f0: 2020 2020 2020 2269 6e74 6572 6573 7422        "interest"
+0005b200: 3a20 2230 222c 0a20 2020 2020 2020 2023  : "0",.        #
+0005b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005b220: 2020 2020 2022 6672 6565 223a 2022 302e       "free": "0.
+0005b230: 3030 3034 3836 3231 220a 2020 2020 2020  00048621".      
+0005b240: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0005b250: 2020 2020 7d2c 0a20 2020 2020 2020 2023      },.        #
+0005b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005b270: 202e 2e2e 0a20 2020 2020 2020 2023 2020   ....        #  
+0005b280: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0005b290: 2020 2020 2023 2020 2020 2020 2020 207d       #         }
+0005b2a0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+0005b2b0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005b2c0: 2020 2064 6174 6120 3d20 7365 6c66 2e73     data = self.s
+0005b2d0: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
+0005b2e0: 7365 2c20 2772 6573 756c 7427 2c20 7b7d  se, 'result', {}
+0005b2f0: 290a 2020 2020 2020 2020 726f 7773 203d  ).        rows =
+0005b300: 2073 656c 662e 7361 6665 5f76 616c 7565   self.safe_value
+0005b310: 2864 6174 612c 2027 6c6f 616e 4163 636f  (data, 'loanAcco
+0005b320: 756e 744c 6973 7427 2c20 5b5d 290a 2020  untList', []).  
+0005b330: 2020 2020 2020 696e 7465 7265 7374 203d        interest =
+0005b340: 2073 656c 662e 7061 7273 655f 626f 7272   self.parse_borr
+0005b350: 6f77 5f69 6e74 6572 6573 7473 2872 6f77  ow_interests(row
+0005b360: 732c 204e 6f6e 6529 0a20 2020 2020 2020  s, None).       
+0005b370: 2072 6574 7572 6e20 7365 6c66 2e66 696c   return self.fil
+0005b380: 7465 725f 6279 5f63 7572 7265 6e63 795f  ter_by_currency_
+0005b390: 7369 6e63 655f 6c69 6d69 7428 696e 7465  since_limit(inte
+0005b3a0: 7265 7374 2c20 636f 6465 2c20 7369 6e63  rest, code, sinc
+0005b3b0: 652c 206c 696d 6974 290a 0a20 2020 2064  e, limit)..    d
+0005b3c0: 6566 2070 6172 7365 5f62 6f72 726f 775f  ef parse_borrow_
+0005b3d0: 696e 7465 7265 7374 2873 656c 662c 2069  interest(self, i
+0005b3e0: 6e66 6f2c 206d 6172 6b65 743d 4e6f 6e65  nfo, market=None
+0005b3f0: 293a 0a20 2020 2020 2020 2023 0a20 2020  ):.        #.   
+0005b400: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
+0005b410: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005b420: 746f 6b65 6e49 6422 3a20 2242 5443 222c  tokenId": "BTC",
+0005b430: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005b440: 2020 2022 746f 7461 6c22 3a20 2230 2e30     "total": "0.0
+0005b450: 3030 3438 3632 3122 2c0a 2020 2020 2020  0048621",.      
+0005b460: 2020 2320 2020 2020 2020 2020 226c 6f63    #         "loc
+0005b470: 6b65 6422 3a20 2230 222c 0a20 2020 2020  ked": "0",.     
+0005b480: 2020 2023 2020 2020 2020 2020 2022 6c6f     #         "lo
+0005b490: 616e 223a 2022 3022 2c0a 2020 2020 2020  an": "0",.      
+0005b4a0: 2020 2320 2020 2020 2020 2020 2269 6e74    #         "int
+0005b4b0: 6572 6573 7422 3a20 2230 222c 0a20 2020  erest": "0",.   
+0005b4c0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005b4d0: 6672 6565 223a 2022 302e 3030 3034 3836  free": "0.000486
+0005b4e0: 3231 220a 2020 2020 2020 2020 2320 2020  21".        #   
+0005b4f0: 2020 7d2c 0a20 2020 2020 2020 2023 0a20    },.        #. 
+0005b500: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+0005b510: 2020 2020 2020 2020 2020 2020 2773 796d              'sym
+0005b520: 626f 6c27 3a20 4e6f 6e65 2c0a 2020 2020  bol': None,.    
+0005b530: 2020 2020 2020 2020 276d 6172 6769 6e4d          'marginM
+0005b540: 6f64 6527 3a20 2763 726f 7373 272c 0a20  ode': 'cross',. 
+0005b550: 2020 2020 2020 2020 2020 2027 6375 7272             'curr
+0005b560: 656e 6379 273a 2073 656c 662e 7361 6665  ency': self.safe
+0005b570: 5f63 7572 7265 6e63 795f 636f 6465 2873  _currency_code(s
+0005b580: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005b590: 696e 666f 2c20 2774 6f6b 656e 4964 2729  info, 'tokenId')
+0005b5a0: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
+0005b5b0: 696e 7465 7265 7374 273a 2073 656c 662e  interest': self.
+0005b5c0: 7361 6665 5f6e 756d 6265 7228 696e 666f  safe_number(info
+0005b5d0: 2c20 2769 6e74 6572 6573 7427 292c 0a20  , 'interest'),. 
+0005b5e0: 2020 2020 2020 2020 2020 2027 696e 7465             'inte
+0005b5f0: 7265 7374 5261 7465 273a 204e 6f6e 652c  restRate': None,
+0005b600: 0a20 2020 2020 2020 2020 2020 2027 616d  .            'am
+0005b610: 6f75 6e74 426f 7272 6f77 6564 273a 2073  ountBorrowed': s
+0005b620: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
+0005b630: 696e 666f 2c20 276c 6f61 6e27 292c 0a20  info, 'loan'),. 
+0005b640: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
+0005b650: 7374 616d 7027 3a20 4e6f 6e65 2c0a 2020  stamp': None,.  
+0005b660: 2020 2020 2020 2020 2020 2764 6174 6574            'datet
+0005b670: 696d 6527 3a20 4e6f 6e65 2c0a 2020 2020  ime': None,.    
+0005b680: 2020 2020 2020 2020 2769 6e66 6f27 3a20          'info': 
+0005b690: 696e 666f 2c0a 2020 2020 2020 2020 7d0a  info,.        }.
+0005b6a0: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+0005b6b0: 7261 6e73 6665 7228 7365 6c66 2c20 636f  ransfer(self, co
+0005b6c0: 6465 3a20 7374 722c 2061 6d6f 756e 742c  de: str, amount,
+0005b6d0: 2066 726f 6d41 6363 6f75 6e74 2c20 746f   fromAccount, to
+0005b6e0: 4163 636f 756e 742c 2070 6172 616d 733d  Account, params=
+0005b6f0: 7b7d 293a 0a20 2020 2020 2020 2022 2222  {}):.        """
+0005b700: 0a20 2020 2020 2020 2074 7261 6e73 6665  .        transfe
+0005b710: 7220 6375 7272 656e 6379 2069 6e74 6572  r currency inter
+0005b720: 6e61 6c6c 7920 6265 7477 6565 6e20 7761  nally between wa
+0005b730: 6c6c 6574 7320 6f6e 2074 6865 2073 616d  llets on the sam
+0005b740: 6520 6163 636f 756e 740a 2020 2020 2020  e account.      
+0005b750: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
+0005b760: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
+0005b770: 6875 622e 696f 2f64 6f63 732f 6163 636f  hub.io/docs/acco
+0005b780: 756e 745f 6173 7365 742f 2374 2d63 7265  unt_asset/#t-cre
+0005b790: 6174 6569 6e74 6572 6e61 6c74 7261 6e73  ateinternaltrans
+0005b7a0: 6665 720a 2020 2020 2020 2020 7365 6520  fer.        see 
+0005b7b0: 6874 7470 733a 2f2f 6279 6269 742d 6578  https://bybit-ex
+0005b7c0: 6368 616e 6765 2e67 6974 6875 622e 696f  change.github.io
+0005b7d0: 2f64 6f63 732f 6163 636f 756e 745f 6173  /docs/account_as
+0005b7e0: 7365 742f 7633 2f23 742d 6372 6561 7465  set/v3/#t-create
+0005b7f0: 696e 7465 726e 616c 7472 616e 7366 6572  internaltransfer
+0005b800: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0005b810: 7374 7220 636f 6465 3a20 756e 6966 6965  str code: unifie
+0005b820: 6420 6375 7272 656e 6379 2063 6f64 650a  d currency code.
+0005b830: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+0005b840: 6c6f 6174 2061 6d6f 756e 743a 2061 6d6f  loat amount: amo
+0005b850: 756e 7420 746f 2074 7261 6e73 6665 720a  unt to transfer.
+0005b860: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+0005b870: 7472 2066 726f 6d41 6363 6f75 6e74 3a20  tr fromAccount: 
+0005b880: 6163 636f 756e 7420 746f 2074 7261 6e73  account to trans
+0005b890: 6665 7220 6672 6f6d 0a20 2020 2020 2020  fer from.       
+0005b8a0: 203a 7061 7261 6d20 7374 7220 746f 4163   :param str toAc
+0005b8b0: 636f 756e 743a 2061 6363 6f75 6e74 2074  count: account t
+0005b8c0: 6f20 7472 616e 7366 6572 2074 6f0a 2020  o transfer to.  
+0005b8d0: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+0005b8e0: 7420 7061 7261 6d73 3a20 6578 7472 6120  t params: extra 
+0005b8f0: 7061 7261 6d65 7465 7273 2073 7065 6369  parameters speci
+0005b900: 6669 6320 746f 2074 6865 2062 7962 6974  fic to the bybit
+0005b910: 2061 7069 2065 6e64 706f 696e 740a 2020   api endpoint.  
+0005b920: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+0005b930: 2070 6172 616d 735b 2774 7261 6e73 6665   params['transfe
+0005b940: 7249 6427 5d3a 2055 5549 442c 2077 6869  rId']: UUID, whi
+0005b950: 6368 2069 7320 756e 6971 7565 2061 6372  ch is unique acr
+0005b960: 6f73 7320 7468 6520 706c 6174 666f 726d  oss the platform
+0005b970: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0005b980: 7320 6469 6374 3a20 6120 6074 7261 6e73  s dict: a `trans
+0005b990: 6665 7220 7374 7275 6374 7572 6520 3c68  fer structure <h
+0005b9a0: 7474 7073 3a2f 2f64 6f63 732e 6363 7874  ttps://docs.ccxt
+0005b9b0: 2e63 6f6d 2f23 2f3f 6964 3d74 7261 6e73  .com/#/?id=trans
+0005b9c0: 6665 722d 7374 7275 6374 7572 653e 600a  fer-structure>`.
+0005b9d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0005b9e0: 2020 2020 6177 6169 7420 7365 6c66 2e6c      await self.l
+0005b9f0: 6f61 645f 6d61 726b 6574 7328 290a 2020  oad_markets().  
+0005ba00: 2020 2020 2020 7472 616e 7366 6572 4964        transferId
+0005ba10: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
+0005ba20: 696e 6728 7061 7261 6d73 2c20 2774 7261  ing(params, 'tra
+0005ba30: 6e73 6665 7249 6427 2c20 7365 6c66 2e75  nsferId', self.u
+0005ba40: 7569 6428 2929 0a20 2020 2020 2020 2061  uid()).        a
+0005ba50: 6363 6f75 6e74 5479 7065 7320 3d20 7365  ccountTypes = se
+0005ba60: 6c66 2e73 6166 655f 7661 6c75 6528 7365  lf.safe_value(se
+0005ba70: 6c66 2e6f 7074 696f 6e73 2c20 2761 6363  lf.options, 'acc
+0005ba80: 6f75 6e74 7342 7954 7970 6527 2c20 7b7d  ountsByType', {}
+0005ba90: 290a 2020 2020 2020 2020 6672 6f6d 4964  ).        fromId
+0005baa0: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
+0005bab0: 696e 6728 6163 636f 756e 7454 7970 6573  ing(accountTypes
+0005bac0: 2c20 6672 6f6d 4163 636f 756e 742c 2066  , fromAccount, f
+0005bad0: 726f 6d41 6363 6f75 6e74 290a 2020 2020  romAccount).    
+0005bae0: 2020 2020 746f 4964 203d 2073 656c 662e      toId = self.
+0005baf0: 7361 6665 5f73 7472 696e 6728 6163 636f  safe_string(acco
+0005bb00: 756e 7454 7970 6573 2c20 746f 4163 636f  untTypes, toAcco
+0005bb10: 756e 742c 2074 6f41 6363 6f75 6e74 290a  unt, toAccount).
+0005bb20: 2020 2020 2020 2020 6375 7272 656e 6379          currency
+0005bb30: 203d 2073 656c 662e 6375 7272 656e 6379   = self.currency
+0005bb40: 2863 6f64 6529 0a20 2020 2020 2020 2061  (code).        a
+0005bb50: 6d6f 756e 7454 6f50 7265 6369 7369 6f6e  mountToPrecision
+0005bb60: 203d 2073 656c 662e 6375 7272 656e 6379   = self.currency
+0005bb70: 5f74 6f5f 7072 6563 6973 696f 6e28 636f  _to_precision(co
+0005bb80: 6465 2c20 616d 6f75 6e74 290a 2020 2020  de, amount).    
+0005bb90: 2020 2020 6d65 7468 6f64 203d 204e 6f6e      method = Non
+0005bba0: 650a 2020 2020 2020 2020 6d65 7468 6f64  e.        method
+0005bbb0: 2c20 7061 7261 6d73 203d 2073 656c 662e  , params = self.
+0005bbc0: 6861 6e64 6c65 5f6f 7074 696f 6e5f 616e  handle_option_an
+0005bbd0: 645f 7061 7261 6d73 2870 6172 616d 732c  d_params(params,
+0005bbe0: 2027 7472 616e 7366 6572 272c 2027 6d65   'transfer', 'me
+0005bbf0: 7468 6f64 272c 2027 7072 6976 6174 6550  thod', 'privateP
+0005bc00: 6f73 7441 7373 6574 5631 5072 6976 6174  ostAssetV1Privat
+0005bc10: 6554 7261 6e73 6665 7227 2920 2023 2076  eTransfer')  # v
+0005bc20: 3120 7072 6566 6572 7265 6420 6174 6d2c  1 preferred atm,
+0005bc30: 2062 6563 6175 7365 2069 7420 7375 7070   because it supp
+0005bc40: 6f72 7473 2066 756e 6469 6e67 0a20 2020  orts funding.   
+0005bc50: 2020 2020 2072 6571 7565 7374 203d 204e       request = N
+0005bc60: 6f6e 650a 2020 2020 2020 2020 6966 206d  one.        if m
+0005bc70: 6574 686f 6420 3d3d 2027 7072 6976 6174  ethod == 'privat
+0005bc80: 6550 6f73 7441 7373 6574 5633 5072 6976  ePostAssetV3Priv
+0005bc90: 6174 6554 7261 6e73 6665 7249 6e74 6572  ateTransferInter
+0005bca0: 5472 616e 7366 6572 2720 6f72 206d 6574  Transfer' or met
+0005bcb0: 686f 6420 3d3d 2027 7072 6976 6174 6550  hod == 'privateP
+0005bcc0: 6f73 7456 3541 7373 6574 5472 616e 7366  ostV5AssetTransf
+0005bcd0: 6572 496e 7465 7254 7261 6e73 6665 7227  erInterTransfer'
+0005bce0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0005bcf0: 7175 6573 7420 3d20 7b0a 2020 2020 2020  quest = {.      
+0005bd00: 2020 2020 2020 2020 2020 2774 7261 6e73            'trans
+0005bd10: 6665 7249 6427 3a20 7472 616e 7366 6572  ferId': transfer
+0005bd20: 4964 2c0a 2020 2020 2020 2020 2020 2020  Id,.            
+0005bd30: 2020 2020 2766 726f 6d41 6363 6f75 6e74      'fromAccount
+0005bd40: 5479 7065 273a 2066 726f 6d49 642c 0a20  Type': fromId,. 
+0005bd50: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0005bd60: 746f 4163 636f 756e 7454 7970 6527 3a20  toAccountType': 
+0005bd70: 746f 4964 2c0a 2020 2020 2020 2020 2020  toId,.          
+0005bd80: 2020 2020 2020 2763 6f69 6e27 3a20 6375        'coin': cu
+0005bd90: 7272 656e 6379 5b27 6964 275d 2c0a 2020  rrency['id'],.  
+0005bda0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+0005bdb0: 6d6f 756e 7427 3a20 616d 6f75 6e74 546f  mount': amountTo
+0005bdc0: 5072 6563 6973 696f 6e2c 0a20 2020 2020  Precision,.     
+0005bdd0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0005bde0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0005bdf0: 2020 2072 6571 7565 7374 203d 207b 0a20     request = {. 
+0005be00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0005be10: 7472 616e 7366 6572 5f69 6427 3a20 7472  transfer_id': tr
+0005be20: 616e 7366 6572 4964 2c0a 2020 2020 2020  ansferId,.      
+0005be30: 2020 2020 2020 2020 2020 2766 726f 6d5f            'from_
+0005be40: 6163 636f 756e 745f 7479 7065 273a 2066  account_type': f
+0005be50: 726f 6d49 642c 0a20 2020 2020 2020 2020  romId,.         
+0005be60: 2020 2020 2020 2027 746f 5f61 6363 6f75         'to_accou
+0005be70: 6e74 5f74 7970 6527 3a20 746f 4964 2c0a  nt_type': toId,.
+0005be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005be90: 2763 6f69 6e27 3a20 6375 7272 656e 6379  'coin': currency
+0005bea0: 5b27 6964 275d 2c0a 2020 2020 2020 2020  ['id'],.        
+0005beb0: 2020 2020 2020 2020 2761 6d6f 756e 7427          'amount'
+0005bec0: 3a20 616d 6f75 6e74 546f 5072 6563 6973  : amountToPrecis
+0005bed0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+0005bee0: 207d 0a20 2020 2020 2020 2072 6573 706f   }.        respo
+0005bef0: 6e73 6520 3d20 6177 6169 7420 6765 7461  nse = await geta
+0005bf00: 7474 7228 7365 6c66 2c20 6d65 7468 6f64  ttr(self, method
+0005bf10: 2928 7365 6c66 2e65 7874 656e 6428 7265  )(self.extend(re
+0005bf20: 7175 6573 742c 2070 6172 616d 7329 290a  quest, params)).
+0005bf30: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0005bf40: 2020 2320 7b0a 2020 2020 2020 2020 2320    # {.        # 
+0005bf50: 2020 2020 2272 6574 436f 6465 223a 2030      "retCode": 0
+0005bf60: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005bf70: 2272 6574 4d73 6722 3a20 2273 7563 6365  "retMsg": "succe
+0005bf80: 7373 222c 0a20 2020 2020 2020 2023 2020  ss",.        #  
+0005bf90: 2020 2022 7265 7375 6c74 223a 207b 0a20     "result": {. 
+0005bfa0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005bfb0: 2022 7472 616e 7366 6572 4964 223a 2022   "transferId": "
+0005bfc0: 3432 3434 6166 3434 2d66 3362 302d 3463  4244af44-f3b0-4c
+0005bfd0: 6636 2d61 3734 332d 6235 3635 3630 6539  f6-a743-b56560e9
+0005bfe0: 3837 6263 2220 2023 2074 7261 6e73 6665  87bc"  # transfe
+0005bff0: 725f 6964 2069 6e20 7631 0a20 2020 2020  r_id in v1.     
+0005c000: 2020 2023 2020 2020 207d 2c0a 2020 2020     #     },.    
+0005c010: 2020 2020 2320 2020 2020 2272 6574 4578      #     "retEx
+0005c020: 7449 6e66 6f22 3a20 7b7d 2c0a 2020 2020  tInfo": {},.    
+0005c030: 2020 2020 2320 2020 2020 2274 696d 6522      #     "time"
+0005c040: 3a20 3136 3636 3837 3538 3537 3230 350a  : 1666875857205.
+0005c050: 2020 2020 2020 2020 2320 7d0a 2020 2020          # }.    
+0005c060: 2020 2020 230a 2020 2020 2020 2020 7469      #.        ti
+0005c070: 6d65 7374 616d 7020 3d20 7365 6c66 2e73  mestamp = self.s
+0005c080: 6166 655f 696e 7465 6765 725f 3228 7265  afe_integer_2(re
+0005c090: 7370 6f6e 7365 2c20 2774 696d 6527 2c20  sponse, 'time', 
+0005c0a0: 2774 696d 655f 6e6f 7727 290a 2020 2020  'time_now').    
+0005c0b0: 2020 2020 7472 616e 7366 6572 203d 2073      transfer = s
+0005c0c0: 656c 662e 7361 6665 5f76 616c 7565 2872  elf.safe_value(r
+0005c0d0: 6573 706f 6e73 652c 2027 7265 7375 6c74  esponse, 'result
+0005c0e0: 272c 207b 7d29 0a20 2020 2020 2020 2073  ', {}).        s
+0005c0f0: 7461 7475 7352 6177 203d 2073 656c 662e  tatusRaw = self.
+0005c100: 7361 6665 5f73 7472 696e 675f 6e28 7265  safe_string_n(re
+0005c110: 7370 6f6e 7365 2c20 5b27 7265 7443 6f64  sponse, ['retCod
+0005c120: 6527 2c20 2772 6574 4d73 6727 2c20 2772  e', 'retMsg', 'r
+0005c130: 6574 5f63 6f64 6527 2c20 2772 6574 5f6d  et_code', 'ret_m
+0005c140: 7367 275d 290a 2020 2020 2020 2020 7374  sg']).        st
+0005c150: 6174 7573 203d 2073 656c 662e 7061 7273  atus = self.pars
+0005c160: 655f 7472 616e 7366 6572 5f73 7461 7475  e_transfer_statu
+0005c170: 7328 7374 6174 7573 5261 7729 0a20 2020  s(statusRaw).   
+0005c180: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0005c190: 2e65 7874 656e 6428 7365 6c66 2e70 6172  .extend(self.par
+0005c1a0: 7365 5f74 7261 6e73 6665 7228 7472 616e  se_transfer(tran
+0005c1b0: 7366 6572 2c20 6375 7272 656e 6379 292c  sfer, currency),
+0005c1c0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0005c1d0: 7469 6d65 7374 616d 7027 3a20 7469 6d65  timestamp': time
+0005c1e0: 7374 616d 702c 0a20 2020 2020 2020 2020  stamp,.         
+0005c1f0: 2020 2027 6461 7465 7469 6d65 273a 2073     'datetime': s
+0005c200: 656c 662e 6973 6f38 3630 3128 7469 6d65  elf.iso8601(time
+0005c210: 7374 616d 7029 2c0a 2020 2020 2020 2020  stamp),.        
+0005c220: 2020 2020 2761 6d6f 756e 7427 3a20 7365      'amount': se
+0005c230: 6c66 2e70 6172 7365 5f6e 756d 6265 7228  lf.parse_number(
+0005c240: 616d 6f75 6e74 546f 5072 6563 6973 696f  amountToPrecisio
+0005c250: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
+0005c260: 2766 726f 6d41 6363 6f75 6e74 273a 2066  'fromAccount': f
+0005c270: 726f 6d41 6363 6f75 6e74 2c0a 2020 2020  romAccount,.    
+0005c280: 2020 2020 2020 2020 2774 6f41 6363 6f75          'toAccou
+0005c290: 6e74 273a 2074 6f41 6363 6f75 6e74 2c0a  nt': toAccount,.
+0005c2a0: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
+0005c2b0: 7475 7327 3a20 7374 6174 7573 2c0a 2020  tus': status,.  
+0005c2c0: 2020 2020 2020 7d29 0a0a 2020 2020 6173        })..    as
+0005c2d0: 796e 6320 6465 6620 6665 7463 685f 7472  ync def fetch_tr
+0005c2e0: 616e 7366 6572 7328 7365 6c66 2c20 636f  ansfers(self, co
+0005c2f0: 6465 3a20 4f70 7469 6f6e 616c 5b73 7472  de: Optional[str
+0005c300: 5d20 3d20 4e6f 6e65 2c20 7369 6e63 653a  ] = None, since:
+0005c310: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0005c320: 204e 6f6e 652c 206c 696d 6974 3a20 4f70   None, limit: Op
+0005c330: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0005c340: 6e65 2c20 7061 7261 6d73 3d7b 7d29 3a0a  ne, params={}):.
+0005c350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0005c360: 2020 2020 6665 7463 6820 6120 6869 7374      fetch a hist
+0005c370: 6f72 7920 6f66 2069 6e74 6572 6e61 6c20  ory of internal 
+0005c380: 7472 616e 7366 6572 7320 6d61 6465 206f  transfers made o
+0005c390: 6e20 616e 2061 6363 6f75 6e74 0a20 2020  n an account.   
+0005c3a0: 2020 2020 2073 6565 2068 7474 7073 3a2f       see https:/
+0005c3b0: 2f62 7962 6974 2d65 7863 6861 6e67 652e  /bybit-exchange.
+0005c3c0: 6769 7468 7562 2e69 6f2f 646f 6373 2f76  github.io/docs/v
+0005c3d0: 352f 6173 7365 742f 696e 7465 722d 7472  5/asset/inter-tr
+0005c3e0: 616e 7366 6572 2d6c 6973 740a 2020 2020  ansfer-list.    
+0005c3f0: 2020 2020 3a70 6172 616d 2073 7472 7c4e      :param str|N
+0005c400: 6f6e 6520 636f 6465 3a20 756e 6966 6965  one code: unifie
+0005c410: 6420 6375 7272 656e 6379 2063 6f64 6520  d currency code 
+0005c420: 6f66 2074 6865 2063 7572 7265 6e63 7920  of the currency 
+0005c430: 7472 616e 7366 6572 7265 640a 2020 2020  transferred.    
+0005c440: 2020 2020 3a70 6172 616d 2069 6e74 7c4e      :param int|N
+0005c450: 6f6e 6520 7369 6e63 653a 2074 6865 2065  one since: the e
+0005c460: 6172 6c69 6573 7420 7469 6d65 2069 6e20  arliest time in 
+0005c470: 6d73 2074 6f20 6665 7463 6820 7472 616e  ms to fetch tran
+0005c480: 7366 6572 7320 666f 720a 2020 2020 2020  sfers for.      
+0005c490: 2020 3a70 6172 616d 2069 6e74 7c4e 6f6e    :param int|Non
+0005c4a0: 6520 6c69 6d69 743a 2074 6865 206d 6178  e limit: the max
+0005c4b0: 696d 756d 206e 756d 6265 7220 6f66 2020  imum number of  
+0005c4c0: 7472 616e 7366 6572 7320 7374 7275 6374  transfers struct
+0005c4d0: 7572 6573 2074 6f20 7265 7472 6965 7665  ures to retrieve
+0005c4e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0005c4f0: 6469 6374 2070 6172 616d 733a 2065 7874  dict params: ext
+0005c500: 7261 2070 6172 616d 6574 6572 7320 7370  ra parameters sp
+0005c510: 6563 6966 6963 2074 6f20 7468 6520 6279  ecific to the by
+0005c520: 6269 7420 6170 6920 656e 6470 6f69 6e74  bit api endpoint
+0005c530: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0005c540: 7320 5b64 6963 745d 3a20 6120 6c69 7374  s [dict]: a list
+0005c550: 206f 6620 6074 7261 6e73 6665 7220 7374   of `transfer st
+0005c560: 7275 6374 7572 6573 203c 6874 7470 733a  ructures <https:
+0005c570: 2f2f 646f 6373 2e63 6378 742e 636f 6d2f  //docs.ccxt.com/
+0005c580: 232f 3f69 643d 7472 616e 7366 6572 2d73  #/?id=transfer-s
+0005c590: 7472 7563 7475 7265 3e60 0a20 2020 2020  tructure>`.     
+0005c5a0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0005c5b0: 7761 6974 2073 656c 662e 6c6f 6164 5f6d  wait self.load_m
+0005c5c0: 6172 6b65 7473 2829 0a20 2020 2020 2020  arkets().       
+0005c5d0: 2063 7572 7265 6e63 7920 3d20 4e6f 6e65   currency = None
+0005c5e0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0005c5f0: 203d 207b 7d0a 2020 2020 2020 2020 6966   = {}.        if
+0005c600: 2063 6f64 6520 6973 206e 6f74 204e 6f6e   code is not Non
+0005c610: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+0005c620: 7572 7265 6e63 7920 3d20 7365 6c66 2e73  urrency = self.s
+0005c630: 6166 655f 6375 7272 656e 6379 5f63 6f64  afe_currency_cod
+0005c640: 6528 636f 6465 290a 2020 2020 2020 2020  e(code).        
+0005c650: 2020 2020 7265 7175 6573 745b 2763 6f69      request['coi
+0005c660: 6e27 5d20 3d20 6375 7272 656e 6379 0a20  n'] = currency. 
+0005c670: 2020 2020 2020 2069 6620 7369 6e63 6520         if since 
+0005c680: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0005c690: 2020 2020 2020 2020 2072 6571 7565 7374           request
+0005c6a0: 5b27 7374 6172 7454 696d 6527 5d20 3d20  ['startTime'] = 
+0005c6b0: 7369 6e63 650a 2020 2020 2020 2020 6966  since.        if
+0005c6c0: 206c 696d 6974 2069 7320 6e6f 7420 4e6f   limit is not No
+0005c6d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0005c6e0: 7265 7175 6573 745b 276c 696d 6974 275d  request['limit']
+0005c6f0: 203d 206c 696d 6974 0a20 2020 2020 2020   = limit.       
+0005c700: 2072 6573 706f 6e73 6520 3d20 6177 6169   response = awai
+0005c710: 7420 7365 6c66 2e70 7269 7661 7465 4765  t self.privateGe
+0005c720: 7456 3541 7373 6574 5472 616e 7366 6572  tV5AssetTransfer
+0005c730: 5175 6572 7949 6e74 6572 5472 616e 7366  QueryInterTransf
+0005c740: 6572 4c69 7374 2873 656c 662e 6578 7465  erList(self.exte
+0005c750: 6e64 2872 6571 7565 7374 2c20 7061 7261  nd(request, para
+0005c760: 6d73 2929 0a20 2020 2020 2020 2023 0a20  ms)).        #. 
+0005c770: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
+0005c780: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005c790: 2022 7265 7443 6f64 6522 3a20 302c 0a20   "retCode": 0,. 
+0005c7a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005c7b0: 2022 7265 744d 7367 223a 2022 7375 6363   "retMsg": "succ
+0005c7c0: 6573 7322 2c0a 2020 2020 2020 2020 2320  ess",.        # 
+0005c7d0: 2020 2020 2020 2020 2272 6573 756c 7422          "result"
+0005c7e0: 3a20 7b0a 2020 2020 2020 2020 2320 2020  : {.        #   
+0005c7f0: 2020 2020 2020 2020 2020 226c 6973 7422            "list"
+0005c800: 3a20 5b0a 2020 2020 2020 2020 2320 2020  : [.        #   
+0005c810: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+0005c820: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005c830: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+0005c840: 7261 6e73 6665 7249 6422 3a20 2273 656c  ransferId": "sel
+0005c850: 6654 7261 6e73 6665 725f 6131 3039 3163  fTransfer_a1091c
+0005c860: 6337 2d39 3336 342d 3462 3734 2d38 6465  c7-9364-4b74-8de
+0005c870: 312d 3138 6630 3263 3666 3264 3563 222c  1-18f02c6f2d5c",
+0005c880: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005c890: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0005c8a0: 636f 696e 223a 2022 5553 4454 222c 0a20  coin": "USDT",. 
+0005c8b0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005c8c0: 2020 2020 2020 2020 2020 2020 2022 616d               "am
+0005c8d0: 6f75 6e74 223a 2022 3530 3030 222c 0a20  ount": "5000",. 
+0005c8e0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005c8f0: 2020 2020 2020 2020 2020 2020 2022 6672               "fr
+0005c900: 6f6d 4163 636f 756e 7454 7970 6522 3a20  omAccountType": 
+0005c910: 2253 504f 5422 2c0a 2020 2020 2020 2020  "SPOT",.        
+0005c920: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0005c930: 2020 2020 2020 2274 6f41 6363 6f75 6e74        "toAccount
+0005c940: 5479 7065 223a 2022 554e 4946 4945 4422  Type": "UNIFIED"
+0005c950: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005c970: 2274 696d 6573 7461 6d70 223a 2022 3136  "timestamp": "16
+0005c980: 3637 3238 3332 3633 3030 3022 2c0a 2020  67283263000",.  
+0005c990: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005c9a0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+0005c9b0: 7475 7322 3a20 2253 5543 4345 5353 220a  tus": "SUCCESS".
+0005c9c0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005c9d0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+0005c9e0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005c9f0: 2020 5d2c 0a20 2020 2020 2020 2023 2020    ],.        #  
+0005ca00: 2020 2020 2020 2020 2020 2022 6e65 7874             "next
+0005ca10: 5061 6765 4375 7273 6f72 223a 2022 6579  PageCursor": "ey
+0005ca20: 4a74 6157 354a 5243 4936 4d54 4d31 4f44  JtaW5JRCI6MTM1OD
+0005ca30: 5132 4f43 7769 6257 4634 5355 5169 4f6a  Q2OCwibWF4SUQiOj
+0005ca40: 457a 4e54 6730 4e6a 6839 220a 2020 2020  EzNTg0Njh9".    
+0005ca50: 2020 2020 2320 2020 2020 2020 2020 7d2c      #         },
+0005ca60: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005ca70: 2020 2022 7265 7445 7874 496e 666f 223a     "retExtInfo":
+0005ca80: 207b 7d2c 0a20 2020 2020 2020 2023 2020   {},.        #  
+0005ca90: 2020 2020 2020 2022 7469 6d65 223a 2031         "time": 1
+0005caa0: 3637 3039 3838 3237 3136 3737 0a20 2020  670988271677.   
+0005cab0: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
+0005cac0: 2020 2020 2023 0a20 2020 2020 2020 2064       #.        d
+0005cad0: 6174 6120 3d20 7365 6c66 2e73 6166 655f  ata = self.safe_
+0005cae0: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
+0005caf0: 2772 6573 756c 7427 2c20 7b7d 290a 2020  'result', {}).  
+0005cb00: 2020 2020 2020 7472 616e 7366 6572 7320        transfers 
+0005cb10: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
+0005cb20: 6528 6461 7461 2c20 276c 6973 7427 2c20  e(data, 'list', 
+0005cb30: 5b5d 290a 2020 2020 2020 2020 7265 7475  []).        retu
+0005cb40: 726e 2073 656c 662e 7061 7273 655f 7472  rn self.parse_tr
+0005cb50: 616e 7366 6572 7328 7472 616e 7366 6572  ansfers(transfer
+0005cb60: 732c 2063 7572 7265 6e63 792c 2073 696e  s, currency, sin
+0005cb70: 6365 2c20 6c69 6d69 7429 0a0a 2020 2020  ce, limit)..    
+0005cb80: 6173 796e 6320 6465 6620 626f 7272 6f77  async def borrow
+0005cb90: 5f6d 6172 6769 6e28 7365 6c66 2c20 636f  _margin(self, co
+0005cba0: 6465 3a20 7374 722c 2061 6d6f 756e 742c  de: str, amount,
+0005cbb0: 2073 796d 626f 6c3a 204f 7074 696f 6e61   symbol: Optiona
+0005cbc0: 6c5b 7374 725d 203d 204e 6f6e 652c 2070  l[str] = None, p
+0005cbd0: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
+0005cbe0: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
+0005cbf0: 7265 6174 6520 6120 6c6f 616e 2074 6f20  reate a loan to 
+0005cc00: 626f 7272 6f77 206d 6172 6769 6e0a 2020  borrow margin.  
+0005cc10: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
+0005cc20: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
+0005cc30: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
+0005cc40: 7370 6f74 2f76 332f 2374 2d62 6f72 726f  spot/v3/#t-borro
+0005cc50: 776d 6172 6769 6e6c 6f61 6e0a 2020 2020  wmarginloan.    
+0005cc60: 2020 2020 3a70 6172 616d 2073 7472 2063      :param str c
+0005cc70: 6f64 653a 2075 6e69 6669 6564 2063 7572  ode: unified cur
+0005cc80: 7265 6e63 7920 636f 6465 206f 6620 7468  rency code of th
+0005cc90: 6520 6375 7272 656e 6379 2074 6f20 626f  e currency to bo
+0005cca0: 7272 6f77 0a20 2020 2020 2020 203a 7061  rrow.        :pa
+0005ccb0: 7261 6d20 666c 6f61 7420 616d 6f75 6e74  ram float amount
+0005ccc0: 3a20 7468 6520 616d 6f75 6e74 2074 6f20  : the amount to 
+0005ccd0: 626f 7272 6f77 0a20 2020 2020 2020 203a  borrow.        :
+0005cce0: 7061 7261 6d20 7374 727c 4e6f 6e65 2073  param str|None s
+0005ccf0: 796d 626f 6c3a 206e 6f74 2075 7365 6420  ymbol: not used 
+0005cd00: 6279 2062 7962 6974 2e62 6f72 726f 774d  by bybit.borrowM
+0005cd10: 6172 6769 6e28 290a 2020 2020 2020 2020  argin().        
+0005cd20: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
+0005cd30: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
+0005cd40: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
+0005cd50: 2074 6865 2062 7962 6974 2061 7069 2065   the bybit api e
+0005cd60: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
+0005cd70: 3a72 6574 7572 6e73 2064 6963 743a 2061  :returns dict: a
+0005cd80: 2060 6d61 7267 696e 206c 6f61 6e20 7374   `margin loan st
+0005cd90: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
+0005cda0: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
+0005cdb0: 2f3f 6964 3d6d 6172 6769 6e2d 6c6f 616e  /?id=margin-loan
+0005cdc0: 2d73 7472 7563 7475 7265 3e60 0a20 2020  -structure>`.   
+0005cdd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0005cde0: 2061 7761 6974 2073 656c 662e 6c6f 6164   await self.load
+0005cdf0: 5f6d 6172 6b65 7473 2829 0a20 2020 2020  _markets().     
+0005ce00: 2020 2063 7572 7265 6e63 7920 3d20 7365     currency = se
+0005ce10: 6c66 2e63 7572 7265 6e63 7928 636f 6465  lf.currency(code
+0005ce20: 290a 2020 2020 2020 2020 6d61 7267 696e  ).        margin
+0005ce30: 4d6f 6465 2c20 7175 6572 7920 3d20 7365  Mode, query = se
+0005ce40: 6c66 2e68 616e 646c 655f 6d61 7267 696e  lf.handle_margin
+0005ce50: 5f6d 6f64 655f 616e 645f 7061 7261 6d73  _mode_and_params
+0005ce60: 2827 626f 7272 6f77 4d61 7267 696e 272c  ('borrowMargin',
+0005ce70: 2070 6172 616d 7329 0a20 2020 2020 2020   params).       
+0005ce80: 2069 6620 6d61 7267 696e 4d6f 6465 203d   if marginMode =
+0005ce90: 3d20 2769 736f 6c61 7465 6427 3a0a 2020  = 'isolated':.  
+0005cea0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0005ceb0: 4e6f 7453 7570 706f 7274 6564 2873 656c  NotSupported(sel
+0005cec0: 662e 6964 202b 2027 2062 6f72 726f 774d  f.id + ' borrowM
+0005ced0: 6172 6769 6e28 2920 6361 6e6e 6f74 2075  argin() cannot u
+0005cee0: 7365 2069 736f 6c61 7465 6420 6d61 7267  se isolated marg
+0005cef0: 696e 2729 0a20 2020 2020 2020 2072 6571  in').        req
+0005cf00: 7565 7374 203d 207b 0a20 2020 2020 2020  uest = {.       
+0005cf10: 2020 2020 2027 636f 696e 273a 2063 7572       'coin': cur
+0005cf20: 7265 6e63 795b 2769 6427 5d2c 0a20 2020  rency['id'],.   
+0005cf30: 2020 2020 2020 2020 2027 7174 7927 3a20           'qty': 
+0005cf40: 7365 6c66 2e63 7572 7265 6e63 795f 746f  self.currency_to
+0005cf50: 5f70 7265 6369 7369 6f6e 2863 6f64 652c  _precision(code,
+0005cf60: 2061 6d6f 756e 7429 2c0a 2020 2020 2020   amount),.      
+0005cf70: 2020 7d0a 2020 2020 2020 2020 7265 7370    }.        resp
+0005cf80: 6f6e 7365 203d 2061 7761 6974 2073 656c  onse = await sel
+0005cf90: 662e 7072 6976 6174 6550 6f73 7453 706f  f.privatePostSpo
+0005cfa0: 7456 3350 7269 7661 7465 4372 6f73 734d  tV3PrivateCrossM
+0005cfb0: 6172 6769 6e4c 6f61 6e28 7365 6c66 2e65  arginLoan(self.e
+0005cfc0: 7874 656e 6428 7265 7175 6573 742c 2071  xtend(request, q
+0005cfd0: 7565 7279 2929 0a20 2020 2020 2020 2023  uery)).        #
+0005cfe0: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+0005cff0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d000: 2020 2022 7265 7443 6f64 6522 3a20 302c     "retCode": 0,
+0005d010: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d020: 2020 2022 7265 744d 7367 223a 2022 7375     "retMsg": "su
+0005d030: 6363 6573 7322 2c0a 2020 2020 2020 2020  ccess",.        
+0005d040: 2320 2020 2020 2020 2020 2272 6573 756c  #         "resul
+0005d050: 7422 3a20 7b0a 2020 2020 2020 2020 2320  t": {.        # 
+0005d060: 2020 2020 2020 2020 2020 2020 2274 7261              "tra
+0005d070: 6e73 6163 7449 6422 3a20 2231 3431 3433  nsactId": "14143
+0005d080: 220a 2020 2020 2020 2020 2320 2020 2020  ".        #     
+0005d090: 2020 2020 7d2c 0a20 2020 2020 2020 2023      },.        #
+0005d0a0: 2020 2020 2020 2020 2022 7265 7445 7874           "retExt
+0005d0b0: 496e 666f 223a 206e 756c 6c2c 0a20 2020  Info": null,.   
+0005d0c0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005d0d0: 7469 6d65 223a 2031 3636 3236 3137 3834  time": 166261784
+0005d0e0: 3839 3730 0a20 2020 2020 2020 2023 2020  8970.        #  
+0005d0f0: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
+0005d100: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0005d110: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
+0005d120: 7265 7370 6f6e 7365 2c20 2772 6573 756c  response, 'resul
+0005d130: 7427 2c20 7b7d 290a 2020 2020 2020 2020  t', {}).        
+0005d140: 7472 616e 7361 6374 696f 6e20 3d20 7365  transaction = se
+0005d150: 6c66 2e70 6172 7365 5f6d 6172 6769 6e5f  lf.parse_margin_
+0005d160: 6c6f 616e 2872 6573 756c 742c 2063 7572  loan(result, cur
+0005d170: 7265 6e63 7929 0a20 2020 2020 2020 2072  rency).        r
+0005d180: 6574 7572 6e20 7365 6c66 2e65 7874 656e  eturn self.exten
+0005d190: 6428 7472 616e 7361 6374 696f 6e2c 207b  d(transaction, {
+0005d1a0: 0a20 2020 2020 2020 2020 2020 2027 7379  .            'sy
+0005d1b0: 6d62 6f6c 273a 2073 796d 626f 6c2c 0a20  mbol': symbol,. 
+0005d1c0: 2020 2020 2020 2020 2020 2027 616d 6f75             'amou
+0005d1d0: 6e74 273a 2061 6d6f 756e 742c 0a20 2020  nt': amount,.   
+0005d1e0: 2020 2020 207d 290a 0a20 2020 2061 7379       })..    asy
+0005d1f0: 6e63 2064 6566 2072 6570 6179 5f6d 6172  nc def repay_mar
+0005d200: 6769 6e28 7365 6c66 2c20 636f 6465 3a20  gin(self, code: 
+0005d210: 7374 722c 2061 6d6f 756e 742c 2073 796d  str, amount, sym
+0005d220: 626f 6c3a 204f 7074 696f 6e61 6c5b 7374  bol: Optional[st
+0005d230: 725d 203d 204e 6f6e 652c 2070 6172 616d  r] = None, param
+0005d240: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
+0005d250: 2222 0a20 2020 2020 2020 2072 6570 6179  "".        repay
+0005d260: 2062 6f72 726f 7765 6420 6d61 7267 696e   borrowed margin
+0005d270: 2061 6e64 2069 6e74 6572 6573 740a 2020   and interest.  
+0005d280: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
+0005d290: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
+0005d2a0: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
+0005d2b0: 7370 6f74 2f76 332f 2374 2d72 6570 6179  spot/v3/#t-repay
+0005d2c0: 6d61 7267 696e 6c6f 616e 0a20 2020 2020  marginloan.     
+0005d2d0: 2020 203a 7061 7261 6d20 7374 7220 636f     :param str co
+0005d2e0: 6465 3a20 756e 6966 6965 6420 6375 7272  de: unified curr
+0005d2f0: 656e 6379 2063 6f64 6520 6f66 2074 6865  ency code of the
+0005d300: 2063 7572 7265 6e63 7920 746f 2072 6570   currency to rep
+0005d310: 6179 0a20 2020 2020 2020 203a 7061 7261  ay.        :para
+0005d320: 6d20 666c 6f61 7420 616d 6f75 6e74 3a20  m float amount: 
+0005d330: 7468 6520 616d 6f75 6e74 2074 6f20 7265  the amount to re
+0005d340: 7061 790a 2020 2020 2020 2020 3a70 6172  pay.        :par
+0005d350: 616d 2073 7472 7c4e 6f6e 6520 7379 6d62  am str|None symb
+0005d360: 6f6c 3a20 6e6f 7420 7573 6564 2062 7920  ol: not used by 
+0005d370: 6279 6269 742e 7265 7061 794d 6172 6769  bybit.repayMargi
+0005d380: 6e28 290a 2020 2020 2020 2020 3a70 6172  n().        :par
+0005d390: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
+0005d3a0: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
+0005d3b0: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
+0005d3c0: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
+0005d3d0: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
+0005d3e0: 7572 6e73 2064 6963 743a 2061 2060 6d61  urns dict: a `ma
+0005d3f0: 7267 696e 206c 6f61 6e20 7374 7275 6374  rgin loan struct
+0005d400: 7572 6520 3c68 7474 7073 3a2f 2f64 6f63  ure <https://doc
+0005d410: 732e 6363 7874 2e63 6f6d 2f23 2f3f 6964  s.ccxt.com/#/?id
+0005d420: 3d6d 6172 6769 6e2d 6c6f 616e 2d73 7472  =margin-loan-str
+0005d430: 7563 7475 7265 3e60 0a20 2020 2020 2020  ucture>`.       
+0005d440: 2022 2222 0a20 2020 2020 2020 2061 7761   """.        awa
+0005d450: 6974 2073 656c 662e 6c6f 6164 5f6d 6172  it self.load_mar
+0005d460: 6b65 7473 2829 0a20 2020 2020 2020 2063  kets().        c
+0005d470: 7572 7265 6e63 7920 3d20 7365 6c66 2e63  urrency = self.c
+0005d480: 7572 7265 6e63 7928 636f 6465 290a 2020  urrency(code).  
+0005d490: 2020 2020 2020 6d61 7267 696e 4d6f 6465        marginMode
+0005d4a0: 2c20 7175 6572 7920 3d20 7365 6c66 2e68  , query = self.h
+0005d4b0: 616e 646c 655f 6d61 7267 696e 5f6d 6f64  andle_margin_mod
+0005d4c0: 655f 616e 645f 7061 7261 6d73 2827 7265  e_and_params('re
+0005d4d0: 7061 794d 6172 6769 6e27 2c20 7061 7261  payMargin', para
+0005d4e0: 6d73 290a 2020 2020 2020 2020 6966 206d  ms).        if m
+0005d4f0: 6172 6769 6e4d 6f64 6520 3d3d 2027 6973  arginMode == 'is
+0005d500: 6f6c 6174 6564 273a 0a20 2020 2020 2020  olated':.       
+0005d510: 2020 2020 2072 6169 7365 204e 6f74 5375       raise NotSu
+0005d520: 7070 6f72 7465 6428 7365 6c66 2e69 6420  pported(self.id 
+0005d530: 2b20 2720 7265 7061 794d 6172 6769 6e28  + ' repayMargin(
+0005d540: 2920 6361 6e6e 6f74 2075 7365 2069 736f  ) cannot use iso
+0005d550: 6c61 7465 6420 6d61 7267 696e 2729 0a20  lated margin'). 
+0005d560: 2020 2020 2020 2072 6571 7565 7374 203d         request =
+0005d570: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0005d580: 636f 696e 273a 2063 7572 7265 6e63 795b  coin': currency[
+0005d590: 2769 6427 5d2c 0a20 2020 2020 2020 2020  'id'],.         
+0005d5a0: 2020 2027 7174 7927 3a20 7365 6c66 2e6e     'qty': self.n
+0005d5b0: 756d 6265 725f 746f 5f73 7472 696e 6728  umber_to_string(
+0005d5c0: 616d 6f75 6e74 292c 0a20 2020 2020 2020  amount),.       
+0005d5d0: 207d 0a20 2020 2020 2020 2072 6573 706f   }.        respo
+0005d5e0: 6e73 6520 3d20 6177 6169 7420 7365 6c66  nse = await self
+0005d5f0: 2e70 7269 7661 7465 506f 7374 5370 6f74  .privatePostSpot
+0005d600: 5633 5072 6976 6174 6543 726f 7373 4d61  V3PrivateCrossMa
+0005d610: 7267 696e 5265 7061 7928 7365 6c66 2e65  rginRepay(self.e
+0005d620: 7874 656e 6428 7265 7175 6573 742c 2071  xtend(request, q
+0005d630: 7565 7279 2929 0a20 2020 2020 2020 2023  uery)).        #
+0005d640: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+0005d650: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d660: 2020 2022 7265 7443 6f64 6522 3a20 302c     "retCode": 0,
+0005d670: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d680: 2020 2022 7265 744d 7367 223a 2022 7375     "retMsg": "su
+0005d690: 6363 6573 7322 2c0a 2020 2020 2020 2020  ccess",.        
+0005d6a0: 2320 2020 2020 2020 2020 2272 6573 756c  #         "resul
+0005d6b0: 7422 3a20 7b0a 2020 2020 2020 2020 2320  t": {.        # 
+0005d6c0: 2020 2020 2020 2020 2020 2022 7265 7061             "repa
+0005d6d0: 7949 6422 3a20 2231 3231 3238 220a 2020  yId": "12128".  
+0005d6e0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005d6f0: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
+0005d700: 2020 2020 2022 7265 7445 7874 496e 666f       "retExtInfo
+0005d710: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
+0005d720: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
+0005d730: 223a 2031 3636 3236 3138 3239 3834 3532  ": 1662618298452
+0005d740: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+0005d750: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005d760: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0005d770: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
+0005d780: 6f6e 7365 2c20 2772 6573 756c 7427 2c20  onse, 'result', 
+0005d790: 7b7d 290a 2020 2020 2020 2020 7472 616e  {}).        tran
+0005d7a0: 7361 6374 696f 6e20 3d20 7365 6c66 2e70  saction = self.p
+0005d7b0: 6172 7365 5f6d 6172 6769 6e5f 6c6f 616e  arse_margin_loan
+0005d7c0: 2872 6573 756c 742c 2063 7572 7265 6e63  (result, currenc
+0005d7d0: 7929 0a20 2020 2020 2020 2072 6574 7572  y).        retur
+0005d7e0: 6e20 7365 6c66 2e65 7874 656e 6428 7472  n self.extend(tr
+0005d7f0: 616e 7361 6374 696f 6e2c 207b 0a20 2020  ansaction, {.   
+0005d800: 2020 2020 2020 2020 2027 7379 6d62 6f6c           'symbol
+0005d810: 273a 2073 796d 626f 6c2c 0a20 2020 2020  ': symbol,.     
+0005d820: 2020 2020 2020 2027 616d 6f75 6e74 273a         'amount':
+0005d830: 2061 6d6f 756e 742c 0a20 2020 2020 2020   amount,.       
+0005d840: 207d 290a 0a20 2020 2064 6566 2070 6172   })..    def par
+0005d850: 7365 5f6d 6172 6769 6e5f 6c6f 616e 2873  se_margin_loan(s
+0005d860: 656c 662c 2069 6e66 6f2c 2063 7572 7265  elf, info, curre
+0005d870: 6e63 793d 4e6f 6e65 293a 0a20 2020 2020  ncy=None):.     
+0005d880: 2020 2023 0a20 2020 2020 2020 2023 2062     #.        # b
+0005d890: 6f72 726f 774d 6172 6769 6e0a 2020 2020  orrowMargin.    
+0005d8a0: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
+0005d8b0: 2020 2020 7b0a 2020 2020 2020 2020 2320      {.        # 
+0005d8c0: 2020 2020 2020 2020 2274 7261 6e73 6163          "transac
+0005d8d0: 7449 6422 3a20 2231 3431 3433 220a 2020  tId": "14143".  
+0005d8e0: 2020 2020 2020 2320 2020 2020 7d0a 2020        #     }.  
+0005d8f0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+0005d900: 2320 7265 7061 794d 6172 6769 6e0a 2020  # repayMargin.  
+0005d910: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+0005d920: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
+0005d930: 2320 2020 2020 2020 2020 2272 6570 6179  #         "repay
+0005d940: 4964 223a 2022 3132 3132 3822 0a20 2020  Id": "12128".   
+0005d950: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
+0005d960: 2020 2020 2023 0a20 2020 2020 2020 2072       #.        r
+0005d970: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+0005d980: 2020 2020 2769 6427 3a20 7365 6c66 2e73      'id': self.s
+0005d990: 6166 655f 7374 7269 6e67 5f32 2869 6e66  afe_string_2(inf
+0005d9a0: 6f2c 2027 7472 616e 7361 6374 4964 272c  o, 'transactId',
+0005d9b0: 2027 7265 7061 7949 6427 292c 0a20 2020   'repayId'),.   
+0005d9c0: 2020 2020 2020 2020 2027 6375 7272 656e           'curren
+0005d9d0: 6379 273a 2073 656c 662e 7361 6665 5f73  cy': self.safe_s
+0005d9e0: 7472 696e 6728 6375 7272 656e 6379 2c20  tring(currency, 
+0005d9f0: 2763 6f64 6527 292c 0a20 2020 2020 2020  'code'),.       
+0005da00: 2020 2020 2027 616d 6f75 6e74 273a 204e       'amount': N
+0005da10: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0005da20: 2027 7379 6d62 6f6c 273a 204e 6f6e 652c   'symbol': None,
+0005da30: 0a20 2020 2020 2020 2020 2020 2027 7469  .            'ti
+0005da40: 6d65 7374 616d 7027 3a20 4e6f 6e65 2c0a  mestamp': None,.
+0005da50: 2020 2020 2020 2020 2020 2020 2764 6174              'dat
+0005da60: 6574 696d 6527 3a20 4e6f 6e65 2c0a 2020  etime': None,.  
+0005da70: 2020 2020 2020 2020 2020 2769 6e66 6f27            'info'
+0005da80: 3a20 696e 666f 2c0a 2020 2020 2020 2020  : info,.        
+0005da90: 7d0a 0a20 2020 2064 6566 2070 6172 7365  }..    def parse
+0005daa0: 5f74 7261 6e73 6665 725f 7374 6174 7573  _transfer_status
+0005dab0: 2873 656c 662c 2073 7461 7475 7329 3a0a  (self, status):.
+0005dac0: 2020 2020 2020 2020 7374 6174 7573 6573          statuses
+0005dad0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0005dae0: 2027 3027 3a20 276f 6b27 2c0a 2020 2020   '0': 'ok',.    
+0005daf0: 2020 2020 2020 2020 274f 4b27 3a20 276f          'OK': 'o
+0005db00: 6b27 2c0a 2020 2020 2020 2020 2020 2020  k',.            
+0005db10: 2753 5543 4345 5353 273a 2027 6f6b 272c  'SUCCESS': 'ok',
+0005db20: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0005db30: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+0005db40: 6166 655f 7374 7269 6e67 2873 7461 7475  afe_string(statu
+0005db50: 7365 732c 2073 7461 7475 732c 2073 7461  ses, status, sta
+0005db60: 7475 7329 0a0a 2020 2020 6465 6620 7061  tus)..    def pa
+0005db70: 7273 655f 7472 616e 7366 6572 2873 656c  rse_transfer(sel
+0005db80: 662c 2074 7261 6e73 6665 722c 2063 7572  f, transfer, cur
+0005db90: 7265 6e63 793d 4e6f 6e65 293a 0a20 2020  rency=None):.   
+0005dba0: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+0005dbb0: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
+0005dbc0: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
+0005dbd0: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
+0005dbe0: 2020 2020 2020 2274 7261 6e73 6665 7249        "transferI
+0005dbf0: 6422 3a20 2232 3263 3262 6331 312d 6564  d": "22c2bc11-ed
+0005dc00: 3562 2d34 3961 342d 3836 3437 2d63 3465  5b-49a4-8647-c4e
+0005dc10: 3066 3566 3666 3262 3222 2020 2320 7472  0f5f6f2b2"  # tr
+0005dc20: 616e 7366 6572 5f69 6420 696e 2076 310a  ansfer_id in v1.
+0005dc30: 2020 2020 2020 2020 2320 2020 2020 7d0a          #     }.
+0005dc40: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0005dc50: 2020 2320 6665 7463 6854 7261 6e73 6665    # fetchTransfe
+0005dc60: 7273 0a20 2020 2020 2020 2023 0a20 2020  rs.        #.   
+0005dc70: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
+0005dc80: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005dc90: 7472 616e 7366 6572 4964 223a 2022 6539  transferId": "e9
+0005dca0: 6334 3231 6334 2d62 3031 302d 3462 3136  c421c4-b010-4b16
+0005dcb0: 2d61 6264 362d 3130 3631 3739 6632 3737  -abd6-106179f277
+0005dcc0: 3032 222c 2020 2320 7472 616e 7366 6572  02",  # transfer
+0005dcd0: 5f69 6420 696e 2076 310a 2020 2020 2020  _id in v1.      
+0005dce0: 2020 2320 2020 2020 2020 2020 2263 6f69    #         "coi
+0005dcf0: 6e22 3a20 2255 5344 5422 2c0a 2020 2020  n": "USDT",.    
+0005dd00: 2020 2020 2320 2020 2020 2020 2020 2261      #         "a
+0005dd10: 6d6f 756e 7422 3a20 2238 222c 0a20 2020  mount": "8",.   
+0005dd20: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005dd30: 6672 6f6d 4163 636f 756e 7454 7970 6522  fromAccountType"
+0005dd40: 3a20 2246 554e 4422 2c20 2023 2066 726f  : "FUND",  # fro
+0005dd50: 6d5f 6163 636f 756e 745f 7479 7065 2069  m_account_type i
+0005dd60: 6e20 7631 0a20 2020 2020 2020 2023 2020  n v1.        #  
+0005dd70: 2020 2020 2020 2022 746f 4163 636f 756e         "toAccoun
+0005dd80: 7454 7970 6522 3a20 2253 504f 5422 2c20  tType": "SPOT", 
+0005dd90: 2023 2074 6f5f 6163 636f 756e 745f 7479   # to_account_ty
+0005dda0: 7065 2069 6e20 7631 0a20 2020 2020 2020  pe in v1.       
+0005ddb0: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
+0005ddc0: 7374 616d 7022 3a20 2231 3636 3638 3739  stamp": "1666879
+0005ddd0: 3432 3630 3030 222c 0a20 2020 2020 2020  426000",.       
+0005dde0: 2023 2020 2020 2020 2020 2022 7374 6174   #         "stat
+0005ddf0: 7573 223a 2022 5355 4343 4553 5322 0a20  us": "SUCCESS". 
+0005de00: 2020 2020 2020 2023 2020 2020 2020 7d0a         #      }.
+0005de10: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0005de20: 2020 6375 7272 656e 6379 4964 203d 2073    currencyId = s
+0005de30: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005de40: 7472 616e 7366 6572 2c20 2763 6f69 6e27  transfer, 'coin'
+0005de50: 290a 2020 2020 2020 2020 7469 6d65 7374  ).        timest
+0005de60: 616d 7020 3d20 7365 6c66 2e73 6166 655f  amp = self.safe_
+0005de70: 696e 7465 6765 7228 7472 616e 7366 6572  integer(transfer
+0005de80: 2c20 2774 696d 6573 7461 6d70 2729 0a20  , 'timestamp'). 
+0005de90: 2020 2020 2020 2066 726f 6d41 6363 6f75         fromAccou
+0005dea0: 6e74 4964 203d 2073 656c 662e 7361 6665  ntId = self.safe
+0005deb0: 5f73 7472 696e 675f 3228 7472 616e 7366  _string_2(transf
+0005dec0: 6572 2c20 2766 726f 6d41 6363 6f75 6e74  er, 'fromAccount
+0005ded0: 5479 7065 272c 2027 6672 6f6d 5f61 6363  Type', 'from_acc
+0005dee0: 6f75 6e74 5f74 7970 6527 290a 2020 2020  ount_type').    
+0005def0: 2020 2020 746f 4163 636f 756e 7449 6420      toAccountId 
+0005df00: 3d20 7365 6c66 2e73 6166 655f 7374 7269  = self.safe_stri
+0005df10: 6e67 5f32 2874 7261 6e73 6665 722c 2027  ng_2(transfer, '
+0005df20: 746f 4163 636f 756e 7454 7970 6527 2c20  toAccountType', 
+0005df30: 2774 6f5f 6163 636f 756e 745f 7479 7065  'to_account_type
+0005df40: 2729 0a20 2020 2020 2020 2061 6363 6f75  ').        accou
+0005df50: 6e74 4964 7320 3d20 7365 6c66 2e73 6166  ntIds = self.saf
+0005df60: 655f 7661 6c75 6528 7365 6c66 2e6f 7074  e_value(self.opt
+0005df70: 696f 6e73 2c20 2761 6363 6f75 6e74 7342  ions, 'accountsB
+0005df80: 7949 6427 2c20 7b7d 290a 2020 2020 2020  yId', {}).      
+0005df90: 2020 6672 6f6d 4163 636f 756e 7420 3d20    fromAccount = 
+0005dfa0: 7365 6c66 2e73 6166 655f 7374 7269 6e67  self.safe_string
+0005dfb0: 2861 6363 6f75 6e74 4964 732c 2066 726f  (accountIds, fro
+0005dfc0: 6d41 6363 6f75 6e74 4964 2c20 6672 6f6d  mAccountId, from
+0005dfd0: 4163 636f 756e 7449 6429 0a20 2020 2020  AccountId).     
+0005dfe0: 2020 2074 6f41 6363 6f75 6e74 203d 2073     toAccount = s
+0005dff0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005e000: 6163 636f 756e 7449 6473 2c20 746f 4163  accountIds, toAc
+0005e010: 636f 756e 7449 642c 2074 6f41 6363 6f75  countId, toAccou
+0005e020: 6e74 4964 290a 2020 2020 2020 2020 7265  ntId).        re
+0005e030: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
+0005e040: 2020 2027 696e 666f 273a 2074 7261 6e73     'info': trans
+0005e050: 6665 722c 0a20 2020 2020 2020 2020 2020  fer,.           
+0005e060: 2027 6964 273a 2073 656c 662e 7361 6665   'id': self.safe
+0005e070: 5f73 7472 696e 675f 3228 7472 616e 7366  _string_2(transf
+0005e080: 6572 2c20 2774 7261 6e73 6665 7249 6427  er, 'transferId'
+0005e090: 2c20 2774 7261 6e73 6665 725f 6964 2729  , 'transfer_id')
+0005e0a0: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+0005e0b0: 696d 6573 7461 6d70 273a 2074 696d 6573  imestamp': times
+0005e0c0: 7461 6d70 2c0a 2020 2020 2020 2020 2020  tamp,.          
+0005e0d0: 2020 2764 6174 6574 696d 6527 3a20 7365    'datetime': se
+0005e0e0: 6c66 2e69 736f 3836 3031 2874 696d 6573  lf.iso8601(times
+0005e0f0: 7461 6d70 292c 0a20 2020 2020 2020 2020  tamp),.         
+0005e100: 2020 2027 6375 7272 656e 6379 273a 2073     'currency': s
+0005e110: 656c 662e 7361 6665 5f63 7572 7265 6e63  elf.safe_currenc
+0005e120: 795f 636f 6465 2863 7572 7265 6e63 7949  y_code(currencyI
+0005e130: 642c 2063 7572 7265 6e63 7929 2c0a 2020  d, currency),.  
+0005e140: 2020 2020 2020 2020 2020 2761 6d6f 756e            'amoun
+0005e150: 7427 3a20 7365 6c66 2e73 6166 655f 6e75  t': self.safe_nu
+0005e160: 6d62 6572 2874 7261 6e73 6665 722c 2027  mber(transfer, '
+0005e170: 616d 6f75 6e74 2729 2c0a 2020 2020 2020  amount'),.      
+0005e180: 2020 2020 2020 2766 726f 6d41 6363 6f75        'fromAccou
+0005e190: 6e74 273a 2066 726f 6d41 6363 6f75 6e74  nt': fromAccount
+0005e1a0: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+0005e1b0: 6f41 6363 6f75 6e74 273a 2074 6f41 6363  oAccount': toAcc
+0005e1c0: 6f75 6e74 2c0a 2020 2020 2020 2020 2020  ount,.          
+0005e1d0: 2020 2773 7461 7475 7327 3a20 7365 6c66    'status': self
+0005e1e0: 2e70 6172 7365 5f74 7261 6e73 6665 725f  .parse_transfer_
+0005e1f0: 7374 6174 7573 2873 656c 662e 7361 6665  status(self.safe
+0005e200: 5f73 7472 696e 6728 7472 616e 7366 6572  _string(transfer
+0005e210: 2c20 2773 7461 7475 7327 2929 2c0a 2020  , 'status')),.  
+0005e220: 2020 2020 2020 7d0a 0a20 2020 2061 7379        }..    asy
+0005e230: 6e63 2064 6566 2066 6574 6368 5f64 6572  nc def fetch_der
+0005e240: 6976 6174 6976 6573 5f6d 6172 6b65 745f  ivatives_market_
+0005e250: 6c65 7665 7261 6765 5f74 6965 7273 2873  leverage_tiers(s
+0005e260: 656c 662c 2073 796d 626f 6c3a 2073 7472  elf, symbol: str
+0005e270: 2c20 7061 7261 6d73 3d7b 7d29 3a0a 2020  , params={}):.  
+0005e280: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+0005e290: 2e6c 6f61 645f 6d61 726b 6574 7328 290a  .load_markets().
+0005e2a0: 2020 2020 2020 2020 6d61 726b 6574 203d          market =
+0005e2b0: 2073 656c 662e 6d61 726b 6574 2873 796d   self.market(sym
+0005e2c0: 626f 6c29 0a20 2020 2020 2020 2072 6571  bol).        req
+0005e2d0: 7565 7374 203d 207b 0a20 2020 2020 2020  uest = {.       
+0005e2e0: 2020 2020 2027 7379 6d62 6f6c 273a 206d       'symbol': m
+0005e2f0: 6172 6b65 745b 2769 6427 5d2c 0a20 2020  arket['id'],.   
+0005e300: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
+0005e310: 6620 6d61 726b 6574 5b27 6c69 6e65 6172  f market['linear
+0005e320: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+0005e330: 7265 7175 6573 745b 2763 6174 6567 6f72  request['categor
+0005e340: 7927 5d20 3d20 276c 696e 6561 7227 0a20  y'] = 'linear'. 
+0005e350: 2020 2020 2020 2065 6c69 6620 6d61 726b         elif mark
+0005e360: 6574 5b27 696e 7665 7273 6527 5d3a 0a20  et['inverse']:. 
+0005e370: 2020 2020 2020 2020 2020 2072 6571 7565             reque
+0005e380: 7374 5b27 6361 7465 676f 7279 275d 203d  st['category'] =
+0005e390: 2027 696e 7665 7273 6527 0a20 2020 2020   'inverse'.     
+0005e3a0: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
+0005e3b0: 6169 7420 7365 6c66 2e70 7562 6c69 6347  ait self.publicG
+0005e3c0: 6574 5635 4d61 726b 6574 5269 736b 4c69  etV5MarketRiskLi
+0005e3d0: 6d69 7428 7365 6c66 2e65 7874 656e 6428  mit(self.extend(
+0005e3e0: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
+0005e3f0: 290a 2020 2020 2020 2020 230a 2020 2020  ).        #.    
+0005e400: 2020 2020 2320 2020 2020 7b0a 2020 2020      #     {.    
+0005e410: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
+0005e420: 6574 436f 6465 223a 2030 2c0a 2020 2020  etCode": 0,.    
+0005e430: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
+0005e440: 6574 4d73 6722 3a20 224f 4b22 2c0a 2020  etMsg": "OK",.  
+0005e450: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005e460: 2272 6573 756c 7422 3a20 7b0a 2020 2020  "result": {.    
+0005e470: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005e480: 2020 2263 6174 6567 6f72 7922 3a20 2269    "category": "i
+0005e490: 6e76 6572 7365 222c 0a20 2020 2020 2020  nverse",.       
+0005e4a0: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
+0005e4b0: 6c69 7374 223a 205b 0a20 2020 2020 2020  list": [.       
+0005e4c0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0005e4d0: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
+0005e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005e4f0: 2020 2022 6964 223a 2031 2c0a 2020 2020     "id": 1,.    
+0005e500: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005e510: 2020 2020 2020 2020 2020 2273 796d 626f            "symbo
+0005e520: 6c22 3a20 2242 5443 5553 4422 2c0a 2020  l": "BTCUSD",.  
+0005e530: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005e540: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
+0005e550: 6b4c 696d 6974 5661 6c75 6522 3a20 2231  kLimitValue": "1
+0005e560: 3530 222c 0a20 2020 2020 2020 2023 2020  50",.        #  
+0005e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005e580: 2020 2022 6d61 696e 7465 6e61 6e63 654d     "maintenanceM
+0005e590: 6172 6769 6e22 3a20 2230 2e35 222c 0a20  argin": "0.5",. 
+0005e5a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005e5b0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+0005e5c0: 6974 6961 6c4d 6172 6769 6e22 3a20 2231  itialMargin": "1
+0005e5d0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0005e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005e5f0: 2022 6973 4c6f 7765 7374 5269 736b 223a   "isLowestRisk":
+0005e600: 2031 2c0a 2020 2020 2020 2020 2320 2020   1,.        #   
+0005e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005e620: 2020 226d 6178 4c65 7665 7261 6765 223a    "maxLeverage":
+0005e630: 2022 3130 302e 3030 220a 2020 2020 2020   "100.00".      
+0005e640: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0005e650: 2020 2020 7d2c 0a20 2020 2020 2020 2023      },.        #
+0005e660: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
+0005e670: 2e0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0005e680: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0005e690: 2020 2320 2020 2020 2020 2020 7d2c 0a20    #         },. 
+0005e6a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005e6b0: 2022 7265 7445 7874 496e 666f 223a 207b   "retExtInfo": {
+0005e6c0: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
+0005e6d0: 2020 2020 2022 7469 6d65 223a 2031 3637       "time": 167
+0005e6e0: 3230 3534 3438 3830 3130 0a20 2020 2020  2054488010.     
+0005e6f0: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
+0005e700: 2020 2023 0a20 2020 2020 2020 2072 6573     #.        res
+0005e710: 756c 7420 3d20 7365 6c66 2e73 6166 655f  ult = self.safe_
+0005e720: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
+0005e730: 2772 6573 756c 7427 290a 2020 2020 2020  'result').      
+0005e740: 2020 7469 6572 7320 3d20 7365 6c66 2e73    tiers = self.s
+0005e750: 6166 655f 7661 6c75 6528 7265 7375 6c74  afe_value(result
+0005e760: 2c20 276c 6973 7427 290a 2020 2020 2020  , 'list').      
+0005e770: 2020 7265 7475 726e 2073 656c 662e 7061    return self.pa
+0005e780: 7273 655f 6d61 726b 6574 5f6c 6576 6572  rse_market_lever
+0005e790: 6167 655f 7469 6572 7328 7469 6572 732c  age_tiers(tiers,
+0005e7a0: 206d 6172 6b65 7429 0a0a 2020 2020 6173   market)..    as
+0005e7b0: 796e 6320 6465 6620 6665 7463 685f 6d61  ync def fetch_ma
+0005e7c0: 726b 6574 5f6c 6576 6572 6167 655f 7469  rket_leverage_ti
+0005e7d0: 6572 7328 7365 6c66 2c20 7379 6d62 6f6c  ers(self, symbol
+0005e7e0: 3a20 7374 722c 2070 6172 616d 733d 7b7d  : str, params={}
+0005e7f0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0005e800: 2020 2020 2020 2072 6574 7269 6576 6520         retrieve 
+0005e810: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
+0005e820: 6865 206d 6178 696d 756d 206c 6576 6572  he maximum lever
+0005e830: 6167 652c 2061 6e64 206d 6169 6e74 656e  age, and mainten
+0005e840: 616e 6365 206d 6172 6769 6e20 666f 7220  ance margin for 
+0005e850: 7472 6164 6573 206f 6620 7661 7279 696e  trades of varyin
+0005e860: 6720 7472 6164 6520 7369 7a65 7320 666f  g trade sizes fo
+0005e870: 7220 6120 7369 6e67 6c65 206d 6172 6b65  r a single marke
+0005e880: 740a 2020 2020 2020 2020 7365 6520 6874  t.        see ht
+0005e890: 7470 733a 2f2f 6279 6269 742d 6578 6368  tps://bybit-exch
+0005e8a0: 616e 6765 2e67 6974 6875 622e 696f 2f64  ange.github.io/d
+0005e8b0: 6f63 732f 7635 2f6d 6172 6b65 742f 7269  ocs/v5/market/ri
+0005e8c0: 736b 2d6c 696d 6974 0a20 2020 2020 2020  sk-limit.       
+0005e8d0: 203a 7061 7261 6d20 7374 7220 7379 6d62   :param str symb
+0005e8e0: 6f6c 3a20 756e 6966 6965 6420 6d61 726b  ol: unified mark
+0005e8f0: 6574 2073 796d 626f 6c0a 2020 2020 2020  et symbol.      
+0005e900: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
+0005e910: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
+0005e920: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
+0005e930: 746f 2074 6865 2062 7962 6974 2061 7069  to the bybit api
+0005e940: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
+0005e950: 2020 3a72 6574 7572 6e73 2064 6963 743a    :returns dict:
+0005e960: 2061 2060 6c65 7665 7261 6765 2074 6965   a `leverage tie
+0005e970: 7273 2073 7472 7563 7475 7265 203c 6874  rs structure <ht
+0005e980: 7470 733a 2f2f 646f 6373 2e63 6378 742e  tps://docs.ccxt.
+0005e990: 636f 6d2f 232f 3f69 643d 6c65 7665 7261  com/#/?id=levera
+0005e9a0: 6765 2d74 6965 7273 2d73 7472 7563 7475  ge-tiers-structu
+0005e9b0: 7265 3e60 0a20 2020 2020 2020 2022 2222  re>`.        """
+0005e9c0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+0005e9d0: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+0005e9e0: 2829 0a20 2020 2020 2020 2072 6571 7565  ().        reque
+0005e9f0: 7374 203d 207b 7d0a 2020 2020 2020 2020  st = {}.        
+0005ea00: 6d61 726b 6574 203d 204e 6f6e 650a 2020  market = None.  
+0005ea10: 2020 2020 2020 6d61 726b 6574 203d 2073        market = s
+0005ea20: 656c 662e 6d61 726b 6574 2873 796d 626f  elf.market(symbo
+0005ea30: 6c29 0a20 2020 2020 2020 2069 6620 6d61  l).        if ma
+0005ea40: 726b 6574 5b27 7370 6f74 275d 206f 7220  rket['spot'] or 
+0005ea50: 6d61 726b 6574 5b27 6f70 7469 6f6e 275d  market['option']
+0005ea60: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0005ea70: 6973 6520 4261 6452 6571 7565 7374 2873  ise BadRequest(s
+0005ea80: 656c 662e 6964 202b 2027 2066 6574 6368  elf.id + ' fetch
+0005ea90: 4d61 726b 6574 4c65 7665 7261 6765 5469  MarketLeverageTi
+0005eaa0: 6572 7328 2920 7379 6d62 6f6c 2064 6f65  ers() symbol doe
+0005eab0: 7320 6e6f 7420 7375 7070 6f72 7420 6d61  s not support ma
+0005eac0: 726b 6574 2027 202b 2073 796d 626f 6c29  rket ' + symbol)
+0005ead0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0005eae0: 5b27 7379 6d62 6f6c 275d 203d 206d 6172  ['symbol'] = mar
+0005eaf0: 6b65 745b 2769 6427 5d0a 2020 2020 2020  ket['id'].      
+0005eb00: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+0005eb10: 656c 662e 6665 7463 685f 6465 7269 7661  elf.fetch_deriva
+0005eb20: 7469 7665 735f 6d61 726b 6574 5f6c 6576  tives_market_lev
+0005eb30: 6572 6167 655f 7469 6572 7328 7379 6d62  erage_tiers(symb
+0005eb40: 6f6c 2c20 7061 7261 6d73 290a 0a20 2020  ol, params)..   
+0005eb50: 2064 6566 2070 6172 7365 5f6d 6172 6b65   def parse_marke
+0005eb60: 745f 6c65 7665 7261 6765 5f74 6965 7273  t_leverage_tiers
+0005eb70: 2873 656c 662c 2069 6e66 6f2c 206d 6172  (self, info, mar
+0005eb80: 6b65 743d 4e6f 6e65 293a 0a20 2020 2020  ket=None):.     
+0005eb90: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+0005eba0: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
+0005ebb0: 2020 2020 2020 2022 6964 223a 2031 2c0a         "id": 1,.
+0005ebc0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005ebd0: 2020 2273 796d 626f 6c22 3a20 2242 5443    "symbol": "BTC
+0005ebe0: 5553 4422 2c0a 2020 2020 2020 2020 2320  USD",.        # 
+0005ebf0: 2020 2020 2020 2020 2272 6973 6b4c 696d          "riskLim
+0005ec00: 6974 5661 6c75 6522 3a20 2231 3530 222c  itValue": "150",
+0005ec10: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005ec20: 2020 2022 6d61 696e 7465 6e61 6e63 654d     "maintenanceM
+0005ec30: 6172 6769 6e22 3a20 2230 2e35 222c 0a20  argin": "0.5",. 
+0005ec40: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005ec50: 2022 696e 6974 6961 6c4d 6172 6769 6e22   "initialMargin"
+0005ec60: 3a20 2231 222c 0a20 2020 2020 2020 2023  : "1",.        #
+0005ec70: 2020 2020 2020 2020 2022 6973 4c6f 7765           "isLowe
+0005ec80: 7374 5269 736b 223a 2031 2c0a 2020 2020  stRisk": 1,.    
+0005ec90: 2020 2020 2320 2020 2020 2020 2020 226d      #         "m
+0005eca0: 6178 4c65 7665 7261 6765 223a 2022 3130  axLeverage": "10
+0005ecb0: 302e 3030 220a 2020 2020 2020 2020 2320  0.00".        # 
+0005ecc0: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
+0005ecd0: 2020 2020 2020 2020 6d69 6e4e 6f74 696f          minNotio
+0005ece0: 6e61 6c20 3d20 300a 2020 2020 2020 2020  nal = 0.        
+0005ecf0: 7469 6572 7320 3d20 5b5d 0a20 2020 2020  tiers = [].     
+0005ed00: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0005ed10: 6528 302c 206c 656e 2869 6e66 6f29 293a  e(0, len(info)):
+0005ed20: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
+0005ed30: 6d20 3d20 696e 666f 5b69 5d0a 2020 2020  m = info[i].    
+0005ed40: 2020 2020 2020 2020 6d61 784e 6f74 696f          maxNotio
+0005ed50: 6e61 6c20 3d20 7365 6c66 2e73 6166 655f  nal = self.safe_
+0005ed60: 6e75 6d62 6572 2869 7465 6d2c 2027 7269  number(item, 'ri
+0005ed70: 736b 4c69 6d69 7456 616c 7565 2729 0a20  skLimitValue'). 
+0005ed80: 2020 2020 2020 2020 2020 2074 6965 7273             tiers
+0005ed90: 2e61 7070 656e 6428 7b0a 2020 2020 2020  .append({.      
+0005eda0: 2020 2020 2020 2020 2020 2774 6965 7227            'tier'
+0005edb0: 3a20 7365 6c66 2e73 756d 2869 2c20 3129  : self.sum(i, 1)
+0005edc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0005edd0: 2020 2763 7572 7265 6e63 7927 3a20 6d61    'currency': ma
+0005ede0: 726b 6574 5b27 6261 7365 275d 2c0a 2020  rket['base'],.  
+0005edf0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+0005ee00: 696e 4e6f 7469 6f6e 616c 273a 206d 696e  inNotional': min
+0005ee10: 4e6f 7469 6f6e 616c 2c0a 2020 2020 2020  Notional,.      
+0005ee20: 2020 2020 2020 2020 2020 276d 6178 4e6f            'maxNo
+0005ee30: 7469 6f6e 616c 273a 206d 6178 4e6f 7469  tional': maxNoti
+0005ee40: 6f6e 616c 2c0a 2020 2020 2020 2020 2020  onal,.          
+0005ee50: 2020 2020 2020 276d 6169 6e74 656e 616e        'maintenan
+0005ee60: 6365 4d61 7267 696e 5261 7465 273a 2073  ceMarginRate': s
+0005ee70: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
+0005ee80: 6974 656d 2c20 276d 6169 6e74 656e 616e  item, 'maintenan
+0005ee90: 6365 4d61 7267 696e 2729 2c0a 2020 2020  ceMargin'),.    
+0005eea0: 2020 2020 2020 2020 2020 2020 276d 6178              'max
+0005eeb0: 4c65 7665 7261 6765 273a 2073 656c 662e  Leverage': self.
+0005eec0: 7361 6665 5f6e 756d 6265 7228 6974 656d  safe_number(item
+0005eed0: 2c20 276d 6178 4c65 7665 7261 6765 2729  , 'maxLeverage')
+0005eee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0005eef0: 2020 2769 6e66 6f27 3a20 6974 656d 2c0a    'info': item,.
+0005ef00: 2020 2020 2020 2020 2020 2020 7d29 0a20              }). 
+0005ef10: 2020 2020 2020 2020 2020 206d 696e 4e6f             minNo
+0005ef20: 7469 6f6e 616c 203d 206d 6178 4e6f 7469  tional = maxNoti
+0005ef30: 6f6e 616c 0a20 2020 2020 2020 2072 6574  onal.        ret
+0005ef40: 7572 6e20 7469 6572 730a 0a20 2020 2064  urn tiers..    d
+0005ef50: 6566 2070 6172 7365 5f74 7261 6469 6e67  ef parse_trading
+0005ef60: 5f66 6565 2873 656c 662c 2066 6565 2c20  _fee(self, fee, 
+0005ef70: 6d61 726b 6574 3d4e 6f6e 6529 3a0a 2020  market=None):.  
+0005ef80: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+0005ef90: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
+0005efa0: 2320 2020 2020 2020 2020 2273 796d 626f  #         "symbo
+0005efb0: 6c22 3a20 2245 5448 5553 4454 222c 0a20  l": "ETHUSDT",. 
+0005efc0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005efd0: 2022 6d61 6b65 7246 6565 5261 7465 223a   "makerFeeRate":
+0005efe0: 2030 2e30 3031 2c0a 2020 2020 2020 2020   0.001,.        
+0005eff0: 2320 2020 2020 2020 2020 2274 616b 6572  #         "taker
+0005f000: 4665 6552 6174 6522 3a20 302e 3030 310a  FeeRate": 0.001.
+0005f010: 2020 2020 2020 2020 2320 2020 2020 7d0a          #     }.
+0005f020: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0005f030: 2020 6d61 726b 6574 4964 203d 2073 656c    marketId = sel
+0005f040: 662e 7361 6665 5f73 7472 696e 6728 6665  f.safe_string(fe
+0005f050: 652c 2027 7379 6d62 6f6c 2729 0a20 2020  e, 'symbol').   
+0005f060: 2020 2020 2073 796d 626f 6c20 3d20 7365       symbol = se
+0005f070: 6c66 2e73 6166 655f 7379 6d62 6f6c 286d  lf.safe_symbol(m
+0005f080: 6172 6b65 7449 642c 204e 6f6e 652c 204e  arketId, None, N
+0005f090: 6f6e 652c 2027 636f 6e74 7261 6374 2729  one, 'contract')
+0005f0a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0005f0b0: 7b0a 2020 2020 2020 2020 2020 2020 2769  {.            'i
+0005f0c0: 6e66 6f27 3a20 6665 652c 0a20 2020 2020  nfo': fee,.     
+0005f0d0: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
+0005f0e0: 2073 796d 626f 6c2c 0a20 2020 2020 2020   symbol,.       
+0005f0f0: 2020 2020 2027 6d61 6b65 7227 3a20 7365       'maker': se
+0005f100: 6c66 2e73 6166 655f 6e75 6d62 6572 2866  lf.safe_number(f
+0005f110: 6565 2c20 276d 616b 6572 4665 6552 6174  ee, 'makerFeeRat
+0005f120: 6527 292c 0a20 2020 2020 2020 2020 2020  e'),.           
+0005f130: 2027 7461 6b65 7227 3a20 7365 6c66 2e73   'taker': self.s
+0005f140: 6166 655f 6e75 6d62 6572 2866 6565 2c20  afe_number(fee, 
+0005f150: 2774 616b 6572 4665 6552 6174 6527 292c  'takerFeeRate'),
+0005f160: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+0005f170: 6173 796e 6320 6465 6620 6665 7463 685f  async def fetch_
+0005f180: 7472 6164 696e 675f 6665 6528 7365 6c66  trading_fee(self
+0005f190: 2c20 7379 6d62 6f6c 3a20 7374 722c 2070  , symbol: str, p
+0005f1a0: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
+0005f1b0: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+0005f1c0: 6574 6368 2074 6865 2074 7261 6469 6e67  etch the trading
+0005f1d0: 2066 6565 7320 666f 7220 6120 6d61 726b   fees for a mark
+0005f1e0: 6574 0a20 2020 2020 2020 2073 6565 2068  et.        see h
+0005f1f0: 7474 7073 3a2f 2f62 7962 6974 2d65 7863  ttps://bybit-exc
+0005f200: 6861 6e67 652e 6769 7468 7562 2e69 6f2f  hange.github.io/
+0005f210: 646f 6373 2f76 352f 6163 636f 756e 742f  docs/v5/account/
+0005f220: 6665 652d 7261 7465 0a20 2020 2020 2020  fee-rate.       
+0005f230: 203a 7061 7261 6d20 7374 7220 7379 6d62   :param str symb
+0005f240: 6f6c 3a20 756e 6966 6965 6420 6d61 726b  ol: unified mark
+0005f250: 6574 2073 796d 626f 6c0a 2020 2020 2020  et symbol.      
+0005f260: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
+0005f270: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
+0005f280: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
+0005f290: 746f 2074 6865 2062 7962 6974 2061 7069  to the bybit api
+0005f2a0: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
+0005f2b0: 2020 3a72 6574 7572 6e73 2064 6963 743a    :returns dict:
+0005f2c0: 2061 2060 6665 6520 7374 7275 6374 7572   a `fee structur
+0005f2d0: 6520 3c68 7474 7073 3a2f 2f64 6f63 732e  e <https://docs.
+0005f2e0: 6363 7874 2e63 6f6d 2f23 2f3f 6964 3d66  ccxt.com/#/?id=f
+0005f2f0: 6565 2d73 7472 7563 7475 7265 3e60 0a20  ee-structure>`. 
+0005f300: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0005f310: 2020 2061 7761 6974 2073 656c 662e 6c6f     await self.lo
+0005f320: 6164 5f6d 6172 6b65 7473 2829 0a20 2020  ad_markets().   
+0005f330: 2020 2020 206d 6172 6b65 7420 3d20 7365       market = se
+0005f340: 6c66 2e6d 6172 6b65 7428 7379 6d62 6f6c  lf.market(symbol
+0005f350: 290a 2020 2020 2020 2020 6966 206d 6172  ).        if mar
+0005f360: 6b65 745b 2773 706f 7427 5d3a 0a20 2020  ket['spot']:.   
+0005f370: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+0005f380: 6f74 5375 7070 6f72 7465 6428 7365 6c66  otSupported(self
+0005f390: 2e69 6420 2b20 2720 6665 7463 6854 7261  .id + ' fetchTra
+0005f3a0: 6469 6e67 4665 6528 2920 6973 206e 6f74  dingFee() is not
+0005f3b0: 2073 7570 706f 7274 6564 2066 6f72 2073   supported for s
+0005f3c0: 706f 7420 6d61 726b 6574 2729 0a20 2020  pot market').   
+0005f3d0: 2020 2020 2072 6571 7565 7374 203d 207b       request = {
+0005f3e0: 0a20 2020 2020 2020 2020 2020 2027 7379  .            'sy
+0005f3f0: 6d62 6f6c 273a 206d 6172 6b65 745b 2769  mbol': market['i
+0005f400: 6427 5d2c 0a20 2020 2020 2020 207d 0a20  d'],.        }. 
+0005f410: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0005f420: 3d20 6177 6169 7420 7365 6c66 2e70 7269  = await self.pri
+0005f430: 7661 7465 4765 7456 3541 6363 6f75 6e74  vateGetV5Account
+0005f440: 4665 6552 6174 6528 7365 6c66 2e65 7874  FeeRate(self.ext
+0005f450: 656e 6428 7265 7175 6573 742c 2070 6172  end(request, par
+0005f460: 616d 7329 290a 2020 2020 2020 2020 230a  ams)).        #.
+0005f470: 2020 2020 2020 2020 2320 2020 2020 7b0a          #     {.
+0005f480: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005f490: 2020 2272 6574 436f 6465 223a 2030 2c0a    "retCode": 0,.
+0005f4a0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005f4b0: 2020 2272 6574 4d73 6722 3a20 224f 4b22    "retMsg": "OK"
+0005f4c0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005f4d0: 2020 2020 2272 6573 756c 7422 3a20 7b0a      "result": {.
+0005f4e0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005f4f0: 2020 2020 2020 226c 6973 7422 3a20 5b0a        "list": [.
+0005f500: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005f510: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+0005f520: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005f530: 2020 2020 2020 2020 2020 2273 796d 626f            "symbo
+0005f540: 6c22 3a20 2245 5448 5553 4454 222c 0a20  l": "ETHUSDT",. 
+0005f550: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005f560: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
+0005f570: 6b65 7246 6565 5261 7465 223a 2022 302e  kerFeeRate": "0.
+0005f580: 3030 3036 222c 0a20 2020 2020 2020 2023  0006",.        #
+0005f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005f5a0: 2020 2020 2022 6d61 6b65 7246 6565 5261       "makerFeeRa
+0005f5b0: 7465 223a 2022 302e 3030 3031 220a 2020  te": "0.0001".  
+0005f5c0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005f5d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0005f5e0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0005f5f0: 5d0a 2020 2020 2020 2020 2320 2020 2020  ].        #     
+0005f600: 2020 2020 7d2c 0a20 2020 2020 2020 2023      },.        #
+0005f610: 2020 2020 2020 2020 2022 7265 7445 7874           "retExt
+0005f620: 496e 666f 223a 207b 7d2c 0a20 2020 2020  Info": {},.     
+0005f630: 2020 2023 2020 2020 2020 2020 2022 7469     #         "ti
+0005f640: 6d65 223a 2031 3637 3633 3630 3431 3235  me": 16763604125
+0005f650: 3736 0a20 2020 2020 2020 2023 2020 2020  76.        #    
+0005f660: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
+0005f670: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+0005f680: 6c66 2e73 6166 655f 7661 6c75 6528 7265  lf.safe_value(re
+0005f690: 7370 6f6e 7365 2c20 2772 6573 756c 7427  sponse, 'result'
+0005f6a0: 2c20 7b7d 290a 2020 2020 2020 2020 6665  , {}).        fe
+0005f6b0: 6573 203d 2073 656c 662e 7361 6665 5f76  es = self.safe_v
+0005f6c0: 616c 7565 2872 6573 756c 742c 2027 6c69  alue(result, 'li
+0005f6d0: 7374 272c 205b 5d29 0a20 2020 2020 2020  st', []).       
+0005f6e0: 2066 6972 7374 203d 2073 656c 662e 7361   first = self.sa
+0005f6f0: 6665 5f76 616c 7565 2866 6565 732c 2030  fe_value(fees, 0
+0005f700: 2c20 7b7d 290a 2020 2020 2020 2020 7265  , {}).        re
+0005f710: 7475 726e 2073 656c 662e 7061 7273 655f  turn self.parse_
+0005f720: 7472 6164 696e 675f 6665 6528 6669 7273  trading_fee(firs
+0005f730: 7429 0a0a 2020 2020 6173 796e 6320 6465  t)..    async de
+0005f740: 6620 6665 7463 685f 7472 6164 696e 675f  f fetch_trading_
+0005f750: 6665 6573 2873 656c 662c 2070 6172 616d  fees(self, param
+0005f760: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
+0005f770: 2222 0a20 2020 2020 2020 2066 6574 6368  "".        fetch
+0005f780: 2074 6865 2074 7261 6469 6e67 2066 6565   the trading fee
+0005f790: 7320 666f 7220 6d75 6c74 6970 6c65 206d  s for multiple m
+0005f7a0: 6172 6b65 7473 0a20 2020 2020 2020 2073  arkets.        s
+0005f7b0: 6565 2068 7474 7073 3a2f 2f62 7962 6974  ee https://bybit
+0005f7c0: 2d65 7863 6861 6e67 652e 6769 7468 7562  -exchange.github
+0005f7d0: 2e69 6f2f 646f 6373 2f76 352f 6163 636f  .io/docs/v5/acco
+0005f7e0: 756e 742f 6665 652d 7261 7465 0a20 2020  unt/fee-rate.   
+0005f7f0: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
+0005f800: 2070 6172 616d 733a 2065 7874 7261 2070   params: extra p
+0005f810: 6172 616d 6574 6572 7320 7370 6563 6966  arameters specif
+0005f820: 6963 2074 6f20 7468 6520 6279 6269 7420  ic to the bybit 
+0005f830: 6170 6920 656e 6470 6f69 6e74 0a20 2020  api endpoint.   
+0005f840: 2020 2020 203a 7265 7475 726e 7320 6469       :returns di
+0005f850: 6374 3a20 6120 6469 6374 696f 6e61 7279  ct: a dictionary
+0005f860: 206f 6620 6066 6565 2073 7472 7563 7475   of `fee structu
+0005f870: 7265 7320 3c68 7474 7073 3a2f 2f64 6f63  res <https://doc
+0005f880: 732e 6363 7874 2e63 6f6d 2f23 2f3f 6964  s.ccxt.com/#/?id
+0005f890: 3d66 6565 2d73 7472 7563 7475 7265 3e60  =fee-structure>`
+0005f8a0: 2069 6e64 6578 6564 2062 7920 6d61 726b   indexed by mark
+0005f8b0: 6574 2073 796d 626f 6c73 0a20 2020 2020  et symbols.     
+0005f8c0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0005f8d0: 7761 6974 2073 656c 662e 6c6f 6164 5f6d  wait self.load_m
+0005f8e0: 6172 6b65 7473 2829 0a20 2020 2020 2020  arkets().       
+0005f8f0: 2074 7970 6520 3d20 4e6f 6e65 0a20 2020   type = None.   
+0005f900: 2020 2020 2074 7970 652c 2070 6172 616d       type, param
+0005f910: 7320 3d20 7365 6c66 2e68 616e 646c 655f  s = self.handle_
+0005f920: 6f70 7469 6f6e 5f61 6e64 5f70 6172 616d  option_and_param
+0005f930: 7328 7061 7261 6d73 2c20 2766 6574 6368  s(params, 'fetch
+0005f940: 5472 6164 696e 6746 6565 7327 2c20 2774  TradingFees', 't
+0005f950: 7970 6527 2c20 2766 7574 7572 6527 290a  ype', 'future').
+0005f960: 2020 2020 2020 2020 6966 2074 7970 6520          if type 
+0005f970: 3d3d 2027 7370 6f74 273a 0a20 2020 2020  == 'spot':.     
+0005f980: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+0005f990: 5375 7070 6f72 7465 6428 7365 6c66 2e69  Supported(self.i
+0005f9a0: 6420 2b20 2720 6665 7463 6854 7261 6469  d + ' fetchTradi
+0005f9b0: 6e67 4665 6573 2829 2069 7320 6e6f 7420  ngFees() is not 
+0005f9c0: 7375 7070 6f72 7465 6420 666f 7220 7370  supported for sp
+0005f9d0: 6f74 206d 6172 6b65 7427 290a 2020 2020  ot market').    
+0005f9e0: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+0005f9f0: 7761 6974 2073 656c 662e 7072 6976 6174  wait self.privat
+0005fa00: 6547 6574 5635 4163 636f 756e 7446 6565  eGetV5AccountFee
+0005fa10: 5261 7465 2870 6172 616d 7329 0a20 2020  Rate(params).   
+0005fa20: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+0005fa30: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
+0005fa40: 2020 2020 2020 2020 2022 7265 7443 6f64           "retCod
+0005fa50: 6522 3a20 302c 0a20 2020 2020 2020 2023  e": 0,.        #
+0005fa60: 2020 2020 2020 2020 2022 7265 744d 7367           "retMsg
+0005fa70: 223a 2022 4f4b 222c 0a20 2020 2020 2020  ": "OK",.       
+0005fa80: 2023 2020 2020 2020 2020 2022 7265 7375   #         "resu
+0005fa90: 6c74 223a 207b 0a20 2020 2020 2020 2023  lt": {.        #
+0005faa0: 2020 2020 2020 2020 2020 2020 2022 6c69               "li
+0005fab0: 7374 223a 205b 0a20 2020 2020 2020 2023  st": [.        #
+0005fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fad0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0005fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005faf0: 2022 7379 6d62 6f6c 223a 2022 4554 4855   "symbol": "ETHU
+0005fb00: 5344 5422 2c0a 2020 2020 2020 2020 2320  SDT",.        # 
+0005fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fb20: 2020 2020 2274 616b 6572 4665 6552 6174      "takerFeeRat
+0005fb30: 6522 3a20 2230 2e30 3030 3622 2c0a 2020  e": "0.0006",.  
+0005fb40: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005fb50: 2020 2020 2020 2020 2020 2020 226d 616b              "mak
+0005fb60: 6572 4665 6552 6174 6522 3a20 2230 2e30  erFeeRate": "0.0
+0005fb70: 3030 3122 0a20 2020 2020 2020 2023 2020  001".        #  
+0005fb80: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0005fb90: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005fba0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+0005fbb0: 2023 2020 2020 2020 2020 207d 2c0a 2020   #         },.  
+0005fbc0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005fbd0: 2272 6574 4578 7449 6e66 6f22 3a20 7b7d  "retExtInfo": {}
+0005fbe0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005fbf0: 2020 2020 2274 696d 6522 3a20 3136 3736      "time": 1676
+0005fc00: 3336 3034 3132 3537 360a 2020 2020 2020  360412576.      
+0005fc10: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
+0005fc20: 2020 230a 2020 2020 2020 2020 6665 6573    #.        fees
+0005fc30: 203d 2073 656c 662e 7361 6665 5f76 616c   = self.safe_val
+0005fc40: 7565 2872 6573 706f 6e73 652c 2027 7265  ue(response, 're
+0005fc50: 7375 6c74 272c 207b 7d29 0a20 2020 2020  sult', {}).     
+0005fc60: 2020 2066 6565 7320 3d20 7365 6c66 2e73     fees = self.s
+0005fc70: 6166 655f 7661 6c75 6528 6665 6573 2c20  afe_value(fees, 
+0005fc80: 276c 6973 7427 2c20 5b5d 290a 2020 2020  'list', []).    
+0005fc90: 2020 2020 7265 7375 6c74 203d 207b 7d0a      result = {}.
+0005fca0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0005fcb0: 2072 616e 6765 2830 2c20 6c65 6e28 6665   range(0, len(fe
+0005fcc0: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+0005fcd0: 2020 6665 6520 3d20 7365 6c66 2e70 6172    fee = self.par
+0005fce0: 7365 5f74 7261 6469 6e67 5f66 6565 2866  se_trading_fee(f
+0005fcf0: 6565 735b 695d 290a 2020 2020 2020 2020  ees[i]).        
+0005fd00: 2020 2020 7379 6d62 6f6c 203d 2066 6565      symbol = fee
+0005fd10: 5b27 7379 6d62 6f6c 275d 0a20 2020 2020  ['symbol'].     
+0005fd20: 2020 2020 2020 2072 6573 756c 745b 7379         result[sy
+0005fd30: 6d62 6f6c 5d20 3d20 6665 650a 2020 2020  mbol] = fee.    
+0005fd40: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0005fd50: 740a 0a20 2020 2064 6566 2073 6967 6e28  t..    def sign(
+0005fd60: 7365 6c66 2c20 7061 7468 2c20 6170 693d  self, path, api=
+0005fd70: 2770 7562 6c69 6327 2c20 6d65 7468 6f64  'public', method
+0005fd80: 3d27 4745 5427 2c20 7061 7261 6d73 3d7b  ='GET', params={
+0005fd90: 7d2c 2068 6561 6465 7273 3d4e 6f6e 652c  }, headers=None,
+0005fda0: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+0005fdb0: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
+0005fdc0: 696d 706c 6f64 655f 686f 7374 6e61 6d65  implode_hostname
+0005fdd0: 2873 656c 662e 7572 6c73 5b27 6170 6927  (self.urls['api'
+0005fde0: 5d5b 6170 695d 2920 2b20 272f 2720 2b20  ][api]) + '/' + 
+0005fdf0: 7061 7468 0a20 2020 2020 2020 2069 6620  path.        if 
+0005fe00: 6170 6920 3d3d 2027 7075 626c 6963 273a  api == 'public':
+0005fe10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0005fe20: 7061 7261 6d73 3a0a 2020 2020 2020 2020  params:.        
+0005fe30: 2020 2020 2020 2020 7572 6c20 2b3d 2027          url += '
+0005fe40: 3f27 202b 2073 656c 662e 7261 7765 6e63  ?' + self.rawenc
+0005fe50: 6f64 6528 7061 7261 6d73 290a 2020 2020  ode(params).    
+0005fe60: 2020 2020 656c 6966 2061 7069 203d 3d20      elif api == 
+0005fe70: 2770 7269 7661 7465 273a 0a20 2020 2020  'private':.     
+0005fe80: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+0005fe90: 6b5f 7265 7175 6972 6564 5f63 7265 6465  k_required_crede
+0005fea0: 6e74 6961 6c73 2829 0a20 2020 2020 2020  ntials().       
+0005feb0: 2020 2020 2069 734f 7065 6e61 7069 203d       isOpenapi =
+0005fec0: 2075 726c 2e66 696e 6428 276f 7065 6e61   url.find('opena
+0005fed0: 7069 2729 203e 3d20 300a 2020 2020 2020  pi') >= 0.      
+0005fee0: 2020 2020 2020 6973 5633 556e 6966 6965        isV3Unifie
+0005fef0: 644d 6172 6769 6e20 3d20 7572 6c2e 6669  dMargin = url.fi
+0005ff00: 6e64 2827 756e 6966 6965 642f 7633 2729  nd('unified/v3')
+0005ff10: 203e 3d20 300a 2020 2020 2020 2020 2020   >= 0.          
+0005ff20: 2020 6973 5633 436f 6e74 7261 6374 203d    isV3Contract =
+0005ff30: 2075 726c 2e66 696e 6428 2763 6f6e 7472   url.find('contr
+0005ff40: 6163 742f 7633 2729 203e 3d20 300a 2020  act/v3') >= 0.  
+0005ff50: 2020 2020 2020 2020 2020 6973 5635 556e            isV5Un
+0005ff60: 6966 6965 6441 6363 6f75 6e74 203d 2075  ifiedAccount = u
+0005ff70: 726c 2e66 696e 6428 2776 3527 2920 3e3d  rl.find('v5') >=
+0005ff80: 2030 0a20 2020 2020 2020 2020 2020 2074   0.            t
+0005ff90: 696d 6573 7461 6d70 203d 2073 7472 2873  imestamp = str(s
+0005ffa0: 656c 662e 6e6f 6e63 6528 2929 0a20 2020  elf.nonce()).   
+0005ffb0: 2020 2020 2020 2020 2069 6620 6973 4f70           if isOp
+0005ffc0: 656e 6170 693a 0a20 2020 2020 2020 2020  enapi:.         
+0005ffd0: 2020 2020 2020 2069 6620 7061 7261 6d73         if params
+0005ffe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0005fff0: 2020 2020 2020 626f 6479 203d 2073 656c        body = sel
+00060000: 662e 6a73 6f6e 2870 6172 616d 7329 0a20  f.json(params). 
+00060010: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00060020: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00060030: 2020 2020 2020 2020 2023 2073 656c 6620           # self 
+00060040: 6669 7820 666f 7220 5048 5020 6973 2072  fix for PHP is r
+00060050: 6571 7569 7265 6420 6f74 6865 7277 6973  equired otherwis
+00060060: 6520 6974 2067 656e 6572 6174 6573 0a20  e it generates. 
+00060070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060080: 2020 2023 2027 5b5d 2720 6f6e 2065 6d70     # '[]' on emp
+00060090: 7479 2061 7272 6179 7320 6576 656e 2077  ty arrays even w
+000600a0: 6865 6e20 666f 7263 6564 2074 6f20 7573  hen forced to us
+000600b0: 6520 6f62 6a65 6374 730a 2020 2020 2020  e objects.      
+000600c0: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+000600d0: 6479 203d 2027 7b7d 270a 2020 2020 2020  dy = '{}'.      
+000600e0: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
+000600f0: 6420 3d20 7469 6d65 7374 616d 7020 2b20  d = timestamp + 
+00060100: 7365 6c66 2e61 7069 4b65 7920 2b20 626f  self.apiKey + bo
+00060110: 6479 0a20 2020 2020 2020 2020 2020 2020  dy.             
+00060120: 2020 2073 6967 6e61 7475 7265 203d 2073     signature = s
+00060130: 656c 662e 686d 6163 2873 656c 662e 656e  elf.hmac(self.en
+00060140: 636f 6465 2870 6179 6c6f 6164 292c 2073  code(payload), s
+00060150: 656c 662e 656e 636f 6465 2873 656c 662e  elf.encode(self.
+00060160: 7365 6372 6574 292c 2068 6173 686c 6962  secret), hashlib
+00060170: 2e73 6861 3235 362c 2027 6865 7827 290a  .sha256, 'hex').
+00060180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060190: 6865 6164 6572 7320 3d20 7b0a 2020 2020  headers = {.    
+000601a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000601b0: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
+000601c0: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
+000601d0: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
+000601e0: 2020 2020 2020 2020 2758 2d42 4150 492d          'X-BAPI-
+000601f0: 4150 492d 4b45 5927 3a20 7365 6c66 2e61  API-KEY': self.a
+00060200: 7069 4b65 792c 0a20 2020 2020 2020 2020  piKey,.         
+00060210: 2020 2020 2020 2020 2020 2027 582d 4241             'X-BA
+00060220: 5049 2d54 494d 4553 5441 4d50 273a 2074  PI-TIMESTAMP': t
+00060230: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
+00060240: 2020 2020 2020 2020 2020 2020 2020 2758                'X
+00060250: 2d42 4150 492d 5349 474e 273a 2073 6967  -BAPI-SIGN': sig
+00060260: 6e61 7475 7265 2c0a 2020 2020 2020 2020  nature,.        
+00060270: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00060280: 2020 2020 2020 656c 6966 2069 7356 3355        elif isV3U
+00060290: 6e69 6669 6564 4d61 7267 696e 206f 7220  nifiedMargin or 
+000602a0: 6973 5633 436f 6e74 7261 6374 206f 7220  isV3Contract or 
+000602b0: 6973 5635 556e 6966 6965 6441 6363 6f75  isV5UnifiedAccou
+000602c0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+000602d0: 2020 2020 6865 6164 6572 7320 3d20 7b0a      headers = {.
+000602e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000602f0: 2020 2020 2743 6f6e 7465 6e74 2d54 7970      'Content-Typ
+00060300: 6527 3a20 2761 7070 6c69 6361 7469 6f6e  e': 'application
+00060310: 2f6a 736f 6e27 2c0a 2020 2020 2020 2020  /json',.        
+00060320: 2020 2020 2020 2020 2020 2020 2758 2d42              'X-B
+00060330: 4150 492d 4150 492d 4b45 5927 3a20 7365  API-API-KEY': se
+00060340: 6c66 2e61 7069 4b65 792c 0a20 2020 2020  lf.apiKey,.     
+00060350: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00060360: 582d 4241 5049 2d54 494d 4553 5441 4d50  X-BAPI-TIMESTAMP
+00060370: 273a 2074 696d 6573 7461 6d70 2c0a 2020  ': timestamp,.  
+00060380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060390: 2020 2758 2d42 4150 492d 5245 4356 2d57    'X-BAPI-RECV-W
+000603a0: 494e 444f 5727 3a20 7374 7228 7365 6c66  INDOW': str(self
+000603b0: 2e6f 7074 696f 6e73 5b27 7265 6376 5769  .options['recvWi
+000603c0: 6e64 6f77 275d 292c 0a20 2020 2020 2020  ndow']),.       
+000603d0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000603e0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000603f0: 5633 556e 6966 6965 644d 6172 6769 6e20  V3UnifiedMargin 
+00060400: 6f72 2069 7356 3343 6f6e 7472 6163 743a  or isV3Contract:
+00060410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00060420: 2020 2020 2068 6561 6465 7273 5b27 582d       headers['X-
+00060430: 4241 5049 2d53 4947 4e2d 5459 5045 275d  BAPI-SIGN-TYPE']
+00060440: 203d 2027 3227 0a20 2020 2020 2020 2020   = '2'.         
+00060450: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
+00060460: 656c 662e 6578 7465 6e64 287b 7d2c 2070  elf.extend({}, p
+00060470: 6172 616d 7329 0a20 2020 2020 2020 2020  arams).         
+00060480: 2020 2020 2020 2071 7565 7279 456e 636f         queryEnco
+00060490: 6465 6420 3d20 7365 6c66 2e72 6177 656e  ded = self.rawen
+000604a0: 636f 6465 2871 7565 7279 290a 2020 2020  code(query).    
+000604b0: 2020 2020 2020 2020 2020 2020 6175 7468              auth
+000604c0: 5f62 6173 6520 3d20 7374 7228 7469 6d65  _base = str(time
+000604d0: 7374 616d 7029 202b 2073 656c 662e 6170  stamp) + self.ap
+000604e0: 694b 6579 202b 2073 7472 2873 656c 662e  iKey + str(self.
+000604f0: 6f70 7469 6f6e 735b 2772 6563 7657 696e  options['recvWin
+00060500: 646f 7727 5d29 0a20 2020 2020 2020 2020  dow']).         
+00060510: 2020 2020 2020 2061 7574 6846 756c 6c20         authFull 
+00060520: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00060530: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+00060540: 203d 3d20 2750 4f53 5427 3a0a 2020 2020   == 'POST':.    
+00060550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060560: 626f 6479 203d 2073 656c 662e 6a73 6f6e  body = self.json
+00060570: 2871 7565 7279 290a 2020 2020 2020 2020  (query).        
+00060580: 2020 2020 2020 2020 2020 2020 6175 7468              auth
+00060590: 4675 6c6c 203d 2061 7574 685f 6261 7365  Full = auth_base
+000605a0: 202b 2062 6f64 790a 2020 2020 2020 2020   + body.        
+000605b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000605c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000605d0: 2020 6175 7468 4675 6c6c 203d 2061 7574    authFull = aut
+000605e0: 685f 6261 7365 202b 2071 7565 7279 456e  h_base + queryEn
+000605f0: 636f 6465 640a 2020 2020 2020 2020 2020  coded.          
+00060600: 2020 2020 2020 2020 2020 7572 6c20 2b3d            url +=
+00060610: 2027 3f27 202b 2073 656c 662e 7261 7765   '?' + self.rawe
+00060620: 6e63 6f64 6528 7175 6572 7929 0a20 2020  ncode(query).   
+00060630: 2020 2020 2020 2020 2020 2020 2073 6967               sig
+00060640: 6e61 7475 7265 203d 204e 6f6e 650a 2020  nature = None.  
+00060650: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00060660: 2073 656c 662e 7365 6372 6574 2e66 696e   self.secret.fin
+00060670: 6428 2750 5249 5641 5445 204b 4559 2729  d('PRIVATE KEY')
+00060680: 203e 202d 313a 0a20 2020 2020 2020 2020   > -1:.         
+00060690: 2020 2020 2020 2020 2020 2073 6967 6e61             signa
+000606a0: 7475 7265 203d 2073 656c 662e 7273 6128  ture = self.rsa(
+000606b0: 6175 7468 4675 6c6c 2c20 7365 6c66 2e73  authFull, self.s
+000606c0: 6563 7265 742c 2027 7368 6132 3536 2729  ecret, 'sha256')
 000606d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000606e0: 2020 2020 2027 6170 695f 6b65 7927 3a20       'api_key': 
-000606f0: 7365 6c66 2e61 7069 4b65 792c 0a20 2020  self.apiKey,.   
-00060700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060710: 2027 7265 6376 5f77 696e 646f 7727 3a20   'recv_window': 
-00060720: 7365 6c66 2e6f 7074 696f 6e73 5b27 7265  self.options['re
-00060730: 6376 5769 6e64 6f77 275d 2c0a 2020 2020  cvWindow'],.    
-00060740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060750: 2774 696d 6573 7461 6d70 273a 2074 696d  'timestamp': tim
-00060760: 6573 7461 6d70 2c0a 2020 2020 2020 2020  estamp,.        
-00060770: 2020 2020 2020 2020 7d29 0a20 2020 2020          }).     
-00060780: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00060790: 6451 7565 7279 203d 2073 656c 662e 6b65  dQuery = self.ke
-000607a0: 7973 6f72 7428 7175 6572 7929 0a20 2020  ysort(query).   
-000607b0: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-000607c0: 6820 3d20 7365 6c66 2e72 6177 656e 636f  h = self.rawenco
-000607d0: 6465 2873 6f72 7465 6451 7565 7279 290a  de(sortedQuery).
-000607e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000607f0: 7369 676e 6174 7572 6520 3d20 4e6f 6e65  signature = None
-00060800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060810: 2069 6620 7365 6c66 2e73 6563 7265 742e   if self.secret.
-00060820: 6669 6e64 2827 5052 4956 4154 4520 4b45  find('PRIVATE KE
-00060830: 5927 2920 3e20 2d31 3a0a 2020 2020 2020  Y') > -1:.      
-00060840: 2020 2020 2020 2020 2020 2020 2020 7369                si
-00060850: 676e 6174 7572 6520 3d20 7365 6c66 2e72  gnature = self.r
-00060860: 7361 2861 7574 682c 2073 656c 662e 7365  sa(auth, self.se
-00060870: 6372 6574 2c20 2773 6861 3235 3627 290a  cret, 'sha256').
-00060880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060890: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000608a0: 2020 2020 2020 2020 2020 7369 676e 6174            signat
-000608b0: 7572 6520 3d20 7365 6c66 2e68 6d61 6328  ure = self.hmac(
-000608c0: 7365 6c66 2e65 6e63 6f64 6528 6175 7468  self.encode(auth
-000608d0: 292c 2073 656c 662e 656e 636f 6465 2873  ), self.encode(s
-000608e0: 656c 662e 7365 6372 6574 292c 2068 6173  elf.secret), has
-000608f0: 686c 6962 2e73 6861 3235 3629 0a20 2020  hlib.sha256).   
-00060900: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00060910: 6d65 7468 6f64 203d 3d20 2750 4f53 5427  method == 'POST'
-00060920: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00060930: 2020 2020 2020 6973 5370 6f74 203d 2075        isSpot = u
-00060940: 726c 2e66 696e 6428 2773 706f 7427 2920  rl.find('spot') 
-00060950: 3e3d 2030 0a20 2020 2020 2020 2020 2020  >= 0.           
-00060960: 2020 2020 2020 2020 2065 7874 656e 6465           extende
-00060970: 6451 7565 7279 203d 2073 656c 662e 6578  dQuery = self.ex
-00060980: 7465 6e64 2871 7565 7279 2c20 7b0a 2020  tend(query, {.  
-00060990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000609a0: 2020 2020 2020 2773 6967 6e27 3a20 7369        'sign': si
-000609b0: 676e 6174 7572 652c 0a20 2020 2020 2020  gnature,.       
-000609c0: 2020 2020 2020 2020 2020 2020 207d 290a               }).
-000609d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000609e0: 2020 2020 6966 2069 7353 706f 743a 0a20      if isSpot:. 
-000609f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060a00: 2020 2020 2020 2062 6f64 7920 3d20 7365         body = se
-00060a10: 6c66 2e75 726c 656e 636f 6465 2865 7874  lf.urlencode(ext
-00060a20: 656e 6465 6451 7565 7279 290a 2020 2020  endedQuery).    
-00060a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060a40: 2020 2020 6865 6164 6572 7320 3d20 7b0a      headers = {.
-00060a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060a60: 2020 2020 2020 2020 2020 2020 2743 6f6e              'Con
-00060a70: 7465 6e74 2d54 7970 6527 3a20 2761 7070  tent-Type': 'app
-00060a80: 6c69 6361 7469 6f6e 2f78 2d77 7777 2d66  lication/x-www-f
-00060a90: 6f72 6d2d 7572 6c65 6e63 6f64 6564 272c  orm-urlencoded',
-00060aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060ab0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00060ac0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00060ad0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00060ae0: 2020 2020 2020 2020 2020 2020 2062 6f64               bod
-00060af0: 7920 3d20 7365 6c66 2e6a 736f 6e28 6578  y = self.json(ex
-00060b00: 7465 6e64 6564 5175 6572 7929 0a20 2020  tendedQuery).   
-00060b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060b20: 2020 2020 2068 6561 6465 7273 203d 207b       headers = {
-00060b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060b40: 2020 2020 2020 2020 2020 2020 2027 436f               'Co
-00060b50: 6e74 656e 742d 5479 7065 273a 2027 6170  ntent-Type': 'ap
-00060b60: 706c 6963 6174 696f 6e2f 6a73 6f6e 272c  plication/json',
-00060b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060b80: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00060b90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00060ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060bb0: 2020 2020 2075 726c 202b 3d20 273f 2720       url += '?' 
-00060bc0: 2b20 7365 6c66 2e72 6177 656e 636f 6465  + self.rawencode
-00060bd0: 2873 6f72 7465 6451 7565 7279 290a 2020  (sortedQuery).  
-00060be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060bf0: 2020 7572 6c20 2b3d 2027 2673 6967 6e3d    url += '&sign=
-00060c00: 2720 2b20 7369 676e 6174 7572 650a 2020  ' + signature.  
-00060c10: 2020 2020 2020 6966 206d 6574 686f 6420        if method 
-00060c20: 3d3d 2027 504f 5354 273a 0a20 2020 2020  == 'POST':.     
-00060c30: 2020 2020 2020 2062 726f 6b65 7249 6420         brokerId 
-00060c40: 3d20 7365 6c66 2e73 6166 655f 7374 7269  = self.safe_stri
-00060c50: 6e67 2873 656c 662e 6f70 7469 6f6e 732c  ng(self.options,
-00060c60: 2027 6272 6f6b 6572 4964 2729 0a20 2020   'brokerId').   
-00060c70: 2020 2020 2020 2020 2069 6620 6272 6f6b           if brok
-00060c80: 6572 4964 2069 7320 6e6f 7420 4e6f 6e65  erId is not None
-00060c90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00060ca0: 2020 6865 6164 6572 735b 2752 6566 6572    headers['Refer
-00060cb0: 6572 275d 203d 2062 726f 6b65 7249 640a  er'] = brokerId.
-00060cc0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-00060cd0: 2775 726c 273a 2075 726c 2c20 276d 6574  'url': url, 'met
-00060ce0: 686f 6427 3a20 6d65 7468 6f64 2c20 2762  hod': method, 'b
-00060cf0: 6f64 7927 3a20 626f 6479 2c20 2768 6561  ody': body, 'hea
-00060d00: 6465 7273 273a 2068 6561 6465 7273 7d0a  ders': headers}.
-00060d10: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-00060d20: 6572 726f 7273 2873 656c 662c 2068 7474  errors(self, htt
-00060d30: 7043 6f64 652c 2072 6561 736f 6e2c 2075  pCode, reason, u
-00060d40: 726c 2c20 6d65 7468 6f64 2c20 6865 6164  rl, method, head
-00060d50: 6572 732c 2062 6f64 792c 2072 6573 706f  ers, body, respo
-00060d60: 6e73 652c 2072 6571 7565 7374 4865 6164  nse, requestHead
-00060d70: 6572 732c 2072 6571 7565 7374 426f 6479  ers, requestBody
-00060d80: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
-00060d90: 7420 7265 7370 6f6e 7365 3a0a 2020 2020  t response:.    
-00060da0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00060db0: 6f6e 6520 2023 2066 616c 6c62 6163 6b20  one  # fallback 
-00060dc0: 746f 2064 6566 6175 6c74 2065 7272 6f72  to default error
-00060dd0: 2068 616e 646c 6572 0a20 2020 2020 2020   handler.       
-00060de0: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-00060df0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-00060e00: 2020 2020 2072 6574 5f63 6f64 653a 2031       ret_code: 1
-00060e10: 3030 3031 2c0a 2020 2020 2020 2020 2320  0001,.        # 
-00060e20: 2020 2020 2020 2020 7265 745f 6d73 673a          ret_msg:
-00060e30: 2027 5265 6164 4d61 7043 423a 2065 7870   'ReadMapCB: exp
-00060e40: 6563 7420 7b6f 7220 6e2c 2062 7574 2066  ect {or n, but f
-00060e50: 6f75 6e64 205c 7530 3030 302c 2065 7272  ound \u0000, err
-00060e60: 6f72 2027 202b 0a20 2020 2020 2020 2023  or ' +.        #
-00060e70: 2020 2020 2020 2020 2027 666f 756e 6420           'found 
-00060e80: 696e 2020 2330 2062 7974 6520 6f66 202e  in  #0 byte of .
-00060e90: 2e2e 7c7c 2e2e 2e2c 2062 6967 6765 7220  ..||..., bigger 
-00060ea0: 636f 6e74 6578 7420 2720 2b0a 2020 2020  context ' +.    
-00060eb0: 2020 2020 2320 2020 2020 2020 2020 272e      #         '.
-00060ec0: 2e2e 7c7c 2e2e 2e27 2c0a 2020 2020 2020  ..||...',.      
-00060ed0: 2020 2320 2020 2020 2020 2020 6578 745f    #         ext_
-00060ee0: 636f 6465 3a20 2727 2c0a 2020 2020 2020  code: '',.      
-00060ef0: 2020 2320 2020 2020 2020 2020 6578 745f    #         ext_
-00060f00: 696e 666f 3a20 2727 2c0a 2020 2020 2020  info: '',.      
-00060f10: 2020 2320 2020 2020 2020 2020 7265 7375    #         resu
-00060f20: 6c74 3a20 6e75 6c6c 2c0a 2020 2020 2020  lt: null,.      
-00060f30: 2020 2320 2020 2020 2020 2020 7469 6d65    #         time
-00060f40: 5f6e 6f77 3a20 2731 3538 3339 3334 3130  _now: '158393410
-00060f50: 362e 3539 3034 3336 270a 2020 2020 2020  6.590436'.      
-00060f60: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
-00060f70: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
-00060f80: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-00060f90: 2020 2020 2020 2272 6574 436f 6465 223a        "retCode":
-00060fa0: 3130 3030 312c 0a20 2020 2020 2020 2023  10001,.        #
-00060fb0: 2020 2020 2020 2020 2022 7265 744d 7367           "retMsg
-00060fc0: 223a 2273 796d 626f 6c20 7061 7261 6d73  ":"symbol params
-00060fd0: 2065 7272 222c 0a20 2020 2020 2020 2023   err",.        #
-00060fe0: 2020 2020 2020 2020 2022 7265 7375 6c74           "result
-00060ff0: 223a 7b22 7379 6d62 6f6c 223a 2222 2c22  ":{"symbol":"","
-00061000: 6269 6422 3a22 222c 2262 6964 4976 223a  bid":"","bidIv":
-00061010: 2222 2c22 6269 6453 697a 6522 3a22 222c  "","bidSize":"",
-00061020: 2261 736b 223a 2222 2c22 6173 6b49 7622  "ask":"","askIv"
-00061030: 3a22 222c 2261 736b 5369 7a65 223a 2222  :"","askSize":""
-00061040: 2c22 6c61 7374 5072 6963 6522 3a22 222c  ,"lastPrice":"",
-00061050: 226f 7065 6e49 6e74 6572 6573 7422 3a22  "openInterest":"
-00061060: 222c 2269 6e64 6578 5072 6963 6522 3a22  ","indexPrice":"
-00061070: 222c 226d 6172 6b50 7269 6365 223a 2222  ","markPrice":""
-00061080: 2c22 6d61 726b 5072 6963 6549 7622 3a22  ,"markPriceIv":"
-00061090: 222c 2263 6861 6e67 6532 3468 223a 2222  ","change24h":""
-000610a0: 2c22 6869 6768 3234 6822 3a22 222c 226c  ,"high24h":"","l
-000610b0: 6f77 3234 6822 3a22 222c 2276 6f6c 756d  ow24h":"","volum
-000610c0: 6532 3468 223a 2222 2c22 7475 726e 6f76  e24h":"","turnov
-000610d0: 6572 3234 6822 3a22 222c 2274 6f74 616c  er24h":"","total
-000610e0: 566f 6c75 6d65 223a 2222 2c22 746f 7461  Volume":"","tota
-000610f0: 6c54 7572 6e6f 7665 7222 3a22 222c 2266  lTurnover":"","f
-00061100: 756e 6469 6e67 5261 7465 223a 2222 2c22  undingRate":"","
-00061110: 7072 6564 6963 7465 6446 756e 6469 6e67  predictedFunding
-00061120: 5261 7465 223a 2222 2c22 6e65 7874 4675  Rate":"","nextFu
-00061130: 6e64 696e 6754 696d 6522 3a22 222c 2263  ndingTime":"","c
-00061140: 6f75 6e74 646f 776e 486f 7572 223a 2230  ountdownHour":"0
-00061150: 222c 2270 7265 6469 6374 6564 4465 6c69  ","predictedDeli
-00061160: 7665 7279 5072 6963 6522 3a22 222c 2275  veryPrice":"","u
-00061170: 6e64 6572 6c79 696e 6750 7269 6365 223a  nderlyingPrice":
-00061180: 2222 2c22 6465 6c74 6122 3a22 222c 2267  "","delta":"","g
-00061190: 616d 6d61 223a 2222 2c22 7665 6761 223a  amma":"","vega":
-000611a0: 2222 2c22 7468 6574 6122 3a22 227d 0a20  "","theta":""}. 
-000611b0: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
-000611c0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-000611d0: 2065 7272 6f72 436f 6465 203d 2073 656c   errorCode = sel
-000611e0: 662e 7361 6665 5f73 7472 696e 675f 3228  f.safe_string_2(
-000611f0: 7265 7370 6f6e 7365 2c20 2772 6574 5f63  response, 'ret_c
-00061200: 6f64 6527 2c20 2772 6574 436f 6465 2729  ode', 'retCode')
-00061210: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
-00061220: 7243 6f64 6520 213d 2027 3027 3a0a 2020  rCode != '0':.  
-00061230: 2020 2020 2020 2020 2020 6966 2065 7272            if err
-00061240: 6f72 436f 6465 203d 3d20 2733 3030 3834  orCode == '30084
-00061250: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00061260: 2020 2023 206e 6f74 2061 6e20 6572 726f     # not an erro
-00061270: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00061280: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
-00061290: 7562 2e63 6f6d 2f63 6378 742f 6363 7874  ub.com/ccxt/ccxt
-000612a0: 2f69 7373 7565 732f 3131 3236 380a 2020  /issues/11268.  
-000612b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000612c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000612d0: 6f6d 2f63 6378 742f 6363 7874 2f70 756c  om/ccxt/ccxt/pul
-000612e0: 6c2f 3131 3632 340a 2020 2020 2020 2020  l/11624.        
-000612f0: 2020 2020 2020 2020 2320 504f 5354 2068          # POST h
-00061300: 7474 7073 3a2f 2f61 7069 2e62 7962 6974  ttps://api.bybit
-00061310: 2e63 6f6d 2f76 322f 7072 6976 6174 652f  .com/v2/private/
-00061320: 706f 7369 7469 6f6e 2f73 7769 7463 682d  position/switch-
-00061330: 6973 6f6c 6174 6564 2032 3030 204f 4b0a  isolated 200 OK.
-00061340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00061350: 2320 7b22 7265 745f 636f 6465 223a 3330  # {"ret_code":30
-00061360: 3038 342c 2272 6574 5f6d 7367 223a 2249  084,"ret_msg":"I
-00061370: 736f 6c61 7465 6420 6e6f 7420 6d6f 6469  solated not modi
-00061380: 6669 6564 222c 2265 7874 5f63 6f64 6522  fied","ext_code"
-00061390: 3a22 222c 2265 7874 5f69 6e66 6f22 3a22  :"","ext_info":"
-000613a0: 222c 2272 6573 756c 7422 3a6e 756c 6c2c  ","result":null,
-000613b0: 2274 696d 655f 6e6f 7722 3a22 3136 3432  "time_now":"1642
-000613c0: 3030 3532 3139 2e39 3337 3938 3822 2c22  005219.937988","
-000613d0: 7261 7465 5f6c 696d 6974 5f73 7461 7475  rate_limit_statu
-000613e0: 7322 3a37 332c 2272 6174 655f 6c69 6d69  s":73,"rate_limi
-000613f0: 745f 7265 7365 745f 6d73 223a 3136 3432  t_reset_ms":1642
-00061400: 3030 3532 3139 3839 342c 2272 6174 655f  005219894,"rate_
-00061410: 6c69 6d69 7422 3a37 357d 0a20 2020 2020  limit":75}.     
-00061420: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00061430: 6e20 4e6f 6e65 0a20 2020 2020 2020 2020  n None.         
-00061440: 2020 2066 6565 6462 6163 6b20 3d20 4e6f     feedback = No
-00061450: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-00061460: 6620 6572 726f 7243 6f64 6520 3d3d 2027  f errorCode == '
-00061470: 3130 3030 3527 3a0a 2020 2020 2020 2020  10005':.        
-00061480: 2020 2020 2020 2020 6665 6564 6261 636b          feedback
-00061490: 203d 2073 656c 662e 6964 202b 2027 2070   = self.id + ' p
-000614a0: 7269 7661 7465 2061 7069 2075 7365 7320  rivate api uses 
-000614b0: 2f75 7365 722f 7633 2f70 7269 7661 7465  /user/v3/private
-000614c0: 2f71 7565 7279 2d61 7069 2074 6f20 6368  /query-api to ch
-000614d0: 6563 6b20 6966 2079 6f75 2068 6176 6520  eck if you have 
-000614e0: 6120 756e 6966 6965 6420 6163 636f 756e  a unified accoun
-000614f0: 742e 2054 6865 2041 5049 206b 6579 206f  t. The API key o
-00061500: 6620 7573 6572 2069 6420 6d75 7374 206f  f user id must o
-00061510: 776e 206f 6e65 206f 6620 7065 726d 6973  wn one of permis
-00061520: 7369 6f6e 733a 2022 4163 636f 756e 7420  sions: "Account 
-00061530: 5472 616e 7366 6572 222c 2022 5375 6261  Transfer", "Suba
-00061540: 6363 6f75 6e74 2054 7261 6e73 6665 7222  ccount Transfer"
-00061550: 2c20 2257 6974 6864 7261 7761 6c22 2027  , "Withdrawal" '
-00061560: 202b 2062 6f64 790a 2020 2020 2020 2020   + body.        
-00061570: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00061580: 2020 2020 2020 2020 2020 6665 6564 6261            feedba
-00061590: 636b 203d 2073 656c 662e 6964 202b 2027  ck = self.id + '
-000615a0: 2027 202b 2062 6f64 790a 2020 2020 2020   ' + body.      
-000615b0: 2020 2020 2020 7365 6c66 2e74 6872 6f77        self.throw
-000615c0: 5f62 726f 6164 6c79 5f6d 6174 6368 6564  _broadly_matched
-000615d0: 5f65 7863 6570 7469 6f6e 2873 656c 662e  _exception(self.
-000615e0: 6578 6365 7074 696f 6e73 5b27 6272 6f61  exceptions['broa
-000615f0: 6427 5d2c 2062 6f64 792c 2066 6565 6462  d'], body, feedb
-00061600: 6163 6b29 0a20 2020 2020 2020 2020 2020  ack).           
-00061610: 2073 656c 662e 7468 726f 775f 6578 6163   self.throw_exac
-00061620: 746c 795f 6d61 7463 6865 645f 6578 6365  tly_matched_exce
-00061630: 7074 696f 6e28 7365 6c66 2e65 7863 6570  ption(self.excep
-00061640: 7469 6f6e 735b 2765 7861 6374 275d 2c20  tions['exact'], 
-00061650: 6572 726f 7243 6f64 652c 2066 6565 6462  errorCode, feedb
-00061660: 6163 6b29 0a20 2020 2020 2020 2020 2020  ack).           
-00061670: 2072 6169 7365 2045 7863 6861 6e67 6545   raise ExchangeE
-00061680: 7272 6f72 2866 6565 6462 6163 6b29 2020  rror(feedback)  
-00061690: 2320 756e 6b6e 6f77 6e20 6d65 7373 6167  # unknown messag
-000616a0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-000616b0: 204e 6f6e 650a                            None.
+000606e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000606f0: 2020 2020 2020 2020 2020 2073 6967 6e61             signa
+00060700: 7475 7265 203d 2073 656c 662e 686d 6163  ture = self.hmac
+00060710: 2873 656c 662e 656e 636f 6465 2861 7574  (self.encode(aut
+00060720: 6846 756c 6c29 2c20 7365 6c66 2e65 6e63  hFull), self.enc
+00060730: 6f64 6528 7365 6c66 2e73 6563 7265 7429  ode(self.secret)
+00060740: 2c20 6861 7368 6c69 622e 7368 6132 3536  , hashlib.sha256
+00060750: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00060760: 2020 6865 6164 6572 735b 2758 2d42 4150    headers['X-BAP
+00060770: 492d 5349 474e 275d 203d 2073 6967 6e61  I-SIGN'] = signa
+00060780: 7475 7265 0a20 2020 2020 2020 2020 2020  ture.           
+00060790: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000607a0: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
+000607b0: 656c 662e 6578 7465 6e64 2870 6172 616d  elf.extend(param
+000607c0: 732c 207b 0a20 2020 2020 2020 2020 2020  s, {.           
+000607d0: 2020 2020 2020 2020 2027 6170 695f 6b65           'api_ke
+000607e0: 7927 3a20 7365 6c66 2e61 7069 4b65 792c  y': self.apiKey,
+000607f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00060800: 2020 2020 2027 7265 6376 5f77 696e 646f       'recv_windo
+00060810: 7727 3a20 7365 6c66 2e6f 7074 696f 6e73  w': self.options
+00060820: 5b27 7265 6376 5769 6e64 6f77 275d 2c0a  ['recvWindow'],.
+00060830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060840: 2020 2020 2774 696d 6573 7461 6d70 273a      'timestamp':
+00060850: 2074 696d 6573 7461 6d70 2c0a 2020 2020   timestamp,.    
+00060860: 2020 2020 2020 2020 2020 2020 7d29 0a20              }). 
+00060870: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00060880: 6f72 7465 6451 7565 7279 203d 2073 656c  ortedQuery = sel
+00060890: 662e 6b65 7973 6f72 7428 7175 6572 7929  f.keysort(query)
+000608a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000608b0: 2061 7574 6820 3d20 7365 6c66 2e72 6177   auth = self.raw
+000608c0: 656e 636f 6465 2873 6f72 7465 6451 7565  encode(sortedQue
+000608d0: 7279 290a 2020 2020 2020 2020 2020 2020  ry).            
+000608e0: 2020 2020 7369 676e 6174 7572 6520 3d20      signature = 
+000608f0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00060900: 2020 2020 2069 6620 7365 6c66 2e73 6563       if self.sec
+00060910: 7265 742e 6669 6e64 2827 5052 4956 4154  ret.find('PRIVAT
+00060920: 4520 4b45 5927 2920 3e20 2d31 3a0a 2020  E KEY') > -1:.  
+00060930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060940: 2020 7369 676e 6174 7572 6520 3d20 7365    signature = se
+00060950: 6c66 2e72 7361 2861 7574 682c 2073 656c  lf.rsa(auth, sel
+00060960: 662e 7365 6372 6574 2c20 2773 6861 3235  f.secret, 'sha25
+00060970: 3627 290a 2020 2020 2020 2020 2020 2020  6').            
+00060980: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00060990: 2020 2020 2020 2020 2020 2020 2020 7369                si
+000609a0: 676e 6174 7572 6520 3d20 7365 6c66 2e68  gnature = self.h
+000609b0: 6d61 6328 7365 6c66 2e65 6e63 6f64 6528  mac(self.encode(
+000609c0: 6175 7468 292c 2073 656c 662e 656e 636f  auth), self.enco
+000609d0: 6465 2873 656c 662e 7365 6372 6574 292c  de(self.secret),
+000609e0: 2068 6173 686c 6962 2e73 6861 3235 3629   hashlib.sha256)
+000609f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00060a00: 2069 6620 6d65 7468 6f64 203d 3d20 2750   if method == 'P
+00060a10: 4f53 5427 3a0a 2020 2020 2020 2020 2020  OST':.          
+00060a20: 2020 2020 2020 2020 2020 6973 5370 6f74            isSpot
+00060a30: 203d 2075 726c 2e66 696e 6428 2773 706f   = url.find('spo
+00060a40: 7427 2920 3e3d 2030 0a20 2020 2020 2020  t') >= 0.       
+00060a50: 2020 2020 2020 2020 2020 2020 2065 7874               ext
+00060a60: 656e 6465 6451 7565 7279 203d 2073 656c  endedQuery = sel
+00060a70: 662e 6578 7465 6e64 2871 7565 7279 2c20  f.extend(query, 
+00060a80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00060a90: 2020 2020 2020 2020 2020 2773 6967 6e27            'sign'
+00060aa0: 3a20 7369 676e 6174 7572 652c 0a20 2020  : signature,.   
+00060ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060ac0: 207d 290a 2020 2020 2020 2020 2020 2020   }).            
+00060ad0: 2020 2020 2020 2020 6966 2069 7353 706f          if isSpo
+00060ae0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00060af0: 2020 2020 2020 2020 2020 2062 6f64 7920             body 
+00060b00: 3d20 7365 6c66 2e75 726c 656e 636f 6465  = self.urlencode
+00060b10: 2865 7874 656e 6465 6451 7565 7279 290a  (extendedQuery).
+00060b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060b30: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
+00060b40: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00060b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060b60: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
+00060b70: 2761 7070 6c69 6361 7469 6f6e 2f78 2d77  'application/x-w
+00060b80: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
+00060b90: 6564 272c 0a20 2020 2020 2020 2020 2020  ed',.           
+00060ba0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00060bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060bc0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00060bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060be0: 2062 6f64 7920 3d20 7365 6c66 2e6a 736f   body = self.jso
+00060bf0: 6e28 6578 7465 6e64 6564 5175 6572 7929  n(extendedQuery)
+00060c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00060c10: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+00060c20: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00060c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060c40: 2027 436f 6e74 656e 742d 5479 7065 273a   'Content-Type':
+00060c50: 2027 6170 706c 6963 6174 696f 6e2f 6a73   'application/js
+00060c60: 6f6e 272c 0a20 2020 2020 2020 2020 2020  on',.           
+00060c70: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00060c80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00060c90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00060ca0: 2020 2020 2020 2020 2075 726c 202b 3d20           url += 
+00060cb0: 273f 2720 2b20 7365 6c66 2e72 6177 656e  '?' + self.rawen
+00060cc0: 636f 6465 2873 6f72 7465 6451 7565 7279  code(sortedQuery
+00060cd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00060ce0: 2020 2020 2020 7572 6c20 2b3d 2027 2673        url += '&s
+00060cf0: 6967 6e3d 2720 2b20 7369 676e 6174 7572  ign=' + signatur
+00060d00: 650a 2020 2020 2020 2020 6966 206d 6574  e.        if met
+00060d10: 686f 6420 3d3d 2027 504f 5354 273a 0a20  hod == 'POST':. 
+00060d20: 2020 2020 2020 2020 2020 2062 726f 6b65             broke
+00060d30: 7249 6420 3d20 7365 6c66 2e73 6166 655f  rId = self.safe_
+00060d40: 7374 7269 6e67 2873 656c 662e 6f70 7469  string(self.opti
+00060d50: 6f6e 732c 2027 6272 6f6b 6572 4964 2729  ons, 'brokerId')
+00060d60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00060d70: 6272 6f6b 6572 4964 2069 7320 6e6f 7420  brokerId is not 
+00060d80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00060d90: 2020 2020 2020 6865 6164 6572 735b 2752        headers['R
+00060da0: 6566 6572 6572 275d 203d 2062 726f 6b65  eferer'] = broke
+00060db0: 7249 640a 2020 2020 2020 2020 7265 7475  rId.        retu
+00060dc0: 726e 207b 2775 726c 273a 2075 726c 2c20  rn {'url': url, 
+00060dd0: 276d 6574 686f 6427 3a20 6d65 7468 6f64  'method': method
+00060de0: 2c20 2762 6f64 7927 3a20 626f 6479 2c20  , 'body': body, 
+00060df0: 2768 6561 6465 7273 273a 2068 6561 6465  'headers': heade
+00060e00: 7273 7d0a 0a20 2020 2064 6566 2068 616e  rs}..    def han
+00060e10: 646c 655f 6572 726f 7273 2873 656c 662c  dle_errors(self,
+00060e20: 2068 7474 7043 6f64 652c 2072 6561 736f   httpCode, reaso
+00060e30: 6e2c 2075 726c 2c20 6d65 7468 6f64 2c20  n, url, method, 
+00060e40: 6865 6164 6572 732c 2062 6f64 792c 2072  headers, body, r
+00060e50: 6573 706f 6e73 652c 2072 6571 7565 7374  esponse, request
+00060e60: 4865 6164 6572 732c 2072 6571 7565 7374  Headers, request
+00060e70: 426f 6479 293a 0a20 2020 2020 2020 2069  Body):.        i
+00060e80: 6620 6e6f 7420 7265 7370 6f6e 7365 3a0a  f not response:.
+00060e90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00060ea0: 726e 204e 6f6e 6520 2023 2066 616c 6c62  rn None  # fallb
+00060eb0: 6163 6b20 746f 2064 6566 6175 6c74 2065  ack to default e
+00060ec0: 7272 6f72 2068 616e 646c 6572 0a20 2020  rror handler.   
+00060ed0: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+00060ee0: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
+00060ef0: 2020 2020 2020 2020 2072 6574 5f63 6f64           ret_cod
+00060f00: 653a 2031 3030 3031 2c0a 2020 2020 2020  e: 10001,.      
+00060f10: 2020 2320 2020 2020 2020 2020 7265 745f    #         ret_
+00060f20: 6d73 673a 2027 5265 6164 4d61 7043 423a  msg: 'ReadMapCB:
+00060f30: 2065 7870 6563 7420 7b6f 7220 6e2c 2062   expect {or n, b
+00060f40: 7574 2066 6f75 6e64 205c 7530 3030 302c  ut found \u0000,
+00060f50: 2065 7272 6f72 2027 202b 0a20 2020 2020   error ' +.     
+00060f60: 2020 2023 2020 2020 2020 2020 2027 666f     #         'fo
+00060f70: 756e 6420 696e 2020 2330 2062 7974 6520  und in  #0 byte 
+00060f80: 6f66 202e 2e2e 7c7c 2e2e 2e2c 2062 6967  of ...||..., big
+00060f90: 6765 7220 636f 6e74 6578 7420 2720 2b0a  ger context ' +.
+00060fa0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00060fb0: 2020 272e 2e2e 7c7c 2e2e 2e27 2c0a 2020    '...||...',.  
+00060fc0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00060fd0: 6578 745f 636f 6465 3a20 2727 2c0a 2020  ext_code: '',.  
+00060fe0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00060ff0: 6578 745f 696e 666f 3a20 2727 2c0a 2020  ext_info: '',.  
+00061000: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00061010: 7265 7375 6c74 3a20 6e75 6c6c 2c0a 2020  result: null,.  
+00061020: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00061030: 7469 6d65 5f6e 6f77 3a20 2731 3538 3339  time_now: '15839
+00061040: 3334 3130 362e 3539 3034 3336 270a 2020  34106.590436'.  
+00061050: 2020 2020 2020 2320 2020 2020 7d0a 2020        #     }.  
+00061060: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+00061070: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
+00061080: 2320 2020 2020 2020 2020 2272 6574 436f  #         "retCo
+00061090: 6465 223a 3130 3030 312c 0a20 2020 2020  de":10001,.     
+000610a0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+000610b0: 744d 7367 223a 2273 796d 626f 6c20 7061  tMsg":"symbol pa
+000610c0: 7261 6d73 2065 7272 222c 0a20 2020 2020  rams err",.     
+000610d0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+000610e0: 7375 6c74 223a 7b22 7379 6d62 6f6c 223a  sult":{"symbol":
+000610f0: 2222 2c22 6269 6422 3a22 222c 2262 6964  "","bid":"","bid
+00061100: 4976 223a 2222 2c22 6269 6453 697a 6522  Iv":"","bidSize"
+00061110: 3a22 222c 2261 736b 223a 2222 2c22 6173  :"","ask":"","as
+00061120: 6b49 7622 3a22 222c 2261 736b 5369 7a65  kIv":"","askSize
+00061130: 223a 2222 2c22 6c61 7374 5072 6963 6522  ":"","lastPrice"
+00061140: 3a22 222c 226f 7065 6e49 6e74 6572 6573  :"","openInteres
+00061150: 7422 3a22 222c 2269 6e64 6578 5072 6963  t":"","indexPric
+00061160: 6522 3a22 222c 226d 6172 6b50 7269 6365  e":"","markPrice
+00061170: 223a 2222 2c22 6d61 726b 5072 6963 6549  ":"","markPriceI
+00061180: 7622 3a22 222c 2263 6861 6e67 6532 3468  v":"","change24h
+00061190: 223a 2222 2c22 6869 6768 3234 6822 3a22  ":"","high24h":"
+000611a0: 222c 226c 6f77 3234 6822 3a22 222c 2276  ","low24h":"","v
+000611b0: 6f6c 756d 6532 3468 223a 2222 2c22 7475  olume24h":"","tu
+000611c0: 726e 6f76 6572 3234 6822 3a22 222c 2274  rnover24h":"","t
+000611d0: 6f74 616c 566f 6c75 6d65 223a 2222 2c22  otalVolume":"","
+000611e0: 746f 7461 6c54 7572 6e6f 7665 7222 3a22  totalTurnover":"
+000611f0: 222c 2266 756e 6469 6e67 5261 7465 223a  ","fundingRate":
+00061200: 2222 2c22 7072 6564 6963 7465 6446 756e  "","predictedFun
+00061210: 6469 6e67 5261 7465 223a 2222 2c22 6e65  dingRate":"","ne
+00061220: 7874 4675 6e64 696e 6754 696d 6522 3a22  xtFundingTime":"
+00061230: 222c 2263 6f75 6e74 646f 776e 486f 7572  ","countdownHour
+00061240: 223a 2230 222c 2270 7265 6469 6374 6564  ":"0","predicted
+00061250: 4465 6c69 7665 7279 5072 6963 6522 3a22  DeliveryPrice":"
+00061260: 222c 2275 6e64 6572 6c79 696e 6750 7269  ","underlyingPri
+00061270: 6365 223a 2222 2c22 6465 6c74 6122 3a22  ce":"","delta":"
+00061280: 222c 2267 616d 6d61 223a 2222 2c22 7665  ","gamma":"","ve
+00061290: 6761 223a 2222 2c22 7468 6574 6122 3a22  ga":"","theta":"
+000612a0: 227d 0a20 2020 2020 2020 2023 2020 2020  "}.        #    
+000612b0: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
+000612c0: 2020 2020 2065 7272 6f72 436f 6465 203d       errorCode =
+000612d0: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
+000612e0: 675f 3228 7265 7370 6f6e 7365 2c20 2772  g_2(response, 'r
+000612f0: 6574 5f63 6f64 6527 2c20 2772 6574 436f  et_code', 'retCo
+00061300: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+00061310: 6572 726f 7243 6f64 6520 213d 2027 3027  errorCode != '0'
+00061320: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00061330: 2065 7272 6f72 436f 6465 203d 3d20 2733   errorCode == '3
+00061340: 3030 3834 273a 0a20 2020 2020 2020 2020  0084':.         
+00061350: 2020 2020 2020 2023 206e 6f74 2061 6e20         # not an 
+00061360: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
+00061370: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+00061380: 6769 7468 7562 2e63 6f6d 2f63 6378 742f  github.com/ccxt/
+00061390: 6363 7874 2f69 7373 7565 732f 3131 3236  ccxt/issues/1126
+000613a0: 380a 2020 2020 2020 2020 2020 2020 2020  8.              
+000613b0: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
+000613c0: 7562 2e63 6f6d 2f63 6378 742f 6363 7874  ub.com/ccxt/ccxt
+000613d0: 2f70 756c 6c2f 3131 3632 340a 2020 2020  /pull/11624.    
+000613e0: 2020 2020 2020 2020 2020 2020 2320 504f              # PO
+000613f0: 5354 2068 7474 7073 3a2f 2f61 7069 2e62  ST https://api.b
+00061400: 7962 6974 2e63 6f6d 2f76 322f 7072 6976  ybit.com/v2/priv
+00061410: 6174 652f 706f 7369 7469 6f6e 2f73 7769  ate/position/swi
+00061420: 7463 682d 6973 6f6c 6174 6564 2032 3030  tch-isolated 200
+00061430: 204f 4b0a 2020 2020 2020 2020 2020 2020   OK.            
+00061440: 2020 2020 2320 7b22 7265 745f 636f 6465      # {"ret_code
+00061450: 223a 3330 3038 342c 2272 6574 5f6d 7367  ":30084,"ret_msg
+00061460: 223a 2249 736f 6c61 7465 6420 6e6f 7420  ":"Isolated not 
+00061470: 6d6f 6469 6669 6564 222c 2265 7874 5f63  modified","ext_c
+00061480: 6f64 6522 3a22 222c 2265 7874 5f69 6e66  ode":"","ext_inf
+00061490: 6f22 3a22 222c 2272 6573 756c 7422 3a6e  o":"","result":n
+000614a0: 756c 6c2c 2274 696d 655f 6e6f 7722 3a22  ull,"time_now":"
+000614b0: 3136 3432 3030 3532 3139 2e39 3337 3938  1642005219.93798
+000614c0: 3822 2c22 7261 7465 5f6c 696d 6974 5f73  8","rate_limit_s
+000614d0: 7461 7475 7322 3a37 332c 2272 6174 655f  tatus":73,"rate_
+000614e0: 6c69 6d69 745f 7265 7365 745f 6d73 223a  limit_reset_ms":
+000614f0: 3136 3432 3030 3532 3139 3839 342c 2272  1642005219894,"r
+00061500: 6174 655f 6c69 6d69 7422 3a37 357d 0a20  ate_limit":75}. 
+00061510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00061520: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+00061530: 2020 2020 2020 2066 6565 6462 6163 6b20         feedback 
+00061540: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00061550: 2020 2069 6620 6572 726f 7243 6f64 6520     if errorCode 
+00061560: 3d3d 2027 3130 3030 3527 3a0a 2020 2020  == '10005':.    
+00061570: 2020 2020 2020 2020 2020 2020 6665 6564              feed
+00061580: 6261 636b 203d 2073 656c 662e 6964 202b  back = self.id +
+00061590: 2027 2070 7269 7661 7465 2061 7069 2075   ' private api u
+000615a0: 7365 7320 2f75 7365 722f 7633 2f70 7269  ses /user/v3/pri
+000615b0: 7661 7465 2f71 7565 7279 2d61 7069 2074  vate/query-api t
+000615c0: 6f20 6368 6563 6b20 6966 2079 6f75 2068  o check if you h
+000615d0: 6176 6520 6120 756e 6966 6965 6420 6163  ave a unified ac
+000615e0: 636f 756e 742e 2054 6865 2041 5049 206b  count. The API k
+000615f0: 6579 206f 6620 7573 6572 2069 6420 6d75  ey of user id mu
+00061600: 7374 206f 776e 206f 6e65 206f 6620 7065  st own one of pe
+00061610: 726d 6973 7369 6f6e 733a 2022 4163 636f  rmissions: "Acco
+00061620: 756e 7420 5472 616e 7366 6572 222c 2022  unt Transfer", "
+00061630: 5375 6261 6363 6f75 6e74 2054 7261 6e73  Subaccount Trans
+00061640: 6665 7222 2c20 2257 6974 6864 7261 7761  fer", "Withdrawa
+00061650: 6c22 2027 202b 2062 6f64 790a 2020 2020  l" ' + body.    
+00061660: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00061670: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+00061680: 6564 6261 636b 203d 2073 656c 662e 6964  edback = self.id
+00061690: 202b 2027 2027 202b 2062 6f64 790a 2020   + ' ' + body.  
+000616a0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000616b0: 6872 6f77 5f62 726f 6164 6c79 5f6d 6174  hrow_broadly_mat
+000616c0: 6368 6564 5f65 7863 6570 7469 6f6e 2873  ched_exception(s
+000616d0: 656c 662e 6578 6365 7074 696f 6e73 5b27  elf.exceptions['
+000616e0: 6272 6f61 6427 5d2c 2062 6f64 792c 2066  broad'], body, f
+000616f0: 6565 6462 6163 6b29 0a20 2020 2020 2020  eedback).       
+00061700: 2020 2020 2073 656c 662e 7468 726f 775f       self.throw_
+00061710: 6578 6163 746c 795f 6d61 7463 6865 645f  exactly_matched_
+00061720: 6578 6365 7074 696f 6e28 7365 6c66 2e65  exception(self.e
+00061730: 7863 6570 7469 6f6e 735b 2765 7861 6374  xceptions['exact
+00061740: 275d 2c20 6572 726f 7243 6f64 652c 2066  '], errorCode, f
+00061750: 6565 6462 6163 6b29 0a20 2020 2020 2020  eedback).       
+00061760: 2020 2020 2072 6169 7365 2045 7863 6861       raise Excha
+00061770: 6e67 6545 7272 6f72 2866 6565 6462 6163  ngeError(feedbac
+00061780: 6b29 2020 2320 756e 6b6e 6f77 6e20 6d65  k)  # unknown me
+00061790: 7373 6167 650a 2020 2020 2020 2020 7265  ssage.        re
+000617a0: 7475 726e 204e 6f6e 650a                 turn None.
```

### Comparing `ccxt-3.1.6/ccxt/async_support/cex.py` & `ccxt-3.1.7/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinbase.py` & `ccxt-3.1.7/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinbaseprime.py` & `ccxt-3.1.7/ccxt/async_support/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinbasepro.py` & `ccxt-3.1.7/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coincheck.py` & `ccxt-3.1.7/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinex.py` & `ccxt-3.1.7/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinfalcon.py` & `ccxt-3.1.7/ccxt/async_support/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinmate.py` & `ccxt-3.1.7/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinone.py` & `ccxt-3.1.7/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinsph.py` & `ccxt-3.1.7/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/coinspot.py` & `ccxt-3.1.7/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/cryptocom.py` & `ccxt-3.1.7/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/currencycom.py` & `ccxt-3.1.7/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/delta.py` & `ccxt-3.1.7/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/deribit.py` & `ccxt-3.1.7/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/digifinex.py` & `ccxt-3.1.7/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/exmo.py` & `ccxt-3.1.7/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/flowbtc.py` & `ccxt-3.1.7/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/fmfwio.py` & `ccxt-3.1.7/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/gate.py` & `ccxt-3.1.7/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/gemini.py` & `ccxt-3.1.7/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/hitbtc.py` & `ccxt-3.1.7/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/hitbtc3.py` & `ccxt-3.1.7/ccxt/async_support/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/hollaex.py` & `ccxt-3.1.7/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/huobi.py` & `ccxt-3.1.7/ccxt/async_support/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/huobijp.py` & `ccxt-3.1.7/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/huobipro.py` & `ccxt-3.1.7/ccxt/async_support/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/idex.py` & `ccxt-3.1.7/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/independentreserve.py` & `ccxt-3.1.7/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/indodax.py` & `ccxt-3.1.7/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/itbit.py` & `ccxt-3.1.7/ccxt/async_support/itbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/kraken.py` & `ccxt-3.1.7/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/krakenfutures.py` & `ccxt-3.1.7/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/kucoin.py` & `ccxt-3.1.7/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/kucoinfutures.py` & `ccxt-3.1.7/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/kuna.py` & `ccxt-3.1.7/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/latoken.py` & `ccxt-3.1.7/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/lbank.py` & `ccxt-3.1.7/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/lbank2.py` & `ccxt-3.1.7/ccxt/async_support/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/luno.py` & `ccxt-3.1.7/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/lykke.py` & `ccxt-3.1.7/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/mercado.py` & `ccxt-3.1.7/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/mexc.py` & `ccxt-3.1.7/ccxt/async_support/mexc.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.mexc import ImplicitAPI
 import hashlib
 from ccxt.base.types import OrderSide
+from ccxt.base.types import IndexType
 from typing import Optional
 from typing import List
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
@@ -1002,14 +1003,16 @@
                 },
                 'info': market,
             })
         return result
 
     async def fetch_order_book(self, symbol: str, limit: Optional[int] = None, params={}):
         """
+        see https://mxcdevelop.github.io/apidocs/spot_v3_en/#order-book
+        see https://mxcdevelop.github.io/apidocs/contract_v1_en/#get-the-contract-s-depth-information
         fetches information on open orders with bid(buy) and ask(sell) prices, volumes and other data
         :param str symbol: unified symbol of the market to fetch the order book for
         :param int|None limit: the maximum amount of order book entries to return
         :param dict params: extra parameters specific to the mexc3 api endpoint
         :returns dict: A dictionary of `order book structures <https://docs.ccxt.com/#/?id=order-book-structure>` indexed by market symbols
         """
         await self.load_markets()
@@ -1059,14 +1062,22 @@
             #
             data = self.safe_value(response, 'data')
             timestamp = self.safe_integer(data, 'timestamp')
             orderbook = self.parse_order_book(data, symbol, timestamp)
             orderbook['nonce'] = self.safe_integer(data, 'version')
         return orderbook
 
+    def parse_bid_ask(self, bidask, priceKey: IndexType = 0, amountKey: IndexType = 1, countKey: IndexType = 2):
+        price = self.safe_number(bidask, priceKey)
+        amount = self.safe_number(bidask, amountKey)
+        count = self.safe_number(bidask, countKey)
+        if count is not None:
+            return [price, amount, count]
+        return [price, amount]
+
     async def fetch_trades(self, symbol: str, since: Optional[int] = None, limit: Optional[int] = None, params={}):
         """
         get the list of most recent trades for a particular symbol
         :param str symbol: unified symbol of the market to fetch trades for
         :param int|None since: timestamp in ms of the earliest trade to fetch
         :param int|None limit: the maximum amount of trades to fetch
         :param dict params: extra parameters specific to the mexc3 api endpoint
```

### Comparing `ccxt-3.1.6/ccxt/async_support/ndax.py` & `ccxt-3.1.7/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/novadax.py` & `ccxt-3.1.7/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/oceanex.py` & `ccxt-3.1.7/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/okcoin.py` & `ccxt-3.1.7/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/okx.py` & `ccxt-3.1.7/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/paymium.py` & `ccxt-3.1.7/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/phemex.py` & `ccxt-3.1.7/ccxt/async_support/phemex.py`

 * *Files 1% similar despite different names*

```diff
@@ -11281,745 +11281,807 @@
 0002c100: 6f6c 3a20 756e 6966 6965 6420 6d61 726b  ol: unified mark
 0002c110: 6574 2073 796d 626f 6c0a 2020 2020 2020  et symbol.      
 0002c120: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
 0002c130: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
 0002c140: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
 0002c150: 746f 2074 6865 2070 6865 6d65 7820 6170  to the phemex ap
 0002c160: 6920 656e 6470 6f69 6e74 0a20 2020 2020  i endpoint.     
-0002c170: 2020 203a 7265 7475 726e 7320 6469 6374     :returns dict
-0002c180: 3a20 7265 7370 6f6e 7365 2066 726f 6d20  : response from 
-0002c190: 7468 6520 6578 6368 616e 6765 0a20 2020  the exchange.   
-0002c1a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002c1b0: 2023 2057 4152 4e49 4e47 3a20 5448 4953   # WARNING: THIS
-0002c1c0: 2057 494c 4c20 494e 4352 4541 5345 204c   WILL INCREASE L
-0002c1d0: 4951 5549 4441 5449 4f4e 2050 5249 4345  IQUIDATION PRICE
-0002c1e0: 2046 4f52 204f 5045 4e20 4953 4f4c 4154   FOR OPEN ISOLAT
-0002c1f0: 4544 204c 4f4e 4720 504f 5349 5449 4f4e  ED LONG POSITION
-0002c200: 530a 2020 2020 2020 2020 2320 414e 4420  S.        # AND 
-0002c210: 4445 4352 4541 5345 204c 4951 5549 4441  DECREASE LIQUIDA
-0002c220: 5449 4f4e 2050 5249 4345 2046 4f52 204f  TION PRICE FOR O
-0002c230: 5045 4e20 4953 4f4c 4154 4544 2053 484f  PEN ISOLATED SHO
-0002c240: 5254 2050 4f53 4954 494f 4e53 0a20 2020  RT POSITIONS.   
-0002c250: 2020 2020 2069 6620 7379 6d62 6f6c 2069       if symbol i
-0002c260: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002c270: 2020 2020 7261 6973 6520 4172 6775 6d65      raise Argume
-0002c280: 6e74 7352 6571 7569 7265 6428 7365 6c66  ntsRequired(self
-0002c290: 2e69 6420 2b20 2720 7365 744c 6576 6572  .id + ' setLever
-0002c2a0: 6167 6528 2920 7265 7175 6972 6573 2061  age() requires a
-0002c2b0: 2073 796d 626f 6c20 6172 6775 6d65 6e74   symbol argument
-0002c2c0: 2729 0a20 2020 2020 2020 2069 6620 286c  ').        if (l
-0002c2d0: 6576 6572 6167 6520 3c20 3129 206f 7220  everage < 1) or 
-0002c2e0: 286c 6576 6572 6167 6520 3e20 3130 3029  (leverage > 100)
-0002c2f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0002c300: 6973 6520 4261 6452 6571 7565 7374 2873  ise BadRequest(s
-0002c310: 656c 662e 6964 202b 2027 2073 6574 4c65  elf.id + ' setLe
-0002c320: 7665 7261 6765 2829 206c 6576 6572 6167  verage() leverag
-0002c330: 6520 7368 6f75 6c64 2062 6520 6265 7477  e should be betw
-0002c340: 6565 6e20 3120 616e 6420 3130 3027 290a  een 1 and 100').
-0002c350: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-0002c360: 6c66 2e6c 6f61 645f 6d61 726b 6574 7328  lf.load_markets(
-0002c370: 290a 2020 2020 2020 2020 6d61 726b 6574  ).        market
-0002c380: 203d 2073 656c 662e 6d61 726b 6574 2873   = self.market(s
-0002c390: 796d 626f 6c29 0a20 2020 2020 2020 2072  ymbol).        r
-0002c3a0: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
-0002c3b0: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
-0002c3c0: 206d 6172 6b65 745b 2769 6427 5d2c 0a20   market['id'],. 
-0002c3d0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0002c3e0: 206d 6574 686f 6420 3d20 2770 7269 7661   method = 'priva
-0002c3f0: 7465 5075 7450 6f73 6974 696f 6e73 4c65  tePutPositionsLe
-0002c400: 7665 7261 6765 270a 2020 2020 2020 2020  verage'.        
-0002c410: 6966 206d 6172 6b65 745b 2773 6574 746c  if market['settl
-0002c420: 6527 5d20 3d3d 2027 5553 4454 273a 0a20  e'] == 'USDT':. 
-0002c430: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-0002c440: 6420 3d20 2770 7269 7661 7465 5075 7447  d = 'privatePutG
-0002c450: 506f 7369 7469 6f6e 734c 6576 6572 6167  PositionsLeverag
-0002c460: 6527 0a20 2020 2020 2020 2020 2020 2072  e'.            r
-0002c470: 6571 7565 7374 5b27 6c65 7665 7261 6765  equest['leverage
-0002c480: 5272 275d 203d 206c 6576 6572 6167 650a  Rr'] = leverage.
-0002c490: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002c4a0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0002c4b0: 745b 276c 6576 6572 6167 6527 5d20 3d20  t['leverage'] = 
-0002c4c0: 6c65 7665 7261 6765 0a20 2020 2020 2020  leverage.       
-0002c4d0: 2072 6574 7572 6e20 6177 6169 7420 6765   return await ge
-0002c4e0: 7461 7474 7228 7365 6c66 2c20 6d65 7468  tattr(self, meth
-0002c4f0: 6f64 2928 7365 6c66 2e65 7874 656e 6428  od)(self.extend(
-0002c500: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
-0002c510: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-0002c520: 2074 7261 6e73 6665 7228 7365 6c66 2c20   transfer(self, 
-0002c530: 636f 6465 3a20 7374 722c 2061 6d6f 756e  code: str, amoun
-0002c540: 742c 2066 726f 6d41 6363 6f75 6e74 2c20  t, fromAccount, 
-0002c550: 746f 4163 636f 756e 742c 2070 6172 616d  toAccount, param
-0002c560: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
-0002c570: 2222 0a20 2020 2020 2020 2074 7261 6e73  "".        trans
-0002c580: 6665 7220 6375 7272 656e 6379 2069 6e74  fer currency int
-0002c590: 6572 6e61 6c6c 7920 6265 7477 6565 6e20  ernally between 
-0002c5a0: 7761 6c6c 6574 7320 6f6e 2074 6865 2073  wallets on the s
-0002c5b0: 616d 6520 6163 636f 756e 740a 2020 2020  ame account.    
-0002c5c0: 2020 2020 3a70 6172 616d 2073 7472 2063      :param str c
-0002c5d0: 6f64 653a 2075 6e69 6669 6564 2063 7572  ode: unified cur
-0002c5e0: 7265 6e63 7920 636f 6465 0a20 2020 2020  rency code.     
-0002c5f0: 2020 203a 7061 7261 6d20 666c 6f61 7420     :param float 
-0002c600: 616d 6f75 6e74 3a20 616d 6f75 6e74 2074  amount: amount t
-0002c610: 6f20 7472 616e 7366 6572 0a20 2020 2020  o transfer.     
-0002c620: 2020 203a 7061 7261 6d20 7374 7220 6672     :param str fr
-0002c630: 6f6d 4163 636f 756e 743a 2061 6363 6f75  omAccount: accou
-0002c640: 6e74 2074 6f20 7472 616e 7366 6572 2066  nt to transfer f
-0002c650: 726f 6d0a 2020 2020 2020 2020 3a70 6172  rom.        :par
-0002c660: 616d 2073 7472 2074 6f41 6363 6f75 6e74  am str toAccount
-0002c670: 3a20 6163 636f 756e 7420 746f 2074 7261  : account to tra
-0002c680: 6e73 6665 7220 746f 0a20 2020 2020 2020  nsfer to.       
-0002c690: 203a 7061 7261 6d20 6469 6374 2070 6172   :param dict par
-0002c6a0: 616d 733a 2065 7874 7261 2070 6172 616d  ams: extra param
-0002c6b0: 6574 6572 7320 7370 6563 6966 6963 2074  eters specific t
-0002c6c0: 6f20 7468 6520 7068 656d 6578 2061 7069  o the phemex api
-0002c6d0: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
-0002c6e0: 2020 3a70 6172 616d 2073 7472 7c4e 6f6e    :param str|Non
-0002c6f0: 6520 7061 7261 6d73 5b27 6269 7a54 7970  e params['bizTyp
-0002c700: 6527 5d3a 2066 6f72 2074 7261 6e73 6665  e']: for transfe
-0002c710: 7272 696e 6720 6265 7477 6565 6e20 6d61  rring between ma
-0002c720: 696e 2061 6e64 2073 7562 2d61 636f 756e  in and sub-acoun
-0002c730: 7473 2065 6974 6865 7220 2753 504f 5427  ts either 'SPOT'
-0002c740: 206f 7220 2750 4552 5045 5455 414c 2720   or 'PERPETUAL' 
-0002c750: 6465 6661 756c 7420 6973 2027 5350 4f54  default is 'SPOT
-0002c760: 270a 2020 2020 2020 2020 3a72 6574 7572  '.        :retur
-0002c770: 6e73 2064 6963 743a 2061 2060 7472 616e  ns dict: a `tran
-0002c780: 7366 6572 2073 7472 7563 7475 7265 203c  sfer structure <
-0002c790: 6874 7470 733a 2f2f 646f 6373 2e63 6378  https://docs.ccx
-0002c7a0: 742e 636f 6d2f 232f 3f69 643d 7472 616e  t.com/#/?id=tran
-0002c7b0: 7366 6572 2d73 7472 7563 7475 7265 3e60  sfer-structure>`
-0002c7c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002c7d0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-0002c7e0: 6c6f 6164 5f6d 6172 6b65 7473 2829 0a20  load_markets(). 
-0002c7f0: 2020 2020 2020 2063 7572 7265 6e63 7920         currency 
-0002c800: 3d20 7365 6c66 2e63 7572 7265 6e63 7928  = self.currency(
-0002c810: 636f 6465 290a 2020 2020 2020 2020 6163  code).        ac
-0002c820: 636f 756e 7473 4279 5479 7065 203d 2073  countsByType = s
-0002c830: 656c 662e 7361 6665 5f76 616c 7565 2873  elf.safe_value(s
-0002c840: 656c 662e 6f70 7469 6f6e 732c 2027 6163  elf.options, 'ac
-0002c850: 636f 756e 7473 4279 5479 7065 272c 207b  countsByType', {
-0002c860: 7d29 0a20 2020 2020 2020 2066 726f 6d49  }).        fromI
-0002c870: 6420 3d20 7365 6c66 2e73 6166 655f 7374  d = self.safe_st
-0002c880: 7269 6e67 2861 6363 6f75 6e74 7342 7954  ring(accountsByT
-0002c890: 7970 652c 2066 726f 6d41 6363 6f75 6e74  ype, fromAccount
-0002c8a0: 2c20 6672 6f6d 4163 636f 756e 7429 0a20  , fromAccount). 
-0002c8b0: 2020 2020 2020 2074 6f49 6420 3d20 7365         toId = se
-0002c8c0: 6c66 2e73 6166 655f 7374 7269 6e67 2861  lf.safe_string(a
-0002c8d0: 6363 6f75 6e74 7342 7954 7970 652c 2074  ccountsByType, t
-0002c8e0: 6f41 6363 6f75 6e74 2c20 746f 4163 636f  oAccount, toAcco
-0002c8f0: 756e 7429 0a20 2020 2020 2020 2073 6361  unt).        sca
-0002c900: 6c65 6441 6d6d 6f75 6e74 203d 2073 656c  ledAmmount = sel
-0002c910: 662e 746f 5f65 7628 616d 6f75 6e74 2c20  f.to_ev(amount, 
-0002c920: 6375 7272 656e 6379 290a 2020 2020 2020  currency).      
-0002c930: 2020 6469 7265 6374 696f 6e20 3d20 4e6f    direction = No
-0002c940: 6e65 0a20 2020 2020 2020 2074 7261 6e73  ne.        trans
-0002c950: 6665 7220 3d20 4e6f 6e65 0a20 2020 2020  fer = None.     
-0002c960: 2020 2069 6620 6672 6f6d 4964 203d 3d20     if fromId == 
-0002c970: 2773 706f 7427 2061 6e64 2074 6f49 6420  'spot' and toId 
-0002c980: 3d3d 2027 6675 7475 7265 273a 0a20 2020  == 'future':.   
-0002c990: 2020 2020 2020 2020 2064 6972 6563 7469           directi
-0002c9a0: 6f6e 203d 2032 0a20 2020 2020 2020 2065  on = 2.        e
-0002c9b0: 6c69 6620 6672 6f6d 4964 203d 3d20 2766  lif fromId == 'f
-0002c9c0: 7574 7572 6527 2061 6e64 2074 6f49 6420  uture' and toId 
-0002c9d0: 3d3d 2027 7370 6f74 273a 0a20 2020 2020  == 'spot':.     
-0002c9e0: 2020 2020 2020 2064 6972 6563 7469 6f6e         direction
-0002c9f0: 203d 2031 0a20 2020 2020 2020 2069 6620   = 1.        if 
-0002ca00: 6469 7265 6374 696f 6e20 6973 206e 6f74  direction is not
-0002ca10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002ca20: 2020 2072 6571 7565 7374 203d 207b 0a20     request = {. 
-0002ca30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0002ca40: 6375 7272 656e 6379 273a 2063 7572 7265  currency': curre
-0002ca50: 6e63 795b 2769 6427 5d2c 0a20 2020 2020  ncy['id'],.     
-0002ca60: 2020 2020 2020 2020 2020 2027 6d6f 7665             'move
-0002ca70: 4f70 273a 2064 6972 6563 7469 6f6e 2c0a  Op': direction,.
-0002ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca90: 2761 6d6f 756e 7445 7627 3a20 7363 616c  'amountEv': scal
-0002caa0: 6564 416d 6d6f 756e 742c 0a20 2020 2020  edAmmount,.     
-0002cab0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0002cac0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-0002cad0: 6177 6169 7420 7365 6c66 2e70 7269 7661  await self.priva
-0002cae0: 7465 506f 7374 4173 7365 7473 5472 616e  tePostAssetsTran
-0002caf0: 7366 6572 2873 656c 662e 6578 7465 6e64  sfer(self.extend
-0002cb00: 2872 6571 7565 7374 2c20 7061 7261 6d73  (request, params
-0002cb10: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
-0002cb20: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0002cb30: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-0002cb40: 2023 2020 2020 2020 2020 2063 6f64 653a   #         code:
-0002cb50: 2027 3027 2c0a 2020 2020 2020 2020 2020   '0',.          
-0002cb60: 2020 2320 2020 2020 2020 2020 6d73 673a    #         msg:
-0002cb70: 2027 4f4b 272c 0a20 2020 2020 2020 2020   'OK',.         
-0002cb80: 2020 2023 2020 2020 2020 2020 2064 6174     #         dat
-0002cb90: 613a 207b 0a20 2020 2020 2020 2020 2020  a: {.           
-0002cba0: 2023 2020 2020 2020 2020 2020 2020 206c   #             l
-0002cbb0: 696e 6b4b 6579 3a20 2738 3536 3465 6261  inkKey: '8564eba
-0002cbc0: 342d 6339 6563 2d34 3964 362d 3962 3863  4-c9ec-49d6-9b8c
-0002cbd0: 2d32 6563 3530 3031 6130 6662 3927 2c0a  -2ec5001a0fb9',.
-0002cbe0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0002cbf0: 2020 2020 2020 2020 2020 7573 6572 4964            userId
-0002cc00: 3a20 2734 3031 3833 3430 272c 0a20 2020  : '4018340',.   
-0002cc10: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-0002cc20: 2020 2020 2020 2063 7572 7265 6e63 793a         currency:
-0002cc30: 2027 5553 4427 2c0a 2020 2020 2020 2020   'USD',.        
-0002cc40: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0002cc50: 2020 616d 6f75 6e74 4576 3a20 2731 3027    amountEv: '10'
-0002cc60: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-0002cc70: 2020 2020 2020 2020 2020 2020 7369 6465              side
-0002cc80: 3a20 2732 272c 0a20 2020 2020 2020 2020  : '2',.         
-0002cc90: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0002cca0: 2073 7461 7475 733a 2027 3130 270a 2020   status: '10'.  
-0002ccb0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-0002ccc0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-0002ccd0: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
-0002cce0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-0002ccf0: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
-0002cd00: 7361 6665 5f76 616c 7565 2872 6573 706f  safe_value(respo
-0002cd10: 6e73 652c 2027 6461 7461 272c 207b 7d29  nse, 'data', {})
-0002cd20: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-0002cd30: 6e73 6665 7220 3d20 7365 6c66 2e70 6172  nsfer = self.par
-0002cd40: 7365 5f74 7261 6e73 6665 7228 6461 7461  se_transfer(data
-0002cd50: 2c20 6375 7272 656e 6379 290a 2020 2020  , currency).    
-0002cd60: 2020 2020 656c 7365 3a20 2023 2073 7562      else:  # sub
-0002cd70: 2061 6363 6f75 6e74 2074 7261 6e73 6665   account transfe
-0002cd80: 720a 2020 2020 2020 2020 2020 2020 7265  r.            re
-0002cd90: 7175 6573 7420 3d20 7b0a 2020 2020 2020  quest = {.      
-0002cda0: 2020 2020 2020 2020 2020 2766 726f 6d55            'fromU
-0002cdb0: 7365 7249 6427 3a20 6672 6f6d 4964 2c0a  serId': fromId,.
-0002cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cdd0: 2774 6f55 7365 7249 6427 3a20 746f 4964  'toUserId': toId
-0002cde0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002cdf0: 2020 2761 6d6f 756e 7445 7627 3a20 7363    'amountEv': sc
-0002ce00: 616c 6564 416d 6d6f 756e 742c 0a20 2020  aledAmmount,.   
-0002ce10: 2020 2020 2020 2020 2020 2020 2027 6375               'cu
-0002ce20: 7272 656e 6379 273a 2063 7572 7265 6e63  rrency': currenc
-0002ce30: 795b 2769 6427 5d2c 0a20 2020 2020 2020  y['id'],.       
-0002ce40: 2020 2020 2020 2020 2027 6269 7a54 7970           'bizTyp
-0002ce50: 6527 3a20 7365 6c66 2e73 6166 655f 7374  e': self.safe_st
-0002ce60: 7269 6e67 2870 6172 616d 732c 2027 6269  ring(params, 'bi
-0002ce70: 7a54 7970 6527 2c20 2753 504f 5427 292c  zType', 'SPOT'),
-0002ce80: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-0002ce90: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-0002cea0: 6e73 6520 3d20 6177 6169 7420 7365 6c66  nse = await self
-0002ceb0: 2e70 7269 7661 7465 506f 7374 4173 7365  .privatePostAsse
-0002cec0: 7473 556e 6976 6572 7361 6c54 7261 6e73  tsUniversalTrans
+0002c170: 2020 203a 7061 7261 6d20 626f 6f6c 2070     :param bool p
+0002c180: 6172 616d 735b 2768 6564 6765 6427 5d3a  arams['hedged']:
+0002c190: 2073 6574 2074 6f20 5472 7565 2069 6620   set to True if 
+0002c1a0: 6865 6467 6564 2070 6f73 6974 696f 6e20  hedged position 
+0002c1b0: 6d6f 6465 2069 7320 656e 6162 6c65 6428  mode is enabled(
+0002c1c0: 6279 2064 6566 6175 6c74 206c 6f6e 6720  by default long 
+0002c1d0: 616e 6420 7368 6f72 7420 6c65 7665 7261  and short levera
+0002c1e0: 6765 2061 7265 2073 6574 2074 6f20 7468  ge are set to th
+0002c1f0: 6520 7361 6d65 2076 616c 7565 290a 2020  e same value).  
+0002c200: 2020 2020 2020 3a70 6172 616d 2066 6c6f        :param flo
+0002c210: 6174 2070 6172 616d 735b 276c 6f6e 674c  at params['longL
+0002c220: 6576 6572 6167 6552 7227 5d3a 202a 6865  everageRr']: *he
+0002c230: 6467 6564 206d 6f64 6520 6f6e 6c79 2a20  dged mode only* 
+0002c240: 7365 7420 7468 6520 6c65 7665 7261 6765  set the leverage
+0002c250: 2066 6f72 206c 6f6e 6720 706f 7369 7469   for long positi
+0002c260: 6f6e 730a 2020 2020 2020 2020 3a70 6172  ons.        :par
+0002c270: 616d 2066 6c6f 6174 2070 6172 616d 735b  am float params[
+0002c280: 2773 686f 7274 4c65 7665 7261 6765 5272  'shortLeverageRr
+0002c290: 275d 3a20 2a68 6564 6765 6420 6d6f 6465  ']: *hedged mode
+0002c2a0: 206f 6e6c 792a 2073 6574 2074 6865 206c   only* set the l
+0002c2b0: 6576 6572 6167 6520 666f 7220 7368 6f72  everage for shor
+0002c2c0: 7420 706f 7369 7469 6f6e 730a 2020 2020  t positions.    
+0002c2d0: 2020 2020 3a72 6574 7572 6e73 2064 6963      :returns dic
+0002c2e0: 743a 2072 6573 706f 6e73 6520 6672 6f6d  t: response from
+0002c2f0: 2074 6865 2065 7863 6861 6e67 650a 2020   the exchange.  
+0002c300: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002c310: 2020 2320 5741 524e 494e 473a 2054 4849    # WARNING: THI
+0002c320: 5320 5749 4c4c 2049 4e43 5245 4153 4520  S WILL INCREASE 
+0002c330: 4c49 5155 4944 4154 494f 4e20 5052 4943  LIQUIDATION PRIC
+0002c340: 4520 464f 5220 4f50 454e 2049 534f 4c41  E FOR OPEN ISOLA
+0002c350: 5445 4420 4c4f 4e47 2050 4f53 4954 494f  TED LONG POSITIO
+0002c360: 4e53 0a20 2020 2020 2020 2023 2041 4e44  NS.        # AND
+0002c370: 2044 4543 5245 4153 4520 4c49 5155 4944   DECREASE LIQUID
+0002c380: 4154 494f 4e20 5052 4943 4520 464f 5220  ATION PRICE FOR 
+0002c390: 4f50 454e 2049 534f 4c41 5445 4420 5348  OPEN ISOLATED SH
+0002c3a0: 4f52 5420 504f 5349 5449 4f4e 530a 2020  ORT POSITIONS.  
+0002c3b0: 2020 2020 2020 6966 2073 796d 626f 6c20        if symbol 
+0002c3c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0002c3d0: 2020 2020 2072 6169 7365 2041 7267 756d       raise Argum
+0002c3e0: 656e 7473 5265 7175 6972 6564 2873 656c  entsRequired(sel
+0002c3f0: 662e 6964 202b 2027 2073 6574 4c65 7665  f.id + ' setLeve
+0002c400: 7261 6765 2829 2072 6571 7569 7265 7320  rage() requires 
+0002c410: 6120 7379 6d62 6f6c 2061 7267 756d 656e  a symbol argumen
+0002c420: 7427 290a 2020 2020 2020 2020 6966 2028  t').        if (
+0002c430: 6c65 7665 7261 6765 203c 2031 2920 6f72  leverage < 1) or
+0002c440: 2028 6c65 7665 7261 6765 203e 2031 3030   (leverage > 100
+0002c450: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0002c460: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+0002c470: 7365 6c66 2e69 6420 2b20 2720 7365 744c  self.id + ' setL
+0002c480: 6576 6572 6167 6528 2920 6c65 7665 7261  everage() levera
+0002c490: 6765 2073 686f 756c 6420 6265 2062 6574  ge should be bet
+0002c4a0: 7765 656e 2031 2061 6e64 2031 3030 2729  ween 1 and 100')
+0002c4b0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+0002c4c0: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+0002c4d0: 2829 0a20 2020 2020 2020 2069 7348 6564  ().        isHed
+0002c4e0: 6765 6420 3d20 7365 6c66 2e73 6166 655f  ged = self.safe_
+0002c4f0: 7661 6c75 6528 7061 7261 6d73 2c20 2768  value(params, 'h
+0002c500: 6564 6765 6427 2c20 4661 6c73 6529 0a20  edged', False). 
+0002c510: 2020 2020 2020 206c 6f6e 674c 6576 6572         longLever
+0002c520: 6167 6552 7220 3d20 7365 6c66 2e73 6166  ageRr = self.saf
+0002c530: 655f 696e 7465 6765 7228 7061 7261 6d73  e_integer(params
+0002c540: 2c20 276c 6f6e 674c 6576 6572 6167 6552  , 'longLeverageR
+0002c550: 7227 290a 2020 2020 2020 2020 7368 6f72  r').        shor
+0002c560: 744c 6576 6572 6167 6552 7220 3d20 7365  tLeverageRr = se
+0002c570: 6c66 2e73 6166 655f 696e 7465 6765 7228  lf.safe_integer(
+0002c580: 7061 7261 6d73 2c20 2773 686f 7274 4c65  params, 'shortLe
+0002c590: 7665 7261 6765 5272 2729 0a20 2020 2020  verageRr').     
+0002c5a0: 2020 206d 6172 6b65 7420 3d20 7365 6c66     market = self
+0002c5b0: 2e6d 6172 6b65 7428 7379 6d62 6f6c 290a  .market(symbol).
+0002c5c0: 2020 2020 2020 2020 7265 7175 6573 7420          request 
+0002c5d0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0002c5e0: 2773 796d 626f 6c27 3a20 6d61 726b 6574  'symbol': market
+0002c5f0: 5b27 6964 275d 2c0a 2020 2020 2020 2020  ['id'],.        
+0002c600: 7d0a 2020 2020 2020 2020 7265 7370 6f6e  }.        respon
+0002c610: 7365 203d 204e 6f6e 650a 2020 2020 2020  se = None.      
+0002c620: 2020 6966 206d 6172 6b65 745b 2773 6574    if market['set
+0002c630: 746c 6527 5d20 3d3d 2027 5553 4454 273a  tle'] == 'USDT':
+0002c640: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0002c650: 6e6f 7420 6973 4865 6467 6564 2061 6e64  not isHedged and
+0002c660: 206c 6f6e 674c 6576 6572 6167 6552 7220   longLeverageRr 
+0002c670: 6973 204e 6f6e 6520 616e 6420 7368 6f72  is None and shor
+0002c680: 744c 6576 6572 6167 6552 7220 6973 204e  tLeverageRr is N
+0002c690: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c6a0: 2020 2020 2072 6571 7565 7374 5b27 6c65       request['le
+0002c6b0: 7665 7261 6765 5272 275d 203d 206c 6576  verageRr'] = lev
+0002c6c0: 6572 6167 650a 2020 2020 2020 2020 2020  erage.          
+0002c6d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002c6e0: 2020 2020 2020 2020 6c6f 6e67 203d 206c          long = l
+0002c6f0: 6f6e 674c 6576 6572 6167 6552 7220 6966  ongLeverageRr if
+0002c700: 2028 6c6f 6e67 4c65 7665 7261 6765 5272   (longLeverageRr
+0002c710: 2069 7320 6e6f 7420 4e6f 6e65 2920 656c   is not None) el
+0002c720: 7365 206c 6576 6572 6167 650a 2020 2020  se leverage.    
+0002c730: 2020 2020 2020 2020 2020 2020 7368 6f72              shor
+0002c740: 7420 3d20 7368 6f72 744c 6576 6572 6167  t = shortLeverag
+0002c750: 6552 7220 6966 2028 7368 6f72 744c 6576  eRr if (shortLev
+0002c760: 6572 6167 6552 7220 6973 206e 6f74 204e  erageRr is not N
+0002c770: 6f6e 6529 2065 6c73 6520 6c65 7665 7261  one) else levera
+0002c780: 6765 0a20 2020 2020 2020 2020 2020 2020  ge.             
+0002c790: 2020 2072 6571 7565 7374 5b27 6c6f 6e67     request['long
+0002c7a0: 4c65 7665 7261 6765 5272 275d 203d 206c  LeverageRr'] = l
+0002c7b0: 6f6e 670a 2020 2020 2020 2020 2020 2020  ong.            
+0002c7c0: 2020 2020 7265 7175 6573 745b 2773 686f      request['sho
+0002c7d0: 7274 4c65 7665 7261 6765 5272 275d 203d  rtLeverageRr'] =
+0002c7e0: 2073 686f 7274 0a20 2020 2020 2020 2020   short.         
+0002c7f0: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
+0002c800: 6169 7420 7365 6c66 2e70 7269 7661 7465  ait self.private
+0002c810: 5075 7447 506f 7369 7469 6f6e 734c 6576  PutGPositionsLev
+0002c820: 6572 6167 6528 7365 6c66 2e65 7874 656e  erage(self.exten
+0002c830: 6428 7265 7175 6573 742c 2070 6172 616d  d(request, param
+0002c840: 7329 290a 2020 2020 2020 2020 656c 7365  s)).        else
+0002c850: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002c860: 7175 6573 745b 276c 6576 6572 6167 6527  quest['leverage'
+0002c870: 5d20 3d20 6c65 7665 7261 6765 0a20 2020  ] = leverage.   
+0002c880: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+0002c890: 6520 3d20 6177 6169 7420 7365 6c66 2e70  e = await self.p
+0002c8a0: 7269 7661 7465 5075 7450 6f73 6974 696f  rivatePutPositio
+0002c8b0: 6e73 4c65 7665 7261 6765 2873 656c 662e  nsLeverage(self.
+0002c8c0: 6578 7465 6e64 2872 6571 7565 7374 2c20  extend(request, 
+0002c8d0: 7061 7261 6d73 2929 0a20 2020 2020 2020  params)).       
+0002c8e0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+0002c8f0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0002c900: 7472 616e 7366 6572 2873 656c 662c 2063  transfer(self, c
+0002c910: 6f64 653a 2073 7472 2c20 616d 6f75 6e74  ode: str, amount
+0002c920: 2c20 6672 6f6d 4163 636f 756e 742c 2074  , fromAccount, t
+0002c930: 6f41 6363 6f75 6e74 2c20 7061 7261 6d73  oAccount, params
+0002c940: 3d7b 7d29 3a0a 2020 2020 2020 2020 2222  ={}):.        ""
+0002c950: 220a 2020 2020 2020 2020 7472 616e 7366  ".        transf
+0002c960: 6572 2063 7572 7265 6e63 7920 696e 7465  er currency inte
+0002c970: 726e 616c 6c79 2062 6574 7765 656e 2077  rnally between w
+0002c980: 616c 6c65 7473 206f 6e20 7468 6520 7361  allets on the sa
+0002c990: 6d65 2061 6363 6f75 6e74 0a20 2020 2020  me account.     
+0002c9a0: 2020 203a 7061 7261 6d20 7374 7220 636f     :param str co
+0002c9b0: 6465 3a20 756e 6966 6965 6420 6375 7272  de: unified curr
+0002c9c0: 656e 6379 2063 6f64 650a 2020 2020 2020  ency code.      
+0002c9d0: 2020 3a70 6172 616d 2066 6c6f 6174 2061    :param float a
+0002c9e0: 6d6f 756e 743a 2061 6d6f 756e 7420 746f  mount: amount to
+0002c9f0: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
+0002ca00: 2020 3a70 6172 616d 2073 7472 2066 726f    :param str fro
+0002ca10: 6d41 6363 6f75 6e74 3a20 6163 636f 756e  mAccount: accoun
+0002ca20: 7420 746f 2074 7261 6e73 6665 7220 6672  t to transfer fr
+0002ca30: 6f6d 0a20 2020 2020 2020 203a 7061 7261  om.        :para
+0002ca40: 6d20 7374 7220 746f 4163 636f 756e 743a  m str toAccount:
+0002ca50: 2061 6363 6f75 6e74 2074 6f20 7472 616e   account to tran
+0002ca60: 7366 6572 2074 6f0a 2020 2020 2020 2020  sfer to.        
+0002ca70: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
+0002ca80: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
+0002ca90: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
+0002caa0: 2074 6865 2070 6865 6d65 7820 6170 6920   the phemex api 
+0002cab0: 656e 6470 6f69 6e74 0a20 2020 2020 2020  endpoint.       
+0002cac0: 203a 7061 7261 6d20 7374 727c 4e6f 6e65   :param str|None
+0002cad0: 2070 6172 616d 735b 2762 697a 5479 7065   params['bizType
+0002cae0: 275d 3a20 666f 7220 7472 616e 7366 6572  ']: for transfer
+0002caf0: 7269 6e67 2062 6574 7765 656e 206d 6169  ring between mai
+0002cb00: 6e20 616e 6420 7375 622d 6163 6f75 6e74  n and sub-acount
+0002cb10: 7320 6569 7468 6572 2027 5350 4f54 2720  s either 'SPOT' 
+0002cb20: 6f72 2027 5045 5250 4554 5541 4c27 2064  or 'PERPETUAL' d
+0002cb30: 6566 6175 6c74 2069 7320 2753 504f 5427  efault is 'SPOT'
+0002cb40: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0002cb50: 7320 6469 6374 3a20 6120 6074 7261 6e73  s dict: a `trans
+0002cb60: 6665 7220 7374 7275 6374 7572 6520 3c68  fer structure <h
+0002cb70: 7474 7073 3a2f 2f64 6f63 732e 6363 7874  ttps://docs.ccxt
+0002cb80: 2e63 6f6d 2f23 2f3f 6964 3d74 7261 6e73  .com/#/?id=trans
+0002cb90: 6665 722d 7374 7275 6374 7572 653e 600a  fer-structure>`.
+0002cba0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002cbb0: 2020 2020 6177 6169 7420 7365 6c66 2e6c      await self.l
+0002cbc0: 6f61 645f 6d61 726b 6574 7328 290a 2020  oad_markets().  
+0002cbd0: 2020 2020 2020 6375 7272 656e 6379 203d        currency =
+0002cbe0: 2073 656c 662e 6375 7272 656e 6379 2863   self.currency(c
+0002cbf0: 6f64 6529 0a20 2020 2020 2020 2061 6363  ode).        acc
+0002cc00: 6f75 6e74 7342 7954 7970 6520 3d20 7365  ountsByType = se
+0002cc10: 6c66 2e73 6166 655f 7661 6c75 6528 7365  lf.safe_value(se
+0002cc20: 6c66 2e6f 7074 696f 6e73 2c20 2761 6363  lf.options, 'acc
+0002cc30: 6f75 6e74 7342 7954 7970 6527 2c20 7b7d  ountsByType', {}
+0002cc40: 290a 2020 2020 2020 2020 6672 6f6d 4964  ).        fromId
+0002cc50: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
+0002cc60: 696e 6728 6163 636f 756e 7473 4279 5479  ing(accountsByTy
+0002cc70: 7065 2c20 6672 6f6d 4163 636f 756e 742c  pe, fromAccount,
+0002cc80: 2066 726f 6d41 6363 6f75 6e74 290a 2020   fromAccount).  
+0002cc90: 2020 2020 2020 746f 4964 203d 2073 656c        toId = sel
+0002cca0: 662e 7361 6665 5f73 7472 696e 6728 6163  f.safe_string(ac
+0002ccb0: 636f 756e 7473 4279 5479 7065 2c20 746f  countsByType, to
+0002ccc0: 4163 636f 756e 742c 2074 6f41 6363 6f75  Account, toAccou
+0002ccd0: 6e74 290a 2020 2020 2020 2020 7363 616c  nt).        scal
+0002cce0: 6564 416d 6d6f 756e 7420 3d20 7365 6c66  edAmmount = self
+0002ccf0: 2e74 6f5f 6576 2861 6d6f 756e 742c 2063  .to_ev(amount, c
+0002cd00: 7572 7265 6e63 7929 0a20 2020 2020 2020  urrency).       
+0002cd10: 2064 6972 6563 7469 6f6e 203d 204e 6f6e   direction = Non
+0002cd20: 650a 2020 2020 2020 2020 7472 616e 7366  e.        transf
+0002cd30: 6572 203d 204e 6f6e 650a 2020 2020 2020  er = None.      
+0002cd40: 2020 6966 2066 726f 6d49 6420 3d3d 2027    if fromId == '
+0002cd50: 7370 6f74 2720 616e 6420 746f 4964 203d  spot' and toId =
+0002cd60: 3d20 2766 7574 7572 6527 3a0a 2020 2020  = 'future':.    
+0002cd70: 2020 2020 2020 2020 6469 7265 6374 696f          directio
+0002cd80: 6e20 3d20 320a 2020 2020 2020 2020 656c  n = 2.        el
+0002cd90: 6966 2066 726f 6d49 6420 3d3d 2027 6675  if fromId == 'fu
+0002cda0: 7475 7265 2720 616e 6420 746f 4964 203d  ture' and toId =
+0002cdb0: 3d20 2773 706f 7427 3a0a 2020 2020 2020  = 'spot':.      
+0002cdc0: 2020 2020 2020 6469 7265 6374 696f 6e20        direction 
+0002cdd0: 3d20 310a 2020 2020 2020 2020 6966 2064  = 1.        if d
+0002cde0: 6972 6563 7469 6f6e 2069 7320 6e6f 7420  irection is not 
+0002cdf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002ce00: 2020 7265 7175 6573 7420 3d20 7b0a 2020    request = {.  
+0002ce10: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+0002ce20: 7572 7265 6e63 7927 3a20 6375 7272 656e  urrency': curren
+0002ce30: 6379 5b27 6964 275d 2c0a 2020 2020 2020  cy['id'],.      
+0002ce40: 2020 2020 2020 2020 2020 276d 6f76 654f            'moveO
+0002ce50: 7027 3a20 6469 7265 6374 696f 6e2c 0a20  p': direction,. 
+0002ce60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002ce70: 616d 6f75 6e74 4576 273a 2073 6361 6c65  amountEv': scale
+0002ce80: 6441 6d6d 6f75 6e74 2c0a 2020 2020 2020  dAmmount,.      
+0002ce90: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0002cea0: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+0002ceb0: 7761 6974 2073 656c 662e 7072 6976 6174  wait self.privat
+0002cec0: 6550 6f73 7441 7373 6574 7354 7261 6e73  ePostAssetsTrans
 0002ced0: 6665 7228 7365 6c66 2e65 7874 656e 6428  fer(self.extend(
 0002cee0: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
 0002cef0: 290a 2020 2020 2020 2020 2020 2020 230a  ).            #.
 0002cf00: 2020 2020 2020 2020 2020 2020 2320 2020              #   
 0002cf10: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
 0002cf20: 2320 2020 2020 2020 2020 636f 6465 3a20  #         code: 
 0002cf30: 2730 272c 0a20 2020 2020 2020 2020 2020  '0',.           
 0002cf40: 2023 2020 2020 2020 2020 206d 7367 3a20   #         msg: 
 0002cf50: 274f 4b27 2c0a 2020 2020 2020 2020 2020  'OK',.          
 0002cf60: 2020 2320 2020 2020 2020 2020 6461 7461    #         data
-0002cf70: 3a20 2741 5049 2d39 3233 6462 3832 362d  : 'API-923db826-
-0002cf80: 6161 6161 2d61 6161 612d 6161 6161 2d34  aaaa-aaaa-aaaa-4
-0002cf90: 6439 3863 3361 3763 3966 6427 0a20 2020  d98c3a7c9fd'.   
-0002cfa0: 2020 2020 2020 2020 2023 2020 2020 207d           #     }
-0002cfb0: 0a20 2020 2020 2020 2020 2020 2023 0a20  .            #. 
-0002cfc0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-0002cfd0: 6665 7220 3d20 7365 6c66 2e70 6172 7365  fer = self.parse
-0002cfe0: 5f74 7261 6e73 6665 7228 7265 7370 6f6e  _transfer(respon
-0002cff0: 7365 290a 2020 2020 2020 2020 7472 616e  se).        tran
-0002d000: 7366 6572 4f70 7469 6f6e 7320 3d20 7365  sferOptions = se
-0002d010: 6c66 2e73 6166 655f 7661 6c75 6528 7365  lf.safe_value(se
-0002d020: 6c66 2e6f 7074 696f 6e73 2c20 2774 7261  lf.options, 'tra
-0002d030: 6e73 6665 7227 2c20 7b7d 290a 2020 2020  nsfer', {}).    
-0002d040: 2020 2020 6669 6c6c 5265 7370 6f6e 7365      fillResponse
-0002d050: 4672 6f6d 5265 7175 6573 7420 3d20 7365  FromRequest = se
-0002d060: 6c66 2e73 6166 655f 7661 6c75 6528 7472  lf.safe_value(tr
-0002d070: 616e 7366 6572 4f70 7469 6f6e 732c 2027  ansferOptions, '
-0002d080: 6669 6c6c 5265 7370 6f6e 7365 4672 6f6d  fillResponseFrom
-0002d090: 5265 7175 6573 7427 2c20 5472 7565 290a  Request', True).
-0002d0a0: 2020 2020 2020 2020 6966 2066 696c 6c52          if fillR
-0002d0b0: 6573 706f 6e73 6546 726f 6d52 6571 7565  esponseFromReque
-0002d0c0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-0002d0d0: 6966 2074 7261 6e73 6665 725b 2766 726f  if transfer['fro
-0002d0e0: 6d41 6363 6f75 6e74 275d 2069 7320 4e6f  mAccount'] is No
-0002d0f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002d100: 2020 2020 7472 616e 7366 6572 5b27 6672      transfer['fr
-0002d110: 6f6d 4163 636f 756e 7427 5d20 3d20 6672  omAccount'] = fr
-0002d120: 6f6d 4163 636f 756e 740a 2020 2020 2020  omAccount.      
-0002d130: 2020 2020 2020 6966 2074 7261 6e73 6665        if transfe
-0002d140: 725b 2774 6f41 6363 6f75 6e74 275d 2069  r['toAccount'] i
-0002d150: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002d160: 2020 2020 2020 2020 7472 616e 7366 6572          transfer
-0002d170: 5b27 746f 4163 636f 756e 7427 5d20 3d20  ['toAccount'] = 
-0002d180: 746f 4163 636f 756e 740a 2020 2020 2020  toAccount.      
-0002d190: 2020 2020 2020 6966 2074 7261 6e73 6665        if transfe
-0002d1a0: 725b 2761 6d6f 756e 7427 5d20 6973 204e  r['amount'] is N
-0002d1b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002d1c0: 2020 2020 2074 7261 6e73 6665 725b 2761       transfer['a
-0002d1d0: 6d6f 756e 7427 5d20 3d20 616d 6f75 6e74  mount'] = amount
-0002d1e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0002d1f0: 7472 616e 7366 6572 5b27 6375 7272 656e  transfer['curren
-0002d200: 6379 275d 2069 7320 4e6f 6e65 3a0a 2020  cy'] is None:.  
-0002d210: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0002d220: 616e 7366 6572 5b27 6375 7272 656e 6379  ansfer['currency
-0002d230: 275d 203d 2063 6f64 650a 2020 2020 2020  '] = code.      
-0002d240: 2020 7265 7475 726e 2074 7261 6e73 6665    return transfe
-0002d250: 720a 0a20 2020 2061 7379 6e63 2064 6566  r..    async def
-0002d260: 2066 6574 6368 5f74 7261 6e73 6665 7273   fetch_transfers
-0002d270: 2873 656c 662c 2063 6f64 653a 204f 7074  (self, code: Opt
-0002d280: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0002d290: 652c 2073 696e 6365 3a20 4f70 7469 6f6e  e, since: Option
-0002d2a0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
-0002d2b0: 6c69 6d69 743a 204f 7074 696f 6e61 6c5b  limit: Optional[
-0002d2c0: 696e 745d 203d 204e 6f6e 652c 2070 6172  int] = None, par
-0002d2d0: 616d 733d 7b7d 293a 0a20 2020 2020 2020  ams={}):.       
-0002d2e0: 2022 2222 0a20 2020 2020 2020 2066 6574   """.        fet
-0002d2f0: 6368 2061 2068 6973 746f 7279 206f 6620  ch a history of 
-0002d300: 696e 7465 726e 616c 2074 7261 6e73 6665  internal transfe
-0002d310: 7273 206d 6164 6520 6f6e 2061 6e20 6163  rs made on an ac
-0002d320: 636f 756e 740a 2020 2020 2020 2020 3a70  count.        :p
-0002d330: 6172 616d 2073 7472 7c4e 6f6e 6520 636f  aram str|None co
-0002d340: 6465 3a20 756e 6966 6965 6420 6375 7272  de: unified curr
-0002d350: 656e 6379 2063 6f64 6520 6f66 2074 6865  ency code of the
-0002d360: 2063 7572 7265 6e63 7920 7472 616e 7366   currency transf
-0002d370: 6572 7265 640a 2020 2020 2020 2020 3a70  erred.        :p
-0002d380: 6172 616d 2069 6e74 7c4e 6f6e 6520 7369  aram int|None si
-0002d390: 6e63 653a 2074 6865 2065 6172 6c69 6573  nce: the earlies
-0002d3a0: 7420 7469 6d65 2069 6e20 6d73 2074 6f20  t time in ms to 
-0002d3b0: 6665 7463 6820 7472 616e 7366 6572 7320  fetch transfers 
-0002d3c0: 666f 720a 2020 2020 2020 2020 3a70 6172  for.        :par
-0002d3d0: 616d 2069 6e74 7c4e 6f6e 6520 6c69 6d69  am int|None limi
-0002d3e0: 743a 2074 6865 206d 6178 696d 756d 206e  t: the maximum n
-0002d3f0: 756d 6265 7220 6f66 2020 7472 616e 7366  umber of  transf
-0002d400: 6572 7320 7374 7275 6374 7572 6573 2074  ers structures t
-0002d410: 6f20 7265 7472 6965 7665 0a20 2020 2020  o retrieve.     
-0002d420: 2020 203a 7061 7261 6d20 6469 6374 2070     :param dict p
-0002d430: 6172 616d 733a 2065 7874 7261 2070 6172  arams: extra par
-0002d440: 616d 6574 6572 7320 7370 6563 6966 6963  ameters specific
-0002d450: 2074 6f20 7468 6520 7068 656d 6578 2061   to the phemex a
-0002d460: 7069 2065 6e64 706f 696e 740a 2020 2020  pi endpoint.    
-0002d470: 2020 2020 3a72 6574 7572 6e73 205b 6469      :returns [di
-0002d480: 6374 5d3a 2061 206c 6973 7420 6f66 2060  ct]: a list of `
-0002d490: 7472 616e 7366 6572 2073 7472 7563 7475  transfer structu
-0002d4a0: 7265 7320 3c68 7474 7073 3a2f 2f64 6f63  res <https://doc
-0002d4b0: 732e 6363 7874 2e63 6f6d 2f23 2f3f 6964  s.ccxt.com/#/?id
-0002d4c0: 3d74 7261 6e73 6665 722d 7374 7275 6374  =transfer-struct
-0002d4d0: 7572 653e 600a 2020 2020 2020 2020 2222  ure>`.        ""
-0002d4e0: 220a 2020 2020 2020 2020 6177 6169 7420  ".        await 
-0002d4f0: 7365 6c66 2e6c 6f61 645f 6d61 726b 6574  self.load_market
-0002d500: 7328 290a 2020 2020 2020 2020 6966 2063  s().        if c
-0002d510: 6f64 6520 6973 204e 6f6e 653a 0a20 2020  ode is None:.   
-0002d520: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
-0002d530: 7267 756d 656e 7473 5265 7175 6972 6564  rgumentsRequired
-0002d540: 2873 656c 662e 6964 202b 2027 2066 6574  (self.id + ' fet
-0002d550: 6368 5472 616e 7366 6572 7328 2920 7265  chTransfers() re
-0002d560: 7175 6972 6573 2061 2063 6f64 6520 6172  quires a code ar
-0002d570: 6775 6d65 6e74 2729 0a20 2020 2020 2020  gument').       
-0002d580: 2063 7572 7265 6e63 7920 3d20 7365 6c66   currency = self
-0002d590: 2e63 7572 7265 6e63 7928 636f 6465 290a  .currency(code).
-0002d5a0: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-0002d5b0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0002d5c0: 2763 7572 7265 6e63 7927 3a20 6375 7272  'currency': curr
-0002d5d0: 656e 6379 5b27 6964 275d 2c0a 2020 2020  ency['id'],.    
-0002d5e0: 2020 2020 7d0a 2020 2020 2020 2020 6966      }.        if
-0002d5f0: 2073 696e 6365 2069 7320 6e6f 7420 4e6f   since is not No
-0002d600: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002d610: 7265 7175 6573 745b 2773 7461 7274 275d  request['start']
-0002d620: 203d 2073 696e 6365 0a20 2020 2020 2020   = since.       
-0002d630: 2069 6620 6c69 6d69 7420 6973 206e 6f74   if limit is not
-0002d640: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002d650: 2020 2072 6571 7565 7374 5b27 6c69 6d69     request['limi
-0002d660: 7427 5d20 3d20 6c69 6d69 740a 2020 2020  t'] = limit.    
-0002d670: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
-0002d680: 7761 6974 2073 656c 662e 7072 6976 6174  wait self.privat
-0002d690: 6547 6574 4173 7365 7473 5472 616e 7366  eGetAssetsTransf
-0002d6a0: 6572 2873 656c 662e 6578 7465 6e64 2872  er(self.extend(r
-0002d6b0: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
-0002d6c0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0002d6d0: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
-0002d6e0: 2020 2023 2020 2020 2020 2020 2022 636f     #         "co
-0002d6f0: 6465 223a 2030 2c0a 2020 2020 2020 2020  de": 0,.        
-0002d700: 2320 2020 2020 2020 2020 226d 7367 223a  #         "msg":
-0002d710: 2022 4f4b 222c 0a20 2020 2020 2020 2023   "OK",.        #
-0002d720: 2020 2020 2020 2020 2022 6461 7461 223a           "data":
-0002d730: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0002d740: 2020 2020 2020 2020 2022 726f 7773 223a           "rows":
-0002d750: 205b 0a20 2020 2020 2020 2023 2020 2020   [.        #    
-0002d760: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-0002d770: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002d780: 2020 2020 2020 2020 2020 2020 2022 6c69               "li
-0002d790: 6e6b 4b65 7922 3a20 2238 3763 3037 3161  nkKey": "87c071a
-0002d7a0: 332d 3836 3238 2d34 6163 322d 6163 6131  3-8628-4ac2-aca1
-0002d7b0: 2d36 6365 3064 3166 6164 3636 6322 2c0a  -6ce0d1fad66c",.
-0002d7c0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002d7d0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-0002d7e0: 7365 7249 6422 3a20 3431 3438 3432 382c  serId": 4148428,
-0002d7f0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0002d800: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0002d810: 6375 7272 656e 6379 223a 2022 4254 4322  currency": "BTC"
-0002d820: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0002d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d840: 2261 6d6f 756e 7445 7622 3a20 3637 3933  "amountEv": 6793
-0002d850: 322c 0a20 2020 2020 2020 2023 2020 2020  2,.        #    
-0002d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d870: 2022 7369 6465 223a 2032 2c0a 2020 2020   "side": 2,.    
-0002d880: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0002d890: 2020 2020 2020 2020 2020 2273 7461 7475            "statu
-0002d8a0: 7322 3a20 3130 2c0a 2020 2020 2020 2020  s": 10,.        
-0002d8b0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0002d8c0: 2020 2020 2020 2263 7265 6174 6554 696d        "createTim
-0002d8d0: 6522 3a20 3136 3532 3833 3234 3637 3030  e": 165283246700
-0002d8e0: 302c 0a20 2020 2020 2020 2023 2020 2020  0,.        #    
-0002d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d900: 2022 6269 7a54 7970 6522 3a20 3130 0a20   "bizType": 10. 
-0002d910: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002d920: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-0002d930: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0002d940: 205d 0a20 2020 2020 2020 2023 2020 2020   ].        #    
-0002d950: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0002d960: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0002d970: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0002d980: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0002d990: 7265 7370 6f6e 7365 2c20 2764 6174 6127  response, 'data'
-0002d9a0: 2c20 7b7d 290a 2020 2020 2020 2020 7472  , {}).        tr
-0002d9b0: 616e 7366 6572 7320 3d20 7365 6c66 2e73  ansfers = self.s
-0002d9c0: 6166 655f 7661 6c75 6528 6461 7461 2c20  afe_value(data, 
-0002d9d0: 2772 6f77 7327 2c20 5b5d 290a 2020 2020  'rows', []).    
-0002d9e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0002d9f0: 7061 7273 655f 7472 616e 7366 6572 7328  parse_transfers(
-0002da00: 7472 616e 7366 6572 732c 2063 7572 7265  transfers, curre
-0002da10: 6e63 792c 2073 696e 6365 2c20 6c69 6d69  ncy, since, limi
-0002da20: 7429 0a0a 2020 2020 6465 6620 7061 7273  t)..    def pars
-0002da30: 655f 7472 616e 7366 6572 2873 656c 662c  e_transfer(self,
-0002da40: 2074 7261 6e73 6665 722c 2063 7572 7265   transfer, curre
-0002da50: 6e63 793d 4e6f 6e65 293a 0a20 2020 2020  ncy=None):.     
-0002da60: 2020 2023 0a20 2020 2020 2020 2023 2074     #.        # t
-0002da70: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
-0002da80: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
-0002da90: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0002daa0: 2020 2020 6c69 6e6b 4b65 793a 2027 3835      linkKey: '85
-0002dab0: 3634 6562 6134 2d63 3965 632d 3439 6436  64eba4-c9ec-49d6
-0002dac0: 2d39 6238 632d 3265 6335 3030 3161 3066  -9b8c-2ec5001a0f
-0002dad0: 6239 272c 0a20 2020 2020 2020 2023 2020  b9',.        #  
-0002dae0: 2020 2020 2020 2075 7365 7249 643a 2027         userId: '
-0002daf0: 3430 3138 3334 3027 2c0a 2020 2020 2020  4018340',.      
-0002db00: 2020 2320 2020 2020 2020 2020 6375 7272    #         curr
-0002db10: 656e 6379 3a20 2755 5344 272c 0a20 2020  ency: 'USD',.   
-0002db20: 2020 2020 2023 2020 2020 2020 2020 2061       #         a
-0002db30: 6d6f 756e 7445 763a 2027 3130 272c 0a20  mountEv: '10',. 
-0002db40: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002db50: 2073 6964 653a 2027 3227 2c0a 2020 2020   side: '2',.    
-0002db60: 2020 2020 2320 2020 2020 2020 2020 7374      #         st
-0002db70: 6174 7573 3a20 2731 3027 0a20 2020 2020  atus: '10'.     
-0002db80: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
-0002db90: 2020 2023 0a20 2020 2020 2020 2023 2066     #.        # f
-0002dba0: 6574 6368 5472 616e 7366 6572 730a 2020  etchTransfers.  
-0002dbb0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-0002dbc0: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
-0002dbd0: 2320 2020 2020 2020 2020 226c 696e 6b4b  #         "linkK
-0002dbe0: 6579 223a 2022 3837 6330 3731 6133 2d38  ey": "87c071a3-8
-0002dbf0: 3632 382d 3461 6332 2d61 6361 312d 3663  628-4ac2-aca1-6c
-0002dc00: 6530 6431 6661 6436 3663 222c 0a20 2020  e0d1fad66c",.   
-0002dc10: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0002dc20: 7573 6572 4964 223a 2034 3134 3834 3238  userId": 4148428
+0002cf70: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+0002cf80: 2320 2020 2020 2020 2020 2020 2020 6c69  #             li
+0002cf90: 6e6b 4b65 793a 2027 3835 3634 6562 6134  nkKey: '8564eba4
+0002cfa0: 2d63 3965 632d 3439 6436 2d39 6238 632d  -c9ec-49d6-9b8c-
+0002cfb0: 3265 6335 3030 3161 3066 6239 272c 0a20  2ec5001a0fb9',. 
+0002cfc0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0002cfd0: 2020 2020 2020 2020 2075 7365 7249 643a           userId:
+0002cfe0: 2027 3430 3138 3334 3027 2c0a 2020 2020   '4018340',.    
+0002cff0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002d000: 2020 2020 2020 6375 7272 656e 6379 3a20        currency: 
+0002d010: 2755 5344 272c 0a20 2020 2020 2020 2020  'USD',.         
+0002d020: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0002d030: 2061 6d6f 756e 7445 763a 2027 3130 272c   amountEv: '10',
+0002d040: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0002d050: 2020 2020 2020 2020 2020 2073 6964 653a             side:
+0002d060: 2027 3227 2c0a 2020 2020 2020 2020 2020   '2',.          
+0002d070: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0002d080: 7374 6174 7573 3a20 2731 3027 0a20 2020  status: '10'.   
+0002d090: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+0002d0a0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+0002d0b0: 2023 2020 2020 207d 0a20 2020 2020 2020   #     }.       
+0002d0c0: 2020 2020 2023 0a20 2020 2020 2020 2020       #.         
+0002d0d0: 2020 2064 6174 6120 3d20 7365 6c66 2e73     data = self.s
+0002d0e0: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
+0002d0f0: 7365 2c20 2764 6174 6127 2c20 7b7d 290a  se, 'data', {}).
+0002d100: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+0002d110: 7366 6572 203d 2073 656c 662e 7061 7273  sfer = self.pars
+0002d120: 655f 7472 616e 7366 6572 2864 6174 612c  e_transfer(data,
+0002d130: 2063 7572 7265 6e63 7929 0a20 2020 2020   currency).     
+0002d140: 2020 2065 6c73 653a 2020 2320 7375 6220     else:  # sub 
+0002d150: 6163 636f 756e 7420 7472 616e 7366 6572  account transfer
+0002d160: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+0002d170: 7565 7374 203d 207b 0a20 2020 2020 2020  uest = {.       
+0002d180: 2020 2020 2020 2020 2027 6672 6f6d 5573           'fromUs
+0002d190: 6572 4964 273a 2066 726f 6d49 642c 0a20  erId': fromId,. 
+0002d1a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002d1b0: 746f 5573 6572 4964 273a 2074 6f49 642c  toUserId': toId,
+0002d1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d1d0: 2027 616d 6f75 6e74 4576 273a 2073 6361   'amountEv': sca
+0002d1e0: 6c65 6441 6d6d 6f75 6e74 2c0a 2020 2020  ledAmmount,.    
+0002d1f0: 2020 2020 2020 2020 2020 2020 2763 7572              'cur
+0002d200: 7265 6e63 7927 3a20 6375 7272 656e 6379  rency': currency
+0002d210: 5b27 6964 275d 2c0a 2020 2020 2020 2020  ['id'],.        
+0002d220: 2020 2020 2020 2020 2762 697a 5479 7065          'bizType
+0002d230: 273a 2073 656c 662e 7361 6665 5f73 7472  ': self.safe_str
+0002d240: 696e 6728 7061 7261 6d73 2c20 2762 697a  ing(params, 'biz
+0002d250: 5479 7065 272c 2027 5350 4f54 2729 2c0a  Type', 'SPOT'),.
+0002d260: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0002d270: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0002d280: 7365 203d 2061 7761 6974 2073 656c 662e  se = await self.
+0002d290: 7072 6976 6174 6550 6f73 7441 7373 6574  privatePostAsset
+0002d2a0: 7355 6e69 7665 7273 616c 5472 616e 7366  sUniversalTransf
+0002d2b0: 6572 2873 656c 662e 6578 7465 6e64 2872  er(self.extend(r
+0002d2c0: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
+0002d2d0: 0a20 2020 2020 2020 2020 2020 2023 0a20  .            #. 
+0002d2e0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0002d2f0: 207b 0a20 2020 2020 2020 2020 2020 2023   {.            #
+0002d300: 2020 2020 2020 2020 2063 6f64 653a 2027           code: '
+0002d310: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+0002d320: 2320 2020 2020 2020 2020 6d73 673a 2027  #         msg: '
+0002d330: 4f4b 272c 0a20 2020 2020 2020 2020 2020  OK',.           
+0002d340: 2023 2020 2020 2020 2020 2064 6174 613a   #         data:
+0002d350: 2027 4150 492d 3932 3364 6238 3236 2d61   'API-923db826-a
+0002d360: 6161 612d 6161 6161 2d61 6161 612d 3464  aaa-aaaa-aaaa-4d
+0002d370: 3938 6333 6137 6339 6664 270a 2020 2020  98c3a7c9fd'.    
+0002d380: 2020 2020 2020 2020 2320 2020 2020 7d0a          #     }.
+0002d390: 2020 2020 2020 2020 2020 2020 230a 2020              #.  
+0002d3a0: 2020 2020 2020 2020 2020 7472 616e 7366            transf
+0002d3b0: 6572 203d 2073 656c 662e 7061 7273 655f  er = self.parse_
+0002d3c0: 7472 616e 7366 6572 2872 6573 706f 6e73  transfer(respons
+0002d3d0: 6529 0a20 2020 2020 2020 2074 7261 6e73  e).        trans
+0002d3e0: 6665 724f 7074 696f 6e73 203d 2073 656c  ferOptions = sel
+0002d3f0: 662e 7361 6665 5f76 616c 7565 2873 656c  f.safe_value(sel
+0002d400: 662e 6f70 7469 6f6e 732c 2027 7472 616e  f.options, 'tran
+0002d410: 7366 6572 272c 207b 7d29 0a20 2020 2020  sfer', {}).     
+0002d420: 2020 2066 696c 6c52 6573 706f 6e73 6546     fillResponseF
+0002d430: 726f 6d52 6571 7565 7374 203d 2073 656c  romRequest = sel
+0002d440: 662e 7361 6665 5f76 616c 7565 2874 7261  f.safe_value(tra
+0002d450: 6e73 6665 724f 7074 696f 6e73 2c20 2766  nsferOptions, 'f
+0002d460: 696c 6c52 6573 706f 6e73 6546 726f 6d52  illResponseFromR
+0002d470: 6571 7565 7374 272c 2054 7275 6529 0a20  equest', True). 
+0002d480: 2020 2020 2020 2069 6620 6669 6c6c 5265         if fillRe
+0002d490: 7370 6f6e 7365 4672 6f6d 5265 7175 6573  sponseFromReques
+0002d4a0: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
+0002d4b0: 6620 7472 616e 7366 6572 5b27 6672 6f6d  f transfer['from
+0002d4c0: 4163 636f 756e 7427 5d20 6973 204e 6f6e  Account'] is Non
+0002d4d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002d4e0: 2020 2074 7261 6e73 6665 725b 2766 726f     transfer['fro
+0002d4f0: 6d41 6363 6f75 6e74 275d 203d 2066 726f  mAccount'] = fro
+0002d500: 6d41 6363 6f75 6e74 0a20 2020 2020 2020  mAccount.       
+0002d510: 2020 2020 2069 6620 7472 616e 7366 6572       if transfer
+0002d520: 5b27 746f 4163 636f 756e 7427 5d20 6973  ['toAccount'] is
+0002d530: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002d540: 2020 2020 2020 2074 7261 6e73 6665 725b         transfer[
+0002d550: 2774 6f41 6363 6f75 6e74 275d 203d 2074  'toAccount'] = t
+0002d560: 6f41 6363 6f75 6e74 0a20 2020 2020 2020  oAccount.       
+0002d570: 2020 2020 2069 6620 7472 616e 7366 6572       if transfer
+0002d580: 5b27 616d 6f75 6e74 275d 2069 7320 4e6f  ['amount'] is No
+0002d590: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002d5a0: 2020 2020 7472 616e 7366 6572 5b27 616d      transfer['am
+0002d5b0: 6f75 6e74 275d 203d 2061 6d6f 756e 740a  ount'] = amount.
+0002d5c0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0002d5d0: 7261 6e73 6665 725b 2763 7572 7265 6e63  ransfer['currenc
+0002d5e0: 7927 5d20 6973 204e 6f6e 653a 0a20 2020  y'] is None:.   
+0002d5f0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0002d600: 6e73 6665 725b 2763 7572 7265 6e63 7927  nsfer['currency'
+0002d610: 5d20 3d20 636f 6465 0a20 2020 2020 2020  ] = code.       
+0002d620: 2072 6574 7572 6e20 7472 616e 7366 6572   return transfer
+0002d630: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0002d640: 6665 7463 685f 7472 616e 7366 6572 7328  fetch_transfers(
+0002d650: 7365 6c66 2c20 636f 6465 3a20 4f70 7469  self, code: Opti
+0002d660: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0002d670: 2c20 7369 6e63 653a 204f 7074 696f 6e61  , since: Optiona
+0002d680: 6c5b 696e 745d 203d 204e 6f6e 652c 206c  l[int] = None, l
+0002d690: 696d 6974 3a20 4f70 7469 6f6e 616c 5b69  imit: Optional[i
+0002d6a0: 6e74 5d20 3d20 4e6f 6e65 2c20 7061 7261  nt] = None, para
+0002d6b0: 6d73 3d7b 7d29 3a0a 2020 2020 2020 2020  ms={}):.        
+0002d6c0: 2222 220a 2020 2020 2020 2020 6665 7463  """.        fetc
+0002d6d0: 6820 6120 6869 7374 6f72 7920 6f66 2069  h a history of i
+0002d6e0: 6e74 6572 6e61 6c20 7472 616e 7366 6572  nternal transfer
+0002d6f0: 7320 6d61 6465 206f 6e20 616e 2061 6363  s made on an acc
+0002d700: 6f75 6e74 0a20 2020 2020 2020 203a 7061  ount.        :pa
+0002d710: 7261 6d20 7374 727c 4e6f 6e65 2063 6f64  ram str|None cod
+0002d720: 653a 2075 6e69 6669 6564 2063 7572 7265  e: unified curre
+0002d730: 6e63 7920 636f 6465 206f 6620 7468 6520  ncy code of the 
+0002d740: 6375 7272 656e 6379 2074 7261 6e73 6665  currency transfe
+0002d750: 7272 6564 0a20 2020 2020 2020 203a 7061  rred.        :pa
+0002d760: 7261 6d20 696e 747c 4e6f 6e65 2073 696e  ram int|None sin
+0002d770: 6365 3a20 7468 6520 6561 726c 6965 7374  ce: the earliest
+0002d780: 2074 696d 6520 696e 206d 7320 746f 2066   time in ms to f
+0002d790: 6574 6368 2074 7261 6e73 6665 7273 2066  etch transfers f
+0002d7a0: 6f72 0a20 2020 2020 2020 203a 7061 7261  or.        :para
+0002d7b0: 6d20 696e 747c 4e6f 6e65 206c 696d 6974  m int|None limit
+0002d7c0: 3a20 7468 6520 6d61 7869 6d75 6d20 6e75  : the maximum nu
+0002d7d0: 6d62 6572 206f 6620 2074 7261 6e73 6665  mber of  transfe
+0002d7e0: 7273 2073 7472 7563 7475 7265 7320 746f  rs structures to
+0002d7f0: 2072 6574 7269 6576 650a 2020 2020 2020   retrieve.      
+0002d800: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
+0002d810: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
+0002d820: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
+0002d830: 746f 2074 6865 2070 6865 6d65 7820 6170  to the phemex ap
+0002d840: 6920 656e 6470 6f69 6e74 0a20 2020 2020  i endpoint.     
+0002d850: 2020 203a 7265 7475 726e 7320 5b64 6963     :returns [dic
+0002d860: 745d 3a20 6120 6c69 7374 206f 6620 6074  t]: a list of `t
+0002d870: 7261 6e73 6665 7220 7374 7275 6374 7572  ransfer structur
+0002d880: 6573 203c 6874 7470 733a 2f2f 646f 6373  es <https://docs
+0002d890: 2e63 6378 742e 636f 6d2f 232f 3f69 643d  .ccxt.com/#/?id=
+0002d8a0: 7472 616e 7366 6572 2d73 7472 7563 7475  transfer-structu
+0002d8b0: 7265 3e60 0a20 2020 2020 2020 2022 2222  re>`.        """
+0002d8c0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+0002d8d0: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+0002d8e0: 2829 0a20 2020 2020 2020 2069 6620 636f  ().        if co
+0002d8f0: 6465 2069 7320 4e6f 6e65 3a0a 2020 2020  de is None:.    
+0002d900: 2020 2020 2020 2020 7261 6973 6520 4172          raise Ar
+0002d910: 6775 6d65 6e74 7352 6571 7569 7265 6428  gumentsRequired(
+0002d920: 7365 6c66 2e69 6420 2b20 2720 6665 7463  self.id + ' fetc
+0002d930: 6854 7261 6e73 6665 7273 2829 2072 6571  hTransfers() req
+0002d940: 7569 7265 7320 6120 636f 6465 2061 7267  uires a code arg
+0002d950: 756d 656e 7427 290a 2020 2020 2020 2020  ument').        
+0002d960: 6375 7272 656e 6379 203d 2073 656c 662e  currency = self.
+0002d970: 6375 7272 656e 6379 2863 6f64 6529 0a20  currency(code). 
+0002d980: 2020 2020 2020 2072 6571 7565 7374 203d         request =
+0002d990: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0002d9a0: 6375 7272 656e 6379 273a 2063 7572 7265  currency': curre
+0002d9b0: 6e63 795b 2769 6427 5d2c 0a20 2020 2020  ncy['id'],.     
+0002d9c0: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
+0002d9d0: 7369 6e63 6520 6973 206e 6f74 204e 6f6e  since is not Non
+0002d9e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002d9f0: 6571 7565 7374 5b27 7374 6172 7427 5d20  equest['start'] 
+0002da00: 3d20 7369 6e63 650a 2020 2020 2020 2020  = since.        
+0002da10: 6966 206c 696d 6974 2069 7320 6e6f 7420  if limit is not 
+0002da20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002da30: 2020 7265 7175 6573 745b 276c 696d 6974    request['limit
+0002da40: 275d 203d 206c 696d 6974 0a20 2020 2020  '] = limit.     
+0002da50: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
+0002da60: 6169 7420 7365 6c66 2e70 7269 7661 7465  ait self.private
+0002da70: 4765 7441 7373 6574 7354 7261 6e73 6665  GetAssetsTransfe
+0002da80: 7228 7365 6c66 2e65 7874 656e 6428 7265  r(self.extend(re
+0002da90: 7175 6573 742c 2070 6172 616d 7329 290a  quest, params)).
+0002daa0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0002dab0: 2020 2320 2020 2020 7b0a 2020 2020 2020    #     {.      
+0002dac0: 2020 2320 2020 2020 2020 2020 2263 6f64    #         "cod
+0002dad0: 6522 3a20 302c 0a20 2020 2020 2020 2023  e": 0,.        #
+0002dae0: 2020 2020 2020 2020 2022 6d73 6722 3a20           "msg": 
+0002daf0: 224f 4b22 2c0a 2020 2020 2020 2020 2320  "OK",.        # 
+0002db00: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
+0002db10: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+0002db20: 2020 2020 2020 2020 2272 6f77 7322 3a20          "rows": 
+0002db30: 5b0a 2020 2020 2020 2020 2320 2020 2020  [.        #     
+0002db40: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+0002db50: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0002db60: 2020 2020 2020 2020 2020 2020 226c 696e              "lin
+0002db70: 6b4b 6579 223a 2022 3837 6330 3731 6133  kKey": "87c071a3
+0002db80: 2d38 3632 382d 3461 6332 2d61 6361 312d  -8628-4ac2-aca1-
+0002db90: 3663 6530 6431 6661 6436 3663 222c 0a20  6ce0d1fad66c",. 
+0002dba0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0002dbb0: 2020 2020 2020 2020 2020 2020 2022 7573               "us
+0002dbc0: 6572 4964 223a 2034 3134 3834 3238 2c0a  erId": 4148428,.
+0002dbd0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002dbe0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+0002dbf0: 7572 7265 6e63 7922 3a20 2242 5443 222c  urrency": "BTC",
+0002dc00: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002dc10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0002dc20: 616d 6f75 6e74 4576 223a 2036 3739 3332  amountEv": 67932
 0002dc30: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0002dc40: 2020 2020 2263 7572 7265 6e63 7922 3a20      "currency": 
-0002dc50: 2242 5443 222c 0a20 2020 2020 2020 2023  "BTC",.        #
-0002dc60: 2020 2020 2020 2020 2022 616d 6f75 6e74           "amount
-0002dc70: 4576 223a 2036 3739 3332 2c0a 2020 2020  Ev": 67932,.    
-0002dc80: 2020 2020 2320 2020 2020 2020 2020 2273      #         "s
-0002dc90: 6964 6522 3a20 322c 0a20 2020 2020 2020  ide": 2,.       
-0002dca0: 2023 2020 2020 2020 2020 2022 7374 6174   #         "stat
-0002dcb0: 7573 223a 2031 302c 0a20 2020 2020 2020  us": 10,.       
-0002dcc0: 2023 2020 2020 2020 2020 2022 6372 6561   #         "crea
-0002dcd0: 7465 5469 6d65 223a 2031 3635 3238 3332  teTime": 1652832
-0002dce0: 3436 3730 3030 2c0a 2020 2020 2020 2020  467000,.        
-0002dcf0: 2320 2020 2020 2020 2020 2262 697a 5479  #         "bizTy
-0002dd00: 7065 223a 2031 300a 2020 2020 2020 2020  pe": 10.        
-0002dd10: 2320 2020 2020 7d0a 2020 2020 2020 2020  #     }.        
-0002dd20: 230a 2020 2020 2020 2020 6964 203d 2073  #.        id = s
-0002dd30: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
-0002dd40: 7472 616e 7366 6572 2c20 276c 696e 6b4b  transfer, 'linkK
-0002dd50: 6579 2729 0a20 2020 2020 2020 2073 7461  ey').        sta
-0002dd60: 7475 7320 3d20 7365 6c66 2e73 6166 655f  tus = self.safe_
-0002dd70: 7374 7269 6e67 2874 7261 6e73 6665 722c  string(transfer,
-0002dd80: 2027 7374 6174 7573 2729 0a20 2020 2020   'status').     
-0002dd90: 2020 2061 6d6f 756e 7445 7620 3d20 7365     amountEv = se
-0002dda0: 6c66 2e73 6166 655f 7374 7269 6e67 2874  lf.safe_string(t
-0002ddb0: 7261 6e73 6665 722c 2027 616d 6f75 6e74  ransfer, 'amount
-0002ddc0: 4576 2729 0a20 2020 2020 2020 2061 6d6f  Ev').        amo
-0002ddd0: 756e 7454 7261 6e73 6665 7265 6420 3d20  untTransfered = 
-0002dde0: 7365 6c66 2e66 726f 6d5f 6576 2861 6d6f  self.from_ev(amo
-0002ddf0: 756e 7445 762c 2063 7572 7265 6e63 7929  untEv, currency)
-0002de00: 0a20 2020 2020 2020 2063 7572 7265 6e63  .        currenc
-0002de10: 7949 6420 3d20 7365 6c66 2e73 6166 655f  yId = self.safe_
-0002de20: 7374 7269 6e67 2874 7261 6e73 6665 722c  string(transfer,
-0002de30: 2027 6375 7272 656e 6379 2729 0a20 2020   'currency').   
-0002de40: 2020 2020 2063 6f64 6520 3d20 7365 6c66       code = self
-0002de50: 2e73 6166 655f 6375 7272 656e 6379 5f63  .safe_currency_c
-0002de60: 6f64 6528 6375 7272 656e 6379 4964 2c20  ode(currencyId, 
-0002de70: 6375 7272 656e 6379 290a 2020 2020 2020  currency).      
-0002de80: 2020 7369 6465 203d 2073 656c 662e 7361    side = self.sa
-0002de90: 6665 5f69 6e74 6567 6572 2874 7261 6e73  fe_integer(trans
-0002dea0: 6665 722c 2027 7369 6465 2729 0a20 2020  fer, 'side').   
-0002deb0: 2020 2020 2066 726f 6d49 6420 3d20 4e6f       fromId = No
-0002dec0: 6e65 0a20 2020 2020 2020 2074 6f49 6420  ne.        toId 
-0002ded0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-0002dee0: 6620 7369 6465 203d 3d20 313a 0a20 2020  f side == 1:.   
-0002def0: 2020 2020 2020 2020 2066 726f 6d49 6420           fromId 
-0002df00: 3d20 2773 7761 7027 0a20 2020 2020 2020  = 'swap'.       
-0002df10: 2020 2020 2074 6f49 6420 3d20 2773 706f       toId = 'spo
-0002df20: 7427 0a20 2020 2020 2020 2065 6c69 6620  t'.        elif 
-0002df30: 7369 6465 203d 3d20 323a 0a20 2020 2020  side == 2:.     
-0002df40: 2020 2020 2020 2066 726f 6d49 6420 3d20         fromId = 
-0002df50: 2773 706f 7427 0a20 2020 2020 2020 2020  'spot'.         
-0002df60: 2020 2074 6f49 6420 3d20 2773 7761 7027     toId = 'swap'
-0002df70: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-0002df80: 6d70 203d 2073 656c 662e 7361 6665 5f69  mp = self.safe_i
-0002df90: 6e74 6567 6572 2874 7261 6e73 6665 722c  nteger(transfer,
-0002dfa0: 2027 6372 6561 7465 5469 6d65 2729 0a20   'createTime'). 
-0002dfb0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
-0002dfc0: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
-0002dfd0: 6f27 3a20 7472 616e 7366 6572 2c0a 2020  o': transfer,.  
-0002dfe0: 2020 2020 2020 2020 2020 2769 6427 3a20            'id': 
-0002dff0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002e000: 2774 696d 6573 7461 6d70 273a 2074 696d  'timestamp': tim
-0002e010: 6573 7461 6d70 2c0a 2020 2020 2020 2020  estamp,.        
-0002e020: 2020 2020 2764 6174 6574 696d 6527 3a20      'datetime': 
-0002e030: 7365 6c66 2e69 736f 3836 3031 2874 696d  self.iso8601(tim
-0002e040: 6573 7461 6d70 292c 0a20 2020 2020 2020  estamp),.       
-0002e050: 2020 2020 2027 6375 7272 656e 6379 273a       'currency':
-0002e060: 2063 6f64 652c 0a20 2020 2020 2020 2020   code,.         
-0002e070: 2020 2027 616d 6f75 6e74 273a 2061 6d6f     'amount': amo
-0002e080: 756e 7454 7261 6e73 6665 7265 642c 0a20  untTransfered,. 
-0002e090: 2020 2020 2020 2020 2020 2027 6672 6f6d             'from
-0002e0a0: 4163 636f 756e 7427 3a20 6672 6f6d 4964  Account': fromId
-0002e0b0: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
-0002e0c0: 6f41 6363 6f75 6e74 273a 2074 6f49 642c  oAccount': toId,
-0002e0d0: 0a20 2020 2020 2020 2020 2020 2027 7374  .            'st
-0002e0e0: 6174 7573 273a 2073 656c 662e 7061 7273  atus': self.pars
-0002e0f0: 655f 7472 616e 7366 6572 5f73 7461 7475  e_transfer_statu
-0002e100: 7328 7374 6174 7573 292c 0a20 2020 2020  s(status),.     
-0002e110: 2020 207d 0a0a 2020 2020 6465 6620 7061     }..    def pa
-0002e120: 7273 655f 7472 616e 7366 6572 5f73 7461  rse_transfer_sta
-0002e130: 7475 7328 7365 6c66 2c20 7374 6174 7573  tus(self, status
-0002e140: 293a 0a20 2020 2020 2020 2073 7461 7475  ):.        statu
-0002e150: 7365 7320 3d20 7b0a 2020 2020 2020 2020  ses = {.        
-0002e160: 2020 2020 2733 273a 2027 7265 6a65 6374      '3': 'reject
-0002e170: 6564 272c 2020 2320 2752 656a 6563 7465  ed',  # 'Rejecte
-0002e180: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-0002e190: 2736 273a 2027 6361 6e63 656c 6564 272c  '6': 'canceled',
-0002e1a0: 2020 2320 2747 6f74 2065 7272 6f72 2061    # 'Got error a
-0002e1b0: 6e64 2077 6169 7420 666f 7220 7265 636f  nd wait for reco
-0002e1c0: 7665 7279 272c 0a20 2020 2020 2020 2020  very',.         
-0002e1d0: 2020 2027 3130 273a 2027 6f6b 272c 2020     '10': 'ok',  
-0002e1e0: 2320 2753 7563 6365 7373 272c 0a20 2020  # 'Success',.   
-0002e1f0: 2020 2020 2020 2020 2027 3131 273a 2027           '11': '
-0002e200: 6661 696c 6564 272c 2020 2320 2746 6169  failed',  # 'Fai
-0002e210: 6c65 6427 2c0a 2020 2020 2020 2020 7d0a  led',.        }.
-0002e220: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002e230: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
-0002e240: 7374 6174 7573 6573 2c20 7374 6174 7573  statuses, status
-0002e250: 2c20 7374 6174 7573 290a 0a20 2020 2061  , status)..    a
-0002e260: 7379 6e63 2064 6566 2066 6574 6368 5f66  sync def fetch_f
-0002e270: 756e 6469 6e67 5f72 6174 655f 6869 7374  unding_rate_hist
-0002e280: 6f72 7928 7365 6c66 2c20 7379 6d62 6f6c  ory(self, symbol
-0002e290: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0002e2a0: 3d20 4e6f 6e65 2c20 7369 6e63 653a 204f  = None, since: O
-0002e2b0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0002e2c0: 6f6e 652c 206c 696d 6974 3a20 4f70 7469  one, limit: Opti
-0002e2d0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-0002e2e0: 2c20 7061 7261 6d73 3d7b 7d29 3a0a 2020  , params={}):.  
-0002e2f0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-0002e300: 5f72 6571 7569 7265 645f 7379 6d62 6f6c  _required_symbol
-0002e310: 2827 6665 7463 6846 756e 6469 6e67 5261  ('fetchFundingRa
-0002e320: 7465 4869 7374 6f72 7927 2c20 7379 6d62  teHistory', symb
-0002e330: 6f6c 290a 2020 2020 2020 2020 6177 6169  ol).        awai
-0002e340: 7420 7365 6c66 2e6c 6f61 645f 6d61 726b  t self.load_mark
-0002e350: 6574 7328 290a 2020 2020 2020 2020 6d61  ets().        ma
-0002e360: 726b 6574 203d 2073 656c 662e 6d61 726b  rket = self.mark
-0002e370: 6574 2873 796d 626f 6c29 0a20 2020 2020  et(symbol).     
-0002e380: 2020 2069 7355 7364 7453 6574 746c 6564     isUsdtSettled
-0002e390: 203d 206d 6172 6b65 745b 2773 6574 746c   = market['settl
-0002e3a0: 6527 5d20 3d3d 2027 5553 4454 270a 2020  e'] == 'USDT'.  
-0002e3b0: 2020 2020 2020 6966 206e 6f74 206d 6172        if not mar
-0002e3c0: 6b65 745b 2773 7761 7027 5d3a 0a20 2020  ket['swap']:.   
-0002e3d0: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
-0002e3e0: 6164 5265 7175 6573 7428 7365 6c66 2e69  adRequest(self.i
-0002e3f0: 6420 2b20 2720 6665 7463 6846 756e 6469  d + ' fetchFundi
-0002e400: 6e67 5261 7465 4869 7374 6f72 7928 2920  ngRateHistory() 
-0002e410: 7375 7070 6f72 7473 2073 7761 7020 636f  supports swap co
-0002e420: 6e74 7261 6374 7320 6f6e 6c79 2729 0a20  ntracts only'). 
-0002e430: 2020 2020 2020 2063 7573 746f 6d53 796d         customSym
-0002e440: 626f 6c20 3d20 4e6f 6e65 0a20 2020 2020  bol = None.     
-0002e450: 2020 2069 6620 6973 5573 6474 5365 7474     if isUsdtSett
-0002e460: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-0002e470: 2063 7573 746f 6d53 796d 626f 6c20 3d20   customSymbol = 
-0002e480: 272e 2720 2b20 6d61 726b 6574 5b27 6964  '.' + market['id
-0002e490: 275d 202b 2027 4652 3848 2720 2023 2070  '] + 'FR8H'  # p
-0002e4a0: 6865 6d65 7820 7265 7175 6972 6573 2061  hemex requires a
-0002e4b0: 2063 7573 746f 6d20 7379 6d62 6f6c 2066   custom symbol f
-0002e4c0: 6f72 2066 756e 6469 6e67 2072 6174 6520  or funding rate 
-0002e4d0: 6869 7374 6f72 790a 2020 2020 2020 2020  history.        
-0002e4e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0002e4f0: 2020 6375 7374 6f6d 5379 6d62 6f6c 203d    customSymbol =
-0002e500: 2027 2e27 202b 206d 6172 6b65 745b 2762   '.' + market['b
-0002e510: 6173 6549 6427 5d20 2b20 2746 5238 4827  aseId'] + 'FR8H'
-0002e520: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0002e530: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0002e540: 2027 7379 6d62 6f6c 273a 2063 7573 746f   'symbol': custo
-0002e550: 6d53 796d 626f 6c2c 0a20 2020 2020 2020  mSymbol,.       
-0002e560: 207d 0a20 2020 2020 2020 2069 6620 7369   }.        if si
-0002e570: 6e63 6520 6973 206e 6f74 204e 6f6e 653a  nce is not None:
-0002e580: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-0002e590: 7565 7374 5b27 7374 6172 7427 5d20 3d20  uest['start'] = 
-0002e5a0: 7369 6e63 650a 2020 2020 2020 2020 6966  since.        if
-0002e5b0: 206c 696d 6974 2069 7320 6e6f 7420 4e6f   limit is not No
-0002e5c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002e5d0: 7265 7175 6573 745b 276c 696d 6974 275d  request['limit']
-0002e5e0: 203d 206c 696d 6974 0a20 2020 2020 2020   = limit.       
-0002e5f0: 2072 6573 706f 6e73 6520 3d20 4e6f 6e65   response = None
-0002e600: 0a20 2020 2020 2020 2069 6620 6973 5573  .        if isUs
-0002e610: 6474 5365 7474 6c65 643a 0a20 2020 2020  dtSettled:.     
-0002e620: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0002e630: 3d20 6177 6169 7420 7365 6c66 2e76 3247  = await self.v2G
-0002e640: 6574 4170 6944 6174 6150 7562 6c69 6344  etApiDataPublicD
-0002e650: 6174 6146 756e 6469 6e67 5261 7465 4869  ataFundingRateHi
-0002e660: 7374 6f72 7928 7365 6c66 2e65 7874 656e  story(self.exten
-0002e670: 6428 7265 7175 6573 742c 2070 6172 616d  d(request, param
-0002e680: 7329 290a 2020 2020 2020 2020 656c 7365  s)).        else
-0002e690: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002e6a0: 7370 6f6e 7365 203d 2061 7761 6974 2073  sponse = await s
-0002e6b0: 656c 662e 7631 4765 7441 7069 4461 7461  elf.v1GetApiData
-0002e6c0: 5075 626c 6963 4461 7461 4675 6e64 696e  PublicDataFundin
-0002e6d0: 6752 6174 6548 6973 746f 7279 2873 656c  gRateHistory(sel
-0002e6e0: 662e 6578 7465 6e64 2872 6571 7565 7374  f.extend(request
-0002e6f0: 2c20 7061 7261 6d73 2929 0a20 2020 2020  , params)).     
-0002e700: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-0002e710: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-0002e720: 2020 2020 2022 636f 6465 223a 2230 222c       "code":"0",
-0002e730: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0002e740: 2020 226d 7367 223a 224f 4b22 2c0a 2020    "msg":"OK",.  
-0002e750: 2020 2020 2020 2320 2020 2020 2020 2022        #        "
-0002e760: 6461 7461 223a 7b0a 2020 2020 2020 2020  data":{.        
-0002e770: 2320 2020 2020 2020 2020 2020 2272 6f77  #           "row
-0002e780: 7322 3a5b 0a20 2020 2020 2020 2023 2020  s":[.        #  
-0002e790: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-0002e7a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0002e7b0: 2020 2020 2020 2020 2273 796d 626f 6c22          "symbol"
-0002e7c0: 3a22 2e42 5443 5553 4454 4652 3848 222c  :".BTCUSDTFR8H",
-0002e7d0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0002e7e0: 2020 2020 2020 2020 2020 2022 6675 6e64             "fund
-0002e7f0: 696e 6752 6174 6522 3a22 302e 3030 3031  ingRate":"0.0001
-0002e800: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0002e810: 2020 2020 2020 2020 2020 2020 2022 6675               "fu
-0002e820: 6e64 696e 6754 696d 6522 3a22 3136 3832  ndingTime":"1682
-0002e830: 3036 3430 3030 3030 3022 2c0a 2020 2020  064000000",.    
-0002e840: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0002e850: 2020 2020 2020 2269 6e74 6572 7661 6c53        "intervalS
-0002e860: 6563 6f6e 6473 223a 2232 3838 3030 220a  econds":"28800".
-0002e870: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002e880: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0002e890: 2023 2020 2020 2020 2020 2020 205d 0a20   #           ]. 
-0002e8a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002e8b0: 7d0a 2020 2020 2020 2020 2320 2020 207d  }.        #    }
-0002e8c0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0002e8d0: 2020 2064 6174 6120 3d20 7365 6c66 2e73     data = self.s
-0002e8e0: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
-0002e8f0: 7365 2c20 2764 6174 6127 2c20 7b7d 290a  se, 'data', {}).
-0002e900: 2020 2020 2020 2020 7261 7465 7320 3d20          rates = 
-0002e910: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0002e920: 6461 7461 2c20 2772 6f77 7327 290a 2020  data, 'rows').  
-0002e930: 2020 2020 2020 7265 7375 6c74 203d 205b        result = [
-0002e940: 5d0a 2020 2020 2020 2020 666f 7220 6920  ].        for i 
-0002e950: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
-0002e960: 7261 7465 7329 293a 0a20 2020 2020 2020  rates)):.       
-0002e970: 2020 2020 2069 7465 6d20 3d20 7261 7465       item = rate
-0002e980: 735b 695d 0a20 2020 2020 2020 2020 2020  s[i].           
-0002e990: 2074 696d 6573 7461 6d70 203d 2073 656c   timestamp = sel
-0002e9a0: 662e 7361 6665 5f69 6e74 6567 6572 2869  f.safe_integer(i
-0002e9b0: 7465 6d2c 2027 6675 6e64 696e 6754 696d  tem, 'fundingTim
-0002e9c0: 6527 290a 2020 2020 2020 2020 2020 2020  e').            
-0002e9d0: 7265 7375 6c74 2e61 7070 656e 6428 7b0a  result.append({.
-0002e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e9f0: 2769 6e66 6f27 3a20 6974 656d 2c0a 2020  'info': item,.  
-0002ea00: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0002ea10: 796d 626f 6c27 3a20 7379 6d62 6f6c 2c0a  ymbol': symbol,.
-0002ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ea30: 2766 756e 6469 6e67 5261 7465 273a 2073  'fundingRate': s
-0002ea40: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
-0002ea50: 6974 656d 2c20 2766 756e 6469 6e67 5261  item, 'fundingRa
-0002ea60: 7465 2729 2c0a 2020 2020 2020 2020 2020  te'),.          
-0002ea70: 2020 2020 2020 2774 696d 6573 7461 6d70        'timestamp
-0002ea80: 273a 2074 696d 6573 7461 6d70 2c0a 2020  ': timestamp,.  
-0002ea90: 2020 2020 2020 2020 2020 2020 2020 2764                'd
-0002eaa0: 6174 6574 696d 6527 3a20 7365 6c66 2e69  atetime': self.i
-0002eab0: 736f 3836 3031 2874 696d 6573 7461 6d70  so8601(timestamp
-0002eac0: 292c 0a20 2020 2020 2020 2020 2020 207d  ),.            }
-0002ead0: 290a 2020 2020 2020 2020 736f 7274 6564  ).        sorted
-0002eae0: 203d 2073 656c 662e 736f 7274 5f62 7928   = self.sort_by(
-0002eaf0: 7265 7375 6c74 2c20 2774 696d 6573 7461  result, 'timesta
-0002eb00: 6d70 2729 0a20 2020 2020 2020 2072 6574  mp').        ret
-0002eb10: 7572 6e20 7365 6c66 2e66 696c 7465 725f  urn self.filter_
-0002eb20: 6279 5f73 796d 626f 6c5f 7369 6e63 655f  by_symbol_since_
-0002eb30: 6c69 6d69 7428 736f 7274 6564 2c20 7379  limit(sorted, sy
-0002eb40: 6d62 6f6c 2c20 7369 6e63 652c 206c 696d  mbol, since, lim
-0002eb50: 6974 290a 0a20 2020 2064 6566 2068 616e  it)..    def han
-0002eb60: 646c 655f 6572 726f 7273 2873 656c 662c  dle_errors(self,
-0002eb70: 2068 7474 7043 6f64 652c 2072 6561 736f   httpCode, reaso
-0002eb80: 6e2c 2075 726c 2c20 6d65 7468 6f64 2c20  n, url, method, 
-0002eb90: 6865 6164 6572 732c 2062 6f64 792c 2072  headers, body, r
-0002eba0: 6573 706f 6e73 652c 2072 6571 7565 7374  esponse, request
-0002ebb0: 4865 6164 6572 732c 2072 6571 7565 7374  Headers, request
-0002ebc0: 426f 6479 293a 0a20 2020 2020 2020 2069  Body):.        i
-0002ebd0: 6620 7265 7370 6f6e 7365 2069 7320 4e6f  f response is No
-0002ebe0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002ebf0: 7265 7475 726e 204e 6f6e 6520 2023 2066  return None  # f
-0002ec00: 616c 6c62 6163 6b20 746f 2064 6566 6175  allback to defau
-0002ec10: 6c74 2065 7272 6f72 2068 616e 646c 6572  lt error handler
-0002ec20: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0002ec30: 2020 2023 2020 2020 207b 2263 6f64 6522     #     {"code"
-0002ec40: 3a33 3030 3138 2c22 6d73 6722 3a22 7068  :30018,"msg":"ph
-0002ec50: 656d 6578 2e64 6174 612e 7369 7a65 2e75  emex.data.size.u
-0002ec60: 706c 696d 7422 2c22 6461 7461 223a 6e75  plimt","data":nu
-0002ec70: 6c6c 7d0a 2020 2020 2020 2020 2320 2020  ll}.        #   
-0002ec80: 2020 7b22 636f 6465 223a 3431 322c 226d    {"code":412,"m
-0002ec90: 7367 223a 224d 6973 7369 6e67 2070 6172  sg":"Missing par
-0002eca0: 616d 6574 6572 202d 2072 6573 6f6c 7574  ameter - resolut
-0002ecb0: 696f 6e22 2c22 6461 7461 223a 6e75 6c6c  ion","data":null
-0002ecc0: 7d0a 2020 2020 2020 2020 2320 2020 2020  }.        #     
-0002ecd0: 7b22 636f 6465 223a 3431 322c 226d 7367  {"code":412,"msg
-0002ece0: 223a 224d 6973 7369 6e67 2070 6172 616d  ":"Missing param
-0002ecf0: 6574 6572 202d 2074 6f22 2c22 6461 7461  eter - to","data
-0002ed00: 223a 6e75 6c6c 7d0a 2020 2020 2020 2020  ":null}.        
-0002ed10: 2320 2020 2020 7b22 6572 726f 7222 3a7b  #     {"error":{
-0002ed20: 2263 6f64 6522 3a36 3030 312c 226d 6573  "code":6001,"mes
-0002ed30: 7361 6765 223a 2269 6e76 616c 6964 2061  sage":"invalid a
-0002ed40: 7267 756d 656e 7422 7d2c 2269 6422 3a6e  rgument"},"id":n
-0002ed50: 756c 6c2c 2272 6573 756c 7422 3a6e 756c  ull,"result":nul
-0002ed60: 6c7d 0a20 2020 2020 2020 2023 0a20 2020  l}.        #.   
-0002ed70: 2020 2020 2065 7272 6f72 203d 2073 656c       error = sel
-0002ed80: 662e 7361 6665 5f76 616c 7565 2872 6573  f.safe_value(res
-0002ed90: 706f 6e73 652c 2027 6572 726f 7227 2c20  ponse, 'error', 
-0002eda0: 7265 7370 6f6e 7365 290a 2020 2020 2020  response).      
-0002edb0: 2020 6572 726f 7243 6f64 6520 3d20 7365    errorCode = se
-0002edc0: 6c66 2e73 6166 655f 7374 7269 6e67 2865  lf.safe_string(e
-0002edd0: 7272 6f72 2c20 2763 6f64 6527 290a 2020  rror, 'code').  
-0002ede0: 2020 2020 2020 6d65 7373 6167 6520 3d20        message = 
-0002edf0: 7365 6c66 2e73 6166 655f 7374 7269 6e67  self.safe_string
-0002ee00: 2865 7272 6f72 2c20 276d 7367 2729 0a20  (error, 'msg'). 
-0002ee10: 2020 2020 2020 2069 6620 2865 7272 6f72         if (error
-0002ee20: 436f 6465 2069 7320 6e6f 7420 4e6f 6e65  Code is not None
-0002ee30: 2920 616e 6420 2865 7272 6f72 436f 6465  ) and (errorCode
-0002ee40: 2021 3d20 2730 2729 3a0a 2020 2020 2020   != '0'):.      
-0002ee50: 2020 2020 2020 6665 6564 6261 636b 203d        feedback =
-0002ee60: 2073 656c 662e 6964 202b 2027 2027 202b   self.id + ' ' +
-0002ee70: 2062 6f64 790a 2020 2020 2020 2020 2020   body.          
-0002ee80: 2020 7365 6c66 2e74 6872 6f77 5f65 7861    self.throw_exa
-0002ee90: 6374 6c79 5f6d 6174 6368 6564 5f65 7863  ctly_matched_exc
-0002eea0: 6570 7469 6f6e 2873 656c 662e 6578 6365  eption(self.exce
-0002eeb0: 7074 696f 6e73 5b27 6578 6163 7427 5d2c  ptions['exact'],
-0002eec0: 2065 7272 6f72 436f 6465 2c20 6665 6564   errorCode, feed
-0002eed0: 6261 636b 290a 2020 2020 2020 2020 2020  back).          
-0002eee0: 2020 7365 6c66 2e74 6872 6f77 5f62 726f    self.throw_bro
-0002eef0: 6164 6c79 5f6d 6174 6368 6564 5f65 7863  adly_matched_exc
-0002ef00: 6570 7469 6f6e 2873 656c 662e 6578 6365  eption(self.exce
-0002ef10: 7074 696f 6e73 5b27 6272 6f61 6427 5d2c  ptions['broad'],
-0002ef20: 206d 6573 7361 6765 2c20 6665 6564 6261   message, feedba
-0002ef30: 636b 290a 2020 2020 2020 2020 2020 2020  ck).            
-0002ef40: 7261 6973 6520 4578 6368 616e 6765 4572  raise ExchangeEr
-0002ef50: 726f 7228 6665 6564 6261 636b 2920 2023  ror(feedback)  #
-0002ef60: 2075 6e6b 6e6f 776e 206d 6573 7361 6765   unknown message
-0002ef70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002ef80: 4e6f 6e65 0a                             None.
+0002dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dc50: 2273 6964 6522 3a20 322c 0a20 2020 2020  "side": 2,.     
+0002dc60: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0002dc70: 2020 2020 2020 2020 2022 7374 6174 7573           "status
+0002dc80: 223a 2031 302c 0a20 2020 2020 2020 2023  ": 10,.        #
+0002dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dca0: 2020 2020 2022 6372 6561 7465 5469 6d65       "createTime
+0002dcb0: 223a 2031 3635 3238 3332 3436 3730 3030  ": 1652832467000
+0002dcc0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0002dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dce0: 2262 697a 5479 7065 223a 2031 300a 2020  "bizType": 10.  
+0002dcf0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0002dd00: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0002dd10: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0002dd20: 5d0a 2020 2020 2020 2020 2320 2020 2020  ].        #     
+0002dd30: 2020 2020 7d0a 2020 2020 2020 2020 2320      }.        # 
+0002dd40: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
+0002dd50: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+0002dd60: 656c 662e 7361 6665 5f76 616c 7565 2872  elf.safe_value(r
+0002dd70: 6573 706f 6e73 652c 2027 6461 7461 272c  esponse, 'data',
+0002dd80: 207b 7d29 0a20 2020 2020 2020 2074 7261   {}).        tra
+0002dd90: 6e73 6665 7273 203d 2073 656c 662e 7361  nsfers = self.sa
+0002dda0: 6665 5f76 616c 7565 2864 6174 612c 2027  fe_value(data, '
+0002ddb0: 726f 7773 272c 205b 5d29 0a20 2020 2020  rows', []).     
+0002ddc0: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
+0002ddd0: 6172 7365 5f74 7261 6e73 6665 7273 2874  arse_transfers(t
+0002dde0: 7261 6e73 6665 7273 2c20 6375 7272 656e  ransfers, curren
+0002ddf0: 6379 2c20 7369 6e63 652c 206c 696d 6974  cy, since, limit
+0002de00: 290a 0a20 2020 2064 6566 2070 6172 7365  )..    def parse
+0002de10: 5f74 7261 6e73 6665 7228 7365 6c66 2c20  _transfer(self, 
+0002de20: 7472 616e 7366 6572 2c20 6375 7272 656e  transfer, curren
+0002de30: 6379 3d4e 6f6e 6529 3a0a 2020 2020 2020  cy=None):.      
+0002de40: 2020 230a 2020 2020 2020 2020 2320 7472    #.        # tr
+0002de50: 616e 7366 6572 0a20 2020 2020 2020 2023  ansfer.        #
+0002de60: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+0002de70: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002de80: 2020 206c 696e 6b4b 6579 3a20 2738 3536     linkKey: '856
+0002de90: 3465 6261 342d 6339 6563 2d34 3964 362d  4eba4-c9ec-49d6-
+0002dea0: 3962 3863 2d32 6563 3530 3031 6130 6662  9b8c-2ec5001a0fb
+0002deb0: 3927 2c0a 2020 2020 2020 2020 2320 2020  9',.        #   
+0002dec0: 2020 2020 2020 7573 6572 4964 3a20 2734        userId: '4
+0002ded0: 3031 3833 3430 272c 0a20 2020 2020 2020  018340',.       
+0002dee0: 2023 2020 2020 2020 2020 2063 7572 7265   #         curre
+0002def0: 6e63 793a 2027 5553 4427 2c0a 2020 2020  ncy: 'USD',.    
+0002df00: 2020 2020 2320 2020 2020 2020 2020 616d      #         am
+0002df10: 6f75 6e74 4576 3a20 2731 3027 2c0a 2020  ountEv: '10',.  
+0002df20: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0002df30: 7369 6465 3a20 2732 272c 0a20 2020 2020  side: '2',.     
+0002df40: 2020 2023 2020 2020 2020 2020 2073 7461     #         sta
+0002df50: 7475 733a 2027 3130 270a 2020 2020 2020  tus: '10'.      
+0002df60: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
+0002df70: 2020 230a 2020 2020 2020 2020 2320 6665    #.        # fe
+0002df80: 7463 6854 7261 6e73 6665 7273 0a20 2020  tchTransfers.   
+0002df90: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+0002dfa0: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
+0002dfb0: 2020 2020 2020 2020 2022 6c69 6e6b 4b65           "linkKe
+0002dfc0: 7922 3a20 2238 3763 3037 3161 332d 3836  y": "87c071a3-86
+0002dfd0: 3238 2d34 6163 322d 6163 6131 2d36 6365  28-4ac2-aca1-6ce
+0002dfe0: 3064 3166 6164 3636 6322 2c0a 2020 2020  0d1fad66c",.    
+0002dff0: 2020 2020 2320 2020 2020 2020 2020 2275      #         "u
+0002e000: 7365 7249 6422 3a20 3431 3438 3432 382c  serId": 4148428,
+0002e010: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002e020: 2020 2022 6375 7272 656e 6379 223a 2022     "currency": "
+0002e030: 4254 4322 2c0a 2020 2020 2020 2020 2320  BTC",.        # 
+0002e040: 2020 2020 2020 2020 2261 6d6f 756e 7445          "amountE
+0002e050: 7622 3a20 3637 3933 322c 0a20 2020 2020  v": 67932,.     
+0002e060: 2020 2023 2020 2020 2020 2020 2022 7369     #         "si
+0002e070: 6465 223a 2032 2c0a 2020 2020 2020 2020  de": 2,.        
+0002e080: 2320 2020 2020 2020 2020 2273 7461 7475  #         "statu
+0002e090: 7322 3a20 3130 2c0a 2020 2020 2020 2020  s": 10,.        
+0002e0a0: 2320 2020 2020 2020 2020 2263 7265 6174  #         "creat
+0002e0b0: 6554 696d 6522 3a20 3136 3532 3833 3234  eTime": 16528324
+0002e0c0: 3637 3030 302c 0a20 2020 2020 2020 2023  67000,.        #
+0002e0d0: 2020 2020 2020 2020 2022 6269 7a54 7970           "bizTyp
+0002e0e0: 6522 3a20 3130 0a20 2020 2020 2020 2023  e": 10.        #
+0002e0f0: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
+0002e100: 0a20 2020 2020 2020 2069 6420 3d20 7365  .        id = se
+0002e110: 6c66 2e73 6166 655f 7374 7269 6e67 2874  lf.safe_string(t
+0002e120: 7261 6e73 6665 722c 2027 6c69 6e6b 4b65  ransfer, 'linkKe
+0002e130: 7927 290a 2020 2020 2020 2020 7374 6174  y').        stat
+0002e140: 7573 203d 2073 656c 662e 7361 6665 5f73  us = self.safe_s
+0002e150: 7472 696e 6728 7472 616e 7366 6572 2c20  tring(transfer, 
+0002e160: 2773 7461 7475 7327 290a 2020 2020 2020  'status').      
+0002e170: 2020 616d 6f75 6e74 4576 203d 2073 656c    amountEv = sel
+0002e180: 662e 7361 6665 5f73 7472 696e 6728 7472  f.safe_string(tr
+0002e190: 616e 7366 6572 2c20 2761 6d6f 756e 7445  ansfer, 'amountE
+0002e1a0: 7627 290a 2020 2020 2020 2020 616d 6f75  v').        amou
+0002e1b0: 6e74 5472 616e 7366 6572 6564 203d 2073  ntTransfered = s
+0002e1c0: 656c 662e 6672 6f6d 5f65 7628 616d 6f75  elf.from_ev(amou
+0002e1d0: 6e74 4576 2c20 6375 7272 656e 6379 290a  ntEv, currency).
+0002e1e0: 2020 2020 2020 2020 6375 7272 656e 6379          currency
+0002e1f0: 4964 203d 2073 656c 662e 7361 6665 5f73  Id = self.safe_s
+0002e200: 7472 696e 6728 7472 616e 7366 6572 2c20  tring(transfer, 
+0002e210: 2763 7572 7265 6e63 7927 290a 2020 2020  'currency').    
+0002e220: 2020 2020 636f 6465 203d 2073 656c 662e      code = self.
+0002e230: 7361 6665 5f63 7572 7265 6e63 795f 636f  safe_currency_co
+0002e240: 6465 2863 7572 7265 6e63 7949 642c 2063  de(currencyId, c
+0002e250: 7572 7265 6e63 7929 0a20 2020 2020 2020  urrency).       
+0002e260: 2073 6964 6520 3d20 7365 6c66 2e73 6166   side = self.saf
+0002e270: 655f 696e 7465 6765 7228 7472 616e 7366  e_integer(transf
+0002e280: 6572 2c20 2773 6964 6527 290a 2020 2020  er, 'side').    
+0002e290: 2020 2020 6672 6f6d 4964 203d 204e 6f6e      fromId = Non
+0002e2a0: 650a 2020 2020 2020 2020 746f 4964 203d  e.        toId =
+0002e2b0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+0002e2c0: 2073 6964 6520 3d3d 2031 3a0a 2020 2020   side == 1:.    
+0002e2d0: 2020 2020 2020 2020 6672 6f6d 4964 203d          fromId =
+0002e2e0: 2027 7377 6170 270a 2020 2020 2020 2020   'swap'.        
+0002e2f0: 2020 2020 746f 4964 203d 2027 7370 6f74      toId = 'spot
+0002e300: 270a 2020 2020 2020 2020 656c 6966 2073  '.        elif s
+0002e310: 6964 6520 3d3d 2032 3a0a 2020 2020 2020  ide == 2:.      
+0002e320: 2020 2020 2020 6672 6f6d 4964 203d 2027        fromId = '
+0002e330: 7370 6f74 270a 2020 2020 2020 2020 2020  spot'.          
+0002e340: 2020 746f 4964 203d 2027 7377 6170 270a    toId = 'swap'.
+0002e350: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+0002e360: 7020 3d20 7365 6c66 2e73 6166 655f 696e  p = self.safe_in
+0002e370: 7465 6765 7228 7472 616e 7366 6572 2c20  teger(transfer, 
+0002e380: 2763 7265 6174 6554 696d 6527 290a 2020  'createTime').  
+0002e390: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+0002e3a0: 2020 2020 2020 2020 2020 2027 696e 666f             'info
+0002e3b0: 273a 2074 7261 6e73 6665 722c 0a20 2020  ': transfer,.   
+0002e3c0: 2020 2020 2020 2020 2027 6964 273a 2069           'id': i
+0002e3d0: 642c 0a20 2020 2020 2020 2020 2020 2027  d,.            '
+0002e3e0: 7469 6d65 7374 616d 7027 3a20 7469 6d65  timestamp': time
+0002e3f0: 7374 616d 702c 0a20 2020 2020 2020 2020  stamp,.         
+0002e400: 2020 2027 6461 7465 7469 6d65 273a 2073     'datetime': s
+0002e410: 656c 662e 6973 6f38 3630 3128 7469 6d65  elf.iso8601(time
+0002e420: 7374 616d 7029 2c0a 2020 2020 2020 2020  stamp),.        
+0002e430: 2020 2020 2763 7572 7265 6e63 7927 3a20      'currency': 
+0002e440: 636f 6465 2c0a 2020 2020 2020 2020 2020  code,.          
+0002e450: 2020 2761 6d6f 756e 7427 3a20 616d 6f75    'amount': amou
+0002e460: 6e74 5472 616e 7366 6572 6564 2c0a 2020  ntTransfered,.  
+0002e470: 2020 2020 2020 2020 2020 2766 726f 6d41            'fromA
+0002e480: 6363 6f75 6e74 273a 2066 726f 6d49 642c  ccount': fromId,
+0002e490: 0a20 2020 2020 2020 2020 2020 2027 746f  .            'to
+0002e4a0: 4163 636f 756e 7427 3a20 746f 4964 2c0a  Account': toId,.
+0002e4b0: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
+0002e4c0: 7475 7327 3a20 7365 6c66 2e70 6172 7365  tus': self.parse
+0002e4d0: 5f74 7261 6e73 6665 725f 7374 6174 7573  _transfer_status
+0002e4e0: 2873 7461 7475 7329 2c0a 2020 2020 2020  (status),.      
+0002e4f0: 2020 7d0a 0a20 2020 2064 6566 2070 6172    }..    def par
+0002e500: 7365 5f74 7261 6e73 6665 725f 7374 6174  se_transfer_stat
+0002e510: 7573 2873 656c 662c 2073 7461 7475 7329  us(self, status)
+0002e520: 3a0a 2020 2020 2020 2020 7374 6174 7573  :.        status
+0002e530: 6573 203d 207b 0a20 2020 2020 2020 2020  es = {.         
+0002e540: 2020 2027 3327 3a20 2772 656a 6563 7465     '3': 'rejecte
+0002e550: 6427 2c20 2023 2027 5265 6a65 6374 6564  d',  # 'Rejected
+0002e560: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+0002e570: 3627 3a20 2763 616e 6365 6c65 6427 2c20  6': 'canceled', 
+0002e580: 2023 2027 476f 7420 6572 726f 7220 616e   # 'Got error an
+0002e590: 6420 7761 6974 2066 6f72 2072 6563 6f76  d wait for recov
+0002e5a0: 6572 7927 2c0a 2020 2020 2020 2020 2020  ery',.          
+0002e5b0: 2020 2731 3027 3a20 276f 6b27 2c20 2023    '10': 'ok',  #
+0002e5c0: 2027 5375 6363 6573 7327 2c0a 2020 2020   'Success',.    
+0002e5d0: 2020 2020 2020 2020 2731 3127 3a20 2766          '11': 'f
+0002e5e0: 6169 6c65 6427 2c20 2023 2027 4661 696c  ailed',  # 'Fail
+0002e5f0: 6564 272c 0a20 2020 2020 2020 207d 0a20  ed',.        }. 
+0002e600: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0002e610: 6c66 2e73 6166 655f 7374 7269 6e67 2873  lf.safe_string(s
+0002e620: 7461 7475 7365 732c 2073 7461 7475 732c  tatuses, status,
+0002e630: 2073 7461 7475 7329 0a0a 2020 2020 6173   status)..    as
+0002e640: 796e 6320 6465 6620 6665 7463 685f 6675  ync def fetch_fu
+0002e650: 6e64 696e 675f 7261 7465 5f68 6973 746f  nding_rate_histo
+0002e660: 7279 2873 656c 662c 2073 796d 626f 6c3a  ry(self, symbol:
+0002e670: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0002e680: 204e 6f6e 652c 2073 696e 6365 3a20 4f70   None, since: Op
+0002e690: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0002e6a0: 6e65 2c20 6c69 6d69 743a 204f 7074 696f  ne, limit: Optio
+0002e6b0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+0002e6c0: 2070 6172 616d 733d 7b7d 293a 0a20 2020   params={}):.   
+0002e6d0: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
+0002e6e0: 7265 7175 6972 6564 5f73 796d 626f 6c28  required_symbol(
+0002e6f0: 2766 6574 6368 4675 6e64 696e 6752 6174  'fetchFundingRat
+0002e700: 6548 6973 746f 7279 272c 2073 796d 626f  eHistory', symbo
+0002e710: 6c29 0a20 2020 2020 2020 2061 7761 6974  l).        await
+0002e720: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
+0002e730: 7473 2829 0a20 2020 2020 2020 206d 6172  ts().        mar
+0002e740: 6b65 7420 3d20 7365 6c66 2e6d 6172 6b65  ket = self.marke
+0002e750: 7428 7379 6d62 6f6c 290a 2020 2020 2020  t(symbol).      
+0002e760: 2020 6973 5573 6474 5365 7474 6c65 6420    isUsdtSettled 
+0002e770: 3d20 6d61 726b 6574 5b27 7365 7474 6c65  = market['settle
+0002e780: 275d 203d 3d20 2755 5344 5427 0a20 2020  '] == 'USDT'.   
+0002e790: 2020 2020 2069 6620 6e6f 7420 6d61 726b       if not mark
+0002e7a0: 6574 5b27 7377 6170 275d 3a0a 2020 2020  et['swap']:.    
+0002e7b0: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+0002e7c0: 6452 6571 7565 7374 2873 656c 662e 6964  dRequest(self.id
+0002e7d0: 202b 2027 2066 6574 6368 4675 6e64 696e   + ' fetchFundin
+0002e7e0: 6752 6174 6548 6973 746f 7279 2829 2073  gRateHistory() s
+0002e7f0: 7570 706f 7274 7320 7377 6170 2063 6f6e  upports swap con
+0002e800: 7472 6163 7473 206f 6e6c 7927 290a 2020  tracts only').  
+0002e810: 2020 2020 2020 6375 7374 6f6d 5379 6d62        customSymb
+0002e820: 6f6c 203d 204e 6f6e 650a 2020 2020 2020  ol = None.      
+0002e830: 2020 6966 2069 7355 7364 7453 6574 746c    if isUsdtSettl
+0002e840: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+0002e850: 6375 7374 6f6d 5379 6d62 6f6c 203d 2027  customSymbol = '
+0002e860: 2e27 202b 206d 6172 6b65 745b 2769 6427  .' + market['id'
+0002e870: 5d20 2b20 2746 5238 4827 2020 2320 7068  ] + 'FR8H'  # ph
+0002e880: 656d 6578 2072 6571 7569 7265 7320 6120  emex requires a 
+0002e890: 6375 7374 6f6d 2073 796d 626f 6c20 666f  custom symbol fo
+0002e8a0: 7220 6675 6e64 696e 6720 7261 7465 2068  r funding rate h
+0002e8b0: 6973 746f 7279 0a20 2020 2020 2020 2065  istory.        e
+0002e8c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002e8d0: 2063 7573 746f 6d53 796d 626f 6c20 3d20   customSymbol = 
+0002e8e0: 272e 2720 2b20 6d61 726b 6574 5b27 6261  '.' + market['ba
+0002e8f0: 7365 4964 275d 202b 2027 4652 3848 270a  seId'] + 'FR8H'.
+0002e900: 2020 2020 2020 2020 7265 7175 6573 7420          request 
+0002e910: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0002e920: 2773 796d 626f 6c27 3a20 6375 7374 6f6d  'symbol': custom
+0002e930: 5379 6d62 6f6c 2c0a 2020 2020 2020 2020  Symbol,.        
+0002e940: 7d0a 2020 2020 2020 2020 6966 2073 696e  }.        if sin
+0002e950: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ce is not None:.
+0002e960: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0002e970: 6573 745b 2773 7461 7274 275d 203d 2073  est['start'] = s
+0002e980: 696e 6365 0a20 2020 2020 2020 2069 6620  ince.        if 
+0002e990: 6c69 6d69 7420 6973 206e 6f74 204e 6f6e  limit is not Non
+0002e9a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002e9b0: 6571 7565 7374 5b27 6c69 6d69 7427 5d20  equest['limit'] 
+0002e9c0: 3d20 6c69 6d69 740a 2020 2020 2020 2020  = limit.        
+0002e9d0: 7265 7370 6f6e 7365 203d 204e 6f6e 650a  response = None.
+0002e9e0: 2020 2020 2020 2020 6966 2069 7355 7364          if isUsd
+0002e9f0: 7453 6574 746c 6564 3a0a 2020 2020 2020  tSettled:.      
+0002ea00: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+0002ea10: 2061 7761 6974 2073 656c 662e 7632 4765   await self.v2Ge
+0002ea20: 7441 7069 4461 7461 5075 626c 6963 4461  tApiDataPublicDa
+0002ea30: 7461 4675 6e64 696e 6752 6174 6548 6973  taFundingRateHis
+0002ea40: 746f 7279 2873 656c 662e 6578 7465 6e64  tory(self.extend
+0002ea50: 2872 6571 7565 7374 2c20 7061 7261 6d73  (request, params
+0002ea60: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
+0002ea70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002ea80: 706f 6e73 6520 3d20 6177 6169 7420 7365  ponse = await se
+0002ea90: 6c66 2e76 3147 6574 4170 6944 6174 6150  lf.v1GetApiDataP
+0002eaa0: 7562 6c69 6344 6174 6146 756e 6469 6e67  ublicDataFunding
+0002eab0: 5261 7465 4869 7374 6f72 7928 7365 6c66  RateHistory(self
+0002eac0: 2e65 7874 656e 6428 7265 7175 6573 742c  .extend(request,
+0002ead0: 2070 6172 616d 7329 290a 2020 2020 2020   params)).      
+0002eae0: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
+0002eaf0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0002eb00: 2020 2020 2263 6f64 6522 3a22 3022 2c0a      "code":"0",.
+0002eb10: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002eb20: 2022 6d73 6722 3a22 4f4b 222c 0a20 2020   "msg":"OK",.   
+0002eb30: 2020 2020 2023 2020 2020 2020 2020 2264       #        "d
+0002eb40: 6174 6122 3a7b 0a20 2020 2020 2020 2023  ata":{.        #
+0002eb50: 2020 2020 2020 2020 2020 2022 726f 7773             "rows
+0002eb60: 223a 5b0a 2020 2020 2020 2020 2320 2020  ":[.        #   
+0002eb70: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+0002eb80: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0002eb90: 2020 2020 2020 2022 7379 6d62 6f6c 223a         "symbol":
+0002eba0: 222e 4254 4355 5344 5446 5238 4822 2c0a  ".BTCUSDTFR8H",.
+0002ebb0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002ebc0: 2020 2020 2020 2020 2020 2266 756e 6469            "fundi
+0002ebd0: 6e67 5261 7465 223a 2230 2e30 3030 3122  ngRate":"0.0001"
+0002ebe0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0002ebf0: 2020 2020 2020 2020 2020 2020 2266 756e              "fun
+0002ec00: 6469 6e67 5469 6d65 223a 2231 3638 3230  dingTime":"16820
+0002ec10: 3634 3030 3030 3030 222c 0a20 2020 2020  64000000",.     
+0002ec20: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0002ec30: 2020 2020 2022 696e 7465 7276 616c 5365       "intervalSe
+0002ec40: 636f 6e64 7322 3a22 3238 3830 3022 0a20  conds":"28800". 
+0002ec50: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0002ec60: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0002ec70: 2320 2020 2020 2020 2020 2020 5d0a 2020  #           ].  
+0002ec80: 2020 2020 2020 2320 2020 2020 2020 207d        #        }
+0002ec90: 0a20 2020 2020 2020 2023 2020 2020 7d0a  .        #    }.
+0002eca0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0002ecb0: 2020 6461 7461 203d 2073 656c 662e 7361    data = self.sa
+0002ecc0: 6665 5f76 616c 7565 2872 6573 706f 6e73  fe_value(respons
+0002ecd0: 652c 2027 6461 7461 272c 207b 7d29 0a20  e, 'data', {}). 
+0002ece0: 2020 2020 2020 2072 6174 6573 203d 2073         rates = s
+0002ecf0: 656c 662e 7361 6665 5f76 616c 7565 2864  elf.safe_value(d
+0002ed00: 6174 612c 2027 726f 7773 2729 0a20 2020  ata, 'rows').   
+0002ed10: 2020 2020 2072 6573 756c 7420 3d20 5b5d       result = []
+0002ed20: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+0002ed30: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+0002ed40: 6174 6573 2929 3a0a 2020 2020 2020 2020  ates)):.        
+0002ed50: 2020 2020 6974 656d 203d 2072 6174 6573      item = rates
+0002ed60: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
+0002ed70: 7469 6d65 7374 616d 7020 3d20 7365 6c66  timestamp = self
+0002ed80: 2e73 6166 655f 696e 7465 6765 7228 6974  .safe_integer(it
+0002ed90: 656d 2c20 2766 756e 6469 6e67 5469 6d65  em, 'fundingTime
+0002eda0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+0002edb0: 6573 756c 742e 6170 7065 6e64 287b 0a20  esult.append({. 
+0002edc0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002edd0: 696e 666f 273a 2069 7465 6d2c 0a20 2020  info': item,.   
+0002ede0: 2020 2020 2020 2020 2020 2020 2027 7379               'sy
+0002edf0: 6d62 6f6c 273a 2073 796d 626f 6c2c 0a20  mbol': symbol,. 
+0002ee00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002ee10: 6675 6e64 696e 6752 6174 6527 3a20 7365  fundingRate': se
+0002ee20: 6c66 2e73 6166 655f 6e75 6d62 6572 2869  lf.safe_number(i
+0002ee30: 7465 6d2c 2027 6675 6e64 696e 6752 6174  tem, 'fundingRat
+0002ee40: 6527 292c 0a20 2020 2020 2020 2020 2020  e'),.           
+0002ee50: 2020 2020 2027 7469 6d65 7374 616d 7027       'timestamp'
+0002ee60: 3a20 7469 6d65 7374 616d 702c 0a20 2020  : timestamp,.   
+0002ee70: 2020 2020 2020 2020 2020 2020 2027 6461               'da
+0002ee80: 7465 7469 6d65 273a 2073 656c 662e 6973  tetime': self.is
+0002ee90: 6f38 3630 3128 7469 6d65 7374 616d 7029  o8601(timestamp)
+0002eea0: 2c0a 2020 2020 2020 2020 2020 2020 7d29  ,.            })
+0002eeb0: 0a20 2020 2020 2020 2073 6f72 7465 6420  .        sorted 
+0002eec0: 3d20 7365 6c66 2e73 6f72 745f 6279 2872  = self.sort_by(r
+0002eed0: 6573 756c 742c 2027 7469 6d65 7374 616d  esult, 'timestam
+0002eee0: 7027 290a 2020 2020 2020 2020 7265 7475  p').        retu
+0002eef0: 726e 2073 656c 662e 6669 6c74 6572 5f62  rn self.filter_b
+0002ef00: 795f 7379 6d62 6f6c 5f73 696e 6365 5f6c  y_symbol_since_l
+0002ef10: 696d 6974 2873 6f72 7465 642c 2073 796d  imit(sorted, sym
+0002ef20: 626f 6c2c 2073 696e 6365 2c20 6c69 6d69  bol, since, limi
+0002ef30: 7429 0a0a 2020 2020 6465 6620 6861 6e64  t)..    def hand
+0002ef40: 6c65 5f65 7272 6f72 7328 7365 6c66 2c20  le_errors(self, 
+0002ef50: 6874 7470 436f 6465 2c20 7265 6173 6f6e  httpCode, reason
+0002ef60: 2c20 7572 6c2c 206d 6574 686f 642c 2068  , url, method, h
+0002ef70: 6561 6465 7273 2c20 626f 6479 2c20 7265  eaders, body, re
+0002ef80: 7370 6f6e 7365 2c20 7265 7175 6573 7448  sponse, requestH
+0002ef90: 6561 6465 7273 2c20 7265 7175 6573 7442  eaders, requestB
+0002efa0: 6f64 7929 3a0a 2020 2020 2020 2020 6966  ody):.        if
+0002efb0: 2072 6573 706f 6e73 6520 6973 204e 6f6e   response is Non
+0002efc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002efd0: 6574 7572 6e20 4e6f 6e65 2020 2320 6661  eturn None  # fa
+0002efe0: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
+0002eff0: 7420 6572 726f 7220 6861 6e64 6c65 720a  t error handler.
+0002f000: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0002f010: 2020 2320 2020 2020 7b22 636f 6465 223a    #     {"code":
+0002f020: 3330 3031 382c 226d 7367 223a 2270 6865  30018,"msg":"phe
+0002f030: 6d65 782e 6461 7461 2e73 697a 652e 7570  mex.data.size.up
+0002f040: 6c69 6d74 222c 2264 6174 6122 3a6e 756c  limt","data":nul
+0002f050: 6c7d 0a20 2020 2020 2020 2023 2020 2020  l}.        #    
+0002f060: 207b 2263 6f64 6522 3a34 3132 2c22 6d73   {"code":412,"ms
+0002f070: 6722 3a22 4d69 7373 696e 6720 7061 7261  g":"Missing para
+0002f080: 6d65 7465 7220 2d20 7265 736f 6c75 7469  meter - resoluti
+0002f090: 6f6e 222c 2264 6174 6122 3a6e 756c 6c7d  on","data":null}
+0002f0a0: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+0002f0b0: 2263 6f64 6522 3a34 3132 2c22 6d73 6722  "code":412,"msg"
+0002f0c0: 3a22 4d69 7373 696e 6720 7061 7261 6d65  :"Missing parame
+0002f0d0: 7465 7220 2d20 746f 222c 2264 6174 6122  ter - to","data"
+0002f0e0: 3a6e 756c 6c7d 0a20 2020 2020 2020 2023  :null}.        #
+0002f0f0: 2020 2020 207b 2265 7272 6f72 223a 7b22       {"error":{"
+0002f100: 636f 6465 223a 3630 3031 2c22 6d65 7373  code":6001,"mess
+0002f110: 6167 6522 3a22 696e 7661 6c69 6420 6172  age":"invalid ar
+0002f120: 6775 6d65 6e74 227d 2c22 6964 223a 6e75  gument"},"id":nu
+0002f130: 6c6c 2c22 7265 7375 6c74 223a 6e75 6c6c  ll,"result":null
+0002f140: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
+0002f150: 2020 2020 6572 726f 7220 3d20 7365 6c66      error = self
+0002f160: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
+0002f170: 6f6e 7365 2c20 2765 7272 6f72 272c 2072  onse, 'error', r
+0002f180: 6573 706f 6e73 6529 0a20 2020 2020 2020  esponse).       
+0002f190: 2065 7272 6f72 436f 6465 203d 2073 656c   errorCode = sel
+0002f1a0: 662e 7361 6665 5f73 7472 696e 6728 6572  f.safe_string(er
+0002f1b0: 726f 722c 2027 636f 6465 2729 0a20 2020  ror, 'code').   
+0002f1c0: 2020 2020 206d 6573 7361 6765 203d 2073       message = s
+0002f1d0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0002f1e0: 6572 726f 722c 2027 6d73 6727 290a 2020  error, 'msg').  
+0002f1f0: 2020 2020 2020 6966 2028 6572 726f 7243        if (errorC
+0002f200: 6f64 6520 6973 206e 6f74 204e 6f6e 6529  ode is not None)
+0002f210: 2061 6e64 2028 6572 726f 7243 6f64 6520   and (errorCode 
+0002f220: 213d 2027 3027 293a 0a20 2020 2020 2020  != '0'):.       
+0002f230: 2020 2020 2066 6565 6462 6163 6b20 3d20       feedback = 
+0002f240: 7365 6c66 2e69 6420 2b20 2720 2720 2b20  self.id + ' ' + 
+0002f250: 626f 6479 0a20 2020 2020 2020 2020 2020  body.           
+0002f260: 2073 656c 662e 7468 726f 775f 6578 6163   self.throw_exac
+0002f270: 746c 795f 6d61 7463 6865 645f 6578 6365  tly_matched_exce
+0002f280: 7074 696f 6e28 7365 6c66 2e65 7863 6570  ption(self.excep
+0002f290: 7469 6f6e 735b 2765 7861 6374 275d 2c20  tions['exact'], 
+0002f2a0: 6572 726f 7243 6f64 652c 2066 6565 6462  errorCode, feedb
+0002f2b0: 6163 6b29 0a20 2020 2020 2020 2020 2020  ack).           
+0002f2c0: 2073 656c 662e 7468 726f 775f 6272 6f61   self.throw_broa
+0002f2d0: 646c 795f 6d61 7463 6865 645f 6578 6365  dly_matched_exce
+0002f2e0: 7074 696f 6e28 7365 6c66 2e65 7863 6570  ption(self.excep
+0002f2f0: 7469 6f6e 735b 2762 726f 6164 275d 2c20  tions['broad'], 
+0002f300: 6d65 7373 6167 652c 2066 6565 6462 6163  message, feedbac
+0002f310: 6b29 0a20 2020 2020 2020 2020 2020 2072  k).            r
+0002f320: 6169 7365 2045 7863 6861 6e67 6545 7272  aise ExchangeErr
+0002f330: 6f72 2866 6565 6462 6163 6b29 2020 2320  or(feedback)  # 
+0002f340: 756e 6b6e 6f77 6e20 6d65 7373 6167 650a  unknown message.
+0002f350: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+0002f360: 6f6e 650a                                one.
```

### Comparing `ccxt-3.1.6/ccxt/async_support/poloniex.py` & `ccxt-3.1.7/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/poloniexfutures.py` & `ccxt-3.1.7/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/probit.py` & `ccxt-3.1.7/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/ripio.py` & `ccxt-3.1.7/ccxt/async_support/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/stex.py` & `ccxt-3.1.7/ccxt/async_support/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/tidex.py` & `ccxt-3.1.7/ccxt/async_support/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/timex.py` & `ccxt-3.1.7/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/tokocrypto.py` & `ccxt-3.1.7/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/upbit.py` & `ccxt-3.1.7/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/wavesexchange.py` & `ccxt-3.1.7/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/wazirx.py` & `ccxt-3.1.7/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/whitebit.py` & `ccxt-3.1.7/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/woo.py` & `ccxt-3.1.7/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/xt.py` & `ccxt-3.1.7/ccxt/async_support/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/yobit.py` & `ccxt-3.1.7/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/zaif.py` & `ccxt-3.1.7/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/zb.py` & `ccxt-3.1.7/ccxt/async_support/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/async_support/zonda.py` & `ccxt-3.1.7/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/base/__init__.py` & `ccxt-3.1.7/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/base/decimal_to_precision.py` & `ccxt-3.1.7/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/base/errors.py` & `ccxt-3.1.7/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/base/exchange.py` & `ccxt-3.1.7/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-3.1.6/ccxt/base/precise.py` & `ccxt-3.1.7/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/base/types.py` & `ccxt-3.1.7/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bequant.py` & `ccxt-3.1.7/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bigone.py` & `ccxt-3.1.7/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/binance.py` & `ccxt-3.1.7/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/binancecoinm.py` & `ccxt-3.1.7/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/binanceus.py` & `ccxt-3.1.7/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/binanceusdm.py` & `ccxt-3.1.7/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bit2c.py` & `ccxt-3.1.7/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitbank.py` & `ccxt-3.1.7/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitbns.py` & `ccxt-3.1.7/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitfinex.py` & `ccxt-3.1.7/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitfinex2.py` & `ccxt-3.1.7/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitflyer.py` & `ccxt-3.1.7/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitforex.py` & `ccxt-3.1.7/ccxt/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitget.py` & `ccxt-3.1.7/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bithumb.py` & `ccxt-3.1.7/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitmart.py` & `ccxt-3.1.7/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitmex.py` & `ccxt-3.1.7/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitopro.py` & `ccxt-3.1.7/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitpanda.py` & `ccxt-3.1.7/ccxt/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitrue.py` & `ccxt-3.1.7/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitso.py` & `ccxt-3.1.7/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitstamp.py` & `ccxt-3.1.7/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitstamp1.py` & `ccxt-3.1.7/ccxt/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bittrex.py` & `ccxt-3.1.7/ccxt/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bitvavo.py` & `ccxt-3.1.7/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bkex.py` & `ccxt-3.1.7/ccxt/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bl3p.py` & `ccxt-3.1.7/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/blockchaincom.py` & `ccxt-3.1.7/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/btcalpha.py` & `ccxt-3.1.7/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/btcbox.py` & `ccxt-3.1.7/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/btcex.py` & `ccxt-3.1.7/ccxt/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/btcmarkets.py` & `ccxt-3.1.7/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/btctradeua.py` & `ccxt-3.1.7/ccxt/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/btcturk.py` & `ccxt-3.1.7/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/buda.py` & `ccxt-3.1.7/ccxt/buda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/bybit.py` & `ccxt-3.1.7/ccxt/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -22684,2139 +22684,2154 @@
 000589b0: 2274 696d 6522 3a20 3136 3732 3035 3335  "time": 16720535
 000589c0: 3438 3537 390a 2020 2020 2020 2020 2320  48579.        # 
 000589d0: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
 000589e0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
 000589f0: 2073 656c 662e 7361 6665 5f76 616c 7565   self.safe_value
 00058a00: 2872 6573 706f 6e73 652c 2027 7265 7375  (response, 'resu
 00058a10: 6c74 272c 207b 7d29 0a20 2020 2020 2020  lt', {}).       
-00058a20: 2069 6420 3d20 7365 6c66 2e73 6166 655f   id = self.safe_
-00058a30: 7374 7269 6e67 2872 6573 756c 742c 2027  string(result, '
-00058a40: 7379 6d62 6f6c 2729 0a20 2020 2020 2020  symbol').       
-00058a50: 206d 6172 6b65 7420 3d20 7365 6c66 2e73   market = self.s
-00058a60: 6166 655f 6d61 726b 6574 2869 642c 206d  afe_market(id, m
-00058a70: 6172 6b65 742c 204e 6f6e 652c 2027 636f  arket, None, 'co
-00058a80: 6e74 7261 6374 2729 0a20 2020 2020 2020  ntract').       
-00058a90: 2064 6174 6120 3d20 7365 6c66 2e73 6166   data = self.saf
-00058aa0: 655f 7661 6c75 6528 7265 7375 6c74 2c20  e_value(result, 
-00058ab0: 276c 6973 7427 2c20 5b5d 290a 2020 2020  'list', []).    
-00058ac0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00058ad0: 7061 7273 655f 6f70 656e 5f69 6e74 6572  parse_open_inter
-00058ae0: 6573 7473 2864 6174 612c 206d 6172 6b65  ests(data, marke
-00058af0: 742c 2073 696e 6365 2c20 6c69 6d69 7429  t, since, limit)
-00058b00: 0a0a 2020 2020 6465 6620 6665 7463 685f  ..    def fetch_
-00058b10: 6f70 656e 5f69 6e74 6572 6573 7428 7365  open_interest(se
-00058b20: 6c66 2c20 7379 6d62 6f6c 3a20 7374 722c  lf, symbol: str,
-00058b30: 2070 6172 616d 733d 7b7d 293a 0a20 2020   params={}):.   
-00058b40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00058b50: 2052 6574 7269 6576 6573 2074 6865 206f   Retrieves the o
-00058b60: 7065 6e20 696e 7465 7265 7374 206f 6620  pen interest of 
-00058b70: 6120 6465 7269 7661 7469 7665 2074 7261  a derivative tra
-00058b80: 6469 6e67 2070 6169 720a 2020 2020 2020  ding pair.      
-00058b90: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
-00058ba0: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
-00058bb0: 6875 622e 696f 2f64 6f63 732f 7635 2f6d  hub.io/docs/v5/m
-00058bc0: 6172 6b65 742f 6f70 656e 2d69 6e74 6572  arket/open-inter
-00058bd0: 6573 740a 2020 2020 2020 2020 3a70 6172  est.        :par
-00058be0: 616d 2073 7472 2073 796d 626f 6c3a 2055  am str symbol: U
-00058bf0: 6e69 6669 6564 2043 4358 5420 6d61 726b  nified CCXT mark
-00058c00: 6574 2073 796d 626f 6c0a 2020 2020 2020  et symbol.      
-00058c10: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
-00058c20: 7261 6d73 3a20 6578 6368 616e 6765 2073  rams: exchange s
-00058c30: 7065 6369 6669 6320 7061 7261 6d65 7465  pecific paramete
-00058c40: 7273 0a20 2020 2020 2020 203a 7061 7261  rs.        :para
-00058c50: 6d20 7374 727c 4e6f 6e65 2070 6172 616d  m str|None param
-00058c60: 735b 2769 6e74 6572 7661 6c27 5d3a 2035  s['interval']: 5
-00058c70: 6d2c 2031 356d 2c20 3330 6d2c 2031 682c  m, 15m, 30m, 1h,
-00058c80: 2034 682c 2031 640a 2020 2020 2020 2020   4h, 1d.        
-00058c90: 3a70 6172 616d 2073 7472 7c4e 6f6e 6520  :param str|None 
-00058ca0: 7061 7261 6d73 5b27 6361 7465 676f 7279  params['category
-00058cb0: 275d 3a20 226c 696e 6561 7222 206f 7220  ']: "linear" or 
-00058cc0: 2269 6e76 6572 7365 220a 2020 2020 2020  "inverse".      
-00058cd0: 2020 3a72 6574 7572 6e73 2064 6963 747d    :returns dict}
-00058ce0: 2061 6e20 6f70 656e 2069 6e74 6572 6573   an open interes
-00058cf0: 7420 7374 7275 6374 7572 657b 406c 696e  t structure{@lin
-00058d00: 6b20 6874 7470 733a 2f2f 646f 6373 2e63  k https://docs.c
-00058d10: 6378 742e 636f 6d2f 232f 3f69 643d 696e  cxt.com/#/?id=in
-00058d20: 7465 7265 7374 2d68 6973 746f 7279 2d73  terest-history-s
-00058d30: 7472 7563 7475 7265 3a0a 2020 2020 2020  tructure:.      
-00058d40: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00058d50: 6c66 2e6c 6f61 645f 6d61 726b 6574 7328  lf.load_markets(
-00058d60: 290a 2020 2020 2020 2020 6d61 726b 6574  ).        market
-00058d70: 203d 2073 656c 662e 6d61 726b 6574 2873   = self.market(s
-00058d80: 796d 626f 6c29 0a20 2020 2020 2020 2069  ymbol).        i
-00058d90: 6620 6e6f 7420 6d61 726b 6574 5b27 636f  f not market['co
-00058da0: 6e74 7261 6374 275d 3a0a 2020 2020 2020  ntract']:.      
-00058db0: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
-00058dc0: 6571 7565 7374 2873 656c 662e 6964 202b  equest(self.id +
-00058dd0: 2027 2066 6574 6368 4f70 656e 496e 7465   ' fetchOpenInte
-00058de0: 7265 7374 2829 2073 7570 706f 7274 7320  rest() supports 
-00058df0: 636f 6e74 7261 6374 206d 6172 6b65 7473  contract markets
-00058e00: 206f 6e6c 7927 290a 2020 2020 2020 2020   only').        
-00058e10: 7469 6d65 6672 616d 6520 3d20 7365 6c66  timeframe = self
-00058e20: 2e73 6166 655f 7374 7269 6e67 2870 6172  .safe_string(par
-00058e30: 616d 732c 2027 696e 7465 7276 616c 272c  ams, 'interval',
-00058e40: 2027 3168 2729 0a20 2020 2020 2020 2069   '1h').        i
-00058e50: 6e74 6572 7661 6c73 203d 2073 656c 662e  ntervals = self.
-00058e60: 7361 6665 5f76 616c 7565 2873 656c 662e  safe_value(self.
-00058e70: 6f70 7469 6f6e 732c 2027 696e 7465 7276  options, 'interv
-00058e80: 616c 7327 290a 2020 2020 2020 2020 696e  als').        in
-00058e90: 7465 7276 616c 203d 2073 656c 662e 7361  terval = self.sa
-00058ea0: 6665 5f73 7472 696e 6728 696e 7465 7276  fe_string(interv
-00058eb0: 616c 732c 2074 696d 6566 7261 6d65 2920  als, timeframe) 
-00058ec0: 2023 2035 6d69 6e2c 3135 6d69 6e2c 3330   # 5min,15min,30
-00058ed0: 6d69 6e2c 3168 2c34 682c 3164 0a20 2020  min,1h,4h,1d.   
-00058ee0: 2020 2020 2069 6620 696e 7465 7276 616c       if interval
-00058ef0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00058f00: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
-00058f10: 6571 7565 7374 2873 656c 662e 6964 202b  equest(self.id +
-00058f20: 2027 2066 6574 6368 4f70 656e 496e 7465   ' fetchOpenInte
-00058f30: 7265 7374 2829 2063 616e 6e6f 7420 7573  rest() cannot us
-00058f40: 6520 7468 6520 2720 2b20 7469 6d65 6672  e the ' + timefr
-00058f50: 616d 6520 2b20 2720 7469 6d65 6672 616d  ame + ' timefram
-00058f60: 6527 290a 2020 2020 2020 2020 7375 6254  e').        subT
-00058f70: 7970 6520 3d20 276c 696e 6561 7227 2069  ype = 'linear' i
-00058f80: 6620 6d61 726b 6574 5b27 6c69 6e65 6172  f market['linear
-00058f90: 275d 2065 6c73 6520 2769 6e76 6572 7365  '] else 'inverse
-00058fa0: 270a 2020 2020 2020 2020 6361 7465 676f  '.        catego
-00058fb0: 7279 203d 2073 656c 662e 7361 6665 5f73  ry = self.safe_s
-00058fc0: 7472 696e 6728 7061 7261 6d73 2c20 2763  tring(params, 'c
-00058fd0: 6174 6567 6f72 7927 2c20 7375 6254 7970  ategory', subTyp
-00058fe0: 6529 0a20 2020 2020 2020 2072 6571 7565  e).        reque
-00058ff0: 7374 203d 207b 0a20 2020 2020 2020 2020  st = {.         
-00059000: 2020 2027 7379 6d62 6f6c 273a 206d 6172     'symbol': mar
-00059010: 6b65 745b 2769 6427 5d2c 0a20 2020 2020  ket['id'],.     
-00059020: 2020 2020 2020 2027 696e 7465 7276 616c         'interval
-00059030: 5469 6d65 273a 2069 6e74 6572 7661 6c2c  Time': interval,
-00059040: 0a20 2020 2020 2020 2020 2020 2027 6361  .            'ca
-00059050: 7465 676f 7279 273a 2063 6174 6567 6f72  tegory': categor
-00059060: 792c 0a20 2020 2020 2020 207d 0a20 2020  y,.        }.   
-00059070: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-00059080: 7365 6c66 2e70 7562 6c69 6347 6574 5635  self.publicGetV5
-00059090: 4d61 726b 6574 4f70 656e 496e 7465 7265  MarketOpenIntere
-000590a0: 7374 2873 656c 662e 6578 7465 6e64 2872  st(self.extend(r
-000590b0: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
-000590c0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-000590d0: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
-000590e0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
-000590f0: 7443 6f64 6522 3a20 302c 0a20 2020 2020  tCode": 0,.     
-00059100: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
-00059110: 744d 7367 223a 2022 4f4b 222c 0a20 2020  tMsg": "OK",.   
-00059120: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-00059130: 7265 7375 6c74 223a 207b 0a20 2020 2020  result": {.     
-00059140: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-00059150: 2022 7379 6d62 6f6c 223a 2022 4254 4355   "symbol": "BTCU
-00059160: 5344 222c 0a20 2020 2020 2020 2023 2020  SD",.        #  
-00059170: 2020 2020 2020 2020 2020 2022 6361 7465             "cate
-00059180: 676f 7279 223a 2022 696e 7665 7273 6522  gory": "inverse"
-00059190: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-000591a0: 2020 2020 2020 2020 226c 6973 7422 3a20          "list": 
-000591b0: 5b0a 2020 2020 2020 2020 2320 2020 2020  [.        #     
-000591c0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000591d0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-000591e0: 2020 2020 2020 2020 2020 2020 226f 7065              "ope
-000591f0: 6e49 6e74 6572 6573 7422 3a20 2234 3631  nInterest": "461
-00059200: 3133 3433 3834 2e30 3030 3030 3030 3022  134384.00000000"
-00059210: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-00059220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00059230: 2274 696d 6573 7461 6d70 223a 2022 3136  "timestamp": "16
-00059240: 3639 3537 3134 3030 3030 3022 0a20 2020  69571400000".   
-00059250: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-00059260: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00059270: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-00059280: 2020 2020 7b0a 2020 2020 2020 2020 2320      {.        # 
-00059290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000592a0: 2020 2020 226f 7065 6e49 6e74 6572 6573      "openInteres
-000592b0: 7422 3a20 2234 3631 3133 3432 3932 2e30  t": "461134292.0
-000592c0: 3030 3030 3030 3022 2c0a 2020 2020 2020  0000000",.      
-000592d0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-000592e0: 2020 2020 2020 2020 2274 696d 6573 7461          "timesta
-000592f0: 6d70 223a 2022 3136 3639 3537 3131 3030  mp": "1669571100
-00059300: 3030 3022 0a20 2020 2020 2020 2023 2020  000".        #  
-00059310: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00059320: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00059330: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00059340: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-00059350: 226e 6578 7450 6167 6543 7572 736f 7222  "nextPageCursor"
-00059360: 3a20 2222 0a20 2020 2020 2020 2023 2020  : "".        #  
-00059370: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00059380: 2020 2320 2020 2020 2020 2020 2272 6574    #         "ret
-00059390: 4578 7449 6e66 6f22 3a20 7b7d 2c0a 2020  ExtInfo": {},.  
-000593a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-000593b0: 2274 696d 6522 3a20 3136 3732 3035 3335  "time": 16720535
-000593c0: 3438 3537 390a 2020 2020 2020 2020 2320  48579.        # 
-000593d0: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
-000593e0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000593f0: 2073 656c 662e 7361 6665 5f76 616c 7565   self.safe_value
-00059400: 2872 6573 706f 6e73 652c 2027 7265 7375  (response, 'resu
-00059410: 6c74 272c 207b 7d29 0a20 2020 2020 2020  lt', {}).       
-00059420: 2069 6420 3d20 7365 6c66 2e73 6166 655f   id = self.safe_
-00059430: 7374 7269 6e67 2872 6573 756c 742c 2027  string(result, '
-00059440: 7379 6d62 6f6c 2729 0a20 2020 2020 2020  symbol').       
-00059450: 206d 6172 6b65 7420 3d20 7365 6c66 2e73   market = self.s
-00059460: 6166 655f 6d61 726b 6574 2869 642c 206d  afe_market(id, m
-00059470: 6172 6b65 742c 204e 6f6e 652c 2027 636f  arket, None, 'co
-00059480: 6e74 7261 6374 2729 0a20 2020 2020 2020  ntract').       
-00059490: 2064 6174 6120 3d20 7365 6c66 2e73 6166   data = self.saf
-000594a0: 655f 7661 6c75 6528 7265 7375 6c74 2c20  e_value(result, 
-000594b0: 276c 6973 7427 2c20 5b5d 290a 2020 2020  'list', []).    
-000594c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000594d0: 7061 7273 655f 6f70 656e 5f69 6e74 6572  parse_open_inter
-000594e0: 6573 7428 6461 7461 5b30 5d2c 206d 6172  est(data[0], mar
-000594f0: 6b65 7429 0a0a 2020 2020 6465 6620 6665  ket)..    def fe
-00059500: 7463 685f 6f70 656e 5f69 6e74 6572 6573  tch_open_interes
-00059510: 745f 6869 7374 6f72 7928 7365 6c66 2c20  t_history(self, 
-00059520: 7379 6d62 6f6c 3a20 7374 722c 2074 696d  symbol: str, tim
-00059530: 6566 7261 6d65 3d27 3168 272c 2073 696e  eframe='1h', sin
-00059540: 6365 3a20 4f70 7469 6f6e 616c 5b69 6e74  ce: Optional[int
-00059550: 5d20 3d20 4e6f 6e65 2c20 6c69 6d69 743a  ] = None, limit:
-00059560: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00059570: 204e 6f6e 652c 2070 6172 616d 733d 7b7d   None, params={}
-00059580: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00059590: 2020 2020 2020 2047 6574 7320 7468 6520         Gets the 
-000595a0: 746f 7461 6c20 616d 6f75 6e74 206f 6620  total amount of 
-000595b0: 756e 7365 7474 6c65 6420 636f 6e74 7261  unsettled contra
-000595c0: 6374 732e 2049 6e20 6f74 6865 7220 776f  cts. In other wo
-000595d0: 7264 732c 2074 6865 2074 6f74 616c 206e  rds, the total n
-000595e0: 756d 6265 7220 6f66 2063 6f6e 7472 6163  umber of contrac
-000595f0: 7473 2068 656c 6420 696e 206f 7065 6e20  ts held in open 
-00059600: 706f 7369 7469 6f6e 730a 2020 2020 2020  positions.      
-00059610: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
-00059620: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
-00059630: 6875 622e 696f 2f64 6f63 732f 7635 2f6d  hub.io/docs/v5/m
-00059640: 6172 6b65 742f 6f70 656e 2d69 6e74 6572  arket/open-inter
-00059650: 6573 740a 2020 2020 2020 2020 3a70 6172  est.        :par
-00059660: 616d 2073 7472 2073 796d 626f 6c3a 2055  am str symbol: U
-00059670: 6e69 6669 6564 206d 6172 6b65 7420 7379  nified market sy
-00059680: 6d62 6f6c 0a20 2020 2020 2020 203a 7061  mbol.        :pa
-00059690: 7261 6d20 7374 7220 7469 6d65 6672 616d  ram str timefram
-000596a0: 653a 2022 356d 222c 2031 356d 2c20 3330  e: "5m", 15m, 30
-000596b0: 6d2c 2031 682c 2034 682c 2031 640a 2020  m, 1h, 4h, 1d.  
-000596c0: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
-000596d0: 2073 696e 6365 3a20 4e6f 7420 7573 6564   since: Not used
-000596e0: 2062 7920 4279 6269 740a 2020 2020 2020   by Bybit.      
-000596f0: 2020 3a70 6172 616d 2069 6e74 206c 696d    :param int lim
-00059700: 6974 3a20 5468 6520 6e75 6d62 6572 206f  it: The number o
-00059710: 6620 6f70 656e 2069 6e74 6572 6573 7420  f open interest 
-00059720: 7374 7275 6374 7572 6573 2074 6f20 7265  structures to re
-00059730: 7475 726e 2e20 4d61 7820 3230 302c 2064  turn. Max 200, d
-00059740: 6566 6175 6c74 2035 300a 2020 2020 2020  efault 50.      
-00059750: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
-00059760: 7261 6d73 3a20 4578 6368 616e 6765 2073  rams: Exchange s
-00059770: 7065 6369 6669 6320 7061 7261 6d65 7465  pecific paramete
-00059780: 7273 0a20 2020 2020 2020 203a 7265 7475  rs.        :retu
-00059790: 726e 733a 2041 6e20 6172 7261 7920 6f66  rns: An array of
-000597a0: 206f 7065 6e20 696e 7465 7265 7374 2073   open interest s
-000597b0: 7472 7563 7475 7265 730a 2020 2020 2020  tructures.      
-000597c0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000597d0: 2074 696d 6566 7261 6d65 203d 3d20 2731   timeframe == '1
-000597e0: 6d27 3a0a 2020 2020 2020 2020 2020 2020  m':.            
-000597f0: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
-00059800: 2873 656c 662e 6964 202b 2027 6665 7463  (self.id + 'fetc
-00059810: 684f 7065 6e49 6e74 6572 6573 7448 6973  hOpenInterestHis
-00059820: 746f 7279 2063 616e 6e6f 7420 7573 6520  tory cannot use 
-00059830: 7468 6520 316d 2074 696d 6566 7261 6d65  the 1m timeframe
-00059840: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00059850: 6c6f 6164 5f6d 6172 6b65 7473 2829 0a20  load_markets(). 
-00059860: 2020 2020 2020 206d 6172 6b65 7420 3d20         market = 
-00059870: 7365 6c66 2e6d 6172 6b65 7428 7379 6d62  self.market(symb
-00059880: 6f6c 290a 2020 2020 2020 2020 6966 206d  ol).        if m
-00059890: 6172 6b65 745b 2773 706f 7427 5d20 6f72  arket['spot'] or
-000598a0: 206d 6172 6b65 745b 276f 7074 696f 6e27   market['option'
-000598b0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
-000598c0: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
-000598d0: 7365 6c66 2e69 6420 2b20 2720 6665 7463  self.id + ' fetc
-000598e0: 684f 7065 6e49 6e74 6572 6573 7448 6973  hOpenInterestHis
-000598f0: 746f 7279 2829 2073 796d 626f 6c20 646f  tory() symbol do
-00059900: 6573 206e 6f74 2073 7570 706f 7274 206d  es not support m
-00059910: 6172 6b65 7420 2720 2b20 7379 6d62 6f6c  arket ' + symbol
-00059920: 290a 2020 2020 2020 2020 7265 7175 6573  ).        reques
-00059930: 7420 3d20 7b0a 2020 2020 2020 2020 2020  t = {.          
-00059940: 2020 2773 796d 626f 6c27 3a20 6d61 726b    'symbol': mark
-00059950: 6574 5b27 6964 275d 2c0a 2020 2020 2020  et['id'],.      
-00059960: 2020 7d0a 2020 2020 2020 2020 6966 206c    }.        if l
-00059970: 696d 6974 2069 7320 6e6f 7420 4e6f 6e65  imit is not None
-00059980: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00059990: 7175 6573 745b 276c 696d 6974 275d 203d  quest['limit'] =
-000599a0: 206c 696d 6974 0a20 2020 2020 2020 2072   limit.        r
-000599b0: 6574 7572 6e20 7365 6c66 2e66 6574 6368  eturn self.fetch
-000599c0: 5f64 6572 6976 6174 6976 6573 5f6f 7065  _derivatives_ope
-000599d0: 6e5f 696e 7465 7265 7374 5f68 6973 746f  n_interest_histo
-000599e0: 7279 2873 796d 626f 6c2c 2074 696d 6566  ry(symbol, timef
-000599f0: 7261 6d65 2c20 7369 6e63 652c 206c 696d  rame, since, lim
-00059a00: 6974 2c20 7061 7261 6d73 290a 0a20 2020  it, params)..   
-00059a10: 2064 6566 2070 6172 7365 5f6f 7065 6e5f   def parse_open_
-00059a20: 696e 7465 7265 7374 2873 656c 662c 2069  interest(self, i
-00059a30: 6e74 6572 6573 742c 206d 6172 6b65 743d  nterest, market=
-00059a40: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
-00059a50: 0a20 2020 2020 2020 2023 2020 2020 7b0a  .        #    {.
-00059a60: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00059a70: 2022 6f70 656e 496e 7465 7265 7374 223a   "openInterest":
-00059a80: 2036 3437 3537 2e36 3234 3030 3030 302c   64757.62400000,
-00059a90: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00059aa0: 2020 2274 696d 6573 7461 6d70 223a 2031    "timestamp": 1
-00059ab0: 3636 3537 3834 3830 3030 3030 2c0a 2020  665784800000,.  
-00059ac0: 2020 2020 2020 2320 2020 207d 0a20 2020        #    }.   
-00059ad0: 2020 2020 2023 0a20 2020 2020 2020 2074       #.        t
-00059ae0: 696d 6573 7461 6d70 203d 2073 656c 662e  imestamp = self.
-00059af0: 7361 6665 5f69 6e74 6567 6572 2869 6e74  safe_integer(int
-00059b00: 6572 6573 742c 2027 7469 6d65 7374 616d  erest, 'timestam
-00059b10: 7027 290a 2020 2020 2020 2020 7661 6c75  p').        valu
-00059b20: 6520 3d20 7365 6c66 2e73 6166 655f 6e75  e = self.safe_nu
-00059b30: 6d62 6572 5f32 2869 6e74 6572 6573 742c  mber_2(interest,
-00059b40: 2027 6f70 656e 5f69 6e74 6572 6573 7427   'open_interest'
-00059b50: 2c20 276f 7065 6e49 6e74 6572 6573 7427  , 'openInterest'
-00059b60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00059b70: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00059b80: 7379 6d62 6f6c 273a 206d 6172 6b65 745b  symbol': market[
-00059b90: 2773 796d 626f 6c27 5d2c 0a20 2020 2020  'symbol'],.     
-00059ba0: 2020 2020 2020 2027 6f70 656e 496e 7465         'openInte
-00059bb0: 7265 7374 416d 6f75 6e74 273a 204e 6f6e  restAmount': Non
-00059bc0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-00059bd0: 6f70 656e 496e 7465 7265 7374 5661 6c75  openInterestValu
-00059be0: 6527 3a20 7661 6c75 652c 0a20 2020 2020  e': value,.     
-00059bf0: 2020 2020 2020 2027 7469 6d65 7374 616d         'timestam
-00059c00: 7027 3a20 7469 6d65 7374 616d 702c 0a20  p': timestamp,. 
-00059c10: 2020 2020 2020 2020 2020 2027 6461 7465             'date
-00059c20: 7469 6d65 273a 2073 656c 662e 6973 6f38  time': self.iso8
-00059c30: 3630 3128 7469 6d65 7374 616d 7029 2c0a  601(timestamp),.
-00059c40: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
-00059c50: 6f27 3a20 696e 7465 7265 7374 2c0a 2020  o': interest,.  
-00059c60: 2020 2020 2020 7d0a 0a20 2020 2064 6566        }..    def
-00059c70: 2066 6574 6368 5f62 6f72 726f 775f 7261   fetch_borrow_ra
-00059c80: 7465 2873 656c 662c 2063 6f64 653a 2073  te(self, code: s
-00059c90: 7472 2c20 7061 7261 6d73 3d7b 7d29 3a0a  tr, params={}):.
-00059ca0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00059cb0: 2020 2020 6665 7463 6820 7468 6520 7261      fetch the ra
-00059cc0: 7465 206f 6620 696e 7465 7265 7374 2074  te of interest t
-00059cd0: 6f20 626f 7272 6f77 2061 2063 7572 7265  o borrow a curre
-00059ce0: 6e63 7920 666f 7220 6d61 7267 696e 2074  ncy for margin t
-00059cf0: 7261 6469 6e67 0a20 2020 2020 2020 2073  rading.        s
-00059d00: 6565 2068 7474 7073 3a2f 2f62 7962 6974  ee https://bybit
-00059d10: 2d65 7863 6861 6e67 652e 6769 7468 7562  -exchange.github
-00059d20: 2e69 6f2f 646f 6373 2f73 706f 742f 7633  .io/docs/spot/v3
-00059d30: 2f23 742d 7175 6572 7969 6e74 6572 6573  /#t-queryinteres
-00059d40: 7471 756f 7461 0a20 2020 2020 2020 203a  tquota.        :
-00059d50: 7061 7261 6d20 7374 7220 636f 6465 3a20  param str code: 
-00059d60: 756e 6966 6965 6420 6375 7272 656e 6379  unified currency
-00059d70: 2063 6f64 650a 2020 2020 2020 2020 3a70   code.        :p
-00059d80: 6172 616d 2064 6963 7420 7061 7261 6d73  aram dict params
-00059d90: 3a20 6578 7472 6120 7061 7261 6d65 7465  : extra paramete
-00059da0: 7273 2073 7065 6369 6669 6320 746f 2074  rs specific to t
-00059db0: 6865 2062 7962 6974 2061 7069 2065 6e64  he bybit api end
-00059dc0: 706f 696e 740a 2020 2020 2020 2020 3a72  point.        :r
-00059dd0: 6574 7572 6e73 2064 6963 743a 2061 2060  eturns dict: a `
-00059de0: 626f 7272 6f77 2072 6174 6520 7374 7275  borrow rate stru
-00059df0: 6374 7572 6520 3c68 7474 7073 3a2f 2f64  cture <https://d
-00059e00: 6f63 732e 6363 7874 2e63 6f6d 2f23 2f3f  ocs.ccxt.com/#/?
-00059e10: 6964 3d62 6f72 726f 772d 7261 7465 2d73  id=borrow-rate-s
-00059e20: 7472 7563 7475 7265 3e60 0a20 2020 2020  tructure>`.     
-00059e30: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00059e40: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
-00059e50: 2829 0a20 2020 2020 2020 2063 7572 7265  ().        curre
-00059e60: 6e63 7920 3d20 7365 6c66 2e63 7572 7265  ncy = self.curre
-00059e70: 6e63 7928 636f 6465 290a 2020 2020 2020  ncy(code).      
-00059e80: 2020 7265 7175 6573 7420 3d20 7b0a 2020    request = {.  
-00059e90: 2020 2020 2020 2020 2020 2763 6f69 6e27            'coin'
-00059ea0: 3a20 6375 7272 656e 6379 5b27 6964 275d  : currency['id']
-00059eb0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-00059ec0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00059ed0: 656c 662e 7072 6976 6174 6547 6574 5370  elf.privateGetSp
-00059ee0: 6f74 5633 5072 6976 6174 6543 726f 7373  otV3PrivateCross
-00059ef0: 4d61 7267 696e 4c6f 616e 496e 666f 2873  MarginLoanInfo(s
-00059f00: 656c 662e 6578 7465 6e64 2872 6571 7565  elf.extend(reque
-00059f10: 7374 2c20 7061 7261 6d73 2929 0a20 2020  st, params)).   
-00059f20: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-00059f30: 2020 2020 7b0a 2020 2020 2020 2020 2320      {.        # 
-00059f40: 2020 2020 2020 2020 2272 6574 436f 6465          "retCode
-00059f50: 223a 2022 3022 2c0a 2020 2020 2020 2020  ": "0",.        
-00059f60: 2320 2020 2020 2020 2020 2272 6574 4d73  #         "retMs
-00059f70: 6722 3a20 2273 7563 6365 7373 222c 0a20  g": "success",. 
-00059f80: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00059f90: 2022 7265 7375 6c74 223a 207b 0a20 2020   "result": {.   
-00059fa0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-00059fb0: 2020 2022 636f 696e 223a 2022 5553 4454     "coin": "USDT
-00059fc0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-00059fd0: 2020 2020 2020 2020 2022 696e 7465 7265           "intere
-00059fe0: 7374 5261 7465 223a 2022 302e 3030 3031  stRate": "0.0001
-00059ff0: 3037 3030 3030 3030 222c 0a20 2020 2020  07000000",.     
-0005a000: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005a010: 2022 6c6f 616e 4162 6c65 416d 6f75 6e74   "loanAbleAmount
-0005a020: 223a 2022 222c 0a20 2020 2020 2020 2023  ": "",.        #
-0005a030: 2020 2020 2020 2020 2020 2020 2022 6d61               "ma
-0005a040: 784c 6f61 6e41 6d6f 756e 7422 3a20 2237  xLoanAmount": "7
-0005a050: 3939 3939 2e39 3939 220a 2020 2020 2020  9999.999".      
-0005a060: 2020 2320 2020 2020 2020 2020 7d2c 0a20    #         },. 
-0005a070: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005a080: 2022 7265 7445 7874 496e 666f 223a 206e   "retExtInfo": n
-0005a090: 756c 6c2c 0a20 2020 2020 2020 2023 2020  ull,.        #  
-0005a0a0: 2020 2020 2020 2022 7469 6d65 223a 2022         "time": "
-0005a0b0: 3136 3636 3733 3434 3930 3737 3822 0a20  1666734490778". 
-0005a0c0: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
-0005a0d0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0005a0e0: 2064 6174 6120 3d20 7365 6c66 2e73 6166   data = self.saf
-0005a0f0: 655f 7661 6c75 6528 7265 7370 6f6e 7365  e_value(response
-0005a100: 2c20 2772 6573 756c 7427 2c20 7b7d 290a  , 'result', {}).
-0005a110: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0005a120: 656c 662e 7061 7273 655f 626f 7272 6f77  elf.parse_borrow
-0005a130: 5f72 6174 6528 6461 7461 2c20 6375 7272  _rate(data, curr
-0005a140: 656e 6379 290a 0a20 2020 2064 6566 2070  ency)..    def p
-0005a150: 6172 7365 5f62 6f72 726f 775f 7261 7465  arse_borrow_rate
-0005a160: 2873 656c 662c 2069 6e66 6f2c 2063 7572  (self, info, cur
-0005a170: 7265 6e63 793d 4e6f 6e65 293a 0a20 2020  rency=None):.   
-0005a180: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-0005a190: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0005a1a0: 2020 2020 2020 2020 2022 636f 696e 223a           "coin":
-0005a1b0: 2022 5553 4454 222c 0a20 2020 2020 2020   "USDT",.       
-0005a1c0: 2023 2020 2020 2020 2020 2022 696e 7465   #         "inte
-0005a1d0: 7265 7374 5261 7465 223a 2022 302e 3030  restRate": "0.00
-0005a1e0: 3031 3037 3030 3030 3030 222c 0a20 2020  0107000000",.   
-0005a1f0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005a200: 6c6f 616e 4162 6c65 416d 6f75 6e74 223a  loanAbleAmount":
-0005a210: 2022 222c 0a20 2020 2020 2020 2023 2020   "",.        #  
-0005a220: 2020 2020 2020 2022 6d61 784c 6f61 6e41         "maxLoanA
-0005a230: 6d6f 756e 7422 3a20 2237 3939 3939 2e39  mount": "79999.9
-0005a240: 3939 220a 2020 2020 2020 2020 2320 2020  99".        #   
-0005a250: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
-0005a260: 2020 2020 2020 7469 6d65 7374 616d 7020        timestamp 
-0005a270: 3d20 7365 6c66 2e6d 696c 6c69 7365 636f  = self.milliseco
-0005a280: 6e64 7328 290a 2020 2020 2020 2020 6375  nds().        cu
-0005a290: 7272 656e 6379 4964 203d 2073 656c 662e  rrencyId = self.
-0005a2a0: 7361 6665 5f73 7472 696e 6728 696e 666f  safe_string(info
-0005a2b0: 2c20 2763 6f69 6e27 290a 2020 2020 2020  , 'coin').      
-0005a2c0: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-0005a2d0: 2020 2020 2020 2027 6375 7272 656e 6379         'currency
-0005a2e0: 273a 2073 656c 662e 7361 6665 5f63 7572  ': self.safe_cur
-0005a2f0: 7265 6e63 795f 636f 6465 2863 7572 7265  rency_code(curre
-0005a300: 6e63 7949 642c 2063 7572 7265 6e63 7929  ncyId, currency)
-0005a310: 2c0a 2020 2020 2020 2020 2020 2020 2772  ,.            'r
-0005a320: 6174 6527 3a20 7365 6c66 2e73 6166 655f  ate': self.safe_
-0005a330: 6e75 6d62 6572 2869 6e66 6f2c 2027 696e  number(info, 'in
-0005a340: 7465 7265 7374 5261 7465 2729 2c0a 2020  terestRate'),.  
-0005a350: 2020 2020 2020 2020 2020 2770 6572 696f            'perio
-0005a360: 6427 3a20 3836 3430 3030 3030 2c20 2023  d': 86400000,  #
-0005a370: 2044 6169 6c79 0a20 2020 2020 2020 2020   Daily.         
-0005a380: 2020 2027 7469 6d65 7374 616d 7027 3a20     'timestamp': 
-0005a390: 7469 6d65 7374 616d 702c 0a20 2020 2020  timestamp,.     
-0005a3a0: 2020 2020 2020 2027 6461 7465 7469 6d65         'datetime
-0005a3b0: 273a 2073 656c 662e 6973 6f38 3630 3128  ': self.iso8601(
-0005a3c0: 7469 6d65 7374 616d 7029 2c0a 2020 2020  timestamp),.    
-0005a3d0: 2020 2020 2020 2020 2769 6e66 6f27 3a20          'info': 
-0005a3e0: 696e 666f 2c0a 2020 2020 2020 2020 7d0a  info,.        }.
-0005a3f0: 0a20 2020 2064 6566 2066 6574 6368 5f62  .    def fetch_b
-0005a400: 6f72 726f 775f 696e 7465 7265 7374 2873  orrow_interest(s
-0005a410: 656c 662c 2063 6f64 653a 204f 7074 696f  elf, code: Optio
-0005a420: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0005a430: 2073 796d 626f 6c3a 204f 7074 696f 6e61   symbol: Optiona
-0005a440: 6c5b 7374 725d 203d 204e 6f6e 652c 2073  l[str] = None, s
-0005a450: 696e 6365 3a20 4f70 7469 6f6e 616c 5b69  ince: Optional[i
-0005a460: 6e74 5d20 3d20 4e6f 6e65 2c20 6c69 6d69  nt] = None, limi
-0005a470: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
-0005a480: 203d 204e 6f6e 652c 2070 6172 616d 733d   = None, params=
-0005a490: 7b7d 293a 0a20 2020 2020 2020 2022 2222  {}):.        """
-0005a4a0: 0a20 2020 2020 2020 2066 6574 6368 2074  .        fetch t
-0005a4b0: 6865 2069 6e74 6572 6573 7420 6f77 6564  he interest owed
-0005a4c0: 2062 7920 7468 6520 7573 6572 2066 6f72   by the user for
-0005a4d0: 2062 6f72 726f 7769 6e67 2063 7572 7265   borrowing curre
-0005a4e0: 6e63 7920 666f 7220 6d61 7267 696e 2074  ncy for margin t
-0005a4f0: 7261 6469 6e67 0a20 2020 2020 2020 203a  rading.        :
-0005a500: 7061 7261 6d20 7374 727c 4e6f 6e65 2063  param str|None c
-0005a510: 6f64 653a 2075 6e69 6669 6564 2063 7572  ode: unified cur
-0005a520: 7265 6e63 7920 636f 6465 0a20 2020 2020  rency code.     
-0005a530: 2020 203a 7061 7261 6d20 7374 727c 4e6f     :param str|No
-0005a540: 6e65 2073 796d 626f 6c3a 2075 6e69 6669  ne symbol: unifi
-0005a550: 6564 206d 6172 6b65 7420 7379 6d62 6f6c  ed market symbol
-0005a560: 2077 6865 6e20 6665 7463 6820 696e 7465   when fetch inte
-0005a570: 7265 7374 2069 6e20 6973 6f6c 6174 6564  rest in isolated
-0005a580: 206d 6172 6b65 7473 0a20 2020 2020 2020   markets.       
-0005a590: 203a 7061 7261 6d20 6e75 6d62 6572 7c4e   :param number|N
-0005a5a0: 6f6e 6520 7369 6e63 653a 2074 6865 2065  one since: the e
-0005a5b0: 6172 6c69 6573 7420 7469 6d65 2069 6e20  arliest time in 
-0005a5c0: 6d73 2074 6f20 6665 7463 6820 626f 7272  ms to fetch borr
-0005a5d0: 726f 7720 696e 7465 7265 7374 2066 6f72  row interest for
-0005a5e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0005a5f0: 6e75 6d62 6572 7c4e 6f6e 6520 6c69 6d69  number|None limi
-0005a600: 743a 2074 6865 206d 6178 696d 756d 206e  t: the maximum n
-0005a610: 756d 6265 7220 6f66 2073 7472 7563 7475  umber of structu
-0005a620: 7265 7320 746f 2072 6574 7269 6576 650a  res to retrieve.
-0005a630: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-0005a640: 6963 7420 7061 7261 6d73 3a20 6578 7472  ict params: extr
-0005a650: 6120 7061 7261 6d65 7465 7273 2073 7065  a parameters spe
-0005a660: 6369 6669 6320 746f 2074 6865 2062 7962  cific to the byb
-0005a670: 6974 2061 7069 2065 6e64 706f 696e 740a  it api endpoint.
-0005a680: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
-0005a690: 205b 6469 6374 5d3a 2061 206c 6973 7420   [dict]: a list 
-0005a6a0: 6f66 2060 626f 7272 6f77 2069 6e74 6572  of `borrow inter
-0005a6b0: 6573 7420 7374 7275 6374 7572 6573 203c  est structures <
-0005a6c0: 6874 7470 733a 2f2f 646f 6373 2e63 6378  https://docs.ccx
-0005a6d0: 742e 636f 6d2f 232f 3f69 643d 626f 7272  t.com/#/?id=borr
-0005a6e0: 6f77 2d69 6e74 6572 6573 742d 7374 7275  ow-interest-stru
-0005a6f0: 6374 7572 653e 600a 2020 2020 2020 2020  cture>`.        
-0005a700: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-0005a710: 2e6c 6f61 645f 6d61 726b 6574 7328 290a  .load_markets().
-0005a720: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-0005a730: 3d20 7b7d 0a20 2020 2020 2020 2072 6573  = {}.        res
-0005a740: 706f 6e73 6520 3d20 7365 6c66 2e70 7269  ponse = self.pri
-0005a750: 7661 7465 4765 7453 706f 7456 3350 7269  vateGetSpotV3Pri
-0005a760: 7661 7465 4372 6f73 734d 6172 6769 6e41  vateCrossMarginA
-0005a770: 6363 6f75 6e74 2873 656c 662e 6578 7465  ccount(self.exte
-0005a780: 6e64 2872 6571 7565 7374 2c20 7061 7261  nd(request, para
-0005a790: 6d73 2929 0a20 2020 2020 2020 2023 0a20  ms)).        #. 
-0005a7a0: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
-0005a7b0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005a7c0: 2022 7265 745f 636f 6465 223a 2030 2c0a   "ret_code": 0,.
-0005a7d0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005a7e0: 2020 2272 6574 5f6d 7367 223a 2022 222c    "ret_msg": "",
-0005a7f0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005a800: 2020 2022 6578 745f 636f 6465 223a 206e     "ext_code": n
-0005a810: 756c 6c2c 0a20 2020 2020 2020 2023 2020  ull,.        #  
-0005a820: 2020 2020 2020 2022 6578 745f 696e 666f         "ext_info
-0005a830: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
-0005a840: 2023 2020 2020 2020 2020 2022 7265 7375   #         "resu
-0005a850: 6c74 223a 207b 0a20 2020 2020 2020 2023  lt": {.        #
-0005a860: 2020 2020 2020 2020 2020 2020 2022 7374               "st
-0005a870: 6174 7573 223a 2022 3122 2c0a 2020 2020  atus": "1",.    
-0005a880: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005a890: 2020 2272 6973 6b52 6174 6522 3a20 2230    "riskRate": "0
-0005a8a0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005a8b0: 2020 2020 2020 2020 2022 6163 6374 4261           "acctBa
-0005a8c0: 6c61 6e63 6553 756d 223a 2022 302e 3030  lanceSum": "0.00
-0005a8d0: 3034 3836 3231 3338 3137 3638 3038 3537  0486213817680857
-0005a8e0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005a8f0: 2020 2020 2020 2020 2022 6465 6274 4261           "debtBa
-0005a900: 6c61 6e63 6553 756d 223a 2022 3022 2c0a  lanceSum": "0",.
-0005a910: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005a920: 2020 2020 2020 226c 6f61 6e41 6363 6f75        "loanAccou
-0005a930: 6e74 4c69 7374 223a 205b 0a20 2020 2020  ntList": [.     
-0005a940: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005a950: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0005a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005a970: 2020 2020 2022 746f 6b65 6e49 6422 3a20       "tokenId": 
-0005a980: 2242 5443 222c 0a20 2020 2020 2020 2023  "BTC",.        #
-0005a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005a9a0: 2020 2020 2022 746f 7461 6c22 3a20 2230       "total": "0
-0005a9b0: 2e30 3030 3438 3632 3122 2c0a 2020 2020  .00048621",.    
-0005a9c0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005a9d0: 2020 2020 2020 2020 2020 226c 6f63 6b65            "locke
-0005a9e0: 6422 3a20 2230 222c 0a20 2020 2020 2020  d": "0",.       
-0005a9f0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0005aa00: 2020 2020 2020 2022 6c6f 616e 223a 2022         "loan": "
-0005aa10: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0005aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005aa30: 2020 2269 6e74 6572 6573 7422 3a20 2230    "interest": "0
-0005aa40: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-0005aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005aa60: 2022 6672 6565 223a 2022 302e 3030 3034   "free": "0.0004
-0005aa70: 3836 3231 220a 2020 2020 2020 2020 2320  8621".        # 
-0005aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005aa90: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
-0005aaa0: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-0005aab0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005aac0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0005aad0: 2023 2020 2020 2020 2020 207d 0a20 2020   #         }.   
-0005aae0: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-0005aaf0: 2020 2020 2023 0a20 2020 2020 2020 2064       #.        d
-0005ab00: 6174 6120 3d20 7365 6c66 2e73 6166 655f  ata = self.safe_
-0005ab10: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
-0005ab20: 2772 6573 756c 7427 2c20 7b7d 290a 2020  'result', {}).  
-0005ab30: 2020 2020 2020 726f 7773 203d 2073 656c        rows = sel
-0005ab40: 662e 7361 6665 5f76 616c 7565 2864 6174  f.safe_value(dat
-0005ab50: 612c 2027 6c6f 616e 4163 636f 756e 744c  a, 'loanAccountL
-0005ab60: 6973 7427 2c20 5b5d 290a 2020 2020 2020  ist', []).      
-0005ab70: 2020 696e 7465 7265 7374 203d 2073 656c    interest = sel
-0005ab80: 662e 7061 7273 655f 626f 7272 6f77 5f69  f.parse_borrow_i
-0005ab90: 6e74 6572 6573 7473 2872 6f77 732c 204e  nterests(rows, N
-0005aba0: 6f6e 6529 0a20 2020 2020 2020 2072 6574  one).        ret
-0005abb0: 7572 6e20 7365 6c66 2e66 696c 7465 725f  urn self.filter_
-0005abc0: 6279 5f63 7572 7265 6e63 795f 7369 6e63  by_currency_sinc
-0005abd0: 655f 6c69 6d69 7428 696e 7465 7265 7374  e_limit(interest
-0005abe0: 2c20 636f 6465 2c20 7369 6e63 652c 206c  , code, since, l
-0005abf0: 696d 6974 290a 0a20 2020 2064 6566 2070  imit)..    def p
-0005ac00: 6172 7365 5f62 6f72 726f 775f 696e 7465  arse_borrow_inte
-0005ac10: 7265 7374 2873 656c 662c 2069 6e66 6f2c  rest(self, info,
-0005ac20: 206d 6172 6b65 743d 4e6f 6e65 293a 0a20   market=None):. 
-0005ac30: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0005ac40: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
-0005ac50: 2023 2020 2020 2020 2020 2022 746f 6b65   #         "toke
-0005ac60: 6e49 6422 3a20 2242 5443 222c 0a20 2020  nId": "BTC",.   
-0005ac70: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005ac80: 746f 7461 6c22 3a20 2230 2e30 3030 3438  total": "0.00048
-0005ac90: 3632 3122 2c0a 2020 2020 2020 2020 2320  621",.        # 
-0005aca0: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
-0005acb0: 3a20 2230 222c 0a20 2020 2020 2020 2023  : "0",.        #
-0005acc0: 2020 2020 2020 2020 2022 6c6f 616e 223a           "loan":
-0005acd0: 2022 3022 2c0a 2020 2020 2020 2020 2320   "0",.        # 
-0005ace0: 2020 2020 2020 2020 2269 6e74 6572 6573          "interes
-0005acf0: 7422 3a20 2230 222c 0a20 2020 2020 2020  t": "0",.       
-0005ad00: 2023 2020 2020 2020 2020 2022 6672 6565   #         "free
-0005ad10: 223a 2022 302e 3030 3034 3836 3231 220a  ": "0.00048621".
-0005ad20: 2020 2020 2020 2020 2320 2020 2020 7d2c          #     },
-0005ad30: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005ad40: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-0005ad50: 2020 2020 2020 2020 2773 796d 626f 6c27          'symbol'
-0005ad60: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
-0005ad70: 2020 2020 276d 6172 6769 6e4d 6f64 6527      'marginMode'
-0005ad80: 3a20 2763 726f 7373 272c 0a20 2020 2020  : 'cross',.     
-0005ad90: 2020 2020 2020 2027 6375 7272 656e 6379         'currency
-0005ada0: 273a 2073 656c 662e 7361 6665 5f63 7572  ': self.safe_cur
-0005adb0: 7265 6e63 795f 636f 6465 2873 656c 662e  rency_code(self.
-0005adc0: 7361 6665 5f73 7472 696e 6728 696e 666f  safe_string(info
-0005add0: 2c20 2774 6f6b 656e 4964 2729 292c 0a20  , 'tokenId')),. 
-0005ade0: 2020 2020 2020 2020 2020 2027 696e 7465             'inte
-0005adf0: 7265 7374 273a 2073 656c 662e 7361 6665  rest': self.safe
-0005ae00: 5f6e 756d 6265 7228 696e 666f 2c20 2769  _number(info, 'i
-0005ae10: 6e74 6572 6573 7427 292c 0a20 2020 2020  nterest'),.     
-0005ae20: 2020 2020 2020 2027 696e 7465 7265 7374         'interest
-0005ae30: 5261 7465 273a 204e 6f6e 652c 0a20 2020  Rate': None,.   
-0005ae40: 2020 2020 2020 2020 2027 616d 6f75 6e74           'amount
-0005ae50: 426f 7272 6f77 6564 273a 2073 656c 662e  Borrowed': self.
-0005ae60: 7361 6665 5f6e 756d 6265 7228 696e 666f  safe_number(info
-0005ae70: 2c20 276c 6f61 6e27 292c 0a20 2020 2020  , 'loan'),.     
-0005ae80: 2020 2020 2020 2027 7469 6d65 7374 616d         'timestam
-0005ae90: 7027 3a20 4e6f 6e65 2c0a 2020 2020 2020  p': None,.      
-0005aea0: 2020 2020 2020 2764 6174 6574 696d 6527        'datetime'
-0005aeb0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
-0005aec0: 2020 2020 2769 6e66 6f27 3a20 696e 666f      'info': info
-0005aed0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-0005aee0: 2064 6566 2074 7261 6e73 6665 7228 7365   def transfer(se
-0005aef0: 6c66 2c20 636f 6465 3a20 7374 722c 2061  lf, code: str, a
-0005af00: 6d6f 756e 742c 2066 726f 6d41 6363 6f75  mount, fromAccou
-0005af10: 6e74 2c20 746f 4163 636f 756e 742c 2070  nt, toAccount, p
-0005af20: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
-0005af30: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-0005af40: 7261 6e73 6665 7220 6375 7272 656e 6379  ransfer currency
-0005af50: 2069 6e74 6572 6e61 6c6c 7920 6265 7477   internally betw
-0005af60: 6565 6e20 7761 6c6c 6574 7320 6f6e 2074  een wallets on t
-0005af70: 6865 2073 616d 6520 6163 636f 756e 740a  he same account.
-0005af80: 2020 2020 2020 2020 7365 6520 6874 7470          see http
-0005af90: 733a 2f2f 6279 6269 742d 6578 6368 616e  s://bybit-exchan
-0005afa0: 6765 2e67 6974 6875 622e 696f 2f64 6f63  ge.github.io/doc
-0005afb0: 732f 6163 636f 756e 745f 6173 7365 742f  s/account_asset/
-0005afc0: 2374 2d63 7265 6174 6569 6e74 6572 6e61  #t-createinterna
-0005afd0: 6c74 7261 6e73 6665 720a 2020 2020 2020  ltransfer.      
-0005afe0: 2020 7365 6520 6874 7470 733a 2f2f 6279    see https://by
-0005aff0: 6269 742d 6578 6368 616e 6765 2e67 6974  bit-exchange.git
-0005b000: 6875 622e 696f 2f64 6f63 732f 6163 636f  hub.io/docs/acco
-0005b010: 756e 745f 6173 7365 742f 7633 2f23 742d  unt_asset/v3/#t-
-0005b020: 6372 6561 7465 696e 7465 726e 616c 7472  createinternaltr
-0005b030: 616e 7366 6572 0a20 2020 2020 2020 203a  ansfer.        :
-0005b040: 7061 7261 6d20 7374 7220 636f 6465 3a20  param str code: 
-0005b050: 756e 6966 6965 6420 6375 7272 656e 6379  unified currency
-0005b060: 2063 6f64 650a 2020 2020 2020 2020 3a70   code.        :p
-0005b070: 6172 616d 2066 6c6f 6174 2061 6d6f 756e  aram float amoun
-0005b080: 743a 2061 6d6f 756e 7420 746f 2074 7261  t: amount to tra
-0005b090: 6e73 6665 720a 2020 2020 2020 2020 3a70  nsfer.        :p
-0005b0a0: 6172 616d 2073 7472 2066 726f 6d41 6363  aram str fromAcc
-0005b0b0: 6f75 6e74 3a20 6163 636f 756e 7420 746f  ount: account to
-0005b0c0: 2074 7261 6e73 6665 7220 6672 6f6d 0a20   transfer from. 
-0005b0d0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-0005b0e0: 7220 746f 4163 636f 756e 743a 2061 6363  r toAccount: acc
-0005b0f0: 6f75 6e74 2074 6f20 7472 616e 7366 6572  ount to transfer
-0005b100: 2074 6f0a 2020 2020 2020 2020 3a70 6172   to.        :par
-0005b110: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
-0005b120: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
-0005b130: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
-0005b140: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
-0005b150: 696e 740a 2020 2020 2020 2020 3a70 6172  int.        :par
-0005b160: 616d 2073 7472 2070 6172 616d 735b 2774  am str params['t
-0005b170: 7261 6e73 6665 7249 6427 5d3a 2055 5549  ransferId']: UUI
-0005b180: 442c 2077 6869 6368 2069 7320 756e 6971  D, which is uniq
-0005b190: 7565 2061 6372 6f73 7320 7468 6520 706c  ue across the pl
-0005b1a0: 6174 666f 726d 0a20 2020 2020 2020 203a  atform.        :
-0005b1b0: 7265 7475 726e 7320 6469 6374 3a20 6120  returns dict: a 
-0005b1c0: 6074 7261 6e73 6665 7220 7374 7275 6374  `transfer struct
-0005b1d0: 7572 6520 3c68 7474 7073 3a2f 2f64 6f63  ure <https://doc
-0005b1e0: 732e 6363 7874 2e63 6f6d 2f23 2f3f 6964  s.ccxt.com/#/?id
-0005b1f0: 3d74 7261 6e73 6665 722d 7374 7275 6374  =transfer-struct
-0005b200: 7572 653e 600a 2020 2020 2020 2020 2222  ure>`.        ""
-0005b210: 220a 2020 2020 2020 2020 7365 6c66 2e6c  ".        self.l
-0005b220: 6f61 645f 6d61 726b 6574 7328 290a 2020  oad_markets().  
-0005b230: 2020 2020 2020 7472 616e 7366 6572 4964        transferId
-0005b240: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
-0005b250: 696e 6728 7061 7261 6d73 2c20 2774 7261  ing(params, 'tra
-0005b260: 6e73 6665 7249 6427 2c20 7365 6c66 2e75  nsferId', self.u
-0005b270: 7569 6428 2929 0a20 2020 2020 2020 2061  uid()).        a
-0005b280: 6363 6f75 6e74 5479 7065 7320 3d20 7365  ccountTypes = se
-0005b290: 6c66 2e73 6166 655f 7661 6c75 6528 7365  lf.safe_value(se
-0005b2a0: 6c66 2e6f 7074 696f 6e73 2c20 2761 6363  lf.options, 'acc
-0005b2b0: 6f75 6e74 7342 7954 7970 6527 2c20 7b7d  ountsByType', {}
-0005b2c0: 290a 2020 2020 2020 2020 6672 6f6d 4964  ).        fromId
-0005b2d0: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
-0005b2e0: 696e 6728 6163 636f 756e 7454 7970 6573  ing(accountTypes
-0005b2f0: 2c20 6672 6f6d 4163 636f 756e 742c 2066  , fromAccount, f
-0005b300: 726f 6d41 6363 6f75 6e74 290a 2020 2020  romAccount).    
-0005b310: 2020 2020 746f 4964 203d 2073 656c 662e      toId = self.
-0005b320: 7361 6665 5f73 7472 696e 6728 6163 636f  safe_string(acco
-0005b330: 756e 7454 7970 6573 2c20 746f 4163 636f  untTypes, toAcco
-0005b340: 756e 742c 2074 6f41 6363 6f75 6e74 290a  unt, toAccount).
-0005b350: 2020 2020 2020 2020 6375 7272 656e 6379          currency
-0005b360: 203d 2073 656c 662e 6375 7272 656e 6379   = self.currency
-0005b370: 2863 6f64 6529 0a20 2020 2020 2020 2061  (code).        a
-0005b380: 6d6f 756e 7454 6f50 7265 6369 7369 6f6e  mountToPrecision
-0005b390: 203d 2073 656c 662e 6375 7272 656e 6379   = self.currency
-0005b3a0: 5f74 6f5f 7072 6563 6973 696f 6e28 636f  _to_precision(co
-0005b3b0: 6465 2c20 616d 6f75 6e74 290a 2020 2020  de, amount).    
-0005b3c0: 2020 2020 6d65 7468 6f64 203d 204e 6f6e      method = Non
-0005b3d0: 650a 2020 2020 2020 2020 6d65 7468 6f64  e.        method
-0005b3e0: 2c20 7061 7261 6d73 203d 2073 656c 662e  , params = self.
-0005b3f0: 6861 6e64 6c65 5f6f 7074 696f 6e5f 616e  handle_option_an
-0005b400: 645f 7061 7261 6d73 2870 6172 616d 732c  d_params(params,
-0005b410: 2027 7472 616e 7366 6572 272c 2027 6d65   'transfer', 'me
-0005b420: 7468 6f64 272c 2027 7072 6976 6174 6550  thod', 'privateP
-0005b430: 6f73 7441 7373 6574 5631 5072 6976 6174  ostAssetV1Privat
-0005b440: 6554 7261 6e73 6665 7227 2920 2023 2076  eTransfer')  # v
-0005b450: 3120 7072 6566 6572 7265 6420 6174 6d2c  1 preferred atm,
-0005b460: 2062 6563 6175 7365 2069 7420 7375 7070   because it supp
-0005b470: 6f72 7473 2066 756e 6469 6e67 0a20 2020  orts funding.   
-0005b480: 2020 2020 2072 6571 7565 7374 203d 204e       request = N
-0005b490: 6f6e 650a 2020 2020 2020 2020 6966 206d  one.        if m
-0005b4a0: 6574 686f 6420 3d3d 2027 7072 6976 6174  ethod == 'privat
-0005b4b0: 6550 6f73 7441 7373 6574 5633 5072 6976  ePostAssetV3Priv
-0005b4c0: 6174 6554 7261 6e73 6665 7249 6e74 6572  ateTransferInter
-0005b4d0: 5472 616e 7366 6572 2720 6f72 206d 6574  Transfer' or met
-0005b4e0: 686f 6420 3d3d 2027 7072 6976 6174 6550  hod == 'privateP
-0005b4f0: 6f73 7456 3541 7373 6574 5472 616e 7366  ostV5AssetTransf
-0005b500: 6572 496e 7465 7254 7261 6e73 6665 7227  erInterTransfer'
-0005b510: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0005b520: 7175 6573 7420 3d20 7b0a 2020 2020 2020  quest = {.      
-0005b530: 2020 2020 2020 2020 2020 2774 7261 6e73            'trans
-0005b540: 6665 7249 6427 3a20 7472 616e 7366 6572  ferId': transfer
-0005b550: 4964 2c0a 2020 2020 2020 2020 2020 2020  Id,.            
-0005b560: 2020 2020 2766 726f 6d41 6363 6f75 6e74      'fromAccount
-0005b570: 5479 7065 273a 2066 726f 6d49 642c 0a20  Type': fromId,. 
-0005b580: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0005b590: 746f 4163 636f 756e 7454 7970 6527 3a20  toAccountType': 
-0005b5a0: 746f 4964 2c0a 2020 2020 2020 2020 2020  toId,.          
-0005b5b0: 2020 2020 2020 2763 6f69 6e27 3a20 6375        'coin': cu
-0005b5c0: 7272 656e 6379 5b27 6964 275d 2c0a 2020  rrency['id'],.  
-0005b5d0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-0005b5e0: 6d6f 756e 7427 3a20 616d 6f75 6e74 546f  mount': amountTo
-0005b5f0: 5072 6563 6973 696f 6e2c 0a20 2020 2020  Precision,.     
-0005b600: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0005b610: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0005b620: 2020 2072 6571 7565 7374 203d 207b 0a20     request = {. 
-0005b630: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0005b640: 7472 616e 7366 6572 5f69 6427 3a20 7472  transfer_id': tr
-0005b650: 616e 7366 6572 4964 2c0a 2020 2020 2020  ansferId,.      
-0005b660: 2020 2020 2020 2020 2020 2766 726f 6d5f            'from_
-0005b670: 6163 636f 756e 745f 7479 7065 273a 2066  account_type': f
-0005b680: 726f 6d49 642c 0a20 2020 2020 2020 2020  romId,.         
-0005b690: 2020 2020 2020 2027 746f 5f61 6363 6f75         'to_accou
-0005b6a0: 6e74 5f74 7970 6527 3a20 746f 4964 2c0a  nt_type': toId,.
-0005b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005b6c0: 2763 6f69 6e27 3a20 6375 7272 656e 6379  'coin': currency
-0005b6d0: 5b27 6964 275d 2c0a 2020 2020 2020 2020  ['id'],.        
-0005b6e0: 2020 2020 2020 2020 2761 6d6f 756e 7427          'amount'
-0005b6f0: 3a20 616d 6f75 6e74 546f 5072 6563 6973  : amountToPrecis
-0005b700: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-0005b710: 207d 0a20 2020 2020 2020 2072 6573 706f   }.        respo
-0005b720: 6e73 6520 3d20 6765 7461 7474 7228 7365  nse = getattr(se
-0005b730: 6c66 2c20 6d65 7468 6f64 2928 7365 6c66  lf, method)(self
-0005b740: 2e65 7874 656e 6428 7265 7175 6573 742c  .extend(request,
-0005b750: 2070 6172 616d 7329 290a 2020 2020 2020   params)).      
-0005b760: 2020 230a 2020 2020 2020 2020 2320 7b0a    #.        # {.
-0005b770: 2020 2020 2020 2020 2320 2020 2020 2272          #     "r
-0005b780: 6574 436f 6465 223a 2030 2c0a 2020 2020  etCode": 0,.    
-0005b790: 2020 2020 2320 2020 2020 2272 6574 4d73      #     "retMs
-0005b7a0: 6722 3a20 2273 7563 6365 7373 222c 0a20  g": "success",. 
-0005b7b0: 2020 2020 2020 2023 2020 2020 2022 7265         #     "re
-0005b7c0: 7375 6c74 223a 207b 0a20 2020 2020 2020  sult": {.       
-0005b7d0: 2023 2020 2020 2020 2020 2022 7472 616e   #         "tran
-0005b7e0: 7366 6572 4964 223a 2022 3432 3434 6166  sferId": "4244af
-0005b7f0: 3434 2d66 3362 302d 3463 6636 2d61 3734  44-f3b0-4cf6-a74
-0005b800: 332d 6235 3635 3630 6539 3837 6263 2220  3-b56560e987bc" 
-0005b810: 2023 2074 7261 6e73 6665 725f 6964 2069   # transfer_id i
-0005b820: 6e20 7631 0a20 2020 2020 2020 2023 2020  n v1.        #  
-0005b830: 2020 207d 2c0a 2020 2020 2020 2020 2320     },.        # 
-0005b840: 2020 2020 2272 6574 4578 7449 6e66 6f22      "retExtInfo"
-0005b850: 3a20 7b7d 2c0a 2020 2020 2020 2020 2320  : {},.        # 
-0005b860: 2020 2020 2274 696d 6522 3a20 3136 3636      "time": 1666
-0005b870: 3837 3538 3537 3230 350a 2020 2020 2020  875857205.      
-0005b880: 2020 2320 7d0a 2020 2020 2020 2020 230a    # }.        #.
-0005b890: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
-0005b8a0: 7020 3d20 7365 6c66 2e73 6166 655f 696e  p = self.safe_in
-0005b8b0: 7465 6765 725f 3228 7265 7370 6f6e 7365  teger_2(response
-0005b8c0: 2c20 2774 696d 6527 2c20 2774 696d 655f  , 'time', 'time_
-0005b8d0: 6e6f 7727 290a 2020 2020 2020 2020 7472  now').        tr
-0005b8e0: 616e 7366 6572 203d 2073 656c 662e 7361  ansfer = self.sa
-0005b8f0: 6665 5f76 616c 7565 2872 6573 706f 6e73  fe_value(respons
-0005b900: 652c 2027 7265 7375 6c74 272c 207b 7d29  e, 'result', {})
-0005b910: 0a20 2020 2020 2020 2073 7461 7475 7352  .        statusR
-0005b920: 6177 203d 2073 656c 662e 7361 6665 5f73  aw = self.safe_s
-0005b930: 7472 696e 675f 6e28 7265 7370 6f6e 7365  tring_n(response
-0005b940: 2c20 5b27 7265 7443 6f64 6527 2c20 2772  , ['retCode', 'r
-0005b950: 6574 4d73 6727 2c20 2772 6574 5f63 6f64  etMsg', 'ret_cod
-0005b960: 6527 2c20 2772 6574 5f6d 7367 275d 290a  e', 'ret_msg']).
-0005b970: 2020 2020 2020 2020 7374 6174 7573 203d          status =
-0005b980: 2073 656c 662e 7061 7273 655f 7472 616e   self.parse_tran
-0005b990: 7366 6572 5f73 7461 7475 7328 7374 6174  sfer_status(stat
-0005b9a0: 7573 5261 7729 0a20 2020 2020 2020 2072  usRaw).        r
-0005b9b0: 6574 7572 6e20 7365 6c66 2e65 7874 656e  eturn self.exten
-0005b9c0: 6428 7365 6c66 2e70 6172 7365 5f74 7261  d(self.parse_tra
-0005b9d0: 6e73 6665 7228 7472 616e 7366 6572 2c20  nsfer(transfer, 
-0005b9e0: 6375 7272 656e 6379 292c 207b 0a20 2020  currency), {.   
-0005b9f0: 2020 2020 2020 2020 2027 7469 6d65 7374           'timest
-0005ba00: 616d 7027 3a20 7469 6d65 7374 616d 702c  amp': timestamp,
-0005ba10: 0a20 2020 2020 2020 2020 2020 2027 6461  .            'da
-0005ba20: 7465 7469 6d65 273a 2073 656c 662e 6973  tetime': self.is
-0005ba30: 6f38 3630 3128 7469 6d65 7374 616d 7029  o8601(timestamp)
-0005ba40: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
-0005ba50: 6d6f 756e 7427 3a20 7365 6c66 2e70 6172  mount': self.par
-0005ba60: 7365 5f6e 756d 6265 7228 616d 6f75 6e74  se_number(amount
-0005ba70: 546f 5072 6563 6973 696f 6e29 2c0a 2020  ToPrecision),.  
-0005ba80: 2020 2020 2020 2020 2020 2766 726f 6d41            'fromA
-0005ba90: 6363 6f75 6e74 273a 2066 726f 6d41 6363  ccount': fromAcc
-0005baa0: 6f75 6e74 2c0a 2020 2020 2020 2020 2020  ount,.          
-0005bab0: 2020 2774 6f41 6363 6f75 6e74 273a 2074    'toAccount': t
-0005bac0: 6f41 6363 6f75 6e74 2c0a 2020 2020 2020  oAccount,.      
-0005bad0: 2020 2020 2020 2773 7461 7475 7327 3a20        'status': 
-0005bae0: 7374 6174 7573 2c0a 2020 2020 2020 2020  status,.        
-0005baf0: 7d29 0a0a 2020 2020 6465 6620 6665 7463  })..    def fetc
-0005bb00: 685f 7472 616e 7366 6572 7328 7365 6c66  h_transfers(self
-0005bb10: 2c20 636f 6465 3a20 4f70 7469 6f6e 616c  , code: Optional
-0005bb20: 5b73 7472 5d20 3d20 4e6f 6e65 2c20 7369  [str] = None, si
-0005bb30: 6e63 653a 204f 7074 696f 6e61 6c5b 696e  nce: Optional[in
-0005bb40: 745d 203d 204e 6f6e 652c 206c 696d 6974  t] = None, limit
-0005bb50: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0005bb60: 3d20 4e6f 6e65 2c20 7061 7261 6d73 3d7b  = None, params={
-0005bb70: 7d29 3a0a 2020 2020 2020 2020 2222 220a  }):.        """.
-0005bb80: 2020 2020 2020 2020 6665 7463 6820 6120          fetch a 
-0005bb90: 6869 7374 6f72 7920 6f66 2069 6e74 6572  history of inter
-0005bba0: 6e61 6c20 7472 616e 7366 6572 7320 6d61  nal transfers ma
-0005bbb0: 6465 206f 6e20 616e 2061 6363 6f75 6e74  de on an account
-0005bbc0: 0a20 2020 2020 2020 2073 6565 2068 7474  .        see htt
-0005bbd0: 7073 3a2f 2f62 7962 6974 2d65 7863 6861  ps://bybit-excha
-0005bbe0: 6e67 652e 6769 7468 7562 2e69 6f2f 646f  nge.github.io/do
-0005bbf0: 6373 2f76 352f 6173 7365 742f 696e 7465  cs/v5/asset/inte
-0005bc00: 722d 7472 616e 7366 6572 2d6c 6973 740a  r-transfer-list.
-0005bc10: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0005bc20: 7472 7c4e 6f6e 6520 636f 6465 3a20 756e  tr|None code: un
-0005bc30: 6966 6965 6420 6375 7272 656e 6379 2063  ified currency c
-0005bc40: 6f64 6520 6f66 2074 6865 2063 7572 7265  ode of the curre
-0005bc50: 6e63 7920 7472 616e 7366 6572 7265 640a  ncy transferred.
-0005bc60: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0005bc70: 6e74 7c4e 6f6e 6520 7369 6e63 653a 2074  nt|None since: t
-0005bc80: 6865 2065 6172 6c69 6573 7420 7469 6d65  he earliest time
-0005bc90: 2069 6e20 6d73 2074 6f20 6665 7463 6820   in ms to fetch 
-0005bca0: 7472 616e 7366 6572 7320 666f 720a 2020  transfers for.  
-0005bcb0: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
-0005bcc0: 7c4e 6f6e 6520 6c69 6d69 743a 2074 6865  |None limit: the
-0005bcd0: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
-0005bce0: 6f66 2020 7472 616e 7366 6572 7320 7374  of  transfers st
-0005bcf0: 7275 6374 7572 6573 2074 6f20 7265 7472  ructures to retr
-0005bd00: 6965 7665 0a20 2020 2020 2020 203a 7061  ieve.        :pa
-0005bd10: 7261 6d20 6469 6374 2070 6172 616d 733a  ram dict params:
-0005bd20: 2065 7874 7261 2070 6172 616d 6574 6572   extra parameter
-0005bd30: 7320 7370 6563 6966 6963 2074 6f20 7468  s specific to th
-0005bd40: 6520 6279 6269 7420 6170 6920 656e 6470  e bybit api endp
-0005bd50: 6f69 6e74 0a20 2020 2020 2020 203a 7265  oint.        :re
-0005bd60: 7475 726e 7320 5b64 6963 745d 3a20 6120  turns [dict]: a 
-0005bd70: 6c69 7374 206f 6620 6074 7261 6e73 6665  list of `transfe
-0005bd80: 7220 7374 7275 6374 7572 6573 203c 6874  r structures <ht
-0005bd90: 7470 733a 2f2f 646f 6373 2e63 6378 742e  tps://docs.ccxt.
-0005bda0: 636f 6d2f 232f 3f69 643d 7472 616e 7366  com/#/?id=transf
-0005bdb0: 6572 2d73 7472 7563 7475 7265 3e60 0a20  er-structure>`. 
-0005bdc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0005bdd0: 2020 2073 656c 662e 6c6f 6164 5f6d 6172     self.load_mar
-0005bde0: 6b65 7473 2829 0a20 2020 2020 2020 2063  kets().        c
-0005bdf0: 7572 7265 6e63 7920 3d20 4e6f 6e65 0a20  urrency = None. 
-0005be00: 2020 2020 2020 2072 6571 7565 7374 203d         request =
-0005be10: 207b 7d0a 2020 2020 2020 2020 6966 2063   {}.        if c
-0005be20: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-0005be30: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-0005be40: 7265 6e63 7920 3d20 7365 6c66 2e73 6166  rency = self.saf
-0005be50: 655f 6375 7272 656e 6379 5f63 6f64 6528  e_currency_code(
-0005be60: 636f 6465 290a 2020 2020 2020 2020 2020  code).          
-0005be70: 2020 7265 7175 6573 745b 2763 6f69 6e27    request['coin'
-0005be80: 5d20 3d20 6375 7272 656e 6379 0a20 2020  ] = currency.   
-0005be90: 2020 2020 2069 6620 7369 6e63 6520 6973       if since is
-0005bea0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0005beb0: 2020 2020 2020 2072 6571 7565 7374 5b27         request['
-0005bec0: 7374 6172 7454 696d 6527 5d20 3d20 7369  startTime'] = si
-0005bed0: 6e63 650a 2020 2020 2020 2020 6966 206c  nce.        if l
-0005bee0: 696d 6974 2069 7320 6e6f 7420 4e6f 6e65  imit is not None
-0005bef0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0005bf00: 7175 6573 745b 276c 696d 6974 275d 203d  quest['limit'] =
-0005bf10: 206c 696d 6974 0a20 2020 2020 2020 2072   limit.        r
-0005bf20: 6573 706f 6e73 6520 3d20 7365 6c66 2e70  esponse = self.p
-0005bf30: 7269 7661 7465 4765 7456 3541 7373 6574  rivateGetV5Asset
-0005bf40: 5472 616e 7366 6572 5175 6572 7949 6e74  TransferQueryInt
-0005bf50: 6572 5472 616e 7366 6572 4c69 7374 2873  erTransferList(s
-0005bf60: 656c 662e 6578 7465 6e64 2872 6571 7565  elf.extend(reque
-0005bf70: 7374 2c20 7061 7261 6d73 2929 0a20 2020  st, params)).   
-0005bf80: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-0005bf90: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0005bfa0: 2020 2020 2020 2020 2022 7265 7443 6f64           "retCod
-0005bfb0: 6522 3a20 302c 0a20 2020 2020 2020 2023  e": 0,.        #
-0005bfc0: 2020 2020 2020 2020 2022 7265 744d 7367           "retMsg
-0005bfd0: 223a 2022 7375 6363 6573 7322 2c0a 2020  ": "success",.  
-0005bfe0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005bff0: 2272 6573 756c 7422 3a20 7b0a 2020 2020  "result": {.    
-0005c000: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005c010: 2020 226c 6973 7422 3a20 5b0a 2020 2020    "list": [.    
-0005c020: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005c030: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0005c040: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0005c050: 2020 2020 2020 2274 7261 6e73 6665 7249        "transferI
-0005c060: 6422 3a20 2273 656c 6654 7261 6e73 6665  d": "selfTransfe
-0005c070: 725f 6131 3039 3163 6337 2d39 3336 342d  r_a1091cc7-9364-
-0005c080: 3462 3734 2d38 6465 312d 3138 6630 3263  4b74-8de1-18f02c
-0005c090: 3666 3264 3563 222c 0a20 2020 2020 2020  6f2d5c",.       
-0005c0a0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0005c0b0: 2020 2020 2020 2022 636f 696e 223a 2022         "coin": "
-0005c0c0: 5553 4454 222c 0a20 2020 2020 2020 2023  USDT",.        #
-0005c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005c0e0: 2020 2020 2022 616d 6f75 6e74 223a 2022       "amount": "
-0005c0f0: 3530 3030 222c 0a20 2020 2020 2020 2023  5000",.        #
-0005c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005c110: 2020 2020 2022 6672 6f6d 4163 636f 756e       "fromAccoun
-0005c120: 7454 7970 6522 3a20 2253 504f 5422 2c0a  tType": "SPOT",.
-0005c130: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005c140: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-0005c150: 6f41 6363 6f75 6e74 5479 7065 223a 2022  oAccountType": "
-0005c160: 554e 4946 4945 4422 2c0a 2020 2020 2020  UNIFIED",.      
-0005c170: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005c180: 2020 2020 2020 2020 2274 696d 6573 7461          "timesta
-0005c190: 6d70 223a 2022 3136 3637 3238 3332 3633  mp": "1667283263
-0005c1a0: 3030 3022 2c0a 2020 2020 2020 2020 2320  000",.        # 
-0005c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005c1c0: 2020 2020 2273 7461 7475 7322 3a20 2253      "status": "S
-0005c1d0: 5543 4345 5353 220a 2020 2020 2020 2020  UCCESS".        
-0005c1e0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0005c1f0: 2020 7d0a 2020 2020 2020 2020 2320 2020    }.        #   
-0005c200: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-0005c210: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0005c220: 2020 2022 6e65 7874 5061 6765 4375 7273     "nextPageCurs
-0005c230: 6f72 223a 2022 6579 4a74 6157 354a 5243  or": "eyJtaW5JRC
-0005c240: 4936 4d54 4d31 4f44 5132 4f43 7769 6257  I6MTM1ODQ2OCwibW
-0005c250: 4634 5355 5169 4f6a 457a 4e54 6730 4e6a  F4SUQiOjEzNTg0Nj
-0005c260: 6839 220a 2020 2020 2020 2020 2320 2020  h9".        #   
-0005c270: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-0005c280: 2023 2020 2020 2020 2020 2022 7265 7445   #         "retE
-0005c290: 7874 496e 666f 223a 207b 7d2c 0a20 2020  xtInfo": {},.   
-0005c2a0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005c2b0: 7469 6d65 223a 2031 3637 3039 3838 3237  time": 167098827
-0005c2c0: 3136 3737 0a20 2020 2020 2020 2023 2020  1677.        #  
-0005c2d0: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
-0005c2e0: 2020 2020 2020 2064 6174 6120 3d20 7365         data = se
-0005c2f0: 6c66 2e73 6166 655f 7661 6c75 6528 7265  lf.safe_value(re
-0005c300: 7370 6f6e 7365 2c20 2772 6573 756c 7427  sponse, 'result'
-0005c310: 2c20 7b7d 290a 2020 2020 2020 2020 7472  , {}).        tr
-0005c320: 616e 7366 6572 7320 3d20 7365 6c66 2e73  ansfers = self.s
-0005c330: 6166 655f 7661 6c75 6528 6461 7461 2c20  afe_value(data, 
-0005c340: 276c 6973 7427 2c20 5b5d 290a 2020 2020  'list', []).    
-0005c350: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0005c360: 7061 7273 655f 7472 616e 7366 6572 7328  parse_transfers(
-0005c370: 7472 616e 7366 6572 732c 2063 7572 7265  transfers, curre
-0005c380: 6e63 792c 2073 696e 6365 2c20 6c69 6d69  ncy, since, limi
-0005c390: 7429 0a0a 2020 2020 6465 6620 626f 7272  t)..    def borr
-0005c3a0: 6f77 5f6d 6172 6769 6e28 7365 6c66 2c20  ow_margin(self, 
-0005c3b0: 636f 6465 3a20 7374 722c 2061 6d6f 756e  code: str, amoun
-0005c3c0: 742c 2073 796d 626f 6c3a 204f 7074 696f  t, symbol: Optio
-0005c3d0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0005c3e0: 2070 6172 616d 733d 7b7d 293a 0a20 2020   params={}):.   
-0005c3f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0005c400: 2063 7265 6174 6520 6120 6c6f 616e 2074   create a loan t
-0005c410: 6f20 626f 7272 6f77 206d 6172 6769 6e0a  o borrow margin.
-0005c420: 2020 2020 2020 2020 7365 6520 6874 7470          see http
-0005c430: 733a 2f2f 6279 6269 742d 6578 6368 616e  s://bybit-exchan
-0005c440: 6765 2e67 6974 6875 622e 696f 2f64 6f63  ge.github.io/doc
-0005c450: 732f 7370 6f74 2f76 332f 2374 2d62 6f72  s/spot/v3/#t-bor
-0005c460: 726f 776d 6172 6769 6e6c 6f61 6e0a 2020  rowmarginloan.  
-0005c470: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-0005c480: 2063 6f64 653a 2075 6e69 6669 6564 2063   code: unified c
-0005c490: 7572 7265 6e63 7920 636f 6465 206f 6620  urrency code of 
-0005c4a0: 7468 6520 6375 7272 656e 6379 2074 6f20  the currency to 
-0005c4b0: 626f 7272 6f77 0a20 2020 2020 2020 203a  borrow.        :
-0005c4c0: 7061 7261 6d20 666c 6f61 7420 616d 6f75  param float amou
-0005c4d0: 6e74 3a20 7468 6520 616d 6f75 6e74 2074  nt: the amount t
-0005c4e0: 6f20 626f 7272 6f77 0a20 2020 2020 2020  o borrow.       
-0005c4f0: 203a 7061 7261 6d20 7374 727c 4e6f 6e65   :param str|None
-0005c500: 2073 796d 626f 6c3a 206e 6f74 2075 7365   symbol: not use
-0005c510: 6420 6279 2062 7962 6974 2e62 6f72 726f  d by bybit.borro
-0005c520: 774d 6172 6769 6e28 290a 2020 2020 2020  wMargin().      
-0005c530: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
-0005c540: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
-0005c550: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
-0005c560: 746f 2074 6865 2062 7962 6974 2061 7069  to the bybit api
-0005c570: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
-0005c580: 2020 3a72 6574 7572 6e73 2064 6963 743a    :returns dict:
-0005c590: 2061 2060 6d61 7267 696e 206c 6f61 6e20   a `margin loan 
-0005c5a0: 7374 7275 6374 7572 6520 3c68 7474 7073  structure <https
-0005c5b0: 3a2f 2f64 6f63 732e 6363 7874 2e63 6f6d  ://docs.ccxt.com
-0005c5c0: 2f23 2f3f 6964 3d6d 6172 6769 6e2d 6c6f  /#/?id=margin-lo
-0005c5d0: 616e 2d73 7472 7563 7475 7265 3e60 0a20  an-structure>`. 
-0005c5e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0005c5f0: 2020 2073 656c 662e 6c6f 6164 5f6d 6172     self.load_mar
-0005c600: 6b65 7473 2829 0a20 2020 2020 2020 2063  kets().        c
-0005c610: 7572 7265 6e63 7920 3d20 7365 6c66 2e63  urrency = self.c
-0005c620: 7572 7265 6e63 7928 636f 6465 290a 2020  urrency(code).  
-0005c630: 2020 2020 2020 6d61 7267 696e 4d6f 6465        marginMode
-0005c640: 2c20 7175 6572 7920 3d20 7365 6c66 2e68  , query = self.h
-0005c650: 616e 646c 655f 6d61 7267 696e 5f6d 6f64  andle_margin_mod
-0005c660: 655f 616e 645f 7061 7261 6d73 2827 626f  e_and_params('bo
-0005c670: 7272 6f77 4d61 7267 696e 272c 2070 6172  rrowMargin', par
-0005c680: 616d 7329 0a20 2020 2020 2020 2069 6620  ams).        if 
-0005c690: 6d61 7267 696e 4d6f 6465 203d 3d20 2769  marginMode == 'i
-0005c6a0: 736f 6c61 7465 6427 3a0a 2020 2020 2020  solated':.      
-0005c6b0: 2020 2020 2020 7261 6973 6520 4e6f 7453        raise NotS
-0005c6c0: 7570 706f 7274 6564 2873 656c 662e 6964  upported(self.id
-0005c6d0: 202b 2027 2062 6f72 726f 774d 6172 6769   + ' borrowMargi
-0005c6e0: 6e28 2920 6361 6e6e 6f74 2075 7365 2069  n() cannot use i
-0005c6f0: 736f 6c61 7465 6420 6d61 7267 696e 2729  solated margin')
-0005c700: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0005c710: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0005c720: 2027 636f 696e 273a 2063 7572 7265 6e63   'coin': currenc
-0005c730: 795b 2769 6427 5d2c 0a20 2020 2020 2020  y['id'],.       
-0005c740: 2020 2020 2027 7174 7927 3a20 7365 6c66       'qty': self
-0005c750: 2e63 7572 7265 6e63 795f 746f 5f70 7265  .currency_to_pre
-0005c760: 6369 7369 6f6e 2863 6f64 652c 2061 6d6f  cision(code, amo
-0005c770: 756e 7429 2c0a 2020 2020 2020 2020 7d0a  unt),.        }.
-0005c780: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0005c790: 203d 2073 656c 662e 7072 6976 6174 6550   = self.privateP
-0005c7a0: 6f73 7453 706f 7456 3350 7269 7661 7465  ostSpotV3Private
-0005c7b0: 4372 6f73 734d 6172 6769 6e4c 6f61 6e28  CrossMarginLoan(
-0005c7c0: 7365 6c66 2e65 7874 656e 6428 7265 7175  self.extend(requ
-0005c7d0: 6573 742c 2071 7565 7279 2929 0a20 2020  est, query)).   
-0005c7e0: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-0005c7f0: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0005c800: 2020 2020 2020 2020 2022 7265 7443 6f64           "retCod
-0005c810: 6522 3a20 302c 0a20 2020 2020 2020 2023  e": 0,.        #
-0005c820: 2020 2020 2020 2020 2022 7265 744d 7367           "retMsg
-0005c830: 223a 2022 7375 6363 6573 7322 2c0a 2020  ": "success",.  
-0005c840: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005c850: 2272 6573 756c 7422 3a20 7b0a 2020 2020  "result": {.    
-0005c860: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005c870: 2020 2274 7261 6e73 6163 7449 6422 3a20    "transactId": 
-0005c880: 2231 3431 3433 220a 2020 2020 2020 2020  "14143".        
-0005c890: 2320 2020 2020 2020 2020 7d2c 0a20 2020  #         },.   
-0005c8a0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005c8b0: 7265 7445 7874 496e 666f 223a 206e 756c  retExtInfo": nul
-0005c8c0: 6c2c 0a20 2020 2020 2020 2023 2020 2020  l,.        #    
-0005c8d0: 2020 2020 2022 7469 6d65 223a 2031 3636       "time": 166
-0005c8e0: 3236 3137 3834 3839 3730 0a20 2020 2020  2617848970.     
-0005c8f0: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
-0005c900: 2020 2023 0a20 2020 2020 2020 2072 6573     #.        res
-0005c910: 756c 7420 3d20 7365 6c66 2e73 6166 655f  ult = self.safe_
-0005c920: 7661 6c75 6528 7265 7370 6f6e 7365 2c20  value(response, 
-0005c930: 2772 6573 756c 7427 2c20 7b7d 290a 2020  'result', {}).  
-0005c940: 2020 2020 2020 7472 616e 7361 6374 696f        transactio
-0005c950: 6e20 3d20 7365 6c66 2e70 6172 7365 5f6d  n = self.parse_m
-0005c960: 6172 6769 6e5f 6c6f 616e 2872 6573 756c  argin_loan(resul
-0005c970: 742c 2063 7572 7265 6e63 7929 0a20 2020  t, currency).   
-0005c980: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0005c990: 2e65 7874 656e 6428 7472 616e 7361 6374  .extend(transact
-0005c9a0: 696f 6e2c 207b 0a20 2020 2020 2020 2020  ion, {.         
-0005c9b0: 2020 2027 7379 6d62 6f6c 273a 2073 796d     'symbol': sym
-0005c9c0: 626f 6c2c 0a20 2020 2020 2020 2020 2020  bol,.           
-0005c9d0: 2027 616d 6f75 6e74 273a 2061 6d6f 756e   'amount': amoun
-0005c9e0: 742c 0a20 2020 2020 2020 207d 290a 0a20  t,.        }).. 
-0005c9f0: 2020 2064 6566 2072 6570 6179 5f6d 6172     def repay_mar
-0005ca00: 6769 6e28 7365 6c66 2c20 636f 6465 3a20  gin(self, code: 
-0005ca10: 7374 722c 2061 6d6f 756e 742c 2073 796d  str, amount, sym
-0005ca20: 626f 6c3a 204f 7074 696f 6e61 6c5b 7374  bol: Optional[st
-0005ca30: 725d 203d 204e 6f6e 652c 2070 6172 616d  r] = None, param
-0005ca40: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
-0005ca50: 2222 0a20 2020 2020 2020 2072 6570 6179  "".        repay
-0005ca60: 2062 6f72 726f 7765 6420 6d61 7267 696e   borrowed margin
-0005ca70: 2061 6e64 2069 6e74 6572 6573 740a 2020   and interest.  
-0005ca80: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
-0005ca90: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
-0005caa0: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
-0005cab0: 7370 6f74 2f76 332f 2374 2d72 6570 6179  spot/v3/#t-repay
-0005cac0: 6d61 7267 696e 6c6f 616e 0a20 2020 2020  marginloan.     
-0005cad0: 2020 203a 7061 7261 6d20 7374 7220 636f     :param str co
-0005cae0: 6465 3a20 756e 6966 6965 6420 6375 7272  de: unified curr
-0005caf0: 656e 6379 2063 6f64 6520 6f66 2074 6865  ency code of the
-0005cb00: 2063 7572 7265 6e63 7920 746f 2072 6570   currency to rep
-0005cb10: 6179 0a20 2020 2020 2020 203a 7061 7261  ay.        :para
-0005cb20: 6d20 666c 6f61 7420 616d 6f75 6e74 3a20  m float amount: 
-0005cb30: 7468 6520 616d 6f75 6e74 2074 6f20 7265  the amount to re
-0005cb40: 7061 790a 2020 2020 2020 2020 3a70 6172  pay.        :par
-0005cb50: 616d 2073 7472 7c4e 6f6e 6520 7379 6d62  am str|None symb
-0005cb60: 6f6c 3a20 6e6f 7420 7573 6564 2062 7920  ol: not used by 
-0005cb70: 6279 6269 742e 7265 7061 794d 6172 6769  bybit.repayMargi
-0005cb80: 6e28 290a 2020 2020 2020 2020 3a70 6172  n().        :par
-0005cb90: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
-0005cba0: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
-0005cbb0: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
-0005cbc0: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
-0005cbd0: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
-0005cbe0: 7572 6e73 2064 6963 743a 2061 2060 6d61  urns dict: a `ma
-0005cbf0: 7267 696e 206c 6f61 6e20 7374 7275 6374  rgin loan struct
-0005cc00: 7572 6520 3c68 7474 7073 3a2f 2f64 6f63  ure <https://doc
-0005cc10: 732e 6363 7874 2e63 6f6d 2f23 2f3f 6964  s.ccxt.com/#/?id
-0005cc20: 3d6d 6172 6769 6e2d 6c6f 616e 2d73 7472  =margin-loan-str
-0005cc30: 7563 7475 7265 3e60 0a20 2020 2020 2020  ucture>`.       
-0005cc40: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-0005cc50: 662e 6c6f 6164 5f6d 6172 6b65 7473 2829  f.load_markets()
-0005cc60: 0a20 2020 2020 2020 2063 7572 7265 6e63  .        currenc
-0005cc70: 7920 3d20 7365 6c66 2e63 7572 7265 6e63  y = self.currenc
-0005cc80: 7928 636f 6465 290a 2020 2020 2020 2020  y(code).        
-0005cc90: 6d61 7267 696e 4d6f 6465 2c20 7175 6572  marginMode, quer
-0005cca0: 7920 3d20 7365 6c66 2e68 616e 646c 655f  y = self.handle_
-0005ccb0: 6d61 7267 696e 5f6d 6f64 655f 616e 645f  margin_mode_and_
-0005ccc0: 7061 7261 6d73 2827 7265 7061 794d 6172  params('repayMar
-0005ccd0: 6769 6e27 2c20 7061 7261 6d73 290a 2020  gin', params).  
-0005cce0: 2020 2020 2020 6966 206d 6172 6769 6e4d        if marginM
-0005ccf0: 6f64 6520 3d3d 2027 6973 6f6c 6174 6564  ode == 'isolated
-0005cd00: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
-0005cd10: 6169 7365 204e 6f74 5375 7070 6f72 7465  aise NotSupporte
-0005cd20: 6428 7365 6c66 2e69 6420 2b20 2720 7265  d(self.id + ' re
-0005cd30: 7061 794d 6172 6769 6e28 2920 6361 6e6e  payMargin() cann
-0005cd40: 6f74 2075 7365 2069 736f 6c61 7465 6420  ot use isolated 
-0005cd50: 6d61 7267 696e 2729 0a20 2020 2020 2020  margin').       
-0005cd60: 2072 6571 7565 7374 203d 207b 0a20 2020   request = {.   
-0005cd70: 2020 2020 2020 2020 2027 636f 696e 273a           'coin':
-0005cd80: 2063 7572 7265 6e63 795b 2769 6427 5d2c   currency['id'],
-0005cd90: 0a20 2020 2020 2020 2020 2020 2027 7174  .            'qt
-0005cda0: 7927 3a20 7365 6c66 2e6e 756d 6265 725f  y': self.number_
-0005cdb0: 746f 5f73 7472 696e 6728 616d 6f75 6e74  to_string(amount
-0005cdc0: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
-0005cdd0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-0005cde0: 7365 6c66 2e70 7269 7661 7465 506f 7374  self.privatePost
-0005cdf0: 5370 6f74 5633 5072 6976 6174 6543 726f  SpotV3PrivateCro
-0005ce00: 7373 4d61 7267 696e 5265 7061 7928 7365  ssMarginRepay(se
-0005ce10: 6c66 2e65 7874 656e 6428 7265 7175 6573  lf.extend(reques
-0005ce20: 742c 2071 7565 7279 2929 0a20 2020 2020  t, query)).     
-0005ce30: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-0005ce40: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
-0005ce50: 2020 2020 2020 2022 7265 7443 6f64 6522         "retCode"
-0005ce60: 3a20 302c 0a20 2020 2020 2020 2023 2020  : 0,.        #  
-0005ce70: 2020 2020 2020 2022 7265 744d 7367 223a         "retMsg":
-0005ce80: 2022 7375 6363 6573 7322 2c0a 2020 2020   "success",.    
-0005ce90: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
-0005cea0: 6573 756c 7422 3a20 7b0a 2020 2020 2020  esult": {.      
-0005ceb0: 2020 2320 2020 2020 2020 2020 2020 2022    #            "
-0005cec0: 7265 7061 7949 6422 3a20 2231 3231 3238  repayId": "12128
-0005ced0: 220a 2020 2020 2020 2020 2320 2020 2020  ".        #     
-0005cee0: 2020 2020 7d2c 0a20 2020 2020 2020 2023      },.        #
-0005cef0: 2020 2020 2020 2020 2022 7265 7445 7874           "retExt
-0005cf00: 496e 666f 223a 206e 756c 6c2c 0a20 2020  Info": null,.   
-0005cf10: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005cf20: 7469 6d65 223a 2031 3636 3236 3138 3239  time": 166261829
-0005cf30: 3834 3532 0a20 2020 2020 2020 2023 2020  8452.        #  
-0005cf40: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
-0005cf50: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0005cf60: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0005cf70: 7265 7370 6f6e 7365 2c20 2772 6573 756c  response, 'resul
-0005cf80: 7427 2c20 7b7d 290a 2020 2020 2020 2020  t', {}).        
-0005cf90: 7472 616e 7361 6374 696f 6e20 3d20 7365  transaction = se
-0005cfa0: 6c66 2e70 6172 7365 5f6d 6172 6769 6e5f  lf.parse_margin_
-0005cfb0: 6c6f 616e 2872 6573 756c 742c 2063 7572  loan(result, cur
-0005cfc0: 7265 6e63 7929 0a20 2020 2020 2020 2072  rency).        r
-0005cfd0: 6574 7572 6e20 7365 6c66 2e65 7874 656e  eturn self.exten
-0005cfe0: 6428 7472 616e 7361 6374 696f 6e2c 207b  d(transaction, {
-0005cff0: 0a20 2020 2020 2020 2020 2020 2027 7379  .            'sy
-0005d000: 6d62 6f6c 273a 2073 796d 626f 6c2c 0a20  mbol': symbol,. 
-0005d010: 2020 2020 2020 2020 2020 2027 616d 6f75             'amou
-0005d020: 6e74 273a 2061 6d6f 756e 742c 0a20 2020  nt': amount,.   
-0005d030: 2020 2020 207d 290a 0a20 2020 2064 6566       })..    def
-0005d040: 2070 6172 7365 5f6d 6172 6769 6e5f 6c6f   parse_margin_lo
-0005d050: 616e 2873 656c 662c 2069 6e66 6f2c 2063  an(self, info, c
-0005d060: 7572 7265 6e63 793d 4e6f 6e65 293a 0a20  urrency=None):. 
-0005d070: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0005d080: 2023 2062 6f72 726f 774d 6172 6769 6e0a   # borrowMargin.
-0005d090: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-0005d0a0: 2020 2320 2020 2020 7b0a 2020 2020 2020    #     {.      
-0005d0b0: 2020 2320 2020 2020 2020 2020 2274 7261    #         "tra
-0005d0c0: 6e73 6163 7449 6422 3a20 2231 3431 3433  nsactId": "14143
-0005d0d0: 220a 2020 2020 2020 2020 2320 2020 2020  ".        #     
-0005d0e0: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
-0005d0f0: 2020 2020 2320 7265 7061 794d 6172 6769      # repayMargi
-0005d100: 6e0a 2020 2020 2020 2020 230a 2020 2020  n.        #.    
-0005d110: 2020 2020 2320 2020 2020 7b0a 2020 2020      #     {.    
-0005d120: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
-0005d130: 6570 6179 4964 223a 2022 3132 3132 3822  epayId": "12128"
-0005d140: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
-0005d150: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005d160: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-0005d170: 2020 2020 2020 2020 2769 6427 3a20 7365          'id': se
-0005d180: 6c66 2e73 6166 655f 7374 7269 6e67 5f32  lf.safe_string_2
-0005d190: 2869 6e66 6f2c 2027 7472 616e 7361 6374  (info, 'transact
-0005d1a0: 4964 272c 2027 7265 7061 7949 6427 292c  Id', 'repayId'),
-0005d1b0: 0a20 2020 2020 2020 2020 2020 2027 6375  .            'cu
-0005d1c0: 7272 656e 6379 273a 2073 656c 662e 7361  rrency': self.sa
-0005d1d0: 6665 5f73 7472 696e 6728 6375 7272 656e  fe_string(curren
-0005d1e0: 6379 2c20 2763 6f64 6527 292c 0a20 2020  cy, 'code'),.   
-0005d1f0: 2020 2020 2020 2020 2027 616d 6f75 6e74           'amount
-0005d200: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
-0005d210: 2020 2020 2027 7379 6d62 6f6c 273a 204e       'symbol': N
-0005d220: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0005d230: 2027 7469 6d65 7374 616d 7027 3a20 4e6f   'timestamp': No
-0005d240: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0005d250: 2764 6174 6574 696d 6527 3a20 4e6f 6e65  'datetime': None
-0005d260: 2c0a 2020 2020 2020 2020 2020 2020 2769  ,.            'i
-0005d270: 6e66 6f27 3a20 696e 666f 2c0a 2020 2020  nfo': info,.    
-0005d280: 2020 2020 7d0a 0a20 2020 2064 6566 2070      }..    def p
-0005d290: 6172 7365 5f74 7261 6e73 6665 725f 7374  arse_transfer_st
-0005d2a0: 6174 7573 2873 656c 662c 2073 7461 7475  atus(self, statu
-0005d2b0: 7329 3a0a 2020 2020 2020 2020 7374 6174  s):.        stat
-0005d2c0: 7573 6573 203d 207b 0a20 2020 2020 2020  uses = {.       
-0005d2d0: 2020 2020 2027 3027 3a20 276f 6b27 2c0a       '0': 'ok',.
-0005d2e0: 2020 2020 2020 2020 2020 2020 274f 4b27              'OK'
-0005d2f0: 3a20 276f 6b27 2c0a 2020 2020 2020 2020  : 'ok',.        
-0005d300: 2020 2020 2753 5543 4345 5353 273a 2027      'SUCCESS': '
-0005d310: 6f6b 272c 0a20 2020 2020 2020 207d 0a20  ok',.        }. 
-0005d320: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0005d330: 6c66 2e73 6166 655f 7374 7269 6e67 2873  lf.safe_string(s
-0005d340: 7461 7475 7365 732c 2073 7461 7475 732c  tatuses, status,
-0005d350: 2073 7461 7475 7329 0a0a 2020 2020 6465   status)..    de
-0005d360: 6620 7061 7273 655f 7472 616e 7366 6572  f parse_transfer
-0005d370: 2873 656c 662c 2074 7261 6e73 6665 722c  (self, transfer,
-0005d380: 2063 7572 7265 6e63 793d 4e6f 6e65 293a   currency=None):
-0005d390: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005d3a0: 2020 2023 2074 7261 6e73 6665 720a 2020     # transfer.  
-0005d3b0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-0005d3c0: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
-0005d3d0: 2320 2020 2020 2020 2020 2274 7261 6e73  #         "trans
-0005d3e0: 6665 7249 6422 3a20 2232 3263 3262 6331  ferId": "22c2bc1
-0005d3f0: 312d 6564 3562 2d34 3961 342d 3836 3437  1-ed5b-49a4-8647
-0005d400: 2d63 3465 3066 3566 3666 3262 3222 2020  -c4e0f5f6f2b2"  
-0005d410: 2320 7472 616e 7366 6572 5f69 6420 696e  # transfer_id in
-0005d420: 2076 310a 2020 2020 2020 2020 2320 2020   v1.        #   
-0005d430: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
-0005d440: 2020 2020 2020 2320 6665 7463 6854 7261        # fetchTra
-0005d450: 6e73 6665 7273 0a20 2020 2020 2020 2023  nsfers.        #
-0005d460: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
-0005d470: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005d480: 2020 2022 7472 616e 7366 6572 4964 223a     "transferId":
-0005d490: 2022 6539 6334 3231 6334 2d62 3031 302d   "e9c421c4-b010-
-0005d4a0: 3462 3136 2d61 6264 362d 3130 3631 3739  4b16-abd6-106179
-0005d4b0: 6632 3737 3032 222c 2020 2320 7472 616e  f27702",  # tran
-0005d4c0: 7366 6572 5f69 6420 696e 2076 310a 2020  sfer_id in v1.  
-0005d4d0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005d4e0: 2263 6f69 6e22 3a20 2255 5344 5422 2c0a  "coin": "USDT",.
-0005d4f0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005d500: 2020 2261 6d6f 756e 7422 3a20 2238 222c    "amount": "8",
-0005d510: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005d520: 2020 2022 6672 6f6d 4163 636f 756e 7454     "fromAccountT
-0005d530: 7970 6522 3a20 2246 554e 4422 2c20 2023  ype": "FUND",  #
-0005d540: 2066 726f 6d5f 6163 636f 756e 745f 7479   from_account_ty
-0005d550: 7065 2069 6e20 7631 0a20 2020 2020 2020  pe in v1.       
-0005d560: 2023 2020 2020 2020 2020 2022 746f 4163   #         "toAc
-0005d570: 636f 756e 7454 7970 6522 3a20 2253 504f  countType": "SPO
-0005d580: 5422 2c20 2023 2074 6f5f 6163 636f 756e  T",  # to_accoun
-0005d590: 745f 7479 7065 2069 6e20 7631 0a20 2020  t_type in v1.   
-0005d5a0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005d5b0: 7469 6d65 7374 616d 7022 3a20 2231 3636  timestamp": "166
-0005d5c0: 3638 3739 3432 3630 3030 222c 0a20 2020  6879426000",.   
-0005d5d0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0005d5e0: 7374 6174 7573 223a 2022 5355 4343 4553  status": "SUCCES
-0005d5f0: 5322 0a20 2020 2020 2020 2023 2020 2020  S".        #    
-0005d600: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
-0005d610: 2020 2020 2020 6375 7272 656e 6379 4964        currencyId
-0005d620: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
-0005d630: 696e 6728 7472 616e 7366 6572 2c20 2763  ing(transfer, 'c
-0005d640: 6f69 6e27 290a 2020 2020 2020 2020 7469  oin').        ti
-0005d650: 6d65 7374 616d 7020 3d20 7365 6c66 2e73  mestamp = self.s
-0005d660: 6166 655f 696e 7465 6765 7228 7472 616e  afe_integer(tran
-0005d670: 7366 6572 2c20 2774 696d 6573 7461 6d70  sfer, 'timestamp
-0005d680: 2729 0a20 2020 2020 2020 2066 726f 6d41  ').        fromA
-0005d690: 6363 6f75 6e74 4964 203d 2073 656c 662e  ccountId = self.
-0005d6a0: 7361 6665 5f73 7472 696e 675f 3228 7472  safe_string_2(tr
-0005d6b0: 616e 7366 6572 2c20 2766 726f 6d41 6363  ansfer, 'fromAcc
-0005d6c0: 6f75 6e74 5479 7065 272c 2027 6672 6f6d  ountType', 'from
-0005d6d0: 5f61 6363 6f75 6e74 5f74 7970 6527 290a  _account_type').
-0005d6e0: 2020 2020 2020 2020 746f 4163 636f 756e          toAccoun
-0005d6f0: 7449 6420 3d20 7365 6c66 2e73 6166 655f  tId = self.safe_
-0005d700: 7374 7269 6e67 5f32 2874 7261 6e73 6665  string_2(transfe
-0005d710: 722c 2027 746f 4163 636f 756e 7454 7970  r, 'toAccountTyp
-0005d720: 6527 2c20 2774 6f5f 6163 636f 756e 745f  e', 'to_account_
-0005d730: 7479 7065 2729 0a20 2020 2020 2020 2061  type').        a
-0005d740: 6363 6f75 6e74 4964 7320 3d20 7365 6c66  ccountIds = self
-0005d750: 2e73 6166 655f 7661 6c75 6528 7365 6c66  .safe_value(self
-0005d760: 2e6f 7074 696f 6e73 2c20 2761 6363 6f75  .options, 'accou
-0005d770: 6e74 7342 7949 6427 2c20 7b7d 290a 2020  ntsById', {}).  
-0005d780: 2020 2020 2020 6672 6f6d 4163 636f 756e        fromAccoun
-0005d790: 7420 3d20 7365 6c66 2e73 6166 655f 7374  t = self.safe_st
-0005d7a0: 7269 6e67 2861 6363 6f75 6e74 4964 732c  ring(accountIds,
-0005d7b0: 2066 726f 6d41 6363 6f75 6e74 4964 2c20   fromAccountId, 
-0005d7c0: 6672 6f6d 4163 636f 756e 7449 6429 0a20  fromAccountId). 
-0005d7d0: 2020 2020 2020 2074 6f41 6363 6f75 6e74         toAccount
-0005d7e0: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
-0005d7f0: 696e 6728 6163 636f 756e 7449 6473 2c20  ing(accountIds, 
-0005d800: 746f 4163 636f 756e 7449 642c 2074 6f41  toAccountId, toA
-0005d810: 6363 6f75 6e74 4964 290a 2020 2020 2020  ccountId).      
-0005d820: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-0005d830: 2020 2020 2020 2027 696e 666f 273a 2074         'info': t
-0005d840: 7261 6e73 6665 722c 0a20 2020 2020 2020  ransfer,.       
-0005d850: 2020 2020 2027 6964 273a 2073 656c 662e       'id': self.
-0005d860: 7361 6665 5f73 7472 696e 675f 3228 7472  safe_string_2(tr
-0005d870: 616e 7366 6572 2c20 2774 7261 6e73 6665  ansfer, 'transfe
-0005d880: 7249 6427 2c20 2774 7261 6e73 6665 725f  rId', 'transfer_
-0005d890: 6964 2729 2c0a 2020 2020 2020 2020 2020  id'),.          
-0005d8a0: 2020 2774 696d 6573 7461 6d70 273a 2074    'timestamp': t
-0005d8b0: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
-0005d8c0: 2020 2020 2020 2764 6174 6574 696d 6527        'datetime'
-0005d8d0: 3a20 7365 6c66 2e69 736f 3836 3031 2874  : self.iso8601(t
-0005d8e0: 696d 6573 7461 6d70 292c 0a20 2020 2020  imestamp),.     
-0005d8f0: 2020 2020 2020 2027 6375 7272 656e 6379         'currency
-0005d900: 273a 2073 656c 662e 7361 6665 5f63 7572  ': self.safe_cur
-0005d910: 7265 6e63 795f 636f 6465 2863 7572 7265  rency_code(curre
-0005d920: 6e63 7949 642c 2063 7572 7265 6e63 7929  ncyId, currency)
-0005d930: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
-0005d940: 6d6f 756e 7427 3a20 7365 6c66 2e73 6166  mount': self.saf
-0005d950: 655f 6e75 6d62 6572 2874 7261 6e73 6665  e_number(transfe
-0005d960: 722c 2027 616d 6f75 6e74 2729 2c0a 2020  r, 'amount'),.  
-0005d970: 2020 2020 2020 2020 2020 2766 726f 6d41            'fromA
-0005d980: 6363 6f75 6e74 273a 2066 726f 6d41 6363  ccount': fromAcc
-0005d990: 6f75 6e74 2c0a 2020 2020 2020 2020 2020  ount,.          
-0005d9a0: 2020 2774 6f41 6363 6f75 6e74 273a 2074    'toAccount': t
-0005d9b0: 6f41 6363 6f75 6e74 2c0a 2020 2020 2020  oAccount,.      
-0005d9c0: 2020 2020 2020 2773 7461 7475 7327 3a20        'status': 
-0005d9d0: 7365 6c66 2e70 6172 7365 5f74 7261 6e73  self.parse_trans
-0005d9e0: 6665 725f 7374 6174 7573 2873 656c 662e  fer_status(self.
-0005d9f0: 7361 6665 5f73 7472 696e 6728 7472 616e  safe_string(tran
-0005da00: 7366 6572 2c20 2773 7461 7475 7327 2929  sfer, 'status'))
-0005da10: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-0005da20: 2064 6566 2066 6574 6368 5f64 6572 6976   def fetch_deriv
-0005da30: 6174 6976 6573 5f6d 6172 6b65 745f 6c65  atives_market_le
-0005da40: 7665 7261 6765 5f74 6965 7273 2873 656c  verage_tiers(sel
-0005da50: 662c 2073 796d 626f 6c3a 2073 7472 2c20  f, symbol: str, 
-0005da60: 7061 7261 6d73 3d7b 7d29 3a0a 2020 2020  params={}):.    
-0005da70: 2020 2020 7365 6c66 2e6c 6f61 645f 6d61      self.load_ma
-0005da80: 726b 6574 7328 290a 2020 2020 2020 2020  rkets().        
-0005da90: 6d61 726b 6574 203d 2073 656c 662e 6d61  market = self.ma
-0005daa0: 726b 6574 2873 796d 626f 6c29 0a20 2020  rket(symbol).   
-0005dab0: 2020 2020 2072 6571 7565 7374 203d 207b       request = {
-0005dac0: 0a20 2020 2020 2020 2020 2020 2027 7379  .            'sy
-0005dad0: 6d62 6f6c 273a 206d 6172 6b65 745b 2769  mbol': market['i
-0005dae0: 6427 5d2c 0a20 2020 2020 2020 207d 0a20  d'],.        }. 
-0005daf0: 2020 2020 2020 2069 6620 6d61 726b 6574         if market
-0005db00: 5b27 6c69 6e65 6172 275d 3a0a 2020 2020  ['linear']:.    
-0005db10: 2020 2020 2020 2020 7265 7175 6573 745b          request[
-0005db20: 2763 6174 6567 6f72 7927 5d20 3d20 276c  'category'] = 'l
-0005db30: 696e 6561 7227 0a20 2020 2020 2020 2065  inear'.        e
-0005db40: 6c69 6620 6d61 726b 6574 5b27 696e 7665  lif market['inve
-0005db50: 7273 6527 5d3a 0a20 2020 2020 2020 2020  rse']:.         
-0005db60: 2020 2072 6571 7565 7374 5b27 6361 7465     request['cate
-0005db70: 676f 7279 275d 203d 2027 696e 7665 7273  gory'] = 'invers
-0005db80: 6527 0a20 2020 2020 2020 2072 6573 706f  e'.        respo
-0005db90: 6e73 6520 3d20 7365 6c66 2e70 7562 6c69  nse = self.publi
-0005dba0: 6347 6574 5635 4d61 726b 6574 5269 736b  cGetV5MarketRisk
-0005dbb0: 4c69 6d69 7428 7365 6c66 2e65 7874 656e  Limit(self.exten
-0005dbc0: 6428 7265 7175 6573 742c 2070 6172 616d  d(request, param
-0005dbd0: 7329 290a 2020 2020 2020 2020 230a 2020  s)).        #.  
-0005dbe0: 2020 2020 2020 2320 2020 2020 7b0a 2020        #     {.  
-0005dbf0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005dc00: 2272 6574 436f 6465 223a 2030 2c0a 2020  "retCode": 0,.  
-0005dc10: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005dc20: 2272 6574 4d73 6722 3a20 224f 4b22 2c0a  "retMsg": "OK",.
-0005dc30: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005dc40: 2020 2272 6573 756c 7422 3a20 7b0a 2020    "result": {.  
-0005dc50: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005dc60: 2020 2020 2263 6174 6567 6f72 7922 3a20      "category": 
-0005dc70: 2269 6e76 6572 7365 222c 0a20 2020 2020  "inverse",.     
-0005dc80: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005dc90: 2022 6c69 7374 223a 205b 0a20 2020 2020   "list": [.     
-0005dca0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0005dcb0: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-0005dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005dcd0: 2020 2020 2022 6964 223a 2031 2c0a 2020       "id": 1,.  
-0005dce0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005dcf0: 2020 2020 2020 2020 2020 2020 2273 796d              "sym
-0005dd00: 626f 6c22 3a20 2242 5443 5553 4422 2c0a  bol": "BTCUSD",.
-0005dd10: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005dd20: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-0005dd30: 6973 6b4c 696d 6974 5661 6c75 6522 3a20  iskLimitValue": 
-0005dd40: 2231 3530 222c 0a20 2020 2020 2020 2023  "150",.        #
-0005dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005dd60: 2020 2020 2022 6d61 696e 7465 6e61 6e63       "maintenanc
-0005dd70: 654d 6172 6769 6e22 3a20 2230 2e35 222c  eMargin": "0.5",
-0005dd80: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005dd90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0005dda0: 696e 6974 6961 6c4d 6172 6769 6e22 3a20  initialMargin": 
-0005ddb0: 2231 222c 0a20 2020 2020 2020 2023 2020  "1",.        #  
-0005ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005ddd0: 2020 2022 6973 4c6f 7765 7374 5269 736b     "isLowestRisk
-0005dde0: 223a 2031 2c0a 2020 2020 2020 2020 2320  ": 1,.        # 
-0005ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005de00: 2020 2020 226d 6178 4c65 7665 7261 6765      "maxLeverage
-0005de10: 223a 2022 3130 302e 3030 220a 2020 2020  ": "100.00".    
-0005de20: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005de30: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-0005de40: 2023 2020 2020 2020 2020 2020 2020 202e   #             .
-0005de50: 2e2e 2e0a 2020 2020 2020 2020 2320 2020  ....        #   
-0005de60: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-0005de70: 2020 2020 2320 2020 2020 2020 2020 7d2c      #         },
-0005de80: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005de90: 2020 2022 7265 7445 7874 496e 666f 223a     "retExtInfo":
-0005dea0: 207b 7d2c 0a20 2020 2020 2020 2023 2020   {},.        #  
-0005deb0: 2020 2020 2020 2022 7469 6d65 223a 2031         "time": 1
-0005dec0: 3637 3230 3534 3438 3830 3130 0a20 2020  672054488010.   
-0005ded0: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-0005dee0: 2020 2020 2023 0a20 2020 2020 2020 2072       #.        r
-0005def0: 6573 756c 7420 3d20 7365 6c66 2e73 6166  esult = self.saf
-0005df00: 655f 7661 6c75 6528 7265 7370 6f6e 7365  e_value(response
-0005df10: 2c20 2772 6573 756c 7427 290a 2020 2020  , 'result').    
-0005df20: 2020 2020 7469 6572 7320 3d20 7365 6c66      tiers = self
-0005df30: 2e73 6166 655f 7661 6c75 6528 7265 7375  .safe_value(resu
-0005df40: 6c74 2c20 276c 6973 7427 290a 2020 2020  lt, 'list').    
-0005df50: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0005df60: 7061 7273 655f 6d61 726b 6574 5f6c 6576  parse_market_lev
-0005df70: 6572 6167 655f 7469 6572 7328 7469 6572  erage_tiers(tier
-0005df80: 732c 206d 6172 6b65 7429 0a0a 2020 2020  s, market)..    
-0005df90: 6465 6620 6665 7463 685f 6d61 726b 6574  def fetch_market
-0005dfa0: 5f6c 6576 6572 6167 655f 7469 6572 7328  _leverage_tiers(
-0005dfb0: 7365 6c66 2c20 7379 6d62 6f6c 3a20 7374  self, symbol: st
-0005dfc0: 722c 2070 6172 616d 733d 7b7d 293a 0a20  r, params={}):. 
-0005dfd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0005dfe0: 2020 2072 6574 7269 6576 6520 696e 666f     retrieve info
-0005dff0: 726d 6174 696f 6e20 6f6e 2074 6865 206d  rmation on the m
-0005e000: 6178 696d 756d 206c 6576 6572 6167 652c  aximum leverage,
-0005e010: 2061 6e64 206d 6169 6e74 656e 616e 6365   and maintenance
-0005e020: 206d 6172 6769 6e20 666f 7220 7472 6164   margin for trad
-0005e030: 6573 206f 6620 7661 7279 696e 6720 7472  es of varying tr
-0005e040: 6164 6520 7369 7a65 7320 666f 7220 6120  ade sizes for a 
-0005e050: 7369 6e67 6c65 206d 6172 6b65 740a 2020  single market.  
-0005e060: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
-0005e070: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
-0005e080: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
-0005e090: 7635 2f6d 6172 6b65 742f 7269 736b 2d6c  v5/market/risk-l
-0005e0a0: 696d 6974 0a20 2020 2020 2020 203a 7061  imit.        :pa
-0005e0b0: 7261 6d20 7374 7220 7379 6d62 6f6c 3a20  ram str symbol: 
-0005e0c0: 756e 6966 6965 6420 6d61 726b 6574 2073  unified market s
-0005e0d0: 796d 626f 6c0a 2020 2020 2020 2020 3a70  ymbol.        :p
-0005e0e0: 6172 616d 2064 6963 7420 7061 7261 6d73  aram dict params
-0005e0f0: 3a20 6578 7472 6120 7061 7261 6d65 7465  : extra paramete
-0005e100: 7273 2073 7065 6369 6669 6320 746f 2074  rs specific to t
-0005e110: 6865 2062 7962 6974 2061 7069 2065 6e64  he bybit api end
-0005e120: 706f 696e 740a 2020 2020 2020 2020 3a72  point.        :r
-0005e130: 6574 7572 6e73 2064 6963 743a 2061 2060  eturns dict: a `
-0005e140: 6c65 7665 7261 6765 2074 6965 7273 2073  leverage tiers s
-0005e150: 7472 7563 7475 7265 203c 6874 7470 733a  tructure <https:
-0005e160: 2f2f 646f 6373 2e63 6378 742e 636f 6d2f  //docs.ccxt.com/
-0005e170: 232f 3f69 643d 6c65 7665 7261 6765 2d74  #/?id=leverage-t
-0005e180: 6965 7273 2d73 7472 7563 7475 7265 3e60  iers-structure>`
-0005e190: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0005e1a0: 2020 2020 2073 656c 662e 6c6f 6164 5f6d       self.load_m
-0005e1b0: 6172 6b65 7473 2829 0a20 2020 2020 2020  arkets().       
-0005e1c0: 2072 6571 7565 7374 203d 207b 7d0a 2020   request = {}.  
-0005e1d0: 2020 2020 2020 6d61 726b 6574 203d 204e        market = N
-0005e1e0: 6f6e 650a 2020 2020 2020 2020 6d61 726b  one.        mark
-0005e1f0: 6574 203d 2073 656c 662e 6d61 726b 6574  et = self.market
-0005e200: 2873 796d 626f 6c29 0a20 2020 2020 2020  (symbol).       
-0005e210: 2069 6620 6d61 726b 6574 5b27 7370 6f74   if market['spot
-0005e220: 275d 206f 7220 6d61 726b 6574 5b27 6f70  '] or market['op
-0005e230: 7469 6f6e 275d 3a0a 2020 2020 2020 2020  tion']:.        
-0005e240: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
-0005e250: 7565 7374 2873 656c 662e 6964 202b 2027  uest(self.id + '
-0005e260: 2066 6574 6368 4d61 726b 6574 4c65 7665   fetchMarketLeve
-0005e270: 7261 6765 5469 6572 7328 2920 7379 6d62  rageTiers() symb
-0005e280: 6f6c 2064 6f65 7320 6e6f 7420 7375 7070  ol does not supp
-0005e290: 6f72 7420 6d61 726b 6574 2027 202b 2073  ort market ' + s
-0005e2a0: 796d 626f 6c29 0a20 2020 2020 2020 2072  ymbol).        r
-0005e2b0: 6571 7565 7374 5b27 7379 6d62 6f6c 275d  equest['symbol']
-0005e2c0: 203d 206d 6172 6b65 745b 2769 6427 5d0a   = market['id'].
-0005e2d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0005e2e0: 656c 662e 6665 7463 685f 6465 7269 7661  elf.fetch_deriva
-0005e2f0: 7469 7665 735f 6d61 726b 6574 5f6c 6576  tives_market_lev
-0005e300: 6572 6167 655f 7469 6572 7328 7379 6d62  erage_tiers(symb
-0005e310: 6f6c 2c20 7061 7261 6d73 290a 0a20 2020  ol, params)..   
-0005e320: 2064 6566 2070 6172 7365 5f6d 6172 6b65   def parse_marke
-0005e330: 745f 6c65 7665 7261 6765 5f74 6965 7273  t_leverage_tiers
-0005e340: 2873 656c 662c 2069 6e66 6f2c 206d 6172  (self, info, mar
-0005e350: 6b65 743d 4e6f 6e65 293a 0a20 2020 2020  ket=None):.     
-0005e360: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-0005e370: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
-0005e380: 2020 2020 2020 2022 6964 223a 2031 2c0a         "id": 1,.
-0005e390: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005e3a0: 2020 2273 796d 626f 6c22 3a20 2242 5443    "symbol": "BTC
-0005e3b0: 5553 4422 2c0a 2020 2020 2020 2020 2320  USD",.        # 
-0005e3c0: 2020 2020 2020 2020 2272 6973 6b4c 696d          "riskLim
-0005e3d0: 6974 5661 6c75 6522 3a20 2231 3530 222c  itValue": "150",
-0005e3e0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005e3f0: 2020 2022 6d61 696e 7465 6e61 6e63 654d     "maintenanceM
-0005e400: 6172 6769 6e22 3a20 2230 2e35 222c 0a20  argin": "0.5",. 
-0005e410: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005e420: 2022 696e 6974 6961 6c4d 6172 6769 6e22   "initialMargin"
-0005e430: 3a20 2231 222c 0a20 2020 2020 2020 2023  : "1",.        #
-0005e440: 2020 2020 2020 2020 2022 6973 4c6f 7765           "isLowe
-0005e450: 7374 5269 736b 223a 2031 2c0a 2020 2020  stRisk": 1,.    
-0005e460: 2020 2020 2320 2020 2020 2020 2020 226d      #         "m
-0005e470: 6178 4c65 7665 7261 6765 223a 2022 3130  axLeverage": "10
-0005e480: 302e 3030 220a 2020 2020 2020 2020 2320  0.00".        # 
-0005e490: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
-0005e4a0: 2020 2020 2020 2020 6d69 6e4e 6f74 696f          minNotio
-0005e4b0: 6e61 6c20 3d20 300a 2020 2020 2020 2020  nal = 0.        
-0005e4c0: 7469 6572 7320 3d20 5b5d 0a20 2020 2020  tiers = [].     
-0005e4d0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0005e4e0: 6528 302c 206c 656e 2869 6e66 6f29 293a  e(0, len(info)):
-0005e4f0: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-0005e500: 6d20 3d20 696e 666f 5b69 5d0a 2020 2020  m = info[i].    
-0005e510: 2020 2020 2020 2020 6d61 784e 6f74 696f          maxNotio
-0005e520: 6e61 6c20 3d20 7365 6c66 2e73 6166 655f  nal = self.safe_
-0005e530: 6e75 6d62 6572 2869 7465 6d2c 2027 7269  number(item, 'ri
-0005e540: 736b 4c69 6d69 7456 616c 7565 2729 0a20  skLimitValue'). 
-0005e550: 2020 2020 2020 2020 2020 2074 6965 7273             tiers
-0005e560: 2e61 7070 656e 6428 7b0a 2020 2020 2020  .append({.      
-0005e570: 2020 2020 2020 2020 2020 2774 6965 7227            'tier'
-0005e580: 3a20 7365 6c66 2e73 756d 2869 2c20 3129  : self.sum(i, 1)
-0005e590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0005e5a0: 2020 2763 7572 7265 6e63 7927 3a20 6d61    'currency': ma
-0005e5b0: 726b 6574 5b27 6261 7365 275d 2c0a 2020  rket['base'],.  
-0005e5c0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-0005e5d0: 696e 4e6f 7469 6f6e 616c 273a 206d 696e  inNotional': min
-0005e5e0: 4e6f 7469 6f6e 616c 2c0a 2020 2020 2020  Notional,.      
-0005e5f0: 2020 2020 2020 2020 2020 276d 6178 4e6f            'maxNo
-0005e600: 7469 6f6e 616c 273a 206d 6178 4e6f 7469  tional': maxNoti
-0005e610: 6f6e 616c 2c0a 2020 2020 2020 2020 2020  onal,.          
-0005e620: 2020 2020 2020 276d 6169 6e74 656e 616e        'maintenan
-0005e630: 6365 4d61 7267 696e 5261 7465 273a 2073  ceMarginRate': s
-0005e640: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
-0005e650: 6974 656d 2c20 276d 6169 6e74 656e 616e  item, 'maintenan
-0005e660: 6365 4d61 7267 696e 2729 2c0a 2020 2020  ceMargin'),.    
-0005e670: 2020 2020 2020 2020 2020 2020 276d 6178              'max
-0005e680: 4c65 7665 7261 6765 273a 2073 656c 662e  Leverage': self.
-0005e690: 7361 6665 5f6e 756d 6265 7228 6974 656d  safe_number(item
-0005e6a0: 2c20 276d 6178 4c65 7665 7261 6765 2729  , 'maxLeverage')
+00058a20: 2064 6174 6120 3d20 7365 6c66 2e73 6166   data = self.saf
+00058a30: 655f 7661 6c75 6528 7265 7375 6c74 2c20  e_value(result, 
+00058a40: 276c 6973 7427 2c20 5b5d 290a 2020 2020  'list', []).    
+00058a50: 2020 2020 7061 6769 6e61 7469 6f6e 4375      paginationCu
+00058a60: 7273 6f72 203d 2073 656c 662e 7361 6665  rsor = self.safe
+00058a70: 5f73 7472 696e 6728 7265 7375 6c74 2c20  _string(result, 
+00058a80: 276e 6578 7450 6167 6543 7572 736f 7227  'nextPageCursor'
+00058a90: 290a 2020 2020 2020 2020 6966 2028 7061  ).        if (pa
+00058aa0: 6769 6e61 7469 6f6e 4375 7273 6f72 2069  ginationCursor i
+00058ab0: 7320 6e6f 7420 4e6f 6e65 2920 616e 6420  s not None) and 
+00058ac0: 286c 656e 2864 6174 6129 203e 2030 293a  (len(data) > 0):
+00058ad0: 0a20 2020 2020 2020 2020 2020 2066 6972  .            fir
+00058ae0: 7374 203d 2064 6174 615b 305d 0a20 2020  st = data[0].   
+00058af0: 2020 2020 2020 2020 2066 6972 7374 5b27           first['
+00058b00: 6e65 7874 5061 6765 4375 7273 6f72 275d  nextPageCursor']
+00058b10: 203d 2070 6167 696e 6174 696f 6e43 7572   = paginationCur
+00058b20: 736f 720a 2020 2020 2020 2020 2020 2020  sor.            
+00058b30: 6461 7461 5b30 5d20 3d20 6669 7273 740a  data[0] = first.
+00058b40: 2020 2020 2020 2020 6964 203d 2073 656c          id = sel
+00058b50: 662e 7361 6665 5f73 7472 696e 6728 7265  f.safe_string(re
+00058b60: 7375 6c74 2c20 2773 796d 626f 6c27 290a  sult, 'symbol').
+00058b70: 2020 2020 2020 2020 6d61 726b 6574 203d          market =
+00058b80: 2073 656c 662e 7361 6665 5f6d 6172 6b65   self.safe_marke
+00058b90: 7428 6964 2c20 6d61 726b 6574 2c20 4e6f  t(id, market, No
+00058ba0: 6e65 2c20 2763 6f6e 7472 6163 7427 290a  ne, 'contract').
+00058bb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00058bc0: 656c 662e 7061 7273 655f 6f70 656e 5f69  elf.parse_open_i
+00058bd0: 6e74 6572 6573 7473 2864 6174 612c 206d  nterests(data, m
+00058be0: 6172 6b65 742c 2073 696e 6365 2c20 6c69  arket, since, li
+00058bf0: 6d69 7429 0a0a 2020 2020 6465 6620 6665  mit)..    def fe
+00058c00: 7463 685f 6f70 656e 5f69 6e74 6572 6573  tch_open_interes
+00058c10: 7428 7365 6c66 2c20 7379 6d62 6f6c 3a20  t(self, symbol: 
+00058c20: 7374 722c 2070 6172 616d 733d 7b7d 293a  str, params={}):
+00058c30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00058c40: 2020 2020 2052 6574 7269 6576 6573 2074       Retrieves t
+00058c50: 6865 206f 7065 6e20 696e 7465 7265 7374  he open interest
+00058c60: 206f 6620 6120 6465 7269 7661 7469 7665   of a derivative
+00058c70: 2074 7261 6469 6e67 2070 6169 720a 2020   trading pair.  
+00058c80: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
+00058c90: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
+00058ca0: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
+00058cb0: 7635 2f6d 6172 6b65 742f 6f70 656e 2d69  v5/market/open-i
+00058cc0: 6e74 6572 6573 740a 2020 2020 2020 2020  nterest.        
+00058cd0: 3a70 6172 616d 2073 7472 2073 796d 626f  :param str symbo
+00058ce0: 6c3a 2055 6e69 6669 6564 2043 4358 5420  l: Unified CCXT 
+00058cf0: 6d61 726b 6574 2073 796d 626f 6c0a 2020  market symbol.  
+00058d00: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+00058d10: 7420 7061 7261 6d73 3a20 6578 6368 616e  t params: exchan
+00058d20: 6765 2073 7065 6369 6669 6320 7061 7261  ge specific para
+00058d30: 6d65 7465 7273 0a20 2020 2020 2020 203a  meters.        :
+00058d40: 7061 7261 6d20 7374 727c 4e6f 6e65 2070  param str|None p
+00058d50: 6172 616d 735b 2769 6e74 6572 7661 6c27  arams['interval'
+00058d60: 5d3a 2035 6d2c 2031 356d 2c20 3330 6d2c  ]: 5m, 15m, 30m,
+00058d70: 2031 682c 2034 682c 2031 640a 2020 2020   1h, 4h, 1d.    
+00058d80: 2020 2020 3a70 6172 616d 2073 7472 7c4e      :param str|N
+00058d90: 6f6e 6520 7061 7261 6d73 5b27 6361 7465  one params['cate
+00058da0: 676f 7279 275d 3a20 226c 696e 6561 7222  gory']: "linear"
+00058db0: 206f 7220 2269 6e76 6572 7365 220a 2020   or "inverse".  
+00058dc0: 2020 2020 2020 3a72 6574 7572 6e73 2064        :returns d
+00058dd0: 6963 747d 2061 6e20 6f70 656e 2069 6e74  ict} an open int
+00058de0: 6572 6573 7420 7374 7275 6374 7572 657b  erest structure{
+00058df0: 406c 696e 6b20 6874 7470 733a 2f2f 646f  @link https://do
+00058e00: 6373 2e63 6378 742e 636f 6d2f 232f 3f69  cs.ccxt.com/#/?i
+00058e10: 643d 696e 7465 7265 7374 2d68 6973 746f  d=interest-histo
+00058e20: 7279 2d73 7472 7563 7475 7265 3a0a 2020  ry-structure:.  
+00058e30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00058e40: 2020 7365 6c66 2e6c 6f61 645f 6d61 726b    self.load_mark
+00058e50: 6574 7328 290a 2020 2020 2020 2020 6d61  ets().        ma
+00058e60: 726b 6574 203d 2073 656c 662e 6d61 726b  rket = self.mark
+00058e70: 6574 2873 796d 626f 6c29 0a20 2020 2020  et(symbol).     
+00058e80: 2020 2069 6620 6e6f 7420 6d61 726b 6574     if not market
+00058e90: 5b27 636f 6e74 7261 6374 275d 3a0a 2020  ['contract']:.  
+00058ea0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00058eb0: 4261 6452 6571 7565 7374 2873 656c 662e  BadRequest(self.
+00058ec0: 6964 202b 2027 2066 6574 6368 4f70 656e  id + ' fetchOpen
+00058ed0: 496e 7465 7265 7374 2829 2073 7570 706f  Interest() suppo
+00058ee0: 7274 7320 636f 6e74 7261 6374 206d 6172  rts contract mar
+00058ef0: 6b65 7473 206f 6e6c 7927 290a 2020 2020  kets only').    
+00058f00: 2020 2020 7469 6d65 6672 616d 6520 3d20      timeframe = 
+00058f10: 7365 6c66 2e73 6166 655f 7374 7269 6e67  self.safe_string
+00058f20: 2870 6172 616d 732c 2027 696e 7465 7276  (params, 'interv
+00058f30: 616c 272c 2027 3168 2729 0a20 2020 2020  al', '1h').     
+00058f40: 2020 2069 6e74 6572 7661 6c73 203d 2073     intervals = s
+00058f50: 656c 662e 7361 6665 5f76 616c 7565 2873  elf.safe_value(s
+00058f60: 656c 662e 6f70 7469 6f6e 732c 2027 696e  elf.options, 'in
+00058f70: 7465 7276 616c 7327 290a 2020 2020 2020  tervals').      
+00058f80: 2020 696e 7465 7276 616c 203d 2073 656c    interval = sel
+00058f90: 662e 7361 6665 5f73 7472 696e 6728 696e  f.safe_string(in
+00058fa0: 7465 7276 616c 732c 2074 696d 6566 7261  tervals, timefra
+00058fb0: 6d65 2920 2023 2035 6d69 6e2c 3135 6d69  me)  # 5min,15mi
+00058fc0: 6e2c 3330 6d69 6e2c 3168 2c34 682c 3164  n,30min,1h,4h,1d
+00058fd0: 0a20 2020 2020 2020 2069 6620 696e 7465  .        if inte
+00058fe0: 7276 616c 2069 7320 4e6f 6e65 3a0a 2020  rval is None:.  
+00058ff0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00059000: 4261 6452 6571 7565 7374 2873 656c 662e  BadRequest(self.
+00059010: 6964 202b 2027 2066 6574 6368 4f70 656e  id + ' fetchOpen
+00059020: 496e 7465 7265 7374 2829 2063 616e 6e6f  Interest() canno
+00059030: 7420 7573 6520 7468 6520 2720 2b20 7469  t use the ' + ti
+00059040: 6d65 6672 616d 6520 2b20 2720 7469 6d65  meframe + ' time
+00059050: 6672 616d 6527 290a 2020 2020 2020 2020  frame').        
+00059060: 7375 6254 7970 6520 3d20 276c 696e 6561  subType = 'linea
+00059070: 7227 2069 6620 6d61 726b 6574 5b27 6c69  r' if market['li
+00059080: 6e65 6172 275d 2065 6c73 6520 2769 6e76  near'] else 'inv
+00059090: 6572 7365 270a 2020 2020 2020 2020 6361  erse'.        ca
+000590a0: 7465 676f 7279 203d 2073 656c 662e 7361  tegory = self.sa
+000590b0: 6665 5f73 7472 696e 6728 7061 7261 6d73  fe_string(params
+000590c0: 2c20 2763 6174 6567 6f72 7927 2c20 7375  , 'category', su
+000590d0: 6254 7970 6529 0a20 2020 2020 2020 2072  bType).        r
+000590e0: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
+000590f0: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
+00059100: 206d 6172 6b65 745b 2769 6427 5d2c 0a20   market['id'],. 
+00059110: 2020 2020 2020 2020 2020 2027 696e 7465             'inte
+00059120: 7276 616c 5469 6d65 273a 2069 6e74 6572  rvalTime': inter
+00059130: 7661 6c2c 0a20 2020 2020 2020 2020 2020  val,.           
+00059140: 2027 6361 7465 676f 7279 273a 2063 6174   'category': cat
+00059150: 6567 6f72 792c 0a20 2020 2020 2020 207d  egory,.        }
+00059160: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00059170: 6520 3d20 7365 6c66 2e70 7562 6c69 6347  e = self.publicG
+00059180: 6574 5635 4d61 726b 6574 4f70 656e 496e  etV5MarketOpenIn
+00059190: 7465 7265 7374 2873 656c 662e 6578 7465  terest(self.exte
+000591a0: 6e64 2872 6571 7565 7374 2c20 7061 7261  nd(request, para
+000591b0: 6d73 2929 0a20 2020 2020 2020 2023 0a20  ms)).        #. 
+000591c0: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
+000591d0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+000591e0: 2022 7265 7443 6f64 6522 3a20 302c 0a20   "retCode": 0,. 
+000591f0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00059200: 2022 7265 744d 7367 223a 2022 4f4b 222c   "retMsg": "OK",
+00059210: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00059220: 2020 2022 7265 7375 6c74 223a 207b 0a20     "result": {. 
+00059230: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00059240: 2020 2020 2022 7379 6d62 6f6c 223a 2022       "symbol": "
+00059250: 4254 4355 5344 222c 0a20 2020 2020 2020  BTCUSD",.       
+00059260: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
+00059270: 6361 7465 676f 7279 223a 2022 696e 7665  category": "inve
+00059280: 7273 6522 2c0a 2020 2020 2020 2020 2320  rse",.        # 
+00059290: 2020 2020 2020 2020 2020 2020 226c 6973              "lis
+000592a0: 7422 3a20 5b0a 2020 2020 2020 2020 2320  t": [.        # 
+000592b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000592c0: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+000592d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000592e0: 226f 7065 6e49 6e74 6572 6573 7422 3a20  "openInterest": 
+000592f0: 2234 3631 3133 3433 3834 2e30 3030 3030  "461134384.00000
+00059300: 3030 3022 2c0a 2020 2020 2020 2020 2320  000",.        # 
+00059310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00059320: 2020 2020 2274 696d 6573 7461 6d70 223a      "timestamp":
+00059330: 2022 3136 3639 3537 3134 3030 3030 3022   "1669571400000"
+00059340: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00059350: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00059360: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00059370: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00059380: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00059390: 2020 2020 2020 2020 226f 7065 6e49 6e74          "openInt
+000593a0: 6572 6573 7422 3a20 2234 3631 3133 3432  erest": "4611342
+000593b0: 3932 2e30 3030 3030 3030 3022 2c0a 2020  92.00000000",.  
+000593c0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+000593d0: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
+000593e0: 6573 7461 6d70 223a 2022 3136 3639 3537  estamp": "166957
+000593f0: 3131 3030 3030 3022 0a20 2020 2020 2020  1100000".       
+00059400: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+00059410: 2020 207d 0a20 2020 2020 2020 2023 2020     }.        #  
+00059420: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00059430: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00059440: 2020 2020 226e 6578 7450 6167 6543 7572      "nextPageCur
+00059450: 736f 7222 3a20 2222 0a20 2020 2020 2020  sor": "".       
+00059460: 2023 2020 2020 2020 2020 207d 2c0a 2020   #         },.  
+00059470: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00059480: 2272 6574 4578 7449 6e66 6f22 3a20 7b7d  "retExtInfo": {}
+00059490: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+000594a0: 2020 2020 2274 696d 6522 3a20 3136 3732      "time": 1672
+000594b0: 3035 3335 3438 3537 390a 2020 2020 2020  053548579.      
+000594c0: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
+000594d0: 2020 230a 2020 2020 2020 2020 7265 7375    #.        resu
+000594e0: 6c74 203d 2073 656c 662e 7361 6665 5f76  lt = self.safe_v
+000594f0: 616c 7565 2872 6573 706f 6e73 652c 2027  alue(response, '
+00059500: 7265 7375 6c74 272c 207b 7d29 0a20 2020  result', {}).   
+00059510: 2020 2020 2069 6420 3d20 7365 6c66 2e73       id = self.s
+00059520: 6166 655f 7374 7269 6e67 2872 6573 756c  afe_string(resul
+00059530: 742c 2027 7379 6d62 6f6c 2729 0a20 2020  t, 'symbol').   
+00059540: 2020 2020 206d 6172 6b65 7420 3d20 7365       market = se
+00059550: 6c66 2e73 6166 655f 6d61 726b 6574 2869  lf.safe_market(i
+00059560: 642c 206d 6172 6b65 742c 204e 6f6e 652c  d, market, None,
+00059570: 2027 636f 6e74 7261 6374 2729 0a20 2020   'contract').   
+00059580: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
+00059590: 2e73 6166 655f 7661 6c75 6528 7265 7375  .safe_value(resu
+000595a0: 6c74 2c20 276c 6973 7427 2c20 5b5d 290a  lt, 'list', []).
+000595b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000595c0: 656c 662e 7061 7273 655f 6f70 656e 5f69  elf.parse_open_i
+000595d0: 6e74 6572 6573 7428 6461 7461 5b30 5d2c  nterest(data[0],
+000595e0: 206d 6172 6b65 7429 0a0a 2020 2020 6465   market)..    de
+000595f0: 6620 6665 7463 685f 6f70 656e 5f69 6e74  f fetch_open_int
+00059600: 6572 6573 745f 6869 7374 6f72 7928 7365  erest_history(se
+00059610: 6c66 2c20 7379 6d62 6f6c 3a20 7374 722c  lf, symbol: str,
+00059620: 2074 696d 6566 7261 6d65 3d27 3168 272c   timeframe='1h',
+00059630: 2073 696e 6365 3a20 4f70 7469 6f6e 616c   since: Optional
+00059640: 5b69 6e74 5d20 3d20 4e6f 6e65 2c20 6c69  [int] = None, li
+00059650: 6d69 743a 204f 7074 696f 6e61 6c5b 696e  mit: Optional[in
+00059660: 745d 203d 204e 6f6e 652c 2070 6172 616d  t] = None, param
+00059670: 733d 7b7d 293a 0a20 2020 2020 2020 2022  s={}):.        "
+00059680: 2222 0a20 2020 2020 2020 2047 6574 7320  "".        Gets 
+00059690: 7468 6520 746f 7461 6c20 616d 6f75 6e74  the total amount
+000596a0: 206f 6620 756e 7365 7474 6c65 6420 636f   of unsettled co
+000596b0: 6e74 7261 6374 732e 2049 6e20 6f74 6865  ntracts. In othe
+000596c0: 7220 776f 7264 732c 2074 6865 2074 6f74  r words, the tot
+000596d0: 616c 206e 756d 6265 7220 6f66 2063 6f6e  al number of con
+000596e0: 7472 6163 7473 2068 656c 6420 696e 206f  tracts held in o
+000596f0: 7065 6e20 706f 7369 7469 6f6e 730a 2020  pen positions.  
+00059700: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
+00059710: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
+00059720: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
+00059730: 7635 2f6d 6172 6b65 742f 6f70 656e 2d69  v5/market/open-i
+00059740: 6e74 6572 6573 740a 2020 2020 2020 2020  nterest.        
+00059750: 3a70 6172 616d 2073 7472 2073 796d 626f  :param str symbo
+00059760: 6c3a 2055 6e69 6669 6564 206d 6172 6b65  l: Unified marke
+00059770: 7420 7379 6d62 6f6c 0a20 2020 2020 2020  t symbol.       
+00059780: 203a 7061 7261 6d20 7374 7220 7469 6d65   :param str time
+00059790: 6672 616d 653a 2022 356d 222c 2031 356d  frame: "5m", 15m
+000597a0: 2c20 3330 6d2c 2031 682c 2034 682c 2031  , 30m, 1h, 4h, 1
+000597b0: 640a 2020 2020 2020 2020 3a70 6172 616d  d.        :param
+000597c0: 2069 6e74 2073 696e 6365 3a20 4e6f 7420   int since: Not 
+000597d0: 7573 6564 2062 7920 4279 6269 740a 2020  used by Bybit.  
+000597e0: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
+000597f0: 206c 696d 6974 3a20 5468 6520 6e75 6d62   limit: The numb
+00059800: 6572 206f 6620 6f70 656e 2069 6e74 6572  er of open inter
+00059810: 6573 7420 7374 7275 6374 7572 6573 2074  est structures t
+00059820: 6f20 7265 7475 726e 2e20 4d61 7820 3230  o return. Max 20
+00059830: 302c 2064 6566 6175 6c74 2035 300a 2020  0, default 50.  
+00059840: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+00059850: 7420 7061 7261 6d73 3a20 4578 6368 616e  t params: Exchan
+00059860: 6765 2073 7065 6369 6669 6320 7061 7261  ge specific para
+00059870: 6d65 7465 7273 0a20 2020 2020 2020 203a  meters.        :
+00059880: 7265 7475 726e 733a 2041 6e20 6172 7261  returns: An arra
+00059890: 7920 6f66 206f 7065 6e20 696e 7465 7265  y of open intere
+000598a0: 7374 2073 7472 7563 7475 7265 730a 2020  st structures.  
+000598b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000598c0: 2020 6966 2074 696d 6566 7261 6d65 203d    if timeframe =
+000598d0: 3d20 2731 6d27 3a0a 2020 2020 2020 2020  = '1m':.        
+000598e0: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
+000598f0: 7565 7374 2873 656c 662e 6964 202b 2027  uest(self.id + '
+00059900: 6665 7463 684f 7065 6e49 6e74 6572 6573  fetchOpenInteres
+00059910: 7448 6973 746f 7279 2063 616e 6e6f 7420  tHistory cannot 
+00059920: 7573 6520 7468 6520 316d 2074 696d 6566  use the 1m timef
+00059930: 7261 6d65 2729 0a20 2020 2020 2020 2073  rame').        s
+00059940: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+00059950: 2829 0a20 2020 2020 2020 206d 6172 6b65  ().        marke
+00059960: 7420 3d20 7365 6c66 2e6d 6172 6b65 7428  t = self.market(
+00059970: 7379 6d62 6f6c 290a 2020 2020 2020 2020  symbol).        
+00059980: 6966 206d 6172 6b65 745b 2773 706f 7427  if market['spot'
+00059990: 5d20 6f72 206d 6172 6b65 745b 276f 7074  ] or market['opt
+000599a0: 696f 6e27 5d3a 0a20 2020 2020 2020 2020  ion']:.         
+000599b0: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+000599c0: 6573 7428 7365 6c66 2e69 6420 2b20 2720  est(self.id + ' 
+000599d0: 6665 7463 684f 7065 6e49 6e74 6572 6573  fetchOpenInteres
+000599e0: 7448 6973 746f 7279 2829 2073 796d 626f  tHistory() symbo
+000599f0: 6c20 646f 6573 206e 6f74 2073 7570 706f  l does not suppo
+00059a00: 7274 206d 6172 6b65 7420 2720 2b20 7379  rt market ' + sy
+00059a10: 6d62 6f6c 290a 2020 2020 2020 2020 7265  mbol).        re
+00059a20: 7175 6573 7420 3d20 7b0a 2020 2020 2020  quest = {.      
+00059a30: 2020 2020 2020 2773 796d 626f 6c27 3a20        'symbol': 
+00059a40: 6d61 726b 6574 5b27 6964 275d 2c0a 2020  market['id'],.  
+00059a50: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00059a60: 6966 206c 696d 6974 2069 7320 6e6f 7420  if limit is not 
+00059a70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00059a80: 2020 7265 7175 6573 745b 276c 696d 6974    request['limit
+00059a90: 275d 203d 206c 696d 6974 0a20 2020 2020  '] = limit.     
+00059aa0: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+00059ab0: 6574 6368 5f64 6572 6976 6174 6976 6573  etch_derivatives
+00059ac0: 5f6f 7065 6e5f 696e 7465 7265 7374 5f68  _open_interest_h
+00059ad0: 6973 746f 7279 2873 796d 626f 6c2c 2074  istory(symbol, t
+00059ae0: 696d 6566 7261 6d65 2c20 7369 6e63 652c  imeframe, since,
+00059af0: 206c 696d 6974 2c20 7061 7261 6d73 290a   limit, params).
+00059b00: 0a20 2020 2064 6566 2070 6172 7365 5f6f  .    def parse_o
+00059b10: 7065 6e5f 696e 7465 7265 7374 2873 656c  pen_interest(sel
+00059b20: 662c 2069 6e74 6572 6573 742c 206d 6172  f, interest, mar
+00059b30: 6b65 743d 4e6f 6e65 293a 0a20 2020 2020  ket=None):.     
+00059b40: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+00059b50: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
+00059b60: 2020 2020 2022 6f70 656e 496e 7465 7265       "openIntere
+00059b70: 7374 223a 2036 3437 3537 2e36 3234 3030  st": 64757.62400
+00059b80: 3030 302c 0a20 2020 2020 2020 2023 2020  000,.        #  
+00059b90: 2020 2020 2020 2274 696d 6573 7461 6d70        "timestamp
+00059ba0: 223a 2031 3636 3537 3834 3830 3030 3030  ": 1665784800000
+00059bb0: 2c0a 2020 2020 2020 2020 2320 2020 207d  ,.        #    }
+00059bc0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+00059bd0: 2020 2074 696d 6573 7461 6d70 203d 2073     timestamp = s
+00059be0: 656c 662e 7361 6665 5f69 6e74 6567 6572  elf.safe_integer
+00059bf0: 2869 6e74 6572 6573 742c 2027 7469 6d65  (interest, 'time
+00059c00: 7374 616d 7027 290a 2020 2020 2020 2020  stamp').        
+00059c10: 7661 6c75 6520 3d20 7365 6c66 2e73 6166  value = self.saf
+00059c20: 655f 6e75 6d62 6572 5f32 2869 6e74 6572  e_number_2(inter
+00059c30: 6573 742c 2027 6f70 656e 5f69 6e74 6572  est, 'open_inter
+00059c40: 6573 7427 2c20 276f 7065 6e49 6e74 6572  est', 'openInter
+00059c50: 6573 7427 290a 2020 2020 2020 2020 7265  est').        re
+00059c60: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
+00059c70: 2020 2027 7379 6d62 6f6c 273a 206d 6172     'symbol': mar
+00059c80: 6b65 745b 2773 796d 626f 6c27 5d2c 0a20  ket['symbol'],. 
+00059c90: 2020 2020 2020 2020 2020 2027 6f70 656e             'open
+00059ca0: 496e 7465 7265 7374 416d 6f75 6e74 273a  InterestAmount':
+00059cb0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00059cc0: 2020 2027 6f70 656e 496e 7465 7265 7374     'openInterest
+00059cd0: 5661 6c75 6527 3a20 7661 6c75 652c 0a20  Value': value,. 
+00059ce0: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
+00059cf0: 7374 616d 7027 3a20 7469 6d65 7374 616d  stamp': timestam
+00059d00: 702c 0a20 2020 2020 2020 2020 2020 2027  p,.            '
+00059d10: 6461 7465 7469 6d65 273a 2073 656c 662e  datetime': self.
+00059d20: 6973 6f38 3630 3128 7469 6d65 7374 616d  iso8601(timestam
+00059d30: 7029 2c0a 2020 2020 2020 2020 2020 2020  p),.            
+00059d40: 2769 6e66 6f27 3a20 696e 7465 7265 7374  'info': interest
+00059d50: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+00059d60: 2064 6566 2066 6574 6368 5f62 6f72 726f   def fetch_borro
+00059d70: 775f 7261 7465 2873 656c 662c 2063 6f64  w_rate(self, cod
+00059d80: 653a 2073 7472 2c20 7061 7261 6d73 3d7b  e: str, params={
+00059d90: 7d29 3a0a 2020 2020 2020 2020 2222 220a  }):.        """.
+00059da0: 2020 2020 2020 2020 6665 7463 6820 7468          fetch th
+00059db0: 6520 7261 7465 206f 6620 696e 7465 7265  e rate of intere
+00059dc0: 7374 2074 6f20 626f 7272 6f77 2061 2063  st to borrow a c
+00059dd0: 7572 7265 6e63 7920 666f 7220 6d61 7267  urrency for marg
+00059de0: 696e 2074 7261 6469 6e67 0a20 2020 2020  in trading.     
+00059df0: 2020 2073 6565 2068 7474 7073 3a2f 2f62     see https://b
+00059e00: 7962 6974 2d65 7863 6861 6e67 652e 6769  ybit-exchange.gi
+00059e10: 7468 7562 2e69 6f2f 646f 6373 2f73 706f  thub.io/docs/spo
+00059e20: 742f 7633 2f23 742d 7175 6572 7969 6e74  t/v3/#t-queryint
+00059e30: 6572 6573 7471 756f 7461 0a20 2020 2020  erestquota.     
+00059e40: 2020 203a 7061 7261 6d20 7374 7220 636f     :param str co
+00059e50: 6465 3a20 756e 6966 6965 6420 6375 7272  de: unified curr
+00059e60: 656e 6379 2063 6f64 650a 2020 2020 2020  ency code.      
+00059e70: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
+00059e80: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
+00059e90: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
+00059ea0: 746f 2074 6865 2062 7962 6974 2061 7069  to the bybit api
+00059eb0: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
+00059ec0: 2020 3a72 6574 7572 6e73 2064 6963 743a    :returns dict:
+00059ed0: 2061 2060 626f 7272 6f77 2072 6174 6520   a `borrow rate 
+00059ee0: 7374 7275 6374 7572 6520 3c68 7474 7073  structure <https
+00059ef0: 3a2f 2f64 6f63 732e 6363 7874 2e63 6f6d  ://docs.ccxt.com
+00059f00: 2f23 2f3f 6964 3d62 6f72 726f 772d 7261  /#/?id=borrow-ra
+00059f10: 7465 2d73 7472 7563 7475 7265 3e60 0a20  te-structure>`. 
+00059f20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00059f30: 2020 2073 656c 662e 6c6f 6164 5f6d 6172     self.load_mar
+00059f40: 6b65 7473 2829 0a20 2020 2020 2020 2063  kets().        c
+00059f50: 7572 7265 6e63 7920 3d20 7365 6c66 2e63  urrency = self.c
+00059f60: 7572 7265 6e63 7928 636f 6465 290a 2020  urrency(code).  
+00059f70: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
+00059f80: 7b0a 2020 2020 2020 2020 2020 2020 2763  {.            'c
+00059f90: 6f69 6e27 3a20 6375 7272 656e 6379 5b27  oin': currency['
+00059fa0: 6964 275d 2c0a 2020 2020 2020 2020 7d0a  id'],.        }.
+00059fb0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00059fc0: 203d 2073 656c 662e 7072 6976 6174 6547   = self.privateG
+00059fd0: 6574 5370 6f74 5633 5072 6976 6174 6543  etSpotV3PrivateC
+00059fe0: 726f 7373 4d61 7267 696e 4c6f 616e 496e  rossMarginLoanIn
+00059ff0: 666f 2873 656c 662e 6578 7465 6e64 2872  fo(self.extend(r
+0005a000: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
+0005a010: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005a020: 2020 2023 2020 2020 7b0a 2020 2020 2020     #    {.      
+0005a030: 2020 2320 2020 2020 2020 2020 2272 6574    #         "ret
+0005a040: 436f 6465 223a 2022 3022 2c0a 2020 2020  Code": "0",.    
+0005a050: 2020 2020 2320 2020 2020 2020 2020 2272      #         "r
+0005a060: 6574 4d73 6722 3a20 2273 7563 6365 7373  etMsg": "success
+0005a070: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0005a080: 2020 2020 2022 7265 7375 6c74 223a 207b       "result": {
+0005a090: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005a0a0: 2020 2020 2020 2022 636f 696e 223a 2022         "coin": "
+0005a0b0: 5553 4454 222c 0a20 2020 2020 2020 2023  USDT",.        #
+0005a0c0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+0005a0d0: 7465 7265 7374 5261 7465 223a 2022 302e  terestRate": "0.
+0005a0e0: 3030 3031 3037 3030 3030 3030 222c 0a20  000107000000",. 
+0005a0f0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005a100: 2020 2020 2022 6c6f 616e 4162 6c65 416d       "loanAbleAm
+0005a110: 6f75 6e74 223a 2022 222c 0a20 2020 2020  ount": "",.     
+0005a120: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005a130: 2022 6d61 784c 6f61 6e41 6d6f 756e 7422   "maxLoanAmount"
+0005a140: 3a20 2237 3939 3939 2e39 3939 220a 2020  : "79999.999".  
+0005a150: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005a160: 7d2c 0a20 2020 2020 2020 2023 2020 2020  },.        #    
+0005a170: 2020 2020 2022 7265 7445 7874 496e 666f       "retExtInfo
+0005a180: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
+0005a190: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
+0005a1a0: 223a 2022 3136 3636 3733 3434 3930 3737  ": "166673449077
+0005a1b0: 3822 0a20 2020 2020 2020 2023 2020 2020  8".        #    
+0005a1c0: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
+0005a1d0: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
+0005a1e0: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
+0005a1f0: 6f6e 7365 2c20 2772 6573 756c 7427 2c20  onse, 'result', 
+0005a200: 7b7d 290a 2020 2020 2020 2020 7265 7475  {}).        retu
+0005a210: 726e 2073 656c 662e 7061 7273 655f 626f  rn self.parse_bo
+0005a220: 7272 6f77 5f72 6174 6528 6461 7461 2c20  rrow_rate(data, 
+0005a230: 6375 7272 656e 6379 290a 0a20 2020 2064  currency)..    d
+0005a240: 6566 2070 6172 7365 5f62 6f72 726f 775f  ef parse_borrow_
+0005a250: 7261 7465 2873 656c 662c 2069 6e66 6f2c  rate(self, info,
+0005a260: 2063 7572 7265 6e63 793d 4e6f 6e65 293a   currency=None):
+0005a270: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005a280: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+0005a290: 2020 2023 2020 2020 2020 2020 2022 636f     #         "co
+0005a2a0: 696e 223a 2022 5553 4454 222c 0a20 2020  in": "USDT",.   
+0005a2b0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005a2c0: 696e 7465 7265 7374 5261 7465 223a 2022  interestRate": "
+0005a2d0: 302e 3030 3031 3037 3030 3030 3030 222c  0.000107000000",
+0005a2e0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005a2f0: 2020 2022 6c6f 616e 4162 6c65 416d 6f75     "loanAbleAmou
+0005a300: 6e74 223a 2022 222c 0a20 2020 2020 2020  nt": "",.       
+0005a310: 2023 2020 2020 2020 2020 2022 6d61 784c   #         "maxL
+0005a320: 6f61 6e41 6d6f 756e 7422 3a20 2237 3939  oanAmount": "799
+0005a330: 3939 2e39 3939 220a 2020 2020 2020 2020  99.999".        
+0005a340: 2320 2020 2020 7d0a 2020 2020 2020 2020  #     }.        
+0005a350: 230a 2020 2020 2020 2020 7469 6d65 7374  #.        timest
+0005a360: 616d 7020 3d20 7365 6c66 2e6d 696c 6c69  amp = self.milli
+0005a370: 7365 636f 6e64 7328 290a 2020 2020 2020  seconds().      
+0005a380: 2020 6375 7272 656e 6379 4964 203d 2073    currencyId = s
+0005a390: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005a3a0: 696e 666f 2c20 2763 6f69 6e27 290a 2020  info, 'coin').  
+0005a3b0: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+0005a3c0: 2020 2020 2020 2020 2020 2027 6375 7272             'curr
+0005a3d0: 656e 6379 273a 2073 656c 662e 7361 6665  ency': self.safe
+0005a3e0: 5f63 7572 7265 6e63 795f 636f 6465 2863  _currency_code(c
+0005a3f0: 7572 7265 6e63 7949 642c 2063 7572 7265  urrencyId, curre
+0005a400: 6e63 7929 2c0a 2020 2020 2020 2020 2020  ncy),.          
+0005a410: 2020 2772 6174 6527 3a20 7365 6c66 2e73    'rate': self.s
+0005a420: 6166 655f 6e75 6d62 6572 2869 6e66 6f2c  afe_number(info,
+0005a430: 2027 696e 7465 7265 7374 5261 7465 2729   'interestRate')
+0005a440: 2c0a 2020 2020 2020 2020 2020 2020 2770  ,.            'p
+0005a450: 6572 696f 6427 3a20 3836 3430 3030 3030  eriod': 86400000
+0005a460: 2c20 2023 2044 6169 6c79 0a20 2020 2020  ,  # Daily.     
+0005a470: 2020 2020 2020 2027 7469 6d65 7374 616d         'timestam
+0005a480: 7027 3a20 7469 6d65 7374 616d 702c 0a20  p': timestamp,. 
+0005a490: 2020 2020 2020 2020 2020 2027 6461 7465             'date
+0005a4a0: 7469 6d65 273a 2073 656c 662e 6973 6f38  time': self.iso8
+0005a4b0: 3630 3128 7469 6d65 7374 616d 7029 2c0a  601(timestamp),.
+0005a4c0: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
+0005a4d0: 6f27 3a20 696e 666f 2c0a 2020 2020 2020  o': info,.      
+0005a4e0: 2020 7d0a 0a20 2020 2064 6566 2066 6574    }..    def fet
+0005a4f0: 6368 5f62 6f72 726f 775f 696e 7465 7265  ch_borrow_intere
+0005a500: 7374 2873 656c 662c 2063 6f64 653a 204f  st(self, code: O
+0005a510: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0005a520: 6f6e 652c 2073 796d 626f 6c3a 204f 7074  one, symbol: Opt
+0005a530: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0005a540: 652c 2073 696e 6365 3a20 4f70 7469 6f6e  e, since: Option
+0005a550: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
+0005a560: 6c69 6d69 743a 204f 7074 696f 6e61 6c5b  limit: Optional[
+0005a570: 696e 745d 203d 204e 6f6e 652c 2070 6172  int] = None, par
+0005a580: 616d 733d 7b7d 293a 0a20 2020 2020 2020  ams={}):.       
+0005a590: 2022 2222 0a20 2020 2020 2020 2066 6574   """.        fet
+0005a5a0: 6368 2074 6865 2069 6e74 6572 6573 7420  ch the interest 
+0005a5b0: 6f77 6564 2062 7920 7468 6520 7573 6572  owed by the user
+0005a5c0: 2066 6f72 2062 6f72 726f 7769 6e67 2063   for borrowing c
+0005a5d0: 7572 7265 6e63 7920 666f 7220 6d61 7267  urrency for marg
+0005a5e0: 696e 2074 7261 6469 6e67 0a20 2020 2020  in trading.     
+0005a5f0: 2020 203a 7061 7261 6d20 7374 727c 4e6f     :param str|No
+0005a600: 6e65 2063 6f64 653a 2075 6e69 6669 6564  ne code: unified
+0005a610: 2063 7572 7265 6e63 7920 636f 6465 0a20   currency code. 
+0005a620: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
+0005a630: 727c 4e6f 6e65 2073 796d 626f 6c3a 2075  r|None symbol: u
+0005a640: 6e69 6669 6564 206d 6172 6b65 7420 7379  nified market sy
+0005a650: 6d62 6f6c 2077 6865 6e20 6665 7463 6820  mbol when fetch 
+0005a660: 696e 7465 7265 7374 2069 6e20 6973 6f6c  interest in isol
+0005a670: 6174 6564 206d 6172 6b65 7473 0a20 2020  ated markets.   
+0005a680: 2020 2020 203a 7061 7261 6d20 6e75 6d62       :param numb
+0005a690: 6572 7c4e 6f6e 6520 7369 6e63 653a 2074  er|None since: t
+0005a6a0: 6865 2065 6172 6c69 6573 7420 7469 6d65  he earliest time
+0005a6b0: 2069 6e20 6d73 2074 6f20 6665 7463 6820   in ms to fetch 
+0005a6c0: 626f 7272 726f 7720 696e 7465 7265 7374  borrrow interest
+0005a6d0: 2066 6f72 0a20 2020 2020 2020 203a 7061   for.        :pa
+0005a6e0: 7261 6d20 6e75 6d62 6572 7c4e 6f6e 6520  ram number|None 
+0005a6f0: 6c69 6d69 743a 2074 6865 206d 6178 696d  limit: the maxim
+0005a700: 756d 206e 756d 6265 7220 6f66 2073 7472  um number of str
+0005a710: 7563 7475 7265 7320 746f 2072 6574 7269  uctures to retri
+0005a720: 6576 650a 2020 2020 2020 2020 3a70 6172  eve.        :par
+0005a730: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
+0005a740: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
+0005a750: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
+0005a760: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
+0005a770: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
+0005a780: 7572 6e73 205b 6469 6374 5d3a 2061 206c  urns [dict]: a l
+0005a790: 6973 7420 6f66 2060 626f 7272 6f77 2069  ist of `borrow i
+0005a7a0: 6e74 6572 6573 7420 7374 7275 6374 7572  nterest structur
+0005a7b0: 6573 203c 6874 7470 733a 2f2f 646f 6373  es <https://docs
+0005a7c0: 2e63 6378 742e 636f 6d2f 232f 3f69 643d  .ccxt.com/#/?id=
+0005a7d0: 626f 7272 6f77 2d69 6e74 6572 6573 742d  borrow-interest-
+0005a7e0: 7374 7275 6374 7572 653e 600a 2020 2020  structure>`.    
+0005a7f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0005a800: 7365 6c66 2e6c 6f61 645f 6d61 726b 6574  self.load_market
+0005a810: 7328 290a 2020 2020 2020 2020 7265 7175  s().        requ
+0005a820: 6573 7420 3d20 7b7d 0a20 2020 2020 2020  est = {}.       
+0005a830: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+0005a840: 2e70 7269 7661 7465 4765 7453 706f 7456  .privateGetSpotV
+0005a850: 3350 7269 7661 7465 4372 6f73 734d 6172  3PrivateCrossMar
+0005a860: 6769 6e41 6363 6f75 6e74 2873 656c 662e  ginAccount(self.
+0005a870: 6578 7465 6e64 2872 6571 7565 7374 2c20  extend(request, 
+0005a880: 7061 7261 6d73 2929 0a20 2020 2020 2020  params)).       
+0005a890: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
+0005a8a0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0005a8b0: 2020 2020 2022 7265 745f 636f 6465 223a       "ret_code":
+0005a8c0: 2030 2c0a 2020 2020 2020 2020 2320 2020   0,.        #   
+0005a8d0: 2020 2020 2020 2272 6574 5f6d 7367 223a        "ret_msg":
+0005a8e0: 2022 222c 0a20 2020 2020 2020 2023 2020   "",.        #  
+0005a8f0: 2020 2020 2020 2022 6578 745f 636f 6465         "ext_code
+0005a900: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
+0005a910: 2023 2020 2020 2020 2020 2022 6578 745f   #         "ext_
+0005a920: 696e 666f 223a 206e 756c 6c2c 0a20 2020  info": null,.   
+0005a930: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005a940: 7265 7375 6c74 223a 207b 0a20 2020 2020  result": {.     
+0005a950: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005a960: 2022 7374 6174 7573 223a 2022 3122 2c0a   "status": "1",.
+0005a970: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005a980: 2020 2020 2020 2272 6973 6b52 6174 6522        "riskRate"
+0005a990: 3a20 2230 222c 0a20 2020 2020 2020 2023  : "0",.        #
+0005a9a0: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
+0005a9b0: 6374 4261 6c61 6e63 6553 756d 223a 2022  ctBalanceSum": "
+0005a9c0: 302e 3030 3034 3836 3231 3338 3137 3638  0.00048621381768
+0005a9d0: 3038 3537 222c 0a20 2020 2020 2020 2023  0857",.        #
+0005a9e0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+0005a9f0: 6274 4261 6c61 6e63 6553 756d 223a 2022  btBalanceSum": "
+0005aa00: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
+0005aa10: 2020 2020 2020 2020 2020 226c 6f61 6e41            "loanA
+0005aa20: 6363 6f75 6e74 4c69 7374 223a 205b 0a20  ccountList": [. 
+0005aa30: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005aa40: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0005aa50: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005aa60: 2020 2020 2020 2020 2022 746f 6b65 6e49           "tokenI
+0005aa70: 6422 3a20 2242 5443 222c 0a20 2020 2020  d": "BTC",.     
+0005aa80: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005aa90: 2020 2020 2020 2020 2022 746f 7461 6c22           "total"
+0005aaa0: 3a20 2230 2e30 3030 3438 3632 3122 2c0a  : "0.00048621",.
+0005aab0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005aac0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+0005aad0: 6f63 6b65 6422 3a20 2230 222c 0a20 2020  ocked": "0",.   
+0005aae0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0005aaf0: 2020 2020 2020 2020 2020 2022 6c6f 616e             "loan
+0005ab00: 223a 2022 3022 2c0a 2020 2020 2020 2020  ": "0",.        
+0005ab10: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0005ab20: 2020 2020 2020 2269 6e74 6572 6573 7422        "interest"
+0005ab30: 3a20 2230 222c 0a20 2020 2020 2020 2023  : "0",.        #
+0005ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005ab50: 2020 2020 2022 6672 6565 223a 2022 302e       "free": "0.
+0005ab60: 3030 3034 3836 3231 220a 2020 2020 2020  00048621".      
+0005ab70: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0005ab80: 2020 2020 7d2c 0a20 2020 2020 2020 2023      },.        #
+0005ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005aba0: 202e 2e2e 0a20 2020 2020 2020 2023 2020   ....        #  
+0005abb0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0005abc0: 2020 2020 2023 2020 2020 2020 2020 207d       #         }
+0005abd0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+0005abe0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005abf0: 2020 2064 6174 6120 3d20 7365 6c66 2e73     data = self.s
+0005ac00: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
+0005ac10: 7365 2c20 2772 6573 756c 7427 2c20 7b7d  se, 'result', {}
+0005ac20: 290a 2020 2020 2020 2020 726f 7773 203d  ).        rows =
+0005ac30: 2073 656c 662e 7361 6665 5f76 616c 7565   self.safe_value
+0005ac40: 2864 6174 612c 2027 6c6f 616e 4163 636f  (data, 'loanAcco
+0005ac50: 756e 744c 6973 7427 2c20 5b5d 290a 2020  untList', []).  
+0005ac60: 2020 2020 2020 696e 7465 7265 7374 203d        interest =
+0005ac70: 2073 656c 662e 7061 7273 655f 626f 7272   self.parse_borr
+0005ac80: 6f77 5f69 6e74 6572 6573 7473 2872 6f77  ow_interests(row
+0005ac90: 732c 204e 6f6e 6529 0a20 2020 2020 2020  s, None).       
+0005aca0: 2072 6574 7572 6e20 7365 6c66 2e66 696c   return self.fil
+0005acb0: 7465 725f 6279 5f63 7572 7265 6e63 795f  ter_by_currency_
+0005acc0: 7369 6e63 655f 6c69 6d69 7428 696e 7465  since_limit(inte
+0005acd0: 7265 7374 2c20 636f 6465 2c20 7369 6e63  rest, code, sinc
+0005ace0: 652c 206c 696d 6974 290a 0a20 2020 2064  e, limit)..    d
+0005acf0: 6566 2070 6172 7365 5f62 6f72 726f 775f  ef parse_borrow_
+0005ad00: 696e 7465 7265 7374 2873 656c 662c 2069  interest(self, i
+0005ad10: 6e66 6f2c 206d 6172 6b65 743d 4e6f 6e65  nfo, market=None
+0005ad20: 293a 0a20 2020 2020 2020 2023 0a20 2020  ):.        #.   
+0005ad30: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
+0005ad40: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005ad50: 746f 6b65 6e49 6422 3a20 2242 5443 222c  tokenId": "BTC",
+0005ad60: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005ad70: 2020 2022 746f 7461 6c22 3a20 2230 2e30     "total": "0.0
+0005ad80: 3030 3438 3632 3122 2c0a 2020 2020 2020  0048621",.      
+0005ad90: 2020 2320 2020 2020 2020 2020 226c 6f63    #         "loc
+0005ada0: 6b65 6422 3a20 2230 222c 0a20 2020 2020  ked": "0",.     
+0005adb0: 2020 2023 2020 2020 2020 2020 2022 6c6f     #         "lo
+0005adc0: 616e 223a 2022 3022 2c0a 2020 2020 2020  an": "0",.      
+0005add0: 2020 2320 2020 2020 2020 2020 2269 6e74    #         "int
+0005ade0: 6572 6573 7422 3a20 2230 222c 0a20 2020  erest": "0",.   
+0005adf0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005ae00: 6672 6565 223a 2022 302e 3030 3034 3836  free": "0.000486
+0005ae10: 3231 220a 2020 2020 2020 2020 2320 2020  21".        #   
+0005ae20: 2020 7d2c 0a20 2020 2020 2020 2023 0a20    },.        #. 
+0005ae30: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+0005ae40: 2020 2020 2020 2020 2020 2020 2773 796d              'sym
+0005ae50: 626f 6c27 3a20 4e6f 6e65 2c0a 2020 2020  bol': None,.    
+0005ae60: 2020 2020 2020 2020 276d 6172 6769 6e4d          'marginM
+0005ae70: 6f64 6527 3a20 2763 726f 7373 272c 0a20  ode': 'cross',. 
+0005ae80: 2020 2020 2020 2020 2020 2027 6375 7272             'curr
+0005ae90: 656e 6379 273a 2073 656c 662e 7361 6665  ency': self.safe
+0005aea0: 5f63 7572 7265 6e63 795f 636f 6465 2873  _currency_code(s
+0005aeb0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005aec0: 696e 666f 2c20 2774 6f6b 656e 4964 2729  info, 'tokenId')
+0005aed0: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
+0005aee0: 696e 7465 7265 7374 273a 2073 656c 662e  interest': self.
+0005aef0: 7361 6665 5f6e 756d 6265 7228 696e 666f  safe_number(info
+0005af00: 2c20 2769 6e74 6572 6573 7427 292c 0a20  , 'interest'),. 
+0005af10: 2020 2020 2020 2020 2020 2027 696e 7465             'inte
+0005af20: 7265 7374 5261 7465 273a 204e 6f6e 652c  restRate': None,
+0005af30: 0a20 2020 2020 2020 2020 2020 2027 616d  .            'am
+0005af40: 6f75 6e74 426f 7272 6f77 6564 273a 2073  ountBorrowed': s
+0005af50: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
+0005af60: 696e 666f 2c20 276c 6f61 6e27 292c 0a20  info, 'loan'),. 
+0005af70: 2020 2020 2020 2020 2020 2027 7469 6d65             'time
+0005af80: 7374 616d 7027 3a20 4e6f 6e65 2c0a 2020  stamp': None,.  
+0005af90: 2020 2020 2020 2020 2020 2764 6174 6574            'datet
+0005afa0: 696d 6527 3a20 4e6f 6e65 2c0a 2020 2020  ime': None,.    
+0005afb0: 2020 2020 2020 2020 2769 6e66 6f27 3a20          'info': 
+0005afc0: 696e 666f 2c0a 2020 2020 2020 2020 7d0a  info,.        }.
+0005afd0: 0a20 2020 2064 6566 2074 7261 6e73 6665  .    def transfe
+0005afe0: 7228 7365 6c66 2c20 636f 6465 3a20 7374  r(self, code: st
+0005aff0: 722c 2061 6d6f 756e 742c 2066 726f 6d41  r, amount, fromA
+0005b000: 6363 6f75 6e74 2c20 746f 4163 636f 756e  ccount, toAccoun
+0005b010: 742c 2070 6172 616d 733d 7b7d 293a 0a20  t, params={}):. 
+0005b020: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0005b030: 2020 2074 7261 6e73 6665 7220 6375 7272     transfer curr
+0005b040: 656e 6379 2069 6e74 6572 6e61 6c6c 7920  ency internally 
+0005b050: 6265 7477 6565 6e20 7761 6c6c 6574 7320  between wallets 
+0005b060: 6f6e 2074 6865 2073 616d 6520 6163 636f  on the same acco
+0005b070: 756e 740a 2020 2020 2020 2020 7365 6520  unt.        see 
+0005b080: 6874 7470 733a 2f2f 6279 6269 742d 6578  https://bybit-ex
+0005b090: 6368 616e 6765 2e67 6974 6875 622e 696f  change.github.io
+0005b0a0: 2f64 6f63 732f 6163 636f 756e 745f 6173  /docs/account_as
+0005b0b0: 7365 742f 2374 2d63 7265 6174 6569 6e74  set/#t-createint
+0005b0c0: 6572 6e61 6c74 7261 6e73 6665 720a 2020  ernaltransfer.  
+0005b0d0: 2020 2020 2020 7365 6520 6874 7470 733a        see https:
+0005b0e0: 2f2f 6279 6269 742d 6578 6368 616e 6765  //bybit-exchange
+0005b0f0: 2e67 6974 6875 622e 696f 2f64 6f63 732f  .github.io/docs/
+0005b100: 6163 636f 756e 745f 6173 7365 742f 7633  account_asset/v3
+0005b110: 2f23 742d 6372 6561 7465 696e 7465 726e  /#t-createintern
+0005b120: 616c 7472 616e 7366 6572 0a20 2020 2020  altransfer.     
+0005b130: 2020 203a 7061 7261 6d20 7374 7220 636f     :param str co
+0005b140: 6465 3a20 756e 6966 6965 6420 6375 7272  de: unified curr
+0005b150: 656e 6379 2063 6f64 650a 2020 2020 2020  ency code.      
+0005b160: 2020 3a70 6172 616d 2066 6c6f 6174 2061    :param float a
+0005b170: 6d6f 756e 743a 2061 6d6f 756e 7420 746f  mount: amount to
+0005b180: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
+0005b190: 2020 3a70 6172 616d 2073 7472 2066 726f    :param str fro
+0005b1a0: 6d41 6363 6f75 6e74 3a20 6163 636f 756e  mAccount: accoun
+0005b1b0: 7420 746f 2074 7261 6e73 6665 7220 6672  t to transfer fr
+0005b1c0: 6f6d 0a20 2020 2020 2020 203a 7061 7261  om.        :para
+0005b1d0: 6d20 7374 7220 746f 4163 636f 756e 743a  m str toAccount:
+0005b1e0: 2061 6363 6f75 6e74 2074 6f20 7472 616e   account to tran
+0005b1f0: 7366 6572 2074 6f0a 2020 2020 2020 2020  sfer to.        
+0005b200: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
+0005b210: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
+0005b220: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
+0005b230: 2074 6865 2062 7962 6974 2061 7069 2065   the bybit api e
+0005b240: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
+0005b250: 3a70 6172 616d 2073 7472 2070 6172 616d  :param str param
+0005b260: 735b 2774 7261 6e73 6665 7249 6427 5d3a  s['transferId']:
+0005b270: 2055 5549 442c 2077 6869 6368 2069 7320   UUID, which is 
+0005b280: 756e 6971 7565 2061 6372 6f73 7320 7468  unique across th
+0005b290: 6520 706c 6174 666f 726d 0a20 2020 2020  e platform.     
+0005b2a0: 2020 203a 7265 7475 726e 7320 6469 6374     :returns dict
+0005b2b0: 3a20 6120 6074 7261 6e73 6665 7220 7374  : a `transfer st
+0005b2c0: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
+0005b2d0: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
+0005b2e0: 2f3f 6964 3d74 7261 6e73 6665 722d 7374  /?id=transfer-st
+0005b2f0: 7275 6374 7572 653e 600a 2020 2020 2020  ructure>`.      
+0005b300: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+0005b310: 6c66 2e6c 6f61 645f 6d61 726b 6574 7328  lf.load_markets(
+0005b320: 290a 2020 2020 2020 2020 7472 616e 7366  ).        transf
+0005b330: 6572 4964 203d 2073 656c 662e 7361 6665  erId = self.safe
+0005b340: 5f73 7472 696e 6728 7061 7261 6d73 2c20  _string(params, 
+0005b350: 2774 7261 6e73 6665 7249 6427 2c20 7365  'transferId', se
+0005b360: 6c66 2e75 7569 6428 2929 0a20 2020 2020  lf.uuid()).     
+0005b370: 2020 2061 6363 6f75 6e74 5479 7065 7320     accountTypes 
+0005b380: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
+0005b390: 6528 7365 6c66 2e6f 7074 696f 6e73 2c20  e(self.options, 
+0005b3a0: 2761 6363 6f75 6e74 7342 7954 7970 6527  'accountsByType'
+0005b3b0: 2c20 7b7d 290a 2020 2020 2020 2020 6672  , {}).        fr
+0005b3c0: 6f6d 4964 203d 2073 656c 662e 7361 6665  omId = self.safe
+0005b3d0: 5f73 7472 696e 6728 6163 636f 756e 7454  _string(accountT
+0005b3e0: 7970 6573 2c20 6672 6f6d 4163 636f 756e  ypes, fromAccoun
+0005b3f0: 742c 2066 726f 6d41 6363 6f75 6e74 290a  t, fromAccount).
+0005b400: 2020 2020 2020 2020 746f 4964 203d 2073          toId = s
+0005b410: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005b420: 6163 636f 756e 7454 7970 6573 2c20 746f  accountTypes, to
+0005b430: 4163 636f 756e 742c 2074 6f41 6363 6f75  Account, toAccou
+0005b440: 6e74 290a 2020 2020 2020 2020 6375 7272  nt).        curr
+0005b450: 656e 6379 203d 2073 656c 662e 6375 7272  ency = self.curr
+0005b460: 656e 6379 2863 6f64 6529 0a20 2020 2020  ency(code).     
+0005b470: 2020 2061 6d6f 756e 7454 6f50 7265 6369     amountToPreci
+0005b480: 7369 6f6e 203d 2073 656c 662e 6375 7272  sion = self.curr
+0005b490: 656e 6379 5f74 6f5f 7072 6563 6973 696f  ency_to_precisio
+0005b4a0: 6e28 636f 6465 2c20 616d 6f75 6e74 290a  n(code, amount).
+0005b4b0: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
+0005b4c0: 204e 6f6e 650a 2020 2020 2020 2020 6d65   None.        me
+0005b4d0: 7468 6f64 2c20 7061 7261 6d73 203d 2073  thod, params = s
+0005b4e0: 656c 662e 6861 6e64 6c65 5f6f 7074 696f  elf.handle_optio
+0005b4f0: 6e5f 616e 645f 7061 7261 6d73 2870 6172  n_and_params(par
+0005b500: 616d 732c 2027 7472 616e 7366 6572 272c  ams, 'transfer',
+0005b510: 2027 6d65 7468 6f64 272c 2027 7072 6976   'method', 'priv
+0005b520: 6174 6550 6f73 7441 7373 6574 5631 5072  atePostAssetV1Pr
+0005b530: 6976 6174 6554 7261 6e73 6665 7227 2920  ivateTransfer') 
+0005b540: 2023 2076 3120 7072 6566 6572 7265 6420   # v1 preferred 
+0005b550: 6174 6d2c 2062 6563 6175 7365 2069 7420  atm, because it 
+0005b560: 7375 7070 6f72 7473 2066 756e 6469 6e67  supports funding
+0005b570: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0005b580: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0005b590: 6966 206d 6574 686f 6420 3d3d 2027 7072  if method == 'pr
+0005b5a0: 6976 6174 6550 6f73 7441 7373 6574 5633  ivatePostAssetV3
+0005b5b0: 5072 6976 6174 6554 7261 6e73 6665 7249  PrivateTransferI
+0005b5c0: 6e74 6572 5472 616e 7366 6572 2720 6f72  nterTransfer' or
+0005b5d0: 206d 6574 686f 6420 3d3d 2027 7072 6976   method == 'priv
+0005b5e0: 6174 6550 6f73 7456 3541 7373 6574 5472  atePostV5AssetTr
+0005b5f0: 616e 7366 6572 496e 7465 7254 7261 6e73  ansferInterTrans
+0005b600: 6665 7227 3a0a 2020 2020 2020 2020 2020  fer':.          
+0005b610: 2020 7265 7175 6573 7420 3d20 7b0a 2020    request = {.  
+0005b620: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0005b630: 7261 6e73 6665 7249 6427 3a20 7472 616e  ransferId': tran
+0005b640: 7366 6572 4964 2c0a 2020 2020 2020 2020  sferId,.        
+0005b650: 2020 2020 2020 2020 2766 726f 6d41 6363          'fromAcc
+0005b660: 6f75 6e74 5479 7065 273a 2066 726f 6d49  ountType': fromI
+0005b670: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0005b680: 2020 2027 746f 4163 636f 756e 7454 7970     'toAccountTyp
+0005b690: 6527 3a20 746f 4964 2c0a 2020 2020 2020  e': toId,.      
+0005b6a0: 2020 2020 2020 2020 2020 2763 6f69 6e27            'coin'
+0005b6b0: 3a20 6375 7272 656e 6379 5b27 6964 275d  : currency['id']
+0005b6c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0005b6d0: 2020 2761 6d6f 756e 7427 3a20 616d 6f75    'amount': amou
+0005b6e0: 6e74 546f 5072 6563 6973 696f 6e2c 0a20  ntToPrecision,. 
+0005b6f0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+0005b700: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0005b710: 2020 2020 2020 2072 6571 7565 7374 203d         request =
+0005b720: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0005b730: 2020 2027 7472 616e 7366 6572 5f69 6427     'transfer_id'
+0005b740: 3a20 7472 616e 7366 6572 4964 2c0a 2020  : transferId,.  
+0005b750: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+0005b760: 726f 6d5f 6163 636f 756e 745f 7479 7065  rom_account_type
+0005b770: 273a 2066 726f 6d49 642c 0a20 2020 2020  ': fromId,.     
+0005b780: 2020 2020 2020 2020 2020 2027 746f 5f61             'to_a
+0005b790: 6363 6f75 6e74 5f74 7970 6527 3a20 746f  ccount_type': to
+0005b7a0: 4964 2c0a 2020 2020 2020 2020 2020 2020  Id,.            
+0005b7b0: 2020 2020 2763 6f69 6e27 3a20 6375 7272      'coin': curr
+0005b7c0: 656e 6379 5b27 6964 275d 2c0a 2020 2020  ency['id'],.    
+0005b7d0: 2020 2020 2020 2020 2020 2020 2761 6d6f              'amo
+0005b7e0: 756e 7427 3a20 616d 6f75 6e74 546f 5072  unt': amountToPr
+0005b7f0: 6563 6973 696f 6e2c 0a20 2020 2020 2020  ecision,.       
+0005b800: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+0005b810: 6573 706f 6e73 6520 3d20 6765 7461 7474  esponse = getatt
+0005b820: 7228 7365 6c66 2c20 6d65 7468 6f64 2928  r(self, method)(
+0005b830: 7365 6c66 2e65 7874 656e 6428 7265 7175  self.extend(requ
+0005b840: 6573 742c 2070 6172 616d 7329 290a 2020  est, params)).  
+0005b850: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+0005b860: 2320 7b0a 2020 2020 2020 2020 2320 2020  # {.        #   
+0005b870: 2020 2272 6574 436f 6465 223a 2030 2c0a    "retCode": 0,.
+0005b880: 2020 2020 2020 2020 2320 2020 2020 2272          #     "r
+0005b890: 6574 4d73 6722 3a20 2273 7563 6365 7373  etMsg": "success
+0005b8a0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0005b8b0: 2022 7265 7375 6c74 223a 207b 0a20 2020   "result": {.   
+0005b8c0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005b8d0: 7472 616e 7366 6572 4964 223a 2022 3432  transferId": "42
+0005b8e0: 3434 6166 3434 2d66 3362 302d 3463 6636  44af44-f3b0-4cf6
+0005b8f0: 2d61 3734 332d 6235 3635 3630 6539 3837  -a743-b56560e987
+0005b900: 6263 2220 2023 2074 7261 6e73 6665 725f  bc"  # transfer_
+0005b910: 6964 2069 6e20 7631 0a20 2020 2020 2020  id in v1.       
+0005b920: 2023 2020 2020 207d 2c0a 2020 2020 2020   #     },.      
+0005b930: 2020 2320 2020 2020 2272 6574 4578 7449    #     "retExtI
+0005b940: 6e66 6f22 3a20 7b7d 2c0a 2020 2020 2020  nfo": {},.      
+0005b950: 2020 2320 2020 2020 2274 696d 6522 3a20    #     "time": 
+0005b960: 3136 3636 3837 3538 3537 3230 350a 2020  1666875857205.  
+0005b970: 2020 2020 2020 2320 7d0a 2020 2020 2020        # }.      
+0005b980: 2020 230a 2020 2020 2020 2020 7469 6d65    #.        time
+0005b990: 7374 616d 7020 3d20 7365 6c66 2e73 6166  stamp = self.saf
+0005b9a0: 655f 696e 7465 6765 725f 3228 7265 7370  e_integer_2(resp
+0005b9b0: 6f6e 7365 2c20 2774 696d 6527 2c20 2774  onse, 'time', 't
+0005b9c0: 696d 655f 6e6f 7727 290a 2020 2020 2020  ime_now').      
+0005b9d0: 2020 7472 616e 7366 6572 203d 2073 656c    transfer = sel
+0005b9e0: 662e 7361 6665 5f76 616c 7565 2872 6573  f.safe_value(res
+0005b9f0: 706f 6e73 652c 2027 7265 7375 6c74 272c  ponse, 'result',
+0005ba00: 207b 7d29 0a20 2020 2020 2020 2073 7461   {}).        sta
+0005ba10: 7475 7352 6177 203d 2073 656c 662e 7361  tusRaw = self.sa
+0005ba20: 6665 5f73 7472 696e 675f 6e28 7265 7370  fe_string_n(resp
+0005ba30: 6f6e 7365 2c20 5b27 7265 7443 6f64 6527  onse, ['retCode'
+0005ba40: 2c20 2772 6574 4d73 6727 2c20 2772 6574  , 'retMsg', 'ret
+0005ba50: 5f63 6f64 6527 2c20 2772 6574 5f6d 7367  _code', 'ret_msg
+0005ba60: 275d 290a 2020 2020 2020 2020 7374 6174  ']).        stat
+0005ba70: 7573 203d 2073 656c 662e 7061 7273 655f  us = self.parse_
+0005ba80: 7472 616e 7366 6572 5f73 7461 7475 7328  transfer_status(
+0005ba90: 7374 6174 7573 5261 7729 0a20 2020 2020  statusRaw).     
+0005baa0: 2020 2072 6574 7572 6e20 7365 6c66 2e65     return self.e
+0005bab0: 7874 656e 6428 7365 6c66 2e70 6172 7365  xtend(self.parse
+0005bac0: 5f74 7261 6e73 6665 7228 7472 616e 7366  _transfer(transf
+0005bad0: 6572 2c20 6375 7272 656e 6379 292c 207b  er, currency), {
+0005bae0: 0a20 2020 2020 2020 2020 2020 2027 7469  .            'ti
+0005baf0: 6d65 7374 616d 7027 3a20 7469 6d65 7374  mestamp': timest
+0005bb00: 616d 702c 0a20 2020 2020 2020 2020 2020  amp,.           
+0005bb10: 2027 6461 7465 7469 6d65 273a 2073 656c   'datetime': sel
+0005bb20: 662e 6973 6f38 3630 3128 7469 6d65 7374  f.iso8601(timest
+0005bb30: 616d 7029 2c0a 2020 2020 2020 2020 2020  amp),.          
+0005bb40: 2020 2761 6d6f 756e 7427 3a20 7365 6c66    'amount': self
+0005bb50: 2e70 6172 7365 5f6e 756d 6265 7228 616d  .parse_number(am
+0005bb60: 6f75 6e74 546f 5072 6563 6973 696f 6e29  ountToPrecision)
+0005bb70: 2c0a 2020 2020 2020 2020 2020 2020 2766  ,.            'f
+0005bb80: 726f 6d41 6363 6f75 6e74 273a 2066 726f  romAccount': fro
+0005bb90: 6d41 6363 6f75 6e74 2c0a 2020 2020 2020  mAccount,.      
+0005bba0: 2020 2020 2020 2774 6f41 6363 6f75 6e74        'toAccount
+0005bbb0: 273a 2074 6f41 6363 6f75 6e74 2c0a 2020  ': toAccount,.  
+0005bbc0: 2020 2020 2020 2020 2020 2773 7461 7475            'statu
+0005bbd0: 7327 3a20 7374 6174 7573 2c0a 2020 2020  s': status,.    
+0005bbe0: 2020 2020 7d29 0a0a 2020 2020 6465 6620      })..    def 
+0005bbf0: 6665 7463 685f 7472 616e 7366 6572 7328  fetch_transfers(
+0005bc00: 7365 6c66 2c20 636f 6465 3a20 4f70 7469  self, code: Opti
+0005bc10: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0005bc20: 2c20 7369 6e63 653a 204f 7074 696f 6e61  , since: Optiona
+0005bc30: 6c5b 696e 745d 203d 204e 6f6e 652c 206c  l[int] = None, l
+0005bc40: 696d 6974 3a20 4f70 7469 6f6e 616c 5b69  imit: Optional[i
+0005bc50: 6e74 5d20 3d20 4e6f 6e65 2c20 7061 7261  nt] = None, para
+0005bc60: 6d73 3d7b 7d29 3a0a 2020 2020 2020 2020  ms={}):.        
+0005bc70: 2222 220a 2020 2020 2020 2020 6665 7463  """.        fetc
+0005bc80: 6820 6120 6869 7374 6f72 7920 6f66 2069  h a history of i
+0005bc90: 6e74 6572 6e61 6c20 7472 616e 7366 6572  nternal transfer
+0005bca0: 7320 6d61 6465 206f 6e20 616e 2061 6363  s made on an acc
+0005bcb0: 6f75 6e74 0a20 2020 2020 2020 2073 6565  ount.        see
+0005bcc0: 2068 7474 7073 3a2f 2f62 7962 6974 2d65   https://bybit-e
+0005bcd0: 7863 6861 6e67 652e 6769 7468 7562 2e69  xchange.github.i
+0005bce0: 6f2f 646f 6373 2f76 352f 6173 7365 742f  o/docs/v5/asset/
+0005bcf0: 696e 7465 722d 7472 616e 7366 6572 2d6c  inter-transfer-l
+0005bd00: 6973 740a 2020 2020 2020 2020 3a70 6172  ist.        :par
+0005bd10: 616d 2073 7472 7c4e 6f6e 6520 636f 6465  am str|None code
+0005bd20: 3a20 756e 6966 6965 6420 6375 7272 656e  : unified curren
+0005bd30: 6379 2063 6f64 6520 6f66 2074 6865 2063  cy code of the c
+0005bd40: 7572 7265 6e63 7920 7472 616e 7366 6572  urrency transfer
+0005bd50: 7265 640a 2020 2020 2020 2020 3a70 6172  red.        :par
+0005bd60: 616d 2069 6e74 7c4e 6f6e 6520 7369 6e63  am int|None sinc
+0005bd70: 653a 2074 6865 2065 6172 6c69 6573 7420  e: the earliest 
+0005bd80: 7469 6d65 2069 6e20 6d73 2074 6f20 6665  time in ms to fe
+0005bd90: 7463 6820 7472 616e 7366 6572 7320 666f  tch transfers fo
+0005bda0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+0005bdb0: 2069 6e74 7c4e 6f6e 6520 6c69 6d69 743a   int|None limit:
+0005bdc0: 2074 6865 206d 6178 696d 756d 206e 756d   the maximum num
+0005bdd0: 6265 7220 6f66 2020 7472 616e 7366 6572  ber of  transfer
+0005bde0: 7320 7374 7275 6374 7572 6573 2074 6f20  s structures to 
+0005bdf0: 7265 7472 6965 7665 0a20 2020 2020 2020  retrieve.       
+0005be00: 203a 7061 7261 6d20 6469 6374 2070 6172   :param dict par
+0005be10: 616d 733a 2065 7874 7261 2070 6172 616d  ams: extra param
+0005be20: 6574 6572 7320 7370 6563 6966 6963 2074  eters specific t
+0005be30: 6f20 7468 6520 6279 6269 7420 6170 6920  o the bybit api 
+0005be40: 656e 6470 6f69 6e74 0a20 2020 2020 2020  endpoint.       
+0005be50: 203a 7265 7475 726e 7320 5b64 6963 745d   :returns [dict]
+0005be60: 3a20 6120 6c69 7374 206f 6620 6074 7261  : a list of `tra
+0005be70: 6e73 6665 7220 7374 7275 6374 7572 6573  nsfer structures
+0005be80: 203c 6874 7470 733a 2f2f 646f 6373 2e63   <https://docs.c
+0005be90: 6378 742e 636f 6d2f 232f 3f69 643d 7472  cxt.com/#/?id=tr
+0005bea0: 616e 7366 6572 2d73 7472 7563 7475 7265  ansfer-structure
+0005beb0: 3e60 0a20 2020 2020 2020 2022 2222 0a20  >`.        """. 
+0005bec0: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+0005bed0: 5f6d 6172 6b65 7473 2829 0a20 2020 2020  _markets().     
+0005bee0: 2020 2063 7572 7265 6e63 7920 3d20 4e6f     currency = No
+0005bef0: 6e65 0a20 2020 2020 2020 2072 6571 7565  ne.        reque
+0005bf00: 7374 203d 207b 7d0a 2020 2020 2020 2020  st = {}.        
+0005bf10: 6966 2063 6f64 6520 6973 206e 6f74 204e  if code is not N
+0005bf20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0005bf30: 2063 7572 7265 6e63 7920 3d20 7365 6c66   currency = self
+0005bf40: 2e73 6166 655f 6375 7272 656e 6379 5f63  .safe_currency_c
+0005bf50: 6f64 6528 636f 6465 290a 2020 2020 2020  ode(code).      
+0005bf60: 2020 2020 2020 7265 7175 6573 745b 2763        request['c
+0005bf70: 6f69 6e27 5d20 3d20 6375 7272 656e 6379  oin'] = currency
+0005bf80: 0a20 2020 2020 2020 2069 6620 7369 6e63  .        if sinc
+0005bf90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0005bfa0: 2020 2020 2020 2020 2020 2072 6571 7565             reque
+0005bfb0: 7374 5b27 7374 6172 7454 696d 6527 5d20  st['startTime'] 
+0005bfc0: 3d20 7369 6e63 650a 2020 2020 2020 2020  = since.        
+0005bfd0: 6966 206c 696d 6974 2069 7320 6e6f 7420  if limit is not 
+0005bfe0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0005bff0: 2020 7265 7175 6573 745b 276c 696d 6974    request['limit
+0005c000: 275d 203d 206c 696d 6974 0a20 2020 2020  '] = limit.     
+0005c010: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+0005c020: 6c66 2e70 7269 7661 7465 4765 7456 3541  lf.privateGetV5A
+0005c030: 7373 6574 5472 616e 7366 6572 5175 6572  ssetTransferQuer
+0005c040: 7949 6e74 6572 5472 616e 7366 6572 4c69  yInterTransferLi
+0005c050: 7374 2873 656c 662e 6578 7465 6e64 2872  st(self.extend(r
+0005c060: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
+0005c070: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005c080: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+0005c090: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+0005c0a0: 7443 6f64 6522 3a20 302c 0a20 2020 2020  tCode": 0,.     
+0005c0b0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+0005c0c0: 744d 7367 223a 2022 7375 6363 6573 7322  tMsg": "success"
+0005c0d0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005c0e0: 2020 2020 2272 6573 756c 7422 3a20 7b0a      "result": {.
+0005c0f0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005c100: 2020 2020 2020 226c 6973 7422 3a20 5b0a        "list": [.
+0005c110: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005c120: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+0005c130: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005c140: 2020 2020 2020 2020 2020 2274 7261 6e73            "trans
+0005c150: 6665 7249 6422 3a20 2273 656c 6654 7261  ferId": "selfTra
+0005c160: 6e73 6665 725f 6131 3039 3163 6337 2d39  nsfer_a1091cc7-9
+0005c170: 3336 342d 3462 3734 2d38 6465 312d 3138  364-4b74-8de1-18
+0005c180: 6630 3263 3666 3264 3563 222c 0a20 2020  f02c6f2d5c",.   
+0005c190: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0005c1a0: 2020 2020 2020 2020 2020 2022 636f 696e             "coin
+0005c1b0: 223a 2022 5553 4454 222c 0a20 2020 2020  ": "USDT",.     
+0005c1c0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005c1d0: 2020 2020 2020 2020 2022 616d 6f75 6e74           "amount
+0005c1e0: 223a 2022 3530 3030 222c 0a20 2020 2020  ": "5000",.     
+0005c1f0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005c200: 2020 2020 2020 2020 2022 6672 6f6d 4163           "fromAc
+0005c210: 636f 756e 7454 7970 6522 3a20 2253 504f  countType": "SPO
+0005c220: 5422 2c0a 2020 2020 2020 2020 2320 2020  T",.        #   
+0005c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005c240: 2020 2274 6f41 6363 6f75 6e74 5479 7065    "toAccountType
+0005c250: 223a 2022 554e 4946 4945 4422 2c0a 2020  ": "UNIFIED",.  
+0005c260: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005c270: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
+0005c280: 6573 7461 6d70 223a 2022 3136 3637 3238  estamp": "166728
+0005c290: 3332 3633 3030 3022 2c0a 2020 2020 2020  3263000",.      
+0005c2a0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0005c2b0: 2020 2020 2020 2020 2273 7461 7475 7322          "status"
+0005c2c0: 3a20 2253 5543 4345 5353 220a 2020 2020  : "SUCCESS".    
+0005c2d0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005c2e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0005c2f0: 2320 2020 2020 2020 2020 2020 2020 5d2c  #             ],
+0005c300: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005c310: 2020 2020 2020 2022 6e65 7874 5061 6765         "nextPage
+0005c320: 4375 7273 6f72 223a 2022 6579 4a74 6157  Cursor": "eyJtaW
+0005c330: 354a 5243 4936 4d54 4d31 4f44 5132 4f43  5JRCI6MTM1ODQ2OC
+0005c340: 7769 6257 4634 5355 5169 4f6a 457a 4e54  wibWF4SUQiOjEzNT
+0005c350: 6730 4e6a 6839 220a 2020 2020 2020 2020  g0Njh9".        
+0005c360: 2320 2020 2020 2020 2020 7d2c 0a20 2020  #         },.   
+0005c370: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005c380: 7265 7445 7874 496e 666f 223a 207b 7d2c  retExtInfo": {},
+0005c390: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005c3a0: 2020 2022 7469 6d65 223a 2031 3637 3039     "time": 16709
+0005c3b0: 3838 3237 3136 3737 0a20 2020 2020 2020  88271677.       
+0005c3c0: 2023 2020 2020 207d 0a20 2020 2020 2020   #     }.       
+0005c3d0: 2023 0a20 2020 2020 2020 2064 6174 6120   #.        data 
+0005c3e0: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
+0005c3f0: 6528 7265 7370 6f6e 7365 2c20 2772 6573  e(response, 'res
+0005c400: 756c 7427 2c20 7b7d 290a 2020 2020 2020  ult', {}).      
+0005c410: 2020 7472 616e 7366 6572 7320 3d20 7365    transfers = se
+0005c420: 6c66 2e73 6166 655f 7661 6c75 6528 6461  lf.safe_value(da
+0005c430: 7461 2c20 276c 6973 7427 2c20 5b5d 290a  ta, 'list', []).
+0005c440: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0005c450: 656c 662e 7061 7273 655f 7472 616e 7366  elf.parse_transf
+0005c460: 6572 7328 7472 616e 7366 6572 732c 2063  ers(transfers, c
+0005c470: 7572 7265 6e63 792c 2073 696e 6365 2c20  urrency, since, 
+0005c480: 6c69 6d69 7429 0a0a 2020 2020 6465 6620  limit)..    def 
+0005c490: 626f 7272 6f77 5f6d 6172 6769 6e28 7365  borrow_margin(se
+0005c4a0: 6c66 2c20 636f 6465 3a20 7374 722c 2061  lf, code: str, a
+0005c4b0: 6d6f 756e 742c 2073 796d 626f 6c3a 204f  mount, symbol: O
+0005c4c0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0005c4d0: 6f6e 652c 2070 6172 616d 733d 7b7d 293a  one, params={}):
+0005c4e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0005c4f0: 2020 2020 2063 7265 6174 6520 6120 6c6f       create a lo
+0005c500: 616e 2074 6f20 626f 7272 6f77 206d 6172  an to borrow mar
+0005c510: 6769 6e0a 2020 2020 2020 2020 7365 6520  gin.        see 
+0005c520: 6874 7470 733a 2f2f 6279 6269 742d 6578  https://bybit-ex
+0005c530: 6368 616e 6765 2e67 6974 6875 622e 696f  change.github.io
+0005c540: 2f64 6f63 732f 7370 6f74 2f76 332f 2374  /docs/spot/v3/#t
+0005c550: 2d62 6f72 726f 776d 6172 6769 6e6c 6f61  -borrowmarginloa
+0005c560: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
+0005c570: 2073 7472 2063 6f64 653a 2075 6e69 6669   str code: unifi
+0005c580: 6564 2063 7572 7265 6e63 7920 636f 6465  ed currency code
+0005c590: 206f 6620 7468 6520 6375 7272 656e 6379   of the currency
+0005c5a0: 2074 6f20 626f 7272 6f77 0a20 2020 2020   to borrow.     
+0005c5b0: 2020 203a 7061 7261 6d20 666c 6f61 7420     :param float 
+0005c5c0: 616d 6f75 6e74 3a20 7468 6520 616d 6f75  amount: the amou
+0005c5d0: 6e74 2074 6f20 626f 7272 6f77 0a20 2020  nt to borrow.   
+0005c5e0: 2020 2020 203a 7061 7261 6d20 7374 727c       :param str|
+0005c5f0: 4e6f 6e65 2073 796d 626f 6c3a 206e 6f74  None symbol: not
+0005c600: 2075 7365 6420 6279 2062 7962 6974 2e62   used by bybit.b
+0005c610: 6f72 726f 774d 6172 6769 6e28 290a 2020  orrowMargin().  
+0005c620: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+0005c630: 7420 7061 7261 6d73 3a20 6578 7472 6120  t params: extra 
+0005c640: 7061 7261 6d65 7465 7273 2073 7065 6369  parameters speci
+0005c650: 6669 6320 746f 2074 6865 2062 7962 6974  fic to the bybit
+0005c660: 2061 7069 2065 6e64 706f 696e 740a 2020   api endpoint.  
+0005c670: 2020 2020 2020 3a72 6574 7572 6e73 2064        :returns d
+0005c680: 6963 743a 2061 2060 6d61 7267 696e 206c  ict: a `margin l
+0005c690: 6f61 6e20 7374 7275 6374 7572 6520 3c68  oan structure <h
+0005c6a0: 7474 7073 3a2f 2f64 6f63 732e 6363 7874  ttps://docs.ccxt
+0005c6b0: 2e63 6f6d 2f23 2f3f 6964 3d6d 6172 6769  .com/#/?id=margi
+0005c6c0: 6e2d 6c6f 616e 2d73 7472 7563 7475 7265  n-loan-structure
+0005c6d0: 3e60 0a20 2020 2020 2020 2022 2222 0a20  >`.        """. 
+0005c6e0: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+0005c6f0: 5f6d 6172 6b65 7473 2829 0a20 2020 2020  _markets().     
+0005c700: 2020 2063 7572 7265 6e63 7920 3d20 7365     currency = se
+0005c710: 6c66 2e63 7572 7265 6e63 7928 636f 6465  lf.currency(code
+0005c720: 290a 2020 2020 2020 2020 6d61 7267 696e  ).        margin
+0005c730: 4d6f 6465 2c20 7175 6572 7920 3d20 7365  Mode, query = se
+0005c740: 6c66 2e68 616e 646c 655f 6d61 7267 696e  lf.handle_margin
+0005c750: 5f6d 6f64 655f 616e 645f 7061 7261 6d73  _mode_and_params
+0005c760: 2827 626f 7272 6f77 4d61 7267 696e 272c  ('borrowMargin',
+0005c770: 2070 6172 616d 7329 0a20 2020 2020 2020   params).       
+0005c780: 2069 6620 6d61 7267 696e 4d6f 6465 203d   if marginMode =
+0005c790: 3d20 2769 736f 6c61 7465 6427 3a0a 2020  = 'isolated':.  
+0005c7a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0005c7b0: 4e6f 7453 7570 706f 7274 6564 2873 656c  NotSupported(sel
+0005c7c0: 662e 6964 202b 2027 2062 6f72 726f 774d  f.id + ' borrowM
+0005c7d0: 6172 6769 6e28 2920 6361 6e6e 6f74 2075  argin() cannot u
+0005c7e0: 7365 2069 736f 6c61 7465 6420 6d61 7267  se isolated marg
+0005c7f0: 696e 2729 0a20 2020 2020 2020 2072 6571  in').        req
+0005c800: 7565 7374 203d 207b 0a20 2020 2020 2020  uest = {.       
+0005c810: 2020 2020 2027 636f 696e 273a 2063 7572       'coin': cur
+0005c820: 7265 6e63 795b 2769 6427 5d2c 0a20 2020  rency['id'],.   
+0005c830: 2020 2020 2020 2020 2027 7174 7927 3a20           'qty': 
+0005c840: 7365 6c66 2e63 7572 7265 6e63 795f 746f  self.currency_to
+0005c850: 5f70 7265 6369 7369 6f6e 2863 6f64 652c  _precision(code,
+0005c860: 2061 6d6f 756e 7429 2c0a 2020 2020 2020   amount),.      
+0005c870: 2020 7d0a 2020 2020 2020 2020 7265 7370    }.        resp
+0005c880: 6f6e 7365 203d 2073 656c 662e 7072 6976  onse = self.priv
+0005c890: 6174 6550 6f73 7453 706f 7456 3350 7269  atePostSpotV3Pri
+0005c8a0: 7661 7465 4372 6f73 734d 6172 6769 6e4c  vateCrossMarginL
+0005c8b0: 6f61 6e28 7365 6c66 2e65 7874 656e 6428  oan(self.extend(
+0005c8c0: 7265 7175 6573 742c 2071 7565 7279 2929  request, query))
+0005c8d0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005c8e0: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+0005c8f0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+0005c900: 7443 6f64 6522 3a20 302c 0a20 2020 2020  tCode": 0,.     
+0005c910: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+0005c920: 744d 7367 223a 2022 7375 6363 6573 7322  tMsg": "success"
+0005c930: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005c940: 2020 2020 2272 6573 756c 7422 3a20 7b0a      "result": {.
+0005c950: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005c960: 2020 2020 2020 2274 7261 6e73 6163 7449        "transactI
+0005c970: 6422 3a20 2231 3431 3433 220a 2020 2020  d": "14143".    
+0005c980: 2020 2020 2320 2020 2020 2020 2020 7d2c      #         },
+0005c990: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005c9a0: 2020 2022 7265 7445 7874 496e 666f 223a     "retExtInfo":
+0005c9b0: 206e 756c 6c2c 0a20 2020 2020 2020 2023   null,.        #
+0005c9c0: 2020 2020 2020 2020 2022 7469 6d65 223a           "time":
+0005c9d0: 2031 3636 3236 3137 3834 3839 3730 0a20   1662617848970. 
+0005c9e0: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
+0005c9f0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0005ca00: 2072 6573 756c 7420 3d20 7365 6c66 2e73   result = self.s
+0005ca10: 6166 655f 7661 6c75 6528 7265 7370 6f6e  afe_value(respon
+0005ca20: 7365 2c20 2772 6573 756c 7427 2c20 7b7d  se, 'result', {}
+0005ca30: 290a 2020 2020 2020 2020 7472 616e 7361  ).        transa
+0005ca40: 6374 696f 6e20 3d20 7365 6c66 2e70 6172  ction = self.par
+0005ca50: 7365 5f6d 6172 6769 6e5f 6c6f 616e 2872  se_margin_loan(r
+0005ca60: 6573 756c 742c 2063 7572 7265 6e63 7929  esult, currency)
+0005ca70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0005ca80: 7365 6c66 2e65 7874 656e 6428 7472 616e  self.extend(tran
+0005ca90: 7361 6374 696f 6e2c 207b 0a20 2020 2020  saction, {.     
+0005caa0: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
+0005cab0: 2073 796d 626f 6c2c 0a20 2020 2020 2020   symbol,.       
+0005cac0: 2020 2020 2027 616d 6f75 6e74 273a 2061       'amount': a
+0005cad0: 6d6f 756e 742c 0a20 2020 2020 2020 207d  mount,.        }
+0005cae0: 290a 0a20 2020 2064 6566 2072 6570 6179  )..    def repay
+0005caf0: 5f6d 6172 6769 6e28 7365 6c66 2c20 636f  _margin(self, co
+0005cb00: 6465 3a20 7374 722c 2061 6d6f 756e 742c  de: str, amount,
+0005cb10: 2073 796d 626f 6c3a 204f 7074 696f 6e61   symbol: Optiona
+0005cb20: 6c5b 7374 725d 203d 204e 6f6e 652c 2070  l[str] = None, p
+0005cb30: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
+0005cb40: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0005cb50: 6570 6179 2062 6f72 726f 7765 6420 6d61  epay borrowed ma
+0005cb60: 7267 696e 2061 6e64 2069 6e74 6572 6573  rgin and interes
+0005cb70: 740a 2020 2020 2020 2020 7365 6520 6874  t.        see ht
+0005cb80: 7470 733a 2f2f 6279 6269 742d 6578 6368  tps://bybit-exch
+0005cb90: 616e 6765 2e67 6974 6875 622e 696f 2f64  ange.github.io/d
+0005cba0: 6f63 732f 7370 6f74 2f76 332f 2374 2d72  ocs/spot/v3/#t-r
+0005cbb0: 6570 6179 6d61 7267 696e 6c6f 616e 0a20  epaymarginloan. 
+0005cbc0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
+0005cbd0: 7220 636f 6465 3a20 756e 6966 6965 6420  r code: unified 
+0005cbe0: 6375 7272 656e 6379 2063 6f64 6520 6f66  currency code of
+0005cbf0: 2074 6865 2063 7572 7265 6e63 7920 746f   the currency to
+0005cc00: 2072 6570 6179 0a20 2020 2020 2020 203a   repay.        :
+0005cc10: 7061 7261 6d20 666c 6f61 7420 616d 6f75  param float amou
+0005cc20: 6e74 3a20 7468 6520 616d 6f75 6e74 2074  nt: the amount t
+0005cc30: 6f20 7265 7061 790a 2020 2020 2020 2020  o repay.        
+0005cc40: 3a70 6172 616d 2073 7472 7c4e 6f6e 6520  :param str|None 
+0005cc50: 7379 6d62 6f6c 3a20 6e6f 7420 7573 6564  symbol: not used
+0005cc60: 2062 7920 6279 6269 742e 7265 7061 794d   by bybit.repayM
+0005cc70: 6172 6769 6e28 290a 2020 2020 2020 2020  argin().        
+0005cc80: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
+0005cc90: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
+0005cca0: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
+0005ccb0: 2074 6865 2062 7962 6974 2061 7069 2065   the bybit api e
+0005ccc0: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
+0005ccd0: 3a72 6574 7572 6e73 2064 6963 743a 2061  :returns dict: a
+0005cce0: 2060 6d61 7267 696e 206c 6f61 6e20 7374   `margin loan st
+0005ccf0: 7275 6374 7572 6520 3c68 7474 7073 3a2f  ructure <https:/
+0005cd00: 2f64 6f63 732e 6363 7874 2e63 6f6d 2f23  /docs.ccxt.com/#
+0005cd10: 2f3f 6964 3d6d 6172 6769 6e2d 6c6f 616e  /?id=margin-loan
+0005cd20: 2d73 7472 7563 7475 7265 3e60 0a20 2020  -structure>`.   
+0005cd30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0005cd40: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
+0005cd50: 7473 2829 0a20 2020 2020 2020 2063 7572  ts().        cur
+0005cd60: 7265 6e63 7920 3d20 7365 6c66 2e63 7572  rency = self.cur
+0005cd70: 7265 6e63 7928 636f 6465 290a 2020 2020  rency(code).    
+0005cd80: 2020 2020 6d61 7267 696e 4d6f 6465 2c20      marginMode, 
+0005cd90: 7175 6572 7920 3d20 7365 6c66 2e68 616e  query = self.han
+0005cda0: 646c 655f 6d61 7267 696e 5f6d 6f64 655f  dle_margin_mode_
+0005cdb0: 616e 645f 7061 7261 6d73 2827 7265 7061  and_params('repa
+0005cdc0: 794d 6172 6769 6e27 2c20 7061 7261 6d73  yMargin', params
+0005cdd0: 290a 2020 2020 2020 2020 6966 206d 6172  ).        if mar
+0005cde0: 6769 6e4d 6f64 6520 3d3d 2027 6973 6f6c  ginMode == 'isol
+0005cdf0: 6174 6564 273a 0a20 2020 2020 2020 2020  ated':.         
+0005ce00: 2020 2072 6169 7365 204e 6f74 5375 7070     raise NotSupp
+0005ce10: 6f72 7465 6428 7365 6c66 2e69 6420 2b20  orted(self.id + 
+0005ce20: 2720 7265 7061 794d 6172 6769 6e28 2920  ' repayMargin() 
+0005ce30: 6361 6e6e 6f74 2075 7365 2069 736f 6c61  cannot use isola
+0005ce40: 7465 6420 6d61 7267 696e 2729 0a20 2020  ted margin').   
+0005ce50: 2020 2020 2072 6571 7565 7374 203d 207b       request = {
+0005ce60: 0a20 2020 2020 2020 2020 2020 2027 636f  .            'co
+0005ce70: 696e 273a 2063 7572 7265 6e63 795b 2769  in': currency['i
+0005ce80: 6427 5d2c 0a20 2020 2020 2020 2020 2020  d'],.           
+0005ce90: 2027 7174 7927 3a20 7365 6c66 2e6e 756d   'qty': self.num
+0005cea0: 6265 725f 746f 5f73 7472 696e 6728 616d  ber_to_string(am
+0005ceb0: 6f75 6e74 292c 0a20 2020 2020 2020 207d  ount),.        }
+0005cec0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0005ced0: 6520 3d20 7365 6c66 2e70 7269 7661 7465  e = self.private
+0005cee0: 506f 7374 5370 6f74 5633 5072 6976 6174  PostSpotV3Privat
+0005cef0: 6543 726f 7373 4d61 7267 696e 5265 7061  eCrossMarginRepa
+0005cf00: 7928 7365 6c66 2e65 7874 656e 6428 7265  y(self.extend(re
+0005cf10: 7175 6573 742c 2071 7565 7279 2929 0a20  quest, query)). 
+0005cf20: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0005cf30: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
+0005cf40: 2023 2020 2020 2020 2020 2022 7265 7443   #         "retC
+0005cf50: 6f64 6522 3a20 302c 0a20 2020 2020 2020  ode": 0,.       
+0005cf60: 2023 2020 2020 2020 2020 2022 7265 744d   #         "retM
+0005cf70: 7367 223a 2022 7375 6363 6573 7322 2c0a  sg": "success",.
+0005cf80: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005cf90: 2020 2272 6573 756c 7422 3a20 7b0a 2020    "result": {.  
+0005cfa0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005cfb0: 2020 2022 7265 7061 7949 6422 3a20 2231     "repayId": "1
+0005cfc0: 3231 3238 220a 2020 2020 2020 2020 2320  2128".        # 
+0005cfd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+0005cfe0: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+0005cff0: 7445 7874 496e 666f 223a 206e 756c 6c2c  tExtInfo": null,
+0005d000: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d010: 2020 2022 7469 6d65 223a 2031 3636 3236     "time": 16626
+0005d020: 3138 3239 3834 3532 0a20 2020 2020 2020  18298452.       
+0005d030: 2023 2020 2020 207d 0a20 2020 2020 2020   #     }.       
+0005d040: 2023 0a20 2020 2020 2020 2072 6573 756c   #.        resul
+0005d050: 7420 3d20 7365 6c66 2e73 6166 655f 7661  t = self.safe_va
+0005d060: 6c75 6528 7265 7370 6f6e 7365 2c20 2772  lue(response, 'r
+0005d070: 6573 756c 7427 2c20 7b7d 290a 2020 2020  esult', {}).    
+0005d080: 2020 2020 7472 616e 7361 6374 696f 6e20      transaction 
+0005d090: 3d20 7365 6c66 2e70 6172 7365 5f6d 6172  = self.parse_mar
+0005d0a0: 6769 6e5f 6c6f 616e 2872 6573 756c 742c  gin_loan(result,
+0005d0b0: 2063 7572 7265 6e63 7929 0a20 2020 2020   currency).     
+0005d0c0: 2020 2072 6574 7572 6e20 7365 6c66 2e65     return self.e
+0005d0d0: 7874 656e 6428 7472 616e 7361 6374 696f  xtend(transactio
+0005d0e0: 6e2c 207b 0a20 2020 2020 2020 2020 2020  n, {.           
+0005d0f0: 2027 7379 6d62 6f6c 273a 2073 796d 626f   'symbol': symbo
+0005d100: 6c2c 0a20 2020 2020 2020 2020 2020 2027  l,.            '
+0005d110: 616d 6f75 6e74 273a 2061 6d6f 756e 742c  amount': amount,
+0005d120: 0a20 2020 2020 2020 207d 290a 0a20 2020  .        })..   
+0005d130: 2064 6566 2070 6172 7365 5f6d 6172 6769   def parse_margi
+0005d140: 6e5f 6c6f 616e 2873 656c 662c 2069 6e66  n_loan(self, inf
+0005d150: 6f2c 2063 7572 7265 6e63 793d 4e6f 6e65  o, currency=None
+0005d160: 293a 0a20 2020 2020 2020 2023 0a20 2020  ):.        #.   
+0005d170: 2020 2020 2023 2062 6f72 726f 774d 6172       # borrowMar
+0005d180: 6769 6e0a 2020 2020 2020 2020 230a 2020  gin.        #.  
+0005d190: 2020 2020 2020 2320 2020 2020 7b0a 2020        #     {.  
+0005d1a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005d1b0: 2274 7261 6e73 6163 7449 6422 3a20 2231  "transactId": "1
+0005d1c0: 3431 3433 220a 2020 2020 2020 2020 2320  4143".        # 
+0005d1d0: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
+0005d1e0: 2020 2020 2020 2020 2320 7265 7061 794d          # repayM
+0005d1f0: 6172 6769 6e0a 2020 2020 2020 2020 230a  argin.        #.
+0005d200: 2020 2020 2020 2020 2320 2020 2020 7b0a          #     {.
+0005d210: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005d220: 2020 2272 6570 6179 4964 223a 2022 3132    "repayId": "12
+0005d230: 3132 3822 0a20 2020 2020 2020 2023 2020  128".        #  
+0005d240: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
+0005d250: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+0005d260: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
+0005d270: 3a20 7365 6c66 2e73 6166 655f 7374 7269  : self.safe_stri
+0005d280: 6e67 5f32 2869 6e66 6f2c 2027 7472 616e  ng_2(info, 'tran
+0005d290: 7361 6374 4964 272c 2027 7265 7061 7949  sactId', 'repayI
+0005d2a0: 6427 292c 0a20 2020 2020 2020 2020 2020  d'),.           
+0005d2b0: 2027 6375 7272 656e 6379 273a 2073 656c   'currency': sel
+0005d2c0: 662e 7361 6665 5f73 7472 696e 6728 6375  f.safe_string(cu
+0005d2d0: 7272 656e 6379 2c20 2763 6f64 6527 292c  rrency, 'code'),
+0005d2e0: 0a20 2020 2020 2020 2020 2020 2027 616d  .            'am
+0005d2f0: 6f75 6e74 273a 204e 6f6e 652c 0a20 2020  ount': None,.   
+0005d300: 2020 2020 2020 2020 2027 7379 6d62 6f6c           'symbol
+0005d310: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+0005d320: 2020 2020 2027 7469 6d65 7374 616d 7027       'timestamp'
+0005d330: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+0005d340: 2020 2020 2764 6174 6574 696d 6527 3a20      'datetime': 
+0005d350: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0005d360: 2020 2769 6e66 6f27 3a20 696e 666f 2c0a    'info': info,.
+0005d370: 2020 2020 2020 2020 7d0a 0a20 2020 2064          }..    d
+0005d380: 6566 2070 6172 7365 5f74 7261 6e73 6665  ef parse_transfe
+0005d390: 725f 7374 6174 7573 2873 656c 662c 2073  r_status(self, s
+0005d3a0: 7461 7475 7329 3a0a 2020 2020 2020 2020  tatus):.        
+0005d3b0: 7374 6174 7573 6573 203d 207b 0a20 2020  statuses = {.   
+0005d3c0: 2020 2020 2020 2020 2027 3027 3a20 276f           '0': 'o
+0005d3d0: 6b27 2c0a 2020 2020 2020 2020 2020 2020  k',.            
+0005d3e0: 274f 4b27 3a20 276f 6b27 2c0a 2020 2020  'OK': 'ok',.    
+0005d3f0: 2020 2020 2020 2020 2753 5543 4345 5353          'SUCCESS
+0005d400: 273a 2027 6f6b 272c 0a20 2020 2020 2020  ': 'ok',.       
+0005d410: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
+0005d420: 6e20 7365 6c66 2e73 6166 655f 7374 7269  n self.safe_stri
+0005d430: 6e67 2873 7461 7475 7365 732c 2073 7461  ng(statuses, sta
+0005d440: 7475 732c 2073 7461 7475 7329 0a0a 2020  tus, status)..  
+0005d450: 2020 6465 6620 7061 7273 655f 7472 616e    def parse_tran
+0005d460: 7366 6572 2873 656c 662c 2074 7261 6e73  sfer(self, trans
+0005d470: 6665 722c 2063 7572 7265 6e63 793d 4e6f  fer, currency=No
+0005d480: 6e65 293a 0a20 2020 2020 2020 2023 0a20  ne):.        #. 
+0005d490: 2020 2020 2020 2023 2074 7261 6e73 6665         # transfe
+0005d4a0: 720a 2020 2020 2020 2020 230a 2020 2020  r.        #.    
+0005d4b0: 2020 2020 2320 2020 2020 7b0a 2020 2020      #     {.    
+0005d4c0: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
+0005d4d0: 7261 6e73 6665 7249 6422 3a20 2232 3263  ransferId": "22c
+0005d4e0: 3262 6331 312d 6564 3562 2d34 3961 342d  2bc11-ed5b-49a4-
+0005d4f0: 3836 3437 2d63 3465 3066 3566 3666 3262  8647-c4e0f5f6f2b
+0005d500: 3222 2020 2320 7472 616e 7366 6572 5f69  2"  # transfer_i
+0005d510: 6420 696e 2076 310a 2020 2020 2020 2020  d in v1.        
+0005d520: 2320 2020 2020 7d0a 2020 2020 2020 2020  #     }.        
+0005d530: 230a 2020 2020 2020 2020 2320 6665 7463  #.        # fetc
+0005d540: 6854 7261 6e73 6665 7273 0a20 2020 2020  hTransfers.     
+0005d550: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+0005d560: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
+0005d570: 2020 2020 2020 2022 7472 616e 7366 6572         "transfer
+0005d580: 4964 223a 2022 6539 6334 3231 6334 2d62  Id": "e9c421c4-b
+0005d590: 3031 302d 3462 3136 2d61 6264 362d 3130  010-4b16-abd6-10
+0005d5a0: 3631 3739 6632 3737 3032 222c 2020 2320  6179f27702",  # 
+0005d5b0: 7472 616e 7366 6572 5f69 6420 696e 2076  transfer_id in v
+0005d5c0: 310a 2020 2020 2020 2020 2320 2020 2020  1.        #     
+0005d5d0: 2020 2020 2263 6f69 6e22 3a20 2255 5344      "coin": "USD
+0005d5e0: 5422 2c0a 2020 2020 2020 2020 2320 2020  T",.        #   
+0005d5f0: 2020 2020 2020 2261 6d6f 756e 7422 3a20        "amount": 
+0005d600: 2238 222c 0a20 2020 2020 2020 2023 2020  "8",.        #  
+0005d610: 2020 2020 2020 2022 6672 6f6d 4163 636f         "fromAcco
+0005d620: 756e 7454 7970 6522 3a20 2246 554e 4422  untType": "FUND"
+0005d630: 2c20 2023 2066 726f 6d5f 6163 636f 756e  ,  # from_accoun
+0005d640: 745f 7479 7065 2069 6e20 7631 0a20 2020  t_type in v1.   
+0005d650: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005d660: 746f 4163 636f 756e 7454 7970 6522 3a20  toAccountType": 
+0005d670: 2253 504f 5422 2c20 2023 2074 6f5f 6163  "SPOT",  # to_ac
+0005d680: 636f 756e 745f 7479 7065 2069 6e20 7631  count_type in v1
+0005d690: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d6a0: 2020 2022 7469 6d65 7374 616d 7022 3a20     "timestamp": 
+0005d6b0: 2231 3636 3638 3739 3432 3630 3030 222c  "1666879426000",
+0005d6c0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005d6d0: 2020 2022 7374 6174 7573 223a 2022 5355     "status": "SU
+0005d6e0: 4343 4553 5322 0a20 2020 2020 2020 2023  CCESS".        #
+0005d6f0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0005d700: 230a 2020 2020 2020 2020 6375 7272 656e  #.        curren
+0005d710: 6379 4964 203d 2073 656c 662e 7361 6665  cyId = self.safe
+0005d720: 5f73 7472 696e 6728 7472 616e 7366 6572  _string(transfer
+0005d730: 2c20 2763 6f69 6e27 290a 2020 2020 2020  , 'coin').      
+0005d740: 2020 7469 6d65 7374 616d 7020 3d20 7365    timestamp = se
+0005d750: 6c66 2e73 6166 655f 696e 7465 6765 7228  lf.safe_integer(
+0005d760: 7472 616e 7366 6572 2c20 2774 696d 6573  transfer, 'times
+0005d770: 7461 6d70 2729 0a20 2020 2020 2020 2066  tamp').        f
+0005d780: 726f 6d41 6363 6f75 6e74 4964 203d 2073  romAccountId = s
+0005d790: 656c 662e 7361 6665 5f73 7472 696e 675f  elf.safe_string_
+0005d7a0: 3228 7472 616e 7366 6572 2c20 2766 726f  2(transfer, 'fro
+0005d7b0: 6d41 6363 6f75 6e74 5479 7065 272c 2027  mAccountType', '
+0005d7c0: 6672 6f6d 5f61 6363 6f75 6e74 5f74 7970  from_account_typ
+0005d7d0: 6527 290a 2020 2020 2020 2020 746f 4163  e').        toAc
+0005d7e0: 636f 756e 7449 6420 3d20 7365 6c66 2e73  countId = self.s
+0005d7f0: 6166 655f 7374 7269 6e67 5f32 2874 7261  afe_string_2(tra
+0005d800: 6e73 6665 722c 2027 746f 4163 636f 756e  nsfer, 'toAccoun
+0005d810: 7454 7970 6527 2c20 2774 6f5f 6163 636f  tType', 'to_acco
+0005d820: 756e 745f 7479 7065 2729 0a20 2020 2020  unt_type').     
+0005d830: 2020 2061 6363 6f75 6e74 4964 7320 3d20     accountIds = 
+0005d840: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
+0005d850: 7365 6c66 2e6f 7074 696f 6e73 2c20 2761  self.options, 'a
+0005d860: 6363 6f75 6e74 7342 7949 6427 2c20 7b7d  ccountsById', {}
+0005d870: 290a 2020 2020 2020 2020 6672 6f6d 4163  ).        fromAc
+0005d880: 636f 756e 7420 3d20 7365 6c66 2e73 6166  count = self.saf
+0005d890: 655f 7374 7269 6e67 2861 6363 6f75 6e74  e_string(account
+0005d8a0: 4964 732c 2066 726f 6d41 6363 6f75 6e74  Ids, fromAccount
+0005d8b0: 4964 2c20 6672 6f6d 4163 636f 756e 7449  Id, fromAccountI
+0005d8c0: 6429 0a20 2020 2020 2020 2074 6f41 6363  d).        toAcc
+0005d8d0: 6f75 6e74 203d 2073 656c 662e 7361 6665  ount = self.safe
+0005d8e0: 5f73 7472 696e 6728 6163 636f 756e 7449  _string(accountI
+0005d8f0: 6473 2c20 746f 4163 636f 756e 7449 642c  ds, toAccountId,
+0005d900: 2074 6f41 6363 6f75 6e74 4964 290a 2020   toAccountId).  
+0005d910: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+0005d920: 2020 2020 2020 2020 2020 2027 696e 666f             'info
+0005d930: 273a 2074 7261 6e73 6665 722c 0a20 2020  ': transfer,.   
+0005d940: 2020 2020 2020 2020 2027 6964 273a 2073           'id': s
+0005d950: 656c 662e 7361 6665 5f73 7472 696e 675f  elf.safe_string_
+0005d960: 3228 7472 616e 7366 6572 2c20 2774 7261  2(transfer, 'tra
+0005d970: 6e73 6665 7249 6427 2c20 2774 7261 6e73  nsferId', 'trans
+0005d980: 6665 725f 6964 2729 2c0a 2020 2020 2020  fer_id'),.      
+0005d990: 2020 2020 2020 2774 696d 6573 7461 6d70        'timestamp
+0005d9a0: 273a 2074 696d 6573 7461 6d70 2c0a 2020  ': timestamp,.  
+0005d9b0: 2020 2020 2020 2020 2020 2764 6174 6574            'datet
+0005d9c0: 696d 6527 3a20 7365 6c66 2e69 736f 3836  ime': self.iso86
+0005d9d0: 3031 2874 696d 6573 7461 6d70 292c 0a20  01(timestamp),. 
+0005d9e0: 2020 2020 2020 2020 2020 2027 6375 7272             'curr
+0005d9f0: 656e 6379 273a 2073 656c 662e 7361 6665  ency': self.safe
+0005da00: 5f63 7572 7265 6e63 795f 636f 6465 2863  _currency_code(c
+0005da10: 7572 7265 6e63 7949 642c 2063 7572 7265  urrencyId, curre
+0005da20: 6e63 7929 2c0a 2020 2020 2020 2020 2020  ncy),.          
+0005da30: 2020 2761 6d6f 756e 7427 3a20 7365 6c66    'amount': self
+0005da40: 2e73 6166 655f 6e75 6d62 6572 2874 7261  .safe_number(tra
+0005da50: 6e73 6665 722c 2027 616d 6f75 6e74 2729  nsfer, 'amount')
+0005da60: 2c0a 2020 2020 2020 2020 2020 2020 2766  ,.            'f
+0005da70: 726f 6d41 6363 6f75 6e74 273a 2066 726f  romAccount': fro
+0005da80: 6d41 6363 6f75 6e74 2c0a 2020 2020 2020  mAccount,.      
+0005da90: 2020 2020 2020 2774 6f41 6363 6f75 6e74        'toAccount
+0005daa0: 273a 2074 6f41 6363 6f75 6e74 2c0a 2020  ': toAccount,.  
+0005dab0: 2020 2020 2020 2020 2020 2773 7461 7475            'statu
+0005dac0: 7327 3a20 7365 6c66 2e70 6172 7365 5f74  s': self.parse_t
+0005dad0: 7261 6e73 6665 725f 7374 6174 7573 2873  ransfer_status(s
+0005dae0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0005daf0: 7472 616e 7366 6572 2c20 2773 7461 7475  transfer, 'statu
+0005db00: 7327 2929 2c0a 2020 2020 2020 2020 7d0a  s')),.        }.
+0005db10: 0a20 2020 2064 6566 2066 6574 6368 5f64  .    def fetch_d
+0005db20: 6572 6976 6174 6976 6573 5f6d 6172 6b65  erivatives_marke
+0005db30: 745f 6c65 7665 7261 6765 5f74 6965 7273  t_leverage_tiers
+0005db40: 2873 656c 662c 2073 796d 626f 6c3a 2073  (self, symbol: s
+0005db50: 7472 2c20 7061 7261 6d73 3d7b 7d29 3a0a  tr, params={}):.
+0005db60: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+0005db70: 645f 6d61 726b 6574 7328 290a 2020 2020  d_markets().    
+0005db80: 2020 2020 6d61 726b 6574 203d 2073 656c      market = sel
+0005db90: 662e 6d61 726b 6574 2873 796d 626f 6c29  f.market(symbol)
+0005dba0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0005dbb0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0005dbc0: 2027 7379 6d62 6f6c 273a 206d 6172 6b65   'symbol': marke
+0005dbd0: 745b 2769 6427 5d2c 0a20 2020 2020 2020  t['id'],.       
+0005dbe0: 207d 0a20 2020 2020 2020 2069 6620 6d61   }.        if ma
+0005dbf0: 726b 6574 5b27 6c69 6e65 6172 275d 3a0a  rket['linear']:.
+0005dc00: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0005dc10: 6573 745b 2763 6174 6567 6f72 7927 5d20  est['category'] 
+0005dc20: 3d20 276c 696e 6561 7227 0a20 2020 2020  = 'linear'.     
+0005dc30: 2020 2065 6c69 6620 6d61 726b 6574 5b27     elif market['
+0005dc40: 696e 7665 7273 6527 5d3a 0a20 2020 2020  inverse']:.     
+0005dc50: 2020 2020 2020 2072 6571 7565 7374 5b27         request['
+0005dc60: 6361 7465 676f 7279 275d 203d 2027 696e  category'] = 'in
+0005dc70: 7665 7273 6527 0a20 2020 2020 2020 2072  verse'.        r
+0005dc80: 6573 706f 6e73 6520 3d20 7365 6c66 2e70  esponse = self.p
+0005dc90: 7562 6c69 6347 6574 5635 4d61 726b 6574  ublicGetV5Market
+0005dca0: 5269 736b 4c69 6d69 7428 7365 6c66 2e65  RiskLimit(self.e
+0005dcb0: 7874 656e 6428 7265 7175 6573 742c 2070  xtend(request, p
+0005dcc0: 6172 616d 7329 290a 2020 2020 2020 2020  arams)).        
+0005dcd0: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
+0005dce0: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+0005dcf0: 2020 2020 2272 6574 436f 6465 223a 2030      "retCode": 0
+0005dd00: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005dd10: 2020 2020 2272 6574 4d73 6722 3a20 224f      "retMsg": "O
+0005dd20: 4b22 2c0a 2020 2020 2020 2020 2320 2020  K",.        #   
+0005dd30: 2020 2020 2020 2272 6573 756c 7422 3a20        "result": 
+0005dd40: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+0005dd50: 2020 2020 2020 2020 2263 6174 6567 6f72          "categor
+0005dd60: 7922 3a20 2269 6e76 6572 7365 222c 0a20  y": "inverse",. 
+0005dd70: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005dd80: 2020 2020 2022 6c69 7374 223a 205b 0a20       "list": [. 
+0005dd90: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0005dda0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0005ddb0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005ddc0: 2020 2020 2020 2020 2022 6964 223a 2031           "id": 1
+0005ddd0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005ddf0: 2273 796d 626f 6c22 3a20 2242 5443 5553  "symbol": "BTCUS
+0005de00: 4422 2c0a 2020 2020 2020 2020 2320 2020  D",.        #   
+0005de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005de20: 2020 2272 6973 6b4c 696d 6974 5661 6c75    "riskLimitValu
+0005de30: 6522 3a20 2231 3530 222c 0a20 2020 2020  e": "150",.     
+0005de40: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0005de50: 2020 2020 2020 2020 2022 6d61 696e 7465           "mainte
+0005de60: 6e61 6e63 654d 6172 6769 6e22 3a20 2230  nanceMargin": "0
+0005de70: 2e35 222c 0a20 2020 2020 2020 2023 2020  .5",.        #  
+0005de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005de90: 2020 2022 696e 6974 6961 6c4d 6172 6769     "initialMargi
+0005dea0: 6e22 3a20 2231 222c 0a20 2020 2020 2020  n": "1",.       
+0005deb0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0005dec0: 2020 2020 2020 2022 6973 4c6f 7765 7374         "isLowest
+0005ded0: 5269 736b 223a 2031 2c0a 2020 2020 2020  Risk": 1,.      
+0005dee0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0005def0: 2020 2020 2020 2020 226d 6178 4c65 7665          "maxLeve
+0005df00: 7261 6765 223a 2022 3130 302e 3030 220a  rage": "100.00".
+0005df10: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005df20: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+0005df30: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0005df40: 2020 202e 2e2e 2e0a 2020 2020 2020 2020     .....        
+0005df50: 2320 2020 2020 2020 2020 2020 2020 5d0a  #             ].
+0005df60: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005df70: 2020 7d2c 0a20 2020 2020 2020 2023 2020    },.        #  
+0005df80: 2020 2020 2020 2022 7265 7445 7874 496e         "retExtIn
+0005df90: 666f 223a 207b 7d2c 0a20 2020 2020 2020  fo": {},.       
+0005dfa0: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
+0005dfb0: 223a 2031 3637 3230 3534 3438 3830 3130  ": 1672054488010
+0005dfc0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+0005dfd0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0005dfe0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0005dff0: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
+0005e000: 6f6e 7365 2c20 2772 6573 756c 7427 290a  onse, 'result').
+0005e010: 2020 2020 2020 2020 7469 6572 7320 3d20          tiers = 
+0005e020: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
+0005e030: 7265 7375 6c74 2c20 276c 6973 7427 290a  result, 'list').
+0005e040: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0005e050: 656c 662e 7061 7273 655f 6d61 726b 6574  elf.parse_market
+0005e060: 5f6c 6576 6572 6167 655f 7469 6572 7328  _leverage_tiers(
+0005e070: 7469 6572 732c 206d 6172 6b65 7429 0a0a  tiers, market)..
+0005e080: 2020 2020 6465 6620 6665 7463 685f 6d61      def fetch_ma
+0005e090: 726b 6574 5f6c 6576 6572 6167 655f 7469  rket_leverage_ti
+0005e0a0: 6572 7328 7365 6c66 2c20 7379 6d62 6f6c  ers(self, symbol
+0005e0b0: 3a20 7374 722c 2070 6172 616d 733d 7b7d  : str, params={}
+0005e0c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0005e0d0: 2020 2020 2020 2072 6574 7269 6576 6520         retrieve 
+0005e0e0: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
+0005e0f0: 6865 206d 6178 696d 756d 206c 6576 6572  he maximum lever
+0005e100: 6167 652c 2061 6e64 206d 6169 6e74 656e  age, and mainten
+0005e110: 616e 6365 206d 6172 6769 6e20 666f 7220  ance margin for 
+0005e120: 7472 6164 6573 206f 6620 7661 7279 696e  trades of varyin
+0005e130: 6720 7472 6164 6520 7369 7a65 7320 666f  g trade sizes fo
+0005e140: 7220 6120 7369 6e67 6c65 206d 6172 6b65  r a single marke
+0005e150: 740a 2020 2020 2020 2020 7365 6520 6874  t.        see ht
+0005e160: 7470 733a 2f2f 6279 6269 742d 6578 6368  tps://bybit-exch
+0005e170: 616e 6765 2e67 6974 6875 622e 696f 2f64  ange.github.io/d
+0005e180: 6f63 732f 7635 2f6d 6172 6b65 742f 7269  ocs/v5/market/ri
+0005e190: 736b 2d6c 696d 6974 0a20 2020 2020 2020  sk-limit.       
+0005e1a0: 203a 7061 7261 6d20 7374 7220 7379 6d62   :param str symb
+0005e1b0: 6f6c 3a20 756e 6966 6965 6420 6d61 726b  ol: unified mark
+0005e1c0: 6574 2073 796d 626f 6c0a 2020 2020 2020  et symbol.      
+0005e1d0: 2020 3a70 6172 616d 2064 6963 7420 7061    :param dict pa
+0005e1e0: 7261 6d73 3a20 6578 7472 6120 7061 7261  rams: extra para
+0005e1f0: 6d65 7465 7273 2073 7065 6369 6669 6320  meters specific 
+0005e200: 746f 2074 6865 2062 7962 6974 2061 7069  to the bybit api
+0005e210: 2065 6e64 706f 696e 740a 2020 2020 2020   endpoint.      
+0005e220: 2020 3a72 6574 7572 6e73 2064 6963 743a    :returns dict:
+0005e230: 2061 2060 6c65 7665 7261 6765 2074 6965   a `leverage tie
+0005e240: 7273 2073 7472 7563 7475 7265 203c 6874  rs structure <ht
+0005e250: 7470 733a 2f2f 646f 6373 2e63 6378 742e  tps://docs.ccxt.
+0005e260: 636f 6d2f 232f 3f69 643d 6c65 7665 7261  com/#/?id=levera
+0005e270: 6765 2d74 6965 7273 2d73 7472 7563 7475  ge-tiers-structu
+0005e280: 7265 3e60 0a20 2020 2020 2020 2022 2222  re>`.        """
+0005e290: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+0005e2a0: 6164 5f6d 6172 6b65 7473 2829 0a20 2020  ad_markets().   
+0005e2b0: 2020 2020 2072 6571 7565 7374 203d 207b       request = {
+0005e2c0: 7d0a 2020 2020 2020 2020 6d61 726b 6574  }.        market
+0005e2d0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0005e2e0: 6d61 726b 6574 203d 2073 656c 662e 6d61  market = self.ma
+0005e2f0: 726b 6574 2873 796d 626f 6c29 0a20 2020  rket(symbol).   
+0005e300: 2020 2020 2069 6620 6d61 726b 6574 5b27       if market['
+0005e310: 7370 6f74 275d 206f 7220 6d61 726b 6574  spot'] or market
+0005e320: 5b27 6f70 7469 6f6e 275d 3a0a 2020 2020  ['option']:.    
+0005e330: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+0005e340: 6452 6571 7565 7374 2873 656c 662e 6964  dRequest(self.id
+0005e350: 202b 2027 2066 6574 6368 4d61 726b 6574   + ' fetchMarket
+0005e360: 4c65 7665 7261 6765 5469 6572 7328 2920  LeverageTiers() 
+0005e370: 7379 6d62 6f6c 2064 6f65 7320 6e6f 7420  symbol does not 
+0005e380: 7375 7070 6f72 7420 6d61 726b 6574 2027  support market '
+0005e390: 202b 2073 796d 626f 6c29 0a20 2020 2020   + symbol).     
+0005e3a0: 2020 2072 6571 7565 7374 5b27 7379 6d62     request['symb
+0005e3b0: 6f6c 275d 203d 206d 6172 6b65 745b 2769  ol'] = market['i
+0005e3c0: 6427 5d0a 2020 2020 2020 2020 7265 7475  d'].        retu
+0005e3d0: 726e 2073 656c 662e 6665 7463 685f 6465  rn self.fetch_de
+0005e3e0: 7269 7661 7469 7665 735f 6d61 726b 6574  rivatives_market
+0005e3f0: 5f6c 6576 6572 6167 655f 7469 6572 7328  _leverage_tiers(
+0005e400: 7379 6d62 6f6c 2c20 7061 7261 6d73 290a  symbol, params).
+0005e410: 0a20 2020 2064 6566 2070 6172 7365 5f6d  .    def parse_m
+0005e420: 6172 6b65 745f 6c65 7665 7261 6765 5f74  arket_leverage_t
+0005e430: 6965 7273 2873 656c 662c 2069 6e66 6f2c  iers(self, info,
+0005e440: 206d 6172 6b65 743d 4e6f 6e65 293a 0a20   market=None):. 
+0005e450: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0005e460: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
+0005e470: 2023 2020 2020 2020 2020 2022 6964 223a   #         "id":
+0005e480: 2031 2c0a 2020 2020 2020 2020 2320 2020   1,.        #   
+0005e490: 2020 2020 2020 2273 796d 626f 6c22 3a20        "symbol": 
+0005e4a0: 2242 5443 5553 4422 2c0a 2020 2020 2020  "BTCUSD",.      
+0005e4b0: 2020 2320 2020 2020 2020 2020 2272 6973    #         "ris
+0005e4c0: 6b4c 696d 6974 5661 6c75 6522 3a20 2231  kLimitValue": "1
+0005e4d0: 3530 222c 0a20 2020 2020 2020 2023 2020  50",.        #  
+0005e4e0: 2020 2020 2020 2022 6d61 696e 7465 6e61         "maintena
+0005e4f0: 6e63 654d 6172 6769 6e22 3a20 2230 2e35  nceMargin": "0.5
+0005e500: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0005e510: 2020 2020 2022 696e 6974 6961 6c4d 6172       "initialMar
+0005e520: 6769 6e22 3a20 2231 222c 0a20 2020 2020  gin": "1",.     
+0005e530: 2020 2023 2020 2020 2020 2020 2022 6973     #         "is
+0005e540: 4c6f 7765 7374 5269 736b 223a 2031 2c0a  LowestRisk": 1,.
+0005e550: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005e560: 2020 226d 6178 4c65 7665 7261 6765 223a    "maxLeverage":
+0005e570: 2022 3130 302e 3030 220a 2020 2020 2020   "100.00".      
+0005e580: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
+0005e590: 2020 230a 2020 2020 2020 2020 6d69 6e4e    #.        minN
+0005e5a0: 6f74 696f 6e61 6c20 3d20 300a 2020 2020  otional = 0.    
+0005e5b0: 2020 2020 7469 6572 7320 3d20 5b5d 0a20      tiers = []. 
+0005e5c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0005e5d0: 7261 6e67 6528 302c 206c 656e 2869 6e66  range(0, len(inf
+0005e5e0: 6f29 293a 0a20 2020 2020 2020 2020 2020  o)):.           
+0005e5f0: 2069 7465 6d20 3d20 696e 666f 5b69 5d0a   item = info[i].
+0005e600: 2020 2020 2020 2020 2020 2020 6d61 784e              maxN
+0005e610: 6f74 696f 6e61 6c20 3d20 7365 6c66 2e73  otional = self.s
+0005e620: 6166 655f 6e75 6d62 6572 2869 7465 6d2c  afe_number(item,
+0005e630: 2027 7269 736b 4c69 6d69 7456 616c 7565   'riskLimitValue
+0005e640: 2729 0a20 2020 2020 2020 2020 2020 2074  ').            t
+0005e650: 6965 7273 2e61 7070 656e 6428 7b0a 2020  iers.append({.  
+0005e660: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0005e670: 6965 7227 3a20 7365 6c66 2e73 756d 2869  ier': self.sum(i
+0005e680: 2c20 3129 2c0a 2020 2020 2020 2020 2020  , 1),.          
+0005e690: 2020 2020 2020 2763 7572 7265 6e63 7927        'currency'
+0005e6a0: 3a20 6d61 726b 6574 5b27 6261 7365 275d  : market['base']
 0005e6b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0005e6c0: 2020 2769 6e66 6f27 3a20 6974 656d 2c0a    'info': item,.
-0005e6d0: 2020 2020 2020 2020 2020 2020 7d29 0a20              }). 
-0005e6e0: 2020 2020 2020 2020 2020 206d 696e 4e6f             minNo
-0005e6f0: 7469 6f6e 616c 203d 206d 6178 4e6f 7469  tional = maxNoti
-0005e700: 6f6e 616c 0a20 2020 2020 2020 2072 6574  onal.        ret
-0005e710: 7572 6e20 7469 6572 730a 0a20 2020 2064  urn tiers..    d
-0005e720: 6566 2070 6172 7365 5f74 7261 6469 6e67  ef parse_trading
-0005e730: 5f66 6565 2873 656c 662c 2066 6565 2c20  _fee(self, fee, 
-0005e740: 6d61 726b 6574 3d4e 6f6e 6529 3a0a 2020  market=None):.  
-0005e750: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-0005e760: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
-0005e770: 2320 2020 2020 2020 2020 2273 796d 626f  #         "symbo
-0005e780: 6c22 3a20 2245 5448 5553 4454 222c 0a20  l": "ETHUSDT",. 
-0005e790: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005e7a0: 2022 6d61 6b65 7246 6565 5261 7465 223a   "makerFeeRate":
-0005e7b0: 2030 2e30 3031 2c0a 2020 2020 2020 2020   0.001,.        
-0005e7c0: 2320 2020 2020 2020 2020 2274 616b 6572  #         "taker
-0005e7d0: 4665 6552 6174 6522 3a20 302e 3030 310a  FeeRate": 0.001.
-0005e7e0: 2020 2020 2020 2020 2320 2020 2020 7d0a          #     }.
-0005e7f0: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-0005e800: 2020 6d61 726b 6574 4964 203d 2073 656c    marketId = sel
-0005e810: 662e 7361 6665 5f73 7472 696e 6728 6665  f.safe_string(fe
-0005e820: 652c 2027 7379 6d62 6f6c 2729 0a20 2020  e, 'symbol').   
-0005e830: 2020 2020 2073 796d 626f 6c20 3d20 7365       symbol = se
-0005e840: 6c66 2e73 6166 655f 7379 6d62 6f6c 286d  lf.safe_symbol(m
-0005e850: 6172 6b65 7449 642c 204e 6f6e 652c 204e  arketId, None, N
-0005e860: 6f6e 652c 2027 636f 6e74 7261 6374 2729  one, 'contract')
-0005e870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0005e880: 7b0a 2020 2020 2020 2020 2020 2020 2769  {.            'i
-0005e890: 6e66 6f27 3a20 6665 652c 0a20 2020 2020  nfo': fee,.     
-0005e8a0: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
-0005e8b0: 2073 796d 626f 6c2c 0a20 2020 2020 2020   symbol,.       
-0005e8c0: 2020 2020 2027 6d61 6b65 7227 3a20 7365       'maker': se
-0005e8d0: 6c66 2e73 6166 655f 6e75 6d62 6572 2866  lf.safe_number(f
-0005e8e0: 6565 2c20 276d 616b 6572 4665 6552 6174  ee, 'makerFeeRat
-0005e8f0: 6527 292c 0a20 2020 2020 2020 2020 2020  e'),.           
-0005e900: 2027 7461 6b65 7227 3a20 7365 6c66 2e73   'taker': self.s
-0005e910: 6166 655f 6e75 6d62 6572 2866 6565 2c20  afe_number(fee, 
-0005e920: 2774 616b 6572 4665 6552 6174 6527 292c  'takerFeeRate'),
-0005e930: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-0005e940: 6465 6620 6665 7463 685f 7472 6164 696e  def fetch_tradin
-0005e950: 675f 6665 6528 7365 6c66 2c20 7379 6d62  g_fee(self, symb
-0005e960: 6f6c 3a20 7374 722c 2070 6172 616d 733d  ol: str, params=
-0005e970: 7b7d 293a 0a20 2020 2020 2020 2022 2222  {}):.        """
-0005e980: 0a20 2020 2020 2020 2066 6574 6368 2074  .        fetch t
-0005e990: 6865 2074 7261 6469 6e67 2066 6565 7320  he trading fees 
-0005e9a0: 666f 7220 6120 6d61 726b 6574 0a20 2020  for a market.   
-0005e9b0: 2020 2020 2073 6565 2068 7474 7073 3a2f       see https:/
-0005e9c0: 2f62 7962 6974 2d65 7863 6861 6e67 652e  /bybit-exchange.
-0005e9d0: 6769 7468 7562 2e69 6f2f 646f 6373 2f76  github.io/docs/v
-0005e9e0: 352f 6163 636f 756e 742f 6665 652d 7261  5/account/fee-ra
-0005e9f0: 7465 0a20 2020 2020 2020 203a 7061 7261  te.        :para
-0005ea00: 6d20 7374 7220 7379 6d62 6f6c 3a20 756e  m str symbol: un
-0005ea10: 6966 6965 6420 6d61 726b 6574 2073 796d  ified market sym
-0005ea20: 626f 6c0a 2020 2020 2020 2020 3a70 6172  bol.        :par
-0005ea30: 616d 2064 6963 7420 7061 7261 6d73 3a20  am dict params: 
-0005ea40: 6578 7472 6120 7061 7261 6d65 7465 7273  extra parameters
-0005ea50: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
-0005ea60: 2062 7962 6974 2061 7069 2065 6e64 706f   bybit api endpo
-0005ea70: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
-0005ea80: 7572 6e73 2064 6963 743a 2061 2060 6665  urns dict: a `fe
-0005ea90: 6520 7374 7275 6374 7572 6520 3c68 7474  e structure <htt
-0005eaa0: 7073 3a2f 2f64 6f63 732e 6363 7874 2e63  ps://docs.ccxt.c
-0005eab0: 6f6d 2f23 2f3f 6964 3d66 6565 2d73 7472  om/#/?id=fee-str
-0005eac0: 7563 7475 7265 3e60 0a20 2020 2020 2020  ucture>`.       
-0005ead0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-0005eae0: 662e 6c6f 6164 5f6d 6172 6b65 7473 2829  f.load_markets()
-0005eaf0: 0a20 2020 2020 2020 206d 6172 6b65 7420  .        market 
-0005eb00: 3d20 7365 6c66 2e6d 6172 6b65 7428 7379  = self.market(sy
-0005eb10: 6d62 6f6c 290a 2020 2020 2020 2020 6966  mbol).        if
-0005eb20: 206d 6172 6b65 745b 2773 706f 7427 5d3a   market['spot']:
-0005eb30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0005eb40: 7365 204e 6f74 5375 7070 6f72 7465 6428  se NotSupported(
-0005eb50: 7365 6c66 2e69 6420 2b20 2720 6665 7463  self.id + ' fetc
-0005eb60: 6854 7261 6469 6e67 4665 6528 2920 6973  hTradingFee() is
-0005eb70: 206e 6f74 2073 7570 706f 7274 6564 2066   not supported f
-0005eb80: 6f72 2073 706f 7420 6d61 726b 6574 2729  or spot market')
-0005eb90: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0005eba0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0005ebb0: 2027 7379 6d62 6f6c 273a 206d 6172 6b65   'symbol': marke
-0005ebc0: 745b 2769 6427 5d2c 0a20 2020 2020 2020  t['id'],.       
-0005ebd0: 207d 0a20 2020 2020 2020 2072 6573 706f   }.        respo
-0005ebe0: 6e73 6520 3d20 7365 6c66 2e70 7269 7661  nse = self.priva
-0005ebf0: 7465 4765 7456 3541 6363 6f75 6e74 4665  teGetV5AccountFe
-0005ec00: 6552 6174 6528 7365 6c66 2e65 7874 656e  eRate(self.exten
-0005ec10: 6428 7265 7175 6573 742c 2070 6172 616d  d(request, param
-0005ec20: 7329 290a 2020 2020 2020 2020 230a 2020  s)).        #.  
-0005ec30: 2020 2020 2020 2320 2020 2020 7b0a 2020        #     {.  
-0005ec40: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005ec50: 2272 6574 436f 6465 223a 2030 2c0a 2020  "retCode": 0,.  
-0005ec60: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005ec70: 2272 6574 4d73 6722 3a20 224f 4b22 2c0a  "retMsg": "OK",.
-0005ec80: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005ec90: 2020 2272 6573 756c 7422 3a20 7b0a 2020    "result": {.  
-0005eca0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005ecb0: 2020 2020 226c 6973 7422 3a20 5b0a 2020      "list": [.  
-0005ecc0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005ecd0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-0005ece0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005ecf0: 2020 2020 2020 2020 2273 796d 626f 6c22          "symbol"
-0005ed00: 3a20 2245 5448 5553 4454 222c 0a20 2020  : "ETHUSDT",.   
-0005ed10: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0005ed20: 2020 2020 2020 2020 2020 2022 7461 6b65             "take
-0005ed30: 7246 6565 5261 7465 223a 2022 302e 3030  rFeeRate": "0.00
-0005ed40: 3036 222c 0a20 2020 2020 2020 2023 2020  06",.        #  
-0005ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005ed60: 2020 2022 6d61 6b65 7246 6565 5261 7465     "makerFeeRate
-0005ed70: 223a 2022 302e 3030 3031 220a 2020 2020  ": "0.0001".    
-0005ed80: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0005ed90: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0005eda0: 2320 2020 2020 2020 2020 2020 2020 5d0a  #             ].
-0005edb0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0005edc0: 2020 7d2c 0a20 2020 2020 2020 2023 2020    },.        #  
-0005edd0: 2020 2020 2020 2022 7265 7445 7874 496e         "retExtIn
-0005ede0: 666f 223a 207b 7d2c 0a20 2020 2020 2020  fo": {},.       
-0005edf0: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
-0005ee00: 223a 2031 3637 3633 3630 3431 3235 3736  ": 1676360412576
-0005ee10: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
-0005ee20: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0005ee30: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0005ee40: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
-0005ee50: 6f6e 7365 2c20 2772 6573 756c 7427 2c20  onse, 'result', 
-0005ee60: 7b7d 290a 2020 2020 2020 2020 6665 6573  {}).        fees
-0005ee70: 203d 2073 656c 662e 7361 6665 5f76 616c   = self.safe_val
-0005ee80: 7565 2872 6573 756c 742c 2027 6c69 7374  ue(result, 'list
-0005ee90: 272c 205b 5d29 0a20 2020 2020 2020 2066  ', []).        f
-0005eea0: 6972 7374 203d 2073 656c 662e 7361 6665  irst = self.safe
-0005eeb0: 5f76 616c 7565 2866 6565 732c 2030 2c20  _value(fees, 0, 
-0005eec0: 7b7d 290a 2020 2020 2020 2020 7265 7475  {}).        retu
-0005eed0: 726e 2073 656c 662e 7061 7273 655f 7472  rn self.parse_tr
-0005eee0: 6164 696e 675f 6665 6528 6669 7273 7429  ading_fee(first)
-0005eef0: 0a0a 2020 2020 6465 6620 6665 7463 685f  ..    def fetch_
-0005ef00: 7472 6164 696e 675f 6665 6573 2873 656c  trading_fees(sel
-0005ef10: 662c 2070 6172 616d 733d 7b7d 293a 0a20  f, params={}):. 
-0005ef20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0005ef30: 2020 2066 6574 6368 2074 6865 2074 7261     fetch the tra
-0005ef40: 6469 6e67 2066 6565 7320 666f 7220 6d75  ding fees for mu
-0005ef50: 6c74 6970 6c65 206d 6172 6b65 7473 0a20  ltiple markets. 
-0005ef60: 2020 2020 2020 2073 6565 2068 7474 7073         see https
-0005ef70: 3a2f 2f62 7962 6974 2d65 7863 6861 6e67  ://bybit-exchang
-0005ef80: 652e 6769 7468 7562 2e69 6f2f 646f 6373  e.github.io/docs
-0005ef90: 2f76 352f 6163 636f 756e 742f 6665 652d  /v5/account/fee-
-0005efa0: 7261 7465 0a20 2020 2020 2020 203a 7061  rate.        :pa
-0005efb0: 7261 6d20 6469 6374 2070 6172 616d 733a  ram dict params:
-0005efc0: 2065 7874 7261 2070 6172 616d 6574 6572   extra parameter
-0005efd0: 7320 7370 6563 6966 6963 2074 6f20 7468  s specific to th
-0005efe0: 6520 6279 6269 7420 6170 6920 656e 6470  e bybit api endp
-0005eff0: 6f69 6e74 0a20 2020 2020 2020 203a 7265  oint.        :re
-0005f000: 7475 726e 7320 6469 6374 3a20 6120 6469  turns dict: a di
-0005f010: 6374 696f 6e61 7279 206f 6620 6066 6565  ctionary of `fee
-0005f020: 2073 7472 7563 7475 7265 7320 3c68 7474   structures <htt
-0005f030: 7073 3a2f 2f64 6f63 732e 6363 7874 2e63  ps://docs.ccxt.c
-0005f040: 6f6d 2f23 2f3f 6964 3d66 6565 2d73 7472  om/#/?id=fee-str
-0005f050: 7563 7475 7265 3e60 2069 6e64 6578 6564  ucture>` indexed
-0005f060: 2062 7920 6d61 726b 6574 2073 796d 626f   by market symbo
-0005f070: 6c73 0a20 2020 2020 2020 2022 2222 0a20  ls.        """. 
-0005f080: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
-0005f090: 5f6d 6172 6b65 7473 2829 0a20 2020 2020  _markets().     
-0005f0a0: 2020 2074 7970 6520 3d20 4e6f 6e65 0a20     type = None. 
-0005f0b0: 2020 2020 2020 2074 7970 652c 2070 6172         type, par
-0005f0c0: 616d 7320 3d20 7365 6c66 2e68 616e 646c  ams = self.handl
-0005f0d0: 655f 6f70 7469 6f6e 5f61 6e64 5f70 6172  e_option_and_par
-0005f0e0: 616d 7328 7061 7261 6d73 2c20 2766 6574  ams(params, 'fet
-0005f0f0: 6368 5472 6164 696e 6746 6565 7327 2c20  chTradingFees', 
-0005f100: 2774 7970 6527 2c20 2766 7574 7572 6527  'type', 'future'
-0005f110: 290a 2020 2020 2020 2020 6966 2074 7970  ).        if typ
-0005f120: 6520 3d3d 2027 7370 6f74 273a 0a20 2020  e == 'spot':.   
-0005f130: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-0005f140: 6f74 5375 7070 6f72 7465 6428 7365 6c66  otSupported(self
-0005f150: 2e69 6420 2b20 2720 6665 7463 6854 7261  .id + ' fetchTra
-0005f160: 6469 6e67 4665 6573 2829 2069 7320 6e6f  dingFees() is no
-0005f170: 7420 7375 7070 6f72 7465 6420 666f 7220  t supported for 
-0005f180: 7370 6f74 206d 6172 6b65 7427 290a 2020  spot market').  
-0005f190: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0005f1a0: 2073 656c 662e 7072 6976 6174 6547 6574   self.privateGet
-0005f1b0: 5635 4163 636f 756e 7446 6565 5261 7465  V5AccountFeeRate
-0005f1c0: 2870 6172 616d 7329 0a20 2020 2020 2020  (params).       
-0005f1d0: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-0005f1e0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0005f1f0: 2020 2020 2022 7265 7443 6f64 6522 3a20       "retCode": 
-0005f200: 302c 0a20 2020 2020 2020 2023 2020 2020  0,.        #    
-0005f210: 2020 2020 2022 7265 744d 7367 223a 2022       "retMsg": "
-0005f220: 4f4b 222c 0a20 2020 2020 2020 2023 2020  OK",.        #  
-0005f230: 2020 2020 2020 2022 7265 7375 6c74 223a         "result":
-0005f240: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0005f250: 2020 2020 2020 2020 2022 6c69 7374 223a           "list":
-0005f260: 205b 0a20 2020 2020 2020 2023 2020 2020   [.        #    
-0005f270: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-0005f280: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0005f290: 2020 2020 2020 2020 2020 2020 2022 7379               "sy
-0005f2a0: 6d62 6f6c 223a 2022 4554 4855 5344 5422  mbol": "ETHUSDT"
-0005f2b0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0005f2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005f2d0: 2274 616b 6572 4665 6552 6174 6522 3a20  "takerFeeRate": 
-0005f2e0: 2230 2e30 3030 3622 2c0a 2020 2020 2020  "0.0006",.      
-0005f2f0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0005f300: 2020 2020 2020 2020 226d 616b 6572 4665          "makerFe
-0005f310: 6552 6174 6522 3a20 2230 2e30 3030 3122  eRate": "0.0001"
-0005f320: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0005f330: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0005f340: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0005f350: 2020 205d 0a20 2020 2020 2020 2023 2020     ].        #  
-0005f360: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-0005f370: 2020 2320 2020 2020 2020 2020 2272 6574    #         "ret
-0005f380: 4578 7449 6e66 6f22 3a20 7b7d 2c0a 2020  ExtInfo": {},.  
-0005f390: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0005f3a0: 2274 696d 6522 3a20 3136 3736 3336 3034  "time": 16763604
-0005f3b0: 3132 3537 360a 2020 2020 2020 2020 2320  12576.        # 
-0005f3c0: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
-0005f3d0: 2020 2020 2020 2020 6665 6573 203d 2073          fees = s
-0005f3e0: 656c 662e 7361 6665 5f76 616c 7565 2872  elf.safe_value(r
-0005f3f0: 6573 706f 6e73 652c 2027 7265 7375 6c74  esponse, 'result
-0005f400: 272c 207b 7d29 0a20 2020 2020 2020 2066  ', {}).        f
-0005f410: 6565 7320 3d20 7365 6c66 2e73 6166 655f  ees = self.safe_
-0005f420: 7661 6c75 6528 6665 6573 2c20 276c 6973  value(fees, 'lis
-0005f430: 7427 2c20 5b5d 290a 2020 2020 2020 2020  t', []).        
-0005f440: 7265 7375 6c74 203d 207b 7d0a 2020 2020  result = {}.    
-0005f450: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0005f460: 6765 2830 2c20 6c65 6e28 6665 6573 2929  ge(0, len(fees))
-0005f470: 3a0a 2020 2020 2020 2020 2020 2020 6665  :.            fe
-0005f480: 6520 3d20 7365 6c66 2e70 6172 7365 5f74  e = self.parse_t
-0005f490: 7261 6469 6e67 5f66 6565 2866 6565 735b  rading_fee(fees[
-0005f4a0: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-0005f4b0: 7379 6d62 6f6c 203d 2066 6565 5b27 7379  symbol = fee['sy
-0005f4c0: 6d62 6f6c 275d 0a20 2020 2020 2020 2020  mbol'].         
-0005f4d0: 2020 2072 6573 756c 745b 7379 6d62 6f6c     result[symbol
-0005f4e0: 5d20 3d20 6665 650a 2020 2020 2020 2020  ] = fee.        
-0005f4f0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0005f500: 2020 2064 6566 2073 6967 6e28 7365 6c66     def sign(self
-0005f510: 2c20 7061 7468 2c20 6170 693d 2770 7562  , path, api='pub
-0005f520: 6c69 6327 2c20 6d65 7468 6f64 3d27 4745  lic', method='GE
-0005f530: 5427 2c20 7061 7261 6d73 3d7b 7d2c 2068  T', params={}, h
-0005f540: 6561 6465 7273 3d4e 6f6e 652c 2062 6f64  eaders=None, bod
-0005f550: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0005f560: 2075 726c 203d 2073 656c 662e 696d 706c   url = self.impl
-0005f570: 6f64 655f 686f 7374 6e61 6d65 2873 656c  ode_hostname(sel
-0005f580: 662e 7572 6c73 5b27 6170 6927 5d5b 6170  f.urls['api'][ap
-0005f590: 695d 2920 2b20 272f 2720 2b20 7061 7468  i]) + '/' + path
-0005f5a0: 0a20 2020 2020 2020 2069 6620 6170 6920  .        if api 
-0005f5b0: 3d3d 2027 7075 626c 6963 273a 0a20 2020  == 'public':.   
-0005f5c0: 2020 2020 2020 2020 2069 6620 7061 7261           if para
-0005f5d0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-0005f5e0: 2020 2020 7572 6c20 2b3d 2027 3f27 202b      url += '?' +
-0005f5f0: 2073 656c 662e 7261 7765 6e63 6f64 6528   self.rawencode(
-0005f600: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
-0005f610: 656c 6966 2061 7069 203d 3d20 2770 7269  elif api == 'pri
-0005f620: 7661 7465 273a 0a20 2020 2020 2020 2020  vate':.         
-0005f630: 2020 2073 656c 662e 6368 6563 6b5f 7265     self.check_re
-0005f640: 7175 6972 6564 5f63 7265 6465 6e74 6961  quired_credentia
-0005f650: 6c73 2829 0a20 2020 2020 2020 2020 2020  ls().           
-0005f660: 2069 734f 7065 6e61 7069 203d 2075 726c   isOpenapi = url
-0005f670: 2e66 696e 6428 276f 7065 6e61 7069 2729  .find('openapi')
-0005f680: 203e 3d20 300a 2020 2020 2020 2020 2020   >= 0.          
-0005f690: 2020 6973 5633 556e 6966 6965 644d 6172    isV3UnifiedMar
-0005f6a0: 6769 6e20 3d20 7572 6c2e 6669 6e64 2827  gin = url.find('
-0005f6b0: 756e 6966 6965 642f 7633 2729 203e 3d20  unified/v3') >= 
-0005f6c0: 300a 2020 2020 2020 2020 2020 2020 6973  0.            is
-0005f6d0: 5633 436f 6e74 7261 6374 203d 2075 726c  V3Contract = url
-0005f6e0: 2e66 696e 6428 2763 6f6e 7472 6163 742f  .find('contract/
-0005f6f0: 7633 2729 203e 3d20 300a 2020 2020 2020  v3') >= 0.      
-0005f700: 2020 2020 2020 6973 5635 556e 6966 6965        isV5Unifie
-0005f710: 6441 6363 6f75 6e74 203d 2075 726c 2e66  dAccount = url.f
-0005f720: 696e 6428 2776 3527 2920 3e3d 2030 0a20  ind('v5') >= 0. 
-0005f730: 2020 2020 2020 2020 2020 2074 696d 6573             times
-0005f740: 7461 6d70 203d 2073 7472 2873 656c 662e  tamp = str(self.
-0005f750: 6e6f 6e63 6528 2929 0a20 2020 2020 2020  nonce()).       
-0005f760: 2020 2020 2069 6620 6973 4f70 656e 6170       if isOpenap
-0005f770: 693a 0a20 2020 2020 2020 2020 2020 2020  i:.             
-0005f780: 2020 2069 6620 7061 7261 6d73 3a0a 2020     if params:.  
-0005f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005f7a0: 2020 626f 6479 203d 2073 656c 662e 6a73    body = self.js
-0005f7b0: 6f6e 2870 6172 616d 7329 0a20 2020 2020  on(params).     
-0005f7c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0005f7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0005f7e0: 2020 2020 2023 2073 656c 6620 6669 7820       # self fix 
-0005f7f0: 666f 7220 5048 5020 6973 2072 6571 7569  for PHP is requi
-0005f800: 7265 6420 6f74 6865 7277 6973 6520 6974  red otherwise it
-0005f810: 2067 656e 6572 6174 6573 0a20 2020 2020   generates.     
-0005f820: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0005f830: 2027 5b5d 2720 6f6e 2065 6d70 7479 2061   '[]' on empty a
-0005f840: 7272 6179 7320 6576 656e 2077 6865 6e20  rrays even when 
-0005f850: 666f 7263 6564 2074 6f20 7573 6520 6f62  forced to use ob
-0005f860: 6a65 6374 730a 2020 2020 2020 2020 2020  jects.          
-0005f870: 2020 2020 2020 2020 2020 626f 6479 203d            body =
-0005f880: 2027 7b7d 270a 2020 2020 2020 2020 2020   '{}'.          
-0005f890: 2020 2020 2020 7061 796c 6f61 6420 3d20        payload = 
-0005f8a0: 7469 6d65 7374 616d 7020 2b20 7365 6c66  timestamp + self
-0005f8b0: 2e61 7069 4b65 7920 2b20 626f 6479 0a20  .apiKey + body. 
-0005f8c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0005f8d0: 6967 6e61 7475 7265 203d 2073 656c 662e  ignature = self.
-0005f8e0: 686d 6163 2873 656c 662e 656e 636f 6465  hmac(self.encode
-0005f8f0: 2870 6179 6c6f 6164 292c 2073 656c 662e  (payload), self.
-0005f900: 656e 636f 6465 2873 656c 662e 7365 6372  encode(self.secr
-0005f910: 6574 292c 2068 6173 686c 6962 2e73 6861  et), hashlib.sha
-0005f920: 3235 362c 2027 6865 7827 290a 2020 2020  256, 'hex').    
-0005f930: 2020 2020 2020 2020 2020 2020 6865 6164              head
-0005f940: 6572 7320 3d20 7b0a 2020 2020 2020 2020  ers = {.        
-0005f950: 2020 2020 2020 2020 2020 2020 2743 6f6e              'Con
-0005f960: 7465 6e74 2d54 7970 6527 3a20 2761 7070  tent-Type': 'app
-0005f970: 6c69 6361 7469 6f6e 2f6a 736f 6e27 2c0a  lication/json',.
-0005f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005f990: 2020 2020 2758 2d42 4150 492d 4150 492d      'X-BAPI-API-
-0005f9a0: 4b45 5927 3a20 7365 6c66 2e61 7069 4b65  KEY': self.apiKe
-0005f9b0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-0005f9c0: 2020 2020 2020 2027 582d 4241 5049 2d54         'X-BAPI-T
-0005f9d0: 494d 4553 5441 4d50 273a 2074 696d 6573  IMESTAMP': times
-0005f9e0: 7461 6d70 2c0a 2020 2020 2020 2020 2020  tamp,.          
-0005f9f0: 2020 2020 2020 2020 2020 2758 2d42 4150            'X-BAP
-0005fa00: 492d 5349 474e 273a 2073 6967 6e61 7475  I-SIGN': signatu
-0005fa10: 7265 2c0a 2020 2020 2020 2020 2020 2020  re,.            
-0005fa20: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-0005fa30: 2020 656c 6966 2069 7356 3355 6e69 6669    elif isV3Unifi
-0005fa40: 6564 4d61 7267 696e 206f 7220 6973 5633  edMargin or isV3
-0005fa50: 436f 6e74 7261 6374 206f 7220 6973 5635  Contract or isV5
-0005fa60: 556e 6966 6965 6441 6363 6f75 6e74 3a0a  UnifiedAccount:.
-0005fa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005fa80: 6865 6164 6572 7320 3d20 7b0a 2020 2020  headers = {.    
-0005fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005faa0: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
-0005fab0: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
-0005fac0: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-0005fad0: 2020 2020 2020 2020 2758 2d42 4150 492d          'X-BAPI-
-0005fae0: 4150 492d 4b45 5927 3a20 7365 6c66 2e61  API-KEY': self.a
-0005faf0: 7069 4b65 792c 0a20 2020 2020 2020 2020  piKey,.         
-0005fb00: 2020 2020 2020 2020 2020 2027 582d 4241             'X-BA
-0005fb10: 5049 2d54 494d 4553 5441 4d50 273a 2074  PI-TIMESTAMP': t
-0005fb20: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
-0005fb30: 2020 2020 2020 2020 2020 2020 2020 2758                'X
-0005fb40: 2d42 4150 492d 5245 4356 2d57 494e 444f  -BAPI-RECV-WINDO
-0005fb50: 5727 3a20 7374 7228 7365 6c66 2e6f 7074  W': str(self.opt
-0005fb60: 696f 6e73 5b27 7265 6376 5769 6e64 6f77  ions['recvWindow
-0005fb70: 275d 292c 0a20 2020 2020 2020 2020 2020  ']),.           
-0005fb80: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-0005fb90: 2020 2020 2020 2069 6620 6973 5633 556e         if isV3Un
-0005fba0: 6966 6965 644d 6172 6769 6e20 6f72 2069  ifiedMargin or i
-0005fbb0: 7356 3343 6f6e 7472 6163 743a 0a20 2020  sV3Contract:.   
-0005fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005fbd0: 2068 6561 6465 7273 5b27 582d 4241 5049   headers['X-BAPI
-0005fbe0: 2d53 4947 4e2d 5459 5045 275d 203d 2027  -SIGN-TYPE'] = '
-0005fbf0: 3227 0a20 2020 2020 2020 2020 2020 2020  2'.             
-0005fc00: 2020 2071 7565 7279 203d 2073 656c 662e     query = self.
-0005fc10: 6578 7465 6e64 287b 7d2c 2070 6172 616d  extend({}, param
-0005fc20: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-0005fc30: 2020 2071 7565 7279 456e 636f 6465 6420     queryEncoded 
-0005fc40: 3d20 7365 6c66 2e72 6177 656e 636f 6465  = self.rawencode
-0005fc50: 2871 7565 7279 290a 2020 2020 2020 2020  (query).        
-0005fc60: 2020 2020 2020 2020 6175 7468 5f62 6173          auth_bas
-0005fc70: 6520 3d20 7374 7228 7469 6d65 7374 616d  e = str(timestam
-0005fc80: 7029 202b 2073 656c 662e 6170 694b 6579  p) + self.apiKey
-0005fc90: 202b 2073 7472 2873 656c 662e 6f70 7469   + str(self.opti
-0005fca0: 6f6e 735b 2772 6563 7657 696e 646f 7727  ons['recvWindow'
-0005fcb0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0005fcc0: 2020 2061 7574 6846 756c 6c20 3d20 4e6f     authFull = No
-0005fcd0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0005fce0: 2020 2069 6620 6d65 7468 6f64 203d 3d20     if method == 
-0005fcf0: 2750 4f53 5427 3a0a 2020 2020 2020 2020  'POST':.        
-0005fd00: 2020 2020 2020 2020 2020 2020 626f 6479              body
-0005fd10: 203d 2073 656c 662e 6a73 6f6e 2871 7565   = self.json(que
-0005fd20: 7279 290a 2020 2020 2020 2020 2020 2020  ry).            
-0005fd30: 2020 2020 2020 2020 6175 7468 4675 6c6c          authFull
-0005fd40: 203d 2061 7574 685f 6261 7365 202b 2062   = auth_base + b
-0005fd50: 6f64 790a 2020 2020 2020 2020 2020 2020  ody.            
-0005fd60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0005fd70: 2020 2020 2020 2020 2020 2020 2020 6175                au
-0005fd80: 7468 4675 6c6c 203d 2061 7574 685f 6261  thFull = auth_ba
-0005fd90: 7365 202b 2071 7565 7279 456e 636f 6465  se + queryEncode
-0005fda0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0005fdb0: 2020 2020 2020 7572 6c20 2b3d 2027 3f27        url += '?'
-0005fdc0: 202b 2073 656c 662e 7261 7765 6e63 6f64   + self.rawencod
-0005fdd0: 6528 7175 6572 7929 0a20 2020 2020 2020  e(query).       
-0005fde0: 2020 2020 2020 2020 2073 6967 6e61 7475           signatu
-0005fdf0: 7265 203d 204e 6f6e 650a 2020 2020 2020  re = None.      
-0005fe00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0005fe10: 662e 7365 6372 6574 2e66 696e 6428 2750  f.secret.find('P
-0005fe20: 5249 5641 5445 204b 4559 2729 203e 202d  RIVATE KEY') > -
-0005fe30: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-0005fe40: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-0005fe50: 203d 2073 656c 662e 7273 6128 6175 7468   = self.rsa(auth
-0005fe60: 4675 6c6c 2c20 7365 6c66 2e73 6563 7265  Full, self.secre
-0005fe70: 742c 2027 7368 6132 3536 2729 0a20 2020  t, 'sha256').   
-0005fe80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0005fe90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0005fea0: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-0005feb0: 203d 2073 656c 662e 686d 6163 2873 656c   = self.hmac(sel
-0005fec0: 662e 656e 636f 6465 2861 7574 6846 756c  f.encode(authFul
-0005fed0: 6c29 2c20 7365 6c66 2e65 6e63 6f64 6528  l), self.encode(
-0005fee0: 7365 6c66 2e73 6563 7265 7429 2c20 6861  self.secret), ha
-0005fef0: 7368 6c69 622e 7368 6132 3536 290a 2020  shlib.sha256).  
-0005ff00: 2020 2020 2020 2020 2020 2020 2020 6865                he
-0005ff10: 6164 6572 735b 2758 2d42 4150 492d 5349  aders['X-BAPI-SI
-0005ff20: 474e 275d 203d 2073 6967 6e61 7475 7265  GN'] = signature
-0005ff30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0005ff40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0005ff50: 2020 2071 7565 7279 203d 2073 656c 662e     query = self.
-0005ff60: 6578 7465 6e64 2870 6172 616d 732c 207b  extend(params, {
+0005e6c0: 2020 276d 696e 4e6f 7469 6f6e 616c 273a    'minNotional':
+0005e6d0: 206d 696e 4e6f 7469 6f6e 616c 2c0a 2020   minNotional,.  
+0005e6e0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+0005e6f0: 6178 4e6f 7469 6f6e 616c 273a 206d 6178  axNotional': max
+0005e700: 4e6f 7469 6f6e 616c 2c0a 2020 2020 2020  Notional,.      
+0005e710: 2020 2020 2020 2020 2020 276d 6169 6e74            'maint
+0005e720: 656e 616e 6365 4d61 7267 696e 5261 7465  enanceMarginRate
+0005e730: 273a 2073 656c 662e 7361 6665 5f6e 756d  ': self.safe_num
+0005e740: 6265 7228 6974 656d 2c20 276d 6169 6e74  ber(item, 'maint
+0005e750: 656e 616e 6365 4d61 7267 696e 2729 2c0a  enanceMargin'),.
+0005e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005e770: 276d 6178 4c65 7665 7261 6765 273a 2073  'maxLeverage': s
+0005e780: 656c 662e 7361 6665 5f6e 756d 6265 7228  elf.safe_number(
+0005e790: 6974 656d 2c20 276d 6178 4c65 7665 7261  item, 'maxLevera
+0005e7a0: 6765 2729 2c0a 2020 2020 2020 2020 2020  ge'),.          
+0005e7b0: 2020 2020 2020 2769 6e66 6f27 3a20 6974        'info': it
+0005e7c0: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
+0005e7d0: 7d29 0a20 2020 2020 2020 2020 2020 206d  }).            m
+0005e7e0: 696e 4e6f 7469 6f6e 616c 203d 206d 6178  inNotional = max
+0005e7f0: 4e6f 7469 6f6e 616c 0a20 2020 2020 2020  Notional.       
+0005e800: 2072 6574 7572 6e20 7469 6572 730a 0a20   return tiers.. 
+0005e810: 2020 2064 6566 2070 6172 7365 5f74 7261     def parse_tra
+0005e820: 6469 6e67 5f66 6565 2873 656c 662c 2066  ding_fee(self, f
+0005e830: 6565 2c20 6d61 726b 6574 3d4e 6f6e 6529  ee, market=None)
+0005e840: 3a0a 2020 2020 2020 2020 230a 2020 2020  :.        #.    
+0005e850: 2020 2020 2320 2020 2020 7b0a 2020 2020      #     {.    
+0005e860: 2020 2020 2320 2020 2020 2020 2020 2273      #         "s
+0005e870: 796d 626f 6c22 3a20 2245 5448 5553 4454  ymbol": "ETHUSDT
+0005e880: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+0005e890: 2020 2020 2022 6d61 6b65 7246 6565 5261       "makerFeeRa
+0005e8a0: 7465 223a 2030 2e30 3031 2c0a 2020 2020  te": 0.001,.    
+0005e8b0: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
+0005e8c0: 616b 6572 4665 6552 6174 6522 3a20 302e  akerFeeRate": 0.
+0005e8d0: 3030 310a 2020 2020 2020 2020 2320 2020  001.        #   
+0005e8e0: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
+0005e8f0: 2020 2020 2020 6d61 726b 6574 4964 203d        marketId =
+0005e900: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
+0005e910: 6728 6665 652c 2027 7379 6d62 6f6c 2729  g(fee, 'symbol')
+0005e920: 0a20 2020 2020 2020 2073 796d 626f 6c20  .        symbol 
+0005e930: 3d20 7365 6c66 2e73 6166 655f 7379 6d62  = self.safe_symb
+0005e940: 6f6c 286d 6172 6b65 7449 642c 204e 6f6e  ol(marketId, Non
+0005e950: 652c 204e 6f6e 652c 2027 636f 6e74 7261  e, None, 'contra
+0005e960: 6374 2729 0a20 2020 2020 2020 2072 6574  ct').        ret
+0005e970: 7572 6e20 7b0a 2020 2020 2020 2020 2020  urn {.          
+0005e980: 2020 2769 6e66 6f27 3a20 6665 652c 0a20    'info': fee,. 
+0005e990: 2020 2020 2020 2020 2020 2027 7379 6d62             'symb
+0005e9a0: 6f6c 273a 2073 796d 626f 6c2c 0a20 2020  ol': symbol,.   
+0005e9b0: 2020 2020 2020 2020 2027 6d61 6b65 7227           'maker'
+0005e9c0: 3a20 7365 6c66 2e73 6166 655f 6e75 6d62  : self.safe_numb
+0005e9d0: 6572 2866 6565 2c20 276d 616b 6572 4665  er(fee, 'makerFe
+0005e9e0: 6552 6174 6527 292c 0a20 2020 2020 2020  eRate'),.       
+0005e9f0: 2020 2020 2027 7461 6b65 7227 3a20 7365       'taker': se
+0005ea00: 6c66 2e73 6166 655f 6e75 6d62 6572 2866  lf.safe_number(f
+0005ea10: 6565 2c20 2774 616b 6572 4665 6552 6174  ee, 'takerFeeRat
+0005ea20: 6527 292c 0a20 2020 2020 2020 207d 0a0a  e'),.        }..
+0005ea30: 2020 2020 6465 6620 6665 7463 685f 7472      def fetch_tr
+0005ea40: 6164 696e 675f 6665 6528 7365 6c66 2c20  ading_fee(self, 
+0005ea50: 7379 6d62 6f6c 3a20 7374 722c 2070 6172  symbol: str, par
+0005ea60: 616d 733d 7b7d 293a 0a20 2020 2020 2020  ams={}):.       
+0005ea70: 2022 2222 0a20 2020 2020 2020 2066 6574   """.        fet
+0005ea80: 6368 2074 6865 2074 7261 6469 6e67 2066  ch the trading f
+0005ea90: 6565 7320 666f 7220 6120 6d61 726b 6574  ees for a market
+0005eaa0: 0a20 2020 2020 2020 2073 6565 2068 7474  .        see htt
+0005eab0: 7073 3a2f 2f62 7962 6974 2d65 7863 6861  ps://bybit-excha
+0005eac0: 6e67 652e 6769 7468 7562 2e69 6f2f 646f  nge.github.io/do
+0005ead0: 6373 2f76 352f 6163 636f 756e 742f 6665  cs/v5/account/fe
+0005eae0: 652d 7261 7465 0a20 2020 2020 2020 203a  e-rate.        :
+0005eaf0: 7061 7261 6d20 7374 7220 7379 6d62 6f6c  param str symbol
+0005eb00: 3a20 756e 6966 6965 6420 6d61 726b 6574  : unified market
+0005eb10: 2073 796d 626f 6c0a 2020 2020 2020 2020   symbol.        
+0005eb20: 3a70 6172 616d 2064 6963 7420 7061 7261  :param dict para
+0005eb30: 6d73 3a20 6578 7472 6120 7061 7261 6d65  ms: extra parame
+0005eb40: 7465 7273 2073 7065 6369 6669 6320 746f  ters specific to
+0005eb50: 2074 6865 2062 7962 6974 2061 7069 2065   the bybit api e
+0005eb60: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
+0005eb70: 3a72 6574 7572 6e73 2064 6963 743a 2061  :returns dict: a
+0005eb80: 2060 6665 6520 7374 7275 6374 7572 6520   `fee structure 
+0005eb90: 3c68 7474 7073 3a2f 2f64 6f63 732e 6363  <https://docs.cc
+0005eba0: 7874 2e63 6f6d 2f23 2f3f 6964 3d66 6565  xt.com/#/?id=fee
+0005ebb0: 2d73 7472 7563 7475 7265 3e60 0a20 2020  -structure>`.   
+0005ebc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0005ebd0: 2073 656c 662e 6c6f 6164 5f6d 6172 6b65   self.load_marke
+0005ebe0: 7473 2829 0a20 2020 2020 2020 206d 6172  ts().        mar
+0005ebf0: 6b65 7420 3d20 7365 6c66 2e6d 6172 6b65  ket = self.marke
+0005ec00: 7428 7379 6d62 6f6c 290a 2020 2020 2020  t(symbol).      
+0005ec10: 2020 6966 206d 6172 6b65 745b 2773 706f    if market['spo
+0005ec20: 7427 5d3a 0a20 2020 2020 2020 2020 2020  t']:.           
+0005ec30: 2072 6169 7365 204e 6f74 5375 7070 6f72   raise NotSuppor
+0005ec40: 7465 6428 7365 6c66 2e69 6420 2b20 2720  ted(self.id + ' 
+0005ec50: 6665 7463 6854 7261 6469 6e67 4665 6528  fetchTradingFee(
+0005ec60: 2920 6973 206e 6f74 2073 7570 706f 7274  ) is not support
+0005ec70: 6564 2066 6f72 2073 706f 7420 6d61 726b  ed for spot mark
+0005ec80: 6574 2729 0a20 2020 2020 2020 2072 6571  et').        req
+0005ec90: 7565 7374 203d 207b 0a20 2020 2020 2020  uest = {.       
+0005eca0: 2020 2020 2027 7379 6d62 6f6c 273a 206d       'symbol': m
+0005ecb0: 6172 6b65 745b 2769 6427 5d2c 0a20 2020  arket['id'],.   
+0005ecc0: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+0005ecd0: 6573 706f 6e73 6520 3d20 7365 6c66 2e70  esponse = self.p
+0005ece0: 7269 7661 7465 4765 7456 3541 6363 6f75  rivateGetV5Accou
+0005ecf0: 6e74 4665 6552 6174 6528 7365 6c66 2e65  ntFeeRate(self.e
+0005ed00: 7874 656e 6428 7265 7175 6573 742c 2070  xtend(request, p
+0005ed10: 6172 616d 7329 290a 2020 2020 2020 2020  arams)).        
+0005ed20: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
+0005ed30: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+0005ed40: 2020 2020 2272 6574 436f 6465 223a 2030      "retCode": 0
+0005ed50: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005ed60: 2020 2020 2272 6574 4d73 6722 3a20 224f      "retMsg": "O
+0005ed70: 4b22 2c0a 2020 2020 2020 2020 2320 2020  K",.        #   
+0005ed80: 2020 2020 2020 2272 6573 756c 7422 3a20        "result": 
+0005ed90: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+0005eda0: 2020 2020 2020 2020 226c 6973 7422 3a20          "list": 
+0005edb0: 5b0a 2020 2020 2020 2020 2320 2020 2020  [.        #     
+0005edc0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+0005edd0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005ede0: 2020 2020 2020 2020 2020 2020 2273 796d              "sym
+0005edf0: 626f 6c22 3a20 2245 5448 5553 4454 222c  bol": "ETHUSDT",
+0005ee00: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005ee10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0005ee20: 7461 6b65 7246 6565 5261 7465 223a 2022  takerFeeRate": "
+0005ee30: 302e 3030 3036 222c 0a20 2020 2020 2020  0.0006",.       
+0005ee40: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0005ee50: 2020 2020 2020 2022 6d61 6b65 7246 6565         "makerFee
+0005ee60: 5261 7465 223a 2022 302e 3030 3031 220a  Rate": "0.0001".
+0005ee70: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0005ee80: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+0005ee90: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0005eea0: 2020 5d0a 2020 2020 2020 2020 2320 2020    ].        #   
+0005eeb0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0005eec0: 2023 2020 2020 2020 2020 2022 7265 7445   #         "retE
+0005eed0: 7874 496e 666f 223a 207b 7d2c 0a20 2020  xtInfo": {},.   
+0005eee0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+0005eef0: 7469 6d65 223a 2031 3637 3633 3630 3431  time": 167636041
+0005ef00: 3235 3736 0a20 2020 2020 2020 2023 2020  2576.        #  
+0005ef10: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
+0005ef20: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0005ef30: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
+0005ef40: 7265 7370 6f6e 7365 2c20 2772 6573 756c  response, 'resul
+0005ef50: 7427 2c20 7b7d 290a 2020 2020 2020 2020  t', {}).        
+0005ef60: 6665 6573 203d 2073 656c 662e 7361 6665  fees = self.safe
+0005ef70: 5f76 616c 7565 2872 6573 756c 742c 2027  _value(result, '
+0005ef80: 6c69 7374 272c 205b 5d29 0a20 2020 2020  list', []).     
+0005ef90: 2020 2066 6972 7374 203d 2073 656c 662e     first = self.
+0005efa0: 7361 6665 5f76 616c 7565 2866 6565 732c  safe_value(fees,
+0005efb0: 2030 2c20 7b7d 290a 2020 2020 2020 2020   0, {}).        
+0005efc0: 7265 7475 726e 2073 656c 662e 7061 7273  return self.pars
+0005efd0: 655f 7472 6164 696e 675f 6665 6528 6669  e_trading_fee(fi
+0005efe0: 7273 7429 0a0a 2020 2020 6465 6620 6665  rst)..    def fe
+0005eff0: 7463 685f 7472 6164 696e 675f 6665 6573  tch_trading_fees
+0005f000: 2873 656c 662c 2070 6172 616d 733d 7b7d  (self, params={}
+0005f010: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0005f020: 2020 2020 2020 2066 6574 6368 2074 6865         fetch the
+0005f030: 2074 7261 6469 6e67 2066 6565 7320 666f   trading fees fo
+0005f040: 7220 6d75 6c74 6970 6c65 206d 6172 6b65  r multiple marke
+0005f050: 7473 0a20 2020 2020 2020 2073 6565 2068  ts.        see h
+0005f060: 7474 7073 3a2f 2f62 7962 6974 2d65 7863  ttps://bybit-exc
+0005f070: 6861 6e67 652e 6769 7468 7562 2e69 6f2f  hange.github.io/
+0005f080: 646f 6373 2f76 352f 6163 636f 756e 742f  docs/v5/account/
+0005f090: 6665 652d 7261 7465 0a20 2020 2020 2020  fee-rate.       
+0005f0a0: 203a 7061 7261 6d20 6469 6374 2070 6172   :param dict par
+0005f0b0: 616d 733a 2065 7874 7261 2070 6172 616d  ams: extra param
+0005f0c0: 6574 6572 7320 7370 6563 6966 6963 2074  eters specific t
+0005f0d0: 6f20 7468 6520 6279 6269 7420 6170 6920  o the bybit api 
+0005f0e0: 656e 6470 6f69 6e74 0a20 2020 2020 2020  endpoint.       
+0005f0f0: 203a 7265 7475 726e 7320 6469 6374 3a20   :returns dict: 
+0005f100: 6120 6469 6374 696f 6e61 7279 206f 6620  a dictionary of 
+0005f110: 6066 6565 2073 7472 7563 7475 7265 7320  `fee structures 
+0005f120: 3c68 7474 7073 3a2f 2f64 6f63 732e 6363  <https://docs.cc
+0005f130: 7874 2e63 6f6d 2f23 2f3f 6964 3d66 6565  xt.com/#/?id=fee
+0005f140: 2d73 7472 7563 7475 7265 3e60 2069 6e64  -structure>` ind
+0005f150: 6578 6564 2062 7920 6d61 726b 6574 2073  exed by market s
+0005f160: 796d 626f 6c73 0a20 2020 2020 2020 2022  ymbols.        "
+0005f170: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+0005f180: 6c6f 6164 5f6d 6172 6b65 7473 2829 0a20  load_markets(). 
+0005f190: 2020 2020 2020 2074 7970 6520 3d20 4e6f         type = No
+0005f1a0: 6e65 0a20 2020 2020 2020 2074 7970 652c  ne.        type,
+0005f1b0: 2070 6172 616d 7320 3d20 7365 6c66 2e68   params = self.h
+0005f1c0: 616e 646c 655f 6f70 7469 6f6e 5f61 6e64  andle_option_and
+0005f1d0: 5f70 6172 616d 7328 7061 7261 6d73 2c20  _params(params, 
+0005f1e0: 2766 6574 6368 5472 6164 696e 6746 6565  'fetchTradingFee
+0005f1f0: 7327 2c20 2774 7970 6527 2c20 2766 7574  s', 'type', 'fut
+0005f200: 7572 6527 290a 2020 2020 2020 2020 6966  ure').        if
+0005f210: 2074 7970 6520 3d3d 2027 7370 6f74 273a   type == 'spot':
+0005f220: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0005f230: 7365 204e 6f74 5375 7070 6f72 7465 6428  se NotSupported(
+0005f240: 7365 6c66 2e69 6420 2b20 2720 6665 7463  self.id + ' fetc
+0005f250: 6854 7261 6469 6e67 4665 6573 2829 2069  hTradingFees() i
+0005f260: 7320 6e6f 7420 7375 7070 6f72 7465 6420  s not supported 
+0005f270: 666f 7220 7370 6f74 206d 6172 6b65 7427  for spot market'
+0005f280: 290a 2020 2020 2020 2020 7265 7370 6f6e  ).        respon
+0005f290: 7365 203d 2073 656c 662e 7072 6976 6174  se = self.privat
+0005f2a0: 6547 6574 5635 4163 636f 756e 7446 6565  eGetV5AccountFee
+0005f2b0: 5261 7465 2870 6172 616d 7329 0a20 2020  Rate(params).   
+0005f2c0: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+0005f2d0: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
+0005f2e0: 2020 2020 2020 2020 2022 7265 7443 6f64           "retCod
+0005f2f0: 6522 3a20 302c 0a20 2020 2020 2020 2023  e": 0,.        #
+0005f300: 2020 2020 2020 2020 2022 7265 744d 7367           "retMsg
+0005f310: 223a 2022 4f4b 222c 0a20 2020 2020 2020  ": "OK",.       
+0005f320: 2023 2020 2020 2020 2020 2022 7265 7375   #         "resu
+0005f330: 6c74 223a 207b 0a20 2020 2020 2020 2023  lt": {.        #
+0005f340: 2020 2020 2020 2020 2020 2020 2022 6c69               "li
+0005f350: 7374 223a 205b 0a20 2020 2020 2020 2023  st": [.        #
+0005f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005f370: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
+0005f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005f390: 2022 7379 6d62 6f6c 223a 2022 4554 4855   "symbol": "ETHU
+0005f3a0: 5344 5422 2c0a 2020 2020 2020 2020 2320  SDT",.        # 
+0005f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005f3c0: 2020 2020 2274 616b 6572 4665 6552 6174      "takerFeeRat
+0005f3d0: 6522 3a20 2230 2e30 3030 3622 2c0a 2020  e": "0.0006",.  
+0005f3e0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005f3f0: 2020 2020 2020 2020 2020 2020 226d 616b              "mak
+0005f400: 6572 4665 6552 6174 6522 3a20 2230 2e30  erFeeRate": "0.0
+0005f410: 3030 3122 0a20 2020 2020 2020 2023 2020  001".        #  
+0005f420: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0005f430: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0005f440: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+0005f450: 2023 2020 2020 2020 2020 207d 2c0a 2020   #         },.  
+0005f460: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0005f470: 2272 6574 4578 7449 6e66 6f22 3a20 7b7d  "retExtInfo": {}
+0005f480: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0005f490: 2020 2020 2274 696d 6522 3a20 3136 3736      "time": 1676
+0005f4a0: 3336 3034 3132 3537 360a 2020 2020 2020  360412576.      
+0005f4b0: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
+0005f4c0: 2020 230a 2020 2020 2020 2020 6665 6573    #.        fees
+0005f4d0: 203d 2073 656c 662e 7361 6665 5f76 616c   = self.safe_val
+0005f4e0: 7565 2872 6573 706f 6e73 652c 2027 7265  ue(response, 're
+0005f4f0: 7375 6c74 272c 207b 7d29 0a20 2020 2020  sult', {}).     
+0005f500: 2020 2066 6565 7320 3d20 7365 6c66 2e73     fees = self.s
+0005f510: 6166 655f 7661 6c75 6528 6665 6573 2c20  afe_value(fees, 
+0005f520: 276c 6973 7427 2c20 5b5d 290a 2020 2020  'list', []).    
+0005f530: 2020 2020 7265 7375 6c74 203d 207b 7d0a      result = {}.
+0005f540: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0005f550: 2072 616e 6765 2830 2c20 6c65 6e28 6665   range(0, len(fe
+0005f560: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+0005f570: 2020 6665 6520 3d20 7365 6c66 2e70 6172    fee = self.par
+0005f580: 7365 5f74 7261 6469 6e67 5f66 6565 2866  se_trading_fee(f
+0005f590: 6565 735b 695d 290a 2020 2020 2020 2020  ees[i]).        
+0005f5a0: 2020 2020 7379 6d62 6f6c 203d 2066 6565      symbol = fee
+0005f5b0: 5b27 7379 6d62 6f6c 275d 0a20 2020 2020  ['symbol'].     
+0005f5c0: 2020 2020 2020 2072 6573 756c 745b 7379         result[sy
+0005f5d0: 6d62 6f6c 5d20 3d20 6665 650a 2020 2020  mbol] = fee.    
+0005f5e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0005f5f0: 740a 0a20 2020 2064 6566 2073 6967 6e28  t..    def sign(
+0005f600: 7365 6c66 2c20 7061 7468 2c20 6170 693d  self, path, api=
+0005f610: 2770 7562 6c69 6327 2c20 6d65 7468 6f64  'public', method
+0005f620: 3d27 4745 5427 2c20 7061 7261 6d73 3d7b  ='GET', params={
+0005f630: 7d2c 2068 6561 6465 7273 3d4e 6f6e 652c  }, headers=None,
+0005f640: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+0005f650: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
+0005f660: 696d 706c 6f64 655f 686f 7374 6e61 6d65  implode_hostname
+0005f670: 2873 656c 662e 7572 6c73 5b27 6170 6927  (self.urls['api'
+0005f680: 5d5b 6170 695d 2920 2b20 272f 2720 2b20  ][api]) + '/' + 
+0005f690: 7061 7468 0a20 2020 2020 2020 2069 6620  path.        if 
+0005f6a0: 6170 6920 3d3d 2027 7075 626c 6963 273a  api == 'public':
+0005f6b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0005f6c0: 7061 7261 6d73 3a0a 2020 2020 2020 2020  params:.        
+0005f6d0: 2020 2020 2020 2020 7572 6c20 2b3d 2027          url += '
+0005f6e0: 3f27 202b 2073 656c 662e 7261 7765 6e63  ?' + self.rawenc
+0005f6f0: 6f64 6528 7061 7261 6d73 290a 2020 2020  ode(params).    
+0005f700: 2020 2020 656c 6966 2061 7069 203d 3d20      elif api == 
+0005f710: 2770 7269 7661 7465 273a 0a20 2020 2020  'private':.     
+0005f720: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+0005f730: 6b5f 7265 7175 6972 6564 5f63 7265 6465  k_required_crede
+0005f740: 6e74 6961 6c73 2829 0a20 2020 2020 2020  ntials().       
+0005f750: 2020 2020 2069 734f 7065 6e61 7069 203d       isOpenapi =
+0005f760: 2075 726c 2e66 696e 6428 276f 7065 6e61   url.find('opena
+0005f770: 7069 2729 203e 3d20 300a 2020 2020 2020  pi') >= 0.      
+0005f780: 2020 2020 2020 6973 5633 556e 6966 6965        isV3Unifie
+0005f790: 644d 6172 6769 6e20 3d20 7572 6c2e 6669  dMargin = url.fi
+0005f7a0: 6e64 2827 756e 6966 6965 642f 7633 2729  nd('unified/v3')
+0005f7b0: 203e 3d20 300a 2020 2020 2020 2020 2020   >= 0.          
+0005f7c0: 2020 6973 5633 436f 6e74 7261 6374 203d    isV3Contract =
+0005f7d0: 2075 726c 2e66 696e 6428 2763 6f6e 7472   url.find('contr
+0005f7e0: 6163 742f 7633 2729 203e 3d20 300a 2020  act/v3') >= 0.  
+0005f7f0: 2020 2020 2020 2020 2020 6973 5635 556e            isV5Un
+0005f800: 6966 6965 6441 6363 6f75 6e74 203d 2075  ifiedAccount = u
+0005f810: 726c 2e66 696e 6428 2776 3527 2920 3e3d  rl.find('v5') >=
+0005f820: 2030 0a20 2020 2020 2020 2020 2020 2074   0.            t
+0005f830: 696d 6573 7461 6d70 203d 2073 7472 2873  imestamp = str(s
+0005f840: 656c 662e 6e6f 6e63 6528 2929 0a20 2020  elf.nonce()).   
+0005f850: 2020 2020 2020 2020 2069 6620 6973 4f70           if isOp
+0005f860: 656e 6170 693a 0a20 2020 2020 2020 2020  enapi:.         
+0005f870: 2020 2020 2020 2069 6620 7061 7261 6d73         if params
+0005f880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0005f890: 2020 2020 2020 626f 6479 203d 2073 656c        body = sel
+0005f8a0: 662e 6a73 6f6e 2870 6172 616d 7329 0a20  f.json(params). 
+0005f8b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0005f8c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0005f8d0: 2020 2020 2020 2020 2023 2073 656c 6620           # self 
+0005f8e0: 6669 7820 666f 7220 5048 5020 6973 2072  fix for PHP is r
+0005f8f0: 6571 7569 7265 6420 6f74 6865 7277 6973  equired otherwis
+0005f900: 6520 6974 2067 656e 6572 6174 6573 0a20  e it generates. 
+0005f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005f920: 2020 2023 2027 5b5d 2720 6f6e 2065 6d70     # '[]' on emp
+0005f930: 7479 2061 7272 6179 7320 6576 656e 2077  ty arrays even w
+0005f940: 6865 6e20 666f 7263 6564 2074 6f20 7573  hen forced to us
+0005f950: 6520 6f62 6a65 6374 730a 2020 2020 2020  e objects.      
+0005f960: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0005f970: 6479 203d 2027 7b7d 270a 2020 2020 2020  dy = '{}'.      
+0005f980: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
+0005f990: 6420 3d20 7469 6d65 7374 616d 7020 2b20  d = timestamp + 
+0005f9a0: 7365 6c66 2e61 7069 4b65 7920 2b20 626f  self.apiKey + bo
+0005f9b0: 6479 0a20 2020 2020 2020 2020 2020 2020  dy.             
+0005f9c0: 2020 2073 6967 6e61 7475 7265 203d 2073     signature = s
+0005f9d0: 656c 662e 686d 6163 2873 656c 662e 656e  elf.hmac(self.en
+0005f9e0: 636f 6465 2870 6179 6c6f 6164 292c 2073  code(payload), s
+0005f9f0: 656c 662e 656e 636f 6465 2873 656c 662e  elf.encode(self.
+0005fa00: 7365 6372 6574 292c 2068 6173 686c 6962  secret), hashlib
+0005fa10: 2e73 6861 3235 362c 2027 6865 7827 290a  .sha256, 'hex').
+0005fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fa30: 6865 6164 6572 7320 3d20 7b0a 2020 2020  headers = {.    
+0005fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fa50: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
+0005fa60: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
+0005fa70: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
+0005fa80: 2020 2020 2020 2020 2758 2d42 4150 492d          'X-BAPI-
+0005fa90: 4150 492d 4b45 5927 3a20 7365 6c66 2e61  API-KEY': self.a
+0005faa0: 7069 4b65 792c 0a20 2020 2020 2020 2020  piKey,.         
+0005fab0: 2020 2020 2020 2020 2020 2027 582d 4241             'X-BA
+0005fac0: 5049 2d54 494d 4553 5441 4d50 273a 2074  PI-TIMESTAMP': t
+0005fad0: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
+0005fae0: 2020 2020 2020 2020 2020 2020 2020 2758                'X
+0005faf0: 2d42 4150 492d 5349 474e 273a 2073 6967  -BAPI-SIGN': sig
+0005fb00: 6e61 7475 7265 2c0a 2020 2020 2020 2020  nature,.        
+0005fb10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0005fb20: 2020 2020 2020 656c 6966 2069 7356 3355        elif isV3U
+0005fb30: 6e69 6669 6564 4d61 7267 696e 206f 7220  nifiedMargin or 
+0005fb40: 6973 5633 436f 6e74 7261 6374 206f 7220  isV3Contract or 
+0005fb50: 6973 5635 556e 6966 6965 6441 6363 6f75  isV5UnifiedAccou
+0005fb60: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+0005fb70: 2020 2020 6865 6164 6572 7320 3d20 7b0a      headers = {.
+0005fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fb90: 2020 2020 2743 6f6e 7465 6e74 2d54 7970      'Content-Typ
+0005fba0: 6527 3a20 2761 7070 6c69 6361 7469 6f6e  e': 'application
+0005fbb0: 2f6a 736f 6e27 2c0a 2020 2020 2020 2020  /json',.        
+0005fbc0: 2020 2020 2020 2020 2020 2020 2758 2d42              'X-B
+0005fbd0: 4150 492d 4150 492d 4b45 5927 3a20 7365  API-API-KEY': se
+0005fbe0: 6c66 2e61 7069 4b65 792c 0a20 2020 2020  lf.apiKey,.     
+0005fbf0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0005fc00: 582d 4241 5049 2d54 494d 4553 5441 4d50  X-BAPI-TIMESTAMP
+0005fc10: 273a 2074 696d 6573 7461 6d70 2c0a 2020  ': timestamp,.  
+0005fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fc30: 2020 2758 2d42 4150 492d 5245 4356 2d57    'X-BAPI-RECV-W
+0005fc40: 494e 444f 5727 3a20 7374 7228 7365 6c66  INDOW': str(self
+0005fc50: 2e6f 7074 696f 6e73 5b27 7265 6376 5769  .options['recvWi
+0005fc60: 6e64 6f77 275d 292c 0a20 2020 2020 2020  ndow']),.       
+0005fc70: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+0005fc80: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0005fc90: 5633 556e 6966 6965 644d 6172 6769 6e20  V3UnifiedMargin 
+0005fca0: 6f72 2069 7356 3343 6f6e 7472 6163 743a  or isV3Contract:
+0005fcb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0005fcc0: 2020 2020 2068 6561 6465 7273 5b27 582d       headers['X-
+0005fcd0: 4241 5049 2d53 4947 4e2d 5459 5045 275d  BAPI-SIGN-TYPE']
+0005fce0: 203d 2027 3227 0a20 2020 2020 2020 2020   = '2'.         
+0005fcf0: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
+0005fd00: 656c 662e 6578 7465 6e64 287b 7d2c 2070  elf.extend({}, p
+0005fd10: 6172 616d 7329 0a20 2020 2020 2020 2020  arams).         
+0005fd20: 2020 2020 2020 2071 7565 7279 456e 636f         queryEnco
+0005fd30: 6465 6420 3d20 7365 6c66 2e72 6177 656e  ded = self.rawen
+0005fd40: 636f 6465 2871 7565 7279 290a 2020 2020  code(query).    
+0005fd50: 2020 2020 2020 2020 2020 2020 6175 7468              auth
+0005fd60: 5f62 6173 6520 3d20 7374 7228 7469 6d65  _base = str(time
+0005fd70: 7374 616d 7029 202b 2073 656c 662e 6170  stamp) + self.ap
+0005fd80: 694b 6579 202b 2073 7472 2873 656c 662e  iKey + str(self.
+0005fd90: 6f70 7469 6f6e 735b 2772 6563 7657 696e  options['recvWin
+0005fda0: 646f 7727 5d29 0a20 2020 2020 2020 2020  dow']).         
+0005fdb0: 2020 2020 2020 2061 7574 6846 756c 6c20         authFull 
+0005fdc0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0005fdd0: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+0005fde0: 203d 3d20 2750 4f53 5427 3a0a 2020 2020   == 'POST':.    
+0005fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fe00: 626f 6479 203d 2073 656c 662e 6a73 6f6e  body = self.json
+0005fe10: 2871 7565 7279 290a 2020 2020 2020 2020  (query).        
+0005fe20: 2020 2020 2020 2020 2020 2020 6175 7468              auth
+0005fe30: 4675 6c6c 203d 2061 7574 685f 6261 7365  Full = auth_base
+0005fe40: 202b 2062 6f64 790a 2020 2020 2020 2020   + body.        
+0005fe50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0005fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0005fe70: 2020 6175 7468 4675 6c6c 203d 2061 7574    authFull = aut
+0005fe80: 685f 6261 7365 202b 2071 7565 7279 456e  h_base + queryEn
+0005fe90: 636f 6465 640a 2020 2020 2020 2020 2020  coded.          
+0005fea0: 2020 2020 2020 2020 2020 7572 6c20 2b3d            url +=
+0005feb0: 2027 3f27 202b 2073 656c 662e 7261 7765   '?' + self.rawe
+0005fec0: 6e63 6f64 6528 7175 6572 7929 0a20 2020  ncode(query).   
+0005fed0: 2020 2020 2020 2020 2020 2020 2073 6967               sig
+0005fee0: 6e61 7475 7265 203d 204e 6f6e 650a 2020  nature = None.  
+0005fef0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0005ff00: 2073 656c 662e 7365 6372 6574 2e66 696e   self.secret.fin
+0005ff10: 6428 2750 5249 5641 5445 204b 4559 2729  d('PRIVATE KEY')
+0005ff20: 203e 202d 313a 0a20 2020 2020 2020 2020   > -1:.         
+0005ff30: 2020 2020 2020 2020 2020 2073 6967 6e61             signa
+0005ff40: 7475 7265 203d 2073 656c 662e 7273 6128  ture = self.rsa(
+0005ff50: 6175 7468 4675 6c6c 2c20 7365 6c66 2e73  authFull, self.s
+0005ff60: 6563 7265 742c 2027 7368 6132 3536 2729  ecret, 'sha256')
 0005ff70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0005ff80: 2020 2020 2027 6170 695f 6b65 7927 3a20       'api_key': 
-0005ff90: 7365 6c66 2e61 7069 4b65 792c 0a20 2020  self.apiKey,.   
-0005ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005ffb0: 2027 7265 6376 5f77 696e 646f 7727 3a20   'recv_window': 
-0005ffc0: 7365 6c66 2e6f 7074 696f 6e73 5b27 7265  self.options['re
-0005ffd0: 6376 5769 6e64 6f77 275d 2c0a 2020 2020  cvWindow'],.    
-0005ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0005fff0: 2774 696d 6573 7461 6d70 273a 2074 696d  'timestamp': tim
-00060000: 6573 7461 6d70 2c0a 2020 2020 2020 2020  estamp,.        
-00060010: 2020 2020 2020 2020 7d29 0a20 2020 2020          }).     
-00060020: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00060030: 6451 7565 7279 203d 2073 656c 662e 6b65  dQuery = self.ke
-00060040: 7973 6f72 7428 7175 6572 7929 0a20 2020  ysort(query).   
-00060050: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-00060060: 6820 3d20 7365 6c66 2e72 6177 656e 636f  h = self.rawenco
-00060070: 6465 2873 6f72 7465 6451 7565 7279 290a  de(sortedQuery).
-00060080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060090: 7369 676e 6174 7572 6520 3d20 4e6f 6e65  signature = None
-000600a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000600b0: 2069 6620 7365 6c66 2e73 6563 7265 742e   if self.secret.
-000600c0: 6669 6e64 2827 5052 4956 4154 4520 4b45  find('PRIVATE KE
-000600d0: 5927 2920 3e20 2d31 3a0a 2020 2020 2020  Y') > -1:.      
-000600e0: 2020 2020 2020 2020 2020 2020 2020 7369                si
-000600f0: 676e 6174 7572 6520 3d20 7365 6c66 2e72  gnature = self.r
-00060100: 7361 2861 7574 682c 2073 656c 662e 7365  sa(auth, self.se
-00060110: 6372 6574 2c20 2773 6861 3235 3627 290a  cret, 'sha256').
-00060120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060130: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00060140: 2020 2020 2020 2020 2020 7369 676e 6174            signat
-00060150: 7572 6520 3d20 7365 6c66 2e68 6d61 6328  ure = self.hmac(
-00060160: 7365 6c66 2e65 6e63 6f64 6528 6175 7468  self.encode(auth
-00060170: 292c 2073 656c 662e 656e 636f 6465 2873  ), self.encode(s
-00060180: 656c 662e 7365 6372 6574 292c 2068 6173  elf.secret), has
-00060190: 686c 6962 2e73 6861 3235 3629 0a20 2020  hlib.sha256).   
-000601a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000601b0: 6d65 7468 6f64 203d 3d20 2750 4f53 5427  method == 'POST'
-000601c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000601d0: 2020 2020 2020 6973 5370 6f74 203d 2075        isSpot = u
-000601e0: 726c 2e66 696e 6428 2773 706f 7427 2920  rl.find('spot') 
-000601f0: 3e3d 2030 0a20 2020 2020 2020 2020 2020  >= 0.           
-00060200: 2020 2020 2020 2020 2065 7874 656e 6465           extende
-00060210: 6451 7565 7279 203d 2073 656c 662e 6578  dQuery = self.ex
-00060220: 7465 6e64 2871 7565 7279 2c20 7b0a 2020  tend(query, {.  
-00060230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060240: 2020 2020 2020 2773 6967 6e27 3a20 7369        'sign': si
-00060250: 676e 6174 7572 652c 0a20 2020 2020 2020  gnature,.       
-00060260: 2020 2020 2020 2020 2020 2020 207d 290a               }).
-00060270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060280: 2020 2020 6966 2069 7353 706f 743a 0a20      if isSpot:. 
-00060290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000602a0: 2020 2020 2020 2062 6f64 7920 3d20 7365         body = se
-000602b0: 6c66 2e75 726c 656e 636f 6465 2865 7874  lf.urlencode(ext
-000602c0: 656e 6465 6451 7565 7279 290a 2020 2020  endedQuery).    
-000602d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000602e0: 2020 2020 6865 6164 6572 7320 3d20 7b0a      headers = {.
-000602f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060300: 2020 2020 2020 2020 2020 2020 2743 6f6e              'Con
-00060310: 7465 6e74 2d54 7970 6527 3a20 2761 7070  tent-Type': 'app
-00060320: 6c69 6361 7469 6f6e 2f78 2d77 7777 2d66  lication/x-www-f
-00060330: 6f72 6d2d 7572 6c65 6e63 6f64 6564 272c  orm-urlencoded',
-00060340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060350: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00060360: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00060370: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00060380: 2020 2020 2020 2020 2020 2020 2062 6f64               bod
-00060390: 7920 3d20 7365 6c66 2e6a 736f 6e28 6578  y = self.json(ex
-000603a0: 7465 6e64 6564 5175 6572 7929 0a20 2020  tendedQuery).   
-000603b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000603c0: 2020 2020 2068 6561 6465 7273 203d 207b       headers = {
-000603d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000603e0: 2020 2020 2020 2020 2020 2020 2027 436f               'Co
-000603f0: 6e74 656e 742d 5479 7065 273a 2027 6170  ntent-Type': 'ap
-00060400: 706c 6963 6174 696f 6e2f 6a73 6f6e 272c  plication/json',
-00060410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060420: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00060430: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00060440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00060450: 2020 2020 2075 726c 202b 3d20 273f 2720       url += '?' 
-00060460: 2b20 7365 6c66 2e72 6177 656e 636f 6465  + self.rawencode
-00060470: 2873 6f72 7465 6451 7565 7279 290a 2020  (sortedQuery).  
-00060480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060490: 2020 7572 6c20 2b3d 2027 2673 6967 6e3d    url += '&sign=
-000604a0: 2720 2b20 7369 676e 6174 7572 650a 2020  ' + signature.  
-000604b0: 2020 2020 2020 6966 206d 6574 686f 6420        if method 
-000604c0: 3d3d 2027 504f 5354 273a 0a20 2020 2020  == 'POST':.     
-000604d0: 2020 2020 2020 2062 726f 6b65 7249 6420         brokerId 
-000604e0: 3d20 7365 6c66 2e73 6166 655f 7374 7269  = self.safe_stri
-000604f0: 6e67 2873 656c 662e 6f70 7469 6f6e 732c  ng(self.options,
-00060500: 2027 6272 6f6b 6572 4964 2729 0a20 2020   'brokerId').   
-00060510: 2020 2020 2020 2020 2069 6620 6272 6f6b           if brok
-00060520: 6572 4964 2069 7320 6e6f 7420 4e6f 6e65  erId is not None
-00060530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00060540: 2020 6865 6164 6572 735b 2752 6566 6572    headers['Refer
-00060550: 6572 275d 203d 2062 726f 6b65 7249 640a  er'] = brokerId.
-00060560: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-00060570: 2775 726c 273a 2075 726c 2c20 276d 6574  'url': url, 'met
-00060580: 686f 6427 3a20 6d65 7468 6f64 2c20 2762  hod': method, 'b
-00060590: 6f64 7927 3a20 626f 6479 2c20 2768 6561  ody': body, 'hea
-000605a0: 6465 7273 273a 2068 6561 6465 7273 7d0a  ders': headers}.
-000605b0: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-000605c0: 6572 726f 7273 2873 656c 662c 2068 7474  errors(self, htt
-000605d0: 7043 6f64 652c 2072 6561 736f 6e2c 2075  pCode, reason, u
-000605e0: 726c 2c20 6d65 7468 6f64 2c20 6865 6164  rl, method, head
-000605f0: 6572 732c 2062 6f64 792c 2072 6573 706f  ers, body, respo
-00060600: 6e73 652c 2072 6571 7565 7374 4865 6164  nse, requestHead
-00060610: 6572 732c 2072 6571 7565 7374 426f 6479  ers, requestBody
-00060620: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
-00060630: 7420 7265 7370 6f6e 7365 3a0a 2020 2020  t response:.    
-00060640: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00060650: 6f6e 6520 2023 2066 616c 6c62 6163 6b20  one  # fallback 
-00060660: 746f 2064 6566 6175 6c74 2065 7272 6f72  to default error
-00060670: 2068 616e 646c 6572 0a20 2020 2020 2020   handler.       
-00060680: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-00060690: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-000606a0: 2020 2020 2072 6574 5f63 6f64 653a 2031       ret_code: 1
-000606b0: 3030 3031 2c0a 2020 2020 2020 2020 2320  0001,.        # 
-000606c0: 2020 2020 2020 2020 7265 745f 6d73 673a          ret_msg:
-000606d0: 2027 5265 6164 4d61 7043 423a 2065 7870   'ReadMapCB: exp
-000606e0: 6563 7420 7b6f 7220 6e2c 2062 7574 2066  ect {or n, but f
-000606f0: 6f75 6e64 205c 7530 3030 302c 2065 7272  ound \u0000, err
-00060700: 6f72 2027 202b 0a20 2020 2020 2020 2023  or ' +.        #
-00060710: 2020 2020 2020 2020 2027 666f 756e 6420           'found 
-00060720: 696e 2020 2330 2062 7974 6520 6f66 202e  in  #0 byte of .
-00060730: 2e2e 7c7c 2e2e 2e2c 2062 6967 6765 7220  ..||..., bigger 
-00060740: 636f 6e74 6578 7420 2720 2b0a 2020 2020  context ' +.    
-00060750: 2020 2020 2320 2020 2020 2020 2020 272e      #         '.
-00060760: 2e2e 7c7c 2e2e 2e27 2c0a 2020 2020 2020  ..||...',.      
-00060770: 2020 2320 2020 2020 2020 2020 6578 745f    #         ext_
-00060780: 636f 6465 3a20 2727 2c0a 2020 2020 2020  code: '',.      
-00060790: 2020 2320 2020 2020 2020 2020 6578 745f    #         ext_
-000607a0: 696e 666f 3a20 2727 2c0a 2020 2020 2020  info: '',.      
-000607b0: 2020 2320 2020 2020 2020 2020 7265 7375    #         resu
-000607c0: 6c74 3a20 6e75 6c6c 2c0a 2020 2020 2020  lt: null,.      
-000607d0: 2020 2320 2020 2020 2020 2020 7469 6d65    #         time
-000607e0: 5f6e 6f77 3a20 2731 3538 3339 3334 3130  _now: '158393410
-000607f0: 362e 3539 3034 3336 270a 2020 2020 2020  6.590436'.      
-00060800: 2020 2320 2020 2020 7d0a 2020 2020 2020    #     }.      
-00060810: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
-00060820: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
-00060830: 2020 2020 2020 2272 6574 436f 6465 223a        "retCode":
-00060840: 3130 3030 312c 0a20 2020 2020 2020 2023  10001,.        #
-00060850: 2020 2020 2020 2020 2022 7265 744d 7367           "retMsg
-00060860: 223a 2273 796d 626f 6c20 7061 7261 6d73  ":"symbol params
-00060870: 2065 7272 222c 0a20 2020 2020 2020 2023   err",.        #
-00060880: 2020 2020 2020 2020 2022 7265 7375 6c74           "result
-00060890: 223a 7b22 7379 6d62 6f6c 223a 2222 2c22  ":{"symbol":"","
-000608a0: 6269 6422 3a22 222c 2262 6964 4976 223a  bid":"","bidIv":
-000608b0: 2222 2c22 6269 6453 697a 6522 3a22 222c  "","bidSize":"",
-000608c0: 2261 736b 223a 2222 2c22 6173 6b49 7622  "ask":"","askIv"
-000608d0: 3a22 222c 2261 736b 5369 7a65 223a 2222  :"","askSize":""
-000608e0: 2c22 6c61 7374 5072 6963 6522 3a22 222c  ,"lastPrice":"",
-000608f0: 226f 7065 6e49 6e74 6572 6573 7422 3a22  "openInterest":"
-00060900: 222c 2269 6e64 6578 5072 6963 6522 3a22  ","indexPrice":"
-00060910: 222c 226d 6172 6b50 7269 6365 223a 2222  ","markPrice":""
-00060920: 2c22 6d61 726b 5072 6963 6549 7622 3a22  ,"markPriceIv":"
-00060930: 222c 2263 6861 6e67 6532 3468 223a 2222  ","change24h":""
-00060940: 2c22 6869 6768 3234 6822 3a22 222c 226c  ,"high24h":"","l
-00060950: 6f77 3234 6822 3a22 222c 2276 6f6c 756d  ow24h":"","volum
-00060960: 6532 3468 223a 2222 2c22 7475 726e 6f76  e24h":"","turnov
-00060970: 6572 3234 6822 3a22 222c 2274 6f74 616c  er24h":"","total
-00060980: 566f 6c75 6d65 223a 2222 2c22 746f 7461  Volume":"","tota
-00060990: 6c54 7572 6e6f 7665 7222 3a22 222c 2266  lTurnover":"","f
-000609a0: 756e 6469 6e67 5261 7465 223a 2222 2c22  undingRate":"","
-000609b0: 7072 6564 6963 7465 6446 756e 6469 6e67  predictedFunding
-000609c0: 5261 7465 223a 2222 2c22 6e65 7874 4675  Rate":"","nextFu
-000609d0: 6e64 696e 6754 696d 6522 3a22 222c 2263  ndingTime":"","c
-000609e0: 6f75 6e74 646f 776e 486f 7572 223a 2230  ountdownHour":"0
-000609f0: 222c 2270 7265 6469 6374 6564 4465 6c69  ","predictedDeli
-00060a00: 7665 7279 5072 6963 6522 3a22 222c 2275  veryPrice":"","u
-00060a10: 6e64 6572 6c79 696e 6750 7269 6365 223a  nderlyingPrice":
-00060a20: 2222 2c22 6465 6c74 6122 3a22 222c 2267  "","delta":"","g
-00060a30: 616d 6d61 223a 2222 2c22 7665 6761 223a  amma":"","vega":
-00060a40: 2222 2c22 7468 6574 6122 3a22 227d 0a20  "","theta":""}. 
-00060a50: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
-00060a60: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-00060a70: 2065 7272 6f72 436f 6465 203d 2073 656c   errorCode = sel
-00060a80: 662e 7361 6665 5f73 7472 696e 675f 3228  f.safe_string_2(
-00060a90: 7265 7370 6f6e 7365 2c20 2772 6574 5f63  response, 'ret_c
-00060aa0: 6f64 6527 2c20 2772 6574 436f 6465 2729  ode', 'retCode')
-00060ab0: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
-00060ac0: 7243 6f64 6520 213d 2027 3027 3a0a 2020  rCode != '0':.  
-00060ad0: 2020 2020 2020 2020 2020 6966 2065 7272            if err
-00060ae0: 6f72 436f 6465 203d 3d20 2733 3030 3834  orCode == '30084
-00060af0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00060b00: 2020 2023 206e 6f74 2061 6e20 6572 726f     # not an erro
-00060b10: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00060b20: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
-00060b30: 7562 2e63 6f6d 2f63 6378 742f 6363 7874  ub.com/ccxt/ccxt
-00060b40: 2f69 7373 7565 732f 3131 3236 380a 2020  /issues/11268.  
-00060b50: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00060b60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00060b70: 6f6d 2f63 6378 742f 6363 7874 2f70 756c  om/ccxt/ccxt/pul
-00060b80: 6c2f 3131 3632 340a 2020 2020 2020 2020  l/11624.        
-00060b90: 2020 2020 2020 2020 2320 504f 5354 2068          # POST h
-00060ba0: 7474 7073 3a2f 2f61 7069 2e62 7962 6974  ttps://api.bybit
-00060bb0: 2e63 6f6d 2f76 322f 7072 6976 6174 652f  .com/v2/private/
-00060bc0: 706f 7369 7469 6f6e 2f73 7769 7463 682d  position/switch-
-00060bd0: 6973 6f6c 6174 6564 2032 3030 204f 4b0a  isolated 200 OK.
-00060be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00060bf0: 2320 7b22 7265 745f 636f 6465 223a 3330  # {"ret_code":30
-00060c00: 3038 342c 2272 6574 5f6d 7367 223a 2249  084,"ret_msg":"I
-00060c10: 736f 6c61 7465 6420 6e6f 7420 6d6f 6469  solated not modi
-00060c20: 6669 6564 222c 2265 7874 5f63 6f64 6522  fied","ext_code"
-00060c30: 3a22 222c 2265 7874 5f69 6e66 6f22 3a22  :"","ext_info":"
-00060c40: 222c 2272 6573 756c 7422 3a6e 756c 6c2c  ","result":null,
-00060c50: 2274 696d 655f 6e6f 7722 3a22 3136 3432  "time_now":"1642
-00060c60: 3030 3532 3139 2e39 3337 3938 3822 2c22  005219.937988","
-00060c70: 7261 7465 5f6c 696d 6974 5f73 7461 7475  rate_limit_statu
-00060c80: 7322 3a37 332c 2272 6174 655f 6c69 6d69  s":73,"rate_limi
-00060c90: 745f 7265 7365 745f 6d73 223a 3136 3432  t_reset_ms":1642
-00060ca0: 3030 3532 3139 3839 342c 2272 6174 655f  005219894,"rate_
-00060cb0: 6c69 6d69 7422 3a37 357d 0a20 2020 2020  limit":75}.     
-00060cc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00060cd0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2020  n None.         
-00060ce0: 2020 2066 6565 6462 6163 6b20 3d20 4e6f     feedback = No
-00060cf0: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-00060d00: 6620 6572 726f 7243 6f64 6520 3d3d 2027  f errorCode == '
-00060d10: 3130 3030 3527 3a0a 2020 2020 2020 2020  10005':.        
-00060d20: 2020 2020 2020 2020 6665 6564 6261 636b          feedback
-00060d30: 203d 2073 656c 662e 6964 202b 2027 2070   = self.id + ' p
-00060d40: 7269 7661 7465 2061 7069 2075 7365 7320  rivate api uses 
-00060d50: 2f75 7365 722f 7633 2f70 7269 7661 7465  /user/v3/private
-00060d60: 2f71 7565 7279 2d61 7069 2074 6f20 6368  /query-api to ch
-00060d70: 6563 6b20 6966 2079 6f75 2068 6176 6520  eck if you have 
-00060d80: 6120 756e 6966 6965 6420 6163 636f 756e  a unified accoun
-00060d90: 742e 2054 6865 2041 5049 206b 6579 206f  t. The API key o
-00060da0: 6620 7573 6572 2069 6420 6d75 7374 206f  f user id must o
-00060db0: 776e 206f 6e65 206f 6620 7065 726d 6973  wn one of permis
-00060dc0: 7369 6f6e 733a 2022 4163 636f 756e 7420  sions: "Account 
-00060dd0: 5472 616e 7366 6572 222c 2022 5375 6261  Transfer", "Suba
-00060de0: 6363 6f75 6e74 2054 7261 6e73 6665 7222  ccount Transfer"
-00060df0: 2c20 2257 6974 6864 7261 7761 6c22 2027  , "Withdrawal" '
-00060e00: 202b 2062 6f64 790a 2020 2020 2020 2020   + body.        
-00060e10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00060e20: 2020 2020 2020 2020 2020 6665 6564 6261            feedba
-00060e30: 636b 203d 2073 656c 662e 6964 202b 2027  ck = self.id + '
-00060e40: 2027 202b 2062 6f64 790a 2020 2020 2020   ' + body.      
-00060e50: 2020 2020 2020 7365 6c66 2e74 6872 6f77        self.throw
-00060e60: 5f62 726f 6164 6c79 5f6d 6174 6368 6564  _broadly_matched
-00060e70: 5f65 7863 6570 7469 6f6e 2873 656c 662e  _exception(self.
-00060e80: 6578 6365 7074 696f 6e73 5b27 6272 6f61  exceptions['broa
-00060e90: 6427 5d2c 2062 6f64 792c 2066 6565 6462  d'], body, feedb
-00060ea0: 6163 6b29 0a20 2020 2020 2020 2020 2020  ack).           
-00060eb0: 2073 656c 662e 7468 726f 775f 6578 6163   self.throw_exac
-00060ec0: 746c 795f 6d61 7463 6865 645f 6578 6365  tly_matched_exce
-00060ed0: 7074 696f 6e28 7365 6c66 2e65 7863 6570  ption(self.excep
-00060ee0: 7469 6f6e 735b 2765 7861 6374 275d 2c20  tions['exact'], 
-00060ef0: 6572 726f 7243 6f64 652c 2066 6565 6462  errorCode, feedb
-00060f00: 6163 6b29 0a20 2020 2020 2020 2020 2020  ack).           
-00060f10: 2072 6169 7365 2045 7863 6861 6e67 6545   raise ExchangeE
-00060f20: 7272 6f72 2866 6565 6462 6163 6b29 2020  rror(feedback)  
-00060f30: 2320 756e 6b6e 6f77 6e20 6d65 7373 6167  # unknown messag
-00060f40: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00060f50: 204e 6f6e 650a                            None.
+0005ff80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0005ff90: 2020 2020 2020 2020 2020 2073 6967 6e61             signa
+0005ffa0: 7475 7265 203d 2073 656c 662e 686d 6163  ture = self.hmac
+0005ffb0: 2873 656c 662e 656e 636f 6465 2861 7574  (self.encode(aut
+0005ffc0: 6846 756c 6c29 2c20 7365 6c66 2e65 6e63  hFull), self.enc
+0005ffd0: 6f64 6528 7365 6c66 2e73 6563 7265 7429  ode(self.secret)
+0005ffe0: 2c20 6861 7368 6c69 622e 7368 6132 3536  , hashlib.sha256
+0005fff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00060000: 2020 6865 6164 6572 735b 2758 2d42 4150    headers['X-BAP
+00060010: 492d 5349 474e 275d 203d 2073 6967 6e61  I-SIGN'] = signa
+00060020: 7475 7265 0a20 2020 2020 2020 2020 2020  ture.           
+00060030: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00060040: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
+00060050: 656c 662e 6578 7465 6e64 2870 6172 616d  elf.extend(param
+00060060: 732c 207b 0a20 2020 2020 2020 2020 2020  s, {.           
+00060070: 2020 2020 2020 2020 2027 6170 695f 6b65           'api_ke
+00060080: 7927 3a20 7365 6c66 2e61 7069 4b65 792c  y': self.apiKey,
+00060090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000600a0: 2020 2020 2027 7265 6376 5f77 696e 646f       'recv_windo
+000600b0: 7727 3a20 7365 6c66 2e6f 7074 696f 6e73  w': self.options
+000600c0: 5b27 7265 6376 5769 6e64 6f77 275d 2c0a  ['recvWindow'],.
+000600d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000600e0: 2020 2020 2774 696d 6573 7461 6d70 273a      'timestamp':
+000600f0: 2074 696d 6573 7461 6d70 2c0a 2020 2020   timestamp,.    
+00060100: 2020 2020 2020 2020 2020 2020 7d29 0a20              }). 
+00060110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00060120: 6f72 7465 6451 7565 7279 203d 2073 656c  ortedQuery = sel
+00060130: 662e 6b65 7973 6f72 7428 7175 6572 7929  f.keysort(query)
+00060140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00060150: 2061 7574 6820 3d20 7365 6c66 2e72 6177   auth = self.raw
+00060160: 656e 636f 6465 2873 6f72 7465 6451 7565  encode(sortedQue
+00060170: 7279 290a 2020 2020 2020 2020 2020 2020  ry).            
+00060180: 2020 2020 7369 676e 6174 7572 6520 3d20      signature = 
+00060190: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+000601a0: 2020 2020 2069 6620 7365 6c66 2e73 6563       if self.sec
+000601b0: 7265 742e 6669 6e64 2827 5052 4956 4154  ret.find('PRIVAT
+000601c0: 4520 4b45 5927 2920 3e20 2d31 3a0a 2020  E KEY') > -1:.  
+000601d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000601e0: 2020 7369 676e 6174 7572 6520 3d20 7365    signature = se
+000601f0: 6c66 2e72 7361 2861 7574 682c 2073 656c  lf.rsa(auth, sel
+00060200: 662e 7365 6372 6574 2c20 2773 6861 3235  f.secret, 'sha25
+00060210: 3627 290a 2020 2020 2020 2020 2020 2020  6').            
+00060220: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00060230: 2020 2020 2020 2020 2020 2020 2020 7369                si
+00060240: 676e 6174 7572 6520 3d20 7365 6c66 2e68  gnature = self.h
+00060250: 6d61 6328 7365 6c66 2e65 6e63 6f64 6528  mac(self.encode(
+00060260: 6175 7468 292c 2073 656c 662e 656e 636f  auth), self.enco
+00060270: 6465 2873 656c 662e 7365 6372 6574 292c  de(self.secret),
+00060280: 2068 6173 686c 6962 2e73 6861 3235 3629   hashlib.sha256)
+00060290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000602a0: 2069 6620 6d65 7468 6f64 203d 3d20 2750   if method == 'P
+000602b0: 4f53 5427 3a0a 2020 2020 2020 2020 2020  OST':.          
+000602c0: 2020 2020 2020 2020 2020 6973 5370 6f74            isSpot
+000602d0: 203d 2075 726c 2e66 696e 6428 2773 706f   = url.find('spo
+000602e0: 7427 2920 3e3d 2030 0a20 2020 2020 2020  t') >= 0.       
+000602f0: 2020 2020 2020 2020 2020 2020 2065 7874               ext
+00060300: 656e 6465 6451 7565 7279 203d 2073 656c  endedQuery = sel
+00060310: 662e 6578 7465 6e64 2871 7565 7279 2c20  f.extend(query, 
+00060320: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00060330: 2020 2020 2020 2020 2020 2773 6967 6e27            'sign'
+00060340: 3a20 7369 676e 6174 7572 652c 0a20 2020  : signature,.   
+00060350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060360: 207d 290a 2020 2020 2020 2020 2020 2020   }).            
+00060370: 2020 2020 2020 2020 6966 2069 7353 706f          if isSpo
+00060380: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00060390: 2020 2020 2020 2020 2020 2062 6f64 7920             body 
+000603a0: 3d20 7365 6c66 2e75 726c 656e 636f 6465  = self.urlencode
+000603b0: 2865 7874 656e 6465 6451 7565 7279 290a  (extendedQuery).
+000603c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000603d0: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
+000603e0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000603f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060400: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
+00060410: 2761 7070 6c69 6361 7469 6f6e 2f78 2d77  'application/x-w
+00060420: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
+00060430: 6564 272c 0a20 2020 2020 2020 2020 2020  ed',.           
+00060440: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00060450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060460: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00060470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00060480: 2062 6f64 7920 3d20 7365 6c66 2e6a 736f   body = self.jso
+00060490: 6e28 6578 7465 6e64 6564 5175 6572 7929  n(extendedQuery)
+000604a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000604b0: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+000604c0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+000604d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000604e0: 2027 436f 6e74 656e 742d 5479 7065 273a   'Content-Type':
+000604f0: 2027 6170 706c 6963 6174 696f 6e2f 6a73   'application/js
+00060500: 6f6e 272c 0a20 2020 2020 2020 2020 2020  on',.           
+00060510: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00060520: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00060530: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00060540: 2020 2020 2020 2020 2075 726c 202b 3d20           url += 
+00060550: 273f 2720 2b20 7365 6c66 2e72 6177 656e  '?' + self.rawen
+00060560: 636f 6465 2873 6f72 7465 6451 7565 7279  code(sortedQuery
+00060570: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00060580: 2020 2020 2020 7572 6c20 2b3d 2027 2673        url += '&s
+00060590: 6967 6e3d 2720 2b20 7369 676e 6174 7572  ign=' + signatur
+000605a0: 650a 2020 2020 2020 2020 6966 206d 6574  e.        if met
+000605b0: 686f 6420 3d3d 2027 504f 5354 273a 0a20  hod == 'POST':. 
+000605c0: 2020 2020 2020 2020 2020 2062 726f 6b65             broke
+000605d0: 7249 6420 3d20 7365 6c66 2e73 6166 655f  rId = self.safe_
+000605e0: 7374 7269 6e67 2873 656c 662e 6f70 7469  string(self.opti
+000605f0: 6f6e 732c 2027 6272 6f6b 6572 4964 2729  ons, 'brokerId')
+00060600: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00060610: 6272 6f6b 6572 4964 2069 7320 6e6f 7420  brokerId is not 
+00060620: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00060630: 2020 2020 2020 6865 6164 6572 735b 2752        headers['R
+00060640: 6566 6572 6572 275d 203d 2062 726f 6b65  eferer'] = broke
+00060650: 7249 640a 2020 2020 2020 2020 7265 7475  rId.        retu
+00060660: 726e 207b 2775 726c 273a 2075 726c 2c20  rn {'url': url, 
+00060670: 276d 6574 686f 6427 3a20 6d65 7468 6f64  'method': method
+00060680: 2c20 2762 6f64 7927 3a20 626f 6479 2c20  , 'body': body, 
+00060690: 2768 6561 6465 7273 273a 2068 6561 6465  'headers': heade
+000606a0: 7273 7d0a 0a20 2020 2064 6566 2068 616e  rs}..    def han
+000606b0: 646c 655f 6572 726f 7273 2873 656c 662c  dle_errors(self,
+000606c0: 2068 7474 7043 6f64 652c 2072 6561 736f   httpCode, reaso
+000606d0: 6e2c 2075 726c 2c20 6d65 7468 6f64 2c20  n, url, method, 
+000606e0: 6865 6164 6572 732c 2062 6f64 792c 2072  headers, body, r
+000606f0: 6573 706f 6e73 652c 2072 6571 7565 7374  esponse, request
+00060700: 4865 6164 6572 732c 2072 6571 7565 7374  Headers, request
+00060710: 426f 6479 293a 0a20 2020 2020 2020 2069  Body):.        i
+00060720: 6620 6e6f 7420 7265 7370 6f6e 7365 3a0a  f not response:.
+00060730: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00060740: 726e 204e 6f6e 6520 2023 2066 616c 6c62  rn None  # fallb
+00060750: 6163 6b20 746f 2064 6566 6175 6c74 2065  ack to default e
+00060760: 7272 6f72 2068 616e 646c 6572 0a20 2020  rror handler.   
+00060770: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
+00060780: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
+00060790: 2020 2020 2020 2020 2072 6574 5f63 6f64           ret_cod
+000607a0: 653a 2031 3030 3031 2c0a 2020 2020 2020  e: 10001,.      
+000607b0: 2020 2320 2020 2020 2020 2020 7265 745f    #         ret_
+000607c0: 6d73 673a 2027 5265 6164 4d61 7043 423a  msg: 'ReadMapCB:
+000607d0: 2065 7870 6563 7420 7b6f 7220 6e2c 2062   expect {or n, b
+000607e0: 7574 2066 6f75 6e64 205c 7530 3030 302c  ut found \u0000,
+000607f0: 2065 7272 6f72 2027 202b 0a20 2020 2020   error ' +.     
+00060800: 2020 2023 2020 2020 2020 2020 2027 666f     #         'fo
+00060810: 756e 6420 696e 2020 2330 2062 7974 6520  und in  #0 byte 
+00060820: 6f66 202e 2e2e 7c7c 2e2e 2e2c 2062 6967  of ...||..., big
+00060830: 6765 7220 636f 6e74 6578 7420 2720 2b0a  ger context ' +.
+00060840: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00060850: 2020 272e 2e2e 7c7c 2e2e 2e27 2c0a 2020    '...||...',.  
+00060860: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00060870: 6578 745f 636f 6465 3a20 2727 2c0a 2020  ext_code: '',.  
+00060880: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00060890: 6578 745f 696e 666f 3a20 2727 2c0a 2020  ext_info: '',.  
+000608a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+000608b0: 7265 7375 6c74 3a20 6e75 6c6c 2c0a 2020  result: null,.  
+000608c0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+000608d0: 7469 6d65 5f6e 6f77 3a20 2731 3538 3339  time_now: '15839
+000608e0: 3334 3130 362e 3539 3034 3336 270a 2020  34106.590436'.  
+000608f0: 2020 2020 2020 2320 2020 2020 7d0a 2020        #     }.  
+00060900: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+00060910: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
+00060920: 2320 2020 2020 2020 2020 2272 6574 436f  #         "retCo
+00060930: 6465 223a 3130 3030 312c 0a20 2020 2020  de":10001,.     
+00060940: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+00060950: 744d 7367 223a 2273 796d 626f 6c20 7061  tMsg":"symbol pa
+00060960: 7261 6d73 2065 7272 222c 0a20 2020 2020  rams err",.     
+00060970: 2020 2023 2020 2020 2020 2020 2022 7265     #         "re
+00060980: 7375 6c74 223a 7b22 7379 6d62 6f6c 223a  sult":{"symbol":
+00060990: 2222 2c22 6269 6422 3a22 222c 2262 6964  "","bid":"","bid
+000609a0: 4976 223a 2222 2c22 6269 6453 697a 6522  Iv":"","bidSize"
+000609b0: 3a22 222c 2261 736b 223a 2222 2c22 6173  :"","ask":"","as
+000609c0: 6b49 7622 3a22 222c 2261 736b 5369 7a65  kIv":"","askSize
+000609d0: 223a 2222 2c22 6c61 7374 5072 6963 6522  ":"","lastPrice"
+000609e0: 3a22 222c 226f 7065 6e49 6e74 6572 6573  :"","openInteres
+000609f0: 7422 3a22 222c 2269 6e64 6578 5072 6963  t":"","indexPric
+00060a00: 6522 3a22 222c 226d 6172 6b50 7269 6365  e":"","markPrice
+00060a10: 223a 2222 2c22 6d61 726b 5072 6963 6549  ":"","markPriceI
+00060a20: 7622 3a22 222c 2263 6861 6e67 6532 3468  v":"","change24h
+00060a30: 223a 2222 2c22 6869 6768 3234 6822 3a22  ":"","high24h":"
+00060a40: 222c 226c 6f77 3234 6822 3a22 222c 2276  ","low24h":"","v
+00060a50: 6f6c 756d 6532 3468 223a 2222 2c22 7475  olume24h":"","tu
+00060a60: 726e 6f76 6572 3234 6822 3a22 222c 2274  rnover24h":"","t
+00060a70: 6f74 616c 566f 6c75 6d65 223a 2222 2c22  otalVolume":"","
+00060a80: 746f 7461 6c54 7572 6e6f 7665 7222 3a22  totalTurnover":"
+00060a90: 222c 2266 756e 6469 6e67 5261 7465 223a  ","fundingRate":
+00060aa0: 2222 2c22 7072 6564 6963 7465 6446 756e  "","predictedFun
+00060ab0: 6469 6e67 5261 7465 223a 2222 2c22 6e65  dingRate":"","ne
+00060ac0: 7874 4675 6e64 696e 6754 696d 6522 3a22  xtFundingTime":"
+00060ad0: 222c 2263 6f75 6e74 646f 776e 486f 7572  ","countdownHour
+00060ae0: 223a 2230 222c 2270 7265 6469 6374 6564  ":"0","predicted
+00060af0: 4465 6c69 7665 7279 5072 6963 6522 3a22  DeliveryPrice":"
+00060b00: 222c 2275 6e64 6572 6c79 696e 6750 7269  ","underlyingPri
+00060b10: 6365 223a 2222 2c22 6465 6c74 6122 3a22  ce":"","delta":"
+00060b20: 222c 2267 616d 6d61 223a 2222 2c22 7665  ","gamma":"","ve
+00060b30: 6761 223a 2222 2c22 7468 6574 6122 3a22  ga":"","theta":"
+00060b40: 227d 0a20 2020 2020 2020 2023 2020 2020  "}.        #    
+00060b50: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
+00060b60: 2020 2020 2065 7272 6f72 436f 6465 203d       errorCode =
+00060b70: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
+00060b80: 675f 3228 7265 7370 6f6e 7365 2c20 2772  g_2(response, 'r
+00060b90: 6574 5f63 6f64 6527 2c20 2772 6574 436f  et_code', 'retCo
+00060ba0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+00060bb0: 6572 726f 7243 6f64 6520 213d 2027 3027  errorCode != '0'
+00060bc0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00060bd0: 2065 7272 6f72 436f 6465 203d 3d20 2733   errorCode == '3
+00060be0: 3030 3834 273a 0a20 2020 2020 2020 2020  0084':.         
+00060bf0: 2020 2020 2020 2023 206e 6f74 2061 6e20         # not an 
+00060c00: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
+00060c10: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+00060c20: 6769 7468 7562 2e63 6f6d 2f63 6378 742f  github.com/ccxt/
+00060c30: 6363 7874 2f69 7373 7565 732f 3131 3236  ccxt/issues/1126
+00060c40: 380a 2020 2020 2020 2020 2020 2020 2020  8.              
+00060c50: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
+00060c60: 7562 2e63 6f6d 2f63 6378 742f 6363 7874  ub.com/ccxt/ccxt
+00060c70: 2f70 756c 6c2f 3131 3632 340a 2020 2020  /pull/11624.    
+00060c80: 2020 2020 2020 2020 2020 2020 2320 504f              # PO
+00060c90: 5354 2068 7474 7073 3a2f 2f61 7069 2e62  ST https://api.b
+00060ca0: 7962 6974 2e63 6f6d 2f76 322f 7072 6976  ybit.com/v2/priv
+00060cb0: 6174 652f 706f 7369 7469 6f6e 2f73 7769  ate/position/swi
+00060cc0: 7463 682d 6973 6f6c 6174 6564 2032 3030  tch-isolated 200
+00060cd0: 204f 4b0a 2020 2020 2020 2020 2020 2020   OK.            
+00060ce0: 2020 2020 2320 7b22 7265 745f 636f 6465      # {"ret_code
+00060cf0: 223a 3330 3038 342c 2272 6574 5f6d 7367  ":30084,"ret_msg
+00060d00: 223a 2249 736f 6c61 7465 6420 6e6f 7420  ":"Isolated not 
+00060d10: 6d6f 6469 6669 6564 222c 2265 7874 5f63  modified","ext_c
+00060d20: 6f64 6522 3a22 222c 2265 7874 5f69 6e66  ode":"","ext_inf
+00060d30: 6f22 3a22 222c 2272 6573 756c 7422 3a6e  o":"","result":n
+00060d40: 756c 6c2c 2274 696d 655f 6e6f 7722 3a22  ull,"time_now":"
+00060d50: 3136 3432 3030 3532 3139 2e39 3337 3938  1642005219.93798
+00060d60: 3822 2c22 7261 7465 5f6c 696d 6974 5f73  8","rate_limit_s
+00060d70: 7461 7475 7322 3a37 332c 2272 6174 655f  tatus":73,"rate_
+00060d80: 6c69 6d69 745f 7265 7365 745f 6d73 223a  limit_reset_ms":
+00060d90: 3136 3432 3030 3532 3139 3839 342c 2272  1642005219894,"r
+00060da0: 6174 655f 6c69 6d69 7422 3a37 357d 0a20  ate_limit":75}. 
+00060db0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00060dc0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+00060dd0: 2020 2020 2020 2066 6565 6462 6163 6b20         feedback 
+00060de0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00060df0: 2020 2069 6620 6572 726f 7243 6f64 6520     if errorCode 
+00060e00: 3d3d 2027 3130 3030 3527 3a0a 2020 2020  == '10005':.    
+00060e10: 2020 2020 2020 2020 2020 2020 6665 6564              feed
+00060e20: 6261 636b 203d 2073 656c 662e 6964 202b  back = self.id +
+00060e30: 2027 2070 7269 7661 7465 2061 7069 2075   ' private api u
+00060e40: 7365 7320 2f75 7365 722f 7633 2f70 7269  ses /user/v3/pri
+00060e50: 7661 7465 2f71 7565 7279 2d61 7069 2074  vate/query-api t
+00060e60: 6f20 6368 6563 6b20 6966 2079 6f75 2068  o check if you h
+00060e70: 6176 6520 6120 756e 6966 6965 6420 6163  ave a unified ac
+00060e80: 636f 756e 742e 2054 6865 2041 5049 206b  count. The API k
+00060e90: 6579 206f 6620 7573 6572 2069 6420 6d75  ey of user id mu
+00060ea0: 7374 206f 776e 206f 6e65 206f 6620 7065  st own one of pe
+00060eb0: 726d 6973 7369 6f6e 733a 2022 4163 636f  rmissions: "Acco
+00060ec0: 756e 7420 5472 616e 7366 6572 222c 2022  unt Transfer", "
+00060ed0: 5375 6261 6363 6f75 6e74 2054 7261 6e73  Subaccount Trans
+00060ee0: 6665 7222 2c20 2257 6974 6864 7261 7761  fer", "Withdrawa
+00060ef0: 6c22 2027 202b 2062 6f64 790a 2020 2020  l" ' + body.    
+00060f00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00060f10: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+00060f20: 6564 6261 636b 203d 2073 656c 662e 6964  edback = self.id
+00060f30: 202b 2027 2027 202b 2062 6f64 790a 2020   + ' ' + body.  
+00060f40: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00060f50: 6872 6f77 5f62 726f 6164 6c79 5f6d 6174  hrow_broadly_mat
+00060f60: 6368 6564 5f65 7863 6570 7469 6f6e 2873  ched_exception(s
+00060f70: 656c 662e 6578 6365 7074 696f 6e73 5b27  elf.exceptions['
+00060f80: 6272 6f61 6427 5d2c 2062 6f64 792c 2066  broad'], body, f
+00060f90: 6565 6462 6163 6b29 0a20 2020 2020 2020  eedback).       
+00060fa0: 2020 2020 2073 656c 662e 7468 726f 775f       self.throw_
+00060fb0: 6578 6163 746c 795f 6d61 7463 6865 645f  exactly_matched_
+00060fc0: 6578 6365 7074 696f 6e28 7365 6c66 2e65  exception(self.e
+00060fd0: 7863 6570 7469 6f6e 735b 2765 7861 6374  xceptions['exact
+00060fe0: 275d 2c20 6572 726f 7243 6f64 652c 2066  '], errorCode, f
+00060ff0: 6565 6462 6163 6b29 0a20 2020 2020 2020  eedback).       
+00061000: 2020 2020 2072 6169 7365 2045 7863 6861       raise Excha
+00061010: 6e67 6545 7272 6f72 2866 6565 6462 6163  ngeError(feedbac
+00061020: 6b29 2020 2320 756e 6b6e 6f77 6e20 6d65  k)  # unknown me
+00061030: 7373 6167 650a 2020 2020 2020 2020 7265  ssage.        re
+00061040: 7475 726e 204e 6f6e 650a                 turn None.
```

### Comparing `ccxt-3.1.6/ccxt/cex.py` & `ccxt-3.1.7/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinbase.py` & `ccxt-3.1.7/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinbaseprime.py` & `ccxt-3.1.7/ccxt/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinbasepro.py` & `ccxt-3.1.7/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coincheck.py` & `ccxt-3.1.7/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinex.py` & `ccxt-3.1.7/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinfalcon.py` & `ccxt-3.1.7/ccxt/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinmate.py` & `ccxt-3.1.7/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinone.py` & `ccxt-3.1.7/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinsph.py` & `ccxt-3.1.7/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/coinspot.py` & `ccxt-3.1.7/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/cryptocom.py` & `ccxt-3.1.7/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/currencycom.py` & `ccxt-3.1.7/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/delta.py` & `ccxt-3.1.7/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/deribit.py` & `ccxt-3.1.7/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/digifinex.py` & `ccxt-3.1.7/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/exmo.py` & `ccxt-3.1.7/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/flowbtc.py` & `ccxt-3.1.7/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/fmfwio.py` & `ccxt-3.1.7/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/gate.py` & `ccxt-3.1.7/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/gemini.py` & `ccxt-3.1.7/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/hitbtc.py` & `ccxt-3.1.7/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/hitbtc3.py` & `ccxt-3.1.7/ccxt/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/hollaex.py` & `ccxt-3.1.7/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/huobi.py` & `ccxt-3.1.7/ccxt/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/huobijp.py` & `ccxt-3.1.7/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/huobipro.py` & `ccxt-3.1.7/ccxt/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/idex.py` & `ccxt-3.1.7/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/independentreserve.py` & `ccxt-3.1.7/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/indodax.py` & `ccxt-3.1.7/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/itbit.py` & `ccxt-3.1.7/ccxt/itbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/kraken.py` & `ccxt-3.1.7/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/krakenfutures.py` & `ccxt-3.1.7/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/kucoin.py` & `ccxt-3.1.7/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/kucoinfutures.py` & `ccxt-3.1.7/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/kuna.py` & `ccxt-3.1.7/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/latoken.py` & `ccxt-3.1.7/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/lbank.py` & `ccxt-3.1.7/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/lbank2.py` & `ccxt-3.1.7/ccxt/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/luno.py` & `ccxt-3.1.7/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/lykke.py` & `ccxt-3.1.7/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/mercado.py` & `ccxt-3.1.7/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/mexc.py` & `ccxt-3.1.7/ccxt/mexc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
 from ccxt.base.exchange import Exchange
 from ccxt.abstract.mexc import ImplicitAPI
 import hashlib
 from ccxt.base.types import OrderSide
+from ccxt.base.types import IndexType
 from typing import Optional
 from typing import List
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import PermissionDenied
 from ccxt.base.errors import AccountSuspended
 from ccxt.base.errors import ArgumentsRequired
 from ccxt.base.errors import BadRequest
@@ -1002,14 +1003,16 @@
                 },
                 'info': market,
             })
         return result
 
     def fetch_order_book(self, symbol: str, limit: Optional[int] = None, params={}):
         """
+        see https://mxcdevelop.github.io/apidocs/spot_v3_en/#order-book
+        see https://mxcdevelop.github.io/apidocs/contract_v1_en/#get-the-contract-s-depth-information
         fetches information on open orders with bid(buy) and ask(sell) prices, volumes and other data
         :param str symbol: unified symbol of the market to fetch the order book for
         :param int|None limit: the maximum amount of order book entries to return
         :param dict params: extra parameters specific to the mexc3 api endpoint
         :returns dict: A dictionary of `order book structures <https://docs.ccxt.com/#/?id=order-book-structure>` indexed by market symbols
         """
         self.load_markets()
@@ -1059,14 +1062,22 @@
             #
             data = self.safe_value(response, 'data')
             timestamp = self.safe_integer(data, 'timestamp')
             orderbook = self.parse_order_book(data, symbol, timestamp)
             orderbook['nonce'] = self.safe_integer(data, 'version')
         return orderbook
 
+    def parse_bid_ask(self, bidask, priceKey: IndexType = 0, amountKey: IndexType = 1, countKey: IndexType = 2):
+        price = self.safe_number(bidask, priceKey)
+        amount = self.safe_number(bidask, amountKey)
+        count = self.safe_number(bidask, countKey)
+        if count is not None:
+            return [price, amount, count]
+        return [price, amount]
+
     def fetch_trades(self, symbol: str, since: Optional[int] = None, limit: Optional[int] = None, params={}):
         """
         get the list of most recent trades for a particular symbol
         :param str symbol: unified symbol of the market to fetch trades for
         :param int|None since: timestamp in ms of the earliest trade to fetch
         :param int|None limit: the maximum amount of trades to fetch
         :param dict params: extra parameters specific to the mexc3 api endpoint
```

### Comparing `ccxt-3.1.6/ccxt/ndax.py` & `ccxt-3.1.7/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/novadax.py` & `ccxt-3.1.7/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/oceanex.py` & `ccxt-3.1.7/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/okcoin.py` & `ccxt-3.1.7/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/okx.py` & `ccxt-3.1.7/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/paymium.py` & `ccxt-3.1.7/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/phemex.py` & `ccxt-3.1.7/ccxt/phemex.py`

 * *Files 0% similar despite different names*

```diff
@@ -11249,740 +11249,802 @@
 0002bf00: 7220 7379 6d62 6f6c 3a20 756e 6966 6965  r symbol: unifie
 0002bf10: 6420 6d61 726b 6574 2073 796d 626f 6c0a  d market symbol.
 0002bf20: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
 0002bf30: 6963 7420 7061 7261 6d73 3a20 6578 7472  ict params: extr
 0002bf40: 6120 7061 7261 6d65 7465 7273 2073 7065  a parameters spe
 0002bf50: 6369 6669 6320 746f 2074 6865 2070 6865  cific to the phe
 0002bf60: 6d65 7820 6170 6920 656e 6470 6f69 6e74  mex api endpoint
-0002bf70: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0002bf80: 7320 6469 6374 3a20 7265 7370 6f6e 7365  s dict: response
-0002bf90: 2066 726f 6d20 7468 6520 6578 6368 616e   from the exchan
-0002bfa0: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
-0002bfb0: 2020 2020 2020 2023 2057 4152 4e49 4e47         # WARNING
-0002bfc0: 3a20 5448 4953 2057 494c 4c20 494e 4352  : THIS WILL INCR
-0002bfd0: 4541 5345 204c 4951 5549 4441 5449 4f4e  EASE LIQUIDATION
-0002bfe0: 2050 5249 4345 2046 4f52 204f 5045 4e20   PRICE FOR OPEN 
-0002bff0: 4953 4f4c 4154 4544 204c 4f4e 4720 504f  ISOLATED LONG PO
-0002c000: 5349 5449 4f4e 530a 2020 2020 2020 2020  SITIONS.        
-0002c010: 2320 414e 4420 4445 4352 4541 5345 204c  # AND DECREASE L
-0002c020: 4951 5549 4441 5449 4f4e 2050 5249 4345  IQUIDATION PRICE
-0002c030: 2046 4f52 204f 5045 4e20 4953 4f4c 4154   FOR OPEN ISOLAT
-0002c040: 4544 2053 484f 5254 2050 4f53 4954 494f  ED SHORT POSITIO
-0002c050: 4e53 0a20 2020 2020 2020 2069 6620 7379  NS.        if sy
-0002c060: 6d62 6f6c 2069 7320 4e6f 6e65 3a0a 2020  mbol is None:.  
-0002c070: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002c080: 4172 6775 6d65 6e74 7352 6571 7569 7265  ArgumentsRequire
-0002c090: 6428 7365 6c66 2e69 6420 2b20 2720 7365  d(self.id + ' se
-0002c0a0: 744c 6576 6572 6167 6528 2920 7265 7175  tLeverage() requ
-0002c0b0: 6972 6573 2061 2073 796d 626f 6c20 6172  ires a symbol ar
-0002c0c0: 6775 6d65 6e74 2729 0a20 2020 2020 2020  gument').       
-0002c0d0: 2069 6620 286c 6576 6572 6167 6520 3c20   if (leverage < 
-0002c0e0: 3129 206f 7220 286c 6576 6572 6167 6520  1) or (leverage 
-0002c0f0: 3e20 3130 3029 3a0a 2020 2020 2020 2020  > 100):.        
-0002c100: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
-0002c110: 7565 7374 2873 656c 662e 6964 202b 2027  uest(self.id + '
-0002c120: 2073 6574 4c65 7665 7261 6765 2829 206c   setLeverage() l
-0002c130: 6576 6572 6167 6520 7368 6f75 6c64 2062  everage should b
-0002c140: 6520 6265 7477 6565 6e20 3120 616e 6420  e between 1 and 
-0002c150: 3130 3027 290a 2020 2020 2020 2020 7365  100').        se
-0002c160: 6c66 2e6c 6f61 645f 6d61 726b 6574 7328  lf.load_markets(
-0002c170: 290a 2020 2020 2020 2020 6d61 726b 6574  ).        market
-0002c180: 203d 2073 656c 662e 6d61 726b 6574 2873   = self.market(s
-0002c190: 796d 626f 6c29 0a20 2020 2020 2020 2072  ymbol).        r
-0002c1a0: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
-0002c1b0: 2020 2020 2020 2027 7379 6d62 6f6c 273a         'symbol':
-0002c1c0: 206d 6172 6b65 745b 2769 6427 5d2c 0a20   market['id'],. 
-0002c1d0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0002c1e0: 206d 6574 686f 6420 3d20 2770 7269 7661   method = 'priva
-0002c1f0: 7465 5075 7450 6f73 6974 696f 6e73 4c65  tePutPositionsLe
-0002c200: 7665 7261 6765 270a 2020 2020 2020 2020  verage'.        
-0002c210: 6966 206d 6172 6b65 745b 2773 6574 746c  if market['settl
-0002c220: 6527 5d20 3d3d 2027 5553 4454 273a 0a20  e'] == 'USDT':. 
-0002c230: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-0002c240: 6420 3d20 2770 7269 7661 7465 5075 7447  d = 'privatePutG
-0002c250: 506f 7369 7469 6f6e 734c 6576 6572 6167  PositionsLeverag
-0002c260: 6527 0a20 2020 2020 2020 2020 2020 2072  e'.            r
-0002c270: 6571 7565 7374 5b27 6c65 7665 7261 6765  equest['leverage
-0002c280: 5272 275d 203d 206c 6576 6572 6167 650a  Rr'] = leverage.
-0002c290: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002c2a0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0002c2b0: 745b 276c 6576 6572 6167 6527 5d20 3d20  t['leverage'] = 
-0002c2c0: 6c65 7665 7261 6765 0a20 2020 2020 2020  leverage.       
-0002c2d0: 2072 6574 7572 6e20 6765 7461 7474 7228   return getattr(
-0002c2e0: 7365 6c66 2c20 6d65 7468 6f64 2928 7365  self, method)(se
-0002c2f0: 6c66 2e65 7874 656e 6428 7265 7175 6573  lf.extend(reques
-0002c300: 742c 2070 6172 616d 7329 290a 0a20 2020  t, params))..   
-0002c310: 2064 6566 2074 7261 6e73 6665 7228 7365   def transfer(se
-0002c320: 6c66 2c20 636f 6465 3a20 7374 722c 2061  lf, code: str, a
-0002c330: 6d6f 756e 742c 2066 726f 6d41 6363 6f75  mount, fromAccou
-0002c340: 6e74 2c20 746f 4163 636f 756e 742c 2070  nt, toAccount, p
-0002c350: 6172 616d 733d 7b7d 293a 0a20 2020 2020  arams={}):.     
-0002c360: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-0002c370: 7261 6e73 6665 7220 6375 7272 656e 6379  ransfer currency
-0002c380: 2069 6e74 6572 6e61 6c6c 7920 6265 7477   internally betw
-0002c390: 6565 6e20 7761 6c6c 6574 7320 6f6e 2074  een wallets on t
-0002c3a0: 6865 2073 616d 6520 6163 636f 756e 740a  he same account.
-0002c3b0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0002c3c0: 7472 2063 6f64 653a 2075 6e69 6669 6564  tr code: unified
-0002c3d0: 2063 7572 7265 6e63 7920 636f 6465 0a20   currency code. 
-0002c3e0: 2020 2020 2020 203a 7061 7261 6d20 666c         :param fl
-0002c3f0: 6f61 7420 616d 6f75 6e74 3a20 616d 6f75  oat amount: amou
-0002c400: 6e74 2074 6f20 7472 616e 7366 6572 0a20  nt to transfer. 
-0002c410: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-0002c420: 7220 6672 6f6d 4163 636f 756e 743a 2061  r fromAccount: a
-0002c430: 6363 6f75 6e74 2074 6f20 7472 616e 7366  ccount to transf
-0002c440: 6572 2066 726f 6d0a 2020 2020 2020 2020  er from.        
-0002c450: 3a70 6172 616d 2073 7472 2074 6f41 6363  :param str toAcc
-0002c460: 6f75 6e74 3a20 6163 636f 756e 7420 746f  ount: account to
-0002c470: 2074 7261 6e73 6665 7220 746f 0a20 2020   transfer to.   
-0002c480: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
-0002c490: 2070 6172 616d 733a 2065 7874 7261 2070   params: extra p
-0002c4a0: 6172 616d 6574 6572 7320 7370 6563 6966  arameters specif
-0002c4b0: 6963 2074 6f20 7468 6520 7068 656d 6578  ic to the phemex
-0002c4c0: 2061 7069 2065 6e64 706f 696e 740a 2020   api endpoint.  
-0002c4d0: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-0002c4e0: 7c4e 6f6e 6520 7061 7261 6d73 5b27 6269  |None params['bi
-0002c4f0: 7a54 7970 6527 5d3a 2066 6f72 2074 7261  zType']: for tra
-0002c500: 6e73 6665 7272 696e 6720 6265 7477 6565  nsferring betwee
-0002c510: 6e20 6d61 696e 2061 6e64 2073 7562 2d61  n main and sub-a
-0002c520: 636f 756e 7473 2065 6974 6865 7220 2753  counts either 'S
-0002c530: 504f 5427 206f 7220 2750 4552 5045 5455  POT' or 'PERPETU
-0002c540: 414c 2720 6465 6661 756c 7420 6973 2027  AL' default is '
-0002c550: 5350 4f54 270a 2020 2020 2020 2020 3a72  SPOT'.        :r
-0002c560: 6574 7572 6e73 2064 6963 743a 2061 2060  eturns dict: a `
-0002c570: 7472 616e 7366 6572 2073 7472 7563 7475  transfer structu
-0002c580: 7265 203c 6874 7470 733a 2f2f 646f 6373  re <https://docs
-0002c590: 2e63 6378 742e 636f 6d2f 232f 3f69 643d  .ccxt.com/#/?id=
-0002c5a0: 7472 616e 7366 6572 2d73 7472 7563 7475  transfer-structu
-0002c5b0: 7265 3e60 0a20 2020 2020 2020 2022 2222  re>`.        """
-0002c5c0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-0002c5d0: 6164 5f6d 6172 6b65 7473 2829 0a20 2020  ad_markets().   
-0002c5e0: 2020 2020 2063 7572 7265 6e63 7920 3d20       currency = 
-0002c5f0: 7365 6c66 2e63 7572 7265 6e63 7928 636f  self.currency(co
-0002c600: 6465 290a 2020 2020 2020 2020 6163 636f  de).        acco
-0002c610: 756e 7473 4279 5479 7065 203d 2073 656c  untsByType = sel
-0002c620: 662e 7361 6665 5f76 616c 7565 2873 656c  f.safe_value(sel
-0002c630: 662e 6f70 7469 6f6e 732c 2027 6163 636f  f.options, 'acco
-0002c640: 756e 7473 4279 5479 7065 272c 207b 7d29  untsByType', {})
-0002c650: 0a20 2020 2020 2020 2066 726f 6d49 6420  .        fromId 
-0002c660: 3d20 7365 6c66 2e73 6166 655f 7374 7269  = self.safe_stri
-0002c670: 6e67 2861 6363 6f75 6e74 7342 7954 7970  ng(accountsByTyp
-0002c680: 652c 2066 726f 6d41 6363 6f75 6e74 2c20  e, fromAccount, 
-0002c690: 6672 6f6d 4163 636f 756e 7429 0a20 2020  fromAccount).   
-0002c6a0: 2020 2020 2074 6f49 6420 3d20 7365 6c66       toId = self
-0002c6b0: 2e73 6166 655f 7374 7269 6e67 2861 6363  .safe_string(acc
-0002c6c0: 6f75 6e74 7342 7954 7970 652c 2074 6f41  ountsByType, toA
-0002c6d0: 6363 6f75 6e74 2c20 746f 4163 636f 756e  ccount, toAccoun
-0002c6e0: 7429 0a20 2020 2020 2020 2073 6361 6c65  t).        scale
-0002c6f0: 6441 6d6d 6f75 6e74 203d 2073 656c 662e  dAmmount = self.
-0002c700: 746f 5f65 7628 616d 6f75 6e74 2c20 6375  to_ev(amount, cu
-0002c710: 7272 656e 6379 290a 2020 2020 2020 2020  rrency).        
-0002c720: 6469 7265 6374 696f 6e20 3d20 4e6f 6e65  direction = None
-0002c730: 0a20 2020 2020 2020 2074 7261 6e73 6665  .        transfe
-0002c740: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
-0002c750: 2069 6620 6672 6f6d 4964 203d 3d20 2773   if fromId == 's
-0002c760: 706f 7427 2061 6e64 2074 6f49 6420 3d3d  pot' and toId ==
-0002c770: 2027 6675 7475 7265 273a 0a20 2020 2020   'future':.     
-0002c780: 2020 2020 2020 2064 6972 6563 7469 6f6e         direction
-0002c790: 203d 2032 0a20 2020 2020 2020 2065 6c69   = 2.        eli
-0002c7a0: 6620 6672 6f6d 4964 203d 3d20 2766 7574  f fromId == 'fut
-0002c7b0: 7572 6527 2061 6e64 2074 6f49 6420 3d3d  ure' and toId ==
-0002c7c0: 2027 7370 6f74 273a 0a20 2020 2020 2020   'spot':.       
-0002c7d0: 2020 2020 2064 6972 6563 7469 6f6e 203d       direction =
-0002c7e0: 2031 0a20 2020 2020 2020 2069 6620 6469   1.        if di
-0002c7f0: 7265 6374 696f 6e20 6973 206e 6f74 204e  rection is not N
-0002c800: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002c810: 2072 6571 7565 7374 203d 207b 0a20 2020   request = {.   
-0002c820: 2020 2020 2020 2020 2020 2020 2027 6375               'cu
-0002c830: 7272 656e 6379 273a 2063 7572 7265 6e63  rrency': currenc
-0002c840: 795b 2769 6427 5d2c 0a20 2020 2020 2020  y['id'],.       
-0002c850: 2020 2020 2020 2020 2027 6d6f 7665 4f70           'moveOp
-0002c860: 273a 2064 6972 6563 7469 6f6e 2c0a 2020  ': direction,.  
-0002c870: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-0002c880: 6d6f 756e 7445 7627 3a20 7363 616c 6564  mountEv': scaled
-0002c890: 416d 6d6f 756e 742c 0a20 2020 2020 2020  Ammount,.       
-0002c8a0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-0002c8b0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-0002c8c0: 6c66 2e70 7269 7661 7465 506f 7374 4173  lf.privatePostAs
-0002c8d0: 7365 7473 5472 616e 7366 6572 2873 656c  setsTransfer(sel
-0002c8e0: 662e 6578 7465 6e64 2872 6571 7565 7374  f.extend(request
-0002c8f0: 2c20 7061 7261 6d73 2929 0a20 2020 2020  , params)).     
-0002c900: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-0002c910: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
-0002c920: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-0002c930: 2020 2063 6f64 653a 2027 3027 2c0a 2020     code: '0',.  
-0002c940: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-0002c950: 2020 2020 6d73 673a 2027 4f4b 272c 0a20      msg: 'OK',. 
-0002c960: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-0002c970: 2020 2020 2064 6174 613a 207b 0a20 2020       data: {.   
-0002c980: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-0002c990: 2020 2020 2020 206c 696e 6b4b 6579 3a20         linkKey: 
-0002c9a0: 2738 3536 3465 6261 342d 6339 6563 2d34  '8564eba4-c9ec-4
-0002c9b0: 3964 362d 3962 3863 2d32 6563 3530 3031  9d6-9b8c-2ec5001
-0002c9c0: 6130 6662 3927 2c0a 2020 2020 2020 2020  a0fb9',.        
-0002c9d0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0002c9e0: 2020 7573 6572 4964 3a20 2734 3031 3833    userId: '40183
-0002c9f0: 3430 272c 0a20 2020 2020 2020 2020 2020  40',.           
-0002ca00: 2023 2020 2020 2020 2020 2020 2020 2063   #             c
-0002ca10: 7572 7265 6e63 793a 2027 5553 4427 2c0a  urrency: 'USD',.
-0002ca20: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0002ca30: 2020 2020 2020 2020 2020 616d 6f75 6e74            amount
-0002ca40: 4576 3a20 2731 3027 2c0a 2020 2020 2020  Ev: '10',.      
-0002ca50: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0002ca60: 2020 2020 7369 6465 3a20 2732 272c 0a20      side: '2',. 
-0002ca70: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-0002ca80: 2020 2020 2020 2020 2073 7461 7475 733a           status:
-0002ca90: 2027 3130 270a 2020 2020 2020 2020 2020   '10'.          
-0002caa0: 2020 2320 2020 2020 2020 2020 7d0a 2020    #         }.  
-0002cab0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-0002cac0: 7d0a 2020 2020 2020 2020 2020 2020 230a  }.            #.
-0002cad0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0002cae0: 203d 2073 656c 662e 7361 6665 5f76 616c   = self.safe_val
-0002caf0: 7565 2872 6573 706f 6e73 652c 2027 6461  ue(response, 'da
-0002cb00: 7461 272c 207b 7d29 0a20 2020 2020 2020  ta', {}).       
-0002cb10: 2020 2020 2074 7261 6e73 6665 7220 3d20       transfer = 
-0002cb20: 7365 6c66 2e70 6172 7365 5f74 7261 6e73  self.parse_trans
-0002cb30: 6665 7228 6461 7461 2c20 6375 7272 656e  fer(data, curren
-0002cb40: 6379 290a 2020 2020 2020 2020 656c 7365  cy).        else
-0002cb50: 3a20 2023 2073 7562 2061 6363 6f75 6e74  :  # sub account
-0002cb60: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
-0002cb70: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
-0002cb80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0002cb90: 2020 2766 726f 6d55 7365 7249 6427 3a20    'fromUserId': 
-0002cba0: 6672 6f6d 4964 2c0a 2020 2020 2020 2020  fromId,.        
-0002cbb0: 2020 2020 2020 2020 2774 6f55 7365 7249          'toUserI
-0002cbc0: 6427 3a20 746f 4964 2c0a 2020 2020 2020  d': toId,.      
-0002cbd0: 2020 2020 2020 2020 2020 2761 6d6f 756e            'amoun
-0002cbe0: 7445 7627 3a20 7363 616c 6564 416d 6d6f  tEv': scaledAmmo
-0002cbf0: 756e 742c 0a20 2020 2020 2020 2020 2020  unt,.           
-0002cc00: 2020 2020 2027 6375 7272 656e 6379 273a       'currency':
-0002cc10: 2063 7572 7265 6e63 795b 2769 6427 5d2c   currency['id'],
-0002cc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002cc30: 2027 6269 7a54 7970 6527 3a20 7365 6c66   'bizType': self
-0002cc40: 2e73 6166 655f 7374 7269 6e67 2870 6172  .safe_string(par
-0002cc50: 616d 732c 2027 6269 7a54 7970 6527 2c20  ams, 'bizType', 
-0002cc60: 2753 504f 5427 292c 0a20 2020 2020 2020  'SPOT'),.       
-0002cc70: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-0002cc80: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-0002cc90: 6c66 2e70 7269 7661 7465 506f 7374 4173  lf.privatePostAs
-0002cca0: 7365 7473 556e 6976 6572 7361 6c54 7261  setsUniversalTra
+0002bf70: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0002bf80: 626f 6f6c 2070 6172 616d 735b 2768 6564  bool params['hed
+0002bf90: 6765 6427 5d3a 2073 6574 2074 6f20 5472  ged']: set to Tr
+0002bfa0: 7565 2069 6620 6865 6467 6564 2070 6f73  ue if hedged pos
+0002bfb0: 6974 696f 6e20 6d6f 6465 2069 7320 656e  ition mode is en
+0002bfc0: 6162 6c65 6428 6279 2064 6566 6175 6c74  abled(by default
+0002bfd0: 206c 6f6e 6720 616e 6420 7368 6f72 7420   long and short 
+0002bfe0: 6c65 7665 7261 6765 2061 7265 2073 6574  leverage are set
+0002bff0: 2074 6f20 7468 6520 7361 6d65 2076 616c   to the same val
+0002c000: 7565 290a 2020 2020 2020 2020 3a70 6172  ue).        :par
+0002c010: 616d 2066 6c6f 6174 2070 6172 616d 735b  am float params[
+0002c020: 276c 6f6e 674c 6576 6572 6167 6552 7227  'longLeverageRr'
+0002c030: 5d3a 202a 6865 6467 6564 206d 6f64 6520  ]: *hedged mode 
+0002c040: 6f6e 6c79 2a20 7365 7420 7468 6520 6c65  only* set the le
+0002c050: 7665 7261 6765 2066 6f72 206c 6f6e 6720  verage for long 
+0002c060: 706f 7369 7469 6f6e 730a 2020 2020 2020  positions.      
+0002c070: 2020 3a70 6172 616d 2066 6c6f 6174 2070    :param float p
+0002c080: 6172 616d 735b 2773 686f 7274 4c65 7665  arams['shortLeve
+0002c090: 7261 6765 5272 275d 3a20 2a68 6564 6765  rageRr']: *hedge
+0002c0a0: 6420 6d6f 6465 206f 6e6c 792a 2073 6574  d mode only* set
+0002c0b0: 2074 6865 206c 6576 6572 6167 6520 666f   the leverage fo
+0002c0c0: 7220 7368 6f72 7420 706f 7369 7469 6f6e  r short position
+0002c0d0: 730a 2020 2020 2020 2020 3a72 6574 7572  s.        :retur
+0002c0e0: 6e73 2064 6963 743a 2072 6573 706f 6e73  ns dict: respons
+0002c0f0: 6520 6672 6f6d 2074 6865 2065 7863 6861  e from the excha
+0002c100: 6e67 650a 2020 2020 2020 2020 2222 220a  nge.        """.
+0002c110: 2020 2020 2020 2020 2320 5741 524e 494e          # WARNIN
+0002c120: 473a 2054 4849 5320 5749 4c4c 2049 4e43  G: THIS WILL INC
+0002c130: 5245 4153 4520 4c49 5155 4944 4154 494f  REASE LIQUIDATIO
+0002c140: 4e20 5052 4943 4520 464f 5220 4f50 454e  N PRICE FOR OPEN
+0002c150: 2049 534f 4c41 5445 4420 4c4f 4e47 2050   ISOLATED LONG P
+0002c160: 4f53 4954 494f 4e53 0a20 2020 2020 2020  OSITIONS.       
+0002c170: 2023 2041 4e44 2044 4543 5245 4153 4520   # AND DECREASE 
+0002c180: 4c49 5155 4944 4154 494f 4e20 5052 4943  LIQUIDATION PRIC
+0002c190: 4520 464f 5220 4f50 454e 2049 534f 4c41  E FOR OPEN ISOLA
+0002c1a0: 5445 4420 5348 4f52 5420 504f 5349 5449  TED SHORT POSITI
+0002c1b0: 4f4e 530a 2020 2020 2020 2020 6966 2073  ONS.        if s
+0002c1c0: 796d 626f 6c20 6973 204e 6f6e 653a 0a20  ymbol is None:. 
+0002c1d0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0002c1e0: 2041 7267 756d 656e 7473 5265 7175 6972   ArgumentsRequir
+0002c1f0: 6564 2873 656c 662e 6964 202b 2027 2073  ed(self.id + ' s
+0002c200: 6574 4c65 7665 7261 6765 2829 2072 6571  etLeverage() req
+0002c210: 7569 7265 7320 6120 7379 6d62 6f6c 2061  uires a symbol a
+0002c220: 7267 756d 656e 7427 290a 2020 2020 2020  rgument').      
+0002c230: 2020 6966 2028 6c65 7665 7261 6765 203c    if (leverage <
+0002c240: 2031 2920 6f72 2028 6c65 7665 7261 6765   1) or (leverage
+0002c250: 203e 2031 3030 293a 0a20 2020 2020 2020   > 100):.       
+0002c260: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
+0002c270: 7175 6573 7428 7365 6c66 2e69 6420 2b20  quest(self.id + 
+0002c280: 2720 7365 744c 6576 6572 6167 6528 2920  ' setLeverage() 
+0002c290: 6c65 7665 7261 6765 2073 686f 756c 6420  leverage should 
+0002c2a0: 6265 2062 6574 7765 656e 2031 2061 6e64  be between 1 and
+0002c2b0: 2031 3030 2729 0a20 2020 2020 2020 2073   100').        s
+0002c2c0: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+0002c2d0: 2829 0a20 2020 2020 2020 2069 7348 6564  ().        isHed
+0002c2e0: 6765 6420 3d20 7365 6c66 2e73 6166 655f  ged = self.safe_
+0002c2f0: 7661 6c75 6528 7061 7261 6d73 2c20 2768  value(params, 'h
+0002c300: 6564 6765 6427 2c20 4661 6c73 6529 0a20  edged', False). 
+0002c310: 2020 2020 2020 206c 6f6e 674c 6576 6572         longLever
+0002c320: 6167 6552 7220 3d20 7365 6c66 2e73 6166  ageRr = self.saf
+0002c330: 655f 696e 7465 6765 7228 7061 7261 6d73  e_integer(params
+0002c340: 2c20 276c 6f6e 674c 6576 6572 6167 6552  , 'longLeverageR
+0002c350: 7227 290a 2020 2020 2020 2020 7368 6f72  r').        shor
+0002c360: 744c 6576 6572 6167 6552 7220 3d20 7365  tLeverageRr = se
+0002c370: 6c66 2e73 6166 655f 696e 7465 6765 7228  lf.safe_integer(
+0002c380: 7061 7261 6d73 2c20 2773 686f 7274 4c65  params, 'shortLe
+0002c390: 7665 7261 6765 5272 2729 0a20 2020 2020  verageRr').     
+0002c3a0: 2020 206d 6172 6b65 7420 3d20 7365 6c66     market = self
+0002c3b0: 2e6d 6172 6b65 7428 7379 6d62 6f6c 290a  .market(symbol).
+0002c3c0: 2020 2020 2020 2020 7265 7175 6573 7420          request 
+0002c3d0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0002c3e0: 2773 796d 626f 6c27 3a20 6d61 726b 6574  'symbol': market
+0002c3f0: 5b27 6964 275d 2c0a 2020 2020 2020 2020  ['id'],.        
+0002c400: 7d0a 2020 2020 2020 2020 7265 7370 6f6e  }.        respon
+0002c410: 7365 203d 204e 6f6e 650a 2020 2020 2020  se = None.      
+0002c420: 2020 6966 206d 6172 6b65 745b 2773 6574    if market['set
+0002c430: 746c 6527 5d20 3d3d 2027 5553 4454 273a  tle'] == 'USDT':
+0002c440: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0002c450: 6e6f 7420 6973 4865 6467 6564 2061 6e64  not isHedged and
+0002c460: 206c 6f6e 674c 6576 6572 6167 6552 7220   longLeverageRr 
+0002c470: 6973 204e 6f6e 6520 616e 6420 7368 6f72  is None and shor
+0002c480: 744c 6576 6572 6167 6552 7220 6973 204e  tLeverageRr is N
+0002c490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c4a0: 2020 2020 2072 6571 7565 7374 5b27 6c65       request['le
+0002c4b0: 7665 7261 6765 5272 275d 203d 206c 6576  verageRr'] = lev
+0002c4c0: 6572 6167 650a 2020 2020 2020 2020 2020  erage.          
+0002c4d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002c4e0: 2020 2020 2020 2020 6c6f 6e67 203d 206c          long = l
+0002c4f0: 6f6e 674c 6576 6572 6167 6552 7220 6966  ongLeverageRr if
+0002c500: 2028 6c6f 6e67 4c65 7665 7261 6765 5272   (longLeverageRr
+0002c510: 2069 7320 6e6f 7420 4e6f 6e65 2920 656c   is not None) el
+0002c520: 7365 206c 6576 6572 6167 650a 2020 2020  se leverage.    
+0002c530: 2020 2020 2020 2020 2020 2020 7368 6f72              shor
+0002c540: 7420 3d20 7368 6f72 744c 6576 6572 6167  t = shortLeverag
+0002c550: 6552 7220 6966 2028 7368 6f72 744c 6576  eRr if (shortLev
+0002c560: 6572 6167 6552 7220 6973 206e 6f74 204e  erageRr is not N
+0002c570: 6f6e 6529 2065 6c73 6520 6c65 7665 7261  one) else levera
+0002c580: 6765 0a20 2020 2020 2020 2020 2020 2020  ge.             
+0002c590: 2020 2072 6571 7565 7374 5b27 6c6f 6e67     request['long
+0002c5a0: 4c65 7665 7261 6765 5272 275d 203d 206c  LeverageRr'] = l
+0002c5b0: 6f6e 670a 2020 2020 2020 2020 2020 2020  ong.            
+0002c5c0: 2020 2020 7265 7175 6573 745b 2773 686f      request['sho
+0002c5d0: 7274 4c65 7665 7261 6765 5272 275d 203d  rtLeverageRr'] =
+0002c5e0: 2073 686f 7274 0a20 2020 2020 2020 2020   short.         
+0002c5f0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+0002c600: 6c66 2e70 7269 7661 7465 5075 7447 506f  lf.privatePutGPo
+0002c610: 7369 7469 6f6e 734c 6576 6572 6167 6528  sitionsLeverage(
+0002c620: 7365 6c66 2e65 7874 656e 6428 7265 7175  self.extend(requ
+0002c630: 6573 742c 2070 6172 616d 7329 290a 2020  est, params)).  
+0002c640: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0002c650: 2020 2020 2020 2020 7265 7175 6573 745b          request[
+0002c660: 276c 6576 6572 6167 6527 5d20 3d20 6c65  'leverage'] = le
+0002c670: 7665 7261 6765 0a20 2020 2020 2020 2020  verage.         
+0002c680: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+0002c690: 6c66 2e70 7269 7661 7465 5075 7450 6f73  lf.privatePutPos
+0002c6a0: 6974 696f 6e73 4c65 7665 7261 6765 2873  itionsLeverage(s
+0002c6b0: 656c 662e 6578 7465 6e64 2872 6571 7565  elf.extend(reque
+0002c6c0: 7374 2c20 7061 7261 6d73 2929 0a20 2020  st, params)).   
+0002c6d0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0002c6e0: 6f6e 7365 0a0a 2020 2020 6465 6620 7472  onse..    def tr
+0002c6f0: 616e 7366 6572 2873 656c 662c 2063 6f64  ansfer(self, cod
+0002c700: 653a 2073 7472 2c20 616d 6f75 6e74 2c20  e: str, amount, 
+0002c710: 6672 6f6d 4163 636f 756e 742c 2074 6f41  fromAccount, toA
+0002c720: 6363 6f75 6e74 2c20 7061 7261 6d73 3d7b  ccount, params={
+0002c730: 7d29 3a0a 2020 2020 2020 2020 2222 220a  }):.        """.
+0002c740: 2020 2020 2020 2020 7472 616e 7366 6572          transfer
+0002c750: 2063 7572 7265 6e63 7920 696e 7465 726e   currency intern
+0002c760: 616c 6c79 2062 6574 7765 656e 2077 616c  ally between wal
+0002c770: 6c65 7473 206f 6e20 7468 6520 7361 6d65  lets on the same
+0002c780: 2061 6363 6f75 6e74 0a20 2020 2020 2020   account.       
+0002c790: 203a 7061 7261 6d20 7374 7220 636f 6465   :param str code
+0002c7a0: 3a20 756e 6966 6965 6420 6375 7272 656e  : unified curren
+0002c7b0: 6379 2063 6f64 650a 2020 2020 2020 2020  cy code.        
+0002c7c0: 3a70 6172 616d 2066 6c6f 6174 2061 6d6f  :param float amo
+0002c7d0: 756e 743a 2061 6d6f 756e 7420 746f 2074  unt: amount to t
+0002c7e0: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
+0002c7f0: 3a70 6172 616d 2073 7472 2066 726f 6d41  :param str fromA
+0002c800: 6363 6f75 6e74 3a20 6163 636f 756e 7420  ccount: account 
+0002c810: 746f 2074 7261 6e73 6665 7220 6672 6f6d  to transfer from
+0002c820: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0002c830: 7374 7220 746f 4163 636f 756e 743a 2061  str toAccount: a
+0002c840: 6363 6f75 6e74 2074 6f20 7472 616e 7366  ccount to transf
+0002c850: 6572 2074 6f0a 2020 2020 2020 2020 3a70  er to.        :p
+0002c860: 6172 616d 2064 6963 7420 7061 7261 6d73  aram dict params
+0002c870: 3a20 6578 7472 6120 7061 7261 6d65 7465  : extra paramete
+0002c880: 7273 2073 7065 6369 6669 6320 746f 2074  rs specific to t
+0002c890: 6865 2070 6865 6d65 7820 6170 6920 656e  he phemex api en
+0002c8a0: 6470 6f69 6e74 0a20 2020 2020 2020 203a  dpoint.        :
+0002c8b0: 7061 7261 6d20 7374 727c 4e6f 6e65 2070  param str|None p
+0002c8c0: 6172 616d 735b 2762 697a 5479 7065 275d  arams['bizType']
+0002c8d0: 3a20 666f 7220 7472 616e 7366 6572 7269  : for transferri
+0002c8e0: 6e67 2062 6574 7765 656e 206d 6169 6e20  ng between main 
+0002c8f0: 616e 6420 7375 622d 6163 6f75 6e74 7320  and sub-acounts 
+0002c900: 6569 7468 6572 2027 5350 4f54 2720 6f72  either 'SPOT' or
+0002c910: 2027 5045 5250 4554 5541 4c27 2064 6566   'PERPETUAL' def
+0002c920: 6175 6c74 2069 7320 2753 504f 5427 0a20  ault is 'SPOT'. 
+0002c930: 2020 2020 2020 203a 7265 7475 726e 7320         :returns 
+0002c940: 6469 6374 3a20 6120 6074 7261 6e73 6665  dict: a `transfe
+0002c950: 7220 7374 7275 6374 7572 6520 3c68 7474  r structure <htt
+0002c960: 7073 3a2f 2f64 6f63 732e 6363 7874 2e63  ps://docs.ccxt.c
+0002c970: 6f6d 2f23 2f3f 6964 3d74 7261 6e73 6665  om/#/?id=transfe
+0002c980: 722d 7374 7275 6374 7572 653e 600a 2020  r-structure>`.  
+0002c990: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002c9a0: 2020 7365 6c66 2e6c 6f61 645f 6d61 726b    self.load_mark
+0002c9b0: 6574 7328 290a 2020 2020 2020 2020 6375  ets().        cu
+0002c9c0: 7272 656e 6379 203d 2073 656c 662e 6375  rrency = self.cu
+0002c9d0: 7272 656e 6379 2863 6f64 6529 0a20 2020  rrency(code).   
+0002c9e0: 2020 2020 2061 6363 6f75 6e74 7342 7954       accountsByT
+0002c9f0: 7970 6520 3d20 7365 6c66 2e73 6166 655f  ype = self.safe_
+0002ca00: 7661 6c75 6528 7365 6c66 2e6f 7074 696f  value(self.optio
+0002ca10: 6e73 2c20 2761 6363 6f75 6e74 7342 7954  ns, 'accountsByT
+0002ca20: 7970 6527 2c20 7b7d 290a 2020 2020 2020  ype', {}).      
+0002ca30: 2020 6672 6f6d 4964 203d 2073 656c 662e    fromId = self.
+0002ca40: 7361 6665 5f73 7472 696e 6728 6163 636f  safe_string(acco
+0002ca50: 756e 7473 4279 5479 7065 2c20 6672 6f6d  untsByType, from
+0002ca60: 4163 636f 756e 742c 2066 726f 6d41 6363  Account, fromAcc
+0002ca70: 6f75 6e74 290a 2020 2020 2020 2020 746f  ount).        to
+0002ca80: 4964 203d 2073 656c 662e 7361 6665 5f73  Id = self.safe_s
+0002ca90: 7472 696e 6728 6163 636f 756e 7473 4279  tring(accountsBy
+0002caa0: 5479 7065 2c20 746f 4163 636f 756e 742c  Type, toAccount,
+0002cab0: 2074 6f41 6363 6f75 6e74 290a 2020 2020   toAccount).    
+0002cac0: 2020 2020 7363 616c 6564 416d 6d6f 756e      scaledAmmoun
+0002cad0: 7420 3d20 7365 6c66 2e74 6f5f 6576 2861  t = self.to_ev(a
+0002cae0: 6d6f 756e 742c 2063 7572 7265 6e63 7929  mount, currency)
+0002caf0: 0a20 2020 2020 2020 2064 6972 6563 7469  .        directi
+0002cb00: 6f6e 203d 204e 6f6e 650a 2020 2020 2020  on = None.      
+0002cb10: 2020 7472 616e 7366 6572 203d 204e 6f6e    transfer = Non
+0002cb20: 650a 2020 2020 2020 2020 6966 2066 726f  e.        if fro
+0002cb30: 6d49 6420 3d3d 2027 7370 6f74 2720 616e  mId == 'spot' an
+0002cb40: 6420 746f 4964 203d 3d20 2766 7574 7572  d toId == 'futur
+0002cb50: 6527 3a0a 2020 2020 2020 2020 2020 2020  e':.            
+0002cb60: 6469 7265 6374 696f 6e20 3d20 320a 2020  direction = 2.  
+0002cb70: 2020 2020 2020 656c 6966 2066 726f 6d49        elif fromI
+0002cb80: 6420 3d3d 2027 6675 7475 7265 2720 616e  d == 'future' an
+0002cb90: 6420 746f 4964 203d 3d20 2773 706f 7427  d toId == 'spot'
+0002cba0: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
+0002cbb0: 7265 6374 696f 6e20 3d20 310a 2020 2020  rection = 1.    
+0002cbc0: 2020 2020 6966 2064 6972 6563 7469 6f6e      if direction
+0002cbd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002cbe0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+0002cbf0: 7420 3d20 7b0a 2020 2020 2020 2020 2020  t = {.          
+0002cc00: 2020 2020 2020 2763 7572 7265 6e63 7927        'currency'
+0002cc10: 3a20 6375 7272 656e 6379 5b27 6964 275d  : currency['id']
+0002cc20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002cc30: 2020 276d 6f76 654f 7027 3a20 6469 7265    'moveOp': dire
+0002cc40: 6374 696f 6e2c 0a20 2020 2020 2020 2020  ction,.         
+0002cc50: 2020 2020 2020 2027 616d 6f75 6e74 4576         'amountEv
+0002cc60: 273a 2073 6361 6c65 6441 6d6d 6f75 6e74  ': scaledAmmount
+0002cc70: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+0002cc80: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0002cc90: 6f6e 7365 203d 2073 656c 662e 7072 6976  onse = self.priv
+0002cca0: 6174 6550 6f73 7441 7373 6574 7354 7261  atePostAssetsTra
 0002ccb0: 6e73 6665 7228 7365 6c66 2e65 7874 656e  nsfer(self.exten
 0002ccc0: 6428 7265 7175 6573 742c 2070 6172 616d  d(request, param
 0002ccd0: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
 0002cce0: 230a 2020 2020 2020 2020 2020 2020 2320  #.            # 
 0002ccf0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
 0002cd00: 2020 2320 2020 2020 2020 2020 636f 6465    #         code
 0002cd10: 3a20 2730 272c 0a20 2020 2020 2020 2020  : '0',.         
 0002cd20: 2020 2023 2020 2020 2020 2020 206d 7367     #         msg
 0002cd30: 3a20 274f 4b27 2c0a 2020 2020 2020 2020  : 'OK',.        
 0002cd40: 2020 2020 2320 2020 2020 2020 2020 6461      #         da
-0002cd50: 7461 3a20 2741 5049 2d39 3233 6462 3832  ta: 'API-923db82
-0002cd60: 362d 6161 6161 2d61 6161 612d 6161 6161  6-aaaa-aaaa-aaaa
-0002cd70: 2d34 6439 3863 3361 3763 3966 6427 0a20  -4d98c3a7c9fd'. 
-0002cd80: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-0002cd90: 207d 0a20 2020 2020 2020 2020 2020 2023   }.            #
-0002cda0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-0002cdb0: 6e73 6665 7220 3d20 7365 6c66 2e70 6172  nsfer = self.par
-0002cdc0: 7365 5f74 7261 6e73 6665 7228 7265 7370  se_transfer(resp
-0002cdd0: 6f6e 7365 290a 2020 2020 2020 2020 7472  onse).        tr
-0002cde0: 616e 7366 6572 4f70 7469 6f6e 7320 3d20  ansferOptions = 
-0002cdf0: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0002ce00: 7365 6c66 2e6f 7074 696f 6e73 2c20 2774  self.options, 't
-0002ce10: 7261 6e73 6665 7227 2c20 7b7d 290a 2020  ransfer', {}).  
-0002ce20: 2020 2020 2020 6669 6c6c 5265 7370 6f6e        fillRespon
-0002ce30: 7365 4672 6f6d 5265 7175 6573 7420 3d20  seFromRequest = 
-0002ce40: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0002ce50: 7472 616e 7366 6572 4f70 7469 6f6e 732c  transferOptions,
-0002ce60: 2027 6669 6c6c 5265 7370 6f6e 7365 4672   'fillResponseFr
-0002ce70: 6f6d 5265 7175 6573 7427 2c20 5472 7565  omRequest', True
-0002ce80: 290a 2020 2020 2020 2020 6966 2066 696c  ).        if fil
-0002ce90: 6c52 6573 706f 6e73 6546 726f 6d52 6571  lResponseFromReq
-0002cea0: 7565 7374 3a0a 2020 2020 2020 2020 2020  uest:.          
-0002ceb0: 2020 6966 2074 7261 6e73 6665 725b 2766    if transfer['f
-0002cec0: 726f 6d41 6363 6f75 6e74 275d 2069 7320  romAccount'] is 
-0002ced0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002cee0: 2020 2020 2020 7472 616e 7366 6572 5b27        transfer['
-0002cef0: 6672 6f6d 4163 636f 756e 7427 5d20 3d20  fromAccount'] = 
-0002cf00: 6672 6f6d 4163 636f 756e 740a 2020 2020  fromAccount.    
-0002cf10: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
-0002cf20: 6665 725b 2774 6f41 6363 6f75 6e74 275d  fer['toAccount']
-0002cf30: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0002cf40: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-0002cf50: 6572 5b27 746f 4163 636f 756e 7427 5d20  er['toAccount'] 
-0002cf60: 3d20 746f 4163 636f 756e 740a 2020 2020  = toAccount.    
-0002cf70: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
-0002cf80: 6665 725b 2761 6d6f 756e 7427 5d20 6973  fer['amount'] is
-0002cf90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002cfa0: 2020 2020 2020 2074 7261 6e73 6665 725b         transfer[
-0002cfb0: 2761 6d6f 756e 7427 5d20 3d20 616d 6f75  'amount'] = amou
-0002cfc0: 6e74 0a20 2020 2020 2020 2020 2020 2069  nt.            i
-0002cfd0: 6620 7472 616e 7366 6572 5b27 6375 7272  f transfer['curr
-0002cfe0: 656e 6379 275d 2069 7320 4e6f 6e65 3a0a  ency'] is None:.
-0002cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d000: 7472 616e 7366 6572 5b27 6375 7272 656e  transfer['curren
-0002d010: 6379 275d 203d 2063 6f64 650a 2020 2020  cy'] = code.    
-0002d020: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
-0002d030: 6665 720a 0a20 2020 2064 6566 2066 6574  fer..    def fet
-0002d040: 6368 5f74 7261 6e73 6665 7273 2873 656c  ch_transfers(sel
-0002d050: 662c 2063 6f64 653a 204f 7074 696f 6e61  f, code: Optiona
-0002d060: 6c5b 7374 725d 203d 204e 6f6e 652c 2073  l[str] = None, s
-0002d070: 696e 6365 3a20 4f70 7469 6f6e 616c 5b69  ince: Optional[i
-0002d080: 6e74 5d20 3d20 4e6f 6e65 2c20 6c69 6d69  nt] = None, limi
-0002d090: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
-0002d0a0: 203d 204e 6f6e 652c 2070 6172 616d 733d   = None, params=
-0002d0b0: 7b7d 293a 0a20 2020 2020 2020 2022 2222  {}):.        """
-0002d0c0: 0a20 2020 2020 2020 2066 6574 6368 2061  .        fetch a
-0002d0d0: 2068 6973 746f 7279 206f 6620 696e 7465   history of inte
-0002d0e0: 726e 616c 2074 7261 6e73 6665 7273 206d  rnal transfers m
-0002d0f0: 6164 6520 6f6e 2061 6e20 6163 636f 756e  ade on an accoun
-0002d100: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-0002d110: 2073 7472 7c4e 6f6e 6520 636f 6465 3a20   str|None code: 
-0002d120: 756e 6966 6965 6420 6375 7272 656e 6379  unified currency
-0002d130: 2063 6f64 6520 6f66 2074 6865 2063 7572   code of the cur
-0002d140: 7265 6e63 7920 7472 616e 7366 6572 7265  rency transferre
-0002d150: 640a 2020 2020 2020 2020 3a70 6172 616d  d.        :param
-0002d160: 2069 6e74 7c4e 6f6e 6520 7369 6e63 653a   int|None since:
-0002d170: 2074 6865 2065 6172 6c69 6573 7420 7469   the earliest ti
-0002d180: 6d65 2069 6e20 6d73 2074 6f20 6665 7463  me in ms to fetc
-0002d190: 6820 7472 616e 7366 6572 7320 666f 720a  h transfers for.
-0002d1a0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0002d1b0: 6e74 7c4e 6f6e 6520 6c69 6d69 743a 2074  nt|None limit: t
-0002d1c0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-0002d1d0: 7220 6f66 2020 7472 616e 7366 6572 7320  r of  transfers 
-0002d1e0: 7374 7275 6374 7572 6573 2074 6f20 7265  structures to re
-0002d1f0: 7472 6965 7665 0a20 2020 2020 2020 203a  trieve.        :
-0002d200: 7061 7261 6d20 6469 6374 2070 6172 616d  param dict param
-0002d210: 733a 2065 7874 7261 2070 6172 616d 6574  s: extra paramet
-0002d220: 6572 7320 7370 6563 6966 6963 2074 6f20  ers specific to 
-0002d230: 7468 6520 7068 656d 6578 2061 7069 2065  the phemex api e
-0002d240: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
-0002d250: 3a72 6574 7572 6e73 205b 6469 6374 5d3a  :returns [dict]:
-0002d260: 2061 206c 6973 7420 6f66 2060 7472 616e   a list of `tran
-0002d270: 7366 6572 2073 7472 7563 7475 7265 7320  sfer structures 
-0002d280: 3c68 7474 7073 3a2f 2f64 6f63 732e 6363  <https://docs.cc
-0002d290: 7874 2e63 6f6d 2f23 2f3f 6964 3d74 7261  xt.com/#/?id=tra
-0002d2a0: 6e73 6665 722d 7374 7275 6374 7572 653e  nsfer-structure>
-0002d2b0: 600a 2020 2020 2020 2020 2222 220a 2020  `.        """.  
-0002d2c0: 2020 2020 2020 7365 6c66 2e6c 6f61 645f        self.load_
-0002d2d0: 6d61 726b 6574 7328 290a 2020 2020 2020  markets().      
-0002d2e0: 2020 6966 2063 6f64 6520 6973 204e 6f6e    if code is Non
-0002d2f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002d300: 6169 7365 2041 7267 756d 656e 7473 5265  aise ArgumentsRe
-0002d310: 7175 6972 6564 2873 656c 662e 6964 202b  quired(self.id +
-0002d320: 2027 2066 6574 6368 5472 616e 7366 6572   ' fetchTransfer
-0002d330: 7328 2920 7265 7175 6972 6573 2061 2063  s() requires a c
-0002d340: 6f64 6520 6172 6775 6d65 6e74 2729 0a20  ode argument'). 
-0002d350: 2020 2020 2020 2063 7572 7265 6e63 7920         currency 
-0002d360: 3d20 7365 6c66 2e63 7572 7265 6e63 7928  = self.currency(
-0002d370: 636f 6465 290a 2020 2020 2020 2020 7265  code).        re
-0002d380: 7175 6573 7420 3d20 7b0a 2020 2020 2020  quest = {.      
-0002d390: 2020 2020 2020 2763 7572 7265 6e63 7927        'currency'
-0002d3a0: 3a20 6375 7272 656e 6379 5b27 6964 275d  : currency['id']
-0002d3b0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-0002d3c0: 2020 2020 6966 2073 696e 6365 2069 7320      if since is 
-0002d3d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002d3e0: 2020 2020 2020 7265 7175 6573 745b 2773        request['s
-0002d3f0: 7461 7274 275d 203d 2073 696e 6365 0a20  tart'] = since. 
-0002d400: 2020 2020 2020 2069 6620 6c69 6d69 7420         if limit 
-0002d410: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d420: 2020 2020 2020 2020 2072 6571 7565 7374           request
-0002d430: 5b27 6c69 6d69 7427 5d20 3d20 6c69 6d69  ['limit'] = limi
-0002d440: 740a 2020 2020 2020 2020 7265 7370 6f6e  t.        respon
-0002d450: 7365 203d 2073 656c 662e 7072 6976 6174  se = self.privat
-0002d460: 6547 6574 4173 7365 7473 5472 616e 7366  eGetAssetsTransf
-0002d470: 6572 2873 656c 662e 6578 7465 6e64 2872  er(self.extend(r
-0002d480: 6571 7565 7374 2c20 7061 7261 6d73 2929  equest, params))
-0002d490: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-0002d4a0: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
-0002d4b0: 2020 2023 2020 2020 2020 2020 2022 636f     #         "co
-0002d4c0: 6465 223a 2030 2c0a 2020 2020 2020 2020  de": 0,.        
-0002d4d0: 2320 2020 2020 2020 2020 226d 7367 223a  #         "msg":
-0002d4e0: 2022 4f4b 222c 0a20 2020 2020 2020 2023   "OK",.        #
-0002d4f0: 2020 2020 2020 2020 2022 6461 7461 223a           "data":
-0002d500: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-0002d510: 2020 2020 2020 2020 2022 726f 7773 223a           "rows":
-0002d520: 205b 0a20 2020 2020 2020 2023 2020 2020   [.        #    
-0002d530: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-0002d540: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002d550: 2020 2020 2020 2020 2020 2020 2022 6c69               "li
-0002d560: 6e6b 4b65 7922 3a20 2238 3763 3037 3161  nkKey": "87c071a
-0002d570: 332d 3836 3238 2d34 6163 322d 6163 6131  3-8628-4ac2-aca1
-0002d580: 2d36 6365 3064 3166 6164 3636 6322 2c0a  -6ce0d1fad66c",.
-0002d590: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002d5a0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-0002d5b0: 7365 7249 6422 3a20 3431 3438 3432 382c  serId": 4148428,
-0002d5c0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0002d5d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0002d5e0: 6375 7272 656e 6379 223a 2022 4254 4322  currency": "BTC"
-0002d5f0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0002d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d610: 2261 6d6f 756e 7445 7622 3a20 3637 3933  "amountEv": 6793
-0002d620: 322c 0a20 2020 2020 2020 2023 2020 2020  2,.        #    
-0002d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d640: 2022 7369 6465 223a 2032 2c0a 2020 2020   "side": 2,.    
-0002d650: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0002d660: 2020 2020 2020 2020 2020 2273 7461 7475            "statu
-0002d670: 7322 3a20 3130 2c0a 2020 2020 2020 2020  s": 10,.        
-0002d680: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0002d690: 2020 2020 2020 2263 7265 6174 6554 696d        "createTim
-0002d6a0: 6522 3a20 3136 3532 3833 3234 3637 3030  e": 165283246700
-0002d6b0: 302c 0a20 2020 2020 2020 2023 2020 2020  0,.        #    
-0002d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d6d0: 2022 6269 7a54 7970 6522 3a20 3130 0a20   "bizType": 10. 
-0002d6e0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002d6f0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-0002d700: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0002d710: 205d 0a20 2020 2020 2020 2023 2020 2020   ].        #    
-0002d720: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0002d730: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0002d740: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0002d750: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-0002d760: 7265 7370 6f6e 7365 2c20 2764 6174 6127  response, 'data'
-0002d770: 2c20 7b7d 290a 2020 2020 2020 2020 7472  , {}).        tr
-0002d780: 616e 7366 6572 7320 3d20 7365 6c66 2e73  ansfers = self.s
-0002d790: 6166 655f 7661 6c75 6528 6461 7461 2c20  afe_value(data, 
-0002d7a0: 2772 6f77 7327 2c20 5b5d 290a 2020 2020  'rows', []).    
-0002d7b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0002d7c0: 7061 7273 655f 7472 616e 7366 6572 7328  parse_transfers(
-0002d7d0: 7472 616e 7366 6572 732c 2063 7572 7265  transfers, curre
-0002d7e0: 6e63 792c 2073 696e 6365 2c20 6c69 6d69  ncy, since, limi
-0002d7f0: 7429 0a0a 2020 2020 6465 6620 7061 7273  t)..    def pars
-0002d800: 655f 7472 616e 7366 6572 2873 656c 662c  e_transfer(self,
-0002d810: 2074 7261 6e73 6665 722c 2063 7572 7265   transfer, curre
-0002d820: 6e63 793d 4e6f 6e65 293a 0a20 2020 2020  ncy=None):.     
-0002d830: 2020 2023 0a20 2020 2020 2020 2023 2074     #.        # t
-0002d840: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
-0002d850: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
-0002d860: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
-0002d870: 2020 2020 6c69 6e6b 4b65 793a 2027 3835      linkKey: '85
-0002d880: 3634 6562 6134 2d63 3965 632d 3439 6436  64eba4-c9ec-49d6
-0002d890: 2d39 6238 632d 3265 6335 3030 3161 3066  -9b8c-2ec5001a0f
-0002d8a0: 6239 272c 0a20 2020 2020 2020 2023 2020  b9',.        #  
-0002d8b0: 2020 2020 2020 2075 7365 7249 643a 2027         userId: '
-0002d8c0: 3430 3138 3334 3027 2c0a 2020 2020 2020  4018340',.      
-0002d8d0: 2020 2320 2020 2020 2020 2020 6375 7272    #         curr
-0002d8e0: 656e 6379 3a20 2755 5344 272c 0a20 2020  ency: 'USD',.   
-0002d8f0: 2020 2020 2023 2020 2020 2020 2020 2061       #         a
-0002d900: 6d6f 756e 7445 763a 2027 3130 272c 0a20  mountEv: '10',. 
-0002d910: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002d920: 2073 6964 653a 2027 3227 2c0a 2020 2020   side: '2',.    
-0002d930: 2020 2020 2320 2020 2020 2020 2020 7374      #         st
-0002d940: 6174 7573 3a20 2731 3027 0a20 2020 2020  atus: '10'.     
-0002d950: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
-0002d960: 2020 2023 0a20 2020 2020 2020 2023 2066     #.        # f
-0002d970: 6574 6368 5472 616e 7366 6572 730a 2020  etchTransfers.  
-0002d980: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-0002d990: 2320 2020 2020 7b0a 2020 2020 2020 2020  #     {.        
-0002d9a0: 2320 2020 2020 2020 2020 226c 696e 6b4b  #         "linkK
-0002d9b0: 6579 223a 2022 3837 6330 3731 6133 2d38  ey": "87c071a3-8
-0002d9c0: 3632 382d 3461 6332 2d61 6361 312d 3663  628-4ac2-aca1-6c
-0002d9d0: 6530 6431 6661 6436 3663 222c 0a20 2020  e0d1fad66c",.   
-0002d9e0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-0002d9f0: 7573 6572 4964 223a 2034 3134 3834 3238  userId": 4148428
-0002da00: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-0002da10: 2020 2020 2263 7572 7265 6e63 7922 3a20      "currency": 
-0002da20: 2242 5443 222c 0a20 2020 2020 2020 2023  "BTC",.        #
-0002da30: 2020 2020 2020 2020 2022 616d 6f75 6e74           "amount
-0002da40: 4576 223a 2036 3739 3332 2c0a 2020 2020  Ev": 67932,.    
-0002da50: 2020 2020 2320 2020 2020 2020 2020 2273      #         "s
-0002da60: 6964 6522 3a20 322c 0a20 2020 2020 2020  ide": 2,.       
-0002da70: 2023 2020 2020 2020 2020 2022 7374 6174   #         "stat
-0002da80: 7573 223a 2031 302c 0a20 2020 2020 2020  us": 10,.       
-0002da90: 2023 2020 2020 2020 2020 2022 6372 6561   #         "crea
-0002daa0: 7465 5469 6d65 223a 2031 3635 3238 3332  teTime": 1652832
-0002dab0: 3436 3730 3030 2c0a 2020 2020 2020 2020  467000,.        
-0002dac0: 2320 2020 2020 2020 2020 2262 697a 5479  #         "bizTy
-0002dad0: 7065 223a 2031 300a 2020 2020 2020 2020  pe": 10.        
-0002dae0: 2320 2020 2020 7d0a 2020 2020 2020 2020  #     }.        
-0002daf0: 230a 2020 2020 2020 2020 6964 203d 2073  #.        id = s
-0002db00: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
-0002db10: 7472 616e 7366 6572 2c20 276c 696e 6b4b  transfer, 'linkK
-0002db20: 6579 2729 0a20 2020 2020 2020 2073 7461  ey').        sta
-0002db30: 7475 7320 3d20 7365 6c66 2e73 6166 655f  tus = self.safe_
-0002db40: 7374 7269 6e67 2874 7261 6e73 6665 722c  string(transfer,
-0002db50: 2027 7374 6174 7573 2729 0a20 2020 2020   'status').     
-0002db60: 2020 2061 6d6f 756e 7445 7620 3d20 7365     amountEv = se
-0002db70: 6c66 2e73 6166 655f 7374 7269 6e67 2874  lf.safe_string(t
-0002db80: 7261 6e73 6665 722c 2027 616d 6f75 6e74  ransfer, 'amount
-0002db90: 4576 2729 0a20 2020 2020 2020 2061 6d6f  Ev').        amo
-0002dba0: 756e 7454 7261 6e73 6665 7265 6420 3d20  untTransfered = 
-0002dbb0: 7365 6c66 2e66 726f 6d5f 6576 2861 6d6f  self.from_ev(amo
-0002dbc0: 756e 7445 762c 2063 7572 7265 6e63 7929  untEv, currency)
-0002dbd0: 0a20 2020 2020 2020 2063 7572 7265 6e63  .        currenc
-0002dbe0: 7949 6420 3d20 7365 6c66 2e73 6166 655f  yId = self.safe_
-0002dbf0: 7374 7269 6e67 2874 7261 6e73 6665 722c  string(transfer,
-0002dc00: 2027 6375 7272 656e 6379 2729 0a20 2020   'currency').   
-0002dc10: 2020 2020 2063 6f64 6520 3d20 7365 6c66       code = self
-0002dc20: 2e73 6166 655f 6375 7272 656e 6379 5f63  .safe_currency_c
-0002dc30: 6f64 6528 6375 7272 656e 6379 4964 2c20  ode(currencyId, 
-0002dc40: 6375 7272 656e 6379 290a 2020 2020 2020  currency).      
-0002dc50: 2020 7369 6465 203d 2073 656c 662e 7361    side = self.sa
-0002dc60: 6665 5f69 6e74 6567 6572 2874 7261 6e73  fe_integer(trans
-0002dc70: 6665 722c 2027 7369 6465 2729 0a20 2020  fer, 'side').   
-0002dc80: 2020 2020 2066 726f 6d49 6420 3d20 4e6f       fromId = No
-0002dc90: 6e65 0a20 2020 2020 2020 2074 6f49 6420  ne.        toId 
-0002dca0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-0002dcb0: 6620 7369 6465 203d 3d20 313a 0a20 2020  f side == 1:.   
-0002dcc0: 2020 2020 2020 2020 2066 726f 6d49 6420           fromId 
-0002dcd0: 3d20 2773 7761 7027 0a20 2020 2020 2020  = 'swap'.       
-0002dce0: 2020 2020 2074 6f49 6420 3d20 2773 706f       toId = 'spo
-0002dcf0: 7427 0a20 2020 2020 2020 2065 6c69 6620  t'.        elif 
-0002dd00: 7369 6465 203d 3d20 323a 0a20 2020 2020  side == 2:.     
-0002dd10: 2020 2020 2020 2066 726f 6d49 6420 3d20         fromId = 
-0002dd20: 2773 706f 7427 0a20 2020 2020 2020 2020  'spot'.         
-0002dd30: 2020 2074 6f49 6420 3d20 2773 7761 7027     toId = 'swap'
-0002dd40: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-0002dd50: 6d70 203d 2073 656c 662e 7361 6665 5f69  mp = self.safe_i
-0002dd60: 6e74 6567 6572 2874 7261 6e73 6665 722c  nteger(transfer,
-0002dd70: 2027 6372 6561 7465 5469 6d65 2729 0a20   'createTime'). 
-0002dd80: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
-0002dd90: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
-0002dda0: 6f27 3a20 7472 616e 7366 6572 2c0a 2020  o': transfer,.  
-0002ddb0: 2020 2020 2020 2020 2020 2769 6427 3a20            'id': 
-0002ddc0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002ddd0: 2774 696d 6573 7461 6d70 273a 2074 696d  'timestamp': tim
-0002dde0: 6573 7461 6d70 2c0a 2020 2020 2020 2020  estamp,.        
-0002ddf0: 2020 2020 2764 6174 6574 696d 6527 3a20      'datetime': 
-0002de00: 7365 6c66 2e69 736f 3836 3031 2874 696d  self.iso8601(tim
-0002de10: 6573 7461 6d70 292c 0a20 2020 2020 2020  estamp),.       
-0002de20: 2020 2020 2027 6375 7272 656e 6379 273a       'currency':
-0002de30: 2063 6f64 652c 0a20 2020 2020 2020 2020   code,.         
-0002de40: 2020 2027 616d 6f75 6e74 273a 2061 6d6f     'amount': amo
-0002de50: 756e 7454 7261 6e73 6665 7265 642c 0a20  untTransfered,. 
-0002de60: 2020 2020 2020 2020 2020 2027 6672 6f6d             'from
-0002de70: 4163 636f 756e 7427 3a20 6672 6f6d 4964  Account': fromId
-0002de80: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
-0002de90: 6f41 6363 6f75 6e74 273a 2074 6f49 642c  oAccount': toId,
-0002dea0: 0a20 2020 2020 2020 2020 2020 2027 7374  .            'st
-0002deb0: 6174 7573 273a 2073 656c 662e 7061 7273  atus': self.pars
-0002dec0: 655f 7472 616e 7366 6572 5f73 7461 7475  e_transfer_statu
-0002ded0: 7328 7374 6174 7573 292c 0a20 2020 2020  s(status),.     
-0002dee0: 2020 207d 0a0a 2020 2020 6465 6620 7061     }..    def pa
-0002def0: 7273 655f 7472 616e 7366 6572 5f73 7461  rse_transfer_sta
-0002df00: 7475 7328 7365 6c66 2c20 7374 6174 7573  tus(self, status
-0002df10: 293a 0a20 2020 2020 2020 2073 7461 7475  ):.        statu
-0002df20: 7365 7320 3d20 7b0a 2020 2020 2020 2020  ses = {.        
-0002df30: 2020 2020 2733 273a 2027 7265 6a65 6374      '3': 'reject
-0002df40: 6564 272c 2020 2320 2752 656a 6563 7465  ed',  # 'Rejecte
-0002df50: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-0002df60: 2736 273a 2027 6361 6e63 656c 6564 272c  '6': 'canceled',
-0002df70: 2020 2320 2747 6f74 2065 7272 6f72 2061    # 'Got error a
-0002df80: 6e64 2077 6169 7420 666f 7220 7265 636f  nd wait for reco
-0002df90: 7665 7279 272c 0a20 2020 2020 2020 2020  very',.         
-0002dfa0: 2020 2027 3130 273a 2027 6f6b 272c 2020     '10': 'ok',  
-0002dfb0: 2320 2753 7563 6365 7373 272c 0a20 2020  # 'Success',.   
-0002dfc0: 2020 2020 2020 2020 2027 3131 273a 2027           '11': '
-0002dfd0: 6661 696c 6564 272c 2020 2320 2746 6169  failed',  # 'Fai
-0002dfe0: 6c65 6427 2c0a 2020 2020 2020 2020 7d0a  led',.        }.
-0002dff0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002e000: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
-0002e010: 7374 6174 7573 6573 2c20 7374 6174 7573  statuses, status
-0002e020: 2c20 7374 6174 7573 290a 0a20 2020 2064  , status)..    d
-0002e030: 6566 2066 6574 6368 5f66 756e 6469 6e67  ef fetch_funding
-0002e040: 5f72 6174 655f 6869 7374 6f72 7928 7365  _rate_history(se
-0002e050: 6c66 2c20 7379 6d62 6f6c 3a20 4f70 7469  lf, symbol: Opti
-0002e060: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0002e070: 2c20 7369 6e63 653a 204f 7074 696f 6e61  , since: Optiona
-0002e080: 6c5b 696e 745d 203d 204e 6f6e 652c 206c  l[int] = None, l
-0002e090: 696d 6974 3a20 4f70 7469 6f6e 616c 5b69  imit: Optional[i
-0002e0a0: 6e74 5d20 3d20 4e6f 6e65 2c20 7061 7261  nt] = None, para
-0002e0b0: 6d73 3d7b 7d29 3a0a 2020 2020 2020 2020  ms={}):.        
-0002e0c0: 7365 6c66 2e63 6865 636b 5f72 6571 7569  self.check_requi
-0002e0d0: 7265 645f 7379 6d62 6f6c 2827 6665 7463  red_symbol('fetc
-0002e0e0: 6846 756e 6469 6e67 5261 7465 4869 7374  hFundingRateHist
-0002e0f0: 6f72 7927 2c20 7379 6d62 6f6c 290a 2020  ory', symbol).  
-0002e100: 2020 2020 2020 7365 6c66 2e6c 6f61 645f        self.load_
-0002e110: 6d61 726b 6574 7328 290a 2020 2020 2020  markets().      
-0002e120: 2020 6d61 726b 6574 203d 2073 656c 662e    market = self.
-0002e130: 6d61 726b 6574 2873 796d 626f 6c29 0a20  market(symbol). 
-0002e140: 2020 2020 2020 2069 7355 7364 7453 6574         isUsdtSet
-0002e150: 746c 6564 203d 206d 6172 6b65 745b 2773  tled = market['s
-0002e160: 6574 746c 6527 5d20 3d3d 2027 5553 4454  ettle'] == 'USDT
-0002e170: 270a 2020 2020 2020 2020 6966 206e 6f74  '.        if not
-0002e180: 206d 6172 6b65 745b 2773 7761 7027 5d3a   market['swap']:
-0002e190: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0002e1a0: 7365 2042 6164 5265 7175 6573 7428 7365  se BadRequest(se
-0002e1b0: 6c66 2e69 6420 2b20 2720 6665 7463 6846  lf.id + ' fetchF
-0002e1c0: 756e 6469 6e67 5261 7465 4869 7374 6f72  undingRateHistor
-0002e1d0: 7928 2920 7375 7070 6f72 7473 2073 7761  y() supports swa
-0002e1e0: 7020 636f 6e74 7261 6374 7320 6f6e 6c79  p contracts only
-0002e1f0: 2729 0a20 2020 2020 2020 2063 7573 746f  ').        custo
-0002e200: 6d53 796d 626f 6c20 3d20 4e6f 6e65 0a20  mSymbol = None. 
-0002e210: 2020 2020 2020 2069 6620 6973 5573 6474         if isUsdt
-0002e220: 5365 7474 6c65 643a 0a20 2020 2020 2020  Settled:.       
-0002e230: 2020 2020 2063 7573 746f 6d53 796d 626f       customSymbo
-0002e240: 6c20 3d20 272e 2720 2b20 6d61 726b 6574  l = '.' + market
-0002e250: 5b27 6964 275d 202b 2027 4652 3848 2720  ['id'] + 'FR8H' 
-0002e260: 2023 2070 6865 6d65 7820 7265 7175 6972   # phemex requir
-0002e270: 6573 2061 2063 7573 746f 6d20 7379 6d62  es a custom symb
-0002e280: 6f6c 2066 6f72 2066 756e 6469 6e67 2072  ol for funding r
-0002e290: 6174 6520 6869 7374 6f72 790a 2020 2020  ate history.    
-0002e2a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002e2b0: 2020 2020 2020 6375 7374 6f6d 5379 6d62        customSymb
-0002e2c0: 6f6c 203d 2027 2e27 202b 206d 6172 6b65  ol = '.' + marke
-0002e2d0: 745b 2762 6173 6549 6427 5d20 2b20 2746  t['baseId'] + 'F
-0002e2e0: 5238 4827 0a20 2020 2020 2020 2072 6571  R8H'.        req
-0002e2f0: 7565 7374 203d 207b 0a20 2020 2020 2020  uest = {.       
-0002e300: 2020 2020 2027 7379 6d62 6f6c 273a 2063       'symbol': c
-0002e310: 7573 746f 6d53 796d 626f 6c2c 0a20 2020  ustomSymbol,.   
-0002e320: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
-0002e330: 6620 7369 6e63 6520 6973 206e 6f74 204e  f since is not N
-0002e340: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002e350: 2072 6571 7565 7374 5b27 7374 6172 7427   request['start'
-0002e360: 5d20 3d20 7369 6e63 650a 2020 2020 2020  ] = since.      
-0002e370: 2020 6966 206c 696d 6974 2069 7320 6e6f    if limit is no
-0002e380: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002e390: 2020 2020 7265 7175 6573 745b 276c 696d      request['lim
-0002e3a0: 6974 275d 203d 206c 696d 6974 0a20 2020  it'] = limit.   
-0002e3b0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-0002e3c0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-0002e3d0: 6973 5573 6474 5365 7474 6c65 643a 0a20  isUsdtSettled:. 
-0002e3e0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-0002e3f0: 6e73 6520 3d20 7365 6c66 2e76 3247 6574  nse = self.v2Get
-0002e400: 4170 6944 6174 6150 7562 6c69 6344 6174  ApiDataPublicDat
-0002e410: 6146 756e 6469 6e67 5261 7465 4869 7374  aFundingRateHist
-0002e420: 6f72 7928 7365 6c66 2e65 7874 656e 6428  ory(self.extend(
-0002e430: 7265 7175 6573 742c 2070 6172 616d 7329  request, params)
-0002e440: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0002e450: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-0002e460: 6f6e 7365 203d 2073 656c 662e 7631 4765  onse = self.v1Ge
-0002e470: 7441 7069 4461 7461 5075 626c 6963 4461  tApiDataPublicDa
-0002e480: 7461 4675 6e64 696e 6752 6174 6548 6973  taFundingRateHis
-0002e490: 746f 7279 2873 656c 662e 6578 7465 6e64  tory(self.extend
-0002e4a0: 2872 6571 7565 7374 2c20 7061 7261 6d73  (request, params
-0002e4b0: 2929 0a20 2020 2020 2020 2023 0a20 2020  )).        #.   
-0002e4c0: 2020 2020 2023 2020 2020 7b0a 2020 2020       #    {.    
-0002e4d0: 2020 2020 2320 2020 2020 2020 2022 636f      #        "co
-0002e4e0: 6465 223a 2230 222c 0a20 2020 2020 2020  de":"0",.       
-0002e4f0: 2023 2020 2020 2020 2020 226d 7367 223a   #        "msg":
-0002e500: 224f 4b22 2c0a 2020 2020 2020 2020 2320  "OK",.        # 
-0002e510: 2020 2020 2020 2022 6461 7461 223a 7b0a         "data":{.
-0002e520: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002e530: 2020 2020 2272 6f77 7322 3a5b 0a20 2020      "rows":[.   
-0002e540: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0002e550: 2020 2020 7b0a 2020 2020 2020 2020 2320      {.        # 
-0002e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e570: 2273 796d 626f 6c22 3a22 2e42 5443 5553  "symbol":".BTCUS
-0002e580: 4454 4652 3848 222c 0a20 2020 2020 2020  DTFR8H",.       
-0002e590: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0002e5a0: 2020 2022 6675 6e64 696e 6752 6174 6522     "fundingRate"
-0002e5b0: 3a22 302e 3030 3031 222c 0a20 2020 2020  :"0.0001",.     
-0002e5c0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0002e5d0: 2020 2020 2022 6675 6e64 696e 6754 696d       "fundingTim
-0002e5e0: 6522 3a22 3136 3832 3036 3430 3030 3030  e":"168206400000
-0002e5f0: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-0002e600: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-0002e610: 6e74 6572 7661 6c53 6563 6f6e 6473 223a  ntervalSeconds":
-0002e620: 2232 3838 3030 220a 2020 2020 2020 2020  "28800".        
-0002e630: 2320 2020 2020 2020 2020 2020 2020 207d  #              }
-0002e640: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-0002e650: 2020 2020 205d 0a20 2020 2020 2020 2023       ].        #
-0002e660: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0002e670: 2020 2320 2020 207d 0a20 2020 2020 2020    #    }.       
-0002e680: 2023 0a20 2020 2020 2020 2064 6174 6120   #.        data 
-0002e690: 3d20 7365 6c66 2e73 6166 655f 7661 6c75  = self.safe_valu
-0002e6a0: 6528 7265 7370 6f6e 7365 2c20 2764 6174  e(response, 'dat
-0002e6b0: 6127 2c20 7b7d 290a 2020 2020 2020 2020  a', {}).        
-0002e6c0: 7261 7465 7320 3d20 7365 6c66 2e73 6166  rates = self.saf
-0002e6d0: 655f 7661 6c75 6528 6461 7461 2c20 2772  e_value(data, 'r
-0002e6e0: 6f77 7327 290a 2020 2020 2020 2020 7265  ows').        re
-0002e6f0: 7375 6c74 203d 205b 5d0a 2020 2020 2020  sult = [].      
-0002e700: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0002e710: 2830 2c20 6c65 6e28 7261 7465 7329 293a  (0, len(rates)):
-0002e720: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-0002e730: 6d20 3d20 7261 7465 735b 695d 0a20 2020  m = rates[i].   
-0002e740: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
-0002e750: 6d70 203d 2073 656c 662e 7361 6665 5f69  mp = self.safe_i
-0002e760: 6e74 6567 6572 2869 7465 6d2c 2027 6675  nteger(item, 'fu
-0002e770: 6e64 696e 6754 696d 6527 290a 2020 2020  ndingTime').    
-0002e780: 2020 2020 2020 2020 7265 7375 6c74 2e61          result.a
-0002e790: 7070 656e 6428 7b0a 2020 2020 2020 2020  ppend({.        
-0002e7a0: 2020 2020 2020 2020 2769 6e66 6f27 3a20          'info': 
-0002e7b0: 6974 656d 2c0a 2020 2020 2020 2020 2020  item,.          
-0002e7c0: 2020 2020 2020 2773 796d 626f 6c27 3a20        'symbol': 
-0002e7d0: 7379 6d62 6f6c 2c0a 2020 2020 2020 2020  symbol,.        
-0002e7e0: 2020 2020 2020 2020 2766 756e 6469 6e67          'funding
-0002e7f0: 5261 7465 273a 2073 656c 662e 7361 6665  Rate': self.safe
-0002e800: 5f6e 756d 6265 7228 6974 656d 2c20 2766  _number(item, 'f
-0002e810: 756e 6469 6e67 5261 7465 2729 2c0a 2020  undingRate'),.  
-0002e820: 2020 2020 2020 2020 2020 2020 2020 2774                't
-0002e830: 696d 6573 7461 6d70 273a 2074 696d 6573  imestamp': times
-0002e840: 7461 6d70 2c0a 2020 2020 2020 2020 2020  tamp,.          
-0002e850: 2020 2020 2020 2764 6174 6574 696d 6527        'datetime'
-0002e860: 3a20 7365 6c66 2e69 736f 3836 3031 2874  : self.iso8601(t
-0002e870: 696d 6573 7461 6d70 292c 0a20 2020 2020  imestamp),.     
-0002e880: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
-0002e890: 2020 736f 7274 6564 203d 2073 656c 662e    sorted = self.
-0002e8a0: 736f 7274 5f62 7928 7265 7375 6c74 2c20  sort_by(result, 
-0002e8b0: 2774 696d 6573 7461 6d70 2729 0a20 2020  'timestamp').   
-0002e8c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002e8d0: 2e66 696c 7465 725f 6279 5f73 796d 626f  .filter_by_symbo
-0002e8e0: 6c5f 7369 6e63 655f 6c69 6d69 7428 736f  l_since_limit(so
-0002e8f0: 7274 6564 2c20 7379 6d62 6f6c 2c20 7369  rted, symbol, si
-0002e900: 6e63 652c 206c 696d 6974 290a 0a20 2020  nce, limit)..   
-0002e910: 2064 6566 2068 616e 646c 655f 6572 726f   def handle_erro
-0002e920: 7273 2873 656c 662c 2068 7474 7043 6f64  rs(self, httpCod
-0002e930: 652c 2072 6561 736f 6e2c 2075 726c 2c20  e, reason, url, 
-0002e940: 6d65 7468 6f64 2c20 6865 6164 6572 732c  method, headers,
-0002e950: 2062 6f64 792c 2072 6573 706f 6e73 652c   body, response,
-0002e960: 2072 6571 7565 7374 4865 6164 6572 732c   requestHeaders,
-0002e970: 2072 6571 7565 7374 426f 6479 293a 0a20   requestBody):. 
-0002e980: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
-0002e990: 7365 2069 7320 4e6f 6e65 3a0a 2020 2020  se is None:.    
-0002e9a0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-0002e9b0: 6f6e 6520 2023 2066 616c 6c62 6163 6b20  one  # fallback 
-0002e9c0: 746f 2064 6566 6175 6c74 2065 7272 6f72  to default error
-0002e9d0: 2068 616e 646c 6572 0a20 2020 2020 2020   handler.       
-0002e9e0: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-0002e9f0: 207b 2263 6f64 6522 3a33 3030 3138 2c22   {"code":30018,"
-0002ea00: 6d73 6722 3a22 7068 656d 6578 2e64 6174  msg":"phemex.dat
-0002ea10: 612e 7369 7a65 2e75 706c 696d 7422 2c22  a.size.uplimt","
-0002ea20: 6461 7461 223a 6e75 6c6c 7d0a 2020 2020  data":null}.    
-0002ea30: 2020 2020 2320 2020 2020 7b22 636f 6465      #     {"code
-0002ea40: 223a 3431 322c 226d 7367 223a 224d 6973  ":412,"msg":"Mis
-0002ea50: 7369 6e67 2070 6172 616d 6574 6572 202d  sing parameter -
-0002ea60: 2072 6573 6f6c 7574 696f 6e22 2c22 6461   resolution","da
-0002ea70: 7461 223a 6e75 6c6c 7d0a 2020 2020 2020  ta":null}.      
-0002ea80: 2020 2320 2020 2020 7b22 636f 6465 223a    #     {"code":
-0002ea90: 3431 322c 226d 7367 223a 224d 6973 7369  412,"msg":"Missi
-0002eaa0: 6e67 2070 6172 616d 6574 6572 202d 2074  ng parameter - t
-0002eab0: 6f22 2c22 6461 7461 223a 6e75 6c6c 7d0a  o","data":null}.
-0002eac0: 2020 2020 2020 2020 2320 2020 2020 7b22          #     {"
-0002ead0: 6572 726f 7222 3a7b 2263 6f64 6522 3a36  error":{"code":6
-0002eae0: 3030 312c 226d 6573 7361 6765 223a 2269  001,"message":"i
-0002eaf0: 6e76 616c 6964 2061 7267 756d 656e 7422  nvalid argument"
-0002eb00: 7d2c 2269 6422 3a6e 756c 6c2c 2272 6573  },"id":null,"res
-0002eb10: 756c 7422 3a6e 756c 6c7d 0a20 2020 2020  ult":null}.     
-0002eb20: 2020 2023 0a20 2020 2020 2020 2065 7272     #.        err
-0002eb30: 6f72 203d 2073 656c 662e 7361 6665 5f76  or = self.safe_v
-0002eb40: 616c 7565 2872 6573 706f 6e73 652c 2027  alue(response, '
-0002eb50: 6572 726f 7227 2c20 7265 7370 6f6e 7365  error', response
-0002eb60: 290a 2020 2020 2020 2020 6572 726f 7243  ).        errorC
-0002eb70: 6f64 6520 3d20 7365 6c66 2e73 6166 655f  ode = self.safe_
-0002eb80: 7374 7269 6e67 2865 7272 6f72 2c20 2763  string(error, 'c
-0002eb90: 6f64 6527 290a 2020 2020 2020 2020 6d65  ode').        me
-0002eba0: 7373 6167 6520 3d20 7365 6c66 2e73 6166  ssage = self.saf
-0002ebb0: 655f 7374 7269 6e67 2865 7272 6f72 2c20  e_string(error, 
-0002ebc0: 276d 7367 2729 0a20 2020 2020 2020 2069  'msg').        i
-0002ebd0: 6620 2865 7272 6f72 436f 6465 2069 7320  f (errorCode is 
-0002ebe0: 6e6f 7420 4e6f 6e65 2920 616e 6420 2865  not None) and (e
-0002ebf0: 7272 6f72 436f 6465 2021 3d20 2730 2729  rrorCode != '0')
-0002ec00: 3a0a 2020 2020 2020 2020 2020 2020 6665  :.            fe
-0002ec10: 6564 6261 636b 203d 2073 656c 662e 6964  edback = self.id
-0002ec20: 202b 2027 2027 202b 2062 6f64 790a 2020   + ' ' + body.  
-0002ec30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0002ec40: 6872 6f77 5f65 7861 6374 6c79 5f6d 6174  hrow_exactly_mat
-0002ec50: 6368 6564 5f65 7863 6570 7469 6f6e 2873  ched_exception(s
-0002ec60: 656c 662e 6578 6365 7074 696f 6e73 5b27  elf.exceptions['
-0002ec70: 6578 6163 7427 5d2c 2065 7272 6f72 436f  exact'], errorCo
-0002ec80: 6465 2c20 6665 6564 6261 636b 290a 2020  de, feedback).  
-0002ec90: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0002eca0: 6872 6f77 5f62 726f 6164 6c79 5f6d 6174  hrow_broadly_mat
-0002ecb0: 6368 6564 5f65 7863 6570 7469 6f6e 2873  ched_exception(s
-0002ecc0: 656c 662e 6578 6365 7074 696f 6e73 5b27  elf.exceptions['
-0002ecd0: 6272 6f61 6427 5d2c 206d 6573 7361 6765  broad'], message
-0002ece0: 2c20 6665 6564 6261 636b 290a 2020 2020  , feedback).    
-0002ecf0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-0002ed00: 6368 616e 6765 4572 726f 7228 6665 6564  changeError(feed
-0002ed10: 6261 636b 2920 2023 2075 6e6b 6e6f 776e  back)  # unknown
-0002ed20: 206d 6573 7361 6765 0a20 2020 2020 2020   message.       
-0002ed30: 2072 6574 7572 6e20 4e6f 6e65 0a          return None.
+0002cd50: 7461 3a20 7b0a 2020 2020 2020 2020 2020  ta: {.          
+0002cd60: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0002cd70: 6c69 6e6b 4b65 793a 2027 3835 3634 6562  linkKey: '8564eb
+0002cd80: 6134 2d63 3965 632d 3439 6436 2d39 6238  a4-c9ec-49d6-9b8
+0002cd90: 632d 3265 6335 3030 3161 3066 6239 272c  c-2ec5001a0fb9',
+0002cda0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0002cdb0: 2020 2020 2020 2020 2020 2075 7365 7249             userI
+0002cdc0: 643a 2027 3430 3138 3334 3027 2c0a 2020  d: '4018340',.  
+0002cdd0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0002cde0: 2020 2020 2020 2020 6375 7272 656e 6379          currency
+0002cdf0: 3a20 2755 5344 272c 0a20 2020 2020 2020  : 'USD',.       
+0002ce00: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0002ce10: 2020 2061 6d6f 756e 7445 763a 2027 3130     amountEv: '10
+0002ce20: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
+0002ce30: 2020 2020 2020 2020 2020 2020 2073 6964               sid
+0002ce40: 653a 2027 3227 2c0a 2020 2020 2020 2020  e: '2',.        
+0002ce50: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0002ce60: 2020 7374 6174 7573 3a20 2731 3027 0a20    status: '10'. 
+0002ce70: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0002ce80: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+0002ce90: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
+0002cea0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+0002ceb0: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
+0002cec0: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
+0002ced0: 6f6e 7365 2c20 2764 6174 6127 2c20 7b7d  onse, 'data', {}
+0002cee0: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
+0002cef0: 616e 7366 6572 203d 2073 656c 662e 7061  ansfer = self.pa
+0002cf00: 7273 655f 7472 616e 7366 6572 2864 6174  rse_transfer(dat
+0002cf10: 612c 2063 7572 7265 6e63 7929 0a20 2020  a, currency).   
+0002cf20: 2020 2020 2065 6c73 653a 2020 2320 7375       else:  # su
+0002cf30: 6220 6163 636f 756e 7420 7472 616e 7366  b account transf
+0002cf40: 6572 0a20 2020 2020 2020 2020 2020 2072  er.            r
+0002cf50: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
+0002cf60: 2020 2020 2020 2020 2020 2027 6672 6f6d             'from
+0002cf70: 5573 6572 4964 273a 2066 726f 6d49 642c  UserId': fromId,
+0002cf80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cf90: 2027 746f 5573 6572 4964 273a 2074 6f49   'toUserId': toI
+0002cfa0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0002cfb0: 2020 2027 616d 6f75 6e74 4576 273a 2073     'amountEv': s
+0002cfc0: 6361 6c65 6441 6d6d 6f75 6e74 2c0a 2020  caledAmmount,.  
+0002cfd0: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+0002cfe0: 7572 7265 6e63 7927 3a20 6375 7272 656e  urrency': curren
+0002cff0: 6379 5b27 6964 275d 2c0a 2020 2020 2020  cy['id'],.      
+0002d000: 2020 2020 2020 2020 2020 2762 697a 5479            'bizTy
+0002d010: 7065 273a 2073 656c 662e 7361 6665 5f73  pe': self.safe_s
+0002d020: 7472 696e 6728 7061 7261 6d73 2c20 2762  tring(params, 'b
+0002d030: 697a 5479 7065 272c 2027 5350 4f54 2729  izType', 'SPOT')
+0002d040: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+0002d050: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0002d060: 6f6e 7365 203d 2073 656c 662e 7072 6976  onse = self.priv
+0002d070: 6174 6550 6f73 7441 7373 6574 7355 6e69  atePostAssetsUni
+0002d080: 7665 7273 616c 5472 616e 7366 6572 2873  versalTransfer(s
+0002d090: 656c 662e 6578 7465 6e64 2872 6571 7565  elf.extend(reque
+0002d0a0: 7374 2c20 7061 7261 6d73 2929 0a20 2020  st, params)).   
+0002d0b0: 2020 2020 2020 2020 2023 0a20 2020 2020           #.     
+0002d0c0: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
+0002d0d0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0002d0e0: 2020 2020 2063 6f64 653a 2027 3027 2c0a       code: '0',.
+0002d0f0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0002d100: 2020 2020 2020 6d73 673a 2027 4f4b 272c        msg: 'OK',
+0002d110: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0002d120: 2020 2020 2020 2064 6174 613a 2027 4150         data: 'AP
+0002d130: 492d 3932 3364 6238 3236 2d61 6161 612d  I-923db826-aaaa-
+0002d140: 6161 6161 2d61 6161 612d 3464 3938 6333  aaaa-aaaa-4d98c3
+0002d150: 6137 6339 6664 270a 2020 2020 2020 2020  a7c9fd'.        
+0002d160: 2020 2020 2320 2020 2020 7d0a 2020 2020      #     }.    
+0002d170: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0002d180: 2020 2020 2020 7472 616e 7366 6572 203d        transfer =
+0002d190: 2073 656c 662e 7061 7273 655f 7472 616e   self.parse_tran
+0002d1a0: 7366 6572 2872 6573 706f 6e73 6529 0a20  sfer(response). 
+0002d1b0: 2020 2020 2020 2074 7261 6e73 6665 724f         transferO
+0002d1c0: 7074 696f 6e73 203d 2073 656c 662e 7361  ptions = self.sa
+0002d1d0: 6665 5f76 616c 7565 2873 656c 662e 6f70  fe_value(self.op
+0002d1e0: 7469 6f6e 732c 2027 7472 616e 7366 6572  tions, 'transfer
+0002d1f0: 272c 207b 7d29 0a20 2020 2020 2020 2066  ', {}).        f
+0002d200: 696c 6c52 6573 706f 6e73 6546 726f 6d52  illResponseFromR
+0002d210: 6571 7565 7374 203d 2073 656c 662e 7361  equest = self.sa
+0002d220: 6665 5f76 616c 7565 2874 7261 6e73 6665  fe_value(transfe
+0002d230: 724f 7074 696f 6e73 2c20 2766 696c 6c52  rOptions, 'fillR
+0002d240: 6573 706f 6e73 6546 726f 6d52 6571 7565  esponseFromReque
+0002d250: 7374 272c 2054 7275 6529 0a20 2020 2020  st', True).     
+0002d260: 2020 2069 6620 6669 6c6c 5265 7370 6f6e     if fillRespon
+0002d270: 7365 4672 6f6d 5265 7175 6573 743a 0a20  seFromRequest:. 
+0002d280: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
+0002d290: 616e 7366 6572 5b27 6672 6f6d 4163 636f  ansfer['fromAcco
+0002d2a0: 756e 7427 5d20 6973 204e 6f6e 653a 0a20  unt'] is None:. 
+0002d2b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0002d2c0: 7261 6e73 6665 725b 2766 726f 6d41 6363  ransfer['fromAcc
+0002d2d0: 6f75 6e74 275d 203d 2066 726f 6d41 6363  ount'] = fromAcc
+0002d2e0: 6f75 6e74 0a20 2020 2020 2020 2020 2020  ount.           
+0002d2f0: 2069 6620 7472 616e 7366 6572 5b27 746f   if transfer['to
+0002d300: 4163 636f 756e 7427 5d20 6973 204e 6f6e  Account'] is Non
+0002d310: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002d320: 2020 2074 7261 6e73 6665 725b 2774 6f41     transfer['toA
+0002d330: 6363 6f75 6e74 275d 203d 2074 6f41 6363  ccount'] = toAcc
+0002d340: 6f75 6e74 0a20 2020 2020 2020 2020 2020  ount.           
+0002d350: 2069 6620 7472 616e 7366 6572 5b27 616d   if transfer['am
+0002d360: 6f75 6e74 275d 2069 7320 4e6f 6e65 3a0a  ount'] is None:.
+0002d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d380: 7472 616e 7366 6572 5b27 616d 6f75 6e74  transfer['amount
+0002d390: 275d 203d 2061 6d6f 756e 740a 2020 2020  '] = amount.    
+0002d3a0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
+0002d3b0: 6665 725b 2763 7572 7265 6e63 7927 5d20  fer['currency'] 
+0002d3c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0002d3d0: 2020 2020 2020 2020 2074 7261 6e73 6665           transfe
+0002d3e0: 725b 2763 7572 7265 6e63 7927 5d20 3d20  r['currency'] = 
+0002d3f0: 636f 6465 0a20 2020 2020 2020 2072 6574  code.        ret
+0002d400: 7572 6e20 7472 616e 7366 6572 0a0a 2020  urn transfer..  
+0002d410: 2020 6465 6620 6665 7463 685f 7472 616e    def fetch_tran
+0002d420: 7366 6572 7328 7365 6c66 2c20 636f 6465  sfers(self, code
+0002d430: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0002d440: 3d20 4e6f 6e65 2c20 7369 6e63 653a 204f  = None, since: O
+0002d450: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0002d460: 6f6e 652c 206c 696d 6974 3a20 4f70 7469  one, limit: Opti
+0002d470: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0002d480: 2c20 7061 7261 6d73 3d7b 7d29 3a0a 2020  , params={}):.  
+0002d490: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002d4a0: 2020 6665 7463 6820 6120 6869 7374 6f72    fetch a histor
+0002d4b0: 7920 6f66 2069 6e74 6572 6e61 6c20 7472  y of internal tr
+0002d4c0: 616e 7366 6572 7320 6d61 6465 206f 6e20  ansfers made on 
+0002d4d0: 616e 2061 6363 6f75 6e74 0a20 2020 2020  an account.     
+0002d4e0: 2020 203a 7061 7261 6d20 7374 727c 4e6f     :param str|No
+0002d4f0: 6e65 2063 6f64 653a 2075 6e69 6669 6564  ne code: unified
+0002d500: 2063 7572 7265 6e63 7920 636f 6465 206f   currency code o
+0002d510: 6620 7468 6520 6375 7272 656e 6379 2074  f the currency t
+0002d520: 7261 6e73 6665 7272 6564 0a20 2020 2020  ransferred.     
+0002d530: 2020 203a 7061 7261 6d20 696e 747c 4e6f     :param int|No
+0002d540: 6e65 2073 696e 6365 3a20 7468 6520 6561  ne since: the ea
+0002d550: 726c 6965 7374 2074 696d 6520 696e 206d  rliest time in m
+0002d560: 7320 746f 2066 6574 6368 2074 7261 6e73  s to fetch trans
+0002d570: 6665 7273 2066 6f72 0a20 2020 2020 2020  fers for.       
+0002d580: 203a 7061 7261 6d20 696e 747c 4e6f 6e65   :param int|None
+0002d590: 206c 696d 6974 3a20 7468 6520 6d61 7869   limit: the maxi
+0002d5a0: 6d75 6d20 6e75 6d62 6572 206f 6620 2074  mum number of  t
+0002d5b0: 7261 6e73 6665 7273 2073 7472 7563 7475  ransfers structu
+0002d5c0: 7265 7320 746f 2072 6574 7269 6576 650a  res to retrieve.
+0002d5d0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+0002d5e0: 6963 7420 7061 7261 6d73 3a20 6578 7472  ict params: extr
+0002d5f0: 6120 7061 7261 6d65 7465 7273 2073 7065  a parameters spe
+0002d600: 6369 6669 6320 746f 2074 6865 2070 6865  cific to the phe
+0002d610: 6d65 7820 6170 6920 656e 6470 6f69 6e74  mex api endpoint
+0002d620: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0002d630: 7320 5b64 6963 745d 3a20 6120 6c69 7374  s [dict]: a list
+0002d640: 206f 6620 6074 7261 6e73 6665 7220 7374   of `transfer st
+0002d650: 7275 6374 7572 6573 203c 6874 7470 733a  ructures <https:
+0002d660: 2f2f 646f 6373 2e63 6378 742e 636f 6d2f  //docs.ccxt.com/
+0002d670: 232f 3f69 643d 7472 616e 7366 6572 2d73  #/?id=transfer-s
+0002d680: 7472 7563 7475 7265 3e60 0a20 2020 2020  tructure>`.     
+0002d690: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0002d6a0: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+0002d6b0: 2829 0a20 2020 2020 2020 2069 6620 636f  ().        if co
+0002d6c0: 6465 2069 7320 4e6f 6e65 3a0a 2020 2020  de is None:.    
+0002d6d0: 2020 2020 2020 2020 7261 6973 6520 4172          raise Ar
+0002d6e0: 6775 6d65 6e74 7352 6571 7569 7265 6428  gumentsRequired(
+0002d6f0: 7365 6c66 2e69 6420 2b20 2720 6665 7463  self.id + ' fetc
+0002d700: 6854 7261 6e73 6665 7273 2829 2072 6571  hTransfers() req
+0002d710: 7569 7265 7320 6120 636f 6465 2061 7267  uires a code arg
+0002d720: 756d 656e 7427 290a 2020 2020 2020 2020  ument').        
+0002d730: 6375 7272 656e 6379 203d 2073 656c 662e  currency = self.
+0002d740: 6375 7272 656e 6379 2863 6f64 6529 0a20  currency(code). 
+0002d750: 2020 2020 2020 2072 6571 7565 7374 203d         request =
+0002d760: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0002d770: 6375 7272 656e 6379 273a 2063 7572 7265  currency': curre
+0002d780: 6e63 795b 2769 6427 5d2c 0a20 2020 2020  ncy['id'],.     
+0002d790: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
+0002d7a0: 7369 6e63 6520 6973 206e 6f74 204e 6f6e  since is not Non
+0002d7b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002d7c0: 6571 7565 7374 5b27 7374 6172 7427 5d20  equest['start'] 
+0002d7d0: 3d20 7369 6e63 650a 2020 2020 2020 2020  = since.        
+0002d7e0: 6966 206c 696d 6974 2069 7320 6e6f 7420  if limit is not 
+0002d7f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002d800: 2020 7265 7175 6573 745b 276c 696d 6974    request['limit
+0002d810: 275d 203d 206c 696d 6974 0a20 2020 2020  '] = limit.     
+0002d820: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+0002d830: 6c66 2e70 7269 7661 7465 4765 7441 7373  lf.privateGetAss
+0002d840: 6574 7354 7261 6e73 6665 7228 7365 6c66  etsTransfer(self
+0002d850: 2e65 7874 656e 6428 7265 7175 6573 742c  .extend(request,
+0002d860: 2070 6172 616d 7329 290a 2020 2020 2020   params)).      
+0002d870: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
+0002d880: 2020 7b0a 2020 2020 2020 2020 2320 2020    {.        #   
+0002d890: 2020 2020 2020 2263 6f64 6522 3a20 302c        "code": 0,
+0002d8a0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002d8b0: 2020 2022 6d73 6722 3a20 224f 4b22 2c0a     "msg": "OK",.
+0002d8c0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002d8d0: 2020 2264 6174 6122 3a20 7b0a 2020 2020    "data": {.    
+0002d8e0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0002d8f0: 2020 2272 6f77 7322 3a20 5b0a 2020 2020    "rows": [.    
+0002d900: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0002d910: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0002d920: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0002d930: 2020 2020 2020 226c 696e 6b4b 6579 223a        "linkKey":
+0002d940: 2022 3837 6330 3731 6133 2d38 3632 382d   "87c071a3-8628-
+0002d950: 3461 6332 2d61 6361 312d 3663 6530 6431  4ac2-aca1-6ce0d1
+0002d960: 6661 6436 3663 222c 0a20 2020 2020 2020  fad66c",.       
+0002d970: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0002d980: 2020 2020 2020 2022 7573 6572 4964 223a         "userId":
+0002d990: 2034 3134 3834 3238 2c0a 2020 2020 2020   4148428,.      
+0002d9a0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0002d9b0: 2020 2020 2020 2020 2263 7572 7265 6e63          "currenc
+0002d9c0: 7922 3a20 2242 5443 222c 0a20 2020 2020  y": "BTC",.     
+0002d9d0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0002d9e0: 2020 2020 2020 2020 2022 616d 6f75 6e74           "amount
+0002d9f0: 4576 223a 2036 3739 3332 2c0a 2020 2020  Ev": 67932,.    
+0002da00: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0002da10: 2020 2020 2020 2020 2020 2273 6964 6522            "side"
+0002da20: 3a20 322c 0a20 2020 2020 2020 2023 2020  : 2,.        #  
+0002da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002da40: 2020 2022 7374 6174 7573 223a 2031 302c     "status": 10,
+0002da50: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002da60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0002da70: 6372 6561 7465 5469 6d65 223a 2031 3635  createTime": 165
+0002da80: 3238 3332 3436 3730 3030 2c0a 2020 2020  2832467000,.    
+0002da90: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0002daa0: 2020 2020 2020 2020 2020 2262 697a 5479            "bizTy
+0002dab0: 7065 223a 2031 300a 2020 2020 2020 2020  pe": 10.        
+0002dac0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0002dad0: 2020 7d0a 2020 2020 2020 2020 2320 2020    }.        #   
+0002dae0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+0002daf0: 2020 2020 2320 2020 2020 2020 2020 7d0a      #         }.
+0002db00: 2020 2020 2020 2020 2320 2020 2020 7d0a          #     }.
+0002db10: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+0002db20: 2020 6461 7461 203d 2073 656c 662e 7361    data = self.sa
+0002db30: 6665 5f76 616c 7565 2872 6573 706f 6e73  fe_value(respons
+0002db40: 652c 2027 6461 7461 272c 207b 7d29 0a20  e, 'data', {}). 
+0002db50: 2020 2020 2020 2074 7261 6e73 6665 7273         transfers
+0002db60: 203d 2073 656c 662e 7361 6665 5f76 616c   = self.safe_val
+0002db70: 7565 2864 6174 612c 2027 726f 7773 272c  ue(data, 'rows',
+0002db80: 205b 5d29 0a20 2020 2020 2020 2072 6574   []).        ret
+0002db90: 7572 6e20 7365 6c66 2e70 6172 7365 5f74  urn self.parse_t
+0002dba0: 7261 6e73 6665 7273 2874 7261 6e73 6665  ransfers(transfe
+0002dbb0: 7273 2c20 6375 7272 656e 6379 2c20 7369  rs, currency, si
+0002dbc0: 6e63 652c 206c 696d 6974 290a 0a20 2020  nce, limit)..   
+0002dbd0: 2064 6566 2070 6172 7365 5f74 7261 6e73   def parse_trans
+0002dbe0: 6665 7228 7365 6c66 2c20 7472 616e 7366  fer(self, transf
+0002dbf0: 6572 2c20 6375 7272 656e 6379 3d4e 6f6e  er, currency=Non
+0002dc00: 6529 3a0a 2020 2020 2020 2020 230a 2020  e):.        #.  
+0002dc10: 2020 2020 2020 2320 7472 616e 7366 6572        # transfer
+0002dc20: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0002dc30: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+0002dc40: 2020 2023 2020 2020 2020 2020 206c 696e     #         lin
+0002dc50: 6b4b 6579 3a20 2738 3536 3465 6261 342d  kKey: '8564eba4-
+0002dc60: 6339 6563 2d34 3964 362d 3962 3863 2d32  c9ec-49d6-9b8c-2
+0002dc70: 6563 3530 3031 6130 6662 3927 2c0a 2020  ec5001a0fb9',.  
+0002dc80: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0002dc90: 7573 6572 4964 3a20 2734 3031 3833 3430  userId: '4018340
+0002dca0: 272c 0a20 2020 2020 2020 2023 2020 2020  ',.        #    
+0002dcb0: 2020 2020 2063 7572 7265 6e63 793a 2027       currency: '
+0002dcc0: 5553 4427 2c0a 2020 2020 2020 2020 2320  USD',.        # 
+0002dcd0: 2020 2020 2020 2020 616d 6f75 6e74 4576          amountEv
+0002dce0: 3a20 2731 3027 2c0a 2020 2020 2020 2020  : '10',.        
+0002dcf0: 2320 2020 2020 2020 2020 7369 6465 3a20  #         side: 
+0002dd00: 2732 272c 0a20 2020 2020 2020 2023 2020  '2',.        #  
+0002dd10: 2020 2020 2020 2073 7461 7475 733a 2027         status: '
+0002dd20: 3130 270a 2020 2020 2020 2020 2320 2020  10'.        #   
+0002dd30: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
+0002dd40: 2020 2020 2020 2320 6665 7463 6854 7261        # fetchTra
+0002dd50: 6e73 6665 7273 0a20 2020 2020 2020 2023  nsfers.        #
+0002dd60: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+0002dd70: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002dd80: 2020 2022 6c69 6e6b 4b65 7922 3a20 2238     "linkKey": "8
+0002dd90: 3763 3037 3161 332d 3836 3238 2d34 6163  7c071a3-8628-4ac
+0002dda0: 322d 6163 6131 2d36 6365 3064 3166 6164  2-aca1-6ce0d1fad
+0002ddb0: 3636 6322 2c0a 2020 2020 2020 2020 2320  66c",.        # 
+0002ddc0: 2020 2020 2020 2020 2275 7365 7249 6422          "userId"
+0002ddd0: 3a20 3431 3438 3432 382c 0a20 2020 2020  : 4148428,.     
+0002dde0: 2020 2023 2020 2020 2020 2020 2022 6375     #         "cu
+0002ddf0: 7272 656e 6379 223a 2022 4254 4322 2c0a  rrency": "BTC",.
+0002de00: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002de10: 2020 2261 6d6f 756e 7445 7622 3a20 3637    "amountEv": 67
+0002de20: 3933 322c 0a20 2020 2020 2020 2023 2020  932,.        #  
+0002de30: 2020 2020 2020 2022 7369 6465 223a 2032         "side": 2
+0002de40: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0002de50: 2020 2020 2273 7461 7475 7322 3a20 3130      "status": 10
+0002de60: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0002de70: 2020 2020 2263 7265 6174 6554 696d 6522      "createTime"
+0002de80: 3a20 3136 3532 3833 3234 3637 3030 302c  : 1652832467000,
+0002de90: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002dea0: 2020 2022 6269 7a54 7970 6522 3a20 3130     "bizType": 10
+0002deb0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+0002dec0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+0002ded0: 2020 2069 6420 3d20 7365 6c66 2e73 6166     id = self.saf
+0002dee0: 655f 7374 7269 6e67 2874 7261 6e73 6665  e_string(transfe
+0002def0: 722c 2027 6c69 6e6b 4b65 7927 290a 2020  r, 'linkKey').  
+0002df00: 2020 2020 2020 7374 6174 7573 203d 2073        status = s
+0002df10: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0002df20: 7472 616e 7366 6572 2c20 2773 7461 7475  transfer, 'statu
+0002df30: 7327 290a 2020 2020 2020 2020 616d 6f75  s').        amou
+0002df40: 6e74 4576 203d 2073 656c 662e 7361 6665  ntEv = self.safe
+0002df50: 5f73 7472 696e 6728 7472 616e 7366 6572  _string(transfer
+0002df60: 2c20 2761 6d6f 756e 7445 7627 290a 2020  , 'amountEv').  
+0002df70: 2020 2020 2020 616d 6f75 6e74 5472 616e        amountTran
+0002df80: 7366 6572 6564 203d 2073 656c 662e 6672  sfered = self.fr
+0002df90: 6f6d 5f65 7628 616d 6f75 6e74 4576 2c20  om_ev(amountEv, 
+0002dfa0: 6375 7272 656e 6379 290a 2020 2020 2020  currency).      
+0002dfb0: 2020 6375 7272 656e 6379 4964 203d 2073    currencyId = s
+0002dfc0: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0002dfd0: 7472 616e 7366 6572 2c20 2763 7572 7265  transfer, 'curre
+0002dfe0: 6e63 7927 290a 2020 2020 2020 2020 636f  ncy').        co
+0002dff0: 6465 203d 2073 656c 662e 7361 6665 5f63  de = self.safe_c
+0002e000: 7572 7265 6e63 795f 636f 6465 2863 7572  urrency_code(cur
+0002e010: 7265 6e63 7949 642c 2063 7572 7265 6e63  rencyId, currenc
+0002e020: 7929 0a20 2020 2020 2020 2073 6964 6520  y).        side 
+0002e030: 3d20 7365 6c66 2e73 6166 655f 696e 7465  = self.safe_inte
+0002e040: 6765 7228 7472 616e 7366 6572 2c20 2773  ger(transfer, 's
+0002e050: 6964 6527 290a 2020 2020 2020 2020 6672  ide').        fr
+0002e060: 6f6d 4964 203d 204e 6f6e 650a 2020 2020  omId = None.    
+0002e070: 2020 2020 746f 4964 203d 204e 6f6e 650a      toId = None.
+0002e080: 2020 2020 2020 2020 6966 2073 6964 6520          if side 
+0002e090: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+0002e0a0: 2020 6672 6f6d 4964 203d 2027 7377 6170    fromId = 'swap
+0002e0b0: 270a 2020 2020 2020 2020 2020 2020 746f  '.            to
+0002e0c0: 4964 203d 2027 7370 6f74 270a 2020 2020  Id = 'spot'.    
+0002e0d0: 2020 2020 656c 6966 2073 6964 6520 3d3d      elif side ==
+0002e0e0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0002e0f0: 6672 6f6d 4964 203d 2027 7370 6f74 270a  fromId = 'spot'.
+0002e100: 2020 2020 2020 2020 2020 2020 746f 4964              toId
+0002e110: 203d 2027 7377 6170 270a 2020 2020 2020   = 'swap'.      
+0002e120: 2020 7469 6d65 7374 616d 7020 3d20 7365    timestamp = se
+0002e130: 6c66 2e73 6166 655f 696e 7465 6765 7228  lf.safe_integer(
+0002e140: 7472 616e 7366 6572 2c20 2763 7265 6174  transfer, 'creat
+0002e150: 6554 696d 6527 290a 2020 2020 2020 2020  eTime').        
+0002e160: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
+0002e170: 2020 2020 2027 696e 666f 273a 2074 7261       'info': tra
+0002e180: 6e73 6665 722c 0a20 2020 2020 2020 2020  nsfer,.         
+0002e190: 2020 2027 6964 273a 2069 642c 0a20 2020     'id': id,.   
+0002e1a0: 2020 2020 2020 2020 2027 7469 6d65 7374           'timest
+0002e1b0: 616d 7027 3a20 7469 6d65 7374 616d 702c  amp': timestamp,
+0002e1c0: 0a20 2020 2020 2020 2020 2020 2027 6461  .            'da
+0002e1d0: 7465 7469 6d65 273a 2073 656c 662e 6973  tetime': self.is
+0002e1e0: 6f38 3630 3128 7469 6d65 7374 616d 7029  o8601(timestamp)
+0002e1f0: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
+0002e200: 7572 7265 6e63 7927 3a20 636f 6465 2c0a  urrency': code,.
+0002e210: 2020 2020 2020 2020 2020 2020 2761 6d6f              'amo
+0002e220: 756e 7427 3a20 616d 6f75 6e74 5472 616e  unt': amountTran
+0002e230: 7366 6572 6564 2c0a 2020 2020 2020 2020  sfered,.        
+0002e240: 2020 2020 2766 726f 6d41 6363 6f75 6e74      'fromAccount
+0002e250: 273a 2066 726f 6d49 642c 0a20 2020 2020  ': fromId,.     
+0002e260: 2020 2020 2020 2027 746f 4163 636f 756e         'toAccoun
+0002e270: 7427 3a20 746f 4964 2c0a 2020 2020 2020  t': toId,.      
+0002e280: 2020 2020 2020 2773 7461 7475 7327 3a20        'status': 
+0002e290: 7365 6c66 2e70 6172 7365 5f74 7261 6e73  self.parse_trans
+0002e2a0: 6665 725f 7374 6174 7573 2873 7461 7475  fer_status(statu
+0002e2b0: 7329 2c0a 2020 2020 2020 2020 7d0a 0a20  s),.        }.. 
+0002e2c0: 2020 2064 6566 2070 6172 7365 5f74 7261     def parse_tra
+0002e2d0: 6e73 6665 725f 7374 6174 7573 2873 656c  nsfer_status(sel
+0002e2e0: 662c 2073 7461 7475 7329 3a0a 2020 2020  f, status):.    
+0002e2f0: 2020 2020 7374 6174 7573 6573 203d 207b      statuses = {
+0002e300: 0a20 2020 2020 2020 2020 2020 2027 3327  .            '3'
+0002e310: 3a20 2772 656a 6563 7465 6427 2c20 2023  : 'rejected',  #
+0002e320: 2027 5265 6a65 6374 6564 272c 0a20 2020   'Rejected',.   
+0002e330: 2020 2020 2020 2020 2027 3627 3a20 2763           '6': 'c
+0002e340: 616e 6365 6c65 6427 2c20 2023 2027 476f  anceled',  # 'Go
+0002e350: 7420 6572 726f 7220 616e 6420 7761 6974  t error and wait
+0002e360: 2066 6f72 2072 6563 6f76 6572 7927 2c0a   for recovery',.
+0002e370: 2020 2020 2020 2020 2020 2020 2731 3027              '10'
+0002e380: 3a20 276f 6b27 2c20 2023 2027 5375 6363  : 'ok',  # 'Succ
+0002e390: 6573 7327 2c0a 2020 2020 2020 2020 2020  ess',.          
+0002e3a0: 2020 2731 3127 3a20 2766 6169 6c65 6427    '11': 'failed'
+0002e3b0: 2c20 2023 2027 4661 696c 6564 272c 0a20  ,  # 'Failed',. 
+0002e3c0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0002e3d0: 2072 6574 7572 6e20 7365 6c66 2e73 6166   return self.saf
+0002e3e0: 655f 7374 7269 6e67 2873 7461 7475 7365  e_string(statuse
+0002e3f0: 732c 2073 7461 7475 732c 2073 7461 7475  s, status, statu
+0002e400: 7329 0a0a 2020 2020 6465 6620 6665 7463  s)..    def fetc
+0002e410: 685f 6675 6e64 696e 675f 7261 7465 5f68  h_funding_rate_h
+0002e420: 6973 746f 7279 2873 656c 662c 2073 796d  istory(self, sym
+0002e430: 626f 6c3a 204f 7074 696f 6e61 6c5b 7374  bol: Optional[st
+0002e440: 725d 203d 204e 6f6e 652c 2073 696e 6365  r] = None, since
+0002e450: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+0002e460: 3d20 4e6f 6e65 2c20 6c69 6d69 743a 204f  = None, limit: O
+0002e470: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0002e480: 6f6e 652c 2070 6172 616d 733d 7b7d 293a  one, params={}):
+0002e490: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+0002e4a0: 6563 6b5f 7265 7175 6972 6564 5f73 796d  eck_required_sym
+0002e4b0: 626f 6c28 2766 6574 6368 4675 6e64 696e  bol('fetchFundin
+0002e4c0: 6752 6174 6548 6973 746f 7279 272c 2073  gRateHistory', s
+0002e4d0: 796d 626f 6c29 0a20 2020 2020 2020 2073  ymbol).        s
+0002e4e0: 656c 662e 6c6f 6164 5f6d 6172 6b65 7473  elf.load_markets
+0002e4f0: 2829 0a20 2020 2020 2020 206d 6172 6b65  ().        marke
+0002e500: 7420 3d20 7365 6c66 2e6d 6172 6b65 7428  t = self.market(
+0002e510: 7379 6d62 6f6c 290a 2020 2020 2020 2020  symbol).        
+0002e520: 6973 5573 6474 5365 7474 6c65 6420 3d20  isUsdtSettled = 
+0002e530: 6d61 726b 6574 5b27 7365 7474 6c65 275d  market['settle']
+0002e540: 203d 3d20 2755 5344 5427 0a20 2020 2020   == 'USDT'.     
+0002e550: 2020 2069 6620 6e6f 7420 6d61 726b 6574     if not market
+0002e560: 5b27 7377 6170 275d 3a0a 2020 2020 2020  ['swap']:.      
+0002e570: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
+0002e580: 6571 7565 7374 2873 656c 662e 6964 202b  equest(self.id +
+0002e590: 2027 2066 6574 6368 4675 6e64 696e 6752   ' fetchFundingR
+0002e5a0: 6174 6548 6973 746f 7279 2829 2073 7570  ateHistory() sup
+0002e5b0: 706f 7274 7320 7377 6170 2063 6f6e 7472  ports swap contr
+0002e5c0: 6163 7473 206f 6e6c 7927 290a 2020 2020  acts only').    
+0002e5d0: 2020 2020 6375 7374 6f6d 5379 6d62 6f6c      customSymbol
+0002e5e0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0002e5f0: 6966 2069 7355 7364 7453 6574 746c 6564  if isUsdtSettled
+0002e600: 3a0a 2020 2020 2020 2020 2020 2020 6375  :.            cu
+0002e610: 7374 6f6d 5379 6d62 6f6c 203d 2027 2e27  stomSymbol = '.'
+0002e620: 202b 206d 6172 6b65 745b 2769 6427 5d20   + market['id'] 
+0002e630: 2b20 2746 5238 4827 2020 2320 7068 656d  + 'FR8H'  # phem
+0002e640: 6578 2072 6571 7569 7265 7320 6120 6375  ex requires a cu
+0002e650: 7374 6f6d 2073 796d 626f 6c20 666f 7220  stom symbol for 
+0002e660: 6675 6e64 696e 6720 7261 7465 2068 6973  funding rate his
+0002e670: 746f 7279 0a20 2020 2020 2020 2065 6c73  tory.        els
+0002e680: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+0002e690: 7573 746f 6d53 796d 626f 6c20 3d20 272e  ustomSymbol = '.
+0002e6a0: 2720 2b20 6d61 726b 6574 5b27 6261 7365  ' + market['base
+0002e6b0: 4964 275d 202b 2027 4652 3848 270a 2020  Id'] + 'FR8H'.  
+0002e6c0: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
+0002e6d0: 7b0a 2020 2020 2020 2020 2020 2020 2773  {.            's
+0002e6e0: 796d 626f 6c27 3a20 6375 7374 6f6d 5379  ymbol': customSy
+0002e6f0: 6d62 6f6c 2c0a 2020 2020 2020 2020 7d0a  mbol,.        }.
+0002e700: 2020 2020 2020 2020 6966 2073 696e 6365          if since
+0002e710: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002e720: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+0002e730: 745b 2773 7461 7274 275d 203d 2073 696e  t['start'] = sin
+0002e740: 6365 0a20 2020 2020 2020 2069 6620 6c69  ce.        if li
+0002e750: 6d69 7420 6973 206e 6f74 204e 6f6e 653a  mit is not None:
+0002e760: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+0002e770: 7565 7374 5b27 6c69 6d69 7427 5d20 3d20  uest['limit'] = 
+0002e780: 6c69 6d69 740a 2020 2020 2020 2020 7265  limit.        re
+0002e790: 7370 6f6e 7365 203d 204e 6f6e 650a 2020  sponse = None.  
+0002e7a0: 2020 2020 2020 6966 2069 7355 7364 7453        if isUsdtS
+0002e7b0: 6574 746c 6564 3a0a 2020 2020 2020 2020  ettled:.        
+0002e7c0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+0002e7d0: 656c 662e 7632 4765 7441 7069 4461 7461  elf.v2GetApiData
+0002e7e0: 5075 626c 6963 4461 7461 4675 6e64 696e  PublicDataFundin
+0002e7f0: 6752 6174 6548 6973 746f 7279 2873 656c  gRateHistory(sel
+0002e800: 662e 6578 7465 6e64 2872 6571 7565 7374  f.extend(request
+0002e810: 2c20 7061 7261 6d73 2929 0a20 2020 2020  , params)).     
+0002e820: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002e830: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0002e840: 7365 6c66 2e76 3147 6574 4170 6944 6174  self.v1GetApiDat
+0002e850: 6150 7562 6c69 6344 6174 6146 756e 6469  aPublicDataFundi
+0002e860: 6e67 5261 7465 4869 7374 6f72 7928 7365  ngRateHistory(se
+0002e870: 6c66 2e65 7874 656e 6428 7265 7175 6573  lf.extend(reques
+0002e880: 742c 2070 6172 616d 7329 290a 2020 2020  t, params)).    
+0002e890: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
+0002e8a0: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
+0002e8b0: 2020 2020 2020 2263 6f64 6522 3a22 3022        "code":"0"
+0002e8c0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0002e8d0: 2020 2022 6d73 6722 3a22 4f4b 222c 0a20     "msg":"OK",. 
+0002e8e0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0002e8f0: 2264 6174 6122 3a7b 0a20 2020 2020 2020  "data":{.       
+0002e900: 2023 2020 2020 2020 2020 2020 2022 726f   #           "ro
+0002e910: 7773 223a 5b0a 2020 2020 2020 2020 2320  ws":[.        # 
+0002e920: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+0002e930: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0002e940: 2020 2020 2020 2020 2022 7379 6d62 6f6c           "symbol
+0002e950: 223a 222e 4254 4355 5344 5446 5238 4822  ":".BTCUSDTFR8H"
+0002e960: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+0002e970: 2020 2020 2020 2020 2020 2020 2266 756e              "fun
+0002e980: 6469 6e67 5261 7465 223a 2230 2e30 3030  dingRate":"0.000
+0002e990: 3122 2c0a 2020 2020 2020 2020 2320 2020  1",.        #   
+0002e9a0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+0002e9b0: 756e 6469 6e67 5469 6d65 223a 2231 3638  undingTime":"168
+0002e9c0: 3230 3634 3030 3030 3030 222c 0a20 2020  2064000000",.   
+0002e9d0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0002e9e0: 2020 2020 2020 2022 696e 7465 7276 616c         "interval
+0002e9f0: 5365 636f 6e64 7322 3a22 3238 3830 3022  Seconds":"28800"
+0002ea00: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002ea10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0002ea20: 2020 2320 2020 2020 2020 2020 2020 5d0a    #           ].
+0002ea30: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002ea40: 207d 0a20 2020 2020 2020 2023 2020 2020   }.        #    
+0002ea50: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
+0002ea60: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
+0002ea70: 7361 6665 5f76 616c 7565 2872 6573 706f  safe_value(respo
+0002ea80: 6e73 652c 2027 6461 7461 272c 207b 7d29  nse, 'data', {})
+0002ea90: 0a20 2020 2020 2020 2072 6174 6573 203d  .        rates =
+0002eaa0: 2073 656c 662e 7361 6665 5f76 616c 7565   self.safe_value
+0002eab0: 2864 6174 612c 2027 726f 7773 2729 0a20  (data, 'rows'). 
+0002eac0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0002ead0: 5b5d 0a20 2020 2020 2020 2066 6f72 2069  [].        for i
+0002eae0: 2069 6e20 7261 6e67 6528 302c 206c 656e   in range(0, len
+0002eaf0: 2872 6174 6573 2929 3a0a 2020 2020 2020  (rates)):.      
+0002eb00: 2020 2020 2020 6974 656d 203d 2072 6174        item = rat
+0002eb10: 6573 5b69 5d0a 2020 2020 2020 2020 2020  es[i].          
+0002eb20: 2020 7469 6d65 7374 616d 7020 3d20 7365    timestamp = se
+0002eb30: 6c66 2e73 6166 655f 696e 7465 6765 7228  lf.safe_integer(
+0002eb40: 6974 656d 2c20 2766 756e 6469 6e67 5469  item, 'fundingTi
+0002eb50: 6d65 2729 0a20 2020 2020 2020 2020 2020  me').           
+0002eb60: 2072 6573 756c 742e 6170 7065 6e64 287b   result.append({
+0002eb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002eb80: 2027 696e 666f 273a 2069 7465 6d2c 0a20   'info': item,. 
+0002eb90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002eba0: 7379 6d62 6f6c 273a 2073 796d 626f 6c2c  symbol': symbol,
+0002ebb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ebc0: 2027 6675 6e64 696e 6752 6174 6527 3a20   'fundingRate': 
+0002ebd0: 7365 6c66 2e73 6166 655f 6e75 6d62 6572  self.safe_number
+0002ebe0: 2869 7465 6d2c 2027 6675 6e64 696e 6752  (item, 'fundingR
+0002ebf0: 6174 6527 292c 0a20 2020 2020 2020 2020  ate'),.         
+0002ec00: 2020 2020 2020 2027 7469 6d65 7374 616d         'timestam
+0002ec10: 7027 3a20 7469 6d65 7374 616d 702c 0a20  p': timestamp,. 
+0002ec20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002ec30: 6461 7465 7469 6d65 273a 2073 656c 662e  datetime': self.
+0002ec40: 6973 6f38 3630 3128 7469 6d65 7374 616d  iso8601(timestam
+0002ec50: 7029 2c0a 2020 2020 2020 2020 2020 2020  p),.            
+0002ec60: 7d29 0a20 2020 2020 2020 2073 6f72 7465  }).        sorte
+0002ec70: 6420 3d20 7365 6c66 2e73 6f72 745f 6279  d = self.sort_by
+0002ec80: 2872 6573 756c 742c 2027 7469 6d65 7374  (result, 'timest
+0002ec90: 616d 7027 290a 2020 2020 2020 2020 7265  amp').        re
+0002eca0: 7475 726e 2073 656c 662e 6669 6c74 6572  turn self.filter
+0002ecb0: 5f62 795f 7379 6d62 6f6c 5f73 696e 6365  _by_symbol_since
+0002ecc0: 5f6c 696d 6974 2873 6f72 7465 642c 2073  _limit(sorted, s
+0002ecd0: 796d 626f 6c2c 2073 696e 6365 2c20 6c69  ymbol, since, li
+0002ece0: 6d69 7429 0a0a 2020 2020 6465 6620 6861  mit)..    def ha
+0002ecf0: 6e64 6c65 5f65 7272 6f72 7328 7365 6c66  ndle_errors(self
+0002ed00: 2c20 6874 7470 436f 6465 2c20 7265 6173  , httpCode, reas
+0002ed10: 6f6e 2c20 7572 6c2c 206d 6574 686f 642c  on, url, method,
+0002ed20: 2068 6561 6465 7273 2c20 626f 6479 2c20   headers, body, 
+0002ed30: 7265 7370 6f6e 7365 2c20 7265 7175 6573  response, reques
+0002ed40: 7448 6561 6465 7273 2c20 7265 7175 6573  tHeaders, reques
+0002ed50: 7442 6f64 7929 3a0a 2020 2020 2020 2020  tBody):.        
+0002ed60: 6966 2072 6573 706f 6e73 6520 6973 204e  if response is N
+0002ed70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002ed80: 2072 6574 7572 6e20 4e6f 6e65 2020 2320   return None  # 
+0002ed90: 6661 6c6c 6261 636b 2074 6f20 6465 6661  fallback to defa
+0002eda0: 756c 7420 6572 726f 7220 6861 6e64 6c65  ult error handle
+0002edb0: 720a 2020 2020 2020 2020 230a 2020 2020  r.        #.    
+0002edc0: 2020 2020 2320 2020 2020 7b22 636f 6465      #     {"code
+0002edd0: 223a 3330 3031 382c 226d 7367 223a 2270  ":30018,"msg":"p
+0002ede0: 6865 6d65 782e 6461 7461 2e73 697a 652e  hemex.data.size.
+0002edf0: 7570 6c69 6d74 222c 2264 6174 6122 3a6e  uplimt","data":n
+0002ee00: 756c 6c7d 0a20 2020 2020 2020 2023 2020  ull}.        #  
+0002ee10: 2020 207b 2263 6f64 6522 3a34 3132 2c22     {"code":412,"
+0002ee20: 6d73 6722 3a22 4d69 7373 696e 6720 7061  msg":"Missing pa
+0002ee30: 7261 6d65 7465 7220 2d20 7265 736f 6c75  rameter - resolu
+0002ee40: 7469 6f6e 222c 2264 6174 6122 3a6e 756c  tion","data":nul
+0002ee50: 6c7d 0a20 2020 2020 2020 2023 2020 2020  l}.        #    
+0002ee60: 207b 2263 6f64 6522 3a34 3132 2c22 6d73   {"code":412,"ms
+0002ee70: 6722 3a22 4d69 7373 696e 6720 7061 7261  g":"Missing para
+0002ee80: 6d65 7465 7220 2d20 746f 222c 2264 6174  meter - to","dat
+0002ee90: 6122 3a6e 756c 6c7d 0a20 2020 2020 2020  a":null}.       
+0002eea0: 2023 2020 2020 207b 2265 7272 6f72 223a   #     {"error":
+0002eeb0: 7b22 636f 6465 223a 3630 3031 2c22 6d65  {"code":6001,"me
+0002eec0: 7373 6167 6522 3a22 696e 7661 6c69 6420  ssage":"invalid 
+0002eed0: 6172 6775 6d65 6e74 227d 2c22 6964 223a  argument"},"id":
+0002eee0: 6e75 6c6c 2c22 7265 7375 6c74 223a 6e75  null,"result":nu
+0002eef0: 6c6c 7d0a 2020 2020 2020 2020 230a 2020  ll}.        #.  
+0002ef00: 2020 2020 2020 6572 726f 7220 3d20 7365        error = se
+0002ef10: 6c66 2e73 6166 655f 7661 6c75 6528 7265  lf.safe_value(re
+0002ef20: 7370 6f6e 7365 2c20 2765 7272 6f72 272c  sponse, 'error',
+0002ef30: 2072 6573 706f 6e73 6529 0a20 2020 2020   response).     
+0002ef40: 2020 2065 7272 6f72 436f 6465 203d 2073     errorCode = s
+0002ef50: 656c 662e 7361 6665 5f73 7472 696e 6728  elf.safe_string(
+0002ef60: 6572 726f 722c 2027 636f 6465 2729 0a20  error, 'code'). 
+0002ef70: 2020 2020 2020 206d 6573 7361 6765 203d         message =
+0002ef80: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
+0002ef90: 6728 6572 726f 722c 2027 6d73 6727 290a  g(error, 'msg').
+0002efa0: 2020 2020 2020 2020 6966 2028 6572 726f          if (erro
+0002efb0: 7243 6f64 6520 6973 206e 6f74 204e 6f6e  rCode is not Non
+0002efc0: 6529 2061 6e64 2028 6572 726f 7243 6f64  e) and (errorCod
+0002efd0: 6520 213d 2027 3027 293a 0a20 2020 2020  e != '0'):.     
+0002efe0: 2020 2020 2020 2066 6565 6462 6163 6b20         feedback 
+0002eff0: 3d20 7365 6c66 2e69 6420 2b20 2720 2720  = self.id + ' ' 
+0002f000: 2b20 626f 6479 0a20 2020 2020 2020 2020  + body.         
+0002f010: 2020 2073 656c 662e 7468 726f 775f 6578     self.throw_ex
+0002f020: 6163 746c 795f 6d61 7463 6865 645f 6578  actly_matched_ex
+0002f030: 6365 7074 696f 6e28 7365 6c66 2e65 7863  ception(self.exc
+0002f040: 6570 7469 6f6e 735b 2765 7861 6374 275d  eptions['exact']
+0002f050: 2c20 6572 726f 7243 6f64 652c 2066 6565  , errorCode, fee
+0002f060: 6462 6163 6b29 0a20 2020 2020 2020 2020  dback).         
+0002f070: 2020 2073 656c 662e 7468 726f 775f 6272     self.throw_br
+0002f080: 6f61 646c 795f 6d61 7463 6865 645f 6578  oadly_matched_ex
+0002f090: 6365 7074 696f 6e28 7365 6c66 2e65 7863  ception(self.exc
+0002f0a0: 6570 7469 6f6e 735b 2762 726f 6164 275d  eptions['broad']
+0002f0b0: 2c20 6d65 7373 6167 652c 2066 6565 6462  , message, feedb
+0002f0c0: 6163 6b29 0a20 2020 2020 2020 2020 2020  ack).           
+0002f0d0: 2072 6169 7365 2045 7863 6861 6e67 6545   raise ExchangeE
+0002f0e0: 7272 6f72 2866 6565 6462 6163 6b29 2020  rror(feedback)  
+0002f0f0: 2320 756e 6b6e 6f77 6e20 6d65 7373 6167  # unknown messag
+0002f100: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0002f110: 204e 6f6e 650a                            None.
```

### Comparing `ccxt-3.1.6/ccxt/poloniex.py` & `ccxt-3.1.7/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/poloniexfutures.py` & `ccxt-3.1.7/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/__init__.py` & `ccxt-3.1.7/ccxt/pro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-3.1.6/ccxt/pro/alpaca.py` & `ccxt-3.1.7/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/ascendex.py` & `ccxt-3.1.7/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bequant.py` & `ccxt-3.1.7/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/binance.py` & `ccxt-3.1.7/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/binancecoinm.py` & `ccxt-3.1.7/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/binanceus.py` & `ccxt-3.1.7/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/binanceusdm.py` & `ccxt-3.1.7/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitcoincom.py` & `ccxt-3.1.7/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitfinex.py` & `ccxt-3.1.7/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitfinex2.py` & `ccxt-3.1.7/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitget.py` & `ccxt-3.1.7/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitmart.py` & `ccxt-3.1.7/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitmex.py` & `ccxt-3.1.7/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitopro.py` & `ccxt-3.1.7/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitpanda.py` & `ccxt-3.1.7/ccxt/pro/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitrue.py` & `ccxt-3.1.7/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitstamp.py` & `ccxt-3.1.7/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bittrex.py` & `ccxt-3.1.7/ccxt/pro/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bitvavo.py` & `ccxt-3.1.7/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/blockchaincom.py` & `ccxt-3.1.7/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/btcex.py` & `ccxt-3.1.7/ccxt/pro/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/bybit.py` & `ccxt-3.1.7/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/cex.py` & `ccxt-3.1.7/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/coinbaseprime.py` & `ccxt-3.1.7/ccxt/pro/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/coinbasepro.py` & `ccxt-3.1.7/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/coinex.py` & `ccxt-3.1.7/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/cryptocom.py` & `ccxt-3.1.7/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/currencycom.py` & `ccxt-3.1.7/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/deribit.py` & `ccxt-3.1.7/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/exmo.py` & `ccxt-3.1.7/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/gate.py` & `ccxt-3.1.7/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/gemini.py` & `ccxt-3.1.7/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/hitbtc.py` & `ccxt-3.1.7/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/hollaex.py` & `ccxt-3.1.7/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/huobi.py` & `ccxt-3.1.7/ccxt/pro/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/huobijp.py` & `ccxt-3.1.7/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/idex.py` & `ccxt-3.1.7/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/independentreserve.py` & `ccxt-3.1.7/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/kraken.py` & `ccxt-3.1.7/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/krakenfutures.py` & `ccxt-3.1.7/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/kucoin.py` & `ccxt-3.1.7/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/kucoinfutures.py` & `ccxt-3.1.7/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/luno.py` & `ccxt-3.1.7/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/mexc.py` & `ccxt-3.1.7/ccxt/pro/mexc.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                     '4h': 'Hour4',
                     '8h': 'Hour8',
                     '1d': 'Day1',
                     '1w': 'Week1',
                     '1M': 'Month1',
                 },
                 'watchOrderBook': {
-                    'snapshotDelay': 5,
+                    'snapshotDelay': 25,
                     'maxRetries': 3,
                 },
                 'listenKey': None,
             },
             'streaming': {
                 'ping': self.ping,
                 'keepAlive': 10000,
@@ -434,15 +434,15 @@
             # once we have received the first delta and initialized the orderbook
             client.subscriptions[messageHash] = 1
             self.orderbooks[symbol] = self.counted_order_book({})
         storedOrderBook = self.safe_value(self.orderbooks, symbol)
         nonce = self.safe_integer(storedOrderBook, 'nonce')
         if nonce is None:
             cacheLength = len(storedOrderBook.cache)
-            snapshotDelay = self.handle_option('watchOrderBook', 'snapshotDelay', 5)
+            snapshotDelay = self.handle_option('watchOrderBook', 'snapshotDelay', 25)
             if cacheLength == snapshotDelay:
                 self.spawn(self.load_order_book, client, messageHash, symbol)
             storedOrderBook.cache.append(data)
             return
         try:
             self.handle_delta(storedOrderBook, data)
             timestamp = self.safe_integer(message, 't')
```

### Comparing `ccxt-3.1.6/ccxt/pro/ndax.py` & `ccxt-3.1.7/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/okcoin.py` & `ccxt-3.1.7/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/okx.py` & `ccxt-3.1.7/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/phemex.py` & `ccxt-3.1.7/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/poloniexfutures.py` & `ccxt-3.1.7/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/probit.py` & `ccxt-3.1.7/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/ripio.py` & `ccxt-3.1.7/ccxt/pro/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/upbit.py` & `ccxt-3.1.7/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/wazirx.py` & `ccxt-3.1.7/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/whitebit.py` & `ccxt-3.1.7/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/woo.py` & `ccxt-3.1.7/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/pro/zb.py` & `ccxt-3.1.7/ccxt/pro/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/probit.py` & `ccxt-3.1.7/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/ripio.py` & `ccxt-3.1.7/ccxt/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-3.1.7/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-3.1.7/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/stex.py` & `ccxt-3.1.7/ccxt/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/__init__.py` & `ccxt-3.1.7/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_account.py` & `ccxt-3.1.7/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_balance.py` & `ccxt-3.1.7/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_borrow_interest.py` & `ccxt-3.1.7/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_borrow_rate.py` & `ccxt-3.1.7/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_calculate_fee.py` & `ccxt-3.1.7/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_crypto.py` & `ccxt-3.1.7/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_currency.py` & `ccxt-3.1.7/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_datetime.py` & `ccxt-3.1.7/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-3.1.7/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_deep_extend.py` & `ccxt-3.1.7/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-3.1.7/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-3.1.7/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_funding_rate_history.py` & `ccxt-3.1.7/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_ledger_entry.py` & `ccxt-3.1.7/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_ledger_item.py` & `ccxt-3.1.7/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_leverage_tier.py` & `ccxt-3.1.7/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_margin_modification.py` & `ccxt-3.1.7/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_market.py` & `ccxt-3.1.7/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_number.py` & `ccxt-3.1.7/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_ohlcv.py` & `ccxt-3.1.7/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_open_interest.py` & `ccxt-3.1.7/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_order.py` & `ccxt-3.1.7/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_order_book.py` & `ccxt-3.1.7/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_position.py` & `ccxt-3.1.7/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_shared_methods.py` & `ccxt-3.1.7/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_status.py` & `ccxt-3.1.7/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_throttle.py` & `ccxt-3.1.7/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_ticker.py` & `ccxt-3.1.7/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_trade.py` & `ccxt-3.1.7/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_trading_fee.py` & `ccxt-3.1.7/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/base/test_transaction.py` & `ccxt-3.1.7/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/test_async.py` & `ccxt-3.1.7/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/test/test_sync.py` & `ccxt-3.1.7/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/tidex.py` & `ccxt-3.1.7/ccxt/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/timex.py` & `ccxt-3.1.7/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/tokocrypto.py` & `ccxt-3.1.7/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/upbit.py` & `ccxt-3.1.7/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/wavesexchange.py` & `ccxt-3.1.7/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/wazirx.py` & `ccxt-3.1.7/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/whitebit.py` & `ccxt-3.1.7/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/woo.py` & `ccxt-3.1.7/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/xt.py` & `ccxt-3.1.7/ccxt/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/yobit.py` & `ccxt-3.1.7/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/zaif.py` & `ccxt-3.1.7/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/zb.py` & `ccxt-3.1.7/ccxt/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt/zonda.py` & `ccxt-3.1.7/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/ccxt.egg-info/PKG-INFO` & `ccxt-3.1.7/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 3.1.6
+Version: 3.1.7
 Summary: A JavaScript / Python / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -228,21 +228,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.1.6/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@3.1.6/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.1.7/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@3.1.7/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.1.6/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.1.7/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-3.1.6/ccxt.egg-info/SOURCES.txt` & `ccxt-3.1.7/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-3.1.6/package.json` & `ccxt-3.1.7/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'3.1.7'"}*

```diff
@@ -219,9 +219,9 @@
         "update-badges": "node build/update-badges",
         "update-links": "node build/update-links",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "3.1.6"
+    "version": "3.1.7"
 }
```

### Comparing `ccxt-3.1.6/setup.py` & `ccxt-3.1.7/setup.py`

 * *Files identical despite different names*

