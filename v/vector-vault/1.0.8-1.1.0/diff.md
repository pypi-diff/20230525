# Comparing `tmp/vector_vault-1.0.8.tar.gz` & `tmp/vector_vault-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.0.8.tar", last modified: Wed May 24 21:06:30 2023, max compression
+gzip compressed data, was "vector_vault-1.1.0.tar", last modified: Wed May 24 23:10:34 2023, max compression
```

## Comparing `vector_vault-1.0.8.tar` & `vector_vault-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 21:06:30.496311 vector_vault-1.0.8/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.0.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    12741 2023-05-24 21:06:30.496146 vector_vault-1.0.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    12016 2023-05-24 21:06:05.000000 vector_vault-1.0.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 21:06:30.496348 vector_vault-1.0.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 21:06:09.000000 vector_vault-1.0.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 21:06:30.493083 vector_vault-1.0.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    12741 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 21:06:30.000000 vector_vault-1.0.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 21:06:30.495725 vector_vault-1.0.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.0.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6181 2023-05-24 19:11:23.000000 vector_vault-1.0.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 19:28:03.000000 vector_vault-1.0.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.0.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.0.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.0.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.0.8/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17637 2023-05-24 19:27:56.000000 vector_vault-1.0.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.0.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 23:10:34.750413 vector_vault-1.1.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.1.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    14614 2023-05-24 23:10:34.750230 vector_vault-1.1.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    13889 2023-05-24 23:07:07.000000 vector_vault-1.1.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-24 23:10:34.750451 vector_vault-1.1.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-24 22:40:00.000000 vector_vault-1.1.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 23:10:34.747226 vector_vault-1.1.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    14614 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-24 23:10:34.000000 vector_vault-1.1.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-24 23:10:34.749892 vector_vault-1.1.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.1.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.1.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 23:04:10.000000 vector_vault-1.1.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.1.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.1.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.1.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.1.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17569 2023-05-24 23:04:02.000000 vector_vault-1.1.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.1.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.0.8/LICENSE` & `vector_vault-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/PKG-INFO` & `vector_vault-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,104 +1,84 @@
-Metadata-Version: 2.1
-Name: vector_vault
-Version: 1.0.8
-Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
-Home-page: https://github.com/John-Rood/VectorVault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
-Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
+Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
+Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
-This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
+This python library allows you to interact with Vector Vault using its Python-based API. Each vault is a seperate vector database. The `vectorvault` package includes operations such as creating a vault, deleting a vault, adding data to a vault, getting vector embeddings for data, saving data with embeddings to the cloud, referencing cloud vault data, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses by automatically integrating referenced vault data as context.
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="500" height="500" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
 </p>
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
 `add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
 <br>
-`save` : Saves the vectors to the Vault and uploads any metadata
+`save` : Saves the vectors embeddings and data to the Cloud Vault along with any metadata
 <br>
-`delete` : Deletes the current Vault
+`delete` : Deletes the current Vault and all contents
 <br>
 `get_vaults` : Retrieves a list of vaults in the current vault 
 <br>
-`get_similar` : Retrieves similar vectors for a given input text
+`get_similar` : Retrieves similar texts from the vault for a given input text, default = 4 items returned
 <br>
-`get_vectors` : Retrieves the vectors for all items in the Vault
+`get_vectors` : Retrieves vectors embeddings for all data that was added to the Vault
 <br>
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 
 ## Basic usage:
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
-Get Your Vector Vault API Key:
+### Get Your Vector Vault API Key:
 ```
 from vectorvault import register
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
-
-# The api key will be sent to your email
 ```
+The api key will be sent to your email.
+
 <br>
 
 # Use Vector Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (a new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
-4. Get vectors embeddings
+4. Get vectors embeddings - (Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time)
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
 vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
 
-# Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time.
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 <br>
@@ -111,49 +91,94 @@
 
 vault.save()
 ```
 
 <br>
 <br>
 
-`vault.add()` is cool. You can add any length of text, even a full book...and it will be all automatically split and processed.
-`vault.get_vectors()` is also cool, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed
-
-
+`vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed.
+`vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
 ```
 vault.add(insanely_large_text_data)
 vault.get_vectors() 
 vault.save() 
 ```
