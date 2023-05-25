# Comparing `tmp/lazynovel-0.1.0.tar.gz` & `tmp/lazynovel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazynovel-0.1.0.tar", last modified: Tue Feb 28 06:30:45 2023, max compression
+gzip compressed data, was "lazynovel-0.1.1.tar", last modified: Thu May 25 09:43:13 2023, max compression
```

## Comparing `lazynovel-0.1.0.tar` & `lazynovel-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-02-28 06:30:45.882135 lazynovel-0.1.0/
--rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.0/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-02-28 06:30:45.881993 lazynovel-0.1.0/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.0/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-02-28 06:30:45.880657 lazynovel-0.1.0/lazynovel/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      352 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5355 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/crawler_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10729 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/crawler_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1932 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/crawler_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_dianzhong.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    14527 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_yangguang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_yiqbook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.0/lazynovel/open_yuewen.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-02-28 06:30:45.881781 lazynovel-0.1.0/lazynovel.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-02-28 06:30:45.000000 lazynovel-0.1.0/lazynovel.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-02-28 06:30:45.000000 lazynovel-0.1.0/lazynovel.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-02-28 06:30:45.000000 lazynovel-0.1.0/lazynovel.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-02-28 06:30:45.000000 lazynovel-0.1.0/lazynovel.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-02-28 06:30:45.000000 lazynovel-0.1.0/lazynovel.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-02-28 06:30:45.882190 lazynovel-0.1.0/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-02-28 06:29:07.000000 lazynovel-0.1.0/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-25 09:43:13.516248 lazynovel-0.1.1/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.1/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-25 09:43:13.516140 lazynovel-0.1.1/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.1/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-25 09:43:13.515253 lazynovel-0.1.1/lazynovel/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      352 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.1/lazynovel/crawler_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10729 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/crawler_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1932 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/crawler_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_dianzhong.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    14527 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_yangguang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_yiqbook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.1/lazynovel/open_yuewen.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-25 09:43:13.515962 lazynovel-0.1.1/lazynovel.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-25 09:43:13.000000 lazynovel-0.1.1/lazynovel.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-05-25 09:43:13.000000 lazynovel-0.1.1/lazynovel.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-05-25 09:43:13.000000 lazynovel-0.1.1/lazynovel.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-05-25 09:43:13.000000 lazynovel-0.1.1/lazynovel.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-05-25 09:43:13.000000 lazynovel-0.1.1/lazynovel.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-05-25 09:43:13.516289 lazynovel-0.1.1/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-05-25 09:42:12.000000 lazynovel-0.1.1/setup.py
```

### Comparing `lazynovel-0.1.0/LICENSE` & `lazynovel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/PKG-INFO` & `lazynovel-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.0
+Version: 0.1.1
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.0/README.md` & `lazynovel-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/crawler_changdu.py` & `lazynovel-0.1.1/lazynovel/crawler_changdu.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,14 +121,65 @@
         method='GET',
         url=url,
         headers=headers,
         return_json=True
     )
 
 
+def wx_get_activity_list(
+        cookie: str,
+        app_id,
+        app_type,
+        distributor_id,
+        page: int = 1,
+        page_size: int = 10
+):
+    """
+    位置：（H5书城分销）运营配置-客服消息-新建消息-消息链接（插入活动链接）
+    功能：获取 活动链接列表
+    :param cookie: cookie
+    :param app_id: 应用id
+    :param app_type: 应用类型：3-公众号
+    :param distributor_id:
+    :param page: 页码
+    :param page_size: 每页数量
+    """
+    url = 'https://www.changdunovel.com/novelsale/distributor/get_activity_list/v1/'
+    params = {
+        'activity_type': 2,  # 看似固定
+        'activity_status': "1,2,3",  # 看似固定
+        'page_index': page - 1,
+        'page_size': page_size,
+    }
+    headers = {
+        "Accept": "application/json, text/plain, */*",
+        "Accept-Encoding": "gzip, deflate",
+        "Accept-Language": "zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2",
+        "Connection": "keep-alive",
+        "Cookie": cookie,
+        "Host": "www.changdunovel.com",
+        "Sec-Fetch-Dest": "empty",
+        "Sec-Fetch-Mode": "cors",
+        "Sec-Fetch-Site": "same-origin",
+        "TE": "trailers",
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:108.0) Gecko/20100101 Firefox/108.0",
+        "agw-js-conv": "str",
+        "appid": str(app_id),
+        "apptype": str(app_type),
+        "distributorid": str(distributor_id)
+    }
+    return lazyrequests.lazy_requests(
+        method='GET',
+        url=url,
+        headers=headers,
+        params=params,
+        return_json=True
+    )
+
+
 def customer_service_message_upload(
         cookie: str,
         app_id,
         app_type,
         distributor_id,
         file_dir
 ):
```

### Comparing `lazynovel-0.1.0/lazynovel/crawler_mbookcn.py` & `lazynovel-0.1.1/lazynovel/crawler_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/crawler_reading163.py` & `lazynovel-0.1.1/lazynovel/crawler_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_changdu.py` & `lazynovel-0.1.1/lazynovel/open_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_dianzhong.py` & `lazynovel-0.1.1/lazynovel/open_dianzhong.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_mbookcn.py` & `lazynovel-0.1.1/lazynovel/open_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_reading163.py` & `lazynovel-0.1.1/lazynovel/open_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_yangguang.py` & `lazynovel-0.1.1/lazynovel/open_yangguang.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_yiqbook.py` & `lazynovel-0.1.1/lazynovel/open_yiqbook.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel/open_yuewen.py` & `lazynovel-0.1.1/lazynovel/open_yuewen.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.0/lazynovel.egg-info/PKG-INFO` & `lazynovel-0.1.1/lazynovel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.0
+Version: 0.1.1
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.0/setup.py` & `lazynovel-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazynovel",
-    version="0.1.0",
+    version="0.1.1",
     description="小说平台接口封包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazynovel",
     packages=setuptools.find_packages(),
```

