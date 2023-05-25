# Comparing `tmp/t8s-0.1.4.tar.gz` & `tmp/t8s-0.1.5.tar.gz`

## Comparing `t8s-0.1.4.tar` & `t8s-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 t8s-0.1.4/main.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.4/publish-to-pypi.md
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.4/test-all.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.4/.pytest_cache/README.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 t8s-0.1.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 t8s-0.1.4/docs/dp-strategy.md
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.4/docs/img/strategy-pattern.png
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.4/src/t8s/__about__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 t8s-0.1.4/src/t8s/__init__.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 t8s-0.1.4/src/t8s/log_config.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 t8s-0.1.4/src/t8s/ts.py
--rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 t8s-0.1.4/src/t8s/ts_builder.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 t8s-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 t8s-0.1.4/tests/test_build_from_file.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 t8s-0.1.4/tests/test_to_parquet.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 t8s-0.1.4/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 t8s-0.1.4/README.md
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 t8s-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 t8s-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 t8s-0.1.5/main.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.5/publish-to-pypi.md
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.5/test-all.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 t8s-0.1.5/.vscode/launch.json
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 t8s-0.1.5/docs/dp-strategy.md
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.5/docs/img/strategy-pattern.png
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.5/src/t8s/__about__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 t8s-0.1.5/src/t8s/__init__.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 t8s-0.1.5/src/t8s/log_config.py
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 t8s-0.1.5/src/t8s/ts.py
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 t8s-0.1.5/src/t8s/ts_builder.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 t8s-0.1.5/src/t8s/ts_writer.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 t8s-0.1.5/tests/test_build_from_file.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 t8s-0.1.5/tests/test_to_parquet.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 t8s-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 t8s-0.1.5/README.md
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 t8s-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 t8s-0.1.5/PKG-INFO
```

### Comparing `t8s-0.1.4/main.py` & `t8s-0.1.5/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 from t8s.log_config import LogConfig
 from pathlib import Path
 from datetime import datetime
+import numpy as np
+import pandas as pd
 import t8s
-from t8s import TimeSerie, TSBuilder, ReadParquetFile, ReadCsvFile
-
+from t8s.ts import TimeSerie
+from t8s.ts_builder import TSBuilder, ReadParquetFile, ReadCsvFile
+from t8s.log_config import LogConfig
+from t8s.ts_writer import TSWriter, WriteParquetFile, WriteCsvFile
 from logging import INFO, DEBUG, WARNING, ERROR, CRITICAL
 
 if __name__ == "__main__":
     # print('globals:', globals())
     # The client code.
     LogConfig().initialize_logger(INFO)
     logger = LogConfig().getLogger()
-
+    ts = TSBuilder.empty()
     # initialize_logger(INFO)
     logger.info('t8s package version:' + t8s.__version__)
     path_str: str = 'ts_01.parquet'
     path = Path(path_str)
     # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e velocidade
     data = {
         'timestamp': [
             datetime(2022, 1, 1, 0, 0, 0), 
             datetime(2022, 1, 1, 1, 0, 0),
             datetime(2022, 1, 1, 2, 0, 0), 
             datetime(2022, 1, 1, 3, 0, 0)],
-        'temperatura': [25.0, 26.0, 27.0, 23.2],
-        'velocidade': [2000.1, 1100.3, 1200.5, 4000.4]
+        'temperatura': np.array([25.0, 26.0, 27.0, 23.2], dtype=np.float32),
+        'velocidade': [2000, 1100, 1200, 4000]
     }
-
-    ts = TimeSerie(data, format='wide', features_qty=len(data))
-    df = ts.df
-    cols_str = [name for name in sorted(df.columns)]
+    # Convertendo os tipos de dado para temperatura e velocidade para 
+    # np.float32 e np.int32 respectivamente, pois o padrão é np.float64 e np.int64
+    data['temperatura'] = np.array(data['temperatura'], dtype=np.float32)
+    data['velocidade'] = np.array(data['velocidade'], dtype=np.int32)
+    # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e
+    # velocidade para o proposito de teste
+    ts = TimeSerie(data, format='wide', features_qty = 3)
+    cols_str = [name for name in sorted(ts.df.columns)]
     cols_str = ', '.join(cols_str)
-    logger.info(f'Dataframe com {len(df.columns)} colunas: {cols_str}')
-    # Imprime a série temporal
+    logger.info(f'Dataframe com {len(ts.df.columns)} colunas: {cols_str}')
+    # Faz o display da série temporal no terminal
     print(ts)
