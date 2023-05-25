# Comparing `tmp/django-sweet-utils-1.3.2.tar.gz` & `tmp/django-sweet-utils-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sweet-utils-1.3.2.tar", last modified: Mon Mar 27 08:55:33 2023, max compression
+gzip compressed data, was "django-sweet-utils-1.3.3.tar", last modified: Thu May 25 16:17:09 2023, max compression
```

## Comparing `django-sweet-utils-1.3.2.tar` & `django-sweet-utils-1.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.164648 django-sweet-utils-1.3.2/
--rw-r--r--   0 rustam     (501) staff       (20)     1545 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/LICENSE
--rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     3043 2023-03-27 08:55:33.164766 django-sweet-utils-1.3.2/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)     1677 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.156531 django-sweet-utils-1.3.2/django_sweet_utils/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/django_sweet_utils/__init__.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.159863 django-sweet-utils-1.3.2/django_sweet_utils/api/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/django_sweet_utils/api/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1438 2023-02-24 11:38:03.000000 django-sweet-utils-1.3.2/django_sweet_utils/api/metadata.py
--rw-r--r--   0 rustam     (501) staff       (20)      246 2023-02-24 12:25:50.000000 django-sweet-utils-1.3.2/django_sweet_utils/api/permissions.py
--rw-r--r--   0 rustam     (501) staff       (20)      962 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/django_sweet_utils/api/views.py
--rw-r--r--   0 rustam     (501) staff       (20)      166 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/django_sweet_utils/apps.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.160481 django-sweet-utils-1.3.2/django_sweet_utils/db/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/django_sweet_utils/db/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     2159 2023-03-27 08:55:23.000000 django-sweet-utils-1.3.2/django_sweet_utils/db/models.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.161455 django-sweet-utils-1.3.2/django_sweet_utils/misc/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/django_sweet_utils/misc/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      342 2022-12-22 11:02:57.000000 django-sweet-utils-1.3.2/django_sweet_utils/misc/json.py
--rw-r--r--   0 rustam     (501) staff       (20)     1465 2022-12-20 04:47:46.000000 django-sweet-utils-1.3.2/django_sweet_utils/misc/logging.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.162222 django-sweet-utils-1.3.2/django_sweet_utils/serializers/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-01-26 10:20:33.000000 django-sweet-utils-1.3.2/django_sweet_utils/serializers/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1213 2023-02-10 07:18:14.000000 django-sweet-utils-1.3.2/django_sweet_utils/serializers/fields.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.163994 django-sweet-utils-1.3.2/django_sweet_utils/templatetags/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.2/django_sweet_utils/templatetags/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      169 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.2/django_sweet_utils/templatetags/format_str.py
--rw-r--r--   0 rustam     (501) staff       (20)     4670 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.2/django_sweet_utils/templatetags/query_string.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-03-27 08:55:33.157786 django-sweet-utils-1.3.2/django_sweet_utils.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     3043 2023-03-27 08:55:33.000000 django-sweet-utils-1.3.2/django_sweet_utils.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      846 2023-03-27 08:55:33.000000 django-sweet-utils-1.3.2/django_sweet_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-03-27 08:55:33.000000 django-sweet-utils-1.3.2/django_sweet_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       32 2023-03-27 08:55:33.000000 django-sweet-utils-1.3.2/django_sweet_utils.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       19 2023-03-27 08:55:33.000000 django-sweet-utils-1.3.2/django_sweet_utils.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1212 2023-03-27 08:55:33.165385 django-sweet-utils-1.3.2/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.2/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.673938 django-sweet-utils-1.3.3/
+-rw-r--r--   0 rustam     (501) staff       (20)     1545 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/LICENSE
+-rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     3043 2023-05-25 16:17:09.674099 django-sweet-utils-1.3.3/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     1677 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.618015 django-sweet-utils-1.3.3/django_sweet_utils/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/django_sweet_utils/__init__.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.630777 django-sweet-utils-1.3.3/django_sweet_utils/api/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/django_sweet_utils/api/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1438 2023-02-24 11:38:03.000000 django-sweet-utils-1.3.3/django_sweet_utils/api/metadata.py
+-rw-r--r--   0 rustam     (501) staff       (20)      246 2023-02-24 12:25:50.000000 django-sweet-utils-1.3.3/django_sweet_utils/api/permissions.py
+-rw-r--r--   0 rustam     (501) staff       (20)      962 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/django_sweet_utils/api/views.py
+-rw-r--r--   0 rustam     (501) staff       (20)      166 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/django_sweet_utils/apps.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.631433 django-sweet-utils-1.3.3/django_sweet_utils/db/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/django_sweet_utils/db/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     2232 2023-05-25 16:16:51.000000 django-sweet-utils-1.3.3/django_sweet_utils/db/models.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.670951 django-sweet-utils-1.3.3/django_sweet_utils/misc/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/django_sweet_utils/misc/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      342 2022-12-22 11:02:57.000000 django-sweet-utils-1.3.3/django_sweet_utils/misc/json.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1465 2022-12-20 04:47:46.000000 django-sweet-utils-1.3.3/django_sweet_utils/misc/logging.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.671898 django-sweet-utils-1.3.3/django_sweet_utils/serializers/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-01-26 10:20:33.000000 django-sweet-utils-1.3.3/django_sweet_utils/serializers/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1213 2023-02-10 07:18:14.000000 django-sweet-utils-1.3.3/django_sweet_utils/serializers/fields.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.673405 django-sweet-utils-1.3.3/django_sweet_utils/templatetags/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.3/django_sweet_utils/templatetags/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      169 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.3/django_sweet_utils/templatetags/format_str.py
+-rw-r--r--   0 rustam     (501) staff       (20)     4670 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.3/django_sweet_utils/templatetags/query_string.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:17:09.629222 django-sweet-utils-1.3.3/django_sweet_utils.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     3043 2023-05-25 16:17:09.000000 django-sweet-utils-1.3.3/django_sweet_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      846 2023-05-25 16:17:09.000000 django-sweet-utils-1.3.3/django_sweet_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-05-25 16:17:09.000000 django-sweet-utils-1.3.3/django_sweet_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       32 2023-05-25 16:17:09.000000 django-sweet-utils-1.3.3/django_sweet_utils.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       19 2023-05-25 16:17:09.000000 django-sweet-utils-1.3.3/django_sweet_utils.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1212 2023-05-25 16:17:09.674653 django-sweet-utils-1.3.3/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.3/setup.py
```

### Comparing `django-sweet-utils-1.3.2/LICENSE` & `django-sweet-utils-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/PKG-INFO` & `django-sweet-utils-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sweet-utils
-Version: 1.3.2
+Version: 1.3.3
 Summary: A little django code sugar.
 Home-page: https://github.com/HarleyK1ng/django-sweet-utils
 Author: Astafeev Rustam
 Author-email: astafeev0308@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-sweet-utils-1.3.2/README.md` & `django-sweet-utils-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils/api/metadata.py` & `django-sweet-utils-1.3.3/django_sweet_utils/api/metadata.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils/api/views.py` & `django-sweet-utils-1.3.3/django_sweet_utils/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils/db/models.py` & `django-sweet-utils-1.3.3/django_sweet_utils/db/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 class FakeDeletionQuerySet(models.query.QuerySet):
     # Fake deletion that also "deletes" related objects
     def delete(self):
         self.update(is_deleted=True)
         for obj in self:
             delete_related(obj)
 
