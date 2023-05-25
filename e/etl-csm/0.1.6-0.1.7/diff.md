# Comparing `tmp/etl_csm-0.1.6.tar.gz` & `tmp/etl_csm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.6.tar", last modified: Mon Apr 24 14:59:51 2023, max compression
+gzip compressed data, was "etl_csm-0.1.7.tar", last modified: Thu May 25 11:49:20 2023, max compression
```

## Comparing `etl_csm-0.1.6.tar` & `etl_csm-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:59:51.549074 etl_csm-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:59:51.544074 etl_csm-0.1.6/Etl/
--rw-rw-rw-   0        0        0     3379 2023-04-24 14:33:51.000000 etl_csm-0.1.6/Etl/Execute.py
--rw-rw-rw-   0        0        0     1547 2023-04-24 14:33:51.000000 etl_csm-0.1.6/Etl/Extrator.py
--rw-rw-rw-   0        0        0     2768 2023-04-24 14:52:17.000000 etl_csm-0.1.6/Etl/Helper.py
--rw-rw-rw-   0        0        0     1966 2023-04-24 14:59:10.000000 etl_csm-0.1.6/Etl/Loader.py
--rw-rw-rw-   0        0        0     5006 2023-04-24 14:48:37.000000 etl_csm-0.1.6/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.6/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.6/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.6/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-24 14:59:51.548074 etl_csm-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:59:51.548074 etl_csm-0.1.6/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-24 14:59:51.000000 etl_csm-0.1.6/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-24 14:59:51.000000 etl_csm-0.1.6/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:59:51.000000 etl_csm-0.1.6/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-24 14:59:51.000000 etl_csm-0.1.6/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 14:59:51.000000 etl_csm-0.1.6/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 14:59:51.549074 etl_csm-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      911 2023-04-24 14:51:43.000000 etl_csm-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 11:49:20.978730 etl_csm-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-05-25 11:49:20.973729 etl_csm-0.1.7/Etl/
+-rw-rw-rw-   0        0        0     3766 2023-05-25 11:48:03.000000 etl_csm-0.1.7/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1619 2023-05-25 11:48:03.000000 etl_csm-0.1.7/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     3396 2023-05-22 20:35:16.000000 etl_csm-0.1.7/Etl/Helper.py
+-rw-rw-rw-   0        0        0     2344 2023-05-25 11:48:03.000000 etl_csm-0.1.7/Etl/Loader.py
+-rw-rw-rw-   0        0        0     6126 2023-05-22 20:35:16.000000 etl_csm-0.1.7/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0     6935 2023-05-24 18:19:00.000000 etl_csm-0.1.7/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0     7798 2023-05-22 20:35:16.000000 etl_csm-0.1.7/Etl/Unique_treatments.py
+-rw-rw-rw-   0        0        0      679 2023-05-24 18:21:41.000000 etl_csm-0.1.7/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-05-22 20:35:16.000000 etl_csm-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      548 2023-05-25 11:49:20.977728 etl_csm-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      922 2023-05-25 11:48:03.000000 etl_csm-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 11:49:20.976729 etl_csm-0.1.7/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-25 11:49:20.000000 etl_csm-0.1.7/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 11:49:20.978730 etl_csm-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-05-25 11:48:45.000000 etl_csm-0.1.7/setup.py
```

### Comparing `etl_csm-0.1.6/Etl/Execute.py` & `etl_csm-0.1.7/Etl/Execute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,53 @@
-from typing import Type
-from pandas import concat
-from logging import basicConfig,INFO
-from .Extrator import form_df_tracking,form_df_extras
-from .Treatment_tracking import fill_na_tracking,dtype_tracking,remove_test
-from .Treatment_tracking import steps_residential,errors,flag_duplicated_tracks
-from .Treatment_extras import patternizing_columns,ensure_nan_extras,dtype_extras,fill_na_extras
-from .Treatment_tracking_pme import steps_pme
-from .Helper import timing
+from pandas import concat, DataFrame
+from logging import basicConfig, INFO, DEBUG
+from .Extrator import form_df_tracking, form_df_extras
+from .Treatment_tracking import (fill_na_tracking, dtype_tracking, remove_test,
+                                 remove_unecessary_trackings, flag_duplicated_tracks, 
+                                 create_dates, clean_action)
+from .Treatment_extras import (patternizing_columns, ensure_nan_extras, dtype_extras,
+                                 fill_na_extras)
+from .Unique_treatments import steps_residential, errors, steps_pme
+from .Helper import timing, json_deserializer
 from .Loader import load_cloud
 
