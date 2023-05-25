# Comparing `tmp/salesea-1.0.15.tar.gz` & `tmp/salesea-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.15.tar", last modified: Thu May 25 03:40:53 2023, max compression
+gzip compressed data, was "salesea-1.0.16.tar", last modified: Thu May 25 03:53:44 2023, max compression
```

## Comparing `salesea-1.0.15.tar` & `salesea-1.0.16.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 03:40:53.850926 salesea-1.0.15/
--rw-rw-rw-   0        0        0     2588 2023-05-25 03:40:53.850926 salesea-1.0.15/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.15/README.md
--rw-rw-rw-   0        0        0      111 2023-05-25 03:40:53.851927 salesea-1.0.15/setup.cfg
--rw-rw-rw-   0        0        0     2300 2023-05-25 03:40:50.000000 salesea-1.0.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:40:53.825685 salesea-1.0.15/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 03:40:53.843928 salesea-1.0.15/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.15/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     4545 2023-05-25 03:12:20.000000 salesea-1.0.15/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7358 2023-05-25 02:35:58.000000 salesea-1.0.15/src/salesea/app.py
--rw-rw-rw-   0        0        0     3746 2023-05-24 08:02:59.000000 salesea-1.0.15/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.15/src/salesea/log.py
--rw-rw-rw-   0        0        0    18424 2023-05-25 03:40:15.000000 salesea-1.0.15/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.15/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.15/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:40:53.849926 salesea-1.0.15/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-05-25 03:40:53.000000 salesea-1.0.15/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-25 03:40:53.000000 salesea-1.0.15/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 03:40:53.000000 salesea-1.0.15/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 03:40:53.000000 salesea-1.0.15/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-25 03:40:53.000000 salesea-1.0.15/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 03:40:53.000000 salesea-1.0.15/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 03:53:44.699846 salesea-1.0.16/
+-rw-rw-rw-   0        0        0     2588 2023-05-25 03:53:44.699846 salesea-1.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.16/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-25 03:53:44.700846 salesea-1.0.16/setup.cfg
+-rw-rw-rw-   0        0        0     2300 2023-05-25 03:53:30.000000 salesea-1.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:53:44.681849 salesea-1.0.16/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 03:53:44.692846 salesea-1.0.16/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.16/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     4545 2023-05-25 03:12:20.000000 salesea-1.0.16/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7358 2023-05-25 02:35:58.000000 salesea-1.0.16/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3746 2023-05-24 08:02:59.000000 salesea-1.0.16/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.16/src/salesea/log.py
+-rw-rw-rw-   0        0        0    18579 2023-05-25 03:53:09.000000 salesea-1.0.16/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.16/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.16/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 03:53:44.698848 salesea-1.0.16/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2588 2023-05-25 03:53:44.000000 salesea-1.0.16/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-25 03:53:44.000000 salesea-1.0.16/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 03:53:44.000000 salesea-1.0.16/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 03:53:44.000000 salesea-1.0.16/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-25 03:53:44.000000 salesea-1.0.16/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 03:53:44.000000 salesea-1.0.16/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.15/PKG-INFO` & `salesea-1.0.16/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.15
+Version: 1.0.16
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `salesea-1.0.15/README.md` & `salesea-1.0.16/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.15/setup.py` & `salesea-1.0.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.15',
+    version='1.0.16',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
```

### Comparing `salesea-1.0.15/src/salesea/__main__.py` & `salesea-1.0.16/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.15/src/salesea/app.py` & `salesea-1.0.16/src/salesea/app.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.15/src/salesea/config.py` & `salesea-1.0.16/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.15/src/salesea/log.py` & `salesea-1.0.16/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.15/src/salesea/nginx.py` & `salesea-1.0.16/src/salesea/nginx.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,23 +149,24 @@
         self.parse_server_block()
 
     def is_salesea(self):
         return self.logFormats.get("salesea") is not None
 
     def write_salesea_log_format(self):
         logger.debug("检查[log_format salesea]状态")
+        logger.debug(f"[{self.httpConfigPath}] [{self.nginxConfigs}]")
         if self.is_salesea():
             return
         salesea_log_format = """    # --------Salesea Config Start--------
     log_format salesea '$remote_addr - $remote_user [$time_local] "$request" '
              '$status $body_bytes_sent "$http_referer" '
              '"$http_user_agent" "$http_x_forwarded_for"';
     # --------Salesea Config End--------"""
 
-        content = self.nginxConfigs[self.httpConfigPath]
+        content = self.nginxConfigs.get(self.httpConfigPath)
         if re.search(r"(\s*log_format\s+salesea\s+)", content) is None:
             logger.info(f"更新[{self.httpConfigPath}]文件")
             # 在http块前不能有注释符号# 前面可能是\n
             content = re.sub(
                 r"(\n\s*http\s+\{)",
                 r"\1\n" + salesea_log_format,
                 content
@@ -200,14 +201,15 @@
             self.nginx_conf = os.popen(f"{self.nginx_path} -T").read()
 
     # 拆分nginx配置文件
     def parse_file(self):
         current_path = None
         for line in self.nginx_conf.splitlines():
             config_file = re.findall('^# configuration\s+file\s+(.*):', line)
+            logger.debug(f"current_path: {current_path} config_file: {line}")
             if len(config_file) > 0:
                 current_path = config_file[0]
                 self.nginxConfigs[current_path] = ""
             else:
                 if current_path is not None:
                     self.nginxConfigs[current_path] += line + "\n"
```

### Comparing `salesea-1.0.15/src/salesea/solution.py` & `salesea-1.0.16/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.15/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.16/src/salesea.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.15
+Version: 1.0.16
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

