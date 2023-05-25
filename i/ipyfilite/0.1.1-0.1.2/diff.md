# Comparing `tmp/ipyfilite-0.1.1.tar.gz` & `tmp/ipyfilite-0.1.2.tar.gz`

## Comparing `ipyfilite-0.1.1.tar` & `ipyfilite-0.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.prettierrc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/jest.config.js
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/make.bat
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/develop-install.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/examples/example.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/examples/introduction.ipynb
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/_frontend.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/_pyodide.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/_version.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/upload.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/package.json
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/static/480.de9ad5492f82a03bdbf6.js
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/static/568.8c18863548aa30d504fc.js
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/static/687.5f576dec2f11535ef5d4.js
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/static/remoteEntry.71bb3ef6c8e7b0ddac51.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/static/style.js
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/nbextension/extension.js
--rw-r--r--   0        0        0    21897 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/nbextension/index.js
--rw-r--r--   0        0        0    72707 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/tests/conftest.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/ipyfilite/tests/test_upload.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/version.ts
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/widget.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 ipyfilite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.prettierrc
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/jest.config.js
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/examples/example.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/_frontend.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/_pyodide.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/_version.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/upload.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/package.json
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/480.d8f11be59adb4b02a2b1.js
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/568.7493dd3e4afb6b5b893b.js
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/687.5f576dec2f11535ef5d4.js
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/remoteEntry.baad50c678f67758255b.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/style.js
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/nbextension/extension.js
+-rw-r--r--   0        0        0    21897 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/nbextension/index.js
+-rw-r--r--   0        0        0    72707 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/conftest.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/test_upload.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/version.ts
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/widget.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/PKG-INFO
```

### Comparing `ipyfilite-0.1.1/.eslintrc.js` & `ipyfilite-0.1.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/MANIFEST.in` & `ipyfilite-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/package.json` & `ipyfilite-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -89,9 +89,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `ipyfilite-0.1.1/tsconfig.json` & `ipyfilite-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/webpack.config.js` & `ipyfilite-0.1.2/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/docs/Makefile` & `ipyfilite-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/docs/make.bat` & `ipyfilite-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/docs/source/conf.py` & `ipyfilite-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/docs/source/develop-install.rst` & `ipyfilite-0.1.2/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/docs/source/index.rst` & `ipyfilite-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/docs/source/installing.rst` & `ipyfilite-0.1.2/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/examples/introduction.ipynb` & `ipyfilite-0.1.2/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/ipyfilite/__init__.py` & `ipyfilite-0.1.2/ipyfilite/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/ipyfilite/_pyodide.py` & `ipyfilite-0.1.2/ipyfilite/_pyodide.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             ),
             str(upload_path),
         )
 
     js.ipyfilite = pyodide.ffi.to_js(
         {
             "channel": js.Reflect.construct(
-                js.BroadcastChannel, ["ipyfilite"]
+                js.BroadcastChannel,
+                pyodide.ffi.to_js(["ipyfilite"]),
             ),
             "session": str(uuid.uuid4()),
         },
         dict_converter=js.Object.fromEntries,
         create_pyproxies=False,
     )
     js.ipyfilite.channel.onmessage = files_upload_callback
```