-
 class Runner:
+    #batatatatata
     """
         Runner é a classe que executa todo o conjunto de funcoes de tratamento.
         Ele tambem inicializa o processo de logs
         ARGS:
-        query = String que representa um SQL query valido  
+            query = String que representa um SQL query valido  
     """
-    def __init__(self,query:str,bot:str) -> Type:
+    def __init__(self,query:str,bot:str) -> None:
         if bot:
             self.bot = bot
             self.query = query
-            basicConfig(filename='etl.log',filemode='a',level=INFO, format='%(levelname)s: %(message)s')
+            basicConfig(filename='etl.log',filemode='w',level= DEBUG, format='%(asctime)s - %(levelname)s: %(message)s')
         else:
             raise Exception("Para poder rodar essa classe repasse um bot, corparate/residential")
 
     def etl_df(self):
         """
             Funcao que roda ETL do dataframe tracking,
             nao arquiva em memoria o dataframe extras_df
         """ 
         df = form_df_tracking(self.query) #1
         df = fill_na_tracking(df) #2
         df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
         flag_duplicated_tracks(df) #4
         df = dtype_tracking(df) #5
-        df['steps'] = steps_residential(df['category']) #6
-        df['errors'] = errors(df['category']) #7
+        df = create_dates(df) #6
+        df = remove_unecessary_trackings(df) #7
+        df = clean_action(df) #8
+        df['steps'] = steps_residential(df['category']) #9
+        df['errors'] = errors(df['category']) #10
         return df
 
-    def etl_extras_df(self,df:Type) -> Type:
+    def etl_extras_df(self,df:DataFrame) -> DataFrame:
         """
             Funcao que forma o dataframe de extras
             e os trata
         """
         extras_df = form_df_extras(df) #1
         extras_df = patternizing_columns(extras_df) #2
         extras_df = ensure_nan_extras(extras_df) #3
@@ -53,31 +57,34 @@
 
     def etl_df_pme(self):
         df = form_df_tracking(self.query) #1
         df = fill_na_tracking(df) #2
         df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
         flag_duplicated_tracks(df) #4
         df = dtype_tracking(df) #5
-        df['steps'] = steps_pme(df['category']) #6
-        df['errors'] = errors(df['category']) #7
+        df = remove_unecessary_trackings(df) #6
+        df['steps'] = steps_pme(df['category']) #7
+        df['errors'] = errors(df['category']) #8
         return df
 
-    def etl_extras_df_pme(self,df:Type) -> Type:
+    def etl_extras_df_pme(self,df:DataFrame) -> DataFrame:
         extras_df = form_df_extras(df) #1
         extras_df = patternizing_columns(extras_df) #2
-        # extras_df = ensure_nan_extras(extras_df) #3 Deixar para avaliacao
-        # extras_df = fill_na_extras(extras_df) #4 Deixar para avaliacao
-        # extras_df = dtype_extras(extras_df) #5 Deixar para avaliacao
+        extras_df = ensure_nan_extras(extras_df) #3 
+        extras_df = fill_na_extras(extras_df) #4 
+        extras_df = dtype_extras(extras_df) #5 
         return extras_df
-
+    
     def run(self) -> None:
         if self.bot == 'residential':
             df = self.etl_df()
             extras_df = self.etl_extras_df(df)
             df = concat([df,extras_df],axis = 1)
+            df = json_deserializer(df)
             load_cloud(df,self.bot)
         if self.bot == 'corporate':
             df = self.etl_df_pme()
             extras_df = self.etl_extras_df_pme(df)
             df = concat([df,extras_df],axis = 1)
+            df = json_deserializer(df)
             load_cloud(df,self.bot)
