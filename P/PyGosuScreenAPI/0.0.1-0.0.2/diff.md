# Comparing `tmp/PyGosuScreenAPI-0.0.1.tar.gz` & `tmp/PyGosuScreenAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGosuScreenAPI-0.0.1.tar", last modified: Mon May  1 21:25:02 2023, max compression
+gzip compressed data, was "PyGosuScreenAPI-0.0.2.tar", last modified: Thu May 25 08:52:52 2023, max compression
```

## Comparing `PyGosuScreenAPI-0.0.1.tar` & `PyGosuScreenAPI-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zcxw       (501) staff       (20)        0 2023-05-01 21:25:02.243954 PyGosuScreenAPI-0.0.1/
-drwxr-xr-x   0 zcxw       (501) staff       (20)        0 2023-05-01 21:25:02.242889 PyGosuScreenAPI-0.0.1/GosuScreenAPI/
--rw-r--r--   0 zcxw       (501) staff       (20)       51 2023-05-01 20:41:02.000000 PyGosuScreenAPI-0.0.1/GosuScreenAPI/__init__.py
--rw-r--r--   0 zcxw       (501) staff       (20)     3040 2023-05-01 20:47:00.000000 PyGosuScreenAPI-0.0.1/GosuScreenAPI/api.py
--rw-r--r--   0 zcxw       (501) staff       (20)      979 2023-05-01 21:25:02.243832 PyGosuScreenAPI-0.0.1/PKG-INFO
-drwxr-xr-x   0 zcxw       (501) staff       (20)        0 2023-05-01 21:25:02.243652 PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/
--rw-r--r--   0 zcxw       (501) staff       (20)      979 2023-05-01 21:25:02.000000 PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/PKG-INFO
--rw-r--r--   0 zcxw       (501) staff       (20)      259 2023-05-01 21:25:02.000000 PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/SOURCES.txt
--rw-r--r--   0 zcxw       (501) staff       (20)        1 2023-05-01 21:25:02.000000 PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/dependency_links.txt
--rw-r--r--   0 zcxw       (501) staff       (20)       17 2023-05-01 21:25:02.000000 PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/requires.txt
--rw-r--r--   0 zcxw       (501) staff       (20)       14 2023-05-01 21:25:02.000000 PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/top_level.txt
--rw-r--r--   0 zcxw       (501) staff       (20)      545 2023-05-01 21:21:04.000000 PyGosuScreenAPI-0.0.1/README.md
--rw-r--r--   0 zcxw       (501) staff       (20)       38 2023-05-01 21:25:02.243991 PyGosuScreenAPI-0.0.1/setup.cfg
--rw-r--r--   0 zcxw       (501) staff       (20)     2712 2023-05-01 21:24:35.000000 PyGosuScreenAPI-0.0.1/setup.py
+drwxr-xr-x   0 zcxw       (501) staff       (20)        0 2023-05-25 08:52:52.532488 PyGosuScreenAPI-0.0.2/
+drwxr-xr-x   0 zcxw       (501) staff       (20)        0 2023-05-25 08:52:52.531563 PyGosuScreenAPI-0.0.2/GosuScreenAPI/
+-rw-r--r--   0 zcxw       (501) staff       (20)       51 2023-05-01 20:41:02.000000 PyGosuScreenAPI-0.0.2/GosuScreenAPI/__init__.py
+-rw-r--r--   0 zcxw       (501) staff       (20)     4138 2023-05-25 08:47:20.000000 PyGosuScreenAPI-0.0.2/GosuScreenAPI/api.py
+-rw-r--r--   0 zcxw       (501) staff       (20)     1097 2023-05-25 08:52:52.532372 PyGosuScreenAPI-0.0.2/PKG-INFO
+drwxr-xr-x   0 zcxw       (501) staff       (20)        0 2023-05-25 08:52:52.532198 PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/
+-rw-r--r--   0 zcxw       (501) staff       (20)     1097 2023-05-25 08:52:52.000000 PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/PKG-INFO
+-rw-r--r--   0 zcxw       (501) staff       (20)      259 2023-05-25 08:52:52.000000 PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 zcxw       (501) staff       (20)        1 2023-05-25 08:52:52.000000 PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 zcxw       (501) staff       (20)        9 2023-05-25 08:52:52.000000 PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/requires.txt
+-rw-r--r--   0 zcxw       (501) staff       (20)       14 2023-05-25 08:52:52.000000 PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/top_level.txt
+-rw-r--r--   0 zcxw       (501) staff       (20)      663 2023-05-25 08:52:25.000000 PyGosuScreenAPI-0.0.2/README.md
+-rw-r--r--   0 zcxw       (501) staff       (20)       38 2023-05-25 08:52:52.532524 PyGosuScreenAPI-0.0.2/setup.cfg
+-rw-r--r--   0 zcxw       (501) staff       (20)     2837 2023-05-25 08:50:54.000000 PyGosuScreenAPI-0.0.2/setup.py
```

### Comparing `PyGosuScreenAPI-0.0.1/GosuScreenAPI/api.py` & `PyGosuScreenAPI-0.0.2/GosuScreenAPI/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,41 @@
 
     def return_image(self, bytes_image: bytes, name: str):
         image = io.BytesIO(bytes_image)
         image.seek(0)
         image.name = name
         return image
 
