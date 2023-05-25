# Comparing `tmp/sharetop-1.2.4.tar.gz` & `tmp/sharetop-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.2.4.tar", last modified: Thu May  4 04:13:57 2023, max compression
+gzip compressed data, was "sharetop-1.3.4.tar", last modified: Tue May 16 14:29:17 2023, max compression
```

## Comparing `sharetop-1.2.4.tar` & `sharetop-1.3.4.tar`

### file list

```diff
@@ -1,72 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.167508 sharetop-1.2.4/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    39532 2023-05-04 04:13:57.166507 sharetop-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    38260 2023-05-02 15:48:40.000000 sharetop-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 04:13:57.167508 sharetop-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.069973 sharetop-1.2.4/sharetop/
--rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.2.4/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-05-04 04:13:40.000000 sharetop-1.2.4/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.120562 sharetop-1.2.4/sharetop/api/
--rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.2.4/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.122562 sharetop-1.2.4/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.2.4/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.2.4/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.127839 sharetop-1.2.4/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.2.4/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.131838 sharetop-1.2.4/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.2.4/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.2.4/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.2.4/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.2.4/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.134838 sharetop-1.2.4/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.2.4/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     2374 2023-05-02 15:19:23.000000 sharetop-1.2.4/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.2.4/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12266 2023-05-04 04:12:59.000000 sharetop-1.2.4/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.2.4/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.147263 sharetop-1.2.4/sharetop/core/fund/
--rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.2.4/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.2.4/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.149363 sharetop-1.2.4/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.2.4/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.2.4/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.154843 sharetop-1.2.4/sharetop/core/stock/
--rw-rw-rw-   0        0        0      569 2023-05-02 15:39:30.000000 sharetop-1.2.4/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.2.4/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.2.4/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14302 2023-05-02 01:29:25.000000 sharetop-1.2.4/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.2.4/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.2.4/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.2.4/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     6349 2023-05-04 04:01:07.000000 sharetop-1.2.4/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.160153 sharetop-1.2.4/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.2.4/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.2.4/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     2873 2023-05-02 14:46:41.000000 sharetop-1.2.4/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.163507 sharetop-1.2.4/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.2.4/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     3678 2023-05-03 06:46:06.000000 sharetop-1.2.4/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     1948 2023-05-02 15:34:17.000000 sharetop-1.2.4/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.166507 sharetop-1.2.4/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.2.4/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.2.4/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.2.4/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.2.4/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-1.2.4/sharetop/test/test4.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.119563 sharetop-1.2.4/sharetop.egg-info/
--rw-rw-rw-   0        0        0    39532 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1715 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.962612 sharetop-1.3.4/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0    47157 2023-05-16 14:29:17.958467 sharetop-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    45738 2023-05-16 14:18:16.000000 sharetop-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 14:29:17.962612 sharetop-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:16.509730 sharetop-1.3.4/sharetop/
+-rw-rw-rw-   0        0        0      262 2023-05-16 01:30:15.000000 sharetop-1.3.4/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-05-16 14:27:59.000000 sharetop-1.3.4/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:16.595367 sharetop-1.3.4/sharetop/api/
+-rw-rw-rw-   0        0        0      255 2023-05-16 01:11:05.000000 sharetop-1.3.4/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:16.648961 sharetop-1.3.4/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.3.4/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.3.4/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:16.721342 sharetop-1.3.4/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.3.4/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:16.894006 sharetop-1.3.4/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.3.4/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.3.4/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.3.4/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.3.4/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.3.4/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.035220 sharetop-1.3.4/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.3.4/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     2374 2023-05-02 15:19:23.000000 sharetop-1.3.4/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.3.4/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12266 2023-05-04 04:12:59.000000 sharetop-1.3.4/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.3.4/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.081611 sharetop-1.3.4/sharetop/core/country/
+-rw-rw-rw-   0        0        0      101 2023-05-16 01:30:15.000000 sharetop-1.3.4/sharetop/core/country/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-1.3.4/sharetop/core/country/config.py
+-rw-rw-rw-   0        0        0      494 2023-05-11 04:40:55.000000 sharetop-1.3.4/sharetop/core/country/country_base_info.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.441884 sharetop-1.3.4/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.3.4/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.3.4/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.3.4/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.3.4/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.3.4/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.3.4/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.3.4/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.3.4/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.3.4/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.3.4/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.3.4/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.501215 sharetop-1.3.4/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.3.4/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.3.4/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.527049 sharetop-1.3.4/sharetop/core/oil/
+-rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-1.3.4/sharetop/core/oil/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-1.3.4/sharetop/core/oil/config.py
+-rw-rw-rw-   0        0        0     2970 2023-05-16 01:17:51.000000 sharetop-1.3.4/sharetop/core/oil/oil_detail.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.535647 sharetop-1.3.4/sharetop/core/pig/
+-rw-rw-rw-   0        0        0       76 2023-05-16 01:17:51.000000 sharetop-1.3.4/sharetop/core/pig/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-1.3.4/sharetop/core/pig/config.py
+-rw-rw-rw-   0        0        0     1127 2023-05-16 00:59:27.000000 sharetop-1.3.4/sharetop/core/pig/pig_detail.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.711955 sharetop-1.3.4/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      569 2023-05-02 15:39:30.000000 sharetop-1.3.4/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.3.4/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.3.4/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14368 2023-05-04 12:15:59.000000 sharetop-1.3.4/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.3.4/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.3.4/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.3.4/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     6349 2023-05-04 04:01:07.000000 sharetop-1.3.4/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.798698 sharetop-1.3.4/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.3.4/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-05-11 04:25:42.000000 sharetop-1.3.4/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     2957 2023-05-08 14:46:45.000000 sharetop-1.3.4/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.837464 sharetop-1.3.4/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.3.4/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     3893 2023-05-11 04:40:55.000000 sharetop-1.3.4/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     1948 2023-05-02 15:34:17.000000 sharetop-1.3.4/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:17.957260 sharetop-1.3.4/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.3.4/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.3.4/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.3.4/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.3.4/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-1.3.4/sharetop/test/test4.py
+-rw-rw-rw-   0        0        0      509 2023-05-16 14:17:41.000000 sharetop-1.3.4/sharetop/test/test5.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:29:16.595367 sharetop-1.3.4/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    47157 2023-05-16 14:29:16.000000 sharetop-1.3.4/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2027 2023-05-16 14:29:16.000000 sharetop-1.3.4/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:29:16.000000 sharetop-1.3.4/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-16 14:29:16.000000 sharetop-1.3.4/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 14:29:16.000000 sharetop-1.3.4/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.2.4/LICENSE` & `sharetop-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/PKG-INFO` & `sharetop-1.3.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.2.4
+Version: 1.3.4
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
@@ -19,15 +19,15 @@
 License-File: LICENSE
 
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
 [![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
 
-[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油进出口数据等。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油相关数据等。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -208,14 +208,18 @@
 {'300033':   股票名称    股票代码     最新价    最高价    最低价  ...  市盈率(TTM)    市净率     涨跌值  涨跌幅(%)  振幅(%)
 0  同花顺  300033  174.92  198.0  172.3  ...     55.27  15.63 -0.2009   -10.3  13.18
 
 [1 rows x 23 columns], '516110':     股票名称    股票代码    最新价    最高价  ...   内盘(手)       涨跌值  涨跌幅(%)  振幅(%)
 0  汽车ETF  516110  0.945  0.953  ...  466383  0.000023   0.249  0.358
 
 [1 rows x 19 columns]}
+>>> stock_code = '1.000001'
+>>> sp.stock.get_real_time_data(stock_code)
+股票名称    股票代码      最新价      最高价      最低价  ...  市盈率(TTM)  市净率    涨跌值  涨跌幅(%)  振幅(%)
+0  上证指数  000001  3341.73  3348.78  3302.03  ...       0.0  0.0  18.46    0.56   1.41
 ```
 
 - 股票龙虎榜
 
 ```python
 >>> import sharetop as sp
 >>> # 获取最新一个公开的龙虎榜数据(后面还有获取指定日期区间的示例代码)
@@ -547,13 +551,156 @@
 1526  动力煤主力  ZCM  2021-08-19  776.8  777.6  798.0  764.6  97229  7.597474e+09  4.30  0.03   0.2  0.0
 1527  动力煤主力  ZCM  2021-08-20  778.0  793.0  795.0  775.2  70549  5.553617e+09  2.53  1.48  11.6  0.0
 1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
 [1529 rows x 13 columns]
 ```
 
+- 获取国家相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取国家基础数据
+>>> country_data = sp.country.get_country_base_info(10)
+        国家简称      国家全称                      英文简称  ...     首都(中文)           首都(英文)  所属组织
+0     中国   中华人民共和国                     China  ...         北京          Beijing  None
+1     美国    美利坚合众国             United States  ...  华盛顿哥伦比亚特区  Washington D.C.  None
+2    俄罗斯     俄罗斯联邦                    Russia  ...        莫斯科           Moscow  None
+3  沙特阿拉伯   沙特阿拉伯王国              Saudi Arabia  ...        利雅得           Riyadh   欧佩克
+4    加拿大       加拿大                    Canada  ...       None             None  None
+5    伊拉克    伊拉克共和国                      Iraq  ...        巴格达          Baghdad   欧佩克
+6     伊朗  伊朗伊斯兰共和国                      Iran  ...        德黑兰           Tehran   欧佩克
+7    阿联酋  阿拉伯联合酋长国  The United Arab Emirates  ...       阿布扎比        Abu Dhabi   欧佩克
+8     巴西   巴西联邦共和国                    Brazil  ...       None             None  None
+9    科威特      科威特国                    Kuwait  ...       科威特城       Kuwait Cit   欧佩克
+
+[10 rows x 11 columns]
+
+```
+
+- 获取石油相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取石油储量数据
+>>> sp.oil.get_oil_reserves('1', 10)
+        年份  储量(十亿桶)  总储量占比   储产比    产品名称 机构名称
+0  2000   181.50    NaN   NaN  探明储量石油  加拿大
+1  2010   174.85    NaN   NaN  探明储量石油  加拿大
+2  2020   168.10  0.097  89.4  探明储量石油  加拿大
+3  2000    24.63    NaN   NaN  探明储量石油  墨西哥
+4  2010    10.42    NaN   NaN  探明储量石油  墨西哥
+5  2020     6.10  0.004   8.7  探明储量石油  墨西哥
+6  2000    30.39    NaN   NaN  探明储量石油   美国
+7  2010    34.99    NaN   NaN  探明储量石油   美国
+8  2020    68.80  0.040  11.4  探明储量石油   美国
+9  2000     2.97    NaN   NaN  探明储量石油  阿根廷
+>>> # 获取石油生产数据
+>>> sp.oil.get_oil_products('1', 10)
+     年份  产量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010   3332.08  None  探明储量石油  加拿大
+1  2011   3514.82  None  探明储量石油  加拿大
+2  2012   3740.24  None  探明储量石油  加拿大
+3  2013   4000.41  None  探明储量石油  加拿大
+4  2014   4270.53  None  探明储量石油  加拿大
+5  2015   4388.14  None  探明储量石油  加拿大
+6  2016   4463.64  None  探明储量石油  加拿大
+7  2017   4813.03  None  探明储量石油  加拿大
+8  2018   5243.88  None  探明储量石油  加拿大
+9  2019   5372.42  None  探明储量石油  加拿大
+>>> # 获取石油消费数据
+>>> sp.oil.get_oil_consumption('1', 10)
+     年份  消费量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010    2386.08  None  探明储量石油  加拿大
+1  2011    2399.81  None  探明储量石油  加拿大
+2  2012    2426.03  None  探明储量石油  加拿大
+3  2013    2422.27  None  探明储量石油  加拿大
+4  2014    2420.13  None  探明储量石油  加拿大
+5  2015    2442.79  None  探明储量石油  加拿大
+6  2016    2453.38  None  探明储量石油  加拿大
+7  2017    2424.31  None  探明储量石油  加拿大
+8  2018    2500.60  None  探明储量石油  加拿大
+9  2019    2491.24  None  探明储量石油  加拿大
+>>> # 获取石油加工能力数据
+>>> sp.oil.get_oil_refinerycapacity('1', 10)
+     年份  产能(千桶/天) 总产能占比    产品名称 机构名称
+0  2010   1913.18  None  探明储量石油  加拿大
+1  2011   2004.54  None  探明储量石油  加拿大
+2  2012   2014.85  None  探明储量石油  加拿大
+3  2013   1929.44  None  探明储量石油  加拿大
+4  2014   1929.44  None  探明储量石油  加拿大
+5  2015   1930.79  None  探明储量石油  加拿大
+6  2016   1933.71  None  探明储量石油  加拿大
+7  2017   1969.56  None  探明储量石油  加拿大
+8  2018   1939.20  None  探明储量石油  加拿大
+9  2019   2054.15  None  探明储量石油  加拿大
+>>> # 获取石油加工量数据
+>>> sp.oil.get_oil_refinerythroughput('1', 10)
+年份  加工量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010     1769.0  None  探明储量石油  加拿大
+1  2011     1680.0  None  探明储量石油  加拿大
+2  2012     1752.0  None  探明储量石油  加拿大
+3  2013     1718.0  None  探明储量石油  加拿大
+4  2014     1615.0  None  探明储量石油  加拿大
+5  2015     1639.0  None  探明储量石油  加拿大
+6  2016     1594.0  None  探明储量石油  加拿大
+7  2017     1757.0  None  探明储量石油  加拿大
+8  2018     1652.0  None  探明储量石油  加拿大
+9  2019     1822.0  None  探明储量石油  加拿大
+>>> # 获取石油加工量数据
+>>> sp.oil.get_oil_crudeoilpricehistory(20)
+年份  价格(当年真实价格)  价格(按2022年美国消费者物价指数平减) 产品名称
+0   1861        0.49                  14.06   原油
+1   1862        1.05                  27.11   原油
+2   1863        3.15                  65.94   原油
+3   1864        8.06                 132.83   原油
+4   1865        6.59                 110.97   原油
+5   1866        3.74                  65.84   原油
+6   1867        2.41                  44.45   原油
+7   1868        3.63                  70.29   原油
+8   1869        3.64                  70.49   原油
+9   1870        3.86                  78.68   原油
+10  1871        4.34                  93.38   原油
+11  1872        3.64                  78.32   原油
+12  1873        1.83                  39.37   原油
+13  1874        1.17                  26.65   原油
+14  1875        1.35                  31.69   原油
+15  1876        2.56                  61.97   原油
+16  1877        2.42                  58.58   原油
+17  1878        1.19                  31.78   原油
+18  1879        0.86                  23.79   原油
+19  1880        0.95                  25.37   原油
+```
+
+- 获取猪周期相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取国家基础数据
+>>> start_date = '2023-05-01'
+>>> end_date = '2023-05-16'
+>>> sp.pig.get_fcr(start_date, end_date)
+        发布时间  生猪(外三元)(元/公斤)   猪粮比
+0   2023-05-01          14.63  5.16
+1   2023-05-02          14.64  5.09
+2   2023-05-03          14.55  5.10
+3   2023-05-04          14.57  5.03
+4   2023-05-05          14.57  5.06
+5   2023-05-06          14.49  5.06
+6   2023-05-07          14.37  5.01
+7   2023-05-08          14.39  5.01
+8   2023-05-09          14.39  5.01
+9   2023-05-10          14.32  4.95
+10  2023-05-11          14.33  4.97
+11  2023-05-12          14.31  4.97
+12  2023-05-13          14.26  4.96
+13  2023-05-14          14.27  5.02
+14  2023-05-15          14.28  4.96
+15  2023-05-16          14.29  5.01
+
+```
 
 ## Contact
 - 对市场感兴趣的同学可以联系我，对互联网金融感兴趣的同学可以联系我，对市场行业相关数据感兴趣的同学可以联系我，对数据有需求的同学可以联系我。欢迎志同道合的同学联系我
 - 微信：share_top
 <img src="static/sharetop.jpg" width="350">
```

### Comparing `sharetop-1.2.4/README.md` & `sharetop-1.3.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
 [![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
 
-[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油进出口数据等。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油相关数据等。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -188,14 +188,18 @@
 {'300033':   股票名称    股票代码     最新价    最高价    最低价  ...  市盈率(TTM)    市净率     涨跌值  涨跌幅(%)  振幅(%)
 0  同花顺  300033  174.92  198.0  172.3  ...     55.27  15.63 -0.2009   -10.3  13.18
 
 [1 rows x 23 columns], '516110':     股票名称    股票代码    最新价    最高价  ...   内盘(手)       涨跌值  涨跌幅(%)  振幅(%)
 0  汽车ETF  516110  0.945  0.953  ...  466383  0.000023   0.249  0.358
 
 [1 rows x 19 columns]}
+>>> stock_code = '1.000001'
+>>> sp.stock.get_real_time_data(stock_code)
+股票名称    股票代码      最新价      最高价      最低价  ...  市盈率(TTM)  市净率    涨跌值  涨跌幅(%)  振幅(%)
+0  上证指数  000001  3341.73  3348.78  3302.03  ...       0.0  0.0  18.46    0.56   1.41
 ```
 
 - 股票龙虎榜
 
 ```python
 >>> import sharetop as sp
 >>> # 获取最新一个公开的龙虎榜数据(后面还有获取指定日期区间的示例代码)
@@ -527,13 +531,156 @@
 1526  动力煤主力  ZCM  2021-08-19  776.8  777.6  798.0  764.6  97229  7.597474e+09  4.30  0.03   0.2  0.0
 1527  动力煤主力  ZCM  2021-08-20  778.0  793.0  795.0  775.2  70549  5.553617e+09  2.53  1.48  11.6  0.0
 1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
 [1529 rows x 13 columns]
 ```
 
+- 获取国家相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取国家基础数据
+>>> country_data = sp.country.get_country_base_info(10)
+        国家简称      国家全称                      英文简称  ...     首都(中文)           首都(英文)  所属组织
+0     中国   中华人民共和国                     China  ...         北京          Beijing  None
+1     美国    美利坚合众国             United States  ...  华盛顿哥伦比亚特区  Washington D.C.  None
+2    俄罗斯     俄罗斯联邦                    Russia  ...        莫斯科           Moscow  None
+3  沙特阿拉伯   沙特阿拉伯王国              Saudi Arabia  ...        利雅得           Riyadh   欧佩克
+4    加拿大       加拿大                    Canada  ...       None             None  None
+5    伊拉克    伊拉克共和国                      Iraq  ...        巴格达          Baghdad   欧佩克
+6     伊朗  伊朗伊斯兰共和国                      Iran  ...        德黑兰           Tehran   欧佩克
+7    阿联酋  阿拉伯联合酋长国  The United Arab Emirates  ...       阿布扎比        Abu Dhabi   欧佩克
+8     巴西   巴西联邦共和国                    Brazil  ...       None             None  None
+9    科威特      科威特国                    Kuwait  ...       科威特城       Kuwait Cit   欧佩克
+
+[10 rows x 11 columns]
+
+```
+
+- 获取石油相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取石油储量数据
+>>> sp.oil.get_oil_reserves('1', 10)
+        年份  储量(十亿桶)  总储量占比   储产比    产品名称 机构名称
+0  2000   181.50    NaN   NaN  探明储量石油  加拿大
+1  2010   174.85    NaN   NaN  探明储量石油  加拿大
+2  2020   168.10  0.097  89.4  探明储量石油  加拿大
+3  2000    24.63    NaN   NaN  探明储量石油  墨西哥
+4  2010    10.42    NaN   NaN  探明储量石油  墨西哥
+5  2020     6.10  0.004   8.7  探明储量石油  墨西哥
+6  2000    30.39    NaN   NaN  探明储量石油   美国
+7  2010    34.99    NaN   NaN  探明储量石油   美国
+8  2020    68.80  0.040  11.4  探明储量石油   美国
+9  2000     2.97    NaN   NaN  探明储量石油  阿根廷
+>>> # 获取石油生产数据
+>>> sp.oil.get_oil_products('1', 10)
+     年份  产量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010   3332.08  None  探明储量石油  加拿大
+1  2011   3514.82  None  探明储量石油  加拿大
+2  2012   3740.24  None  探明储量石油  加拿大
+3  2013   4000.41  None  探明储量石油  加拿大
+4  2014   4270.53  None  探明储量石油  加拿大
+5  2015   4388.14  None  探明储量石油  加拿大
+6  2016   4463.64  None  探明储量石油  加拿大
+7  2017   4813.03  None  探明储量石油  加拿大
+8  2018   5243.88  None  探明储量石油  加拿大
+9  2019   5372.42  None  探明储量石油  加拿大
+>>> # 获取石油消费数据
+>>> sp.oil.get_oil_consumption('1', 10)
+     年份  消费量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010    2386.08  None  探明储量石油  加拿大
+1  2011    2399.81  None  探明储量石油  加拿大
+2  2012    2426.03  None  探明储量石油  加拿大
+3  2013    2422.27  None  探明储量石油  加拿大
+4  2014    2420.13  None  探明储量石油  加拿大
+5  2015    2442.79  None  探明储量石油  加拿大
+6  2016    2453.38  None  探明储量石油  加拿大
+7  2017    2424.31  None  探明储量石油  加拿大
+8  2018    2500.60  None  探明储量石油  加拿大
+9  2019    2491.24  None  探明储量石油  加拿大
+>>> # 获取石油加工能力数据
+>>> sp.oil.get_oil_refinerycapacity('1', 10)
+     年份  产能(千桶/天) 总产能占比    产品名称 机构名称
+0  2010   1913.18  None  探明储量石油  加拿大
+1  2011   2004.54  None  探明储量石油  加拿大
+2  2012   2014.85  None  探明储量石油  加拿大
+3  2013   1929.44  None  探明储量石油  加拿大
+4  2014   1929.44  None  探明储量石油  加拿大
+5  2015   1930.79  None  探明储量石油  加拿大
+6  2016   1933.71  None  探明储量石油  加拿大
+7  2017   1969.56  None  探明储量石油  加拿大
+8  2018   1939.20  None  探明储量石油  加拿大
+9  2019   2054.15  None  探明储量石油  加拿大
+>>> # 获取石油加工量数据
+>>> sp.oil.get_oil_refinerythroughput('1', 10)
+年份  加工量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010     1769.0  None  探明储量石油  加拿大
+1  2011     1680.0  None  探明储量石油  加拿大
+2  2012     1752.0  None  探明储量石油  加拿大
+3  2013     1718.0  None  探明储量石油  加拿大
+4  2014     1615.0  None  探明储量石油  加拿大
+5  2015     1639.0  None  探明储量石油  加拿大
+6  2016     1594.0  None  探明储量石油  加拿大
+7  2017     1757.0  None  探明储量石油  加拿大
+8  2018     1652.0  None  探明储量石油  加拿大
+9  2019     1822.0  None  探明储量石油  加拿大
+>>> # 获取石油加工量数据
+>>> sp.oil.get_oil_crudeoilpricehistory(20)
+年份  价格(当年真实价格)  价格(按2022年美国消费者物价指数平减) 产品名称
+0   1861        0.49                  14.06   原油
+1   1862        1.05                  27.11   原油
+2   1863        3.15                  65.94   原油
+3   1864        8.06                 132.83   原油
+4   1865        6.59                 110.97   原油
+5   1866        3.74                  65.84   原油
+6   1867        2.41                  44.45   原油
+7   1868        3.63                  70.29   原油
+8   1869        3.64                  70.49   原油
+9   1870        3.86                  78.68   原油
+10  1871        4.34                  93.38   原油
+11  1872        3.64                  78.32   原油
+12  1873        1.83                  39.37   原油
+13  1874        1.17                  26.65   原油
+14  1875        1.35                  31.69   原油
+15  1876        2.56                  61.97   原油
+16  1877        2.42                  58.58   原油
+17  1878        1.19                  31.78   原油
+18  1879        0.86                  23.79   原油
+19  1880        0.95                  25.37   原油
+```
+
+- 获取猪周期相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取国家基础数据
+>>> start_date = '2023-05-01'
+>>> end_date = '2023-05-16'
+>>> sp.pig.get_fcr(start_date, end_date)
+        发布时间  生猪(外三元)(元/公斤)   猪粮比
+0   2023-05-01          14.63  5.16
+1   2023-05-02          14.64  5.09
+2   2023-05-03          14.55  5.10
+3   2023-05-04          14.57  5.03
+4   2023-05-05          14.57  5.06
+5   2023-05-06          14.49  5.06
+6   2023-05-07          14.37  5.01
+7   2023-05-08          14.39  5.01
+8   2023-05-09          14.39  5.01
+9   2023-05-10          14.32  4.95
+10  2023-05-11          14.33  4.97
+11  2023-05-12          14.31  4.97
+12  2023-05-13          14.26  4.96
+13  2023-05-14          14.27  5.02
+14  2023-05-15          14.28  4.96
+15  2023-05-16          14.29  5.01
+
+```
 
 ## Contact
 - 对市场感兴趣的同学可以联系我，对互联网金融感兴趣的同学可以联系我，对市场行业相关数据感兴趣的同学可以联系我，对数据有需求的同学可以联系我。欢迎志同道合的同学联系我
 - 微信：share_top
 <img src="static/sharetop.jpg" width="350">
```

### Comparing `sharetop-1.2.4/setup.py` & `sharetop-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/application/base.py` & `sharetop-1.3.4/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/bond/__init__.py` & `sharetop-1.3.4/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/bond/config.py` & `sharetop-1.3.4/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/bond/get_bond_info.py` & `sharetop-1.3.4/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.3.4/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/cache.py` & `sharetop-1.3.4/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/common/common_base.py` & `sharetop-1.3.4/sharetop/core/common/common_base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/common/config.py` & `sharetop-1.3.4/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/common/getter.py` & `sharetop-1.3.4/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/config.py` & `sharetop-1.3.4/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/__init__.py` & `sharetop-1.3.4/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/fund_list.py` & `sharetop-1.3.4/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.3.4/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.3.4/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.3.4/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.3.4/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_fund_rank.py` & `sharetop-1.3.4/sharetop/core/fund/get_fund_rank.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.3.4/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.3.4/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.3.4/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/futures/get_futures_info.py` & `sharetop-1.3.4/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/stock/__init__.py` & `sharetop-1.3.4/sharetop/core/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/stock/bill_monitor.py` & `sharetop-1.3.4/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/stock/config.py` & `sharetop-1.3.4/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/stock/getter.py` & `sharetop-1.3.4/sharetop/core/stock/getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
 
 def get_real_time_data(
         stock_codes: Union[str, List[str]],
 ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
     :param stock_codes: 单个或者多个股票代码
+    也可以是1.000001 0为深证，1为上证， 116为港股
     :return: 获取单个或者多个股票的实时股价和相关信息
     """
     df = get_real_time(stock_codes)
     return df
 
 
 @process_dataframe_and_series(remove_columns_and_indexes=['市场编号'])
```

### Comparing `sharetop-1.2.4/sharetop/core/stock/quarterly_report.py` & `sharetop-1.3.4/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/stock/rank_list.py` & `sharetop-1.3.4/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/core/utils.py` & `sharetop-1.3.4/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/crawl/base.py` & `sharetop-1.3.4/sharetop/crawl/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,22 @@
         pass
 
     def get(self, url, data, user_agent=False, headers=None, *args, **kwargs):
         if user_agent:
             headers = {
                 'User-Agent': choice(user_agent_list)
             }
-        return requests.get(url, data, headers=headers)
+        try:
+            return requests.get(url, data, headers=headers)
+        except:
+            raise "request error and contact author"
 
     def post(self, url, data, user_agent=False, headers=None, *args, **kwargs):
         if user_agent:
             headers = {
                 'User-Agent': choice(user_agent_list)
             }
-        return requests.post(url, data, headers=headers)
+        try:
+            return requests.post(url, data, headers=headers)
+        except:
+            raise "request error and contact author"
```

### Comparing `sharetop-1.2.4/sharetop/crawl/settings.py` & `sharetop-1.3.4/sharetop/crawl/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,8 +34,10 @@
 
 fund_industry_url = ['htt', 'ps:/', '/fun', 'dmo', 'bap', 'i.ea', 'stm', 'one', 'y.co', 'm/Fu', 'ndM', 'NewA', 'pi/', 'Fun', 'dMNS', 'ecto', 'rAl', 'loc', 'ation']
 
 bond_base_list_url = ['htt', 'p:/', '/dat', 'acen', 'ter', '-we', 'b.ea', 'stmo', 'ney', '.co', 'm/a', 'pi/d', 'ata', '/v', '1/g', 'et']
 
 bond_base_info_url = ['htt', 'p:/', '/dat', 'acen', 'ter-w', 'eb.e', 'astm', 'one', 'y.co', 'm/ap', 'i/da', 'ta/v', '1/g', 'et']
 
-stock_base_info_url = ['htt', 'p:/', '/em', 'we', 'b.se', 'curi', 'ties.', 'eas', 'tmon', 'ey.c', 'om/P', 'C_HS', 'F10/C', 'ompa', 'nySu', 'rve', 'y/Pa', 'geAj', 'ax']
+stock_base_info_url = ['htt', 'p:/', '/em', 'we', 'b.se', 'curi', 'ties.', 'eas', 'tmon', 'ey.c', 'om/P', 'C_HS', 'F10/C', 'ompa', 'nySu', 'rve', 'y/Pa', 'geAj', 'ax']
+
+base_url_list = ["htt", "p:/", "/12", "1.37", ".16.", "150:", "686", "9/a", "pi"]
```

### Comparing `sharetop-1.2.4/sharetop/parser/base.py` & `sharetop-1.3.4/sharetop/parser/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,20 @@
         return json_r
 
     def parse_fund_json(self, text_response):
         results = re.findall('\[.*\]', text_response)
         json_data = eval(results[0])
         return json_data
 
+    def parse_god_cup_json(self, data_json, country_field_dict):
+        data = data_json['data']
+        df = pd.DataFrame(data)
+        df.rename(columns=country_field_dict, inplace=True)
+        return df
+
     def parse_stock_base_info(self, base_data):
         jbzl = base_data['jbzl'][0]
         fxxg = base_data['fxxg'][0]
         fxxg = {k.lower(): v for k, v in fxxg.items()}
         jbzl = {k.lower(): v for k, v in jbzl.items()}
         secucode = jbzl['secucode']
         code, mk_code = secucode.split(".")
```

### Comparing `sharetop-1.2.4/sharetop/parser/config.py` & `sharetop-1.3.4/sharetop/parser/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/test/test2-akshare.py` & `sharetop-1.3.4/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop/test/test3.py` & `sharetop-1.3.4/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.4/sharetop.egg-info/PKG-INFO` & `sharetop-1.3.4/sharetop.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.2.4
+Version: 1.3.4
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
@@ -19,15 +19,15 @@
 License-File: LICENSE
 
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
 [![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
 
-[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油进出口数据等。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油相关数据等。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -208,14 +208,18 @@
 {'300033':   股票名称    股票代码     最新价    最高价    最低价  ...  市盈率(TTM)    市净率     涨跌值  涨跌幅(%)  振幅(%)
 0  同花顺  300033  174.92  198.0  172.3  ...     55.27  15.63 -0.2009   -10.3  13.18
 
 [1 rows x 23 columns], '516110':     股票名称    股票代码    最新价    最高价  ...   内盘(手)       涨跌值  涨跌幅(%)  振幅(%)
 0  汽车ETF  516110  0.945  0.953  ...  466383  0.000023   0.249  0.358
 
 [1 rows x 19 columns]}
+>>> stock_code = '1.000001'
+>>> sp.stock.get_real_time_data(stock_code)
+股票名称    股票代码      最新价      最高价      最低价  ...  市盈率(TTM)  市净率    涨跌值  涨跌幅(%)  振幅(%)
+0  上证指数  000001  3341.73  3348.78  3302.03  ...       0.0  0.0  18.46    0.56   1.41
 ```
 
 - 股票龙虎榜
 
 ```python
 >>> import sharetop as sp
 >>> # 获取最新一个公开的龙虎榜数据(后面还有获取指定日期区间的示例代码)
@@ -547,13 +551,156 @@
 1526  动力煤主力  ZCM  2021-08-19  776.8  777.6  798.0  764.6  97229  7.597474e+09  4.30  0.03   0.2  0.0
 1527  动力煤主力  ZCM  2021-08-20  778.0  793.0  795.0  775.2  70549  5.553617e+09  2.53  1.48  11.6  0.0
 1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
 [1529 rows x 13 columns]
 ```
 
+- 获取国家相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取国家基础数据
+>>> country_data = sp.country.get_country_base_info(10)
+        国家简称      国家全称                      英文简称  ...     首都(中文)           首都(英文)  所属组织
+0     中国   中华人民共和国                     China  ...         北京          Beijing  None
+1     美国    美利坚合众国             United States  ...  华盛顿哥伦比亚特区  Washington D.C.  None
+2    俄罗斯     俄罗斯联邦                    Russia  ...        莫斯科           Moscow  None
+3  沙特阿拉伯   沙特阿拉伯王国              Saudi Arabia  ...        利雅得           Riyadh   欧佩克
+4    加拿大       加拿大                    Canada  ...       None             None  None
+5    伊拉克    伊拉克共和国                      Iraq  ...        巴格达          Baghdad   欧佩克
+6     伊朗  伊朗伊斯兰共和国                      Iran  ...        德黑兰           Tehran   欧佩克
+7    阿联酋  阿拉伯联合酋长国  The United Arab Emirates  ...       阿布扎比        Abu Dhabi   欧佩克
+8     巴西   巴西联邦共和国                    Brazil  ...       None             None  None
+9    科威特      科威特国                    Kuwait  ...       科威特城       Kuwait Cit   欧佩克
+
+[10 rows x 11 columns]
+
+```
+
+- 获取石油相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取石油储量数据
+>>> sp.oil.get_oil_reserves('1', 10)
+        年份  储量(十亿桶)  总储量占比   储产比    产品名称 机构名称
+0  2000   181.50    NaN   NaN  探明储量石油  加拿大
+1  2010   174.85    NaN   NaN  探明储量石油  加拿大
+2  2020   168.10  0.097  89.4  探明储量石油  加拿大
+3  2000    24.63    NaN   NaN  探明储量石油  墨西哥
+4  2010    10.42    NaN   NaN  探明储量石油  墨西哥
+5  2020     6.10  0.004   8.7  探明储量石油  墨西哥
+6  2000    30.39    NaN   NaN  探明储量石油   美国
+7  2010    34.99    NaN   NaN  探明储量石油   美国
+8  2020    68.80  0.040  11.4  探明储量石油   美国
+9  2000     2.97    NaN   NaN  探明储量石油  阿根廷
+>>> # 获取石油生产数据
+>>> sp.oil.get_oil_products('1', 10)
+     年份  产量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010   3332.08  None  探明储量石油  加拿大
+1  2011   3514.82  None  探明储量石油  加拿大
+2  2012   3740.24  None  探明储量石油  加拿大
+3  2013   4000.41  None  探明储量石油  加拿大
+4  2014   4270.53  None  探明储量石油  加拿大
+5  2015   4388.14  None  探明储量石油  加拿大
+6  2016   4463.64  None  探明储量石油  加拿大
+7  2017   4813.03  None  探明储量石油  加拿大
+8  2018   5243.88  None  探明储量石油  加拿大
+9  2019   5372.42  None  探明储量石油  加拿大
+>>> # 获取石油消费数据
+>>> sp.oil.get_oil_consumption('1', 10)
+     年份  消费量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010    2386.08  None  探明储量石油  加拿大
+1  2011    2399.81  None  探明储量石油  加拿大
+2  2012    2426.03  None  探明储量石油  加拿大
+3  2013    2422.27  None  探明储量石油  加拿大
+4  2014    2420.13  None  探明储量石油  加拿大
+5  2015    2442.79  None  探明储量石油  加拿大
+6  2016    2453.38  None  探明储量石油  加拿大
+7  2017    2424.31  None  探明储量石油  加拿大
+8  2018    2500.60  None  探明储量石油  加拿大
+9  2019    2491.24  None  探明储量石油  加拿大
+>>> # 获取石油加工能力数据
+>>> sp.oil.get_oil_refinerycapacity('1', 10)
+     年份  产能(千桶/天) 总产能占比    产品名称 机构名称
+0  2010   1913.18  None  探明储量石油  加拿大
+1  2011   2004.54  None  探明储量石油  加拿大
+2  2012   2014.85  None  探明储量石油  加拿大
+3  2013   1929.44  None  探明储量石油  加拿大
+4  2014   1929.44  None  探明储量石油  加拿大
+5  2015   1930.79  None  探明储量石油  加拿大
+6  2016   1933.71  None  探明储量石油  加拿大
+7  2017   1969.56  None  探明储量石油  加拿大
+8  2018   1939.20  None  探明储量石油  加拿大
+9  2019   2054.15  None  探明储量石油  加拿大
+>>> # 获取石油加工量数据
+>>> sp.oil.get_oil_refinerythroughput('1', 10)
+年份  加工量(千桶/天) 总产量占比    产品名称 机构名称
+0  2010     1769.0  None  探明储量石油  加拿大
+1  2011     1680.0  None  探明储量石油  加拿大
+2  2012     1752.0  None  探明储量石油  加拿大
+3  2013     1718.0  None  探明储量石油  加拿大
+4  2014     1615.0  None  探明储量石油  加拿大
+5  2015     1639.0  None  探明储量石油  加拿大
+6  2016     1594.0  None  探明储量石油  加拿大
+7  2017     1757.0  None  探明储量石油  加拿大
+8  2018     1652.0  None  探明储量石油  加拿大
+9  2019     1822.0  None  探明储量石油  加拿大
+>>> # 获取石油加工量数据
+>>> sp.oil.get_oil_crudeoilpricehistory(20)
+年份  价格(当年真实价格)  价格(按2022年美国消费者物价指数平减) 产品名称
+0   1861        0.49                  14.06   原油
+1   1862        1.05                  27.11   原油
+2   1863        3.15                  65.94   原油
+3   1864        8.06                 132.83   原油
+4   1865        6.59                 110.97   原油
+5   1866        3.74                  65.84   原油
+6   1867        2.41                  44.45   原油
+7   1868        3.63                  70.29   原油
+8   1869        3.64                  70.49   原油
+9   1870        3.86                  78.68   原油
+10  1871        4.34                  93.38   原油
+11  1872        3.64                  78.32   原油
+12  1873        1.83                  39.37   原油
+13  1874        1.17                  26.65   原油
+14  1875        1.35                  31.69   原油
+15  1876        2.56                  61.97   原油
+16  1877        2.42                  58.58   原油
+17  1878        1.19                  31.78   原油
+18  1879        0.86                  23.79   原油
+19  1880        0.95                  25.37   原油
+```
+
+- 获取猪周期相关数据
+
+```python
+>>> import sharetop as sp
+>>> # 获取国家基础数据
+>>> start_date = '2023-05-01'
+>>> end_date = '2023-05-16'
+>>> sp.pig.get_fcr(start_date, end_date)
+        发布时间  生猪(外三元)(元/公斤)   猪粮比
+0   2023-05-01          14.63  5.16
+1   2023-05-02          14.64  5.09
+2   2023-05-03          14.55  5.10
+3   2023-05-04          14.57  5.03
+4   2023-05-05          14.57  5.06
+5   2023-05-06          14.49  5.06
+6   2023-05-07          14.37  5.01
+7   2023-05-08          14.39  5.01
+8   2023-05-09          14.39  5.01
+9   2023-05-10          14.32  4.95
+10  2023-05-11          14.33  4.97
+11  2023-05-12          14.31  4.97
+12  2023-05-13          14.26  4.96
+13  2023-05-14          14.27  5.02
+14  2023-05-15          14.28  4.96
+15  2023-05-16          14.29  5.01
+
+```
 
 ## Contact
 - 对市场感兴趣的同学可以联系我，对互联网金融感兴趣的同学可以联系我，对市场行业相关数据感兴趣的同学可以联系我，对数据有需求的同学可以联系我。欢迎志同道合的同学联系我
 - 微信：share_top
 <img src="static/sharetop.jpg" width="350">
```

### Comparing `sharetop-1.2.4/sharetop.egg-info/SOURCES.txt` & `sharetop-1.3.4/sharetop.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,27 +19,36 @@
 sharetop/core/bond/config.py
 sharetop/core/bond/get_bond_info.py
 sharetop/core/bond/get_bond_public_info.py
 sharetop/core/common/__init__.py
 sharetop/core/common/common_base.py
 sharetop/core/common/config.py
 sharetop/core/common/getter.py
+sharetop/core/country/__init__.py
+sharetop/core/country/config.py
+sharetop/core/country/country_base_info.py
 sharetop/core/fund/__init__.py
 sharetop/core/fund/config.py
 sharetop/core/fund/fund_list.py
 sharetop/core/fund/get_fund_base_info.py
 sharetop/core/fund/get_fund_history_data.py
 sharetop/core/fund/get_fund_industry_info.py
 sharetop/core/fund/get_fund_invest_info.py
 sharetop/core/fund/get_fund_rank.py
 sharetop/core/fund/get_fund_real_time.py
 sharetop/core/fund/get_period_change_info.py
 sharetop/core/fund/get_types_percentage_info.py
 sharetop/core/futures/__init__.py
 sharetop/core/futures/get_futures_info.py
+sharetop/core/oil/__init__.py
+sharetop/core/oil/config.py
+sharetop/core/oil/oil_detail.py
+sharetop/core/pig/__init__.py
+sharetop/core/pig/config.py
+sharetop/core/pig/pig_detail.py
 sharetop/core/stock/__init__.py
 sharetop/core/stock/bill_monitor.py
 sharetop/core/stock/config.py
 sharetop/core/stock/getter.py
 sharetop/core/stock/quarterly_report.py
 sharetop/core/stock/rank_list.py
 sharetop/core/stock/stock_base_info.py
@@ -49,8 +58,9 @@
 sharetop/parser/__init__.py
 sharetop/parser/base.py
 sharetop/parser/config.py
 sharetop/test/__init__.py
 sharetop/test/test1.py
 sharetop/test/test2-akshare.py
 sharetop/test/test3.py
-sharetop/test/test4.py
+sharetop/test/test4.py
+sharetop/test/test5.py
```

