# Comparing `tmp/proxpi-1.1.0rc0.tar.gz` & `tmp/proxpi-1.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxpi-1.1.0rc0.tar", last modified: Tue Dec 13 01:12:19 2022, max compression
+gzip compressed data, was "proxpi-1.2.0a0.tar", last modified: Thu May 25 15:02:38 2023, max compression
```

## Comparing `proxpi-1.1.0rc0.tar` & `proxpi-1.2.0a0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.842234 proxpi-1.1.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/workflows/publish-docker-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/workflows/publish-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/app.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/scripts/benchmark-json-api-response-size.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-13 01:12:19.854235 proxpi-1.1.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.838235 proxpi-1.1.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.846234 proxpi-1.1.0rc0/src/proxpi/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27997 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/src/proxpi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/src/proxpi/templates/packages.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/src/proxpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-13 01:12:19.000000 proxpi-1.1.0rc0/src/proxpi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 01:12:19.850235 proxpi-1.1.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17730 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2022-12-13 01:12:04.000000 proxpi-1.1.0rc0/tests/test_pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/workflows/publish-docker-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/workflows/publish-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/app.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/scripts/benchmark-json-api-response-size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.552456 proxpi-1.2.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/src/proxpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28628 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/src/proxpi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/templates/packages.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/src/proxpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/test_pypi.py
```

### Comparing `proxpi-1.1.0rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/.github/workflows/publish-docker-image.yml` & `proxpi-1.2.0a0/.github/workflows/publish-docker-image.yml`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/.github/workflows/publish-python-package.yml` & `proxpi-1.2.0a0/.github/workflows/publish-python-package.yml`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/.github/workflows/test-python-package.yml` & `proxpi-1.2.0a0/.github/workflows/test-python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,10 @@
         pip install -r tests/requirements.txt
         pytest -vvra \
           --cov proxpi \
           --cov-report xml \
           --cov-report term \
           --cov-config setup.cfg
     - name: Upload coverage
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `proxpi-1.1.0rc0/CODE_OF_CONDUCT.md` & `proxpi-1.2.0a0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/Dockerfile` & `proxpi-1.2.0a0/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.10-alpine
+FROM python:3.11-alpine
 
 RUN --mount=source=.,target=/root/src/proxpi,rw \
     uname -a && cat /etc/issue && apk --version && python --version && pip --version \
  && apk --no-cache add git \
  && git -C /root/src/proxpi restore .dockerignore \
  && pip install --no-cache-dir --no-deps \
     --requirement /root/src/proxpi/app.requirements.txt \
```