-^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
+^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
+>> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 
 <br>
 <br>
 
 # Reference Your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="500" height="500" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 After you've added some data and want to reference it later, you can call it like this:
 ```
-similar_data = vault.get_similar(text_input) # returns a list with 4 results
+similar_data = vault.get_similar("Your text input") 
 
-# Print each similar item 
 for result in similar_data:
     print(result['data'])
 ```
-`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of the default of 4.
+^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
+`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of 4.
+
+<br>
+
+Print the metadata:
+```
+similar_data = vault.get_similar("Your text input") 
+
+for result in similar_data:
+    print(result['data'])
+    print(result['metadata'])
+```
+
+<br>
+
+To add meta data to your vault, just include it as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+```
+metadata = {
+    'name': 'Lifestyle in LA',
+    'country': 'United State',
+    'city': 'LA' 
+}
+
+vault.add(more_text_data, metadata)
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
+```
+vault.add(more_text_data, name='Lifestyle in LA')
 
+vault.get_vectors()
+
+vault.save()
+```
+
+Find the name later:
+```
+similar_data = vault.get_similar("Your text input") 
+
+for result in similar_data:
+    print(result['metadata']['name'])
+```
 
 <br>
 
 ## Use the `get_chat()` function to get a response from chatgpt
-The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
+Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
@@ -202,43 +227,43 @@
 
 <br>
 <br>
 
 # `get_chat()`
 Chat get response from OpenAI's ChatGPT. 
 Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
-Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
+Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
 - Example Chat: 
 `response = vault.get_chat(text, chat_history)`
 
 - Example Summary: 
 `summary = vault.get_chat(text, summary=True)`
 
 - Example Context-Based Response:
-`response = vault.get_chat(text, get_context = True)`
+`response = vault.get_chat(text, get_context=True)`
 
 - Example Context-Based Response w/ Chat History:
-`response = vault.get_chat(text, chat_history, get_context = True)`
+`response = vault.get_chat(text, chat_history, get_context=True)`
 
 - Example Context-Response with Context Samples Returned:
-`vault_response = vault.get_chat(text, get_context = True, return_context = True)`
+`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
 <br>
 
-Response is a string, unless `return_context = True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
+Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
 ```
 # print response:
-print(vault_response['response'])` 
+print(vault_response['response'])
 
 # print context:
-for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 ```
 
 # Summarize Anything:
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
@@ -255,16 +280,16 @@
 # Get response from Language model
 vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
 
 answer = vault_response['response']
 print("Question:", user_input, "\n\nAnswer:", answer)
 
 # show the context used to generate the answer
-for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 
 ```
 
 >> Question: 
 What is a token broker? 
  
@@ -349,12 +374,10 @@
 <br>
 <br>
 
 If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/8ba5c4eb-e880-426a-94e7-16c750e1bfe7/Looking+out+with+hope+vector+vault+small.png" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
-
-
```

### Comparing `vector_vault-1.0.8/README.md` & `vector_vault-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,103 @@
+Metadata-Version: 2.1
+Name: vector_vault
+Version: 1.1.0
+Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
-Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
+Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
+Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
-This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
+This python library allows you to interact with Vector Vault using its Python-based API. Each vault is a seperate vector database. The `vectorvault` package includes operations such as creating a vault, deleting a vault, adding data to a vault, getting vector embeddings for data, saving data with embeddings to the cloud, referencing cloud vault data, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses by automatically integrating referenced vault data as context.
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="500" height="500" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
 </p>
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
 `add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
 <br>
-`save` : Saves the vectors to the Vault and uploads any metadata
+`save` : Saves the vectors embeddings and data to the Cloud Vault along with any metadata
 <br>
-`delete` : Deletes the current Vault
+`delete` : Deletes the current Vault and all contents
 <br>
 `get_vaults` : Retrieves a list of vaults in the current vault 
 <br>
-`get_similar` : Retrieves similar vectors for a given input text
+`get_similar` : Retrieves similar texts from the vault for a given input text, default = 4 items returned
 <br>
-`get_vectors` : Retrieves the vectors for all items in the Vault
+`get_vectors` : Retrieves vectors embeddings for all data that was added to the Vault
 <br>
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 
 ## Basic usage:
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
-Get Your Vector Vault API Key:
+### Get Your Vector Vault API Key:
 ```
 from vectorvault import register
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
-
-# The api key will be sent to your email
 ```
+The api key will be sent to your email.
+
 <br>
 
 # Use Vector Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (a new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
-4. Get vectors embeddings
+4. Get vectors embeddings - (Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time)
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
 vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
 
-# Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time.
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 <br>
@@ -92,49 +110,94 @@
 
 vault.save()
 ```
 
 <br>
 <br>
 
