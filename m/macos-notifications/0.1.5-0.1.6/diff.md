# Comparing `tmp/macos-notifications-0.1.5.tar.gz` & `tmp/macos_notifications-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macos-notifications-0.1.5.tar", last modified: Mon Aug  1 20:59:24 2022, max compression
+gzip compressed data, was "macos_notifications-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `macos-notifications-0.1.5.tar` & `macos_notifications-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0       68 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.flake8
--rw-r--r--   0        0        0      158 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.github/mkdocs-requirements.txt
--rw-r--r--   0        0        0      528 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.github/workflows/deploy-pypi.yml
--rw-r--r--   0        0        0      703 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      418 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0    14002 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.gitignore
--rw-r--r--   0        0        0     1739 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      455 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/LICENSE
--rw-r--r--   0        0        0     3296 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/README.md
--rw-r--r--   0        0        0      464 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/code/client.md
--rw-r--r--   0        0        0      124 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/code/listener_process.md
--rw-r--r--   0        0        0      238 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/code/manager.md
--rw-r--r--   0        0        0      325 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/code/notification_config.md
--rw-r--r--   0        0        0      142 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/code/notification_sender.md
--rw-r--r--   0        0        0      232 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/code/singleton.md
--rw-r--r--   0        0        0     3490 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/examples.md
--rw-r--r--   0        0        0      976 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/faq.md
--rw-r--r--   0        0        0   207427 2022-08-01 20:59:20.895942 macos-notifications-0.1.5/docs/img/enable-notifications.png
--rw-r--r--   0        0        0   351785 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/docs/img/example-run.gif
--rw-r--r--   0        0        0   117487 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/docs/img/macos-notifications.png
--rw-r--r--   0        0        0     2637 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/docs/index.md
--rw-r--r--   0        0        0     1132 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/docs/release-notes.md
--rw-r--r--   0        0        0      267 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/docs/user_guide.md
--rw-r--r--   0        0        0    10224 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/examples/img/chat.png
--rw-r--r--   0        0        0    20963 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/examples/img/zoom.png
--rw-r--r--   0        0        0     1355 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/examples/multiple_notifications_with_callbacks.py
--rw-r--r--   0        0        0      725 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/examples/notification_with_action.py
--rw-r--r--   0        0        0      699 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/examples/notification_with_reply.py
--rw-r--r--   0        0        0      151 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/examples/simple_notification.py
--rw-r--r--   0        0        0     2499 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/mkdocs.yml
--rw-r--r--   0        0        0     2557 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      140 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/__init__.py
--rw-r--r--   0        0        0     2369 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/client.py
--rw-r--r--   0        0        0     1365 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/listener_process.py
--rw-r--r--   0        0        0     7885 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/manager.py
--rw-r--r--   0        0        0     3164 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/notification_config.py
--rw-r--r--   0        0        0     4730 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/notification_sender.py
--rw-r--r--   0        0        0      550 2022-08-01 20:59:20.899944 macos-notifications-0.1.5/src/mac_notifications/singleton.py
--rw-r--r--   0        0        0     5613 1970-01-01 00:00:00.000000 macos-notifications-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.flake8
+-rw-r--r--   0        0        0      158 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.github/mkdocs-requirements.txt
+-rw-r--r--   0        0        0      528 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.github/workflows/deploy-pypi.yml
+-rw-r--r--   0        0        0      703 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      418 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0    14002 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1739 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      455 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3296 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/README.md
+-rw-r--r--   0        0        0      464 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/code/client.md
+-rw-r--r--   0        0        0      124 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/code/listener_process.md
+-rw-r--r--   0        0        0      238 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/code/manager.md
+-rw-r--r--   0        0        0      325 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/code/notification_config.md
+-rw-r--r--   0        0        0      142 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/code/notification_sender.md
+-rw-r--r--   0        0        0      232 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/code/singleton.md
+-rw-r--r--   0        0        0     3490 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/examples.md
+-rw-r--r--   0        0        0      976 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/faq.md
+-rw-r--r--   0        0        0   207427 2023-05-25 15:03:37.090177 macos_notifications-0.1.6/docs/img/enable-notifications.png
+-rw-r--r--   0        0        0   351785 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/docs/img/example-run.gif
+-rw-r--r--   0        0        0   117487 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/docs/img/macos-notifications.png
+-rw-r--r--   0        0        0     2637 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/docs/index.md
+-rw-r--r--   0        0        0     1132 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/docs/release-notes.md
+-rw-r--r--   0        0        0      267 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/docs/user_guide.md
+-rw-r--r--   0        0        0    10224 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/examples/img/chat.png
+-rw-r--r--   0        0        0    20963 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/examples/img/zoom.png
+-rw-r--r--   0        0        0     1355 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/examples/multiple_notifications_with_callbacks.py
+-rw-r--r--   0        0        0      725 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/examples/notification_with_action.py
+-rw-r--r--   0        0        0      699 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/examples/notification_with_reply.py
+-rw-r--r--   0        0        0      151 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/examples/simple_notification.py
+-rw-r--r--   0        0        0     2499 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/mkdocs.yml
+-rw-r--r--   0        0        0     2561 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/__init__.py
+-rw-r--r--   0        0        0     2369 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/client.py
+-rw-r--r--   0        0        0     1365 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/listener_process.py
+-rw-r--r--   0        0        0     7885 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/manager.py
+-rw-r--r--   0        0        0     3164 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/notification_config.py
+-rw-r--r--   0        0        0     4730 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/notification_sender.py
+-rw-r--r--   0        0        0      550 2023-05-25 15:03:37.094177 macos_notifications-0.1.6/src/mac_notifications/singleton.py
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 macos_notifications-0.1.6/PKG-INFO
```

### Comparing `macos-notifications-0.1.5/.github/workflows/deploy-pypi.yml` & `macos_notifications-0.1.6/.github/workflows/deploy-pypi.yml`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/.github/workflows/latest-changes.yml` & `macos_notifications-0.1.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/.gitignore` & `macos_notifications-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/.pre-commit-config.yaml` & `macos_notifications-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/LICENSE` & `macos_notifications-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/README.md` & `macos_notifications-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/examples.md` & `macos_notifications-0.1.6/docs/examples.md`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/faq.md` & `macos_notifications-0.1.6/docs/faq.md`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/img/enable-notifications.png` & `macos_notifications-0.1.6/docs/img/enable-notifications.png`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/img/example-run.gif` & `macos_notifications-0.1.6/docs/img/example-run.gif`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/img/macos-notifications.png` & `macos_notifications-0.1.6/docs/img/macos-notifications.png`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/index.md` & `macos_notifications-0.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/docs/release-notes.md` & `macos_notifications-0.1.6/docs/release-notes.md`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/examples/img/chat.png` & `macos_notifications-0.1.6/examples/img/chat.png`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/examples/img/zoom.png` & `macos_notifications-0.1.6/examples/img/zoom.png`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/examples/multiple_notifications_with_callbacks.py` & `macos_notifications-0.1.6/examples/multiple_notifications_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/examples/notification_with_action.py` & `macos_notifications-0.1.6/examples/notification_with_action.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/examples/notification_with_reply.py` & `macos_notifications-0.1.6/examples/notification_with_reply.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/mkdocs.yml` & `macos_notifications-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/pyproject.toml` & `macos_notifications-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 dependencies = [
-    "pyobjc-core==8.5",
-    "pyobjc-framework-Cocoa==8.5",
+    "pyobjc-core>=9.1.1",
+    "pyobjc-framework-Cocoa>=9.1.1",
 ]
 
 [project.optional-dependencies]
 test = [
     "flake8 >=4.0.0,<5.0.0",
     "black >= 22.6.0,<23.0.0",
     "isort >=5.10.1,<6.0.0",
```