-    # Imprime a série temporal em parquet
-    print(f'Converte a série temporal (formato {ts.format}) em arquivo parquet {path}')
-    ts.to_parquet(Path(path_str))
+    # Grava a série temporal em parquet
+    print(f'Grava a série temporal (formato {ts.format}) em um arquivo parquet {path}')
+    context = TSWriter(WriteParquetFile())
+    print("Client: Strategy was seted to write Parquet file.")
+    context.write(Path(path_str), ts)
+    print(f'\nArquivo {str(path)} gerado à partir da TimeSerie fornecida')
+    # --------------------------------------------------------------------------------
+    # Limpando objeto ts para garantir que será lido corretamente.
+    ts = TSBuilder.empty()
     # Lê a série temporal gravada no arquivo parquet
-    print('\nLendo path: ', path)
-    # ts = TimeSerie.build_from_file(path) 
+    print(f'\nLendo path {str(path)} e gerando TimeSerie')
     
-    # --------------------------------------------------------------------------------
     # The client code picks a concrete strategy and passes it to the context.
     # The client should be aware of the differences between strategies in order
     # to make the right choice.
-
-    ts = TimeSerie(format = 'wide', features_qty = 0)
     assert isinstance(path, Path), "path must be a Path object"
     if  (str(path)).endswith('.parquet'):
         context = TSBuilder(ReadParquetFile())
-        print("Client: Strategy is set to read Parquet file.")
+        print("Client: ReadStrategy is set to read Parquet file.")
         ts = context.build_from_file(Path(path_str))
     else:
         assert str(path).endswith('.csv'), "If path is not a Parquet file the path must be a CSV file"
-        print("Client: Strategy is set to read CSV file.")
+        print("Client: ReadStrategy is set to read CSV file.")
         context = TSBuilder(ReadCsvFile())
         ts = context.build_from_file(Path(path_str))
 
     assert int(ts.features) == 3
     assert ts.format == 'wide'
-    assert ts.df.__len__() == 4
+    assert len(ts.df) == 4
+    print('Tipos das colunas no Dataframe da Série Temporal:')
+    for col in ts.df.columns:
+        print(col, '\t', type(ts.df[col][0]))
+
+    # pd._libs.tslibs.timestamps.Timestamp é privado e devo usar pd.Timestamp
+    assert type(ts.df['timestamp'][0]) == pd.Timestamp
+    assert type(ts.df['temperatura'][0]) == np.float32
+    assert type(ts.df['velocidade'][0]) == np.int32
```

### Comparing `t8s-0.1.4/publish-to-pypi.md` & `t8s-0.1.5/publish-to-pypi.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.4/docs/dp-strategy.md` & `t8s-0.1.5/docs/dp-strategy.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.4/docs/img/strategy-pattern.png` & `t8s-0.1.5/docs/img/strategy-pattern.png`

 * *Files identical despite different names*

### Comparing `t8s-0.1.4/src/t8s/log_config.py` & `t8s-0.1.5/src/t8s/log_config.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.4/src/t8s/ts.py` & `t8s-0.1.5/src/t8s/ts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from datetime import datetime
 import yaml
 from abc import ABC, abstractmethod
-from typing import List, Dict, Any
+from typing import Any, Optional
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 from t8s.log_config import LogConfig
 
@@ -36,18 +36,14 @@
         # Verifica se a série temporal é univariada
         return False
 
     @abstractmethod
     def is_multivariate(self) -> bool:
         # Verifica se a série temporal é multivariada
         return False
-    
-    @abstractmethod
-    def to_parquet(self, path:Path):
-        pass
 
 """Rastreia a proveniência dos ativos de informação, Série Temporal neste caso"""
 class IProvenancable(ABC):
     def __init__(self):
         self.format: str
         self.features: str
         self.df: pd.DataFrame
