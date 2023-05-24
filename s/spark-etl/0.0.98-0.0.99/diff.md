# Comparing `tmp/spark-etl-0.0.98.tar.gz` & `tmp/spark-etl-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spark-etl-0.0.98.tar", last modified: Sat Apr 17 03:50:06 2021, max compression
+gzip compressed data, was "dist/spark-etl-0.0.99.tar", last modified: Thu Aug 12 21:21:46 2021, max compression
```

## Comparing `spark-etl-0.0.98.tar` & `spark-etl-0.0.99.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      881 2021-04-17 03:49:56.000000 spark-etl-0.0.98/setup.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6406 2021-03-07 07:42:55.000000 spark-etl-0.0.98/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2021-04-17 03:50:06.000000 spark-etl-0.0.98/setup.cfg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    14237 2021-03-10 01:22:22.000000 spark-etl-0.0.98/src/spark_etl/utils.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/job_submitters/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11185 2021-04-12 21:44:15.000000 spark-etl-0.0.98/src/spark_etl/job_submitters/livy_job_submitter.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      817 2020-07-22 00:20:10.000000 spark-etl-0.0.98/src/spark_etl/job_submitters/abstract_job_submitter.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2021-03-08 14:08:49.000000 spark-etl-0.0.98/src/spark_etl/job_submitters/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/core/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      660 2021-02-10 10:08:01.000000 spark-etl-0.0.98/src/spark_etl/core/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       64 2021-02-10 10:08:01.000000 spark-etl-0.0.98/src/spark_etl/core/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4242 2021-02-03 22:21:56.000000 spark-etl-0.0.98/src/spark_etl/application.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      632 2021-02-03 22:30:33.000000 spark-etl-0.0.98/src/spark_etl/build.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      154 2021-03-08 14:08:49.000000 spark-etl-0.0.98/src/spark_etl/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/deployers/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2028 2021-04-12 22:06:15.000000 spark-etl-0.0.98/src/spark_etl/deployers/s3_deployer.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      464 2021-03-07 21:58:51.000000 spark-etl-0.0.98/src/spark_etl/deployers/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      178 2020-07-22 00:20:10.000000 spark-etl-0.0.98/src/spark_etl/deployers/abstract_deployer.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4795 2021-02-19 11:03:07.000000 spark-etl-0.0.98/src/spark_etl/deployers/job_loader.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2248 2021-04-12 21:44:15.000000 spark-etl-0.0.98/src/spark_etl/deployers/hdfs_deployer.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      679 2021-03-08 14:08:49.000000 spark-etl-0.0.98/src/spark_etl/exceptions.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/vendors/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/vendors/oracle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      492 2020-07-22 00:20:10.000000 spark-etl-0.0.98/src/spark_etl/vendors/oracle/tools.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5568 2021-03-03 08:02:37.000000 spark-etl-0.0.98/src/spark_etl/vendors/oracle/dataflow_deployer.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      104 2020-07-22 00:20:10.000000 spark-etl-0.0.98/src/spark_etl/vendors/oracle/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8112 2021-02-10 10:08:01.000000 spark-etl-0.0.98/src/spark_etl/vendors/oracle/job_loader.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6697 2021-04-12 23:58:35.000000 spark-etl-0.0.98/src/spark_etl/vendors/oracle/dataflow_job_submitter.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2020-07-22 00:20:10.000000 spark-etl-0.0.98/src/spark_etl/vendors/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl/vendors/local/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3160 2021-04-12 21:44:15.000000 spark-etl-0.0.98/src/spark_etl/vendors/local/pyspark_job_submitter.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)       97 2020-11-06 03:57:38.000000 spark-etl-0.0.98/src/spark_etl/vendors/local/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1469 2021-02-18 20:40:35.000000 spark-etl-0.0.98/src/spark_etl/vendors/local/local_deployer.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4222 2021-04-12 21:44:15.000000 spark-etl-0.0.98/src/spark_etl/vendors/local/job_loader.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5288 2021-04-17 03:49:56.000000 spark-etl-0.0.98/src/spark_etl/ssh_config.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1217 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       10 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl.egg-info/top_level.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8057 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       26 2021-04-17 03:50:06.000000 spark-etl-0.0.98/src/spark_etl.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8057 2021-04-17 03:50:06.000000 spark-etl-0.0.98/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2019-11-23 20:00:22.000000 spark-etl-0.0.98/MANIFEST.in
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      881 2021-08-12 21:21:38.000000 spark-etl-0.0.99/setup.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6406 2021-03-07 07:42:55.000000 spark-etl-0.0.99/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2021-08-12 21:21:46.000000 spark-etl-0.0.99/setup.cfg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    14237 2021-08-12 21:21:38.000000 spark-etl-0.0.99/src/spark_etl/utils.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/job_submitters/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11185 2021-04-12 21:44:15.000000 spark-etl-0.0.99/src/spark_etl/job_submitters/livy_job_submitter.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      817 2020-07-22 00:20:10.000000 spark-etl-0.0.99/src/spark_etl/job_submitters/abstract_job_submitter.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2021-03-08 14:08:49.000000 spark-etl-0.0.99/src/spark_etl/job_submitters/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/core/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      660 2021-02-10 10:08:01.000000 spark-etl-0.0.99/src/spark_etl/core/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       64 2021-02-10 10:08:01.000000 spark-etl-0.0.99/src/spark_etl/core/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4242 2021-02-03 22:21:56.000000 spark-etl-0.0.99/src/spark_etl/application.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      632 2021-02-03 22:30:33.000000 spark-etl-0.0.99/src/spark_etl/build.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      154 2021-03-08 14:08:49.000000 spark-etl-0.0.99/src/spark_etl/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/deployers/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2028 2021-04-12 22:06:15.000000 spark-etl-0.0.99/src/spark_etl/deployers/s3_deployer.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      464 2021-03-07 21:58:51.000000 spark-etl-0.0.99/src/spark_etl/deployers/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      178 2020-07-22 00:20:10.000000 spark-etl-0.0.99/src/spark_etl/deployers/abstract_deployer.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4795 2021-02-19 11:03:07.000000 spark-etl-0.0.99/src/spark_etl/deployers/job_loader.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2248 2021-04-12 21:44:15.000000 spark-etl-0.0.99/src/spark_etl/deployers/hdfs_deployer.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      679 2021-03-08 14:08:49.000000 spark-etl-0.0.99/src/spark_etl/exceptions.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/vendors/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/vendors/oracle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      492 2020-07-22 00:20:10.000000 spark-etl-0.0.99/src/spark_etl/vendors/oracle/tools.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5568 2021-03-03 08:02:37.000000 spark-etl-0.0.99/src/spark_etl/vendors/oracle/dataflow_deployer.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      104 2020-07-22 00:20:10.000000 spark-etl-0.0.99/src/spark_etl/vendors/oracle/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8112 2021-02-10 10:08:01.000000 spark-etl-0.0.99/src/spark_etl/vendors/oracle/job_loader.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6697 2021-04-12 23:58:35.000000 spark-etl-0.0.99/src/spark_etl/vendors/oracle/dataflow_job_submitter.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2020-07-22 00:20:10.000000 spark-etl-0.0.99/src/spark_etl/vendors/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl/vendors/local/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3160 2021-04-12 21:44:15.000000 spark-etl-0.0.99/src/spark_etl/vendors/local/pyspark_job_submitter.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)       97 2020-11-06 03:57:38.000000 spark-etl-0.0.99/src/spark_etl/vendors/local/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1469 2021-02-18 20:40:35.000000 spark-etl-0.0.99/src/spark_etl/vendors/local/local_deployer.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4222 2021-04-12 21:44:15.000000 spark-etl-0.0.99/src/spark_etl/vendors/local/job_loader.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5288 2021-04-17 03:49:56.000000 spark-etl-0.0.99/src/spark_etl/ssh_config.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1217 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       10 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl.egg-info/top_level.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8057 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       26 2021-08-12 21:21:46.000000 spark-etl-0.0.99/src/spark_etl.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8057 2021-08-12 21:21:46.000000 spark-etl-0.0.99/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2019-11-23 20:00:22.000000 spark-etl-0.0.99/MANIFEST.in
```

### Comparing `spark-etl-0.0.98/setup.py` & `spark-etl-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="spark-etl",
-    version="0.0.98",
+    version="0.0.99",
     description="Generic ETL Pipeline Framework for Apache Spark",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/spark_etl",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `spark-etl-0.0.98/README.md` & `spark-etl-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/utils.py` & `spark-etl-0.0.99/src/spark_etl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                     print()
                     continue
 
                 # for any other command, we will append to the cli buffer
                 if line_mode == "off":
                     cli_lines.append(command)
                 else:
-                    self.client_channel_write_json(
+                    self.client_channel.write_json(
                         CLI_REQUEST_NAME,
                         {
                             "type": "@@" + line_mode,
                             "lines": [ command ]
                         }
                     )
                     is_waiting_for_response = True
```

### Comparing `spark-etl-0.0.98/src/spark_etl/job_submitters/livy_job_submitter.py` & `spark-etl-0.0.99/src/spark_etl/job_submitters/livy_job_submitter.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/job_submitters/abstract_job_submitter.py` & `spark-etl-0.0.99/src/spark_etl/job_submitters/abstract_job_submitter.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/core/main.py` & `spark-etl-0.0.99/src/spark_etl/core/main.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/application.py` & `spark-etl-0.0.99/src/spark_etl/application.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/build.py` & `spark-etl-0.0.99/src/spark_etl/build.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/deployers/s3_deployer.py` & `spark-etl-0.0.99/src/spark_etl/deployers/s3_deployer.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/deployers/job_loader.py` & `spark-etl-0.0.99/src/spark_etl/deployers/job_loader.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/deployers/hdfs_deployer.py` & `spark-etl-0.0.99/src/spark_etl/deployers/hdfs_deployer.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/exceptions.py` & `spark-etl-0.0.99/src/spark_etl/exceptions.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/vendors/oracle/dataflow_deployer.py` & `spark-etl-0.0.99/src/spark_etl/vendors/oracle/dataflow_deployer.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/vendors/oracle/job_loader.py` & `spark-etl-0.0.99/src/spark_etl/vendors/oracle/job_loader.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/vendors/oracle/dataflow_job_submitter.py` & `spark-etl-0.0.99/src/spark_etl/vendors/oracle/dataflow_job_submitter.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/vendors/local/pyspark_job_submitter.py` & `spark-etl-0.0.99/src/spark_etl/vendors/local/pyspark_job_submitter.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/vendors/local/local_deployer.py` & `spark-etl-0.0.99/src/spark_etl/vendors/local/local_deployer.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/vendors/local/job_loader.py` & `spark-etl-0.0.99/src/spark_etl/vendors/local/job_loader.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl/ssh_config.py` & `spark-etl-0.0.99/src/spark_etl/ssh_config.py`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl.egg-info/SOURCES.txt` & `spark-etl-0.0.99/src/spark_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spark-etl-0.0.98/src/spark_etl.egg-info/PKG-INFO` & `spark-etl-0.0.99/src/spark_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-etl
-Version: 0.0.98
+Version: 0.0.99
 Summary: Generic ETL Pipeline Framework for Apache Spark
 Home-page: https://github.com/stonezhong/spark_etl
 Author: Stone Zhong
 Author-email: stonezhong@hotmail.com
 License: MIT
 Description: * [Overview](#overview)
             * [Goal](#goal)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spark-etl Version: 0.0.98 Summary: Generic ETL
+Metadata-Version: 2.1 Name: spark-etl Version: 0.0.99 Summary: Generic ETL
 Pipeline Framework for Apache Spark Home-page: https://github.com/stonezhong/
 spark_etl Author: Stone Zhong Author-email: stonezhong@hotmail.com License: MIT
 Description: * [Overview](#overview) * [Goal](#goal) * [Benefit](#benefit) *
 [Supported platforms](#supported_platforms) * [APIs](#apis) * [Application]
 (#application) * [Application entry signature](#application-entry-signature) *
 [Job Deployer](#job-deployer) * [Job Submitter](#job-submitter) * [Tool:
 etl.py](#tool-etlpy) * [Build an application](#build-an-application) * [Deploy
```

### Comparing `spark-etl-0.0.98/PKG-INFO` & `spark-etl-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-etl
-Version: 0.0.98
+Version: 0.0.99
 Summary: Generic ETL Pipeline Framework for Apache Spark
 Home-page: https://github.com/stonezhong/spark_etl
 Author: Stone Zhong
 Author-email: stonezhong@hotmail.com
 License: MIT
 Description: * [Overview](#overview)
             * [Goal](#goal)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spark-etl Version: 0.0.98 Summary: Generic ETL
+Metadata-Version: 2.1 Name: spark-etl Version: 0.0.99 Summary: Generic ETL
 Pipeline Framework for Apache Spark Home-page: https://github.com/stonezhong/
 spark_etl Author: Stone Zhong Author-email: stonezhong@hotmail.com License: MIT
 Description: * [Overview](#overview) * [Goal](#goal) * [Benefit](#benefit) *
 [Supported platforms](#supported_platforms) * [APIs](#apis) * [Application]
 (#application) * [Application entry signature](#application-entry-signature) *
 [Job Deployer](#job-deployer) * [Job Submitter](#job-submitter) * [Tool:
 etl.py](#tool-etlpy) * [Build an application](#build-an-application) * [Deploy
```

