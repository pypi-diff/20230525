# Comparing `tmp/pyjej-0.1.2.tar.gz` & `tmp/pyjej-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjej-0.1.2.tar", max compression
+gzip compressed data, was "pyjej-0.1.3.tar", max compression
```

## Comparing `pyjej-0.1.2.tar` & `pyjej-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7662 2023-05-24 20:03:42.364015 pyjej-0.1.2/README.md
--rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.2/pyjej/__main__.py
--rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.2/pyjej/selflib.py
--rw-r--r--   0        0        0     3002 2023-05-24 20:06:14.371635 pyjej-0.1.2/pyjej/tasks.py
--rw-r--r--   0        0        0      379 2023-05-24 20:07:59.571380 pyjej-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 pyjej-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7897 2023-05-24 20:27:19.164867 pyjej-0.1.3/README.md
+-rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.3/pyjej/__main__.py
+-rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.3/pyjej/selflib.py
+-rw-r--r--   0        0        0     3511 2023-05-25 06:37:24.300533 pyjej-0.1.3/pyjej/tasks.py
+-rw-r--r--   0        0        0      400 2023-05-25 06:38:17.676288 pyjej-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8528 1970-01-01 00:00:00.000000 pyjej-0.1.3/PKG-INFO
```

### Comparing `pyjej-0.1.2/README.md` & `pyjej-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # README.md
 
 Этот репозиторий содержит код для взаимодействия с Jenkins с использованием библиотеки `invoke`. Он предоставляет функциональность для экспорта всех заданий из Jenkins и создания/обновления конкретных заданий.
 
 ## Предварительные требования
 
--   Python 3.6 или выше
+-   Python 3.8 или выше
 -   Библиотека `invoke`
 -   Библиотека `pyyaml`
 
 ## Начало работы
 
 1. Клонируйте этот репозиторий на свой локальный компьютер.
 2. Установите необходимые зависимости, выполнив следующую команду:
@@ -17,38 +17,44 @@
     ```
 3. Настройте информацию о сервере Jenkins в файле `inventory.yml`. Добавьте необходимую информацию о серверах Jenkins, с которыми вы хотите взаимодействовать.
 
 ## Пример
 
 Вот пример использования задач:
 
-1. Экспорт всех заданий с сервера Jenkins:
+1. Экспорт всех заданий с сервера Jenkins в XML файлы:
 
     ```
     python -m pyjej job.export-all -s мой_сервер_jenkins
     ```
 
-2. Создание задания на сервере Jenkins:
+2. Создание задания на сервере Jenkins из XML файла:
 
     ```
     python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -i входная_папка
     ```
 
-3. Обновление задания на сервере Jenkins:
+3. Обновление задания на сервере Jenkins из XML файла:
 
     ```
     python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -i входная_папка
     ```
 
-4. Экспорт всех плагинов
+4. Экспорт всех плагинов:
 
     ```
     python -m pyjej plugins.export-all -s мой_сервер_jenkins
     ```
 
+5. Установка указного плагина в Jenkins:
+
+    ```
+    python -m pyjej plugins.install -s мой_сервер_jenkins -p имя_плагина
+    ```
+
 Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
 
 ## Использование
 
 ### tasks.py
 
 В этом файле содержатся основные задачи для взаимодействия с Jenkins.
```

### Comparing `pyjej-0.1.2/pyjej/selflib.py` & `pyjej-0.1.3/pyjej/selflib.py`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.2/pyjej/tasks.py` & `pyjej-0.1.3/pyjej/tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import pathlib
-
+import requests
 from invoke import Collection, Result, task
 
 from .selflib import getInventory, os_exe_async
 
 
 INVENTORY = getInventory(os.getenv("INVENTORY_FILE"))
 
@@ -58,39 +58,49 @@
     base_command_cli = INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
     res: Result = ctx.run(
         f"{base_command_cli} list-plugins",
     )
     print(res)
     if not res.stderr:
