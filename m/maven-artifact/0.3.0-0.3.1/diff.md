# Comparing `tmp/maven_artifact-0.3.0.tar.gz` & `tmp/maven_artifact-0.3.1.tar.gz`

## Comparing `maven_artifact-0.3.0.tar` & `maven_artifact-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/_version.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/.github/workflows/linting.yml
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/.github/workflows/pypi-build-n-publish.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/src/maven_artifact/__init__.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/src/maven_artifact/artifact.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/src/maven_artifact/downloader.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/src/maven_artifact/requestor.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/src/maven_artifact/resolver.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/tests/integration/maven_artifact/test_downloader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/tests/unit/conftest.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/tests/unit/maven_artifact/test_artifact.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/.gitignore
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/README.md
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 maven_artifact-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/.envrc
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/_version.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/dev-requirements.txt
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/.github/workflows/linting.yml
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/.github/workflows/pypi-build-n-publish.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/artifact.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/downloader.py
+-rwxr-xr-x   0        0        0     4937 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/main.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/requestor.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/resolver.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/src/maven_artifact/utils.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/tests/integration/maven_artifact/test_downloader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/tests/unit/maven_artifact/test_artifact.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/.gitignore
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/README.md
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 maven_artifact-0.3.1/PKG-INFO
```

### Comparing `maven_artifact-0.3.0/.github/dependabot.yml` & `maven_artifact-0.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.0/.github/workflows/linting.yml` & `maven_artifact-0.3.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.0/.github/workflows/pypi-build-n-publish.yml` & `maven_artifact-0.3.1/.github/workflows/pypi-build-n-publish.yml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.0/src/maven_artifact/artifact.py` & `maven_artifact-0.3.1/src/maven_artifact/artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,23 +51,23 @@
             return "%s:%s:%s:%s:%s" % (self.group_id, self.artifact_id, self.extension, self.classifier, self.version)
         elif self.extension != "jar":
             return "%s:%s:%s:%s" % (self.group_id, self.artifact_id, self.extension, self.version)
         else:
             return "%s:%s:%s" % (self.group_id, self.artifact_id, self.version)
 
     @staticmethod
-    def parse(input):
-        parts = input.split(":")
+    def parse(maven_coordinate):
+        parts = maven_coordinate.split(":")
         if len(parts) >= 3:
             g = parts[0]
             a = parts[1]
             v = parts[len(parts) - 1]
             t = None
             c = None
             if len(parts) == 4:
                 t = parts[2]
             if len(parts) == 5:
                 t = parts[2]
                 c = parts[3]
-            return Artifact(g, a, v, c, t)
+            return Artifact(group_id=g, artifact_id=a, version=v, classifier=c, extension=t)
         else:
             return None
```

### Comparing `maven_artifact-0.3.0/src/maven_artifact/requestor.py` & `maven_artifact-0.3.1/src/maven_artifact/requestor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import base64
 import requests
 
+from maven_artifact.utils import Utils
+
 
 class RequestException(Exception):
     def __init__(self, msg):
         self.msg = msg
 
 
 class Requestor(object):
-    def __init__(self, username=None, password=None, user_agent="Maven Artifact Downloader/1.0"):
+    def __init__(self, username=None, password=None, token=None, user_agent="Maven Artifact Downloader/1.0"):
         self.user_agent = user_agent
         self.username = username
         self.password = password
+        self.token = token
 
     def request(self, url, onFail, onSuccess=None, method: str = "get", **kwargs):
         headers = {"User-Agent": self.user_agent}
+
         if self.username and self.password:
             token = self.username + ":" + self.password
-            headers["Authorization"] = "Basic " + base64.b64encode(token.encode()).decode()
+            headers["Authorization"] = f"Basic {base64.b64encode(token.encode()).decode()}"
+        elif Utils.is_base64(self.password):
+            headers["Authorization"] = f"Basic {self.password}"
+        elif self.token:
+            headers["Authorization"] = f"Bearer {base64.b64encode(self.token.encode()).decode()}"
 
         try:
             response = getattr(requests, method)(url, headers=headers, **kwargs)
             response.raise_for_status()
             if onSuccess:
                 return onSuccess(response)
             return response
```

### Comparing `maven_artifact-0.3.0/src/maven_artifact/resolver.py` & `maven_artifact-0.3.1/src/maven_artifact/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from lxml import etree
 
-from .requestor import RequestException
+from maven_artifact.requestor import RequestException
 
 
 class Resolver(object):
     def __init__(self, base, requestor):
         self.requestor = requestor
         if base.endswith("/"):
             base = base.rstrip("/")
```

### Comparing `maven_artifact-0.3.0/README.md` & `maven_artifact-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.0/pyproject.toml` & `maven_artifact-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ]
 
 requires-python = ">=3.8"
 
 dependencies = ["lxml", "requests"]
 
 [project.scripts]
-maven-artifact = "maven_artifact.downloader:main"
+maven-artifact = "maven_artifact.main:main"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "_version.py"
```

### Comparing `maven_artifact-0.3.0/PKG-INFO` & `maven_artifact-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maven-artifact
-Version: 0.3.0
+Version: 0.3.1
 Summary: Download and resolve maven artifacts
 Author-email: Erlend Hamnaberg <erlend@hamnaberg.net>
 License-Expression: Apache-2.0
 Keywords: artifact,download,maven,mvn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

