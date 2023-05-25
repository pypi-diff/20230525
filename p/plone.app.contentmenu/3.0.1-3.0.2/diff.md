# Comparing `tmp/plone.app.contentmenu-3.0.1.tar.gz` & `tmp/plone.app.contentmenu-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contentmenu-3.0.1.tar", last modified: Thu Apr  6 10:29:50 2023, max compression
+gzip compressed data, was "plone.app.contentmenu-3.0.2.tar", last modified: Thu May 25 13:37:28 2023, max compression
```

## Comparing `plone.app.contentmenu-3.0.1.tar` & `plone.app.contentmenu-3.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.136319 plone.app.contentmenu-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      270 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      128 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)    13391 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      144 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    18184 2023-04-06 10:29:50.136464 plone.app.contentmenu-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3834 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.129991 plone.app.contentmenu-3.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.130287 plone.app.contentmenu-3.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.132962 plone.app.contentmenu-3.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.135454 plone.app.contentmenu-3.0.1/plone/app/contentmenu/
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4139 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4973 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/contentmenu.pt
--rw-r--r--   0 maurits    (501) staff       (20)      947 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/displayviewsmenu.py
--rw-r--r--   0 maurits    (501) staff       (20)     3846 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    38182 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/menu.py
--rw-r--r--   0 maurits    (501) staff       (20)     1299 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.136012 plone.app.contentmenu-3.0.1/plone/app/contentmenu/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    35089 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/tests/test_menu.py
--rw-r--r--   0 maurits    (501) staff       (20)     1130 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/plone/app/contentmenu/view.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:29:50.132658 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18184 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      909 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-06 10:29:50.000000 plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-06 10:29:50.137006 plone.app.contentmenu-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1780 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-04-06 10:29:49.000000 plone.app.contentmenu-3.0.1/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.978901 plone.app.contentmenu-3.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      270 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      128 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      975 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)    13590 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      144 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    18383 2023-05-25 13:37:28.979069 plone.app.contentmenu-3.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3834 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.972141 plone.app.contentmenu-3.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.972459 plone.app.contentmenu-3.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.975349 plone.app.contentmenu-3.0.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.978046 plone.app.contentmenu-3.0.2/plone/app/contentmenu/
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4139 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5580 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/contentmenu.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      947 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/displayviewsmenu.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3846 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    38209 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1299 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.978586 plone.app.contentmenu-3.0.2/plone/app/contentmenu/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35089 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/tests/test_menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1130 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone/app/contentmenu/view.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:37:28.975027 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    18383 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      909 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-25 13:37:28.979692 plone.app.contentmenu-3.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1780 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-05-25 13:37:28.000000 plone.app.contentmenu-3.0.2/tox.ini
```

### Comparing `plone.app.contentmenu-3.0.1/.editorconfig` & `plone.app.contentmenu-3.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/.pre-commit-config.yaml` & `plone.app.contentmenu-3.0.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # https://github.com/plone/meta/tree/master/config/default
 ci:
     autofix_prs: false
     autoupdate_schedule: monthly
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
     -   id: isort
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/collective/zpretty
-    rev: 3.0.3
+    rev: 3.1.0a2
     hooks:
     -   id: zpretty
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/codespell-project/codespell
```

### Comparing `plone.app.contentmenu-3.0.1/CHANGES.rst` & `plone.app.contentmenu-3.0.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-05-25)
+------------------
+
+Bug fixes:
+
+
+- Add description to actions' menu items
+  [kshitiz305] (#24)
+- Show workflow state title also when the toolbar is at the top.
+  [maurits] (#49)
+
+
 3.0.1 (2023-04-06)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentmenu-3.0.1/PKG-INFO` & `plone.app.contentmenu-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentmenu
-Version: 3.0.1
+Version: 3.0.2
 Summary: Plone's content menu implementation
 Home-page: https://pypi.org/project/plone.app.contentmenu
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone contentmenu menu
 Classifier: Development Status :: 5 - Production/Stable
@@ -152,14 +152,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-05-25)
+------------------
+
+Bug fixes:
+
+
+- Add description to actions' menu items
+  [kshitiz305] (#24)
+- Show workflow state title also when the toolbar is at the top.
+  [maurits] (#49)
+
+
 3.0.1 (2023-04-06)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentmenu-3.0.1/README.rst` & `plone.app.contentmenu-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/docs/LICENSE.GPL` & `plone.app.contentmenu-3.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/docs/LICENSE.txt` & `plone.app.contentmenu-3.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/configure.zcml` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/contentmenu.pt` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/contentmenu.pt`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,29 @@
 
         </a>
 
         <ul class="dropdown-menu"
             tal:condition="submenu | nothing"
         >
           <li>
-            <h6 class="dropdown-header">${menuItem/title}</h6>
+            <h6 class="dropdown-header">
+              ${menuItem/title}
+              <tal:show-state-if-top tal:condition="python:toolbar_pos == 'top'">
+                <span class="${state_class}"
+                      tal:define="
+                        state_class menuItem/extra/class | nothing;
+                        state_class python:'label-%s' % state_class if state_class else '';
+                        state_title menuItem/extra/stateTitle|nothing;
+                      "
+                      tal:condition="state_title"
+                >
+                ${state_title}
+                </span>
+              </tal:show-state-if-top>
+            </h6>
           </li>
           <li tal:repeat="subMenuItem submenu">
             <tal:block define="
                          extra_class subMenuItem/extra/class | string:;
                        ">
               <tal:noaction tal:define="
                               is_separator subMenuItem/extra/separator|nothing;
```

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/displayviewsmenu.py` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/displayviewsmenu.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/interfaces.py` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/menu.py` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             modal = action.get("modal", None)
             if modal:
                 cssClass += " pat-plone-modal"
 
             results.append(
                 {
                     "title": action["title"],
-                    "description": "",
+                    "description": action.get("description", ""),
                     "action": addTokenToUrl(action["url"], request),
                     "selected": False,
                     "icon": icon,
                     "extra": {
                         "id": "plone-contentmenu-actions-" + aid,
                         "separator": None,
                         "class": cssClass,
```

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/testing.py` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/tests/test_menu.py` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone/app/contentmenu/view.py` & `plone.app.contentmenu-3.0.2/plone/app/contentmenu/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/PKG-INFO` & `plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentmenu
-Version: 3.0.1
+Version: 3.0.2
 Summary: Plone's content menu implementation
 Home-page: https://pypi.org/project/plone.app.contentmenu
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone contentmenu menu
 Classifier: Development Status :: 5 - Production/Stable
@@ -152,14 +152,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-05-25)
+------------------
+
+Bug fixes:
+
+
+- Add description to actions' menu items
+  [kshitiz305] (#24)
+- Show workflow state title also when the toolbar is at the top.
+  [maurits] (#49)
+
+
 3.0.1 (2023-04-06)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentmenu-3.0.1/plone.app.contentmenu.egg-info/SOURCES.txt` & `plone.app.contentmenu-3.0.2/plone.app.contentmenu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/pyproject.toml` & `plone.app.contentmenu-3.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.1/setup.py` & `plone.app.contentmenu-3.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.1"
+version = "3.0.2"
 long_description = open("README.rst").read() + "\n"
 long_description += open("CHANGES.rst").read()
 
 setup(
     name="plone.app.contentmenu",
     version=version,
     description="Plone's content menu implementation",
```

### Comparing `plone.app.contentmenu-3.0.1/tox.ini` & `plone.app.contentmenu-3.0.2/tox.ini`

 * *Files identical despite different names*

