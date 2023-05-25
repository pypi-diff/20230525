# Comparing `tmp/jfExt-1.9.2.tar.gz` & `tmp/jfExt-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jfExt-1.9.2.tar", last modified: Wed Nov 30 16:28:54 2022, max compression
+gzip compressed data, was "jfExt-1.9.3.tar", last modified: Thu Dec  8 18:06:18 2022, max compression
```

## Comparing `jfExt-1.9.2.tar` & `jfExt-1.9.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-11-30 16:28:54.072007 jfExt-1.9.2/
--rw-r--r--   0 jifu       (501) staff       (20)      198 2022-11-30 16:28:54.071891 jfExt-1.9.2/PKG-INFO
--rw-r--r--   0 jifu       (501) staff       (20)       82 2021-09-18 12:52:53.000000 jfExt-1.9.2/README.md
-drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-11-30 16:28:54.068309 jfExt-1.9.2/jfExt/
-drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-11-30 16:28:54.070513 jfExt-1.9.2/jfExt/BasicType/
--rw-r--r--   0 jifu       (501) staff       (20)     1733 2022-10-20 15:21:21.000000 jfExt-1.9.2/jfExt/BasicType/BooleanExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     2195 2022-09-16 15:29:56.000000 jfExt-1.9.2/jfExt/BasicType/DictExt.py
--rw-r--r--   0 jifu       (501) staff       (20)      435 2022-05-13 20:33:49.000000 jfExt-1.9.2/jfExt/BasicType/FloatExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     1027 2022-05-13 20:46:59.000000 jfExt-1.9.2/jfExt/BasicType/JsonExt.py
--rw-r--r--   0 jifu       (501) staff       (20)      384 2022-05-13 21:39:23.000000 jfExt-1.9.2/jfExt/BasicType/ListExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     1913 2022-10-01 11:27:28.000000 jfExt-1.9.2/jfExt/BasicType/StringExt.py
--rw-r--r--   0 jifu       (501) staff       (20)        0 2022-05-13 20:28:15.000000 jfExt-1.9.2/jfExt/BasicType/__init__.py
--rw-r--r--   0 jifu       (501) staff       (20)     1409 2022-11-30 16:28:43.000000 jfExt-1.9.2/jfExt/CommonExt.py
--rw-r--r--   0 jifu       (501) staff       (20)      848 2022-10-06 16:07:51.000000 jfExt-1.9.2/jfExt/CurrencyExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     1224 2022-06-06 11:52:56.000000 jfExt-1.9.2/jfExt/EncryptExt.py
--rw-r--r--   0 jifu       (501) staff       (20)      901 2022-06-18 16:02:19.000000 jfExt-1.9.2/jfExt/GeoExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     1078 2022-11-29 01:44:02.000000 jfExt-1.9.2/jfExt/ImageExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     2788 2022-09-10 19:44:15.000000 jfExt-1.9.2/jfExt/IpExt.py
-drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-11-30 16:28:54.071086 jfExt-1.9.2/jfExt/Mgr/
--rw-r--r--   0 jifu       (501) staff       (20)        0 2022-05-13 20:56:02.000000 jfExt-1.9.2/jfExt/Mgr/__init__.py
--rw-r--r--   0 jifu       (501) staff       (20)     1652 2022-11-23 16:19:42.000000 jfExt-1.9.2/jfExt/Mgr/mailMgr.py
--rw-r--r--   0 jifu       (501) staff       (20)     4146 2022-08-02 17:19:22.000000 jfExt-1.9.2/jfExt/Mgr/redisMgr.py
--rw-r--r--   0 jifu       (501) staff       (20)     3892 2022-11-20 16:21:21.000000 jfExt-1.9.2/jfExt/Mgr/responseMgr.py
--rw-r--r--   0 jifu       (501) staff       (20)      835 2022-06-08 11:16:01.000000 jfExt-1.9.2/jfExt/OrderExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     1433 2022-11-30 16:27:32.000000 jfExt-1.9.2/jfExt/PrintExt.py
--rw-r--r--   0 jifu       (501) staff       (20)      999 2022-05-13 20:54:26.000000 jfExt-1.9.2/jfExt/RequestExt.py
--rw-r--r--   0 jifu       (501) staff       (20)      456 2022-05-13 21:39:23.000000 jfExt-1.9.2/jfExt/SingletonExt.py
-drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-11-30 16:28:54.071748 jfExt-1.9.2/jfExt/Time/
--rw-r--r--   0 jifu       (501) staff       (20)     7826 2022-05-13 21:39:23.000000 jfExt-1.9.2/jfExt/Time/DateExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     3641 2022-06-08 11:16:01.000000 jfExt-1.9.2/jfExt/Time/TimeExt.py
--rw-r--r--   0 jifu       (501) staff       (20)        0 2022-05-13 20:31:09.000000 jfExt-1.9.2/jfExt/Time/__init__.py
--rw-r--r--   0 jifu       (501) staff       (20)     2362 2022-05-13 20:54:29.000000 jfExt-1.9.2/jfExt/ValidExt.py
--rw-r--r--   0 jifu       (501) staff       (20)     1139 2022-10-20 15:21:21.000000 jfExt-1.9.2/jfExt/__init__.py
--rw-r--r--   0 jifu       (501) staff       (20)     1949 2022-09-21 20:38:29.000000 jfExt-1.9.2/jfExt/fileExt.py
-drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-11-30 16:28:54.069032 jfExt-1.9.2/jfExt.egg-info/
--rw-r--r--   0 jifu       (501) staff       (20)      198 2022-11-30 16:28:54.000000 jfExt-1.9.2/jfExt.egg-info/PKG-INFO
--rw-r--r--   0 jifu       (501) staff       (20)      779 2022-11-30 16:28:54.000000 jfExt-1.9.2/jfExt.egg-info/SOURCES.txt
--rw-r--r--   0 jifu       (501) staff       (20)        1 2022-11-30 16:28:54.000000 jfExt-1.9.2/jfExt.egg-info/dependency_links.txt
--rw-r--r--   0 jifu       (501) staff       (20)       94 2022-11-30 16:28:54.000000 jfExt-1.9.2/jfExt.egg-info/requires.txt
--rw-r--r--   0 jifu       (501) staff       (20)        6 2022-11-30 16:28:54.000000 jfExt-1.9.2/jfExt.egg-info/top_level.txt
--rw-r--r--   0 jifu       (501) staff       (20)        1 2022-05-13 21:15:03.000000 jfExt-1.9.2/jfExt.egg-info/zip-safe
--rw-r--r--   0 jifu       (501) staff       (20)       38 2022-11-30 16:28:54.072041 jfExt-1.9.2/setup.cfg
--rw-r--r--   0 jifu       (501) staff       (20)     1083 2022-11-30 16:28:48.000000 jfExt-1.9.2/setup.py
+drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-12-08 18:06:18.475503 jfExt-1.9.3/
+-rw-r--r--   0 jifu       (501) staff       (20)      198 2022-12-08 18:06:18.475376 jfExt-1.9.3/PKG-INFO
+-rw-r--r--   0 jifu       (501) staff       (20)       82 2021-09-18 12:52:53.000000 jfExt-1.9.3/README.md
+drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-12-08 18:06:18.471132 jfExt-1.9.3/jfExt/
+drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-12-08 18:06:18.473870 jfExt-1.9.3/jfExt/BasicType/
+-rw-r--r--   0 jifu       (501) staff       (20)     1733 2022-10-20 15:21:21.000000 jfExt-1.9.3/jfExt/BasicType/BooleanExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     2195 2022-09-16 15:29:56.000000 jfExt-1.9.3/jfExt/BasicType/DictExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)      435 2022-05-13 20:33:49.000000 jfExt-1.9.3/jfExt/BasicType/FloatExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1027 2022-05-13 20:46:59.000000 jfExt-1.9.3/jfExt/BasicType/JsonExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)      384 2022-05-13 21:39:23.000000 jfExt-1.9.3/jfExt/BasicType/ListExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1913 2022-10-01 11:27:28.000000 jfExt-1.9.3/jfExt/BasicType/StringExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)        0 2022-05-13 20:28:15.000000 jfExt-1.9.3/jfExt/BasicType/__init__.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1409 2022-11-30 16:28:43.000000 jfExt-1.9.3/jfExt/CommonExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)      848 2022-10-06 16:07:51.000000 jfExt-1.9.3/jfExt/CurrencyExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1224 2022-06-06 11:52:56.000000 jfExt-1.9.3/jfExt/EncryptExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)      901 2022-06-18 16:02:19.000000 jfExt-1.9.3/jfExt/GeoExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1078 2022-11-29 01:44:02.000000 jfExt-1.9.3/jfExt/ImageExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     2788 2022-09-10 19:44:15.000000 jfExt-1.9.3/jfExt/IpExt.py
+drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-12-08 18:06:18.474482 jfExt-1.9.3/jfExt/Mgr/
+-rw-r--r--   0 jifu       (501) staff       (20)        0 2022-05-13 20:56:02.000000 jfExt-1.9.3/jfExt/Mgr/__init__.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1652 2022-11-23 16:19:42.000000 jfExt-1.9.3/jfExt/Mgr/mailMgr.py
+-rw-r--r--   0 jifu       (501) staff       (20)     4145 2022-12-08 18:05:53.000000 jfExt-1.9.3/jfExt/Mgr/redisMgr.py
+-rw-r--r--   0 jifu       (501) staff       (20)     3892 2022-11-20 16:21:21.000000 jfExt-1.9.3/jfExt/Mgr/responseMgr.py
+-rw-r--r--   0 jifu       (501) staff       (20)      835 2022-06-08 11:16:01.000000 jfExt-1.9.3/jfExt/OrderExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1433 2022-11-30 16:27:32.000000 jfExt-1.9.3/jfExt/PrintExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)      999 2022-05-13 20:54:26.000000 jfExt-1.9.3/jfExt/RequestExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)      456 2022-05-13 21:39:23.000000 jfExt-1.9.3/jfExt/SingletonExt.py
+drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-12-08 18:06:18.475202 jfExt-1.9.3/jfExt/Time/
+-rw-r--r--   0 jifu       (501) staff       (20)     7828 2022-12-07 18:27:28.000000 jfExt-1.9.3/jfExt/Time/DateExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     3641 2022-06-08 11:16:01.000000 jfExt-1.9.3/jfExt/Time/TimeExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)        0 2022-05-13 20:31:09.000000 jfExt-1.9.3/jfExt/Time/__init__.py
+-rw-r--r--   0 jifu       (501) staff       (20)     2362 2022-05-13 20:54:29.000000 jfExt-1.9.3/jfExt/ValidExt.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1139 2022-10-20 15:21:21.000000 jfExt-1.9.3/jfExt/__init__.py
+-rw-r--r--   0 jifu       (501) staff       (20)     1949 2022-09-21 20:38:29.000000 jfExt-1.9.3/jfExt/fileExt.py
+drwxr-xr-x   0 jifu       (501) staff       (20)        0 2022-12-08 18:06:18.472017 jfExt-1.9.3/jfExt.egg-info/
+-rw-r--r--   0 jifu       (501) staff       (20)      198 2022-12-08 18:06:18.000000 jfExt-1.9.3/jfExt.egg-info/PKG-INFO
+-rw-r--r--   0 jifu       (501) staff       (20)      779 2022-12-08 18:06:18.000000 jfExt-1.9.3/jfExt.egg-info/SOURCES.txt
+-rw-r--r--   0 jifu       (501) staff       (20)        1 2022-12-08 18:06:18.000000 jfExt-1.9.3/jfExt.egg-info/dependency_links.txt
+-rw-r--r--   0 jifu       (501) staff       (20)       94 2022-12-08 18:06:18.000000 jfExt-1.9.3/jfExt.egg-info/requires.txt
+-rw-r--r--   0 jifu       (501) staff       (20)        6 2022-12-08 18:06:18.000000 jfExt-1.9.3/jfExt.egg-info/top_level.txt
+-rw-r--r--   0 jifu       (501) staff       (20)        1 2022-05-13 21:15:03.000000 jfExt-1.9.3/jfExt.egg-info/zip-safe
+-rw-r--r--   0 jifu       (501) staff       (20)       38 2022-12-08 18:06:18.475538 jfExt-1.9.3/setup.cfg
+-rw-r--r--   0 jifu       (501) staff       (20)     1083 2022-12-08 18:05:58.000000 jfExt-1.9.3/setup.py
```

### Comparing `jfExt-1.9.2/jfExt/BasicType/BooleanExt.py` & `jfExt-1.9.3/jfExt/BasicType/BooleanExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/BasicType/DictExt.py` & `jfExt-1.9.3/jfExt/BasicType/DictExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/BasicType/JsonExt.py` & `jfExt-1.9.3/jfExt/BasicType/JsonExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/BasicType/StringExt.py` & `jfExt-1.9.3/jfExt/BasicType/StringExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/CommonExt.py` & `jfExt-1.9.3/jfExt/CommonExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/CurrencyExt.py` & `jfExt-1.9.3/jfExt/CurrencyExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/EncryptExt.py` & `jfExt-1.9.3/jfExt/EncryptExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/GeoExt.py` & `jfExt-1.9.3/jfExt/GeoExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/ImageExt.py` & `jfExt-1.9.3/jfExt/ImageExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/IpExt.py` & `jfExt-1.9.3/jfExt/IpExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/Mgr/mailMgr.py` & `jfExt-1.9.3/jfExt/Mgr/mailMgr.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/Mgr/redisMgr.py` & `jfExt-1.9.3/jfExt/Mgr/redisMgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def get_value_by_prefix(self, key_prefix):
         """
         >>> 通配符获取 Key Value
         :param {String} key_prefix: 键名 通配符
         :returns {List<String>}: list<键名key>
         """
