# Comparing `tmp/bkapi-plugins-py-0.524.tar.gz` & `tmp/bkapi-plugins-py-0.525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.524.tar", last modified: Wed May 24 02:38:56 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.525.tar", last modified: Thu May 25 05:28:41 2023, max compression
```

## Comparing `bkapi-plugins-py-0.524.tar` & `bkapi-plugins-py-0.525.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:56.809882 bkapi-plugins-py-0.524/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.524/MANIFEST.in
--rw-rw-rw-   0        0        0      257 2023-05-24 02:38:56.809882 bkapi-plugins-py-0.524/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:56.794896 bkapi-plugins-py-0.524/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:56.802883 bkapi-plugins-py-0.524/bkapi_plugins/files/
--rw-rw-rw-   0        0        0     1331 2023-05-24 02:36:37.000000 bkapi-plugins-py-0.524/bkapi_plugins/files/feishu-alert.zip
-drwxrwxrwx   0        0        0        0 2023-05-24 02:38:56.808883 bkapi-plugins-py-0.524/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      257 2023-05-24 02:38:56.000000 bkapi-plugins-py-0.524/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-24 02:38:56.000000 bkapi-plugins-py-0.524/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:38:56.000000 bkapi-plugins-py-0.524/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:38:56.000000 bkapi-plugins-py-0.524/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 02:38:56.810881 bkapi-plugins-py-0.524/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-05-24 02:38:04.000000 bkapi-plugins-py-0.524/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.232976 bkapi-plugins-py-0.525/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.525/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-05-25 05:28:41.233977 bkapi-plugins-py-0.525/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.221976 bkapi-plugins-py-0.525/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.226977 bkapi-plugins-py-0.525/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0   177080 2023-05-25 05:26:18.000000 bkapi-plugins-py-0.525/bkapi_plugins/files/nginx_upstream_check_module-master.zip
+drwxrwxrwx   0        0        0        0 2023-05-25 05:28:41.231982 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:28:41.000000 bkapi-plugins-py-0.525/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 05:28:41.235978 bkapi-plugins-py-0.525/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-05-25 05:28:21.000000 bkapi-plugins-py-0.525/setup.py
```

### Comparing `bkapi-plugins-py-0.524/setup.py` & `bkapi-plugins-py-0.525/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.524', # 版本号每次打包完要改一下
+    version='0.525', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

