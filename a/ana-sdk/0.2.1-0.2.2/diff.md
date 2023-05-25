# Comparing `tmp/ana_sdk-0.2.1.tar.gz` & `tmp/ana_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.2.1.tar", max compression
+gzip compressed data, was "ana_sdk-0.2.2.tar", max compression
```

## Comparing `ana_sdk-0.2.1.tar` & `ana_sdk-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.1/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14791 2023-05-23 18:27:45.153492 ana_sdk-0.2.1/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.1/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.1/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.1/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.1/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.1/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.1/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      463 2023-05-23 18:27:52.206419 ana_sdk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.1/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.2/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14685 2023-05-25 20:01:36.382463 ana_sdk-0.2.2/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.2/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.2/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.2/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.2/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.2/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.2/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      333 2023-05-25 19:31:13.365688 ana_sdk-0.2.2/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     4162 2023-05-25 19:48:03.999218 ana_sdk-0.2.2/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-05-25 20:01:51.551945 ana_sdk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.2/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.2/PKG-INFO
```

### Comparing `ana_sdk-0.2.1/ana_sdk/ana.py` & `ana_sdk-0.2.2/ana_sdk/ana.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from requests import HTTPError
 from dotenv import load_dotenv
 
 from .clients.oauth_client import OAuthClient
 from .clients.dashboard_api_client import DashboardAPIClient
 from .clients.rpa_api_client import RPAAPIClient
 from .clients.ana_data_client import ANADataClient
+from .result_factory import ResultFactory
 
 
 class ANA:
     """
     A classe ANA fornece uma interface para interagir com os serviços
     relacionados ao ambiente de automação de negócios, dados e clientes.
     Permite realizar login, executar comandos, definir tenant, cliente
@@ -337,15 +338,15 @@
         return task
 
     def execute(
         self,
         mope: str,
         data: dict,
         wait_for_task: bool = True
-    ) -> tuple[dict, dict] | dict:
+    ):
         """
         Executa o comando identificado pelo MOPE passado utilizando os
         dados passados.
 
         Envia uma requisição para que a RPA API execute um comando
         com base no MOPE e nos dados fornecidos. Valida os dados em
         relação ao JSON Schema antes de fazer a requisição.
@@ -358,34 +359,27 @@
         Args:
             mope (str): O MOPE do comando.
             data (dict): Os dados necessários para o comando de automação.
             wait_for_task (bool): Se deve ou não esperar pela conclusão
             de forma síncrona.
 
         Returns:
-            tuple[dict, dict]: O resultado da automação e a resposta da
-            RPA API no ato do enfileiramento do comando, para propósitos
-            de debug.
+            AbstractResultHandler: O manipulador de resultado da task.
 
         Raises:
-            Exception: Se a tarefa de automação falhar, uma exceção
-            será levantada com a mensagem de erro gerada pela automação.
+            ResultNotFoundError: Se o resultado não estiver presente nas
+            informações da tarefa executada.
+            NoResultHandlerImplementedError: Se não houver um manipulador
+            de resultado implementado para o tipo de resultado em questão.
             jsonschema.ValidationError: Se a pré-validação dos dados
             falhar.
         """
 
         schema = self.rpa.get_json_schema(mope)
         validate(instance=data, schema=schema)
         
         response = self.rpa.execute_command(mope, data)
         task_id = response.get("job_id")
 
         if wait_for_task:
-            task = self._wait_for_task(task_id)
-
-            if task['status'] == "FAILURE":
-                raise Exception(task['erro'])
-            else:
-                return (task['result'], response)
-        
-        else:
-            return response
+            task_info = self._wait_for_task(task_id)
+            return ResultFactory.create_result_handler(task_info)
```

### Comparing `ana_sdk-0.2.1/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.2.2/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.1/ana_sdk/clients/base_client.py` & `ana_sdk-0.2.2/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.1/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.2.2/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.1/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.2.2/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.1/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.2.2/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.1/README.md` & `ana_sdk-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.1/PKG-INFO` & `ana_sdk-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

