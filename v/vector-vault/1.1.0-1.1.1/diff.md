# Comparing `tmp/vector_vault-1.1.0.tar.gz` & `tmp/vector_vault-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.1.0.tar", last modified: Wed May 24 23:10:34 2023, max compression
+gzip compressed data, was "vector_vault-1.1.1.tar", last modified: Thu May 25 00:58:10 2023, max compression
```

## Comparing `vector_vault-1.1.0.tar` & `vector_vault-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 23:10:34.750413 vector_vault-1.1.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.1.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    14614 2023-05-24 23:10:34.750230 vector_vault-1.1.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    13889 2023-05-24 23:07:07.000000 vector_vault-1.1.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 23:10:34.750451 vector_vault-1.1.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 22:40:00.000000 vector_vault-1.1.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 23:10:34.747226 vector_vault-1.1.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    14614 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 23:10:34.749892 vector_vault-1.1.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.1.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.1.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 23:04:10.000000 vector_vault-1.1.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.1.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.1.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.1.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.1.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17569 2023-05-24 23:04:02.000000 vector_vault-1.1.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.1.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 00:58:10.965165 vector_vault-1.1.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.1.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    15143 2023-05-25 00:58:10.964930 vector_vault-1.1.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    14418 2023-05-25 00:56:42.000000 vector_vault-1.1.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-25 00:58:10.965318 vector_vault-1.1.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-25 00:58:05.000000 vector_vault-1.1.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 00:58:10.954732 vector_vault-1.1.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    15143 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 00:58:10.964361 vector_vault-1.1.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.1.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.1.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 23:04:10.000000 vector_vault-1.1.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.1.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.1.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.1.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.1.1/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17569 2023-05-24 23:04:02.000000 vector_vault-1.1.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.1.1/vectorvault/wrap.py
```

### Comparing `vector_vault-1.1.0/LICENSE` & `vector_vault-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/PKG-INFO` & `vector_vault-1.1.1/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vector_vault
-Version: 1.1.0
+Name: vector-vault
+Version: 1.1.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -178,25 +178,28 @@
 vault.add(more_text_data, name='Lifestyle in LA')
 
 vault.get_vectors()
 
 vault.save()
 ```
 
-Find the name later:
+<br>
+
+To find the name later:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['metadata']['name'])
 ```
 
 <br>
+<br>
 
-## Use the `get_chat()` function to get a response from chatgpt
+### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
 Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
@@ -244,14 +247,17 @@
 lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 <br>
 <br>
 
 # `get_chat()`
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
+</p>
 Chat get response from OpenAI's ChatGPT. 
 Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
 Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
@@ -353,14 +359,17 @@
 
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
+</p>
 In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
```

### Comparing `vector_vault-1.1.0/README.md` & `vector_vault-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,25 +159,28 @@
 vault.add(more_text_data, name='Lifestyle in LA')
 
 vault.get_vectors()
 
 vault.save()
 ```
 
-Find the name later:
+<br>
+
+To find the name later:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['metadata']['name'])
 ```
 
 <br>
+<br>
 
-## Use the `get_chat()` function to get a response from chatgpt
+### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
 Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
@@ -225,14 +228,17 @@
 lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 <br>
 <br>
 
 # `get_chat()`
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
+</p>
 Chat get response from OpenAI's ChatGPT. 
 Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
 Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
@@ -334,14 +340,17 @@
 
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
+</p>
 In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
```

### Comparing `vector_vault-1.1.0/setup.py` & `vector_vault-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.1.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vector-vault
-Version: 1.1.0
+Name: vector_vault
+Version: 1.1.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -178,25 +178,28 @@
 vault.add(more_text_data, name='Lifestyle in LA')
 
 vault.get_vectors()
 
 vault.save()
 ```
 
-Find the name later:
+<br>
+
+To find the name later:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['metadata']['name'])
 ```
 
 <br>
+<br>
 
-## Use the `get_chat()` function to get a response from chatgpt
+### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
 Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
@@ -244,14 +247,17 @@
 lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 <br>
 <br>
 
 # `get_chat()`
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
+</p>
 Chat get response from OpenAI's ChatGPT. 
 Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
 Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
@@ -353,14 +359,17 @@
 
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
+</p>
 In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
```

### Comparing `vector_vault-1.1.0/vectorvault/__init__.py` & `vector_vault-1.1.1/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/ai.py` & `vector_vault-1.1.1/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/cloudmanager.py` & `vector_vault-1.1.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/creds.py` & `vector_vault-1.1.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/download.py` & `vector_vault-1.1.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/itemize.py` & `vector_vault-1.1.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/signup.py` & `vector_vault-1.1.1/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/vault.py` & `vector_vault-1.1.1/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.0/vectorvault/wrap.py` & `vector_vault-1.1.1/vectorvault/wrap.py`

 * *Files identical despite different names*