+    # Real deletion
+    def hard_delete(self):
+        super().delete()
+
 
 class Manager(models.Manager):
     """ Base manager with the following additions:
         - 'existing()' method that filters queryset by 'is_deleted=False'
         - 'get_or_none()' method that returns object or None
         - 'delete()' method that only sets 'is_deleted' field to True and also "deletes" related objects
     """
```

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils/misc/logging.py` & `django-sweet-utils-1.3.3/django_sweet_utils/misc/logging.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils/serializers/fields.py` & `django-sweet-utils-1.3.3/django_sweet_utils/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils/templatetags/query_string.py` & `django-sweet-utils-1.3.3/django_sweet_utils/templatetags/query_string.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils.egg-info/PKG-INFO` & `django-sweet-utils-1.3.3/django_sweet_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sweet-utils
-Version: 1.3.2
+Version: 1.3.3
 Summary: A little django code sugar.
 Home-page: https://github.com/HarleyK1ng/django-sweet-utils
 Author: Astafeev Rustam
 Author-email: astafeev0308@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-sweet-utils-1.3.2/django_sweet_utils.egg-info/SOURCES.txt` & `django-sweet-utils-1.3.3/django_sweet_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.2/setup.cfg` & `django-sweet-utils-1.3.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-sweet-utils
-version = 1.3.2
+version = 1.3.3
 description = A little django code sugar.
 url = https://github.com/HarleyK1ng/django-sweet-utils
 author = Astafeev Rustam
 author_email = astafeev0308@gmail.com
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
```

