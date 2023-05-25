# Comparing `tmp/txfdjangomix-1.7.tar.gz` & `tmp/txfdjangomix-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txfdjangomix-1.7.tar", last modified: Thu Nov 17 06:05:07 2022, max compression
+gzip compressed data, was "txfdjangomix-1.8.tar", last modified: Thu May 25 06:40:26 2023, max compression
```

## Comparing `txfdjangomix-1.7.tar` & `txfdjangomix-1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.835139 txfdjangomix-1.7/
--rw-rw-rw-   0        0        0    11558 2022-06-17 08:26:46.000000 txfdjangomix-1.7/LICENSE
--rw-rw-rw-   0        0        0      425 2022-11-17 06:05:07.835139 txfdjangomix-1.7/PKG-INFO
--rw-rw-rw-   0        0        0       31 2022-06-17 09:05:06.000000 txfdjangomix-1.7/README.md
--rw-rw-rw-   0        0        0       42 2022-11-17 06:05:07.836135 txfdjangomix-1.7/setup.cfg
--rw-rw-rw-   0        0        0      875 2022-11-16 08:58:40.000000 txfdjangomix-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.737398 txfdjangomix-1.7/txfdjangomix/
--rw-rw-rw-   0        0        0     1205 2022-06-17 02:10:26.000000 txfdjangomix-1.7/txfdjangomix/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.753357 txfdjangomix-1.7/txfdjangomix/django_log/
--rw-rw-rw-   0        0        0     1205 2022-06-13 09:56:48.000000 txfdjangomix-1.7/txfdjangomix/django_log/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.788264 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/
--rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/__init__.py
--rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/admin.py
--rw-rw-rw-   0        0        0      151 2022-06-13 09:59:01.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/apps.py
--rw-rw-rw-   0        0        0     2279 2022-06-16 09:45:23.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/insert_django_sql.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.789260 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/migrations/
--rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/migrations/__init__.py
--rw-rw-rw-   0        0        0      936 2022-06-16 09:32:42.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/models.py
--rw-rw-rw-   0        0        0       63 2022-06-13 09:59:01.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/tests.py
--rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-1.7/txfdjangomix/django_log/sql_log/views.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.814193 txfdjangomix-1.7/txfdjangomix/django_response_middleware/
--rw-rw-rw-   0        0        0      734 2021-12-06 02:22:57.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/__init__.py
--rw-rw-rw-   0        0        0     3219 2022-09-22 09:05:48.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/django_response_middleware.py
--rw-rw-rw-   0        0        0     3496 2021-12-06 02:22:57.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/response_codes.py
--rw-rw-rw-   0        0        0     3393 2022-11-16 08:48:59.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/response_data.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.827159 txfdjangomix-1.7/txfdjangomix/django_response_middleware/utils/
--rw-rw-rw-   0        0        0        0 2021-12-06 03:12:37.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/utils/__init__.py
--rw-rw-rw-   0        0        0     1388 2022-06-06 01:56:29.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/utils/json_cls.py
--rw-rw-rw-   0        0        0      720 2022-02-17 07:07:07.000000 txfdjangomix-1.7/txfdjangomix/django_response_middleware/utils/type_conversion.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.834140 txfdjangomix-1.7/txfdjangomix/utils/
--rw-rw-rw-   0        0        0        0 2022-07-05 11:50:18.000000 txfdjangomix-1.7/txfdjangomix/utils/__init__.py
--rw-rw-rw-   0        0        0     6176 2022-11-15 02:17:48.000000 txfdjangomix-1.7/txfdjangomix/utils/models.py
-drwxrwxrwx   0        0        0        0 2022-11-17 06:05:07.751361 txfdjangomix-1.7/txfdjangomix.egg-info/
--rw-rw-rw-   0        0        0      425 2022-11-17 06:05:07.000000 txfdjangomix-1.7/txfdjangomix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2022-11-17 06:05:07.000000 txfdjangomix-1.7/txfdjangomix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 06:05:07.000000 txfdjangomix-1.7/txfdjangomix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-11-17 06:05:07.000000 txfdjangomix-1.7/txfdjangomix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-17 06:05:07.000000 txfdjangomix-1.7/txfdjangomix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-05 11:52:46.000000 txfdjangomix-1.7/txfdjangomix.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.342841 txfdjangomix-1.8/
+-rw-rw-rw-   0        0        0    11558 2022-06-17 08:26:46.000000 txfdjangomix-1.8/LICENSE
+-rw-rw-rw-   0        0        0      425 2023-05-25 06:40:26.341844 txfdjangomix-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2022-06-17 09:05:06.000000 txfdjangomix-1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 06:40:26.342841 txfdjangomix-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-05-25 06:38:18.000000 txfdjangomix-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.229080 txfdjangomix-1.8/txfdjangomix/
+-rw-rw-rw-   0        0        0     1205 2022-06-17 02:10:26.000000 txfdjangomix-1.8/txfdjangomix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.250024 txfdjangomix-1.8/txfdjangomix/django_log/
+-rw-rw-rw-   0        0        0     1205 2022-06-13 09:56:48.000000 txfdjangomix-1.8/txfdjangomix/django_log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.292913 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/
+-rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/admin.py
+-rw-rw-rw-   0        0        0      151 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/apps.py
+-rw-rw-rw-   0        0        0     2279 2022-06-16 09:45:23.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/insert_django_sql.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.293907 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/migrations/
+-rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/migrations/__init__.py
+-rw-rw-rw-   0        0        0      936 2022-06-16 09:32:42.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/models.py
+-rw-rw-rw-   0        0        0       63 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/tests.py
+-rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/views.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.319838 txfdjangomix-1.8/txfdjangomix/django_response_middleware/
+-rw-rw-rw-   0        0        0      734 2021-12-06 02:22:57.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/__init__.py
+-rw-rw-rw-   0        0        0     3219 2022-09-22 09:05:48.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/django_response_middleware.py
+-rw-rw-rw-   0        0        0     3496 2021-12-06 02:22:57.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_codes.py
+-rw-rw-rw-   0        0        0     3500 2023-05-25 06:38:18.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_data.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.329875 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-06 03:12:37.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/__init__.py
+-rw-rw-rw-   0        0        0     1388 2022-06-06 01:56:29.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/json_cls.py
+-rw-rw-rw-   0        0        0      755 2023-05-25 06:38:18.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/type_conversion.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.340846 txfdjangomix-1.8/txfdjangomix/utils/
+-rw-rw-rw-   0        0        0        0 2022-07-05 11:50:18.000000 txfdjangomix-1.8/txfdjangomix/utils/__init__.py
+-rw-rw-rw-   0        0        0     6381 2022-12-16 03:10:31.000000 txfdjangomix-1.8/txfdjangomix/utils/models.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.247032 txfdjangomix-1.8/txfdjangomix.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-07-05 11:52:46.000000 txfdjangomix-1.8/txfdjangomix.egg-info/zip-safe
```

### Comparing `txfdjangomix-1.7/LICENSE` & `txfdjangomix-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/setup.py` & `txfdjangomix-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='txfdjangomix',  # 名字
-      version='1.7',  # 版本
+      version='1.8',  # 版本
       description='django response middleware',  # 简介一般我们放在readme.md
       classifiers=[
           'Programming Language :: Python',  # python
           'Intended Audience :: Developers',  # 受众人
           'Operating System :: OS Independent',  # 系统
       ],
       long_description_content_type="text/markdown",  # 类型
