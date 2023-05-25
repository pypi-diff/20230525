# Comparing `tmp/adslproxy-enhance-3.5.0.tar.gz` & `tmp/adslproxy-enhance-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adslproxy-enhance-3.5.0.tar", last modified: Tue Aug  2 06:42:27 2022, max compression
+gzip compressed data, was "adslproxy-enhance-3.7.0.tar", last modified: Thu May 25 14:29:54 2023, max compression
```

## Comparing `adslproxy-enhance-3.5.0.tar` & `adslproxy-enhance-3.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-08-02 06:42:27.588005 adslproxy-enhance-3.5.0/
--rw-rw-rw-   0        0        0     1098 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/LICENSE
--rw-rw-rw-   0        0        0     3244 2022-08-02 06:42:27.588005 adslproxy-enhance-3.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2561 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-02 06:42:27.567128 adslproxy-enhance-3.5.0/adslproxy/
--rw-rw-rw-   0        0        0      174 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/__init__.py
--rw-rw-rw-   0        0        0       99 2022-08-02 06:41:40.000000 adslproxy-enhance-3.5.0/adslproxy/__version__.py
-drwxrwxrwx   0        0        0        0 2022-08-02 06:42:27.569100 adslproxy-enhance-3.5.0/adslproxy/checker/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/checker/__init__.py
--rw-rw-rw-   0        0        0     2218 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/checker/checker.py
--rw-rw-rw-   0        0        0     3988 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/cmd.py
--rw-rw-rw-   0        0        0     2318 2022-08-02 03:59:20.000000 adslproxy-enhance-3.5.0/adslproxy/db.py
-drwxrwxrwx   0        0        0        0 2022-08-02 06:42:27.571106 adslproxy-enhance-3.5.0/adslproxy/sender/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/sender/__init__.py
--rw-rw-rw-   0        0        0     4357 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/sender/sender.py
-drwxrwxrwx   0        0        0        0 2022-08-02 06:42:27.573100 adslproxy-enhance-3.5.0/adslproxy/server/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:41:27.000000 adslproxy-enhance-3.5.0/adslproxy/server/__init__.py
--rw-rw-rw-   0        0        0     2055 2022-08-02 03:54:13.000000 adslproxy-enhance-3.5.0/adslproxy/server/server.py
--rw-rw-rw-   0        0        0     1292 2022-08-02 03:42:35.000000 adslproxy-enhance-3.5.0/adslproxy/settings.py
-drwxrwxrwx   0        0        0        0 2022-08-02 06:42:27.587005 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/
--rw-rw-rw-   0        0        0     3244 2022-08-02 06:42:27.000000 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2022-08-02 06:42:27.000000 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-02 06:42:27.000000 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-08-02 06:42:27.000000 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2022-08-02 06:42:27.000000 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-02 06:42:27.000000 adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-02 06:42:27.588005 adslproxy-enhance-3.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3459 2022-08-02 06:20:25.000000 adslproxy-enhance-3.5.0/setup.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:29:54.090037 adslproxy-enhance-3.7.0/
+-rw-r--r--   0 andylee    (501) staff       (20)     1076 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/LICENSE
+-rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-25 14:29:54.089767 adslproxy-enhance-3.7.0/PKG-INFO
+-rw-r--r--   0 andylee    (501) staff       (20)     2501 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/README.md
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:29:54.085932 adslproxy-enhance-3.7.0/adslproxy/
+-rw-r--r--   0 andylee    (501) staff       (20)      165 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)       94 2023-05-25 14:24:32.000000 adslproxy-enhance-3.7.0/adslproxy/__version__.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:29:54.086416 adslproxy-enhance-3.7.0/adslproxy/checker/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/checker/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     2141 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/checker/checker.py
+-rw-r--r--   0 andylee    (501) staff       (20)     3871 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/cmd.py
+-rw-r--r--   0 andylee    (501) staff       (20)     2229 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/db.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:29:54.086929 adslproxy-enhance-3.7.0/adslproxy/sender/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/sender/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     4990 2023-05-25 14:20:09.000000 adslproxy-enhance-3.7.0/adslproxy/sender/sender.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:29:54.087397 adslproxy-enhance-3.7.0/adslproxy/server/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/server/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     1981 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/adslproxy/server/server.py
+-rw-r--r--   0 andylee    (501) staff       (20)     1303 2023-05-25 13:56:44.000000 adslproxy-enhance-3.7.0/adslproxy/settings.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-25 14:29:54.089373 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/
+-rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-25 14:29:54.000000 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/PKG-INFO
+-rw-r--r--   0 andylee    (501) staff       (20)      547 2023-05-25 14:29:54.000000 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/SOURCES.txt
+-rw-r--r--   0 andylee    (501) staff       (20)        1 2023-05-25 14:29:54.000000 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/dependency_links.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       48 2023-05-25 14:29:54.000000 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/entry_points.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       60 2023-05-25 14:29:54.000000 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/requires.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       10 2023-05-25 14:29:54.000000 adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/top_level.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       38 2023-05-25 14:29:54.090160 adslproxy-enhance-3.7.0/setup.cfg
+-rw-r--r--   0 andylee    (501) staff       (20)     3336 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.0/setup.py
```

### Comparing `adslproxy-enhance-3.5.0/LICENSE` & `adslproxy-enhance-3.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-The MIT License (MIT)
-
-Copyright (c) 2015 bexidcom
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+The MIT License (MIT)
+
+Copyright (c) 2015 bexidcom
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `adslproxy-enhance-3.5.0/PKG-INFO` & `adslproxy-enhance-3.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-Metadata-Version: 2.1
-Name: adslproxy-enhance
-Version: 3.5.0
-Summary: ADSL Proxy Pool Tool 
-Home-page: https://github.com/thefantasystudio/AdslProxy
-Author: Germey
-Author-email: cqc@cuiqingcai.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-## 拨号主机设置
-
-首先配置好代理，如使用 Squid，运行在 3128 端口，并设置好用户名和密码。
-
-配置好代理之后，即可使用本工具定时拨号并发送至 Redis。
-
-### 安装 ADSLProxy
-
-```
-pip3 install -U adslproxy
-```
-
-### 设置环境变量
-
-```
-# Redis 数据库地址、端口和密码
-export REDIS_HOST=
-export REDIS_PORT=
-export REDIS_PASSWORD=
-# 拨号云主机配置的代理端口
-export PROXY_PORT=
-# 拨号云主机的代理用户名，无认证则留空
-export PROXY_USERNAME=
-# 拨号云主机配置的代理密码，无认证则留空
-export PROXY_PASSWORD=
-```
-
-### 执行
-
-```
-adslproxy send
-```
-
-运行结果：
-
-运行结果：
-
-```
-2020-04-13 01:39:30.811 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:39:30.893 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-2020-04-13 01:39:37.034 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.9.239
-2020-04-13 01:39:42.221 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.9.239:3389
-2020-04-13 01:39:42.458 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
-2020-04-13 01:43:02.560 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:43:02.630 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-2020-04-13 01:43:08.770 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.31.230
-2020-04-13 01:43:13.955 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.31.230:3389
-2020-04-13 01:43:14.037 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
-2020-04-13 01:46:34.216 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:46:34.298 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-```
-
-此时有效代理就会发送到 Redis。
-
-
-
+Metadata-Version: 2.1
+Name: adslproxy-enhance
+Version: 3.7.0
+Summary: ADSL Proxy Pool Tool 
+Home-page: https://github.com/thefantasystudio/AdslProxy
+Author: Germey
+Author-email: cqc@cuiqingcai.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.5.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+## 拨号主机设置
+
+首先配置好代理，如使用 Squid，运行在 3128 端口，并设置好用户名和密码。
+
+配置好代理之后，即可使用本工具定时拨号并发送至 Redis。
+
+### 安装 ADSLProxy
+
+```
+pip3 install -U adslproxy
+```
+
+### 设置环境变量
+
+```
+# Redis 数据库地址、端口和密码
+export REDIS_HOST=
+export REDIS_PORT=
+export REDIS_PASSWORD=
+# 拨号云主机配置的代理端口
+export PROXY_PORT=
+# 拨号云主机的代理用户名，无认证则留空
+export PROXY_USERNAME=
+# 拨号云主机配置的代理密码，无认证则留空
+export PROXY_PASSWORD=
+```
+
+### 执行
+
+```
+adslproxy send
+```
+
+运行结果：
+
+运行结果：
+
+```
+2020-04-13 01:39:30.811 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:39:30.893 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+2020-04-13 01:39:37.034 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.9.239
+2020-04-13 01:39:42.221 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.9.239:3389
+2020-04-13 01:39:42.458 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
+2020-04-13 01:43:02.560 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:43:02.630 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+2020-04-13 01:43:08.770 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.31.230
+2020-04-13 01:43:13.955 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.31.230:3389
+2020-04-13 01:43:14.037 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
+2020-04-13 01:46:34.216 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:46:34.298 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+```
+
+此时有效代理就会发送到 Redis。
+
```

