# Comparing `tmp/apertium2ud-0.0.1.tar.gz` & `tmp/apertium2ud-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium2ud-0.0.1.tar", last modified: Sat May 20 12:51:50 2023, max compression
+gzip compressed data, was "apertium2ud-0.0.2.tar", last modified: Thu May 25 10:33:59 2023, max compression
```

## Comparing `apertium2ud-0.0.1.tar` & `apertium2ud-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-20 12:51:50.865295 apertium2ud-0.0.1/
--rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.1/LICENSE
--rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.1/MANIFEST.in
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2248 2023-05-20 12:51:50.857304 apertium2ud-0.0.1/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1725 2023-05-20 12:32:00.000000 apertium2ud-0.0.1/README.md
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-20 12:51:50.327426 apertium2ud-0.0.1/apertium2ud/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1326 2023-05-20 12:50:57.000000 apertium2ud-0.0.1/apertium2ud/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)      617 2023-05-20 12:50:57.000000 apertium2ud-0.0.1/apertium2ud/_map_processing.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-05-19 19:22:22.000000 apertium2ud-0.0.1/apertium2ud/meta.py
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-20 12:51:50.780367 apertium2ud-0.0.1/apertium2ud/resources/
--rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.1/apertium2ud/resources/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)    37392 2023-05-20 12:08:09.000000 apertium2ud-0.0.1/apertium2ud/resources/tags_map.json
--rwxrwxrwx   0 aam       (1000) aam       (1000)      700 2023-05-20 12:26:36.000000 apertium2ud-0.0.1/apertium2ud/ud2apertium.py
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-20 12:51:50.630366 apertium2ud-0.0.1/apertium2ud.egg-info/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2248 2023-05-20 12:51:49.000000 apertium2ud-0.0.1/apertium2ud.egg-info/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)      384 2023-05-20 12:51:49.000000 apertium2ud-0.0.1/apertium2ud.egg-info/SOURCES.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-05-20 12:51:49.000000 apertium2ud-0.0.1/apertium2ud.egg-info/dependency_links.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-05-20 12:51:48.000000 apertium2ud-0.0.1/apertium2ud.egg-info/not-zip-safe
--rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-05-20 12:51:49.000000 apertium2ud-0.0.1/apertium2ud.egg-info/top_level.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-05-20 12:51:50.868356 apertium2ud-0.0.1/setup.cfg
--rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-05-20 12:31:27.000000 apertium2ud-0.0.1/setup.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:59.144171 apertium2ud-0.0.2/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.2/LICENSE
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2509 2023-05-25 10:33:59.139121 apertium2ud-0.0.2/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1995 2023-05-25 10:30:51.000000 apertium2ud-0.0.2/README.md
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:58.696427 apertium2ud-0.0.2/apertium2ud/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1874 2023-05-25 10:05:00.000000 apertium2ud-0.0.2/apertium2ud/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1818 2023-05-25 10:21:43.000000 apertium2ud-0.0.2/apertium2ud/_map_processing.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      955 2023-05-25 10:24:17.000000 apertium2ud-0.0.2/apertium2ud/convert.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-05-25 07:20:31.000000 apertium2ud-0.0.2/apertium2ud/meta.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:59.085735 apertium2ud-0.0.2/apertium2ud/resources/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.2/apertium2ud/resources/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.2/apertium2ud/resources/tags_map.json
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:58.985730 apertium2ud-0.0.2/apertium2ud.egg-info/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2509 2023-05-25 10:33:57.000000 apertium2ud-0.0.2/apertium2ud.egg-info/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      380 2023-05-25 10:33:58.000000 apertium2ud-0.0.2/apertium2ud.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-05-25 10:33:57.000000 apertium2ud-0.0.2/apertium2ud.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-05-25 10:33:56.000000 apertium2ud-0.0.2/apertium2ud.egg-info/not-zip-safe
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-05-25 10:33:57.000000 apertium2ud-0.0.2/apertium2ud.egg-info/top_level.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-05-25 10:33:59.147143 apertium2ud-0.0.2/setup.cfg
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-05-25 07:20:31.000000 apertium2ud-0.0.2/setup.py
```

### Comparing `apertium2ud-0.0.1/LICENSE` & `apertium2ud-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.1/PKG-INFO` & `apertium2ud-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,16 +23,27 @@
 hence the GPLv3 license.
 
 To build the machine-readable mapping, run
 
 ```bash
 python apertium_wiki_parser.py
 ```
+## Apertium to Universal tags
 
