# Comparing `tmp/tidy_tweet-0.4.0.tar.gz` & `tmp/tidy_tweet-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-0.4.0.tar", last modified: Wed Jun 22 04:06:42 2022, max compression
+gzip compressed data, was "tidy_tweet-1.0.0a1.tar", last modified: Thu May 25 00:46:45 2023, max compression
```

## Comparing `tidy_tweet-0.4.0.tar` & `tidy_tweet-1.0.0a1.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.135580 tidy_tweet-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9161 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8430 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.135580 tidy_tweet-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-22 04:06:41.000000 tidy_tweet-0.4.0/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    12851 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9161 2022-06-22 04:06:41.000000 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-06-22 04:06:42.000000 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 04:06:41.000000 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-22 04:06:41.000000 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-22 04:06:41.000000 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-22 04:06:41.000000 tidy_tweet-0.4.0/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 04:06:42.139580 tidy_tweet-0.4.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   586918 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-22 04:06:23.000000 tidy_tweet-0.4.0/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.731817 tidy_tweet-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.731817 tidy_tweet-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16794 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/test_overall.py
```

### Comparing `tidy_tweet-0.4.0/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0a1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-0.4.0/.github/workflows/tests.yml` & `tidy_tweet-1.0.0a1/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9]
+        python-version: [3.8, 3.9, 3.10.11, 3.11]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `tidy_tweet-0.4.0/LICENSE` & `tidy_tweet-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-0.4.0/PKG-INFO` & `tidy_tweet-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 0.4.0
+Version: 1.0.0a1
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -61,15 +61,15 @@
 page object, and no commas between top-level objects.
 
 ### Output: Sqlite database of tweets and metadata
 
 After processing your Twitter results pages with tidy_tweet (see [Usage](#usage)), you will have an 
 [SQLite][sqlite] database file at the location you specified.
 
-Database schema will be published here as soon as the initial schema is finalised.
+See the [current database schema](docs/schema.md).
 
 ## Prerequisites
 
 - Python 3.8+
 - A command line shell/terminal, such as bash, Mac Terminal, Git Bash, Anaconda Prompt, etc
 
 This tool requires Python 3.8 or later, the instructions assume you already have Python installed. If you haven't
```

