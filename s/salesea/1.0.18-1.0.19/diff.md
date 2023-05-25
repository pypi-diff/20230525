# Comparing `tmp/salesea-1.0.18.tar.gz` & `tmp/salesea-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.18.tar", last modified: Thu May 25 04:59:10 2023, max compression
+gzip compressed data, was "salesea-1.0.19.tar", last modified: Thu May 25 05:16:08 2023, max compression
```

## Comparing `salesea-1.0.18.tar` & `salesea-1.0.19.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 04:59:10.829275 salesea-1.0.18/
--rw-rw-rw-   0        0        0     2588 2023-05-25 04:59:10.829275 salesea-1.0.18/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.18/README.md
--rw-rw-rw-   0        0        0      111 2023-05-25 04:59:10.830275 salesea-1.0.18/setup.cfg
--rw-rw-rw-   0        0        0     2300 2023-05-25 04:55:21.000000 salesea-1.0.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:59:10.810737 salesea-1.0.18/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 04:59:10.822275 salesea-1.0.18/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.18/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     4545 2023-05-25 03:12:20.000000 salesea-1.0.18/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7361 2023-05-25 04:57:16.000000 salesea-1.0.18/src/salesea/app.py
--rw-rw-rw-   0        0        0     3746 2023-05-24 08:02:59.000000 salesea-1.0.18/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.18/src/salesea/log.py
--rw-rw-rw-   0        0        0    18653 2023-05-25 04:55:13.000000 salesea-1.0.18/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.18/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.18/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:59:10.828304 salesea-1.0.18/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-05-25 04:59:10.000000 salesea-1.0.18/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-25 04:59:10.000000 salesea-1.0.18/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 04:59:10.000000 salesea-1.0.18/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 04:59:10.000000 salesea-1.0.18/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-25 04:59:10.000000 salesea-1.0.18/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 04:59:10.000000 salesea-1.0.18/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 05:16:08.274768 salesea-1.0.19/
+-rw-rw-rw-   0        0        0     2588 2023-05-25 05:16:08.274768 salesea-1.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.19/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-25 05:16:08.275789 salesea-1.0.19/setup.cfg
+-rw-rw-rw-   0        0        0     2300 2023-05-25 05:14:41.000000 salesea-1.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:16:08.256206 salesea-1.0.19/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 05:16:08.267768 salesea-1.0.19/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.19/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     4545 2023-05-25 03:12:20.000000 salesea-1.0.19/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7361 2023-05-25 04:57:16.000000 salesea-1.0.19/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3746 2023-05-24 08:02:59.000000 salesea-1.0.19/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.19/src/salesea/log.py
+-rw-rw-rw-   0        0        0    18905 2023-05-25 05:15:52.000000 salesea-1.0.19/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      970 2023-05-24 10:13:19.000000 salesea-1.0.19/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.19/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:16:08.273770 salesea-1.0.19/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2588 2023-05-25 05:16:08.000000 salesea-1.0.19/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-25 05:16:08.000000 salesea-1.0.19/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:16:08.000000 salesea-1.0.19/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 05:16:08.000000 salesea-1.0.19/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-25 05:16:08.000000 salesea-1.0.19/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 05:16:08.000000 salesea-1.0.19/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.18/PKG-INFO` & `salesea-1.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.18
+Version: 1.0.19
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `salesea-1.0.18/README.md` & `salesea-1.0.19/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.18/setup.py` & `salesea-1.0.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.18',
+    version='1.0.19',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
```