```

### Comparing `etl_csm-0.1.6/Etl/Extrator.py` & `etl_csm-0.1.7/Etl/Loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 import psycopg2
-import pandas as pd
+import sqlalchemy.exc
 from os import environ
-from sys import exit
-from typing import Type
-from .Helper import timing,helper_columns
+from re import findall
+from logging import info, warning
+from sqlalchemy import create_engine
+from pandas import DataFrame
+from .Helper import timing,sqlcol
 
-        
 @timing
-def form_df_tracking(query:str) -> type(pd.DataFrame):
+def load_cloud(df:DataFrame,bot:str) -> None:
     """
-        Extrai os dados do RDS, e transforma em pandas object
-        ARGS
-        query = Query a ser feita
+    1- Ira fazer o processo de carregamento para o RDS.
+    2- Ira inserir com os datatypes corretos
+    3- Em seu exception irá acrescentar a coluna com o datatype varchar faltante para nao quebra toda vez que um extra global e lancado
+    ARGS
+        df = pd.DataFrame
+        bot = Bot que irá ser carregado
     """
-    try:
-        engine = psycopg2.connect(
-            database = 'postgres',
-            user = 'tracking',
-            password = environ['SQL_PRD_PASSWORD'],
-            host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
-            port = '5432',
-        )
-    except (Exception,psycopg2.Error) as error:
-        print(f'''
-            Erro na conexão
-            {error}
-            ''',)
-        exit(1)
-
-    cursor = engine.cursor()
-    cursor.execute(query) # Executando query, para obtencao de dados
-    data = cursor.fetchall() # Pegando esse dados
-    cols = helper_columns(cursor = cursor)
-    df = pd.DataFrame(data = data, columns = cols)
-    if df.empty:
-        raise Exception('O seu dataframe está vazio! Algo está de errado com o seu query')
-    return df
-    
-@timing
-def form_df_extras(df:Type):
-    """  
-        Explode os extras globais dentro da coluna,
-        global_extras_raw
-        ARGS
-        df = Dataframe base
-    """
-    new_df = pd.DataFrame(list(df['global_extras_raw']))
-    if new_df.empty:
-        raise Exception('O seu dataframe de extras está vazio! Verifique o seu query')
-    return new_df
-
-
-
+    engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PRD_PASSWORD']}@prd-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
+    tries = 15
+    sql_dict = sqlcol(df)
+    for _ in range(tries):
+        try:
+            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',dtype = sql_dict,index = False,chunksize = 10000)
+            break
+        except sqlalchemy.exc.ProgrammingError as error:
+                warning(f"Tivemos um erro {error}")
+                if isinstance(error.orig, psycopg2.errors.UndefinedColumn):
+                    warning("Vou executar um handler para ver se consigo resolver!")         
+                    engine = psycopg2.connect(
+                        database = 'clean_data',
+                        user = 'tracking',
+                        password = environ['SQL_PRD_PASSWORD'],
+                        host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
+                        port = '5432',
+                    )
+                    cursor = engine.cursor()
+                    column = findall('"(.*?)"',str(error))[0]
+                    warning(f"Tive que acrescentar mais uma coluna ao seu dataframe ja existente a coluna foi {column}")
+                    query = f"""
+                    ALTER TABLE {bot}_tracking_treated
+                    ADD COLUMN {column} VARCHAR NULL;
+                    """
+                    info(query)
+                    cursor.execute(query)
+                    engine.commit()
+                    tries -= 1
+                else:
+                    warning("Erro severo sem exception handling no load_cloud!")
+        # Sempre fazer esse commit pelo amor
```

### Comparing `etl_csm-0.1.6/Etl/Helper.py` & `etl_csm-0.1.7/Etl/Helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,108 @@
 import sqlalchemy
+from pandas import DataFrame
 from typing import Type
 from functools import wraps
 from time import time
-from logging import info
-from io import StringIO
-from csv import writer
+from logging import info,warning
 from numpy import nan
