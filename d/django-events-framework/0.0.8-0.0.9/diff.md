# Comparing `tmp/django-events-framework-0.0.8.tar.gz` & `tmp/django-events-framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-events-framework-0.0.8.tar", last modified: Fri Mar  4 10:57:38 2022, max compression
+gzip compressed data, was "django-events-framework-0.0.9.tar", last modified: Wed May 24 20:29:24 2023, max compression
```

## Comparing `django-events-framework-0.0.8.tar` & `django-events-framework-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-04 10:57:38.766779 django-events-framework-0.0.8/
--rw-r--r--   0 root         (0) root         (0)       76 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1061 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1541 2022-03-04 10:57:38.769308 django-events-framework-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-04 10:57:38.636339 django-events-framework-0.0.8/django_events_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1541 2022-03-04 10:57:37.000000 django-events-framework-0.0.8/django_events_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      617 2022-03-04 10:57:38.000000 django-events-framework-0.0.8/django_events_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-04 10:57:37.000000 django-events-framework-0.0.8/django_events_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-04 10:57:37.000000 django-events-framework-0.0.8/django_events_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-03-04 10:57:38.000000 django-events-framework-0.0.8/django_events_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-04 10:57:38.715848 django-events-framework-0.0.8/events_framework/
--rw-r--r--   0 root         (0) root         (0)      604 2022-03-04 10:43:53.000000 django-events-framework-0.0.8/events_framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)      308 2022-03-04 10:41:56.000000 django-events-framework-0.0.8/events_framework/apps.py
--rw-r--r--   0 root         (0) root         (0)      271 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/events_framework/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-04 10:57:38.728071 django-events-framework-0.0.8/events_framework/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/events_framework/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-04 10:57:38.757808 django-events-framework-0.0.8/events_framework/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/events_framework/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      175 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/events_framework/management/commands/process_events.py
--rw-r--r--   0 root         (0) root         (0)     1305 2022-03-04 10:40:03.000000 django-events-framework-0.0.8/events_framework/manager.py
--rw-r--r--   0 root         (0) root         (0)      768 2021-12-21 07:05:16.000000 django-events-framework-0.0.8/events_framework/models.py
--rw-r--r--   0 root         (0) root         (0)      162 2021-12-21 06:35:22.000000 django-events-framework-0.0.8/events_framework/utils.py
--rw-r--r--   0 root         (0) root         (0)       96 2021-12-21 06:43:54.000000 django-events-framework-0.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1863 2022-03-04 10:57:38.775882 django-events-framework-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1344 2022-03-04 10:44:19.000000 django-events-framework-0.0.8/setup.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-24 20:29:24.500210 django-events-framework-0.0.9/
+-rw-r--r--   0 dev        (501) staff       (20)       79 2023-05-24 20:27:10.000000 django-events-framework-0.0.9/AUTHORS
+-rw-r--r--   0 dev        (501) staff       (20)     1061 2021-12-20 17:16:00.000000 django-events-framework-0.0.9/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)       82 2021-12-20 23:26:50.000000 django-events-framework-0.0.9/MANIFEST.in
+-rw-r--r--   0 dev        (501) staff       (20)     1540 2023-05-24 20:29:24.500278 django-events-framework-0.0.9/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      397 2021-12-20 22:54:14.000000 django-events-framework-0.0.9/README.md
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-24 20:29:24.498853 django-events-framework-0.0.9/django_events_framework.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)     1540 2023-05-24 20:29:24.000000 django-events-framework-0.0.9/django_events_framework.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      617 2023-05-24 20:29:24.000000 django-events-framework-0.0.9/django_events_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2023-05-24 20:29:24.000000 django-events-framework-0.0.9/django_events_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)       29 2023-05-24 20:29:24.000000 django-events-framework-0.0.9/django_events_framework.egg-info/requires.txt
+-rw-r--r--   0 dev        (501) staff       (20)       17 2023-05-24 20:29:24.000000 django-events-framework-0.0.9/django_events_framework.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-24 20:29:24.499597 django-events-framework-0.0.9/events_framework/
+-rw-r--r--   0 dev        (501) staff       (20)      449 2022-02-08 17:56:59.000000 django-events-framework-0.0.9/events_framework/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)      308 2021-12-20 17:16:03.000000 django-events-framework-0.0.9/events_framework/apps.py
+-rw-r--r--   0 dev        (501) staff       (20)      271 2021-12-20 23:57:22.000000 django-events-framework-0.0.9/events_framework/decorators.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-24 20:29:24.499746 django-events-framework-0.0.9/events_framework/management/
+-rw-r--r--   0 dev        (501) staff       (20)        0 2021-12-20 17:16:03.000000 django-events-framework-0.0.9/events_framework/management/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-24 20:29:24.500008 django-events-framework-0.0.9/events_framework/management/commands/
+-rw-r--r--   0 dev        (501) staff       (20)        0 2021-12-20 17:16:03.000000 django-events-framework-0.0.9/events_framework/management/commands/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)      175 2021-12-20 23:58:41.000000 django-events-framework-0.0.9/events_framework/management/commands/process_events.py
+-rw-r--r--   0 dev        (501) staff       (20)     1305 2022-02-08 17:59:46.000000 django-events-framework-0.0.9/events_framework/manager.py
+-rw-r--r--   0 dev        (501) staff       (20)      915 2023-05-24 20:07:11.000000 django-events-framework-0.0.9/events_framework/models.py
+-rw-r--r--   0 dev        (501) staff       (20)      162 2021-12-20 17:16:03.000000 django-events-framework-0.0.9/events_framework/utils.py
+-rw-r--r--   0 dev        (501) staff       (20)       96 2022-02-08 17:54:31.000000 django-events-framework-0.0.9/requirements.txt
+-rw-r--r--   0 dev        (501) staff       (20)     1863 2023-05-24 20:29:24.500681 django-events-framework-0.0.9/setup.cfg
+-rw-r--r--   0 dev        (501) staff       (20)     1344 2023-05-24 20:27:30.000000 django-events-framework-0.0.9/setup.py
```

### Comparing `django-events-framework-0.0.8/LICENSE` & `django-events-framework-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-events-framework-0.0.8/PKG-INFO` & `django-events-framework-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-events-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: An events framework for logging and processing Django models events.
 Home-page: https://github.com/Reve/django-events-framework
 Author: Alexandru Gheorghita
 Author-email: gheorghitacristian@mac.com
 Maintainer: Alexandru Gheorghita
 Maintainer-email: gheorghitacristian@mac.ro
 License: MIT
