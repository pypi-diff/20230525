# Comparing `tmp/datanalyse-0.0.7.tar.gz` & `tmp/datanalyse-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanalyse-0.0.7.tar", last modified: Thu May 25 20:21:18 2023, max compression
+gzip compressed data, was "datanalyse-0.0.8.tar", last modified: Thu May 25 21:42:40 2023, max compression
```

## Comparing `datanalyse-0.0.7.tar` & `datanalyse-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.7/LICENSE
--rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.7/README.md
--rw-r--r--   0        0        0      687 2023-05-25 20:21:18.495375 datanalyse-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 18:40:19.058776 datanalyse-0.0.7/src/datanalyse/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.7/src/datanalyse/dataelement/__init__.py
--rw-r--r--   0        0        0     8844 2023-05-09 19:26:05.392037 datanalyse-0.0.7/src/datanalyse/dataelement/dataelement.py
--rw-r--r--   0        0        0     3492 2023-05-08 19:59:39.673710 datanalyse-0.0.7/src/datanalyse/dataelement/dfmanipulation.py
--rw-r--r--   0        0        0    32002 2023-05-25 20:18:54.971395 datanalyse-0.0.7/src/datanalyse/dataelement/formate.py
--rw-r--r--   0        0        0      362 2023-05-08 19:59:45.459719 datanalyse-0.0.7/src/datanalyse/dataelement/stoffwerte.py
--rw-r--r--   0        0        0        0 2023-05-08 18:40:19.069280 datanalyse-0.0.7/src/datanalyse/diagramme/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-08 20:30:15.275768 datanalyse-0.0.7/src/datanalyse/diagramme/balken.py
--rw-r--r--   0        0        0     2863 2023-05-08 19:59:19.452792 datanalyse-0.0.7/src/datanalyse/diagramme/diagramm.py
--rw-r--r--   0        0        0     4224 2023-05-08 19:59:23.694912 datanalyse-0.0.7/src/datanalyse/diagramme/globalbewertung.py
--rw-r--r--   0        0        0     1102 2023-05-08 19:59:25.417764 datanalyse-0.0.7/src/datanalyse/diagramme/matplotlib_parameter.py
--rw-r--r--   0        0        0     3115 2023-05-08 20:30:59.493810 datanalyse-0.0.7/src/datanalyse/diagramme/zeitreihe.py
--rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.7/src/datanalyse/pfade.py
--rw-r--r--   0        0        0   149819 2023-05-09 12:45:52.677187 datanalyse-0.0.7/tests/Ahlborn.xlsx
--rw-r--r--   0        0        0      382 2023-05-25 20:20:01.734815 datanalyse-0.0.7/tests/test_dataelement.py
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 datanalyse-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.8/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.8/README.md
+-rw-r--r--   0        0        0      687 2023-05-25 21:42:40.489539 datanalyse-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 18:40:19.058776 datanalyse-0.0.8/src/datanalyse/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.8/src/datanalyse/dataelement/__init__.py
+-rw-r--r--   0        0        0     8795 2023-05-25 21:32:50.649825 datanalyse-0.0.8/src/datanalyse/dataelement/dataelement.py
+-rw-r--r--   0        0        0     3492 2023-05-08 19:59:39.673710 datanalyse-0.0.8/src/datanalyse/dataelement/dfmanipulation.py
+-rw-r--r--   0        0        0    32004 2023-05-25 21:38:15.211287 datanalyse-0.0.8/src/datanalyse/dataelement/formate.py
+-rw-r--r--   0        0        0      362 2023-05-08 19:59:45.459719 datanalyse-0.0.8/src/datanalyse/dataelement/stoffwerte.py
+-rw-r--r--   0        0        0        0 2023-05-08 18:40:19.069280 datanalyse-0.0.8/src/datanalyse/diagramme/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-08 20:30:15.275768 datanalyse-0.0.8/src/datanalyse/diagramme/balken.py
+-rw-r--r--   0        0        0     2863 2023-05-08 19:59:19.452792 datanalyse-0.0.8/src/datanalyse/diagramme/diagramm.py
+-rw-r--r--   0        0        0     4224 2023-05-08 19:59:23.694912 datanalyse-0.0.8/src/datanalyse/diagramme/globalbewertung.py
+-rw-r--r--   0        0        0     1102 2023-05-08 19:59:25.417764 datanalyse-0.0.8/src/datanalyse/diagramme/matplotlib_parameter.py
+-rw-r--r--   0        0        0     3115 2023-05-08 20:30:59.493810 datanalyse-0.0.8/src/datanalyse/diagramme/zeitreihe.py
+-rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.8/src/datanalyse/pfade.py
+-rw-r--r--   0        0        0   149819 2023-05-09 12:45:52.677187 datanalyse-0.0.8/tests/Ahlborn.xlsx
+-rw-r--r--   0        0        0      424 2023-05-25 21:40:52.754957 datanalyse-0.0.8/tests/test_dataelement.py
+-rw-r--r--   0        0        0      487 2023-05-25 21:35:14.309574 datanalyse-0.0.8/tests/unterlemente.py
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 datanalyse-0.0.8/PKG-INFO
```

### Comparing `datanalyse-0.0.7/LICENSE` & `datanalyse-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/pyproject.toml` & `datanalyse-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datanalyse"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "Maximilian Beyer", email = "maximilian.beyer@tu-dresden.de" },
 ]
 description = "A data analysis package."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `datanalyse-0.0.7/src/datanalyse/dataelement/dataelement.py` & `datanalyse-0.0.8/src/datanalyse/dataelement/dataelement.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         oberelement=None,
         unterelemente: list = [],
     ):
         """
         Objekt, welches die Daten einer Datei / eines Versuchs / einer Versuchsreihe beinhaltet.
         Ein Dataelement kann wiederum aus mehreren Unterelementen bestehen und/oder zu einem Oberelement dazugehören.
         :param pfad: Pfad zur Datei / zum Versuch(sreihen)ordner (als pathlib-Objekt)
-        :param daten: Daten (als Dataframe-Objekt, optional)        
+        :param daten: Daten (als Dataframe-Objekt, optional)
         :param name: Name des Dataelements (optional), entspricht falls nicht angegeben dem Datei-/Ordnernamen
         :param oberelement: Zuweisung des Objekts zu einem übergeordneten Dataelement (optional)
         :param unterelemente: Liste mit allen zum Objekt gehörenden untergeordneten Dataelementen (optional)
         """
 
         # übergebene statische Attribute:
         self.pfad = pfad
@@ -47,18 +47,17 @@
         # Oberelement festlegen, wenn eines angegeben ist (kann auch später erfolgen)
         if oberelement is None:
             self.oberelement = None
         else:
             self.ist_unterelement_von(oberelement)
 
         # Liste der Unterelement(e) festlegen, wenn welche angegeben sind (kann auch später erfolgen)
-        if unterelemente is None:
-            self.unterelemente = list()
-        else:
-            self.unterelemente = unterelemente
+        self.unterelemente = list()
+        for unterelement in unterelemente:
+            self.unterelemente.append(unterelement)
 
     def ist_unterelement_von(self, oberelement):
         """
         weist das Dataelement einem übergeordneten Dataelement zu
         :param oberelement: muss selbst ein Dataelement sein
         """
         if type(oberelement) == Dataelement:
@@ -223,18 +222,16 @@
             liste_der_unterelementnamen.append(unterelement.name)
             anzahl_der_unterelemente += 1
 
         print(
             datetime.now(),
             "Testfunktion ausgelöst von",
             self.name + ":",
-            "Anzahl Unterelemente?",
+            "\nAnzahl Unterelemente?",
             anzahl_der_unterelemente,
-            "Namen der Unterelemente?",
+            "\nNamen der Unterelemente?",
             liste_der_unterelementnamen,
         )
 
-        return self.unterelemente[0]
-
 
 if __name__ == "__main__":
     pass
```

