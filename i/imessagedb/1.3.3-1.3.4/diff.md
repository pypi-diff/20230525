# Comparing `tmp/imessagedb-1.3.3.tar.gz` & `tmp/imessagedb-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.3.3.tar", max compression
+gzip compressed data, was "imessagedb-1.3.4.tar", max compression
```

## Comparing `imessagedb-1.3.3.tar` & `imessagedb-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-24 16:37:12.578633 imessagedb-1.3.3/LICENSE
--rw-r--r--   0        0        0     9175 2023-05-24 16:37:12.578633 imessagedb-1.3.3/README.md
--rw-r--r--   0        0        0     1309 2023-05-24 16:37:51.988357 imessagedb-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    12415 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3186 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2365 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/chat.py
--rw-r--r--   0        0        0     4100 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3300 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/default.ini
--rw-r--r--   0        0        0     1092 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/handle.py
--rw-r--r--   0        0        0     3760 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/handles.py
--rw-r--r--   0        0        0    24304 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/html.py
--rw-r--r--   0        0        0     4975 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/message.py
--rw-r--r--   0        0        0     6269 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/messages.py
--rw-r--r--   0        0        0     6655 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/text.py
--rw-r--r--   0        0        0      677 2023-05-24 16:37:12.590633 imessagedb-1.3.3/src/imessagedb/utils.py
--rw-r--r--   0        0        0     9881 1970-01-01 00:00:00.000000 imessagedb-1.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-25 14:27:25.168008 imessagedb-1.3.4/LICENSE
+-rw-r--r--   0        0        0     9251 2023-05-25 14:27:25.168008 imessagedb-1.3.4/README.md
+-rw-r--r--   0        0        0     1309 2023-05-25 14:27:58.251901 imessagedb-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    12623 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3186 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2365 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     4100 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3300 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/default.ini
+-rw-r--r--   0        0        0     1092 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     3760 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    24304 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/html.py
+-rw-r--r--   0        0        0     4975 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/message.py
+-rw-r--r--   0        0        0     6269 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     6655 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/text.py
+-rw-r--r--   0        0        0      677 2023-05-25 14:27:25.180008 imessagedb-1.3.4/src/imessagedb/utils.py
+-rw-r--r--   0        0        0     9957 1970-01-01 00:00:00.000000 imessagedb-1.3.4/PKG-INFO
```

### Comparing `imessagedb-1.3.3/LICENSE` & `imessagedb-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/README.md` & `imessagedb-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,17 @@
 *** Note that you can only have one of --handle or --name, not both ***
 
 **-c CONFIGFILE, --configfile CONFIGFILE** The location of the configuration file. If the 
 file does not exist, a default configuration file will be created there. If this option is 
 not provided, the default location is `~/.conf/iMessageDB.ini`.
 
 **-o OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY** The output directory where the 
-output and attachments go. If this option is not provided, the default location is `/tmp`. 
-The files will be `/tmp/NAME.html` and attachments will be in `/tmp/NAME_Attachments`.
+output and attachments go. If this option is not provided, the default location is your
+home directory. The files will be `~/NAME.html` and attachments will be in 
+`~/NAME_Attachments`.
 
 **--database DATABASE**  The database file to open. If this option is not provided it will
 default to `~/Library/Messages/chat.db`, which is where Apple puts it.
 
 **-m ME, --me ME** The name to use to refer to you in the output. If this option is not 
 provided it will default to `Me`.
 
@@ -144,17 +145,18 @@
 # Whether or not to copy the attachments into a different directory. This is needed for two reasons:
 #  1) The web browser does not have access to the directory that the attachments are stored, so it cannot display them
 #  2) Some of the attachments need to be converted in order to be viewed in the browser
 
 copy = True
 
 # The directory to put the output. The html file will go in {copy_directory}/{Person}.html,
-#   and the attachments will go in {copy_directory}/{Person}_Attachments
+#   and the attachments will go in {copy_directory}/{Person}_Attachments. If you specify HOME, then
+#   it will put it in your home directory
 
-copy directory = /tmp
+copy directory = HOME
 
 # If the file already exists in the destination directory it is not recopied, but that can be overridden by
 #  specifying 'force copy' as true
 
 force copy = False
 
 # 'Skip attachments' ignores attachments
```

### Comparing `imessagedb-1.3.3/pyproject.toml` & `imessagedb-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.3.3"
+version = "1.3.4"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.3.3/src/imessagedb/__init__.py` & `imessagedb-1.3.4/src/imessagedb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 # Whether or not to copy the attachments into a different directory. This is needed for two reasons:
 #  1) The web browser does not have access to the directory that the attachments are stored, so it cannot display them
 #  2) Some of the attachments need to be converted in order to be viewed in the browser
 
 copy = True
 
 # The directory to put the output. The html file will go in {copy_directory}/{Person}.html,