@@ -51,8 +51,7 @@
 
 ```text
 INSTALLED_APPS = [
     ...,
     "events_framework"
 ]
 ```
-
```

### Comparing `django-events-framework-0.0.8/django_events_framework.egg-info/PKG-INFO` & `django-events-framework-0.0.9/django_events_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-events-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: An events framework for logging and processing Django models events.
 Home-page: https://github.com/Reve/django-events-framework
 Author: Alexandru Gheorghita
 Author-email: gheorghitacristian@mac.com
 Maintainer: Alexandru Gheorghita
 Maintainer-email: gheorghitacristian@mac.ro
 License: MIT
@@ -51,8 +51,7 @@
 
 ```text
 INSTALLED_APPS = [
     ...,
     "events_framework"
 ]
 ```
-
```

### Comparing `django-events-framework-0.0.8/django_events_framework.egg-info/SOURCES.txt` & `django-events-framework-0.0.9/django_events_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-events-framework-0.0.8/events_framework/manager.py` & `django-events-framework-0.0.9/events_framework/manager.py`

 * *Files identical despite different names*

### Comparing `django-events-framework-0.0.8/events_framework/models.py` & `django-events-framework-0.0.9/events_framework/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,13 +23,21 @@
     )
 
     processed = models.BooleanField(
         _("Proccesed"),
         default=False,
     )
 
+    error = models.BooleanField(
+        _("Has error?"),
+        default=False,
+    )
+
+    error_message = models.TextField(_("Error message"))
+
     class Meta:
         abstract = True
         ordering = ("date",)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(type={self.type!r})"
+
```

### Comparing `django-events-framework-0.0.8/setup.cfg` & `django-events-framework-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-events-framework-0.0.8/setup.py` & `django-events-framework-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="django-events-framework",
-    version="0.0.8",
+    version="0.0.9",
     author="Alexandru Gheorghita",
     author_email="gheorghitacristian@mac.com",
     description="An events framework for logging and processing Django models events.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points="",
     url="https://github.com/Reve/django-events-framework",
```

