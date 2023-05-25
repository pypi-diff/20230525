# Comparing `tmp/vector_vault-1.1.1.tar.gz` & `tmp/vector_vault-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.1.1.tar", last modified: Thu May 25 00:58:10 2023, max compression
+gzip compressed data, was "vector_vault-1.1.2.tar", last modified: Thu May 25 05:58:25 2023, max compression
```

## Comparing `vector_vault-1.1.1.tar` & `vector_vault-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 00:58:10.965165 vector_vault-1.1.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.1.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    15143 2023-05-25 00:58:10.964930 vector_vault-1.1.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    14418 2023-05-25 00:56:42.000000 vector_vault-1.1.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-25 00:58:10.965318 vector_vault-1.1.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-25 00:58:05.000000 vector_vault-1.1.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 00:58:10.954732 vector_vault-1.1.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    15143 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-25 00:58:10.000000 vector_vault-1.1.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 00:58:10.964361 vector_vault-1.1.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.1.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.1.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 23:04:10.000000 vector_vault-1.1.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.1.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.1.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.1.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.1.1/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17569 2023-05-24 23:04:02.000000 vector_vault-1.1.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.1.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 05:58:25.481999 vector_vault-1.1.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.1.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    15801 2023-05-25 05:58:25.481813 vector_vault-1.1.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    15076 2023-05-25 03:57:49.000000 vector_vault-1.1.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-25 05:58:25.482035 vector_vault-1.1.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-25 05:56:14.000000 vector_vault-1.1.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 05:58:25.478866 vector_vault-1.1.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    15801 2023-05-25 05:58:25.000000 vector_vault-1.1.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-25 05:58:25.000000 vector_vault-1.1.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-25 05:58:25.000000 vector_vault-1.1.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-25 05:58:25.000000 vector_vault-1.1.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-25 05:58:25.000000 vector_vault-1.1.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 05:58:25.481394 vector_vault-1.1.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.1.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.1.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 23:04:10.000000 vector_vault-1.1.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.1.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.1.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.1.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.1.2/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17695 2023-05-25 05:58:14.000000 vector_vault-1.1.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.1.2/vectorvault/wrap.py
```

### Comparing `vector_vault-1.1.1/LICENSE` & `vector_vault-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/PKG-INFO` & `vector_vault-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,45 @@
-Metadata-Version: 2.1
-Name: vector_vault
-Version: 1.1.1
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
 
-Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
+Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
-Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
+By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
-This python library allows you to interact with Vector Vault using its Python-based API. Each vault is a seperate vector database. The `vectorvault` package includes operations such as creating a vault, deleting a vault, adding data to a vault, getting vector embeddings for data, saving data with embeddings to the cloud, referencing cloud vault data, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses by automatically integrating referenced vault data as context.
+The `vectorvault` package allows you to interact with your Cloud Vaults using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
 
 <br>
 
-# Interact with your Vault:
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
-</p>
+Basic Interactions:
 
-`add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
-<br>
-`add_item` : Add item to the Vault
+`add()` : Prepares data to be added to the Vault, with automatic text splitting and processing for long texts. 
 <br>
-`add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
+`get_vectors()` : Retrieves vectors embeddings for all prepared data 
 <br>
-`save` : Saves the vectors embeddings and data to the Cloud Vault along with any metadata
+`save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
-`delete` : Deletes the current Vault and all contents
+`delete()` : Deletes the current Vault and all contents
 <br>
-`get_vaults` : Retrieves a list of vaults in the current vault 
+`get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar` : Retrieves similar texts from the vault for a given input text, default = 4 items returned
+`get_similar()` : Retrieves similar texts from the Vault for a given input text 
 <br>
-`get_vectors` : Retrieves vectors embeddings for all data that was added to the Vault
-<br>
-`get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
+`get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
+
+>> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-## Basic usage:
+# Interact with your Vault:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
+</p>
+
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
 ### Get Your Vector Vault API Key:
@@ -75,18 +55,18 @@
 # Use Vector Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
-1. Create a Vault instance - (a new vault will be created if name does not exist)
+1. Create a Vault instance - (new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
-4. Get vectors embeddings - (Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time)
+4. Get vectors embeddings 
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
 vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
 
@@ -208,22 +188,23 @@
 answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
-# Change Vault
+# Change Vaults
+
 In this example science vault, we will print a list of vaults in the current vault directory
 ```
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
 ```
->> ['biology', 'physics', 'chemistry']
+>> Output: ['biology', 'physics', 'chemistry']
 
 
 
 ## Access vaults within vaults
 
 - biology vault within science vault
 ```
