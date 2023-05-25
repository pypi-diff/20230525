# Comparing `tmp/yjs_widgets-0.2.0.tar.gz` & `tmp/yjs_widgets-0.3.0.tar.gz`

## Comparing `yjs_widgets-0.2.0.tar` & `yjs_widgets-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/.prettierignore
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/.prettierrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/install.json
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   236775 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/yarn.lock
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/index.ts
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/model.ts
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/types.ts
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/notebookrenderer/index.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/notebookrenderer/model.ts
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/notebookrenderer/types.ts
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/notebookrenderer/view.ts
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/notebookrenderer/widgetManager.ts
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/src/notebookrenderer/yCommProvider.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/style/index.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/yjs_widgets/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/yjs_widgets/_version.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/LICENSE
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/README.md
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 yjs_widgets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/.eslintrc.js
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/install.json
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0   201745 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/yarn.lock
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/index.ts
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/model.ts
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/types.ts
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/notebookrenderer/types.ts
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/style/index.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/yjs_widgets/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/yjs_widgets/_version.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/README.md
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 yjs_widgets-0.3.0/PKG-INFO
```

### Comparing `yjs_widgets-0.2.0/.eslintrc.js` & `yjs_widgets-0.3.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/CONTRIBUTING.md` & `yjs_widgets-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/package.json` & `yjs_widgets-0.3.0/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9470833333333333%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/notebook': '^4.0.0', "*

 * *                   "'@jupyterlab/services': '^7.0.0', '@lumino/coreutils': '^2.1.1', "*

 * *                   "'@lumino/signaling': '^2.1.1', '@lumino/widgets': '^2.1.1', 'lib0': '^0.2.76', "*

 * *                   "'uuid': '^9.0.0', delete: ['@jupyterlab/docprovider', "*

 * *                   "'@jupyterlab/docregistry', '@jupyterlab/fil […]*

```diff
@@ -5,40 +5,31 @@
     },
     "bugs": {
         "url": "https://github.com/QuantStack/yjs-widgets/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^6.0.2",
         "@jupyter/ydoc": "^1.0.2",
-        "@jupyterlab/application": "^4.0.0-beta.2",
-        "@jupyterlab/apputils": "^4.0.0-beta.2",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/collaboration": "^4.0.0-alpha.18",
-        "@jupyterlab/coreutils": "^6.0.0-beta.2",
-        "@jupyterlab/docprovider": "^4.0.0-alpha.18",
-        "@jupyterlab/docregistry": "^4.0.0-beta.2",
-        "@jupyterlab/filebrowser": "^4.0.0-beta.2",
-        "@jupyterlab/launcher": "^4.0.0-beta.2",
-        "@jupyterlab/mainmenu": "^4.0.0-beta.2",
-        "@jupyterlab/notebook": "^4.0.0-beta.2",
-        "@jupyterlab/observables": "^5.0.0-beta.2",
-        "@jupyterlab/services": "^7.0.0-beta.2",
-        "@jupyterlab/translation": "^4.0.0-beta.2",
-        "@jupyterlab/ui-components": "^4.0.0-beta.2",
-        "@lumino/commands": "^2.1.0",
-        "@lumino/coreutils": "^2.1.0",
-        "@lumino/signaling": "^2.1.0",
-        "@lumino/widgets": "^2.1.0",
-        "lib0": "^0.2.62",
-        "uuid": "^8.3.2",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@lumino/coreutils": "^2.1.1",
+        "@lumino/signaling": "^2.1.1",
+        "@lumino/widgets": "^2.1.1",
+        "lib0": "^0.2.76",
+        "uuid": "^9.0.0",
         "webpack": "^5.77.0",
         "webpack-cli": "^5.0.1"
     },
     "description": "A JupyterLab extension for widgets based on Yjs.",
     "devDependencies": {
-        "@jupyterlab/builder": "~4.0.0-beta.0",
+        "@jupyterlab/builder": "~4.0.0",
         "@types/node": "^16.11.10",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "copy-webpack-plugin": "^10.0.0",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
@@ -72,17 +63,17 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/QuantStack/yjs-widgets.git"
     },
     "resolutions": {
-        "@jupyterlab/apputils": "~4.0.0-beta.0",
-        "@jupyterlab/notebook": "~4.0.0-beta.0",
-        "@lumino/coreutils": "^2.1.0"
+        "@jupyterlab/apputils": "~4.0.0",
+        "@jupyterlab/notebook": "~4.0.0",
+        "@lumino/coreutils": "^2.1.1"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
@@ -104,9 +95,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `yjs_widgets-0.2.0/tsconfig.json` & `yjs_widgets-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/yarn.lock` & `yjs_widgets-0.3.0/yarn.lock`

 * *Files 10% similar despite different names*

```diff
@@ -29,39 +29,39 @@
     chalk: ^2.0.0
     js-tokens: ^4.0.0
   checksum: 92d8ee61549de5ff5120e945e774728e5ccd57fd3b2ed6eace020ec744823d4a98e242be1453d21764a30a14769ecd62170fba28539b211799bbaf232bbb2789
   languageName: node
   linkType: hard
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1":
-  version: 6.6.0
-  resolution: "@codemirror/autocomplete@npm:6.6.0"
+  version: 6.7.1
+  resolution: "@codemirror/autocomplete@npm:6.7.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.6.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 01d5d81e46d179da2c742020d7cb7c97cceb1af5772ac1fbf81abfe18408d694a78851234137fabadce1ed8f829d598a2e9c4b6fbd9632a813fa72772e458f9d
+  checksum: 5f1331cceb6a7b0bd4dc9bad6025d16d1c415bfc2fba29b452f9f5501abd34b75a240e3a20fb9fed92a82a666e54562c32cfe220892713bfbd5a5a16fa004cd8
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
-  version: 6.2.3
-  resolution: "@codemirror/commands@npm:6.2.3"
+  version: 6.2.4
+  resolution: "@codemirror/commands@npm:6.2.4"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: e6b7d07818d6df4372a272539b84a256e651cfa3416a33f9e1859f2ced0f6e3c944e0c40c2c407dcd5b13ffab2931d4e5ea5952db439837071de336e7a31c722
+  checksum: 468895fa19ff0554181b698c81f850820de5c0289cab92c44392fb127286f09ca72b921d6ea4353b70b616a4fd0c3667d86b6f917202a3ad2e196eb7b581f7b6
   languageName: node
   linkType: hard
 
 "@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
@@ -108,25 +108,25 @@
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
-  version: 6.1.7
-  resolution: "@codemirror/lang-javascript@npm:6.1.7"
+  version: 6.1.8
+  resolution: "@codemirror/lang-javascript@npm:6.1.8"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: 15ce6695e7276102dbc874d178cbc4434d126b7a3e08f89aa9338c7dce5d2d6bdd5f1c6d114a744a8fa26dfc62b0dc639fe6e5c7b306bd14ed37272e75739736
+  checksum: 58ccd1c96db52edc95015b3fc77021540c18b4b87ce2c9426402a53993a67d7946647aba7198223dc51a56ec55379603a6d986fe32332d85cb3d8768c92a562e
   languageName: node
   linkType: hard
 
 "@codemirror/lang-json@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-json@npm:6.0.1"
   dependencies:
@@ -181,23 +181,23 @@
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.4.1
-  resolution: "@codemirror/lang-sql@npm:6.4.1"
+  version: 6.5.0
+  resolution: "@codemirror/lang-sql@npm:6.5.0"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: d1823e760b88bb15399684b1136b3c7167f104854645b971aa80d7e261e4ad204a5258f1ccd9bbb37a90b20821d2b8fcfac9092198e599b21e7a0cb1e50dc0ee
+  checksum: 5bc73293d85f3892633703f277787336c00135011b14ca34a3590975a02c5ec1d6826d201d827e3dfc1d3427e28d23f36b1ef4fd69fc5d79c98290030c11dad5
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-wast@npm:6.0.1"
   dependencies:
@@ -218,24 +218,24 @@
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
   checksum: e156ecafaa87e9b6ef4ab6812ccd00d8f3c6cb81f232837636b36336d80513b61936dfee6f4f6800574f236208b61e95a2abcb997cdcd7366585a6b796e0e13b
   languageName: node
   linkType: hard
 
 "@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0":
-  version: 6.6.0
-  resolution: "@codemirror/language@npm:6.6.0"
+  version: 6.7.0
+  resolution: "@codemirror/language@npm:6.7.0"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
-  checksum: bb9411620e2f231653a3f0c4429e0d19a3843bff5dbc117df4649d7bf783ec4ad809c0add8bc0887a4ec3f48b4f8f941621168e47d76101d5383f0d670af1722
+  checksum: 673905e9eb80f039a5e6c59a8aeca217e124a9a03734848043192aeff9e5b3a82f150559f7bd637ee197c4b2171eb5b04e757d717922128ea4fecca1ac6ecac4
   languageName: node
   linkType: hard
 
 "@codemirror/legacy-modes@npm:^6.3.2":
   version: 6.3.2
   resolution: "@codemirror/legacy-modes@npm:6.3.2"
   dependencies:
@@ -263,28 +263,28 @@
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 441e04fc896ac984f224e3adb20bc8a6c63d929778335c70d2cb1e3843674c7998db93e2ab1cd05e8276cb3819766cd23951eec748fdf8e66e3611bd9a55aab5
   languageName: node
   linkType: hard
 
 "@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.1.4, @codemirror/state@npm:^6.2.0":
-  version: 6.2.0
-  resolution: "@codemirror/state@npm:6.2.0"
-  checksum: fdc99c773dc09c700dd02bf918f06132aa8d3069c262cc4eb6ca5c810ce24ae2d7e90719ae7630a8158fd263018de6d40bd78f312e6bfba754e737b64e6c6b3d
+  version: 6.2.1
+  resolution: "@codemirror/state@npm:6.2.1"
+  checksum: d12a321d0471b264b9d3259042bff913a8b939e8d28d408ff452004538a71ca9d5329df3f8a1d8a9183f5b42a7ef5b200737bcab1065714f5ae8e0a5ba9d59d3
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.9.6":
-  version: 6.10.0
-  resolution: "@codemirror/view@npm:6.10.0"
+  version: 6.12.0
+  resolution: "@codemirror/view@npm:6.12.0"
   dependencies:
     "@codemirror/state": ^6.1.4
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
-  checksum: ff6a370319fc62a70af062e187b28c0ae2f9df3edd29fd8096129b3be76b46ccfebb8baa1fef36a7a1b73977e5d54b036e3a4b52bd0b0bc70d82ffb8842541f2
+  checksum: 512cbc9c05ac2cfa738cdf7aac711847b44e24ff5869f31839a9fcc11da6a512448fa9bc980535d55b897de80d49e744336a2724ca1fe3dae8bfcb31e339fe64
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.7
   resolution: "@discoveryjs/json-ext@npm:0.5.7"
   checksum: 2176d301cc258ea5c2324402997cf8134ebb212469c0d397591636cea8d3c02f2b3cf9fd58dcb748c7a0dade77ebdc1b10284fa63e608c033a1db52fddc69918
@@ -311,21 +311,14 @@
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
-"@gar/promisify@npm:^1.1.3":
-  version: 1.1.3
-  resolution: "@gar/promisify@npm:1.1.3"
-  checksum: 4059f790e2d07bf3c3ff3e0fec0daa8144fe35c1f6e0111c9921bd32106adaa97a4ab096ad7dab1e28ee6a9060083c4d1a4ada42a7f5f3f7a96b8812e2b757c1
-  languageName: node
-  linkType: hard
-
 "@humanwhocodes/config-array@npm:^0.5.0":
   version: 0.5.0
   resolution: "@humanwhocodes/config-array@npm:0.5.0"
   dependencies:
     "@humanwhocodes/object-schema": ^1.2.0
     debug: ^4.1.1
     minimatch: ^3.0.4
@@ -412,116 +405,102 @@
     backbone: 1.4.0
     jquery: ^3.1.1
     lodash: ^4.17.4
   checksum: f82b4eec8fc819adaab6728077700484fc0ab7b64c6ecbf95bf960bbfff0515a18b88ab5c84f92f3ea1636e03f8dc4c4db264ca69d9783fd37149ca1f970ac1c
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^0.3.1":
-  version: 0.3.4
-  resolution: "@jupyter/ydoc@npm:0.3.4"
-  dependencies:
-    "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.15
-    "@lumino/coreutils": ^1.11.0 || ^2.0.0-alpha.6
-    "@lumino/disposable": ^1.10.0 || ^2.0.0-alpha.6
-    "@lumino/signaling": ^1.10.0 || ^2.0.0-alpha.6
-    y-protocols: ^1.0.5
-    yjs: ^13.5.40
-  checksum: edd14a01be6ceac437d3ebfb5f7a2d2c8eac60fec91e48d8d2ef2bef9f1423b4350c57dba25b3b043759ffb61b601a3815c1ea56532d1d707e3fbeb5df86b7e6
-  languageName: node
-  linkType: hard
-
 "@jupyter/ydoc@npm:^1.0.2":
   version: 1.0.2
   resolution: "@jupyter/ydoc@npm:1.0.2"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: 739f9630940466b3cfcd7b742dd06479f81772ca13f863d057af0bbb5e318829506969066ab72977e7c721644982b5c8f88cf44e1ae81955ed1c27e87632d1f2
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.0-beta.2":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/application@npm:4.0.0-rc.0"
+"@jupyterlab/application@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/application@npm:4.0.0"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/application": ^2.1.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: a287f484f412c02ba67e1b87364750b5457a73e5c4a547cf197e580ed591c32df1ae58b6012af817e78c223ca3e007009805eccfb1836cf6366c08a51edfc5f3
+  checksum: 82750647de5997d6945627f517d82ffad3e7c272bce0c195819cc138b59546fbe43ee6c0ef4baf88de303964288ed1ac36234a99bedfb319eaf456b1321b199c
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:~4.0.0-beta.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/apputils@npm:4.0.0-rc.0"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/settingregistry": ^4.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+"@jupyterlab/apputils@npm:~4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/apputils@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 1236e35b5a52c0de2f3895680e1e885df32704f84a926d8cd221c0da0e44935e57c47de128427f23f76aee4f80658d9b64cd36dc75b11417a1b68f0eaaaef526
+  checksum: 360bf34e9810a7014c6637a6ac5c23a2ee73da8339675235cee3866beb3a477dc3b4d993c0a79da5ebe472f5c28fa131d507d62e20b3a93853f05e62b126add9
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/attachments@npm:4.0.0-rc.0"
+"@jupyterlab/attachments@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/attachments@npm:4.0.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
-  checksum: 8bdd87fcc1b780c3f20f6cf76a312af1dce8e54d4683c56978cb052779a2d255199ffa8559d3f290f0604ab10b2e2dd0cb608dc64954c5db079bc29f8368e1e7
+  checksum: 71c8e488a0d31e00e1345336edece04faa0d2b6fbf5de284fad05bb2a8f732c57e9b2ffe10999dd416a1d00cdce4bc425f9f88dd91684cb8b55eea52a1d5ed98
   languageName: node
   linkType: hard
 
-"@jupyterlab/builder@npm:~4.0.0-beta.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/builder@npm:4.0.0-rc.0"
+"@jupyterlab/builder@npm:~4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/builder@npm:4.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/application": ^2.1.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
@@ -548,80 +527,80 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 0f958759b1210cf2d2293d681adf7ab279e63c918ae23ebf891cb1aab15d865446d640ef019f63acd33a917362db36a04e066d1ee57da80e963019925e97dab4
+  checksum: c359031858376e37b2fe46bc7897fe0568b0cf90bcaaee6bded2e22f207c61a32d4b00b6954de00082e551dd07b6259997c00feeb25e7d44acf9ac97934fdd45
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/cells@npm:4.0.0-rc.0"
+"@jupyterlab/cells@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/cells@npm:4.0.0"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/attachments": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/codemirror": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/documentsearch": ^4.0.0-rc.0
-    "@jupyterlab/filebrowser": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/outputarea": ^4.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/toc": ^6.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/attachments": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/codemirror": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/filebrowser": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/outputarea": ^4.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/toc": ^6.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: ee71d6f4763ea6ad44e0662d9f0fc4c0e7a81b5881160c00477b09e3c6094561bb01592286edcb05ac76d1a9756fdda0cf40d5df4554c119265e3bcbaceb196e
+  checksum: 2474642428f344a316b0296640f9adb07e805d3c8896d1a601a2a5131fc4f4a8a4a627583f3dff904f7c318d6c0f236bc0d9cd200545f395796fcfe4244ecbcb
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/codeeditor@npm:4.0.0-rc.0"
+"@jupyterlab/codeeditor@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/codeeditor@npm:4.0.0"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: f6d869bf526a14478576d55f98470ee31d147e52c65843d5dedc8e62cd83ee36084e3cdcbde9363edaf28522a4d92414f0caf19c0482da9cbdcb40267248b79c
+  checksum: 8287d77738a41814eb83621691adbcee119e6a7b3d4741250e53fc11b8664ce1f6ae5a79150222b235d45ec7b22db980d773d77a517d6b5c6a241b8a27817b7a
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/codemirror@npm:4.0.0-rc.0"
+"@jupyterlab/codemirror@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/codemirror@npm:4.0.0"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
@@ -636,27 +615,28 @@
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/documentsearch": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
+    "@lezer/markdown": ^1.0.2
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     yjs: ^13.5.40
-  checksum: 9ac820eb1b8dd239b47f1cebea86e15342bf75ca14c0a03858ece85876e8ce509acf02d4f9eba4f4149014ec9ef54f093ec7547ab89343e133571382e24fcdd4
+  checksum: 3252c57f1d35924d6d6ad2a48690fa8bbe4e1a22455f9e1514b4405d16ff379532477aed331cd28908e8d0ef572ee76937ee5f382c95dc62e5dd97fa911603d5
   languageName: node
   linkType: hard
 
 "@jupyterlab/collaboration@npm:^4.0.0-alpha.18":
   version: 4.0.0-alpha.18
   resolution: "@jupyterlab/collaboration@npm:4.0.0-alpha.18"
   dependencies:
@@ -685,244 +665,194 @@
     moment: ^2.24.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.1
   checksum: a9bfd0732ef8623212f34ea71b3f5e6556cb7a14dc00e692abca4ea97c6ca0799f7c9a879b71be477194bcbe5d83160c6a99c9158a82ff4aef9db0f8b40a624d
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.0-alpha.18, @jupyterlab/coreutils@npm:^6.0.0-beta.2, @jupyterlab/coreutils@npm:^6.0.0-rc.0":
-  version: 6.0.0-rc.0
-  resolution: "@jupyterlab/coreutils@npm:6.0.0-rc.0"
+"@jupyterlab/coreutils@npm:^6.0.0, @jupyterlab/coreutils@npm:^6.0.0-alpha.18":
+  version: 6.0.0
+  resolution: "@jupyterlab/coreutils@npm:6.0.0"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: 5b1e3e19aa2a9aec27ddf8c1997480c46dfbda46719e6cb1e6529b151fc95058554d80cf40e96a0a4328c74e25249cf75819a5fc5f2357f726a51c530a040b41
+  checksum: c46bb60af792186b4d9d60378fdb2f03473055736e438e05971bcbf1d5edb62c7722f1465e5ef2fd2dc9c4b5b6043301012478b218cf6c475a99914b26a1fd14
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/docmanager@npm:4.0.0-rc.0"
+"@jupyterlab/docmanager@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/docmanager@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 601c285b79f8a9bfb01a4ff729f65e76c0131593e9f2bc216cd99fd9457552187c3663f31f86109981fb2e7edb8fe074b731795d610f2b4fc173969f017b5a13
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/docprovider@npm:^4.0.0-alpha.18":
-  version: 4.0.0-alpha.18
-  resolution: "@jupyterlab/docprovider@npm:4.0.0-alpha.18"
-  dependencies:
-    "@jupyter/ydoc": ^0.3.1
-    "@jupyterlab/coreutils": ^6.0.0-alpha.18
-    "@jupyterlab/services": ^7.0.0-alpha.18
-    "@lumino/coreutils": ^2.0.0-alpha.6
-    "@lumino/disposable": ^2.0.0-alpha.6
-    "@lumino/signaling": ^2.0.0-alpha.6
-    y-protocols: ^1.0.5
-    y-websocket: ^1.3.15
-    yjs: ^13.5.40
-  checksum: b8cb826b63fd7d0e87b650913a63defa39bb15afb8b70d683c4b9e5e995ca9019b200f6d2af761fac36ccb2555cfeca8b5e799e14ab9ec5dc4675c4100801763
+  checksum: d9495bea5f5e5de2d133be0ea097b9d2634575d1054dafb198d49398bfed6b9ff52d5d2ce0848ae11462fa5070f6651eccda3242f867661758f135b0703839f9
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.0-beta.2, @jupyterlab/docregistry@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/docregistry@npm:4.0.0-rc.0"
+"@jupyterlab/docregistry@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/docregistry@npm:4.0.0"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: d34ad77d8aadc33652f1fed858dc100580425ce005426796a4c9589933ba926c79fca95fe79460c7f04a58887f3e814c3616e45b823689d7d24582a3c5ca4645
+  checksum: 8927ea10312238333d1036ea6f4047d86779120cdf6c8391f91e5d859e85d504c2345f629a2a8cf50cdc394739828cc4868a46ebefe1c20932a2f496463ca250
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/documentsearch@npm:4.0.0-rc.0"
+"@jupyterlab/documentsearch@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/documentsearch@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: c0cf07ff23625e20f67715a5296a4b2918087152991afa541aca60f3bc552be5ebdc9fd216b80e047cf3cedbfc4326d4ede02585e9274c7e21a1fb61b7863c48
+  checksum: 686befb5ae48a485530f298f7d067b5c77d17524fff779f8c468857c44baab75f1ed3c504546f6440cf0cfc8420e617abcbaa120208d2166cfb124a6455e5472
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.0-beta.2, @jupyterlab/filebrowser@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/filebrowser@npm:4.0.0-rc.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docmanager": ^4.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+"@jupyterlab/filebrowser@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/filebrowser@npm:4.0.0"
+  dependencies:
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docmanager": ^4.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statedb": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 9ce98e059792e02984b142d009314ee56331156f2b09bc11787322188ec99412acb8b04ada1f40e815f5b37031da48a8e1fe88b91e42f99052bc005850518ae6
+  checksum: 58e61e9b0e6d373fa5cd93398dfee146c635d5f5008d00e640c4f0687ed8ed7135779806e159703a88ecd55f45b1725214c657a466e63577b70b0380c5852df5
   languageName: node
   linkType: hard
 
