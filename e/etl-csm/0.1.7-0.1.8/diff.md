# Comparing `tmp/etl_csm-0.1.7.tar.gz` & `tmp/etl_csm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.7.tar", last modified: Thu May 25 11:49:20 2023, max compression
+gzip compressed data, was "etl_csm-0.1.8.tar", last modified: Thu May 25 15:06:55 2023, max compression
```

## Comparing `etl_csm-0.1.7.tar` & `etl_csm-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:49:20.978730 etl_csm-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-05-25 11:49:20.973729 etl_csm-0.1.7/Etl/
--rw-rw-rw-   0        0        0     3766 2023-05-25 11:48:03.000000 etl_csm-0.1.7/Etl/Execute.py
--rw-rw-rw-   0        0        0     1619 2023-05-25 11:48:03.000000 etl_csm-0.1.7/Etl/Extrator.py
--rw-rw-rw-   0        0        0     3396 2023-05-22 20:35:16.000000 etl_csm-0.1.7/Etl/Helper.py
--rw-rw-rw-   0        0        0     2344 2023-05-25 11:48:03.000000 etl_csm-0.1.7/Etl/Loader.py
--rw-rw-rw-   0        0        0     6126 2023-05-22 20:35:16.000000 etl_csm-0.1.7/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0     6935 2023-05-24 18:19:00.000000 etl_csm-0.1.7/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0     7798 2023-05-22 20:35:16.000000 etl_csm-0.1.7/Etl/Unique_treatments.py
--rw-rw-rw-   0        0        0      679 2023-05-24 18:21:41.000000 etl_csm-0.1.7/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-05-22 20:35:16.000000 etl_csm-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      548 2023-05-25 11:49:20.977728 etl_csm-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      922 2023-05-25 11:48:03.000000 etl_csm-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:49:20.976729 etl_csm-0.1.7/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      548 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 11:49:20.978730 etl_csm-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-25 11:48:45.000000 etl_csm-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:06:55.755742 etl_csm-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:06:55.750741 etl_csm-0.1.8/Etl/
+-rw-rw-rw-   0        0        0     3747 2023-05-25 15:05:18.000000 etl_csm-0.1.8/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1606 2023-05-25 15:05:04.000000 etl_csm-0.1.8/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     3396 2023-05-22 20:35:16.000000 etl_csm-0.1.8/Etl/Helper.py
+-rw-rw-rw-   0        0        0     2532 2023-05-25 15:03:00.000000 etl_csm-0.1.8/Etl/Loader.py
+-rw-rw-rw-   0        0        0     6126 2023-05-22 20:35:16.000000 etl_csm-0.1.8/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0     6948 2023-05-25 15:02:04.000000 etl_csm-0.1.8/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0     7798 2023-05-22 20:35:16.000000 etl_csm-0.1.8/Etl/Unique_treatments.py
+-rw-rw-rw-   0        0        0      698 2023-05-25 15:01:20.000000 etl_csm-0.1.8/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-05-22 20:35:16.000000 etl_csm-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      548 2023-05-25 15:06:55.754741 etl_csm-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      922 2023-05-25 14:47:15.000000 etl_csm-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 15:06:55.753739 etl_csm-0.1.8/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-05-25 15:06:55.000000 etl_csm-0.1.8/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-05-25 15:06:55.000000 etl_csm-0.1.8/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:06:55.000000 etl_csm-0.1.8/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-25 15:06:55.000000 etl_csm-0.1.8/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-25 15:06:55.000000 etl_csm-0.1.8/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:06:55.755742 etl_csm-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-25 15:06:21.000000 etl_csm-0.1.8/setup.py
```

### Comparing `etl_csm-0.1.7/Etl/Execute.py` & `etl_csm-0.1.8/Etl/Execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .Treatment_extras import (patternizing_columns, ensure_nan_extras, dtype_extras,
                                  fill_na_extras)
 from .Unique_treatments import steps_residential, errors, steps_pme
 from .Helper import timing, json_deserializer
 from .Loader import load_cloud
 
 class Runner:
-    #batatatatata
     """
         Runner é a classe que executa todo o conjunto de funcoes de tratamento.
         Ele tambem inicializa o processo de logs
         ARGS:
             query = String que representa um SQL query valido  
     """
     def __init__(self,query:str,bot:str) -> None:
```

### Comparing `etl_csm-0.1.7/Etl/Extrator.py` & `etl_csm-0.1.8/Etl/Extrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from logging import warning
 from pandas import DataFrame
 from .Helper import timing,helper_columns
 
         
 @timing
 def form_df_tracking(query:str) -> type(DataFrame):
-    # teste
     """
         Extrai os dados do RDS, e transforma em pandas object
         ARGS
             query = Query a ser feita
     """
     try:
         engine = psycopg2.connect(
```

### Comparing `etl_csm-0.1.7/Etl/Helper.py` & `etl_csm-0.1.8/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.7/Etl/Loader.py` & `etl_csm-0.1.8/Etl/Loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import psycopg2
 import sqlalchemy.exc
 from os import environ
 from re import findall
 from logging import info, warning
 from sqlalchemy import create_engine
 from pandas import DataFrame
+from datetime import datetime
 from .Helper import timing,sqlcol
 
 @timing
 def load_cloud(df:DataFrame,bot:str) -> None:
     """
     1- Ira fazer o processo de carregamento para o RDS.
     2- Ira inserir com os datatypes corretos
     3- Em seu exception irá acrescentar a coluna com o datatype varchar faltante para nao quebra toda vez que um extra global e lancado
     ARGS
         df = pd.DataFrame
         bot = Bot que irá ser carregado
     """
+    current_year = datetime.now().year
+    current_month = datetime.now().month
     engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PRD_PASSWORD']}@prd-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
-    tries = 15
     sql_dict = sqlcol(df)
+    # Definindo dict de datatypes
+    tries = 15
     for _ in range(tries):
         try:
-            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',dtype = sql_dict,index = False,chunksize = 10000)
+            df.to_sql(f'{bot}_child_{current_year}_{current_month}',engine_alchemy,if_exists = 'append',dtype = sql_dict,index = False,chunksize = 10000)
             break
         except sqlalchemy.exc.ProgrammingError as error:
                 warning(f"Tivemos um erro {error}")
                 if isinstance(error.orig, psycopg2.errors.UndefinedColumn):
                     warning("Vou executar um handler para ver se consigo resolver!")         
                     engine = psycopg2.connect(
                         database = 'clean_data',
@@ -35,15 +39,15 @@
                         host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
                         port = '5432',
                     )
                     cursor = engine.cursor()
                     column = findall('"(.*?)"',str(error))[0]
                     warning(f"Tive que acrescentar mais uma coluna ao seu dataframe ja existente a coluna foi {column}")
                     query = f"""
-                    ALTER TABLE {bot}_tracking_treated
+                    ALTER TABLE {bot}_child_{current_year}_{current_month}
                     ADD COLUMN {column} VARCHAR NULL;
                     """
                     info(query)
                     cursor.execute(query)
                     engine.commit()
                     tries -= 1
                 else:
```

### Comparing `etl_csm-0.1.7/Etl/Treatment_extras.py` & `etl_csm-0.1.8/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.7/Etl/Treatment_tracking.py` & `etl_csm-0.1.8/Etl/Treatment_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,9 +169,9 @@
         Ira fazer a remocao de acentos e \t charaters da coluna new action
         tambem ira deixar todo mundo em lower
         ARGS
             Dataframe com action sujo
         RETURN
             Dataframe com action limpa
     """
-    df['action'] = df['action'].apply(lambda x : unidecode(x)).str.replace(r'\t|\r|\n','')
+    df['action'] = df['action'].apply(lambda x : unidecode(x)).str.replace(r'\t|\r|\n','',regex = True)
     return df
```

### Comparing `etl_csm-0.1.7/Etl/Unique_treatments.py` & `etl_csm-0.1.8/Etl/Unique_treatments.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.7/LICENSE` & `etl_csm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.7/PKG-INFO` & `etl_csm-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.7/README.md` & `etl_csm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.7/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.8/etl_csm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.7/setup.py` & `etl_csm-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
     author_email = "francisco.froes@globalhitss.com.br",
     description = DESCRIPTION,
     long_description = 'Biblioteca para aproveitar classes de tratamento CSM, direcionada para pet',
     packages = find_packages(),
     url = 'https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl',
     keywords = ['python', 'etl'],
     license = 'MIT',
-    install_requires = ['numpy', 'pandas', 'orjson','SQLAlchemy','psycopg2-binary'],
+    install_requires = ['numpy', 'pandas', 'orjson','SQLAlchemy','psycopg2-binary','undefined'],
     extras_require = {
         'dev':['twine>=4.0.2'],
     },
     classifiers = [
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Operating System :: OS Independent',
```

