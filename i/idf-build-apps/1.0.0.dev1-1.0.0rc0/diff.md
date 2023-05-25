# Comparing `tmp/idf_build_apps-1.0.0.dev1.tar.gz` & `tmp/idf_build_apps-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.0.dev1.tar` & `idf_build_apps-1.0.0rc0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      351 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.editorconfig
--rw-r--r--   0        0        0      123 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.gitattributes
--rw-r--r--   0        0        0      253 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3707 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.gitignore
--rw-r--r--   0        0        0     1077 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.readthedocs.yml
--rw-r--r--   0        0        0     4754 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/CHANGELOG.md
--rw-r--r--   0        0        0     1834 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/LICENSE
--rw-r--r--   0        0        0     3843 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/README.md
--rw-r--r--   0        0        0       33 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/config_file.md
--rw-r--r--   0        0        0    10368 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/index.rst
--rw-r--r--   0        0        0     3651 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/manifest.md
--rw-r--r--   0        0        0      486 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    26619 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/config.py
--rw-r--r--   0        0        0     2187 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6087 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/log.py
--rw-r--r--   0        0        0    32327 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6144 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5956 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     6577 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/license_header.txt
--rw-r--r--   0        0        0     1874 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/conftest.py
--rw-r--r--   0        0        0     2864 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_build.py
--rw-r--r--   0        0        0    14263 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_manifest.py
--rw-r--r--   0        0        0     2394 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_utils.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev1/setup.py
--rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.editorconfig
+-rw-r--r--   0        0        0      123 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.gitattributes
+-rw-r--r--   0        0        0      253 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3685 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.readthedocs.yml
+-rw-r--r--   0        0        0     5128 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1834 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     3843 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/README.md
+-rw-r--r--   0        0        0       33 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/config_file.md
+-rw-r--r--   0        0        0    10368 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/index.rst
+-rw-r--r--   0        0        0     5648 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/manifest.md
+-rw-r--r--   0        0        0      485 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    26619 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2187 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6087 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30651 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6321 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5956 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     6577 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/license_header.txt
+-rw-r--r--   0        0        0     1874 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_build.py
+-rw-r--r--   0        0        0    16010 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_finder.py
+-rw-r--r--   0        0        0      995 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_manifest.py
+-rw-r--r--   0        0        0     2394 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0rc0/setup.py
+-rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0rc0/PKG-INFO
```

### Comparing `idf_build_apps-1.0.0.dev1/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.0rc0/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.0rc0/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.0rc0/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.0rc0/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.0rc0/.github/workflows/test-build-idf-apps.yml`

 * *Files 6% similar despite different names*

```diff
@@ -62,17 +62,18 @@
           rm $(which python3)
           bash $IDF_PATH/install.sh
           . $IDF_PATH/export.sh
           pip install idf_build_apps-*-py2.py3-none-any.whl
           python -m idf_build_apps build -vv -t esp32 \
             -p $IDF_PATH/examples/get-started/hello_world \
             --size-file size_info.json \
-            --ignore-warning-str "Python 3 versions older than 3.6 are not supported" \
-            --ignore-warning-str "Python 2 is no longer supported" \
-            --ignore-warning-str "Support for Python 2 is deprecated"
+            --ignore-warning-str \
+              "Python 3 versions older than 3.6 are not supported" \
+              "Python 2 is no longer supported" \
+              "Support for Python 2 is deprecated"
 
   build-apps-on-idf-env:
     if: ${{ github.ref == 'refs/heads/main' }}
     needs: build-python-packages
     strategy:
       matrix:
         idf-branch: [ release-v4.3, release-v4.4, release-v5.0]
```

### Comparing `idf_build_apps-1.0.0.dev1/.gitignore` & `idf_build_apps-1.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/.pre-commit-config.yaml` & `idf_build_apps-1.0.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/CHANGELOG.md` & `idf_build_apps-1.0.0rc0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased - 1.0.0]
 
 ## Added
 
 - Support keyword `depends_filepatterns` in the manifest file
