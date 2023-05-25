# Comparing `tmp/gerador_posts-0.0.1.tar.gz` & `tmp/gerador_posts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerador_posts-0.0.1.tar", last modified: Thu May 25 19:39:37 2023, max compression
+gzip compressed data, was "gerador_posts-0.1.0.tar", last modified: Thu May 25 21:50:58 2023, max compression
```

## Comparing `gerador_posts-0.0.1.tar` & `gerador_posts-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-25 19:39:37.181709 gerador_posts-0.0.1/
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1076 2023-05-25 13:15:36.000000 gerador_posts-0.0.1/LICENSE
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1400 2023-05-25 19:39:37.181709 gerador_posts-0.0.1/PKG-INFO
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1015 2023-05-25 19:20:18.000000 gerador_posts-0.0.1/README.md
-drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-25 19:39:37.181709 gerador_posts-0.0.1/gerador_posts/
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        0 2023-05-25 17:56:44.000000 gerador_posts-0.0.1/gerador_posts/__init__.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      426 2023-05-25 17:09:28.000000 gerador_posts-0.0.1/gerador_posts/__main__.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1189 2023-05-25 17:08:30.000000 gerador_posts-0.0.1/gerador_posts/configuracao.py
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      831 2023-05-25 18:29:15.000000 gerador_posts-0.0.1/gerador_posts/tratar_dados.py
-drwxrwxr-x   0 ufpe      (1000) ufpe      (1000)        0 2023-05-25 19:39:37.181709 gerador_posts-0.0.1/gerador_posts.egg-info/
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)     1400 2023-05-25 19:39:37.000000 gerador_posts-0.0.1/gerador_posts.egg-info/PKG-INFO
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      358 2023-05-25 19:39:37.000000 gerador_posts-0.0.1/gerador_posts.egg-info/SOURCES.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        1 2023-05-25 19:39:37.000000 gerador_posts-0.0.1/gerador_posts.egg-info/dependency_links.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)        1 2023-05-25 19:32:41.000000 gerador_posts-0.0.1/gerador_posts.egg-info/not-zip-safe
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       44 2023-05-25 19:39:37.000000 gerador_posts-0.0.1/gerador_posts.egg-info/requires.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       14 2023-05-25 19:39:37.000000 gerador_posts-0.0.1/gerador_posts.egg-info/top_level.txt
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)       38 2023-05-25 19:39:37.181709 gerador_posts-0.0.1/setup.cfg
--rw-rw-r--   0 ufpe      (1000) ufpe      (1000)      738 2023-05-25 19:38:44.000000 gerador_posts-0.0.1/setup.py
+drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1076 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/LICENSE
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1386 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/PKG-INFO
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1001 2023-05-25 21:41:43.000000 gerador_posts-0.1.0/README.md
+drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/gerador_posts/
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/__init__.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       86 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/__main__.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1189 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/configuracao.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      418 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/gerador_posts.py
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      831 2023-05-25 21:40:24.000000 gerador_posts-0.1.0/gerador_posts/tratar_dados.py
+drwxrwxr-x   0 cecivieira  (1000) cecivieira  (1000)        0 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/gerador_posts.egg-info/
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)     1386 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/PKG-INFO
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      429 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/SOURCES.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        1 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/dependency_links.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       74 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/entry_points.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)        1 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/not-zip-safe
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       44 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/requires.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       14 2023-05-25 21:50:58.000000 gerador_posts-0.1.0/gerador_posts.egg-info/top_level.txt
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)       38 2023-05-25 21:50:58.452872 gerador_posts-0.1.0/setup.cfg
+-rw-rw-r--   0 cecivieira  (1000) cecivieira  (1000)      873 2023-05-25 21:50:13.000000 gerador_posts-0.1.0/setup.py
```

### Comparing `gerador_posts-0.0.1/LICENSE` & `gerador_posts-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.0.1/PKG-INFO` & `gerador_posts-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerador_posts
-Version: 0.0.1
+Version: 0.1.0
 Summary: Gerador de posts baseado em templates e dados 
 Home-page: https://github.com/cecivieira/gerador-posts
 Author: Ana Cecília Vieira
 Author-email: cecivieira@gmail.com
 License: MIT
 Keywords: jinja2,yaml,templates
 Platform: UNKNOWN