### Comparing `macos-notifications-0.1.5/src/mac_notifications/client.py` & `macos_notifications-0.1.6/src/mac_notifications/client.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/src/mac_notifications/listener_process.py` & `macos_notifications-0.1.6/src/mac_notifications/listener_process.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/src/mac_notifications/manager.py` & `macos_notifications-0.1.6/src/mac_notifications/manager.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/src/mac_notifications/notification_config.py` & `macos_notifications-0.1.6/src/mac_notifications/notification_config.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/src/mac_notifications/notification_sender.py` & `macos_notifications-0.1.6/src/mac_notifications/notification_sender.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/src/mac_notifications/singleton.py` & `macos_notifications-0.1.6/src/mac_notifications/singleton.py`

 * *Files identical despite different names*

### Comparing `macos-notifications-0.1.5/PKG-INFO` & `macos_notifications-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macos-notifications
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple interactable Mac notifications with only pure-python dependencies
 Author-email: Jorrick Sleijster <jorricks3@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pyobjc-core==8.5
-Requires-Dist: pyobjc-framework-Cocoa==8.5
+Requires-Dist: pyobjc-core>=9.1.1
+Requires-Dist: pyobjc-framework-Cocoa>=9.1.1
 Requires-Dist: pre-commit >=2.19.0,<3.0.0 ; extra == "dev"
 Requires-Dist: mkdocs >=1.3.0,<2.0.0 ; extra == "doc"
 Requires-Dist: mkdocs-material >=8.3.9,<9.0.0 ; extra == "doc"
 Requires-Dist: mkdocstrings[python] >=0.19.0,<1.0.0 ; extra == "doc"
 Requires-Dist: termynal >=0.2.0,<1.0.0 ; extra == "doc"
 Requires-Dist: flake8 >=4.0.0,<5.0.0 ; extra == "test"
 Requires-Dist: black >= 22.6.0,<23.0.0 ; extra == "test"
```