+from orjson import loads
+from sqlalchemy.dialects.postgresql import JSONB
+from sqlalchemy.types import UnicodeText
+
 
 def timing(f):
     # Decorator simples para medir tempo de excecucao de funcao
     @wraps(f)
     def wrap(*args, **kw):
         ts = time()
         result = f(*args, **kw)
         te = time()
-        info(f'Funcao {f.__name__} demoro {te-ts:2.4f} segundos')
+        warning(f'Funcao {f.__name__} demoro {te-ts:2.4f} segundos')
         return result
     return wrap
 
 def helper_columns(cursor:Type) -> Type:
     # Funcao simples para extracao de nomenclatura de colunas
     # Para formar dataframe
     cols = []
     for col in cursor.description:
         cols.append(col[0])
     return cols
 
-def psql_insert_copy(table, conn, keys, data_iter):
+def map_substring(s, dict_map) -> dict:
     """
-    Executa sql query unico para por dados de maneira eficiente em postgresql
-    ARGS
-    table = pandas.io.sql.SQLTable - Tabela
-    conn = sqlalchemy.engine.Engine ou sqlalchemy.engine.Connection
-    keys = lista de strings com nomes das colunas, nao precisa passar
-    data_iter = Iterador que vai fazer o trampo todo
-    """
-    dbapi_conn = conn.connection
-    with dbapi_conn.cursor() as cur:
-        s_buf = StringIO()
-        writer_obj = writer(s_buf)
-        writer_obj.writerows(data_iter)
-        s_buf.seek(0)
-        columns = ', '.join(['"{}"'.format(k) for k in keys])
-        if table.schema:
-            table_name = '{}.{}'.format(table.schema, table.name)
-        else:
-            table_name = table.name
-        sql = 'COPY {} ({}) FROM STDIN WITH CSV'.format(
-            table_name, columns)
-        cur.copy_expert(sql=sql, file=s_buf)
-
-def map_substring(s, dict_map):
-    """
-    Funcao helper mapeia as sub strings com facilidade
-    ARGS
-    s = pd.Series a ser interada por
-    dict_map = mapa se substrings
+        Funcao helper mapeia as sub strings com facilidade
+        ARGS
+            s = pd.Series a ser interada por
+        RETURNS
+            dict_map = mapa se substrings
     
     """
     for key in dict_map.keys():
         if key in s: 
             return dict_map[key]
     return nan
 
-def sqlcol(df) -> dict:
+def sqlcol(df:DataFrame) -> dict:
     """
-    Funcao que mapeia os datatype das tabelas e retorna o datatype adequado do SQLalchemy
-    ARGS
-    df, para acessar os objetos de colunas e datatypes
+        Funcao que mapeia os datatype das tabelas e retorna o datatype adequado do SQLalchemy
+        ARGS
+            df, para acessar os objetos de colunas e datatypes
     """
     info("Formulando dict_map de datatype SQLalchemy")
+
+    valid_json_b = ['global_extras_raw','plan_value','plan_name','plan_offer']
+
     dtypedict = {}
     for i,j in zip(df.columns, df.dtypes):
-        if "object" in str(j):
-            dtypedict.update({i: sqlalchemy.types.VARCHAR()})                 
+        if i in valid_json_b:
+            dtypedict.update({i: JSONB(astext_type=UnicodeText)})
+            continue
+            # Depois adicionar colunas a mais
+        if 'object' in str(j):
+            dtypedict.update({i: sqlalchemy.types.VARCHAR()})     
         if "datetime" in str(j):
             dtypedict.update({i: sqlalchemy.types.DateTime()})
         if "float" in str(j):
             dtypedict.update({i: sqlalchemy.types.Float(precision=3, asdecimal=True)})
         if "int" in str(j):
             dtypedict.update({i: sqlalchemy.types.INT()})
 