@@ -16,24 +16,24 @@
 Gerador de posts baseado em templates e dados armazenados em arquivo csv.
 
 Essa aplicação surgiu da necessidade de gerar textos a partir de um template, cujos dados deveriam ser coletados de um arquivo .csv e .yaml. Então, é isso que esse programa faz: ler dados de um arquivo .csv, outros dados de um arquivo .yaml e preenche um ou mais templates.
 
 ## Instalação
 
 ```bash
-(.venv) $ pip install gerador_posts
+(.venv) $ pip install gerador-posts
 ```
 
 ## Uso
 
 1. Crie os dados:
     1. Crie a pasta `./dados`;
     1. Dentro dessa pasta, crie dois arquivos de dados: `links.csv` e `variaveis.yaml` (os arquivos devem ter exatamente esses títulos).
 1. Crie os templates:
     1. Crie a pasta `./posts_templates`;
     1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir dados no template use a sintaxe do Jinja2).
 1. Crie a pasta aonde os posts prontos serão armazenados: `./posts_prontos`;
 1. Execute o pacote:
     ```bash
-    (.venv) $ pip install gerador_posts
+    (.venv) $ gerar-posts
     ```
```

### Comparing `gerador_posts-0.0.1/README.md` & `gerador_posts-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Gerador de posts baseado em templates e dados armazenados em arquivo csv.
 
 Essa aplicação surgiu da necessidade de gerar textos a partir de um template, cujos dados deveriam ser coletados de um arquivo .csv e .yaml. Então, é isso que esse programa faz: ler dados de um arquivo .csv, outros dados de um arquivo .yaml e preenche um ou mais templates.
 
 ## Instalação
 
 ```bash
-(.venv) $ pip install gerador_posts
+(.venv) $ pip install gerador-posts
 ```
 
 ## Uso
 
 1. Crie os dados:
     1. Crie a pasta `./dados`;
     1. Dentro dessa pasta, crie dois arquivos de dados: `links.csv` e `variaveis.yaml` (os arquivos devem ter exatamente esses títulos).
 1. Crie os templates:
     1. Crie a pasta `./posts_templates`;
     1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir dados no template use a sintaxe do Jinja2).
 1. Crie a pasta aonde os posts prontos serão armazenados: `./posts_prontos`;
 1. Execute o pacote:
     ```bash
-    (.venv) $ pip install gerador_posts
+    (.venv) $ gerar-posts
     ```
```

### Comparing `gerador_posts-0.0.1/gerador_posts/configuracao.py` & `gerador_posts-0.1.0/gerador_posts/configuracao.py`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.0.1/gerador_posts/tratar_dados.py` & `gerador_posts-0.1.0/gerador_posts/tratar_dados.py`

 * *Files identical despite different names*

### Comparing `gerador_posts-0.0.1/gerador_posts.egg-info/PKG-INFO` & `gerador_posts-0.1.0/gerador_posts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerador-posts
-Version: 0.0.1
+Version: 0.1.0
 Summary: Gerador de posts baseado em templates e dados 
 Home-page: https://github.com/cecivieira/gerador-posts
 Author: Ana Cecília Vieira
 Author-email: cecivieira@gmail.com
 License: MIT
 Keywords: jinja2,yaml,templates
 Platform: UNKNOWN
@@ -16,24 +16,24 @@
 Gerador de posts baseado em templates e dados armazenados em arquivo csv.
 
 Essa aplicação surgiu da necessidade de gerar textos a partir de um template, cujos dados deveriam ser coletados de um arquivo .csv e .yaml. Então, é isso que esse programa faz: ler dados de um arquivo .csv, outros dados de um arquivo .yaml e preenche um ou mais templates.
 
 ## Instalação
 
 ```bash
-(.venv) $ pip install gerador_posts
+(.venv) $ pip install gerador-posts
 ```
 
 ## Uso
 
 1. Crie os dados:
     1. Crie a pasta `./dados`;
     1. Dentro dessa pasta, crie dois arquivos de dados: `links.csv` e `variaveis.yaml` (os arquivos devem ter exatamente esses títulos).
 1. Crie os templates:
     1. Crie a pasta `./posts_templates`;
     1. Dentro dessa pasta você pode criar quantos templates desejar, em qualquer formato de arquivo. (para inserir dados no template use a sintaxe do Jinja2).
 1. Crie a pasta aonde os posts prontos serão armazenados: `./posts_prontos`;
 1. Execute o pacote:
     ```bash
-    (.venv) $ pip install gerador_posts
+    (.venv) $ gerar-posts
     ```
```

### Comparing `gerador_posts-0.0.1/setup.py` & `gerador_posts-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,11 +17,16 @@
     ],
     keywords=['jinja2', 'yaml', 'templates'],
     license='MIT',
     long_description_content_type='text/markdown',
     long_description=long_description,
     name='gerador_posts',
     packages=find_packages(),
+    entry_points={
+        'console_scripts': [
+            'gerar-posts = gerador_posts.gerador_posts:GeradorPosts',
+        ]
+    },
     url=REPO_URL,
     python_requires='>=3.10.6',
-    version='0.0.1',
+    version='0.1.0',
 )
```

