# Comparing `tmp/abuscom-libs-0.1.6.tar.gz` & `tmp/abuscom-libs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuscom-libs-0.1.6.tar", last modified: Mon Apr 24 10:03:14 2023, max compression
+gzip compressed data, was "abuscom-libs-0.1.7.tar", last modified: Thu May 25 06:53:26 2023, max compression
```

## Comparing `abuscom-libs-0.1.6.tar` & `abuscom-libs-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.772857 abuscom-libs-0.1.6/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-24 10:03:14.772381 abuscom-libs-0.1.6/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.6/README.md
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.759965 abuscom-libs-0.1.6/abuscom/
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.767988 abuscom-libs-0.1.6/abuscom/connectors/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.6/abuscom/connectors/__init__.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     1887 2023-04-19 09:17:07.000000 abuscom-libs-0.1.6/abuscom/connectors/compass.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     8401 2023-04-13 12:20:45.000000 abuscom-libs-0.1.6/abuscom/connectors/hubspot.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6017 2023-04-24 10:02:05.000000 abuscom-libs-0.1.6/abuscom/connectors/oracle.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.6/abuscom/connectors/planio.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.6/abuscom/connectors/postgres.py
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.771789 abuscom-libs-0.1.6/abuscom_libs.egg-info/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/SOURCES.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/dependency_links.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/requires.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/top_level.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-24 10:03:14.772991 abuscom-libs-0.1.6/setup.cfg
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-24 10:02:05.000000 abuscom-libs-0.1.6/setup.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.983530 abuscom-libs-0.1.7/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-25 06:53:26.983093 abuscom-libs-0.1.7/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.7/README.md
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.974801 abuscom-libs-0.1.7/abuscom/
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.979602 abuscom-libs-0.1.7/abuscom/connectors/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.7/abuscom/connectors/__init__.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     1887 2023-04-19 09:17:07.000000 abuscom-libs-0.1.7/abuscom/connectors/compass.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     8661 2023-05-25 06:52:16.000000 abuscom-libs-0.1.7/abuscom/connectors/hubspot.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6017 2023-04-24 10:02:05.000000 abuscom-libs-0.1.7/abuscom/connectors/oracle.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.7/abuscom/connectors/planio.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.7/abuscom/connectors/postgres.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.982396 abuscom-libs-0.1.7/abuscom_libs.egg-info/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/requires.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/top_level.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-05-25 06:53:26.983688 abuscom-libs-0.1.7/setup.cfg
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-05-25 06:52:34.000000 abuscom-libs-0.1.7/setup.py
```

### Comparing `abuscom-libs-0.1.6/README.md` & `abuscom-libs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.6/abuscom/connectors/compass.py` & `abuscom-libs-0.1.7/abuscom/connectors/compass.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.6/abuscom/connectors/hubspot.py` & `abuscom-libs-0.1.7/abuscom/connectors/hubspot.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         except KeyError:
             tuple = tuple + ('UNDEFINED',)
         return tuple
 
     def read_deals(self, colNames):
 
 
-        dealsEndpoint = "/crm/v4/objects/deals?limit=100&properties=critical_opp_review&properties=dealname&properties=dealType&properties=dealstage&properties=amount&properties=deal_currency_code&properties=hy2_market&properties=hy2_product&properties=hy2_application&properties=hubspot_owner_id&properties=hs_deal_stage_probability&properties=hs_exchange_rate&properties=of_systems&properties=expected_delivery&properties=h2_kg_&properties=hy2_battery&properties=hy2_storage&properties=hs_object_id&properties=electrolyzer&properties=sales_team&properties=hy_invoice_co_&properties=hy_mfg_co_&associations=companies"
+        dealsEndpoint = "/crm/v4/objects/deals?limit=100&properties=closed_lost_category&properties=critical_opp_review&properties=dealname&properties=dealType&properties=dealstage&properties=amount&properties=deal_currency_code&properties=hy2_market&properties=hy2_product&properties=hy2_application&properties=hubspot_owner_id&properties=hs_deal_stage_probability&properties=hs_exchange_rate&properties=of_systems&properties=expected_delivery&properties=h2_kg_&properties=hy2_battery&properties=hy2_storage&properties=hs_object_id&properties=electrolyzer&properties=sales_team&properties=hy_invoice_co_&properties=hy_mfg_co_&associations=companies"
         dealList = self.__read_page(endpoint=dealsEndpoint, resultProperty='results')
         try:
             data = [*map(lambda x: self.__companyToTuple(x, colNames), dealList)]
             return data
 
         except (JSONDecodeError, LookupError, AirflowException) as ex:
             print(ex)
