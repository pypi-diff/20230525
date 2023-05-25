# Comparing `tmp/pytmac-3.3.1.tar.gz` & `tmp/pytmac-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.3.1.tar", last modified: Wed May 24 20:11:58 2023, max compression
+gzip compressed data, was "pytmac-3.3.2.tar", last modified: Thu May 25 20:04:52 2023, max compression
```

## Comparing `pytmac-3.3.1.tar` & `pytmac-3.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:11:58.496597 pytmac-3.3.1/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-24 20:11:55.000000 pytmac-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6061 2023-05-24 20:11:58.496597 pytmac-3.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5948 2023-05-24 20:11:55.000000 pytmac-3.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 20:11:56.000000 pytmac-3.3.1/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:11:58.492597 pytmac-3.3.1/bin/
--rw-r--r--   0 root         (0) root         (0)     2954 2023-05-24 20:11:55.000000 pytmac-3.3.1/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-24 20:11:55.000000 pytmac-3.3.1/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2823 2023-05-24 20:11:55.000000 pytmac-3.3.1/bin/resource_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:11:58.496597 pytmac-3.3.1/docs/
--rw-r--r--   0 root         (0) root         (0)      241 2023-05-24 20:11:55.000000 pytmac-3.3.1/docs/config.yaml
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-24 20:11:55.000000 pytmac-3.3.1/docs/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-24 20:11:55.000000 pytmac-3.3.1/docs/resources.yaml
--rw-r--r--   0 root         (0) root         (0)     7555 2023-05-24 20:11:55.000000 pytmac-3.3.1/docs/security_checks.yaml
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-24 20:11:55.000000 pytmac-3.3.1/docs/swagger.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-24 20:11:55.000000 pytmac-3.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    19795 2023-05-24 20:11:58.000000 pytmac-3.3.1/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:11:58.496597 pytmac-3.3.1/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6061 2023-05-24 20:11:58.000000 pytmac-3.3.1/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-24 20:11:58.000000 pytmac-3.3.1/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 20:11:58.000000 pytmac-3.3.1/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-24 20:11:58.000000 pytmac-3.3.1/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 20:11:58.000000 pytmac-3.3.1/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 20:11:58.496597 pytmac-3.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      868 2023-05-24 20:11:55.000000 pytmac-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.015907 pytmac-3.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-25 20:04:48.000000 pytmac-3.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7413 2023-05-25 20:04:52.015907 pytmac-3.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7300 2023-05-25 20:04:48.000000 pytmac-3.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-25 20:04:49.000000 pytmac-3.3.2/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.011907 pytmac-3.3.2/bin/
+-rw-r--r--   0 root         (0) root         (0)     5175 2023-05-25 20:04:48.000000 pytmac-3.3.2/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-25 20:04:48.000000 pytmac-3.3.2/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2023-05-25 20:04:48.000000 pytmac-3.3.2/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.011907 pytmac-3.3.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-25 20:04:48.000000 pytmac-3.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    21594 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.015907 pytmac-3.3.2/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7413 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-25 20:04:52.000000 pytmac-3.3.2/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 20:04:52.015907 pytmac-3.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      868 2023-05-25 20:04:48.000000 pytmac-3.3.2/setup.py
```

### Comparing `pytmac-3.3.1/LICENSE` & `pytmac-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/PKG-INFO` & `pytmac-3.3.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: pytmac
-Version: 3.3.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -63,14 +57,40 @@
 pytmac --demo
 ```
 
 This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
+## Config file
+
+pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
+
+```
+resource_file: "docs/resources.yaml"
+config_file: "docs/config.yaml"
+defaults_file: "docs/defaults.yaml"
+```
+
+If both a config file value and a manual override is added via the command line, the command line value will take precedence.
+
+Eg if you have a .pytmac file with the following:
+
+```
+resource_file: "docs/resources.yaml"
+```
+
+and call pytmac with the following:
+
+```
+pytmac --resources-file resources.yaml
+```
+
+the resources.yaml file will be used over the one defined in the .pytmac file.
+
 ## Resources
 
 Resources are defined as any asset that is part of the system being modelled under the following categories:
 
 - Databases
 - Networks
 - Systems
@@ -103,15 +123,39 @@
 ## Security Checks
 
 Security checks have been included to cover use cases for the Owasp top 10, however you may want to extend pytmac with custom checks can be written and added to `./docs/security_checks.yaml`. These files should be written as below, the 
 checks are iterated over and executed individually, all fields are required.
 
 Severity should be used as a combination of Risk vs Likelihood, any security findings are prioritised by severity in the report output. 
 
+```## Config file
+
+pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
+
+```
+resource_file: "docs/resources.yaml"
+config_file: "docs/config.yaml"
+defaults_file: "docs/defaults.yaml"
+```
+
+If both a config file value and a manual override is added via the command line, the command line value will take precedence.
+
+Eg if you have a .pytmac file with the following:
+
+```
+resource_file: "docs/resources.yaml"
 ```