-"@jupyterlab/launcher@npm:^4.0.0-beta.2":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/launcher@npm:4.0.0-rc.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/properties": ^2.0.0
-    "@lumino/widgets": ^2.1.1
-    react: ^18.2.0
-  checksum: d2ee1e9cffef482bfb30ab79eee450e34c73e98f5ae9907d3a4c8c51e681beffeeedf5358eda6fcf557001343b5d495c79d278847e2dc0467ed95f8d6b71a89f
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/lsp@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/lsp@npm:4.0.0-rc.0"
+"@jupyterlab/lsp@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/lsp@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 216fb96098f5b736fb237ee060309a766fee0b378d8bbe45ae2db4858d942fd41a5f58bbad8d26af771e704b0eff09252702e0538fe30086012128a840940b2b
+  checksum: 7657fe88fc155e7a988558b9b8d34a36d6bb5fee0571a0953ac77add170f82b2f7ad1d76c1f90185087daebb4d40c5ff9e7f44478abbcb485736f7806d3d7fb8
   languageName: node
   linkType: hard
 
-"@jupyterlab/mainmenu@npm:^4.0.0-beta.2":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/mainmenu@npm:4.0.0-rc.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/widgets": ^2.1.1
-  checksum: 2d82b3129819287b835fc01d56ce7d639fc57d32447ff26702dbd3e848b4bdc59f71e9b333b927828100d25069492a57b964687d44633525e43df0483e796ead
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.15, @jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/nbformat@npm:4.0.0-rc.0"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/nbformat@npm:4.0.0"
   dependencies:
     "@lumino/coreutils": ^2.1.1
-  checksum: b37a04681f7a4364bb87a038298b40468306b8d83799fa0f1fec6c09f330c4f878320e82ebb08945a0c9377fb385fbf65a12e7a2f5895966af25e4db6561d062
+  checksum: 152da6b9622c7683543ad2bd9525857a8a39b4b8a5474998e921232f108c366dd8625daeb14e2cc2aa8aac124b9a5d16f285310cd241c9769d51af80730dbd59
   languageName: node
   linkType: hard
 
 "@jupyterlab/nbformat@npm:^3.6.3":
   version: 3.6.3
   resolution: "@jupyterlab/nbformat@npm:3.6.3"
   dependencies:
     "@lumino/coreutils": ^1.11.0
   checksum: 5118877af7b7d54a699adbf4f42dd00f04738c9ee04233a40de24843830bfe6515b82b648a629cf019c51a1342158e358670702fd666637986551b626de25f26
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:~4.0.0-beta.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/notebook@npm:4.0.0-rc.0"
+"@jupyterlab/notebook@npm:~4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/notebook@npm:4.0.0"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/cells": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/codemirror": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/documentsearch": ^4.0.0-rc.0
-    "@jupyterlab/lsp": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/settingregistry": ^4.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/toc": ^6.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/cells": ^4.0.0
+    "@jupyterlab/codeeditor": ^4.0.0
+    "@jupyterlab/codemirror": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/documentsearch": ^4.0.0
+    "@jupyterlab/lsp": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statusbar": ^4.0.0
+    "@jupyterlab/toc": ^6.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: a2ea0c8e13827957c70b69a28ee7a8eefc60ff858778d36fbac9040c40af8c36f46ed8311e8c400c40ef904939459f72b437d8376fa8f2bbcc3d16070a1490be
+  checksum: 29ba29519fba567d0d686426b750d58bfddf6235cb3ad812ef671750637dbfcdafb5348feda44168d83f65936e5478562cffdc7ceeabac221fcdfab38f11bc31
   languageName: node
   linkType: hard
 
 "@jupyterlab/observables@npm:^4.6.3":
   version: 4.6.3
   resolution: "@jupyterlab/observables@npm:4.6.3"
   dependencies:
@@ -931,76 +861,76 @@
     "@lumino/disposable": ^1.10.0
     "@lumino/messaging": ^1.10.0
     "@lumino/signaling": ^1.10.0
   checksum: f16620454bd88fc37edf078df9c33a91de5fa74e6a9e20f6de0e45ea142d086332014700f3815ca734001c791cb28fd47070c8aa13ffc460d25b3925b77a03d4
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.0-beta.2, @jupyterlab/observables@npm:^5.0.0-rc.0":
-  version: 5.0.0-rc.0
-  resolution: "@jupyterlab/observables@npm:5.0.0-rc.0"
+"@jupyterlab/observables@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "@jupyterlab/observables@npm:5.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
-  checksum: ab5a846b80fec04c16d1021fa15a82de2e7b57ac343c0d13d3893277c07364d1986a7aac7668f0d340de3471a8b922ce6c3a5459c77f5ec3998ffe6d4c8052c9
+  checksum: 1554f473e0ab0eef288ea86945c03a07d79f478bfdf55651036161a58cd1d9a0695e202ced0ebe3a6863f73ba12ccd85b86f7a4c2e6f9fe41ccddb0c4fbbc33e
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/outputarea@npm:4.0.0-rc.0"
+"@jupyterlab/outputarea@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/outputarea@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: ec9c3ccb3a743f487172cde5e78088cdf5eb0d005d5e52ca688b8005f3e9ebe59a659956d2210a50927610339a194af5efd664c149bebca4ef5fc49919b0bba4
+  checksum: d2c22e1fe1ebe4407e7a5d383addda64561b5a3afda277a0c4750be48bf30fbb90ee6a3401ac0a9410a7e3c969792d34bc2dcc880806fa3b290ecace01710e80
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.8.0-rc.0":
-  version: 3.8.0-rc.0
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.0-rc.0"
+"@jupyterlab/rendermime-interfaces@npm:^3.8.0":
+  version: 3.8.0
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.0"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: 373045bbc1cfb8fee5cc373741419ef11f97fb163ef22f1ad4e69cdaa51c714f369ec07cca8e10a00dc64c510b4aa08b1630419632c61e4f1219678bb35bc904
+  checksum: 5e70a58a4d8aa7380a041d267972851b9b3fa5e4d68d254ede51c9e5bea4a76b38d47bc5c512e2fd84cd297f5bcaf9cbc9f73ba0824b5b910b10043309a820c7
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/rendermime@npm:4.0.0-rc.0"
+"@jupyterlab/rendermime@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/rendermime@npm:4.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/translation": ^4.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     lodash.escape: ^4.0.1
-  checksum: 3605eb77a905ae3767e10b4202de5686d6bff215a23a1dafb59c2c6045a55d208136bf786f26c6db6cce4c1e710eb374a98726b2bbf97aafcffb965094cdf116
+  checksum: fb6373517bf2fa2557b38ccf53ba95b45c9327f86f14726dedd433f0b3466f439ab98cb2c8ae10aded9f269bf7c11225765e286aeca56f3755bada8f5d5e102a
   languageName: node
   linkType: hard
 
 "@jupyterlab/services@npm:^6.0.0":
   version: 6.6.3
   resolution: "@jupyterlab/services@npm:6.6.3"
   dependencies:
@@ -1016,30 +946,30 @@
     "@lumino/signaling": ^1.10.0
     node-fetch: ^2.6.0
     ws: ^7.4.6
   checksum: a8eb3138c83107449acb1df4f244bca9c6f0fad35a25e0dca16a2544149a87a438592cdb6c73c83caf875907f0238f3164292b20d6a3404ddd0354142dbac5ac
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.0-alpha.18, @jupyterlab/services@npm:^7.0.0-beta.2, @jupyterlab/services@npm:^7.0.0-rc.0":
-  version: 7.0.0-rc.0
-  resolution: "@jupyterlab/services@npm:7.0.0-rc.0"
+"@jupyterlab/services@npm:^7.0.0, @jupyterlab/services@npm:^7.0.0-alpha.18":
+  version: 7.0.0
+  resolution: "@jupyterlab/services@npm:7.0.0"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/settingregistry": ^4.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     ws: ^8.11.0
-  checksum: 92f6b6944cab467683d8fa535cd8361497cc52d54fb621a2f6fface82f99b57e00b86bff0f31ada6fad9a0833ff3de331eae2585dea0d10f3dc9597127c5d508
+  checksum: 96e986e8007247aa5258586263e31e48dfa6e7e7bb2a9d61f699e41b291f50c8653a9c42ae340a428c9af58946c47f7021ccb6b79b74b750cf1547b8d6c81b03
   languageName: node
   linkType: hard
 
 "@jupyterlab/settingregistry@npm:^3.6.3":
   version: 3.6.3
   resolution: "@jupyterlab/settingregistry@npm:3.6.3"
   dependencies:
@@ -1050,30 +980,30 @@
     "@lumino/signaling": ^1.10.0
     ajv: ^6.12.3
     json5: ^2.1.1
   checksum: 6382746aa715d8e3e8d0abe48429975e7432eb1ac767413a3107b77e8135ab0cea869a0d20e1cb8f1f7c6dba1f1ffb16a9a9973d1be68e65115c44c573bdf30a
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/settingregistry@npm:4.0.0-rc.0"
+"@jupyterlab/settingregistry@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/settingregistry@npm:4.0.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
+    "@jupyterlab/nbformat": ^4.0.0
+    "@jupyterlab/statedb": ^4.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@rjsf/utils": ^5.1.0
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: c4d7d0b0777f6cc5e614153db51277516c1e665db37b7a42f4de03b449ffd61f2a30b63ce9e0e9e4011dd88f3b0ff57ee7fe10f5044e8bbc5ff41c17f48c2bb5
+  checksum: f52cd36c28336ad554a4eb43f6cef7f82cb7a9161897e8b633da8c0b4519d0ed7e3e34846fec132714867b0190a9c19754e88edef31ffdf6dc2d1afe49b50041
   languageName: node
   linkType: hard
 
 "@jupyterlab/statedb@npm:^3.6.3":
   version: 3.6.3
   resolution: "@jupyterlab/statedb@npm:3.6.3"
   dependencies:
@@ -1082,85 +1012,85 @@
     "@lumino/disposable": ^1.10.0
     "@lumino/properties": ^1.8.0
     "@lumino/signaling": ^1.10.0
   checksum: e3ea76524184ac62797e894ba4146a66ecdddada0167af9d8d360b0439e04dcf89d0da5b7e2fe0d02bc968796909659054a8c076eced17519773cddfb1ab0e96
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/statedb@npm:4.0.0-rc.0"
+"@jupyterlab/statedb@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/statedb@npm:4.0.0"
   dependencies:
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
-  checksum: cb2ed22b6b66d43e03cf07d3a95c09551fd812770e66d950c4eb7e1c6c4bb59e9cd65ec7522dd61de66af4c92492c8cf49db7ee89d63fc17cfc3e15d8696d7ad
+  checksum: e90c943b4486df3a1bd53c64c0860e40706a26f4307628f2c71168090f47f85bab2fd68529366aa74211501a6875bd6d7098e1cd976f2e7d2d197a687b6b3bd3
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/statusbar@npm:4.0.0-rc.0"
+"@jupyterlab/statusbar@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/statusbar@npm:4.0.0"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: df1e481c2a681ec133c1f2cc9e3094dfa1297cbb9bfafc9a1351bf5381952dcee09c07ec3b16f3c73ecbdb16c775dd58c7b6d9e8a8766f47a7f98fe876c55031
+  checksum: 861444ba5ca001f9174b58d5a2c46e4d7947856b1c5302d3ec70e6c72d1608c77b65c792904e07fd8612f11d51ac9f30aa2ad3cbd256e701d6c12138e3f9b89f
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.0.0-rc.0":
-  version: 6.0.0-rc.0
-  resolution: "@jupyterlab/toc@npm:6.0.0-rc.0"
+"@jupyterlab/toc@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "@jupyterlab/toc@npm:6.0.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/docregistry": ^4.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime": ^4.0.0
+    "@jupyterlab/translation": ^4.0.0
+    "@jupyterlab/ui-components": ^4.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 091bb3b0988e63b4a232dca4a2e2ee1b023daad67dbb0cc65883ba08b72c7673d82d506228d5919b9f33dff9815b4f4a6d5ea172fb2af22e5fb87b56d7562197
+  checksum: 7fd8cbbeaaad272355296d8ddab01c54233373d2c0457d93beae1efa2e491845980746b75f46f78f49370668a323f42ef923b76c55bf9a520548845f7c5e2d57
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.0-beta.2, @jupyterlab/translation@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/translation@npm:4.0.0-rc.0"
+"@jupyterlab/translation@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "@jupyterlab/translation@npm:4.0.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/statedb": ^4.0.0
     "@lumino/coreutils": ^2.1.1
-  checksum: f0c2abfd3b7c3e93c3e42b39f1e3fa92ba2d2edb6ba86d7ea0cfff6fb889de9d81fcf4cf3c76bddf0fa79d333009dbd46aed0800a84aee99470eb751e1fdb1f6
+  checksum: f3124bff6e3eb9c1adbe91f60dd823a3b4a4b8b453fbf024a605f5be44463fa7eb15e176238255a775c96b50e4cc551bde757a03531e56a76db25a30feed469f
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.0-alpha.33, @jupyterlab/ui-components@npm:^4.0.0-beta.2, @jupyterlab/ui-components@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/ui-components@npm:4.0.0-rc.0"
+"@jupyterlab/ui-components@npm:^4.0.0, @jupyterlab/ui-components@npm:^4.0.0-alpha.33":
+  version: 4.0.0
+  resolution: "@jupyterlab/ui-components@npm:4.0.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/observables": ^5.0.0
+    "@jupyterlab/rendermime-interfaces": ^3.8.0
+    "@jupyterlab/translation": ^4.0.0
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
@@ -1170,15 +1100,15 @@
     "@rjsf/core": ^5.1.0
     "@rjsf/utils": ^5.1.0
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: b6c01808b0e02e4289aca18c62967c0bde1f380954fa4342274cf692d0d4615df371e19e19a63bf3419fa690d23ba87fc92f78ecabedf36a8c19702d6dc14f3f
+  checksum: 781a5b48acc16a098f9f88ec4cc840912100da96f9d1f64c93cd5fdb9afddd33bbeb891d0a6383ee8f12f001056d9c0beabded2a99a05d374dcf7d952e784e40
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2":
   version: 1.0.2
   resolution: "@lezer/common@npm:1.0.2"
   checksum: bbcc58e07be02652bf0700d2856042ec089d5be0b95893d628b3e18192ade864fac83b61b19653e10b9f1472261a178b12318d934e9004edd5483a577c0db56b
@@ -1192,20 +1122,20 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 9b25c881fc9b64fd2b019a077a85b0ba7cfda0bbdd92dbb0ff43300c9ba1ec4360128fe912bfe0f06a1c1bb5a564c5ace375c8aad254d07a717768a8f268695d
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.1
-  resolution: "@lezer/css@npm:1.1.1"
+  version: 1.1.2
+  resolution: "@lezer/css@npm:1.1.2"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: a7e4893aacaa7f26d5679c77a640f401b37d14155cb54863aa91b59dfd220b280360a341c0fedafc65d31101de13a5ae33cf3876c352f2da528344dafdc9b3d7
+  checksum: 02218fe6901428e191a91a1f1a3728a051af982bafaf37144884c9261a7e24b2ad1dfdaa6e7feeb160e5bc34157ce92213cd92ae244cdf0b8485b8b8113850f8
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
   version: 1.2.3
   resolution: "@lezer/generator@npm:1.2.3"
   dependencies:
@@ -1214,19 +1144,19 @@
   bin:
     lezer-generator: dist/lezer-generator.cjs
   checksum: 300edf525f15ff27b84c366f1e9e66d741222f4b206cf015851679d7d153f5653b205ed9c3241f8df225eb97cefc99207343e148fe26bf2c4f636a00839976a8
   languageName: node
   linkType: hard
 
 "@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
-  version: 1.1.4
-  resolution: "@lezer/highlight@npm:1.1.4"
+  version: 1.1.5
+  resolution: "@lezer/highlight@npm:1.1.5"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 30e848c02839bfcd9472fcd6e74d71cba12379cef38f27d0c6cab0e6831f92150cfc629d267a40cc31f84cf46ac0a935400163fdf931b2672c516bec29417485
+  checksum: 1f0b0a3dc7e1f23d889ce7a61d9ce1ba4d3b307205baf58f97252588df4c6751e4c86d39c20cd0bc7ac39ab82ff78a9251db91148b3b069965ec55d5fe9c4ef5
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
   version: 1.3.4
   resolution: "@lezer/html@npm:1.3.4"
   dependencies:
@@ -1272,15 +1202,15 @@
   resolution: "@lezer/lr@npm:1.3.4"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 58bc25a9ba891dc6ca713fc8768706935e65d6e54d79a8ddb40c742cc799e87eddf4f49a6d6566a649c4726a9ab79a4200d36c9351608285a9bee6cdf3b33341
   languageName: node
   linkType: hard
 
-"@lezer/markdown@npm:^1.0.0":
+"@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
   version: 1.0.2
   resolution: "@lezer/markdown@npm:1.0.2"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
   checksum: c4bbfcd8a5a9d924a7cf2b5e5e99c78e7705473cc59804070278b5cfcf478af9dd567025d0926cbf03e3ea6abb8f173425220d3107c05a2d7e0ca3fe3d5c92ef
   languageName: node
@@ -1293,20 +1223,20 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
   checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.0.0":
-  version: 1.1.5
-  resolution: "@lezer/python@npm:1.1.5"
+  version: 1.1.6
+  resolution: "@lezer/python@npm:1.1.6"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 0327b90d18135bcc6e0b13369074f6e4cbc3204f6b91e0ffac674a2f8e4d32a0ecb7450fa0974c066018f09ec4be2c6568a0fac219336696188363a8cf1c92a3
+  checksum: 3a75790816612c7da6dfd95cf40ab3c6a2c9864d18170eae7ba933c09c9e0a7527a48a477a6b54b4cce85fd874d04af6a0b25713897ebe035eebc929cb66f125
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
   version: 1.0.0
   resolution: "@lezer/rust@npm:1.0.0"
   dependencies:
@@ -1380,37 +1310,37 @@
     "@lumino/keyboard": ^1.8.2
     "@lumino/signaling": ^1.11.1
     "@lumino/virtualdom": ^1.14.3
   checksum: 1e2ee7ce14b7241aee829df76f2bee6c046a82c2c137c6bb58049142c52a67f8ae74168fdcc4027b0d5a1c9f2ffa8b8f5231ef89f6f0ea8dcc4cab8d475e1ad4
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.1.0, @lumino/commands@npm:^2.1.1":
+"@lumino/commands@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/commands@npm:2.1.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/keyboard": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
   checksum: a076244e9c4f7a3c6dab02642fdd38dbbaab6e5754acaeeb84a5195dc5c2fc19343ba754c3a0f89c9b60f16c61cb793301cdb6e8d69bdc30e18ed7e32f40d524
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^2.1.0":
+"@lumino/coreutils@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/coreutils@npm:2.1.1"
   checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/disposable@npm:^2.0.0-alpha.6, @lumino/disposable@npm:^2.1.1":
+"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/disposable@npm:2.1.1"
   dependencies:
     "@lumino/signaling": ^2.1.1
   checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
   languageName: node
   linkType: hard
@@ -1525,15 +1455,15 @@
 "@lumino/properties@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/properties@npm:2.0.0"
   checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/signaling@npm:^2.0.0-alpha.6, @lumino/signaling@npm:^2.1.0, @lumino/signaling@npm:^2.1.1":
+"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/signaling@npm:2.1.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
   checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
   languageName: node
@@ -1582,15 +1512,15 @@
     "@lumino/properties": ^1.8.2
     "@lumino/signaling": ^1.11.1
     "@lumino/virtualdom": ^1.14.3
   checksum: 3193f8cca4bad2c9d59031515b7b81b8a3655088f2b8c4f69f575116140d45c5caed935da0ed3fab9dc5ce96fde037bfa5fef0c129921955b3fb73cf725d1b06
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^2.0.0-alpha.6, @lumino/widgets@npm:^2.1.0, @lumino/widgets@npm:^2.1.1":
+"@lumino/widgets@npm:^2.0.0-alpha.6, @lumino/widgets@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/widgets@npm:2.1.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
@@ -1628,69 +1558,42 @@
   dependencies:
     "@nodelib/fs.scandir": 2.1.5
     fastq: ^1.6.0
   checksum: 190c643f156d8f8f277bf2a6078af1ffde1fd43f498f187c2db24d35b4b4b5785c02c7dc52e356497b9a1b65b13edc996de08de0b961c32844364da02986dc53
   languageName: node
   linkType: hard
 
-"@npmcli/fs@npm:^2.1.0":
-  version: 2.1.2
-  resolution: "@npmcli/fs@npm:2.1.2"
-  dependencies:
-    "@gar/promisify": ^1.1.3
-    semver: ^7.3.5
-  checksum: 405074965e72d4c9d728931b64d2d38e6ea12066d4fad651ac253d175e413c06fe4350970c783db0d749181da8fe49c42d3880bd1cbc12cd68e3a7964d820225
-  languageName: node
-  linkType: hard
-
-"@npmcli/move-file@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "@npmcli/move-file@npm:2.0.1"
-  dependencies:
-    mkdirp: ^1.0.4
-    rimraf: ^3.0.2
-  checksum: 52dc02259d98da517fae4cb3a0a3850227bdae4939dda1980b788a7670636ca2b4a01b58df03dd5f65c1e3cb70c50fa8ce5762b582b3f499ec30ee5ce1fd9380
-  languageName: node
-  linkType: hard
-
 "@rjsf/core@npm:^5.1.0":
-  version: 5.6.2
-  resolution: "@rjsf/core@npm:5.6.2"
+  version: 5.7.2
+  resolution: "@rjsf/core@npm:5.7.2"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.2.0
     nanoid: ^3.3.6
     prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": 5.6.x
+    "@rjsf/utils": 5.7.x
     react: ^16.14.0 || >=17
-  checksum: 8cc9c1a439fcb232be66464aa1bc370b49dc0f872ae09cca296adf07ea993cb8dbec366c26414ff2ea92490f89fafd39ca5fb2369b424ff0035cbf045de44927
+  checksum: a2c40a71db35b4609a41bebb173060ff0fdab7007cbd1fe6f958e50fb15b2ecef4f0d63648d882b5af59b35327c1d92c34178f1609c5b9d9f7ca77b2704ca427
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.6.2
-  resolution: "@rjsf/utils@npm:5.6.2"
+  version: 5.7.2
+  resolution: "@rjsf/utils@npm:5.7.2"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: f6ab90d2cf383f8f7d14ba70f51b2e0171997aeee1f822115734ec39d0f208477374046e4cc2b4cbabe544f8bb6a6250f0bd5fb9e9470aae876a0896eabfa23e
-  languageName: node
-  linkType: hard
-
-"@tootallnate/once@npm:2":
-  version: 2.0.0
-  resolution: "@tootallnate/once@npm:2.0.0"
-  checksum: ad87447820dd3f24825d2d947ebc03072b20a42bfc96cbafec16bff8bbda6c1a81fcb0be56d5b21968560c5359a0af4038a68ba150c3e1694fe4c109a063bed8
+  checksum: 77dd1365b509fb246094dbb20c02917788fea0ff18b3afd7dcc2f9330b6310a3ca5e1d7983e8eee56c0734ebd45bc110e862b9366ef9616fad351304d514262a
   languageName: node
   linkType: hard
 
 "@types/backbone@npm:1.4.14":
   version: 1.4.14
   resolution: "@types/backbone@npm:1.4.14"
   dependencies:
@@ -1707,20 +1610,20 @@
     "@types/eslint": "*"
     "@types/estree": "*"
   checksum: ea6a9363e92f301cd3888194469f9ec9d0021fe0a397a97a6dd689e7545c75de0bd2153dfb13d3ab532853a278b6572c6f678ce846980669e41029d205653460
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.37.0
-  resolution: "@types/eslint@npm:8.37.0"
+  version: 8.40.0
+  resolution: "@types/eslint@npm:8.40.0"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 06d3b3fba12004294591b5c7a52e3cec439472195da54e096076b1f2ddfbb8a445973b9681046dd530a6ac31eca502f635abc1e3ce37d03513089358e6f822ee
+  checksum: bab41d7f590182e743853cdd5bf5359cbc4240df986223457c8a5f5674743a3fe2a8626704b65bf9121dfa0ce0a0efd760da8339cc329018f229d4d2d6ee1c43
   languageName: node
   linkType: hard
 
 "@types/estree@npm:*, @types/estree@npm:^1.0.0":
   version: 1.0.1
   resolution: "@types/estree@npm:1.0.1"
   checksum: e9aa175eacb797216fafce4d41e8202c7a75555bc55232dee0f9903d7171f8f19f0ae7d5191bb1a88cb90e65468be508c0df850a9fb81b4433b293a5a749899d
@@ -1747,42 +1650,42 @@
   version: 4.14.194
   resolution: "@types/lodash@npm:4.14.194"
   checksum: 113f34831c461469d91feca2dde737f88487732898b4d25e9eb23b087bb193985f864d1e1e0f3b777edc5022e460443588b6000a3b2348c966f72d17eedc35ea
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 18.16.2
-  resolution: "@types/node@npm:18.16.2"
-  checksum: 7ad66d23b3b93885a9f879bff98e0196790ad35589b47a3d81b52db969ad17ee298082020296df5166c2d72d3cd6a4b9ab34d254483637d967944a4b3e6febdb
+  version: 20.2.3
+  resolution: "@types/node@npm:20.2.3"
+  checksum: 576065e8fc1fa45798c8f59a6bf809169582d04abc2e25fab1a048ffc734975b9992ae31be0d960cf705a21fb37112f7fcde11aa322beddf7491e73d5a5a988c
   languageName: node
   linkType: hard
 
 "@types/node@npm:^16.11.10":
-  version: 16.18.25
-  resolution: "@types/node@npm:16.18.25"
-  checksum: 181760ad6b54fcc498dfeb249e98bbf0be51d7c35e92e760e1a82004fa42b86e8c33a8f8dd7743b5ef872bda0753d9e6a5b8e3f0aed63e9eb79b4e65760c1fbe
+  version: 16.18.32
+  resolution: "@types/node@npm:16.18.32"
+  checksum: c5966c8e671205b2971ae66ae548ce92235cef89ae1a0f2ecbf118e775923259dc85f57c58cfc56267089d56dfce967700c058276199c6ed9510d0a0b077af2d
   languageName: node
   linkType: hard
 
 "@types/prop-types@npm:*":
   version: 15.7.5
   resolution: "@types/prop-types@npm:15.7.5"
   checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.0
-  resolution: "@types/react@npm:18.2.0"
+  version: 18.2.7
+  resolution: "@types/react@npm:18.2.7"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: db3d92b423150222a666329f7aa3023e3e942044700557b8a7d161530847e621aec9f56c9e7f71761b06dd164c8a7b17ad52355863efe80963dffa5537e8e5fd
+  checksum: caa5da4cf929766738ec789301dc6fb6624bd48dd317d851c4c9b84b1f47cd8ebe17fe01398cadaa0bc938cd4d502d67f4b9de9ff771dc132096bdc86228efba
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
   version: 0.16.3
   resolution: "@types/scheduler@npm:0.16.3"
   checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
@@ -1917,195 +1820,195 @@
   dependencies:
     "@typescript-eslint/types": 4.33.0
     eslint-visitor-keys: ^2.0.0
   checksum: 59953e474ad4610c1aa23b2b1a964445e2c6201521da6367752f37939d854352bbfced5c04ea539274065e012b1337ba3ffa49c2647a240a4e87155378ba9873
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ast@npm:1.11.5, @webassemblyjs/ast@npm:^1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/ast@npm:1.11.5"
+"@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/ast@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/helper-numbers": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-  checksum: 7df16d8d4364d40e2506776330f8114fddc6494e6e18e8d5ec386312a0881a564cef136b0a74cc4a6ba284e2ff6bad890ddc029a0ba6cf45cc15186e638db118
+    "@webassemblyjs/helper-numbers": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+  checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
   languageName: node
   linkType: hard
 
-"@webassemblyjs/floating-point-hex-parser@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.5"
-  checksum: a6f35e3035a1ec4e446fa43da01539f3ed7e0f4b53d152f36ff34be1b63b08d86c4b09b6af375c95472a75f0c37b3b98b07199d157e767b8b3274e7a3962890c
+"@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
+  checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-api-error@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-api-error@npm:1.11.5"
-  checksum: 717a6ffb3283bd24a7b74710c9bd3d71ec331a26c15446441af19fae9f087e36acb8dcf25b900b6897a1d1eff838e463fe678d66281e7eccee9a3ac0e3447372
+"@webassemblyjs/helper-api-error@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
+  checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.5"
-  checksum: 2c0925b1c3c9b115c183b88d9cf1a12e87fa4fc83ef985aa2a65d72cda543eba6b73b378d231b4feb810b17d3aa6cd297bd603199854346f8a50e3458d7ebbc0
+"@webassemblyjs/helper-buffer@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
+  checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-numbers@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-numbers@npm:1.11.5"
+"@webassemblyjs/helper-numbers@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/floating-point-hex-parser": 1.11.5
-    "@webassemblyjs/helper-api-error": 1.11.5
+    "@webassemblyjs/floating-point-hex-parser": 1.11.6
+    "@webassemblyjs/helper-api-error": 1.11.6
     "@xtuc/long": 4.2.2
-  checksum: 49c8bbf561d4df38009e38e6357c396f4454773fd31a03579a8e050a2b28053f5c47f675f00a37f79a65082c938c2159fa603049688ac01b1bafdb472c21110c
+  checksum: f4b562fa219f84368528339e0f8d273ad44e047a07641ffcaaec6f93e5b76fd86490a009aa91a294584e1436d74b0a01fa9fde45e333a4c657b58168b04da424
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-bytecode@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.5"
-  checksum: 4e868de92587e131a7f22bc4eb44eee60c178d4c2c3eeabcb973b4eac73ec477f25d5f838394797265dbe4b600e781c6e150c762a45f249b94bf0711e73409a7
+"@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
+  checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.5"
+"@webassemblyjs/helper-wasm-section@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-buffer": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/wasm-gen": 1.11.5
-  checksum: 1752d7e0dbbf236a5cdc2257e1626a3562bfb0a7d2e967dc5e798c73088f18f20a991491565e2ffee61615f08035b4760e7aa080380bb60b86b393b6eb7486ae
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+  checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ieee754@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/ieee754@npm:1.11.5"
+"@webassemblyjs/ieee754@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
     "@xtuc/ieee754": ^1.2.0
-  checksum: 68a855a3e3dd488fff4d2d100e491cb6ac07f728c9432f3216b8e1bb0a374b397b0a5f58fd3b71195e525d49c0c827db15c18897e1c220c629e759b19978e64c
+  checksum: 13574b8e41f6ca39b700e292d7edf102577db5650fe8add7066a320aa4b7a7c09a5056feccac7a74eb68c10dea9546d4461412af351f13f6b24b5f32379b49de
   languageName: node
   linkType: hard
 
-"@webassemblyjs/leb128@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/leb128@npm:1.11.5"
+"@webassemblyjs/leb128@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/leb128@npm:1.11.6"
   dependencies:
     "@xtuc/long": 4.2.2
-  checksum: 555314708b6615c203c31a9dd810141c6de728e0043c2169ca69905ccf4d8603102994cb74ac5d057ac229bfc2be40f69cad2edd134ef2b909ef694eefe7bba6
+  checksum: 7ea942dc9777d4b18a5ebfa3a937b30ae9e1d2ce1fee637583ed7f376334dd1d4274f813d2e250056cca803e0952def4b954913f1a3c9068bcd4ab4ee5143bf0
   languageName: node
   linkType: hard
 
-"@webassemblyjs/utf8@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/utf8@npm:1.11.5"
-  checksum: d8f67a5650d9bf26810da76e72d0547211a44f30f35657953f547e08185facb39ff326920bddec96d35b5cc65e4e66b1f23c6461847e2f93fad2a60b0bb20211
+"@webassemblyjs/utf8@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/utf8@npm:1.11.6"
+  checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
 "@webassemblyjs/wasm-edit@npm:^1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.5"
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-buffer": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/helper-wasm-section": 1.11.5
-    "@webassemblyjs/wasm-gen": 1.11.5
-    "@webassemblyjs/wasm-opt": 1.11.5
-    "@webassemblyjs/wasm-parser": 1.11.5
-    "@webassemblyjs/wast-printer": 1.11.5
-  checksum: 790142a1e282848201c7b68860aabc0141ee44a98a62c3f0af05f8de3cc69b439c3af54ae9a06acbbfbf7fd192b30ee97fb31eda3e08973cae373534ad2135c7
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/helper-wasm-section": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+    "@webassemblyjs/wasm-opt": 1.11.6
+    "@webassemblyjs/wasm-parser": 1.11.6
+    "@webassemblyjs/wast-printer": 1.11.6
+  checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.5"
+"@webassemblyjs/wasm-gen@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/ieee754": 1.11.5
-    "@webassemblyjs/leb128": 1.11.5
-    "@webassemblyjs/utf8": 1.11.5
-  checksum: 0122df4e5ce52d873f19f34b3ebe8237072e9e6a69667cbec42a2d98ba49f85ea2ed3d935195e6a7ad4f64b9dd7da42883f057fe1103d2062bc90f3428b063fe
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/ieee754": 1.11.6
+    "@webassemblyjs/leb128": 1.11.6
+    "@webassemblyjs/utf8": 1.11.6
+  checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.5"
+"@webassemblyjs/wasm-opt@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-buffer": 1.11.5
-    "@webassemblyjs/wasm-gen": 1.11.5
-    "@webassemblyjs/wasm-parser": 1.11.5
-  checksum: f9416b0dece071e308616fb30e560f0c3c53b5bb23cc4409781b8c47d31e935b27e9a248c65aee9dd9136271e37a4c5cb0971b27e5adf623020fbb298423fe55
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+    "@webassemblyjs/wasm-parser": 1.11.6
+  checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.5, @webassemblyjs/wasm-parser@npm:^1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.5"
+"@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-api-error": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/ieee754": 1.11.5
-    "@webassemblyjs/leb128": 1.11.5
-    "@webassemblyjs/utf8": 1.11.5
-  checksum: 094b3df07532cd2a1db91710622cbaf3d7467a361f9f73dc564999385a472fcc08497d8ccf9294bd7c8813d5e2056c06a81e032abb60520168899605fde9b12c
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-api-error": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/ieee754": 1.11.6
+    "@webassemblyjs/leb128": 1.11.6
+    "@webassemblyjs/utf8": 1.11.6
+  checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.5"
+"@webassemblyjs/wast-printer@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
+    "@webassemblyjs/ast": 1.11.6
     "@xtuc/long": 4.2.2
-  checksum: c2995224c56b403be7fce7afbb3ad6b2ceadce07a47b28bce745eabb0435fa363c0180bca907d28703ece02422d0de219e689253b55de288c79b8f92416c1d71
+  checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
   languageName: node
   linkType: hard
 
-"@webpack-cli/configtest@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@webpack-cli/configtest@npm:2.0.1"
+"@webpack-cli/configtest@npm:^2.1.0":
+  version: 2.1.0
+  resolution: "@webpack-cli/configtest@npm:2.1.0"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
-  checksum: 15d0ca835f2e16ec99e9f295f07b676435b9e706d7700df0ad088692fea065e34772fc44b96a4f6a86178b9ca8cf1ff941fbce15269587cf0925d70b18928cea
+  checksum: b875fccd8be9a936924e24986725823347703e3eb72ea884e74669ca20f007704e859855a6a05940d5d3805ce2fc08b183a0f1658d5395b5454b3f5f88293081
   languageName: node
   linkType: hard
 
 "@webpack-cli/info@npm:^2.0.1":
   version: 2.0.1
   resolution: "@webpack-cli/info@npm:2.0.1"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
   checksum: b8fba49fee10d297c2affb0b064c9a81e9038d75517c6728fb85f9fb254cae634e5d33e696dac5171e6944ae329d85fddac72f781c7d833f7e9dfe43151ce60d
   languageName: node
   linkType: hard
 
-"@webpack-cli/serve@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "@webpack-cli/serve@npm:2.0.2"
+"@webpack-cli/serve@npm:^2.0.4":
+  version: 2.0.4
+  resolution: "@webpack-cli/serve@npm:2.0.4"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
   peerDependenciesMeta:
     webpack-dev-server:
       optional: true
-  checksum: f74c8cc7d3e4de58e1261c6d09af0e8b8a23f53ada4ec336140f30fa16d57d9f56de954e87125947c090c06a30b10a243ca1e093c3e4bd60ba3f19c852cb20b7
+  checksum: 561ea2e6eb551415f0b1675393a8480e1201293fe37eae334cbb1fdc466986668cca76ca1ca327ada9b498eae27cbecef0793e3bb5677288f1a5216cad414efe
   languageName: node
   linkType: hard
 
 "@xtuc/ieee754@npm:^1.2.0":
   version: 1.2.0
   resolution: "@xtuc/ieee754@npm:1.2.0"
   checksum: ac56d4ca6e17790f1b1677f978c0c6808b1900a5b138885d3da21732f62e30e8f0d9120fcf8f6edfff5100ca902b46f8dd7c1e3f903728634523981e80e2885a
@@ -2122,53 +2025,20 @@
 "abab@npm:^2.0.3, abab@npm:^2.0.5":
   version: 2.0.6
   resolution: "abab@npm:2.0.6"
   checksum: 6ffc1af4ff315066c62600123990d87551ceb0aafa01e6539da77b0f5987ac7019466780bf480f1787576d4385e3690c81ccc37cfda12819bf510b8ab47e5a3e
   languageName: node
   linkType: hard
 
-"abbrev@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "abbrev@npm:1.1.1"
-  checksum: a4a97ec07d7ea112c517036882b2ac22f3109b7b19077dc656316d07d308438aac28e4d9746dc4d84bf6b1e75b4a7b0a5f3cb30592419f128ca9a8cee3bcfa17
-  languageName: node
-  linkType: hard
-
-"abstract-leveldown@npm:^6.2.1":
-  version: 6.3.0
-  resolution: "abstract-leveldown@npm:6.3.0"
-  dependencies:
-    buffer: ^5.5.0
-    immediate: ^3.2.3
-    level-concat-iterator: ~2.0.0
-    level-supports: ~1.0.0
-    xtend: ~4.0.0
-  checksum: 121a8509d8c6a540e656c2a69e5b8d853d4df71072011afefc868b98076991bb00120550e90643de9dc18889c675f62413409eeb4c8c204663124c7d215e4ec3
-  languageName: node
-  linkType: hard
-
-"abstract-leveldown@npm:~6.2.1, abstract-leveldown@npm:~6.2.3":
-  version: 6.2.3
-  resolution: "abstract-leveldown@npm:6.2.3"
-  dependencies:
-    buffer: ^5.5.0
-    immediate: ^3.2.3
-    level-concat-iterator: ~2.0.0
-    level-supports: ~1.0.0
-    xtend: ~4.0.0
-  checksum: 00202b2eb7955dd7bc04f3e44d225e60160cedb8f96fe6ae0e6dca9c356d57071f001ece8ae1d53f48095c4c036d92b3440f2bc7666730610ddea030f9fbde4a
-  languageName: node
-  linkType: hard
-
-"acorn-import-assertions@npm:^1.7.6":
-  version: 1.8.0
-  resolution: "acorn-import-assertions@npm:1.8.0"
+"acorn-import-assertions@npm:^1.9.0":
+  version: 1.9.0
+  resolution: "acorn-import-assertions@npm:1.9.0"
   peerDependencies:
     acorn: ^8
-  checksum: 5c4cf7c850102ba7ae0eeae0deb40fb3158c8ca5ff15c0bca43b5c47e307a1de3d8ef761788f881343680ea374631ae9e9615ba8876fee5268dbe068c98bcba6
+  checksum: 944fb2659d0845c467066bdcda2e20c05abe3aaf11972116df457ce2627628a81764d800dd55031ba19de513ee0d43bb771bc679cc0eda66dc8b4fade143bc0c
   languageName: node
   linkType: hard
 
 "acorn-jsx@npm:^5.3.1":
   version: 5.3.2
   resolution: "acorn-jsx@npm:5.3.2"
   peerDependencies:
@@ -2191,44 +2061,14 @@
   resolution: "acorn@npm:8.8.2"
   bin:
     acorn: bin/acorn
   checksum: f790b99a1bf63ef160c967e23c46feea7787e531292bb827126334612c234ed489a0dc2c7ba33156416f0ffa8d25bf2b0fdb7f35c2ba60eb3e960572bece4001
   languageName: node
   linkType: hard
 
-"agent-base@npm:6, agent-base@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "agent-base@npm:6.0.2"
-  dependencies:
-    debug: 4
-  checksum: f52b6872cc96fd5f622071b71ef200e01c7c4c454ee68bc9accca90c98cfb39f2810e3e9aa330435835eedc8c23f4f8a15267f67c6e245d2b33757575bdac49d
-  languageName: node
-  linkType: hard
-
-"agentkeepalive@npm:^4.2.1":
-  version: 4.3.0
-  resolution: "agentkeepalive@npm:4.3.0"
-  dependencies:
-    debug: ^4.1.0
-    depd: ^2.0.0
-    humanize-ms: ^1.2.1
-  checksum: 982453aa44c11a06826c836025e5162c846e1200adb56f2d075400da7d32d87021b3b0a58768d949d824811f5654223d5a8a3dad120921a2439625eb847c6260
-  languageName: node
-  linkType: hard
-
-"aggregate-error@npm:^3.0.0":
-  version: 3.1.0
-  resolution: "aggregate-error@npm:3.1.0"
-  dependencies:
-    clean-stack: ^2.0.0
-    indent-string: ^4.0.0
-  checksum: 1101a33f21baa27a2fa8e04b698271e64616b886795fd43c31068c07533c7b3facfcaf4e9e0cab3624bd88f729a592f1c901a1a229c9e490eafce411a8644b79
-  languageName: node
-  linkType: hard
-
 "ajv-formats@npm:^2.1.1":
   version: 2.1.1
   resolution: "ajv-formats@npm:2.1.1"
   dependencies:
     ajv: ^8.0.0
   peerDependencies:
     ajv: ^8.0.0
@@ -2311,31 +2151,14 @@
   resolution: "ansi-styles@npm:4.3.0"
   dependencies:
     color-convert: ^2.0.1
   checksum: 513b44c3b2105dd14cc42a19271e80f386466c4be574bccf60b627432f9198571ebf4ab1e4c3ba17347658f4ee1711c163d574248c0c1cdc2d5917a0ad582ec4
   languageName: node
   linkType: hard
 
-"aproba@npm:^1.0.3 || ^2.0.0":
-  version: 2.0.0
-  resolution: "aproba@npm:2.0.0"
-  checksum: 5615cadcfb45289eea63f8afd064ab656006361020e1735112e346593856f87435e02d8dcc7ff0d11928bc7d425f27bc7c2a84f6c0b35ab0ff659c814c138a24
-  languageName: node
-  linkType: hard
-
-"are-we-there-yet@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "are-we-there-yet@npm:3.0.1"
-  dependencies:
-    delegates: ^1.0.0
-    readable-stream: ^3.6.0
-  checksum: 52590c24860fa7173bedeb69a4c05fb573473e860197f618b9a28432ee4379049336727ae3a1f9c4cb083114601c1140cee578376164d0e651217a9843f9fe83
-  languageName: node
-  linkType: hard
-
 "argparse@npm:^1.0.7":
   version: 1.0.10
   resolution: "argparse@npm:1.0.10"
   dependencies:
     sprintf-js: ~1.0.2
   checksum: 7ca6e45583a28de7258e39e13d81e925cfa25d7d4aacbf806a382d3c02fcb13403a07fb8aeef949f10a7cfe4a62da0e2e807b348a5980554cc28ee573ef95945
   languageName: node
@@ -2368,21 +2191,14 @@
 "astral-regex@npm:^2.0.0":
   version: 2.0.0
   resolution: "astral-regex@npm:2.0.0"
   checksum: 876231688c66400473ba505731df37ea436e574dd524520294cc3bbc54ea40334865e01fa0d074d74d036ee874ee7e62f486ea38bc421ee8e6a871c06f011766
   languageName: node
   linkType: hard
 
-"async-limiter@npm:~1.0.0":
-  version: 1.0.1
-  resolution: "async-limiter@npm:1.0.1"
-  checksum: 2b849695b465d93ad44c116220dee29a5aeb63adac16c1088983c339b0de57d76e82533e8e364a93a9f997f28bbfc6a92948cefc120652bd07f3b59f8d75cf2b
-  languageName: node
-  linkType: hard
-
 "available-typed-arrays@npm:^1.0.5":
   version: 1.0.5
   resolution: "available-typed-arrays@npm:1.0.5"
   checksum: 20eb47b3cefd7db027b9bbb993c658abd36d4edd3fe1060e83699a03ee275b0c9b216cc076ff3f2db29073225fb70e7613987af14269ac1fe2a19803ccc97f1a
   languageName: node
   linkType: hard
 
