# Comparing `tmp/giant_mixins-0.3.4.tar.gz` & `tmp/giant_mixins-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_mixins-0.3.4.tar", max compression
+gzip compressed data, was "giant_mixins-0.3.5.tar", max compression
```

## Comparing `giant_mixins-0.3.4.tar` & `giant_mixins-0.3.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/LICENSE
--rw-r--r--   0        0        0      616 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/README.md
--rw-r--r--   0        0        0       24 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/mixins/__init__.py
--rw-r--r--   0        0        0     1912 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/mixins/admin.py
--rw-r--r--   0        0        0      262 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/mixins/fields.py
--rw-r--r--   0        0        0     4275 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/mixins/models.py
--rw-r--r--   0        0        0      468 2023-03-07 12:58:37.843017 giant_mixins-0.3.4/mixins/views.py
--rw-r--r--   0        0        0     1080 2023-03-07 15:29:35.315991 giant_mixins-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 giant_mixins-0.3.4/setup.py
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 giant_mixins-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-25 07:42:00.700610 giant_mixins-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1522 2023-05-25 08:14:32.730594 giant_mixins-0.3.5/README.md
+-rw-r--r--   0        0        0       24 2023-05-25 07:42:00.700896 giant_mixins-0.3.5/mixins/__init__.py
+-rw-r--r--   0        0        0     1912 2023-05-25 07:42:00.701013 giant_mixins-0.3.5/mixins/admin.py
+-rw-r--r--   0        0        0      262 2023-05-25 07:42:00.701126 giant_mixins-0.3.5/mixins/fields.py
+-rw-r--r--   0        0        0     4373 2023-05-25 08:14:32.731001 giant_mixins-0.3.5/mixins/models.py
+-rw-r--r--   0        0        0      468 2023-05-25 07:42:00.701352 giant_mixins-0.3.5/mixins/views.py
+-rw-r--r--   0        0        0     1080 2023-05-25 08:14:32.731373 giant_mixins-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 giant_mixins-0.3.5/PKG-INFO
```

### Comparing `giant_mixins-0.3.4/LICENSE` & `giant_mixins-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_mixins-0.3.4/mixins/admin.py` & `giant_mixins-0.3.5/mixins/admin.py`

 * *Files identical despite different names*

### Comparing `giant_mixins-0.3.4/mixins/models.py` & `giant_mixins-0.3.5/mixins/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     file = FilerFileField(
         related_name="%(app_label)s_%(class)s_files",
         verbose_name="File",
         blank=True,
         null=True,
         on_delete=models.SET_NULL,
     )
+    new_tab = models.BooleanField(default=False, help_text="Open this link in a new tab/window.")
 
     class Meta:
         abstract = True
 
     def get_absolute_url(self):
         """
         Returns the URL's in order of importance
```

### Comparing `giant_mixins-0.3.4/pyproject.toml` & `giant_mixins-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-mixins"
-version = "0.3.4"
+version = "0.3.5"
 description = "A mixins app that provides some standard mixins for Giant projects"
 authors = ["Will-Hoey <will.hoey@giantmade.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-mixins"
 repository = "https://github.com/giantmade/giant-mixins"
 keywords = ["mixins", "app"]
```

### Comparing `giant_mixins-0.3.4/PKG-INFO` & `giant_mixins-0.3.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-mixins
-Version: 0.3.4
+Version: 0.3.5
 Summary: A mixins app that provides some standard mixins for Giant projects
 Home-page: https://github.com/giantmade/giant-mixins
 License: MIT
 Keywords: mixins,app
 Author: Will-Hoey
 Author-email: will.hoey@giantmade.com
 Requires-Python: >=3.9,<4.0
@@ -36,7 +36,24 @@
 
 However if your project has django-cms installed then you can make use of the full range of mixins in this app. For this, install the package with the extra dependencies,
 
     $ poetry add giant-mixins --extras "cms"
 
 You should then add `"mixins"` to the `INSTALLED_APPS` in your settings file.
 
+## Preparing for release
+
+In order to prep the package for a new release on TestPyPi and PyPi there is one key thing that you need to do. You need to update the version number in the `pyproject.toml`.
+This is so that the package can be published without running into version number conflicts. The version numbering must also follow the Semantic Version rules which can be found here https://semver.org/.
+
+## Publishing
+
+Publishing a package with poetry is incredibly easy. Once you have checked that the version number has been updated (not the same as a previous version) then you only need to run two commands.
+
+    $ `poetry build`
+
+will package the project up for you into a way that can be published.
+
+    $ `poetry publish`
+
+will publish the package to PyPi. You will need to enter the company username (Giant-Digital) and password for the account which can be found in the company password manager
+
```

