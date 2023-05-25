# Comparing `tmp/django-walletpass-2.0.tar.gz` & `tmp/django-walletpass-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-walletpass-2.0.tar", last modified: Mon Jan  9 17:18:34 2023, max compression
+gzip compressed data, was "django-walletpass-3.0.tar", last modified: Thu May 25 15:41:06 2023, max compression
```

## Comparing `django-walletpass-2.0.tar` & `django-walletpass-3.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-01-09 17:18:34.411499 django-walletpass-2.0/
--rw-r--r--   0 user       (501) staff       (20)      335 2023-01-09 17:14:17.000000 django-walletpass-2.0/CHANGELOG.md
--rw-r--r--   0 user       (501) staff       (20)     1545 2023-01-09 11:52:46.000000 django-walletpass-2.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     1052 2023-01-09 11:52:46.000000 django-walletpass-2.0/LICENSE.old
--rw-r--r--   0 user       (501) staff       (20)      130 2023-01-09 11:52:46.000000 django-walletpass-2.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     7292 2023-01-09 17:18:34.411357 django-walletpass-2.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     5859 2023-01-09 17:11:25.000000 django-walletpass-2.0/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-01-09 17:18:34.408455 django-walletpass-2.0/django_walletpass/
--rw-r--r--   0 user       (501) staff       (20)      117 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      180 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/admin.py
--rw-r--r--   0 user       (501) staff       (20)      231 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/apps.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-01-09 17:18:34.409451 django-walletpass-2.0/django_walletpass/certs/
--rw-r--r--   0 user       (501) staff       (20)     1062 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/certs/AppleWWDRCA.cer
--rw-r--r--   0 user       (501) staff       (20)     1493 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/certs/AppleWWDRCA.pem
--rw-r--r--   0 user       (501) staff       (20)     4987 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/classviews.py
--rw-r--r--   0 user       (501) staff       (20)     1797 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/crypto.py
--rw-r--r--   0 user       (501) staff       (20)      140 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/files.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-01-09 17:18:34.410814 django-walletpass-2.0/django_walletpass/migrations/
--rw-r--r--   0 user       (501) staff       (20)     1663 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0001_initial.py
--rw-r--r--   0 user       (501) staff       (20)      351 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0002_auto_20190429_1819.py
--rw-r--r--   0 user       (501) staff       (20)      483 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0003_auto_20190610_1434.py
--rw-r--r--   0 user       (501) staff       (20)      407 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0004_auto_20190611_1306.py
--rw-r--r--   0 user       (501) staff       (20)      909 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0005_auto_20190613_1433.py
--rw-r--r--   0 user       (501) staff       (20)      521 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0006_auto_20190613_1607.py
--rw-r--r--   0 user       (501) staff       (20)      400 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/0007_auto_20190613_1807.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/migrations/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    11882 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/models.py
--rw-r--r--   0 user       (501) staff       (20)     2646 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/services.py
--rw-r--r--   0 user       (501) staff       (20)     2102 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/settings.py
--rw-r--r--   0 user       (501) staff       (20)      249 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/signals.py
--rw-r--r--   0 user       (501) staff       (20)      238 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/storage.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-01-09 17:18:34.411099 django-walletpass-2.0/django_walletpass/tests/
--rw-r--r--   0 user       (501) staff       (20)       77 2023-01-09 11:52:46.000000 django-walletpass-2.0/django_walletpass/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2030 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/tests/main.py
--rw-r--r--   0 user       (501) staff       (20)      980 2023-01-09 17:11:25.000000 django-walletpass-2.0/django_walletpass/urls.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-01-09 17:18:34.409161 django-walletpass-2.0/django_walletpass.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     7292 2023-01-09 17:18:34.000000 django-walletpass-2.0/django_walletpass.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1179 2023-01-09 17:18:34.000000 django-walletpass-2.0/django_walletpass.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-01-09 17:18:34.000000 django-walletpass-2.0/django_walletpass.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       80 2023-01-09 17:18:34.000000 django-walletpass-2.0/django_walletpass.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       18 2023-01-09 17:18:34.000000 django-walletpass-2.0/django_walletpass.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-01-09 17:18:34.411545 django-walletpass-2.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1898 2023-01-09 17:15:11.000000 django-walletpass-2.0/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-25 15:41:06.876347 django-walletpass-3.0/
+-rw-r--r--   0 user       (501) staff       (20)      618 2023-05-25 15:33:11.000000 django-walletpass-3.0/CHANGELOG.md
+-rw-r--r--   0 user       (501) staff       (20)     1545 2023-01-09 11:52:46.000000 django-walletpass-3.0/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     1052 2023-01-09 11:52:46.000000 django-walletpass-3.0/LICENSE.old
+-rw-r--r--   0 user       (501) staff       (20)      130 2023-01-09 11:52:46.000000 django-walletpass-3.0/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     7483 2023-05-25 15:41:06.876221 django-walletpass-3.0/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     6050 2023-05-25 15:33:11.000000 django-walletpass-3.0/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-25 15:41:06.873515 django-walletpass-3.0/django_walletpass/
+-rw-r--r--   0 user       (501) staff       (20)      117 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      180 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/admin.py
+-rw-r--r--   0 user       (501) staff       (20)      231 2023-01-09 17:26:21.000000 django-walletpass-3.0/django_walletpass/apps.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-25 15:41:06.874364 django-walletpass-3.0/django_walletpass/certs/
+-rw-r--r--   0 user       (501) staff       (20)     1062 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/certs/AppleWWDRCA.cer
+-rw-r--r--   0 user       (501) staff       (20)     1493 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/certs/AppleWWDRCA.pem
+-rw-r--r--   0 user       (501) staff       (20)     5509 2023-05-25 15:33:11.000000 django-walletpass-3.0/django_walletpass/classviews.py
+-rw-r--r--   0 user       (501) staff       (20)     1797 2023-01-09 17:26:21.000000 django-walletpass-3.0/django_walletpass/crypto.py
+-rw-r--r--   0 user       (501) staff       (20)      140 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/files.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-25 15:41:06.875793 django-walletpass-3.0/django_walletpass/migrations/
+-rw-r--r--   0 user       (501) staff       (20)     1663 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0001_initial.py
+-rw-r--r--   0 user       (501) staff       (20)      351 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0002_auto_20190429_1819.py
+-rw-r--r--   0 user       (501) staff       (20)      483 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0003_auto_20190610_1434.py
+-rw-r--r--   0 user       (501) staff       (20)      407 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0004_auto_20190611_1306.py
+-rw-r--r--   0 user       (501) staff       (20)      909 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0005_auto_20190613_1433.py
+-rw-r--r--   0 user       (501) staff       (20)      521 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0006_auto_20190613_1607.py
+-rw-r--r--   0 user       (501) staff       (20)      400 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/0007_auto_20190613_1807.py
+-rw-r--r--   0 user       (501) staff       (20)      504 2023-05-25 13:43:01.000000 django-walletpass-3.0/django_walletpass/migrations/0008_alter_pass_data.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/migrations/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    11956 2023-05-25 15:33:11.000000 django-walletpass-3.0/django_walletpass/models.py
+-rw-r--r--   0 user       (501) staff       (20)     1854 2023-05-25 15:33:11.000000 django-walletpass-3.0/django_walletpass/services.py
+-rw-r--r--   0 user       (501) staff       (20)     2102 2023-01-09 17:26:21.000000 django-walletpass-3.0/django_walletpass/settings.py
+-rw-r--r--   0 user       (501) staff       (20)      249 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/signals.py
+-rw-r--r--   0 user       (501) staff       (20)      238 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/storage.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-25 15:41:06.876026 django-walletpass-3.0/django_walletpass/tests/
+-rw-r--r--   0 user       (501) staff       (20)       77 2023-01-09 11:52:46.000000 django-walletpass-3.0/django_walletpass/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3146 2023-05-25 15:33:11.000000 django-walletpass-3.0/django_walletpass/tests/main.py
+-rw-r--r--   0 user       (501) staff       (20)      980 2023-01-09 17:26:21.000000 django-walletpass-3.0/django_walletpass/urls.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-25 15:41:06.874087 django-walletpass-3.0/django_walletpass.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     7483 2023-05-25 15:41:06.000000 django-walletpass-3.0/django_walletpass.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1232 2023-05-25 15:41:06.000000 django-walletpass-3.0/django_walletpass.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-25 15:41:06.000000 django-walletpass-3.0/django_walletpass.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       96 2023-05-25 15:41:06.000000 django-walletpass-3.0/django_walletpass.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       18 2023-05-25 15:41:06.000000 django-walletpass-3.0/django_walletpass.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-25 15:41:06.876383 django-walletpass-3.0/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1924 2023-05-25 15:33:11.000000 django-walletpass-3.0/setup.py
```

### Comparing `django-walletpass-2.0/LICENSE` & `django-walletpass-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/LICENSE.old` & `django-walletpass-3.0/LICENSE.old`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/PKG-INFO` & `django-walletpass-3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-walletpass
-Version: 2.0
+Version: 3.0
 Summary: Django .pkpass builder, server and push notifications
 Home-page: http://github.com/develatio/django-walletpass/
 Author: Develatio Technologies S.L.
 Author-email: contacto@develat.io
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -13,24 +13,24 @@
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.old
 
 ![PyPI](https://img.shields.io/pypi/v/django-walletpass.svg)
 ![t](https://img.shields.io/badge/status-beta-red.svg)
 
@@ -48,16 +48,16 @@
 - Server implementation for store, registration, update and logging
 - Push notifications (APNs) on pass update
 - Individual storage backend setting
 - Support for mime-type upload using django-storages S3
 
 ## Requirements
 
-- Django 2.*
-- Python >= 3.5
+- Django 2.*, 3.*, 4.*
+- Python >= 3.6
 - pyca/cryptography (for .pkpass SMIME sign)
 - djangorestframework >= 3.8
 
 ## Getting Started
 
 ### Install
 
@@ -65,147 +65,148 @@
 $ pip install django-walletpass
 ```
 
 ### Configure
 
 Add 'django_walletpass' to you installed apps in the settings.py file.
 
