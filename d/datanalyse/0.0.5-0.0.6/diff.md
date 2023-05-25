# Comparing `tmp/datanalyse-0.0.5.tar.gz` & `tmp/datanalyse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanalyse-0.0.5.tar", last modified: Wed May 10 08:48:10 2023, max compression
+gzip compressed data, was "datanalyse-0.0.6.tar", last modified: Thu May 25 19:04:07 2023, max compression
```

## Comparing `datanalyse-0.0.5.tar` & `datanalyse-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1078 2023-05-08 10:35:18.120135 datanalyse-0.0.5/LICENSE
--rw-r--r--   0        0        0      459 2023-05-08 11:21:31.284922 datanalyse-0.0.5/README.md
--rw-r--r--   0        0        0      664 2023-05-10 08:48:10.438077 datanalyse-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 13:28:09.975326 datanalyse-0.0.5/src/datanalyse/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 21:03:10.188371 datanalyse-0.0.5/src/datanalyse/dataelement/__init__.py
--rw-r--r--   0        0        0     8844 2023-05-10 07:45:44.270328 datanalyse-0.0.5/src/datanalyse/dataelement/dataelement.py
--rw-r--r--   0        0        0     3492 2023-05-08 20:06:25.263720 datanalyse-0.0.5/src/datanalyse/dataelement/dfmanipulation.py
--rw-r--r--   0        0        0    32051 2023-05-10 07:45:44.276278 datanalyse-0.0.5/src/datanalyse/dataelement/formate.py
--rw-r--r--   0        0        0      362 2023-05-08 20:06:25.269023 datanalyse-0.0.5/src/datanalyse/dataelement/stoffwerte.py
--rw-r--r--   0        0        0        0 2022-11-21 14:15:44.602999 datanalyse-0.0.5/src/datanalyse/diagramme/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-10 07:45:44.282229 datanalyse-0.0.5/src/datanalyse/diagramme/balken.py
--rw-r--r--   0        0        0     2863 2023-05-08 20:06:25.272554 datanalyse-0.0.5/src/datanalyse/diagramme/diagramm.py
--rw-r--r--   0        0        0     4224 2023-05-08 20:06:25.274579 datanalyse-0.0.5/src/datanalyse/diagramme/globalbewertung.py
--rw-r--r--   0        0        0     1102 2023-05-08 20:06:25.278540 datanalyse-0.0.5/src/datanalyse/diagramme/matplotlib_parameter.py
--rw-r--r--   0        0        0     3115 2023-05-10 07:45:44.288184 datanalyse-0.0.5/src/datanalyse/diagramme/zeitreihe.py
--rw-r--r--   0        0        0      703 2023-05-08 10:35:18.138208 datanalyse-0.0.5/src/datanalyse/pfade.py
--rw-r--r--   0        0        0   149819 2023-05-10 07:45:44.296614 datanalyse-0.0.5/tests/Ahlborn.xlsx
--rw-r--r--   0        0        0      376 2023-05-10 08:29:38.906242 datanalyse-0.0.5/tests/test_dataelement.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 datanalyse-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-08 10:35:18.120135 datanalyse-0.0.6/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-08 11:21:31.284922 datanalyse-0.0.6/README.md
+-rw-r--r--   0        0        0      687 2023-05-25 19:04:07.831587 datanalyse-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 13:28:09.975326 datanalyse-0.0.6/src/datanalyse/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:03:10.188371 datanalyse-0.0.6/src/datanalyse/dataelement/__init__.py
+-rw-r--r--   0        0        0     8844 2023-05-10 07:45:44.270328 datanalyse-0.0.6/src/datanalyse/dataelement/dataelement.py
+-rw-r--r--   0        0        0     3492 2023-05-08 20:06:25.263720 datanalyse-0.0.6/src/datanalyse/dataelement/dfmanipulation.py
+-rw-r--r--   0        0        0    32204 2023-05-10 12:53:17.678047 datanalyse-0.0.6/src/datanalyse/dataelement/formate.py
+-rw-r--r--   0        0        0      362 2023-05-08 20:06:25.269023 datanalyse-0.0.6/src/datanalyse/dataelement/stoffwerte.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:15:44.602999 datanalyse-0.0.6/src/datanalyse/diagramme/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-10 07:45:44.282229 datanalyse-0.0.6/src/datanalyse/diagramme/balken.py
+-rw-r--r--   0        0        0     2863 2023-05-08 20:06:25.272554 datanalyse-0.0.6/src/datanalyse/diagramme/diagramm.py
+-rw-r--r--   0        0        0     4224 2023-05-08 20:06:25.274579 datanalyse-0.0.6/src/datanalyse/diagramme/globalbewertung.py
+-rw-r--r--   0        0        0     1102 2023-05-08 20:06:25.278540 datanalyse-0.0.6/src/datanalyse/diagramme/matplotlib_parameter.py
+-rw-r--r--   0        0        0     3115 2023-05-10 07:45:44.288184 datanalyse-0.0.6/src/datanalyse/diagramme/zeitreihe.py
+-rw-r--r--   0        0        0      703 2023-05-08 10:35:18.138208 datanalyse-0.0.6/src/datanalyse/pfade.py
+-rw-r--r--   0        0        0   149819 2023-05-10 07:45:44.296614 datanalyse-0.0.6/tests/Ahlborn.xlsx
+-rw-r--r--   0        0        0      331 2023-05-10 12:30:07.304385 datanalyse-0.0.6/tests/test_dataelement.py
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 datanalyse-0.0.6/PKG-INFO
```

### Comparing `datanalyse-0.0.5/LICENSE` & `datanalyse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/pyproject.toml` & `datanalyse-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "datanalyse"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Maximilian Beyer", email = "maximilian.beyer@tu-dresden.de" },
 ]
 description = "A data analysis package."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pandas>=2.0.1",
     "matplotlib>=3.7.1",