-    info(dtypedict)
-    return dtypedict
+    warning(f"Segue dicionario de datatypes{dtypedict}")
+    return dtypedict
+
+
+def try_to_deserialize_json(x) -> str:
+    """
+        Pega celulas unicas transforma elas para string caso elas estejam em formato json caso nao
+        Transforma elas, em string
+        ARGS
+            X = CelulaS com possibiidade json
+        RETURNS
+            Celula em formato str
+    """
+    try:
+        x = str(x)
+    except:
+        info(f"O seguinte valor {x} veio como json, e nao foi convertido para string corretamente")
+    return x
+
+@timing
+def json_deserializer(df:DataFrame) -> DataFrame:
+    """
+        1- Transformar elas em string
+        2- Repassar elas como datatype json
+        ARG
+            Dataframe com jsons em formato dict
+        RETURNS
+            Dataframe com json em formato string
+    """
+    valid_json_columns = ['global_extras_raw','plan_value','plan_name','plan_offer']
+
+    for series in valid_json_columns:
+        try:
+            df[series] = df[series].apply(try_to_deserialize_json)
+        except KeyError as e:
+            warning(f"A coluna {series} nao foi achada, nao vou transformar em string!" )
+    return df
+
```

### Comparing `etl_csm-0.1.6/Etl/__init__.py` & `etl_csm-0.1.7/Etl/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 from Etl.Extrator import (
     form_df_tracking,
     form_df_extras
 )
 from Etl.Helper import (
     timing,
     helper_columns,
-    psql_insert_copy,
-    map_substring
+    map_substring,
+    sqlcol,
+    json_deserializer
 )
 from Etl.Treatment_extras import (
     patternizing_columns,
     ensure_nan_extras,
     fill_na_extras,
     dtype_extras,
 )
 from Etl.Treatment_tracking import (
     fill_na_tracking,
     dtype_tracking,
     remove_test,
-    steps_residential,
-    errors,
-    flag_duplicated_tracks
+    flag_duplicated_tracks,
+    create_dates,
+    remove_unecessary_trackings,
 )
 
-from Etl.Treatment_tracking_pme import (
+from Etl.Unique_treatments import (
+    steps_residential,
+    errors,
     steps_pme
 )
 
 from Etl.Loader import (
     load_cloud
 )
```

### Comparing `etl_csm-0.1.6/LICENSE` & `etl_csm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.6/PKG-INFO` & `etl_csm-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Provides-Extra: dev
 License-File: LICENSE
 
-Biblioteca para aproveitar classes de tratamento CSM
+Biblioteca para aproveitar classes de tratamento CSM, direcionada para pet
```

### Comparing `etl_csm-0.1.6/README.md` & `etl_csm-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 * As demandos do ambiente cloud localizam-se no serverless.yml.
 # Links importantes
 ## Verificação de testes realizados na lambda apos subir a pipeline
 * https://us-east-1.console.aws.amazon.com/lambda/home?region=us-east-1#/functions/etl-pet-csm?tab=code
 ## Pipeline
 * https://jenkins.clarobrasil.mobi/view/ChatBot/job/csm-etl/job/pet/
 ## Logs de testes
-* https://us-east-1.console.aws.amazon.com/cloudwatch/home?region=us-east-1#logsV2:log-groups/log-group/$252Faws$252Flambda$252Fetl-pet-csm
+* https://us-east-1.console.aws.amazon.com/cloudwatch/home?region=us-east-1#logsV2:log-groups/log-group/$252Faws$252Flambda$252Fetl-pet-csm
+batatatatata
```

### Comparing `etl_csm-0.1.6/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.7/etl_csm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Provides-Extra: dev
 License-File: LICENSE
 
-Biblioteca para aproveitar classes de tratamento CSM
+Biblioteca para aproveitar classes de tratamento CSM, direcionada para pet
```

### Comparing `etl_csm-0.1.6/setup.py` & `etl_csm-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
     author_email = "francisco.froes@globalhitss.com.br",
     description = DESCRIPTION,
-    long_description = 'Biblioteca para aproveitar classes de tratamento CSM',
+    long_description = 'Biblioteca para aproveitar classes de tratamento CSM, direcionada para pet',
     packages = find_packages(),
     url = 'https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl',
     keywords = ['python', 'etl'],
     license = 'MIT',
     install_requires = ['numpy', 'pandas', 'orjson','SQLAlchemy','psycopg2-binary'],
     extras_require = {
         'dev':['twine>=4.0.2'],
```