+- Support expanding environment variables in the manifest files
 
 ## BREAKING CHANGES
 
 - Attributes Renamed
   - `App.requires_components` renamed to `App.depends_components`
   - `FolderRule.requires_components` renamed to `FolderRule.depends_components`
 - Functions Renamed
@@ -19,14 +20,21 @@
   - `App.build()`
   - `App.is_modified()`
   - `find_apps()`
   - `build_apps()`
 - CLI Options Renamed
   - `--depends-on-components` renamed to `--modified-components`
   - `--depends-on-files` renamed to `--modified-files`
+  - `--ignore-components-dependencies-file-patterns` renamed to `--ignore-app-dependencies-filepatterns`
+- Removed the deprecated CLI call methods, now these options only support space-separated list
+  - `--exclude`
+  - `--config`
+  - `--manifest-file`
+  - `--ignore-warning-str`
+  - `--default-build-targets`
 
 ## [0.6.1] (2023-05-10)
 
 ### Fixed
 
 - Add missing dependency `pyyaml`. It's wrongly removed in 0.6.0.
```

### Comparing `idf_build_apps-1.0.0.dev1/CONTRIBUTING.md` & `idf_build_apps-1.0.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/LICENSE` & `idf_build_apps-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/README.md` & `idf_build_apps-1.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/docs/Makefile` & `idf_build_apps-1.0.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.0rc0/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.0rc0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/docs/conf.py` & `idf_build_apps-1.0.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/docs/config_file.md` & `idf_build_apps-1.0.0rc0/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/docs/find_build.md` & `idf_build_apps-1.0.0rc0/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/app.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/app.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/config.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/constants.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/finder.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/log.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/main.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
-import io
 import json
 import os
 import re
 import shutil
 import sys
 import textwrap
-import warnings
 from pathlib import (
     Path,
 )
 
 from . import (
     LOGGER,
 )
@@ -51,30 +49,30 @@
     pass
 
 
 def _check_app_dependency(
     manifest_rootpath,  # type: str
     modified_components,  # type: list[str] | None
     modified_files,  # type: list[str] | None
-    ignore_component_dependencies_file_patterns,  # type: list[str] | None
+    ignore_app_dependencies_filepatterns,  # type: list[str] | None
 ):  # type: (...) -> bool
     # not check since modified_components and modified_files are not passed
     if modified_components is None and modified_files is None:
         return False
 
-    # not check since ignore_component_dependencies_file_patterns is passed and matched
+    # not check since ignore_app_dependencies_filepatterns is passed and matched
     if (
-        ignore_component_dependencies_file_patterns
+        ignore_app_dependencies_filepatterns
         and modified_files is not None
-        and files_matches_patterns(modified_files, ignore_component_dependencies_file_patterns, manifest_rootpath)
+        and files_matches_patterns(modified_files, ignore_app_dependencies_filepatterns, manifest_rootpath)
     ):
         LOGGER.debug(
             'Skipping check component dependencies for apps since files %s matches patterns: %s',
             ', '.join(modified_files),
-            ', '.join(ignore_component_dependencies_file_patterns),
+            ', '.join(ignore_app_dependencies_filepatterns),
         )
         return False
 
     return True
 
 
 def find_apps(
@@ -91,15 +89,15 @@
     check_warnings=False,  # type: bool
     preserve=True,  # type: bool
     manifest_rootpath=None,  # type: str | None
     manifest_files=None,  # type: list[str] | str | None
     default_build_targets=None,  # type: list[str] | str | None
     modified_components=None,  # type: list[str] | str | None
     modified_files=None,  # type: list[str] | str | None
-    ignore_component_dependencies_file_patterns=None,  # type: list[str] | str | None
+    ignore_app_dependencies_filepatterns=None,  # type: list[str] | str | None
     sdkconfig_defaults=None,  # type: str | None
 ):  # type: (...) -> list[App]
     """
     Find app directories in paths (possibly recursively), which contain apps for the given build system, compatible
     with the given target
 
     :param paths: list of app directories (can be / usually will be a relative path)
@@ -135,17 +133,17 @@
     :type manifest_files: list[str] | str | None
     :param default_build_targets: default build targets used in manifest files
     :type default_build_targets: list[str] | str | None
     :param modified_components: modified components
     :type modified_components: list[str] | str | None
     :param modified_files: modified files
     :type modified_files: list[str] | str | None
-    :param ignore_component_dependencies_file_patterns: file patterns that used for ignoring checking the component
+    :param ignore_app_dependencies_filepatterns: file patterns that used for ignoring checking the component
         dependencies
-    :type ignore_component_dependencies_file_patterns: list[str] | str | None
+    :type ignore_app_dependencies_filepatterns: list[str] | str | None
     :param sdkconfig_defaults: semicolon-separated string, pass to idf.py -DSDKCONFIG_DEFAULTS if specified,
         also could be set via environment variables "SDKCONFIG_DEFAULTS"
     :type sdkconfig_defaults: str | None
     :return: list of found apps
     :rtype: list[App]
     """
     if default_build_targets:
@@ -162,15 +160,15 @@
             LOGGER.debug('Loading manifest file: %s', _manifest_file)
             rules.update(Manifest.from_file(_manifest_file).rules)
         manifest = Manifest(rules)
         App.MANIFEST = manifest
 
     modified_components = to_list(modified_components)
     modified_files = to_list(modified_files)
-    ignore_component_dependencies_file_patterns = to_list(ignore_component_dependencies_file_patterns)
+    ignore_app_dependencies_filepatterns = to_list(ignore_app_dependencies_filepatterns)
 
     apps = []
     if target == 'all':
         targets = ALL_TARGETS
     else:
         targets = [target]
 
@@ -191,15 +189,15 @@
                     check_warnings=check_warnings,
                     preserve=preserve,
                     manifest_rootpath=manifest_rootpath,
                     check_app_dependencies=_check_app_dependency(
                         manifest_rootpath=manifest_rootpath,
                         modified_components=modified_components,
                         modified_files=modified_files,
-                        ignore_component_dependencies_file_patterns=ignore_component_dependencies_file_patterns,
+                        ignore_app_dependencies_filepatterns=ignore_app_dependencies_filepatterns,
                     ),
                     modified_components=modified_components,
                     modified_files=modified_files,
                     sdkconfig_defaults_str=sdkconfig_defaults,
                 )
             )
     apps.sort()
@@ -219,15 +217,15 @@
     collect_app_info=None,  # type: str | t.TextIO | None
     ignore_warning_strs=None,  # type: list[str] | None
     ignore_warning_file=None,  # type: t.TextIO | None
     copy_sdkconfig=False,  # type: bool
     manifest_rootpath=None,  # type: str | None
     modified_components=None,  # type: list[str] | str | None
     modified_files=None,  # type: list[str] | str | None
-    ignore_component_dependencies_file_patterns=None,  # type: list[str] | str | None
+    ignore_app_dependencies_filepatterns=None,  # type: list[str] | str | None
 ):  # type: (...) -> (int, list[App]) | int
     """
     Build all the specified apps
 
     :param apps: list of apps to be built
     :type apps: list[App] | App
     :param build_verbose: call ``--verbose`` in ``idf.py build`` or not
@@ -254,26 +252,26 @@
     :param manifest_rootpath: The root path of the manifest files. Usually the folders specified in the manifest files
         are relative paths. Use the current directory if not specified
     :type manifest_rootpath: str | None
     :param modified_components: modified components
     :type modified_components: list[str] | str | None
     :param modified_files: modified files
     :type modified_files: list[str] | str | None
-    :param ignore_component_dependencies_file_patterns: file patterns that used for ignoring checking the component
+    :param ignore_app_dependencies_filepatterns: file patterns that used for ignoring checking the component
         dependencies
-    :type ignore_component_dependencies_file_patterns: list[str] | str | None
+    :type ignore_app_dependencies_filepatterns: list[str] | str | None
     :return: (exit_code, built_apps) if specified ``modified_components``
     :rtype: int, list[App]
     :return: exit_code if not specified ``modified_components``
     :rtype: int
     """
     apps = to_list(apps)  # type: list[App]
     modified_components = to_list(modified_components)
     modified_files = to_list(modified_files)