@@ -56,96 +52,117 @@
     uma transformação específica. Ele recebe como parâmetros o nome da transformação 
     e um dicionário com os parâmetros usados na transformação."""
     @abstractmethod
     def add_provenance(self, transformation: str, parameters: dict): 
         pass 
     
     @abstractmethod
-    def get_provenances(self) -> List[Dict[str, Any]]: 
+    def get_provenances(self) -> list[dict[str, Any]]: 
         """Este método retorna uma lista de dicionários com as informações de 
         proveniência de todas as transformações realizadas no objeto TimeSerie."""
         pass
 
     @abstractmethod
-    def get_provenance_by_transformation(self, transformation: str) -> Dict[str, Any]: 
+    def get_provenance_by_transformation(self, transformation: str) -> dict[str, Any]: 
         """Este método retorna as informações de proveniência de uma dada transformação 
         realizadas no objeto TimeSerie."""
         pass
 
     @abstractmethod
-    def get_last_transformation(self, transformation: str) -> Dict[str, Any]: 
+    def get_last_transformation(self, transformation: str) -> dict[str, Any]: 
         """Este método retorna informações da ultima transformação realizada no objeto TimeSerie."""
         pass
 
-    def apply_transformation(self, transformation: str, **kwargs) -> ITimeSeriesProcessor: 
+    @abstractmethod
+    def apply_transformation(self, transformation: str, **kwargs) -> Any : 
         """Este método aplica uma transformação ao objeto TimeSerie e retorna um novo 
         objeto TimeSerie com as informações de proveniência atualizadas. Ele recebe como 
         parâmetros o nome da transformação e os parâmetros específicos da transformação."""
         pass
 
-class TimeSerie(ITimeSeriesProcessor, IProvenancable):
+class ITimeSerie(ITimeSeriesProcessor, IProvenancable):
+    """
+    Interface que estende as outras interfaces. ë apenas uma Marker Interface
+    """
+    pass
+
+class TimeSerie(ITimeSerie):
     def __init__(self, *args, format, features_qty, **kwargs):
         assert isinstance(format, str), "format must be a string"
         assert isinstance(features_qty, int), "features_qty must be a int"
         assert format in ['long', 'wide'], "format must be 'long' or 'wide'"
         self.format: str = format
         self.features: str = str(features_qty)
         self.df = pd.DataFrame(*args, **kwargs)
 
     def __repr__(self):
         # Retorna uma representação em string do objeto TimeSerie
         return f'TimeSerie(format={self.format}, features={self.features}, df=\n{self.df.__repr__()})'
-    
+        
     def to_long(self):
         # Converte a série temporal para o formato Long
         # Implementação aqui
+        # TODO: Implementar to_long()
         pass
 
     def to_wide(self):
         # Converte a série temporal para o formato Wide
         # Implementação aqui
+        # TODO: Implementar to_wide()
         pass
 
     def is_univariate(self):
         # Verifica se a série temporal é univariada
         # Implementação aqui
+        # TODO: Implementar is_univariate()
         pass
 
     def is_multivariate(self):
         # Verifica se a série temporal é multivariada
         # Implementação aqui
+        # TODO: Implementar is_multivariate()
         pass
 
-    def to_parquet(self, path):
+    def write_parquet_file(self, path):
         # Grava os dados em formato Parquet com metadados do objeto TimeSerie
         # to_parquet(path, df, self.format, self.features)
         table = pa.Table.from_pandas(self.df)
         # table = table.replace_schema_metadata({'format': self.format, 'features': self.features})
         table = table.replace_schema_metadata({
             b'format': str(self.format).encode(),
             b'features': str(self.features).encode()})
         pq.write_table(table, path)
 
     ### Métodos de IProvenancable
     def add_provenance(self, transformation: str, parameters: dict):
         # Este método adiciona informações de proveniência ao objeto TimeSerie para 
         # uma transformação específica. Ele recebe como parâmetros o nome da transformação 
         # e um dicionário com os parâmetros usados na transformação.
+        # TODO: Implementar add_provenance()
         pass
 
-    def get_provenances(self) -> List[Dict[str, Any]]:
+    def get_provenances(self) -> list[dict[str, Any]]:
         # Este método retorna uma lista de dicionários com as informações de 
         # proveniência de todas as transformações realizadas no objeto TimeSerie.
+        # TODO: Implementar get_provenances()
         return []
 
-    def get_provenance_by_transformation(self, transformation: str) -> Dict[str, Any]:
+    def get_provenance_by_transformation(self, transformation: str) -> dict[str, Any]:
         # Este método retorna as informações de proveniência de uma dada transformação 
         # realizadas no objeto TimeSerie.
+        # TODO: Implementar get_provenance_by_transformation()
         return {}
 
-    def get_last_transformation(self, transformation: str) -> Dict[str, Any]:
+    def get_last_transformation(self, transformation: str) -> dict[str, Any]:
+        # TODO: Implementar get_provenance_by_transformation()
         return {}
 
-    """
+    def apply_transformation(self, transformation: str, **kwargs) -> Optional['TimeSerie']: 
+        """Este método aplica uma transformação ao objeto TimeSerie e retorna um novo 
+        objeto TimeSerie com as informações de proveniência atualizadas. Ele recebe como 
+        parâmetros o nome da transformação e os parâmetros específicos da transformação."""
+        # TODO: Implementar apply_transformation()
+        return TimeSerie.empty()
+    
     @staticmethod