@@ -2398,21 +2214,14 @@
 "balanced-match@npm:^1.0.0":
   version: 1.0.2
   resolution: "balanced-match@npm:1.0.2"
   checksum: 9706c088a283058a8a99e0bf91b0a2f75497f185980d9ffa8b304de1d9e58ebda7c72c07ebf01dadedaac5b2907b2c6f566f660d62bd336c3468e960403b9d65
   languageName: node
   linkType: hard
 
-"base64-js@npm:^1.3.1":
-  version: 1.5.1
-  resolution: "base64-js@npm:1.5.1"
-  checksum: 669632eb3745404c2f822a18fc3a0122d2f9a7a13f7fb8b5823ee19d1d2ff9ee5b52c53367176ea4ad093c332fd5ab4bd0ebae5a8e27917a4105a4cfc86b1005
-  languageName: node
-  linkType: hard
-
 "big.js@npm:^5.2.2":
   version: 5.2.2
   resolution: "big.js@npm:5.2.2"
   checksum: b89b6e8419b097a8fb4ed2399a1931a68c612bce3cfd5ca8c214b2d017531191070f990598de2fc6f3f993d91c0f08aa82697717f6b3b8732c9731866d233c9e
   languageName: node
   linkType: hard
 
@@ -2422,23 +2231,14 @@
   dependencies:
     balanced-match: ^1.0.0
     concat-map: 0.0.1
   checksum: faf34a7bb0c3fcf4b59c7808bc5d2a96a40988addf2e7e09dfbb67a2251800e0d14cd2bfc1aa79174f2f5095c54ff27f46fb1289fe2d77dac755b5eb3434cc07
   languageName: node
   linkType: hard
 
-"brace-expansion@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "brace-expansion@npm:2.0.1"
-  dependencies:
-    balanced-match: ^1.0.0
-  checksum: a61e7cd2e8a8505e9f0036b3b6108ba5e926b4b55089eeb5550cd04a471fe216c96d4fe7e4c7f995c728c554ae20ddfc4244cad10aef255e72b62930afd233d1
-  languageName: node
-  linkType: hard
-
 "braces@npm:^3.0.2":
   version: 3.0.2
   resolution: "braces@npm:3.0.2"
   dependencies:
     fill-range: ^7.0.1
   checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
   languageName: node
@@ -2461,50 +2261,14 @@
 "buffer-from@npm:^1.0.0":
   version: 1.1.2
   resolution: "buffer-from@npm:1.1.2"
   checksum: 0448524a562b37d4d7ed9efd91685a5b77a50672c556ea254ac9a6d30e3403a517d8981f10e565db24e8339413b43c97ca2951f10e399c6125a0d8911f5679bb
   languageName: node
   linkType: hard
 
-"buffer@npm:^5.5.0, buffer@npm:^5.6.0":
-  version: 5.7.1
-  resolution: "buffer@npm:5.7.1"
-  dependencies:
-    base64-js: ^1.3.1
-    ieee754: ^1.1.13
-  checksum: e2cf8429e1c4c7b8cbd30834ac09bd61da46ce35f5c22a78e6c2f04497d6d25541b16881e30a019c6fd3154150650ccee27a308eff3e26229d788bbdeb08ab84
-  languageName: node
-  linkType: hard
-
-"cacache@npm:^16.1.0":
-  version: 16.1.3
-  resolution: "cacache@npm:16.1.3"
-  dependencies:
-    "@npmcli/fs": ^2.1.0
-    "@npmcli/move-file": ^2.0.0
-    chownr: ^2.0.0
-    fs-minipass: ^2.1.0
-    glob: ^8.0.1
-    infer-owner: ^1.0.4
-    lru-cache: ^7.7.1
-    minipass: ^3.1.6
-    minipass-collect: ^1.0.2
-    minipass-flush: ^1.0.5
-    minipass-pipeline: ^1.2.4
-    mkdirp: ^1.0.4
-    p-map: ^4.0.0
-    promise-inflight: ^1.0.1
-    rimraf: ^3.0.2
-    ssri: ^9.0.0
-    tar: ^6.1.11
-    unique-filename: ^2.0.0
-  checksum: d91409e6e57d7d9a3a25e5dcc589c84e75b178ae8ea7de05cbf6b783f77a5fae938f6e8fda6f5257ed70000be27a681e1e44829251bfffe4c10216002f8f14e6
-  languageName: node
-  linkType: hard
-
 "call-bind@npm:^1.0.0, call-bind@npm:^1.0.2":
   version: 1.0.2
   resolution: "call-bind@npm:1.0.2"
   dependencies:
     function-bind: ^1.1.1
     get-intrinsic: ^1.0.2
   checksum: f8e31de9d19988a4b80f3e704788c4a2d6b6f3d17cfec4f57dc29ced450c53a49270dc66bf0fbd693329ee948dd33e6c90a329519aef17474a4d961e8d6426b0
@@ -2515,17 +2279,17 @@
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001449":
-  version: 1.0.30001481
-  resolution: "caniuse-lite@npm:1.0.30001481"
-  checksum: 8200a043c191b4fd4fe0beda37a58fd61869c895ab93f87bdd0420e5927453f48434d716ce9da8552ff6c3ecc4dcd1366354cda3a134f3cc844af741574a7cab
+  version: 1.0.30001489
+  resolution: "caniuse-lite@npm:1.0.30001489"
+  checksum: 94585a351fd7661b855c83eace474db0ee5a617159b46f2eff1f6fe4b85d7a205418471fdec8cf5cd647a7f79958706d5e664c0bbf3c7c09118b35db9bb95a1b
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.0.0, chalk@npm:^2.3.0, chalk@npm:^2.4.1":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -2542,35 +2306,21 @@
   dependencies:
     ansi-styles: ^4.1.0
     supports-color: ^7.1.0
   checksum: fe75c9d5c76a7a98d45495b91b2172fa3b7a09e0cc9370e5c8feb1c567b85c4288e2b3fded7cfdd7359ac28d6b3844feb8b82b8686842e93d23c827c417e83fc
   languageName: node
   linkType: hard
 
-"chownr@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "chownr@npm:2.0.0"
-  checksum: c57cf9dd0791e2f18a5ee9c1a299ae6e801ff58fee96dc8bfd0dcb4738a6ce58dd252a3605b1c93c6418fe4f9d5093b28ffbf4d66648cb2a9c67eaef9679be2f
-  languageName: node
-  linkType: hard
-
 "chrome-trace-event@npm:^1.0.2":
   version: 1.0.3
   resolution: "chrome-trace-event@npm:1.0.3"
   checksum: cb8b1fc7e881aaef973bd0c4a43cd353c2ad8323fb471a041e64f7c2dd849cde4aad15f8b753331a32dda45c973f032c8a03b8177fc85d60eaa75e91e08bfb97
   languageName: node
   linkType: hard
 
-"clean-stack@npm:^2.0.0":
-  version: 2.2.0
-  resolution: "clean-stack@npm:2.2.0"
-  checksum: 2ac8cd2b2f5ec986a3c743935ec85b07bc174d5421a5efc8017e1f146a1cf5f781ae962618f416352103b32c9cd7e203276e8c28241bbe946160cab16149fb68
-  languageName: node
-  linkType: hard
-
 "clone-deep@npm:^4.0.1":
   version: 4.0.1
   resolution: "clone-deep@npm:4.0.1"
   dependencies:
     is-plain-object: ^2.0.4
     kind-of: ^6.0.2
     shallow-clone: ^3.0.0
@@ -2606,23 +2356,14 @@
 "color-name@npm:~1.1.4":
   version: 1.1.4
   resolution: "color-name@npm:1.1.4"
   checksum: b0445859521eb4021cd0fb0cc1a75cecf67fceecae89b63f62b201cca8d345baf8b952c966862a9d9a2632987d4f6581f0ec8d957dfacece86f0a7919316f610
   languageName: node
   linkType: hard
 
-"color-support@npm:^1.1.3":
-  version: 1.1.3
-  resolution: "color-support@npm:1.1.3"
-  bin:
-    color-support: bin.js
-  checksum: 9b7356817670b9a13a26ca5af1c21615463b500783b739b7634a0c2047c16cef4b2865d7576875c31c3cddf9dd621fa19285e628f20198b233a5cfdda6d0793b
-  languageName: node
-  linkType: hard
-
 "colorette@npm:^2.0.14":
   version: 2.0.20
   resolution: "colorette@npm:2.0.20"
   checksum: 0c016fea2b91b733eb9f4bcdb580018f52c0bc0979443dad930e5037a968237ac53d9beb98e218d2e9235834f8eebce7f8e080422d6194e957454255bde71d3d
   languageName: node
   linkType: hard
 
@@ -2673,21 +2414,14 @@
 "concat-map@npm:0.0.1":
   version: 0.0.1
   resolution: "concat-map@npm:0.0.1"
   checksum: 902a9f5d8967a3e2faf138d5cb784b9979bad2e6db5357c5b21c568df4ebe62bcb15108af1b2253744844eb964fc023fbd9afbbbb6ddd0bcc204c6fb5b7bf3af
   languageName: node
   linkType: hard
 
-"console-control-strings@npm:^1.1.0":
-  version: 1.1.0
-  resolution: "console-control-strings@npm:1.1.0"
-  checksum: 8755d76787f94e6cf79ce4666f0c5519906d7f5b02d4b884cf41e11dcd759ed69c57da0670afd9236d229a46e0f9cf519db0cd829c6dca820bb5a5c3def584ed
-  languageName: node
-  linkType: hard
-
 "copy-webpack-plugin@npm:^10.0.0":
   version: 10.2.4
   resolution: "copy-webpack-plugin@npm:10.2.4"
   dependencies:
     fast-glob: ^3.2.7
     glob-parent: ^6.0.1
     globby: ^12.0.2
@@ -2697,17 +2431,17 @@
   peerDependencies:
     webpack: ^5.1.0
   checksum: 87f0f4530ab3e58ec06a7c3182028dfd8cc85b045a0d18c4464caafeae1ed1141c2aad6eae37e100a74a72b69dc48c93af358c07038b7a22f490a678c0ab142e
   languageName: node
   linkType: hard
 
 "crelt@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "crelt@npm:1.0.5"
-  checksum: 04a618c5878e12a14a9a328a49ff6e37bed76abb88b72e661c56b5f161d8a9aca133650da6bcbc5224ad1f7f43a69325627f209e92a21002986d52a8f844b367
+  version: 1.0.6
+  resolution: "crelt@npm:1.0.6"
+  checksum: dad842093371ad702afbc0531bfca2b0a8dd920b23a42f26e66dabbed9aad9acd5b9030496359545ef3937c3aced0fd4ac39f7a2d280a23ddf9eb7fdcb94a69f
   languageName: node
   linkType: hard
 
 "cross-spawn@npm:^6.0.5":
   version: 6.0.5
   resolution: "cross-spawn@npm:6.0.5"
   dependencies:
@@ -2728,28 +2462,28 @@
     shebang-command: ^2.0.0
     which: ^2.0.1
   checksum: 671cc7c7288c3a8406f3c69a3ae2fc85555c04169e9d611def9a675635472614f1c0ed0ef80955d5b6d4e724f6ced67f0ad1bb006c2ea643488fcfef994d7f52
   languageName: node
   linkType: hard
 
 "css-loader@npm:^6.7.1":
-  version: 6.7.3
-  resolution: "css-loader@npm:6.7.3"
+  version: 6.7.4
+  resolution: "css-loader@npm:6.7.4"
   dependencies:
     icss-utils: ^5.1.0
-    postcss: ^8.4.19
+    postcss: ^8.4.21
     postcss-modules-extract-imports: ^3.0.0
-    postcss-modules-local-by-default: ^4.0.0
+    postcss-modules-local-by-default: ^4.0.1
     postcss-modules-scope: ^3.0.0
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
     semver: ^7.3.8
   peerDependencies:
     webpack: ^5.0.0
-  checksum: 473cc32b6c837c2848e2051ad1ba331c1457449f47442e75a8c480d9891451434ada241f7e3de2347e57de17fcd84610b3bcfc4a9da41102cdaedd1e17902d31
+  checksum: 6021fa9e375d767b9675e295c1513f2ee4ae04f76d9de69a75b8446e05f6e02b2170407ea72939925b788dcd5aa308527f6b41be3870dc1f4b0bfff8d2532c6e
   languageName: node
   linkType: hard
 
 "cssesc@npm:^3.0.0":
   version: 3.0.0
   resolution: "cssesc@npm:3.0.0"
   bin:
@@ -2779,15 +2513,15 @@
     abab: ^2.0.3
     whatwg-mimetype: ^2.3.0
     whatwg-url: ^8.0.0
   checksum: 97caf828aac25e25e04ba6869db0f99c75e6859bb5b424ada28d3e7841941ebf08ddff3c1b1bb4585986bd507a5d54c2a716853ea6cb98af877400e637393e71
   languageName: node
   linkType: hard
 
-"debug@npm:4, debug@npm:^4.0.1, debug@npm:^4.1.0, debug@npm:^4.1.1, debug@npm:^4.3.1, debug@npm:^4.3.3":
+"debug@npm:^4.0.1, debug@npm:^4.1.1, debug@npm:^4.3.1":
   version: 4.3.4
   resolution: "debug@npm:4.3.4"
   dependencies:
     ms: 2.1.2
   peerDependenciesMeta:
     supports-color:
       optional: true
@@ -2805,48 +2539,24 @@
 "deepmerge@npm:^4.2.2":
   version: 4.3.1
   resolution: "deepmerge@npm:4.3.1"
   checksum: 2024c6a980a1b7128084170c4cf56b0fd58a63f2da1660dcfe977415f27b17dbe5888668b59d0b063753f3220719d5e400b7f113609489c90160bb9a5518d052
   languageName: node
   linkType: hard
 
-"deferred-leveldown@npm:~5.3.0":
-  version: 5.3.0
-  resolution: "deferred-leveldown@npm:5.3.0"
-  dependencies:
-    abstract-leveldown: ~6.2.1
-    inherits: ^2.0.3
-  checksum: 5631e153528bb9de1aa60d59a5065d1a519374c5e4c1d486f2190dba4008dcf5c2ee8dd7f2f81396fc4d5a6bb6e7d0055e3dfe68afe00da02adaa3bf329addf7
-  languageName: node
-  linkType: hard
-
 "define-properties@npm:^1.1.3, define-properties@npm:^1.1.4, define-properties@npm:^1.2.0":
   version: 1.2.0
   resolution: "define-properties@npm:1.2.0"
   dependencies:
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
   checksum: e60aee6a19b102df4e2b1f301816804e81ab48bb91f00d0d935f269bf4b3f79c88b39e4f89eaa132890d23267335fd1140dfcd8d5ccd61031a0a2c41a54e33a6
   languageName: node
   linkType: hard
 
-"delegates@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "delegates@npm:1.0.0"
-  checksum: a51744d9b53c164ba9c0492471a1a2ffa0b6727451bdc89e31627fdf4adda9d51277cfcbfb20f0a6f08ccb3c436f341df3e92631a3440226d93a8971724771fd
-  languageName: node
-  linkType: hard
-
-"depd@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "depd@npm:2.0.0"
-  checksum: abbe19c768c97ee2eed6282d8ce3031126662252c58d711f646921c9623f9052e3e1906443066beec1095832f534e57c523b7333f8e7e0d93051ab6baef5ab3a
-  languageName: node
-  linkType: hard
-
 "dir-glob@npm:^3.0.1":
   version: 3.0.1
   resolution: "dir-glob@npm:3.0.1"
   dependencies:
     path-type: ^4.0.0
   checksum: fa05e18324510d7283f55862f3161c6759a3f2f8dbce491a2fc14c8324c498286c54282c1f0e933cb930da8419b30679389499b919122952a4f8592362ef4615
   languageName: node
@@ -2908,17 +2618,17 @@
     lodash: ^4.17.4
     semver: ^5.4.1
   checksum: d77be45cb72d79a429c64d8f8f7603fea681d182fb795459a3d4afa608faad9a923378a7e80c6855f465263e1983140b6fc3682bd0213228b8cd7906ab4b934d
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.284":
-  version: 1.4.376
-  resolution: "electron-to-chromium@npm:1.4.376"
-  checksum: 881351d25e0e983432c10844540bb664ee4c54f781b81b7247c36d6e617dc85305fd87ffb5de6d9630c6a54f4432afd8e97565a11c62bb77b63051e43cb8a942
+  version: 1.4.407
+  resolution: "electron-to-chromium@npm:1.4.407"
+  checksum: 44619c189c082953c0d12454c38aaf9c2e0226bbe4bcc2b6aef70fb5f655fd9e4e9630e2fedb256ec972327225f610ef5ddcc299c4f7f436a45ed48d1b8367f9
   languageName: node
   linkType: hard
 
 "emoji-regex@npm:^8.0.0":
   version: 8.0.0
   resolution: "emoji-regex@npm:8.0.0"
   checksum: d4c5c39d5a9868b5fa152f00cada8a936868fd3367f33f71be515ecee4c803132d11b31a6222b2571b1e5f7e13890156a94880345594d0ce7e3c9895f560f192
@@ -2928,42 +2638,21 @@
 "emojis-list@npm:^3.0.0":
   version: 3.0.0
   resolution: "emojis-list@npm:3.0.0"
   checksum: ddaaa02542e1e9436c03970eeed445f4ed29a5337dfba0fe0c38dfdd2af5da2429c2a0821304e8a8d1cadf27fdd5b22ff793571fa803ae16852a6975c65e8e70
   languageName: node
   linkType: hard
 
-"encoding-down@npm:^6.3.0":
-  version: 6.3.0
-  resolution: "encoding-down@npm:6.3.0"
-  dependencies:
-    abstract-leveldown: ^6.2.1
-    inherits: ^2.0.3
-    level-codec: ^9.0.0
-    level-errors: ^2.0.0
-  checksum: 74043e6d9061a470614ff61d708c849259ab32932a428fd5ddfb0878719804f56a52f59b31cccd95fddc2e636c0fd22dc3e02481fb98d5bf1bdbbbc44ca09bdc
-  languageName: node
-  linkType: hard
-
-"encoding@npm:^0.1.13":
-  version: 0.1.13
-  resolution: "encoding@npm:0.1.13"
-  dependencies:
-    iconv-lite: ^0.6.2
-  checksum: bb98632f8ffa823996e508ce6a58ffcf5856330fde839ae42c9e1f436cc3b5cc651d4aeae72222916545428e54fd0f6aa8862fd8d25bdbcc4589f1e3f3715e7f
-  languageName: node
-  linkType: hard
-
-"enhanced-resolve@npm:^5.0.0, enhanced-resolve@npm:^5.13.0":
-  version: 5.13.0
-  resolution: "enhanced-resolve@npm:5.13.0"
+"enhanced-resolve@npm:^5.0.0, enhanced-resolve@npm:^5.14.1":
+  version: 5.14.1
+  resolution: "enhanced-resolve@npm:5.14.1"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: 76d6844c4393d76beed5b3ce6cf5a98dee3ad5c84a9887f49ccde1224e3b7af201dfbd5a57ebf2b49f623b74883df262d50ff480d3cc02fc2881fc58b84e1bbe
+  checksum: ad2a31928b6649eed40d364838449587f731baa63863e83d2629bebaa8be1eabac18b90f89c1784bc805b0818363e99b22547159edd485d7e5ccf18cdc640642
   languageName: node
   linkType: hard
 
 "enquirer@npm:^2.3.5":
   version: 2.3.6
   resolution: "enquirer@npm:2.3.6"
   dependencies:
@@ -2975,48 +2664,23 @@
 "entities@npm:^2.0.0":
   version: 2.2.0
   resolution: "entities@npm:2.2.0"
   checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
   languageName: node
   linkType: hard
 
-"env-paths@npm:^2.2.0":
-  version: 2.2.1
-  resolution: "env-paths@npm:2.2.1"
-  checksum: 65b5df55a8bab92229ab2b40dad3b387fad24613263d103a97f91c9fe43ceb21965cd3392b1ccb5d77088021e525c4e0481adb309625d0cb94ade1d1fb8dc17e
-  languageName: node
-  linkType: hard
-
 "envinfo@npm:^7.7.3":
   version: 7.8.1
   resolution: "envinfo@npm:7.8.1"
   bin:
     envinfo: dist/cli.js
   checksum: de736c98d6311c78523628ff127af138451b162e57af5293c1b984ca821d0aeb9c849537d2fde0434011bed33f6bca5310ca2aab8a51a3f28fc719e89045d648
   languageName: node
   linkType: hard
 
-"err-code@npm:^2.0.2":
-  version: 2.0.3
-  resolution: "err-code@npm:2.0.3"
-  checksum: 8b7b1be20d2de12d2255c0bc2ca638b7af5171142693299416e6a9339bd7d88fc8d7707d913d78e0993176005405a236b066b45666b27b797252c771156ace54
-  languageName: node
-  linkType: hard
-
-"errno@npm:~0.1.1":
-  version: 0.1.8
-  resolution: "errno@npm:0.1.8"
-  dependencies:
-    prr: ~1.0.1
-  bin:
-    errno: cli.js
-  checksum: 1271f7b9fbb3bcbec76ffde932485d1e3561856d21d847ec613a9722ee924cdd4e523a62dc71a44174d91e898fe21fdc8d5b50823f4b5e0ce8c35c8271e6ef4a
-  languageName: node
-  linkType: hard
-
 "error-ex@npm:^1.3.1":
   version: 1.3.2
   resolution: "error-ex@npm:1.3.2"
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
@@ -3307,17 +2971,17 @@
   version: 3.1.3
   resolution: "fast-deep-equal@npm:3.1.3"
   checksum: e21a9d8d84f53493b6aa15efc9cfd53dd5b714a1f23f67fb5dc8f574af80df889b3bce25dc081887c6d25457cce704e636395333abad896ccdec03abaf1f3f9d
   languageName: node
   linkType: hard
 
 "fast-diff@npm:^1.1.2":
-  version: 1.2.0
-  resolution: "fast-diff@npm:1.2.0"
-  checksum: 1b5306eaa9e826564d9e5ffcd6ebd881eb5f770b3f977fcbf38f05c824e42172b53c79920e8429c54eb742ce15a0caf268b0fdd5b38f6de52234c4a8368131ae
+  version: 1.3.0
+  resolution: "fast-diff@npm:1.3.0"
+  checksum: d22d371b994fdc8cce9ff510d7b8dc4da70ac327bcba20df607dd5b9cae9f908f4d1028f5fe467650f058d1e7270235ae0b8230809a262b4df587a3b3aa216c3
   languageName: node
   linkType: hard
 
 "fast-glob@npm:^3.2.7, fast-glob@npm:^3.2.9":
   version: 3.2.12
   resolution: "fast-glob@npm:3.2.12"
   dependencies:
@@ -3447,23 +3111,14 @@
     graceful-fs: ^4.2.0
     jsonfile: ^6.0.1
     universalify: ^2.0.0
   checksum: dc94ab37096f813cc3ca12f0f1b5ad6744dfed9ed21e953d72530d103cea193c2f81584a39e9dee1bea36de5ee66805678c0dddc048e8af1427ac19c00fffc50
   languageName: node
   linkType: hard
 
-"fs-minipass@npm:^2.0.0, fs-minipass@npm:^2.1.0":
-  version: 2.1.0
-  resolution: "fs-minipass@npm:2.1.0"
-  dependencies:
-    minipass: ^3.0.0
-  checksum: 1b8d128dae2ac6cc94230cc5ead341ba3e0efaef82dab46a33d171c044caaa6ca001364178d42069b2809c35a1c3c35079a32107c770e9ffab3901b59af8c8b1
-  languageName: node
-  linkType: hard
-
 "fs.realpath@npm:^1.0.0":
   version: 1.0.0
   resolution: "fs.realpath@npm:1.0.0"
   checksum: 99ddea01a7e75aa276c250a04eedeffe5662bce66c65c07164ad6264f9de18fb21be9433ead460e54cff20e31721c811f4fb5d70591799df5f85dce6d6746fd0
   languageName: node
   linkType: hard
 
@@ -3496,38 +3151,23 @@
 "functions-have-names@npm:^1.2.2, functions-have-names@npm:^1.2.3":
   version: 1.2.3
   resolution: "functions-have-names@npm:1.2.3"
   checksum: c3f1f5ba20f4e962efb71344ce0a40722163e85bee2101ce25f88214e78182d2d2476aa85ef37950c579eb6cf6ee811c17b3101bb84004bb75655f3e33f3fdb5
   languageName: node
   linkType: hard
 
-"gauge@npm:^4.0.3":
-  version: 4.0.4
-  resolution: "gauge@npm:4.0.4"
-  dependencies:
-    aproba: ^1.0.3 || ^2.0.0
-    color-support: ^1.1.3
-    console-control-strings: ^1.1.0
-    has-unicode: ^2.0.1
-    signal-exit: ^3.0.7
-    string-width: ^4.2.3
-    strip-ansi: ^6.0.1
-    wide-align: ^1.1.5
-  checksum: 788b6bfe52f1dd8e263cda800c26ac0ca2ff6de0b6eee2fe0d9e3abf15e149b651bd27bf5226be10e6e3edb5c4e5d5985a5a1a98137e7a892f75eff76467ad2d
-  languageName: node
-  linkType: hard
-
 "get-intrinsic@npm:^1.0.2, get-intrinsic@npm:^1.1.1, get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.0":
-  version: 1.2.0
-  resolution: "get-intrinsic@npm:1.2.0"
+  version: 1.2.1
+  resolution: "get-intrinsic@npm:1.2.1"
   dependencies:
     function-bind: ^1.1.1
     has: ^1.0.3
+    has-proto: ^1.0.1
     has-symbols: ^1.0.3
-  checksum: 78fc0487b783f5c58cf2dccafc3ae656ee8d2d8062a8831ce4a95e7057af4587a1d4882246c033aca0a7b4965276f4802b45cc300338d1b77a73d3e3e3f4877d
+  checksum: 5b61d88552c24b0cf6fa2d1b3bc5459d7306f699de060d76442cce49a4721f52b8c560a33ab392cf5575b7810277d54ded9d4d39a1ea61855619ebc005aa7e5f
   languageName: node
   linkType: hard
 
 "get-stdin@npm:^6.0.0":
   version: 6.0.0
   resolution: "get-stdin@npm:6.0.0"
   checksum: 593f6fb4fff4c8d49ec93a07c430c1edc6bd4fe7e429d222b5da2f367276a98809af9e90467ad88a2d83722ff95b9b35bbaba02b56801421c5e3668173fe12b4
@@ -3565,41 +3205,28 @@
 "glob-to-regexp@npm:^0.4.1":
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
-"glob@npm:^7.1.3, glob@npm:^7.1.4":
+"glob@npm:^7.1.3":
   version: 7.2.3
   resolution: "glob@npm:7.2.3"
   dependencies:
     fs.realpath: ^1.0.0
     inflight: ^1.0.4
     inherits: 2
     minimatch: ^3.1.1
     once: ^1.3.0
     path-is-absolute: ^1.0.0
   checksum: 29452e97b38fa704dabb1d1045350fb2467cf0277e155aa9ff7077e90ad81d1ea9d53d3ee63bd37c05b09a065e90f16aec4a65f5b8de401d1dac40bc5605d133
   languageName: node
   linkType: hard
 
-"glob@npm:^8.0.1":
-  version: 8.1.0
-  resolution: "glob@npm:8.1.0"
-  dependencies:
-    fs.realpath: ^1.0.0
-    inflight: ^1.0.4
-    inherits: 2
-    minimatch: ^5.0.1
-    once: ^1.3.0
-  checksum: 92fbea3221a7d12075f26f0227abac435de868dd0736a17170663783296d0dd8d3d532a5672b4488a439bf5d7fb85cdd07c11185d6cd39184f0385cbdfb86a47
-  languageName: node
-  linkType: hard
-
 "glob@npm:~7.1.6":
   version: 7.1.7
   resolution: "glob@npm:7.1.7"
   dependencies:
     fs.realpath: ^1.0.0
     inflight: ^1.0.4
     inherits: 2
@@ -3661,15 +3288,15 @@
   resolution: "gopd@npm:1.0.1"
   dependencies:
     get-intrinsic: ^1.1.3
   checksum: a5ccfb8806e0917a94e0b3de2af2ea4979c1da920bc381667c260e00e7cafdbe844e2cb9c5bcfef4e5412e8bf73bab837285bc35c7ba73aaaf0134d4583393a6
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
+"graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.9":
   version: 4.2.11
   resolution: "graceful-fs@npm:4.2.11"
   checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
   languageName: node
   linkType: hard
 
 "has-bigints@npm:^1.0.1, has-bigints@npm:^1.0.2":
@@ -3721,21 +3348,14 @@
   resolution: "has-tostringtag@npm:1.0.0"
   dependencies:
     has-symbols: ^1.0.2
   checksum: cc12eb28cb6ae22369ebaad3a8ab0799ed61270991be88f208d508076a1e99abe4198c965935ce85ea90b60c94ddda73693b0920b58e7ead048b4a391b502c1c
   languageName: node
   linkType: hard
 
-"has-unicode@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "has-unicode@npm:2.0.1"
-  checksum: 1eab07a7436512db0be40a710b29b5dc21fa04880b7f63c9980b706683127e3c1b57cb80ea96d47991bdae2dfe479604f6a1ba410106ee1046a41d1bd0814400
-  languageName: node
-  linkType: hard
-
 "has@npm:^1.0.3":
   version: 1.0.3
   resolution: "has@npm:1.0.3"
   dependencies:
     function-bind: ^1.1.1
   checksum: b9ad53d53be4af90ce5d1c38331e712522417d017d5ef1ebd0507e07c2fbad8686fffb8e12ddecd4c39ca9b9b47431afbb975b8abf7f3c3b82c98e9aad052792
   languageName: node
@@ -3756,51 +3376,14 @@
     domhandler: ^4.0.0
     domutils: ^2.5.2
     entities: ^2.0.0
   checksum: 81a7b3d9c3bb9acb568a02fc9b1b81ffbfa55eae7f1c41ae0bf840006d1dbf54cb3aa245b2553e2c94db674840a9f0fdad7027c9a9d01a062065314039058c4e
   languageName: node
   linkType: hard
 
-"http-cache-semantics@npm:^4.1.0":
-  version: 4.1.1
-  resolution: "http-cache-semantics@npm:4.1.1"
-  checksum: 83ac0bc60b17a3a36f9953e7be55e5c8f41acc61b22583060e8dedc9dd5e3607c823a88d0926f9150e571f90946835c7fe150732801010845c72cd8bbff1a236
-  languageName: node
-  linkType: hard
-
-"http-proxy-agent@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "http-proxy-agent@npm:5.0.0"
-  dependencies:
-    "@tootallnate/once": 2
-    agent-base: 6
-    debug: 4
-  checksum: e2ee1ff1656a131953839b2a19cd1f3a52d97c25ba87bd2559af6ae87114abf60971e498021f9b73f9fd78aea8876d1fb0d4656aac8a03c6caa9fc175f22b786
-  languageName: node
-  linkType: hard
-
-"https-proxy-agent@npm:^5.0.0":
-  version: 5.0.1
-  resolution: "https-proxy-agent@npm:5.0.1"
-  dependencies:
-    agent-base: 6
-    debug: 4
-  checksum: 571fccdf38184f05943e12d37d6ce38197becdd69e58d03f43637f7fa1269cf303a7d228aa27e5b27bbd3af8f09fd938e1c91dcfefff2df7ba77c20ed8dfc765
-  languageName: node
-  linkType: hard
-
-"humanize-ms@npm:^1.2.1":
-  version: 1.2.1
-  resolution: "humanize-ms@npm:1.2.1"
-  dependencies:
-    ms: ^2.0.0
-  checksum: 9c7a74a2827f9294c009266c82031030eae811ca87b0da3dceb8d6071b9bde22c9f3daef0469c3c533cc67a97d8a167cd9fc0389350e5f415f61a79b171ded16
-  languageName: node
-  linkType: hard
-
 "iconv-lite@npm:^0.6.2, iconv-lite@npm:^0.6.3":
   version: 0.6.3
   resolution: "iconv-lite@npm:0.6.3"
   dependencies:
     safer-buffer: ">= 2.1.2 < 3.0.0"
   checksum: 3f60d47a5c8fc3313317edfd29a00a692cc87a19cac0159e2ce711d0ebc9019064108323b5e493625e25594f11c6236647d8e256fbe7a58f4a3b33b89e6d30bf
   languageName: node
@@ -3811,42 +3394,28 @@
   resolution: "icss-utils@npm:5.1.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 5c324d283552b1269cfc13a503aaaa172a280f914e5b81544f3803bc6f06a3b585fb79f66f7c771a2c052db7982c18bf92d001e3b47282e3abbbb4c4cc488d68
   languageName: node
   linkType: hard
 
-"ieee754@npm:^1.1.13":
-  version: 1.2.1
-  resolution: "ieee754@npm:1.2.1"
-  checksum: 5144c0c9815e54ada181d80a0b810221a253562422e7c6c3a60b1901154184f49326ec239d618c416c1c5945a2e197107aee8d986a3dd836b53dffefd99b5e7e
-  languageName: node
-  linkType: hard
-
 "ignore@npm:^4.0.6":
   version: 4.0.6
   resolution: "ignore@npm:4.0.6"
   checksum: 248f82e50a430906f9ee7f35e1158e3ec4c3971451dd9f99c9bc1548261b4db2b99709f60ac6c6cac9333494384176cc4cc9b07acbe42d52ac6a09cad734d800
   languageName: node
   linkType: hard
 
 "ignore@npm:^5.1.8, ignore@npm:^5.1.9, ignore@npm:^5.2.0":
   version: 5.2.4
   resolution: "ignore@npm:5.2.4"
   checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
   languageName: node
   linkType: hard
 
-"immediate@npm:^3.2.3":
-  version: 3.3.0
-  resolution: "immediate@npm:3.3.0"
-  checksum: 634b4305101e2452eba6c07d485bf3e415995e533c94b9c3ffbc37026fa1be34def6e4f2276b0dc2162a3f91628564a4bfb26280278b89d3ee54624e854d2f5f
-  languageName: node
-  linkType: hard
-
 "import-fresh@npm:^3.0.0, import-fresh@npm:^3.2.1":
   version: 3.3.0
   resolution: "import-fresh@npm:3.3.0"
   dependencies:
     parent-module: ^1.0.0
     resolve-from: ^4.0.0
   checksum: 2cacfad06e652b1edc50be650f7ec3be08c5e5a6f6d12d035c440a42a8cc028e60a5b99ca08a77ab4d6b1346da7d971915828f33cdab730d3d42f08242d09baa
@@ -3868,39 +3437,25 @@
 "imurmurhash@npm:^0.1.4":
   version: 0.1.4
   resolution: "imurmurhash@npm:0.1.4"
   checksum: 7cae75c8cd9a50f57dadd77482359f659eaebac0319dd9368bcd1714f55e65badd6929ca58569da2b6494ef13fdd5598cd700b1eba23f8b79c5f19d195a3ecf7
   languageName: node
   linkType: hard
 
-"indent-string@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "indent-string@npm:4.0.0"
-  checksum: 824cfb9929d031dabf059bebfe08cf3137365e112019086ed3dcff6a0a7b698cb80cf67ccccde0e25b9e2d7527aa6cc1fed1ac490c752162496caba3e6699612
-  languageName: node
-  linkType: hard
-
-"infer-owner@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "infer-owner@npm:1.0.4"
-  checksum: 181e732764e4a0611576466b4b87dac338972b839920b2a8cde43642e4ed6bd54dc1fb0b40874728f2a2df9a1b097b8ff83b56d5f8f8e3927f837fdcb47d8a89
-  languageName: node
-  linkType: hard
-
 "inflight@npm:^1.0.4":
   version: 1.0.6
   resolution: "inflight@npm:1.0.6"
   dependencies:
     once: ^1.3.0
     wrappy: 1
   checksum: f4f76aa072ce19fae87ce1ef7d221e709afb59d445e05d47fba710e85470923a75de35bfae47da6de1b18afc3ce83d70facf44cfb0aff89f0a3f45c0a0244dfd
   languageName: node
   linkType: hard
 
-"inherits@npm:2, inherits@npm:^2.0.3, inherits@npm:^2.0.4":
+"inherits@npm:2":
   version: 2.0.4
   resolution: "inherits@npm:2.0.4"
   checksum: 4a48a733847879d6cf6691860a6b1e3f0f4754176e4d71494c41f3475553768b10f84b5ce1d40fbd0e34e6bfbb864ee35858ad4dd2cf31e02fc4a154b724d7f1
   languageName: node
   linkType: hard
 
 "internal-slot@npm:^1.0.5":
@@ -3917,21 +3472,14 @@
 "interpret@npm:^3.1.1":
   version: 3.1.1
   resolution: "interpret@npm:3.1.1"
   checksum: 35cebcf48c7351130437596d9ab8c8fe131ce4038da4561e6d665f25640e0034702a031cf7e3a5cea60ac7ac548bf17465e0571ede126f3d3a6933152171ac82
   languageName: node
   linkType: hard
 
-"ip@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "ip@npm:2.0.0"
-  checksum: cfcfac6b873b701996d71ec82a7dd27ba92450afdb421e356f44044ed688df04567344c36cbacea7d01b1c39a4c732dc012570ebe9bebfb06f27314bca625349
-  languageName: node
-  linkType: hard
-
 "is-array-buffer@npm:^3.0.1, is-array-buffer@npm:^3.0.2":
   version: 3.0.2
   resolution: "is-array-buffer@npm:3.0.2"
   dependencies:
     call-bind: ^1.0.2
     get-intrinsic: ^1.2.0
     is-typed-array: ^1.1.10
@@ -3969,19 +3517,19 @@
   version: 1.2.7
   resolution: "is-callable@npm:1.2.7"
   checksum: 61fd57d03b0d984e2ed3720fb1c7a897827ea174bd44402878e059542ea8c4aeedee0ea0985998aa5cc2736b2fa6e271c08587addb5b3959ac52cf665173d1ac
   languageName: node
   linkType: hard
 
 "is-core-module@npm:^2.12.0":
-  version: 2.12.0
-  resolution: "is-core-module@npm:2.12.0"
+  version: 2.12.1
+  resolution: "is-core-module@npm:2.12.1"
   dependencies:
     has: ^1.0.3
-  checksum: f7f7eb2ab71fd769ee9fb2385c095d503aa4b5ce0028c04557de03f1e67a87c85e5bac1f215945fc3c955867a139a415a3ec4c4234a0bffdf715232660f440a6
+  checksum: f04ea30533b5e62764e7b2e049d3157dc0abd95ef44275b32489ea2081176ac9746ffb1cdb107445cf1ff0e0dfcad522726ca27c27ece64dadf3795428b8e468
   languageName: node
   linkType: hard
 
 "is-date-object@npm:^1.0.1":
   version: 1.0.5
   resolution: "is-date-object@npm:1.0.5"
   dependencies:
@@ -4009,21 +3557,14 @@
   resolution: "is-glob@npm:4.0.3"
   dependencies:
     is-extglob: ^2.1.1
   checksum: d381c1319fcb69d341cc6e6c7cd588e17cd94722d9a32dbd60660b993c4fb7d0f19438674e68dfec686d09b7c73139c9166b47597f846af387450224a8101ab4
   languageName: node
   linkType: hard
 
-"is-lambda@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "is-lambda@npm:1.0.1"
-  checksum: 93a32f01940220532e5948538699ad610d5924ac86093fcee83022252b363eb0cc99ba53ab084a04e4fb62bf7b5731f55496257a4c38adf87af9c4d352c71c35
-  languageName: node
-  linkType: hard
-
 "is-negative-zero@npm:^2.0.2":
   version: 2.0.2
   resolution: "is-negative-zero@npm:2.0.2"
   checksum: f3232194c47a549da60c3d509c9a09be442507616b69454716692e37ae9f37c4dea264fb208ad0c9f3efd15a796a46b79df07c7e53c6227c32170608b809149a
   languageName: node
   linkType: hard
 
@@ -4147,17 +3688,17 @@
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
   checksum: 98cd68b696781caed61c983a3ee30bf880b5bd021c01d98f47b143d4362b85d0737f8523761e2713d45e18b4f9a2b98af1eaee77afade4111bb65c77d6f7c980
   languageName: node
   linkType: hard
 
 "jquery@npm:^3.1.1":
-  version: 3.6.4
-  resolution: "jquery@npm:3.6.4"
-  checksum: 8354f7bd0a0424aa714ee1b6b1ef74b410f834eb5c8501682289b358bc151f11677f11188b544f3bb49309d6ec4d15d1a5de175661250c206b06185a252f706f
+  version: 3.7.0
+  resolution: "jquery@npm:3.7.0"
+  checksum: 907785e133afc427650a131af5fccef66a404885037513b3d4d7d63aee6409bcc32a39836868c60e59b05aa0fb8ace8961c18b2ee3ffdf6ffdb571d6d7cd88ff
   languageName: node
   linkType: hard
 
 "js-tokens@npm:^3.0.0 || ^4.0.0, js-tokens@npm:^4.0.0":
   version: 4.0.0
   resolution: "js-tokens@npm:4.0.0"
   checksum: 8a95213a5a77deb6cbe94d86340e8d9ace2b93bc367790b260101d2f36a2eaf4e4e22d9fa9cf459b38af3a32fb4190e638024cf82ec95ef708680e405ea7cc78
@@ -4263,136 +3804,33 @@
 "kind-of@npm:^6.0.2":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
   languageName: node
   linkType: hard
 
-"level-codec@npm:^9.0.0":
-  version: 9.0.2
-  resolution: "level-codec@npm:9.0.2"
-  dependencies:
-    buffer: ^5.6.0
-  checksum: 289003d51b8afcdd24c4d318606abf2bae81975e4b527d7349abfdbacc8fef26711f2f24e2d20da0e1dce0bb216a856c9433ccb9ca25fa78a96aed9f51e506ed
-  languageName: node
-  linkType: hard
-
-"level-concat-iterator@npm:~2.0.0":
-  version: 2.0.1
-  resolution: "level-concat-iterator@npm:2.0.1"
-  checksum: 562583ef1292215f8e749c402510cb61c4d6fccf4541082b3d21dfa5ecde9fcccfe52bdcb5cfff9d2384e7ce5891f44df9439a6ddb39b0ffe31015600b4a828a
-  languageName: node
-  linkType: hard
-
-"level-errors@npm:^2.0.0, level-errors@npm:~2.0.0":
-  version: 2.0.1
-  resolution: "level-errors@npm:2.0.1"
-  dependencies:
-    errno: ~0.1.1
-  checksum: aca5d7670e2a40609db8d7743fce289bb5202c0bc13e4a78f81f36a6642e9abc0110f48087d3d3c2c04f023d70d4ee6f2db0e20c63d29b3fda323a67bfff6526
-  languageName: node
-  linkType: hard
-
-"level-iterator-stream@npm:~4.0.0":
-  version: 4.0.2
-  resolution: "level-iterator-stream@npm:4.0.2"
-  dependencies:
-    inherits: ^2.0.4
-    readable-stream: ^3.4.0
-    xtend: ^4.0.2
-  checksum: 239e2c7e62bffb485ed696bcd3b98de7a2bc455d13be4fce175ae3544fe9cda81c2ed93d3e88b61380ae6d28cce02511862d77b86fb2ba5b5cf00471f3c1eccc
-  languageName: node
-  linkType: hard
-
-"level-js@npm:^5.0.0":
-  version: 5.0.2
-  resolution: "level-js@npm:5.0.2"
-  dependencies:
-    abstract-leveldown: ~6.2.3
-    buffer: ^5.5.0
-    inherits: ^2.0.3
-    ltgt: ^2.1.2
-  checksum: 3c7f75979bb8c042e95a58245b8fe1230bb0f56a11ee418e08156e3eadda371efae6eb7b9bf10bf1e08e0b1b2a25d80c026858ca99ffd49109d6541e3d9d3b37
-  languageName: node
-  linkType: hard
-
-"level-packager@npm:^5.1.0":
-  version: 5.1.1
-  resolution: "level-packager@npm:5.1.1"
-  dependencies:
-    encoding-down: ^6.3.0
-    levelup: ^4.3.2
-  checksum: befe2aa54f2010a6ecf7ddce392c8dee225e1839205080a2704d75e560e28b01191b345494696196777b70d376e3eaae4c9e7c330cc70d3000839f5b18dd78f2
-  languageName: node
-  linkType: hard
-
-"level-supports@npm:~1.0.0":
-  version: 1.0.1
-  resolution: "level-supports@npm:1.0.1"
-  dependencies:
-    xtend: ^4.0.2
-  checksum: 5d6bdb88cf00c3d9adcde970db06a548c72c5a94bf42c72f998b58341a105bfe2ea30d313ce1e84396b98cc9ddbc0a9bd94574955a86e929f73c986e10fc0df0
-  languageName: node
-  linkType: hard
-
-"level@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "level@npm:6.0.1"
-  dependencies:
-    level-js: ^5.0.0
-    level-packager: ^5.1.0
-    leveldown: ^5.4.0
-  checksum: bd4981f94162469a82a6c98d267d814d9d4a7beed4fc3d18fbe3b156f71cf4c6d35b424d14c46d401dbf0cd91425e842950a7cd17ddf7bf57acdab5af4c278da
-  languageName: node
-  linkType: hard
-
-"leveldown@npm:^5.4.0":
-  version: 5.6.0
-  resolution: "leveldown@npm:5.6.0"
-  dependencies:
-    abstract-leveldown: ~6.2.1
-    napi-macros: ~2.0.0
-    node-gyp: latest
-    node-gyp-build: ~4.1.0
-  checksum: 06d4683170d7fc661acd65457e531b42ad66480e9339d3154ba6d0de38ff0503d7d017c1c6eba12732b5488ecd2915c70c8dc3a7d67f4a836f3de34b8a993949
-  languageName: node
-  linkType: hard
-
-"levelup@npm:^4.3.2":
-  version: 4.4.0
-  resolution: "levelup@npm:4.4.0"
-  dependencies:
-    deferred-leveldown: ~5.3.0
-    level-errors: ~2.0.0
-    level-iterator-stream: ~4.0.0
-    level-supports: ~1.0.0
-    xtend: ~4.0.0
-  checksum: 5a09e34c78cd7c23f9f6cb73563f1ebe8121ffc5f9f5f232242529d4fbdd40e8d1ffb337d2defa0b842334e0dbd4028fbfe7a072eebfe2c4d07174f0aa4aabca
-  languageName: node
-  linkType: hard
-
 "levn@npm:^0.4.1":
   version: 0.4.1
   resolution: "levn@npm:0.4.1"
   dependencies:
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.31, lib0@npm:^0.2.42, lib0@npm:^0.2.52, lib0@npm:^0.2.62, lib0@npm:^0.2.74":
-  version: 0.2.74
-  resolution: "lib0@npm:0.2.74"
+"lib0@npm:^0.2.42, lib0@npm:^0.2.74, lib0@npm:^0.2.76":
+  version: 0.2.76
+  resolution: "lib0@npm:0.2.76"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: a468fc2f8d231bdcb305f04706d0e568ad53a0aa968aaf3d1769fcfbf326a5b158e98d86c0aa8edf26b3223cb60687480f15cfc0d07c681333f9d9d55dd7c802
+  checksum: e3700ca40e1d58dadbe9a578fec43e5d45a17bb4c82fb3c349308285ff3b76cea554d382a402747f45c7c2c173930cf15a317093ed880f373527f77c57fecbad
   languageName: node
   linkType: hard
 
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
@@ -4447,21 +3885,14 @@
 "lodash-es@npm:^4.17.21":
   version: 4.17.21
   resolution: "lodash-es@npm:4.17.21"
   checksum: 05cbffad6e2adbb331a4e16fbd826e7faee403a1a04873b82b42c0f22090f280839f85b95393f487c1303c8a3d2a010048bf06151a6cbe03eee4d388fb0a12d2
   languageName: node
   linkType: hard
 
