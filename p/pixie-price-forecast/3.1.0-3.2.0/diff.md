# Comparing `tmp/pixie_price_forecast-3.1.0.tar.gz` & `tmp/pixie_price_forecast-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixie_price_forecast-3.1.0.tar", last modified: Tue Mar  7 13:44:52 2023, max compression
+gzip compressed data, was "pixie_price_forecast-3.2.0.tar", last modified: Thu May 25 14:58:11 2023, max compression
```

## Comparing `pixie_price_forecast-3.1.0.tar` & `pixie_price_forecast-3.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-03-07 13:44:52.277663 pixie_price_forecast-3.1.0/
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     7250 2023-03-07 13:44:52.277309 pixie_price_forecast-3.1.0/PKG-INFO
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     6667 2022-12-22 09:50:31.000000 pixie_price_forecast-3.1.0/README.md
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)       38 2023-03-07 13:44:52.277785 pixie_price_forecast-3.1.0/setup.cfg
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     1287 2023-03-07 10:40:59.000000 pixie_price_forecast-3.1.0/setup.py
-drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-03-07 13:44:52.259994 pixie_price_forecast-3.1.0/src/
-drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-03-07 13:44:52.264748 pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     7250 2023-03-07 13:44:52.000000 pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/PKG-INFO
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)      607 2023-03-07 13:44:52.000000 pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)        1 2023-03-07 13:44:52.000000 pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)      121 2023-03-07 13:44:52.000000 pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/requires.txt
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)       15 2023-03-07 13:44:52.000000 pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/top_level.txt
-drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-03-07 13:44:52.276273 pixie_price_forecast-3.1.0/src/price_forecast/
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)        0 2022-10-03 15:28:21.000000 pixie_price_forecast-3.1.0/src/price_forecast/__init__.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     6403 2022-12-19 10:02:48.000000 pixie_price_forecast-3.1.0/src/price_forecast/data_quality_reference.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     6708 2023-03-07 10:35:46.000000 pixie_price_forecast-3.1.0/src/price_forecast/data_quality_tools.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     1476 2023-03-07 10:21:34.000000 pixie_price_forecast-3.1.0/src/price_forecast/data_scrapper.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     2876 2022-12-14 09:42:46.000000 pixie_price_forecast-3.1.0/src/price_forecast/drive_connection.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     4814 2022-12-28 12:51:08.000000 pixie_price_forecast-3.1.0/src/price_forecast/etl.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)    32567 2023-02-20 18:06:12.000000 pixie_price_forecast-3.1.0/src/price_forecast/forecaster.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)    16005 2022-12-28 09:59:46.000000 pixie_price_forecast-3.1.0/src/price_forecast/misc.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     4754 2022-12-19 16:12:51.000000 pixie_price_forecast-3.1.0/src/price_forecast/queries_templates.py
--rw-r--r--   0 joseangel.mielgo   (504) staff       (20)      404 2022-11-21 10:01:09.000000 pixie_price_forecast-3.1.0/src/price_forecast/viz_tools.py
+drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-05-25 14:58:11.295103 pixie_price_forecast-3.2.0/
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     7250 2023-05-25 14:58:11.294691 pixie_price_forecast-3.2.0/PKG-INFO
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     6667 2022-12-22 09:50:31.000000 pixie_price_forecast-3.2.0/README.md
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)       38 2023-05-25 14:58:11.295233 pixie_price_forecast-3.2.0/setup.cfg
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     1287 2023-05-25 14:58:07.000000 pixie_price_forecast-3.2.0/setup.py
+drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-05-25 14:58:11.274880 pixie_price_forecast-3.2.0/src/
+drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-05-25 14:58:11.281849 pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     7250 2023-05-25 14:58:11.000000 pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)      607 2023-05-25 14:58:11.000000 pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)        1 2023-05-25 14:58:11.000000 pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)      121 2023-05-25 14:58:11.000000 pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/requires.txt
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)       15 2023-05-25 14:58:11.000000 pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 joseangel.mielgo   (504) staff       (20)        0 2023-05-25 14:58:11.293824 pixie_price_forecast-3.2.0/src/price_forecast/
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)        0 2022-10-03 15:28:21.000000 pixie_price_forecast-3.2.0/src/price_forecast/__init__.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     8038 2023-05-25 11:46:46.000000 pixie_price_forecast-3.2.0/src/price_forecast/data_quality_reference.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     6708 2023-03-07 10:35:46.000000 pixie_price_forecast-3.2.0/src/price_forecast/data_quality_tools.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     1476 2023-03-07 10:21:34.000000 pixie_price_forecast-3.2.0/src/price_forecast/data_scrapper.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     2876 2022-12-14 09:42:46.000000 pixie_price_forecast-3.2.0/src/price_forecast/drive_connection.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     4814 2022-12-28 12:51:08.000000 pixie_price_forecast-3.2.0/src/price_forecast/etl.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)    33847 2023-05-25 14:49:39.000000 pixie_price_forecast-3.2.0/src/price_forecast/forecaster.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)    16073 2023-05-25 08:44:23.000000 pixie_price_forecast-3.2.0/src/price_forecast/misc.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)     4754 2022-12-19 16:12:51.000000 pixie_price_forecast-3.2.0/src/price_forecast/queries_templates.py
+-rw-r--r--   0 joseangel.mielgo   (504) staff       (20)      404 2022-11-21 10:01:09.000000 pixie_price_forecast-3.2.0/src/price_forecast/viz_tools.py
```

### Comparing `pixie_price_forecast-3.1.0/PKG-INFO` & `pixie_price_forecast-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixie_price_forecast
-Version: 3.1.0
+Version: 3.2.0
 Summary: Price forecast tools.
 Home-page: https://github.mpi-internal.com/joseangel-mielgo/pixie-price-forecast
 Author: Pixie Pixel
 Author-email: joseangel.mielgo@adevinta.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.mpi-internal.com/joseangel-mielgo/pixie-price-forecast
 Platform: UNKNOWN
