# Comparing `tmp/dcarte-0.4.8.tar.gz` & `tmp/dcarte-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcarte-0.4.8.tar", max compression
+gzip compressed data, was "dcarte-0.4.9.tar", max compression
```

## Comparing `dcarte-0.4.8.tar` & `dcarte-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     6148 2023-03-02 10:28:43.355568 dcarte-0.4.8/dcarte/.DS_Store
--rw-r--r--   0        0        0      328 2023-03-02 13:05:04.634212 dcarte-0.4.8/dcarte/__init__.py
--rw-r--r--   0        0        0      144 2023-03-17 05:12:35.384344 dcarte-0.4.8/dcarte/__version__.py
--rw-r--r--   0        0        0     5131 2023-02-27 06:27:50.653600 dcarte-0.4.8/dcarte/_delete.py
--rw-r--r--   0        0        0    15537 2023-02-27 09:42:54.218682 dcarte-0.4.8/dcarte/config.py
--rw-r--r--   0        0        0     6148 2023-03-02 10:28:43.353594 dcarte-0.4.8/dcarte/derived/.DS_Store
--rw-r--r--   0        0        0      136 2023-02-26 17:30:23.964408 dcarte-0.4.8/dcarte/derived/__init__.py
--rw-r--r--   0        0        0    10693 2023-03-02 11:14:10.739785 dcarte-0.4.8/dcarte/derived/base.py
--rw-r--r--   0        0        0     3515 2023-02-22 07:38:53.086830 dcarte-0.4.8/dcarte/derived/bed_occupancy.py
--rw-r--r--   0        0        0    14591 2023-03-02 11:13:29.284780 dcarte-0.4.8/dcarte/derived/weekly_profile.py
--rw-r--r--   0        0        0      739 2023-02-22 07:38:53.087185 dcarte-0.4.8/dcarte/domains.py
--rw-r--r--   0        0        0      705 2023-03-02 21:24:44.904574 dcarte-0.4.8/dcarte/download.py
--rw-r--r--   0        0        0     9289 2023-02-22 07:38:53.087807 dcarte-0.4.8/dcarte/legacy/legacy.py
--rw-r--r--   0        0        0     4027 2023-03-17 05:12:42.003485 dcarte-0.4.8/dcarte/load.py
--rw-r--r--   0        0        0     8067 2023-03-13 14:04:14.626517 dcarte-0.4.8/dcarte/local.py
--rw-r--r--   0        0        0    11841 2023-03-02 08:47:24.007338 dcarte-0.4.8/dcarte/minder.py
--rw-r--r--   0        0        0     1887 2023-02-26 16:51:05.307768 dcarte-0.4.8/dcarte/source_yaml/care.yaml
--rw-r--r--   0        0        0      774 2023-02-22 07:38:53.088896 dcarte-0.4.8/dcarte/source_yaml/lookup.yaml
--rw-r--r--   0        0        0     4229 2023-02-26 16:51:49.446097 dcarte-0.4.8/dcarte/source_yaml/raw.yaml
--rw-r--r--   0        0        0     1764 2023-02-27 08:42:53.945890 dcarte-0.4.8/dcarte/update.py
--rw-r--r--   0        0        0    31778 2023-03-13 13:06:39.009511 dcarte-0.4.8/dcarte/utils.py
--rw-r--r--   0        0        0      942 2023-03-17 05:12:28.140109 dcarte-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 dcarte-0.4.8/setup.py
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 dcarte-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2023-03-02 10:28:43.355568 dcarte-0.4.9/dcarte/.DS_Store
+-rw-r--r--   0        0        0      328 2023-03-02 13:05:04.634212 dcarte-0.4.9/dcarte/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-09 04:16:26.747408 dcarte-0.4.9/dcarte/__version__.py
+-rw-r--r--   0        0        0     5131 2023-02-27 06:27:50.653600 dcarte-0.4.9/dcarte/_delete.py
+-rw-r--r--   0        0        0    15537 2023-02-27 09:42:54.218682 dcarte-0.4.9/dcarte/config.py
+-rw-r--r--   0        0        0     6148 2023-03-02 10:28:43.353594 dcarte-0.4.9/dcarte/derived/.DS_Store
+-rw-r--r--   0        0        0      136 2023-02-26 17:30:23.964408 dcarte-0.4.9/dcarte/derived/__init__.py
+-rw-r--r--   0        0        0    10647 2023-03-17 08:17:29.438838 dcarte-0.4.9/dcarte/derived/base.py
+-rw-r--r--   0        0        0     3515 2023-02-22 07:38:53.086830 dcarte-0.4.9/dcarte/derived/bed_occupancy.py
+-rw-r--r--   0        0        0    14658 2023-05-05 08:58:54.318060 dcarte-0.4.9/dcarte/derived/weekly_profile.py
+-rw-r--r--   0        0        0      739 2023-02-22 07:38:53.087185 dcarte-0.4.9/dcarte/domains.py
+-rw-r--r--   0        0        0      705 2023-03-02 21:24:44.904574 dcarte-0.4.9/dcarte/download.py
+-rw-r--r--   0        0        0     9289 2023-02-22 07:38:53.087807 dcarte-0.4.9/dcarte/legacy/legacy.py
+-rw-r--r--   0        0        0     4147 2023-05-05 08:43:23.948366 dcarte-0.4.9/dcarte/load.py
+-rw-r--r--   0        0        0     8067 2023-03-13 14:04:14.626517 dcarte-0.4.9/dcarte/local.py
+-rw-r--r--   0        0        0    11841 2023-03-02 08:47:24.007338 dcarte-0.4.9/dcarte/minder.py
+-rw-r--r--   0        0        0     1887 2023-02-26 16:51:05.307768 dcarte-0.4.9/dcarte/source_yaml/care.yaml
+-rw-r--r--   0        0        0      774 2023-02-22 07:38:53.088896 dcarte-0.4.9/dcarte/source_yaml/lookup.yaml
+-rw-r--r--   0        0        0     4229 2023-02-26 16:51:49.446097 dcarte-0.4.9/dcarte/source_yaml/raw.yaml
+-rw-r--r--   0        0        0     1764 2023-02-27 08:42:53.945890 dcarte-0.4.9/dcarte/update.py
+-rw-r--r--   0        0        0    31773 2023-04-14 04:40:42.360111 dcarte-0.4.9/dcarte/utils.py
+-rw-r--r--   0        0        0      942 2023-05-09 04:16:16.210323 dcarte-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 dcarte-0.4.9/setup.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 dcarte-0.4.9/PKG-INFO
```

### Comparing `dcarte-0.4.8/dcarte/.DS_Store` & `dcarte-0.4.9/dcarte/.DS_Store`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/_delete.py` & `dcarte-0.4.9/dcarte/_delete.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/config.py` & `dcarte-0.4.9/dcarte/config.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/derived/.DS_Store` & `dcarte-0.4.9/dcarte/derived/.DS_Store`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/derived/base.py` & `dcarte-0.4.9/dcarte/derived/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     activity = activity[['patient_id', 'start_date', 'device_type', 'location_name']]\
                         .rename({'location_name': 'activity'}, axis=1)       
     appliances = appliances[['patient_id', 'start_date', 'device_type', 'value']]\
                             .rename({'value': 'activity'}, axis=1) 
     kitchen = pd.concat([doors, activity, appliances.dropna()])   
     kitchen = kitchen[kitchen.patient_id != ''].sort_values(['patient_id', 'start_date']) 
     kitchen = process_transition(kitchen, ['patient_id'], 'start_date', 'activity', ['device_type'])
