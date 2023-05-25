# Comparing `tmp/relativedate-1.2.0.tar.gz` & `tmp/relativedate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-1.2.0.tar", last modified: Tue May 23 18:34:23 2023, max compression
+gzip compressed data, was "relativedate-1.3.0.tar", last modified: Wed May 24 12:55:45 2023, max compression
```

## Comparing `relativedate-1.2.0.tar` & `relativedate-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 18:34:23.039123 relativedate-1.2.0/
--rw-rw-rw-   0        0        0     2387 2023-05-23 18:34:23.038125 relativedate-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2023-05-23 18:33:38.000000 relativedate-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 18:34:23.024163 relativedate-1.2.0/relativedate/
--rw-rw-rw-   0        0        0     1427 2023-05-23 18:25:53.000000 relativedate-1.2.0/relativedate/__init__.py
--rw-rw-rw-   0        0        0      394 2023-05-23 18:27:39.000000 relativedate-1.2.0/relativedate/dtget.py
--rw-rw-rw-   0        0        0     1369 2023-05-23 15:07:39.000000 relativedate-1.2.0/relativedate/dtmath.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:34:23.037132 relativedate-1.2.0/relativedate.egg-info/
--rw-rw-rw-   0        0        0     2387 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 18:34:23.039123 relativedate-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-05-23 18:34:19.000000 relativedate-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:55:45.573289 relativedate-1.3.0/
+-rw-rw-rw-   0        0        0     2414 2023-05-24 12:55:45.573289 relativedate-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2254 2023-05-24 11:24:35.000000 relativedate-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 12:55:45.556336 relativedate-1.3.0/relativedate/
+-rw-rw-rw-   0        0        0     1649 2023-05-24 12:48:06.000000 relativedate-1.3.0/relativedate/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-05-24 12:43:06.000000 relativedate-1.3.0/relativedate/dtget.py
+-rw-rw-rw-   0        0        0     1243 2023-05-24 12:25:12.000000 relativedate-1.3.0/relativedate/dtmath.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:55:45.572292 relativedate-1.3.0/relativedate.egg-info/
+-rw-rw-rw-   0        0        0     2414 2023-05-24 12:55:45.000000 relativedate-1.3.0/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-24 12:55:45.000000 relativedate-1.3.0/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:55:45.000000 relativedate-1.3.0/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-24 12:55:45.000000 relativedate-1.3.0/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 12:55:45.573289 relativedate-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-24 12:55:39.000000 relativedate-1.3.0/setup.py
```

### Comparing `relativedate-1.2.0/PKG-INFO` & `relativedate-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.2.0
+Version: 1.3.0
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
@@ -12,17 +12,18 @@
 </p>
 <p>
     O objetivo desta biblioteca é facilitar a manipulação de datas relativas e calculos com datas, em sua primeira versão estamos trabalhando apenas com a data relativa baseado em mês, onde pode se passar o argumento de meses (positivo e negativo) e retornará a data relativa ao mês desejado
 </p>
 
 <hr>
 <b>Links</b> <br>
+<b>Documentação:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
 <b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
-<b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
-<b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
+<b>PyPI (last version):</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
+
 
 <hr>
 <b>Instalação:</b>
 <p>pip install relativedate</p>
 <hr>
 
 <hr>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.2.0 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.3.0 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
 data relativa baseado em mÃªs, onde pode se passar o argumento de meses
 (positivo e negativo) e retornarÃ¡ a data relativa ao mÃªs desejado
 ===============================================================================
 Links
+DocumentaÃ§Ã£o: https://jmiante.github.io/relativedate
 GitHub: https://github.com/jmiante/relativedate
-PyPI: https://pypi.org/project/relativedate
-Site: https://jmiante.github.io/relativedate
+PyPI (last version): https://pypi.org/project/relativedate
 ===============================================================================
 InstalaÃ§Ã£o:
 pip install relativedate
 ===============================================================================
 ===============================================================================
 Exemplo UtilizaÃ§Ã£o:
 from datetime import datetime
```

### Comparing `relativedate-1.2.0/README.md` & `relativedate-1.3.0/relativedate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+Metadata-Version: 2.1
+Name: relativedate
+Version: 1.3.0
+Summary: Pacote Python para tabalhar com Datas Relativas
+Description-Content-Type: text/markdown
+
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
     Biblioteca Python relacionada a datas, onde é criado um objeto "RelativeDate" que possui o atributo datetime, onde é retornado um objeto datetime.
 </p>
 <p>
     O objetivo desta biblioteca é facilitar a manipulação de datas relativas e calculos com datas, em sua primeira versão estamos trabalhando apenas com a data relativa baseado em mês, onde pode se passar o argumento de meses (positivo e negativo) e retornará a data relativa ao mês desejado
 </p>
 
 <hr>
 <b>Links</b> <br>
+<b>Documentação:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
 <b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
-<b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
-<b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
+<b>PyPI (last version):</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
+
 
 <hr>
 <b>Instalação:</b>
 <p>pip install relativedate</p>
 <hr>
 
 <hr>
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
+Metadata-Version: 2.1 Name: relativedate Version: 1.3.0 Summary: Pacote Python
+para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
 data relativa baseado em mÃªs, onde pode se passar o argumento de meses
 (positivo e negativo) e retornarÃ¡ a data relativa ao mÃªs desejado
 ===============================================================================
 Links
