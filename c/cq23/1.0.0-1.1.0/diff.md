# Comparing `tmp/cq23-1.0.0.tar.gz` & `tmp/cq23-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.0.0.tar", last modified: Thu May 25 04:42:05 2023, max compression
+gzip compressed data, was "cq23-1.1.0.tar", last modified: Thu May 25 07:20:48 2023, max compression
```

## Comparing `cq23-1.0.0.tar` & `cq23-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.631007 cq23-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 04:42:05.631007 cq23-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 04:41:56.000000 cq23-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 04:41:56.000000 cq23-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-25 04:42:05.631007 cq23-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.627007 cq23-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.627007 cq23-1.0.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 04:42:05.000000 cq23-1.0.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.631007 cq23-1.0.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 04:41:56.000000 cq23-1.0.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 04:41:56.000000 cq23-1.0.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 04:41:56.000000 cq23-1.0.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 04:42:05.631007 cq23-1.0.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 04:41:56.000000 cq23-1.0.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:48.845411 cq23-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 07:20:48.845411 cq23-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 07:20:39.000000 cq23-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 07:20:39.000000 cq23-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-25 07:20:48.845411 cq23-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:48.841411 cq23-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:48.841411 cq23-1.1.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:39.000000 cq23-1.1.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 07:20:39.000000 cq23-1.1.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:48.841411 cq23-1.1.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 07:20:48.000000 cq23-1.1.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 07:20:48.000000 cq23-1.1.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:20:48.000000 cq23-1.1.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 07:20:48.000000 cq23-1.1.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 07:20:48.000000 cq23-1.1.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 07:20:48.000000 cq23-1.1.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:48.841411 cq23-1.1.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:39.000000 cq23-1.1.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 07:20:39.000000 cq23-1.1.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 07:20:39.000000 cq23-1.1.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:48.845411 cq23-1.1.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:39.000000 cq23-1.1.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-25 07:20:39.000000 cq23-1.1.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-25 07:20:39.000000 cq23-1.1.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 07:20:39.000000 cq23-1.1.0/src/run_game/gcs.py
```

### Comparing `cq23-1.0.0/PKG-INFO` & `cq23-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.0.0
+Version: 1.1.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.0.0/setup.cfg` & `cq23-1.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.0.0
+version = 1.1.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.0.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.1.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.0.0
+Version: 1.1.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.0.0/src/run_game/command.py` & `cq23-1.1.0/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.0.0/src/run_game/docker_tools.py` & `cq23-1.1.0/src/run_game/docker_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def get_client_image_tag():
     return "cq-local-dev-client:latest"
 
 
 def pull_latest_game_server():
-    print("Pulling the game server...", end=" ")
+    print("Pulling the game server...", end=" ", flush=True)
     game_server_image = get_server_image_tag()
     try:
         DOCKER_CLIENT.images.pull(game_server_image)
         print("Done!")
     except APIError:
         print("Failed to pull the game server!")
         return False
@@ -42,21 +42,20 @@
             "Dockerfile not found! Make sure you run `cq23_run` from the directory that contains your bot's"
             "Dockerfile."
         )
 
 
 def build_and_tag_image(image_tag):
     print("Building the image...")
-    client = docker.from_env()
     current_dir = os.getcwd()
     dockerfile_path = os.path.join(current_dir, "Dockerfile")
 
     # Build the Docker image
-    image, _ = client.images.build(
-        path=current_dir, dockerfile=dockerfile_path, tag=image_tag
+    image, _ = DOCKER_CLIENT.images.build(
+        path=current_dir, dockerfile=dockerfile_path, tag=image_tag, rm=True
     )
 
     # Print the ID of the built image
     print("Docker image built with ID:", image.id)
 
 
 def copy_replay_files(game_files_abs_path):
```

### Comparing `cq23-1.0.0/src/run_game/gcs.py` & `cq23-1.1.0/src/run_game/gcs.py`

 * *Files identical despite different names*

