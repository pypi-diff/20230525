# Comparing `tmp/GoogleBard-1.0.3.tar.gz` & `tmp/GoogleBard-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.0.3.tar", last modified: Wed May 17 01:06:06 2023, max compression
+gzip compressed data, was "GoogleBard-1.1.0.tar", last modified: Thu May 25 06:50:17 2023, max compression
```

## Comparing `GoogleBard-1.0.3.tar` & `GoogleBard-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:06:06.226187 GoogleBard-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 01:05:40.000000 GoogleBard-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 01:06:06.226187 GoogleBard-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-17 01:05:40.000000 GoogleBard-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 01:06:06.226187 GoogleBard-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 01:05:40.000000 GoogleBard-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:06:06.222187 GoogleBard-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-17 01:05:40.000000 GoogleBard-1.0.3/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:06:06.226187 GoogleBard-1.0.3/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 01:06:06.000000 GoogleBard-1.0.3/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-17 01:06:06.000000 GoogleBard-1.0.3/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:06:06.000000 GoogleBard-1.0.3/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 01:06:06.000000 GoogleBard-1.0.3/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 01:06:06.000000 GoogleBard-1.0.3/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:50:17.771108 GoogleBard-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 06:49:54.000000 GoogleBard-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-25 06:50:17.771108 GoogleBard-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 06:49:54.000000 GoogleBard-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 06:50:17.771108 GoogleBard-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 06:49:54.000000 GoogleBard-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:50:17.771108 GoogleBard-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-25 06:49:54.000000 GoogleBard-1.1.0/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:50:17.771108 GoogleBard-1.1.0/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-25 06:50:17.000000 GoogleBard-1.1.0/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 06:50:17.000000 GoogleBard-1.1.0/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:50:17.000000 GoogleBard-1.1.0/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 06:50:17.000000 GoogleBard-1.1.0/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 06:50:17.000000 GoogleBard-1.1.0/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.0.3/LICENSE` & `GoogleBard-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.0.3/PKG-INFO` & `GoogleBard-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.0.3
+Version: 1.1.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.0.3/README.md` & `GoogleBard-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.0.3/setup.py` & `GoogleBard-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.0.3",
+    version="1.1.0",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.0.3/src/Bard.py` & `GoogleBard-1.1.0/src/Bard.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
-            "bl": "boq_assistant-bard-web-server_20230514.20_p0",
+            "bl": "boq_assistant-bard-web-server_20230523.13_p0",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
 
         # message arr -> data["f.req"]. Message is double json stringified
         message_struct = [
             [message],
@@ -132,21 +132,26 @@
             timeout=120,
         )
 
         chat_data = json.loads(resp.content.splitlines()[3])[0][2]
         if not chat_data:
             return {"content": f"Google Bard encountered an error: {resp.content}."}
         json_chat_data = json.loads(chat_data)
+        images = set()
+        if len(json_chat_data) >= 3:
+            for img in json_chat_data[4][0][4]:
+                images.add(img[0][0][0])
         results = {
             "content": json_chat_data[0][0],
             "conversation_id": json_chat_data[1][0],
             "response_id": json_chat_data[1][1],
             "factualityQueries": json_chat_data[3],
             "textQuery": json_chat_data[2][0] if json_chat_data[2] is not None else "",
             "choices": [{"id": i[0], "content": i[1]} for i in json_chat_data[4]],
+            "images": images,
         }
         self.conversation_id = results["conversation_id"]
         self.response_id = results["response_id"]
         self.choice_id = results["choices"][0]["id"]
         self._reqid += 100000
         return results
 
@@ -165,15 +170,17 @@
         session = os.getenv("BARD_SESSION")
         if not session:
             print("BARD_SESSION environment variable not set.")
             sys.exit(1)
         chatbot = Chatbot(session)
         # Join arguments into a single string
         MESSAGE = " ".join(sys.argv[1:])
-        console.print(Markdown(chatbot.ask(MESSAGE)["content"]))
+        response = chatbot.ask(MESSAGE)
+        console.print(Markdown((response["content"])))
+        console.print(response["images"] if response["images"] else "")
         sys.exit(0)
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--session",
         help="__Secure-1PSID cookie.",
         type=str,
         required=True,
@@ -195,10 +202,11 @@
                 chatbot.conversation_id = ""
                 chatbot.response_id = ""
                 chatbot.choice_id = ""
                 continue
             print("Google Bard:")
             response = chatbot.ask(user_prompt)
             console.print(Markdown(response["content"]))
+            console.print(response["images"] if response["images"] else "")
             print()
     except KeyboardInterrupt:
         print("Exiting...")
```

### Comparing `GoogleBard-1.0.3/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.1.0/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.0.3
+Version: 1.1.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