-"lodash.debounce@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "lodash.debounce@npm:4.0.8"
-  checksum: a3f527d22c548f43ae31c861ada88b2637eb48ac6aa3eb56e82d44917971b8aa96fbb37aa60efea674dc4ee8c42074f90f7b1f772e9db375435f6c83a19b3bc6
-  languageName: node
-  linkType: hard
-
 "lodash.escape@npm:^4.0.1":
   version: 4.0.1
   resolution: "lodash.escape@npm:4.0.1"
   checksum: fcb54f457497256964d619d5cccbd80a961916fca60df3fe0fa3e7f052715c2944c0ed5aefb4f9e047d127d44aa2d55555f3350cb42c6549e9e293fb30b41e7f
   languageName: node
   linkType: hard
 
@@ -4509,52 +3940,14 @@
   resolution: "lru-cache@npm:6.0.0"
   dependencies:
     yallist: ^4.0.0
   checksum: f97f499f898f23e4585742138a22f22526254fdba6d75d41a1c2526b3b6cc5747ef59c5612ba7375f42aca4f8461950e925ba08c991ead0651b4918b7c978297
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^7.7.1":
-  version: 7.18.3
-  resolution: "lru-cache@npm:7.18.3"
-  checksum: e550d772384709deea3f141af34b6d4fa392e2e418c1498c078de0ee63670f1f46f5eee746e8ef7e69e1c895af0d4224e62ee33e66a543a14763b0f2e74c1356
-  languageName: node
-  linkType: hard
-
-"ltgt@npm:^2.1.2":
-  version: 2.2.1
-  resolution: "ltgt@npm:2.2.1"
-  checksum: 7e3874296f7538bc8087b428ac4208008d7b76916354b34a08818ca7c83958c1df10ec427eeeaad895f6b81e41e24745b18d30f89abcc21d228b94f6961d50a2
-  languageName: node
-  linkType: hard
-
-"make-fetch-happen@npm:^10.0.3":
-  version: 10.2.1
-  resolution: "make-fetch-happen@npm:10.2.1"
-  dependencies:
-    agentkeepalive: ^4.2.1
-    cacache: ^16.1.0
-    http-cache-semantics: ^4.1.0
-    http-proxy-agent: ^5.0.0
-    https-proxy-agent: ^5.0.0
-    is-lambda: ^1.0.1
-    lru-cache: ^7.7.1
-    minipass: ^3.1.6
-    minipass-collect: ^1.0.2
-    minipass-fetch: ^2.0.3
-    minipass-flush: ^1.0.5
-    minipass-pipeline: ^1.2.4
-    negotiator: ^0.6.3
-    promise-retry: ^2.0.1
-    socks-proxy-agent: ^7.0.0
-    ssri: ^9.0.0
-  checksum: 2332eb9a8ec96f1ffeeea56ccefabcb4193693597b132cd110734d50f2928842e22b84cfa1508e921b8385cdfd06dda9ad68645fed62b50fff629a580f5fb72c
-  languageName: node
-  linkType: hard
-
 "markdown-to-jsx@npm:^7.2.0":
   version: 7.2.0
   resolution: "markdown-to-jsx@npm:7.2.0"
   peerDependencies:
     react: ">= 0.14.0"
   checksum: ea417e684d7eec9f1beebc9423aba377116ef77c3cd83a2d622df1b9030ffef99aa9b3f431192b94f3237943a33560e6dda9be8a4c1d25187518d09986dad22f
   languageName: node
@@ -4604,21 +3997,21 @@
   dependencies:
     mime-db: 1.52.0
   checksum: 89a5b7f1def9f3af5dad6496c5ed50191ae4331cc5389d7c521c8ad28d5fdad2d06fd81baf38fed813dc4e46bb55c8145bb0ff406330818c9cf712fb2e9b3836
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.7.5
-  resolution: "mini-css-extract-plugin@npm:2.7.5"
+  version: 2.7.6
+  resolution: "mini-css-extract-plugin@npm:2.7.6"
   dependencies:
     schema-utils: ^4.0.0
   peerDependencies:
     webpack: ^5.0.0
-  checksum: afc37cdfb765e8826a1babbab3cd8a99ffc4eaeabb6c013a6b3c80801e44ebc37d930b98c6f66168bb8cd545fcb2e8fc2630d72b4501a1bb8add1547c2534a53
+  checksum: be6f7cefc6275168eb0a6b8fe977083a18c743c9612c9f00e6c1a62c3393ca7960e93fba1a7ebb09b75f36a0204ad087d772c1ef574bc29c90c0e8175a3c0b83
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
@@ -4632,167 +4025,51 @@
   resolution: "minimatch@npm:3.1.2"
   dependencies:
     brace-expansion: ^1.1.7
   checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
   languageName: node
   linkType: hard
 
-"minimatch@npm:^5.0.1":
-  version: 5.1.6
-  resolution: "minimatch@npm:5.1.6"
-  dependencies:
-    brace-expansion: ^2.0.1
-  checksum: 7564208ef81d7065a370f788d337cd80a689e981042cb9a1d0e6580b6c6a8c9279eba80010516e258835a988363f99f54a6f711a315089b8b42694f5da9d0d77
-  languageName: node
-  linkType: hard
-
 "minimist@npm:~1.2.0":
   version: 1.2.8
   resolution: "minimist@npm:1.2.8"
   checksum: 75a6d645fb122dad29c06a7597bddea977258957ed88d7a6df59b5cd3fe4a527e253e9bbf2e783e4b73657f9098b96a5fe96ab8a113655d4109108577ecf85b0
   languageName: node
   linkType: hard
 
-"minipass-collect@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "minipass-collect@npm:1.0.2"
-  dependencies:
-    minipass: ^3.0.0
-  checksum: 14df761028f3e47293aee72888f2657695ec66bd7d09cae7ad558da30415fdc4752bbfee66287dcc6fd5e6a2fa3466d6c484dc1cbd986525d9393b9523d97f10
-  languageName: node
-  linkType: hard
-
-"minipass-fetch@npm:^2.0.3":
-  version: 2.1.2
-  resolution: "minipass-fetch@npm:2.1.2"
-  dependencies:
-    encoding: ^0.1.13
-    minipass: ^3.1.6
-    minipass-sized: ^1.0.3
-    minizlib: ^2.1.2
-  dependenciesMeta:
-    encoding:
-      optional: true
-  checksum: 3f216be79164e915fc91210cea1850e488793c740534985da017a4cbc7a5ff50506956d0f73bb0cb60e4fe91be08b6b61ef35101706d3ef5da2c8709b5f08f91
-  languageName: node
-  linkType: hard
-
-"minipass-flush@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "minipass-flush@npm:1.0.5"
-  dependencies:
-    minipass: ^3.0.0
-  checksum: 56269a0b22bad756a08a94b1ffc36b7c9c5de0735a4dd1ab2b06c066d795cfd1f0ac44a0fcae13eece5589b908ecddc867f04c745c7009be0b566421ea0944cf
-  languageName: node
-  linkType: hard
-
-"minipass-pipeline@npm:^1.2.4":
-  version: 1.2.4
-  resolution: "minipass-pipeline@npm:1.2.4"
-  dependencies:
-    minipass: ^3.0.0
-  checksum: b14240dac0d29823c3d5911c286069e36d0b81173d7bdf07a7e4a91ecdef92cdff4baaf31ea3746f1c61e0957f652e641223970870e2353593f382112257971b
-  languageName: node
-  linkType: hard
-
-"minipass-sized@npm:^1.0.3":
-  version: 1.0.3
-  resolution: "minipass-sized@npm:1.0.3"
-  dependencies:
-    minipass: ^3.0.0
-  checksum: 79076749fcacf21b5d16dd596d32c3b6bf4d6e62abb43868fac21674078505c8b15eaca4e47ed844985a4514854f917d78f588fcd029693709417d8f98b2bd60
-  languageName: node
-  linkType: hard
-
-"minipass@npm:^3.0.0, minipass@npm:^3.1.1, minipass@npm:^3.1.6":
-  version: 3.3.6
-  resolution: "minipass@npm:3.3.6"
-  dependencies:
-    yallist: ^4.0.0
-  checksum: a30d083c8054cee83cdcdc97f97e4641a3f58ae743970457b1489ce38ee1167b3aaf7d815cd39ec7a99b9c40397fd4f686e83750e73e652b21cb516f6d845e48
-  languageName: node
-  linkType: hard
-
-"minipass@npm:^4.0.0":
-  version: 4.2.8
-  resolution: "minipass@npm:4.2.8"
-  checksum: 7f4914d5295a9a30807cae5227a37a926e6d910c03f315930fde52332cf0575dfbc20295318f91f0baf0e6bb11a6f668e30cde8027dea7a11b9d159867a3c830
-  languageName: node
-  linkType: hard
-
-"minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "minizlib@npm:2.1.2"
-  dependencies:
-    minipass: ^3.0.0
-    yallist: ^4.0.0
-  checksum: f1fdeac0b07cf8f30fcf12f4b586795b97be856edea22b5e9072707be51fc95d41487faec3f265b42973a304fe3a64acd91a44a3826a963e37b37bafde0212c3
-  languageName: node
-  linkType: hard
-
-"mkdirp@npm:^1.0.3, mkdirp@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "mkdirp@npm:1.0.4"
-  bin:
-    mkdirp: bin/cmd.js
-  checksum: a96865108c6c3b1b8e1d5e9f11843de1e077e57737602de1b82030815f311be11f96f09cce59bd5b903d0b29834733e5313f9301e3ed6d6f6fba2eae0df4298f
-  languageName: node
-  linkType: hard
-
 "moment@npm:^2.24.0":
   version: 2.29.4
   resolution: "moment@npm:2.29.4"
   checksum: 0ec3f9c2bcba38dc2451b1daed5daded747f17610b92427bebe1d08d48d8b7bdd8d9197500b072d14e326dd0ccf3e326b9e3d07c5895d3d49e39b6803b76e80e
   languageName: node
   linkType: hard
 
 "ms@npm:2.1.2":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
-"ms@npm:^2.0.0":
-  version: 2.1.3
-  resolution: "ms@npm:2.1.3"
-  checksum: aa92de608021b242401676e35cfa5aa42dd70cbdc082b916da7fb925c542173e36bce97ea3e804923fe92c0ad991434e4a38327e15a1b5b5f945d66df615ae6d
-  languageName: node
-  linkType: hard
-
 "nanoid@npm:^3.3.6":
   version: 3.3.6
   resolution: "nanoid@npm:3.3.6"
   bin:
     nanoid: bin/nanoid.cjs
   checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
   languageName: node
   linkType: hard
 
-"napi-macros@npm:~2.0.0":
-  version: 2.0.0
-  resolution: "napi-macros@npm:2.0.0"
-  checksum: 30384819386977c1f82034757014163fa60ab3c5a538094f778d38788bebb52534966279956f796a92ea771c7f8ae072b975df65de910d051ffbdc927f62320c
-  languageName: node
-  linkType: hard
-
 "natural-compare@npm:^1.4.0":
   version: 1.4.0
   resolution: "natural-compare@npm:1.4.0"
   checksum: 23ad088b08f898fc9b53011d7bb78ec48e79de7627e01ab5518e806033861bef68d5b0cd0e2205c2f36690ac9571ff6bcb05eb777ced2eeda8d4ac5b44592c3d
   languageName: node
   linkType: hard
 
-"negotiator@npm:^0.6.3":
-  version: 0.6.3
-  resolution: "negotiator@npm:0.6.3"
-  checksum: b8ffeb1e262eff7968fc90a2b6767b04cfd9842582a9d0ece0af7049537266e7b2506dfb1d107a32f06dd849ab2aea834d5830f7f4d0e5cb7d36e1ae55d021d9
-  languageName: node
-  linkType: hard
-
 "neo-async@npm:^2.6.2":
   version: 2.6.2
   resolution: "neo-async@npm:2.6.2"
   checksum: deac9f8d00eda7b2e5cd1b2549e26e10a0faa70adaa6fdadca701cc55f49ee9018e427f424bac0c790b7c7e2d3068db97f3093f1093975f2acb8f8818b936ed9
   languageName: node
   linkType: hard
 
@@ -4800,73 +4077,31 @@
   version: 1.0.5
   resolution: "nice-try@npm:1.0.5"
   checksum: 0b4af3b5bb5d86c289f7a026303d192a7eb4417231fe47245c460baeabae7277bcd8fd9c728fb6bd62c30b3e15cd6620373e2cf33353b095d8b403d3e8a15aff
   languageName: node
   linkType: hard
 
 "node-fetch@npm:^2.6.0":
-  version: 2.6.9
-  resolution: "node-fetch@npm:2.6.9"
+  version: 2.6.11
+  resolution: "node-fetch@npm:2.6.11"
   dependencies:
     whatwg-url: ^5.0.0
   peerDependencies:
     encoding: ^0.1.0
   peerDependenciesMeta:
     encoding:
       optional: true
-  checksum: acb04f9ce7224965b2b59e71b33c639794d8991efd73855b0b250921382b38331ffc9d61bce502571f6cc6e11a8905ca9b1b6d4aeb586ab093e2756a1fd190d0
-  languageName: node
-  linkType: hard
-
-"node-gyp-build@npm:~4.1.0":
-  version: 4.1.1
-  resolution: "node-gyp-build@npm:4.1.1"
-  bin:
-    node-gyp-build: ./bin.js
-    node-gyp-build-optional: ./optional.js
-    node-gyp-build-test: ./build-test.js
-  checksum: 959d42221cc44b92700003efae741652bc4e379e4cf375830ddde03ba43c89f99694bf0883078ed0d4e03ffe2f85decab0572e04068d3900b8538d165dbc17df
-  languageName: node
-  linkType: hard
-
-"node-gyp@npm:latest":
-  version: 9.3.1
-  resolution: "node-gyp@npm:9.3.1"
-  dependencies:
-    env-paths: ^2.2.0
-    glob: ^7.1.4
-    graceful-fs: ^4.2.6
-    make-fetch-happen: ^10.0.3
-    nopt: ^6.0.0
-    npmlog: ^6.0.0
-    rimraf: ^3.0.2
-    semver: ^7.3.5
-    tar: ^6.1.2
-    which: ^2.0.2
-  bin:
-    node-gyp: bin/node-gyp.js
-  checksum: b860e9976fa645ca0789c69e25387401b4396b93c8375489b5151a6c55cf2640a3b6183c212b38625ef7c508994930b72198338e3d09b9d7ade5acc4aaf51ea7
+  checksum: 249d0666a9497553384d46b5ab296ba223521ac88fed4d8a17d6ee6c2efb0fc890f3e8091cafe7f9fba8151a5b8d925db2671543b3409a56c3cd522b468b47b3
   languageName: node
   linkType: hard
 
 "node-releases@npm:^2.0.8":
-  version: 2.0.10
-  resolution: "node-releases@npm:2.0.10"
-  checksum: d784ecde25696a15d449c4433077f5cce620ed30a1656c4abf31282bfc691a70d9618bae6868d247a67914d1be5cc4fde22f65a05f4398cdfb92e0fc83cadfbc
-  languageName: node
-  linkType: hard
-
-"nopt@npm:^6.0.0":
-  version: 6.0.0
-  resolution: "nopt@npm:6.0.0"
-  dependencies:
-    abbrev: ^1.0.0
-  bin:
-    nopt: bin/nopt.js
-  checksum: 82149371f8be0c4b9ec2f863cc6509a7fd0fa729929c009f3a58e4eb0c9e4cae9920e8f1f8eb46e7d032fec8fb01bede7f0f41a67eb3553b7b8e14fa53de1dac
+  version: 2.0.12
+  resolution: "node-releases@npm:2.0.12"
+  checksum: b8c56db82c4642a0f443332b331a4396dae452a2ac5a65c8dbd93ef89ecb2fbb0da9d42ac5366d4764973febadca816cf7587dad492dce18d2a6b2af59cda260
   languageName: node
   linkType: hard
 
 "normalize-package-data@npm:^2.3.2":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
@@ -4902,26 +4137,14 @@
     npm-run-all: bin/npm-run-all/index.js
     run-p: bin/run-p/index.js
     run-s: bin/run-s/index.js
   checksum: 373b72c6a36564da13c1642c1fd9bb4dcc756bce7a3648f883772f02661095319820834ff813762d2fee403e9b40c1cd27c8685807c107440f10eb19c006d4a0
   languageName: node
   linkType: hard
 
-"npmlog@npm:^6.0.0":
-  version: 6.0.2
-  resolution: "npmlog@npm:6.0.2"
-  dependencies:
-    are-we-there-yet: ^3.0.0
-    console-control-strings: ^1.1.0
-    gauge: ^4.0.3
-    set-blocking: ^2.0.0
-  checksum: ae238cd264a1c3f22091cdd9e2b106f684297d3c184f1146984ecbe18aaa86343953f26b9520dedd1b1372bc0316905b736c1932d778dbeb1fcf5a1001390e2a
-  languageName: node
-  linkType: hard
-
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
   languageName: node
   linkType: hard
 
@@ -4988,23 +4211,14 @@
   resolution: "p-locate@npm:4.1.0"
   dependencies:
     p-limit: ^2.2.0
   checksum: 513bd14a455f5da4ebfcb819ef706c54adb09097703de6aeaa5d26fe5ea16df92b48d1ac45e01e3944ce1e6aa2a66f7f8894742b8c9d6e276e16cd2049a2b870
   languageName: node
   linkType: hard
 
-"p-map@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "p-map@npm:4.0.0"
-  dependencies:
-    aggregate-error: ^3.0.0
-  checksum: cb0ab21ec0f32ddffd31dfc250e3afa61e103ef43d957cc45497afe37513634589316de4eb88abdfd969fe6410c22c0b93ab24328833b8eb1ccc087fc0442a1c
-  languageName: node
-  linkType: hard
-
 "p-try@npm:^2.0.0":
   version: 2.2.0
   resolution: "p-try@npm:2.2.0"
   checksum: f8a8e9a7693659383f06aec604ad5ead237c7a261c18048a6e1b5b85a5f8a067e469aa24f5bc009b991ea3b058a87f5065ef4176793a200d4917349881216cae
   languageName: node
   linkType: hard
 
@@ -5136,24 +4350,24 @@
   resolution: "postcss-modules-extract-imports@npm:3.0.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
   languageName: node
   linkType: hard
 
-"postcss-modules-local-by-default@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "postcss-modules-local-by-default@npm:4.0.0"
+"postcss-modules-local-by-default@npm:^4.0.1":
+  version: 4.0.3
+  resolution: "postcss-modules-local-by-default@npm:4.0.3"
   dependencies:
     icss-utils: ^5.0.0
     postcss-selector-parser: ^6.0.2
     postcss-value-parser: ^4.1.0
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 6cf570badc7bc26c265e073f3ff9596b69bb954bc6ac9c5c1b8cba2995b80834226b60e0a3cbb87d5f399dbb52e6466bba8aa1d244f6218f99d834aec431a69d
+  checksum: 2f8083687f3d6067885f8863dd32dbbb4f779cfcc7e52c17abede9311d84faf6d3ed8760e7c54c6380281732ae1f78e5e56a28baf3c271b33f450a11c9e30485
   languageName: node
   linkType: hard
 
 "postcss-modules-scope@npm:^3.0.0":
   version: 3.0.0
   resolution: "postcss-modules-scope@npm:3.0.0"
   dependencies:
@@ -5172,31 +4386,31 @@
   peerDependencies:
     postcss: ^8.1.0
   checksum: f7f2cdf14a575b60e919ad5ea52fed48da46fe80db2733318d71d523fc87db66c835814940d7d05b5746b0426e44661c707f09bdb83592c16aea06e859409db6
   languageName: node
   linkType: hard
 
 "postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.11