-    . . .
-    """
+    def empty() -> Any:
+        return TimeSerie(format='long', features_qty=0, data={})
```

### Comparing `t8s-0.1.4/src/t8s/ts_builder.py` & `t8s-0.1.5/src/t8s/ts_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,107 @@
-from __future__ import annotations
+# from __future__ import annotations usado apenas nas versões anteriores a 3.7
 from abc import ABC, abstractmethod
 from typing import List, Any
 from pathlib import Path
 from datetime import datetime
 from t8s.log_config import LogConfig
-from t8s import TimeSerie
+from t8s.ts import TimeSerie # , ITimeSerie, ITimeSeriesProcessor, IProvenancable
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 logger = LogConfig().getLogger()
 
+class ReadStrategy(ABC):
+    """
+    The Strategy interface declares operations common to all supported versions
+    of some algorithm.
+
+    The Context uses this interface to call the algorithm defined by Concrete
+    Strategies.
+    """
+
+    @abstractmethod
+    def do_read(self, data: Any) -> Any:
+        pass
+
+
+"""
+Concrete Strategies implement the algorithm while following the base Strategy
+interface. The interface makes them interchangeable in the Context.
+"""
+
 class TSBuilder():
     """
     The Context defines the interface of interest to clients.
     """
 
-    def __init__(self, strategy: Strategy) -> None:
+    def __init__(self, strategy: ReadStrategy) -> None:
         """
         Usually, the Context accepts a strategy through the constructor, but
         also provides a setter to change it at runtime.
         """
         logger.info('TSBuilder constructor received strategy: %s', strategy)
         self._strategy = strategy
 
     @property
-    def strategy(self) -> Strategy:
+    def strategy(self) -> ReadStrategy:
         """
         The Context maintains a reference to one of the Strategy objects. The
         Context does not know the concrete class of a strategy. It should work
         with all strategies via the Strategy interface.
         """
 
         return self._strategy
 
     @strategy.setter
-    def strategy(self, strategy: Strategy) -> None:
+    def strategy(self, strategy: ReadStrategy) -> None:
         """
         Usually, the Context allows replacing a Strategy object at runtime.
         """
 
         self._strategy = strategy
 
-    def build_from_file(self, path: Path) -> TimeSerie:
+    def build_from_file(self, path: Path) -> Any:
         """
         The Context delegates some work to the Strategy object instead of
         implementing multiple versions of the algorithm on its own.
         """
 
         # ...
 
-        logger.info("Context: build_from_file")
-        result = self._strategy.do_algorithm(path)
+        logger.info(f"Context: build_from_file {path}")
+        result = self._strategy.do_read(path)
         logger.info('result type is: ' + str(type(result)))
 
         # ...
         return result
 
-    def build_from_socket(self, uri) -> TimeSerie:
+    def build_from_socket(self, uri) -> Any:
         """
         The Context delegates some work to the Strategy object instead of
         implementing multiple versions of the algorithm on its own.
         """
 
         # ...
 
         print("Context: build_from_socket")
-        result = self._strategy.do_algorithm(None)
+        result = self._strategy.do_read(None)
         logger.info('result type is: ' + str(type(result)))
 
         # ...
         return result
 
-class Strategy(ABC):
-    """
-    The Strategy interface declares operations common to all supported versions
-    of some algorithm.
-
-    The Context uses this interface to call the algorithm defined by Concrete
-    Strategies.
-    """
-
-    @abstractmethod
-    def do_algorithm(self, data: Any) -> TimeSerie:
-        pass
-
-
-"""
-Concrete Strategies implement the algorithm while following the base Strategy
-interface. The interface makes them interchangeable in the Context.
-"""
-
-
-class ReadParquetFile(Strategy):
-    def do_algorithm(self, data: Path) -> TimeSerie:
-        logger.info('Using ReadParquetFile strategy')
+    @staticmethod
+    def empty() -> Any:
+        return TimeSerie.empty()
+
+class ReadParquetFile(ReadStrategy):
+    def do_read(self, data: Path) -> Any:
+        logger.info('Using ReadParquetFile strategy to read data from: ' + str(data))
         assert isinstance(data, Path), "path must be a Path object"
         assert (str(data)).endswith('.parquet'), "path must be a Path object"
         # Lê os metadados do arquivo Parquet
         metadata: pq.FileMetaData = pq.read_metadata(data)
         logger.debug('\nParquet file metadata:\n' + str(metadata.to_dict()) + '\n' + str(metadata.metadata))
         assert isinstance(metadata, pq.FileMetaData), "metadata must be a pq.FileMetaData object"
         dict_meta: dict = metadata.to_dict()
@@ -107,33 +110,32 @@
         # Imprime o valor do metadado 'format'
         format = metadata.metadata[b'format'].decode()
         features = metadata.metadata[b'features'].decode()
         logger.info('format: ' + format + ' type(format) ' + str(type(format)))
         logger.info('features: ' + str(features) + ' type(features): ' + str(type(features)))
         assert isinstance(format, str), "format metadada must be a string"
         assert isinstance(features, str), "features metadada must be a string"
+        features_qty = int(features)
+        assert features_qty > 1, "features_qty must be greater than one"
         # print('format', dict_meta['format'])
         # print('features', dict_meta['features'])
         # Imprime o esquema do arquivo Parquet
         logger.debug('\ntype(metadata.schema): ' + str(type(metadata.schema)) + '\t' + str(metadata.schema))
         # Imprime as colunas do arquivo Parquet
         # print('metadata.column_names', metadata.column_names)
         # Imprime as estatísticas do arquivo Parquet
         logger.debug(metadata.row_group(0).column(0).statistics)
-        # Leia os metadados do arquivo Parquet
-        features_qty = int(features)
         # Leia o arquivo Parquet
         parquet_file: pa.parquet.core.ParquetFile = pq.ParquetFile(data)
         logger.debug('\ntype(parquet_file): ' + str(type(parquet_file)) + '\n' + str(parquet_file))
         logger.debug('\n-------------------------------')
         df = pd.read_parquet(data)
         logger.debug('\ndf:\n' + str(df))
         # Cria o objeto 
-        ts = TimeSerie(data=df, format=format, features_qty=features_qty)
-        logger.info('\nts:\n' + str(ts))
+        ts = TimeSerie(df, format=format, features_qty=features_qty)
+        logger.debug('\nts:\n' + str(ts))
         return ts
 
-
-class ReadCsvFile(Strategy):
-    def do_algorithm(self, data: List) -> TimeSerie:
+class ReadCsvFile(ReadStrategy):
+    def do_read(self, data: List) -> Any:
         logger.info('Using ReadCsvFile strategy')
-        return TimeSerie(format = 'wide', features_qty = 0)
+        return TSBuilder.empty()
```

### Comparing `t8s-0.1.4/LICENSE.txt` & `t8s-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t8s-0.1.4/README.md` & `t8s-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 ```console
 pip install t8s
 ```
 
 ## Testing
 
 ```console
+# Para inspecionar a configuração do ambiente de testes:
+hatch config show
+hatch clean
 hatch build
 hatch run python3 main.py
 ./test-all.sh
 ```
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `t8s-0.1.4/pyproject.toml` & `t8s-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "t8s"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "João Antonio Ferreira", email = "joao.parana@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "keyring",
@@ -52,15 +51,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `t8s-0.1.4/PKG-INFO` & `t8s-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: t8s
-Version: 0.1.4
+Version: 0.1.5
 Project-URL: Documentation, https://github.com/unknown/t8s#readme
 Project-URL: Issues, https://github.com/unknown/t8s/issues
 Project-URL: Source, https://github.com/unknown/t8s
 Author-email: João Antonio Ferreira <joao.parana@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: keyring
 Requires-Dist: keyrings-google-artifactregistry-auth
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
@@ -39,14 +38,17 @@
 ```console
 pip install t8s
 ```
 
 ## Testing
 
 ```console
+# Para inspecionar a configuração do ambiente de testes:
+hatch config show
+hatch clean
 hatch build
 hatch run python3 main.py
 ./test-all.sh
 ```
 
 ## License
```

