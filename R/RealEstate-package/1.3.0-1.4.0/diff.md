# Comparing `tmp/RealEstate_package-1.3.0.tar.gz` & `tmp/RealEstate_package-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealEstate_package-1.3.0.tar", last modified: Wed May 24 17:37:00 2023, max compression
+gzip compressed data, was "RealEstate_package-1.4.0.tar", last modified: Thu May 25 07:46:44 2023, max compression
```

## Comparing `RealEstate_package-1.3.0.tar` & `RealEstate_package-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-24 17:37:00.449520 RealEstate_package-1.3.0/
--rw-rw-r--   0 lada      (1000) lada      (1000)      271 2023-05-24 17:27:43.000000 RealEstate_package-1.3.0/MANIFEST.in
--rw-rw-r--   0 lada      (1000) lada      (1000)     3326 2023-05-24 17:37:00.449520 RealEstate_package-1.3.0/PKG-INFO
--rw-rw-r--   0 lada      (1000) lada      (1000)     2353 2023-05-24 17:36:33.000000 RealEstate_package-1.3.0/README.md
-drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-24 17:37:00.437520 RealEstate_package-1.3.0/RealEstate_package.egg-info/
--rw-rw-r--   0 lada      (1000) lada      (1000)     3326 2023-05-24 17:37:00.000000 RealEstate_package-1.3.0/RealEstate_package.egg-info/PKG-INFO
--rw-rw-r--   0 lada      (1000) lada      (1000)      523 2023-05-24 17:37:00.000000 RealEstate_package-1.3.0/RealEstate_package.egg-info/SOURCES.txt
--rw-rw-r--   0 lada      (1000) lada      (1000)        1 2023-05-24 17:37:00.000000 RealEstate_package-1.3.0/RealEstate_package.egg-info/dependency_links.txt
--rw-rw-r--   0 lada      (1000) lada      (1000)      349 2023-05-24 17:37:00.000000 RealEstate_package-1.3.0/RealEstate_package.egg-info/requires.txt
--rw-rw-r--   0 lada      (1000) lada      (1000)       18 2023-05-24 17:37:00.000000 RealEstate_package-1.3.0/RealEstate_package.egg-info/top_level.txt
--rw-rw-r--   0 lada      (1000) lada      (1000)     2112 2023-05-23 21:30:49.000000 RealEstate_package-1.3.0/pyproject.toml
-drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-24 17:37:00.437520 RealEstate_package-1.3.0/real_estate_model/
--rw-rw-r--   0 lada      (1000) lada      (1000)        0 2023-05-23 19:54:47.000000 RealEstate_package-1.3.0/real_estate_model/__init__.py
--rw-rw-r--   0 lada      (1000) lada      (1000)      910 2023-05-24 14:22:16.000000 RealEstate_package-1.3.0/real_estate_model/config.py
--rw-rw-r--   0 lada      (1000) lada      (1000)      623 2023-05-24 17:27:28.000000 RealEstate_package-1.3.0/real_estate_model/config.yml
--rw-rw-r--   0 lada      (1000) lada      (1000)      963 2023-05-24 14:42:44.000000 RealEstate_package-1.3.0/real_estate_model/predict.py
--rw-rw-r--   0 lada      (1000) lada      (1000)     2487 2023-05-24 14:42:56.000000 RealEstate_package-1.3.0/real_estate_model/train.py
-drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-24 17:37:00.437520 RealEstate_package-1.3.0/real_estate_model/trained_models/
--rw-rw-r--   0 lada      (1000) lada      (1000) 14250145 2023-05-23 19:54:47.000000 RealEstate_package-1.3.0/real_estate_model/trained_models/lgb_model.txt
-drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-24 17:37:00.437520 RealEstate_package-1.3.0/requirements/
--rw-rw-r--   0 lada      (1000) lada      (1000)      349 2023-05-24 08:05:26.000000 RealEstate_package-1.3.0/requirements/requirements.txt
--rw-rw-r--   0 lada      (1000) lada      (1000)      154 2023-05-24 10:50:04.000000 RealEstate_package-1.3.0/requirements/test_requirements.txt
--rw-rw-r--   0 lada      (1000) lada      (1000)      101 2023-05-24 17:37:00.449520 RealEstate_package-1.3.0/setup.cfg
--rw-rw-r--   0 lada      (1000) lada      (1000)     1231 2023-05-24 17:28:43.000000 RealEstate_package-1.3.0/setup.py
+drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-25 07:46:44.300009 RealEstate_package-1.4.0/
+-rw-rw-r--   0 lada      (1000) lada      (1000)      271 2023-05-24 17:27:43.000000 RealEstate_package-1.4.0/MANIFEST.in
+-rw-rw-r--   0 lada      (1000) lada      (1000)     3624 2023-05-25 07:46:44.300009 RealEstate_package-1.4.0/PKG-INFO
+-rw-rw-r--   0 lada      (1000) lada      (1000)     2563 2023-05-24 17:46:20.000000 RealEstate_package-1.4.0/README.md
+drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-25 07:46:44.288009 RealEstate_package-1.4.0/RealEstate_package.egg-info/
+-rw-rw-r--   0 lada      (1000) lada      (1000)     3624 2023-05-25 07:46:44.000000 RealEstate_package-1.4.0/RealEstate_package.egg-info/PKG-INFO
+-rw-rw-r--   0 lada      (1000) lada      (1000)      523 2023-05-25 07:46:44.000000 RealEstate_package-1.4.0/RealEstate_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 lada      (1000) lada      (1000)        1 2023-05-25 07:46:44.000000 RealEstate_package-1.4.0/RealEstate_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 lada      (1000) lada      (1000)      349 2023-05-25 07:46:44.000000 RealEstate_package-1.4.0/RealEstate_package.egg-info/requires.txt
+-rw-rw-r--   0 lada      (1000) lada      (1000)       18 2023-05-25 07:46:44.000000 RealEstate_package-1.4.0/RealEstate_package.egg-info/top_level.txt
+-rw-rw-r--   0 lada      (1000) lada      (1000)     2112 2023-05-23 21:30:49.000000 RealEstate_package-1.4.0/pyproject.toml
+drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-25 07:46:44.288009 RealEstate_package-1.4.0/real_estate_model/
+-rw-rw-r--   0 lada      (1000) lada      (1000)        0 2023-05-23 19:54:47.000000 RealEstate_package-1.4.0/real_estate_model/__init__.py
+-rw-rw-r--   0 lada      (1000) lada      (1000)      910 2023-05-24 14:22:16.000000 RealEstate_package-1.4.0/real_estate_model/config.py
+-rw-rw-r--   0 lada      (1000) lada      (1000)      659 2023-05-25 07:43:48.000000 RealEstate_package-1.4.0/real_estate_model/config.yml
+-rw-rw-r--   0 lada      (1000) lada      (1000)      963 2023-05-24 14:42:44.000000 RealEstate_package-1.4.0/real_estate_model/predict.py
+-rw-rw-r--   0 lada      (1000) lada      (1000)     2590 2023-05-25 07:42:45.000000 RealEstate_package-1.4.0/real_estate_model/train.py
+drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-25 07:46:44.288009 RealEstate_package-1.4.0/real_estate_model/trained_models/
+-rw-rw-r--   0 lada      (1000) lada      (1000) 14250145 2023-05-23 19:54:47.000000 RealEstate_package-1.4.0/real_estate_model/trained_models/lgb_model.txt
+drwxrwxr-x   0 lada      (1000) lada      (1000)        0 2023-05-25 07:46:44.288009 RealEstate_package-1.4.0/requirements/
+-rw-rw-r--   0 lada      (1000) lada      (1000)      349 2023-05-24 08:05:26.000000 RealEstate_package-1.4.0/requirements/requirements.txt
+-rw-rw-r--   0 lada      (1000) lada      (1000)      154 2023-05-24 10:50:04.000000 RealEstate_package-1.4.0/requirements/test_requirements.txt
+-rw-rw-r--   0 lada      (1000) lada      (1000)      101 2023-05-25 07:46:44.304008 RealEstate_package-1.4.0/setup.cfg
+-rw-rw-r--   0 lada      (1000) lada      (1000)     1231 2023-05-25 07:46:25.000000 RealEstate_package-1.4.0/setup.py
```

### Comparing `RealEstate_package-1.3.0/PKG-INFO` & `RealEstate_package-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: RealEstate_package
-Version: 1.3.0
+Version: 1.4.0
 Summary: МЛ-модель, предсказывающая стоимость недвижимости по её параметрам.
 Home-page: https://github.com/Lada-Rom/RealEstate_package
 Author: Клейменов А., Толстенко Л.
 Author-email: notmy@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/Lada-Rom/RealEstate_package
 Description: # Структура проекта
         
         - `real_estate_model/` содержит весь основной код пакета: `train.py`, `predict.py`, `config.py` (загрузка параметров обучения и предсказания из файла `config.yml`). Здесь же находится директория `trained_models/`, куда при обучении будут попадать веса новых моделей, и в которой уже есть одна обученная модель.
         - `requirements/` содержит все необходимые зависимости для использования (`requirements.txt`) и тестирования (`test_requirements.txt`) пакета.
         - `tests/` содержит код тестов, запускаемый при помощи pytest.
         
         