+
+and call pytmac with the following:
+
+```
+pytmac --resources-file resources.yaml
+```
+
+the resources.yaml file will be used over the one defined in the .pytmac file.
 user_owned_device:
   name: Non company device used
   description: Checks for users with company_user true and company_device false.
   remediation: Understand and remediate or document known exception.
   severity: 3
   resource_scope:
     - users
```

### Comparing `pytmac-3.3.1/README.md` & `pytmac-3.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: pytmac
+Version: 3.3.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -57,14 +63,40 @@
 pytmac --demo
 ```
 
 This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
+## Config file
+
+pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
+
+```
+resource_file: "docs/resources.yaml"
+config_file: "docs/config.yaml"
+defaults_file: "docs/defaults.yaml"
+```
+
+If both a config file value and a manual override is added via the command line, the command line value will take precedence.
+
+Eg if you have a .pytmac file with the following:
+
+```
+resource_file: "docs/resources.yaml"
+```
+
+and call pytmac with the following:
+
+```
+pytmac --resources-file resources.yaml
+```
+
+the resources.yaml file will be used over the one defined in the .pytmac file.
+
 ## Resources
 
 Resources are defined as any asset that is part of the system being modelled under the following categories:
 
 - Databases
 - Networks
 - Systems
@@ -97,15 +129,39 @@
 ## Security Checks
 
 Security checks have been included to cover use cases for the Owasp top 10, however you may want to extend pytmac with custom checks can be written and added to `./docs/security_checks.yaml`. These files should be written as below, the 
 checks are iterated over and executed individually, all fields are required.
 
 Severity should be used as a combination of Risk vs Likelihood, any security findings are prioritised by severity in the report output. 
 
+```## Config file
+
+pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
+
+```
+resource_file: "docs/resources.yaml"
+config_file: "docs/config.yaml"
+defaults_file: "docs/defaults.yaml"
+```
+
+If both a config file value and a manual override is added via the command line, the command line value will take precedence.
+
+Eg if you have a .pytmac file with the following:
+
+```
+resource_file: "docs/resources.yaml"
 ```
+
+and call pytmac with the following:
+
+```
+pytmac --resources-file resources.yaml
+```
+
+the resources.yaml file will be used over the one defined in the .pytmac file.
 user_owned_device:
   name: Non company device used
   description: Checks for users with company_user true and company_device false.
   remediation: Understand and remediate or document known exception.
   severity: 3
   resource_scope:
     - users
