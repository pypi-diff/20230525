# Comparing `tmp/dj-jwt-auth-0.3.0.tar.gz` & `tmp/dj-jwt-auth-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-0.3.0.tar", last modified: Wed Dec  7 14:42:43 2022, max compression
+gzip compressed data, was "dj-jwt-auth-0.3.1.tar", last modified: Thu May 25 14:31:59 2023, max compression
```

## Comparing `dj-jwt-auth-0.3.0.tar` & `dj-jwt-auth-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-12-07 14:42:43.644670 dj-jwt-auth-0.3.0/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2344 2022-12-07 14:42:43.644820 dj-jwt-auth-0.3.0/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1454 2022-10-24 08:47:04.000000 dj-jwt-auth-0.3.0/README.md
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-12-07 14:42:43.637143 dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2344 2022-12-07 14:42:43.000000 dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      418 2022-12-07 14:42:43.000000 dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        1 2022-12-07 14:42:43.000000 dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       68 2022-12-07 14:42:43.000000 dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       17 2022-12-07 14:42:43.000000 dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-12-07 14:42:43.641425 dj-jwt-auth-0.3.0/django_jwt/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 11:25:09.000000 dj-jwt-auth-0.3.0/django_jwt/__init__.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1111 2022-11-21 13:54:58.000000 dj-jwt-auth-0.3.0/django_jwt/jwt.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1022 2022-10-27 12:06:32.000000 dj-jwt-auth-0.3.0/django_jwt/middleware.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      778 2022-10-14 14:12:54.000000 dj-jwt-auth-0.3.0/django_jwt/settings.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1967 2022-10-24 09:36:32.000000 dj-jwt-auth-0.3.0/django_jwt/user.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      200 2022-12-07 14:39:32.000000 dj-jwt-auth-0.3.0/django_jwt/views.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      221 2022-10-24 09:36:12.000000 dj-jwt-auth-0.3.0/pyproject.toml
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      959 2022-12-07 14:42:43.645497 dj-jwt-auth-0.3.0/setup.cfg
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       90 2022-10-24 09:36:32.000000 dj-jwt-auth-0.3.0/setup.py
-drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-12-07 14:42:43.644007 dj-jwt-auth-0.3.0/tests/
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 13:02:24.000000 dj-jwt-auth-0.3.0/tests/__init__.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      190 2022-10-14 08:57:49.000000 dj-jwt-auth-0.3.0/tests/models.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     3974 2022-10-24 09:36:56.000000 dj-jwt-auth-0.3.0/tests/test_middleware.py
--rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      212 2022-10-14 10:04:40.000000 dj-jwt-auth-0.3.0/tests/urls.py
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.669137 dj-jwt-auth-0.3.1/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2385 2023-05-25 14:31:59.669339 dj-jwt-auth-0.3.1/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1444 2023-05-25 14:31:29.000000 dj-jwt-auth-0.3.1/README.md
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.661285 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2385 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      418 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        1 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       63 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       17 2023-05-25 14:31:59.000000 dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.665417 dj-jwt-auth-0.3.1/django_jwt/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 11:25:09.000000 dj-jwt-auth-0.3.1/django_jwt/__init__.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1111 2022-11-21 13:54:58.000000 dj-jwt-auth-0.3.1/django_jwt/jwt.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1022 2022-10-27 12:06:32.000000 dj-jwt-auth-0.3.1/django_jwt/middleware.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      778 2022-10-14 14:12:54.000000 dj-jwt-auth-0.3.1/django_jwt/settings.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1967 2022-10-24 09:36:32.000000 dj-jwt-auth-0.3.1/django_jwt/user.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      200 2022-12-07 14:39:32.000000 dj-jwt-auth-0.3.1/django_jwt/views.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      221 2022-10-24 09:36:12.000000 dj-jwt-auth-0.3.1/pyproject.toml
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      991 2023-05-25 14:31:59.670183 dj-jwt-auth-0.3.1/setup.cfg
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       90 2022-10-24 09:36:32.000000 dj-jwt-auth-0.3.1/setup.py
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-05-25 14:31:59.668393 dj-jwt-auth-0.3.1/tests/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 13:02:24.000000 dj-jwt-auth-0.3.1/tests/__init__.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      190 2022-10-14 08:57:49.000000 dj-jwt-auth-0.3.1/tests/models.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     3974 2022-10-24 09:36:56.000000 dj-jwt-auth-0.3.1/tests/test_middleware.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      212 2022-10-14 10:04:40.000000 dj-jwt-auth-0.3.1/tests/urls.py
```

### Comparing `dj-jwt-auth-0.3.0/PKG-INFO` & `dj-jwt-auth-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -12,22 +12,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-=====
-Django-JWT
-=====
+# Django-JWT
 
 This is a package to verify and validate JSON Web Tokens (JWT) in Django.
 
 ### Installation
 1. Install the package using pip.
 
 2. Add "django_jwt" to your INSTALLED_APPS setting like this::
```

### Comparing `dj-jwt-auth-0.3.0/README.md` & `dj-jwt-auth-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-=====
-Django-JWT
-=====
+# Django-JWT
 
 This is a package to verify and validate JSON Web Tokens (JWT) in Django.
 
 ### Installation
 1. Install the package using pip.
 
 2. Add "django_jwt" to your INSTALLED_APPS setting like this::
```

### Comparing `dj-jwt-auth-0.3.0/dj_jwt_auth.egg-info/PKG-INFO` & `dj-jwt-auth-0.3.1/dj_jwt_auth.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -12,22 +12,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-=====
-Django-JWT
-=====
+# Django-JWT
 
 This is a package to verify and validate JSON Web Tokens (JWT) in Django.
 
 ### Installation
 1. Install the package using pip.
 
 2. Add "django_jwt" to your INSTALLED_APPS setting like this::
```

### Comparing `dj-jwt-auth-0.3.0/django_jwt/jwt.py` & `dj-jwt-auth-0.3.1/django_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-0.3.0/django_jwt/middleware.py` & `dj-jwt-auth-0.3.1/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-0.3.0/django_jwt/settings.py` & `dj-jwt-auth-0.3.1/django_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-0.3.0/django_jwt/user.py` & `dj-jwt-auth-0.3.1/django_jwt/user.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-0.3.0/setup.cfg` & `dj-jwt-auth-0.3.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 0.3.0
+version = 0.3.1
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers = 
@@ -14,24 +14,25 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	Django >= 3.0 , < 4.0
-	pyjwt == 2.5.0
+	Django >= 3.0
+	pyjwt >= 2.5.0
 	requests >= 2.28.1
 	cryptography >= 36.0.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dj-jwt-auth-0.3.0/tests/test_middleware.py` & `dj-jwt-auth-0.3.1/tests/test_middleware.py`

 * *Files identical despite different names*

