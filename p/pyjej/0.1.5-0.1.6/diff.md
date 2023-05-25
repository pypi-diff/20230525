# Comparing `tmp/pyjej-0.1.5.tar.gz` & `tmp/pyjej-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjej-0.1.5.tar", max compression
+gzip compressed data, was "pyjej-0.1.6.tar", max compression
```

## Comparing `pyjej-0.1.5.tar` & `pyjej-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9524 2023-05-25 10:26:47.612345 pyjej-0.1.5/README.md
--rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.5/pyjej/__main__.py
--rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.5/pyjej/selflib.py
--rw-r--r--   0        0        0     3725 2023-05-25 10:52:10.585147 pyjej-0.1.5/pyjej/tasks.py
--rw-r--r--   0        0        0      400 2023-05-25 10:52:24.725155 pyjej-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    10155 1970-01-01 00:00:00.000000 pyjej-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     9522 2023-05-25 11:06:33.644668 pyjej-0.1.6/README.md
+-rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.6/pyjej/__main__.py
+-rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.6/pyjej/selflib.py
+-rw-r--r--   0        0        0     3701 2023-05-25 11:12:00.060233 pyjej-0.1.6/pyjej/tasks.py
+-rw-r--r--   0        0        0      400 2023-05-25 11:13:50.644074 pyjej-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    10153 1970-01-01 00:00:00.000000 pyjej-0.1.6/PKG-INFO
```

### Comparing `pyjej-0.1.5/README.md` & `pyjej-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 ### tasks.py
 
 В этом файле содержатся основные задачи для взаимодействия с Jenkins.
 
 #### Задача `job.export`
 
-Эта задача экспортирует указанную задачу с указанного сервера Jenkins и сохраняет её в виде файлов XML.
+Эта задача экспортирует указанную задачу с указанного сервера Jenkins и сохраняет её в виде файла XML.
 
 **Использование:**
 
 ```shell
 python -m pyjej job.export --server <имя_сервера> --jobname <имя_задания>
 ```
```

### Comparing `pyjej-0.1.5/pyjej/selflib.py` & `pyjej-0.1.6/pyjej/selflib.py`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.5/pyjej/tasks.py` & `pyjej-0.1.6/pyjej/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,15 @@
     )
 
 
 @task
 def export_all_plugins(ctx: Runner, server: str):
     """Получить список всех плагинов"""
 
-    res: Result = ctx.run(
-        f"{get_base_command_cli(server)} list-plugins",
-    )
+    res: Result = ctx.run(f"{get_base_command_cli(server)} list-plugins", hide=True)
     if not res.stderr:
         pathlib.Path("data", server, "plugins.txt").write_text(res.stdout)
 
 
 @task
 def install_plugins(ctx: Runner, server: str, plugin: str):
     """Установить указанный плагин"""
@@ -83,15 +81,14 @@
 @task
 def export_JCasC(ctx: Runner, server: str):
     """Загрузить настройки из плагина 'Jenkins Configuration as Code'"""
     i = INVENTORY[server]
     res: requests.Response = requests.post(
         f"http://{i['JENKINS_USER_ID']}:{i['JENKINS_API_TOKEN']}@{i['JENKINS_URL']}/configuration-as-code/export"
     )
-    print(res.text)
     if res.status_code == 200 and res.text:
         pathlib.Path("data", server, "jenkins.yaml").write_text(res.text)
 
 
 job_nsp = Collection()
 job_nsp.add_task(export_all_jobs, "export-all")
 job_nsp.add_task(export_job, "export")
```

### Comparing `pyjej-0.1.5/PKG-INFO` & `pyjej-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjej
-Version: 0.1.5
+Version: 0.1.6
 Summary: Проект для взаимодействия с Jenkins через CLI
 Author: Кустов Денис
 Author-email: kudv@pkzdrav.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -86,15 +86,15 @@
 
 ### tasks.py
 
 В этом файле содержатся основные задачи для взаимодействия с Jenkins.
 
 #### Задача `job.export`
 
-Эта задача экспортирует указанную задачу с указанного сервера Jenkins и сохраняет её в виде файлов XML.
+Эта задача экспортирует указанную задачу с указанного сервера Jenkins и сохраняет её в виде файла XML.
 
 **Использование:**
 
 ```shell
 python -m pyjej job.export --server <имя_сервера> --jobname <имя_задания>
 ```
```