-    return kitchen.reset_index(drop=True)
+    return kitchen.reset_index()
 
 
 def process_motion(self):
     activity = self.datasets['activity']
     activity = localize_time(activity,['start_date'])
     entryway = self.datasets['entryway']
     bed_occupancy = self.datasets['bed_occupancy']
@@ -257,12 +257,11 @@
         
         LocalDataset(dataset_name = dataset,
                      datasets = p_datasets,
                      pipeline = [f'process_{dataset.lower()}'],
                      domain = domain,
                      module = module,
                      module_path = module_path,
-                     reapply = True,
                      dependencies = parent_datasets[dataset])
     
 if __name__ == "__main__":
     create_base_datasets()
```

### Comparing `dcarte-0.4.8/dcarte/derived/bed_occupancy.py` & `dcarte-0.4.9/dcarte/derived/bed_occupancy.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/derived/weekly_profile.py` & `dcarte-0.4.9/dcarte/derived/weekly_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 
     diurnal_habits = resample_sleep_metrics(sleep_periods,'Diurnal')
     diurnal_habits = diurnal_habits.assign(nap_ibp = diurnal_habits.time_in_bed)
     sleep_metrics = pd.merge(sleep_metrics,diurnal_habits.nap_ibp,how='left',left_index=True, right_index=True)
     sleep_metrics.nap_ibp = sleep_metrics.nap_ibp.fillna(0)
     sleep_metrics = sleep_metrics.assign(time_to_bed = (sleep_metrics.start_time.dt.time.apply(time_to_angles)+180)%360,
                                          wake_up_time = sleep_metrics.end_time.dt.time.apply(time_to_angles))