@@ -143,28 +143,30 @@
         companiesResponse = HttpHook(method="GET", http_conn_id=self.__hubspot_conn_id).run(companiesPropertiesEndpoint)
         try:
             dealsResult = json.loads(dealsResponse.content)["results"]
             hy2Applications = [*filter(lambda x: x['name'] == "hy2_application", dealsResult)][0]['options']
             hy2Markets = [*filter(lambda x: x['name'] == "hy2_market", dealsResult)][0]['options']
             dealtypes = [*filter(lambda x: x['name'] == "dealtype", dealsResult)][0]['options']
             hy2Products = [*filter(lambda x: x['name'] == "hy2_product", dealsResult)][0]['options']
+            closedLostCategory = [*filter(lambda x: x['name'] == "closed_lost_category", dealsResult)][0]['options']
             expectedDeliveries = [*filter(lambda x: x['name'] == "expected_delivery", dealsResult)][0]['options']
             hy2Batteries = [*filter(lambda x: x['name'] == "hy2_battery", dealsResult)][0]['options']
             hy2Storages = [*filter(lambda x: x['name'] == "hy2_storage", dealsResult)][0]['options']
             electrolyzers = [*filter(lambda x: x['name'] == "electrolyzer", dealsResult)][0]['options']
             salesteams = [*filter(lambda x: x['name'] == "sales_team", dealsResult)][0]['options']
 
             companiesResult = json.loads(companiesResponse.content)["results"]
             industries = [*filter(lambda x: x['name'] == "industry", companiesResult)][0]['options']
             types = [*filter(lambda x: x['name'] == "type", companiesResult)][0]['options']
 
             data = [*map(lambda x: self.__labelToTuple('hy2_application', x), hy2Applications)]
             data = data + [*map(lambda x: self.__labelToTuple('hy2_market', x), hy2Markets)]
             data = data + [*map(lambda x: self.__labelToTuple('dealtype', x), dealtypes)]
             data = data + [*map(lambda x: self.__labelToTuple('hy2_product', x), hy2Products)]
+            data = data + [*map(lambda x: self.__labelToTuple('closed_lost_category', x), closedLostCategory)]
             data = data + [*map(lambda x: self.__labelToTuple('expected_delivery', x), expectedDeliveries)]
             data = data + [*map(lambda x: self.__labelToTuple('hy2_battery', x), hy2Batteries)]
             data = data + [*map(lambda x: self.__labelToTuple('hy2_storage', x), hy2Storages)]
             data = data + [*map(lambda x: self.__labelToTuple('electrolyzer', x), electrolyzers)]
             data = data + [*map(lambda x: self.__labelToTuple('salesteam', x), salesteams)]
 
             data = data + [*map(lambda x: self.__labelToTuple('industry', x), industries)]
```

### Comparing `abuscom-libs-0.1.6/abuscom/connectors/oracle.py` & `abuscom-libs-0.1.7/abuscom/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.6/abuscom/connectors/planio.py` & `abuscom-libs-0.1.7/abuscom/connectors/planio.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.6/abuscom/connectors/postgres.py` & `abuscom-libs-0.1.7/abuscom/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.6/setup.py` & `abuscom-libs-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='abuscom-libs',
-    version='0.1.6',
+    version='0.1.7',
     description='Utility classes for airflow DAGs',
     url='https://abuscom.com',
     author='Leonhard Holzer',
     author_email='leonhard.holzer@abuscom.com',
     license='BSD 2-clause',
     packages=['abuscom.connectors'],
     install_requires=['apache-airflow>=2.4.3',
```

