# Comparing `tmp/napari-svg-0.1.6.tar.gz` & `tmp/napari-svg-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-svg-0.1.6.tar", last modified: Thu Jan 13 14:20:44 2022, max compression
+gzip compressed data, was "napari-svg-0.1.7.tar", last modified: Thu May 25 21:21:54 2023, max compression
```

## Comparing `napari-svg-0.1.6.tar` & `napari-svg-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-01-13 14:20:27.000000 napari-svg-0.1.6/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.502407 napari-svg-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-01-13 14:20:27.000000 napari-svg-0.1.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-01-13 14:20:27.000000 napari-svg-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-01-13 14:20:27.000000 napari-svg-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-13 14:20:27.000000 napari-svg-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-01-13 14:20:44.506407 napari-svg-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-01-13 14:20:27.000000 napari-svg-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-01-13 14:20:27.000000 napari-svg-0.1.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-01-13 14:20:27.000000 napari-svg-0.1.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/napari_svg/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/_shape_to_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/napari_svg/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/_tests/test_get_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/_tests/test_write_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     9253 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/hook_implementations.py
--rw-r--r--   0 runner    (1001) docker     (121)    10359 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/layer_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-01-13 14:20:27.000000 napari-svg-0.1.6/napari_svg/xml_to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/napari_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-13 14:20:44.000000 napari-svg-0.1.6/napari_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 14:20:44.506407 napari-svg-0.1.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-01-13 14:20:27.000000 napari-svg-0.1.6/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-13 14:20:27.000000 napari-svg-0.1.6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-13 14:20:27.000000 napari-svg-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-01-13 14:20:44.506407 napari-svg-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-01-13 14:20:27.000000 napari-svg-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-01-13 14:20:27.000000 napari-svg-0.1.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.695243 napari-svg-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-25 21:21:43.000000 napari-svg-0.1.7/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.683243 napari-svg-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.687243 napari-svg-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-25 21:21:43.000000 napari-svg-0.1.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 21:21:43.000000 napari-svg-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-25 21:21:43.000000 napari-svg-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 21:21:43.000000 napari-svg-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 21:21:54.695243 napari-svg-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-25 21:21:43.000000 napari-svg-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.687243 napari-svg-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 21:21:43.000000 napari-svg-0.1.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 21:21:43.000000 napari-svg-0.1.7/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.691243 napari-svg-0.1.7/napari_svg/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_shape_to_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.691243 napari-svg-0.1.7/napari_svg/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_tests/test_get_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_tests/test_write_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/hook_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/layer_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/xml_to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.691243 napari-svg-0.1.7/napari_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.695243 napari-svg-0.1.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 21:21:43.000000 napari-svg-0.1.7/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 21:21:43.000000 napari-svg-0.1.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 21:21:43.000000 napari-svg-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 21:21:54.695243 napari-svg-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 21:21:43.000000 napari-svg-0.1.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-25 21:21:43.000000 napari-svg-0.1.7/tox.ini
```

### Comparing `napari-svg-0.1.6/.cruft.json` & `napari-svg-0.1.7/.cruft.json`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/.github/workflows/test_and_deploy.yml` & `napari-svg-0.1.7/.github/workflows/test_and_deploy.yml`

 * *Files 23% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
         python-version: [3.7, 3.8, 3.9]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
@@ -43,16 +43,22 @@
           sudo apt-get install -y libdbus-1-3 libxkbcommon-x11-0 libxcb-icccm4 \
             libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 \
             libxcb-xinerama0 libxcb-xinput0 libxcb-xfixes0
 
       # strategy borrowed from vispy for installing opengl libs on windows
       - name: Install Windows OpenGL
         if: runner.os == 'Windows'
+        uses: actions/checkout@v3
+        with:
+          path: gl-ci-helpers
+          repository: pyvista/gl-ci-helpers
+          fetch-depth: 1
+      - name: Install Windows OpenGL
+        if: runner.os == 'Windows'
         run: |
-          git clone --depth 1 git://github.com/pyvista/gl-ci-helpers.git
           powershell gl-ci-helpers/appveyor/install_opengl.ps1
 
       # note: if you need dependencies from conda, considering using
       # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
       # and
       # tox-conda: https://github.com/tox-dev/tox-conda
       - name: Install dependencies
```

### Comparing `napari-svg-0.1.6/.gitignore` & `napari-svg-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/LICENSE` & `napari-svg-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/PKG-INFO` & `napari-svg-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: napari-svg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A plugin for reading and writing svg files with napari
 Home-page: https://github.com/napari/napari-svg
+Download-URL: https://github.com/napari/napari-svg
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD-3
-Download-URL: https://github.com/napari/napari-svg
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -77,9 +76,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/napari/napari-svg/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-svg-0.1.6/README.md` & `napari-svg-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/napari_svg/_shape_to_xml.py` & `napari-svg-0.1.7/napari_svg/_shape_to_xml.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/napari_svg/_tests/test_get_writer.py` & `napari-svg-0.1.7/napari_svg/_tests/test_get_writer.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/napari_svg/_tests/test_write_layer.py` & `napari-svg-0.1.7/napari_svg/_tests/test_write_layer.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/napari_svg/hook_implementations.py` & `napari-svg-0.1.7/napari_svg/hook_implementations.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/napari_svg/layer_to_xml.py` & `napari-svg-0.1.7/napari_svg/layer_to_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,17 @@
         svg specification
     extrema : array (2, 2)
         Extrema of data, specified as a minumum then maximum of the (x, y)
         coordinates.
     """
     # Extract metadata parameters
     if 'size' in meta:
-        size = np.mean(meta['size'], axis=1)
+        size = meta['size']
+        if size.ndim == 2:
+            size = np.mean(size, axis=1)
     else:
         size = np.ones(data.shape[0])
 
     if 'face_color' in meta:
         face_color = meta['face_color']
     else:
         face_color = np.ones((data.shape[0], 4))
```

### Comparing `napari-svg-0.1.6/napari_svg/xml_to_svg.py` & `napari-svg-0.1.7/napari_svg/xml_to_svg.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/napari_svg.egg-info/PKG-INFO` & `napari-svg-0.1.7/napari_svg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: napari-svg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A plugin for reading and writing svg files with napari
 Home-page: https://github.com/napari/napari-svg
+Download-URL: https://github.com/napari/napari-svg
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD-3
-Download-URL: https://github.com/napari/napari-svg
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -77,9 +76,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/napari/napari-svg/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-svg-0.1.6/napari_svg.egg-info/SOURCES.txt` & `napari-svg-0.1.7/napari_svg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/setup.cfg` & `napari-svg-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.6/tox.ini` & `napari-svg-0.1.7/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 platform = 
     macos: darwin
     linux: linux
     windows: win32
 passenv = 
     CI
     GITHUB_ACTIONS
-    DISPLAY XAUTHORITY
+    DISPLAY
+    XAUTHORITY
     PYVISTA_OFF_SCREEN
 deps =
     pytest-xvfb ; sys_platform == 'linux'
 extras =
     testing
 commands = 
     pytest -v --color=yes --cov=napari_svg --cov-report=xml
```

