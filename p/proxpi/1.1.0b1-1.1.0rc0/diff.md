# Comparing `tmp/proxpi-1.1.0b1.tar.gz` & `tmp/proxpi-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxpi-1.1.0b1.tar", last modified: Mon Aug  8 09:59:30 2022, max compression
+gzip compressed data, was "proxpi-1.1.0rc0.tar", last modified: Tue Dec 13 01:12:19 2022, max compression
```

## Comparing `proxpi-1.1.0b1.tar` & `proxpi-1.1.0rc0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.github/workflows/publish-docker-image.yml
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.github/workflows/publish-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6376 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    12101 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/app.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/scripts/benchmark-json-api-response-size.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.940141 proxpi-1.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/src/proxpi/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/src/proxpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27997 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/src/proxpi/_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/src/proxpi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/src/proxpi/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/src/proxpi/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/src/proxpi/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/src/proxpi/templates/packages.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/src/proxpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2022-08-08 09:59:30.000000 proxpi-1.1.0b1/src/proxpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-08-08 09:59:30.000000 proxpi-1.1.0b1/src/proxpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 09:59:30.000000 proxpi-1.1.0b1/src/proxpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-08 09:59:30.000000 proxpi-1.1.0b1/src/proxpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-08 09:59:30.000000 proxpi-1.1.0b1/src/proxpi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 09:59:30.944141 proxpi-1.1.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17730 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-08-08 09:59:08.000000 proxpi-1.1.0b1/tests/test_pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.842234 proxpi-1.1.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/workflows/publish-docker-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/workflows/publish-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/app.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/scripts/benchmark-json-api-response-size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-13 01:12:19.854235 proxpi-1.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.838235 proxpi-1.1.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/src/proxpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27997 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/src/proxpi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/templates/packages.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/src/proxpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17730 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/test_pypi.py
```

### Comparing `proxpi-1.1.0b1/.github/workflows/publish-docker-image.yml` & `proxpi-1.1.0rc0/.github/workflows/publish-docker-image.yml`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   release:
     types: [created]
 
 jobs:
   release:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Build image
       run: docker buildx build . --tag "epicwink/proxpi:${{ github.ref_name }}"
     - name: Login to DockerHub
       run: >
         echo ${{ secrets.DOCKERHUB_PASSWORD }}
         | docker login --password-stdin -u epicwink
     - name: Publish image
```

### Comparing `proxpi-1.1.0b1/.github/workflows/publish-python-package.yml` & `proxpi-1.1.0rc0/.github/workflows/publish-python-package.yml`

 * *Files 21% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [created]
 
 jobs:
   release:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install build tools
       run: |
         pip install -U pip
         pip install build
     - name: Build package
```

### Comparing `proxpi-1.1.0b1/.github/workflows/test-python-package.yml` & `proxpi-1.1.0rc0/.github/workflows/test-python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -11,31 +11,35 @@
       - v*
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9, '3.10']
+        python-version: [3.7, 3.8, 3.9, '3.10', '3.11']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
     - name: Update pip
       run: pip install -U pip
     - name: Install package
       run: pip install .
     - name: Lint with black
       run: |
         pip install black
         black --check src/
     - name: Test with pytest
       run: |
         pip install -r tests/requirements.txt
-        pytest -vvra --cov proxpi --cov-report xml --cov-report term
+        pytest -vvra \
+          --cov proxpi \
+          --cov-report xml \
+          --cov-report term \
+          --cov-config setup.cfg
     - name: Upload coverage
       uses: codecov/codecov-action@v1
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `proxpi-1.1.0b1/Dockerfile` & `proxpi-1.1.0rc0/Dockerfile`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/LICENSE` & `proxpi-1.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/PKG-INFO` & `proxpi-1.1.0rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.1.0b1
+Version: 1.1.0rc0
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
@@ -49,14 +49,20 @@
 ```bash
 docker run -p 5000:5000 epicwink/proxpi
 ```
 
 Without arguments, runs with 2 threads. If passing arguments, make sure to bind to an
 exported address (or all with `0.0.0.0`) on port 5000 (ie `--bind 0.0.0.0:5000`).
 