```

### Comparing `txfdjangomix-1.7/txfdjangomix/__init__.py` & `txfdjangomix-1.8/txfdjangomix/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_log/__init__.py` & `txfdjangomix-1.8/txfdjangomix/django_log/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_log/sql_log/insert_django_sql.py` & `txfdjangomix-1.8/txfdjangomix/django_log/sql_log/insert_django_sql.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_log/sql_log/models.py` & `txfdjangomix-1.8/txfdjangomix/django_log/sql_log/models.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_response_middleware/__init__.py` & `txfdjangomix-1.8/txfdjangomix/django_response_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_response_middleware/django_response_middleware.py` & `txfdjangomix-1.8/txfdjangomix/django_response_middleware/django_response_middleware.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_response_middleware/response_codes.py` & `txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_codes.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_response_middleware/response_data.py` & `txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         if response_code['200'].get('datas'):
             del response_code['200']['datas']
 
         code = response_code['200']['code']
         message = response_code['200']['message']
         if not data:
             ret = {code_key: code, message_key: message, datas_key: {}}
-            return Response(ret)
+            json_data = json.dumps(ret, cls=cls)
+            return HttpResponse(json_data, content_type="application/json;charset=utf-8")
         else:
             ret = {code_key: code, message_key: message, datas_key: data}
             json_data = json.dumps(ret, cls=cls)
             return HttpResponse(json_data, content_type="application/json;charset=utf-8")
 
     def customize_code_message(self, code, message, data=None,
                                code_key='code',
```

### Comparing `txfdjangomix-1.7/txfdjangomix/django_response_middleware/utils/json_cls.py` & `txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/json_cls.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.7/txfdjangomix/django_response_middleware/utils/type_conversion.py` & `txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/type_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,21 +25,24 @@
 00000180: 6929 2066 6f72 2069 2069 6e20 7175 6572  i) for i in quer
 00000190: 795f 6c69 7374 5d0d 0a20 2020 2020 2020  y_list]..       
 000001a0: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
 000001b0: 2020 2020 2020 7265 7475 726e 205b 6920        return [i 
 000001c0: 666f 7220 6920 696e 2071 7565 7279 5f6c  for i in query_l
 000001d0: 6973 745d 0d0a 0d0a 0d0a 6465 6620 6c69  ist]......def li
 000001e0: 7374 5f73 7472 2865 7272 6f72 5f6c 6973  st_str(error_lis
-000001f0: 7429 3a0d 0a20 2020 2065 7272 6f72 5f6c  t):..    error_l
-00000200: 6973 745f 203d 205b 5d0d 0a20 2020 2069  ist_ = []..    i
-00000210: 6620 6973 696e 7374 616e 6365 2865 7272  f isinstance(err
-00000220: 6f72 5f6c 6973 742c 2064 6963 7429 3a0d  or_list, dict):.
-00000230: 0a20 2020 2020 2020 2065 7272 6f72 5f6c  .        error_l
-00000240: 6973 7420 3d20 5b65 7272 6f72 5f6c 6973  ist = [error_lis
-00000250: 745d 0d0a 2020 2020 666f 7220 6969 2069  t]..    for ii i
-00000260: 6e20 6572 726f 725f 6c69 7374 3a0d 0a20  n error_list:.. 
-00000270: 2020 2020 2020 2066 6f72 206b 2c20 7620         for k, v 
-00000280: 696e 2069 692e 6974 656d 7328 293a 0d0a  in ii.items():..
-00000290: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-000002a0: 725f 6c69 7374 5f2e 6170 7065 6e64 287b  r_list_.append({
-000002b0: 6b3a 2076 7d29 0d0a 2020 2020 7265 7475  k: v})..    retu
-000002c0: 726e 2065 7272 6f72 5f6c 6973 745f 0d0a  rn error_list_..
+000001f0: 7429 3a0d 0a20 2020 2023 2065 7272 6f72  t):..    # error
+00000200: 5f6c 6973 745f 203d 205b 5d0d 0a20 2020  _list_ = []..   
+00000210: 2023 2069 6620 6973 696e 7374 616e 6365   # if isinstance
+00000220: 2865 7272 6f72 5f6c 6973 742c 2064 6963  (error_list, dic
+00000230: 7429 3a0d 0a20 2020 2023 2020 2020 2065  t):..    #     e
+00000240: 7272 6f72 5f6c 6973 7420 3d20 5b65 7272  rror_list = [err
+00000250: 6f72 5f6c 6973 745d 0d0a 2020 2020 2320  or_list]..    # 
+00000260: 666f 7220 6969 2069 6e20 6572 726f 725f  for ii in error_
+00000270: 6c69 7374 3a0d 0a20 2020 2023 2020 2020  list:..    #    
+00000280: 2066 6f72 206b 2c20 7620 696e 2069 692e   for k, v in ii.
+00000290: 6974 656d 7328 293a 0d0a 2020 2020 2320  items():..    # 
+000002a0: 2020 2020 2020 2020 6572 726f 725f 6c69          error_li
+000002b0: 7374 5f2e 6170 7065 6e64 287b 6b3a 2076  st_.append({k: v
+000002c0: 7d29 0d0a 2020 2020 2320 7265 7475 726e  })..    # return
+000002d0: 2065 7272 6f72 5f6c 6973 745f 0d0a 2020   error_list_..  
+000002e0: 2020 7265 7475 726e 2065 7272 6f72 5f6c    return error_l
+000002f0: 6973 74                                  ist
```

### Comparing `txfdjangomix-1.7/txfdjangomix/utils/models.py` & `txfdjangomix-1.8/txfdjangomix/utils/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
         abstract = True
 
 
 def model_field_relation(app_name, model_name):
     """返回模型类对象信息
     app_name : 模型类models所在的文件夹的名称 str
     model_nam : 模型类的名称 str
+                如 ’User‘ 不是db_table
+                如果通过对象获取使用 User.__name__ 会得到字符串 “User”
+                model_obj._meta 可以获取 Meta的属性信息
     return (<django.db.models.fields.BigAutoField: id>, <django.db.models.fields.DateTimeField: create_time>)
     """
     model_obj = apps.get_model(app_name, model_name)
     filed = model_obj._meta.fields
     return filed
```

### Comparing `txfdjangomix-1.7/txfdjangomix.egg-info/SOURCES.txt` & `txfdjangomix-1.8/txfdjangomix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

