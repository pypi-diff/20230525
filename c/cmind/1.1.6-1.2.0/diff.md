# Comparing `tmp/cmind-1.1.6.tar.gz` & `tmp/cmind-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.1.6.tar", last modified: Tue May 16 11:03:23 2023, max compression
+gzip compressed data, was "cmind-1.2.0.tar", last modified: Thu May 25 13:53:12 2023, max compression
```

## Comparing `cmind-1.1.6.tar` & `cmind-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-16 11:03:23.020871 cmind-1.1.6/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5112 2023-05-16 11:03:10.000000 cmind-1.1.6/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41095 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3189 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    22853 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1858 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1020 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1032 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8771 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    29217 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18370 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    40730 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1207 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-16 11:03:23.020871 cmind-1.1.6/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-05-16 11:03:10.000000 cmind-1.1.6/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-25 13:53:12.221126 cmind-1.2.0/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5112 2023-05-25 12:12:27.000000 cmind-1.2.0/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-25 13:52:19.000000 cmind-1.2.0/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    46002 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    24428 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9241 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.211126 cmind-1.2.0/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1858 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-04-16 15:58:21.000000 cmind-1.2.0/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-04-05 20:14:04.000000 cmind-1.2.0/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1020 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-04-16 15:58:21.000000 cmind-1.2.0/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1032 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-04-16 15:58:21.000000 cmind-1.2.0/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8771 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    31178 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-25 13:53:12.221126 cmind-1.2.0/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-03-26 14:33:39.000000 cmind-1.2.0/setup.py
```

### Comparing `cmind-1.1.6/PKG-INFO` & `cmind-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.1.6
+Version: 1.2.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
```

### Comparing `cmind-1.1.6/README.md` & `cmind-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/artifact.py` & `cmind-1.2.0/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/automation.py` & `cmind-1.2.0/cmind/automation.py`

 * *Files 13% similar despite different names*

```diff
@@ -144,28 +144,34 @@
                                       [ (artifact alias, artifact UID) ] or
                                       [ (artifact alias, artifact UID), (artifact repo alias, artifact repo UID) ]
 
             ignore_inheritance (bool): if 'True', ignore artifact meta description inheritance 
                                        and just load meta to match UID/alias
 
 
