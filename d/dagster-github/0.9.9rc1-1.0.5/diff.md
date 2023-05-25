# Comparing `tmp/dagster-github-0.9.9rc1.tar.gz` & `tmp/dagster-github-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-github-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:43 2020, max compression
+gzip compressed data, was "dagster-github-1.0.5.tar", last modified: Fri Aug 26 13:46:27 2022, max compression
```

## Comparing `dagster-github-0.9.9rc1.tar` & `dagster-github-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      619 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github/
--rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5922 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      619 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      464 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       31 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6489 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1367 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:27.556785 dagster-github-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-github-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-26 13:33:01.000000 dagster-github-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      678 2022-08-26 13:46:27.556785 dagster-github-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2022-08-26 13:33:01.000000 dagster-github-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:27.552785 dagster-github-1.0.5/dagster_github/
+-rw-r--r--   0 root         (0) root         (0)      228 2022-08-26 13:33:01.000000 dagster-github-1.0.5/dagster_github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-github-1.0.5/dagster_github/py.typed
+-rw-r--r--   0 root         (0) root         (0)     6743 2022-08-26 13:33:01.000000 dagster-github-1.0.5/dagster_github/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-github-1.0.5/dagster_github/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:27.552785 dagster-github-1.0.5/dagster_github.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2022-08-26 13:46:27.000000 dagster-github-1.0.5/dagster_github.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2022-08-26 13:46:27.000000 dagster-github-1.0.5/dagster_github.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:27.000000 dagster-github-1.0.5/dagster_github.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:27.000000 dagster-github-1.0.5/dagster_github.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-26 13:46:27.000000 dagster-github-1.0.5/dagster_github.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:46:27.000000 dagster-github-1.0.5/dagster_github.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2022-08-26 13:46:27.556785 dagster-github-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2022-08-26 13:33:01.000000 dagster-github-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-github-0.9.9rc1/LICENSE` & `dagster-github-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-github-0.9.9rc1/dagster_github/resources.py` & `dagster-github-1.0.5/dagster_github/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 
 def to_seconds(dt):
     return (dt - datetime(1970, 1, 1)).total_seconds()
 
 
 class GithubResource:
-    def __init__(self, client, app_id, app_private_rsa_key, default_installation_id):
+    def __init__(self, client, app_id, app_private_rsa_key, default_installation_id, hostname=None):
         self.client = client
         self.app_private_rsa_key = app_private_rsa_key
         self.app_id = app_id
         self.default_installation_id = default_installation_id
         self.installation_tokens = {}
         self.app_token = {}
+        self.hostname = hostname
 
     def __set_app_token(self):
         # from https://developer.github.com/apps/building-github-apps/authenticating-with-github-apps/
         # needing to self-sign a JWT
         now = int(time.time())
         # JWT expiration time (10 minute maximum)
         expires = now + (10 * 60)
@@ -33,15 +34,15 @@
                 # JWT expiration time
                 "exp": expires,
                 # GitHub App's identifier
                 "iss": self.app_id,
             },
             self.app_private_rsa_key,
             algorithm="RS256",
-        ).decode("utf-8")
+        )
         self.app_token = {
             "value": encoded_token,
             "expires": expires,
         }
 
     def __check_app_token(self):
         if ("expires" not in self.app_token) or (
@@ -51,26 +52,35 @@
 
     def get_installations(self, headers=None):
         if headers is None:
             headers = {}
         self.__check_app_token()
         headers["Authorization"] = "Bearer {}".format(self.app_token["value"])
         headers["Accept"] = "application/vnd.github.machine-man-preview+json"
-        request = self.client.get("https://api.github.com/app/installations", headers=headers,)
+        request = self.client.get(
+            "https://api.github.com/app/installations"
+            if self.hostname is None
+            else "https://{}/api/v3/app/installations".format(self.hostname),
+            headers=headers,
+        )
         request.raise_for_status()
         return request.json()
 
     def __set_installation_token(self, installation_id, headers=None):
         if headers is None:
             headers = {}
         self.__check_app_token()
         headers["Authorization"] = "Bearer {}".format(self.app_token["value"])
         headers["Accept"] = "application/vnd.github.machine-man-preview+json"
         request = requests.post(
-            "https://api.github.com/app/installations/{}/access_tokens".format(installation_id),
+            "https://api.github.com/app/installations/{}/access_tokens".format(installation_id)
+            if self.hostname is None
+            else "https://{}/api/v3/app/installations/{}/access_tokens".format(
+                self.hostname, installation_id
+            ),
             headers=headers,
         )
         request.raise_for_status()
         auth = request.json()
         self.installation_tokens[installation_id] = {
             "value": auth["token"],
             "expires": to_seconds(datetime.strptime(auth["expires_at"], "%Y-%m-%dT%H:%M:%SZ")),
@@ -88,15 +98,17 @@
         if installation_id is None:
             installation_id = self.default_installation_id
         self.__check_installation_tokens(installation_id)
         headers["Authorization"] = "token {}".format(
             self.installation_tokens[installation_id]["value"]
         )
         request = requests.post(
-            "https://api.github.com/graphql",
+            "https://api.github.com/graphql"
+            if self.hostname is None
+            else "https://{}/api/graphql".format(self.hostname),
             json={"query": query, "variables": variables},
             headers=headers,
         )
         request.raise_for_status()
         return request.json()
 
     def create_issue(self, repo_name, repo_owner, title, body, installation_id=None):
@@ -127,15 +139,19 @@
                         body
                         title
                         url
                     }
                 }
                 }
             """,
-            variables={"id": res["data"]["repository"]["id"], "title": title, "body": body,},
+            variables={
+                "id": res["data"]["repository"]["id"],
+                "title": title,
+                "body": body,
+            },
             installation_id=installation_id,
         )
 
 
 @resource(
     config_schema={
         "github_app_id": Field(
@@ -147,17 +163,23 @@
             description="Github Application Private RSA key text, for more info see https://developer.github.com/apps/",
         ),
         "github_installation_id": Field(
             IntSource,
             is_required=False,
             description="Github Application Installation ID, for more info see https://developer.github.com/apps/",
         ),
+        "github_hostname": Field(
+            StringSource,
+            is_required=False,
+            description="Github hostname. Defaults to `api.github.com`, for more info see https://developer.github.com/apps/",
+        ),
     },
     description="This resource is for connecting to Github",
 )
 def github_resource(context):
     return GithubResource(
         client=requests.Session(),
         app_id=context.resource_config["github_app_id"],
         app_private_rsa_key=context.resource_config["github_app_private_rsa_key"],
         default_installation_id=context.resource_config["github_installation_id"],
+        hostname=context.resource_config.get("github_hostname", None),
     )
```

### Comparing `dagster-github-0.9.9rc1/setup.py` & `dagster-github-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_github/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_github/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-github",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="A Github client resource for interacting with the github API with a github App",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-github",
         classifiers=[
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
+        packages=find_packages(exclude=["dagster_github_tests*"]),
         install_requires=[
-            "dagster",
+            "dagster==1.0.5",
             # Using a Github app requires signing your own JWT :(
             # https://developer.github.com/apps/building-github-apps/authenticating-with-github-apps/
             "pyjwt[crypto]",
             # No officially supported python sdk for github :(
             "requests",
         ],
         zip_safe=False,
```