```

### Comparing `pixie_price_forecast-3.1.0/README.md` & `pixie_price_forecast-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pixie_price_forecast-3.1.0/setup.py` & `pixie_price_forecast-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pixie_price_forecast",
-    version="3.1.0",
+    version="3.2.0",
     author="Pixie Pixel",
     author_email="joseangel.mielgo@adevinta.com",
     description="Price forecast tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.mpi-internal.com/joseangel-mielgo/pixie-price-forecast",
     project_urls={
```

### Comparing `pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/PKG-INFO` & `pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixie-price-forecast
-Version: 3.1.0
+Version: 3.2.0
 Summary: Price forecast tools.
 Home-page: https://github.mpi-internal.com/joseangel-mielgo/pixie-price-forecast
 Author: Pixie Pixel
 Author-email: joseangel.mielgo@adevinta.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.mpi-internal.com/joseangel-mielgo/pixie-price-forecast
 Platform: UNKNOWN
```

### Comparing `pixie_price_forecast-3.1.0/src/pixie_price_forecast.egg-info/SOURCES.txt` & `pixie_price_forecast-3.2.0/src/pixie_price_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/data_quality_reference.py` & `pixie_price_forecast-3.2.0/src/price_forecast/data_quality_reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,28 +104,48 @@
         'perc_price_05': min,
         'perc_price_01': min,
         'visits': sum,
         'leads': sum
     }
 }
 mode_dict = {
+    'demand_flat_rent': {'variables': {'is_professional': True, 'leads_only': True, 'operation_type': 'is_rent'},
+                         'name_export_file': 'agg_prices_demand_rent.csv'},
+    'offer_flat_rent': {'variables': {'is_professional': True, 'leads_only': False, 'operation_type': 'is_rent'},
+                        'name_export_file': 'agg_prices_offer_rent.csv'},
+    'demand_houses_rent': {'variables': {'is_professional': True, 'leads_only': True,
+                                         'prop_type': 'house', 'operation_type': 'is_rent'},
+                           'name_export_file': 'agg_prices_demand_houses_rent.csv'},
+    'offer_houses_rent': {'variables': {'is_professional': True, 'leads_only': False,
+                                        'operation_type': 'is_rent', 'prop_type': 'house'},
+                          'name_export_file': 'agg_prices_demand_houses_rent.csv'},
+    'demand_flat_sell': {'variables': {'is_professional': True, 'leads_only': True},
+                         'name_export_file': 'agg_prices_demand_sell.csv'},
+    'offer_flat_sell': {'variables': {'is_professional': True, 'leads_only': False},
+                        'name_export_file': 'agg_prices_offer_sell.csv'},
+    'demand_houses_sell': {'variables': {'is_professional': True, 'leads_only': True, 'prop_type': 'house'},
+                           'name_export_file': 'agg_prices_demand_houses_sell.csv'},
+    'offer_houses_sell': {'variables': {'is_professional': True, 'leads_only': False, 'prop_type': 'house'},
+                          'name_export_file': 'agg_prices_offer_houses_sell.csv'}
+}
+mode_dict_deprecated = {
     'demand_flat_rent': {'variables': {'is_professional': False, 'leads_only': True, 'operation_type': 'is_rent'},
                          'name_export_file': 'agg_prices_demand_rent.csv'},
     'offer_flat_rent': {'variables': {'is_professional': False, 'leads_only': False, 'operation_type': 'is_rent'},
                         'name_export_file': 'agg_prices_offer_rent.csv'},
     'professionals_flat_rent': {'variables': {'is_professional': True, 'leads_only': True, 'operation_type': 'is_rent'},
                                 'name_export_file': 'agg_prices_pro_rent.csv'},
     'demand_houses_rent': {'variables': {'is_professional': False, 'leads_only': True,
                                          'prop_type': 'house', 'operation_type': 'is_rent'},
                            'name_export_file': 'agg_prices_demand_houses_rent.csv'},
     'offer_houses_rent': {'variables': {'is_professional': False, 'leads_only': False,
                                         'operation_type': 'is_rent', 'prop_type': 'house'},
                           'name_export_file': 'agg_prices_demand_houses_rent.csv'},
     'professionals_houses_rent': {'variables': {'is_professional': True, 'leads_only': True,
-                                                'operation_type': 'is_rent',  'prop_type': 'house'},
+                                                'operation_type': 'is_rent', 'prop_type': 'house'},
                                   'name_export_file': 'agg_prices_pro_houses_rent.csv'},
     'demand_flat_sell': {'variables': {'is_professional': False, 'leads_only': True},
                          'name_export_file': 'agg_prices_demand_sell.csv'},
     'offer_flat_sell': {'variables': {'is_professional': False, 'leads_only': False},
                         'name_export_file': 'agg_prices_offer_sell.csv'},
     'professionals_flat_sell': {'variables': {'is_professional': True, 'leads_only': True},
                                 'name_export_file': 'agg_prices_pro_sell.csv'},