+            (skip_index_search) (bool): If True, skip indexing
+            (force_index_add) (bool): If True, force index add (for reindexing)
+
         Returns: 
             (CM return dict):
 
             * return (int): return code == 0 if no error and >0 if error
             * (error) (str): error string if return>0
 
             * list (list): list of CM artifact objects
 
         """
 
         import copy
 
         console = i.get('out') == 'con'
 
+        skip_index_search = i.get('skip_index_search', False)
+        force_index_add = i.get('force_index_add', False)
+
         lst = []
 
         # Check tags
         tags = utils.get_list_from_cli(i, key='tags')
 
         and_tags = []
         no_tags = []
@@ -181,15 +187,15 @@
         ignore_inheritance = i.get('ignore_inheritance',False) == True
 
         # Get parsed automation
         # First object in a list is an automation
         # Second optional object in a list is a repo
         parsed_automation = i.get('parsed_automation',[])
 
-        auto_name = parsed_automation[0] if len(parsed_automation)>0 else ('','')
+        automation_name = parsed_automation[0] if len(parsed_automation)>0 else ('','')
 
         # Get parsed artifact
         parsed_artifact = i.get('parsed_artifact',[])
 
         artifact_obj = parsed_artifact[0] if len(parsed_artifact)>0 else ('','')
         artifact_repo = parsed_artifact[1] if len(parsed_artifact)>1 else None
 
@@ -219,40 +225,79 @@
                 if r['return']>0: return r
 
                 add_repo = r['match']
 
             if add_repo:
                  pruned_repos.append(repo)
 
+
+        # Check index and bypass search
+        if not skip_index_search:
+            r = self.cmind.index.find(automation_name, artifact_obj, artifact_repo, pruned_repos, and_tags, no_tags)
+            if r['return']==0:
+                artifacts = r.get('list',[])
+                if len(artifacts)>0:
+                    lst = []
+
+                    repo_extra_info = self.cmind.repos.extra_info
+
+                    for artifact in artifacts:
+                        artifact_object = Artifact(cmind = self.cmind, path = artifact['path'])
+
+                        for j in [0,1]:
+                            x = artifact['repo'][j]
+                            if x in repo_extra_info:
+                                # Add extra info to artifact about the repo
+                                artifact_object.repo_path = repo_extra_info[x].path
+                                artifact_object.repo_meta = repo_extra_info[x].meta
+
+                        r = artifact_object.load(ignore_inheritance = ignore_inheritance)
+                        if r['return']>0: return r
+
+                        lst.append(artifact_object)
+
+                        # Output to console if forced
+                        if console:
+                            print (artifact_object.path)
+
+                    return {'return':0, 'list':lst}
+        
+        
+        
+
+        
         # Iterate over pruned repositories
         for repo in pruned_repos:
             path_repo = repo.path_with_prefix
 
             repo_meta = copy.deepcopy(repo.meta)
 
-            automations = os.listdir(path_repo)
+            # May or may not be automation
+            automations = sorted(os.listdir(path_repo))
 
             for automation in automations:
                 path_automations = os.path.join(path_repo, automation)
 
                 if os.path.isdir(path_automations):
                     # Pruning by automation
                     # Will need to get first entry to get UID and alias of the automation
 
                     path_artifacts = os.path.join(path_repo, path_automations)
 
-                    artifacts = os.listdir(path_artifacts)
+                    # Potential CM artifacts or just some directories
+                    artifacts = sorted(os.listdir(path_artifacts))
 
                     # Check if artifact is first to get meta about automation UID/alias
                     first_artifact = True
 
                     for artifact in artifacts:
                         path_artifact = os.path.join(path_artifacts, artifact)
 
                         if os.path.isdir(path_artifact):
+                            
                             # Check if has CM meta to make sure that it's a CM object
                             path_artifact_meta = os.path.join(path_artifact, self.cmind.cfg['file_cmeta'])
 
                             r = utils.is_file_json_or_yaml(file_name = path_artifact_meta)
                             if r['return']>0: return r
 
                             if r['is_file']:
@@ -262,14 +307,15 @@
                                 # Add extra info to artifact about the repo
                                 artifact_object.repo_path = path_repo
                                 artifact_object.repo_meta = repo_meta
 
                                 # Force no inheritance if first artifact just to check automation UID and alias
                                 tmp_ignore_inheritance = True if first_artifact else ignore_inheritance
 
+                                # Force no inheritance to get basic info about aliases and UIDs
                                 r = artifact_object.load(ignore_inheritance = tmp_ignore_inheritance)
                                 if r['return']>0: return r
 
                                 # Check permanent meta
                                 meta = artifact_object.meta
 
                                 uid = meta.get('uid', '')
@@ -278,16 +324,16 @@
                                 alias = meta.get('alias', '')
                                 if alias==None: alias = ''
 
                                 if first_artifact:
                                     # Need to check if automation matches
                                     r = utils.match_objects(uid = meta.get('automation_uid'), 
                                                             alias = meta.get('automation_alias'),
-                                                            uid2 = auto_name[1],
-                                                            alias2 = auto_name[0],
+                                                            uid2 = automation_name[1],
+                                                            alias2 = automation_name[0],
                                                             more_strict = True)
                                     if r['return']>0: return r
 
                                     if not r['match']:
                                         break
 
                                 # Match object
@@ -300,39 +346,36 @@
 
                                 if r['match']:
                                     # Reload object with inheritance if needed before checking tags
                                     if first_artifact:
                                         r = artifact_object.load(ignore_inheritance = ignore_inheritance)
                                         if r['return']>0: return r
 
-                                    tags_in_meta = meta.get('tags',[])
+                                    meta = artifact_object.meta
 
-                                    if len(and_tags)>0:
-                                        if not all(t in tags_in_meta for t in and_tags):
-                                            continue
-
-                                    if len(no_tags)>0:
-                                        skip = False
-                                        for t in no_tags:
-                                            if t in tags_in_meta:
-                                                skip = True
-                                                break
-                                        if skip:
-                                            continue
+                                    # Index
+                                    if self.cmind.use_index or force_index_add:
+                                        r=self.cmind.index.add(meta, path_artifact, 
+                                                                     (repo.meta['alias'], 
+                                                                      repo.meta['uid']))
+                                        # Ignore index output to continue working if issues
+
+                                    # Check if tags match
+                                    if not utils.tags_matched(meta.get('tags',[]), and_tags, no_tags):
+                                        continue
 
                                     lst.append(artifact_object)
 
                                     # Output to console if forced
                                     if console:
                                         print (artifact_object.path)
 
                                 if first_artifact:
                                     first_artifact = False
 
-
         return {'return':0, 'list':lst}
 
 
     ############################################################
     def add(self, i):
         """
         Add CM artifact