### Comparing `salesea-1.0.18/src/salesea/__main__.py` & `salesea-1.0.19/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.18/src/salesea/app.py` & `salesea-1.0.19/src/salesea/app.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.18/src/salesea/config.py` & `salesea-1.0.19/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.18/src/salesea/log.py` & `salesea-1.0.19/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.18/src/salesea/nginx.py` & `salesea-1.0.19/src/salesea/nginx.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 indent = matched.group(1).replace('\n', '')
                 include_salesea = f'\n{indent}# --------Salesea Config Start--------\n'
                 include_salesea += matched.group(1).replace('\n', '') + f"include {salesea_conf_path};"
                 include_salesea += f'\n{indent}# --------Salesea Config End--------'
                 return matched.group() + include_salesea
 
             content = re.sub(
-                rf"[;\n](\s*)server_name\s+{server_name}\s*;",
+                rf"[;\n]([\s\t]*)server_name\s+{server_name}\s*;",
                 include_salesea,
                 content
             )
             self.nginx.nginxConfigs[self.serverConfigPath] = content
             with open(self.serverConfigPath, mode="w", encoding="utf-8") as fobj:
                 fobj.write(content.strip('\n') + '\n')
         return flag
@@ -162,15 +162,15 @@
     # --------Salesea Config End--------"""
 
         content = self.nginxConfigs.get(self.httpConfigPath)
         if re.search(r"(\s*log_format\s+salesea\s+)", content) is None:
             logger.info(f"更新[{self.httpConfigPath}]文件")
             # 在http块前不能有注释符号# 前面可能是\n
             content = re.sub(
-                r"(\n\s*http\s+\{)",
+                r"(\n[\s\t]*http\s+\{)",
                 r"\1\n" + salesea_log_format,
                 content
             )
             with open(self.httpConfigPath, "w") as fp:
                 fp.write(content.strip('\n') + '\n')
 
             self.reload()
@@ -359,15 +359,15 @@
         content = (block_content or self.nginx_conf)
 
         # 去除注释 除了# configuration file
         delete_comment = lambda x: x.group(0) if x.group(0).startswith('# configuration file ') else ''
         content = re.sub(r'#[^\n]*', delete_comment, content)
 
         for line in content.splitlines():
-            x = line.replace(' ', '')
+            x = line.replace(' ', '').replace('\t', '')
 
             config_file = re.findall('^# configuration\s+file\s+(.*):', line)
             if len(config_file) > 0:
                 file = config_file[0]
 
             if x.startswith(block_name + '{'):
                 num_of_quote += 1
@@ -402,18 +402,21 @@
                 num_of_quote = 0
 
         return result
 
     def parse_server_block(self):
         self.serverBlock = self.parse_block('server')
 
+        if len(self.serverBlock) == 0:
+            raise NginxException('没有解析到[server]配置文件')
+
         for block in self.serverBlock:
             serverBlock = block['block']
             serverConfigPath = block['file']
-            logger.debug(f'匹配到[server]配置文件[{serverConfigPath}]')
+            logger.debug(f'解析到[server]配置文件[{serverConfigPath}]')
 
             port = re.findall('listen\s*((?:\d|\s)*)[^;]*;', serverBlock)[0]  # port只有一个
             r = re.findall('server_name\s+([^;]*);', serverBlock)  # server_name只有一个
 
             # 可能存在没有server_name的情况
             if len(r) > 0:
                 servername = r[0]
@@ -464,18 +467,21 @@
 
             self.servers.append(server)
 
     def parse_http_block(self):
         self.httpBlock = self.parse_block('http')
         httpConfigPath = None
 
+        if len(self.httpBlock) == 0:
+            raise NginxException('没有解析到[http]配置文件')
+
         for block in self.httpBlock:
             httpBlock = block['block']
             httpConfigPath = self.httpConfigPath or block['file']
-            logger.debug(f'匹配到[http]配置文件[{httpConfigPath}]')
+            logger.debug(f'解析到[http]配置文件[{httpConfigPath}]')
 
             # 获取log_format log_format后面不能是\n
             for log_format in re.findall('\s*log_format\s+([^;]*);', httpBlock):
                 log_format = log_format.strip()
                 name, log_format = log_format.split(' ', 1)
                 self.logFormats[name] = log_format
```

### Comparing `salesea-1.0.18/src/salesea/solution.py` & `salesea-1.0.19/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.18/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.19/src/salesea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.18
+Version: 1.0.19
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