+    def get_qrcodepro(self, service: int, config: dict):
+        """
+        Параметр	Тип	Описание
+        token	строка	Обязательный. Ваш ключ API
+        service	число	Обязательный. ID сервиса, который будет генерироваться.
+        config	dict	Обязательный. Параметры для qrcode
+
+        Возвращает тип: io.BytesIO(image)
+
+        При ошибке: application/json
+        """
+        try:
+            data = {
+                'token': self.token,
+                'service': str(service),
+                'config': config
+            }
+            response = requests.post(
+                self.main_url + '/qrcodepro', data=json.dumps(data), headers=self.headers)
+            if response.headers.get('Content-Type') == 'application/json':
+                return response.json()
+            else:
+                return self.return_image(response.content, 'qrcode.png')
+        except:
+            return {'status': 'error', 'message': str(sys.exc_info()[1])}
+
+
     def get_qrcode(self, service: int, value: str):
         """
         Параметр	Тип	Описание
         token	строка	Обязательный. Ваш ключ API
         service	число	Обязательный. ID сервиса, который будет генерироваться.
         value	строка	Обязательный. Текст для кодирования. Любой текст
```

### Comparing `PyGosuScreenAPI-0.0.1/PKG-INFO` & `PyGosuScreenAPI-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGosuScreenAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Библиотека Python для GosuScreen API
 Home-page: https://github.com/zcxw-code/GosuScreenAPI
 Author: zcxw
 Author-email: zcxw.code@hotmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,10 +15,11 @@
 # **Библиотека  Python для GosuScreen API**
 ## Документация по запросам
 
 | Название  | Ссылка |
 | ------------- | ------------- |
 | Генерация QRCode  | [QRCode.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/QRCode.md)  |
 | Генерация скриншотов  | [Screen.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/Screen.md) |
+| Генерация QRCodePro  | [QRCodePro.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/QRCodePro.md) |
 ## Authors
 
 - [@zcxw](https://github.com/zcxw-code)
```

### Comparing `PyGosuScreenAPI-0.0.1/PyGosuScreenAPI.egg-info/PKG-INFO` & `PyGosuScreenAPI-0.0.2/PyGosuScreenAPI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGosuScreenAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Библиотека Python для GosuScreen API
 Home-page: https://github.com/zcxw-code/GosuScreenAPI
 Author: zcxw
 Author-email: zcxw.code@hotmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,10 +15,11 @@
 # **Библиотека  Python для GosuScreen API**
 ## Документация по запросам
 
 | Название  | Ссылка |
 | ------------- | ------------- |
 | Генерация QRCode  | [QRCode.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/QRCode.md)  |
 | Генерация скриншотов  | [Screen.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/Screen.md) |
+| Генерация QRCodePro  | [QRCodePro.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/QRCodePro.md) |
 ## Authors
 
 - [@zcxw](https://github.com/zcxw-code)
```

### Comparing `PyGosuScreenAPI-0.0.1/README.md` & `PyGosuScreenAPI-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,10 +2,11 @@
 # **Библиотека  Python для GosuScreen API**
 ## Документация по запросам
 
 | Название  | Ссылка |
 | ------------- | ------------- |
 | Генерация QRCode  | [QRCode.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/QRCode.md)  |
 | Генерация скриншотов  | [Screen.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/Screen.md) |
+| Генерация QRCodePro  | [QRCodePro.md](https://github.com/zcxw-code/GosuScreenAPI/blob/main/QRCodePro.md) |
 ## Authors
 
 - [@zcxw](https://github.com/zcxw-code)
```

### Comparing `PyGosuScreenAPI-0.0.1/setup.py` & `PyGosuScreenAPI-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Импорт недавно установленного пакета setuptools.
 import setuptools
 
 # Открытие README.md и присвоение его long_description.
 with open("README.md", "r") as fh:
-	long_description = fh.read()
+    long_description = fh.read()
 
 # Определение requests как requirements для того, чтобы этот пакет работал. Зависимости проекта.
-requirements = ["requests<=2.21.0"]
+requirements = ["requests"]
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setuptools.setup(
-	# Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
-	name="PyGosuScreenAPI",
-	# Номер версии вашего пакета. Обычно используется семантическое управление версиями.
-	version="0.0.1",
-	# Имя автора.
-	author="zcxw",
-	# Его почта.
-	author_email="zcxw.code@hotmail.com",
-	# Краткое описание, которое будет показано на странице PyPi.
-	description="Библиотека Python для GosuScreen API",
-	# Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
-	long_description=long_description,
-	# Определяет тип контента, используемый в long_description.
-	long_description_content_type="text/markdown",
-	# URL-адрес, представляющий домашнюю страницу проекта. Большинство проектов ссылаются на репозиторий.
-	url="https://github.com/zcxw-code/GosuScreenAPI",
-	# Находит все пакеты внутри проекта и объединяет их в дистрибутив.
-	packages=setuptools.find_packages(),
-	# requirements или dependencies, которые будут установлены вместе с пакетом, когда пользователь установит его через pip.
-	install_requires=requirements,
-	# Предоставляет pip некоторые метаданные о пакете. Также отображается на странице PyPi.
-	classifiers=[
-		"Programming Language :: Python :: 3.10",
-		"License :: OSI Approved :: MIT License",
-		"Operating System :: OS Independent",
-	],
-	# Требуемая версия Python.
-	python_requires='>=3.7',
+    # Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
+    name="PyGosuScreenAPI",
+    # Номер версии вашего пакета. Обычно используется семантическое управление версиями.
+    version="0.0.2",
+    # Имя автора.
+    author="zcxw",
+    # Его почта.
+    author_email="zcxw.code@hotmail.com",
+    # Краткое описание, которое будет показано на странице PyPi.
+    description="Библиотека Python для GosuScreen API",
+    # Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
+    long_description=long_description,
+    # Определяет тип контента, используемый в long_description.
+    long_description_content_type="text/markdown",
+    # URL-адрес, представляющий домашнюю страницу проекта. Большинство проектов ссылаются на репозиторий.
+    url="https://github.com/zcxw-code/GosuScreenAPI",
+    # Находит все пакеты внутри проекта и объединяет их в дистрибутив.
+        packages=setuptools.find_packages(),
+        # requirements или dependencies, которые будут установлены вместе с пакетом, когда пользователь установит его через pip.
+        install_requires=requirements,
+        # Предоставляет pip некоторые метаданные о пакете. Также отображается на странице PyPi.
+        classifiers=[
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: OS Independent",
+        ],
+    # Требуемая версия Python.
+    python_requires='>=3.7',
 
-)
+)
```