+##### Compose
+Alternatively, use [Docker Compose](https://docs.docker.com/compose/)
+```bash
+docker compose up
+```
+
 #### Local
 ```bash
 FLASK_APP=proxpi.server flask run
 ```
 
 See `flask run --help` for more information on address and port binding, and certificate
 specification to use HTTPS. Alternatively, bring your own WSGI server.
```

### Comparing `proxpi-1.1.0b1/README.md` & `proxpi-1.1.0rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 ```bash
 docker run -p 5000:5000 epicwink/proxpi
 ```
 
 Without arguments, runs with 2 threads. If passing arguments, make sure to bind to an
 exported address (or all with `0.0.0.0`) on port 5000 (ie `--bind 0.0.0.0:5000`).
 
+##### Compose
+Alternatively, use [Docker Compose](https://docs.docker.com/compose/)
+```bash
+docker compose up
+```
+
 #### Local
 ```bash
 FLASK_APP=proxpi.server flask run
 ```
 
 See `flask run --help` for more information on address and port binding, and certificate
 specification to use HTTPS. Alternatively, bring your own WSGI server.
```

### Comparing `proxpi-1.1.0b1/app.requirements.txt` & `proxpi-1.1.0rc0/app.requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --generate-hashes --output-file=app.requirements.txt
+#    pip-compile --generate-hashes --output-file=app.requirements.txt --resolver=backtracking
 #
-certifi==2022.6.15 \
-    --hash=sha256:84c85a9078b11105f04f3036a9482ae10e4621616db313fe045dd24743a0820d \
-    --hash=sha256:fe86415d55e84719d75f8b69414f6438ac3547d2078ab91b67e779ef69378412
+certifi==2022.12.7 \
+    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
+    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
     # via requests
-charset-normalizer==2.1.0 \
-    --hash=sha256:5189b6f22b01957427f35b6a08d9a0bc45b46d3788ef5a92e978433c7a35f8a5 \
-    --hash=sha256:575e708016ff3a5e3681541cb9d79312c416835686d054a23accb873b254f413
+charset-normalizer==2.1.1 \
+    --hash=sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845 \
+    --hash=sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via flask
-flask==2.2.1 \
-    --hash=sha256:3c604c48c3d5b4c63e72134044c0b4fe90ff01ef65280b9fe2d38c8860d99fe5 \
-    --hash=sha256:9c2b81b9b1edcc835af72d600f1955e713a065e7cb41d7e51ee762b449d9c65d
+coloredlogs==15.0.1 \
+    --hash=sha256:612ee75c546f53e92e70049c9dbfcc18c935a2b9a53b66085ce9ef6a6e5c0934 \
+    --hash=sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0
+    # via proxpi (setup.py)
+flask==2.2.2 \
+    --hash=sha256:642c450d19c4ad482f96729bd2a8f6d32554aa1e231f4f6b4e7e5264b16cca2b \
+    --hash=sha256:b9c46cc36662a7949f34b52d8ec7bb59c0d74ba08ba6cb9ce9adc1d8676d9526
     # via proxpi (setup.py)
 gunicorn==20.1.0 \
     --hash=sha256:9dcc4547dbb1cb284accfb15ab5667a0e5d1881cc443e0677b4882a4067a807e \
     --hash=sha256:e0a968b5ba15f8a328fdfd7ab1fcb5af4470c28aaf7e55df02a99bc13138e6e8
     # via proxpi (setup.py)
-idna==3.3 \
-    --hash=sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff \
-    --hash=sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d
+humanfriendly==10.0 \
+    --hash=sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477 \
+    --hash=sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc
+    # via coloredlogs
+idna==3.4 \
+    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
+    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 itsdangerous==2.1.2 \
     --hash=sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44 \
     --hash=sha256:5dbbc68b317e5e42f327f9021763545dc3fc3bfe22e6deb96aaf1fc38874156a
     # via flask
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
@@ -154,19 +162,19 @@
     # via
     #   jinja2
     #   werkzeug
 requests==2.28.1 \
     --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
     --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
     # via proxpi (setup.py)
-urllib3==1.26.11 \
-    --hash=sha256:c33ccba33c819596124764c23a97d25f32b28433ba0dedeb77d873a38722c9bc \
-    --hash=sha256:ea6e8fb210b19d950fab93b60c9009226c63a28808bc8386e05301e25883ac0a
+urllib3==1.26.13 \
+    --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
+    --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
     # via requests
-werkzeug==2.2.1 \
-    --hash=sha256:4d7013ef96fd197d1cdeb03e066c6c5a491ccb44758a5b2b91137319383e5a5a \
-    --hash=sha256:7e1db6a5ba6b9a8be061e47e900456355b8714c0f238b0313f53afce1a55a79a
+werkzeug==2.2.2 \
+    --hash=sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f \
+    --hash=sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5
     # via flask
 
 # WARNING: The following packages were not pinned, but pip requires them to be
 # pinned when the requirements file includes hashes. Consider using the --allow-unsafe flag.
 # setuptools
```

### Comparing `proxpi-1.1.0b1/scripts/benchmark-json-api-response-size.py` & `proxpi-1.1.0rc0/scripts/benchmark-json-api-response-size.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/setup.cfg` & `proxpi-1.1.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/src/proxpi/_cache.py` & `proxpi-1.1.0rc0/src/proxpi/_cache.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/src/proxpi/server.py` & `proxpi-1.1.0rc0/src/proxpi/server.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/src/proxpi/templates/index.html` & `proxpi-1.1.0rc0/src/proxpi/templates/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/src/proxpi.egg-info/PKG-INFO` & `proxpi-1.1.0rc0/src/proxpi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.1.0b1
+Version: 1.1.0rc0
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
@@ -49,14 +49,20 @@
 ```bash
 docker run -p 5000:5000 epicwink/proxpi
 ```
 
 Without arguments, runs with 2 threads. If passing arguments, make sure to bind to an
 exported address (or all with `0.0.0.0`) on port 5000 (ie `--bind 0.0.0.0:5000`).
 
+##### Compose
+Alternatively, use [Docker Compose](https://docs.docker.com/compose/)
+```bash
+docker compose up
+```
+
 #### Local
 ```bash
 FLASK_APP=proxpi.server flask run
 ```
 
 See `flask run --help` for more information on address and port binding, and certificate
 specification to use HTTPS. Alternatively, bring your own WSGI server.
```

### Comparing `proxpi-1.1.0b1/src/proxpi.egg-info/SOURCES.txt` & `proxpi-1.1.0rc0/src/proxpi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 .dockerignore
 .gitignore
+CODE_OF_CONDUCT.md
 Dockerfile
 LICENSE
 README.md
+SECURITY.md
 app.requirements.txt
+docker-compose.yml
 pyproject.toml
 setup.cfg
 setup.py
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/publish-docker-image.yml
```

### Comparing `proxpi-1.1.0b1/tests/_utils.py` & `proxpi-1.1.0rc0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/tests/test_integration.py` & `proxpi-1.1.0rc0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0b1/tests/test_pypi.py` & `proxpi-1.1.0rc0/tests/test_pypi.py`

 * *Files identical despite different names*

