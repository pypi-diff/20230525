# Comparing `tmp/SecretManagerCredentials-0.0.5.tar.gz` & `tmp/SecretManagerCredentials-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecretManagerCredentials-0.0.5.tar", last modified: Wed May 17 02:18:37 2023, max compression
+gzip compressed data, was "SecretManagerCredentials-0.0.6.tar", last modified: Thu May 25 11:57:58 2023, max compression
```

## Comparing `SecretManagerCredentials-0.0.5.tar` & `SecretManagerCredentials-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 02:18:37.540338 SecretManagerCredentials-0.0.5/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.5/Licence
--rw-rw-rw-   0        0        0     2151 2023-05-17 02:18:37.541334 SecretManagerCredentials-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1524 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 02:18:37.517434 SecretManagerCredentials-0.0.5/SecretManagerCredentials/
--rw-rw-rw-   0        0        0    10413 2023-05-17 02:07:52.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials/SecretManagerFetcher.py
--rw-rw-rw-   0        0        0      143 2023-05-17 02:18:00.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 02:18:37.537218 SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/
--rw-rw-rw-   0        0        0     2151 2023-05-17 02:18:37.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-05-17 02:18:37.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 02:18:37.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-17 02:18:37.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-17 02:18:37.000000 SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       83 2023-05-17 02:18:37.545335 SecretManagerCredentials-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-05-16 12:39:53.000000 SecretManagerCredentials-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:57:58.896431 SecretManagerCredentials-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.6/Licence
+-rw-rw-rw-   0        0        0     1896 2023-05-25 11:57:58.896431 SecretManagerCredentials-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1269 2023-05-25 11:53:59.000000 SecretManagerCredentials-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 11:57:58.865180 SecretManagerCredentials-0.0.6/SecretManagerCredentials/
+-rw-rw-rw-   0        0        0    10416 2023-05-25 11:53:12.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials/SecretManagerFetcher.py
+-rw-rw-rw-   0        0        0      143 2023-05-25 11:53:59.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:57:58.896431 SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/
+-rw-rw-rw-   0        0        0     1896 2023-05-25 11:57:58.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-05-25 11:57:58.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 11:57:58.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-25 11:57:58.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-25 11:57:58.000000 SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       83 2023-05-25 11:57:58.896431 SecretManagerCredentials-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-05-16 12:39:53.000000 SecretManagerCredentials-0.0.6/setup.py
```

### Comparing `SecretManagerCredentials-0.0.5/Licence` & `SecretManagerCredentials-0.0.6/Licence`

 * *Files identical despite different names*

### Comparing `SecretManagerCredentials-0.0.5/PKG-INFO` & `SecretManagerCredentials-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecretManagerCredentials
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault
 Home-page: 
 Download-URL: 
 Author: Mallikarjuna Devaraya
 License: MIT
 Keywords: Vault Credential Fetch,Credential Fetch,Vault
 Classifier: Development Status :: 4 - Beta
@@ -16,43 +16,39 @@
 License-File: Licence
 
 # Vault Credential Fetcher
 Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault.
 
 ## Install with pip
 ```bash
-$ pip install AwsVaultCredential
+$ pip install SecretManagerCredentials
 ```
 
 ## Usage
 1. Import the library.
     ```python
-   from AwsVaultCredential import VaultCredentialFetcher
+   from SecretManagerCredentials.SecretManagerFetcher import SecretManagerFetcher
     ```
 
 1. Create an instance.
     ```python 
-   vc = VaultCredentialFetcher(project_path="",
+   SM = SecretManagerFetcher(project_path="",
                                logger=<your_logger_instance>,
                                environment="",
-                               vault_region="",
-                               vault_role_id="",
                                display_vault_info=True,
                                vault_config_path="")
     ```
     Arguments (all are mandatory):
     * `project_path`: Project name, which would serve as the logger's name (*if specified*), and the prefix for log filenames.
     * `logger`: your Logger Instance
     * `"environment"`: Execution Environment
-    * `"vault_region"`: Region in which application is deployed on AWS while vault onborarding
-    * `"vault_role_id"`: Role ID/Role Name specific to your application when onboarded 
     * `"display_vault_info"`: By default it is False, used for displaying vault info
     * `"vault_config_path"`: Path where vault config is kept, relative to project path
     
 2. Get a logger and start logging.
     ```python
-   VaultCreds = vc.get_vault_cred()
+   VaultCreds = SM.get_vault_cred()
     ```
 
 ## Author
 
 **&copy; 2022, [Priyansh Gupta](priyansh.gupta@gartner.com)**.