### Comparing `datanalyse-0.0.7/src/datanalyse/dataelement/dfmanipulation.py` & `datanalyse-0.0.8/src/datanalyse/dataelement/dfmanipulation.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/src/datanalyse/dataelement/formate.py` & `datanalyse-0.0.8/src/datanalyse/dataelement/formate.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :param nur_ergebniszeile:
     :return: formatiertes Dataelement
     """
     df = pd.read_excel(
         dataelement.pfad,
         sheet_name=0,
         parse_dates=[["Datum", "Zeit"]],
-        date_format=None,
+        # date_format=None,
     )
 
     # Zeitstempel wird als Index gesetzt
     df.set_index("Datum_Zeit", inplace=True)
 
     # drop alle Spalten, bei denen absolut nichts drin steht (beugt Fehlern vor, tritt vor allem bei Sollwerten auf)
     if dropna_spalten:
```

### Comparing `datanalyse-0.0.7/src/datanalyse/diagramme/balken.py` & `datanalyse-0.0.8/src/datanalyse/diagramme/balken.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/src/datanalyse/diagramme/diagramm.py` & `datanalyse-0.0.8/src/datanalyse/diagramme/diagramm.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/src/datanalyse/diagramme/globalbewertung.py` & `datanalyse-0.0.8/src/datanalyse/diagramme/globalbewertung.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/src/datanalyse/diagramme/matplotlib_parameter.py` & `datanalyse-0.0.8/src/datanalyse/diagramme/matplotlib_parameter.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/src/datanalyse/diagramme/zeitreihe.py` & `datanalyse-0.0.8/src/datanalyse/diagramme/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/src/datanalyse/pfade.py` & `datanalyse-0.0.8/src/datanalyse/pfade.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/tests/Ahlborn.xlsx` & `datanalyse-0.0.8/tests/Ahlborn.xlsx`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.7/PKG-INFO` & `datanalyse-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datanalyse
-Version: 0.0.7
+Version: 0.0.8
 Summary: A data analysis package.
 Author-Email: Maximilian Beyer <maximilian.beyer@tu-dresden.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/MakusuB/datanalyse
 Project-URL: Bug tracker, https://github.com/MakusuB/datanalyse/issues
```

