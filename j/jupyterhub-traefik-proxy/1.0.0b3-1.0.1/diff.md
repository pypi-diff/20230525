# Comparing `tmp/jupyterhub-traefik-proxy-1.0.0b3.tar.gz` & `tmp/jupyterhub-traefik-proxy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-traefik-proxy-1.0.0b3.tar", last modified: Thu May 11 14:36:38 2023, max compression
+gzip compressed data, was "jupyterhub-traefik-proxy-1.0.1.tar", last modified: Thu May 25 11:24:04 2023, max compression
```

## Comparing `jupyterhub-traefik-proxy-1.0.0b3.tar` & `jupyterhub-traefik-proxy-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.760954 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/consul.py
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/etcd.py
--rw-r--r--   0 runner    (1001) docker     (122)     7035 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/fileprovider.py
--rw-r--r--   0 runner    (1001) docker     (122)     5533 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/install.py
--rw-r--r--   0 runner    (1001) docker     (122)    11844 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/kv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)    26372 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5018 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/traefik_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.760954 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.760954 jupyterhub-traefik-proxy-1.0.0b3/performance/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10504 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/check_perf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/dummy_http_server.py
--rw-r--r--   0 runner    (1001) docker     (122)    10061 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/perf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_kv.py
--rw-r--r--   0 runner    (1001) docker     (122)    15524 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_api_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.239746 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/consul.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7035 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/fileprovider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11844 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/kv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26372 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5018 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/traefik_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.239746 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/tests/config_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/consul_config.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/etcd.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/etcd.key
+-rw-r--r--   0 runner    (1001) docker     (122)    22149 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/dummy_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_kv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15532 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_api_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/utils.py
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/LICENSE` & `jupyterhub-traefik-proxy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/PKG-INFO` & `jupyterhub-traefik-proxy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-traefik-proxy
-Version: 1.0.0b3
+Version: 1.0.1
 Summary: JupyterHub proxy implementation with traefik
 Home-page: https://jupyterhub-traefik-proxy.readthedocs.io
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://jupyterhub-traefik-proxy.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/traefik-proxy/
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/README.md` & `jupyterhub-traefik-proxy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/consul.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/consul.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/etcd.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/etcd.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/fileprovider.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/fileprovider.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/install.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         action="store_true",
         help="DEPRECATED, IGNORED",
     )
 
     parser.add_argument(
         "--traefik-version",
         dest="traefik_version",
-        default="2.9.8",
+        default="2.10.1",
         help=textwrap.dedent(
             """\
             The version of traefik to download.
             If no version is provided, it defaults to:
             --- %(default)s ---
             """
         ),
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/kv_proxy.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/kv_proxy.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/proxy.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/toml.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/toml.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/traefik_utils.py` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/traefik_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/PKG-INFO` & `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-traefik-proxy
-Version: 1.0.0b3
+Version: 1.0.1
 Summary: JupyterHub proxy implementation with traefik
 Home-page: https://jupyterhub-traefik-proxy.readthedocs.io
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://jupyterhub-traefik-proxy.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/traefik-proxy/
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/pyproject.toml` & `jupyterhub-traefik-proxy-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # Ignore thousands of tests in dependencies installed in a virtual environment
 norecursedirs = "lib lib64"
 
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/traefik-proxy"
 
 [tool.tbump.version]
-current = "1.0.0b3"
+current = "1.0.1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/setup.py` & `jupyterhub-traefik-proxy-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup(
     name="jupyterhub-traefik-proxy",
-    version="1.0.0b3",
+    version="1.0.1",
     install_requires=open("requirements.txt").read().splitlines(),
     python_requires=">=3.6",
     author="Project Jupyter Contributors",
     author_email="jupyter@googlegroups.com",
     url="https://jupyterhub-traefik-proxy.readthedocs.io",
     project_urls={
         "Documentation": "https://jupyterhub-traefik-proxy.readthedocs.io",
@@ -34,15 +34,15 @@
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-    packages=find_packages(),
+    packages=find_packages(exclude=["performance", "tests"]),
     include_package_data=True,
     entry_points={
         "jupyterhub.proxies": [
             "traefik_consul = jupyterhub_traefik_proxy.consul:TraefikConsulProxy",
             "traefik_etcd = jupyterhub_traefik_proxy.etcd:TraefikEtcdProxy",
             "traefik_file = jupyterhub_traefik_proxy.fileprovider:TraefikFileProviderProxy",
             "traefik_toml = jupyterhub_traefik_proxy.toml:TraefikTomlProxy",
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/tests/test_deprecations.py` & `jupyterhub-traefik-proxy-1.0.1/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/tests/test_installer.py` & `jupyterhub-traefik-proxy-1.0.1/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/tests/test_kv.py` & `jupyterhub-traefik-proxy-1.0.1/tests/test_kv.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/tests/test_proxy.py` & `jupyterhub-traefik-proxy-1.0.1/tests/test_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 from contextlib import contextmanager
 from os.path import abspath, dirname, join
 from random import randint
 from unittest.mock import Mock
 from urllib.parse import quote, urlparse
 
 import pytest
-import utils
 import websockets
 from jupyterhub.objects import Hub, Server
 from jupyterhub.user import User
 from jupyterhub.utils import exponential_backoff, url_path_join
 from tornado.httpclient import AsyncHTTPClient, HTTPClientError, HTTPRequest
 
 from jupyterhub_traefik_proxy.proxy import TraefikProxy
 
+from . import utils
+
 # Mark all tests in this file as slow
 pytestmark = [pytest.mark.slow]
 
 pp = pprint.PrettyPrinter(indent=2)
 
 
 class MockApp:
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_api_auth.py` & `jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_api_auth.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_utils.py` & `jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_utils.py`

 * *Files identical despite different names*