-Load the content of your cert.pem and key.pem in your settings.py file.
+Load the content of your cert.pem and key.pem in your settings.py file. This is required
+for signing the .pkpass file.
 
-```
 
+```python
 WALLETPASS = {
     'CERT_PATH': 'path/to/your/cert.pem',
     'KEY_PATH': 'path/to/your/key.pem',
     # (None if isn't protected)
     # MUST be in bytes-like
     'KEY_PASSWORD': b'1234',
 }
 ```
 
 Add extra needed conf to your settings.py file.
 
-```
+```python
 WALLETPASS = {
     'CERT_PATH': 'path/to/your/cert.pem',
     'KEY_PATH': 'path/to/your/key.pem',
     # (None if isn't protected)
     # MUST be in bytes-like
     'KEY_PASSWORD': b'1234',
 
     'PASS_TYPE_ID': 'pass.io.develat.devpubs.example',
     'TEAM_ID': '123456',
     'SERVICE_URL': 'https://example.com/passes/',
 }
 ```
 
-If you plan to use token JWT auth instead key/cert, use:
+Add token JWT config data to allow APNs push:
 
-```
+```python
 WALLETPASS = {
     'PUSH_AUTH_STRATEGY': 'token',
     'TOKEN_AUTH_KEY_PATH': 'path/to/your/key.p8',
     'TOKEN_AUTH_KEY_ID': 'key_id',
 
     'PASS_TYPE_ID': 'pass.io.develat.devpubs.example',
     'TEAM_ID': '123456',
     'SERVICE_URL': 'https://example.com/passes/',
 }
 ```
 
 
 You should also import the urls into your site urls.
-```
+```python
 urlpatterns = [
     url(r'^api/passes/', include('django_walletpass.urls')),
 ```
 
 django-walletpass signals certain events that might come handy in your
 application.
 
