# Comparing `tmp/cltl.combot-0.0.dev1.tar.gz` & `tmp/cltl.combot-1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltl.combot-0.0.dev1.tar", last modified: Mon Dec 13 08:11:26 2021, max compression
+gzip compressed data, was "cltl.combot-1.0.dev0.tar", last modified: Thu May 25 12:46:02 2023, max compression
```

## Comparing `cltl.combot-0.0.dev1.tar` & `cltl.combot-1.0.dev0.tar`

### file list

```diff
@@ -1,40 +1,68 @@
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.903544 cltl.combot-0.0.dev1/
--rw-r--r--   0 tkb        (501) staff       (20)     1060 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/LICENCE
--rw-r--r--   0 tkb        (501) staff       (20)     2001 2021-12-13 08:11:26.903114 cltl.combot-0.0.dev1/PKG-INFO
--rw-r--r--   0 tkb        (501) staff       (20)     1661 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/README.md
--rw-r--r--   0 tkb        (501) staff       (20)        9 2021-12-13 08:11:16.000000 cltl.combot-0.0.dev1/VERSION
--rw-r--r--   0 tkb        (501) staff       (20)       38 2021-12-13 08:11:26.903671 cltl.combot-0.0.dev1/setup.cfg
--rw-r--r--   0 tkb        (501) staff       (20)      789 2021-12-09 12:00:13.000000 cltl.combot-0.0.dev1/setup.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.886317 cltl.combot-0.0.dev1/src/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.886433 cltl.combot-0.0.dev1/src/cltl/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.890875 cltl.combot-0.0.dev1/src/cltl/combot/
--rw-r--r--   0 tkb        (501) staff       (20)     3482 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/__init__.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.892542 cltl.combot-0.0.dev1/src/cltl/combot/infra/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/__init__.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.895106 cltl.combot-0.0.dev1/src/cltl/combot/infra/config/
--rw-r--r--   0 tkb        (501) staff       (20)       76 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/config/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     6774 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/config/api.py
--rw-r--r--   0 tkb        (501) staff       (20)     1663 2021-12-09 12:00:40.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/config/k8config.py
--rw-r--r--   0 tkb        (501) staff       (20)     3440 2021-12-09 12:02:39.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/config/local.py
--rw-r--r--   0 tkb        (501) staff       (20)     2159 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/di_container.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.899198 cltl.combot-0.0.dev1/src/cltl/combot/infra/event/
--rw-r--r--   0 tkb        (501) staff       (20)       78 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/event/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     2254 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/event/api.py
--rw-r--r--   0 tkb        (501) staff       (20)     5385 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/event/kombu.py
--rw-r--r--   0 tkb        (501) staff       (20)     1929 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/event/memory.py
--rw-r--r--   0 tkb        (501) staff       (20)      122 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/event/util.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.901202 cltl.combot-0.0.dev1/src/cltl/combot/infra/resource/
--rw-r--r--   0 tkb        (501) staff       (20)      105 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/resource/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     9031 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/resource/api.py
--rw-r--r--   0 tkb        (501) staff       (20)    11878 2021-12-09 12:01:43.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/resource/threaded.py
--rw-r--r--   0 tkb        (501) staff       (20)     5423 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/topic_worker.py
--rw-r--r--   0 tkb        (501) staff       (20)     1993 2021-11-05 10:32:01.000000 cltl.combot-0.0.dev1/src/cltl/combot/infra/util.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.902262 cltl.combot-0.0.dev1/src/cltl/combot/test/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/test/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)      961 2021-09-23 06:24:17.000000 cltl.combot-0.0.dev1/src/cltl/combot/test/util.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 08:11:26.890603 cltl.combot-0.0.dev1/src/cltl.combot.egg-info/
--rw-r--r--   0 tkb        (501) staff       (20)     2001 2021-12-13 08:11:26.000000 cltl.combot-0.0.dev1/src/cltl.combot.egg-info/PKG-INFO
--rw-r--r--   0 tkb        (501) staff       (20)      924 2021-12-13 08:11:26.000000 cltl.combot-0.0.dev1/src/cltl.combot.egg-info/SOURCES.txt
--rw-r--r--   0 tkb        (501) staff       (20)        1 2021-12-13 08:11:26.000000 cltl.combot-0.0.dev1/src/cltl.combot.egg-info/dependency_links.txt
--rw-r--r--   0 tkb        (501) staff       (20)       18 2021-12-13 08:11:26.000000 cltl.combot-0.0.dev1/src/cltl.combot.egg-info/requires.txt
--rw-r--r--   0 tkb        (501) staff       (20)        5 2021-12-13 08:11:26.000000 cltl.combot-0.0.dev1/src/cltl.combot.egg-info/top_level.txt
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.405907 cltl.combot-1.0.dev0/
+-rw-r--r--   0 sbaez      (501) staff       (20)     1060 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/LICENCE
+-rw-r--r--   0 sbaez      (501) staff       (20)     9712 2023-05-25 12:46:02.405732 cltl.combot-1.0.dev0/PKG-INFO
+-rw-r--r--   0 sbaez      (501) staff       (20)     9392 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/README.md
+-rw-r--r--   0 sbaez      (501) staff       (20)        9 2023-05-25 12:45:51.000000 cltl.combot-1.0.dev0/VERSION
+-rw-r--r--   0 sbaez      (501) staff       (20)       38 2023-05-25 12:46:02.405946 cltl.combot-1.0.dev0/setup.cfg
+-rw-r--r--   0 sbaez      (501) staff       (20)      886 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/setup.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.397668 cltl.combot-1.0.dev0/src/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.397545 cltl.combot-1.0.dev0/src/cltl/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.399109 cltl.combot-1.0.dev0/src/cltl/combot/
+-rw-r--r--   0 sbaez      (501) staff       (20)     3482 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/__init__.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.399723 cltl.combot-1.0.dev0/src/cltl/combot/event/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/event/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      465 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/event/bdi.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     3029 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/event/emissor.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.401063 cltl.combot-1.0.dev0/src/cltl/combot/infra/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/__init__.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.401681 cltl.combot-1.0.dev0/src/cltl/combot/infra/config/
+-rw-r--r--   0 sbaez      (501) staff       (20)       76 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/config/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     7260 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/config/api.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     1663 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/config/k8config.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     3753 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/config/local.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2372 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/di_container.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2014 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/docker.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.402658 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/
+-rw-r--r--   0 sbaez      (501) staff       (20)       78 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2384 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/api.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     5385 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/kombu.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2104 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/memory.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      924 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/serialization.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      122 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event/util.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     1732 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/event_log.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     9077 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/groupby_processor.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.403200 cltl.combot-1.0.dev0/src/cltl/combot/infra/resource/
+-rw-r--r--   0 sbaez      (501) staff       (20)      105 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/resource/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     9031 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/resource/api.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    11878 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/resource/threaded.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      316 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/time_util.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    10545 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/topic_worker.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2253 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl/combot/infra/util.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.403509 cltl.combot-1.0.dev0/src/cltl/combot/test/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/test/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      961 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/combot/test/util.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.404512 cltl.combot-1.0.dev0/src/cltl/commons/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     1058 2023-02-28 22:09:37.000000 cltl.combot-1.0.dev0/src/cltl/commons/casefolding.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     5379 2022-11-15 21:07:41.000000 cltl.combot-1.0.dev0/src/cltl/commons/discrete.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.405266 cltl.combot-1.0.dev0/src/cltl/commons/language_data/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_data/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2615 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_data/animations.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      193 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_data/base_cases.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      402 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_data/cfg.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)    24557 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_data/lexicon.json
+-rw-r--r--   0 sbaez      (501) staff       (20)     9287 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_data/sentences.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     5513 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/language_helpers.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2560 2022-11-15 18:30:11.000000 cltl.combot-1.0.dev0/src/cltl/commons/triple_helpers.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.398990 cltl.combot-1.0.dev0/src/cltl.combot.egg-info/
+-rw-r--r--   0 sbaez      (501) staff       (20)     9712 2023-05-25 12:46:02.000000 cltl.combot-1.0.dev0/src/cltl.combot.egg-info/PKG-INFO
+-rw-r--r--   0 sbaez      (501) staff       (20)     1759 2023-05-25 12:46:02.000000 cltl.combot-1.0.dev0/src/cltl.combot.egg-info/SOURCES.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)        1 2023-05-25 12:46:02.000000 cltl.combot-1.0.dev0/src/cltl.combot.egg-info/dependency_links.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)       26 2023-05-25 12:46:02.000000 cltl.combot-1.0.dev0/src/cltl.combot.egg-info/requires.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)       18 2023-05-25 12:46:02.000000 cltl.combot-1.0.dev0/src/cltl.combot.egg-info/top_level.txt
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.397709 cltl.combot-1.0.dev0/src/cltl_service/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.405387 cltl.combot-1.0.dev0/src/cltl_service/combot/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl_service/combot/__init__.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:46:02.405547 cltl.combot-1.0.dev0/src/cltl_service/combot/event_log/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl_service/combot/event_log/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     1806 2023-05-24 16:05:49.000000 cltl.combot-1.0.dev0/src/cltl_service/combot/event_log/service.py
```

### Comparing `cltl.combot-0.0.dev1/LICENCE` & `cltl.combot-1.0.dev0/LICENCE`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/setup.py` & `cltl.combot-1.0.dev0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 with open("VERSION", "r") as fh:
     version = fh.read().strip()
 
 setup(
     name='cltl.combot',
     version=version,
     package_dir={'': 'src'},
-    packages=find_namespace_packages(include=['cltl.*'], where='src'),
+    packages=find_namespace_packages(include=['cltl.*', 'cltl_service.*'], where='src'),
+    package_data={'cltl.commons.language_data': ["*.txt", "*.json"]},
     data_files=[('VERSION', ['VERSION'])],
     url="https://github.com/leolani/cltl-combot",
     license='MIT License',
     author='CLTL',
     author_email='t.baier@vu.nl',
     description='Communication Robot Framework',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.7',
-    install_requires=[],
+    install_requires=['emissor'],
     extras_require={
         "external": [
             "kombu"
         ],
     }
 )
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/__init__.py` & `cltl.combot-1.0.dev0/src/cltl/combot/__init__.py`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/config/api.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/config/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,34 @@
         Raises
         ------
         :class:`ValueError`
             If there is not Configuration with the given name
         """
         raise NotImplementedError()
 
+    def has_config(self, name):
+        # type: (str) -> bool
+        """
+        Test if a configuration with the specified name is available.
+
+        Parameters
+        ----------
+        name : str
+            The name identifying the configuration.
+
+        Returns
+        -------
+        bool
+            True if the configuration is present, False otherwise.
+        """
+        raise NotImplementedError()
+
+    def __contains__(self, key):
+        return self.has_config(key)
+
 
 class Configuration(object):
     def get(self, key, multi=False):
         # type: (str) -> str
         """
         Get a configuration value as String for the specified key.
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/config/k8config.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/config/k8config.py`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/config/local.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/config/local.py`

 * *Files 19% similar despite different names*