@@ -234,15 +215,15 @@
 
 - chemistry vault within science vault
 ```
 chemistry_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry')
 
 print(chemistry_vault.get_vaults())
 ```
->> ['reactions', 'formulas', 'lab notes']
+>> Output: ['reactions', 'formulas', 'lab notes']
 
 
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
@@ -283,20 +264,36 @@
 print(vault_response['response'])
 
 # print context:
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 ```
+<br>
+<br>
 
 # Summarize Anything:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
+</p>
+
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
 ```
+<br>
+
+want to make a summary of a certain length?...
+```
+summary = vault.get_chat(text, summary=True)
+
+while len(summary) > 1000:
+    summary = vault.get_chat(summary, summary=True)
+```
+^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than a thousand characters of text. 
 
 <br>
 <br>
 <br>
 
 ## Real world usage:
 ```
@@ -311,15 +308,15 @@
 # show the context used to generate the answer
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 
 ```
 
->> Question: 
+>> Output: Question: 
 What is a token broker? 
  
 >>Answer: 
 A token broker is a service that generates downscoped access tokens for token
 consumers to access or modify specific resources...
 >>
 
@@ -346,15 +343,15 @@
 history = user_input + answer
 
 # Get response from Language model
 vault_response = vault.get_chat(user_input2, history=history, get_context=True)
 
 print("Question:", user_input2, "\n\nAnswer:", vault_response2)
 ```
->> Question: 
+>> Output: Question: 
 How do I use it? 
  
 >>Answer: 
 You can use it by...
 
 
 
@@ -384,30 +381,32 @@
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
-And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` function with `get_context=True`. The call `get_chat(text, get_context=True)` will take the customer's question, search the vault, find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
 question = 'customer question text string'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 
 That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
 
 
 <br>
 <br>
 
-If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
+If have any questions, leave a message/comment on github repo. 
+
+<br>
+
+Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
-
-
```

### Comparing `vector_vault-1.1.1/README.md` & `vector_vault-1.1.2/vector_vault.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,64 @@
+Metadata-Version: 2.1
+Name: vector-vault
+Version: 1.1.2
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
 
-Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
+Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
-Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
+By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
-This python library allows you to interact with Vector Vault using its Python-based API. Each vault is a seperate vector database. The `vectorvault` package includes operations such as creating a vault, deleting a vault, adding data to a vault, getting vector embeddings for data, saving data with embeddings to the cloud, referencing cloud vault data, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses by automatically integrating referenced vault data as context.
+The `vectorvault` package allows you to interact with your Cloud Vaults using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
 
 <br>
 
-# Interact with your Vault:
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
-</p>
+Basic Interactions:
 
-`add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
-<br>
-`add_item` : Add item to the Vault
+`add()` : Prepares data to be added to the Vault, with automatic text splitting and processing for long texts. 
 <br>
-`add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
+`get_vectors()` : Retrieves vectors embeddings for all prepared data 
 <br>
-`save` : Saves the vectors embeddings and data to the Cloud Vault along with any metadata
+`save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
-`delete` : Deletes the current Vault and all contents
+`delete()` : Deletes the current Vault and all contents
 <br>
-`get_vaults` : Retrieves a list of vaults in the current vault 
+`get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar` : Retrieves similar texts from the vault for a given input text, default = 4 items returned
+`get_similar()` : Retrieves similar texts from the Vault for a given input text 
 <br>
-`get_vectors` : Retrieves vectors embeddings for all data that was added to the Vault
-<br>
-`get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
+`get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
+
+>> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-## Basic usage:
+# Interact with your Vault:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
+</p>
+
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
 ### Get Your Vector Vault API Key:
@@ -56,18 +74,18 @@
 # Use Vector Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
-1. Create a Vault instance - (a new vault will be created if name does not exist)
+1. Create a Vault instance - (new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
-4. Get vectors embeddings - (Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time)
+4. Get vectors embeddings 
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
 vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
 
@@ -189,22 +207,23 @@
 answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
-# Change Vault
+# Change Vaults
+
 In this example science vault, we will print a list of vaults in the current vault directory
 ```
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
 ```
->> ['biology', 'physics', 'chemistry']
+>> Output: ['biology', 'physics', 'chemistry']
 
 
 
 ## Access vaults within vaults
 
 - biology vault within science vault
 ```