@@ -370,15 +413,15 @@
 
         # Get parsed automation
         if 'parsed_automation' not in i:
            return {'return':1, 'error':'automation is not specified'}
 
         parsed_automation = i.get('parsed_automation',[])
 
-        auto_name = parsed_automation[0] if len(parsed_automation)>0 else ('','')
+        automation_name = parsed_automation[0] if len(parsed_automation)>0 else ('','')
 
         # Get parsed artifact
         parsed_artifact = i.get('parsed_artifact',[])
 
         artifact_obj = parsed_artifact[0] if len(parsed_artifact)>0 else ('','')
         artifact_repo = parsed_artifact[1] if len(parsed_artifact)>1 else None
 
@@ -402,15 +445,15 @@
             return {'return':1, 'error':'more than 1 repository found (ambiguity)'}
 
         repo = lst[0]
 
         repo_path = repo.path_with_prefix
 
         # Check automation (if exists)
-        automation_path = os.path.join(repo_path, auto_name[0]) if auto_name[0]!='' else os.path.join(repo_path, auto_name[1])
+        automation_path = os.path.join(repo_path, automation_name[0]) if automation_name[0]!='' else os.path.join(repo_path, automation_name[1])
 
         if not os.path.isdir(automation_path):
             os.makedirs(automation_path)
 
         # Check object UID
         if artifact_obj[1]=='' or artifact_obj[1] is None:
             r=utils.gen_uid()
@@ -432,29 +475,37 @@
 
         # Prepare meta
         meta = i.get('meta',{})
         tags = utils.get_list_from_cli(i, key='tags')
 
         if meta.get('alias','')=='': meta['alias']=artifact_obj[0]
         if meta.get('uid','')=='': meta['uid']=artifact_obj[1]
-        if meta.get('automation_alias','')=='': meta['automation_alias']=auto_name[0]
-        if meta.get('automation_uid','')=='': meta['automation_uid']=auto_name[1]
+        if meta.get('automation_alias','')=='': meta['automation_alias']=automation_name[0]
+        if meta.get('automation_uid','')=='': meta['automation_uid']=automation_name[1]
 
         existing_tags = meta.get('tags',[])
         if len(tags)>0: 
             existing_tags += tags
         meta['tags'] = utils.filter_tags(existing_tags)
 
         # Record meta
         if i.get('yaml', False):
             r = utils.save_yaml(meta_path_yaml, meta=meta)
         else:
             r = utils.save_json(meta_path_json, meta=meta)
         if r['return']>0: return r
 
+        # Index
+        if self.cmind.use_index:
+            r=self.cmind.index.add(meta, obj_path, 
+                                   (repo.meta['alias'], repo.meta['uid']),
+                                   update = True)
+            # Ignore index output to continue working if issues
+
+        
         if console:
             print ('Added CM object at {}'.format(obj_path))
 
         return {'return':0, 'meta':meta, 'path':obj_path}
 
     ############################################################
     def delete(self, i):