```diff
@@ -55,52 +55,64 @@
             raise ValueError("No configuration loaded")
 
         return LocalConfigurationManager(LocalConfigurationContainer.__config)
 
 
 class LocalConfigurationManager(ConfigurationManager):
     def __init__(self, config):
+        # type: (ConfigParser) -> None
         self._config = config
 
+    def has_config(self, name):
+        return self._config.has_section(name)
+
     def get_config(self, name, callback=None):
         if callback:
             callback(LocalConfig(self._config, name))
 
         return LocalConfig(self._config, name)
 
+    def __contains__(self, key):
+        return self.has_config(key)
+
 
 class LocalConfig(Configuration):
     def __init__(self, parser, section):
         # type: (ConfigParser, str) -> None
         self._parser = parser
         self._section = section
 
     def get(self, key, multi=False):
         # TODO Python 3 Cast to string (instead of unicode string)
-        val = str(self._parser.get(self._section, key))
+        value = str(self._parser.get(self._section, key))
+        if not value:
+            return value if not multi else []
 
-        return val if not multi else [v.strip() for v in val.split(_DELIMITER)]
+        return value if not multi else [v.strip() for v in value.split(_DELIMITER)]
 
     def get_int(self, key):
         return self._parser.getint(self._section, key)
 
     def get_float(self, key):
         return self._parser.getfloat(self._section, key)
 
     def get_boolean(self, key):
         return self._parser.getboolean(self._section, key)
 
     def get_enum(self, key, type, multi=False):
         value = self.get(key, multi)
+        if not value:
+            return value if not multi else []
+
         string_values = value if multi else [value]
         enum_vals = [getattr(type, val.strip().upper()) for val in string_values]
 
         return enum_vals if multi else enum_vals[0]
 
     def __contains__(self, key):
-        return self._parser.items(self._section).__contains__(key)
+        return self._parser.has_option(self._section, key)
 
     def __iter__(self):
-        return self._parser.items(self._section).__iter__()
+        return iter(self._parser.items(self._section))
 
     def __len__(self):
-        return self._parser.items(self._section).__len__()
+        return len(self._parser.items(self._section))
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/di_container.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/di_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,28 @@
     _singletons = dict()
 
     @classmethod
     def _reset(cls):
         cls._lock = Lock()
         cls._singletons = dict()
 
+    def start(self):
+        pass
+
+    def stop(self):
+        pass
+
+    def __enter__(self):
+        self.start()
+
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.stop()
+
 
 def singleton_for_kw(keys):
     """
     Decorator to provide singleton instances from methods of a DIContainer for
     each distinct value of the keyword argument name.
     """
     def plain_singleton(method):
@@ -35,15 +49,15 @@
                 with self._lock:
                     if not singleton_attr in DIContainer._singletons:
                         #First set to None and then instantiate outside the lock to avoid dead-locks
                         DIContainer._singletons[singleton_attr] = None
                         create_instance = True
                 if create_instance:
                     instance = method(self, *args, **kwargs)
-                    if not instance:
+                    if instance is None:
                         raise ValueError("could not set " + singleton_attr)
                     DIContainer._singletons[singleton_attr] = instance
 
             cnt = 0
             # The instance is created outside the lock, therefore we can end up here with None
             while DIContainer._singletons[singleton_attr] is None:
                 sleep(0.01)
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/event/api.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/event/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import uuid
 from dataclasses import dataclass
 from typing import TypeVar, Generic, Optional, Iterable, Callable
 
-import time
-
 from cltl.combot.infra.di_container import DIContainer
+from cltl.combot.infra.time_util import timestamp_now
 
 
 class TopicError(ValueError):
     pass
 
 
 @dataclass
 class EventMetadata:
-    timestamp: float = time.time()
+    timestamp: int = timestamp_now()
     offset: int = -1
     topic: str = ""
 
     @classmethod
-    def with_(cls, metadata, timestamp: float = None, offset: int = None, topic: str = None) -> Optional["EventMetadata"]:
+    def with_(cls, metadata, timestamp: int = None, offset: int = None, topic: str = None) -> Optional["EventMetadata"]:
         new_timestamp = timestamp if timestamp is not None else metadata.timestamp
         new_offset = offset if offset is not None else metadata.offset
         new_topic = topic if topic is not None else metadata.topic
 
         return cls(new_timestamp, new_offset, new_topic)
 
 
@@ -38,15 +37,18 @@
         return cls(str(uuid.uuid4()), payload)
 
     @classmethod
     def with_topic(cls, event, topic: str) -> Optional["Event"]:
         return cls(event.id, event.payload, EventMetadata.with_(event.metadata, topic=topic))
 
     def __eq__(self, other):
-        return self.id == other.id
+        return other and self.id == other.id
+
+    def __hash__(self):
+        return hash(self.id) if self.id else hash("")
 
 
 class EventBus:
     """
     Supports publishing of and subscribing to events based on topics.
 
     Events published to a topic are delivered to all subscribers in the order
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/event/kombu.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/event/kombu.py`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/event/memory.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/event/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from threading import RLock
 
 from cltl.combot.infra.di_container import singleton
 from cltl.combot.infra.event.api import EventBusContainer, EventBus, Event
