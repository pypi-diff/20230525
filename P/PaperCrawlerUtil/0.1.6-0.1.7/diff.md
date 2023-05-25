# Comparing `tmp/PaperCrawlerUtil-0.1.6.tar.gz` & `tmp/PaperCrawlerUtil-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaperCrawlerUtil-0.1.6.tar", last modified: Thu Oct 13 07:47:08 2022, max compression
+gzip compressed data, was "PaperCrawlerUtil-0.1.7.tar", last modified: Tue Oct 18 02:00:27 2022, max compression
```

## Comparing `PaperCrawlerUtil-0.1.6.tar` & `PaperCrawlerUtil-0.1.7.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.043646 PaperCrawlerUtil-0.1.6/
--rw-rw-rw-   0        0        0     1085 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      654 2022-07-16 04:37:31.000000 PaperCrawlerUtil-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    20369 2022-10-13 07:47:08.042648 PaperCrawlerUtil-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.662103 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/
--rw-rw-rw-   0        0        0      407 2022-10-13 07:46:40.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/__init__.py
--rw-rw-rw-   0        0        0     2041 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/application.py
--rw-rw-rw-   0        0        0    35754 2022-10-13 07:18:04.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/common_util.py
--rw-rw-rw-   0        0        0     7631 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/constant.py
--rw-rw-rw-   0        0        0    24341 2022-10-13 07:18:04.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/crawler_util.py
--rw-rw-rw-   0        0        0      430 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/document_util.py
--rw-rw-rw-   0        0        0      678 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/global_val.py
--rw-rw-rw-   0        0        0     9904 2022-10-13 07:31:49.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/office_util.py
--rw-rw-rw-   0        0        0    41291 2022-10-13 07:18:04.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/pdf_util.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.732430 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/
--rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.735461 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/
--rw-rw-rw-   0        0        0      550 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.739410 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__pycache__/
--rw-rw-rw-   0        0        0      593 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2073 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__pycache__/base.cpython-39.pyc
--rw-rw-rw-   0        0        0     1875 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/base.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.741405 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/private/
--rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/private/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.743402 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/private/__pycache__/
--rw-rw-rw-   0        0        0      185 2022-07-17 09:31:19.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/private/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.952956 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/
--rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.986991 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/
--rw-rw-rw-   0        0        0      184 2022-07-17 09:31:19.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1334 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/daili66.cpython-39.pyc
--rw-rw-rw-   0        0        0     1102 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/data5u.cpython-39.pyc
--rw-rw-rw-   0        0        0     1066 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/fatezero.cpython-39.pyc
--rw-rw-rw-   0        0        0     1307 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/goubanjia.cpython-39.pyc
--rw-rw-rw-   0        0        0     1233 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ihuan.cpython-39.pyc
--rw-rw-rw-   0        0        0     1349 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip3366.cpython-39.pyc
--rw-rw-rw-   0        0        0     1178 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip89.cpython-39.pyc
--rw-rw-rw-   0        0        0     1275 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/iphai.cpython-39.pyc
--rw-rw-rw-   0        0        0     1365 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/jiangxianli.cpython-39.pyc
--rw-rw-rw-   0        0        0     1385 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/kuaidaili.cpython-39.pyc
--rw-rw-rw-   0        0        0     1221 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/seofangfa.cpython-39.pyc
--rw-rw-rw-   0        0        0     1352 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/taiyangdaili.cpython-39.pyc
--rw-rw-rw-   0        0        0     1863 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiaoshudaili.cpython-39.pyc
--rw-rw-rw-   0        0        0     1232 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xicidaili.cpython-39.pyc
--rw-rw-rw-   0        0        0     1132 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiladaili.cpython-39.pyc
--rw-rw-rw-   0        0        0     1142 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/yqie.cpython-39.pyc
--rw-rw-rw-   0        0        0     2435 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/zhandaye.cpython-39.pyc
--rw-rw-rw-   0        0        0      872 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/daili66.py
--rw-rw-rw-   0        0        0      780 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/data5u.py
--rw-rw-rw-   0        0        0      817 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/fatezero.py
--rw-rw-rw-   0        0        0     1348 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/goubanjia.py
--rw-rw-rw-   0        0        0      999 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/ihuan.py
--rw-rw-rw-   0        0        0      935 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/ip3366.py
--rw-rw-rw-   0        0        0      915 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/ip89.py
--rw-rw-rw-   0        0        0     1057 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/iphai.py
--rw-rw-rw-   0        0        0     1011 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/jiangxianli.py
--rw-rw-rw-   0        0        0      952 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/kuaidaili.py
--rw-rw-rw-   0        0        0      894 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/seofangfa.py
--rw-rw-rw-   0        0        0      866 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/taiyangdaili.py
--rw-rw-rw-   0        0        0     1506 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/xiaoshudaili.py
--rw-rw-rw-   0        0        0      971 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/xicidaili.py
--rw-rw-rw-   0        0        0      833 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/xiladaili.py
--rw-rw-rw-   0        0        0      809 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/yqie.py
--rw-rw-rw-   0        0        0     1810 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/zhandaye.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.989983 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/
--rw-rw-rw-   0        0        0       37 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.992975 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/__pycache__/
--rw-rw-rw-   0        0        0      227 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      562 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/__pycache__/empty.cpython-39.pyc
--rw-rw-rw-   0        0        0      183 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/empty.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.999956 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/
--rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.007934 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/
--rw-rw-rw-   0        0        0      179 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1879 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/getter.cpython-39.pyc
--rw-rw-rw-   0        0        0     2443 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/server.cpython-39.pyc
--rw-rw-rw-   0        0        0     3981 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/tester.cpython-39.pyc
--rw-rw-rw-   0        0        0     1659 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/getter.py
--rw-rw-rw-   0        0        0     2477 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/server.py
--rw-rw-rw-   0        0        0     4862 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/tester.py
--rw-rw-rw-   0        0        0     5604 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/scheduler.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.011759 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/
--rw-rw-rw-   0        0        0       24 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.014753 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/__pycache__/
--rw-rw-rw-   0        0        0      211 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      973 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/__pycache__/proxy.cpython-39.pyc
--rw-rw-rw-   0        0        0      607 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/proxy.py
--rw-rw-rw-   0        0        0     1738 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/setting.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.019709 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/
--rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.024695 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__pycache__/
--rw-rw-rw-   0        0        0      177 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5973 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__pycache__/proxy_dict.cpython-39.pyc
--rw-rw-rw-   0        0        0     5500 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__pycache__/redis.cpython-39.pyc
--rw-rw-rw-   0        0        0     6721 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/proxy_dict.py
--rw-rw-rw-   0        0        0     5644 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/redis.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.027730 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/
--rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:08.040654 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/__pycache__/
--rw-rw-rw-   0        0        0      174 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1390 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/__pycache__/proxy.cpython-39.pyc
--rw-rw-rw-   0        0        0     1381 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/proxy.py
--rw-rw-rw-   0        0        0    22400 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/translate_util.py
-drwxrwxrwx   0        0        0        0 2022-10-13 07:47:07.706452 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/
--rw-rw-rw-   0        0        0    20369 2022-10-13 07:47:06.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4997 2022-10-13 07:47:07.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-13 07:47:06.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      413 2022-10-13 07:47:07.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-10-13 07:47:07.000000 PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    19831 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.6/README.md
--rw-rw-rw-   0        0        0      350 2022-07-03 13:51:34.000000 PaperCrawlerUtil-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-10-13 07:47:08.043646 PaperCrawlerUtil-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2208 2022-10-13 07:45:47.000000 PaperCrawlerUtil-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.605777 PaperCrawlerUtil-0.1.7/
+-rw-rw-rw-   0        0        0     1085 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      654 2022-07-16 04:37:31.000000 PaperCrawlerUtil-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    20369 2022-10-18 02:00:27.604780 PaperCrawlerUtil-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:26.968877 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/
+-rw-rw-rw-   0        0        0      407 2022-10-18 02:00:10.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/__init__.py
+-rw-rw-rw-   0        0        0     2041 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/application.py
+-rw-rw-rw-   0        0        0    35924 2022-10-18 01:59:53.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/common_util.py
+-rw-rw-rw-   0        0        0     7631 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/constant.py
+-rw-rw-rw-   0        0        0    24341 2022-10-13 07:18:04.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/crawler_util.py
+-rw-rw-rw-   0        0        0      430 2022-10-13 07:54:08.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/document_util.py
+-rw-rw-rw-   0        0        0      678 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/global_val.py
+-rw-rw-rw-   0        0        0     9904 2022-10-13 07:31:49.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/office_util.py
+-rw-rw-rw-   0        0        0    41291 2022-10-13 07:18:04.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/pdf_util.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.006782 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/
+-rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.010772 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/
+-rw-rw-rw-   0        0        0      550 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.013763 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__pycache__/
+-rw-rw-rw-   0        0        0      593 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2073 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__pycache__/base.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1875 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/base.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.036054 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/private/
+-rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/private/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.038050 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/private/__pycache__/
+-rw-rw-rw-   0        0        0      185 2022-07-17 09:31:19.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/private/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.179175 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/
+-rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.329519 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/
+-rw-rw-rw-   0        0        0      184 2022-07-17 09:31:19.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1334 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/daili66.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1102 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/data5u.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1066 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/fatezero.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1307 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/goubanjia.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1233 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ihuan.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1349 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip3366.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1178 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip89.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1275 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/iphai.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1365 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/jiangxianli.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1385 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/kuaidaili.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1221 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/seofangfa.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1352 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/taiyangdaili.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1863 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiaoshudaili.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1232 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xicidaili.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1132 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiladaili.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1142 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/yqie.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2435 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/zhandaye.cpython-39.pyc
+-rw-rw-rw-   0        0        0      872 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/daili66.py
+-rw-rw-rw-   0        0        0      780 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/data5u.py
+-rw-rw-rw-   0        0        0      817 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/fatezero.py
+-rw-rw-rw-   0        0        0     1348 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/goubanjia.py
+-rw-rw-rw-   0        0        0      999 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/ihuan.py
+-rw-rw-rw-   0        0        0      935 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/ip3366.py
+-rw-rw-rw-   0        0        0      915 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/ip89.py
+-rw-rw-rw-   0        0        0     1057 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/iphai.py
+-rw-rw-rw-   0        0        0     1011 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/jiangxianli.py
+-rw-rw-rw-   0        0        0      952 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/kuaidaili.py
+-rw-rw-rw-   0        0        0      894 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/seofangfa.py
+-rw-rw-rw-   0        0        0      866 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/taiyangdaili.py
+-rw-rw-rw-   0        0        0     1506 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/xiaoshudaili.py
+-rw-rw-rw-   0        0        0      971 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/xicidaili.py
+-rw-rw-rw-   0        0        0      833 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/xiladaili.py
+-rw-rw-rw-   0        0        0      809 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/yqie.py
+-rw-rw-rw-   0        0        0     1810 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/zhandaye.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.346471 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/
+-rw-rw-rw-   0        0        0       37 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.350458 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/__pycache__/
+-rw-rw-rw-   0        0        0      227 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      562 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/__pycache__/empty.cpython-39.pyc
+-rw-rw-rw-   0        0        0      183 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/empty.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.395340 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/
+-rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.442218 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/
+-rw-rw-rw-   0        0        0      179 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1879 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/getter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2443 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/server.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3981 2022-09-10 02:25:00.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/tester.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1659 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/getter.py
+-rw-rw-rw-   0        0        0     2477 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/server.py
+-rw-rw-rw-   0        0        0     4862 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/tester.py
+-rw-rw-rw-   0        0        0     5604 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/scheduler.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.486099 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/
+-rw-rw-rw-   0        0        0       24 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.500059 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/__pycache__/
+-rw-rw-rw-   0        0        0      211 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      973 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/__pycache__/proxy.cpython-39.pyc
+-rw-rw-rw-   0        0        0      607 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/proxy.py
+-rw-rw-rw-   0        0        0     1738 2022-08-12 06:10:20.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/setting.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.521004 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/
+-rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.554912 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__pycache__/
+-rw-rw-rw-   0        0        0      177 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5973 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__pycache__/proxy_dict.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5500 2022-09-10 02:24:59.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__pycache__/redis.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6721 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/proxy_dict.py
+-rw-rw-rw-   0        0        0     5644 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/redis.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.558901 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/
+-rw-rw-rw-   0        0        0        0 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.584832 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/__pycache__/
+-rw-rw-rw-   0        0        0      174 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1390 2022-07-17 09:31:18.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/__pycache__/proxy.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1381 2022-07-03 13:10:17.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/proxy.py
+-rw-rw-rw-   0        0        0    22400 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/translate_util.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:00:27.000799 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/
+-rw-rw-rw-   0        0        0    20369 2022-10-18 02:00:25.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4997 2022-10-18 02:00:26.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-18 02:00:25.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      413 2022-10-18 02:00:26.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-10-18 02:00:26.000000 PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19831 2022-10-02 11:53:43.000000 PaperCrawlerUtil-0.1.7/README.md
+-rw-rw-rw-   0        0        0      350 2022-07-03 13:51:34.000000 PaperCrawlerUtil-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-10-18 02:00:27.605777 PaperCrawlerUtil-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2208 2022-10-13 07:45:47.000000 PaperCrawlerUtil-0.1.7/setup.py
```

### Comparing `PaperCrawlerUtil-0.1.6/LICENSE` & `PaperCrawlerUtil-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/MANIFEST.in` & `PaperCrawlerUtil-0.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PKG-INFO` & `PaperCrawlerUtil-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaperCrawlerUtil
-Version: 0.1.6
+Version: 0.1.7
 Summary: a collection of utils used to create crawler and document process
 Home-page: https://github.com/Liwu-di/PaperCrawlerUtil
 Author: liwudi@liwudi.fun
 Author-email: a154125960@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/application.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/application.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/common_util.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/common_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,19 @@
                 self.current = self.total
                 self.bar.set_postfix_str(self.final_prompt)
             else:
                 self.bar.update(self.batch)
                 self.current = self.current + self.batch
 
     def __del__(self):
