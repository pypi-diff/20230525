# Comparing `tmp/django-vite-2.0.2.tar.gz` & `tmp/django-vite-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vite-2.0.2.tar", last modified: Tue Mar 15 20:07:07 2022, max compression
+gzip compressed data, was "django-vite-2.1.0.tar", last modified: Thu May 25 13:33:07 2023, max compression
```

## Comparing `django-vite-2.0.2.tar` & `django-vite-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:07:07.828186 django-vite-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-03-15 20:06:56.000000 django-vite-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-15 20:06:56.000000 django-vite-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8868 2022-03-15 20:07:07.828186 django-vite-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8549 2022-03-15 20:06:56.000000 django-vite-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:07:07.824186 django-vite-2.0.2/django_vite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:06:56.000000 django-vite-2.0.2/django_vite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:07:07.828186 django-vite-2.0.2/django_vite/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:06:56.000000 django-vite-2.0.2/django_vite/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15305 2022-03-15 20:06:56.000000 django-vite-2.0.2/django_vite/templatetags/django_vite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:07:07.824186 django-vite-2.0.2/django_vite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8868 2022-03-15 20:07:07.000000 django-vite-2.0.2/django_vite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-03-15 20:07:07.000000 django-vite-2.0.2/django_vite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 20:07:07.000000 django-vite-2.0.2/django_vite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-15 20:07:07.000000 django-vite-2.0.2/django_vite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-15 20:07:07.000000 django-vite-2.0.2/django_vite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-03-15 20:06:56.000000 django-vite-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 20:07:07.828186 django-vite-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-03-15 20:06:56.000000 django-vite-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-25 13:32:52.000000 django-vite-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 13:32:52.000000 django-vite-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-25 13:33:07.659424 django-vite-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-05-25 13:32:52.000000 django-vite-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/django_vite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:52.000000 django-vite-2.1.0/django_vite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/django_vite/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:52.000000 django-vite-2.1.0/django_vite/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-25 13:32:52.000000 django-vite-2.1.0/django_vite/templatetags/django_vite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:33:07.659424 django-vite-2.1.0/django_vite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 13:33:07.000000 django-vite-2.1.0/django_vite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 13:32:52.000000 django-vite-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:33:07.659424 django-vite-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 13:32:52.000000 django-vite-2.1.0/setup.py
```

### Comparing `django-vite-2.0.2/LICENSE` & `django-vite-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vite-2.0.2/PKG-INFO` & `django-vite-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 2.0.2
+Version: 2.1.0
 Summary: Integration of ViteJS in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
-License: UNKNOWN
-Platform: UNKNOWN
+License: Apache License, Version 2.0
+Classifier: License :: OSI Approved :: Apache Software License
 Requires: Django (>=1.11)
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Django Vite
 