-    ignore_component_dependencies_file_patterns = to_list(ignore_component_dependencies_file_patterns)
+    ignore_app_dependencies_filepatterns = to_list(ignore_app_dependencies_filepatterns)
 
     ignore_warnings_regexes = []
     if ignore_warning_strs:
         for s in ignore_warning_strs:
             ignore_warnings_regexes.append(re.compile(s))
     if ignore_warning_file:
         for s in ignore_warning_file:
@@ -296,35 +294,21 @@
     # cleanup collect files if exists at this early-stage
     collect_files = []
     for app in apps[start - 1 : stop]:  # we use 1-based
         app.parallel_index = parallel_index
         app.parallel_count = parallel_count
 
         if collect_app_info:
-            if isinstance(collect_app_info, io.TextIOWrapper):
-                warnings.warn(
-                    '"collect_app_info" does not support file stream in idf-build-apps 1.0.0, Please use str instead',
-                    DeprecationWarning,
-                )
-                app._collect_app_info = collect_app_info.name
-            else:
-                app._collect_app_info = collect_app_info
+            app._collect_app_info = collect_app_info
 
             if app.collect_app_info not in collect_files:
                 collect_files.append(app.collect_app_info)
 
         if collect_size_info:
-            if isinstance(collect_size_info, io.TextIOWrapper):
-                warnings.warn(
-                    '"collect_size_info" does not support file stream in idf-build-apps 1.0.0, Please use str instead',
-                    DeprecationWarning,
-                )
-                app._collect_size_info = collect_size_info.name
-            else:
-                app._collect_size_info = collect_size_info
+            app._collect_size_info = collect_size_info
 
             if app.collect_size_info not in collect_files:
                 collect_files.append(app.collect_size_info)
 
     for f in collect_files:
         if os.path.isfile(f):
             os.remove(f)
@@ -348,15 +332,15 @@
         is_built = False
         try:
             is_built = app.build(
                 manifest_rootpath=manifest_rootpath,
                 modified_components=modified_components,
                 modified_files=modified_files,
                 check_app_dependencies=_check_app_dependency(
-                    manifest_rootpath, modified_components, modified_files, ignore_component_dependencies_file_patterns
+                    manifest_rootpath, modified_components, modified_files, ignore_app_dependencies_filepatterns
                 ),
             )
         except BuildError as e:
             LOGGER.error(str(e))
             if keep_going:
                 failed_apps.append(app)
                 exit_code = 1
@@ -464,23 +448,15 @@
 
         if action.default is not argparse.SUPPRESS:
             if action.default is None:
                 default_type = str
             else:
                 default_type = type(action.default)
 
-            if isinstance(action, argparse._AppendAction):  # noqa
-                _help += (
-                    '. Could be specified for multiple times'
-                    '{} ! DeprecationWarning: will change to space-separated list in idf-build-apps 1.0.0 version'.format(
-                        self.LINE_SEP
-                    )
-                )
-                _type = 'list[{}]'.format(default_type.__name__)
-            elif action.nargs in [argparse.ZERO_OR_MORE, argparse.ONE_OR_MORE]:
+            if action.nargs in [argparse.ZERO_OR_MORE, argparse.ONE_OR_MORE]:
                 _type = 'list[{}]'.format(default_type.__name__)
             else:
                 _type = default_type.__name__
 
             defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
             if action.option_strings or action.nargs in defaulting_nargs:
                 _help += '{} - default: %(default)s'.format(self.LINE_SEP)