+    sleep_metrics = sleep_metrics.reset_index().rename(columns={'datetime':'start_date'})
     return sleep_metrics
 
 
 def resample_sleep_metrics(sleep_periods,period_type:str="Nocturnal"):
     habits = sleep_periods.query('period_type == @period_type').drop(columns=['period_type'])
     habits = (habits.
               reset_index().
@@ -200,15 +201,15 @@
     df = df.rename(columns=mapper)            
     df = df.assign(
         deep_ratio = (df.DEEP)/df.ibp,
         awake_ratio = (df.AWAKE)/df.ibp,
         rem_ratio = (df.REM)/df.ibp,
         light_ratio = (df.LIGHT)/df.ibp,
         exit_ratio = (df.nb_awakenings/(df.ibp+df.obp)),
-        night = df.index.get_level_values(1).date   
+        night = df.start_date
     )
 
     return df
     
 
 def process_physiology_dailies(obj):
     """physiology_dailies creates a daily summary across key features from the dialy vital signs
```

### Comparing `dcarte-0.4.8/dcarte/domains.py` & `dcarte-0.4.9/dcarte/domains.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/download.py` & `dcarte-0.4.9/dcarte/download.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/legacy/legacy.py` & `dcarte-0.4.9/dcarte/legacy/legacy.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/load.py` & `dcarte-0.4.9/dcarte/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         raise Exception(f"Sorry, {dataset} is not a registered dataset in {domain} domain in dcarte")
     
     
         
     local_file = f'{data_folder}{sep}{domain}{sep}{dataset}.parquet'
     if path_exists(local_file):
         local_dataset = read_table(local_file)
-        if 'start_date' in local_dataset.columns:
-            last_update = local_dataset.start_date.max()
+        if any(col in local_dataset.columns for col in ['start_date', 'start_time']):
+            col = 'start_date' if 'start_date' in local_dataset.columns else 'start_time'
+            last_update = local_dataset[col].max()
     
 
     if (dflt['reapply'] or dflt['reload']) and path_exists(local_file):
         dflt['reapply'] = False
         Path(local_file).unlink()
         return load(dataset,domain,**dflt)
```

### Comparing `dcarte-0.4.8/dcarte/local.py` & `dcarte-0.4.9/dcarte/local.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/minder.py` & `dcarte-0.4.9/dcarte/minder.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/source_yaml/care.yaml` & `dcarte-0.4.9/dcarte/source_yaml/care.yaml`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/source_yaml/lookup.yaml` & `dcarte-0.4.9/dcarte/source_yaml/lookup.yaml`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/source_yaml/raw.yaml` & `dcarte-0.4.9/dcarte/source_yaml/raw.yaml`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/update.py` & `dcarte-0.4.9/dcarte/update.py`

 * *Files identical despite different names*

### Comparing `dcarte-0.4.8/dcarte/utils.py` & `dcarte-0.4.9/dcarte/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     Segment a pandas series into a frequency polygon using a sliding window and a Savitzky-Golay filter.
 
     Parameters
     ----------
     v : pandas.Series
         A series of values to segment.
     window_length : int, optional
-        Length of the window used by the Savitzky-Golay filter. Must be odd and positive. Default is 59.
+        Length of the window used by the 
+         filter. Must be odd and positive. Default is 59.
     polyorder : int, optional
         Order of the polynomial used by the Savitzky-Golay filter. Default is 1.
     r : int, optional
         Radius of the neighborhood used by the segmentation algorithm. Default is 10.
     lb : float, optional
         Lower bound of the range of values to segment. Default is 0.0.
     ub : float, optional
```

### Comparing `dcarte-0.4.8/pyproject.toml` & `dcarte-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcarte"
-version = "0.4.08"
+version = "0.4.09"
 description = "DCARTE is a dataset ingestion tool from DCARTE UK-DRI CAre Research and TEchnology"
 authors = ["eyal soreq"]
 documentation = "https://esoreq.github.io/dcarte/_build/html/index.html"
 repository = "https://github.com/esoreq/dcarte"
 
 
 [tool.poetry.dependencies]
```

### Comparing `dcarte-0.4.8/setup.py` & `dcarte-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests>=2.26.0,<3.0.0',
  'scipy>=1.7.3,<2.0.0',
  'tqdm>=4.62.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'dcarte',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'DCARTE is a dataset ingestion tool from DCARTE UK-DRI CAre Research and TEchnology',
     'long_description': 'None',
     'author': 'eyal soreq',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/esoreq/dcarte',
```

### Comparing `dcarte-0.4.8/PKG-INFO` & `dcarte-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcarte
-Version: 0.4.8
+Version: 0.4.9
 Summary: DCARTE is a dataset ingestion tool from DCARTE UK-DRI CAre Research and TEchnology
 Home-page: https://github.com/esoreq/dcarte
 Author: eyal soreq
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