-`vault.add()` is cool. You can add any length of text, even a full book...and it will be all automatically split and processed.
-`vault.get_vectors()` is also cool, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed
-
-
+`vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed.
+`vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
 ```
 vault.add(insanely_large_text_data)
 vault.get_vectors() 
 vault.save() 
 ```
-^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
+^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
+>> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 
 <br>
 <br>
 
 # Reference Your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="500" height="500" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 After you've added some data and want to reference it later, you can call it like this:
 ```
-similar_data = vault.get_similar(text_input) # returns a list with 4 results
+similar_data = vault.get_similar("Your text input") 
 
-# Print each similar item 
 for result in similar_data:
     print(result['data'])
 ```
-`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of the default of 4.
+^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
+`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of 4.
+
+<br>
+
+Print the metadata:
+```
+similar_data = vault.get_similar("Your text input") 
+
+for result in similar_data:
+    print(result['data'])
+    print(result['metadata'])
+```
+
+<br>
+
+To add meta data to your vault, just include it as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+```
+metadata = {
+    'name': 'Lifestyle in LA',
+    'country': 'United State',
+    'city': 'LA' 
+}
+
+vault.add(more_text_data, metadata)
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
+```
+vault.add(more_text_data, name='Lifestyle in LA')
 
+vault.get_vectors()
+
+vault.save()
+```
+
+Find the name later:
+```
+similar_data = vault.get_similar("Your text input") 
+
+for result in similar_data:
+    print(result['metadata']['name'])
+```
 
 <br>
 
 ## Use the `get_chat()` function to get a response from chatgpt
-The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
+Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
@@ -183,43 +246,43 @@
 
 <br>
 <br>
 
 # `get_chat()`
 Chat get response from OpenAI's ChatGPT. 
 Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
-Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
+Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
 - Example Chat: 
 `response = vault.get_chat(text, chat_history)`
 
 - Example Summary: 
 `summary = vault.get_chat(text, summary=True)`
 
 - Example Context-Based Response:
-`response = vault.get_chat(text, get_context = True)`
+`response = vault.get_chat(text, get_context=True)`
 
 - Example Context-Based Response w/ Chat History:
-`response = vault.get_chat(text, chat_history, get_context = True)`
+`response = vault.get_chat(text, chat_history, get_context=True)`
 
 - Example Context-Response with Context Samples Returned:
-`vault_response = vault.get_chat(text, get_context = True, return_context = True)`
+`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
 <br>
 
-Response is a string, unless `return_context = True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
+Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
 ```
 # print response:
-print(vault_response['response'])` 
+print(vault_response['response'])
 
 # print context:
-for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 ```
 
 # Summarize Anything:
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
@@ -236,16 +299,16 @@
 # Get response from Language model
 vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
 
 answer = vault_response['response']
 print("Question:", user_input, "\n\nAnswer:", answer)
 
 # show the context used to generate the answer
-for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 
 ```
 
 >> Question: 
 What is a token broker? 
  
@@ -330,10 +393,12 @@
 <br>
 <br>
 
 If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/8ba5c4eb-e880-426a-94e7-16c750e1bfe7/Looking+out+with+hope+vector+vault+small.png" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
+
+
```