```

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/data_quality_tools.py` & `pixie_price_forecast-3.2.0/src/price_forecast/data_quality_tools.py`

 * *Files identical despite different names*

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/data_scrapper.py` & `pixie_price_forecast-3.2.0/src/price_forecast/data_scrapper.py`

 * *Files identical despite different names*

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/drive_connection.py` & `pixie_price_forecast-3.2.0/src/price_forecast/drive_connection.py`

 * *Files identical despite different names*

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/etl.py` & `pixie_price_forecast-3.2.0/src/price_forecast/etl.py`

 * *Files identical despite different names*

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/forecaster.py` & `pixie_price_forecast-3.2.0/src/price_forecast/forecaster.py`

 * *Files 4% similar despite different names*

```diff
@@ -616,31 +616,33 @@
 
 
 def run_forecast(model_name: str,
                  input_path: str,
                  province_list: list,
                  search_grid: dict,
                  train_from: str, operation_type: str, db_engine,
-                 train_to: str, max_date: str, mode: str = 'pixie', horizon: int = 12):
+                 train_to: str, max_date: str, mode: str = 'pixie', horizon: int = 12, debug: bool = False):
     """
-
-    :param data_source:
-    :param model_name: Model as in run_dict
-    :param input_path: Location of input data.
+    Call forecast algorithm using parameters
+    :param max_date: last month to be used in the test set. Test set goes from train_to+1 to max_date, both inclusive.
+    :param model_name: Model key as in run_dict: arima, random_forest, nn.
+    :param input_path: Name of the forecast: key from mode_dict (from data_quality_reference)
     :param province_list: List of provinces to be forecasted.
     :param search_grid: Dictionary containing the search space
     :param operation_type: rent or buy.
     :param db_engine: Database Engine
-    :param train_from: Start date for backtesting
-    :param train_to: End date for backtesting
-    :param mode: Mode of loading data (csv, s3, etc.)
-    :param horizon: Number of months
+    :param train_from: Start date for backtesting.
+    :param train_to: End date for backtesting (not inclusive in training).
+    :param mode: Mode of loading data (csv, s3, etc.). pixie gets data from Datavenues.
+    :param horizon: Number of months to be forecasted.
+    :param debug: Do nothing
     :return: Export forecast with format model_name.csv. It contains history with the forecast and interval of
     confidence.
     """
+    t0 = datetime.now()
     list_res = list()
     input_model = {'mode': mode, 'train_from': train_from, 'train_to': train_to, 'date_col_name': 'version_date',
                    'input_path': input_path, 'horizon': horizon, 'max_date': max_date, 'db_engine': db_engine}
     if 'rent' in operation_type:
         input_model['target'] = 'mean_price'
     else:
         input_model['target'] = 'mean_unitary_price'
@@ -658,59 +660,78 @@
     list_res = pd.concat(list_res)
     list_res['model'] = model_name
     list_res['target_name'] = input_model['target']
     list_res.rename({input_model['target']: 'target'}, axis=1, inplace=True)
     list_res['forecast_date'] = datetime.strftime(datetime.today(), '%Y-%m-%d')
     list_res['tag_use'] = True
     list_res['extraction_type'] = input_path
-    list_res.to_sql('price_forecasts', db_engine, if_exists='append')
+    if debug:
+        print(f'{model_name} took {datetime.now()-t0}')
+    else:
+        list_res.to_sql('price_forecasts', db_engine, if_exists='append')
 
 
-def run_all_forecasts(credentials: dict, train_from, train_to, max_date):
+def run_all_forecasts(credentials: dict, train_from, train_to, max_date, debug: bool = False):
+    """
+    Run all the forecast models defined in models_dict. This function contains the setup of grid search.
+    :param credentials: Credentials to connect to Datavenues.
+    :param train_from: Training set is defined as (train_from, train_to). format '%Y-%m-%d'
+    :param train_to: Last day of training data (This month is not inclusive).
+    :param max_date: Last day that defines test set. test_set = (train_to, max_date) both inclusive.
+    :param debug:
+    :return: Appends forecasts in table price_forecasts in datavenues.
+    """
     tunnel_server = setup_tunnel(ssh_user=credentials['ssh_user'],
                                  ssh_pass=credentials['ssh_pass'],
                                  ssh_host=credentials['ssh_host'],
                                  ssh_port=credentials['ssh_port'],
                                  host=credentials['host'],
                                  port=credentials['port'])
     tunnel_server.start()
     local_port = tunnel_server.local_bind_port
     pixie_engine = create_pixie_engine(local_port=local_port,
                                        user=credentials['user'],
                                        password=credentials['password'],
                                        db_name=credentials['db_name'])
-    q = reset_use_tag('price_forecasts')
-    pixie_engine.execute(q)
+    if not debug:
+        # This deprecates the last forecast
+        q = reset_use_tag('price_forecasts')
+        pixie_engine.execute(q)
     for data_source, _ in mode_dict.items():
         print(data_source)
+        if (data_source != 'demand_flat_sell') and debug:
+            continue
         path = data_source
         op_type = data_source
-        df = pd.read_sql(query_read_data(table_name='price_clean_data', mode=data_source, use_tag=True),
-                         pixie_engine)
-        provinces = df.province.unique()
+        if debug:
+            provinces = ['Barcelona', 'Madrid']
+        else:
+            df = pd.read_sql(query_read_data(table_name='price_clean_data', mode=data_source, use_tag=True),
+                             pixie_engine)
+            provinces = df.province.unique()
         # Arima
         search_grid = {'autoregression': [2, 3, 4, 5], 'order': [1, 2], 'm_avg': [0, 1, 2]}
         run_forecast(model_name='arima', input_path=path, province_list=provinces,
                      search_grid=search_grid, train_from=train_from, train_to=train_to,
                      operation_type=op_type, max_date=max_date,
-                     db_engine=pixie_engine, horizon=3)
+                     db_engine=pixie_engine, horizon=3, debug=debug)
         # NN
         run_forecast(model_name='nn', input_path=path, province_list=provinces,
                      search_grid=search_grid, train_from=train_from, train_to=train_to,
                      operation_type=op_type, max_date=max_date,
-                     horizon=3, db_engine=pixie_engine)
+                     horizon=3, db_engine=pixie_engine, debug=debug)
         # RF
         search_grid = {'bootstrap': [False],
-                       'max_depth': [10, 20, 30, 40, 50],
+                       'max_depth': [10, 30, 50],
                        'max_features': ['auto'],
-                       'min_samples_leaf': [1, 2, 4],
-                       'min_samples_split': [2, 5, 10],
+                       'min_samples_leaf': [1],
+                       'min_samples_split': [2],
                        'n_estimators': [100, 200, 400]}
         run_forecast(model_name='random_forest', input_path=path, province_list=provinces,
                      search_grid=search_grid, train_from=train_from, train_to=train_to,
                      operation_type=op_type, max_date=max_date,
-                     db_engine=pixie_engine, horizon=3)
+                     db_engine=pixie_engine, horizon=3, debug=debug)
     tunnel_server.stop()
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/misc.py` & `pixie_price_forecast-3.2.0/src/price_forecast/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,18 +167,18 @@
 
 
 def join_datasets(db_engine,
                   date_col: str = 'datetime',
                   province_col: str = 'province'):
     """
     Join all predictions into a single dataset for reporting purposes.
-    :param db_engine:
+    :param db_engine: Engine to connect to datavenues.
     :param date_col: Name of the common date column.
     :param province_col: Name of the common column containing province.
-    :return:
+    :return: Save results in price_viz_forecast
     """
     all_df = list()
     for mode_name, _ in mode_dict.items():
         print(mode_name)
         models = ['nn', 'random_forest', 'arima']
         df = pd.read_sql(query_read_data(table_name='price_forecasts', mode=mode_name, use_tag=True), db_engine)
         for mod in models:
```

### Comparing `pixie_price_forecast-3.1.0/src/price_forecast/queries_templates.py` & `pixie_price_forecast-3.2.0/src/price_forecast/queries_templates.py`

 * *Files identical despite different names*

