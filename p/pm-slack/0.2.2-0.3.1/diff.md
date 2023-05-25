# Comparing `tmp/pm_slack-0.2.2.tar.gz` & `tmp/pm_slack-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm_slack-0.2.2.tar", max compression
+gzip compressed data, was "pm_slack-0.3.1.tar", max compression
```

## Comparing `pm_slack-0.2.2.tar` & `pm_slack-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-05-17 13:00:09.942545 pm_slack-0.2.2/LICENSE
--rw-r--r--   0        0        0       45 2023-05-17 13:00:09.942545 pm_slack-0.2.2/README.md
--rw-r--r--   0        0        0       76 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/main.py
--rw-r--r--   0        0        0        0 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/py.typed
--rw-r--r--   0        0        0      391 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/templates/__init__.py
--rw-r--r--   0        0        0     6131 2023-05-17 13:00:09.942545 pm_slack-0.2.2/pm_slack/templates/_templates.py
--rw-r--r--   0        0        0     1098 2023-05-17 13:00:32.242980 pm_slack-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-25 09:25:16.560981 pm_slack-0.3.1/LICENSE
+-rw-r--r--   0        0        0       45 2023-05-25 09:25:16.560981 pm_slack-0.3.1/README.md
+-rw-r--r--   0        0        0       76 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/py.typed
+-rw-r--r--   0        0        0     1079 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/templates/__init__.py
+-rw-r--r--   0        0        0    21356 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/templates/_templates.py
+-rw-r--r--   0        0        0     1107 2023-05-25 09:25:44.417058 pm_slack-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.3.1/PKG-INFO
```

### Comparing `pm_slack-0.2.2/LICENSE` & `pm_slack-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pm_slack-0.2.2/pm_slack/main.py` & `pm_slack-0.3.1/pm_slack/main.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.2.2/pyproject.toml` & `pm_slack-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pm_slack"
-version = "v0.2.2"
+version = "0.3.1"
 description = "A Slack Library for Paket Mutfak"
 authors = ["Paket Mutfak Dev Team <dev@paketmutfak.com.tr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 slack-sdk = "^3.21.3"
-ruff = "^0.0.267"
+ruff = ">=0.0.267,<0.0.271"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3.0"
 mypy = ">=1.2.0"
 pre-commit = ">=3.3.1"
 pytest = ">=7.3.0"
 pytest-cov = ">=4.0.0"
```

### Comparing `pm_slack-0.2.2/PKG-INFO` & `pm_slack-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pm-slack
-Version: 0.2.2
+Version: 0.3.1
 Summary: A Slack Library for Paket Mutfak
 License: MIT
 Author: Paket Mutfak Dev Team
 Author-email: dev@paketmutfak.com.tr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ruff (>=0.0.267,<0.0.268)
+Requires-Dist: ruff (>=0.0.267,<0.0.271)
 Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 # pm_slack
 
 A Slack Library for Paket Mutfak
```