+DocumentaÃ§Ã£o: https://jmiante.github.io/relativedate
 GitHub: https://github.com/jmiante/relativedate
-PyPI: https://pypi.org/project/relativedate
-Site: https://jmiante.github.io/relativedate
+PyPI (last version): https://pypi.org/project/relativedate
 ===============================================================================
 InstalaÃ§Ã£o:
 pip install relativedate
 ===============================================================================
 ===============================================================================
 Exemplo UtilizaÃ§Ã£o:
 from datetime import datetime
```

### Comparing `relativedate-1.2.0/relativedate/__init__.py` & `relativedate-1.3.0/relativedate/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,8 +37,13 @@
     
     ### DATE GET ###
     def lastDay(self):
         return dtget.lastDay(self.datetime)
     
     def lastDate(self):
         return dtget.lastDate(self.datetime)
+    
+    def getUtilDay(self, util_day, disregard=[]):
+        return dtget.getUtilDay(self.datetime, util_day, disregard)
 
+    def utilDays(self, disregard=[]):
+        return dtget.utilDays(self.datetime, disregard)
```

### Comparing `relativedate-1.2.0/relativedate/dtmath.py` & `relativedate-1.3.0/relativedate/dtmath.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from datetime import timedelta
 
-def addYear(datetime, relative_year):
+def addYear(dt, relative_year):
     try:
-        year = datetime.year + int(relative_year)
+        year = dt.year + int(relative_year)
     except:
          raise Exception('O atributo relative_year deve ser do tipo INT')
-    return datetime.replace(year=year)
+    return dt.replace(year=year)
 
-def addMonth(datetime, relative_month):
+def addMonth(dt, relative_month):
         """
         """
-        month = datetime.month + relative_month
-        year = datetime.year
+        month = dt.month + relative_month
+        year = dt.year
             
         # Tratado Ano
         if abs(relative_month) > 12:
             year_delta = int(relative_month / 12)
             year += year_delta
             month += (abs(year_delta) * 12) 
         
         # Tratamento do Mês
         if month < 1: 
             month += 12
             year -= 1
         elif month > 12: 
             month -= 12
             year += 1
-        return datetime.replace(year=year, month=month)
+        return dt.replace(year=year, month=month)
 
-def addDay(datetime, relative_day):
-     return datetime + timedelta(days=relative_day)
+def addDay(dt, relative_day):
+     return dt + timedelta(days=relative_day)
 
 
-def add(datetime, year=0, month=0, day=0, hour=0, minute=0, second=0):
-    datetime = datetime
+def add(dt, year=0, month=0, day=0, hour=0, minute=0, second=0):
+    dt = dt
     if month != 0:
-        datetime = addMonth(datetime, month)
+        dt = addMonth(dt, month)
     if year != 0:
-        datetime = addYear(datetime, year)
-    return datetime + timedelta(days=day, hours=hour, minutes=minute, seconds=second)
+        dt = addYear(dt, year)
+    return dt + timedelta(days=day, hours=hour, minutes=minute, seconds=second)
 
-def dateDiff(first_datetime, second_datetime):
-     return second_datetime - first_datetime
+def dateDiff(first_dt, second_dt):
+     return second_dt - first_dt
```

### Comparing `relativedate-1.2.0/relativedate.egg-info/PKG-INFO` & `relativedate-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-Metadata-Version: 2.1
-Name: relativedate
-Version: 1.2.0
-Summary: Pacote Python para tabalhar com Datas Relativas
-Description-Content-Type: text/markdown
-
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
     Biblioteca Python relacionada a datas, onde é criado um objeto "RelativeDate" que possui o atributo datetime, onde é retornado um objeto datetime.
 </p>
 <p>
     O objetivo desta biblioteca é facilitar a manipulação de datas relativas e calculos com datas, em sua primeira versão estamos trabalhando apenas com a data relativa baseado em mês, onde pode se passar o argumento de meses (positivo e negativo) e retornará a data relativa ao mês desejado
 </p>
 
 <hr>
 <b>Links</b> <br>
+<b>Documentação:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
 <b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
-<b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
-<b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
+<b>PyPI (last version):</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
+
 
 <hr>
 <b>Instalação:</b>
 <p>pip install relativedate</p>
 <hr>
 
 <hr>
```

#### html2text {}

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.2.0 Summary: Pacote Python
-para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
 data relativa baseado em mÃªs, onde pode se passar o argumento de meses
 (positivo e negativo) e retornarÃ¡ a data relativa ao mÃªs desejado
 ===============================================================================
 Links
+DocumentaÃ§Ã£o: https://jmiante.github.io/relativedate
 GitHub: https://github.com/jmiante/relativedate
-PyPI: https://pypi.org/project/relativedate
-Site: https://jmiante.github.io/relativedate
+PyPI (last version): https://pypi.org/project/relativedate
 ===============================================================================
 InstalaÃ§Ã£o:
 pip install relativedate
 ===============================================================================
 ===============================================================================
 Exemplo UtilizaÃ§Ã£o:
 from datetime import datetime
```