+[![PyPI version](https://badge.fury.io/py/django-vite.svg)](https://badge.fury.io/py/django-vite)
+
 Integration of [ViteJS](https://vitejs.dev/) in a Django project.
 
 ## Installation
 
 ### Django
 
 ```
@@ -109,15 +111,15 @@
 {% vite_hmr_client %}
 ```
 
 - This will add a `<script>` tag to include the ViteJS HMR client.
 - This tag will include this script only if `DJANGO_VITE_DEV_MODE` is true,
   otherwise this will do nothing.
 
-Then add this tag to load your scripts :
+Then add this tag (in your `<head>` element too) to load your scripts :
 
 ```
 {% vite_asset '<path to your asset>' %}
 ```
 
 This will add a `<script>` tag including your JS/TS script :
 
@@ -142,14 +144,19 @@
 {% vite_asset_url '<path to your asset>' %}
 ```
 
 This will generate only the URL to an asset with no tag surrounding it.
 **Warning, this does not generate URLs for dependant assets of this one
 like the previous tag.**
 
+```
+{% vite_react_refresh %}
+```
+If you're using React, this will generate the Javascript needed to support React HMR.
+
 ### Custom attributes
 
 By default, all scripts tags are generated with a `type="module"` and `crossorigin=""` attributes just like ViteJS do by default if you are building a single-page app.
 You can override this behavior by adding or overriding this attributes like so :
 
 ```
 {% vite_asset '<path to your asset>' foo="bar" hello="world" %}
@@ -265,9 +272,7 @@
 
 If you are struggling on how to setup a project using Django / ViteJS and Django Vite,
 I've made an [example project here](https://github.com/MrBin99/django-vite-example).
 
 ## Thanks
 
 Thanks to [Evan You](https://github.com/yyx990803) for the ViteJS library.
-
-
```

### Comparing `django-vite-2.0.2/README.md` & `django-vite-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Django Vite
 
+[![PyPI version](https://badge.fury.io/py/django-vite.svg)](https://badge.fury.io/py/django-vite)
+
 Integration of [ViteJS](https://vitejs.dev/) in a Django project.
 
 ## Installation
 
 ### Django
 
 ```
@@ -96,15 +98,15 @@
 {% vite_hmr_client %}
 ```
 
 - This will add a `<script>` tag to include the ViteJS HMR client.
 - This tag will include this script only if `DJANGO_VITE_DEV_MODE` is true,
   otherwise this will do nothing.
 
-Then add this tag to load your scripts :
+Then add this tag (in your `<head>` element too) to load your scripts :
 
 ```
 {% vite_asset '<path to your asset>' %}
 ```
 
 This will add a `<script>` tag including your JS/TS script :
 
@@ -129,14 +131,19 @@
 {% vite_asset_url '<path to your asset>' %}
 ```
 
 This will generate only the URL to an asset with no tag surrounding it.
 **Warning, this does not generate URLs for dependant assets of this one
 like the previous tag.**
 
+```
+{% vite_react_refresh %}
+```
+If you're using React, this will generate the Javascript needed to support React HMR.
+
 ### Custom attributes
 
 By default, all scripts tags are generated with a `type="module"` and `crossorigin=""` attributes just like ViteJS do by default if you are building a single-page app.
 You can override this behavior by adding or overriding this attributes like so :
 
 ```
 {% vite_asset '<path to your asset>' foo="bar" hello="world" %}
```

### Comparing `django-vite-2.0.2/django_vite/templatetags/django_vite.py` & `django-vite-2.1.0/django_vite/templatetags/django_vite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 from typing import Dict, List
 from urllib.parse import urljoin
 
 from django import template
+from django.apps import apps
 from django.conf import settings
 from django.utils.safestring import mark_safe
 
 register = template.Library()
 
 
 # If using in development or production mode.
@@ -29,14 +30,18 @@
 )
 
 # Default Vite server path to HMR script.
 DJANGO_VITE_WS_CLIENT_URL = getattr(
     settings, "DJANGO_VITE_WS_CLIENT_URL", "@vite/client"
 )
 
+DJANGO_VITE_REACT_REFRESH_URL = getattr(
+    settings, "DJANGO_VITE_REACT_REFRESH_URL", "@react-refresh"
+)
+
 # Location of Vite compiled assets (only used in Vite production mode).
 # Must be included in your "STATICFILES_DIRS".
 # In Django production mode this folder need to be collected as static
 # files using "python manage.py collectstatic".
 DJANGO_VITE_ASSETS_PATH = Path(getattr(settings, "DJANGO_VITE_ASSETS_PATH"))
 
 # Prefix for STATIC_URL
@@ -111,15 +116,15 @@
             str -- The <script> tag and all <link> tags to import
                 this asset in your page.
         """
 
         if DJANGO_VITE_DEV_MODE:
             return DjangoViteAssetLoader._generate_script_tag(
                 DjangoViteAssetLoader._generate_vite_server_url(path),
-                {"type": "module"},
+                {"type": "module", **kwargs},
             )
 
         if not self._manifest or path not in self._manifest:
             raise RuntimeError(
                 f"Cannot find {path} in Vite manifest "
                 f"at {DJANGO_VITE_MANIFEST_PATH}"
             )
@@ -130,15 +135,17 @@
 
         # Add dependent CSS
         tags.extend(self._generate_css_files_of_asset(path, []))
 
         # Add the script by itself
         tags.append(
             DjangoViteAssetLoader._generate_script_tag(
-                urljoin(DJANGO_VITE_STATIC_URL, manifest_entry["file"]),
+                DjangoViteAssetLoader._generate_production_server_url(
+                    manifest_entry["file"]
+                ),
                 attrs=scripts_attrs,
             )
         )
 
         return "\n".join(tags)
 
     def _generate_css_files_of_asset(
@@ -165,19 +172,22 @@
                         import_path, already_processed
                     )
                 )
 
         if "css" in manifest_entry:
             for css_path in manifest_entry["css"]:
                 if css_path not in already_processed:
-                    tags.append(
-                        DjangoViteAssetLoader._generate_stylesheet_tag(
-                            urljoin(DJANGO_VITE_STATIC_URL, css_path)
+                    url = (
+                        DjangoViteAssetLoader._generate_production_server_url(
+                            css_path
                         )
                     )
+                    tags.append(
+                        DjangoViteAssetLoader._generate_stylesheet_tag(url)
+                    )
 
                 already_processed.append(css_path)
 
         return tags
 
     def generate_vite_asset_url(self, path: str) -> str:
         """
@@ -200,15 +210,17 @@
 
         if not self._manifest or path not in self._manifest:
             raise RuntimeError(
                 f"Cannot find {path} in Vite manifest "
                 f"at {DJANGO_VITE_MANIFEST_PATH}"
             )
 
-        return urljoin(DJANGO_VITE_STATIC_URL, self._manifest[path]["file"])
+        return DjangoViteAssetLoader._generate_production_server_url(
+            self._manifest[path]["file"]
+        )
 
     def generate_vite_legacy_polyfills(
         self,
         **kwargs: Dict[str, str],
     ) -> str:
         """
         Generates a <script> tag to the polyfills
@@ -232,15 +244,17 @@
             return ""
 
         scripts_attrs = {"nomodule": "", "crossorigin": "", **kwargs}
 
         for path, content in self._manifest.items():
             if DJANGO_VITE_LEGACY_POLYFILLS_MOTIF in path:
                 return DjangoViteAssetLoader._generate_script_tag(
-                    urljoin(DJANGO_VITE_STATIC_URL, content["file"]),
+                    DjangoViteAssetLoader._generate_production_server_url(
+                        content["file"]
+                    ),
                     attrs=scripts_attrs,
                 )
 
         raise RuntimeError(
             f"Vite legacy polyfills not found in manifest "
             f"at {DJANGO_VITE_MANIFEST_PATH}"
         )
@@ -280,15 +294,17 @@
                 f"at {DJANGO_VITE_MANIFEST_PATH}"
             )
 
         manifest_entry = self._manifest[path]
         scripts_attrs = {"nomodule": "", "crossorigin": "", **kwargs}
 
         return DjangoViteAssetLoader._generate_script_tag(
-            urljoin(DJANGO_VITE_STATIC_URL, manifest_entry["file"]),
+            DjangoViteAssetLoader._generate_production_server_url(
+                manifest_entry["file"]
+            ),
             attrs=scripts_attrs,
         )
 
     def _parse_manifest(self) -> None:
         """
         Read and parse the Vite manifest file.
 
@@ -325,30 +341,34 @@
             # Manifest is only used in production.
             if not DJANGO_VITE_DEV_MODE:
                 cls._instance._parse_manifest()
 
         return cls._instance
 
     @classmethod
-    def generate_vite_ws_client(cls) -> str:
+    def generate_vite_ws_client(cls, **kwargs: Dict[str, str]) -> str:
         """
         Generates the script tag for the Vite WS client for HMR.
         Only used in development, in production this method returns
         an empty string.
 
         Returns:
             str -- The script tag or an empty string.
+
+        Keyword Arguments:
+            **kwargs {Dict[str, str]} -- Adds new attributes to generated
+                script tags.
         """
 
         if not DJANGO_VITE_DEV_MODE:
             return ""
 
         return cls._generate_script_tag(
             cls._generate_vite_server_url(DJANGO_VITE_WS_CLIENT_URL),
-            {"type": "module"},
+            {"type": "module", **kwargs},
         )
 
     @staticmethod
     def _generate_script_tag(src: str, attrs: Dict[str, str]) -> str:
         """
         Generates an HTML script tag.
 
@@ -397,28 +417,80 @@
 
         return urljoin(
             f"{DJANGO_VITE_DEV_SERVER_PROTOCOL}://"
             f"{DJANGO_VITE_DEV_SERVER_HOST}:{DJANGO_VITE_DEV_SERVER_PORT}",
             urljoin(DJANGO_VITE_STATIC_URL, path),
         )
 
+    @classmethod
+    def generate_vite_react_refresh_url(cls) -> str:
+        """
+        Generates the script for the Vite React Refresh for HMR.
+        Only used in development, in production this method returns
+        an empty string.
+
+        Returns:
+            str -- The script or an empty string.
+        """
+
+        if not DJANGO_VITE_DEV_MODE:
+            return ""
+
+        return f"""<script type="module">
+            import RefreshRuntime from \
+            '{cls._generate_vite_server_url(DJANGO_VITE_REACT_REFRESH_URL)}'
+            RefreshRuntime.injectIntoGlobalHook(window)
+            window.$RefreshReg$ = () => {{}}
+            window.$RefreshSig$ = () => (type) => type
+            window.__vite_plugin_react_preamble_installed__ = true
+        </script>"""
+
+    @staticmethod
+    def _generate_production_server_url(path: str) -> str:
+        """
+        Generates an URL to an asset served during production.
+
+        Keyword Arguments:
+            path {str} -- Path to the asset.
+
+        Returns:
+            str -- Full URL to the asset.
+        """
+
+        if apps.is_installed("django.contrib.staticfiles"):
+            from django.contrib.staticfiles.storage import staticfiles_storage
+
+            return staticfiles_storage.url(
+                urljoin(DJANGO_VITE_STATIC_URL_PREFIX, path)
+            )
+        else:
+            return urljoin(DJANGO_VITE_STATIC_URL_PREFIX, path)
+
+
+# Make Loader instance at startup to prevent threading problems
+DjangoViteAssetLoader.instance()
+
 
 @register.simple_tag
 @mark_safe
-def vite_hmr_client() -> str:
+def vite_hmr_client(**kwargs: Dict[str, str]) -> str:
     """
     Generates the script tag for the Vite WS client for HMR.
     Only used in development, in production this method returns
     an empty string.
 
     Returns:
         str -- The script tag or an empty string.
+
+    Keyword Arguments:
+        **kwargs {Dict[str, str]} -- Adds new attributes to generated
+            script tags.
     """
 
-    return DjangoViteAssetLoader.generate_vite_ws_client()
+    return DjangoViteAssetLoader.generate_vite_ws_client(**kwargs)
 
 
 @register.simple_tag
 @mark_safe
 def vite_asset(
     path: str,
     **kwargs: Dict[str, str],
@@ -529,7 +601,21 @@
     """
 
     assert path is not None
 
     return DjangoViteAssetLoader.instance().generate_vite_legacy_asset(
         path, **kwargs
     )
+
+
+@register.simple_tag
+@mark_safe
+def vite_react_refresh() -> str:
+    """
+    Generates the script for the Vite React Refresh for HMR.
+    Only used in development, in production this method returns
+    an empty string.
+
+    Returns:
+        str -- The script or an empty string.
+    """
+    return DjangoViteAssetLoader.generate_vite_react_refresh_url()
```

### Comparing `django-vite-2.0.2/django_vite.egg-info/PKG-INFO` & `django-vite-2.1.0/django_vite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 2.0.2
+Version: 2.1.0
 Summary: Integration of ViteJS in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
-License: UNKNOWN
-Platform: UNKNOWN
+License: Apache License, Version 2.0
+Classifier: License :: OSI Approved :: Apache Software License
 Requires: Django (>=1.11)
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Django Vite
 
+[![PyPI version](https://badge.fury.io/py/django-vite.svg)](https://badge.fury.io/py/django-vite)
+
 Integration of [ViteJS](https://vitejs.dev/) in a Django project.
 
 ## Installation
 
 ### Django
 
 ```
@@ -109,15 +111,15 @@
 {% vite_hmr_client %}
 ```
 
 - This will add a `<script>` tag to include the ViteJS HMR client.
 - This tag will include this script only if `DJANGO_VITE_DEV_MODE` is true,
   otherwise this will do nothing.
 
-Then add this tag to load your scripts :
+Then add this tag (in your `<head>` element too) to load your scripts :
 
 ```
 {% vite_asset '<path to your asset>' %}
 ```
 
 This will add a `<script>` tag including your JS/TS script :
 
@@ -142,14 +144,19 @@
 {% vite_asset_url '<path to your asset>' %}
 ```
 
 This will generate only the URL to an asset with no tag surrounding it.
 **Warning, this does not generate URLs for dependant assets of this one
 like the previous tag.**
 
+```
+{% vite_react_refresh %}
+```
+If you're using React, this will generate the Javascript needed to support React HMR.
+
 ### Custom attributes
 
 By default, all scripts tags are generated with a `type="module"` and `crossorigin=""` attributes just like ViteJS do by default if you are building a single-page app.
 You can override this behavior by adding or overriding this attributes like so :
 
 ```
 {% vite_asset '<path to your asset>' foo="bar" hello="world" %}
@@ -265,9 +272,7 @@
 
 If you are struggling on how to setup a project using Django / ViteJS and Django Vite,
 I've made an [example project here](https://github.com/MrBin99/django-vite-example).
 
 ## Thanks
 
 Thanks to [Evan You](https://github.com/yyx990803) for the ViteJS library.
-
-
```

