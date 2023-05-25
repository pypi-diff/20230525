# Comparing `tmp/pyjej-0.1.3.tar.gz` & `tmp/pyjej-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjej-0.1.3.tar", max compression
+gzip compressed data, was "pyjej-0.1.4.tar", max compression
```

## Comparing `pyjej-0.1.3.tar` & `pyjej-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7897 2023-05-24 20:27:19.164867 pyjej-0.1.3/README.md
--rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.3/pyjej/__main__.py
--rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.3/pyjej/selflib.py
--rw-r--r--   0        0        0     3511 2023-05-25 06:37:24.300533 pyjej-0.1.3/pyjej/tasks.py
--rw-r--r--   0        0        0      400 2023-05-25 06:38:17.676288 pyjej-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8528 1970-01-01 00:00:00.000000 pyjej-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     8765 2023-05-25 06:46:51.184961 pyjej-0.1.4/README.md
+-rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.4/pyjej/__main__.py
+-rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.4/pyjej/selflib.py
+-rw-r--r--   0        0        0     3511 2023-05-25 06:47:05.901019 pyjej-0.1.4/pyjej/tasks.py
+-rw-r--r--   0        0        0      400 2023-05-25 06:47:53.857212 pyjej-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9396 1970-01-01 00:00:00.000000 pyjej-0.1.4/PKG-INFO
```

### Comparing `pyjej-0.1.3/README.md` & `pyjej-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 
 5. Установка указного плагина в Jenkins:
 
     ```
     python -m pyjej plugins.install -s мой_сервер_jenkins -p имя_плагина
     ```
 
+6. Скачать настройки из плагина Jenkins Configuration as Code:
+
+    ```
+    python -m pyjej jcasc.export -s мой_сервер_jenkins
+    ```
+
 Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
 
 ## Использование
 
 ### tasks.py
 
 В этом файле содержатся основные задачи для взаимодействия с Jenkins.
@@ -74,29 +80,29 @@
 #### Задача `job.create`
 
 Эта задача создает конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для создания.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `job.update`
 
 Эта задача обновляет конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для обновления.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `plugins.export-all`
@@ -124,14 +130,29 @@
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_плагина>`: Имя плагина, который нужно установить.
 
 Результат выполнения команды будет выведен на экран.
 
+#### Задача `jcasc.export`
+
+Эта задача позволяет скачать конфигурации Jenkins которые формируются через плагин `Jenkins Configuration as Code (a.k.a. JCasC) Plugin`.
+https://github.com/jenkinsci/configuration-as-code-plugin
+
+**Использование:**
+
+```shell
+python -m pyjej jcasc.export --server <имя_сервера>
+```
+
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
+
+Результат выполнения команды будет выведен на экран и записан в файл `data/<имя_сервера>/jenkins.yaml`.
+
 # Пример создания файла inventory.yml
 
 Файл `inventory.yml` используется для настройки подключения к серверам Jenkins в коде. В этой главе мы предоставим пример создания файла `inventory.yml` с фиктивными значениями.
 
 Пример содержимого файла `inventory.yml`:
 
 ```yaml
```

### Comparing `pyjej-0.1.3/pyjej/selflib.py` & `pyjej-0.1.4/pyjej/selflib.py`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.3/pyjej/tasks.py` & `pyjej-0.1.4/pyjej/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,31 +27,31 @@
         handle=lambda label, stdout, stderr, cod, cmd: pathlib.Path(
             "data", server, "jobs", f"{label}.xml"
         ).write_text(stdout),
     )
 
 
 @task
-def create_job(ctx, server: str, jobname: str, in_folder):
+def create_job(ctx, server: str, jobname: str, in_server):
     """Создать указанную Job на Jenkins"""
     base_command_cli = INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
     res: Result = ctx.run(
-        f"{base_command_cli} create-job {jobname} < {pathlib.Path('data', in_folder,'jobs',f'{jobname}.xml')}",
+        f"{base_command_cli} create-job {jobname} < {pathlib.Path('data', in_server,'jobs',f'{jobname}.xml')}",
     )
     print(res)
 
 
 @task
-def update_job(ctx, server: str, jobname: str, in_folder):
+def update_job(ctx, server: str, jobname: str, in_server):
     """Обновить указанный Job в Jenkins"""
     base_command_cli = INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
     res: Result = ctx.run(
-        f"{base_command_cli} update-job {jobname} < {pathlib.Path('data',in_folder,'jobs',f'{jobname}.xml')}",
+        f"{base_command_cli} update-job {jobname} < {pathlib.Path('data',in_server,'jobs',f'{jobname}.xml')}",
     )
     print(res)
 
 
 @task
 def export_all_plugins(ctx, server: str):
     """Получить список всех плагинов"""
```

### Comparing `pyjej-0.1.3/PKG-INFO` & `pyjej-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjej
-Version: 0.1.3
+Version: 0.1.4
 Summary: Проект для взаимодействия с Jenkins через CLI
 Author: Кустов Денис
 Author-email: kudv@pkzdrav.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -64,14 +64,20 @@
 
 5. Установка указного плагина в Jenkins:
 
     ```
     python -m pyjej plugins.install -s мой_сервер_jenkins -p имя_плагина
     ```
 
+6. Скачать настройки из плагина Jenkins Configuration as Code:
+
+    ```
+    python -m pyjej jcasc.export -s мой_сервер_jenkins
+    ```
+
 Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
 
 ## Использование
 
 ### tasks.py
 
 В этом файле содержатся основные задачи для взаимодействия с Jenkins.
@@ -91,29 +97,29 @@
 #### Задача `job.create`
 
 Эта задача создает конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для создания.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `job.update`
 
 Эта задача обновляет конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_folder <входная_папка>
+python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для обновления.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `plugins.export-all`
@@ -141,14 +147,29 @@
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_плагина>`: Имя плагина, который нужно установить.
 
 Результат выполнения команды будет выведен на экран.
 
+#### Задача `jcasc.export`
+
+Эта задача позволяет скачать конфигурации Jenkins которые формируются через плагин `Jenkins Configuration as Code (a.k.a. JCasC) Plugin`.
+https://github.com/jenkinsci/configuration-as-code-plugin
+
+**Использование:**
+
+```shell
+python -m pyjej jcasc.export --server <имя_сервера>
+```
+
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
+
+Результат выполнения команды будет выведен на экран и записан в файл `data/<имя_сервера>/jenkins.yaml`.
+
 # Пример создания файла inventory.yml
 
 Файл `inventory.yml` используется для настройки подключения к серверам Jenkins в коде. В этой главе мы предоставим пример создания файла `inventory.yml` с фиктивными значениями.
 
 Пример содержимого файла `inventory.yml`:
 
 ```yaml
```

