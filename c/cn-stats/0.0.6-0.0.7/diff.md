# Comparing `tmp/cn_stats-0.0.6.tar.gz` & `tmp/cn_stats-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cn_stats-0.0.6.tar", last modified: Thu Mar 31 03:04:56 2022, max compression
+gzip compressed data, was "cn_stats-0.0.7.tar", last modified: Thu May 25 09:37:34 2023, max compression
```

## Comparing `cn_stats-0.0.6.tar` & `cn_stats-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sj        (1000) sj        (1000)        0 2022-03-31 03:04:56.879858 cn_stats-0.0.6/
--rw-r--r--   0 sj        (1000) sj        (1000)    26811 2022-03-31 03:04:56.869858 cn_stats-0.0.6/PKG-INFO
--rw-r--r--   0 sj        (1000) sj        (1000)    26371 2022-03-25 03:19:26.000000 cn_stats-0.0.6/README.md
-drwxr-xr-x   0 sj        (1000) sj        (1000)        0 2022-03-31 03:04:56.869858 cn_stats-0.0.6/cn_stats.egg-info/
--rw-r--r--   0 sj        (1000) sj        (1000)    26811 2022-03-31 03:04:56.000000 cn_stats-0.0.6/cn_stats.egg-info/PKG-INFO
--rw-r--r--   0 sj        (1000) sj        (1000)      252 2022-03-31 03:04:56.000000 cn_stats-0.0.6/cn_stats.egg-info/SOURCES.txt
--rw-r--r--   0 sj        (1000) sj        (1000)        1 2022-03-31 03:04:56.000000 cn_stats-0.0.6/cn_stats.egg-info/dependency_links.txt
--rw-r--r--   0 sj        (1000) sj        (1000)       17 2022-03-31 03:04:56.000000 cn_stats-0.0.6/cn_stats.egg-info/requires.txt
--rw-r--r--   0 sj        (1000) sj        (1000)        8 2022-03-31 03:04:56.000000 cn_stats-0.0.6/cn_stats.egg-info/top_level.txt
-drwxr-xr-x   0 sj        (1000) sj        (1000)        0 2022-03-31 03:04:56.869858 cn_stats-0.0.6/cnstats/
--rw-r--r--   0 sj        (1000) sj        (1000)        0 2022-03-15 07:40:21.000000 cn_stats-0.0.6/cnstats/__init__.py
--rw-r--r--   0 sj        (1000) sj        (1000)      703 2022-03-31 03:02:34.000000 cn_stats-0.0.6/cnstats/__main__.py
--rw-r--r--   0 sj        (1000) sj        (1000)     1555 2022-03-30 09:51:15.000000 cn_stats-0.0.6/cnstats/stats.py
--rw-r--r--   0 sj        (1000) sj        (1000)     1039 2022-03-31 02:43:09.000000 cn_stats-0.0.6/cnstats/zbcode.py
--rw-r--r--   0 sj        (1000) sj        (1000)       38 2022-03-31 03:04:56.879858 cn_stats-0.0.6/setup.cfg
--rw-r--r--   0 sj        (1000) sj        (1000)     1724 2022-03-31 03:04:16.000000 cn_stats-0.0.6/setup.py
+drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2023-05-25 09:37:34.204958 cn_stats-0.0.7/
+-rw-rw-r--   0 sj        (1000) sj        (1000)    26809 2023-05-25 09:37:34.204958 cn_stats-0.0.7/PKG-INFO
+-rw-rw-r--   0 sj        (1000) sj        (1000)    26371 2023-03-26 12:37:15.000000 cn_stats-0.0.7/README.md
+drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2023-05-25 09:37:34.204958 cn_stats-0.0.7/cn_stats.egg-info/
+-rw-rw-r--   0 sj        (1000) sj        (1000)    26809 2023-05-25 09:37:34.000000 cn_stats-0.0.7/cn_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 sj        (1000) sj        (1000)      252 2023-05-25 09:37:34.000000 cn_stats-0.0.7/cn_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 sj        (1000) sj        (1000)        1 2023-05-25 09:37:34.000000 cn_stats-0.0.7/cn_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 sj        (1000) sj        (1000)       31 2023-05-25 09:37:34.000000 cn_stats-0.0.7/cn_stats.egg-info/requires.txt
+-rw-rw-r--   0 sj        (1000) sj        (1000)        8 2023-05-25 09:37:34.000000 cn_stats-0.0.7/cn_stats.egg-info/top_level.txt
+drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2023-05-25 09:37:34.204958 cn_stats-0.0.7/cnstats/
+-rw-rw-r--   0 sj        (1000) sj        (1000)        0 2023-01-06 06:03:41.000000 cn_stats-0.0.7/cnstats/__init__.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)      761 2023-05-25 09:28:26.000000 cn_stats-0.0.7/cnstats/__main__.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1667 2023-05-25 09:28:08.000000 cn_stats-0.0.7/cnstats/stats.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1039 2023-01-06 06:03:41.000000 cn_stats-0.0.7/cnstats/zbcode.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)       38 2023-05-25 09:37:34.204958 cn_stats-0.0.7/setup.cfg
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1740 2023-05-25 09:35:30.000000 cn_stats-0.0.7/setup.py
```

### Comparing `cn_stats-0.0.6/PKG-INFO` & `cn_stats-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cn_stats
-Version: 0.0.6
-Summary: 获取中国国家统计局网站数据
+Version: 0.0.7
+Summary: 获取中国国家统计局网站数据。
 Home-page: https://github.com/songjian/cnstats
 Author: sj
