# Comparing `tmp/t8s-0.1.6.tar.gz` & `tmp/t8s-0.1.7.tar.gz`

## Comparing `t8s-0.1.6.tar` & `t8s-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,42 @@
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 t8s-0.1.6/main.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.6/publish-to-pypi.md
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.6/test-all.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.6/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 t8s-0.1.6/.vscode/launch.json
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 t8s-0.1.6/docs/dp-strategy.md
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.6/docs/img/strategy-pattern.png
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.6/src/t8s/__about__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 t8s-0.1.6/src/t8s/__init__.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 t8s-0.1.6/src/t8s/log_config.py
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 t8s-0.1.6/src/t8s/ts.py
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 t8s-0.1.6/src/t8s/ts_builder.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 t8s-0.1.6/src/t8s/ts_writer.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 t8s-0.1.6/tests/test_build_from_file.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 t8s-0.1.6/tests/test_to_parquet.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 t8s-0.1.6/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 t8s-0.1.6/README.md
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 t8s-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 t8s-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 t8s-0.1.7/main.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.7/publish-to-pypi.md
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.7/test-all.sh
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 t8s-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    11376 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/304549b72d184314
+-rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/37e53140500f6132
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/3efc7ff997958a2f
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/6a6461ff9108736
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/81d77b98d62a2ea
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/b9b8e13161c902cd
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/d3d5adf6aba338ae
+-rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/dbd4b6248442ea85
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/e1951fc7d1998d8f
+-rw-r--r--   0        0        0    26490 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/e7c8c0f9acb696e4
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/ebb21a9ed88aaaf2
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 t8s-0.1.7/.vscode/launch.json
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 t8s-0.1.7/docs/dp-strategy.md
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.7/docs/img/strategy-pattern.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 t8s-0.1.7/src/stubs/.gitkeep
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/__about__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/__init__.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/log_config.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/node.py
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/ts.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/ts_builder.py
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/ts_writer.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 t8s-0.1.7/tests/test_build_from_file.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 t8s-0.1.7/tests/test_to_parquet.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 t8s-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 t8s-0.1.7/README.md
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 t8s-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 t8s-0.1.7/PKG-INFO
```

### Comparing `t8s-0.1.6/main.py` & `t8s-0.1.7/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+
 from t8s.log_config import LogConfig
 from pathlib import Path
 from datetime import datetime
 import numpy as np
 import pandas as pd
 import t8s
 from t8s.ts import TimeSerie
@@ -9,15 +11,15 @@
 from t8s.log_config import LogConfig
 from t8s.ts_writer import TSWriter, WriteParquetFile, WriteCsvFile
 from logging import INFO, DEBUG, WARNING, ERROR, CRITICAL
 
 if __name__ == "__main__":
     # print('globals:', globals())
     # The client code.
-    LogConfig().initialize_logger(INFO)
+    LogConfig().initialize_logger(DEBUG)
     logger = LogConfig().getLogger()
     ts = TSBuilder.empty()
     # initialize_logger(INFO)
     logger.info('t8s package version:' + t8s.__version__)
     path_str: str = 'ts_01.parquet'
     path = Path(path_str)
     # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e velocidade
@@ -76,16 +78,18 @@
         print(col, '\t', type(ts.df[col][0]))
 
     # pd._libs.tslibs.timestamps.Timestamp é privado e devo usar pd.Timestamp
     assert type(ts.df['timestamp'][0]) == pd.Timestamp
     assert type(ts.df['temperatura'][0]) == np.float32
     assert type(ts.df['velocidade'][0]) == np.int32
 
+    print('---------------------------------------------------')
     univariate_list = ts.split()
     for idx, ts_uni in enumerate(univariate_list):
-        print(f'TimeSerie univariada {idx}:')
+        print(f'TimeSerie univariada {idx+1}:')
         print(ts_uni)
         print('---------------------------------------------------')
-        print(f'univariate {idx-1}', '\n ', ts_uni)
 
-    print('---------------------------------------------------')
-    
+    print('\nAgora posso fazer o join das séries temporais univariadas')
+    ts = TimeSerie.join(univariate_list)
+    print("\n\nTimeSerie multivariada, ts:\n")
+    print(ts)
```

### Comparing `t8s-0.1.6/publish-to-pypi.md` & `t8s-0.1.7/publish-to-pypi.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.6/docs/dp-strategy.md` & `t8s-0.1.7/docs/dp-strategy.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.6/docs/img/strategy-pattern.png` & `t8s-0.1.7/docs/img/strategy-pattern.png`

 * *Files identical despite different names*

### Comparing `t8s-0.1.6/src/t8s/log_config.py` & `t8s-0.1.7/src/t8s/log_config.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.6/src/t8s/ts_builder.py` & `t8s-0.1.7/src/t8s/ts_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+
 # from __future__ import annotations usado apenas nas versões anteriores a 3.7
 from abc import ABC, abstractmethod
 from typing import Any, Optional
 from pathlib import Path
 from datetime import datetime
 from t8s.log_config import LogConfig
 from t8s.ts import TimeSerie # , ITimeSerie, ITimeSeriesProcessor, IProvenancable
@@ -58,14 +60,16 @@
         """
         Usually, the Context allows replacing a Strategy object at runtime.
         """
 
         self._strategy = strategy
 
     def build_from_file(self, path: Path) -> TimeSerie:
+        # TODO: garantir que a primeira coluna seja um Timestamp quando o formato for long ou wide
+
         """
         The Context delegates some work to the Strategy object instead of
         implementing multiple versions of the algorithm on its own.
         """
 
         # ...
 
@@ -73,14 +77,16 @@
         result = self._strategy.do_read(path)
         logger.info('result type from build_from_file() is: ' + str(type(result)))
 
         # ...
         return result
 
     def build_from_socket(self, uri) -> Optional['TimeSerie']:
+        # TODO: garantir que a primeira coluna seja um Timestamp quando o formato for long ou wide
+
         """
         The Context delegates some work to the Strategy object instead of
         implementing multiple versions of the algorithm on its own.
         """
 
         # ...
 
@@ -121,18 +127,19 @@
         # Imprime o esquema do arquivo Parquet
         logger.debug('\ntype(metadata.schema): ' + str(type(metadata.schema)) + '\t' + str(metadata.schema))
         # Imprime as colunas do arquivo Parquet
         # print('metadata.column_names', metadata.column_names)
         # Imprime as estatísticas do arquivo Parquet
         logger.debug(metadata.row_group(0).column(0).statistics)
         # Leia o arquivo Parquet
-        parquet_file: pa.parquet.core.ParquetFile = pq.ParquetFile(data)
+        parquet_file = pq.ParquetFile(data)
         logger.debug('\ntype(parquet_file): ' + str(type(parquet_file)) + '\n' + str(parquet_file))
         logger.debug('\n-------------------------------')
         df = pd.read_parquet(data)
+        # TODO: garantir que a primeira coluna seja um Timestamp quando o formato for long ou wide
         logger.debug('\ndf:\n' + str(df))
         # Cria o objeto 
         ts = TimeSerie(df, format=format, features_qty=features_qty)
         logger.debug('\nts:\n' + str(ts))
         return ts
 
 class ReadCsvFile(ReadStrategy):
```

### Comparing `t8s-0.1.6/tests/test_build_from_file.py` & `t8s-0.1.7/tests/test_build_from_file.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.6/tests/test_to_parquet.py` & `t8s-0.1.7/tests/test_to_parquet.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.6/LICENSE.txt` & `t8s-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