+from cltl.combot.infra.time_util import timestamp_now
 
 logger = logging.getLogger(__name__)
 
 
 class SynchronousEventBusContainer(EventBusContainer):
     logger.info("Initialized SynchronousEventBusContainer")
 
@@ -18,17 +19,21 @@
 
 class SynchronousEventBus(EventBus):
     def __init__(self):
         self._handlers = {}
         self._topic_lock = RLock()
 
     def publish(self, topic, event):
+        start = timestamp_now()
+
         for handler in self.__get_handlers(topic):
             handler(Event.with_topic(event, topic))
 
+        logger.debug("Published event %s in %s ms", event.id, timestamp_now() - start)
+
     def subscribe(self, topic, handler):
         with self._topic_lock:
             self.__get_handlers(topic).append(handler)
 
         logger.info("Subscribed %s to topic %s", self.__format_name(handler), topic)
 
     def unsubscribe(self, topic, handler):
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/resource/api.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/resource/api.py`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/resource/threaded.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/resource/threaded.py`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/infra/util.py` & `cltl.combot-1.0.dev0/src/cltl/combot/infra/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import threading
 
 import logging
 from threading import Thread
+from typing import Any
+
 from time import sleep
 
 logger = logging.getLogger(__name__)
 
 
 class Scheduler(Thread):
     """
@@ -55,21 +57,32 @@
         return self._running
 
     def stop(self, timeout=None):
         self._running = False
         logger.info("Stopped %s thread", self.name)
 
 
-class ThreadsafeBoolean:
-    def __init__(self, value: bool = False):
+class ThreadsafeValue:
+    def __init__(self, value: Any):
         self._value = value
         self._lock = threading.Lock()
 
     @property
     def value(self):
         with self._lock:
             return self._value
 
     @value.setter
-    def value(self, value):
+    def value(self, value: Any):
         with self._lock:
-            self._value = value
+            self._value = value
+
+    def __str__(self) -> str:
+        return str(self.value)
+
+
+class ThreadsafeBoolean(ThreadsafeValue):
+    def __init__(self, value: bool = False):
+        super().__init__(value)
+
+    def __bool__(self) -> bool:
+        return self.value
```

### Comparing `cltl.combot-0.0.dev1/src/cltl/combot/test/util.py` & `cltl.combot-1.0.dev0/src/cltl/combot/test/util.py`

 * *Files identical despite different names*

### Comparing `cltl.combot-0.0.dev1/src/cltl.combot.egg-info/SOURCES.txt` & `cltl.combot-1.0.dev0/src/cltl.combot.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,25 +4,47 @@
 setup.py
 src/cltl.combot.egg-info/PKG-INFO
 src/cltl.combot.egg-info/SOURCES.txt
 src/cltl.combot.egg-info/dependency_links.txt
 src/cltl.combot.egg-info/requires.txt
 src/cltl.combot.egg-info/top_level.txt
 src/cltl/combot/__init__.py
+src/cltl/combot/event/__init__.py
+src/cltl/combot/event/bdi.py
+src/cltl/combot/event/emissor.py
 src/cltl/combot/infra/__init__.py
 src/cltl/combot/infra/di_container.py
+src/cltl/combot/infra/docker.py
+src/cltl/combot/infra/event_log.py
+src/cltl/combot/infra/groupby_processor.py
+src/cltl/combot/infra/time_util.py
 src/cltl/combot/infra/topic_worker.py
 src/cltl/combot/infra/util.py
 src/cltl/combot/infra/config/__init__.py
 src/cltl/combot/infra/config/api.py
 src/cltl/combot/infra/config/k8config.py
 src/cltl/combot/infra/config/local.py
 src/cltl/combot/infra/event/__init__.py
 src/cltl/combot/infra/event/api.py
 src/cltl/combot/infra/event/kombu.py
 src/cltl/combot/infra/event/memory.py
+src/cltl/combot/infra/event/serialization.py
 src/cltl/combot/infra/event/util.py
 src/cltl/combot/infra/resource/__init__.py
 src/cltl/combot/infra/resource/api.py
 src/cltl/combot/infra/resource/threaded.py
 src/cltl/combot/test/__init__.py
-src/cltl/combot/test/util.py
+src/cltl/combot/test/util.py
+src/cltl/commons/__init__.py
+src/cltl/commons/casefolding.py
+src/cltl/commons/discrete.py
+src/cltl/commons/language_helpers.py
+src/cltl/commons/triple_helpers.py
+src/cltl/commons/language_data/__init__.py
+src/cltl/commons/language_data/animations.py
+src/cltl/commons/language_data/base_cases.py
+src/cltl/commons/language_data/cfg.txt
+src/cltl/commons/language_data/lexicon.json
+src/cltl/commons/language_data/sentences.py
+src/cltl_service/combot/__init__.py
+src/cltl_service/combot/event_log/__init__.py
+src/cltl_service/combot/event_log/service.py
```

