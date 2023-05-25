# Comparing `tmp/makenote-1.1-py3-none-any.whl.zip` & `tmp/makenote-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17309 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       20 b- defN 22-Dec-01 20:08 makenote/__init__.py
--rwxrwxr-x  2.0 unx     8199 b- defN 22-Dec-01 20:08 makenote-1.1.data/scripts/makenote
--rw-rw-r--  2.0 unx    35099 b- defN 22-Dec-01 20:08 makenote-1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3071 b- defN 22-Dec-01 20:08 makenote-1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Dec-01 20:08 makenote-1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Dec-01 20:08 makenote-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      547 b- defN 22-Dec-01 20:08 makenote-1.1.dist-info/RECORD
-7 files, 47037 bytes uncompressed, 16339 bytes compressed:  65.3%
+Zip file size: 17379 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-25 11:55 makenote/__init__.py
+-rwxrwxr-x  2.0 unx     8459 b- defN 23-May-25 11:57 makenote-1.2.data/scripts/makenote
+-rw-rw-r--  2.0 unx    35099 b- defN 23-May-25 11:57 makenote-1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3046 b- defN 23-May-25 11:57 makenote-1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 11:57 makenote-1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-25 11:57 makenote-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      547 b- defN 23-May-25 11:57 makenote-1.2.dist-info/RECORD
+7 files, 47272 bytes uncompressed, 16409 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: makenote/__init__.py
 Comment: 
 
-Filename: makenote-1.1.data/scripts/makenote
+Filename: makenote-1.2.data/scripts/makenote
 Comment: 
 
-Filename: makenote-1.1.dist-info/LICENSE
+Filename: makenote-1.2.dist-info/LICENSE
 Comment: 
 
-Filename: makenote-1.1.dist-info/METADATA
+Filename: makenote-1.2.dist-info/METADATA
 Comment: 
 
-Filename: makenote-1.1.dist-info/WHEEL
+Filename: makenote-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: makenote-1.1.dist-info/top_level.txt
+Filename: makenote-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: makenote-1.1.dist-info/RECORD
+Filename: makenote-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makenote/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1"
+__version__ = "1.2"
```

## Comparing `makenote-1.1.data/scripts/makenote` & `makenote-1.2.data/scripts/makenote`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!python
 import sys
 import os
 import sqlite3
 import datetime
 import argparse
-
+import shutil
 
 # default table name
 default_table_name = 'journals'
 
 # database file is stored here.
 diaryFileName = f'{os.getenv("HOME")}/.local/share/makenote/databases/diaryFile.db'
 
@@ -27,14 +27,16 @@
                     help="create table", default=None, metavar='TABLE_NAME')
 parser.add_argument("-l", '--list', dest='list_tables',
                     help="list tables", default=None, action="store_true")
 parser.add_argument("-t", "--table", dest="table_name", help="table for notes",
                     default=default_table_name)
 parser.add_argument("-m", "--merge",  help="merge two databases",
                     default=None, nargs=3, metavar=('FIRST','SECOND','OUTPUT'))
+parser.add_argument("-x", "--export",  help="export database into file",
+                    default=None, metavar='FILENAME')
 parser.add_argument("text",  help="text", default=None, nargs='*')
 
 args = parser.parse_args()
 
 def add_note(sqlite_cursor, table_name, note_text):
     
     date_and_time = datetime.datetime.now()
@@ -198,14 +200,17 @@
 
 if args.show:
     show_table(cur, args.show)
 elif args.list_tables:
     list_tables(cur)
 elif args.create_table:
     make_table(cur, args.create_table)
+elif args.export:
+    shutil.copy(diaryFileName, args.export)
+    print(f'exported to {os.path.realpath(args.export)}')
 elif args.merge:
     firstdb, seconddb, outdb = args.merge
     merge_databases_by_name(firstdb, seconddb, outdb)
 # elif args.default:
 #     default_table_name = args.default
 #     table_name = args.default
 else:
```

## Comparing `makenote-1.1.dist-info/LICENSE` & `makenote-1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `makenote-1.1.dist-info/METADATA` & `makenote-1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: makenote
-Version: 1.1
+Version: 1.2
 Summary: command line tool for quickly writing journals
 Home-page: https://github.com/ekm507/makenote
 Author: Erfan Kheirollahi
 Author-email: ekm507@gmail.com
 License: UNKNOWN
 Keywords: makenote
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
-Requires-Dist: pysqlite3
 
 [نسخه فارسی این سند](./fa.README.md)
 
 makenote
 ---
 
 a command line tool for making diary or journals.
```