```

### Comparing `SecretManagerCredentials-0.0.5/README.md` & `SecretManagerCredentials-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # Vault Credential Fetcher
 Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault.
 
 ## Install with pip
 ```bash
-$ pip install AwsVaultCredential
+$ pip install SecretManagerCredentials
 ```
 
 ## Usage
 1. Import the library.
     ```python
-   from AwsVaultCredential import VaultCredentialFetcher
+   from SecretManagerCredentials.SecretManagerFetcher import SecretManagerFetcher
     ```
 
 1. Create an instance.
     ```python 
-   vc = VaultCredentialFetcher(project_path="",
+   SM = SecretManagerFetcher(project_path="",
                                logger=<your_logger_instance>,
                                environment="",
-                               vault_region="",
-                               vault_role_id="",
                                display_vault_info=True,
                                vault_config_path="")
     ```
     Arguments (all are mandatory):
     * `project_path`: Project name, which would serve as the logger's name (*if specified*), and the prefix for log filenames.
     * `logger`: your Logger Instance
     * `"environment"`: Execution Environment
-    * `"vault_region"`: Region in which application is deployed on AWS while vault onborarding
-    * `"vault_role_id"`: Role ID/Role Name specific to your application when onboarded 
     * `"display_vault_info"`: By default it is False, used for displaying vault info
     * `"vault_config_path"`: Path where vault config is kept, relative to project path
     
 2. Get a logger and start logging.
     ```python
-   VaultCreds = vc.get_vault_cred()
+   VaultCreds = SM.get_vault_cred()
     ```
 
 ## Author
 
 **&copy; 2022, [Priyansh Gupta](priyansh.gupta@gartner.com)**.
```

### Comparing `SecretManagerCredentials-0.0.5/SecretManagerCredentials/SecretManagerFetcher.py` & `SecretManagerCredentials-0.0.6/SecretManagerCredentials/SecretManagerFetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             # self.logger.error(str("No such file or directory at path: 'vault_config.json'"))
             # self.logger.error("Vault path is : " + self.vault_config_path)
             print("Exception raised while loading Json File")
             raise FileNotFoundError
         else:
             return v_config
 
-    def get_vault_cred(self, host_name):
+    def get_vault_cred(self, host_name=""):
         """
         :param host_name:
         :param self
         :return:
         """
         print('inside the package get vault cred')
         try:
```

### Comparing `SecretManagerCredentials-0.0.5/SecretManagerCredentials.egg-info/PKG-INFO` & `SecretManagerCredentials-0.0.6/SecretManagerCredentials.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecretManagerCredentials
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault
 Home-page: 
 Download-URL: 
 Author: Mallikarjuna Devaraya
 License: MIT
 Keywords: Vault Credential Fetch,Credential Fetch,Vault
 Classifier: Development Status :: 4 - Beta
@@ -16,43 +16,39 @@
 License-File: Licence
 
 # Vault Credential Fetcher
 Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault.
 
 ## Install with pip
 ```bash
-$ pip install AwsVaultCredential
+$ pip install SecretManagerCredentials
 ```
 
 ## Usage
 1. Import the library.
     ```python
-   from AwsVaultCredential import VaultCredentialFetcher
+   from SecretManagerCredentials.SecretManagerFetcher import SecretManagerFetcher
     ```
 
 1. Create an instance.
     ```python 
-   vc = VaultCredentialFetcher(project_path="",
+   SM = SecretManagerFetcher(project_path="",
                                logger=<your_logger_instance>,
                                environment="",
-                               vault_region="",
-                               vault_role_id="",
                                display_vault_info=True,
                                vault_config_path="")
     ```
     Arguments (all are mandatory):
     * `project_path`: Project name, which would serve as the logger's name (*if specified*), and the prefix for log filenames.
     * `logger`: your Logger Instance
     * `"environment"`: Execution Environment
-    * `"vault_region"`: Region in which application is deployed on AWS while vault onborarding
-    * `"vault_role_id"`: Role ID/Role Name specific to your application when onboarded 
     * `"display_vault_info"`: By default it is False, used for displaying vault info
     * `"vault_config_path"`: Path where vault config is kept, relative to project path
     
 2. Get a logger and start logging.
     ```python
-   VaultCreds = vc.get_vault_cred()
+   VaultCreds = SM.get_vault_cred()
     ```
 
 ## Author
 
 **&copy; 2022, [Priyansh Gupta](priyansh.gupta@gartner.com)**.
```

### Comparing `SecretManagerCredentials-0.0.5/setup.py` & `SecretManagerCredentials-0.0.6/setup.py`

 * *Files identical despite different names*