### Comparing `ipyfilite-0.1.1/ipyfilite/upload.py` & `ipyfilite-0.1.2/ipyfilite/upload.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/ipyfilite/labextension/package.json` & `ipyfilite-0.1.2/ipyfilite/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.baad50c678f67758255b.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -48,15 +48,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.71bb3ef6c8e7b0ddac51.js"
+            "load": "static/remoteEntry.baad50c678f67758255b.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -93,9 +93,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `ipyfilite-0.1.1/ipyfilite/labextension/static/480.de9ad5492f82a03bdbf6.js` & `ipyfilite-0.1.2/ipyfilite/labextension/static/480.d8f11be59adb4b02a2b1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -326,11 +326,11 @@
                         i = o
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.1","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.2","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.1/ipyfilite/labextension/static/568.8c18863548aa30d504fc.js` & `ipyfilite-0.1.2/ipyfilite/labextension/static/568.7493dd3e4afb6b5b893b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -298,11 +298,11 @@
                         i = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.1","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.2","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.1/ipyfilite/labextension/static/687.5f576dec2f11535ef5d4.js` & `ipyfilite-0.1.2/ipyfilite/labextension/static/687.5f576dec2f11535ef5d4.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/ipyfilite/labextension/static/remoteEntry.71bb3ef6c8e7b0ddac51.js` & `ipyfilite-0.1.2/ipyfilite/labextension/static/remoteEntry.baad50c678f67758255b.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, l, f, s, d, c, p, h, v, b, g, m, y = {
+    var e, r, t, n, o, i, a, u, f, l, s, d, c, p, h, v, b, g, m, y = {
             229: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(897), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(897), t.e(480)]).then((() => () => t(480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -37,37 +37,37 @@
     }
     S.m = y, S.c = w, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        480: "de9ad5492f82a03bdbf6",
-        568: "8c18863548aa30d504fc",
+        480: "d8f11be59adb4b02a2b1",
+        568: "7493dd3e4afb6b5b893b",
         687: "5f576dec2f11535ef5d4",
         897: "a37754fc002c48d6bb2f"
     } [e] + ".js?v=" + {
-        480: "de9ad5492f82a03bdbf6",
-        568: "8c18863548aa30d504fc",
+        480: "d8f11be59adb4b02a2b1",
+        568: "7493dd3e4afb6b5b893b",
         687: "5f576dec2f11535ef5d4",
         897: "a37754fc002c48d6bb2f"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", S.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var s = f[l];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         a = s;
                         break
                     }
                 }
             a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var d = (r, n) => {
@@ -104,16 +104,16 @@
                             u = o[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
-                    l = [];
-                return "default" === t && (u("ipyfilite", "0.1.1", (() => Promise.all([S.e(897), S.e(568)]).then((() => () => S(568))))), u("uuid", "9.0.0", (() => S.e(687).then((() => () => S(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (u("ipyfilite", "0.1.2", (() => Promise.all([S.e(897), S.e(568)]).then((() => () => S(568))))), u("uuid", "9.0.0", (() => S.e(687).then((() => () => S(687)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -149,47 +149,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var a = [];
         for (i = 1; i < e.length; i++) {
             var u = e[i];
-            a.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+            a.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, l = !0;; u++, a++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+            for (var a = 0, u = 1, f = !0;; u++, a++) {
+                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(l = r[a]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
-                    if (!l || "u" != d) return !1
-                } else if (l)
+                    if (!f || "u" != d) return !1
+                } else if (f)
                     if (d == s)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (f = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    f = !1, u--
                 } else {
                     if (u <= n || s < d != o) return !1;
-                    l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
@@ -198,26 +198,26 @@
     }, a = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || d(l(e, t, o, n)), c(e[t][o])
+        return i(n, o) || d(f(e, t, o, n)), c(e[t][o])
     }, s = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var i = S.I(r);
         return i && i.then ? i.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (a(e, t), l(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
         var i = r && S.o(r, t) && s(r, t, n);
         return i ? c(i) : o()
     })), b = {}, g = {
         103: () => v("default", "uuid", [1, 9, 0, 0], (() => S.e(687).then((() => () => S(687))))),
         829: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
@@ -267,20 +267,20 @@
                         a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, o, [i, a, u] = t,
-                    l = 0;
+                    f = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in a) S.o(a, n) && (S.m[n] = a[n]);
                     u && u(S)
                 }
-                for (r && r(t); l < i.length; l++) o = i[l], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < i.length; f++) o = i[f], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkipyfilite = self.webpackChunkipyfilite || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var E = S(229);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyfilite = E
 })();
```

### Comparing `ipyfilite-0.1.1/ipyfilite/labextension/static/third-party-licenses.json` & `ipyfilite-0.1.2/ipyfilite/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/ipyfilite/nbextension/index.js` & `ipyfilite-0.1.2/ipyfilite/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -737,15 +737,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.1","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.2","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         n = {};
 
     function i(e) {
         var r = n[e];
         if (void 0 !== r) return r.exports;
```

### Comparing `ipyfilite-0.1.1/ipyfilite/nbextension/index.js.map` & `ipyfilite-0.1.2/ipyfilite/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/ipyfilite/tests/conftest.py` & `ipyfilite-0.1.2/ipyfilite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/src/extension.ts` & `ipyfilite-0.1.2/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/src/plugin.ts` & `ipyfilite-0.1.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/src/version.ts` & `ipyfilite-0.1.2/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/src/widget.ts` & `ipyfilite-0.1.2/src/widget.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/src/__tests__/index.spec.ts` & `ipyfilite-0.1.2/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/src/__tests__/utils.ts` & `ipyfilite-0.1.2/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/.gitignore` & `ipyfilite-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/LICENSE.txt` & `ipyfilite-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/README.md` & `ipyfilite-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.1/pyproject.toml` & `ipyfilite-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
 ]
-version = "0.1.1"
+version = "0.1.2"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -101,15 +101,15 @@
 ]
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "ipyfilite/_version.py" },
 ]
 
 [tool.tbump.version]
-current = "0.1.1"
+current = "0.1.2"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.black]
```

### Comparing `ipyfilite-0.1.1/PKG-INFO` & `ipyfilite-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyfilite
-Version: 0.1.1
+Version: 0.1.2
 Summary: File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 Project-URL: Homepage, https://github.com/juntyr/ipyfilite
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License: Copyright (c) 2023 Juniper Tyree
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

