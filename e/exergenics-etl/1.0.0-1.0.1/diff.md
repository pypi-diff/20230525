# Comparing `tmp/exergenics-etl-1.0.0.tar.gz` & `tmp/exergenics-etl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.0.0.tar", last modified: Tue May 23 02:54:02 2023, max compression
+gzip compressed data, was "exergenics-etl-1.0.1.tar", last modified: Tue May 23 06:58:16 2023, max compression
```

## Comparing `exergenics-etl-1.0.0.tar` & `exergenics-etl-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.563222 exergenics-etl-1.0.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.563222 exergenics-etl-1.0.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47357 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/src/exergenics_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    33594 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/test/test_exergenics_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 02:54:01.000000 exergenics-etl-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:16.171528 exergenics-etl-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 06:58:16.171528 exergenics-etl-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:16.167528 exergenics-etl-1.0.1/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:16.167528 exergenics-etl-1.0.1/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:16.167528 exergenics-etl-1.0.1/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47693 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/app/exergenics_etl/src/exergenics_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:16.171528 exergenics-etl-1.0.1/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33798 2023-05-23 06:58:13.000000 exergenics-etl-1.0.1/app/exergenics_etl/test/test_exergenics_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:16.167528 exergenics-etl-1.0.1/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 06:58:16.000000 exergenics-etl-1.0.1/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 06:58:16.000000 exergenics-etl-1.0.1/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:58:16.000000 exergenics-etl-1.0.1/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 06:58:16.000000 exergenics-etl-1.0.1/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 06:58:16.000000 exergenics-etl-1.0.1/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:58:16.171528 exergenics-etl-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 06:58:15.000000 exergenics-etl-1.0.1/setup.py
```

### Comparing `exergenics-etl-1.0.0/LICENSE` & `exergenics-etl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.0/app/exergenics_etl/__init__.py` & `exergenics-etl-1.0.1/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.0.1/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,106 +370,109 @@
             except AssertionError as e:
                 self.logger.warn(e)
 
         self.logger.info(f'1st verification passed ...')
 
         return
 
-    def _auto_skiprows_csv(self, filePath: str) -> Tuple[pd.DataFrame, int]:
+    def _auto_skiprows_csv(self, fileName: str, zf: zipfile.ZipFile) -> Tuple[pd.DataFrame, int]:
         """
         Reads a CSV file from a zip file object and 
         returns a Pandas dataframe, header row index, 
         and number of rows to skip from the beginning of the file.
 
         Args:
             filepath (str): Absolute path of the CSV file to apply skip rows.
+            zf (zipfile.ZipFile): Zipped folder where the file is.
 
         Returns:
             tuple (pd.DataFrame, int): Return a dataframe of the input 
             filepath with rows skipped if verification passed and None otherwise.
         """
 
         # Try reading the file with different numbers of rows to skip
         skiprowsTrials = range(10)
 
         for skiprowsTrial in skiprowsTrials:
             try:
                 # Try reading the CSV file with the current number of rows to skip
-                df = pd.read_csv(filePath, skiprows=skiprowsTrial, header=None)
+                df = pd.read_csv(zf.open(fileName), skiprows=skiprowsTrial, header=None)
                 skiprows = skiprowsTrial
                 # headerRowID = 0
 
                 self.logger.info(
                     f'Found skiprows value = {skiprowsTrial}')
                 return df, skiprows
 
             except:
                 continue
 
-        errorMessage = f"Table in data file should start at the first 10 rows. Faulty file: {filePath}."
+        errorMessage = f"Table in data file should start at the first 10 rows. Faulty file: {fileName}."
         self.logger.error(errorMessage)
         raise Exception(errorMessage)
 
-    def _auto_skiprows_excel(self, filePath: str) -> Tuple[pd.DataFrame, int]:
+    def _auto_skiprows_excel(self, fileName: str, zf: zipfile.ZipFile) -> Tuple[pd.DataFrame, int]:
         """Skip rows before headers for DataFrame read from an Excel sheet.
         Assume redundant stuffs in excel sheets are in the first column above timestamps.
         That is, the header of a data point is the first non-NA string in that column.
         Verify after skipping rows.
 
         Args:
             filepath (str): Absolute path of the Excel file to apply skip rows.
+            zf (zipfile.ZipFile): Zipped folder where the file is.
 
         Returns:
             tuple (pd.DataFrame, int): Return a dataframe of the input 
             filepath with rows skipped if verification passed and None otherwise.
         """
-        df = pd.read_excel(filePath, index_col=False, header=None)
+        df = pd.read_excel(zf.open(fileName), index_col=False, header=None)
 
         # Find the row ID of header and compute the number of rows to skip
         col1 = df[df.columns[1]]
         headerRowID = col1.dropna().index[0]
         skiprows = headerRowID
 
         # Skip rows
         df.drop(labels=range(skiprows), inplace=True)
 
         self.logger.info(f'Found skiprows = {skiprows}')
 
         return df, skiprows
 