@@ -520,15 +496,15 @@
     common_args.add_argument(
         '--recursive',
         action='store_true',
         help='Look for apps in the specified paths recursively',
     )
     common_args.add_argument(
         '--exclude',
-        action='append',
+        nargs='+',
         help='Ignore specified directory (if --recursive is given)',
     )
     common_args.add_argument(
         '--work-dir',
         help='If set, the app is first copied into the specified directory, and then built. '
         'If not set, the work directory is the directory of the app. Can expand placeholders',
     )
@@ -544,15 +520,15 @@
     )
     common_args.add_argument(
         '--size-file',
         help='Relative to build dir. The size json will be written to this file if specified. Can expand placeholders',
     )
     common_args.add_argument(
         '--config',
-        action='append',
+        nargs='+',
         help='Adds configurations (sdkconfig file names) to build. '
         'This can either be FILENAME[=NAME] or FILEPATTERN. FILENAME is the name of the sdkconfig file, '
         'relative to the project directory, to be used. Optional NAME can be specified, '
         'which can be used as a name of this configuration. FILEPATTERN is the name of '
         'the sdkconfig file, relative to the project directory, with at most one wildcard. '
         'The part captured by the wildcard is used as the name of the configuration',
     )
@@ -574,30 +550,27 @@
         help='Write the log to the specified file, instead of stderr',
     )
     common_args.add_argument(
         '--check-warnings', action='store_true', help='If set, fail the build if warnings are found'
     )
     common_args.add_argument(
         '--manifest-file',
-        action='append',
+        nargs='+',
         help='Manifest files which specify the build test rules of the apps',
     )
     common_args.add_argument(
         '--manifest-rootpath',
         help='Root directory for calculating the realpath of the relative path defined in the manifest files. '
         'Would use the current directory if not set',
     )
     common_args.add_argument(
         '--default-build-targets',
         nargs='+',
         help='space-separated list of supported targets. Targets supported in current ESP-IDF branch '
-        '(except preview ones) would be used if this option is not set.'
-        '{} ! DeprecationWarning: comma-separated list support will be removed in idf-build-apps 1.0.0 version'.format(
-            IdfBuildAppsCliFormatter.LINE_SEP
-        ),
+        '(except preview ones) would be used if this option is not set.',
     )
     common_args.add_argument(
         '--modified-components',
         nargs='*',
         default=None,
         help='space-separated list which specifies the modified components. app with `depends_components` set in the '
         'corresponding manifest files would only be built if depends on any of the specified components.',
@@ -608,15 +581,15 @@
         default=None,
         help='space-separated list which specifies the modified files. app with `depends_filepatterns` set in the '
         'corresponding manifest files would only be built if any of the specified file pattern matches any of the '
         'specified modified files.',
     )
     common_args.add_argument(
         '-if',
-        '--ignore-component-dependencies-file-patterns',
+        '--ignore-app-dependencies-filepatterns',
         nargs='*',
         default=None,
         help='space-separated list which specifies the file patterns used for ignoring the component dependencies. '
         'The `depends_components` and `depends_filepatterns` set in the manifest files will be ignored when any of '
         'the specified file patterns matches any of the modified files. Must be used together with '
         '--modified-files',
     )
@@ -671,15 +644,15 @@
     )
     build_parser.add_argument(
         '--collect-app-info',
         help='write app info json file while building into the specified file. each line is a json object. Can expand placeholders',
     )
     build_parser.add_argument(
         '--ignore-warning-str',
-        action='append',
+        nargs='+',
         help='Ignore the warning string that match the specified regex in the build output',
     )
     build_parser.add_argument(
         '--ignore-warning-file',
         type=argparse.FileType('r'),
         help='Ignore the warning strings in the specified file. Each line should be a regex string',
     )
@@ -708,28 +681,25 @@
             'Must specify current build target with CLI option "-t <target>" or "--target <target>". '
             '(choices: [{}]'.format(','.join(ALL_TARGETS + ['all']))
         )
 
     default_build_targets = []
     if args.default_build_targets:
         for target in args.default_build_targets:
-            t_list = [_t.strip() for _t in target.split(',')] if ',' in target else [target.strip()]
-            for _t in t_list:
-                if _t not in ALL_TARGETS:
-                    raise InvalidCommand(
-                        'Unrecognizable target {} specified with "--default-build-targets". '
-                        'Current ESP-IDF available targets: {}'.format(_t, ALL_TARGETS)
-                    )
-
-                if _t not in default_build_targets:
-                    default_build_targets.append(_t)
+            if target not in ALL_TARGETS:
+                raise InvalidCommand(
+                    'Unrecognizable target {} specified with "--default-build-targets". '
+                    'Current ESP-IDF available targets: {}'.format(target, ALL_TARGETS)
+                )
 
+            if target not in default_build_targets:
+                default_build_targets.append(target)
     args.default_build_targets = default_build_targets
 
-    if args.ignore_component_dependencies_file_patterns:
+    if args.ignore_app_dependencies_filepatterns:
         if args.modified_files is None:
             raise InvalidCommand(
                 'Must specify "--ignore-component-dependencies-file-patterns" with "--modified-files", '
             )
 
 
 def apply_config_args(args):  # type: (argparse.Namespace) -> None
@@ -763,15 +733,15 @@
         size_json_path=args.size_file,
         check_warnings=args.check_warnings,
         manifest_rootpath=args.manifest_rootpath,
         manifest_files=args.manifest_file,
         default_build_targets=args.default_build_targets,
         modified_components=args.modified_components,
         modified_files=args.modified_files,
-        ignore_component_dependencies_file_patterns=args.ignore_component_dependencies_file_patterns,
+        ignore_app_dependencies_filepatterns=args.ignore_app_dependencies_filepatterns,
         sdkconfig_defaults=args.sdkconfig_defaults,
     )
 
     if args.action == 'find':
         if args.output:
             with open(args.output, 'w') as f:
                 for app in apps:
@@ -797,14 +767,14 @@
         collect_app_info=args.collect_app_info,
         ignore_warning_strs=args.ignore_warning_str,
         ignore_warning_file=args.ignore_warning_file,
         copy_sdkconfig=args.copy_sdkconfig,
         manifest_rootpath=args.manifest_rootpath,
         modified_components=args.modified_components,
         modified_files=args.modified_files,
-        ignore_component_dependencies_file_patterns=args.ignore_component_dependencies_file_patterns,
+        ignore_app_dependencies_filepatterns=args.ignore_app_dependencies_filepatterns,
     )
 
     if args.modified_components is not None:
         sys.exit(res[0])
     else:
         sys.exit(res)
```

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/manifest/if_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
+import os
 from ast import (
     literal_eval,
 )
 
 from pyparsing import (
     Keyword,
     Literal,
@@ -82,14 +83,18 @@
 
         if self.attr == 'CONFIG_NAME':
             return config_name
 
         if self.attr in SOC_HEADERS[target]:
             return SOC_HEADERS[target][self.attr]
 
+        # for non-keyword cap words, check if it is defined in the environment variables
+        if self.attr in os.environ:
+            return os.environ[self.attr]
+
         return 0  # default return 0 as false
 
 
 class Integer(Stmt):
     def __init__(self, t):
         self.expr = t[0]
```

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/idf_build_apps/utils.py` & `idf_build_apps-1.0.0rc0/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/pyproject.toml` & `idf_build_apps-1.0.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/tests/conftest.py` & `idf_build_apps-1.0.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/tests/test_build.py` & `idf_build_apps-1.0.0rc0/tests/test_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import shutil
 
 import pytest
 
+from idf_build_apps import (
+    find_apps,
+)
 from idf_build_apps.app import (
     CMakeApp,
 )
 from idf_build_apps.constants import (
     IDF_PATH,
 )
 
@@ -70,14 +73,28 @@
             modified_components=[],
             modified_files=modified_files,
             check_app_dependencies=True,
         )
 
         assert built == is_built
 