-  resolution: "postcss-selector-parser@npm:6.0.11"
+  version: 6.0.13
+  resolution: "postcss-selector-parser@npm:6.0.13"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: 0b01aa9c2d2c8dbeb51e9b204796b678284be9823abc8d6d40a8b16d4149514e922c264a8ed4deb4d6dbced564b9be390f5942c058582d8656351516d6c49cde
+  checksum: f89163338a1ce3b8ece8e9055cd5a3165e79a15e1c408e18de5ad8f87796b61ec2d48a2902d179ae0c4b5de10fccd3a325a4e660596549b040bc5ad1b465f096
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
-"postcss@npm:^8.3.11, postcss@npm:^8.4.19":
+"postcss@npm:^8.3.11, postcss@npm:^8.4.21":
   version: 8.4.23
   resolution: "postcss@npm:8.4.23"
   dependencies:
     nanoid: ^3.3.6
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
   checksum: 8bb9d1b2ea6e694f8987d4f18c94617971b2b8d141602725fedcc2222fdc413b776a6e1b969a25d627d7b2681ca5aabb56f59e727ef94072e1b6ac8412105a2f
@@ -5238,49 +4452,25 @@
 "progress@npm:^2.0.0":
   version: 2.0.3
   resolution: "progress@npm:2.0.3"
   checksum: f67403fe7b34912148d9252cb7481266a354bd99ce82c835f79070643bb3c6583d10dbcfda4d41e04bbc1d8437e9af0fb1e1f2135727878f5308682a579429b7
   languageName: node
   linkType: hard
 
-"promise-inflight@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "promise-inflight@npm:1.0.1"
-  checksum: 22749483091d2c594261517f4f80e05226d4d5ecc1fc917e1886929da56e22b5718b7f2a75f3807e7a7d471bc3be2907fe92e6e8f373ddf5c64bae35b5af3981
-  languageName: node
-  linkType: hard
-
-"promise-retry@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "promise-retry@npm:2.0.1"
-  dependencies:
-    err-code: ^2.0.2
-    retry: ^0.12.0
-  checksum: f96a3f6d90b92b568a26f71e966cbbc0f63ab85ea6ff6c81284dc869b41510e6cdef99b6b65f9030f0db422bf7c96652a3fff9f2e8fb4a0f069d8f4430359429
-  languageName: node
-  linkType: hard
-
 "prop-types@npm:^15.8.1":
   version: 15.8.1
   resolution: "prop-types@npm:15.8.1"
   dependencies:
     loose-envify: ^1.4.0
     object-assign: ^4.1.1
     react-is: ^16.13.1
   checksum: c056d3f1c057cb7ff8344c645450e14f088a915d078dcda795041765047fa080d38e5d626560ccaac94a4e16e3aa15f3557c1a9a8d1174530955e992c675e459
   languageName: node
   linkType: hard
 
-"prr@npm:~1.0.1":
-  version: 1.0.1
-  resolution: "prr@npm:1.0.1"
-  checksum: 3bca2db0479fd38f8c4c9439139b0c42dcaadcc2fbb7bb8e0e6afaa1383457f1d19aea9e5f961d5b080f1cfc05bfa1fe9e45c97a1d3fd6d421950a73d3108381
-  languageName: node
-  linkType: hard
-
 "punycode@npm:^2.1.0, punycode@npm:^2.1.1":
   version: 2.3.0
   resolution: "punycode@npm:2.3.0"
   checksum: 39f760e09a2a3bbfe8f5287cf733ecdad69d6af2fe6f97ca95f24b8921858b91e9ea3c9eeec6e08cede96181b3bb33f95c6ffd8c77e63986508aa2e8159fa200
   languageName: node
   linkType: hard
 
@@ -5349,25 +4539,14 @@
     load-json-file: ^4.0.0
     normalize-package-data: ^2.3.2
     path-type: ^3.0.0
   checksum: 398903ebae6c7e9965419a1062924436cc0b6f516c42c4679a90290d2f87448ed8f977e7aa2dbba4aa1ac09248628c43e493ac25b2bc76640e946035200e34c6
   languageName: node
   linkType: hard
 
-"readable-stream@npm:^3.4.0, readable-stream@npm:^3.6.0":
-  version: 3.6.2
-  resolution: "readable-stream@npm:3.6.2"
-  dependencies:
-    inherits: ^2.0.3
-    string_decoder: ^1.1.1
-    util-deprecate: ^1.0.1
-  checksum: bdcbe6c22e846b6af075e32cf8f4751c2576238c5043169a1c221c92ee2878458a816a4ea33f4c67623c0b6827c8a400409bfb3cf0bf3381392d0b1dfb52ac8d
-  languageName: node
-  linkType: hard
-
 "rechoir@npm:^0.8.0":
   version: 0.8.0
   resolution: "rechoir@npm:0.8.0"
   dependencies:
     resolve: ^1.20.0
   checksum: ad3caed8afdefbc33fbc30e6d22b86c35b3d51c2005546f4e79bcc03c074df804b3640ad18945e6bef9ed12caedc035655ec1082f64a5e94c849ff939dc0a788
   languageName: node
@@ -5450,21 +4629,14 @@
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
   checksum: ad59734723b596d0891321c951592ed9015a77ce84907f89c9d9307dd0c06e11a67906a3e628c4cae143d3e44898603478af0ddeb2bba3f229a9373efe342665
   languageName: node
   linkType: hard
 
-"retry@npm:^0.12.0":
-  version: 0.12.0
-  resolution: "retry@npm:0.12.0"
-  checksum: 623bd7d2e5119467ba66202d733ec3c2e2e26568074923bc0585b6b99db14f357e79bdedb63cab56cec47491c4a0da7e6021a7465ca6dc4f481d3898fdd3158c
-  languageName: node
-  linkType: hard
-
 "reusify@npm:^1.0.4":
   version: 1.0.4
   resolution: "reusify@npm:1.0.4"
   checksum: c3076ebcc22a6bc252cb0b9c77561795256c22b757f40c0d8110b1300723f15ec0fc8685e8d4ea6d7666f36c79ccc793b1939c748bf36f18f542744a4e379fcc
   languageName: node
   linkType: hard
 
@@ -5484,15 +4656,15 @@
   resolution: "run-parallel@npm:1.2.0"
   dependencies:
     queue-microtask: ^1.2.2
   checksum: cb4f97ad25a75ebc11a8ef4e33bb962f8af8516bb2001082ceabd8902e15b98f4b84b4f8a9b222e5d57fc3bd1379c483886ed4619367a7680dad65316993021d
   languageName: node
   linkType: hard
 
-"safe-buffer@npm:^5.1.0, safe-buffer@npm:~5.2.0":
+"safe-buffer@npm:^5.1.0":
   version: 5.2.1
   resolution: "safe-buffer@npm:5.2.1"
   checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
   languageName: node
   linkType: hard
 
 "safe-regex-test@npm:^1.0.0":
@@ -5576,40 +4748,33 @@
   bin:
     semver: ./bin/semver
   checksum: 57fd0acfd0bac382ee87cd52cd0aaa5af086a7dc8d60379dfe65fea491fb2489b6016400813930ecd61fd0952dae75c115287a1b16c234b1550887117744dfaf
   languageName: node
   linkType: hard
 
 "semver@npm:^7.2.1, semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.8":
-  version: 7.5.0
-  resolution: "semver@npm:7.5.0"
+  version: 7.5.1
+  resolution: "semver@npm:7.5.1"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
-  checksum: 2d266937756689a76f124ffb4c1ea3e1bbb2b263219f90ada8a11aebebe1280b13bb76cca2ca96bdee3dbc554cbc0b24752eb895b2a51577aa644427e9229f2b
+  checksum: d16dbedad53c65b086f79524b9ef766bf38670b2395bdad5c957f824dcc566b624988013564f4812bcace3f9d405355c3635e2007396a39d1bffc71cfec4a2fc
   languageName: node
   linkType: hard
 
 "serialize-javascript@npm:^6.0.0, serialize-javascript@npm:^6.0.1":
   version: 6.0.1
   resolution: "serialize-javascript@npm:6.0.1"
   dependencies:
     randombytes: ^2.1.0
   checksum: 3c4f4cb61d0893b988415bdb67243637333f3f574e9e9cc9a006a2ced0b390b0b3b44aef8d51c951272a9002ec50885eefdc0298891bc27eb2fe7510ea87dc4f
   languageName: node
   linkType: hard
 
-"set-blocking@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "set-blocking@npm:2.0.0"
-  checksum: 6e65a05f7cf7ebdf8b7c75b101e18c0b7e3dff4940d480efed8aad3a36a4005140b660fa1d804cb8bce911cac290441dc728084a30504d3516ac2ff7ad607b02
-  languageName: node
-  linkType: hard
-
 "shallow-clone@npm:^3.0.0":
   version: 3.0.1
   resolution: "shallow-clone@npm:3.0.1"
   dependencies:
     kind-of: ^6.0.2
   checksum: 39b3dd9630a774aba288a680e7d2901f5c0eae7b8387fc5c8ea559918b29b3da144b7bdb990d7ccd9e11be05508ac9e459ce51d01fd65e583282f6ffafcba2e7
   languageName: node
@@ -5661,21 +4826,14 @@
     call-bind: ^1.0.0
     get-intrinsic: ^1.0.2
     object-inspect: ^1.9.0
   checksum: 351e41b947079c10bd0858364f32bb3a7379514c399edb64ab3dce683933483fc63fb5e4efe0a15a2e8a7e3c436b6a91736ddb8d8c6591b0460a24bb4a1ee245
   languageName: node
   linkType: hard
 
-"signal-exit@npm:^3.0.7":
-  version: 3.0.7
-  resolution: "signal-exit@npm:3.0.7"
-  checksum: a2f098f247adc367dffc27845853e9959b9e88b01cb301658cfe4194352d8d2bb32e18467c786a7fe15f1d44b233ea35633d076d5e737870b7139949d1ab6318
-  languageName: node
-  linkType: hard
-
 "slash@npm:^3.0.0":
   version: 3.0.0
   resolution: "slash@npm:3.0.0"
   checksum: 94a93fff615f25a999ad4b83c9d5e257a7280c90a32a7cb8b4a87996e4babf322e469c42b7f649fd5796edd8687652f3fb452a86dc97a816f01113183393f11c
   languageName: node
   linkType: hard
 
@@ -5693,42 +4851,14 @@
     ansi-styles: ^4.0.0
     astral-regex: ^2.0.0
     is-fullwidth-code-point: ^3.0.0
   checksum: 4a82d7f085b0e1b070e004941ada3c40d3818563ac44766cca4ceadd2080427d337554f9f99a13aaeb3b4a94d9964d9466c807b3d7b7541d1ec37ee32d308756
   languageName: node
   linkType: hard
 
-"smart-buffer@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "smart-buffer@npm:4.2.0"
-  checksum: b5167a7142c1da704c0e3af85c402002b597081dd9575031a90b4f229ca5678e9a36e8a374f1814c8156a725d17008ae3bde63b92f9cfd132526379e580bec8b
-  languageName: node
-  linkType: hard
-
-"socks-proxy-agent@npm:^7.0.0":
-  version: 7.0.0
-  resolution: "socks-proxy-agent@npm:7.0.0"
-  dependencies:
-    agent-base: ^6.0.2
-    debug: ^4.3.3
-    socks: ^2.6.2
-  checksum: 720554370154cbc979e2e9ce6a6ec6ced205d02757d8f5d93fe95adae454fc187a5cbfc6b022afab850a5ce9b4c7d73e0f98e381879cf45f66317a4895953846
-  languageName: node
-  linkType: hard
-
-"socks@npm:^2.6.2":
-  version: 2.7.1
-  resolution: "socks@npm:2.7.1"
-  dependencies:
-    ip: ^2.0.0
-    smart-buffer: ^4.2.0
-  checksum: 259d9e3e8e1c9809a7f5c32238c3d4d2a36b39b83851d0f573bfde5f21c4b1288417ce1af06af1452569cd1eb0841169afd4998f0e04ba04656f6b7f0e46d748
-  languageName: node
-  linkType: hard
-
 "source-list-map@npm:^2.0.0":
   version: 2.0.1
   resolution: "source-list-map@npm:2.0.1"
   checksum: 806efc6f75e7cd31e4815e7a3aaf75a45c704871ea4075cb2eb49882c6fca28998f44fc5ac91adb6de03b2882ee6fb02f951fdc85e6a22b338c32bfe19557938
   languageName: node
   linkType: hard
 
@@ -5821,24 +4951,15 @@
 "sprintf-js@npm:~1.0.2":
   version: 1.0.3
   resolution: "sprintf-js@npm:1.0.3"
   checksum: 19d79aec211f09b99ec3099b5b2ae2f6e9cdefe50bc91ac4c69144b6d3928a640bb6ae5b3def70c2e85a2c3d9f5ec2719921e3a59d3ca3ef4b2fd1a4656a0df3
   languageName: node
   linkType: hard
 
-"ssri@npm:^9.0.0":
-  version: 9.0.1
-  resolution: "ssri@npm:9.0.1"
-  dependencies:
-    minipass: ^3.1.1
-  checksum: fb58f5e46b6923ae67b87ad5ef1c5ab6d427a17db0bead84570c2df3cd50b4ceb880ebdba2d60726588272890bae842a744e1ecce5bd2a2a582fccd5068309eb
-  languageName: node
-  linkType: hard
-
-"string-width@npm:^1.0.2 || 2 || 3 || 4, string-width@npm:^4.2.3":
+"string-width@npm:^4.2.3":
   version: 4.2.3
   resolution: "string-width@npm:4.2.3"
   dependencies:
     emoji-regex: ^8.0.0
     is-fullwidth-code-point: ^3.0.0
     strip-ansi: ^6.0.1
   checksum: e52c10dc3fbfcd6c3a15f159f54a90024241d0f149cf8aed2982a2d801d2e64df0bf1dc351cf8e95c3319323f9f220c16e740b06faecd53e2462df1d2b5443fb
@@ -5885,23 +5006,14 @@
     call-bind: ^1.0.2
     define-properties: ^1.1.4
     es-abstract: ^1.20.4
   checksum: 89080feef416621e6ef1279588994305477a7a91648d9436490d56010a1f7adc39167cddac7ce0b9884b8cdbef086987c4dcb2960209f2af8bac0d23ceff4f41
   languageName: node
   linkType: hard
 
-"string_decoder@npm:^1.1.1":
-  version: 1.3.0
-  resolution: "string_decoder@npm:1.3.0"
-  dependencies:
-    safe-buffer: ~5.2.0
-  checksum: 8417646695a66e73aefc4420eb3b84cc9ffd89572861fe004e6aeb13c7bc00e2f616247505d2dbbef24247c372f70268f594af7126f43548565c68c117bdeb56
-  languageName: node
-  linkType: hard
-
 "strip-ansi@npm:^6.0.0, strip-ansi@npm:^6.0.1":
   version: 6.0.1
   resolution: "strip-ansi@npm:6.0.1"
   dependencies:
     ansi-regex: ^5.0.1
   checksum: f3cd25890aef3ba6e1a74e20896c21a46f482e93df4a06567cebf2b57edabb15133f1f94e57434e0a958d61186087b1008e89c94875d019910a213181a14fc8c
   languageName: node
@@ -5918,19 +5030,19 @@
   version: 3.1.1
   resolution: "strip-json-comments@npm:3.1.1"
   checksum: 492f73e27268f9b1c122733f28ecb0e7e8d8a531a6662efbd08e22cccb3f9475e90a1b82cab06a392f6afae6d2de636f977e231296400d0ec5304ba70f166443
   languageName: node
   linkType: hard
 
 "style-loader@npm:~3.3.1":
-  version: 3.3.2
-  resolution: "style-loader@npm:3.3.2"
+  version: 3.3.3
+  resolution: "style-loader@npm:3.3.3"
   peerDependencies:
     webpack: ^5.0.0
-  checksum: 5ee5ce2dc885369eccb55d429376e83d02570d473ac5edeb69fd65ee894847f1e51429cf078351f617bd04516ece8a1dd967f9f40464bd8fa76d903c6b2a6f08
+  checksum: f59c953f56f6a935bd6a1dfa409f1128fed2b66b48ce4a7a75b85862a7156e5e90ab163878962762f528ec4d510903d828da645e143fbffd26f055dc1c094078
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0":
   version: 4.0.3
   resolution: "style-mod@npm:4.0.3"
   checksum: 934556e720bd29026ff8fef43a1a35b58957813025b91f996d886e9405acf934ddb1934def4400b174bd7784c9263eb9c71f07ae83925af9271b7d921d546854
@@ -5987,61 +5099,47 @@
 "tapable@npm:^2.1.1, tapable@npm:^2.2.0":
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
-"tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.1.13
-  resolution: "tar@npm:6.1.13"
-  dependencies:
-    chownr: ^2.0.0
-    fs-minipass: ^2.0.0
-    minipass: ^4.0.0
-    minizlib: ^2.1.1
-    mkdirp: ^1.0.3
-    yallist: ^4.0.0
-  checksum: 8a278bed123aa9f53549b256a36b719e317c8b96fe86a63406f3c62887f78267cea9b22dc6f7007009738509800d4a4dccc444abd71d762287c90f35b002eb1c
-  languageName: node
-  linkType: hard
-
 "terser-webpack-plugin@npm:^5.3.7":
-  version: 5.3.7
-  resolution: "terser-webpack-plugin@npm:5.3.7"
+  version: 5.3.9
+  resolution: "terser-webpack-plugin@npm:5.3.9"
   dependencies:
     "@jridgewell/trace-mapping": ^0.3.17
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
-    terser: ^5.16.5
+    terser: ^5.16.8
   peerDependencies:
     webpack: ^5.1.0
   peerDependenciesMeta:
     "@swc/core":
       optional: true
     esbuild:
       optional: true
     uglify-js:
       optional: true
-  checksum: 095e699fdeeb553cdf2c6f75f983949271b396d9c201d7ae9fc633c45c1c1ad14c7257ef9d51ccc62213dd3e97f875870ba31550f6d4f1b6674f2615562da7f7
+  checksum: 41705713d6f9cb83287936b21e27c658891c78c4392159f5148b5623f0e8c48559869779619b058382a4c9758e7820ea034695e57dc7c474b4962b79f553bc5f
   languageName: node
   linkType: hard
 
-"terser@npm:^5.16.5":
-  version: 5.17.1
-  resolution: "terser@npm:5.17.1"
+"terser@npm:^5.16.8":
+  version: 5.17.6
+  resolution: "terser@npm:5.17.6"
   dependencies:
     "@jridgewell/source-map": ^0.3.2
     acorn: ^8.5.0
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 69b0e80e3c4084db2819de4d6ae8a2ba79f2fcd7ed6df40fe4b602ec7bfd8e889cc63c7d5268f30990ffecbf6eeda18f857adad9386fe2c2331b398d58ed855c
+  checksum: 9c0ab0261a99a61c5f53d05d4ecc7f68c552bae6af481464fdd596bc9d7e89ce8e21b1833cb3ce06ad5f658e2b226081d543e4fe6e324b2cdf03ee8b7eeec01a
   languageName: node
   linkType: hard
 
 "text-table@npm:^0.2.0":
   version: 0.2.0
   resolution: "text-table@npm:0.2.0"
   checksum: b6937a38c80c7f84d9c11dd75e49d5c44f71d95e810a3250bd1f1797fc7117c57698204adf676b71497acc205d769d65c16ae8fa10afad832ae1322630aef10a
@@ -6070,25 +5168,25 @@
   version: 0.0.3
   resolution: "tr46@npm:0.0.3"
   checksum: 726321c5eaf41b5002e17ffbd1fb7245999a073e8979085dacd47c4b4e8068ff5777142fc6726d6ca1fd2ff16921b48788b87225cbc57c72636f6efa8efbffe3
   languageName: node
   linkType: hard
 
 "ts-loader@npm:^9.2.6":
-  version: 9.4.2
-  resolution: "ts-loader@npm:9.4.2"
+  version: 9.4.3
+  resolution: "ts-loader@npm:9.4.3"
   dependencies:
     chalk: ^4.1.0
     enhanced-resolve: ^5.0.0
     micromatch: ^4.0.0
     semver: ^7.3.4
   peerDependencies:
     typescript: "*"
     webpack: ^5.0.0
-  checksum: 6f306ee4c615c2a159fb177561e3fb86ca2cbd6c641e710d408a64b4978e1ff3f2c9733df07bff27d3f82efbfa7c287523d4306049510c7485ac2669a9c37eb0
+  checksum: 139ed53bc60717d0ca231cdffbdef7566b9feda11c72fecc697983113f1266ccca2e1cdf191f841a43afa6b87d6afe57a0caf4feecf02f30845aa7ac6f2411a4
   languageName: node
   linkType: hard
 
 "tslib@npm:^1.8.1":
   version: 1.14.1
   resolution: "tslib@npm:1.14.1"
   checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
@@ -6178,32 +5276,14 @@
 "underscore@npm:>=1.8.3":
   version: 1.13.6
   resolution: "underscore@npm:1.13.6"
   checksum: d5cedd14a9d0d91dd38c1ce6169e4455bb931f0aaf354108e47bd46d3f2da7464d49b2171a5cf786d61963204a42d01ea1332a903b7342ad428deaafaf70ec36
   languageName: node
   linkType: hard
 
-"unique-filename@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "unique-filename@npm:2.0.1"
-  dependencies:
-    unique-slug: ^3.0.0
-  checksum: 807acf3381aff319086b64dc7125a9a37c09c44af7620bd4f7f3247fcd5565660ac12d8b80534dcbfd067e6fe88a67e621386dd796a8af828d1337a8420a255f
-  languageName: node
-  linkType: hard
-
-"unique-slug@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "unique-slug@npm:3.0.0"
-  dependencies:
-    imurmurhash: ^0.1.4
-  checksum: 49f8d915ba7f0101801b922062ee46b7953256c93ceca74303bd8e6413ae10aa7e8216556b54dc5382895e8221d04f1efaf75f945c2e4a515b4139f77aa6640c
-  languageName: node
-  linkType: hard
-
 "universalify@npm:^2.0.0":
   version: 2.0.0
   resolution: "universalify@npm:2.0.0"
   checksum: 2406a4edf4a8830aa6813278bab1f953a8e40f2f63a37873ffa9a3bc8f9745d06cc8e88f3572cb899b7e509013f7f6fcc3e37e8a6d914167a5381d8440518c44
   languageName: node
   linkType: hard
 
@@ -6236,27 +5316,27 @@
   dependencies:
     querystringify: ^2.1.1
     requires-port: ^1.0.0
   checksum: fbdba6b1d83336aca2216bbdc38ba658d9cfb8fc7f665eb8b17852de638ff7d1a162c198a8e4ed66001ddbf6c9888d41e4798912c62b4fd777a31657989f7bdf
   languageName: node
   linkType: hard
 