### Comparing `vector_vault-1.0.8/setup.py` & `vector_vault-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.0.8",
+    version="1.1.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.0.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.1.0/vector_vault.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.0.8
+Version: 1.1.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -17,88 +17,87 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
-Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
+Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
+Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
-This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
+This python library allows you to interact with Vector Vault using its Python-based API. Each vault is a seperate vector database. The `vectorvault` package includes operations such as creating a vault, deleting a vault, adding data to a vault, getting vector embeddings for data, saving data with embeddings to the cloud, referencing cloud vault data, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses by automatically integrating referenced vault data as context.
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="500" height="500" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
 </p>
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
 `add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
 <br>
-`save` : Saves the vectors to the Vault and uploads any metadata
+`save` : Saves the vectors embeddings and data to the Cloud Vault along with any metadata
 <br>
-`delete` : Deletes the current Vault
+`delete` : Deletes the current Vault and all contents
 <br>
 `get_vaults` : Retrieves a list of vaults in the current vault 
 <br>
-`get_similar` : Retrieves similar vectors for a given input text
+`get_similar` : Retrieves similar texts from the vault for a given input text, default = 4 items returned
 <br>
-`get_vectors` : Retrieves the vectors for all items in the Vault
+`get_vectors` : Retrieves vectors embeddings for all data that was added to the Vault
 <br>
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 
 ## Basic usage:
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
-Get Your Vector Vault API Key:
+### Get Your Vector Vault API Key:
 ```
 from vectorvault import register
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
-
-# The api key will be sent to your email
 ```
+The api key will be sent to your email.
+
 <br>
 
 # Use Vector Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (a new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
-4. Get vectors embeddings
+4. Get vectors embeddings - (Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time)
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
 vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
 
-# Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time.
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 <br>
@@ -111,49 +110,94 @@
 
 vault.save()
 ```
 
 <br>
 <br>
 
-`vault.add()` is cool. You can add any length of text, even a full book...and it will be all automatically split and processed.
-`vault.get_vectors()` is also cool, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed
-
-
+`vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed.
+`vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
 ```
 vault.add(insanely_large_text_data)
 vault.get_vectors() 
 vault.save() 
 ```
-^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
+^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
+>> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 
 <br>
 <br>
 
 # Reference Your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="500" height="500" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 After you've added some data and want to reference it later, you can call it like this:
 ```
-similar_data = vault.get_similar(text_input) # returns a list with 4 results
+similar_data = vault.get_similar("Your text input") 
+
+for result in similar_data:
+    print(result['data'])
+```
+^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
+`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of 4.
+
+<br>
+
+Print the metadata:
+```
+similar_data = vault.get_similar("Your text input") 
 
-# Print each similar item 
 for result in similar_data:
     print(result['data'])
+    print(result['metadata'])
 ```
-`similar_data = vault.get_similar(text_input, n = 10)` returns 10 results instead of the default of 4.
 
+<br>
+
+To add meta data to your vault, just include it as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+```
+metadata = {
+    'name': 'Lifestyle in LA',
+    'country': 'United State',
+    'city': 'LA' 
+}
+
+vault.add(more_text_data, metadata)
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
+```
+vault.add(more_text_data, name='Lifestyle in LA')
+
+vault.get_vectors()
+
+vault.save()
+```
+
+Find the name later:
+```
+similar_data = vault.get_similar("Your text input") 
+
+for result in similar_data:
+    print(result['metadata']['name'])
+```
 
 <br>
 
 ## Use the `get_chat()` function to get a response from chatgpt
-The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
+Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
@@ -202,43 +246,43 @@
 
 <br>
 <br>
 
 # `get_chat()`
 Chat get response from OpenAI's ChatGPT. 
 Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
-Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
+Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
 - Example Chat: 
 `response = vault.get_chat(text, chat_history)`
 
 - Example Summary: 
 `summary = vault.get_chat(text, summary=True)`
 
 - Example Context-Based Response:
-`response = vault.get_chat(text, get_context = True)`
+`response = vault.get_chat(text, get_context=True)`
 
 - Example Context-Based Response w/ Chat History:
-`response = vault.get_chat(text, chat_history, get_context = True)`
+`response = vault.get_chat(text, chat_history, get_context=True)`
 
 - Example Context-Response with Context Samples Returned:
-`vault_response = vault.get_chat(text, get_context = True, return_context = True)`
+`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
 <br>
 
-Response is a string, unless `return_context = True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
+Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
 ```
 # print response:
-print(vault_response['response'])` 
+print(vault_response['response'])
 
 # print context:
-for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 ```
 
 # Summarize Anything:
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
@@ -255,16 +299,16 @@
 # Get response from Language model
 vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
 
 answer = vault_response['response']
 print("Question:", user_input, "\n\nAnswer:", answer)
 
 # show the context used to generate the answer
-for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 
 ```
 
 >> Question: 
 What is a token broker? 
  
@@ -349,12 +393,12 @@
 <br>
 <br>
 
 If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/8ba5c4eb-e880-426a-94e7-16c750e1bfe7/Looking+out+with+hope+vector+vault+small.png" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
```

### Comparing `vector_vault-1.0.8/vectorvault/__init__.py` & `vector_vault-1.1.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/vectorvault/ai.py` & `vector_vault-1.1.0/vectorvault/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
 
         if intokes + contokes + histokes > 4000:
             tokes_left = 4000 - intokes
             if len(history) > 1:
-                print('history is triggered')
                 tokes_left = 2000 - intokes 
                 char_left = tokes_left * 4
                 history = history[-char_left:]
                 tokes_left_after_hist = 4000 - self.get_tokens(user_input + history)
                 char_left_after_hist = tokes_left_after_hist * 4
                 context = context[-char_left_after_hist:]
                 double_check = self.get_tokens(user_input+history+context)
```

### Comparing `vector_vault-1.0.8/vectorvault/cloudmanager.py` & `vector_vault-1.1.0/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/vectorvault/creds.py` & `vector_vault-1.1.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/vectorvault/download.py` & `vector_vault-1.1.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/vectorvault/itemize.py` & `vector_vault-1.1.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/vectorvault/signup.py` & `vector_vault-1.1.0/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.0.8/vectorvault/vault.py` & `vector_vault-1.1.0/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,23 +161,18 @@
             # Retrieve the item
             item_data = self.cloud_manager.download_text_from_cloud(name(self.vault, vec, item=True))
             # Retrieve the metadata
             meta_data = self.cloud_manager.download_text_from_cloud(name(self.vault, vec, meta=True))
             meta = json.loads(meta_data)
             build_return(results, item_data, meta)
 
-        # Create a return dictionary
-        return_dict = {
-            "results": results
-        }
-
         if self.verbose == True:
             print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
 
-        return return_dict
+        return results
     
 
     def get_similar(self, text, n: int = 4):
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
         return self.get_items_by_vector(vector, n)
 
 
@@ -219,15 +214,15 @@
         """
         if self.x_checked == False:
             self.check_index()
         else: 
             pass
         start_time = time.time()
 
-        if len(text) > 36000:
+        if self.ai.get_tokens(text) > 4000:
             raise 'Text length too long. Use the "split_text() function to get a list of text segments'
 
         # Add vector to vectorspace
         self.vectors.add_item(self.x, vector)
         self.items.append(itemize(self.vault, self.x, meta, text, name))
 
         self.x += 1
@@ -411,21 +406,22 @@
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if include_context_meta:
-                            context = str(self.get_similar(user_input, n=n_context))
+                            context = self.get_similar(user_input, n=n_context)
+                            input = str(context)
                         else:
-                            contexts = self.get_similar(user_input, n=n_context)
-                            context = ''
-                            for text in contexts['results']:
-                                context += text['data']
-                        response = self.ai.llm_w_context(segment, context, history, model=model)
+                            context = self.get_similar(user_input, n=n_context)
+                            input = ''
+                            for text in context:
+                                input += text['data']
+                        response = self.ai.llm_w_context(segment, input, history, model=model)
                     else:
                         response = self.ai.llm(segment, history, model=model)
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 15 seconds")
                     time.sleep(15)
```

### Comparing `vector_vault-1.0.8/vectorvault/wrap.py` & `vector_vault-1.1.0/vectorvault/wrap.py`

 * *Files identical despite different names*