@@ -533,14 +584,21 @@
 
             if os.name == 'nt':
                 # To be able to remove .git files
                 shutil.rmtree(path_to_artifact, ignore_errors = False, onerror = delete_helper)
             else:
                 shutil.rmtree(path_to_artifact)
 
+            # Index
+            if self.cmind.use_index:
+                r=self.cmind.index.add(artifact.meta, artifact.path, 
+                                       (artifact.repo_meta['alias'], artifact.repo_meta['uid']),
+                                       update = True, delete = True)
+                # Ignore index output to continue working if issues
+            
             if console:
                 print ('    Deleted!')
 
         return {'return':0, 'deleted_list':deleted_lst}
 
     ############################################################
     def load(self, i):
@@ -704,14 +762,21 @@
             if len(tags)>0:
                 for t in tags:
                     if t not in meta_tags:
                         meta_tags.append(t)
 
             r = artifact.update(meta, replace = replace, append_lists = not replace_lists, tags = meta_tags)
 
+            # Index
+            if self.cmind.use_index:
+                r=self.cmind.index.add(artifact.meta, artifact.path, 
+                                       (artifact.repo_meta['alias'], artifact.repo_meta['uid']),
+                                       update = True)
+                # Ignore index output to continue working if issues
+
             # Output if console
             if console:
                 print ('Updated {}'.format(artifact.path))
 
         return {'return':0, 'list':lst}
 
     ############################################################
@@ -771,14 +836,15 @@
 
         target_artifact_obj = target_artifact[0]
         target_artifact_obj_alias = target_artifact_obj[0]
         target_artifact_obj_uid = target_artifact_obj[1].lower()
 
         # Check target repo
         target_artifact_repo = target_artifact[1] if len(target_artifact)>1 else None
+        target_artifact_repo_obj = None
 
         target_repo_path = None
 
         if target_artifact_repo is not None:
             r = self.cmind.access({'action':'search',
                                    'automation':'repo',
                                    'artifact': utils.assemble_cm_object2(target_artifact_repo)})
@@ -787,19 +853,27 @@
             target_repo_list = r['list']
 
             if len(target_repo_list) == 0:
                 return {'return':1, 'error':'target repo "{}" not found'.format(target_artifact_repo)}
             elif len(target_repo_list) >1:
                 return {'return':1, 'error':'more than 1 target repo found "{}"'.format(target_artifact_repo)}
 
-            target_repo_path = os.path.abspath(target_repo_list[0].path_with_prefix)
+            target_artifact_repo_obj = target_repo_list[0]
+            target_repo_path = os.path.abspath(target_artifact_repo_obj.path_with_prefix)
 
         # Updating artifacts
         for artifact in lst:
 
+            # Index
+            if self.cmind.use_index:
+                r=self.cmind.index.add(artifact.meta, artifact.path, 
+                                       (artifact.repo_meta['alias'], artifact.repo_meta['uid']),
+                                       update = True, delete = True)
+                # Ignore index output to continue working if issues
+
             artifact_path = os.path.abspath(artifact.path)
 
             artifact_meta = artifact.original_meta
 
             artifact_alias = artifact_meta.get('alias','')
             artifact_uid = artifact_meta.get('uid','')
 
@@ -855,14 +929,27 @@
                     r = utils.update_yaml(meta_path_yaml, update_meta)
                     if r['return']>0: return r
 
                 else:
                     r = artifact.update({})
                     if r['return'] >0: return r
 