-        pathlib.Path("data", server, "plains.txt").write_text(res.stdout)
+        pathlib.Path("data", server, "plugins.txt").write_text(res.stdout)
 
 
 @task
 def install_plugins(ctx, server: str, plugin: str):
     """Установить указанный плагин"""
     base_command_cli = INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
     res: Result = ctx.run(
         f"{base_command_cli} install-plugin {plugin}",
     )
     print(res)
 
 
 @task
-def my_task(ctx):
-    print("!!")
-    ctx.run("ls")
+def export_JCasC(ctx, server: str):
+    """Скачать настройки из плагина Jenkins Configuration as Code"""
+    i = INVENTORY[server]
+    res: requests.Response = requests.post(
+        f"http://{i['JENKINS_USER_ID']}:{i['JENKINS_API_TOKEN']}@{i['JENKINS_URL']}/configuration-as-code/export"
+    )
+    print(res.text)
+    if res.status_code == 200 and res.text:
+        pathlib.Path("data", server, "jenkins.yaml").write_text(res.text)
 
 
 job_nsp = Collection()
 job_nsp.add_task(export_all_jobs, "export-all")
 job_nsp.add_task(create_job, "create")
 job_nsp.add_task(update_job, "update")
 
 plugins_nsp = Collection()
 plugins_nsp.add_task(export_all_plugins, "export-all")
 plugins_nsp.add_task(install_plugins, "install")
+
+jcasc_nsp = Collection()
+jcasc_nsp.add_task(export_JCasC, "export")
+
 namespace = Collection()
 namespace.add_collection(job_nsp, "job")
 namespace.add_collection(plugins_nsp, "plugins")
-namespace.add_task(my_task)
+namespace.add_collection(jcasc_nsp, "jcasc")
```

### Comparing `pyjej-0.1.2/PKG-INFO` & `pyjej-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pyjej
-Version: 0.1.2
+Version: 0.1.3
 Summary: Проект для взаимодействия с Jenkins через CLI
 Author: Кустов Денис
 Author-email: kudv@pkzdrav.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: invoke (>=2.1.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # README.md
 
 Этот репозиторий содержит код для взаимодействия с Jenkins с использованием библиотеки `invoke`. Он предоставляет функциональность для экспорта всех заданий из Jenkins и создания/обновления конкретных заданий.
 
 ## Предварительные требования
 
--   Python 3.6 или выше
+-   Python 3.8 или выше
 -   Библиотека `invoke`
 -   Библиотека `pyyaml`
 
 ## Начало работы
 
 1. Клонируйте этот репозиторий на свой локальный компьютер.
 2. Установите необходимые зависимости, выполнив следующую команду:
@@ -33,38 +34,44 @@
     ```
 3. Настройте информацию о сервере Jenkins в файле `inventory.yml`. Добавьте необходимую информацию о серверах Jenkins, с которыми вы хотите взаимодействовать.
 
 ## Пример
 
 Вот пример использования задач:
 
-1. Экспорт всех заданий с сервера Jenkins:
+1. Экспорт всех заданий с сервера Jenkins в XML файлы:
 
     ```
     python -m pyjej job.export-all -s мой_сервер_jenkins
     ```
 
-2. Создание задания на сервере Jenkins:
+2. Создание задания на сервере Jenkins из XML файла:
 
     ```
     python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -i входная_папка
     ```
 
-3. Обновление задания на сервере Jenkins:
+3. Обновление задания на сервере Jenkins из XML файла:
 
     ```
     python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -i входная_папка
     ```
 
-4. Экспорт всех плагинов
+4. Экспорт всех плагинов:
 
     ```
     python -m pyjej plugins.export-all -s мой_сервер_jenkins
     ```
 
+5. Установка указного плагина в Jenkins:
+
+    ```
+    python -m pyjej plugins.install -s мой_сервер_jenkins -p имя_плагина
+    ```
+
 Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
 
 ## Использование
 
 ### tasks.py
 
 В этом файле содержатся основные задачи для взаимодействия с Jenkins.
```