-    def read(self, filePath: str) -> pd.DataFrame:
-        """Reads a data file while skipping non-data rows on top of the file.
+    def read(self, fileName: str, zf: zipfile.ZipFile = None) -> pd.DataFrame:
+        """Reads a data file from a zipped folder while skipping non-data rows on top of the file.
 
         Args:
-            filePath (str): Absolute path of file to apply skip rows.
+            fileName (str): File name of the file to apply skip rows.
+            zf (zipfile.ZipFile): Zipped folder where the file is.
 
         Returns:
             pd.DataFrame: Pandas DataFrame of the input CSV file with skipped rows.  
         """
 
         # Get the filename extension of the current data file
         extension = [
-            extension for extension in EXTENSIONS if filePath.endswith(extension)][0]
+            extension for extension in EXTENSIONS if fileName.endswith(extension)][0]
 
         if self.skiprows is None:
             # Find skiprows value to read the data file
             if extension == 'xlsx':
-                df, self.skiprows = self._auto_skiprows_excel(filePath)
+                df, self.skiprows = self._auto_skiprows_excel(fileName, zf)
             elif extension == 'csv':
-                df, self.skiprows = self._auto_skiprows_csv(filePath)
+                df, self.skiprows = self._auto_skiprows_csv(fileName, zf)
 
             # Verify
             self.validate_headers(df)
 
         else:
             # Read the data file with the last skiprows value
             if extension == 'csv':
-                df = pd.read_csv(filePath, skiprows=self.skiprows)
+                df = pd.read_csv(zf.open(fileName), skiprows=self.skiprows)
             elif extension == 'xlsx':
-                df = pd.read_excel(filePath, skiprows=self.skiprows)
+                df = pd.read_excel(zf.open(fileName), skiprows=self.skiprows)
 
         # Validate that headers are strings
         self.validate_headers(df)
 
         return df
```

### Comparing `exergenics-etl-1.0.0/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.0.1/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.0.1/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,36 +211,37 @@
         fileNames = get_file_name_list(my_manual_zipfile)
         assert len(fileNames) == 4
 
 
 class TestSkipRowsMachineClass:
 
     @pytest.fixture(scope='class')
-    def my_skiprows_test_csv(self):
-        csvPath = "app/exergenics_etl/test/testData/skiprows_testFile.csv"
-        return csvPath
+    def my_expected_first_row(self):
+        """The first row of the expected output form skipRowsMachine.read."""
+        return pd.Series(['Timestamp', 'Test data point'])
 
-    @pytest.fixture(scope='class')
-    def my_skiprows_test_xlsx(self):
-        xlsxPath = "app/exergenics_etl/test/testData/skiprows_testFile.xlsx"
-        return xlsxPath
-
-    def test_skiprowsmachine_read_csv(self, my_skiprows_test_csv):
-        expectedFirstRow = pd.Series(['Timestamp', 'Test data point'])
+    def test_skiprowsmachine_read_compressed_csv(self, my_expected_first_row):
         skipRowsMachine = SkipRowsMachine()
-        df = skipRowsMachine.read(my_skiprows_test_csv)
+        myTestFilePath = "skiprows_testFileInZip.csv"
+        myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_testFileInZip.csv.zip"
+        myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
 
-        assert all(df.iloc[0] == expectedFirstRow)
+        df = skipRowsMachine.read(myTestFilePath, myTestZippedFile)
 
-    def test_skiprowsmachine_read_xlsx(self, my_skiprows_test_xlsx):
-        expectedFirstRow = pd.Series(['Timestamp', 'Test data point'])
+        assert all(df.iloc[0] == my_expected_first_row)
+
+    def test_skiprowsmachine_read_compressed_xlsx(self, my_expected_first_row):
         skipRowsMachine = SkipRowsMachine()
-        df = skipRowsMachine.read(my_skiprows_test_xlsx)
+        myTestFilePath = "skiprows_testFileInZip.xlsx"
+        myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_testFileInZip.xlsx.zip"
+        myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
+
+        df = skipRowsMachine.read(myTestFilePath, myTestZippedFile)
 
-        assert all(df.iloc[0] == expectedFirstRow)
+        assert all(df.iloc[0] == my_expected_first_row)
 
 
 class TestInputValidationClass:
 
     @pytest.fixture(scope='class')
     def my_wide_format_dataframe(self):
         filePath = 'app/exergenics_etl/test/testData/wide_data.csv'
```

### Comparing `exergenics-etl-1.0.0/setup.py` & `exergenics-etl-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.0.0",
+    version="v1.0.1",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