+    def test_build_without_modified_components_but_ignored_app_dependency_check(self):
+        test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
+
+        apps = find_apps(
+            test_dir,
+            'esp32',
+            modified_components=[],
+            modified_files=['foo.c'],
+            ignore_app_dependencies_filepatterns=['foo.c'],
+        )
+
+        for app in apps:
+            assert app.build()
+
 
 @pytest.mark.skipif(not shutil.which('idf.py'), reason='idf.py not found')
 def test_idf_version_keywords_type():
     from idf_build_apps.constants import (
         IDF_VERSION_MAJOR,
         IDF_VERSION_MINOR,
         IDF_VERSION_PATCH,
```

### Comparing `idf_build_apps-1.0.0.dev1/tests/test_finder.py` & `idf_build_apps-1.0.0rc0/tests/test_finder.py`

 * *Files 18% similar despite different names*

```diff
@@ -413,7 +413,59 @@
         apps = find_apps(
             str(tmp_path / 'test1'), 'esp32s3', recursive=True, config_rules_str=['=default'], manifest_files=yaml_file
         )
         assert len(apps) == 1
         assert apps[0].sdkconfig_files == [
             str(tmp_path / 'test1' / 'sdkconfig.defaults'),
         ]
+
+    def test_env_var(self, tmp_path, monkeypatch):
+        create_project('test1', tmp_path)
+
+        (tmp_path / 'test1' / 'sdkconfig.ci.foo').touch()
+        (tmp_path / 'test1' / 'sdkconfig.ci.bar').touch()
+        (tmp_path / 'test1' / 'sdkconfig.ci.baz').touch()
+
+        yaml_file = tmp_path / 'test.yml'
+        yaml_file.write_text(
+            f'''
+{tmp_path}:
+  enable:
+    - if: CONFIG_NAME == "foo" and IDF_TARGET == "esp32"
+    - if: CONFIG_NAME == "bar" and IDF_TARGET == "esp32s2"
+    - if: TEST_ENV_VAR == "1"
+    - if: CONFIG_NAME == "baz" and TEST_ENV_VAR == 0
+''',
+            encoding='utf8',
+        )
+
+        # in case you set it...
+        monkeypatch.delenv('CONFIG_NAME', raising=False)
+        monkeypatch.delenv('TEST_ENV_VAR', raising=False)
+
+        # CONFIG_NAME should NOT be overridden by env var
+        monkeypatch.setenv('CONFIG_NAME', 'bar')
+        apps = find_apps(
+            str(tmp_path / 'test1'),
+            'esp32',
+            config_rules_str=['sdkconfig.ci=default', 'sdkconfig.ci.*='],
+            manifest_files=yaml_file,
+        )
+        assert len(apps) == 2
+        assert apps[0].sdkconfig_files == [
+            str(tmp_path / 'test1' / 'sdkconfig.ci.baz'),
+        ]
+        assert apps[1].sdkconfig_files == [
+            str(tmp_path / 'test1' / 'sdkconfig.ci.foo'),
+        ]
+        monkeypatch.delenv('CONFIG_NAME')
+
+        # env var should be expanded
+        monkeypatch.setenv('TEST_ENV_VAR', '1')
+        apps = find_apps(
+            str(tmp_path / 'test1'),
+            'esp32',
+            config_rules_str=['sdkconfig.ci=default', 'sdkconfig.ci.*='],
+            manifest_files=yaml_file,
+        )
+        assert len(apps) == 3
+        monkeypatch.delenv('TEST_ENV_VAR')
```

### Comparing `idf_build_apps-1.0.0.dev1/tests/test_manifest.py` & `idf_build_apps-1.0.0rc0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/tests/test_utils.py` & `idf_build_apps-1.0.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev1/setup.py` & `idf_build_apps-1.0.0rc0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.0.dev1',
+      version='1.0.0rc0',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.0.dev1/PKG-INFO` & `idf_build_apps-1.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.0.dev1
+Version: 1.0.0rc0
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