### Comparing `tidy_tweet-0.4.0/README.md` & `tidy_tweet-1.0.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 page object, and no commas between top-level objects.
 
 ### Output: Sqlite database of tweets and metadata
 
 After processing your Twitter results pages with tidy_tweet (see [Usage](#usage)), you will have an 
 [SQLite][sqlite] database file at the location you specified.
 
-Database schema will be published here as soon as the initial schema is finalised.
+See the [current database schema](docs/schema.md).
 
 ## Prerequisites
 
 - Python 3.8+
 - A command line shell/terminal, such as bash, Mac Terminal, Git Bash, Anaconda Prompt, etc
 
 This tool requires Python 3.8 or later, the instructions assume you already have Python installed. If you haven't
```

### Comparing `tidy_tweet-0.4.0/contributing.md` & `tidy_tweet-1.0.0a1/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-0.4.0/setup.cfg` & `tidy_tweet-1.0.0a1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 [options.extras_require]
 development = 
 	nox >= 2021.10.1
 	pytest
 	flake8
 	black
+	setuptools_scm
 
 [options.entry_points]
 console_scripts = 
 	tidy_tweet = tidy_tweet.__main__:tidy_twarc_jsons
 
 [flake8]
 max-line-length = 88
```

### Comparing `tidy_tweet-0.4.0/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0a1/src/tidy_tweet/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-0.4.0/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0a1/src/tidy_tweet/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,25 +79,30 @@
     with sqlite3.connect(db_name) as db:
         cursor = db.cursor()
         for tbl_stmt in mapping.create_table_statements:
             cursor.execute(tbl_stmt)
 
         # Initialise the schema related metadata first, otherwise if an
         # insert fails we end up with a schema version of null.
-        cursor.executemany(
-            mapping.sql_by_table["_metadata"]["insert"],
-            mapping.map_tidy_tweet_metadata()["_metadata"],
-        )
+        # cursor.executemany(
+        #     mapping.sql_by_table["_metadata"]["insert"],
+        #     mapping.map_tidy_tweet_metadata()["_metadata"],
+        # )
 
         if not allow_existing_database:
             # ".tables" only works in the sqlite shell!
             cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
             created_tables = cursor.fetchall()
             logger.debug("Created database tables: " + str(created_tables))
             assert len(created_tables) == len(mapping.create_table_statements)
+            cursor.execute("create table schema_version (schema_version text)")
+            cursor.execute(
+                "insert into schema_version values (:version)",
+                {"version": mapping.SCHEMA_VERSION},
+            )
 
         logger.info("The database schema has been initialised")
 
 
 def check_database_version(db_name):
     """
     Checks the given pre-existing database is valid for use with this version
@@ -109,24 +114,22 @@
     """
     logger.debug(f"Checking version compatibility of {db_name}...")
     conn = sqlite3.connect(db_name)
     with conn:
         db = conn.cursor()
         db.execute(
             """
-            select metadata_value from _metadata
-            where metadata_key='schema_version'
+            select schema_version from schema_version
             """
         )
         result = db.fetchone() or []
         db_schema_version = None if len(result) == 0 else result[0]
         db.execute(
             """
-            select metadata_value from _metadata
-            where metadata_key='tidy_tweet_version'
+            select max(tidy_tweet_version) from results_page
             """
         )
         result = db.fetchone() or []
         db_library_version = None if len(result) == 0 else result[0]
     if db_schema_version != mapping.SCHEMA_VERSION:
         raise SchemaVersionMismatchError(
             mapping.SCHEMA_VERSION, db_schema_version, db_name
```

### Comparing `tidy_tweet-0.4.0/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0a1/src/tidy_tweet/processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import tidy_tweet.tweet_mapping as mapping
 from logging import getLogger
 from tidy_tweet.utilities import add_mappings
 
 logger = getLogger(__name__)
 
 
-def _load_page_object(page_json: Mapping, connection: sqlite3.Connection):
+def _load_page_object(
+    file_name: str, page_json: Mapping, connection: sqlite3.Connection
+):
     """
     Takes a page of twarc Twitter API results and loads it into the database.
 
     If using this function to parse Twitter data from an object direct from Twarc
     without saving the JSON Twarc output, we recommend you save the raw data Twarc json
     output by some other means.
 
@@ -22,27 +24,33 @@
     """
     db = connection.cursor()
 
     mappings = {}
 
     # Metadata
     logger.debug("Processing metadata section of page")
-    if "__twarc" in page_json:
-        add_mappings(mappings, mapping.map_twarc_metadata(page_json["__twarc"]))
+    twitter_metadata = page_json.get("meta", {})
+    twarc_metadata = page_json.get("__twarc", {})
+    # Write this first so we can get the page id
+    db.execute(
+        mapping.sql_by_table["results_page"]["insert"],
+        mapping.map_page_metadata(file_name, twitter_metadata, twarc_metadata),
+    )
+    page_info = (file_name, db.lastrowid)
 
     # Includes
     logger.debug("Processing includes section of page")
     if "media" in page_json["includes"]:
         add_mappings(mappings, mapping.map_media(page_json["includes"]["media"]))
 
     for user in page_json["includes"].get("users", []):
-        add_mappings(mappings, mapping.map_user(user))
+        add_mappings(mappings, mapping.map_user(user, *page_info))
 
     for tweet in page_json["includes"].get("tweets", []):
-        add_mappings(mappings, mapping.map_tweet(tweet, False))
+        add_mappings(mappings, mapping.map_tweet(tweet, False, *page_info))
 
     # Data
     logger.debug("Processing data section of page")
 
     #  - Some endpoints will return responses without data (for example if all
     #    of the tweets in a hydration call are no longer available)
     #  - For most endpoints this will be a list of tweets if present,
@@ -52,15 +60,15 @@
 
     if isinstance(tweet_or_tweets, list):
         tweets = tweet_or_tweets
     elif isinstance(tweet_or_tweets, dict):
         tweets = [tweet_or_tweets]
 
     for tweet in tweets:
-        add_mappings(mappings, mapping.map_tweet(tweet, True))
+        add_mappings(mappings, mapping.map_tweet(tweet, True, *page_info))
 
     logger.debug(f"About to write to {len(mappings)} tables")
     for table, table_mappings in mappings.items():
         if len(table_mappings) == 0:
             continue
         elif not isinstance(table_mappings, list):
             db.execute(mapping.sql_by_table[table]["insert"], table_mappings)
@@ -89,11 +97,11 @@
         logger.info(f"Loading {filename} into {db_name}")
 
         page_num = 0
         for page in json_fh:
             page_num = page_num + 1
             logger.info(f"Processing page {page_num} of {filename}")
             page_json = json.loads(page)
-            _load_page_object(page_json, connection)
+            _load_page_object(str(filename), page_json, connection)
 
         logger.info(f"All {page_num} pages of {filename} processed")
     return page_num
```

### Comparing `tidy_tweet-0.4.0/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0a1/src/tidy_tweet/tweet_mapping.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,233 @@
 from typing import Dict, List
-from tidy_tweet.utilities import add_mappings
+from tidy_tweet.utilities import add_mappings, clean_sql_statement
+from json import dumps
 from logging import getLogger
 
-
 logger = getLogger(__name__)
 
 
+try:
+    from tidy_tweet._version import version
+except ImportError:
+    version = "unspecified"
+    logger.warn(
+        "WARNING: cannot store tidy_tweet version in database as version could not "
+        "be fetched. If running tidy_tweet from source, try installing package in "
+        "editable mode."
+    )
+
+
 # --- SCHEMA VERSION ---
 # Update this every time the database schema is changed!
-SCHEMA_VERSION = "2022-03-10"
+SCHEMA_VERSION = "2022-05-22"
 
 
 sql_by_table: Dict[str, Dict[str, str]] = {}
-
+sql_views: Dict[str, str] = {}
 
 # --- Entities tables ---
 # URLs
-sql_by_table["url"] = {
+# URLs from tweets
+sql_by_table["tweet_url"] = {
     "create": """
-create table url (
-    source_id text, -- the id of the object (user or tweet) this URL is included in
-    source_type text, -- "user" or "tweet"
+create table tweet_url (
+    tweet_id text references tweet (id),
     field text not null, -- e.g. "description", "text" - which field of the source
                          -- object the URL is in
     url text not null, -- t.co shortened URL
     expanded_url text,
-    display_url text
+    display_url text,
+    primary key (tweet_id, url) on conflict ignore
 )
     """,
     "insert": """
-insert into url (
-    source_id, source_type, field,
+insert into tweet_url (
+    tweet_id, field,
     url, expanded_url, display_url
 ) values (
-    :source_id, :source_type, :field,
+    :source_id, :field,
+    :url, :expanded_url, :display_url
+)
+    """,
+}
+# URLs from user profiles
+sql_by_table["user_url"] = {
+    "create": """
+create table user_url (
+    user_id text references user (id),
+    field text not null, -- e.g. "description", "text" - which field of the source
+                         -- object the URL is in
+    url text not null, -- t.co shortened URL
+    expanded_url text,
+    display_url text,
+    primary key (user_id, url) on conflict ignore
+)
+    """,
+    "insert": """
+insert into user_url (
+    user_id, field,
+    url, expanded_url, display_url
+) values (
+    :source_id, :field,
     :url, :expanded_url, :display_url
 )
     """,
 }
 
 
 def map_urls(
     source_id: str, source_type: str, field: str, url_json_list: List[Dict]
 ) -> Dict[str, List[Dict]]:
-    url_maps = []
+    table_name = "tweet_url" if source_type == "tweet" else "user_url"
 
+    url_maps = []
     for url_json in url_json_list:
         url_maps.append(
             {
                 "source_id": source_id,
-                "source_type": source_type,
                 "field": field,
                 "url": url_json["url"],
                 # These fields are not guaranteed to be present - if a user
                 # copies and pastes a shortened url into a profile, it won't
                 # be expanded - eg https://twitter.com/SAHU_Finance
                 "expanded_url": url_json.get("expanded_url", None),
                 "display_url": url_json.get("display_url", None),
             }
         )
 
-    return {"url": url_maps}
+    return {table_name: url_maps}
 
 
 # Hashtags
-sql_by_table["hashtag"] = {
+# Hashtags from tweets
+sql_by_table["tweet_hashtag"] = {
+    "create": """
+create table tweet_hashtag (
+    tweet_id text references tweet (id),
+    field text not null, -- e.g. "description", "text" - which field of the source
+                         -- object the hashtag is in
+    hashtag text not null,
+    hashtag_lower text, -- Normalised, as hashtags are case-insensitive on Twitter
+    primary key (tweet_id, hashtag) on conflict ignore
+)
+    """,
+    "insert": """
+insert into tweet_hashtag (
+    tweet_id, field,
+    hashtag, hashtag_lower
+) values (
+    :source_id, :field,
+    :hashtag, :hashtag_lower
+)
+    """,
+}
+# Hashtags from user profiles
+sql_by_table["user_hashtag"] = {
     "create": """
-create table hashtag (
-    source_id text, -- the id of the object (user or tweet) this hashtag is included in
-    source_type text, -- "user" or "tweet"
+create table user_hashtag (
+    user_id text references user (id),
     field text not null, -- e.g. "description", "text" - which field of the source
                          -- object the hashtag is in
-    tag text not null
+    hashtag text not null,
+    hashtag_lower text, -- Normalised, as hashtags are case-insensitive on Twitter
+    primary key (user_id, hashtag) on conflict ignore
 )
     """,
     "insert": """
-insert into hashtag (
-    source_id, source_type, field,
-    tag
+insert into user_hashtag (
+    user_id, field,
+    hashtag, hashtag_lower
 ) values (
-    :source_id, :source_type, :field,
-    :tag
+    :source_id, :field,
+    :hashtag, :hashtag_lower
 )
     """,
 }
 
 
 def map_hashtags(
     source_id: str, source_type: str, field: str, tag_json_list: List[Dict]
 ) -> Dict[str, List[Dict]]:
+    table_name = "tweet_hashtag" if source_type == "tweet" else "user_hashtag"
+
     tag_mappings = [
         {
             "source_id": source_id,
-            "source_type": source_type,
             "field": field,
-            "tag": t["tag"],
+            "hashtag": t["tag"],
+            # Note that lower() could be done in SQLite by making hashtag_lower a
+            # generated column, however the SQLite lower() only handles ASCII while
+            # the python str.lower() handles Unicode
+            "hashtag_lower": t["tag"].lower(),
         }
         for t in tag_json_list
     ]
-    return {"hashtag": tag_mappings}
+    return {table_name: tag_mappings}
 
 
 # Mentions
-sql_by_table["mention"] = {
+# Mentions in tweets
+sql_by_table["tweet_mention"] = {
     "create": """
-create table mention (
-    source_id text, -- the id of the object (user or tweet) this mention is included in
-    source_type text, -- "user" or "tweet"
+create table tweet_mention (
+    tweet_id text references tweet (id),
     field text not null, -- e.g. "description", "text" - which field of the source
                          -- object the mention is in
-    username text not null -- username of mentioned user
+    username text not null, -- username of mentioned user
+    primary key (tweet_id, username) on conflict ignore
 )
     """,
     "insert": """
-insert into mention (
-    source_id, source_type, field,
+insert into tweet_mention (
+    tweet_id, field,
     username
 ) values (
-    :source_id, :source_type, :field,
+    :source_id, :field,
+    :username
+)
+    """,
+}
+# Mentions in user profiles
+sql_by_table["user_mention"] = {
+    "create": """
+create table user_mention (
+    user_id text references user (id),
+    field text not null, -- e.g. "description", "text" - which field of the source
+                         -- object the mention is in
+    username text not null, -- username of mentioned user
+    primary key (user_id, username) on conflict ignore
+)
+    """,
+    "insert": """
+insert into user_mention (
+    user_id, field,
+    username
+) values (
+    :source_id, :field,
     :username
 )
     """,
 }
 
 
 def map_mentions(
     source_id: str, source_type: str, field: str, mention_json_list: List[Dict]
 ) -> Dict[str, List[Dict]]:
+    table_name = "tweet_mention" if source_type == "tweet" else "user_mention"
+
     mention_mappings = [
         {
             "source_id": source_id,
-            "source_type": source_type,
             "field": field,
             "username": t["username"],
         }
         for t in mention_json_list
     ]
-    return {"mention": mention_mappings}
+    return {table_name: mention_mappings}
 
 
 # Entities objects
 def map_entities(source_id, source_type, field, entities_json) -> Dict[str, List[Dict]]:
     mappings = {}
 
     for entity_type, entity_data in entities_json.items():
@@ -172,15 +259,15 @@
     duration_ms integer,
     view_count integer,
     alt_text string,
     media_key text primary key
 )
     """,
     "insert": """
-insert or ignore into media (
+insert or replace into media (
     media_key, url, type,
     height, width, preview_image_url, alt_text,
     duration_ms, view_count
 ) values (
     :media_key, :url, :type,
     :height, :width, :preview_image_url, :alt_text,
     :duration_ms, :view_count
@@ -219,23 +306,26 @@
 # TODO: Fields not included yet:
 # - public_metrics
 sql_by_table["user"] = {
     "create": """
 create table user (
     name text,
     profile_image_url text,
-    id text primary key,
+    id text,
     created_at text,
     protected text,
     description text,
     location text,
     pinned_tweet_id text,
     verified integer, -- boolean
     url text,
-    username text
+    username text,
+    page_id integer references results_page (id),
+    source_file text references results_page (filename),
+    primary key (id, page_id)
 )
     """,
     "insert": """
 insert or ignore into user (
     id, username, name, url,
     profile_image_url, description,
     created_at,
@@ -250,27 +340,29 @@
     :location,
     :pinned_tweet_id
 )
     """,
 }
 
 
-def map_user(user_json) -> Dict[str, List[Dict]]:
+def map_user(user_json, source_file, page_id) -> Dict[str, List[Dict]]:
     user_map = {
         "id": user_json["id"],
         "username": user_json["username"],
         "name": user_json["name"],
         "url": user_json["url"],
         "profile_image_url": user_json["profile_image_url"],
         "description": user_json.get("description", None),
         "created_at": user_json["created_at"],
         "protected": user_json["protected"],
         "verified": user_json["verified"],
         "location": user_json.get("location", None),
         "pinned_tweet_id": user_json.get("pinned_tweet_id", None),
+        "source_file": source_file,
+        "page_id": page_id,
     }
 
     mappings = {"user": [user_map]}
 
     # Entities
     if "entities" in user_json:
         for field, entities in user_json["entities"].items():
@@ -285,15 +377,16 @@
 # TODO: fields not yet included:
 # - entities
 # - context_annotations
 
 sql_by_table["tweet"] = {
     "create": """
 create table tweet (
-    id text primary key,
+    id text,
+    page_id integer references results_page (id),
     reply_settings text,
     conversation_id text,
     created_at text,
     retweeted_tweet_id text references tweet (id),
     quoted_tweet_id text references tweet (id),
     replied_to_tweet_id text references tweet (id),
     in_reply_to_user_id text references user (id),
@@ -302,48 +395,52 @@
     lang text,
     source text,
     possibly_sensitive integer, -- boolean
     like_count integer,
     quote_count integer,
     reply_count integer,
     retweet_count integer,
-    directly_collected integer -- boolean
+    source_file text references results_page (filename),
+    directly_collected integer, -- boolean
+    primary key (id, page_id)
 )
     """,
     "insert": """
 insert or ignore into tweet (
     id, author_id,
     text, lang, source,
     possibly_sensitive, reply_settings,
     created_at,
     conversation_id,
     retweeted_tweet_id,
     quoted_tweet_id,
     replied_to_tweet_id,
     in_reply_to_user_id,
     like_count, quote_count, reply_count, retweet_count,
-    directly_collected
+    directly_collected, source_file, page_id
 ) values (
     :id, :author_id,
     :text, :lang, :source,
     :possibly_sensitive, :reply_settings,
     :created_at,
     :conversation_id,
     :retweeted_tweet_id,
     :quoted_tweet_id,
     :replied_to_tweet_id,
     :in_reply_to_user_id,
     :like_count, :quote_count, :reply_count, :retweet_count,
-    :directly_collected
+    :directly_collected, :source_file, :page_id
 )
     """,
 }
 
 
-def map_tweet(tweet_json, directly_collected: bool) -> Dict[str, List[Dict]]:
+def map_tweet(
+    tweet_json, directly_collected: bool, source_file: str, page_id
+) -> Dict[str, List[Dict]]:
     tweet_map = {
         "id": tweet_json["id"],
         "author_id": tweet_json["author_id"],
         "text": tweet_json["text"],
         "lang": tweet_json["lang"],
         "source": tweet_json.get("source", None),
         "possibly_sensitive": tweet_json["possibly_sensitive"],
@@ -352,14 +449,16 @@
         "conversation_id": tweet_json["conversation_id"],
         "in_reply_to_user_id": None,
         "like_count": tweet_json["public_metrics"]["like_count"],
         "quote_count": tweet_json["public_metrics"]["quote_count"],
         "reply_count": tweet_json["public_metrics"]["reply_count"],
         "retweet_count": tweet_json["public_metrics"]["retweet_count"],
         "directly_collected": directly_collected,
+        "source_file": source_file,
+        "page_id": page_id,
     }
 
     if "in_reply_to_user_id" in tweet_json:
         tweet_map["in_reply_to_user_id"] = tweet_json["in_reply_to_user_id"]
 
     # A tweet can have no more than one referenced tweet per type, but may have
     # multiple references of different types.
@@ -389,75 +488,103 @@
             map_entities(tweet_json["id"], "tweet", "text", tweet_json["entities"]),
         )
 
     return mappings
 
 
 # --- Metadata ---
-
-sql_by_table["_metadata"] = {
+# --- Results files
+sql_by_table["results_page"] = {
     "create": """
-create table _metadata (
-    metadata_key text, --primary key on conflict fail,
-    metadata_value text
+create table results_page (
+    id integer primary key,
+    file_name text,
+    oldest_id text,  -- oldest tweet id in page
+    newest_id text,  -- newest tweet id in page
+    result_count text,  -- count given in API response
+    inserted_at text default current_timestamp,
+    twarc_version text,
+    tidy_tweet_version text,
+    retrieved_at text, -- time response from twitter was recorded
+    request_url text,
+    additional_metadata text -- extra metadata from twarc and twitter
 )
     """,
     "insert": """
-insert into _metadata (metadata_key, metadata_value)
-    values (:metadata_key, :metadata_value)
+insert into results_page (
+    file_name,
+    oldest_id, newest_id, result_count,
+    retrieved_at, request_url,
+    twarc_version, tidy_tweet_version,
+    additional_metadata
+) values (
+    :file_name,
+    :oldest_id, :newest_id, :result_count,
+    :retrieved_at, :request_url,
+    :twarc_version, :tidy_tweet_version,
+    :additional_metadata
+)
     """,
 }
+sql_views[
+    "results_file"
+] = """
+create view results_file as
+select
+    file_name,
+    min(oldest_id) as oldest_id,  -- oldest tweet id in file
+    max(newest_id) as newest_id,  -- newest tweet id in file
+    sum(result_count) as result_count,  -- count given in API response
+    -- (sum of all page result counts)
+    max(inserted_at) as inserted_at,
+    twarc_version,
+    min(retrieved_at) as retrieved_at_min, -- earliest retrieval time for pages in file
+    max(retrieved_at) as retrieved_at_max -- latest retrieval time for pages in file
+from results_page
+group by file_name
+"""
+
+
+def map_page_metadata(
+    filename: str, page_metadata_json: Dict, twarc_metadata_json: Dict
+) -> Dict:
+    metadata = {"file_name": filename}
+
+    # Tidy tweet metadata
+    metadata["tidy_tweet_version"] = version
+
+    # Twitter result page metadata
+    key_columns = ["oldest_id", "newest_id", "result_count"]
+    for key in key_columns:
+        metadata[key] = page_metadata_json.pop(key, None)
+
+    # Twarc metadata
+    metadata["twarc_version"] = twarc_metadata_json.pop("version", None)
+    metadata["request_url"] = twarc_metadata_json.pop("url", None)
+    metadata["retrieved_at"] = twarc_metadata_json.pop("retrieved_at")
+
+    # Any unexpected items in either metadata should be retained
+    extras = {}
+
+    if len(page_metadata_json) > 0:
+        extras["twarc"] = page_metadata_json
 
+    if len(twarc_metadata_json) > 0:
+        extras["twarc"] = twarc_metadata_json
 
-def map_twarc_metadata(twarc_metadata_json) -> Dict[str, List[Dict]]:
-    # Rename the "version" key for clarity
-    twarc_metadata_json["twarc_version"] = twarc_metadata_json.pop("version")
-    return {
-        "_metadata": [
-            {"metadata_key": k, "metadata_value": v}
-            for k, v in twarc_metadata_json.items()
-        ]
-    }
-
-
-def map_tidy_tweet_metadata() -> Dict[str, List[Dict]]:
-    try:
-        from tidy_tweet._version import version
-    except ImportError:
-        version = "unspecified"
-        logger.warn(
-            "WARNING: cannot store tidy_tweet version in database as version could not "
-            "be fetched. If running tidy_tweet from source, try installing package in "
-            "editable mode."
-        )
+    metadata["additional_metadata"] = dumps(extras)
 
-    # TODO: how to handle db with additions of files with different library versions?
-    return {
-        "_metadata": [
-            {"metadata_key": "schema_version", "metadata_value": SCHEMA_VERSION},
-            {"metadata_key": "tidy_tweet_version", "metadata_value": version},
-        ]
-    }
+    return metadata
 
 
 # --- Validation ---
 
 # We have both create and assert statements for all tables
 for table_sql in sql_by_table.values():
     assert {"create", "insert"} <= table_sql.keys()
 
 
 # --- Convenience lists ---
-def clean_sql_statement(original: str) -> str:
-    """
-    Cleans up SQL statements so that they end with a semicolon and don't have any
-    leading or trailing whitespace
-    """
-    clean = original.strip()
-    if not clean.endswith(";"):
-        clean = clean + ";"
-    return clean
-
 
 create_table_statements = [
     clean_sql_statement(tbl["create"]) for tbl in sql_by_table.values()
 ]
```

### Comparing `tidy_tweet-0.4.0/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 0.4.0
+Version: 1.0.0a1
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -61,15 +61,15 @@
 page object, and no commas between top-level objects.
 
 ### Output: Sqlite database of tweets and metadata
 
 After processing your Twitter results pages with tidy_tweet (see [Usage](#usage)), you will have an 
 [SQLite][sqlite] database file at the location you specified.
 
-Database schema will be published here as soon as the initial schema is finalised.
+See the [current database schema](docs/schema.md).
 
 ## Prerequisites
 
 - Python 3.8+
 - A command line shell/terminal, such as bash, Mac Terminal, Git Bash, Anaconda Prompt, etc
 
 This tool requires Python 3.8 or later, the instructions assume you already have Python installed. If you haven't
```

### Comparing `tidy_tweet-0.4.0/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 contributing.md
+generate_schema_diagram.py
 noxfile.py
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/pypi_publish.yml
 .github/workflows/tests.yml
+docs/data_model.drawio
+docs/data_model.svg
+docs/schema.md
 src/tidy_tweet/__init__.py
 src/tidy_tweet/__main__.py
 src/tidy_tweet/_version.py
 src/tidy_tweet/database.py
 src/tidy_tweet/processing.py
 src/tidy_tweet/tweet_mapping.py
 src/tidy_tweet/utilities.py
```

### Comparing `tidy_tweet-0.4.0/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0a1/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-0.4.0/tests/test_cli.py` & `tidy_tweet-1.0.0a1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-0.4.0/tests/test_overall.py` & `tidy_tweet-1.0.0a1/tests/test_overall.py`

 * *Files identical despite different names*