```

### Comparing `pytmac-3.3.1/bin/input_validator.py` & `pytmac-3.3.2/bin/input_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/bin/resource_validator.py` & `pytmac-3.3.2/bin/resource_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/docs/defaults.yaml` & `pytmac-3.3.2/docs/defaults.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/docs/resources.yaml` & `pytmac-3.3.2/docs/resources.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/docs/security_checks.yaml` & `pytmac-3.3.2/docs/security_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/docs/swagger.json` & `pytmac-3.3.2/docs/swagger.json`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.1/pytmac` & `pytmac-3.3.2/pytmac`

 * *Files 6% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 "description": swagger_json["paths"][swagger_path][
                     str(list(swagger_json["paths"][swagger_path].keys())[0])
                 ]["description"],
             }
             # Append swagger endpoint to default swagger_resource_type resources
             if (
                 resources_yaml["resources"][config_yaml["swagger_resource_type"]]
-                == None
+                is None
             ):
                 resources_yaml["resources"][config_yaml["swagger_resource_type"]] = []
                 resources_yaml["resources"][
                     config_yaml["swagger_resource_type"]
                 ].append(swagger_path_detail)
             else:
                 if isinstance(
@@ -457,60 +457,100 @@
         logging.info("Running in demonstration mode")
         resources_input = get_config.resources("demo")
         config_input = get_config.config("demo")
         defaults_input = get_config.defaults("demo")
         security_checks_input = get_config.security_checks("default")
         swagger_input = get_config.swagger("demo")
     else:
-        if str(args.resources_file) != "None":
-            if args.resources_file == "test":
-                resources_input = get_config.resources("demo")
+        # Check if .pytmac file exists
+        if os.path.isfile(".pytmac"):
+            SETTINGS_FILE_EXISTS = True
+            logging.info("Found .pytmac settings file")
+            settings_input = get_config.settings()
+        else:
+            SETTINGS_FILE_EXISTS = False
+            logging.info("No settings file found")
+
+        error_response_list = []
+        if str(args.resources_file) != "None" or (
+            SETTINGS_FILE_EXISTS and "resource_file" in settings_input
+        ):
+            if str(args.resources_file) != "None":
+                logging.info("Using resources file from command line")
+                resource_source_file = args.resources_file
             else:
-                resources_input = get_config.resources(args.resources_file)
+                resource_source_file = settings_input["resource_file"]
+            resources_input = get_config.resources(resource_source_file)
         else:
-            logging.error("--resource-file is required, see --help for details")
-            sys.exit(1)
+            error_response_list.append(
+                "resource-file is required, see --help for details"
+            )
 
-        if str(args.config_file) != "None":
-            if args.config_file == "test":
-                config_input = get_config.config("demo")
+        if str(args.config_file) != "None" or (
+            SETTINGS_FILE_EXISTS and "config_file" in settings_input
+        ):
+            if str(args.config_file) != "None":
+                logging.info("Using config file from command line")
+                config_source_file = args.config_file
             else:
-                config_input = get_config.config(args.config_file)
+                config_source_file = settings_input["config_file"]
+
+            try:
+                config_input = get_config.config(config_source_file)
+            except Exception as error_message:
+                error_response_list.append(
+                    "Error loading config file: " + str(error_message)
+                )
         else:
-            logging.error("--config-file is required, see --help for details")
-            sys.exit(1)
+            error_response_list.append("config-file is required")
 
-        if str(args.defaults_file) != "None":
-            if args.defaults_file == "test":
-                defaults_input = get_config.defaults("demo")
+        if str(args.defaults_file) != "None" or (
+            SETTINGS_FILE_EXISTS and "defaults_file" in settings_input
+        ):
+            if str(args.defaults_file) != "None":
+                logging.info("Using defaults file from command line")
+                defaults_source_file = args.defaults_file
             else:
-                defaults_input = get_config.defaults(args.defaults_file)
+                defaults_source_file = settings_input["defaults_file"]
+            try:
+                defaults_input = get_config.defaults(defaults_source_file)
+            except Exception as error_message:
+                error_response_list.append(
+                    "Error loading defaults file: " + str(error_message)
+                )
         else:
-            logging.error("--defaults-file is required, see --help for details")
-            sys.exit(1)
+            error_response_list.append("defaults-file is required")
 
-        if str(args.security_checks_file) != "Default":
-            if args.security_checks_file == "test":
-                security_checks_input = get_config.security_checks("default")
+        if str(args.security_checks_file) != "Default" or (
+            SETTINGS_FILE_EXISTS and "security_checks_file" in settings_input
+        ):
+            if str(args.security_checks_file) != "Default":
+                logging.info("Using security checks file from command line")
+                sec_source_file = args.security_checks_file
             else:
-                security_checks_input = get_config.config(args.security_checks_file)
+                sec_source_file = settings_input["security_checks_file"]
+            security_checks_input = get_config.security_checks(sec_source_file)
         else:
             security_checks_input = get_config.security_checks("default")
 
         if str(args.swagger_file) != "None":
-            if args.swagger_file == "test":
-                swagger_input = get_config.swagger("demo")
-            else:
-                swagger_input = get_config.swagger(args.swagger_file)
+            logging.info("Using swagger file from command line")
+            SWAGGER_INPUT = get_config.swagger(args.swagger_file)
         else:
-            swagger_input = "None"
+            SWAGGER_INPUT = "None"
 
-        logging.info("Requires input")
+        if len(error_response_list) > 0:
+            logging.error(
+                "Error loading configuration files: "
+                + ", ".join(error_response_list)
+                + ". See --help for details"
+            )
+            sys.exit(1)
 
-    main(
-        resources_input,
-        config_input,
-        defaults_input,
-        security_checks_input,
-        args.output_dir,
-        swagger_input,
-    )
+        main(
+            resources_input,
+            config_input,
+            defaults_input,
+            security_checks_input,
+            args.output_dir,
+            SWAGGER_INPUT,
+        )
```

### Comparing `pytmac-3.3.1/pytmac.egg-info/PKG-INFO` & `pytmac-3.3.2/pytmac.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.3.1
+Version: 3.3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -63,14 +63,40 @@
 pytmac --demo
 ```
 
 This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
+## Config file
+
+pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
+
+```
+resource_file: "docs/resources.yaml"
+config_file: "docs/config.yaml"
+defaults_file: "docs/defaults.yaml"
+```
+
+If both a config file value and a manual override is added via the command line, the command line value will take precedence.
+
+Eg if you have a .pytmac file with the following:
+
+```
+resource_file: "docs/resources.yaml"
+```
+
+and call pytmac with the following:
+
+```
+pytmac --resources-file resources.yaml
+```
+
+the resources.yaml file will be used over the one defined in the .pytmac file.
+
 ## Resources
 
 Resources are defined as any asset that is part of the system being modelled under the following categories:
 
 - Databases
 - Networks
 - Systems
@@ -103,15 +129,39 @@
 ## Security Checks
 
 Security checks have been included to cover use cases for the Owasp top 10, however you may want to extend pytmac with custom checks can be written and added to `./docs/security_checks.yaml`. These files should be written as below, the 
 checks are iterated over and executed individually, all fields are required.
 
 Severity should be used as a combination of Risk vs Likelihood, any security findings are prioritised by severity in the report output. 
 
+```## Config file
+
+pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
+
+```
+resource_file: "docs/resources.yaml"
+config_file: "docs/config.yaml"
+defaults_file: "docs/defaults.yaml"
+```
+
+If both a config file value and a manual override is added via the command line, the command line value will take precedence.
+
+Eg if you have a .pytmac file with the following:
+
+```
+resource_file: "docs/resources.yaml"
 ```
+
+and call pytmac with the following:
+
+```
+pytmac --resources-file resources.yaml
+```
+
+the resources.yaml file will be used over the one defined in the .pytmac file.
 user_owned_device:
   name: Non company device used
   description: Checks for users with company_user true and company_device false.
   remediation: Understand and remediate or document known exception.
   severity: 3
   resource_scope:
     - users
```

### Comparing `pytmac-3.3.1/setup.py` & `pytmac-3.3.2/setup.py`

 * *Files identical despite different names*

