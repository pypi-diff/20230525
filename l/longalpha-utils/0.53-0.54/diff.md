# Comparing `tmp/longalpha_utils-0.53.tar.gz` & `tmp/longalpha_utils-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.53.tar", last modified: Wed May 24 14:47:48 2023, max compression
+gzip compressed data, was "longalpha_utils-0.54.tar", last modified: Thu May 25 02:35:43 2023, max compression
```

## Comparing `longalpha_utils-0.53.tar` & `longalpha_utils-0.54.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:47:48.782108 longalpha_utils-0.53/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 14:47:48.782108 longalpha_utils-0.53/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:47:48.782108 longalpha_utils-0.53/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-24 14:47:37.000000 longalpha_utils-0.53/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:47:48.782108 longalpha_utils-0.53/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 14:47:48.000000 longalpha_utils-0.53/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:47:48.782108 longalpha_utils-0.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-24 14:47:37.000000 longalpha_utils-0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:35:43.592790 longalpha_utils-0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 02:35:43.592790 longalpha_utils-0.54/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:35:43.592790 longalpha_utils-0.54/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:35:43.592790 longalpha_utils-0.54/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 02:35:43.592790 longalpha_utils-0.54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 02:35:30.000000 longalpha_utils-0.54/setup.py
```

### Comparing `longalpha_utils-0.53/longalpha_utils/messenger.py` & `longalpha_utils-0.54/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.53/longalpha_utils/transfers.py` & `longalpha_utils-0.54/longalpha_utils/transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pyspark.sql import SparkSession, DataFrame
 from sqlalchemy import Engine
 from sqlalchemy import create_engine
 from sqlalchemy import text
 from minio.error import S3Error
 from datetime import date, timedelta
 from pyspark.sql.utils import AnalysisException
-from longalpha_utils.utils import multi_union_by_name
+from longalpha_utils.utils import multi_union_by_name, get_s3_path
 from tqdm import tqdm
 
 
 def init_spark(
     spark_executor_memory: str = "30g",
     spark_driver_memory: str = "90g",
     s3_endpoint: Optional[str] = None,
@@ -208,26 +208,26 @@
 
 
 def get_s3_data_spark(
     spark: SparkSession,
     start_date: date,
     end_date: date,
     bucket: str,
-    subfolder: str,
+    prefix: str,
     show_missing_dates: bool = False,
     progress_bar: bool = True,
 ) -> Union[DataFrame, None]:
     """
     Get data from s3 for a given date range
     Args:
         spark: spark session
         start_date: start date to get options data for
         end_date: end date to get options data for
         bucket: s3 bucket name
-        subfolder: subfolder in the s3 bucket
+        prefix: prefix in the s3 bucket
         show_missing_dates: whether to print out missing dates
         progress_bar: whether to show a progress bar
 
     Returns: a spark dataframe if data exists, None otherwise
 
     """
     dates = []
@@ -235,15 +235,15 @@
         dates.append(start_date)
         start_date += timedelta(days=1)
     if progress_bar:
         dates = tqdm(dates)
 
     options = []
     for day in dates:
-        file_s3_path = "s3a://" + os.path.join(bucket, f"{subfolder}/{day}.parquet")
+        file_s3_path = get_s3_path(bucket, prefix, day)
         try:
             option = spark.read.parquet(file_s3_path)
             options.append(option)
         except AnalysisException:
             if show_missing_dates:
                 print(f"Options data for {start_date} does not exist.")
             else:
```

### Comparing `longalpha_utils-0.53/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.54/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.53/longalpha_utils/utils.py` & `longalpha_utils-0.54/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.53/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.54/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.53/setup.py` & `longalpha_utils-0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.53",
+    version="0.54",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