+    "openpyxl>=3.1.2",
 ]
 
 [project.urls]
 Homepage = "https://github.com/MakusuB/datanalyse"
 "Bug Tracker" = "https://github.com/MakusuB/datanalyse/issues"
 
 [build-system]
```

### Comparing `datanalyse-0.0.5/src/datanalyse/dataelement/dataelement.py` & `datanalyse-0.0.6/src/datanalyse/dataelement/dataelement.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/dataelement/dfmanipulation.py` & `datanalyse-0.0.6/src/datanalyse/dataelement/dfmanipulation.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/dataelement/formate.py` & `datanalyse-0.0.6/src/datanalyse/dataelement/formate.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,19 +24,20 @@
     :param resample_zeitschritt: Resampling aller Daten dient der Umrechnung auf eine gemeinsame Zeitschrittweite, es werden alle zur Zeitschrittweite gehörenden Werte gemittelt
     :param nur_ergebniszeile:
     :return: formatiertes Dataelement
     """
     df = pd.read_excel(
         dataelement.pfad,
         sheet_name=0,
-        parse_dates=[
-            ["Datum", "Zeit"]
-        ],  # Datum und Zeit werden zum Zeitstempel kombiniert
+        # parse_dates=[["Datum", "Zeit"]],  # Kombination von Datum und Zeit nicht mehr möglich, da kein dayfirst
     )
 
+    # Kombination von Datum und Zeit zu Zeitstempel
+    df["Datum_Zeit"] = pd.to_datetime(str(df["Datum"]) + " " + str(df["Zeit"]), dayfirst=True)
+    
     # Zeitstempel wird als Index gesetzt
     df.set_index("Datum_Zeit", inplace=True)
 
     # drop alle Spalten, bei denen absolut nichts drin steht (beugt Fehlern vor, tritt vor allem bei Sollwerten auf)
     if dropna_spalten:
         df.dropna(how="all", axis=1, inplace=True)
 
@@ -101,16 +102,16 @@
         sep=";",
         decimal=",",
         encoding="ANSI",
         index_col=0,
         header=2,
         skiprows=[3, 4, 5, 6],
         parse_dates=[[0, 1]],
-        dayfirst=True,
-    )  # Verhindert Verwechslung von Tag und Monat beim Einlesen des Datums
+        dayfirst=True,  # Verhindert Verwechslung von Tag und Monat beim Einlesen des Datums
+    )
 
     # Indexspalte einen ordentlichen Namen geben (heißt aktuell etwa "Kommentar_Unnamed: 1")
     df.index.names = ["Datum_Zeit"]
 
     # drop alle Spalten, bei denen absolut nichts drin steht (beugt Fehlern vor, tritt vor allem bei Sollwerten auf)
     if dropna_spalten:
         df.dropna(how="all", axis=1, inplace=True)
```

### Comparing `datanalyse-0.0.5/src/datanalyse/diagramme/balken.py` & `datanalyse-0.0.6/src/datanalyse/diagramme/balken.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/diagramme/diagramm.py` & `datanalyse-0.0.6/src/datanalyse/diagramme/diagramm.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/diagramme/globalbewertung.py` & `datanalyse-0.0.6/src/datanalyse/diagramme/globalbewertung.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/diagramme/matplotlib_parameter.py` & `datanalyse-0.0.6/src/datanalyse/diagramme/matplotlib_parameter.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/diagramme/zeitreihe.py` & `datanalyse-0.0.6/src/datanalyse/diagramme/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/src/datanalyse/pfade.py` & `datanalyse-0.0.6/src/datanalyse/pfade.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/tests/Ahlborn.xlsx` & `datanalyse-0.0.6/tests/Ahlborn.xlsx`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.5/PKG-INFO` & `datanalyse-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: datanalyse
-Version: 0.0.5
+Version: 0.0.6
 Summary: A data analysis package.
 Author-Email: Maximilian Beyer <maximilian.beyer@tu-dresden.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/MakusuB/datanalyse
 Project-URL: Bug tracker, https://github.com/MakusuB/datanalyse/issues
 Requires-Python: >=3.11
 Requires-Dist: pandas>=2.0.1
 Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: openpyxl>=3.1.2
 Description-Content-Type: text/markdown
 
 # datanalyse
 
 The package name datanalyse is a suitcase word for data and analyse - mainly of experimental data from the Combined Energy Lab at TU Dresden, but perhaps useful for others as well. However, due to its absolute alpha status, I cannot recommend it to anybody in the world but me.
 
 It is more or less a tool-kit for my daily work as an experimentalist and data scientist and makes use of the fantastic packages pandas, pathlib and matplotlib.
```