-        self.bar.close()
+        try:
+            if self.bar is not None:
+                self.bar.close()
+        except Exception as e:
+            log("进度条关闭失败:{}".format(e), print_file=sys.stderr)
 
 
 def verify_rule(rule: dict, origin: float or str or Tag) -> bool:
     """
     verify the element string. if element satisfy all rules provided by rule arg,
     return true.
     :param rule:a dictionary that represent rules. the key is the match string and the value
```

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/constant.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/constant.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/crawler_util.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/crawler_util.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/global_val.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/global_val.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/office_util.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/office_util.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/pdf_util.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/pdf_util.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__init__.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__pycache__/__init__.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/__pycache__/base.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/base.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/base.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/daili66.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/daili66.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/data5u.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/data5u.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/fatezero.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/fatezero.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/goubanjia.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/goubanjia.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ihuan.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ihuan.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip3366.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip3366.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip89.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/ip89.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/iphai.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/iphai.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/jiangxianli.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/jiangxianli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/kuaidaili.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/kuaidaili.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/seofangfa.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/seofangfa.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/taiyangdaili.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/taiyangdaili.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiaoshudaili.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiaoshudaili.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xicidaili.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xicidaili.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiladaili.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/xiladaili.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/yqie.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/yqie.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/zhandaye.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/__pycache__/zhandaye.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/daili66.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/daili66.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/data5u.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/data5u.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/fatezero.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/fatezero.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/goubanjia.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/goubanjia.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/ihuan.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/ihuan.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/ip3366.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/ip3366.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/ip89.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/ip89.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/iphai.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/iphai.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/jiangxianli.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/jiangxianli.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/kuaidaili.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/kuaidaili.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/seofangfa.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/seofangfa.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/taiyangdaili.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/taiyangdaili.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/xiaoshudaili.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/xiaoshudaili.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/xicidaili.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/xicidaili.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/xiladaili.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/xiladaili.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/yqie.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/yqie.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/crawlers/public/zhandaye.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/crawlers/public/zhandaye.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/exceptions/__pycache__/empty.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/exceptions/__pycache__/empty.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/getter.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/getter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/server.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/server.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/__pycache__/tester.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/__pycache__/tester.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/getter.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/getter.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/server.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/server.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/processors/tester.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/processors/tester.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/scheduler.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/scheduler.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/__pycache__/proxy.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/schemas/proxy.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/schemas/proxy.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/setting.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/setting.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__pycache__/proxy_dict.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__pycache__/proxy_dict.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/__pycache__/redis.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/__pycache__/redis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/proxy_dict.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/proxy_dict.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/storages/redis.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/storages/redis.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/__pycache__/proxy.cpython-39.pyc` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/proxypool/utils/proxy.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/proxypool/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil/translate_util.py` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil/translate_util.py`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/PKG-INFO` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaperCrawlerUtil
-Version: 0.1.6
+Version: 0.1.7
 Summary: a collection of utils used to create crawler and document process
 Home-page: https://github.com/Liwu-di/PaperCrawlerUtil
 Author: liwudi@liwudi.fun
 Author-email: a154125960@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PaperCrawlerUtil-0.1.6/PaperCrawlerUtil.egg-info/SOURCES.txt` & `PaperCrawlerUtil-0.1.7/PaperCrawlerUtil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/README.md` & `PaperCrawlerUtil-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PaperCrawlerUtil-0.1.6/setup.py` & `PaperCrawlerUtil-0.1.7/setup.py`

 * *Files identical despite different names*