### Comparing `proxpi-1.1.0rc0/LICENSE` & `proxpi-1.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/PKG-INFO` & `proxpi-1.2.0a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: proxpi
-Version: 1.1.0rc0
-Summary: PyPI caching mirror
-Home-page: https://github.com/EpicWink/proxpi
-Author: Laurie O
-Author-email: laurie_opperman@hotmail.com
-License: MIT
-Keywords: pypi,index,mirror,cache
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # proxpi
 [![Build status](
 https://github.com/EpicWink/proxpi/workflows/test/badge.svg?branch=master)](
 https://github.com/EpicWink/proxpi/actions?query=branch%3Amaster+workflow%3Atest)
 [![codecov](https://codecov.io/gh/EpicWink/proxpi/branch/master/graph/badge.svg)](
 https://codecov.io/gh/EpicWink/proxpi)
 
@@ -30,21 +11,15 @@
   * Cache the index (project list and projects' file list)
   * Cache the project files
 * Support multiple indices
 * Set index cache times-to-live (individually for each index)
 * Set files cache max-size on disk
 * Manually invalidate index cache
 
-## Installation
-If not using Docker
-```bash
-pip install proxpi
-```
-
-Install `coloredlogs` as well to get coloured logging
+See [Alternatives](#alternatives).
 
 ## Usage
 ### Start server
 #### Docker
 Uses a [Gunicorn](https://gunicorn.org/) WSGI server
 ```bash
 docker run -p 5000:5000 epicwink/proxpi
@@ -56,14 +31,22 @@
 ##### Compose
 Alternatively, use [Docker Compose](https://docs.docker.com/compose/)
 ```bash
 docker compose up
 ```
 
 #### Local
+##### Install
+```bash
+pip install proxpi
+```
+
+Install `coloredlogs` as well to get coloured logging
+
+##### Run server
 ```bash
 FLASK_APP=proxpi.server flask run
 ```
 
 See `flask run --help` for more information on address and port binding, and certificate
 specification to use HTTPS. Alternatively, bring your own WSGI server.
 
@@ -94,14 +77,18 @@
 * `PROXPI_CACHE_SIZE`: size of downloaded project files cache (bytes), default 5GB.
   Disable files-cache by setting this to 0
 * `PROXPI_CACHE_DIR`: downloaded project files cache directory path, default: a new
   temporary directory
 * `PROXPI_BINARY_FILE_MIME_TYPE=1`: force file-response content-type to
   `"application/octet-stream"` instead of letting Flask guess it. This may be needed
   if your package installer (eg Poetry) mishandles responses with declared encoding.
+* `PROXPI_DISABLE_INDEX_SSL_VERIFICATION=1`: don't verify any index SSL certificates
+* `PROXPI_DOWNLOAD_TIMEOUT`: time (in seconds) before `proxpi` will redirect to the
+  proxied index server for file downloads instead of waiting for the download,
+  default: 0.9
 
 ### Considerations with CI
 `proxpi` was designed with three goals (particularly for continuous integration (CI)):
 * to reduce load on PyPI package serving
 * to reduce `pip install` times
 * not require modification to the current workflow
 
@@ -182,7 +169,50 @@
    ```
 
 This is designed to not require any changes to the GitLab CI project configuration (ie
 `gitlab-ci.yml`), unless it already sets the index URL for some reason (if that's the
 case, you're probably already using a cache).
 
 Another option is to set up a proxy, but that's more effort than the above method.
+
+## Alternatives
+* [simpleindex](https://pypi.org/project/simpleindex/): routes URLs to multiple
+  indices (including PyPI), supports local (or S3 with a plygin) directory of packages,
+  no caching without custom plugins
+
+* [bandersnatch](https://pypi.org/project/bandersnatch/): mirrors one index (eg PyPI),
+  storing packages locally, or on S3 with a plugin. Manual update, no proxy
+
+* [devpi](https://pypi.org/project/devpi/): heavyweight, runs a full index (or multiple)
+  in addition to mirroring (in place of proxying), supports proxying (with inheritance),
+  supports package upload, server replication and fail-over
+
+* [pypiserver](https://pypi.org/project/pypiserver/): serves local directory of
+  packages, proxy to PyPI when not-found, supports package upload, no caching
+
+* [PyPI Cloud](https://pypi.org/project/pypicloud/): serves local or cloud-storage
+  directory of packages, with redirecting/cached proxying to indexes, authentication and
+  authorisation.
+
+* [`pypiprivate`](https://pypi.org/project/pypiprivate/): serves local (or S3-hosted)
+  directory of packages, no proxy to package indices (including PyPI)
+
+* [Pulp](https://pypi.org/project/pulpcore/): generic content repository, can host
+  multiple ecosystems' packages.
+  [Python package index plugin](https://pypi.org/project/pulp-python/) supports local/S3
+  mirrors, package upload, proxying to multiple indices, no caching
+
+* [`pip2pi`](https://pypi.org/project/pip2pi/): manual syncing of specific packages,
+  no proxy
+
+* [Flask-Pypi-Proxy](https://pypi.org/project/Flask-Pypi-Proxy/): unmaintained, no cache
+  size limit, no caching index pages
+
+* [`http.server`](https://docs.python.org/3/library/http.server.html): standard-library,
+  hosts directory exactly as laid out, no proxy to package indices (eg PyPI)
+
+* [Apache with `mod_rewrite`](
+  https://httpd.apache.org/docs/current/mod/mod_rewrite.html): I'm not familiar with
+  Apache, but it likely has the capability to proxy and cache (with eg `mod_cache_disk`)
+
+* [Gemfury](https://fury.co/l/pypi-server): hosted, managed. Private index is not free,
+  documentation doesn't say anything about proxying
```

### Comparing `proxpi-1.1.0rc0/scripts/benchmark-json-api-response-size.py` & `proxpi-1.2.0a0/scripts/benchmark-json-api-response-size.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/setup.cfg` & `proxpi-1.2.0a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/src/proxpi/_cache.py` & `proxpi-1.2.0a0/src/proxpi/_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 import dataclasses
 import typing as t
 import urllib.parse
 
 import requests
 import lxml.etree
 
-if t.TYPE_CHECKING:
-    import xml.etree.ElementTree
-
 INDEX_URL = os.environ.get("PROXPI_INDEX_URL", "https://pypi.org/simple/")
 EXTRA_INDEX_URLS = [
     s for s in os.environ.get("PROXPI_EXTRA_INDEX_URLS", "").strip().split(",") if s
 ]
+DISABLE_INDEX_SSL_VERIFICATION = os.environ.get(
+    "PROXPI_DISABLE_INDEX_SSL_VERIFICATION", ""
+) not in ("", "0", "no", "off", "false")
 
 INDEX_TTL = int(os.environ.get("PROXPI_INDEX_TTL", 1800))
 EXTRA_INDEX_TTLS = [
     int(s) for s in os.environ.get("PROXPI_EXTRA_INDEX_TTL", "").strip().split(",") if s
 ] or [180] * len(EXTRA_INDEX_URLS)
 
 CACHE_SIZE = int(os.environ.get("PROXPI_CACHE_SIZE", 5368709120))
 CACHE_DIR = os.environ.get("PROXPI_CACHE_DIR")
+DOWNLOAD_TIMEOUT = float(os.environ.get("PROXPI_DOWNLOAD_TIMEOUT", 0.9))
 
 logger = logging.getLogger(__name__)
 _name_normalise_re = re.compile("[-_.]+")
 _hostname_normalise_pattern = re.compile(r"[^a-z0-9]+")
 _html_parser = lxml.etree.HTMLParser()
 _time_offset = time.time()
 
@@ -115,15 +116,15 @@
     name: str
     url: str
     fragment: str
     attributes: t.Dict[str, str]
 
     @classmethod
     def from_html_element(
-        cls, el: "xml.etree.ElementTree.Element", request_url: str
+        cls, el: "lxml.etree.ElementBase", request_url: str
     ) -> "File":
         """Construct from HTML API response."""
         url = urllib.parse.urljoin(request_url, el.attrib["href"])
         return cls(
             name=el.text,
             url=url,
             fragment=urllib.parse.urlsplit(url).fragment,
@@ -574,26 +575,33 @@
     max_size: int
     cache_dir: str
     _cache_dir_provided: t.Union[str, None]
     _files: t.Dict[str, t.Union[_CachedFile, Thread]]
     _evict_lock: threading.Lock
 
     def __init__(
-        self, max_size: int, cache_dir: str = None, session: requests.Session = None
+        self,
+        max_size: int,
+        cache_dir: str = None,
+        download_timeout: float = 0.9,
+        session: requests.Session = None,
     ):
         """Initialise file-cache.
 
         Args:
             max_size: maximum file-cache size
             cache_dir: file-cache directory
+            download_timeout: file download timeout (seconds), falling back to
+                redirect
             session: index request session
         """
 
         self.max_size = max_size
         self.cache_dir = os.path.abspath(cache_dir or tempfile.mkdtemp())
+        self.download_timeout = download_timeout
         self.session = session or requests.Session()
         self._cache_dir_provided = cache_dir
         self._files = {}
         self._evict_lock = threading.Lock()
 
         self._populate_files_from_existing_cache_dir()
 
@@ -650,19 +658,25 @@
             for chunk in response.iter_content(None):
                 f.write(chunk)
         key = self._get_key(url)
         self._files[key] = _CachedFile(path, os.stat(path).st_size, 0)
         logger.debug(f"Finished downloading '{url_masked}'")
 
     def _wait_for_existing_download(self, url: str) -> bool:
-        """Wait 0.9s for existing download."""
+        """Wait for existing download, if any.
+
+        Returns:
+            whether the wait is given up (ie if time-out was reached or
+                exception was encountered)
+        """
+
         file = self._files.get(url)
         if isinstance(file, Thread):
             try:
-                file.join(0.9)
+                file.join(self.download_timeout)
             except Exception as e:
                 if file.exc and file == self._files[url]:
                     self._files.pop(url, None)
                 url_masked = _mask_password(url)
                 logger.error(f"Failed to download '{url_masked}'", exc_info=e)
                 return True
             if isinstance(self._files[url], Thread):
@@ -742,20 +756,23 @@
     _index_cache_cls = _IndexCache
     _file_cache_cls = _FileCache
 
     @classmethod
     def from_config(cls):
         """Create cache from configuration."""
         session = requests.Session()
+        session.verify = not DISABLE_INDEX_SSL_VERIFICATION
         proxpi_version = get_proxpi_version()
         if proxpi_version:
             session.headers["User-Agent"] = f"proxpi/{proxpi_version}"
 
         root_cache = cls._index_cache_cls(INDEX_URL, INDEX_TTL, session)
-        file_cache = cls._file_cache_cls(CACHE_SIZE, CACHE_DIR, session)
+        file_cache = cls._file_cache_cls(
+            CACHE_SIZE, CACHE_DIR, DOWNLOAD_TIMEOUT, session
+        )
         if len(EXTRA_INDEX_URLS) != len(EXTRA_INDEX_TTLS):
             raise RuntimeError(
                 f"Number of extra index URLs doesn't equal number of extra index "
                 f"times-to-live: {len(EXTRA_INDEX_URLS)} != {len(EXTRA_INDEX_TTLS)}"
             )
         extra_caches = [
             cls._index_cache_cls(url, ttl, session)
```

### Comparing `proxpi-1.1.0rc0/src/proxpi/server.py` & `proxpi-1.2.0a0/src/proxpi/server.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/src/proxpi/templates/index.html` & `proxpi-1.2.0a0/src/proxpi/templates/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/src/proxpi.egg-info/PKG-INFO` & `proxpi-1.2.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.1.0rc0
+Version: 1.2.0a0
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
@@ -30,21 +30,15 @@
   * Cache the index (project list and projects' file list)
   * Cache the project files
 * Support multiple indices
 * Set index cache times-to-live (individually for each index)
 * Set files cache max-size on disk
 * Manually invalidate index cache
 
-## Installation
-If not using Docker
-```bash
-pip install proxpi
-```
-
-Install `coloredlogs` as well to get coloured logging
+See [Alternatives](#alternatives).
 
 ## Usage
 ### Start server
 #### Docker
 Uses a [Gunicorn](https://gunicorn.org/) WSGI server
 ```bash
 docker run -p 5000:5000 epicwink/proxpi
@@ -56,14 +50,22 @@
 ##### Compose
 Alternatively, use [Docker Compose](https://docs.docker.com/compose/)
 ```bash
 docker compose up
 ```
 
 #### Local
+##### Install
+```bash
+pip install proxpi
+```
+
+Install `coloredlogs` as well to get coloured logging
+
+##### Run server
 ```bash
 FLASK_APP=proxpi.server flask run
 ```
 
 See `flask run --help` for more information on address and port binding, and certificate
 specification to use HTTPS. Alternatively, bring your own WSGI server.
 
@@ -94,14 +96,18 @@
 * `PROXPI_CACHE_SIZE`: size of downloaded project files cache (bytes), default 5GB.
   Disable files-cache by setting this to 0
 * `PROXPI_CACHE_DIR`: downloaded project files cache directory path, default: a new
   temporary directory
 * `PROXPI_BINARY_FILE_MIME_TYPE=1`: force file-response content-type to
   `"application/octet-stream"` instead of letting Flask guess it. This may be needed
   if your package installer (eg Poetry) mishandles responses with declared encoding.
+* `PROXPI_DISABLE_INDEX_SSL_VERIFICATION=1`: don't verify any index SSL certificates
+* `PROXPI_DOWNLOAD_TIMEOUT`: time (in seconds) before `proxpi` will redirect to the
+  proxied index server for file downloads instead of waiting for the download,
+  default: 0.9
 
 ### Considerations with CI
 `proxpi` was designed with three goals (particularly for continuous integration (CI)):
 * to reduce load on PyPI package serving
 * to reduce `pip install` times
 * not require modification to the current workflow
 
@@ -182,7 +188,50 @@
    ```
 
 This is designed to not require any changes to the GitLab CI project configuration (ie
 `gitlab-ci.yml`), unless it already sets the index URL for some reason (if that's the
 case, you're probably already using a cache).
 
 Another option is to set up a proxy, but that's more effort than the above method.
+
+## Alternatives
+* [simpleindex](https://pypi.org/project/simpleindex/): routes URLs to multiple
+  indices (including PyPI), supports local (or S3 with a plygin) directory of packages,
+  no caching without custom plugins
+
+* [bandersnatch](https://pypi.org/project/bandersnatch/): mirrors one index (eg PyPI),
+  storing packages locally, or on S3 with a plugin. Manual update, no proxy
+
+* [devpi](https://pypi.org/project/devpi/): heavyweight, runs a full index (or multiple)
+  in addition to mirroring (in place of proxying), supports proxying (with inheritance),
+  supports package upload, server replication and fail-over
+
+* [pypiserver](https://pypi.org/project/pypiserver/): serves local directory of
+  packages, proxy to PyPI when not-found, supports package upload, no caching
+
+* [PyPI Cloud](https://pypi.org/project/pypicloud/): serves local or cloud-storage
+  directory of packages, with redirecting/cached proxying to indexes, authentication and
+  authorisation.
+
+* [`pypiprivate`](https://pypi.org/project/pypiprivate/): serves local (or S3-hosted)
+  directory of packages, no proxy to package indices (including PyPI)
+
+* [Pulp](https://pypi.org/project/pulpcore/): generic content repository, can host
+  multiple ecosystems' packages.
+  [Python package index plugin](https://pypi.org/project/pulp-python/) supports local/S3
+  mirrors, package upload, proxying to multiple indices, no caching
+
+* [`pip2pi`](https://pypi.org/project/pip2pi/): manual syncing of specific packages,
+  no proxy
+
+* [Flask-Pypi-Proxy](https://pypi.org/project/Flask-Pypi-Proxy/): unmaintained, no cache
+  size limit, no caching index pages
+
+* [`http.server`](https://docs.python.org/3/library/http.server.html): standard-library,
+  hosts directory exactly as laid out, no proxy to package indices (eg PyPI)
+
+* [Apache with `mod_rewrite`](
+  https://httpd.apache.org/docs/current/mod/mod_rewrite.html): I'm not familiar with
+  Apache, but it likely has the capability to proxy and cache (with eg `mod_cache_disk`)
+
+* [Gemfury](https://fury.co/l/pypi-server): hosted, managed. Private index is not free,
+  documentation doesn't say anything about proxying
```

### Comparing `proxpi-1.1.0rc0/src/proxpi.egg-info/SOURCES.txt` & `proxpi-1.2.0a0/src/proxpi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .dockerignore
 .gitignore
 CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 Dockerfile
 LICENSE
 README.md
 SECURITY.md
 app.requirements.txt
 docker-compose.yml
 pyproject.toml
```

### Comparing `proxpi-1.1.0rc0/tests/_utils.py` & `proxpi-1.2.0a0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.1.0rc0/tests/test_integration.py` & `proxpi-1.2.0a0/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,17 +219,28 @@
         "extra_caches",
         [proxpi.server.cache._index_cache_cls(f"{mock_extra_index}/", 10, session)],
     )
     with root_patch, extras_patch:
         yield from _utils.make_server(proxpi_server.app)
 
 
+@pytest.fixture
+def clear_index_cache(server):
+    proxpi.server.cache.invalidate_list()
+
+
+@pytest.fixture
+def clear_projects_cache(server):
+    for project_name in proxpi.server.cache.list_projects():
+        proxpi.server.cache.invalidate_project(project_name)
+
+
 @pytest.mark.parametrize("accept", ["text/html", "application/vnd.pypi.simple.v1+html"])
 @pytest.mark.parametrize("index_json_response", [False, True])
-def test_list(server, accept, index_json_response):
+def test_list(server, accept, index_json_response, clear_index_cache):
     """Test getting package list."""
     with set_mock_index_response_is_json(index_json_response):
         response = requests.get(f"{server}/index/", headers={"Accept": accept})
     response.raise_for_status()
 
     assert response.headers["Content-Type"][:9] == "text/html"
     assert any(
@@ -251,15 +262,17 @@
 
 
 @pytest.mark.parametrize("accept", [
     "application/vnd.pypi.simple.v1+json",
     "application/vnd.pypi.simple.latest+json",
 ])
 @pytest.mark.parametrize("index_json_response", [False, True])
-def test_list_json(server, accept, index_json_response):
+def test_list_json(
+    server, accept, index_json_response, mock_root_index, clear_index_cache
+):
     """Test getting package list with JSON API."""
     with set_mock_index_response_is_json(index_json_response):
         response = requests.get(f"{server}/index/", headers={"Accept": accept})
     assert response.status_code == 200
     assert response.headers["Content-Type"][:35] == (
         "application/vnd.pypi.simple.v1+json"
     )
@@ -271,15 +284,15 @@
 
 
 @pytest.mark.parametrize("project", ["proxpi", "numpy", "scipy"])
 @pytest.mark.parametrize("accept", [
     "text/html", "application/vnd.pypi.simple.v1+html", "*/*"
 ])
 @pytest.mark.parametrize("index_json_response", [False, True, "yanked"])
-def test_package(server, project, accept, index_json_response):
+def test_package(server, project, accept, index_json_response, clear_projects_cache):
     """Test getting package files."""
     project_url = f"{server}/index/{project}/"
     with set_mock_index_response_is_json(index_json_response):
         response = requests.get(project_url, headers={"Accept": accept})
     response.raise_for_status()
 
     assert response.headers["Content-Type"][:9] == "text/html"
@@ -350,15 +363,17 @@
 @pytest.mark.parametrize("project", ["proxpi", "numpy", "scipy"])
 @pytest.mark.parametrize("accept", [
     "application/vnd.pypi.simple.v1+json",
     "application/vnd.pypi.simple.latest+json",
 ])
 @pytest.mark.parametrize("query_format", [False, True])
 @pytest.mark.parametrize("index_json_response", [False, True, "yanked"])
-def test_package_json(server, project, accept, query_format, index_json_response):
+def test_package_json(
+    server, project, accept, query_format, index_json_response, clear_projects_cache
+):
     """Test getting package files with JSON API."""
     params = None
     headers = None
     if query_format:
         params = {"format": accept}
     else:
         headers = {"Accept": accept}
```

### Comparing `proxpi-1.1.0rc0/tests/test_pypi.py` & `proxpi-1.2.0a0/tests/test_pypi.py`

 * *Files identical despite different names*

