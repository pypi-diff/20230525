# Comparing `tmp/datacollectors-0.6.8.tar.gz` & `tmp/datacollectors-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacollectors-0.6.8.tar", last modified: Sun Apr  2 09:40:01 2023, max compression
+gzip compressed data, was "datacollectors-0.6.9.tar", last modified: Mon Apr  3 06:20:49 2023, max compression
```

## Comparing `datacollectors-0.6.8.tar` & `datacollectors-0.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 09:40:01.516923 datacollectors-0.6.8/
--rw-rw-rw-   0        0        0    35801 2022-08-09 09:34:43.000000 datacollectors-0.6.8/LICENCE.txt
--rw-rw-rw-   0        0        0      617 2023-04-02 09:40:01.514389 datacollectors-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      303 2022-08-09 09:34:43.000000 datacollectors-0.6.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-02 09:40:01.516923 datacollectors-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-04-02 09:39:20.000000 datacollectors-0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 09:40:01.497773 datacollectors-0.6.8/src/
--rw-rw-rw-   0        0        0      585 2022-08-09 09:34:43.000000 datacollectors-0.6.8/src/datacollector_Boliga.py
--rw-rw-rw-   0        0        0     1407 2022-08-09 09:34:43.000000 datacollectors-0.6.8/src/datacollector_Business_insider.py
--rw-rw-rw-   0        0        0     2637 2022-08-09 09:34:43.000000 datacollectors-0.6.8/src/datacollector_ECB.py
--rw-rw-rw-   0        0        0    13905 2023-03-14 15:49:53.000000 datacollectors-0.6.8/src/datacollector_Entsoe.py
--rw-rw-rw-   0        0        0     2880 2023-01-10 13:56:26.000000 datacollectors-0.6.8/src/datacollector_ICE.py
--rw-rw-rw-   0        0        0     5836 2023-03-14 16:15:15.000000 datacollectors-0.6.8/src/datacollector_energidataservice.py
--rw-rw-rw-   0        0        0     3045 2023-04-02 09:38:08.000000 datacollectors-0.6.8/src/datacollector_trading_economics.py
-drwxrwxrwx   0        0        0        0 2023-04-02 09:40:01.510870 datacollectors-0.6.8/src/datacollectors.egg-info/
--rw-rw-rw-   0        0        0      617 2023-04-02 09:40:01.000000 datacollectors-0.6.8/src/datacollectors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-04-02 09:40:01.000000 datacollectors-0.6.8/src/datacollectors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 09:40:01.000000 datacollectors-0.6.8/src/datacollectors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-02 09:40:01.000000 datacollectors-0.6.8/src/datacollectors.egg-info/requires.txt
--rw-rw-rw-   0        0        0      188 2023-04-02 09:40:01.000000 datacollectors-0.6.8/src/datacollectors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      701 2023-03-14 15:49:53.000000 datacollectors-0.6.8/src/datacollectors.py
+drwxrwxrwx   0        0        0        0 2023-04-03 06:20:49.718101 datacollectors-0.6.9/
+-rw-rw-rw-   0        0        0    35801 2022-08-09 09:34:43.000000 datacollectors-0.6.9/LICENCE.txt
+-rw-rw-rw-   0        0        0      617 2023-04-03 06:20:49.716089 datacollectors-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2022-08-09 09:34:43.000000 datacollectors-0.6.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-03 06:20:49.719097 datacollectors-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-04-03 06:20:43.000000 datacollectors-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-03 06:20:49.692721 datacollectors-0.6.9/src/
+-rw-rw-rw-   0        0        0      585 2022-08-09 09:34:43.000000 datacollectors-0.6.9/src/datacollector_Boliga.py
+-rw-rw-rw-   0        0        0     1407 2022-08-09 09:34:43.000000 datacollectors-0.6.9/src/datacollector_Business_insider.py
+-rw-rw-rw-   0        0        0     2637 2022-08-09 09:34:43.000000 datacollectors-0.6.9/src/datacollector_ECB.py
+-rw-rw-rw-   0        0        0    13905 2023-03-14 15:49:53.000000 datacollectors-0.6.9/src/datacollector_Entsoe.py
+-rw-rw-rw-   0        0        0     2880 2023-01-10 13:56:26.000000 datacollectors-0.6.9/src/datacollector_ICE.py
+-rw-rw-rw-   0        0        0     5836 2023-03-14 16:15:15.000000 datacollectors-0.6.9/src/datacollector_energidataservice.py
+-rw-rw-rw-   0        0        0     3144 2023-04-03 06:20:43.000000 datacollectors-0.6.9/src/datacollector_trading_economics.py
+drwxrwxrwx   0        0        0        0 2023-04-03 06:20:49.712121 datacollectors-0.6.9/src/datacollectors.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-04-03 06:20:49.000000 datacollectors-0.6.9/src/datacollectors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-04-03 06:20:49.000000 datacollectors-0.6.9/src/datacollectors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-03 06:20:49.000000 datacollectors-0.6.9/src/datacollectors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-03 06:20:49.000000 datacollectors-0.6.9/src/datacollectors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      188 2023-04-03 06:20:49.000000 datacollectors-0.6.9/src/datacollectors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      701 2023-03-14 15:49:53.000000 datacollectors-0.6.9/src/datacollectors.py
```

### Comparing `datacollectors-0.6.8/LICENCE.txt` & `datacollectors-0.6.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/PKG-INFO` & `datacollectors-0.6.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacollectors
-Version: 0.6.8
+Version: 0.6.9
 Summary: datacollectors
 Author: Torben Franch
 Author-email: torben@franch.eu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `datacollectors-0.6.8/setup.py` & `datacollectors-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 py_modules = [f.stem for f in (Path(__file__).parent / 'src').glob('*.py') if f.stem[0] !='_']
 
 
 
 setup(
 
     name='datacollectors',
-    version='0.6.8',
+    version='0.6.9',
     description='datacollectors',
     py_modules=py_modules,
     package_dir={'':'src'},
     install_requires=['tabulate', 'incentivedkutils', 'requests', 'xmltodict'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8'],
```