+            # Index
+            if self.cmind.use_index:
+                if target_artifact_repo_obj is not None:
+                    tmp_repo_index = (target_artifact_repo_obj.meta['alias'], 
+                                      target_artifact_repo_obj.meta['uid'])
+                else:
+                   tmp_repo_index = (artifact.repo_meta['alias'], 
+                                     artifact.repo_meta['uid'])
+                
+                r=self.cmind.index.add(artifact.meta, artifact.path, 
+                                       tmp_repo_index, update = True)
+                # Ignore index output to continue working if issues
+
         return {'return':0, 'list':lst}
 
     ############################################################
     def copy(self, i):
         """
         Copy CM artifact(s) either to a new artifact or to a new repository
 
@@ -918,32 +1005,33 @@
 
         target_artifact_obj = target_artifact[0]
         target_artifact_obj_alias = target_artifact_obj[0]
         target_artifact_obj_uid = target_artifact_obj[1].lower()
 
         # Check target repo
         target_artifact_repo = target_artifact[1] if len(target_artifact)>1 else None
+        target_artifact_repo_obj = None
 
         target_repo_path = None
 
         if target_artifact_repo is not None:
-            print (target_artifact_repo)
             r = self.cmind.access({'action':'search',
                                    'automation':'repo',
                                    'artifact': utils.assemble_cm_object2(target_artifact_repo)})
             if r['return']>0: return r
 
             target_repo_list = r['list']
 
             if len(target_repo_list) == 0:
                 return {'return':1, 'error':'target repo "{}" not found'.format(target_artifact_repo)}
             elif len(target_repo_list) >1:
                 return {'return':1, 'error':'more than 1 target repo found "{}"'.format(target_artifact_repo)}
 
-            target_repo_path = os.path.abspath(target_repo_list[0].path_with_prefix)
+            target_artifact_repo_obj = target_repo_list[0]
+            target_repo_path = os.path.abspath(target_artifact_repo_obj.path_with_prefix)
 
         # Updating artifacts
         for artifact in lst:
 
             artifact_path = os.path.abspath(artifact.path)
 
             artifact_meta = artifact.original_meta
@@ -988,25 +1076,41 @@
             # Update meta
             if console:
                 print ('- Updating meta in "{}"'.format(new_artifact_path))
 
             # If only yaml, update yaml and not json
             meta_path_yaml = os.path.join(new_artifact_path, self.cmind.cfg['file_cmeta']+'.yaml')
             meta_path_json = os.path.join(new_artifact_path, self.cmind.cfg['file_cmeta']+'.json')
+
             if os.path.isfile(meta_path_yaml) and not os.path.isfile(meta_path_json):
                 update_meta={'alias':artifact_meta['alias'],
                              'uid':artifact_meta['uid']}
                 
                 r = utils.update_yaml(meta_path_yaml, update_meta)
                 if r['return']>0: return r
 
             else:
                 r = artifact.update({})
                 if r['return'] >0: return r
 
+            # Index added artifact
+            if self.cmind.use_index:
+                # Old
+                if target_artifact_repo_obj is not None:
+                    tmp_repo_index = (target_artifact_repo_obj.meta['alias'], 
+                                      target_artifact_repo_obj.meta['uid'])                    
+                else:
+                    tmp_repo_index = (artifact.repo_meta['alias'], 
+                                      artifact.repo_meta['uid'])
+                                      
+                r=self.cmind.index.add(artifact.meta, artifact.path, 
+                                       tmp_repo_index, update = True)
+                # Ignore index output to continue working if issues
+
+
         return {'return':0, 'list':lst}
 
     ############################################################
     def info(self, i):
         """
         Get info about artifacts