+        # Установка
+        
+        Пакет опубликован на [PyPI](https://pypi.org/project/RealEstate-package/) и устанавливается командой:
+        
+        ```
+        pip install RealEstate-package
+        ```
+        
+        
         # Использование
         
         Код запускается и тестируется при помощи tox. Параметры обучения и предсказания находятся в `real_estate_model/config.yml`.
         
+        
         ## Обучение
         
         В конфиге с параметрам необходимо прописать путь к датасету для обучения - указанный по умолчанию путь работать не будет, так как датасет невозможно загрузить из-за большого размера. Также в конфиге можно указать место для сохранения весов модели (имя автоматическое), какие переменные из датасета не учитывать при обучении и др. Обучение запускается из корневой директории проекта командой:
         
         ```
         tox -e train
         ```
         
+        
         ## Предсказание
         
         Для предсказания в конфиге указывается путь к весам обученной модели (по умолчанию `trained_models/lgb_model.txt`) и список переменных, на которых она обучалась.
         
         ```
         tox -e predict
         ```
```

### Comparing `RealEstate_package-1.3.0/README.md` & `RealEstate_package-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # Структура проекта
 
 - `real_estate_model/` содержит весь основной код пакета: `train.py`, `predict.py`, `config.py` (загрузка параметров обучения и предсказания из файла `config.yml`). Здесь же находится директория `trained_models/`, куда при обучении будут попадать веса новых моделей, и в которой уже есть одна обученная модель.
 - `requirements/` содержит все необходимые зависимости для использования (`requirements.txt`) и тестирования (`test_requirements.txt`) пакета.
 - `tests/` содержит код тестов, запускаемый при помощи pytest.
 
 
+# Установка
+
+Пакет опубликован на [PyPI](https://pypi.org/project/RealEstate-package/) и устанавливается командой:
+
+```
+pip install RealEstate-package
+```
+
+
 # Использование
 
 Код запускается и тестируется при помощи tox. Параметры обучения и предсказания находятся в `real_estate_model/config.yml`.
 
+
 ## Обучение
 
 В конфиге с параметрам необходимо прописать путь к датасету для обучения - указанный по умолчанию путь работать не будет, так как датасет невозможно загрузить из-за большого размера. Также в конфиге можно указать место для сохранения весов модели (имя автоматическое), какие переменные из датасета не учитывать при обучении и др. Обучение запускается из корневой директории проекта командой:
 
 ```
 tox -e train
 ```
 
+
 ## Предсказание
 
 Для предсказания в конфиге указывается путь к весам обученной модели (по умолчанию `trained_models/lgb_model.txt`) и список переменных, на которых она обучалась.
 
 ```
 tox -e predict
 ```
```

### Comparing `RealEstate_package-1.3.0/RealEstate_package.egg-info/PKG-INFO` & `RealEstate_package-1.4.0/RealEstate_package.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: RealEstate-package
-Version: 1.3.0
+Version: 1.4.0
 Summary: МЛ-модель, предсказывающая стоимость недвижимости по её параметрам.
 Home-page: https://github.com/Lada-Rom/RealEstate_package
 Author: Клейменов А., Толстенко Л.
 Author-email: notmy@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/Lada-Rom/RealEstate_package
 Description: # Структура проекта
         
         - `real_estate_model/` содержит весь основной код пакета: `train.py`, `predict.py`, `config.py` (загрузка параметров обучения и предсказания из файла `config.yml`). Здесь же находится директория `trained_models/`, куда при обучении будут попадать веса новых моделей, и в которой уже есть одна обученная модель.
         - `requirements/` содержит все необходимые зависимости для использования (`requirements.txt`) и тестирования (`test_requirements.txt`) пакета.
         - `tests/` содержит код тестов, запускаемый при помощи pytest.
         
         
+        # Установка
+        
+        Пакет опубликован на [PyPI](https://pypi.org/project/RealEstate-package/) и устанавливается командой:
+        
+        ```
+        pip install RealEstate-package
+        ```
+        
+        
         # Использование
         
         Код запускается и тестируется при помощи tox. Параметры обучения и предсказания находятся в `real_estate_model/config.yml`.
         
+        
         ## Обучение
         
         В конфиге с параметрам необходимо прописать путь к датасету для обучения - указанный по умолчанию путь работать не будет, так как датасет невозможно загрузить из-за большого размера. Также в конфиге можно указать место для сохранения весов модели (имя автоматическое), какие переменные из датасета не учитывать при обучении и др. Обучение запускается из корневой директории проекта командой:
         
         ```
         tox -e train
         ```
         
+        
         ## Предсказание
         
         Для предсказания в конфиге указывается путь к весам обученной модели (по умолчанию `trained_models/lgb_model.txt`) и список переменных, на которых она обучалась.
         
         ```
         tox -e predict
         ```
```

### Comparing `RealEstate_package-1.3.0/RealEstate_package.egg-info/SOURCES.txt` & `RealEstate_package-1.4.0/RealEstate_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RealEstate_package-1.3.0/pyproject.toml` & `RealEstate_package-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `RealEstate_package-1.3.0/real_estate_model/config.py` & `RealEstate_package-1.4.0/real_estate_model/config.py`

 * *Files identical despite different names*

### Comparing `RealEstate_package-1.3.0/real_estate_model/config.yml` & `RealEstate_package-1.4.0/real_estate_model/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   - rooms
   - area
   - object_type
   - building_type
   - kitchen_area
 
 # train params
-dataset: ../dataset/Russia_dataset.csv
+dataset: /home/lada/projects/RealEstate_package/dataset/Russia_dataset.csv
 trained_model_path: ./trained_models/
 
 variables_to_drop:
   - date
   - time
   - building_type
   - kitchen_area
```

### Comparing `RealEstate_package-1.3.0/real_estate_model/predict.py` & `RealEstate_package-1.4.0/real_estate_model/predict.py`

 * *Files identical despite different names*

### Comparing `RealEstate_package-1.3.0/real_estate_model/train.py` & `RealEstate_package-1.4.0/real_estate_model/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 def train() -> None:
     # getting train params
     print()
     config = Config(**fetch_config_from_yaml().data)
 
     # read training data
     PACKAGE_ROOT = Path(__file__).resolve().parent
-    DATASET_FILE_PATH = PACKAGE_ROOT / config.dataset
-    data = read_csv(DATASET_FILE_PATH)
+    if Path(config.dataset).is_file():
+        data = read_csv(config.dataset)
+    else:
+        print(f'ERROR! Specify dataset path - file "{config.dataset}" does not exists!')
+        return
 
     # process data
     price = data[data["price"] <= 0].index
     data.drop(price, inplace=True)
 
     rooms = data[data["rooms"] <= 0].index
     data.drop(rooms, inplace=True)
```

### Comparing `RealEstate_package-1.3.0/real_estate_model/trained_models/lgb_model.txt` & `RealEstate_package-1.4.0/real_estate_model/trained_models/lgb_model.txt`

 * *Files identical despite different names*

### Comparing `RealEstate_package-1.3.0/setup.py` & `RealEstate_package-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 REQUIREMENTS_DIR = ROOT_DIR / "requirements"
 def list_reqs(fname="requirements.txt"):
     with open(REQUIREMENTS_DIR / fname) as fd:
         return fd.read().splitlines()
 
 setup(
   name='RealEstate_package',
-  version='1.3.0',
+  version='1.4.0',
   license="BSD-3",
   author='Клейменов А., Толстенко Л.',
   author_email='notmy@gmail.com',
   description='МЛ-модель, предсказывающая стоимость недвижимости по её параметрам.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Lada-Rom/RealEstate_package',
```

