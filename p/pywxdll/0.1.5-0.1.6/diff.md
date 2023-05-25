# Comparing `tmp/pywxdll-0.1.5.tar.gz` & `tmp/pywxdll-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywxdll-0.1.5.tar", last modified: Tue May 23 16:02:50 2023, max compression
+gzip compressed data, was "dist/pywxdll-0.1.6.tar", last modified: Wed May 24 15:58:59 2023, max compression
```

## Comparing `pywxdll-0.1.5.tar` & `pywxdll-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-23 16:02:50.000000 pywxdll-0.1.5/
--rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.5/LICENSE
--rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.5/MANIFEST.in
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-23 16:02:50.000000 pywxdll-0.1.5/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      577 2023-05-02 16:49:34.000000 pywxdll-0.1.5/README.md
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll/
--rw-r--r--   0 henryyang   (501) staff       (20)       74 2023-05-23 15:54:30.000000 pywxdll-0.1.5/pywxdll/__init__.py
--rw-r--r--   0 henryyang   (501) staff       (20)     6260 2023-05-23 15:54:30.000000 pywxdll-0.1.5/pywxdll/pywxdll.py
--rw-r--r--   0 henryyang   (501) staff       (20)     3976 2023-05-23 15:54:53.000000 pywxdll-0.1.5/pywxdll/pywxdll_json.py
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll.egg-info/
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.1.5/pywxdll.egg-info/.gitignore
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll.egg-info/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll.egg-info/SOURCES.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll.egg-info/dependency_links.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll.egg-info/requires.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-23 16:02:50.000000 pywxdll-0.1.5/pywxdll.egg-info/top_level.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-23 16:02:50.000000 pywxdll-0.1.5/setup.cfg
--rw-r--r--   0 henryyang   (501) staff       (20)     3743 2023-05-23 15:56:05.000000 pywxdll-0.1.5/setup.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-24 15:58:59.000000 pywxdll-0.1.6/
+-rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.6/LICENSE
+-rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.6/MANIFEST.in
+-rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-24 15:58:59.000000 pywxdll-0.1.6/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      577 2023-05-02 16:49:34.000000 pywxdll-0.1.6/README.md
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll/
+-rw-r--r--   0 henryyang   (501) staff       (20)       74 2023-05-24 15:49:56.000000 pywxdll-0.1.6/pywxdll/__init__.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     6276 2023-05-24 15:53:10.000000 pywxdll-0.1.6/pywxdll/pywxdll.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     3976 2023-05-23 15:54:53.000000 pywxdll-0.1.6/pywxdll/pywxdll_json.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll.egg-info/
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.1.6/pywxdll.egg-info/.gitignore
+-rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll.egg-info/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll.egg-info/SOURCES.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll.egg-info/dependency_links.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll.egg-info/requires.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-24 15:58:59.000000 pywxdll-0.1.6/pywxdll.egg-info/top_level.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-24 15:58:59.000000 pywxdll-0.1.6/setup.cfg
+-rw-r--r--   0 henryyang   (501) staff       (20)     3743 2023-05-24 15:49:39.000000 pywxdll-0.1.6/setup.py
```

### Comparing `pywxdll-0.1.5/LICENSE` & `pywxdll-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.5/PKG-INFO` & `pywxdll-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.5/README.md` & `pywxdll-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.5/pywxdll/pywxdll.py` & `pywxdll-0.1.6/pywxdll/pywxdll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import threading
-import time
 
 import requests
 import websocket
 
 from .pywxdll_json import *
 
 HEART_BEAT = 5005
@@ -167,15 +166,17 @@
     def get_chatroom_memberlist(self, roomid='null'):
         uri = '/api/get_charroom_member_list'
         return self.send_http(uri, json_get_chatroom_memberlist(roomid))
 
     ######## 信息处理 ########
 
     def recv_txt_handle(self, recieve):
+        '''
         out = {}
         out['content'] = recieve['content']
         out['id'] = recieve['id']
         out['time'] = recieve['time']
         out['type'] = recieve['type']
         out['wxid'] = recieve['wxid']
         out['nick'] = self.get_user_nick(recieve['wxid'])['content']['nick']
-        return out
+        '''
+        return recieve
```

### Comparing `pywxdll-0.1.5/pywxdll/pywxdll_json.py` & `pywxdll-0.1.6/pywxdll/pywxdll_json.py`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.5/pywxdll.egg-info/PKG-INFO` & `pywxdll-0.1.6/pywxdll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.5/setup.py` & `pywxdll-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywxdll'
 DESCRIPTION = 'A Python package for wechat dll hook'
 URL = 'https://github.com/HenryXiaoYang/pywxdll'
 EMAIL = 'henryyang666@hotmal.com'
 AUTHOR = 'HenryXiaoYang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['websocket-client', 'requests']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