-```
-from django_walletpass.views import pass_registered, pass_unregistered
+```python
+from django_walletpass.classviews import PASS_REGISTERED, PASS_UNREGISTERED
 
-@receiver(pass_registered)
+@receiver(PASS_REGISTERED)
 def pass_registered(sender, **kwargs):
     pass
 
-@receiver(pass_unregistered)
+@receiver(PASS_UNREGISTERED)
 def pass_unregistered(sender, **kwargs):
     pass
 ```
 
 
 ### Configure storage and upload path (optional)
 
 Default: DEFAULT_FILE_STORAGE
 
-```
+```python
 WALLETPASS_CONF = {
     # Defaults to DEFAULT_FILE_STORAGE
     'STORAGE_CLASS': 'my.custom.storageclass,
     'UPLOAD_TO': 'passes'
 }
 ```
 
 ### Push notifications sandbox (optional)
 
 Default: False
 
-```
+```python
 WALLETPASS_CONF = {
     'PUSH_SANDBOX': False,
 }
 ```
 
 ### CA certificates path (optional)
 
-```
+```python
 WALLETPASS_CONF = {
     # Cert in pem format.
     'APPLE_WWDRCA_PEM_PATH': 'path/to/cert.pem',
 }
 ```
 
 ### Redirect to pass url (optional)
 Usefull if you are using `django-storages` and you want to serve your .pkpass
 files from `s3`.
 
 Default: False
 
-```
+```python
 WALLETPASS_CONF = {
     STORAGE_HTTP_REDIRECT: True,
 }
 ```
 
 
 ## Build and sign passes
 
 ### Init builder object:
 
 Init empty builder
 
-```
-from django_walletpass.models import  PassBuilder
+```python
+from django_walletpass.models import PassBuilder
 builder = PassBuilder()
 ```
 
 Init builder usign a directory as base
 
-```
-from django_walletpass.models import  PassBuilder
+```python
+from django_walletpass.models import PassBuilder
 builder = PassBuilder(directory='/path/to/your.pass/')
 ```
 
 If the base directory contains a `pass.json` it will be loaded, but remember
 that required attributes of `pass.json` will be overwritten during build process
 using this values:
 
-```
+```python
 {
     "passTypeIdentifier": WALLETPASS_CONF['PASS_TYPE_ID'],
     "serialNumber": secrets.token_urlsafe(20),
     "teamIdentifier": WALLETPASS_CONF['TEAM_ID'],
     "webServiceURL": WALLETPASS_CONF['SERVICE_URL'],
     "authenticationToken": crypto.gen_random_token(),
 }
@@ -215,107 +216,107 @@
 
 To handle `pass.json` data, there is a dict inside your builder instance, you
 can manage it like a normal python dictionary.
 
 
 Update some attrs:
 
-```
+```python
 builder.pass_data.update({
   "barcode": {
     "message": "123456789",
     "format": "PKBarcodeFormatPDF417",
     "messageEncoding": "iso-8859-1"
   },
   "organizationName": "Organic Produce",
   "description": "Organic Produce Loyalty Card",
 })
 ```
 
 Update one attr:
 
-```
+```python
 builder.pass_data['description'] = "Organic Produce Loyalty Card"
 ```
 
 ### Overwrite automatically generated required attribute values
 
-```
+```python
 builder.pass_data_required.update({
     "passTypeIdentifier": "customvalue",
     "serialNumber": "customvalue",
     "teamIdentifier": "customvalue",
     "webServiceURL": "customvalue",
     "authenticationToken": "customvalue",
 })
 ```
 
 you can overwrite individual attributes:
 
 