### Comparing `adslproxy-enhance-3.5.0/README.md` & `adslproxy-enhance-3.7.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-## 拨号主机设置
-
-首先配置好代理，如使用 Squid，运行在 3128 端口，并设置好用户名和密码。
-
-配置好代理之后，即可使用本工具定时拨号并发送至 Redis。
-
-### 安装 ADSLProxy
-
-```
-pip3 install -U adslproxy
-```
-
-### 设置环境变量
-
-```
-# Redis 数据库地址、端口和密码
-export REDIS_HOST=
-export REDIS_PORT=
-export REDIS_PASSWORD=
-# 拨号云主机配置的代理端口
-export PROXY_PORT=
-# 拨号云主机的代理用户名，无认证则留空
-export PROXY_USERNAME=
-# 拨号云主机配置的代理密码，无认证则留空
-export PROXY_PASSWORD=
-```
-
-### 执行
-
-```
-adslproxy send
-```
-
-运行结果：
-
-运行结果：
-
-```
-2020-04-13 01:39:30.811 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:39:30.893 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-2020-04-13 01:39:37.034 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.9.239
-2020-04-13 01:39:42.221 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.9.239:3389
-2020-04-13 01:39:42.458 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
-2020-04-13 01:43:02.560 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:43:02.630 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-2020-04-13 01:43:08.770 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.31.230
-2020-04-13 01:43:13.955 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.31.230:3389
-2020-04-13 01:43:14.037 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
-2020-04-13 01:46:34.216 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:46:34.298 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-```
-
-此时有效代理就会发送到 Redis。
-
+## 拨号主机设置
+
+首先配置好代理，如使用 Squid，运行在 3128 端口，并设置好用户名和密码。
+
+配置好代理之后，即可使用本工具定时拨号并发送至 Redis。
+
+### 安装 ADSLProxy
+
+```
+pip3 install -U adslproxy
+```
+
+### 设置环境变量
+
+```
+# Redis 数据库地址、端口和密码
+export REDIS_HOST=
+export REDIS_PORT=
+export REDIS_PASSWORD=
+# 拨号云主机配置的代理端口
+export PROXY_PORT=
+# 拨号云主机的代理用户名，无认证则留空
+export PROXY_USERNAME=
+# 拨号云主机配置的代理密码，无认证则留空
+export PROXY_PASSWORD=
+```
+
+### 执行
+
+```
+adslproxy send
+```
+
+运行结果：
+
+运行结果：
+
+```
+2020-04-13 01:39:30.811 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:39:30.893 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+2020-04-13 01:39:37.034 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.9.239
+2020-04-13 01:39:42.221 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.9.239:3389
+2020-04-13 01:39:42.458 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
+2020-04-13 01:43:02.560 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:43:02.630 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+2020-04-13 01:43:08.770 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.31.230
+2020-04-13 01:43:13.955 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.31.230:3389
+2020-04-13 01:43:14.037 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
+2020-04-13 01:46:34.216 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:46:34.298 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+```
+
+此时有效代理就会发送到 Redis。
+
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy/checker/checker.py` & `adslproxy-enhance-3.7.0/adslproxy/checker/checker.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import time
-from requests import ReadTimeout
-from adslproxy.db import RedisClient
-import requests
-from adslproxy import settings
-from collections import defaultdict
-from loguru import logger
-
-
-class Checker(object):
-    
-    def __init__(self):
-        self.db = RedisClient()
-        self.counts = defaultdict(int)
-    
-    def check(self, proxy):
-        """
-        测试代理，返回测试结果
-        :param proxy: 代理
-        :return: 测试结果
-        """
-        try:
-            response = requests.get(settings.TEST_URL, proxies={
-                'http': 'http://' + proxy,
-                'https': 'https://' + proxy
-            }, timeout=settings.TEST_TIMEOUT)
-            logger.debug(f'Using {proxy} to test {settings.TEST_URL}...')
-            if response.status_code == 200:
-                return True
-        except (ConnectionError, ReadTimeout):
-            return False
-    
-    def run(self):
-        """
-        测试一轮
-        :return:
-        """
-        proxies = self.db.all()
-        logger.info(f'Try to get all proxies {proxies}')
-        for name, proxy in proxies.items():
-            # 检测无效
-            if not self.check(proxy):
-                logger.info(f'Proxy {proxy} invalid')
-                self.counts[proxy] += 1
-            else:
-                logger.info(f'Proxy {proxy} valid')
-            count = self.counts.get(proxy) or 0
-            logger.debug(f'Count {count}, TEST_MAX_ERROR_COUNT {settings.TEST_MAX_ERROR_COUNT}')
-            if count >= settings.TEST_MAX_ERROR_COUNT:
-                self.db.remove(name)
-    
-    def loop(self):
-        """
-        循环测试
-        :return:
-        """
-        while True:
-            logger.info('Check for infinite')
-            self.run()
-            logger.info(f'Tested, sleeping for {settings.TEST_CYCLE}s...')
-            time.sleep(settings.TEST_CYCLE)
-
-
-def check(loop=True):
-    """
-    check proxies
-    :param loop:
-    :return:
-    """
-    if not loop:
-        settings.TEST_MAX_ERROR_COUNT = 1
-    checker = Checker()
-    checker.loop() if loop else checker.run()
-
-
-if __name__ == '__main__':
-    check()
+import time
+from requests import ReadTimeout
+from adslproxy.db import RedisClient
+import requests
+from adslproxy import settings
+from collections import defaultdict
+from loguru import logger
+
+
+class Checker(object):
+    
+    def __init__(self):
+        self.db = RedisClient()
+        self.counts = defaultdict(int)
+    
+    def check(self, proxy):
+        """
+        测试代理，返回测试结果
+        :param proxy: 代理
+        :return: 测试结果
+        """
+        try:
+            response = requests.get(settings.TEST_URL, proxies={
+                'http': 'http://' + proxy,
+                'https': 'https://' + proxy
+            }, timeout=settings.TEST_TIMEOUT)
+            logger.debug(f'Using {proxy} to test {settings.TEST_URL}...')
+            if response.status_code == 200:
+                return True
+        except (ConnectionError, ReadTimeout):
+            return False
+    
+    def run(self):
+        """
+        测试一轮
+        :return:
+        """
+        proxies = self.db.all()
+        logger.info(f'Try to get all proxies {proxies}')
+        for name, proxy in proxies.items():
+            # 检测无效
+            if not self.check(proxy):
+                logger.info(f'Proxy {proxy} invalid')
+                self.counts[proxy] += 1
+            else:
+                logger.info(f'Proxy {proxy} valid')
+            count = self.counts.get(proxy) or 0
+            logger.debug(f'Count {count}, TEST_MAX_ERROR_COUNT {settings.TEST_MAX_ERROR_COUNT}')
+            if count >= settings.TEST_MAX_ERROR_COUNT:
+                self.db.remove(name)
+    
+    def loop(self):
+        """
+        循环测试
+        :return:
+        """
+        while True:
+            logger.info('Check for infinite')
+            self.run()
+            logger.info(f'Tested, sleeping for {settings.TEST_CYCLE}s...')
+            time.sleep(settings.TEST_CYCLE)
+
+
+def check(loop=True):
+    """
+    check proxies
+    :param loop:
+    :return:
+    """
+    if not loop:
+        settings.TEST_MAX_ERROR_COUNT = 1
+    checker = Checker()
+    checker.loop() if loop else checker.run()
+
+
+if __name__ == '__main__':
+    check()
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy/cmd.py` & `adslproxy-enhance-3.7.0/adslproxy/cmd.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import argparse
-from adslproxy import version
-import sys
-from adslproxy.checker.checker import check
-from adslproxy.sender.sender import send
-from adslproxy.server.server import serve
-
-optional_title = 'optional arguments'
-
-
-def str2bool(v):
-    """
-    convert string to bool
-    :param v:
-    :return:
-    """
-    if isinstance(v, bool):
-        return v
-    if v.lower() in ('yes', 'true', 't', 'y', '1'):
-        return True
-    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
-        return False
-    return True
-
-
-class CapitalisedHelpFormatter(argparse.HelpFormatter):
-    def __init__(self, prog):
-        super(CapitalisedHelpFormatter, self).__init__(prog,
-                                                       indent_increment=2,
-                                                       max_help_position=30,
-                                                       width=200)
-        self._action_max_length = 20
-    
-    def add_usage(self, usage, actions, groups, prefix=None):
-        if prefix is None:
-            prefix = 'Usage: '
-        return super(CapitalisedHelpFormatter, self).add_usage(
-            usage, actions, groups, prefix)
-    
-    class _Section(object):
-        
-        def __init__(self, formatter, parent, heading=None):
-            self.formatter = formatter
-            self.parent = parent
-            self.heading = heading
-            self.items = []
-        
-        def format_help(self):
-            # format the indented section
-            if self.parent is not None:
-                self.formatter._indent()
-            join = self.formatter._join_parts
-            item_help = join([func(*args) for func, args in self.items])
-            if self.parent is not None:
-                self.formatter._dedent()
-            
-            # return nothing if the section was empty
-            if not item_help:  return ''
-            
-            # add the heading if the section was non-empty
-            if self.heading is not argparse.SUPPRESS and self.heading is not None:
-                current_indent = self.formatter._current_indent
-                if self.heading == optional_title:
-                    heading = '%*s\n%s:\n' % (current_indent, '', self.heading.title())
-                else:
-                    heading = '%*s%s:' % (current_indent, '', self.heading.title())
-            else:
-                heading = ''
-            
-            return join(['\n', heading, item_help])
-
-
-parser = argparse.ArgumentParser(description='ADSLProxy %s - Easily to achieve ADSL Proxy Pool' % version(),
-                                 formatter_class=CapitalisedHelpFormatter, add_help=False)
-
-parser.add_argument('-v', '--version', action='version', version=version(), help='Get version of ADSLProxy')
-parser.add_argument('-h', '--help', action='help', help='Show this help message and exit')
-
-subparsers = parser.add_subparsers(dest='command', title='Available commands', metavar='')
-
-# serve
-parser_serve = subparsers.add_parser('serve', help='Run Server')
-
-# check
-parser_check = subparsers.add_parser('check', help='Run Checker')
-parser_check.add_argument('-l', '--loop', default=True, type=str2bool, nargs='?', help='Run checker for infinite')
-
-# send
-parser_send = subparsers.add_parser('send', help='Run Sender')
-parser_send.add_argument('-l', '--loop', default=True, type=str2bool, nargs='?', help='Run sender for infinite')
-
-# show help info when no args
-if len(sys.argv[1:]) == 0:
-    parser.print_help()
-    parser.exit()
-
-
-def cmd():
-    """
-    run from cmd
-    :return:
-    """
-    args = parser.parse_args()
-    command = args.command
-    # run server
-    if command == 'serve':
-        serve()
-    # dial and send proxy to redis
-    elif command == 'send':
-        send(args.loop)
-    # check proxies in redis
-    elif command == 'check':
-        check(args.loop)
-
-
-if __name__ == '__main__':
-    cmd()
+import argparse
+from adslproxy import version
+import sys
+from adslproxy.checker.checker import check
+from adslproxy.sender.sender import send
+from adslproxy.server.server import serve
+
+optional_title = 'optional arguments'
+
+
+def str2bool(v):
+    """
+    convert string to bool
+    :param v:
+    :return:
+    """
+    if isinstance(v, bool):
+        return v
+    if v.lower() in ('yes', 'true', 't', 'y', '1'):
+        return True
+    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
+        return False
+    return True
+
+
+class CapitalisedHelpFormatter(argparse.HelpFormatter):
+    def __init__(self, prog):
+        super(CapitalisedHelpFormatter, self).__init__(prog,
+                                                       indent_increment=2,
+                                                       max_help_position=30,
+                                                       width=200)
+        self._action_max_length = 20
+    
+    def add_usage(self, usage, actions, groups, prefix=None):
+        if prefix is None:
+            prefix = 'Usage: '
+        return super(CapitalisedHelpFormatter, self).add_usage(
+            usage, actions, groups, prefix)
+    
+    class _Section(object):
+        
+        def __init__(self, formatter, parent, heading=None):
+            self.formatter = formatter
+            self.parent = parent
+            self.heading = heading
+            self.items = []
+        
+        def format_help(self):
+            # format the indented section
+            if self.parent is not None:
+                self.formatter._indent()
+            join = self.formatter._join_parts
+            item_help = join([func(*args) for func, args in self.items])
+            if self.parent is not None:
+                self.formatter._dedent()
+            
+            # return nothing if the section was empty
+            if not item_help:  return ''
+            
+            # add the heading if the section was non-empty
+            if self.heading is not argparse.SUPPRESS and self.heading is not None:
+                current_indent = self.formatter._current_indent
+                if self.heading == optional_title:
+                    heading = '%*s\n%s:\n' % (current_indent, '', self.heading.title())
+                else:
+                    heading = '%*s%s:' % (current_indent, '', self.heading.title())
+            else:
+                heading = ''
+            
+            return join(['\n', heading, item_help])
+
+
+parser = argparse.ArgumentParser(description='ADSLProxy %s - Easily to achieve ADSL Proxy Pool' % version(),
+                                 formatter_class=CapitalisedHelpFormatter, add_help=False)
+
+parser.add_argument('-v', '--version', action='version', version=version(), help='Get version of ADSLProxy')
+parser.add_argument('-h', '--help', action='help', help='Show this help message and exit')
+
+subparsers = parser.add_subparsers(dest='command', title='Available commands', metavar='')
+
+# serve
+parser_serve = subparsers.add_parser('serve', help='Run Server')
+
+# check
+parser_check = subparsers.add_parser('check', help='Run Checker')
+parser_check.add_argument('-l', '--loop', default=True, type=str2bool, nargs='?', help='Run checker for infinite')
+
+# send
+parser_send = subparsers.add_parser('send', help='Run Sender')
+parser_send.add_argument('-l', '--loop', default=True, type=str2bool, nargs='?', help='Run sender for infinite')
+
+# show help info when no args
+if len(sys.argv[1:]) == 0:
+    parser.print_help()
+    parser.exit()
+
+
+def cmd():
+    """
+    run from cmd
+    :return:
+    """
+    args = parser.parse_args()
+    command = args.command
+    # run server
+    if command == 'serve':
+        serve()
+    # dial and send proxy to redis
+    elif command == 'send':
+        send(args.loop)
+    # check proxies in redis
+    elif command == 'check':
+        check(args.loop)
+
+
+if __name__ == '__main__':
+    cmd()
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy/db.py` & `adslproxy-enhance-3.7.0/adslproxy/db.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# coding=utf-8
-import redis
-import random
-from adslproxy.settings import *
-
-
-class RedisClient(object):
-    def __init__(self, host=REDIS_HOST, port=REDIS_PORT, password=REDIS_PASSWORD, redis_key=REDIS_KEY):
-        """
-        初始化Redis连接
-        :param host: Redis 地址
-        :param port: Redis 端口
-        :param password: Redis 密码
-        :param redis_key: Redis 哈希表名
-        """
-        self.db = redis.StrictRedis(host=host, port=port, password=password, decode_responses=True)
-        self.redis_key = redis_key
-    
-    def set(self, name, proxy):
-        """
-        设置代理
-        :param name: 主机名称
-        :param proxy: 代理
-        :return: 设置结果
-        """
-        return self.db.hset(self.redis_key, name, proxy)
-    
-    def get(self, name):
-        """
-        获取代理
-        :param name: 主机名称
-        :return: 代理
-        """
-        return self.db.hget(self.redis_key, name)
-    
-    def count(self):
-        """
-        获取代理总数
-        :return: 代理总数
-        """
-        return self.db.hlen(self.redis_key)
-    
-    def remove(self, name):
-        """
-        删除代理
-        :param name: 主机名称
-        :return: 删除结果
-        """
-        return self.db.hdel(self.redis_key, name)
-    
-    def names(self):
-        """
-        获取主机名称列表
-        :return: 获取主机名称列表
-        """
-        return self.db.hkeys(self.redis_key)
-    
-    def proxies(self):
-        """
-        获取代理列表
-        :return: 代理列表
-        """
-        return self.db.hvals(self.redis_key)
-    
-    def random(self, location):
-        """
-        随机获取代理
-        :return:
-        """
-        if location is not None:
-            proxies = self.db.hgetall(self.redis_key)
-            proxies = [v for k, v in proxies.items() if location in k]
-        else:
-            proxies = self.proxies()
-        return random.choice(proxies)
-    
-    def all(self):
-        """
-        获取字典
-        :return:
-        """
-        return self.db.hgetall(self.redis_key)
-    
-    def close(self):
-        """
-        关闭 Redis 连接
-        :return:
-        """
-        del self.db
+# coding=utf-8
+import redis
+import random
+from adslproxy.settings import *
+
+
+class RedisClient(object):
+    def __init__(self, host=REDIS_HOST, port=REDIS_PORT, password=REDIS_PASSWORD, redis_key=REDIS_KEY):
+        """
+        初始化Redis连接
+        :param host: Redis 地址
+        :param port: Redis 端口
+        :param password: Redis 密码
+        :param redis_key: Redis 哈希表名
+        """
+        self.db = redis.StrictRedis(host=host, port=port, password=password, decode_responses=True)
+        self.redis_key = redis_key
+    
+    def set(self, name, proxy):
+        """
+        设置代理
+        :param name: 主机名称
+        :param proxy: 代理
+        :return: 设置结果
+        """
+        return self.db.hset(self.redis_key, name, proxy)
+    
+    def get(self, name):
+        """
+        获取代理
+        :param name: 主机名称
+        :return: 代理
+        """
+        return self.db.hget(self.redis_key, name)
+    
+    def count(self):
+        """
+        获取代理总数
+        :return: 代理总数
+        """
+        return self.db.hlen(self.redis_key)
+    
+    def remove(self, name):
+        """
+        删除代理
+        :param name: 主机名称
+        :return: 删除结果
+        """
+        return self.db.hdel(self.redis_key, name)
+    
+    def names(self):
+        """
+        获取主机名称列表
+        :return: 获取主机名称列表
+        """
+        return self.db.hkeys(self.redis_key)
+    
+    def proxies(self):
+        """
+        获取代理列表
+        :return: 代理列表
+        """
+        return self.db.hvals(self.redis_key)
+    
+    def random(self, location):
+        """
+        随机获取代理
+        :return:
+        """
+        if location is not None:
+            proxies = self.db.hgetall(self.redis_key)
+            proxies = [v for k, v in proxies.items() if location in k]
+        else:
+            proxies = self.proxies()
+        return random.choice(proxies)
+    
+    def all(self):
+        """
+        获取字典
+        :return:
+        """
+        return self.db.hgetall(self.redis_key)
+    
+    def close(self):
+        """
+        关闭 Redis 连接
+        :return:
+        """
+        del self.db
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy/sender/sender.py` & `adslproxy-enhance-3.7.0/adslproxy/sender/sender.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,167 @@
-# coding=utf-8
-import re
-import time
-import requests
-from requests.exceptions import ConnectionError, ReadTimeout
-from adslproxy.db import RedisClient
-from adslproxy.settings import *
-import platform
-from loguru import logger
-from retrying import retry, RetryError
-import redis
-
-if platform.python_version().startswith('2.'):
-    import commands as subprocess
-elif platform.python_version().startswith('3.'):
-    import subprocess
-else:
-    raise ValueError('python version must be 2 or 3')
-
-
-class Sender(object):
-    """
-    拨号并发送到 Redis
-    """
-    
-    def extract_ip(self):
-        """
-        获取本机IP
-        :param ifname: 网卡名称
-        :return:
-        """
-        (status, output) = subprocess.getstatusoutput('ifconfig')
-        if not status == 0: return
-        pattern = re.compile(DIAL_IFNAME + '.*?inet.*?(\d+\.\d+\.\d+\.\d+).*?netmask', re.S)
-        result = re.search(pattern, output)
-        if result:
-            # 返回拨号后的 IP 地址
-            return result.group(1)
-    
-    def test_proxy(self, proxy):
-        """
-        测试代理，返回测试结果
-        :param proxy: 代理
-        :return: 测试结果
-        """
-        try:
-            response = requests.get(TEST_URL, proxies={
-                'http': 'http://' + proxy,
-                'https': 'https://' + proxy
-            }, timeout=TEST_TIMEOUT)
-            if response.status_code == 200:
-                return True
-        except (ConnectionError, ReadTimeout):
-            return False
-    
-    @retry(retry_on_result=lambda x: x is not True, stop_max_attempt_number=10)
-    def remove_proxy(self):
-        """
-        移除代理
-        :return: None
-        """
-        logger.info(f'Removing {CLIENT_NAME}...')
-        try:
-            # 由于拨号就会中断连接，所以每次都要重新建立连接
-            if hasattr(self, 'redis') and self.redis:
-                self.redis.close()
-            self.redis = RedisClient()
-            self.redis.remove(CLIENT_NAME)
-            logger.info(f'Removed {CLIENT_NAME} successfully')
-            return True
-        except redis.ConnectionError:
-            logger.info(f'Remove {CLIENT_NAME} failed')
-    
-    def set_proxy(self, proxy):
-        """
-        设置代理
-        :param proxy: 代理
-        :return: None
-        """
-        self.redis = RedisClient()
-        if self.redis.set(CLIENT_NAME, proxy):
-            logger.info(f'Successfully set proxy {proxy}')
-    
-    def loop(self):
-        """
-        循环拨号
-        :return:
-        """
-        while True:
-            logger.info('Starting dial...')
-            self.run()
-            time.sleep(DIAL_CYCLE)
-    
-    def run(self):
-        """
-        拨号主进程
-        :return: None
-        """
-        logger.info('Dial started, remove proxy')
-        try:
-            self.remove_proxy()
-        except RetryError:
-            logger.error('Retried for max times, continue')
-        # 拨号
-        (status, output) = subprocess.getstatusoutput(DIAL_BASH)
-        if not status == 0:
-            logger.error('Dial failed')
-        # 获取拨号 IP
-        ip = self.extract_ip()
-        if ip:
-            logger.info(f'Get new IP {ip}')
-            if PROXY_USERNAME and PROXY_PASSWORD:
-                proxy = '{username}:{password}@{ip}:{port}'.format(username=PROXY_USERNAME,
-                                                                   password=PROXY_PASSWORD,
-                                                                   ip=ip, port=PROXY_PORT)
-            else:
-                proxy = '{ip}:{port}'.format(ip=ip, port=PROXY_PORT)
-            time.sleep(10)
-            if self.test_proxy(proxy):
-                logger.info(f'Valid proxy {proxy}')
-                # 将代理放入数据库
-                self.set_proxy(proxy)
-                time.sleep(DIAL_CYCLE)
-            else:
-                logger.error(f'Proxy invalid {proxy}')
-        else:
-            # 获取 IP 失败，重新拨号
-            logger.error('Get IP failed, re-dialing')
-            self.run()
-
-
-def send(loop=True):
-    sender = Sender()
-    sender.loop() if loop else sender.run()
-
-
-if __name__ == '__main__':
-    send()
+import re
+import time
+import requests
+from requests.exceptions import ConnectionError, ReadTimeout
+from adslproxy.settings import *
+import platform
+from loguru import logger
+from retrying import retry, RetryError
+import hashlib
+from urllib.parse import urlencode
+
+if platform.python_version().startswith('2.'):
+    import commands as subprocess
+elif platform.python_version().startswith('3.'):
+    import subprocess
+else:
+    raise ValueError('python version must be 2 or 3')
+
+
+def generate_url_signature(payload, key):
+    payload['timestamp'] = int(time.time())
+    qs = ''
+    for i in sorted(payload.items()):
+        qs += f'{i[0]}{i[1]}'
+    qs += key
+    print(qs)
+    payload['signature'] = hashlib.md5(qs.encode('utf-8')).hexdigest()
+    return urlencode(payload)
+
+
+class Sender(object):
+    """
+    拨号并发送到 Redis
+    """
+
+    def extract_ip(self):
+        """
+        获取本机IP
+        :param ifname: 网卡名称
+        :return:
+        """
+        (status, output) = subprocess.getstatusoutput('ifconfig')
+        if not status == 0: return
+        pattern = re.compile(DIAL_IFNAME + '.*?inet.*?(\d+\.\d+\.\d+\.\d+).*?netmask', re.S)
+        result = re.search(pattern, output)
+        if result:
+            # 返回拨号后的 IP 地址
+            return result.group(1)
+
+    def test_proxy(self, proxy):
+        """
+        测试代理，返回测试结果
+        :param proxy: 代理
+        :return: 测试结果
+        """
+        try:
+            response = requests.get(TEST_URL, proxies={
+                'http': 'http://' + proxy,
+                'https': 'http://' + proxy
+            }, timeout=TEST_TIMEOUT)
+            if response.status_code == 200:
+                return True
+        except (ConnectionError, ReadTimeout):
+            return False
+
+    @retry(retry_on_result=lambda x: x is not True, stop_max_attempt_number=10)
+    def remove_proxy(self):
+        """
+        移除代理
+        :return: None
+        """
+        logger.info(f'Removing {CLIENT_NAME}...')
+        try:
+            payload = {
+                'client_name': CLIENT_NAME
+            }
+
+            qs = generate_url_signature(payload)
+
+            url = f"{API_URL}/remove?{qs}"
+            res = requests.get(url)
+            if res.ok:
+                logger.info(f'Result is {res.text} Removed {CLIENT_NAME} successfully')
+                logger.info(f'Removed {CLIENT_NAME} successfully')
+                return True
+            else:
+                logger.info(f'Result is {res.text} Removed {CLIENT_NAME} failed')
+                return False
+        except Exception as e:
+            logger.info(f'Remove {CLIENT_NAME} failed')
+
+    def set_proxy(self, proxy):
+        """
+        设置代理
+        :param proxy: 代理
+        :return: None
+        """
+        payload = {
+            'client_name': CLIENT_NAME,
+            'client_ip': proxy
+        }
+
+        qs = generate_url_signature(payload)
+        url = f"{API_URL}/update?{qs}"
+        res = requests.get(url)
+        if res.ok:
+            logger.info(f'Result is {res.text} Set {CLIENT_NAME} successfully')
+            return True
+        else:
+            logger.info(f'Result is {res.text} Removed {CLIENT_NAME} failed')
+            return False
+
+    def loop(self):
+        """
+        循环拨号
+        :return:
+        """
+        while True:
+            logger.info('Starting dial...')
+            self.run()
+            time.sleep(DIAL_CYCLE)
+
+    def run(self):
+        """
+        拨号主进程
+        :return: None
+        """
+        logger.info('Dial started, remove proxy')
+        try:
+            self.remove_proxy()
+        except RetryError:
+            logger.error('Retried for max times, continue')
+        # 拨号
+        (status, output) = subprocess.getstatusoutput(DIAL_BASH)
+        if not status == 0:
+            logger.error('Dial failed')
+        # 获取拨号 IP
+        ip = self.extract_ip()
+        if ip:
+            logger.info(f'Get new IP {ip}')
+            if PROXY_USERNAME and PROXY_PASSWORD:
+                proxy = '{username}:{password}@{ip}:{port}'.format(username=PROXY_USERNAME,
+                                                                   password=PROXY_PASSWORD,
+                                                                   ip=ip, port=PROXY_PORT)
+            else:
+                proxy = '{ip}:{port}'.format(ip=ip, port=PROXY_PORT)
+            time.sleep(10)
+            if self.test_proxy(proxy):
+                logger.info(f'Valid proxy {proxy}')
+                # 将代理放入数据库
+                self.set_proxy(proxy)
+                time.sleep(DIAL_CYCLE)
+            else:
+                logger.error(f'Proxy invalid {proxy}')
+        else:
+            # 获取 IP 失败，重新拨号
+            logger.error('Get IP failed, re-dialing')
+            self.run()
+
+
+def send(loop=True):
+    sender = Sender()
+    sender.loop() if loop else sender.run()
+
+
+if __name__ == '__main__':
+    send()
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy/settings.py` & `adslproxy-enhance-3.7.0/adslproxy/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-# coding=utf-8
-from environs import Env
-
-env = Env()
-
-# 拨号间隔，单位秒
-DIAL_CYCLE = env.int('DIAL_CYCLE', 100)
-# 拨号出错重试间隔
-DIAL_ERROR_CYCLE = env.int('DIAL_ERROR_CYCLE', 5)
-# 拨号命令
-DIAL_BASH = env.str('DIAL_BASH', 'adsl-stop;adsl-start')
-# 拨号网卡
-DIAL_IFNAME = env.str('DIAL_IFNAME', 'ppp0')
-
-# 客户端唯一标识
-CLIENT_NAME = env.str('CLIENT_NAME', 'adsl1')
-
-# Redis数据库IP
-REDIS_HOST = env.str('REDIS_HOST', '124.220.177.240')
-# Redis数据库密码, 如无则填None
-REDIS_PASSWORD = env.str('REDIS_PASSWORD', 'eYVX7mxKPCDmwMtyKVge8oLd2t81')
-# Redis数据库端口
-REDIS_PORT = env.int('REDIS_PORT', 33479)
-# 代理池键名
-REDIS_KEY = env.str('REDIS_KEY', 'adsl')
-
-# 测试URL
-TEST_URL = env.str('TEST_URL', 'http://www.baidu.com')
-# 测试最大失败次数
-TEST_MAX_ERROR_COUNT = env.int('TEST_MAX_ERROR_COUNT', 10)
-# 测试超时时间
-TEST_TIMEOUT = env.int('TEST_TIMEOUT', 20)
-# 测试周期
-TEST_CYCLE = env.int('TEST_CYCLE', 100)
-
-# 服务器端口
-SERVER_PORT = env.int('SERVER_PORT', 8425)
-SERVER_HOST = env.str('SERVER_HOST', '0.0.0.0')
-
-# 代理端口
-PROXY_PORT = env.int('PROXY_PORT', 3128)
-PROXY_USERNAME = env.str('PROXY_USERNAME', '')
-PROXY_PASSWORD = env.str('PROXY_PASSWORD', '')
+# coding=utf-8
+from environs import Env
+
+env = Env()
+
+# 拨号间隔，单位秒
+DIAL_CYCLE = env.int('DIAL_CYCLE', 100)
+# 拨号出错重试间隔
+DIAL_ERROR_CYCLE = env.int('DIAL_ERROR_CYCLE', 5)
+# 拨号命令
+DIAL_BASH = env.str('DIAL_BASH', 'adsl-stop;adsl-start')
+# 拨号网卡
+DIAL_IFNAME = env.str('DIAL_IFNAME', 'ppp0')
+
+# 客户端唯一标识
+CLIENT_NAME = env.str('CLIENT_NAME', 'adsl1')
+
+# Redis数据库IP
+REDIS_HOST = env.str('REDIS_HOST', '124.220.222.112')
+# Redis数据库密码, 如无则填None
+REDIS_PASSWORD = env.str('REDIS_PASSWORD', '1111')
+# Redis数据库端口
+REDIS_PORT = env.int('REDIS_PORT', 33479)
+# 代理池键名
+REDIS_KEY = env.str('REDIS_KEY', 'adsl')
+
+# 测试URL
+TEST_URL = env.str('TEST_URL', 'http://www.baidu.com')
+# 测试最大失败次数
+TEST_MAX_ERROR_COUNT = env.int('TEST_MAX_ERROR_COUNT', 10)
+# 测试超时时间
+TEST_TIMEOUT = env.int('TEST_TIMEOUT', 20)
+# 测试周期
+TEST_CYCLE = env.int('TEST_CYCLE', 100)
+
+# 服务器端口
+SERVER_PORT = env.int('SERVER_PORT', 8425)
+SERVER_HOST = env.str('SERVER_HOST', '0.0.0.0')
+
+# 代理端口
+PROXY_PORT = env.int('PROXY_PORT', 3128)
+PROXY_USERNAME = env.str('PROXY_USERNAME', '')
+PROXY_PASSWORD = env.str('PROXY_PASSWORD', '')
+API_URL = env.str('API_URL', '')
+API_SIGNATURE = env.str('API_SIGNATURE', '')
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/PKG-INFO` & `adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-Metadata-Version: 2.1
-Name: adslproxy-enhance
-Version: 3.5.0
-Summary: ADSL Proxy Pool Tool 
-Home-page: https://github.com/thefantasystudio/AdslProxy
-Author: Germey
-Author-email: cqc@cuiqingcai.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-## 拨号主机设置
-
-首先配置好代理，如使用 Squid，运行在 3128 端口，并设置好用户名和密码。
-
-配置好代理之后，即可使用本工具定时拨号并发送至 Redis。
-
-### 安装 ADSLProxy
-
-```
-pip3 install -U adslproxy
-```
-
-### 设置环境变量
-
-```
-# Redis 数据库地址、端口和密码
-export REDIS_HOST=
-export REDIS_PORT=
-export REDIS_PASSWORD=
-# 拨号云主机配置的代理端口
-export PROXY_PORT=
-# 拨号云主机的代理用户名，无认证则留空
-export PROXY_USERNAME=
-# 拨号云主机配置的代理密码，无认证则留空
-export PROXY_PASSWORD=
-```
-
-### 执行
-
-```
-adslproxy send
-```
-
-运行结果：
-
-运行结果：
-
-```
-2020-04-13 01:39:30.811 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:39:30.893 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-2020-04-13 01:39:37.034 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.9.239
-2020-04-13 01:39:42.221 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.9.239:3389
-2020-04-13 01:39:42.458 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
-2020-04-13 01:43:02.560 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:43:02.630 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-2020-04-13 01:43:08.770 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.31.230
-2020-04-13 01:43:13.955 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.31.230:3389
-2020-04-13 01:43:14.037 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
-2020-04-13 01:46:34.216 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
-2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
-2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
-2020-04-13 01:46:34.298 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
-```
-
-此时有效代理就会发送到 Redis。
-
-
-
+Metadata-Version: 2.1
+Name: adslproxy-enhance
+Version: 3.7.0
+Summary: ADSL Proxy Pool Tool 
+Home-page: https://github.com/thefantasystudio/AdslProxy
+Author: Germey
+Author-email: cqc@cuiqingcai.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.5.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+## 拨号主机设置
+
+首先配置好代理，如使用 Squid，运行在 3128 端口，并设置好用户名和密码。
+
+配置好代理之后，即可使用本工具定时拨号并发送至 Redis。
+
+### 安装 ADSLProxy
+
+```
+pip3 install -U adslproxy
+```
+
+### 设置环境变量
+
+```
+# Redis 数据库地址、端口和密码
+export REDIS_HOST=
+export REDIS_PORT=
+export REDIS_PASSWORD=
+# 拨号云主机配置的代理端口
+export PROXY_PORT=
+# 拨号云主机的代理用户名，无认证则留空
+export PROXY_USERNAME=
+# 拨号云主机配置的代理密码，无认证则留空
+export PROXY_PASSWORD=
+```
+
+### 执行
+
+```
+adslproxy send
+```
+
+运行结果：
+
+运行结果：
+
+```
+2020-04-13 01:39:30.811 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:39:30.812 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:39:30.893 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+2020-04-13 01:39:37.034 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.9.239
+2020-04-13 01:39:42.221 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.9.239:3389
+2020-04-13 01:39:42.458 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
+2020-04-13 01:43:02.560 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:43:02.561 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:43:02.630 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+2020-04-13 01:43:08.770 | INFO     | adslproxy.sender.sender:run:108 - Get New IP 113.128.31.230
+2020-04-13 01:43:13.955 | INFO     | adslproxy.sender.sender:run:117 - Valid proxy 113.128.31.230:3389
+2020-04-13 01:43:14.037 | INFO     | adslproxy.sender.sender:set_proxy:82 - Successfully Set Proxy
+2020-04-13 01:46:34.216 | INFO     | adslproxy.sender.sender:loop:90 - Starting dial...
+2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:run:99 - Dial Started, Remove Proxy
+2020-04-13 01:46:34.217 | INFO     | adslproxy.sender.sender:remove_proxy:62 - Removing adsl1...
+2020-04-13 01:46:34.298 | INFO     | adslproxy.sender.sender:remove_proxy:69 - Removed adsl1 successfully
+```
+
+此时有效代理就会发送到 Redis。
+
```

### Comparing `adslproxy-enhance-3.5.0/adslproxy_enhance.egg-info/SOURCES.txt` & `adslproxy-enhance-3.7.0/adslproxy_enhance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.5.0/setup.py` & `adslproxy-enhance-3.7.0/setup.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-from os.path import join, isfile
-from os import walk
-import io
-import os
-import sys
-from shutil import rmtree
-from setuptools import find_packages, setup, Command
-
-
-def read_file(filename):
-    with open(filename) as fp:
-        return fp.read().strip()
-
-
-def read_requirements(filename):
-    return [line.strip() for line in read_file(filename).splitlines()
-            if not line.startswith('#')]
-
-
-NAME = 'adslproxy-enhance'
-FOLDER = 'adslproxy'
-DESCRIPTION = 'ADSL Proxy Pool Tool '
-URL = 'https://github.com/thefantasystudio/AdslProxy'
-EMAIL = 'cqc@cuiqingcai.com'
-AUTHOR = 'Germey'
-REQUIRES_PYTHON = '>=3.5.0'
-VERSION = None
-
-REQUIRED = read_requirements('requirements.txt')
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-about = {}
-if not VERSION:
-    with open(os.path.join(here, FOLDER, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-def package_files(directories):
-    paths = []
-    for item in directories:
-        if isfile(item):
-            paths.append(join('..', item))
-            continue
-        for (path, directories, filenames) in walk(item):
-            for filename in filenames:
-                paths.append(join('..', path, filename))
-    return paths
-
-
-class UploadCommand(Command):
-    description = 'Build and publish the package.'
-    user_options = []
-    
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-    
-    def initialize_options(self):
-        pass
-    
-    def finalize_options(self):
-        pass
-    
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-        
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-        
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-        
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-        
-        sys.exit()
-
-
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=('tests',)),
-    install_requires=REQUIRED,
-    include_package_data=True,
-    license='MIT',
-    entry_points={
-        'console_scripts': ['adslproxy = adslproxy.cmd:cmd']
-    },
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    }
-)
+from os.path import join, isfile
+from os import walk
+import io
+import os
+import sys
+from shutil import rmtree
+from setuptools import find_packages, setup, Command
+
+
+def read_file(filename):
+    with open(filename) as fp:
+        return fp.read().strip()
+
+
+def read_requirements(filename):
+    return [line.strip() for line in read_file(filename).splitlines()
+            if not line.startswith('#')]
+
+
+NAME = 'adslproxy-enhance'
+FOLDER = 'adslproxy'
+DESCRIPTION = 'ADSL Proxy Pool Tool '
+URL = 'https://github.com/thefantasystudio/AdslProxy'
+EMAIL = 'cqc@cuiqingcai.com'
+AUTHOR = 'Germey'
+REQUIRES_PYTHON = '>=3.5.0'
+VERSION = None
+
+REQUIRED = read_requirements('requirements.txt')
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+about = {}
+if not VERSION:
+    with open(os.path.join(here, FOLDER, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+def package_files(directories):
+    paths = []
+    for item in directories:
+        if isfile(item):
+            paths.append(join('..', item))
+            continue
+        for (path, directories, filenames) in walk(item):
+            for filename in filenames:
+                paths.append(join('..', path, filename))
+    return paths
+
+
+class UploadCommand(Command):
+    description = 'Build and publish the package.'
+    user_options = []
+    
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+    
+    def initialize_options(self):
+        pass
+    
+    def finalize_options(self):
+        pass
+    
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+        
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+        
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+        
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+        
+        sys.exit()
+
+
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=('tests',)),
+    install_requires=REQUIRED,
+    include_package_data=True,
+    license='MIT',
+    entry_points={
+        'console_scripts': ['adslproxy = adslproxy.cmd:cmd']
+    },
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    }
+)
```