### Comparing `datacollectors-0.6.8/src/datacollector_Boliga.py` & `datacollectors-0.6.9/src/datacollector_Boliga.py`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/src/datacollector_Business_insider.py` & `datacollectors-0.6.9/src/datacollector_Business_insider.py`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/src/datacollector_ECB.py` & `datacollectors-0.6.9/src/datacollector_ECB.py`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/src/datacollector_Entsoe.py` & `datacollectors-0.6.9/src/datacollector_Entsoe.py`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/src/datacollector_ICE.py` & `datacollectors-0.6.9/src/datacollector_ICE.py`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/src/datacollector_energidataservice.py` & `datacollectors-0.6.9/src/datacollector_energidataservice.py`

 * *Files identical despite different names*

### Comparing `datacollectors-0.6.8/src/datacollector_trading_economics.py` & `datacollectors-0.6.9/src/datacollector_trading_economics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-import os
+import re
 from datetime import datetime, timedelta
-from pathlib import Path
-import sys
+
 import incentivedkutils as utils
 import requests
-import re
 
 
 def main():
-    start_date=datetime(2021,1,1)
-    for commodity in ['ttf_gas','urea_ammonium','EUA','brent_oil'][-1:]:
-        indata_list=Trading_economics.commodity_prices_df(commodity,start_date)
-        utils.prt(indata_list[-10:])
+    start_date = datetime(2019, 1, 1)
+    for commodity in ['ttf_gas', 'urea_ammonium', 'EUA', 'brent_oil'][-1:]:
+        indata_list = Trading_economics.commodity_prices_df(commodity, start_date)
+        utils.prt(indata_list[:10])
+
 
 class Trading_economics():
     @staticmethod
     def commodity_prices_df(commodity, start_date):
         import pandas as pd
         indata_list = Trading_economics.commodity_prices(commodity, start_date)
         df = pd.DataFrame(indata_list)
+        df = df.set_index('date')
+        df = df.resample('D').ffill()
         return df
 
     @staticmethod
-    def commodity_prices(commodity,start_date):
-        indata_list=[]
+    def commodity_prices(commodity, start_date):
+        indata_list = []
         commodity_list = Trading_economics._read_commodity_list()
-        period_length=int((datetime.today()-start_date)/timedelta(days=1))+1
+        period_length = int((datetime.today() - start_date) / timedelta(days=1)) + 1
         if commodity in [d['commodity'] for d in commodity_list]:
-            links_dict=[d for d in commodity_list if d['commodity'] == commodity][0]
-            url_site=links_dict['url_site']
-            auth=Trading_economics._get_auth(url_site)
-            url=f"{links_dict['url_data']}&span={period_length}d&AUTH={auth}"
-            indata=requests.get(url).json()
-            indata_list=[{'date': datetime.fromtimestamp(int(obs['x']/1000))-timedelta(hours=1), commodity: obs['y']} for obs in indata['series'][0]['data']]
+            links_dict = [d for d in commodity_list if d['commodity'] == commodity][0]
+            url_site = links_dict['url_site']
+            auth = Trading_economics._get_auth(url_site)
+            url = f"{links_dict['url_data']}&span={period_length}d&AUTH={auth}"
+            indata = requests.get(url).json()
+            indata_list = [
+                {'date': datetime.fromtimestamp(int(obs['x'] / 1000)) - timedelta(hours=1), commodity: obs['y']} for obs
+                in indata['series'][0]['data']]
         return indata_list
 
     @classmethod
     def _get_auth(cls, url_site):
         headers = {"User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:86.0) Gecko/20100101 Firefox/86.0"}
         with requests.Session() as s:
             in_string = s.get(url_site, headers=headers).text
         pattern = re.compile('TESecurify = (.*)')
         match = pattern.findall(in_string)[-1:]
         auth = str(match[0][1:-3])
         return auth
 
     @classmethod
     def _read_commodity_list(cls):
-        commodity_list=[
+        commodity_list = [
             {'commodity': 'ttf_gas', 'url_site': 'https://tradingeconomics.com/commodity/eu-natural-gas',
-              'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/eu-natural-gas&s=ngeu:com'},
+             'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/eu-natural-gas&s=ngeu:com'},
             {'commodity': 'urea_ammonium', 'url_site': 'https://tradingeconomics.com/commodity/urea-ammonium',
-              'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/urea-ammonium&s=uaneu:com'},
+             'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/urea-ammonium&s=uaneu:com'},
             {'commodity': 'brent_oil', 'url_site': 'https://tradingeconomics.com/commodity/brent-crude-oil',
              'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/brent-crude-oil&s=co1:com'},
             {'commodity': 'EUA', 'url_site': 'https://tradingeconomics.com/commodity/carbon',
-              'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/carbon&s=eecxm:ind'},
+             'url_data': 'https://markets.tradingeconomics.com/chart?interval=1d&securify=new&url=/commodity/carbon&s=eecxm:ind'},
         ]
         return commodity_list
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `datacollectors-0.6.8/src/datacollectors.egg-info/PKG-INFO` & `datacollectors-0.6.9/src/datacollectors.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacollectors
-Version: 0.6.8
+Version: 0.6.9
 Summary: datacollectors
 Author: Torben Franch
 Author-email: torben@franch.eu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `datacollectors-0.6.8/src/datacollectors.py` & `datacollectors-0.6.9/src/datacollectors.py`

 * *Files identical despite different names*