@@ -215,15 +234,15 @@
 
 - chemistry vault within science vault
 ```
 chemistry_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry')
 
 print(chemistry_vault.get_vaults())
 ```
->> ['reactions', 'formulas', 'lab notes']
+>> Output: ['reactions', 'formulas', 'lab notes']
 
 
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
@@ -264,20 +283,36 @@
 print(vault_response['response'])
 
 # print context:
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 ```
+<br>
+<br>
 
 # Summarize Anything:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
+</p>
+
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
 ```
+<br>
+
+want to make a summary of a certain length?...
+```
+summary = vault.get_chat(text, summary=True)
+
+while len(summary) > 1000:
+    summary = vault.get_chat(summary, summary=True)
+```
+^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than a thousand characters of text. 
 
 <br>
 <br>
 <br>
 
 ## Real world usage:
 ```
@@ -292,15 +327,15 @@
 # show the context used to generate the answer
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 
 ```
 
->> Question: 
+>> Output: Question: 
 What is a token broker? 
  
 >>Answer: 
 A token broker is a service that generates downscoped access tokens for token
 consumers to access or modify specific resources...
 >>
 
@@ -327,15 +362,15 @@
 history = user_input + answer
 
 # Get response from Language model
 vault_response = vault.get_chat(user_input2, history=history, get_context=True)
 
 print("Question:", user_input2, "\n\nAnswer:", vault_response2)
 ```
->> Question: 
+>> Output: Question: 
 How do I use it? 
  
 >>Answer: 
 You can use it by...
 
 
 
@@ -365,28 +400,34 @@
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
-And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` function with `get_context=True`. The call `get_chat(text, get_context=True)` will take the customer's question, search the vault, find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
 question = 'customer question text string'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 
 That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
 
 
 <br>
 <br>
 
-If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
+If have any questions, leave a message/comment on github repo. 
+
+<br>
+
+Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
+
+
```

### Comparing `vector_vault-1.1.1/setup.py` & `vector_vault-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.1.1",
+    version="1.1.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.1.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vector-vault
-Version: 1.1.1
+Name: vector_vault
+Version: 1.1.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -15,51 +15,50 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. Vector Vault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
+Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
-Vector Vault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
+By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
 
-This python library allows you to interact with Vector Vault using its Python-based API. Each vault is a seperate vector database. The `vectorvault` package includes operations such as creating a vault, deleting a vault, adding data to a vault, getting vector embeddings for data, saving data with embeddings to the cloud, referencing cloud vault data, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses by automatically integrating referenced vault data as context.
+The `vectorvault` package allows you to interact with your Cloud Vaults using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
 
 <br>
 
-# Interact with your Vault:
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
-</p>
+Basic Interactions:
 
-`add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
+`add()` : Prepares data to be added to the Vault, with automatic text splitting and processing for long texts. 
 <br>
-`add_item` : Add item to the Vault
+`get_vectors()` : Retrieves vectors embeddings for all prepared data 
 <br>
-`add_item_with_vector` : Add item to the Vault with vector provided - only accepts vectors of 1536 dimensions
+`save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
-`save` : Saves the vectors embeddings and data to the Cloud Vault along with any metadata
+`delete()` : Deletes the current Vault and all contents
 <br>
-`delete` : Deletes the current Vault and all contents
+`get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_vaults` : Retrieves a list of vaults in the current vault 
+`get_similar()` : Retrieves similar texts from the Vault for a given input text 
 <br>
-`get_similar` : Retrieves similar texts from the vault for a given input text, default = 4 items returned
-<br>
-`get_vectors` : Retrieves vectors embeddings for all data that was added to the Vault
-<br>
-`get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
+`get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
+
+>> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-## Basic usage:
+# Interact with your Vault:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
+</p>
+
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
 
 ### Get Your Vector Vault API Key:
@@ -75,18 +74,18 @@
 # Use Vector Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
-1. Create a Vault instance - (a new vault will be created if name does not exist)
+1. Create a Vault instance - (new vault will be created if name does not exist)
 2. Gather some text data we want to store
 3. Add the data to the Vault
-4. Get vectors embeddings - (Automatic rate limiting built in. Auto batched and concurrently processed for fastest possible embed time)
+4. Get vectors embeddings 
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
 vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
 
@@ -208,22 +207,23 @@
 answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
-# Change Vault
+# Change Vaults
+
 In this example science vault, we will print a list of vaults in the current vault directory
 ```
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
 ```
->> ['biology', 'physics', 'chemistry']
+>> Output: ['biology', 'physics', 'chemistry']
 
 
 
 ## Access vaults within vaults
 
 - biology vault within science vault
 ```
@@ -234,15 +234,15 @@
 
 - chemistry vault within science vault
 ```
 chemistry_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry')
 
 print(chemistry_vault.get_vaults())
 ```
->> ['reactions', 'formulas', 'lab notes']
+>> Output: ['reactions', 'formulas', 'lab notes']
 
 
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
@@ -283,20 +283,36 @@
 print(vault_response['response'])
 
 # print context:
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 ```
+<br>
+<br>
 
 # Summarize Anything:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
+</p>
+
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
 ```
+<br>
+
+want to make a summary of a certain length?...
+```
+summary = vault.get_chat(text, summary=True)
+
+while len(summary) > 1000:
+    summary = vault.get_chat(summary, summary=True)
+```
+^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than a thousand characters of text. 
 
 <br>
 <br>
 <br>
 
 ## Real world usage:
 ```
@@ -311,15 +327,15 @@
 # show the context used to generate the answer
 for item in vault_response['context']:
     print("\n\n", f"item {item['metadata']['name']}")
     print(item['data'])
 
 ```
 
->> Question: 
+>> Output: Question: 
 What is a token broker? 
  
 >>Answer: 
 A token broker is a service that generates downscoped access tokens for token
 consumers to access or modify specific resources...
 >>
 
@@ -346,15 +362,15 @@
 history = user_input + answer
 
 # Get response from Language model
 vault_response = vault.get_chat(user_input2, history=history, get_context=True)
 
 print("Question:", user_input2, "\n\nAnswer:", vault_response2)
 ```
->> Question: 
+>> Output: Question: 
 How do I use it? 
  
 >>Answer: 
 You can use it by...
 
 
 
@@ -384,29 +400,33 @@
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
-And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` function with `get_context=True`. The call `get_chat(text, get_context=True)` will take the customer's question, search the vault, find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
 question = 'customer question text string'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 
 That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
 
 
 <br>
 <br>
 
-If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
+If have any questions, leave a message/comment on github repo. 
+
+<br>
+
+Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
```

### Comparing `vector_vault-1.1.1/vectorvault/__init__.py` & `vector_vault-1.1.2/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/ai.py` & `vector_vault-1.1.2/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/cloudmanager.py` & `vector_vault-1.1.2/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/creds.py` & `vector_vault-1.1.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/download.py` & `vector_vault-1.1.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/itemize.py` & `vector_vault-1.1.2/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/signup.py` & `vector_vault-1.1.2/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.1/vectorvault/vault.py` & `vector_vault-1.1.2/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
 
 class Vault:
     def __init__(self, user: str, api_key: str, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.dims = dims
-        self.cloud_manager = CloudManager(user, api_key, self.vault)
+        try:
+            self.cloud_manager = CloudManager(user, api_key, self.vault)
+        except:
+            # user can still use the get_chat() function without an api key
+            pass
         self.x = 0
         self.x_checked = False
         self.verbose = verbose
         self.items = []
         self.last_time = None
         self.last_chat_time = None
         self.first_run = True
```

### Comparing `vector_vault-1.1.1/vectorvault/wrap.py` & `vector_vault-1.1.2/vectorvault/wrap.py`

 * *Files identical despite different names*