-```
+```python
 builder.pass_data_required.update({
     "serialNumber": "customvalue",
 })
 builder.pass_data_required['serialNumber] = 'cutomvalue'
 ```
 
 ### Add extra files
 
-```
+```python
 file_content = open('myfile', 'rb').read()
 builder.add_file('image.png', file_content)
 ```
 
 You can also add files to directories:
 
-```
+```python
 file_content = open('myfile', 'rb').read()
 builder.add_file('en.lproj/pass.strings', file_content)
 ```
 
 
 ### Build .pkpass
 
 Build the content of .pkpass
 
-```
+```python
 pkpass_content = builder.build()
 ```
 
 Write to file:
 
-```
+```python
 pkpass_file = open('mypass.pkpass', 'rb')
 pkpass_file.write(pkpass_content)
 ```
 
 Save to new record in DB:
 
-```
+```python
 pass_instance = builder.write_to_model()
 pass_instance.save()
 ```
 
 Save to existent record in DB:
 
-```
+```python
 builder.write_to_model(pass_instance)
 pass_instance.save()
 ```
 
 ### Load .pkpass from DB and update
 
-```
+```python
 builder = pass_instance.get_pass_builder()
 builder.pass_data.update({'field': 'value'})
 builder.build()
 builder.save_to_db(pass_instance)
 ```
 
 ### Run tests locally
 
 Checkout source and run from source root directory
 
-```
+```bash
 docker run -it --rm -v "$(pwd):/app" python:3.8 bash -c "cd /app; python setup.py install; ./example/manage.py test django_walletpass"
 ```
```

### Comparing `django-walletpass-2.0/README.md` & `django-walletpass-3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 - Server implementation for store, registration, update and logging
 - Push notifications (APNs) on pass update
 - Individual storage backend setting
 - Support for mime-type upload using django-storages S3
 
 ## Requirements
 
-- Django 2.*
-- Python >= 3.5
+- Django 2.*, 3.*, 4.*
+- Python >= 3.6
 - pyca/cryptography (for .pkpass SMIME sign)
 - djangorestframework >= 3.8
 
 ## Getting Started
 
 ### Install
 
@@ -32,147 +32,148 @@
 $ pip install django-walletpass
 ```
 
 ### Configure
 
 Add 'django_walletpass' to you installed apps in the settings.py file.
 
-Load the content of your cert.pem and key.pem in your settings.py file.
+Load the content of your cert.pem and key.pem in your settings.py file. This is required
+for signing the .pkpass file.
 
-```
 
+```python
 WALLETPASS = {
     'CERT_PATH': 'path/to/your/cert.pem',
     'KEY_PATH': 'path/to/your/key.pem',
     # (None if isn't protected)
     # MUST be in bytes-like
     'KEY_PASSWORD': b'1234',
 }
 ```
 
 Add extra needed conf to your settings.py file.
 
-```
+```python
 WALLETPASS = {
     'CERT_PATH': 'path/to/your/cert.pem',
     'KEY_PATH': 'path/to/your/key.pem',
     # (None if isn't protected)
     # MUST be in bytes-like
     'KEY_PASSWORD': b'1234',
 
     'PASS_TYPE_ID': 'pass.io.develat.devpubs.example',
     'TEAM_ID': '123456',
     'SERVICE_URL': 'https://example.com/passes/',
 }
 ```
 
-If you plan to use token JWT auth instead key/cert, use:
+Add token JWT config data to allow APNs push:
 
-```
+```python
 WALLETPASS = {
     'PUSH_AUTH_STRATEGY': 'token',
     'TOKEN_AUTH_KEY_PATH': 'path/to/your/key.p8',
     'TOKEN_AUTH_KEY_ID': 'key_id',
 
     'PASS_TYPE_ID': 'pass.io.develat.devpubs.example',
     'TEAM_ID': '123456',
     'SERVICE_URL': 'https://example.com/passes/',
 }
 ```
 
 
 You should also import the urls into your site urls.
-```
+```python
 urlpatterns = [
     url(r'^api/passes/', include('django_walletpass.urls')),
 ```
 
 django-walletpass signals certain events that might come handy in your
 application.
 
-```
-from django_walletpass.views import pass_registered, pass_unregistered
+```python
+from django_walletpass.classviews import PASS_REGISTERED, PASS_UNREGISTERED
 
-@receiver(pass_registered)
+@receiver(PASS_REGISTERED)
 def pass_registered(sender, **kwargs):
     pass
 
-@receiver(pass_unregistered)
+@receiver(PASS_UNREGISTERED)
 def pass_unregistered(sender, **kwargs):
     pass
 ```
 
 
 ### Configure storage and upload path (optional)
 
 Default: DEFAULT_FILE_STORAGE
 
-```
+```python
 WALLETPASS_CONF = {
     # Defaults to DEFAULT_FILE_STORAGE
     'STORAGE_CLASS': 'my.custom.storageclass,
     'UPLOAD_TO': 'passes'
 }
 ```
 
 ### Push notifications sandbox (optional)
 
 Default: False
 
-```
+```python
 WALLETPASS_CONF = {
     'PUSH_SANDBOX': False,
 }
 ```
 
 ### CA certificates path (optional)
 
-```
+```python
 WALLETPASS_CONF = {
     # Cert in pem format.
     'APPLE_WWDRCA_PEM_PATH': 'path/to/cert.pem',
 }
 ```
 
 ### Redirect to pass url (optional)
 Usefull if you are using `django-storages` and you want to serve your .pkpass
 files from `s3`.
 
 Default: False
 
-```
+```python
 WALLETPASS_CONF = {
     STORAGE_HTTP_REDIRECT: True,
 }
 ```
 
 
 ## Build and sign passes
 
 ### Init builder object:
 
 Init empty builder
 
-```
-from django_walletpass.models import  PassBuilder
+```python
+from django_walletpass.models import PassBuilder
 builder = PassBuilder()
 ```
 
 Init builder usign a directory as base
 
-```
-from django_walletpass.models import  PassBuilder
+```python
+from django_walletpass.models import PassBuilder
 builder = PassBuilder(directory='/path/to/your.pass/')
 ```
 
 If the base directory contains a `pass.json` it will be loaded, but remember
 that required attributes of `pass.json` will be overwritten during build process
 using this values:
 
-```
+```python
 {
     "passTypeIdentifier": WALLETPASS_CONF['PASS_TYPE_ID'],
     "serialNumber": secrets.token_urlsafe(20),
     "teamIdentifier": WALLETPASS_CONF['TEAM_ID'],
     "webServiceURL": WALLETPASS_CONF['SERVICE_URL'],
     "authenticationToken": crypto.gen_random_token(),
 }
@@ -182,107 +183,107 @@
 
 To handle `pass.json` data, there is a dict inside your builder instance, you
 can manage it like a normal python dictionary.
 
 
 Update some attrs:
 
-```
+```python
 builder.pass_data.update({
   "barcode": {
     "message": "123456789",
     "format": "PKBarcodeFormatPDF417",
     "messageEncoding": "iso-8859-1"
   },
   "organizationName": "Organic Produce",
   "description": "Organic Produce Loyalty Card",
 })
 ```
 
 Update one attr:
 
-```
+```python
 builder.pass_data['description'] = "Organic Produce Loyalty Card"
 ```
 
 ### Overwrite automatically generated required attribute values
 
-```
+```python
 builder.pass_data_required.update({
     "passTypeIdentifier": "customvalue",
     "serialNumber": "customvalue",
     "teamIdentifier": "customvalue",
     "webServiceURL": "customvalue",
     "authenticationToken": "customvalue",
 })
 ```
 
 you can overwrite individual attributes:
 
 
-```
+```python
 builder.pass_data_required.update({
     "serialNumber": "customvalue",
 })
 builder.pass_data_required['serialNumber] = 'cutomvalue'
 ```
 
 ### Add extra files
 
-```
+```python
 file_content = open('myfile', 'rb').read()
 builder.add_file('image.png', file_content)
 ```
 
 You can also add files to directories:
 
-```
+```python
 file_content = open('myfile', 'rb').read()
 builder.add_file('en.lproj/pass.strings', file_content)
 ```
 
 
 ### Build .pkpass
 
 Build the content of .pkpass
 
-```
+```python
 pkpass_content = builder.build()
 ```
 
 Write to file:
 
-```
+```python
 pkpass_file = open('mypass.pkpass', 'rb')
 pkpass_file.write(pkpass_content)
 ```
 
 Save to new record in DB:
 
-```
+```python
 pass_instance = builder.write_to_model()
 pass_instance.save()
 ```
 
 Save to existent record in DB:
 
-```
+```python
 builder.write_to_model(pass_instance)
 pass_instance.save()
 ```
 
 ### Load .pkpass from DB and update
 
-```
+```python
 builder = pass_instance.get_pass_builder()
 builder.pass_data.update({'field': 'value'})
 builder.build()
 builder.save_to_db(pass_instance)
 ```
 
 ### Run tests locally
 
 Checkout source and run from source root directory
 
-```
+```bash
 docker run -it --rm -v "$(pwd):/app" python:3.8 bash -c "cd /app; python setup.py install; ./example/manage.py test django_walletpass"
 ```
```

### Comparing `django-walletpass-2.0/django_walletpass/certs/AppleWWDRCA.cer` & `django-walletpass-3.0/django_walletpass/certs/AppleWWDRCA.cer`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/certs/AppleWWDRCA.pem` & `django-walletpass-3.0/django_walletpass/certs/AppleWWDRCA.pem`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/classviews.py` & `django-walletpass-3.0/django_walletpass/classviews.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import json
-from datetime import datetime
 from calendar import timegm
+
+from pytz.exceptions import NonExistentTimeError
+
+import django.dispatch
+from dateutil.parser import parse
+from django.db.models import Max
 from django.http import HttpResponse
-from django.utils.http import http_date
 from django.middleware.http import ConditionalGetMiddleware
-from django.db.models import Max
-import django.dispatch
 from django.shortcuts import get_object_or_404
-from rest_framework import viewsets, status
-from rest_framework.response import Response
+from django.utils.http import http_date
+from rest_framework import status, viewsets
 from rest_framework.permissions import AllowAny
-from django_walletpass.models import Pass, Registration, Log
+from rest_framework.response import Response
+from django_walletpass.models import Log, Pass, Registration
 from django_walletpass.settings import dwpconfig as WALLETPASS_CONF
 
+# legacy constant, remove when it can be assumed no timestamps of this format are out
+# there anymore
 FORMAT = '%Y-%m-%d %H:%M:%S'
 PASS_REGISTERED = django.dispatch.Signal()
 PASS_UNREGISTERED = django.dispatch.Signal()
 
 
 def get_pass(pass_type_id, serial_number):
     return get_object_or_404(Pass, pass_type_identifier=pass_type_id, serial_number=serial_number)
@@ -33,20 +38,27 @@
             registrations__device_library_identifier=device_library_id,
             pass_type_identifier=pass_type_id,
         )
         if passes.count() == 0:
             return Response({}, status=status.HTTP_400_BAD_REQUEST)
 
         if 'passesUpdatedSince' in request.GET:
-            passes = passes.filter(updated_at__gt=datetime.strptime(request.GET['passesUpdatedSince'], FORMAT))
+            try:
+                # must be able to read UTC isoformat with TZ and FORMAT datetime string
+                # as well
+                date = parse(request.GET['passesUpdatedSince'])
+                passes = passes.filter(updated_at__gt=date)
+            except NonExistentTimeError:
+                date = date.replace(hour=0, minute=0)
+                passes = passes.filter(updated_at__gt=date)
 
         if passes:
             last_updated = passes.aggregate(Max('updated_at'))['updated_at__max']
             serial_numbers = [p.serial_number for p in passes.filter(updated_at=last_updated).all()]
-            response_data = {'lastUpdated': last_updated.strftime(FORMAT), 'serialNumbers': serial_numbers}
+            response_data = {'lastUpdated': last_updated.isoformat(), 'serialNumbers': serial_numbers}
             return Response(response_data)
 
         return Response({}, status=status.HTTP_204_NO_CONTENT)
 
 
 # TODO: Refactor.
 # - Use a ModelViewSet
@@ -109,15 +121,19 @@
         if WALLETPASS_CONF['STORAGE_HTTP_REDIRECT']:
             return Response({}, status=status.HTTP_302_FOUND, headers={'Location': pass_.data.url})
 
         response = HttpResponse(pass_.data.read(), content_type='application/vnd.apple.pkpass')
         response['Content-Disposition'] = 'attachment; filename=pass.pkpass'
 
         response['Last-Modified'] = http_date(timegm(pass_.updated_at.utctimetuple()))
-        return ConditionalGetMiddleware(get_response=response)(request)
+
+        def _get_response(_request):
+            return response
+
+        return ConditionalGetMiddleware(get_response=_get_response)(request)
 
 
 # TODO: use ModelViewSet
 class LogViewSet(viewsets.ViewSet):
     """
     Logs messages from devices
     """
```

### Comparing `django-walletpass-2.0/django_walletpass/crypto.py` & `django-walletpass-3.0/django_walletpass/crypto.py`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/migrations/0001_initial.py` & `django-walletpass-3.0/django_walletpass/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/migrations/0005_auto_20190613_1433.py` & `django-walletpass-3.0/django_walletpass/migrations/0005_auto_20190613_1433.py`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/migrations/0006_auto_20190613_1607.py` & `django-walletpass-3.0/django_walletpass/migrations/0006_auto_20190613_1607.py`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/models.py` & `django-walletpass-3.0/django_walletpass/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,18 +224,21 @@
     authentication_token = models.CharField(max_length=150)
     data = models.FileField(
         upload_to=WALLETPASS_CONF['UPLOAD_TO'],
         storage=WalletPassStorage(),
     )
     updated_at = models.DateTimeField(auto_now=True)
 
+    def get_registrations(self):
+        return self.registrations.all()
+
     def push_notification(self):
         klass = import_string(WALLETPASS_CONF['WALLETPASS_PUSH_CLASS'])
         push_module = klass()
-        for registration in self.registrations.all():
+        for registration in self.get_registrations():
             push_module.push_notification_from_instance(registration)
 
     def new_pass_builder(self, directory=None):
         builder = PassBuilder(directory)
         builder.pass_data_required.update({
             "passTypeIdentifier": self.pass_type_identifier,
             "serialNumber": self.serial_number,
```

### Comparing `django-walletpass-2.0/django_walletpass/services.py` & `django-walletpass-3.0/django_walletpass/services.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,47 @@
+import asyncio
 import logging
 from ssl import SSLError
-from hyper.tls import init_context
-from hyper.http20.exceptions import StreamResetError
-from apns2.client import APNsClient
-from apns2.credentials import Credentials
-from apns2.credentials import TokenCredentials
-from apns2.payload import Payload
+
+from aioapns import APNs, NotificationRequest
+from aioapns.exceptions import ConnectionClosed
 from django_walletpass.models import Registration
 from django_walletpass.settings import dwpconfig as WALLETPASS_CONF
 
 logger = logging.getLogger('walletpass.services')
 
 
 class PushBackend:
-    def push_notification(self, credentials, push_sandbox, pass_type_id, push_token):
-        payload = Payload()
+    def __init__(self):
+        self.loop = asyncio.get_event_loop()
+
+    async def push_notification(self, client, token):
+
         try:
-            client = APNsClient(
-                credentials,
-                use_sandbox=push_sandbox,
-                use_alternative_port=False,
-            )
-            client.send_notification(
-                push_token,
-                payload,
-                pass_type_id,
-            )
+            request = NotificationRequest(device_token=token, message={"aps": {}},)
+            await client.send_notification(request)
+
         except SSLError as e:
             logger.error("django_walletpass SSLError: %s", e)
-        except StreamResetError as e:
+        except (ConnectionError, ConnectionClosed) as e:
             logger.error("django_walletpass StreamResetError. Bad cert or token? %s", e)
         # Errors should never pass silently.
         except Exception as e:  # pylint: disable=broad-except
             # Unless explicitly silenced.
             logger.error("django_walletpass uncaught error %s", e)
 
-    def get_credentials(self):
-        if WALLETPASS_CONF['PUSH_AUTH_STRATEGY'] == 'token':
-            return TokenCredentials(
-                auth_key_path=WALLETPASS_CONF['TOKEN_AUTH_KEY_PATH'],
-                auth_key_id=WALLETPASS_CONF['TOKEN_AUTH_KEY_ID'],
-                team_id=WALLETPASS_CONF['TEAM_ID'],
-            )
-
-        # legacy cert/key auth
-        context = init_context(
-            cert=(
-                WALLETPASS_CONF['CERT_PATH'],
-                WALLETPASS_CONF['KEY_PATH'],
-            ),
-            # cert_path=WALLETPASS_CONF['APPLE_WWDRCA_PEM_PATH'],
-            cert_password=WALLETPASS_CONF['KEY_PASSWORD'],
-        )
-
-        return Credentials(context)
-
     def push_notification_with_token(self, token):
-        self.push_notification(
-            self.get_credentials(),
-            push_sandbox=WALLETPASS_CONF['PUSH_SANDBOX'],
-            pass_type_id=WALLETPASS_CONF['PASS_TYPE_ID'],
-            push_token=token,
+        client = APNs(
+            key=WALLETPASS_CONF["TOKEN_AUTH_KEY_PATH"],
+            key_id=WALLETPASS_CONF["TOKEN_AUTH_KEY_ID"],
+            team_id=WALLETPASS_CONF["TEAM_ID"],
+            topic=WALLETPASS_CONF["PASS_TYPE_ID"],
+            use_sandbox=WALLETPASS_CONF["PUSH_SANDBOX"],
         )
+        return self.loop.run_until_complete(self.push_notification(client, token))
 
     def push_notification_from_instance(self, registration_instance):
-        self.push_notification_with_token(registration_instance.push_token)
+        return self.push_notification_with_token(registration_instance.push_token)
 
     def push_notification_from_pk(self, registration_pk):
         registration = Registration.objects.get(pk=registration_pk)
         return self.push_notification_from_instance(registration)
```

### Comparing `django-walletpass-2.0/django_walletpass/settings.py` & `django-walletpass-3.0/django_walletpass/settings.py`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass/tests/main.py` & `django-walletpass-3.0/django_walletpass/tests/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+from unittest import mock
+
+from dateutil.parser import parse
 from django.test import TestCase
+from django.utils import timezone
 from django_walletpass import crypto
-from django_walletpass.models import PassBuilder
+from django_walletpass.classviews import FORMAT
+from django_walletpass.models import Pass, PassBuilder, Registration
 from django_walletpass.settings import dwpconfig as WALLETPASS_CONF
 
 
+class ClassViewsTestCase(TestCase):
+
+    def test_format_parse(self):
+        """ ensure dateutil reads FORMAT properly """
+        now = timezone.now()
+        now_string = now.strftime(FORMAT)
+        self.assertEqual(parse(now_string), timezone.make_naive(now).replace(microsecond=0))
+
+
 class CryptoTestCase(TestCase):
     def test_smime_sign(self):
         crypto.pkcs7_sign(
             certcontent=WALLETPASS_CONF['CERT_CONTENT'],
             keycontent=WALLETPASS_CONF['KEY_CONTENT'],
             wwdr_certificate=WALLETPASS_CONF['WWDRCA_PEM_CONTENT'],
             data=b'data to be signed',
@@ -52,7 +66,20 @@
         builder3.build()
 
         self.assertEqual(builder2.manifest_dict, builder3.manifest_dict)
         self.assertEqual(builder2.pass_data, builder3.pass_data)
 
         self.assertNotEqual(builder.manifest_dict, builder3.manifest_dict)
         self.assertNotEqual(builder.pass_data, builder3.pass_data)
+
+
+class ModelTestCase(TestCase):
+    @mock.patch("django_walletpass.models.Pass.get_registrations")
+    @mock.patch("django_walletpass.services.APNs.send_notification")
+    def test_push_notification(self, send_notification_mock, get_registrations_mock):
+        get_registrations_mock.return_value = [Registration()]
+        pass_ = Pass(pk=1)
+        with mock.patch("django_walletpass.services.APNs.__init__", return_value=None):
+            pass_.push_notification()
+            send_notification_mock.assert_called_with(mock.ANY)
+            request = send_notification_mock.call_args_list[0][0][0]
+            self.assertEqual(request.message, {"aps": {}})
```

### Comparing `django-walletpass-2.0/django_walletpass/urls.py` & `django-walletpass-3.0/django_walletpass/urls.py`

 * *Files identical despite different names*

### Comparing `django-walletpass-2.0/django_walletpass.egg-info/PKG-INFO` & `django-walletpass-3.0/django_walletpass.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-walletpass
-Version: 2.0
+Version: 3.0
 Summary: Django .pkpass builder, server and push notifications
 Home-page: http://github.com/develatio/django-walletpass/
 Author: Develatio Technologies S.L.
 Author-email: contacto@develat.io
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -13,24 +13,24 @@
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.old
 
 ![PyPI](https://img.shields.io/pypi/v/django-walletpass.svg)
 ![t](https://img.shields.io/badge/status-beta-red.svg)
 
@@ -48,16 +48,16 @@
 - Server implementation for store, registration, update and logging
 - Push notifications (APNs) on pass update
 - Individual storage backend setting
 - Support for mime-type upload using django-storages S3
 
 ## Requirements
 
-- Django 2.*
-- Python >= 3.5
+- Django 2.*, 3.*, 4.*
+- Python >= 3.6
 - pyca/cryptography (for .pkpass SMIME sign)
 - djangorestframework >= 3.8
 
 ## Getting Started
 
 ### Install
 
@@ -65,147 +65,148 @@
 $ pip install django-walletpass
 ```
 
 ### Configure
 
 Add 'django_walletpass' to you installed apps in the settings.py file.
 
-Load the content of your cert.pem and key.pem in your settings.py file.
+Load the content of your cert.pem and key.pem in your settings.py file. This is required
+for signing the .pkpass file.
 
-```
 
+```python
 WALLETPASS = {
     'CERT_PATH': 'path/to/your/cert.pem',
     'KEY_PATH': 'path/to/your/key.pem',
     # (None if isn't protected)
     # MUST be in bytes-like
     'KEY_PASSWORD': b'1234',
 }
 ```
 
 Add extra needed conf to your settings.py file.
 
-```
+```python
 WALLETPASS = {
     'CERT_PATH': 'path/to/your/cert.pem',
     'KEY_PATH': 'path/to/your/key.pem',
     # (None if isn't protected)
     # MUST be in bytes-like
     'KEY_PASSWORD': b'1234',
 
     'PASS_TYPE_ID': 'pass.io.develat.devpubs.example',
     'TEAM_ID': '123456',
     'SERVICE_URL': 'https://example.com/passes/',
 }
 ```
 
-If you plan to use token JWT auth instead key/cert, use:
+Add token JWT config data to allow APNs push:
 
-```
+```python
 WALLETPASS = {
     'PUSH_AUTH_STRATEGY': 'token',
     'TOKEN_AUTH_KEY_PATH': 'path/to/your/key.p8',
     'TOKEN_AUTH_KEY_ID': 'key_id',
 
     'PASS_TYPE_ID': 'pass.io.develat.devpubs.example',
     'TEAM_ID': '123456',
     'SERVICE_URL': 'https://example.com/passes/',
 }
 ```
 
 
 You should also import the urls into your site urls.
-```
+```python
 urlpatterns = [
     url(r'^api/passes/', include('django_walletpass.urls')),
 ```
 
 django-walletpass signals certain events that might come handy in your
 application.
 
-```
-from django_walletpass.views import pass_registered, pass_unregistered
+```python
+from django_walletpass.classviews import PASS_REGISTERED, PASS_UNREGISTERED
 
-@receiver(pass_registered)
+@receiver(PASS_REGISTERED)
 def pass_registered(sender, **kwargs):
     pass
 
-@receiver(pass_unregistered)
+@receiver(PASS_UNREGISTERED)
 def pass_unregistered(sender, **kwargs):
     pass
 ```
 
 
 ### Configure storage and upload path (optional)
 
 Default: DEFAULT_FILE_STORAGE
 
-```
+```python
 WALLETPASS_CONF = {
     # Defaults to DEFAULT_FILE_STORAGE
     'STORAGE_CLASS': 'my.custom.storageclass,
     'UPLOAD_TO': 'passes'
 }
 ```
 
 ### Push notifications sandbox (optional)
 
 Default: False
 
-```
+```python
 WALLETPASS_CONF = {
     'PUSH_SANDBOX': False,
 }
 ```
 
 ### CA certificates path (optional)
 
-```
+```python
 WALLETPASS_CONF = {
     # Cert in pem format.
     'APPLE_WWDRCA_PEM_PATH': 'path/to/cert.pem',
 }
 ```
 
 ### Redirect to pass url (optional)
 Usefull if you are using `django-storages` and you want to serve your .pkpass
 files from `s3`.
 
 Default: False
 
-```
+```python
 WALLETPASS_CONF = {
     STORAGE_HTTP_REDIRECT: True,
 }
 ```
 
 
 ## Build and sign passes
 
 ### Init builder object:
 
 Init empty builder
 
-```
-from django_walletpass.models import  PassBuilder
+```python
+from django_walletpass.models import PassBuilder
 builder = PassBuilder()
 ```
 
 Init builder usign a directory as base
 
-```
-from django_walletpass.models import  PassBuilder
+```python
+from django_walletpass.models import PassBuilder
 builder = PassBuilder(directory='/path/to/your.pass/')
 ```
 
 If the base directory contains a `pass.json` it will be loaded, but remember
 that required attributes of `pass.json` will be overwritten during build process
 using this values:
 
-```
+```python
 {
     "passTypeIdentifier": WALLETPASS_CONF['PASS_TYPE_ID'],
     "serialNumber": secrets.token_urlsafe(20),
     "teamIdentifier": WALLETPASS_CONF['TEAM_ID'],
     "webServiceURL": WALLETPASS_CONF['SERVICE_URL'],
     "authenticationToken": crypto.gen_random_token(),
 }
@@ -215,107 +216,107 @@
 
 To handle `pass.json` data, there is a dict inside your builder instance, you
 can manage it like a normal python dictionary.
 
 
 Update some attrs:
 
-```
+```python
 builder.pass_data.update({
   "barcode": {
     "message": "123456789",
     "format": "PKBarcodeFormatPDF417",
     "messageEncoding": "iso-8859-1"
   },
   "organizationName": "Organic Produce",
   "description": "Organic Produce Loyalty Card",
 })
 ```
 
 Update one attr:
 
-```
+```python
 builder.pass_data['description'] = "Organic Produce Loyalty Card"
 ```
 
 ### Overwrite automatically generated required attribute values
 
-```
+```python
 builder.pass_data_required.update({
     "passTypeIdentifier": "customvalue",
     "serialNumber": "customvalue",
     "teamIdentifier": "customvalue",
     "webServiceURL": "customvalue",
     "authenticationToken": "customvalue",
 })
 ```
 
 you can overwrite individual attributes:
 
 
-```
+```python
 builder.pass_data_required.update({
     "serialNumber": "customvalue",
 })
 builder.pass_data_required['serialNumber] = 'cutomvalue'
 ```
 
 ### Add extra files
 
-```
+```python
 file_content = open('myfile', 'rb').read()
 builder.add_file('image.png', file_content)
 ```
 
 You can also add files to directories:
 
-```
+```python
 file_content = open('myfile', 'rb').read()
 builder.add_file('en.lproj/pass.strings', file_content)
 ```
 
 
 ### Build .pkpass
 
 Build the content of .pkpass
 
-```
+```python
 pkpass_content = builder.build()
 ```
 
 Write to file:
 
-```
+```python
 pkpass_file = open('mypass.pkpass', 'rb')
 pkpass_file.write(pkpass_content)
 ```
 
 Save to new record in DB:
 
-```
+```python
 pass_instance = builder.write_to_model()
 pass_instance.save()
 ```
 
 Save to existent record in DB:
 
-```
+```python
 builder.write_to_model(pass_instance)
 pass_instance.save()
 ```
 
 ### Load .pkpass from DB and update
 
-```
+```python
 builder = pass_instance.get_pass_builder()
 builder.pass_data.update({'field': 'value'})
 builder.build()
 builder.save_to_db(pass_instance)
 ```
 
 ### Run tests locally
 
 Checkout source and run from source root directory
 
-```
+```bash
 docker run -it --rm -v "$(pwd):/app" python:3.8 bash -c "cd /app; python setup.py install; ./example/manage.py test django_walletpass"
 ```
```

### Comparing `django-walletpass-2.0/django_walletpass.egg-info/SOURCES.txt` & `django-walletpass-3.0/django_walletpass.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 django_walletpass/migrations/0001_initial.py
 django_walletpass/migrations/0002_auto_20190429_1819.py
 django_walletpass/migrations/0003_auto_20190610_1434.py
 django_walletpass/migrations/0004_auto_20190611_1306.py
 django_walletpass/migrations/0005_auto_20190613_1433.py
 django_walletpass/migrations/0006_auto_20190613_1607.py
 django_walletpass/migrations/0007_auto_20190613_1807.py
+django_walletpass/migrations/0008_alter_pass_data.py
 django_walletpass/migrations/__init__.py
 django_walletpass/tests/__init__.py
 django_walletpass/tests/main.py
```

### Comparing `django-walletpass-2.0/setup.py` & `django-walletpass-3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'README.md'), 'r', encoding='utf-8') as ffile:
     README = ffile.read()
 
 setup(
     name='django-walletpass',
-    python_requires='>=3.5.0',
-    version='2.0',
+    python_requires='>=3.6.0',
+    version='3.0',
     author='Develatio Technologies S.L.',
     author_email='contacto@develat.io',
     packages=find_packages(),
     include_package_data=True,
     url='http://github.com/develatio/django-walletpass/',
     license='BSD',
     install_requires=[
         'Django>=2.0',
         'cryptography>=2.4.2',
-        'apns2>=0.7.1',
+        'aioapns~=2.2',
         'pyopenssl',
         'djangorestframework>=3.8',
+        'python-dateutil'
     ],
     description='Django .pkpass builder, server and push notifications',
     long_description=README,
     long_description_content_type='text/markdown',
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
@@ -35,17 +36,17 @@
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Internationalization',
         'Topic :: Software Development :: Localization',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
     ],
```