-#   and the attachments will go in {copy_directory}/{Person}_Attachments
+#   and the attachments will go in {copy_directory}/{Person}_Attachments. If you specify HOME, then
+#   it will put it in your home directory
 
-copy directory = /tmp
+copy directory = HOME
 
 # If the file already exists in the destination directory it is not recopied, but that can be overridden by
 #  specifying 'force copy' as true
 
 force copy = False
 
 # 'Skip attachments' ignores attachments
@@ -251,15 +252,17 @@
             else:
                 argument_parser.print_help(sys.stderr)
                 print("\n ** You must supply either a name or one or more handles")
                 exit(1)
 
             config.set(CONTROL, 'Person', person)
 
-        copy_directory = config[CONTROL].get('copy directory', fallback="/tmp")
+        copy_directory = config[CONTROL].get('copy directory', fallback=os.environ['HOME'])
+        if copy_directory == "HOME":
+            copy_directory = os.environ['HOME']
         attachment_directory = f"{copy_directory}/{safe_filename(person)}_attachments"
         config[CONTROL]['attachment directory'] = attachment_directory
 
         filename = f'{safe_filename(person)}.html'
         out = open(f"{copy_directory}/{filename}", 'w')
         try:
             os.mkdir(attachment_directory)
@@ -303,18 +306,19 @@
             exit(1)
 
         message_list = database.Messages('chat', title, chat_id=chat_id)
     else:
 
         message_list = database.Messages('person', person, numbers=numbers)
 
+    me = config.get('DISPLAY', 'me', fallback='Me')
     output_type = config[CONTROL].get('output type', fallback='html')
     if output_type == 'text':
-        database.TextOutput(args.me, message_list, output_file=out).print()
+        database.TextOutput(me, message_list, output_file=out).print()
     else:
-        database.HTMLOutput(args.me, message_list, output_file=out)
+        database.HTMLOutput(me, message_list, output_file=out)
 
     database.disconnect()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `imessagedb-1.3.3/src/imessagedb/attachment.py` & `imessagedb-1.3.4/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/attachments.py` & `imessagedb-1.3.4/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/chat.py` & `imessagedb-1.3.4/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/chats.py` & `imessagedb-1.3.4/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/db.py` & `imessagedb-1.3.4/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/default.ini` & `imessagedb-1.3.4/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/handle.py` & `imessagedb-1.3.4/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/handles.py` & `imessagedb-1.3.4/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/html.py` & `imessagedb-1.3.4/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/message.py` & `imessagedb-1.3.4/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/messages.py` & `imessagedb-1.3.4/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/text.py` & `imessagedb-1.3.4/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/src/imessagedb/utils.py` & `imessagedb-1.3.4/src/imessagedb/utils.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.3.3/PKG-INFO` & `imessagedb-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.3.3
+Version: 1.3.4
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -111,16 +111,17 @@
 *** Note that you can only have one of --handle or --name, not both ***
 
 **-c CONFIGFILE, --configfile CONFIGFILE** The location of the configuration file. If the 
 file does not exist, a default configuration file will be created there. If this option is 
 not provided, the default location is `~/.conf/iMessageDB.ini`.
 
 **-o OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY** The output directory where the 
-output and attachments go. If this option is not provided, the default location is `/tmp`. 
-The files will be `/tmp/NAME.html` and attachments will be in `/tmp/NAME_Attachments`.
+output and attachments go. If this option is not provided, the default location is your
+home directory. The files will be `~/NAME.html` and attachments will be in 
+`~/NAME_Attachments`.
 
 **--database DATABASE**  The database file to open. If this option is not provided it will
 default to `~/Library/Messages/chat.db`, which is where Apple puts it.
 
 **-m ME, --me ME** The name to use to refer to you in the output. If this option is not 
 provided it will default to `Me`.
 
@@ -164,17 +165,18 @@
 # Whether or not to copy the attachments into a different directory. This is needed for two reasons:
 #  1) The web browser does not have access to the directory that the attachments are stored, so it cannot display them
 #  2) Some of the attachments need to be converted in order to be viewed in the browser
 
 copy = True
 
 # The directory to put the output. The html file will go in {copy_directory}/{Person}.html,
-#   and the attachments will go in {copy_directory}/{Person}_Attachments
+#   and the attachments will go in {copy_directory}/{Person}_Attachments. If you specify HOME, then
+#   it will put it in your home directory
 
-copy directory = /tmp
+copy directory = HOME
 
 # If the file already exists in the destination directory it is not recopied, but that can be overridden by
 #  specifying 'force copy' as true
 
 force copy = False
 
 # 'Skip attachments' ignores attachments
```