-        return self.client.keys(pattern="{}.*".format(key_prefix))
+        return self.client.keys(pattern="{}*".format(key_prefix))
 
     def insert_set(self, key, value, expire_time=8640000):
         """
         >>> 插入 set 值
         :param {String} key: set键名称
         :param {String} value: 键值
         :param {Int} expire_time: 过期时间 (default 60s * 60m * 24h * 10 d)
```

### Comparing `jfExt-1.9.2/jfExt/Mgr/responseMgr.py` & `jfExt-1.9.3/jfExt/Mgr/responseMgr.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/OrderExt.py` & `jfExt-1.9.3/jfExt/OrderExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/PrintExt.py` & `jfExt-1.9.3/jfExt/PrintExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/RequestExt.py` & `jfExt-1.9.3/jfExt/RequestExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/Time/DateExt.py` & `jfExt-1.9.3/jfExt/Time/DateExt.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     otherStyleTime = dateDayafter.strftime(DATE_FORMAT)
     return otherStyleTime
 
 
 def date_yesterday_time():
     """
     >>> 获取昨天的时间
-    :return {String}: the time of yesterday
+    :return {Datetime}: the time of yesterday
     """
     oneday = datetime.timedelta(days=1)
     today = datetime.date.today()
     yesterday = today - oneday
     return yesterday
```

### Comparing `jfExt-1.9.2/jfExt/Time/TimeExt.py` & `jfExt-1.9.3/jfExt/Time/TimeExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/ValidExt.py` & `jfExt-1.9.3/jfExt/ValidExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/__init__.py` & `jfExt-1.9.3/jfExt/__init__.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt/fileExt.py` & `jfExt-1.9.3/jfExt/fileExt.py`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/jfExt.egg-info/SOURCES.txt` & `jfExt-1.9.3/jfExt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jfExt-1.9.2/setup.py` & `jfExt-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     #     version = '{}.{}.{}'.format(major, sub, str(int(rev) + 1))
     #     fp.close()
     #     fp = open('version', 'w')
     #     fp.write(version)
     #     return version
     # except Exception:
     #     return "1.0.0"
-    return "1.9.2"
+    return "1.9.3"
 
 
 setup(
     name='jfExt',
     version=update_current_version(),
     description='private common python framework',
     long_description='...',
```