-Author-email: songjian@codeorder.cn
+Author-email: 724385768@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `cn_stats-0.0.6/README.md` & `cn_stats-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.6/cn_stats.egg-info/PKG-INFO` & `cn_stats-0.0.7/cn_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cn-stats
-Version: 0.0.6
-Summary: 获取中国国家统计局网站数据
+Version: 0.0.7
+Summary: 获取中国国家统计局网站数据。
 Home-page: https://github.com/songjian/cnstats
 Author: sj
-Author-email: songjian@codeorder.cn
+Author-email: 724385768@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `cn_stats-0.0.6/cnstats/__main__.py` & `cn_stats-0.0.7/cnstats/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,11 @@
     parser.add_argument('--dbcode', nargs='?', const='hgyd', default='hgyd', help='数据库代码')
     parser.add_argument('zbcode', help='指标代码', nargs='?')
     parser.add_argument('date', help='查询日期', nargs='?')
     args=parser.parse_args()
     if args.tree == 'zb':
         get_tree(args.tree, args.dbcode)
     else:
-        stats(args.zbcode, args.date)
+        r=stats(args.zbcode, args.date)
+        for row in r:
+            print(' '.join(row))
+
```

### Comparing `cn_stats-0.0.6/cnstats/stats.py` & `cn_stats-0.0.7/cnstats/stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,18 +22,22 @@
     'dfwds': '[{"wdcode":"zb","valuecode":"'+code+'"},{"wdcode":"sj","valuecode":"'+datestr+'"}]',
     'k1': random_timestamp()
     }
     requests.packages.urllib3.disable_warnings()
     r = requests.post(url, data=obj, headers=header, verify=False)
     return r.json()
 
+
 def stats(code, datestr):
     ret=easyquery(code, datestr)
     if ret['returncode'] == 200 :
+        data_dict = {}
+        for n in ret['returndata']['wdnodes']:
+            if n['wdcode'] == 'zb':
+                for i in n['nodes']:
+                    data_dict[i['code']] = i['cname']
+
+        result = []
         for n in ret['returndata']['datanodes']:
             if n['data']['hasdata'] == True:
-                print(n['wds'][0]['valuecode'],n['wds'][1]['valuecode'],n['data']['data'])
-
-        # for n in ret['returndata']['wdnodes']:
-        #     if n['wdcode'] == 'zb':
-        #         for i in n['nodes']:
-        #             print(i['code'], i['cname'])
+                result.append([data_dict[n['wds'][0]['valuecode']],n['wds'][0]['valuecode'],n['wds'][1]['valuecode'],n['data']['strdata']])
+        return result
```

### Comparing `cn_stats-0.0.6/cnstats/zbcode.py` & `cn_stats-0.0.7/cnstats/zbcode.py`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.6/setup.py` & `cn_stats-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cn_stats",                                     # 包的分发名称，使用字母、数字、_、-
-    version="0.0.6",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="0.0.7",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="sj",                                       # 作者名字
-    author_email="songjian@codeorder.cn",                      # 作者邮箱
-    description="获取中国国家统计局网站数据",                            # 包的简介描述
+    author_email="724385768@qq.com",                      # 作者邮箱
+    description="获取中国国家统计局网站数据。",                            # 包的简介描述
     long_description=long_description,                      # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",          # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/songjian/cnstats",                              # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),                    # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     classifiers=[                                           # 关于包的其他元数据(metadata)
         "Programming Language :: Python :: 3",              # 该软件包仅与Python3兼容
         "License :: OSI Approved :: MIT License",           # 根据MIT许可证开源
         "Operating System :: OS Independent",               # 与操作系统无关
     ],
-    install_requires=['requests==2.27.1'],  # 依赖的包
+    install_requires=['requests==2.28.1', 'pandas==1.4.1'],  # 依赖的包
     python_requires='>=3'
 )
```