-## UD to Apertium
+```
+>>> from apertium2ud.convert import a2ud
+>>> tags = ["n", "pl", "acc"]
+>>> a2ud(tags)
+(['NOUN'], ['Number=Plur', 'Case=Acc'])
+>>> tags_sophisticated = ["v", "tv", "ger", "nom", "cop", "aor", "p3", "pl"]
+>>> a2ud(tags_sophisticated)
+(['VERB', 'AUX'], ['Subcat=Tran', 'VerbForm=Vnoun', 'Case=Nom', 'Tense=Past', 'Person=3', 'Number=Plur'])
+```
+
+## Universal tags to Apertium
 
 So far the conversion is far from perfect
 ```
 Кыз NOUN {'Number[psor]=Sing', 'Number=Sing', 'Case=Nom', 'Person[psor]=3', 'Person=3'} ->
 <px3sg><n><subj?nom?><sg><p3><px3sp> 
 
 досуна NOUN {'Number[psor]=Sing', 'Number=Sing', 'Person[psor]=3', 'Case=Dat', 'Person=3'} ->
@@ -47,16 +58,14 @@
 . PUNCT set() ->
 <sent?apos?percent?clb?punct?> 
 ```
 
 ## TODO
 
 * Should sections `chunks` and [XML tags](https://wiki.apertium.org/w/index.php?title=List_of_symbols#XML_tags) be added? [No](https://github.com/apertium/apertium/issues/185).
-* Add conversions Apertium -> UD, UD -> Apertium based on the constructed JSON file
-* Upload the converter as a package to PyPI
 * Tests: Apertium -> UD -> Apertium, UD -> Apertium -> UD (sometimes losses are inevitable)
 
 ## How to cite
 
 Greatly appreciated, if you use this work.
 
 ```
```

### Comparing `apertium2ud-0.0.1/README.md` & `apertium2ud-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,16 +7,27 @@
 hence the GPLv3 license.
 
 To build the machine-readable mapping, run
 
 ```bash
 python apertium_wiki_parser.py
 ```
+## Apertium to Universal tags
 
-## UD to Apertium
+```
+>>> from apertium2ud.convert import a2ud
+>>> tags = ["n", "pl", "acc"]
+>>> a2ud(tags)
+(['NOUN'], ['Number=Plur', 'Case=Acc'])
+>>> tags_sophisticated = ["v", "tv", "ger", "nom", "cop", "aor", "p3", "pl"]
+>>> a2ud(tags_sophisticated)
+(['VERB', 'AUX'], ['Subcat=Tran', 'VerbForm=Vnoun', 'Case=Nom', 'Tense=Past', 'Person=3', 'Number=Plur'])
+```
+
+## Universal tags to Apertium
 
 So far the conversion is far from perfect
 ```
 Кыз NOUN {'Number[psor]=Sing', 'Number=Sing', 'Case=Nom', 'Person[psor]=3', 'Person=3'} ->
 <px3sg><n><subj?nom?><sg><p3><px3sp> 
 
 досуна NOUN {'Number[psor]=Sing', 'Number=Sing', 'Person[psor]=3', 'Case=Dat', 'Person=3'} ->
@@ -31,16 +42,14 @@
 . PUNCT set() ->
 <sent?apos?percent?clb?punct?> 
 ```
 
 ## TODO
 
 * Should sections `chunks` and [XML tags](https://wiki.apertium.org/w/index.php?title=List_of_symbols#XML_tags) be added? [No](https://github.com/apertium/apertium/issues/185).
-* Add conversions Apertium -> UD, UD -> Apertium based on the constructed JSON file
-* Upload the converter as a package to PyPI
 * Tests: Apertium -> UD -> Apertium, UD -> Apertium -> UD (sometimes losses are inevitable)
 
 ## How to cite
 
 Greatly appreciated, if you use this work.
 
 ```
```

### Comparing `apertium2ud-0.0.1/apertium2ud.egg-info/PKG-INFO` & `apertium2ud-0.0.2/apertium2ud.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,16 +23,27 @@
 hence the GPLv3 license.
 
 To build the machine-readable mapping, run
 
 ```bash
 python apertium_wiki_parser.py
 ```
+## Apertium to Universal tags
 
-## UD to Apertium
+```
+>>> from apertium2ud.convert import a2ud
+>>> tags = ["n", "pl", "acc"]
+>>> a2ud(tags)
+(['NOUN'], ['Number=Plur', 'Case=Acc'])
+>>> tags_sophisticated = ["v", "tv", "ger", "nom", "cop", "aor", "p3", "pl"]
+>>> a2ud(tags_sophisticated)
+(['VERB', 'AUX'], ['Subcat=Tran', 'VerbForm=Vnoun', 'Case=Nom', 'Tense=Past', 'Person=3', 'Number=Plur'])
+```
+
+## Universal tags to Apertium
 
 So far the conversion is far from perfect
 ```
 Кыз NOUN {'Number[psor]=Sing', 'Number=Sing', 'Case=Nom', 'Person[psor]=3', 'Person=3'} ->
 <px3sg><n><subj?nom?><sg><p3><px3sp> 
 
 досуна NOUN {'Number[psor]=Sing', 'Number=Sing', 'Person[psor]=3', 'Case=Dat', 'Person=3'} ->
@@ -47,16 +58,14 @@
 . PUNCT set() ->
 <sent?apos?percent?clb?punct?> 
 ```
 
 ## TODO
 
 * Should sections `chunks` and [XML tags](https://wiki.apertium.org/w/index.php?title=List_of_symbols#XML_tags) be added? [No](https://github.com/apertium/apertium/issues/185).
-* Add conversions Apertium -> UD, UD -> Apertium based on the constructed JSON file
-* Upload the converter as a package to PyPI
 * Tests: Apertium -> UD -> Apertium, UD -> Apertium -> UD (sometimes losses are inevitable)
 
 ## How to cite
 
 Greatly appreciated, if you use this work.
 
 ```
```

### Comparing `apertium2ud-0.0.1/setup.py` & `apertium2ud-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apertium2ud",
     packages=setuptools.find_packages(),
-    version="0.0.1",
+    version="0.0.2",
     description="Converting universal tags to Apertium tags.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Anton Alekseev",
     author_email="anton.m.alexeye@gmail.com",
     url="https://github.com/alexeyev/apertium2ud",
     keywords=["natural language processing", "apertium", "morphology"],
```

