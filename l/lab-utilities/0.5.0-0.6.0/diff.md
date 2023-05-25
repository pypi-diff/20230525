# Comparing `tmp/lab_utilities-0.5.0.tar.gz` & `tmp/lab_utilities-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab_utilities-0.5.0.tar", last modified: Tue Apr 11 15:21:21 2023, max compression
+gzip compressed data, was "lab_utilities-0.6.0.tar", last modified: Thu May 25 13:03:56 2023, max compression
```

## Comparing `lab_utilities-0.5.0.tar` & `lab_utilities-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:21:21.389198 lab_utilities-0.5.0/
--rw-rw-rw-   0        0        0     1090 2023-03-21 13:38:58.000000 lab_utilities-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      262 2023-04-11 15:21:21.388291 lab_utilities-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-03-28 19:34:28.000000 lab_utilities-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 15:21:21.379721 lab_utilities-0.5.0/lab_utilities/
--rw-rw-rw-   0        0        0      425 2023-04-02 02:08:29.000000 lab_utilities-0.5.0/lab_utilities/__init__.py
--rw-rw-rw-   0        0        0     1603 2023-04-08 15:30:57.000000 lab_utilities-0.5.0/lab_utilities/email.py
--rw-rw-rw-   0        0        0     1573 2023-04-02 01:22:36.000000 lab_utilities-0.5.0/lab_utilities/equipment_config.py
--rw-rw-rw-   0        0        0     4838 2023-04-02 02:39:22.000000 lab_utilities-0.5.0/lab_utilities/experimental_data_repository.py
--rw-rw-rw-   0        0        0     1547 2023-04-02 02:22:30.000000 lab_utilities-0.5.0/lab_utilities/lab_git.py
--rw-rw-rw-   0        0        0      386 2023-03-22 13:48:15.000000 lab_utilities-0.5.0/lab_utilities/make_directory.py
--rw-rw-rw-   0        0        0      850 2022-12-05 04:45:30.000000 lab_utilities-0.5.0/lab_utilities/manifest_time_estimator.py
--rw-rw-rw-   0        0        0     2176 2023-03-25 00:32:51.000000 lab_utilities-0.5.0/lab_utilities/package_to_text.py
--rw-rw-rw-   0        0        0      896 2023-03-27 23:12:39.000000 lab_utilities-0.5.0/lab_utilities/threading_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:21:21.387205 lab_utilities-0.5.0/lab_utilities.egg-info/
--rw-rw-rw-   0        0        0      262 2023-04-11 15:21:21.000000 lab_utilities-0.5.0/lab_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-04-11 15:21:21.000000 lab_utilities-0.5.0/lab_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:21:21.000000 lab_utilities-0.5.0/lab_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-11 15:21:21.000000 lab_utilities-0.5.0/lab_utilities.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 15:21:21.000000 lab_utilities-0.5.0/lab_utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 15:21:21.390195 lab_utilities-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-03-27 23:30:46.000000 lab_utilities-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:03:56.901147 lab_utilities-0.6.0/
+-rw-rw-rw-   0        0        0     1090 2023-03-21 13:38:58.000000 lab_utilities-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      262 2023-05-25 13:03:56.901147 lab_utilities-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1958 2023-04-21 15:05:21.000000 lab_utilities-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:03:56.889813 lab_utilities-0.6.0/lab_utilities/
+-rw-rw-rw-   0        0        0      425 2023-04-02 02:08:29.000000 lab_utilities-0.6.0/lab_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1603 2023-04-08 15:30:57.000000 lab_utilities-0.6.0/lab_utilities/email.py
+-rw-rw-rw-   0        0        0     1573 2023-05-05 05:03:59.000000 lab_utilities-0.6.0/lab_utilities/equipment_config.py
+-rw-rw-rw-   0        0        0     4880 2023-05-04 21:30:58.000000 lab_utilities-0.6.0/lab_utilities/experimental_data_repository.py
+-rw-rw-rw-   0        0        0     1547 2023-04-02 02:22:30.000000 lab_utilities-0.6.0/lab_utilities/lab_git.py
+-rw-rw-rw-   0        0        0      386 2023-03-22 13:48:15.000000 lab_utilities-0.6.0/lab_utilities/make_directory.py
+-rw-rw-rw-   0        0        0      850 2022-12-05 04:45:30.000000 lab_utilities-0.6.0/lab_utilities/manifest_time_estimator.py
+-rw-rw-rw-   0        0        0     2176 2023-03-25 00:32:51.000000 lab_utilities-0.6.0/lab_utilities/package_to_text.py
+-rw-rw-rw-   0        0        0      896 2023-03-27 23:12:39.000000 lab_utilities-0.6.0/lab_utilities/threading_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:03:56.900151 lab_utilities-0.6.0/lab_utilities.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-25 13:03:56.000000 lab_utilities-0.6.0/lab_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-05-25 13:03:56.000000 lab_utilities-0.6.0/lab_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:03:56.000000 lab_utilities-0.6.0/lab_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-25 13:03:56.000000 lab_utilities-0.6.0/lab_utilities.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 13:03:56.000000 lab_utilities-0.6.0/lab_utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 13:03:56.902220 lab_utilities-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-05-25 13:01:24.000000 lab_utilities-0.6.0/setup.py
```

### Comparing `lab_utilities-0.5.0/LICENSE` & `lab_utilities-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/lab_utilities/email.py` & `lab_utilities-0.6.0/lab_utilities/email.py`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/lab_utilities/equipment_config.py` & `lab_utilities-0.6.0/lab_utilities/equipment_config.py`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/lab_utilities/experimental_data_repository.py` & `lab_utilities-0.6.0/lab_utilities/experimental_data_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         
         with open(self.experiment_fields, 'r') as f:
             prompts = json.load(f)
 
         for prompt in prompts:
             parameter = input(prompt['prompt'] + ': ')
             if parameter:
-                experimental_params_dict.update({prompt['field']: parameter})
+                experimental_params_dict.update({prompt['field']: int(parameter)})
             else:
                 try:
                     experimental_params_dict.update({prompt['field']: prompt['default']})
                 except KeyError:
                     raise Exception("No default setting for this field")
         
         self.experimental_params = experimental_params_dict
@@ -109,14 +109,15 @@
         if not os.path.exists(experiment_dir):
             os.makedirs(experiment_dir, exist_ok=True) 
             
         return experiment_dir
     
     def get_user_email(self, user):
         emails_json = os.path.join(self.data_repository, 'user_emails.json')
+        print(self.data_repository)
         with open(emails_json, 'r') as fp:
             emails = json.load(fp)
         user_email = emails[user]
         return user_email
     
     def get_experimental_params(self):
         return self.experimental_params
```

### Comparing `lab_utilities-0.5.0/lab_utilities/lab_git.py` & `lab_utilities-0.6.0/lab_utilities/lab_git.py`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/lab_utilities/manifest_time_estimator.py` & `lab_utilities-0.6.0/lab_utilities/manifest_time_estimator.py`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/lab_utilities/package_to_text.py` & `lab_utilities-0.6.0/lab_utilities/package_to_text.py`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/lab_utilities/threading_utilities.py` & `lab_utilities-0.6.0/lab_utilities/threading_utilities.py`

 * *Files identical despite different names*

### Comparing `lab_utilities-0.5.0/setup.py` & `lab_utilities-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 @author: stefa
 """
 from setuptools import setup, find_packages
 
 setup(
     name='lab_utilities',
-    version='0.5.0',
+    version='0.6.0',
     packages=find_packages(),
     license='MIT',
     description='Lab Utilities',
     long_description='Nothing here yet',
     install_requires=[],
     url='https://github.com/stefangolas/lab_utilities.git',
     author='Stefan Golas',
```