```

### Comparing `cmind-1.1.6/cmind/cli.py` & `cmind-1.2.0/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/config.py` & `cmind-1.2.0/cmind/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.cfg = {
                      "name": "cm",
 
                      "env_home": "CM_HOME",
                      "env_repos": "CM_REPOS",
                      "env_debug": "CM_DEBUG",
                      "env_config": "CM_CONFIG",
+                     "env_index": "CM_INDEX",
 
                      "flag_debug": "cm-debug",
 
                      "flag_help": "h",
                      "flag_help2": "help",
 
                      "error_prefix": "CM error:",
@@ -38,14 +39,16 @@
 
                      "default_home_dir": "CM",
 
                      "file_repos": "repos.json",
                      "dir_repos": "repos",
                      "cmind_repo": "repo",
 
+                     "file_index": "index.json",
+
                      "file_meta_repo": "cmr",
 
                      "common_automation_module_name": "module",
 
                      "action_substitutions": {
                        "ls":"search",
                        "list":"search",
```

### Comparing `cmind-1.1.6/cmind/core.py` & `cmind-1.2.0/cmind/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Collective Mind core functions
 
 from cmind.config import Config
 from cmind.repos import Repos
+from cmind.index import Index
 from cmind.automation import Automation
 from cmind import utils
 
 import sys
 import os
 import imp
 import importlib
 import pkgutil
 import inspect
+import logging
 
 cm = None
 
 ############################################################
 class CM(object):
     """
     Main CM class
@@ -51,15 +53,15 @@
         """
 
         # Initialize and update CM configuration
         self.cfg = Config().cfg
 
         # Check if debug (raise error instead of soft error)
         self.debug = False
-        if debug or os.environ.get(self.cfg['env_debug'],'').strip().lower()=='yes':
+        if debug or os.environ.get(self.cfg['env_debug'],'').strip().lower() in ['yes','on','true']:
             self.debug = True
 
         # Explicit path to direcory with CM repositories and other internals
         self.repos_path = repos_path
         if self.repos_path == '':
             s = os.environ.get(self.cfg['env_repos'],'').strip()
             if s != '':
@@ -90,14 +92,25 @@
 
         # Check Python version
         self.python_version = list(sys.version_info)
 
         # Save output to json (only from CLI)
         self.save_to_json = ''
 
+        # Logging
+        self.logger = None
+        self.log = []
+
+        # Index
+        self.index = None
+
+        self.use_index = False
+        if os.environ.get(self.cfg['env_index'],'').strip().lower() in ['yes','on','true']:
+            self.use_index = True
+
     ############################################################
     def error(self, r):
         """
         If r['return']>0: print CM error and raise error if in debugging mode
 
         Args:
            r (dict): output from CM function with "return" and "error"
@@ -131,14 +144,29 @@
 
         # Force console
         self.error(r)
 
         sys.exit(r['return'])
 
     ############################################################
+    def log(self, s):
+        """
+        Args:
+           s (string): log string
+
+        Returns:
+           None
+        """
+
+        # Force console
+        print (s)
+
+        return
+
+    ############################################################
     def access(self, i, out = None):
         """
         Access CM automation actions in a unified way similar to micro-services.
 
         i (dict | str | argv): unified CM input
 
         Args:
@@ -170,14 +198,18 @@
            i = {}
 
         # Attempt to detect debug flag early (though suggest to use environment)
         # If error in parse_cli, it will raise error
         if self.cfg['flag_debug'] in i:
             self.debug = True
 
+        # Check if log
+        if self.logger is None:
+            self.logger = logging.getLogger("cm")
+
         # Parse as command line if string or list
         if type(i) == str or type(i) == list:
             import cmind.cli
 
             r = cmind.cli.parse(i)
             if r['return'] >0 : return r
 
@@ -240,14 +272,31 @@
 
             r = repos.load()
             if r['return'] >0 : return r
 
             # Set only after all initializations
             self.repos = repos
 
+        # Load index
+        if self.index is None:
+            self.index = Index(self.repos_path, self.cfg)
+
+            if self.use_index:
+                r = self.index.load()
+                if r['return']>0: return r
+
+                if not r['exists']:
+                    # First time
+                    if console:
+                        print ('Warning: CM index is used for the first time. CM will reindex all artifacts now - it may take some time ...')
+
+                    r = self.access({'action':'reindex',
+                                     'automation':'repo,55c3e27e8a140e48'})
+                    if r['return']>0: return r
+
         # Check if forced common automation
         use_common_automation = True if i.get('common',False) else False
 
         automation_lst = []
         use_any_action = False
 
         artifact = i.get('artifact','').strip()
@@ -488,14 +537,21 @@
             i['parsed_artifact'] = r['cm_object']
 
         # Call automation action
         action_addr=getattr(initialized_automation, action)
 
         r = action_addr(i)
 
+        # Check if need to save index
+        if self.use_index and self.index.updated:
+            rx = self.index.save()
+            # Ignore output for now to continue working even if issues ...
+
+            self.index.updated=False
+
         return r
 
 ############################################################
 def parse_cm_object_and_check_current_dir(cmind, artifact):
     """
     Internal function: parses CM object and check if there is '.' 
     to detect CM repository in a current directory.
```

### Comparing `cmind-1.1.6/cmind/net.py` & `cmind-1.2.0/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/automation/README.md` & `cmind-1.2.0/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/automation/module.py` & `cmind-1.2.0/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.2.0/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/automation/module_misc.py` & `cmind-1.2.0/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/ck/README.md` & `cmind-1.2.0/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/ck/module.py` & `cmind-1.2.0/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/core/README.md` & `cmind-1.2.0/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/core/module.py` & `cmind-1.2.0/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/repo/README.md` & `cmind-1.2.0/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repo/automation/repo/module.py` & `cmind-1.2.0/cmind/repo/automation/repo/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,19 @@
         repos = self.cmind.repos
 
         r = repos.pull(alias = alias, url = url, branch = branch, checkout = checkout, console = console, desc=desc, prefix=prefix)
         if r['return']>0: return r
 
         repo_meta = r['meta']
 
+        if self.cmind.use_index:
+            ii = {'out':'con'} if console else {}
+            rx = self.reindex(ii)
+
+
         return {'return':0, 'meta':repo_meta}
 
     ############################################################
     def search(self, i):
         """
         List registered CM repos.
 
@@ -253,14 +258,18 @@
         if len(lst)==0:
            return {'return':1, 'error':'Repository not found'}
 
         remove_all = i.get('all', '')
 
         r = self.cmind.repos.delete(lst, remove_all = remove_all, console = console, force = force)
 
+        if self.cmind.use_index:
+            ii = {'out':'con'} if console else {}
+            rx = self.reindex(ii)
+        
         return r
 
     ############################################################
     def init(self, i):
         """
         Initialize CM repository.
 
@@ -372,14 +381,19 @@
             lst=r['list']
 
             if len(lst)>0: 
                 return {'return':1, 'error':'Repository "{}" is already registered in CM'.format(repo_artifact)}
 
         # Create repository 
         r = self.cmind.repos.init(alias = alias, uid = uid, path = path, console = console, desc=desc, prefix=prefix, only_register=repo_desc_found)
+
+        if self.cmind.use_index:
+            ii = {'out':'con'} if console else {}
+            rx = self.reindex(ii)
+        
         return r
 
     ############################################################
     def add(self, i):
         """
         The same as "init".
         """
@@ -553,14 +567,18 @@
                     file_out = open(file_path, 'wb')
                     file_out.write(repo_pack_zip.read(f))
                     file_out.close()
 
         repo_pack_zip.close()
         repo_pack_file.close()
 
+        if self.cmind.use_index:
+            ii = {'out':'con'} if console else {}
+            rx = self.reindex(ii)
+        
         return r_new
 
     ##############################################################################
     def import_ck_to_cm(self, i):
         """
         Convert all legacy CK repositories to CM repositories
 
@@ -840,17 +858,72 @@
                     print ('')
                     print ('Current directory has a CM artifact:')
 
                     print ('')
                     print ('  Artifact alias: {}'.format(artifact_meta['alias']))
                     print ('  Artifact UID:   {}'.format(artifact_meta['uid']))
 
+        if self.cmind.use_index:
+            ii = {'out':'con'} if console else {}
+            rx = self.reindex(ii)
+
         return rr
 
 
+    ############################################################
+    def reindex(self, i):
+        """
+        Reindex all CM repositories
+
+        Args:
+            (CM input dict)
+
+            (verbose) (bool): If True, print index
+
+        Returns: 
+            (CM return dict):
+
+            * return (int): return code == 0 if no error and >0 if error
+            * (error) (str): error string if return>0
+
+        """
+
+        verbose = i.get('verbose', False)
+
+        console = i.get('out') == 'con'
+
+        if console:
+            print ('')
+            print ('Reindexing all CM artifacts. Can take some time ...')
+        
+        out = 'con' if verbose else ''
+        
+        # Clean index
+        self.cmind.index.meta = {}
+        
+        r = self.cmind.access({'action':'search',
+                               'automation':'*',
+                               'out':out,
+                               'skip_index_search':True,
+                               'force_index_add':True})
+        if r['return']>0: return r
+
+        # Save
+
+        rx = self.cmind.index.save()
+        # Ignore output for now to continue working even if issues ...
+
+        if self.cmind.use_index:
+            rx = self.cmind.index.load()
+            # Ignore output for now to continue working even if issues ...
+
+
+        return {'return':0}
+
+
 
 ##############################################################################
 def convert_ck_dir_to_cm(rpath):
     """
     Convert CK directory to the CM format (internal function).
 
     Args:
```

### Comparing `cmind-1.1.6/cmind/repo.py` & `cmind-1.2.0/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.6/cmind/repos.py` & `cmind-1.2.0/cmind/repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         self.lst = []
 
         # Potential path to internal repo
         self.path_to_internal_repo = path_to_internal_repo
 
         self.full_path_to_repo_paths = ''
 
+        self.extra_info = {}
+
     ############################################################
     def load(self, init = False):
         """
         Load or initialize repos.json file with repositories
 
         Args:
             init (bool): if False do not init individual CM repositories
@@ -124,14 +126,22 @@
                     repo = Repo(full_path_to_repo, self.cfg)
 
                     r = repo.load()
                     if r['return']>0: return r
 
                     # Set only after all initializations
                     self.lst.append(repo)
+                   
+                    repo_uid = repo.meta['uid']
+                    if repo_uid!='':
+                        self.extra_info[repo_uid]=repo
+
+                    repo_alias = repo.meta['alias']
+                    if repo_alias!='':
+                        self.extra_info[repo_alias]=repo
 
                     found = True
                     break
 
             # Repo path exists but repo itself doesn't exist - fail
             if not found:
                 return {'return':1, 'error': 'repository path {} not found (check file {})'.format(path_to_repo, full_path_to_repo_paths)}
```

### Comparing `cmind-1.1.6/cmind/utils.py` & `cmind-1.2.0/cmind/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1556,7 +1556,36 @@
     tmp_module=importlib.import_module(module_name)
 
     del(sys.path[0])
 
     i['self_module'] = module_self
     
     return getattr(tmp_module, module_func)(i)
+
+###########################################################################
+def tags_matched(tags, and_tags, no_tags):
+    """
+    Check if AND tags and NO tags match tags
+
+    Args:    
+        tags (list of str): full list of tags
+        and_tags (list of str): list of AND tags
+        no_tags (list of str): list of NO tags
+
+    Returns:
+        True if tags matched
+
+    """
+
+    matched = True
+    
+    if len(and_tags)>0:
+        if not all(t in tags for t in and_tags):
+            matched = False
+
+    if matched and len(no_tags)>0:
+        for t in no_tags:
+            if t in tags:
+                matched = False
+                break
+
+    return matched
```

### Comparing `cmind-1.1.6/cmind.egg-info/PKG-INFO` & `cmind-1.2.0/cmind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.1.6
+Version: 1.2.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
```

### Comparing `cmind-1.1.6/cmind.egg-info/SOURCES.txt` & `cmind-1.2.0/cmind.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 cmind/__init__.py
 cmind/__main__.py
 cmind/artifact.py
 cmind/automation.py
 cmind/cli.py
 cmind/config.py
 cmind/core.py
+cmind/index.py
 cmind/net.py
 cmind/repo.py
 cmind/repos.py
 cmind/utils.py
 cmind.egg-info/PKG-INFO
 cmind.egg-info/SOURCES.txt
 cmind.egg-info/dependency_links.txt
```

### Comparing `cmind-1.1.6/setup.py` & `cmind-1.2.0/setup.py`

 * *Files identical despite different names*

