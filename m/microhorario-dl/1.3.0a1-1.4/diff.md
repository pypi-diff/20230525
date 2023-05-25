# Comparing `tmp/microhorario-dl-1.3.0a1.tar.gz` & `tmp/microhorario-dl-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microhorario-dl-1.3.0a1.tar", last modified: Wed Apr 20 20:18:01 2022, max compression
+gzip compressed data, was "microhorario-dl-1.4.tar", last modified: Thu May 25 10:39:31 2023, max compression
```

## Comparing `microhorario-dl-1.3.0a1.tar` & `microhorario-dl-1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-04-20 20:18:01.315844 microhorario-dl-1.3.0a1/
--rw-rw-rw-   0        0        0     1095 2022-04-06 01:30:21.000000 microhorario-dl-1.3.0a1/LICENSE
--rw-rw-rw-   0        0        0     4005 2022-04-20 20:18:01.314846 microhorario-dl-1.3.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     3283 2022-04-07 14:36:08.000000 microhorario-dl-1.3.0a1/README.md
--rw-rw-rw-   0        0        0       86 2022-04-06 01:26:50.000000 microhorario-dl-1.3.0a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-20 20:18:01.315844 microhorario-dl-1.3.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1125 2022-04-20 20:15:56.000000 microhorario-dl-1.3.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-20 20:18:01.263847 microhorario-dl-1.3.0a1/src/
-drwxrwxrwx   0        0        0        0 2022-04-20 20:18:01.282847 microhorario-dl-1.3.0a1/src/microhorario_dl/
--rw-rw-rw-   0        0        0     8358 2022-04-20 20:15:11.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/__init__.py
--rw-rw-rw-   0        0        0     7088 2022-04-06 00:48:31.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/consultas.py
--rw-rw-rw-   0        0        0     1471 2022-04-06 14:17:59.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/ementa.py
--rw-rw-rw-   0        0        0     1724 2022-04-05 14:54:10.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/exceptions.py
--rw-rw-rw-   0        0        0     8692 2022-04-07 14:51:34.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/models.py
--rw-rw-rw-   0        0        0     3849 2022-04-05 22:47:54.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/parser.py
--rw-rw-rw-   0        0        0     1044 2022-04-05 14:54:11.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/payloads.py
--rw-rw-rw-   0        0        0      636 2022-04-05 19:17:26.000000 microhorario-dl-1.3.0a1/src/microhorario_dl/utils.py
-drwxrwxrwx   0        0        0        0 2022-04-20 20:18:01.312848 microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/
--rw-rw-rw-   0        0        0     4005 2022-04-20 20:18:00.000000 microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2022-04-20 20:18:01.000000 microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-20 20:18:00.000000 microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-04-20 20:18:01.000000 microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-04-20 20:18:01.000000 microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/top_level.txt
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1074 2023-05-25 10:21:46.000000 microhorario-dl-1.4/LICENSE
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3840 2023-05-25 10:39:31.843625 microhorario-dl-1.4/PKG-INFO
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3179 2023-05-25 10:21:46.000000 microhorario-dl-1.4/README.md
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       84 2023-05-25 10:21:46.000000 microhorario-dl-1.4/pyproject.toml
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       38 2023-05-25 10:39:31.843625 microhorario-dl-1.4/setup.cfg
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1087 2023-05-25 10:37:24.000000 microhorario-dl-1.4/setup.py
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/src/
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/src/microhorario_dl/
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     8114 2023-05-25 10:37:24.000000 microhorario-dl-1.4/src/microhorario_dl/__init__.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     6882 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/consultas.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1419 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/ementa.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1660 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/exceptions.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     8357 2023-05-25 10:31:47.000000 microhorario-dl-1.4/src/microhorario_dl/models.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3833 2023-05-25 10:34:26.000000 microhorario-dl-1.4/src/microhorario_dl/parser.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1004 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/payloads.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)      615 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/utils.py
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/src/microhorario_dl.egg-info/
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3840 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/PKG-INFO
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)      505 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/SOURCES.txt
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)        1 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/dependency_links.txt
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       30 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/requires.txt
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       16 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/top_level.txt
```

### Comparing `microhorario-dl-1.3.0a1/LICENSE` & `microhorario-dl-1.4/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Daniel Guimarães
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Daniel Guimarães
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `microhorario-dl-1.3.0a1/PKG-INFO` & `microhorario-dl-1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,122 @@
-Metadata-Version: 2.1
-Name: microhorario-dl
-Version: 1.3.0a1
-Summary: PUC-Rio Microhorario Downloader
-Home-page: https://github.com/Leinadium/microhorario-dl
-Author: Daniel Guimarães <github@Leinadium>
-Author-email: daniel.sch.guima@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/Leinadium/microhorario-dl/issues
-Project-URL: Source, https://github.com/Leinadium/microhorario-dl/
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Microhorario Downloader
-
-Biblioteca destinada ao download e utilização de dados provenientes do [Microhorario](https://www.puc-rio.br/microhorario)
- da PUC-Rio.
-
-Essa biblioteca permite baixar todos os dados, e disponibiliza modelos para a utilização destes.
-
-A biblioteca não tem poder de alterar nenhum dado, somente baixar os dados e manipular localmente.
-
-
-Além disso, é possível baixar as ementas automaticamente de todas as disciplinas disponíveis.
-
-
-## Funcionamento
-
-O microhorário não disponibiliza nenhuma API para poder fazer um download automático das disciplinas. Por isso, 
-é necessário fazer requests específicos para conseguir simular um usuário baixando os dados.
-
-Para baixar os dados, um usuário precisa carregar a página inicial, fazer uma consulta sem nenhum filtro, e depois
-baixar os dados no formato CSV. Essa biblioteca simula essas três simulações atráves de um GET e dois POSTS.
-
-Para poder baixar o CSV, é preciso fazer um POST enviando os dados do formulário, assim como variáveis de ASP.NET. Essas
-variáveis são adquiridas ao fazer uma consulta sem filtro, por isso é necessário fazer um POST usando os dados do formulário
-para fazer essa consulta. Porém, essa consulta também utiliza variáveis de ASP.NET e um id de sessão adquiridos ao entrar
-na página. Por isso, é necessário fazer um GET na página inicial para poder adquirir essas variáveis e esse id.
-
-Portanto, são feitos três requests, nomeados `consulta_inicial`, `consulta_intermediaria`, e `consulta_final`:
-
-```text
-consulta inicial (GET https://puc-rio.br/microhorario):
-    recebe:
-        cookies
-        id da sessao
-        nomes e códigos dos departamentos
-        nomes e códigos dos destinos
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-consulta intermediaria (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
-    envia:
-        formulario pedindo uma consulta sem filtro
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-    recebe:
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-consulta final (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
-    envia:
-        formulario pedindo para baixar os resultados de uma consulta sem filtro
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-    recebe:
-        arquivo csv em utf-16
-```
-
-## Uso
-
-Instale a biblioteca: 
-```shell
-pip install microhorario-dl
-```
-
-Importe e baixe os dados:
-
-```pycon
->>> from microhorario_dl import Microhorario
-
->>> micro = Microhorario.download()
-<Microhorario object at ...>
-
->>> micro.disciplinas
-[<Disciplina [ACN1000]>, <Disciplina[ACN1002]>, ...]
-```
-
-Baixe as ementas:
-
-```pycon
->>> micro.coletar_ementas(verbose=True)
-[0/ 2000] Baixando ACN1000...  DONE (...)
-[1/ 2000] Baixando ACN1002...  DONE (...)
-[2/ 2000] Baixando ACN1004...
-... 
-```
-
-
-Exporte para um json:
-
-```pycon
->>> import json
-
->>> print(json.dumps(micro.as_json(), indent=2))
-{
-    "periodo": "20221",
-    "emissao": "05/04/2022 22:57 h",
-    # ...
-    "disciplinas": [
-        # ...
-    ]
-}
-```
-
+Metadata-Version: 2.1
+Name: microhorario-dl
+Version: 1.4
+Summary: PUC-Rio Microhorario Downloader
+Home-page: https://github.com/Leinadium/microhorario-dl
+Author: Daniel Guimarães <github@Leinadium>
+Author-email: daniel.sch.guima@gmail.com
+Project-URL: Bug Reports, https://github.com/Leinadium/microhorario-dl/issues
+Project-URL: Source, https://github.com/Leinadium/microhorario-dl/
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Microhorario Downloader
+
+Biblioteca destinada ao download e utilização de dados provenientes do [Microhorario](https://www.puc-rio.br/microhorario)
+ da PUC-Rio.
+
+Essa biblioteca permite baixar todos os dados, e disponibiliza modelos para a utilização destes.
+
+A biblioteca não tem poder de alterar nenhum dado, somente baixar os dados e manipular localmente.
+
+
+Além disso, é possível baixar as ementas automaticamente de todas as disciplinas disponíveis.
+
+
+## Funcionamento
+
+O microhorário não disponibiliza nenhuma API para poder fazer um download automático das disciplinas. Por isso, 
+é necessário fazer requests específicos para conseguir simular um usuário baixando os dados.
+
+Para baixar os dados, um usuário precisa carregar a página inicial, fazer uma consulta sem nenhum filtro, e depois
+baixar os dados no formato CSV. Essa biblioteca simula essas três simulações atráves de um GET e dois POSTS.
+
+Para poder baixar o CSV, é preciso fazer um POST enviando os dados do formulário, assim como variáveis de ASP.NET. Essas
+variáveis são adquiridas ao fazer uma consulta sem filtro, por isso é necessário fazer um POST usando os dados do formulário
+para fazer essa consulta. Porém, essa consulta também utiliza variáveis de ASP.NET e um id de sessão adquiridos ao entrar
+na página. Por isso, é necessário fazer um GET na página inicial para poder adquirir essas variáveis e esse id.
+
+Portanto, são feitos três requests, nomeados `consulta_inicial`, `consulta_intermediaria`, e `consulta_final`:
+
+```text
+consulta inicial (GET https://puc-rio.br/microhorario):
+    recebe:
+        cookies
+        id da sessao
+        nomes e códigos dos departamentos
+        nomes e códigos dos destinos
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+consulta intermediaria (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
+    envia:
+        formulario pedindo uma consulta sem filtro
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+    recebe:
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+consulta final (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
+    envia:
+        formulario pedindo para baixar os resultados de uma consulta sem filtro
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+    recebe:
+        arquivo csv em utf-16
+```
+
+## Uso
+
+Instale a biblioteca: 
+```shell
+pip install microhorario-dl
+```
+
+Importe e baixe os dados:
+
+```pycon
+>>> from microhorario_dl import Microhorario
+
+>>> micro = Microhorario.download()
+<Microhorario object at ...>
+
+>>> micro.disciplinas
+[<Disciplina [ACN1000]>, <Disciplina[ACN1002]>, ...]
+```
+
+Baixe as ementas:
+
+```pycon
+>>> micro.coletar_ementas(verbose=True)
+[0/ 2000] Baixando ACN1000...  DONE (...)
+[1/ 2000] Baixando ACN1002...  DONE (...)
+[2/ 2000] Baixando ACN1004...
+... 
+```
+
+
+Exporte para um json:
+
+```pycon
+>>> import json
+
+>>> print(json.dumps(micro.as_json(), indent=2))
+{
+    "periodo": "20221",
+    "emissao": "05/04/2022 22:57 h",
+    # ...
+    "disciplinas": [
+        # ...
+    ]
+}
+```
```

### Comparing `microhorario-dl-1.3.0a1/README.md` & `microhorario-dl-1.4/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-# Microhorario Downloader
-
-Biblioteca destinada ao download e utilização de dados provenientes do [Microhorario](https://www.puc-rio.br/microhorario)
- da PUC-Rio.
-
-Essa biblioteca permite baixar todos os dados, e disponibiliza modelos para a utilização destes.
-
-A biblioteca não tem poder de alterar nenhum dado, somente baixar os dados e manipular localmente.
-
-
-Além disso, é possível baixar as ementas automaticamente de todas as disciplinas disponíveis.
-
-
-## Funcionamento
-
-O microhorário não disponibiliza nenhuma API para poder fazer um download automático das disciplinas. Por isso, 
-é necessário fazer requests específicos para conseguir simular um usuário baixando os dados.
-
-Para baixar os dados, um usuário precisa carregar a página inicial, fazer uma consulta sem nenhum filtro, e depois
-baixar os dados no formato CSV. Essa biblioteca simula essas três simulações atráves de um GET e dois POSTS.
-
-Para poder baixar o CSV, é preciso fazer um POST enviando os dados do formulário, assim como variáveis de ASP.NET. Essas
-variáveis são adquiridas ao fazer uma consulta sem filtro, por isso é necessário fazer um POST usando os dados do formulário
-para fazer essa consulta. Porém, essa consulta também utiliza variáveis de ASP.NET e um id de sessão adquiridos ao entrar
-na página. Por isso, é necessário fazer um GET na página inicial para poder adquirir essas variáveis e esse id.
-
-Portanto, são feitos três requests, nomeados `consulta_inicial`, `consulta_intermediaria`, e `consulta_final`:
-
-```text
-consulta inicial (GET https://puc-rio.br/microhorario):
-    recebe:
-        cookies
-        id da sessao
-        nomes e códigos dos departamentos
-        nomes e códigos dos destinos
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-consulta intermediaria (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
-    envia:
-        formulario pedindo uma consulta sem filtro
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-    recebe:
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-consulta final (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
-    envia:
-        formulario pedindo para baixar os resultados de uma consulta sem filtro
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-    recebe:
-        arquivo csv em utf-16
-```
-
-## Uso
-
-Instale a biblioteca: 
-```shell
-pip install microhorario-dl
-```
-
-Importe e baixe os dados:
-
-```pycon
->>> from microhorario_dl import Microhorario
-
->>> micro = Microhorario.download()
-<Microhorario object at ...>
-
->>> micro.disciplinas
-[<Disciplina [ACN1000]>, <Disciplina[ACN1002]>, ...]
-```
-
-Baixe as ementas:
-
-```pycon
->>> micro.coletar_ementas(verbose=True)
-[0/ 2000] Baixando ACN1000...  DONE (...)
-[1/ 2000] Baixando ACN1002...  DONE (...)
-[2/ 2000] Baixando ACN1004...
-... 
-```
-
-
-Exporte para um json:
-
-```pycon
->>> import json
-
->>> print(json.dumps(micro.as_json(), indent=2))
-{
-    "periodo": "20221",
-    "emissao": "05/04/2022 22:57 h",
-    # ...
-    "disciplinas": [
-        # ...
-    ]
-}
+# Microhorario Downloader
+
+Biblioteca destinada ao download e utilização de dados provenientes do [Microhorario](https://www.puc-rio.br/microhorario)
+ da PUC-Rio.
+
+Essa biblioteca permite baixar todos os dados, e disponibiliza modelos para a utilização destes.
+
+A biblioteca não tem poder de alterar nenhum dado, somente baixar os dados e manipular localmente.
+
+
+Além disso, é possível baixar as ementas automaticamente de todas as disciplinas disponíveis.
+
+
+## Funcionamento
+
+O microhorário não disponibiliza nenhuma API para poder fazer um download automático das disciplinas. Por isso, 
+é necessário fazer requests específicos para conseguir simular um usuário baixando os dados.
+
+Para baixar os dados, um usuário precisa carregar a página inicial, fazer uma consulta sem nenhum filtro, e depois
+baixar os dados no formato CSV. Essa biblioteca simula essas três simulações atráves de um GET e dois POSTS.
+
+Para poder baixar o CSV, é preciso fazer um POST enviando os dados do formulário, assim como variáveis de ASP.NET. Essas
+variáveis são adquiridas ao fazer uma consulta sem filtro, por isso é necessário fazer um POST usando os dados do formulário
+para fazer essa consulta. Porém, essa consulta também utiliza variáveis de ASP.NET e um id de sessão adquiridos ao entrar
+na página. Por isso, é necessário fazer um GET na página inicial para poder adquirir essas variáveis e esse id.
+
+Portanto, são feitos três requests, nomeados `consulta_inicial`, `consulta_intermediaria`, e `consulta_final`:
+
+```text
+consulta inicial (GET https://puc-rio.br/microhorario):
+    recebe:
+        cookies
+        id da sessao
+        nomes e códigos dos departamentos
+        nomes e códigos dos destinos
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+consulta intermediaria (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
+    envia:
+        formulario pedindo uma consulta sem filtro
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+    recebe:
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+consulta final (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
+    envia:
+        formulario pedindo para baixar os resultados de uma consulta sem filtro
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+    recebe:
+        arquivo csv em utf-16
+```
+
+## Uso
+
+Instale a biblioteca: 
+```shell
+pip install microhorario-dl
+```
+
+Importe e baixe os dados:
+
+```pycon
+>>> from microhorario_dl import Microhorario
+
+>>> micro = Microhorario.download()
+<Microhorario object at ...>
+
+>>> micro.disciplinas
+[<Disciplina [ACN1000]>, <Disciplina[ACN1002]>, ...]
+```
+
+Baixe as ementas:
+
+```pycon
+>>> micro.coletar_ementas(verbose=True)
+[0/ 2000] Baixando ACN1000...  DONE (...)
+[1/ 2000] Baixando ACN1002...  DONE (...)
+[2/ 2000] Baixando ACN1004...
+... 
+```
+
+
+Exporte para um json:
+
+```pycon
+>>> import json
+
+>>> print(json.dumps(micro.as_json(), indent=2))
+{
+    "periodo": "20221",
+    "emissao": "05/04/2022 22:57 h",
+    # ...
+    "disciplinas": [
+        # ...
+    ]
+}
 ```
```

### Comparing `microhorario-dl-1.3.0a1/setup.py` & `microhorario-dl-1.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-long_description = (here / "README.md").read_text(encoding='utf-8')
-
-setup(
-    name='microhorario-dl',
-    version='1.3.0a1',
-    description='PUC-Rio Microhorario Downloader',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/Leinadium/microhorario-dl',
-    author='Daniel Guimarães <github@Leinadium>',
-    author_email='daniel.sch.guima@gmail.com',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
-    install_requires=[
-        "beautifulsoup4>=4",
-        "requests>=2"
-    ],
-    python_requires=">3.7",
-    project_urls={
-        "Bug Reports": "https://github.com/Leinadium/microhorario-dl/issues",
-        "Source": "https://github.com/Leinadium/microhorario-dl/"
-    }
-)
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+
+long_description = (here / "README.md").read_text(encoding='utf-8')
+
+setup(
+    name='microhorario-dl',
+    version='1.4',
+    description='PUC-Rio Microhorario Downloader',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/Leinadium/microhorario-dl',
+    author='Daniel Guimarães <github@Leinadium>',
+    author_email='daniel.sch.guima@gmail.com',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    install_requires=[
+        "beautifulsoup4>=4",
+        "requests>=2"
+    ],
+    python_requires=">3.7",
+    project_urls={
+        "Bug Reports": "https://github.com/Leinadium/microhorario-dl/issues",
+        "Source": "https://github.com/Leinadium/microhorario-dl/"
+    }
+)
```

### Comparing `microhorario-dl-1.3.0a1/src/microhorario_dl/consultas.py` & `microhorario-dl-1.4/src/microhorario_dl/consultas.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-import re
-import requests
-from bs4 import BeautifulSoup
-
-# typing modules
-from typing import Dict, Any, Optional, Match, Union
-from bs4.element import Tag
-
-# local modules
-from .payloads import PAYLOAD_FINAL, PAYLOAD_INTERMEDIARIO
-from .utils import URL_CONSULTA, URL_INICIAL, USER_AGENT, pegar_sessao_da_url
-from .exceptions import EmptyTagValueError, TagNotFoundError, NotCSVError, PatternNotFoundError
-
-
-def de_opcoes_para_dicionario(t: Tag) -> Dict[str, str]:
-    """Converte todas as opções dentro de uma tag de seleção em um dicionario.
-
-    Em vez de pegar o `value` da opção como chave, é feito um regex na string.
-    """
-    ret: Dict[str, str] = {}
-    for x in t.find_all('option'):       # type: Tag
-        m: Match = re.search(r'(?P<ident>[A-Z]{3})\s-\s(?P<nome>[\w\s]+)', x.text)
-        if m is not None:
-            ident = m.group('ident')
-            nome = m.group('nome')
-            if (ident is not None) and (nome is not None):
-                ret[ident] = nome
-    return ret
-
-
-def consulta_inicial() -> Dict[str, Any]:
-    """
-    Faz a primeira consulta no site do microhorario
-
-    A primeira consulta é responsável por coletar os cookies necessários,
-    as variáveis para o ASP.NET, a sessão do usuário,
-    e também o nome dos departamentos e destinos.
-
-    :return: dicionario contendo os cookies e os dados necessários
-    """
-
-    def valida_tag_ou_aborta(nome: str, t: Optional[Tag]) -> str:
-        """
-        Valida se a Tag foi coletada ou não.
-        Se for None, aborta o programa com uma mensagem especifica
-
-        :param nome: nome da tag
-        :param t: tag ou None
-        :return: a string `value` dentro da tag
-        """
-        if t is None:
-            raise TagNotFoundError(nome)
-        else:
-            if isinstance(t, Tag):
-                valor = t.get('value')
-                if valor is None:
-                    raise EmptyTagValueError(nome)
-                else:
-                    return valor
-
-    r = requests.get(
-        url=URL_INICIAL,
-        headers={"User-Agent": USER_AGENT}
-    )
-
-    # pegando os cookies (juntando com os redirects)
-    cookies: dict = r.cookies.get_dict()
-    for r_history in r.history:
-        cookies.update(r_history.cookies.get_dict())
-
-    # pegando propriedades do ASP.NET
-    soup = BeautifulSoup(r.text, features='html.parser')
-    view_state_generator: Tag = soup.find(id='__VIEWSTATEGENERATOR')
-    event_validation: Tag = soup.find(id='__EVENTVALIDATION')
-    view_state: Tag = soup.find(id='__VIEWSTATE')
-
-    # pegando destinos
-    destinos_tag: Tag = soup.find(id='ddlBloqueio', recursive=True)
-    destinos = de_opcoes_para_dicionario(destinos_tag) if destinos_tag is not None else {}
-
-    # pegando departamentos
-    departamentos_tag: Tag = soup.find(id='ddlDeptoSolicitante', recursive=True)
-    departamentos = de_opcoes_para_dicionario(departamentos_tag) if departamentos_tag is not None else {}
-
-    # pegando a sessao
-    sessao = pegar_sessao_da_url(r.url)
-
-    return {
-        'cookies': cookies,
-        'sessao': sessao,
-        'departamentos': departamentos,
-        'destinos': destinos,
-        'dados': {
-            '__VIEWSTATEGENERATOR': valida_tag_ou_aborta(
-                nome='__VIEWSTATEGENERATOR',
-                t=view_state_generator
-            ),
-            '__EVENTVALIDATION': valida_tag_ou_aborta(
-                nome='__EVENTVALIDATION',
-                t=event_validation
-            ),
-            '__VIEWSTATE': valida_tag_ou_aborta(
-                nome='__VIEWSTATE',
-                t=view_state
-            )
-        }
-    }
-
-
-def consulta_intermediaria(dados_iniciais: Dict[str, Any]):
-    """
-    Usando os dados iniciais da primeira consulta, é realiada um segunda consulta simulando
-    uma pesquisa sem filtro, para atualizar as variáveis do ASP.NET necessárias para fazer
-    a consulta final.
-
-    Ao contrário da primeira consulta, essa retorna um texto que o javascript do framework do ASP.NET deveria
-    utilizar. Por isso, para atualizar as variáveis, são utilizados regex
-
-    :param dados_iniciais: dicionario retornada pela `consulta_inicial`
-    :return: dicionario com os novos dados da consulta
-    """
-    def regex_ou_aborta(nome: str, pattern: str, string: str) -> str:
-        m: Match = re.search(pattern, string)
-        if m is None:
-            raise PatternNotFoundError(nome=nome, regex=pattern)
-        return m.group(1)
-
-    payload: dict = PAYLOAD_INTERMEDIARIO
-    payload.update(dados_iniciais['dados'])     # adiciona as variaveis coletadas no dados iniciais
-
-    cookies = dados_iniciais.get('cookies')
-    sessao = dados_iniciais.get('sessao')
-
-    r = requests.post(
-        url=URL_CONSULTA,
-        cookies=cookies,
-        params={'sessao': sessao},
-        headers={
-            'User-Agent': USER_AGENT,
-            'Accept': 'text/plain',
-            'Content-Type': 'application/x-www-form-urlencoded'
-        },
-        data=payload
-    )
-
-    # pegando as novas informacoes
-    return {
-        'cookies': cookies,
-        'sessao': sessao,
-        'dados': {
-            '__VIEWSTATEGENERATOR': regex_ou_aborta(
-                nome='',
-                pattern=r'__VIEWSTATEGENERATOR\|([0-9a-zA-Z+\/=]+)\|',
-                string=r.text
-            ),
-            '__EVENTVALIDATION': regex_ou_aborta(
-                nome='EVENTVALIDATION',
-                pattern=r'__EVENTVALIDATION\|([0-9a-zA-Z+\/=]+)\|',
-                string=r.text
-            ),
-            '__VIEWSTATE': regex_ou_aborta(
-                nome='VIEWSTATE',
-                pattern=r'__VIEWSTATE\|([0-9a-zA-Z+\/=]+)\|',
-                string=r.text
-            )
-        }
-    }
-
-
-def consulta_final(dados_intermediarios: Dict[str, Union[Tag, str]]) -> str:
-    """
-    Faz a consulta final, para obter o CSV com todas as disciplinas no microhorario.
-
-    Usando as variáveis de ASP.NET fornecidas na consulta intermediaria, é feito um POST
-    pedindo o CSV referente àquela consulta.
-
-    :param dados_intermediarios: dados da consulta intermediaria
-
-    :return: o texto do csv baixado
-    """
-    # preparando os dados
-    payload: dict = PAYLOAD_FINAL
-    payload.update(dados_intermediarios.get('dados'))     # adiciona as variaveis coletadas no dados iniciais
-
-    cookies = dados_intermediarios.get('cookies')
-    sessao = dados_intermediarios.get('sessao')
-
-    # preparando a consulta
-    r = requests.post(
-        url=URL_CONSULTA,
-        cookies=cookies,
-        headers={
-            'User-Agent': USER_AGENT,
-            'Accept': 'text/csv',
-            'Content-Type': 'application/x-www-form-urlencoded'
-        },
-        params={'sessao': sessao},
-        data=payload
-    )
-
-    if 'text/csv' not in r.headers.get('Content-Type'):
-        raise NotCSVError
-
-    # pega o texto usando o encoding correto
-    r.encoding = 'utf-16'
-    return r.text
+import re
+import requests
+from bs4 import BeautifulSoup
+
+# typing modules
+from typing import Dict, Any, Optional, Match, Union
+from bs4.element import Tag
+
+# local modules
+from .payloads import PAYLOAD_FINAL, PAYLOAD_INTERMEDIARIO
+from .utils import URL_CONSULTA, URL_INICIAL, USER_AGENT, pegar_sessao_da_url
+from .exceptions import EmptyTagValueError, TagNotFoundError, NotCSVError, PatternNotFoundError
+
+
+def de_opcoes_para_dicionario(t: Tag) -> Dict[str, str]:
+    """Converte todas as opções dentro de uma tag de seleção em um dicionario.
+
+    Em vez de pegar o `value` da opção como chave, é feito um regex na string.
+    """
+    ret: Dict[str, str] = {}
+    for x in t.find_all('option'):       # type: Tag
+        m: Match = re.search(r'(?P<ident>[A-Z]{3})\s-\s(?P<nome>[\w\s]+)', x.text)
+        if m is not None:
+            ident = m.group('ident')
+            nome = m.group('nome')
+            if (ident is not None) and (nome is not None):
+                ret[ident] = nome
+    return ret
+
+
+def consulta_inicial() -> Dict[str, Any]:
+    """
+    Faz a primeira consulta no site do microhorario
+
+    A primeira consulta é responsável por coletar os cookies necessários,
+    as variáveis para o ASP.NET, a sessão do usuário,
+    e também o nome dos departamentos e destinos.
+
+    :return: dicionario contendo os cookies e os dados necessários
+    """
+
+    def valida_tag_ou_aborta(nome: str, t: Optional[Tag]) -> str:
+        """
+        Valida se a Tag foi coletada ou não.
+        Se for None, aborta o programa com uma mensagem especifica
+
+        :param nome: nome da tag
+        :param t: tag ou None
+        :return: a string `value` dentro da tag
+        """
+        if t is None:
+            raise TagNotFoundError(nome)
+        else:
+            if isinstance(t, Tag):
+                valor = t.get('value')
+                if valor is None:
+                    raise EmptyTagValueError(nome)
+                else:
+                    return valor
+
+    r = requests.get(
+        url=URL_INICIAL,
+        headers={"User-Agent": USER_AGENT}
+    )
+
+    # pegando os cookies (juntando com os redirects)
+    cookies: dict = r.cookies.get_dict()
+    for r_history in r.history:
+        cookies.update(r_history.cookies.get_dict())
+
+    # pegando propriedades do ASP.NET
+    soup = BeautifulSoup(r.text, features='html.parser')
+    view_state_generator: Tag = soup.find(id='__VIEWSTATEGENERATOR')
+    event_validation: Tag = soup.find(id='__EVENTVALIDATION')
+    view_state: Tag = soup.find(id='__VIEWSTATE')
+
+    # pegando destinos
+    destinos_tag: Tag = soup.find(id='ddlBloqueio', recursive=True)
+    destinos = de_opcoes_para_dicionario(destinos_tag) if destinos_tag is not None else {}
+
+    # pegando departamentos
+    departamentos_tag: Tag = soup.find(id='ddlDeptoSolicitante', recursive=True)
+    departamentos = de_opcoes_para_dicionario(departamentos_tag) if departamentos_tag is not None else {}
+
+    # pegando a sessao
+    sessao = pegar_sessao_da_url(r.url)
+
+    return {
+        'cookies': cookies,
+        'sessao': sessao,
+        'departamentos': departamentos,
+        'destinos': destinos,
+        'dados': {
+            '__VIEWSTATEGENERATOR': valida_tag_ou_aborta(
+                nome='__VIEWSTATEGENERATOR',
+                t=view_state_generator
+            ),
+            '__EVENTVALIDATION': valida_tag_ou_aborta(
+                nome='__EVENTVALIDATION',
+                t=event_validation
+            ),
+            '__VIEWSTATE': valida_tag_ou_aborta(
+                nome='__VIEWSTATE',
+                t=view_state
+            )
+        }
+    }
+
+
+def consulta_intermediaria(dados_iniciais: Dict[str, Any]):
+    """
+    Usando os dados iniciais da primeira consulta, é realiada um segunda consulta simulando
+    uma pesquisa sem filtro, para atualizar as variáveis do ASP.NET necessárias para fazer
+    a consulta final.
+
+    Ao contrário da primeira consulta, essa retorna um texto que o javascript do framework do ASP.NET deveria
+    utilizar. Por isso, para atualizar as variáveis, são utilizados regex
+
+    :param dados_iniciais: dicionario retornada pela `consulta_inicial`
+    :return: dicionario com os novos dados da consulta
+    """
+    def regex_ou_aborta(nome: str, pattern: str, string: str) -> str:
+        m: Match = re.search(pattern, string)
+        if m is None:
+            raise PatternNotFoundError(nome=nome, regex=pattern)
+        return m.group(1)
+
+    payload: dict = PAYLOAD_INTERMEDIARIO
+    payload.update(dados_iniciais['dados'])     # adiciona as variaveis coletadas no dados iniciais
+
+    cookies = dados_iniciais.get('cookies')
+    sessao = dados_iniciais.get('sessao')
+
+    r = requests.post(
+        url=URL_CONSULTA,
+        cookies=cookies,
+        params={'sessao': sessao},
+        headers={
+            'User-Agent': USER_AGENT,
+            'Accept': 'text/plain',
+            'Content-Type': 'application/x-www-form-urlencoded'
+        },
+        data=payload
+    )
+
+    # pegando as novas informacoes
+    return {
+        'cookies': cookies,
+        'sessao': sessao,
+        'dados': {
+            '__VIEWSTATEGENERATOR': regex_ou_aborta(
+                nome='',
+                pattern=r'__VIEWSTATEGENERATOR\|([0-9a-zA-Z+\/=]+)\|',
+                string=r.text
+            ),
+            '__EVENTVALIDATION': regex_ou_aborta(
+                nome='EVENTVALIDATION',
+                pattern=r'__EVENTVALIDATION\|([0-9a-zA-Z+\/=]+)\|',
+                string=r.text
+            ),
+            '__VIEWSTATE': regex_ou_aborta(
+                nome='VIEWSTATE',
+                pattern=r'__VIEWSTATE\|([0-9a-zA-Z+\/=]+)\|',
+                string=r.text
+            )
+        }
+    }
+
+
+def consulta_final(dados_intermediarios: Dict[str, Union[Tag, str]]) -> str:
+    """
+    Faz a consulta final, para obter o CSV com todas as disciplinas no microhorario.
+
+    Usando as variáveis de ASP.NET fornecidas na consulta intermediaria, é feito um POST
+    pedindo o CSV referente àquela consulta.
+
+    :param dados_intermediarios: dados da consulta intermediaria
+
+    :return: o texto do csv baixado
+    """
+    # preparando os dados
+    payload: dict = PAYLOAD_FINAL
+    payload.update(dados_intermediarios.get('dados'))     # adiciona as variaveis coletadas no dados iniciais
+
+    cookies = dados_intermediarios.get('cookies')
+    sessao = dados_intermediarios.get('sessao')
+
+    # preparando a consulta
+    r = requests.post(
+        url=URL_CONSULTA,
+        cookies=cookies,
+        headers={
+            'User-Agent': USER_AGENT,
+            'Accept': 'text/csv',
+            'Content-Type': 'application/x-www-form-urlencoded'
+        },
+        params={'sessao': sessao},
+        data=payload
+    )
+
+    if 'text/csv' not in r.headers.get('Content-Type'):
+        raise NotCSVError
+
+    # pega o texto usando o encoding correto
+    r.encoding = 'utf-16'
+    return r.text
```

### Comparing `microhorario-dl-1.3.0a1/src/microhorario_dl/ementa.py` & `microhorario-dl-1.4/src/microhorario_dl/ementa.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import requests
-import warnings
-from bs4 import BeautifulSoup
-
-# typing
-from typing import Optional
-from bs4.element import Tag
-
-
-URL_EMENTA = "https://www.puc-rio.br/ferramentas/ementas/ementa.aspx?cd={codigo}"
-
-
-def encontra_ementa(html: str) -> Optional[str]:
-    """
-    Faz o parsing do html, procurando o texto da ementa.
-
-    Retorna o texto da ementa se encontrar, ou None
-
-    :param html: string contendo o html da página da ementa
-
-    :return:
-    """
-
-    soup = BeautifulSoup(html, features='html.parser')
-
-    tag_ementa: Tag = soup.find(id='pEmenta', recursive=True)
-
-    return tag_ementa.text if tag_ementa is not None else None
-
-
-def consulta_ementa(codigo: str) -> str:
-    """
-    Faz uma consulta para a página da ementa, e retorna a ementa.
-
-    Há um sleep de 0.3 segundos para evitar muitas consultas em pouco tempo ao site.
-
-    Se não encontrar ou houver algum erro, a ementa será "Disciplina sem ementa cadastrada."
-
-    :param codigo: código da disciplina no formato XXX0000
-
-    :return: o texto da ementa
-    """
-
-    ementa_erro = "Disciplina sem ementa cadastrada"
-
-    r = requests.get(URL_EMENTA.format(codigo=codigo))
-    if r.status_code != 200:
-        warnings.warn(f"Consulta da ementa da disciplina {codigo} retornou codigo {r.status_code}")
-        return ementa_erro
-
-    ementa = encontra_ementa(r.text)
-    return ementa.strip() if ementa is not None else ementa_erro
+import requests
+import warnings
+from bs4 import BeautifulSoup
+
+# typing
+from typing import Optional
+from bs4.element import Tag
+
+
+URL_EMENTA = "https://www.puc-rio.br/ferramentas/ementas/ementa.aspx?cd={codigo}"
+
+
+def encontra_ementa(html: str) -> Optional[str]:
+    """
+    Faz o parsing do html, procurando o texto da ementa.
+
+    Retorna o texto da ementa se encontrar, ou None
+
+    :param html: string contendo o html da página da ementa
+
+    :return:
+    """
+
+    soup = BeautifulSoup(html, features='html.parser')
+
+    tag_ementa: Tag = soup.find(id='pEmenta', recursive=True)
+
+    return tag_ementa.text if tag_ementa is not None else None
+
+
+def consulta_ementa(codigo: str) -> str:
+    """
+    Faz uma consulta para a página da ementa, e retorna a ementa.
+
+    Há um sleep de 0.3 segundos para evitar muitas consultas em pouco tempo ao site.
+
+    Se não encontrar ou houver algum erro, a ementa será "Disciplina sem ementa cadastrada."
+
+    :param codigo: código da disciplina no formato XXX0000
+
+    :return: o texto da ementa
+    """
+
+    ementa_erro = "Disciplina sem ementa cadastrada"
+
+    r = requests.get(URL_EMENTA.format(codigo=codigo))
+    if r.status_code != 200:
+        warnings.warn(f"Consulta da ementa da disciplina {codigo} retornou codigo {r.status_code}")
+        return ementa_erro
+
+    ementa = encontra_ementa(r.text)
+    return ementa.strip() if ementa is not None else ementa_erro
```

### Comparing `microhorario-dl-1.3.0a1/src/microhorario_dl/exceptions.py` & `microhorario-dl-1.4/src/microhorario_dl/exceptions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-class BaseParsingError(Exception):
-    """Exception base para as exceções no HTML
-
-    Attributes:
-        mensagem -- Mensagem da exceção
-    """
-    def __init__(self, mensagem: str):
-        self.message = mensagem
-        super().__init__(self.message)
-
-
-class TagNotFoundError(BaseParsingError):
-    """Exceção levantada quando o HTML não possui a tag solicitada
-
-    Attributes:
-        tag -- Nome da tag não encontrada
-    """
-
-    def __init__(self, tag: str):
-        self.tag = tag
-        super().__init__(f'Tag {tag} não encontrada' % tag)
-
-
-class EmptyTagValueError(BaseParsingError):
-    """Excecção levantada quando a tag HTML não tem `value` configurada
-
-    Attributes:
-        tag -- Nome da tag sem `value`
-    """
-
-    def __init__(self, tag):
-        self.tag = tag
-        super().__init__(f"Tag {tag} não possui value")
-
-
-class PatternNotFoundError(BaseParsingError):
-    """Exceção levantada quando o pattern não foi encontrado
-    na resposta do servidor, impedindo de prosseguir a consulta
-
-    Attributes:
-        nome -- nome do pattern procurado
-        regex -- regex usado para buscar o pattern
-    """
-
-    def __init__(self, nome: str, regex: str):
-        self.nome = nome
-        self.regex = regex
-        super().__init__(
-            f"{nome} não foi encontrado no HTML (regex: {regex})"
-        )
-
-
-class NotCSVError(BaseParsingError):
-    """Exceção levantada quando a consulta final
-    não retornou um CSV.
-
-    Isso pode acontecer quando os
-    headers ou o payload da consulta estão incorretos.
-    """
-
-    def __init__(self):
-        super().__init__("Consulta final não retornou um CSV")
-
-
+class BaseParsingError(Exception):
+    """Exception base para as exceções no HTML
+
+    Attributes:
+        mensagem -- Mensagem da exceção
+    """
+    def __init__(self, mensagem: str):
+        self.message = mensagem
+        super().__init__(self.message)
+
+
+class TagNotFoundError(BaseParsingError):
+    """Exceção levantada quando o HTML não possui a tag solicitada
+
+    Attributes:
+        tag -- Nome da tag não encontrada
+    """
+
+    def __init__(self, tag: str):
+        self.tag = tag
+        super().__init__(f'Tag {tag} não encontrada' % tag)
+
+
+class EmptyTagValueError(BaseParsingError):
+    """Excecção levantada quando a tag HTML não tem `value` configurada
+
+    Attributes:
+        tag -- Nome da tag sem `value`
+    """
+
+    def __init__(self, tag):
+        self.tag = tag
+        super().__init__(f"Tag {tag} não possui value")
+
+
+class PatternNotFoundError(BaseParsingError):
+    """Exceção levantada quando o pattern não foi encontrado
+    na resposta do servidor, impedindo de prosseguir a consulta
+
+    Attributes:
+        nome -- nome do pattern procurado
+        regex -- regex usado para buscar o pattern
+    """
+
+    def __init__(self, nome: str, regex: str):
+        self.nome = nome
+        self.regex = regex
+        super().__init__(
+            f"{nome} não foi encontrado no HTML (regex: {regex})"
+        )
+
+
+class NotCSVError(BaseParsingError):
+    """Exceção levantada quando a consulta final
+    não retornou um CSV.
+
+    Isso pode acontecer quando os
+    headers ou o payload da consulta estão incorretos.
+    """
+
+    def __init__(self):
+        super().__init__("Consulta final não retornou um CSV")
+
+
```

### Comparing `microhorario-dl-1.3.0a1/src/microhorario_dl/parser.py` & `microhorario-dl-1.4/src/microhorario_dl/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,122 @@
-import re
-import warnings
-
-# typing stuff
-from typing import List, Dict
-
-# local imports
-from .models import RawDisciplina
-
-
-def get_informacoes_csv(info_str: str) -> Dict[str, str]:
-    """
-    Faz um parsing das informações do CSV gerado.
-
-    Procura retirar as informações da primeira linha do CSV, no formato:
-        Período: 20221;Emitido em: 05/04/2022 16:24 h; Data da última atualização: 05/04/2022 13:50h;
-
-    :param info_str: linha contendo as informações do csv
-
-    :return: um dicionario com as chaves "periodo", "emissao" e "atualizacao"
-    """
-
-    lista: List[str] = info_str.split(';')
-    res = {
-        'periodo': '',
-        'emissao': '',
-        'atualizacao': ''
-    }
-
-    for elemento in lista:
-        # separando no ":", onde [0] tem um texto, e [1] o conteudo
-        try:
-            texto_e_conteudo = elemento.split(':')
-            texto, conteudo = texto_e_conteudo[0], ':'.join(texto_e_conteudo[1:])
-            if 'Período' in texto:
-                res['periodo'] = conteudo.strip()
-            elif 'Emitido' in texto:
-                res['emissao'] = conteudo.strip()
-            elif 'atualização' in texto:
-                res['atualizacao'] = conteudo.strip()
-
-        except ValueError:
-            continue
-
-    # verificando integridade
-    for k, v in res.items():
-        if not v:
-            warnings.warn(f"A informacao '{k}' não foi encontrada no csv baixado")
-
-    return res
-
-
-def converte_para_json(texto_csv: str) -> dict:
-
-    ret: dict = {}
-    # le as linhas do csv
-    linhas = texto_csv.splitlines()
-    # salva as informacoes na linha inicial do arquivo
-    ret.update(
-        get_informacoes_csv(linhas[0])
-    )
-
-    # regex para o codigo, que é o primeiro texto na linha
-    re_disciplina = re.compile('^[A-Z]{3}[0-9]{4}')
-
-    lista_disciplinas: List[RawDisciplina] = list()
-
-    for linha in linhas:
-        if re_disciplina.match(linha) is None:
-            continue     # pula a linha que nao tem informacao
-
-        # splitando em brancos e retirando tambem o ';' final se tiver
-        linha_split = linha.strip(' \n\r;').split(';')
-        if len(linha_split) != 13:
-            warnings.warn(f"Linha iniciada em {linha_split[0]} está inválida")
-            continue     # pula a linha que a informacao esta corrompida
-
-        codigo = linha_split[0].strip()
-        nome = linha_split[1].strip()
-        professor = linha_split[2].strip()
-        creditos = linha_split[3].strip()
-        turma = linha_split[4].strip()
-        destino = linha_split[5].strip()
-        vaga = linha_split[6].strip()
-        turno = linha_split[7].strip()
-        horario_local = linha_split[8].strip()
-        horas_distancia = linha_split[9].strip()
-        shf = linha_split[10].strip()
-        pre_req = linha_split[11].strip()
-        depto = linha_split[12].strip()
-
-        # fazendo parsing dos valores numericos
-        creditos = int(creditos) if creditos.isnumeric() else -1
-        vaga = int(vaga) if vaga.isnumeric() else -1
-        horas_distancia = int(horas_distancia) if horas_distancia.isnumeric() else -1
-        shf = int(shf) if shf.isnumeric() else -1
-
-        # fazendo parsing dos valores booleanos
-        pre_req = pre_req == "SIM"
-        lista_disciplinas.append(RawDisciplina(
-            nome=nome,
-            codigo=codigo,
-            professor=professor,
-            creditos=creditos,
-            turma=turma,
-            destino=destino,
-            vaga=vaga,
-            turno=turno,
-            horario_local=horario_local,
-            horas_distancia=horas_distancia,
-            shf=shf,
-            pre_req=pre_req,
-            depto=depto
-        ))
-
-    ret['disciplinas'] = lista_disciplinas
-
-    return ret
+import re
+import warnings
+
+# typing stuff
+from typing import List, Dict
+
+# local imports
+from .models import RawDisciplina
+
+
+def get_informacoes_csv(info_str: str) -> Dict[str, str]:
+    """
+    Faz um parsing das informações do CSV gerado.
+
+    Procura retirar as informações da primeira linha do CSV, no formato:
+        Período: 20221;Emitido em: 05/04/2022 16:24 h; Data da última atualização: 05/04/2022 13:50h;
+
+    :param info_str: linha contendo as informações do csv
+
+    :return: um dicionario com as chaves "periodo", "emissao" e "atualizacao"
+    """
+
+    lista: List[str] = info_str.split(';')
+    res = {
+        'periodo': '',
+        'emissao': '',
+        'atualizacao': ''
+    }
+
+    for elemento in lista:
+        # separando no ":", onde [0] tem um texto, e [1] o conteudo
+        try:
+            texto_e_conteudo = elemento.split(':')
+            texto, conteudo = texto_e_conteudo[0], ':'.join(texto_e_conteudo[1:])
+            if 'Período' in texto:
+                res['periodo'] = conteudo.strip()
+            elif 'Emitido' in texto:
+                res['emissao'] = conteudo.strip()
+            elif 'atualização' in texto:
+                res['atualizacao'] = conteudo.strip()
+
+        except ValueError:
+            continue
+
+    # verificando integridade
+    for k, v in res.items():
+        if not v:
+            warnings.warn(f"A informacao '{k}' não foi encontrada no csv baixado")
+
+    return res
+
+
+def converte_para_json(texto_csv: str) -> dict:
+
+    ret: dict = {}
+    # le as linhas do csv
+    linhas = texto_csv.splitlines()
+    # salva as informacoes na linha inicial do arquivo
+    ret.update(
+        get_informacoes_csv(linhas[0])
+    )
+
+    # regex para o codigo, que é o primeiro texto na linha
+    re_disciplina = re.compile('^[A-Z]{3}[0-9]{4}')
+
+    lista_disciplinas: List[RawDisciplina] = list()
+
+    for linha in linhas:
+        if re_disciplina.match(linha) is None:
+            continue     # pula a linha que nao tem informacao
+
+        # splitando em brancos e retirando tambem o ';' final se tiver
+        linha_split = linha.strip(' \n\r;').split(';')
+
+        if len(linha_split) == 14:
+            linha_split.pop(11)    # removendo horas de extensao
+
+        if len(linha_split) != 13:
+            warnings.warn(f"Linha iniciada em {linha_split[0]} está inválida")
+            continue     # pula a linha que a informacao esta corrompida
+
+        codigo = linha_split[0].strip()
+        nome = linha_split[1].strip()
+        professor = linha_split[2].strip()
+        creditos = linha_split[3].strip()
+        turma = linha_split[4].strip()
+        destino = linha_split[5].strip()
+        vaga = linha_split[6].strip()
+        turno = linha_split[7].strip()
+        horario_local = linha_split[8].strip()
+        horas_distancia = linha_split[9].strip()
+        shf = linha_split[10].strip()
+        pre_req = linha_split[11].strip()
+        depto = linha_split[12].strip()
+
+        # fazendo parsing dos valores numericos
+        creditos = int(creditos) if creditos.isnumeric() else -1
+        vaga = int(vaga) if vaga.isnumeric() else -1
+        horas_distancia = int(horas_distancia) if horas_distancia.isnumeric() else -1
+        shf = int(shf) if shf.isnumeric() else -1
+
+        # fazendo parsing dos valores booleanos
+        pre_req = pre_req == "SIM"
+        lista_disciplinas.append(RawDisciplina(
+            nome=nome,
+            codigo=codigo,
+            professor=professor,
+            creditos=creditos,
+            turma=turma,
+            destino=destino,
+            vaga=vaga,
+            turno=turno,
+            horario_local=horario_local,
+            horas_distancia=horas_distancia,
+            shf=shf,
+            pre_req=pre_req,
+            depto=depto
+        ))
+
+    ret['disciplinas'] = lista_disciplinas
+
+    return ret
```

### Comparing `microhorario-dl-1.3.0a1/src/microhorario_dl/payloads.py` & `microhorario-dl-1.4/src/microhorario_dl/payloads.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 00000000: 5041 594c 4f41 445f 494e 5445 524d 4544  PAYLOAD_INTERMED
-00000010: 4941 5249 4f20 3d20 7b0d 0a20 2022 5363  IARIO = {..  "Sc
-00000020: 7269 7074 4d61 6e61 6765 7231 223a 2022  riptManager1": "
-00000030: 706e 6c43 6f6e 7465 7564 6f7c 6274 6e42  pnlConteudo|btnB
-00000040: 7573 6361 7222 2c0d 0a20 2022 5f5f 4556  uscar",..  "__EV
-00000050: 454e 5454 4152 4745 5422 3a20 2222 2c0d  ENTTARGET": "",.
-00000060: 0a20 2022 5f5f 4556 454e 5441 5247 554d  .  "__EVENTARGUM
-00000070: 454e 5422 3a20 2222 2c0d 0a20 2022 6464  ENT": "",..  "dd
-00000080: 6c4e 6976 656c 223a 2022 5365 6d20 4469  lNivel": "Sem Di
-00000090: 7374 696e c3a7 c3a3 6f22 2c0d 0a20 2022  stin....o",..  "
-000000a0: 7478 7443 6f64 6967 6f44 7074 4463 7022  txtCodigoDptDcp"
-000000b0: 3a20 2222 2c0d 0a20 2022 7478 744e 6f6d  : "",..  "txtNom
-000000c0: 6544 6370 223a 2022 222c 0d0a 2020 2274  eDcp": "",..  "t
-000000d0: 7874 5174 6443 7265 6469 746f 7322 3a20  xtQtdCreditos": 
-000000e0: 2222 2c0d 0a20 2022 7478 744e 6f6d 6550  "",..  "txtNomeP
-000000f0: 726f 6665 7373 6f72 223a 2022 222c 0d0a  rofessor": "",..
-00000100: 2020 2264 646c 426c 6f71 7565 696f 223a    "ddlBloqueio":
-00000110: 2022 2d31 222c 0d0a 2020 2264 646c 4469   "-1",..  "ddlDi
-00000120: 6122 3a20 2251 7561 6c71 7565 7220 6469  a": "Qualquer di
-00000130: 6122 2c0d 0a20 2022 7478 7448 6f72 6149  a",..  "txtHoraI
-00000140: 6e69 6369 6f22 3a20 2222 2c0d 0a20 2022  nicio": "",..  "
-00000150: 7478 7448 6f72 6146 696d 223a 2022 222c  txtHoraFim": "",
-00000160: 0d0a 2020 2264 646c 5475 726e 6f22 3a20  ..  "ddlTurno": 
-00000170: 222d 3122 2c0d 0a20 2022 6464 6c44 6570  "-1",..  "ddlDep
-00000180: 746f 536f 6c69 6369 7461 6e74 6522 3a20  toSolicitante": 
-00000190: 222d 3122 2c0d 0a20 2022 6869 6464 656e  "-1",..  "hidden
-000001a0: 496e 7075 7454 6f55 7064 6174 6541 5442  InputToUpdateATB
-000001b0: 7566 6665 725f 436f 6d6d 6f6e 546f 6f6c  uffer_CommonTool
-000001c0: 6b69 7453 6372 6970 7473 223a 2022 3122  kitScripts": "1"
-000001d0: 2c0d 0a20 2022 5f5f 4153 594e 4350 4f53  ,..  "__ASYNCPOS
-000001e0: 5422 3a20 2274 7275 6522 2c0d 0a20 2022  T": "true",..  "
-000001f0: 6274 6e42 7573 6361 7222 3a20 2242 7573  btnBuscar": "Bus
-00000200: 6361 7222 0d0a 7d0d 0a0d 0a50 4159 4c4f  car"..}....PAYLO
-00000210: 4144 5f46 494e 414c 203d 207b 0d0a 2020  AD_FINAL = {..  
-00000220: 2264 646c 4e69 7665 6c22 3a20 2253 656d  "ddlNivel": "Sem
-00000230: 2044 6973 7469 6ec3 a7c3 a36f 222c 0d0a   Distin....o",..
-00000240: 2020 2274 7874 436f 6469 676f 4470 7444    "txtCodigoDptD
-00000250: 6370 223a 2022 222c 0d0a 2020 2274 7874  cp": "",..  "txt
-00000260: 4e6f 6d65 4463 7022 3a20 2222 2c0d 0a20  NomeDcp": "",.. 
-00000270: 2022 7478 7451 7464 4372 6564 6974 6f73   "txtQtdCreditos
-00000280: 223a 2022 222c 0d0a 2020 2274 7874 4e6f  ": "",..  "txtNo
-00000290: 6d65 5072 6f66 6573 736f 7222 3a20 2222  meProfessor": ""
-000002a0: 2c0d 0a20 2022 6464 6c42 6c6f 7175 6569  ,..  "ddlBloquei
-000002b0: 6f22 3a20 222d 3122 2c0d 0a20 2022 6464  o": "-1",..  "dd
-000002c0: 6c44 6961 223a 2022 5175 616c 7175 6572  lDia": "Qualquer
-000002d0: 2064 6961 222c 0d0a 2020 2274 7874 486f   dia",..  "txtHo
-000002e0: 7261 496e 6963 696f 223a 2022 222c 0d0a  raInicio": "",..
-000002f0: 2020 2274 7874 486f 7261 4669 6d22 3a20    "txtHoraFim": 
-00000300: 2222 2c0d 0a20 2022 6464 6c54 7572 6e6f  "",..  "ddlTurno
-00000310: 223a 2022 2d31 222c 0d0a 2020 2264 646c  ": "-1",..  "ddl
-00000320: 4465 7074 6f53 6f6c 6963 6974 616e 7465  DeptoSolicitante
-00000330: 223a 2022 2d31 222c 0d0a 2020 2264 646c  ": "-1",..  "ddl
-00000340: 4e75 6d52 6573 756c 7461 646f 7322 3a20  NumResultados": 
-00000350: 2232 3522 2c0d 0a20 2022 6464 6c45 7874  "25",..  "ddlExt
-00000360: 656e 7361 6f22 3a20 2254 6578 746f 222c  ensao": "Texto",
-00000370: 0d0a 2020 2262 746e 446f 776e 6c6f 6164  ..  "btnDownload
-00000380: 223a 2022 4261 6978 6172 222c 0d0a 2020  ": "Baixar",..  
-00000390: 2268 6964 6465 6e49 6e70 7574 546f 5570  "hiddenInputToUp
-000003a0: 6461 7465 4154 4275 6666 6572 5f43 6f6d  dateATBuffer_Com
-000003b0: 6d6f 6e54 6f6f 6c6b 6974 5363 7269 7074  monToolkitScript
-000003c0: 7322 3a20 2231 222c 0d0a 2020 225f 5f45  s": "1",..  "__E
-000003d0: 5645 4e54 5441 5247 4554 223a 2022 222c  VENTTARGET": "",
-000003e0: 0d0a 2020 225f 5f45 5645 4e54 4152 4755  ..  "__EVENTARGU
-000003f0: 4d45 4e54 223a 2022 222c 0d0a 2020 225f  MENT": "",..  "_
-00000400: 5f4c 4153 5446 4f43 5553 223a 2022 220d  _LASTFOCUS": "".
-00000410: 0a7d 0d0a                                .}..
+00000010: 4941 5249 4f20 3d20 7b0a 2020 2253 6372  IARIO = {.  "Scr
+00000020: 6970 744d 616e 6167 6572 3122 3a20 2270  iptManager1": "p
+00000030: 6e6c 436f 6e74 6575 646f 7c62 746e 4275  nlConteudo|btnBu
+00000040: 7363 6172 222c 0a20 2022 5f5f 4556 454e  scar",.  "__EVEN
+00000050: 5454 4152 4745 5422 3a20 2222 2c0a 2020  TTARGET": "",.  
+00000060: 225f 5f45 5645 4e54 4152 4755 4d45 4e54  "__EVENTARGUMENT
+00000070: 223a 2022 222c 0a20 2022 6464 6c4e 6976  ": "",.  "ddlNiv
+00000080: 656c 223a 2022 5365 6d20 4469 7374 696e  el": "Sem Distin
+00000090: c3a7 c3a3 6f22 2c0a 2020 2274 7874 436f  ....o",.  "txtCo
+000000a0: 6469 676f 4470 7444 6370 223a 2022 222c  digoDptDcp": "",
+000000b0: 0a20 2022 7478 744e 6f6d 6544 6370 223a  .  "txtNomeDcp":
+000000c0: 2022 222c 0a20 2022 7478 7451 7464 4372   "",.  "txtQtdCr
+000000d0: 6564 6974 6f73 223a 2022 222c 0a20 2022  editos": "",.  "
+000000e0: 7478 744e 6f6d 6550 726f 6665 7373 6f72  txtNomeProfessor
+000000f0: 223a 2022 222c 0a20 2022 6464 6c42 6c6f  ": "",.  "ddlBlo
+00000100: 7175 6569 6f22 3a20 222d 3122 2c0a 2020  queio": "-1",.  
+00000110: 2264 646c 4469 6122 3a20 2251 7561 6c71  "ddlDia": "Qualq
+00000120: 7565 7220 6469 6122 2c0a 2020 2274 7874  uer dia",.  "txt
+00000130: 486f 7261 496e 6963 696f 223a 2022 222c  HoraInicio": "",
+00000140: 0a20 2022 7478 7448 6f72 6146 696d 223a  .  "txtHoraFim":
+00000150: 2022 222c 0a20 2022 6464 6c54 7572 6e6f   "",.  "ddlTurno
+00000160: 223a 2022 2d31 222c 0a20 2022 6464 6c44  ": "-1",.  "ddlD
+00000170: 6570 746f 536f 6c69 6369 7461 6e74 6522  eptoSolicitante"
+00000180: 3a20 222d 3122 2c0a 2020 2268 6964 6465  : "-1",.  "hidde
+00000190: 6e49 6e70 7574 546f 5570 6461 7465 4154  nInputToUpdateAT
+000001a0: 4275 6666 6572 5f43 6f6d 6d6f 6e54 6f6f  Buffer_CommonToo
+000001b0: 6c6b 6974 5363 7269 7074 7322 3a20 2231  lkitScripts": "1
+000001c0: 222c 0a20 2022 5f5f 4153 594e 4350 4f53  ",.  "__ASYNCPOS
+000001d0: 5422 3a20 2274 7275 6522 2c0a 2020 2262  T": "true",.  "b
+000001e0: 746e 4275 7363 6172 223a 2022 4275 7363  tnBuscar": "Busc
+000001f0: 6172 220a 7d0a 0a50 4159 4c4f 4144 5f46  ar".}..PAYLOAD_F
+00000200: 494e 414c 203d 207b 0a20 2022 6464 6c4e  INAL = {.  "ddlN
+00000210: 6976 656c 223a 2022 5365 6d20 4469 7374  ivel": "Sem Dist
+00000220: 696e c3a7 c3a3 6f22 2c0a 2020 2274 7874  in....o",.  "txt
+00000230: 436f 6469 676f 4470 7444 6370 223a 2022  CodigoDptDcp": "
+00000240: 222c 0a20 2022 7478 744e 6f6d 6544 6370  ",.  "txtNomeDcp
+00000250: 223a 2022 222c 0a20 2022 7478 7451 7464  ": "",.  "txtQtd
+00000260: 4372 6564 6974 6f73 223a 2022 222c 0a20  Creditos": "",. 
+00000270: 2022 7478 744e 6f6d 6550 726f 6665 7373   "txtNomeProfess
+00000280: 6f72 223a 2022 222c 0a20 2022 6464 6c42  or": "",.  "ddlB
+00000290: 6c6f 7175 6569 6f22 3a20 222d 3122 2c0a  loqueio": "-1",.
+000002a0: 2020 2264 646c 4469 6122 3a20 2251 7561    "ddlDia": "Qua
+000002b0: 6c71 7565 7220 6469 6122 2c0a 2020 2274  lquer dia",.  "t
+000002c0: 7874 486f 7261 496e 6963 696f 223a 2022  xtHoraInicio": "
+000002d0: 222c 0a20 2022 7478 7448 6f72 6146 696d  ",.  "txtHoraFim
+000002e0: 223a 2022 222c 0a20 2022 6464 6c54 7572  ": "",.  "ddlTur
+000002f0: 6e6f 223a 2022 2d31 222c 0a20 2022 6464  no": "-1",.  "dd
+00000300: 6c44 6570 746f 536f 6c69 6369 7461 6e74  lDeptoSolicitant
+00000310: 6522 3a20 222d 3122 2c0a 2020 2264 646c  e": "-1",.  "ddl
+00000320: 4e75 6d52 6573 756c 7461 646f 7322 3a20  NumResultados": 
+00000330: 2232 3522 2c0a 2020 2264 646c 4578 7465  "25",.  "ddlExte
+00000340: 6e73 616f 223a 2022 5465 7874 6f22 2c0a  nsao": "Texto",.
+00000350: 2020 2262 746e 446f 776e 6c6f 6164 223a    "btnDownload":
+00000360: 2022 4261 6978 6172 222c 0a20 2022 6869   "Baixar",.  "hi
+00000370: 6464 656e 496e 7075 7454 6f55 7064 6174  ddenInputToUpdat
+00000380: 6541 5442 7566 6665 725f 436f 6d6d 6f6e  eATBuffer_Common
+00000390: 546f 6f6c 6b69 7453 6372 6970 7473 223a  ToolkitScripts":
+000003a0: 2022 3122 2c0a 2020 225f 5f45 5645 4e54   "1",.  "__EVENT
+000003b0: 5441 5247 4554 223a 2022 222c 0a20 2022  TARGET": "",.  "
+000003c0: 5f5f 4556 454e 5441 5247 554d 454e 5422  __EVENTARGUMENT"
+000003d0: 3a20 2222 2c0a 2020 225f 5f4c 4153 5446  : "",.  "__LASTF
+000003e0: 4f43 5553 223a 2022 220a 7d0a            OCUS": "".}.
```

### Comparing `microhorario-dl-1.3.0a1/src/microhorario_dl.egg-info/PKG-INFO` & `microhorario-dl-1.4/src/microhorario_dl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,122 @@
-Metadata-Version: 2.1
-Name: microhorario-dl
-Version: 1.3.0a1
-Summary: PUC-Rio Microhorario Downloader
-Home-page: https://github.com/Leinadium/microhorario-dl
-Author: Daniel Guimarães <github@Leinadium>
-Author-email: daniel.sch.guima@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/Leinadium/microhorario-dl/issues
-Project-URL: Source, https://github.com/Leinadium/microhorario-dl/
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Microhorario Downloader
-
-Biblioteca destinada ao download e utilização de dados provenientes do [Microhorario](https://www.puc-rio.br/microhorario)
- da PUC-Rio.
-
-Essa biblioteca permite baixar todos os dados, e disponibiliza modelos para a utilização destes.
-
-A biblioteca não tem poder de alterar nenhum dado, somente baixar os dados e manipular localmente.
-
-
-Além disso, é possível baixar as ementas automaticamente de todas as disciplinas disponíveis.
-
-
-## Funcionamento
-
-O microhorário não disponibiliza nenhuma API para poder fazer um download automático das disciplinas. Por isso, 
-é necessário fazer requests específicos para conseguir simular um usuário baixando os dados.
-
-Para baixar os dados, um usuário precisa carregar a página inicial, fazer uma consulta sem nenhum filtro, e depois
-baixar os dados no formato CSV. Essa biblioteca simula essas três simulações atráves de um GET e dois POSTS.
-
-Para poder baixar o CSV, é preciso fazer um POST enviando os dados do formulário, assim como variáveis de ASP.NET. Essas
-variáveis são adquiridas ao fazer uma consulta sem filtro, por isso é necessário fazer um POST usando os dados do formulário
-para fazer essa consulta. Porém, essa consulta também utiliza variáveis de ASP.NET e um id de sessão adquiridos ao entrar
-na página. Por isso, é necessário fazer um GET na página inicial para poder adquirir essas variáveis e esse id.
-
-Portanto, são feitos três requests, nomeados `consulta_inicial`, `consulta_intermediaria`, e `consulta_final`:
-
-```text
-consulta inicial (GET https://puc-rio.br/microhorario):
-    recebe:
-        cookies
-        id da sessao
-        nomes e códigos dos departamentos
-        nomes e códigos dos destinos
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-consulta intermediaria (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
-    envia:
-        formulario pedindo uma consulta sem filtro
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-    recebe:
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-consulta final (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
-    envia:
-        formulario pedindo para baixar os resultados de uma consulta sem filtro
-        cookies
-        id da sessao
-        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
-
-    recebe:
-        arquivo csv em utf-16
-```
-
-## Uso
-
-Instale a biblioteca: 
-```shell
-pip install microhorario-dl
-```
-
-Importe e baixe os dados:
-
-```pycon
->>> from microhorario_dl import Microhorario
-
->>> micro = Microhorario.download()
-<Microhorario object at ...>
-
->>> micro.disciplinas
-[<Disciplina [ACN1000]>, <Disciplina[ACN1002]>, ...]
-```
-
-Baixe as ementas:
-
-```pycon
->>> micro.coletar_ementas(verbose=True)
-[0/ 2000] Baixando ACN1000...  DONE (...)
-[1/ 2000] Baixando ACN1002...  DONE (...)
-[2/ 2000] Baixando ACN1004...
-... 
-```
-
-
-Exporte para um json:
-
-```pycon
->>> import json
-
->>> print(json.dumps(micro.as_json(), indent=2))
-{
-    "periodo": "20221",
-    "emissao": "05/04/2022 22:57 h",
-    # ...
-    "disciplinas": [
-        # ...
-    ]
-}
-```
-
+Metadata-Version: 2.1
+Name: microhorario-dl
+Version: 1.4
+Summary: PUC-Rio Microhorario Downloader
+Home-page: https://github.com/Leinadium/microhorario-dl
+Author: Daniel Guimarães <github@Leinadium>
+Author-email: daniel.sch.guima@gmail.com
+Project-URL: Bug Reports, https://github.com/Leinadium/microhorario-dl/issues
+Project-URL: Source, https://github.com/Leinadium/microhorario-dl/
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Microhorario Downloader
+
+Biblioteca destinada ao download e utilização de dados provenientes do [Microhorario](https://www.puc-rio.br/microhorario)
+ da PUC-Rio.
+
+Essa biblioteca permite baixar todos os dados, e disponibiliza modelos para a utilização destes.
+
+A biblioteca não tem poder de alterar nenhum dado, somente baixar os dados e manipular localmente.
+
+
+Além disso, é possível baixar as ementas automaticamente de todas as disciplinas disponíveis.
+
+
+## Funcionamento
+
+O microhorário não disponibiliza nenhuma API para poder fazer um download automático das disciplinas. Por isso, 
+é necessário fazer requests específicos para conseguir simular um usuário baixando os dados.
+
+Para baixar os dados, um usuário precisa carregar a página inicial, fazer uma consulta sem nenhum filtro, e depois
+baixar os dados no formato CSV. Essa biblioteca simula essas três simulações atráves de um GET e dois POSTS.
+
+Para poder baixar o CSV, é preciso fazer um POST enviando os dados do formulário, assim como variáveis de ASP.NET. Essas
+variáveis são adquiridas ao fazer uma consulta sem filtro, por isso é necessário fazer um POST usando os dados do formulário
+para fazer essa consulta. Porém, essa consulta também utiliza variáveis de ASP.NET e um id de sessão adquiridos ao entrar
+na página. Por isso, é necessário fazer um GET na página inicial para poder adquirir essas variáveis e esse id.
+
+Portanto, são feitos três requests, nomeados `consulta_inicial`, `consulta_intermediaria`, e `consulta_final`:
+
+```text
+consulta inicial (GET https://puc-rio.br/microhorario):
+    recebe:
+        cookies
+        id da sessao
+        nomes e códigos dos departamentos
+        nomes e códigos dos destinos
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+consulta intermediaria (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
+    envia:
+        formulario pedindo uma consulta sem filtro
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+    recebe:
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+consulta final (POST /WebMicroHorarioConsulta/MicroHorarioConsulta.aspx):
+    envia:
+        formulario pedindo para baixar os resultados de uma consulta sem filtro
+        cookies
+        id da sessao
+        __VIEWSTATEGENERATOR, __VIEWSTATE e __EVENTVALIDATION
+
+    recebe:
+        arquivo csv em utf-16
+```
+
+## Uso
+
+Instale a biblioteca: 
+```shell
+pip install microhorario-dl
+```
+
+Importe e baixe os dados:
+
+```pycon
+>>> from microhorario_dl import Microhorario
+
+>>> micro = Microhorario.download()
+<Microhorario object at ...>
+
+>>> micro.disciplinas
+[<Disciplina [ACN1000]>, <Disciplina[ACN1002]>, ...]
+```
+
+Baixe as ementas:
+
+```pycon
+>>> micro.coletar_ementas(verbose=True)
+[0/ 2000] Baixando ACN1000...  DONE (...)
+[1/ 2000] Baixando ACN1002...  DONE (...)
+[2/ 2000] Baixando ACN1004...
+... 
+```
+
+
+Exporte para um json:
+
+```pycon
+>>> import json
+
+>>> print(json.dumps(micro.as_json(), indent=2))
+{
+    "periodo": "20221",
+    "emissao": "05/04/2022 22:57 h",
+    # ...
+    "disciplinas": [
+        # ...
+    ]
+}
+```
```