-"util-deprecate@npm:^1.0.1, util-deprecate@npm:^1.0.2":
+"util-deprecate@npm:^1.0.2":
   version: 1.0.2
   resolution: "util-deprecate@npm:1.0.2"
   checksum: 474acf1146cb2701fe3b074892217553dfcf9a031280919ba1b8d651a068c9b15d863b7303cb15bd00a862b498e6cf4ad7b4a08fb134edd5a6f7641681cb54a2
   languageName: node
   linkType: hard
 
-"uuid@npm:^8.3.2":
-  version: 8.3.2
-  resolution: "uuid@npm:8.3.2"
+"uuid@npm:^9.0.0":
+  version: 9.0.0
+  resolution: "uuid@npm:9.0.0"
   bin:
     uuid: dist/bin/uuid
-  checksum: 5575a8a75c13120e2f10e6ddc801b2c7ed7d8f3c8ac22c7ed0c7b2ba6383ec0abda88c905085d630e251719e0777045ae3236f04c812184b7c765f63a70e58df
+  checksum: 8dd2c83c43ddc7e1c71e36b60aea40030a6505139af6bee0f382ebcd1a56f6cd3028f7f06ffb07f8cf6ced320b76aea275284b224b002b289f89fe89c389b028
   languageName: node
   linkType: hard
 
 "v8-compile-cache@npm:^2.0.3":
   version: 2.3.0
   resolution: "v8-compile-cache@npm:2.3.0"
   checksum: adb0a271eaa2297f2f4c536acbfee872d0dd26ec2d76f66921aa7fc437319132773483344207bdbeee169225f4739016d8d2dbf0553913a52bb34da6d0334f8e
@@ -6350,17 +5430,17 @@
   dependencies:
     vscode-jsonrpc: ^8.0.2
   checksum: eb2fdb5c96f124326505f06564dfc6584318b748fd6e39b4c0ba16a0d383d13ba0e9433596abdb841428dfc2a5501994c3206723d1cb38c6af5fcac1faf4be26
   languageName: node
   linkType: hard
 
 "w3c-keyname@npm:^2.2.4":
-  version: 2.2.6
-  resolution: "w3c-keyname@npm:2.2.6"
-  checksum: 59a31d23ca9953c01c99ed6695fee5b6ea36eb2412d76a21fe4302ab33a3f5cd96c006a763940b6115c3d042c16d3564eeee1156832217d028af0518098b3a42
+  version: 2.2.7
+  resolution: "w3c-keyname@npm:2.2.7"
+  checksum: 91e057b1ec28e0bafcaf28def12023f0e083fd473c40d0a9c2aa01a975d227200d75ff6d8eb6961bb4608b967b1df1dd86786b52ee9489cb9a2ebeed881a63ae
   languageName: node
   linkType: hard
 
 "watchpack@npm:^2.4.0":
   version: 2.4.0
   resolution: "watchpack@npm:2.4.0"
   dependencies:
@@ -6381,21 +5461,21 @@
   version: 6.1.0
   resolution: "webidl-conversions@npm:6.1.0"
   checksum: 1f526507aa491f972a0c1409d07f8444e1d28778dfa269a9971f2e157182f3d496dc33296e4ed45b157fdb3bf535bb90c90bf10c50dcf1dd6caacb2a34cc84fb
   languageName: node
   linkType: hard
 
 "webpack-cli@npm:^5.0.1":
-  version: 5.0.2
-  resolution: "webpack-cli@npm:5.0.2"
+  version: 5.1.1
+  resolution: "webpack-cli@npm:5.1.1"
   dependencies:
     "@discoveryjs/json-ext": ^0.5.0
-    "@webpack-cli/configtest": ^2.0.1
+    "@webpack-cli/configtest": ^2.1.0
     "@webpack-cli/info": ^2.0.1
-    "@webpack-cli/serve": ^2.0.2
+    "@webpack-cli/serve": ^2.0.4
     colorette: ^2.0.14
     commander: ^10.0.1
     cross-spawn: ^7.0.3
     envinfo: ^7.7.3
     fastest-levenshtein: ^1.0.12
     import-local: ^3.0.2
     interpret: ^3.1.1
@@ -6408,25 +5488,25 @@
       optional: true
     webpack-bundle-analyzer:
       optional: true
     webpack-dev-server:
       optional: true
   bin:
     webpack-cli: bin/cli.js
-  checksum: 98816d84c51487b90e1008ddbcda8827dcb7ae9ab7892f4d742f0d7b93f90a4a18a6ec2671b380e5a7ee4b0917cf0c43921119419d8ba9e1b14ea060115684fd
+  checksum: 7738e6a84a0098886e1e0c0fd0dab44b7dedfbb0580afbb5ef734c5109dcaee80140bebb5d9f4b40f425029563bb09bcbda8b08d904fa14e60ff632e6dcc8a17
   languageName: node
   linkType: hard
 
 "webpack-merge@npm:^5.7.3, webpack-merge@npm:^5.8.0":
-  version: 5.8.0
-  resolution: "webpack-merge@npm:5.8.0"
+  version: 5.9.0
+  resolution: "webpack-merge@npm:5.9.0"
   dependencies:
     clone-deep: ^4.0.1
     wildcard: ^2.0.0
-  checksum: 88786ab91013f1bd2a683834ff381be81c245a4b0f63304a5103e90f6653f44dab496a0768287f8531761f8ad957d1f9f3ccb2cb55df0de1bd9ee343e079da26
+  checksum: 64fe2c23aacc5f19684452a0e84ec02c46b990423aee6fcc5c18d7d471155bd14e9a6adb02bd3656eb3e0ac2532c8e97d69412ad14c97eeafe32fa6d10050872
   languageName: node
   linkType: hard
 
 "webpack-sources@npm:^1.2.0":
   version: 1.4.3
   resolution: "webpack-sources@npm:1.4.3"
   dependencies:
@@ -6440,27 +5520,27 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1, webpack@npm:^5.77.0":
-  version: 5.81.0
-  resolution: "webpack@npm:5.81.0"
+  version: 5.84.0
+  resolution: "webpack@npm:5.84.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^1.0.0
     "@webassemblyjs/ast": ^1.11.5
     "@webassemblyjs/wasm-edit": ^1.11.5
     "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
-    acorn-import-assertions: ^1.7.6
+    acorn-import-assertions: ^1.9.0
     browserslist: ^4.14.5
     chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.13.0
+    enhanced-resolve: ^5.14.1
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.2.9
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
@@ -6472,15 +5552,15 @@
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 1a6eecaffac3226d80f4e8f330b32e0ff117d9dafd8700166d230afbc171d68ea1ff55a9939fa789307f7b9d11881889ccb8e6cd79d4ccbaeef916788ce73fdb
+  checksum: 5837983d81d55edf621317f23de3a7ae49bbf24c9f8605beeba35ea62be5cc4b3b63ace0ec9785912b9ffe70fd969e613597fae21b2334a3913054c41189ef75
   languageName: node
   linkType: hard
 
 "whatwg-mimetype@npm:^2.3.0":
   version: 2.3.0
   resolution: "whatwg-mimetype@npm:2.3.0"
   checksum: 23eb885940bcbcca4ff841c40a78e9cbb893ec42743993a42bf7aed16085b048b44b06f3402018931687153550f9a32d259dfa524e4f03577ab898b6965e5383
@@ -6542,34 +5622,25 @@
     isexe: ^2.0.0
   bin:
     which: ./bin/which
   checksum: f2e185c6242244b8426c9df1510e86629192d93c1a986a7d2a591f2c24869e7ffd03d6dac07ca863b2e4c06f59a4cc9916c585b72ee9fa1aa609d0124df15e04
   languageName: node
   linkType: hard
 
-"which@npm:^2.0.1, which@npm:^2.0.2":
+"which@npm:^2.0.1":
   version: 2.0.2
   resolution: "which@npm:2.0.2"
   dependencies:
     isexe: ^2.0.0
   bin:
     node-which: ./bin/node-which
   checksum: 1a5c563d3c1b52d5f893c8b61afe11abc3bab4afac492e8da5bde69d550de701cf9806235f20a47b5c8fa8a1d6a9135841de2596535e998027a54589000e66d1
   languageName: node
   linkType: hard
 
-"wide-align@npm:^1.1.5":
-  version: 1.1.5
-  resolution: "wide-align@npm:1.1.5"
-  dependencies:
-    string-width: ^1.0.2 || 2 || 3 || 4
-  checksum: d5fc37cd561f9daee3c80e03b92ed3e84d80dde3365a8767263d03dacfc8fa06b065ffe1df00d8c2a09f731482fcacae745abfbb478d4af36d0a891fad4834d3
-  languageName: node
-  linkType: hard
-
 "wildcard@npm:^2.0.0":
   version: 2.0.1
   resolution: "wildcard@npm:2.0.1"
   checksum: e0c60a12a219e4b12065d1199802d81c27b841ed6ad6d9d28240980c73ceec6f856771d575af367cbec2982d9ae7838759168b551776577f155044f5a5ba843c
   languageName: node
   linkType: hard
 
@@ -6595,23 +5666,14 @@
 "wrappy@npm:1":
   version: 1.0.2
   resolution: "wrappy@npm:1.0.2"
   checksum: 159da4805f7e84a3d003d8841557196034155008f817172d4e986bd591f74aa82aa7db55929a54222309e01079a65a92a9e6414da5a6aa4b01ee44a511ac3ee5
   languageName: node
   linkType: hard
 
-"ws@npm:^6.2.1":
-  version: 6.2.2
-  resolution: "ws@npm:6.2.2"
-  dependencies:
-    async-limiter: ~1.0.0
-  checksum: aec3154ec51477c094ac2cb5946a156e17561a581fa27005cbf22c53ac57f8d4e5f791dd4bbba6a488602cb28778c8ab7df06251d590507c3c550fd8ebeee949
-  languageName: node
-  linkType: hard
-
 "ws@npm:^7.4.6":
   version: 7.5.9
   resolution: "ws@npm:7.5.9"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ^5.0.2
   peerDependenciesMeta:
@@ -6634,119 +5696,68 @@
       optional: true
     utf-8-validate:
       optional: true
   checksum: 53e991bbf928faf5dc6efac9b8eb9ab6497c69feeb94f963d648b7a3530a720b19ec2e0ec037344257e05a4f35bd9ad04d9de6f289615ffb133282031b18c61c
   languageName: node
   linkType: hard
 
-"xtend@npm:^4.0.2, xtend@npm:~4.0.0":
-  version: 4.0.2
-  resolution: "xtend@npm:4.0.2"
-  checksum: ac5dfa738b21f6e7f0dd6e65e1b3155036d68104e67e5d5d1bde74892e327d7e5636a076f625599dc394330a731861e87343ff184b0047fef1360a7ec0a5a36a
-  languageName: node
-  linkType: hard
-
-"y-leveldb@npm:^0.1.0":
-  version: 0.1.2
-  resolution: "y-leveldb@npm:0.1.2"
-  dependencies:
-    level: ^6.0.1
-    lib0: ^0.2.31
-  peerDependencies:
-    yjs: ^13.0.0
-  checksum: 38e3293cfc5e754ba50af4c6bd03a96efde34c92809baf504b38cb4f45959187f896fe6971fa6a91823763e178807aaa14e190d1f7bea1b3a1e9b7265bb88b6d
-  languageName: node
-  linkType: hard
-
 "y-protocols@npm:^1.0.5":
   version: 1.0.5
   resolution: "y-protocols@npm:1.0.5"
   dependencies:
     lib0: ^0.2.42
   checksum: d19404a4ebafcf3761c28b881abe8c32ab6e457db0e5ffc7dbb749cbc2c3bb98e003a43f3e8eba7f245b2698c76f2c4cdd1c2db869f8ec0c6ef94736d9a88652
   languageName: node
   linkType: hard
 
-"y-websocket@npm:^1.3.15":
-  version: 1.5.0
-  resolution: "y-websocket@npm:1.5.0"
-  dependencies:
-    lib0: ^0.2.52
-    lodash.debounce: ^4.0.8
-    ws: ^6.2.1
-    y-leveldb: ^0.1.0
-    y-protocols: ^1.0.5
-  peerDependencies:
-    yjs: ^13.5.6
-  dependenciesMeta:
-    ws:
-      optional: true
-    y-leveldb:
-      optional: true
-  bin:
-    y-websocket: bin/server.js
-    y-websocket-server: bin/server.js
-  checksum: 0e532f7d488e9430b011814eab67f37c002b0b102ccc169c65250ad9fddd901b2f979ac0f26453e7ac625fe2f2fe84d208b90b47e9e3572ac449b01572884fb8
-  languageName: node
-  linkType: hard
-
 "yallist@npm:^4.0.0":
   version: 4.0.0
   resolution: "yallist@npm:4.0.0"
   checksum: 343617202af32df2a15a3be36a5a8c0c8545208f3d3dfbc6bb7c3e3b7e8c6f8e7485432e4f3b88da3031a6e20afa7c711eded32ddfb122896ac5d914e75848d5
   languageName: node
   linkType: hard
 
 "yjs-widgets@workspace:.":
   version: 0.0.0-use.local
   resolution: "yjs-widgets@workspace:."
   dependencies:
     "@jupyter-widgets/base": ^6.0.2
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/application": ^4.0.0-beta.2
-    "@jupyterlab/apputils": ^4.0.0-beta.2
-    "@jupyterlab/builder": ~4.0.0-beta.0
+    "@jupyterlab/application": ^4.0.0
+    "@jupyterlab/apputils": ^4.0.0
+    "@jupyterlab/builder": ~4.0.0
     "@jupyterlab/collaboration": ^4.0.0-alpha.18
-    "@jupyterlab/coreutils": ^6.0.0-beta.2
-    "@jupyterlab/docprovider": ^4.0.0-alpha.18
-    "@jupyterlab/docregistry": ^4.0.0-beta.2
-    "@jupyterlab/filebrowser": ^4.0.0-beta.2
-    "@jupyterlab/launcher": ^4.0.0-beta.2
-    "@jupyterlab/mainmenu": ^4.0.0-beta.2
-    "@jupyterlab/notebook": ^4.0.0-beta.2
-    "@jupyterlab/observables": ^5.0.0-beta.2
-    "@jupyterlab/services": ^7.0.0-beta.2
-    "@jupyterlab/translation": ^4.0.0-beta.2
-    "@jupyterlab/ui-components": ^4.0.0-beta.2
-    "@lumino/commands": ^2.1.0
-    "@lumino/coreutils": ^2.1.0
-    "@lumino/signaling": ^2.1.0
-    "@lumino/widgets": ^2.1.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/notebook": ^4.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+    "@lumino/widgets": ^2.1.1
     "@types/node": ^16.11.10
     "@typescript-eslint/eslint-plugin": ^4.8.1
     "@typescript-eslint/parser": ^4.8.1
     copy-webpack-plugin: ^10.0.0
     eslint: ^7.14.0
     eslint-config-prettier: ^6.15.0
     eslint-plugin-prettier: ^3.1.4
     file-loader: ^6.2.0
-    lib0: ^0.2.62
+    lib0: ^0.2.76
     npm-run-all: ^4.1.5
     prettier: ^2.1.1
     rimraf: ^3.0.2
     source-map-loader: ^3.0.0
     ts-loader: ^9.2.6
     typescript: ~5.0.4
-    uuid: ^8.3.2
+    uuid: ^9.0.0
     webpack: ^5.77.0
     webpack-cli: ^5.0.1
   languageName: unknown
   linkType: soft
 
 "yjs@npm:^13.5.40":
-  version: 13.6.0
-  resolution: "yjs@npm:13.6.0"
+  version: 13.6.1
+  resolution: "yjs@npm:13.6.1"
   dependencies:
     lib0: ^0.2.74
-  checksum: 54bd3b0c8a8dc5724044356c8015210f9840b7ac46c8d87d66a0cc5f5bf669298d45324942681ad01ea22c7a4de6a29aa22180d63596e18734bc90335ced982f
+  checksum: bf18ed3f53b4baed61363461b2567cf841f27c326ae107736bb46239fb7273d9d0ef71ea83ae792e96e406d074218d6666f2909a680214b940ada39b58545336
   languageName: node
   linkType: hard
```

### Comparing `yjs_widgets-0.2.0/src/model.ts` & `yjs_widgets-0.3.0/src/model.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/types.ts` & `yjs_widgets-0.3.0/src/types.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/notebookrenderer/index.ts` & `yjs_widgets-0.3.0/src/notebookrenderer/index.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/notebookrenderer/model.ts` & `yjs_widgets-0.3.0/src/notebookrenderer/model.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/notebookrenderer/types.ts` & `yjs_widgets-0.3.0/src/notebookrenderer/types.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/notebookrenderer/view.ts` & `yjs_widgets-0.3.0/src/notebookrenderer/view.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/notebookrenderer/widgetManager.ts` & `yjs_widgets-0.3.0/src/notebookrenderer/widgetManager.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/src/notebookrenderer/yCommProvider.ts` & `yjs_widgets-0.3.0/src/notebookrenderer/yCommProvider.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/.gitignore` & `yjs_widgets-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/LICENSE` & `yjs_widgets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.2.0/README.md` & `yjs_widgets-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,43 +19,40 @@
 import { JupyterYModel } from './model';
 import { IJupyterYWidgetManager } from './notebookrenderer/types';
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
-class MyWidget1 {
+class MyWidget {
   constructor(yModel: IJupyterYModel, node: HTMLElement) {
     this.yModel = yModel;
     this.node = node;
     yModel.sharedModel.attrsChanged.connect(() => {
-      this._update();
+      this._attrsChanged();
     });
-    node.textContent = 'hello from my widget';
+    node.textContent = 'Hello world!';
   }
 
-  _update(): void {
-    const foo1: string = this.yModel.sharedModel.getAttr('foo1') as string;
-    const bar1: string = this.yModel.sharedModel.getAttr('bar1') as string;
-    if (bar1 != 'abc') {
-      this.yModel.sharedModel.setAttr('bar1', 'abc');
-    }
-    this.node.textContent = foo1;
+  _attrsChanged(): void {
+    const foo: string = this.yModel.sharedModel.getAttr('foo') as string;
+    const bar: string = this.yModel.sharedModel.getAttr('bar') as string;
+    this.node.textContent = `foo=${foo}, bar=${bar}`;
   }
 
   yModel: IJupyterYModel;
   node: HTMLElement;
 }
 
 export const foo: JupyterFrontEndPlugin<void> = {
   id: 'foo:bar',
   autoStart: true,
   requires: [IJupyterYWidgetManager],
   activate: (app: JupyterFrontEnd, wm: IJupyterYWidgetManager): void => {
-    wm.registerWidget('MyWidget1', JupyterYModel, MyWidget1);
+    wm.registerWidget('MyWidget', JupyterYModel, MyWidget);
   }
 };
 ```
 
 ## Contributing
 
 yjs-widgets is an open-source project, and contributions are always welcome. If you would like to contribute, please fork the repository and submit a pull request.
```

### Comparing `yjs_widgets-0.2.0/pyproject.toml` & `yjs_widgets-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
-    "hatchling>=1.5.0",
+    "hatchling",
     "hatch-nodejs-version",
-    "jupyterlab>=4.0.0b2,<5",
+    "jupyterlab>=4.0.0,<5",
 ]
 
 
 [project]
 name = "yjs_widgets"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
-    "jupyterlab>=4.0.0b2",
-    "jupyter_collaboration >=1.0.0a7",
-    "jupyter_server>=2.0.6",
+    "jupyterlab>=4.0.0",
     "ypywidgets>=0.4.0,<1",
     "comm>=0.1.3,<0.2.0"
 ]
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 3",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
```

### Comparing `yjs_widgets-0.2.0/PKG-INFO` & `yjs_widgets-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yjs_widgets
-Version: 0.2.0
+Version: 0.3.0
 Summary: A JupyterLab extension for widgets based on Yjs.
 Project-URL: Homepage, https://github.com/QuantStack/yjs-widgets
 Project-URL: Bug Tracker, https://github.com/QuantStack/yjs-widgets/issues
 Project-URL: Repository, https://github.com/QuantStack/yjs-widgets.git
 Author-email: Trung Le <leductrungxf@gmail.com>
 License: BSD 3-Clause License
         
@@ -40,23 +40,22 @@
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: comm<0.2.0,>=0.1.3
-Requires-Dist: jupyter-collaboration>=1.0.0a7
-Requires-Dist: jupyter-server>=2.0.6
-Requires-Dist: jupyterlab>=4.0.0b2
+Requires-Dist: jupyterlab>=4.0.0
 Requires-Dist: ypywidgets<1,>=0.4.0
 Description-Content-Type: text/markdown
 
 # JupyterLab extension for widgets based on Yjs
 
 ## Requirements
 
@@ -77,43 +76,40 @@
 import { JupyterYModel } from './model';
 import { IJupyterYWidgetManager } from './notebookrenderer/types';
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
-class MyWidget1 {
+class MyWidget {
   constructor(yModel: IJupyterYModel, node: HTMLElement) {
     this.yModel = yModel;
     this.node = node;
     yModel.sharedModel.attrsChanged.connect(() => {
-      this._update();
+      this._attrsChanged();
     });
-    node.textContent = 'hello from my widget';
+    node.textContent = 'Hello world!';
   }
 
-  _update(): void {
-    const foo1: string = this.yModel.sharedModel.getAttr('foo1') as string;
-    const bar1: string = this.yModel.sharedModel.getAttr('bar1') as string;
-    if (bar1 != 'abc') {
-      this.yModel.sharedModel.setAttr('bar1', 'abc');
-    }
-    this.node.textContent = foo1;
+  _attrsChanged(): void {
+    const foo: string = this.yModel.sharedModel.getAttr('foo') as string;
+    const bar: string = this.yModel.sharedModel.getAttr('bar') as string;
+    this.node.textContent = `foo=${foo}, bar=${bar}`;
   }
 
   yModel: IJupyterYModel;
   node: HTMLElement;
 }
 
 export const foo: JupyterFrontEndPlugin<void> = {
   id: 'foo:bar',
   autoStart: true,
   requires: [IJupyterYWidgetManager],
   activate: (app: JupyterFrontEnd, wm: IJupyterYWidgetManager): void => {
-    wm.registerWidget('MyWidget1', JupyterYModel, MyWidget1);
+    wm.registerWidget('MyWidget', JupyterYModel, MyWidget);
   }
 };
 ```
 
 ## Contributing
 
 yjs-widgets is an open-source project, and contributions are always welcome. If you would like to contribute, please fork the repository and submit a pull request.
```

