# Comparing `tmp/openAIInsight-0.0.7-py3-none-any.whl.zip` & `tmp/openAIInsight-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5636 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     9399 b- defN 23-May-23 06:50 openAIInsight/OpenAI_PineConeVector.py
--rw-rw-r--  2.0 unx       84 b- defN 23-May-23 10:16 openAIInsight/__init__.py
--rw-rw-r--  2.0 unx     3604 b- defN 23-May-23 10:15 openAIInsight/openAI.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-23 10:18 openAIInsight-0.0.7.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      609 b- defN 23-May-23 10:18 openAIInsight-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-23 10:18 openAIInsight-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-23 10:18 openAIInsight-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      674 b- defN 23-May-23 10:18 openAIInsight-0.0.7.dist-info/RECORD
-8 files, 15549 bytes uncompressed, 4448 bytes compressed:  71.4%
+Zip file size: 6033 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx    12218 b- defN 23-May-25 19:47 openAIInsight/OpenAI_PineConeVector.py
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-25 19:30 openAIInsight/__init__.py
+-rw-rw-r--  2.0 unx     3604 b- defN 23-May-25 19:30 openAIInsight/openAI.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      675 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/RECORD
+8 files, 18369 bytes uncompressed, 4845 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: openAIInsight/__init__.py
 Comment: 
 
 Filename: openAIInsight/openAI.py
 Comment: 
 
-Filename: openAIInsight-0.0.7.dist-info/LICENCE.txt
+Filename: openAIInsight-0.0.8.dist-info/LICENCE.txt
 Comment: 
 
-Filename: openAIInsight-0.0.7.dist-info/METADATA
+Filename: openAIInsight-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: openAIInsight-0.0.7.dist-info/WHEEL
+Filename: openAIInsight-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: openAIInsight-0.0.7.dist-info/top_level.txt
+Filename: openAIInsight-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: openAIInsight-0.0.7.dist-info/RECORD
+Filename: openAIInsight-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openAIInsight/OpenAI_PineConeVector.py

```diff
@@ -1,28 +1,30 @@
 import json
 import openai
 import pinecone
+import datetime
 import traceback
 import pandas as pd
 from flask import request
 import loggerutility as logger
 import commonutility as common
 from openai.embeddings_utils import get_embedding, get_embeddings, cosine_similarity
 
+
 class OpenAI_PineConeVector:
     
     index_name      =   "" 
     openAI_apiKey   =   "" 
     pineCone_apiKey =   "" 
     queryList       =   "" 
     dfJson          =   ""
     engineName      =   "text-embedding-ada-002" # Model that we want to use 
     dimensions      =   1536
     my_index        =   ""
-    trainingMethod  =   ""
+    enterpriseName  =   ""
 
     def trainData(self, pineCone_json):
         # When calling from process definition, we need to pass hard-coded openAI_apiKey & pineCone_apiKey.
         try:
             
             logger.log("inside PineConeVector class trainData()","0")
             
@@ -42,80 +44,90 @@
                 self.dfJson = pineCone_json["dfJson"]
                 logger.log(f"\ntrain_PineConeVector dfJson:::\t{self.dfJson} \t{type(self.dfJson)}","0")
             
             if "trainData" in pineCone_json and pineCone_json["trainData"] != None:
                 self.dfJson = pineCone_json["trainData"]
                 logger.log(f"\ntrain_PineConeVector trainData:::\t{self.trainData} \t{type(self.trainData)}","0")
 
+            if "enterprise" in pineCone_json and pineCone_json["enterprise"] != None:
+                self.enterpriseName = pineCone_json["enterprise"]
+                logger.log(f"\nPineConeVector class LookUpData() enterprise:::\t{self.enterpriseName} \t{type(self.enterpriseName)}","0")
+
             logger.log(f"\nPineConeVector class trainData() all Parameters:::  \n{locals()}\n","0")
             
-            if self.trainingMethod == "item" :
-                parsed_json = (json.loads( self.dfJson))
-                df = pd.DataFrame(parsed_json[1:])
-                logger.log(f"\ntrain_PineConeVector df befor col change:::\t{df.head()} \t{type(df)}","0")
-                df.columns = ['id', 'material_description', 'product', 'delivery_method', 'strength', 'size']
-                logger.log(f"\ntrain_PineConeVector df aster col name:::\t{df.head()} \t{type(df)}","0")
+            parsed_json = (json.loads( self.dfJson))
+            df = pd.DataFrame(parsed_json[1:])
+            
+            pinecone.init(api_key=self.pineCone_apiKey, environment='us-west4-gcp')
+            openai.api_key = self.openAI_apiKey                 
 
-                pinecone.init(api_key=self.pineCone_apiKey, environment='us-west4-gcp')
-                openai.api_key = self.openAI_apiKey                 
+            logger.log(f"Pinecone Available indexes List  :: \t {pinecone.list_indexes()}", "0")    
+            # Creating index
+            if self.index_name not in pinecone.list_indexes():
+                logger.log(f" '{self.index_name}' index not present. Creating New!!!", "0")
+                pinecone.create_index(name = self.index_name, dimension=self.dimensions, metric='cosine')
+            else:
+                logger.log(f" '{self.index_name}' index is present. Loading now!!!", "0")
+                self.my_index = pinecone.Index(index_name=self.index_name)
+                
+            logger.log(f"Pinecone Available indexes List  :: \t {pinecone.list_indexes()}", "0")    
 
-                # Creating index
-                if self.index_name not in pinecone.list_indexes():
-                    logger.log(f" '{self.index_name}' index not present. Creating New!!!", "0")
-                    pinecone.create_index(name = self.index_name, dimension=self.dimensions, metric='cosine')
-                else:
-                    logger.log(f" '{self.index_name}' index is present. Loading now!!!", "0")
-                    self.my_index = pinecone.Index(index_name=self.index_name)
-                    
-                logger.log(f"Pinecone Available indexes List  :: \t {pinecone.list_indexes()}", "0")    
-
-                df.columns = ['_'.join(column.lower().split(' ')) for column in df.columns]
-                df.fillna("N/A",inplace=True)
-                #Changing column names to lowercase and replacing nan values with a string placeholder
-                df.columns = ['_'.join(column.lower().split(' ')) for column in df.columns]
-                df.fillna("N/A",inplace=True)
+            df.columns = ['_'.join(column.lower().split(' ')) for column in df.columns]
+            df.fillna("N/A",inplace=True)
+            #Changing column names to lowercase and replacing nan values with a string placeholder
+            df.columns = ['_'.join(column.lower().split(' ')) for column in df.columns]
+            df.fillna("N/A",inplace=True)
+            
+            df['enterprise'] = self.enterpriseName
+            
+            if self.index_name == "item":
+                logger.log(f"\ntrain_PineConeVector df.head() line 84:: {df.head()},\n {df.head()}", "0")    
+                df.columns = ['id', 'material_description', 'product', 'delivery_method', 'strength', 'size', 'enterprise']
+                logger.log(f"\ntrain_PineConeVector df.head() line 86:: {df.head()},\n {df.head()}", "0")    
                 df['embedding'] = get_embeddings(df['material_description'].to_list(), engine=self.engineName)
-                logger.log(f"\ntrain_PineConeVector df.head() :: {df.head()},\n {df.head()}", "0")    
+                metadata = df[['material_description', 'product', 'delivery_method', 'strength', 'size', 'enterprise']].to_dict(orient='records')
+            
+            elif self.index_name == "document":
+                df['embedding'] = get_embeddings(df['description'].to_list(), engine=self.engineName)
+                metadata = df[['description','enterprise']].to_dict(orient='records')
 
-                metadata = df[['material_description', 'product', 'delivery_method', 'strength', 'size']].to_dict(orient='records')
-                upsert = list(zip(df.id, df.embedding, metadata))
-                _ = self.my_index.upsert(vectors=upsert)
-                logger.log(f"{self.my_index.describe_index_stats()}","0")
+            else:
+                logger.log(f"\n\n INVALID INDEX NAME ::: \t{self.index_name}\n", "0")    
+            
+            logger.log(f"\ntrain_PineConeVector df.head() line 96 :: {df.head()},\n {df.head()}", "0")    
+            upsert = list(zip(df['id'], df['embedding'], metadata))
+            _ = self.my_index.upsert(vectors=upsert)
+            logger.log(f"{self.my_index.describe_index_stats()}","0")
 
-                logger.log(f"\nOpenAI_PineConeVector class trainData:::\t{self.my_index}","0")
+            logger.log(f"\nOpenAI_PineConeVector class trainData:::\t{self.my_index}","0")
 
-                if self.my_index != "":
-                    return f" '{self.index_name}' Index Creation successful. "
-                else:
-                    return f" '{self.index_name}' Index Creation failed. "
+            if self.my_index != "":
+                return f" '{self.index_name}' Index Creation successful. "
+            else:
+                return f" '{self.index_name}' Index Creation failed. "
             
-            elif self.trainingMethod == "document":
-                pass
             
-            elif self.trainingMethod == "":
-                logger.log(f"\n\n Invalid trainingMethod passed:::\t{self.trainingMethod}", "0")
-
-                
-
         except Exception as e:
             logger.log(f"OpenAI_PineConeVector class trainData() Issue::: \n{e}","0")
             trace = traceback.format_exc()
             descr = str(e)
             errorXml = common.getErrorXml(descr, trace)
             logger.log(f'\n OpenAI_PineConeVector class trainData() errorXml::: \n{errorXml}', "0")
             raise str(errorXml)
 
     def getLookupData(self):               
         try:
+            
             logger.log("inside PineConeVector class LookUpData()","0")
-            logger.log(f"\nPineConeVector class trainData() all Parameters:::  \n{locals()}\n","0")
-            result   = []
-            id_list   = []
+            logger.log(f"\nPineConeVector class LookUpData() all Parameters:::  \n{locals()}\n","0")
+            result      = []
+            id_list     = []
+            finalResult = ""
             pineCone_json =  request.get_data('jsonData', None)
-            logger.log(f"\nPineConeVector class trainData() pineCone_json raw:::\t{pineCone_json} \t{type(pineCone_json)}","0")
+            logger.log(f"\nPineConeVector class LookUpData() pineCone_json raw:::\t{pineCone_json} \t{type(pineCone_json)}","0")
             pineCone_json = json.loads(pineCone_json[9:])
             logger.log(f"\nPineConeVector class trainData() pineCone_json:::\t{pineCone_json} \t{type(pineCone_json)}","0")
 
             if "openAI_apiKey" in pineCone_json and pineCone_json["openAI_apiKey"] != None:
                 self.openAI_apiKey = pineCone_json["openAI_apiKey"]          
                 logger.log(f"\nPineConeVector class LookUpData() openAI_apiKey:::\t{self.openAI_apiKey} \t{type(self.openAI_apiKey)}","0")
                 openai.api_key = self.openAI_apiKey                 
@@ -127,42 +139,65 @@
             if "index_name" in pineCone_json and pineCone_json["index_name"] != None:
                 self.index_name = pineCone_json["index_name"]
                 logger.log(f"\nPineConeVector class LookUpData() index_name:::\t{self.index_name} \t{type(self.index_name)}","0")
             
             if "queryList" in pineCone_json and pineCone_json["queryList"] != None:
                 self.queryList = pineCone_json["queryList"]
                 logger.log(f"\nPineConeVector class LookUpData() queryList:::\t{self.queryList} \t{type(self.queryList)}","0")
+            
+            if "enterprise" in pineCone_json and pineCone_json["enterprise"] != None:
+                self.enterpriseName = pineCone_json["enterprise"]
+                logger.log(f"\nPineConeVector class LookUpData() enterprise:::\t{self.enterpriseName} \t{type(self.enterpriseName)}","0")
 
             openai.api_key  =  self.openAI_apiKey         
             pinecone.init(api_key=self.pineCone_apiKey, environment='us-west4-gcp')
             
             pinecone_IndexList = pinecone.list_indexes()
             
             if self.index_name in pinecone_IndexList:
                 self.my_index = pinecone.Index(index_name=self.index_name)
                 logger.log(f"self.my_index::: {self.my_index}","0")
-                for i in self.queryList:
-                    if i != "" and i != None:
-                        result.append(self.my_index.query(vector=get_embedding(i, engine=self.engineName),top_k=1, include_metadata=True))
-                logger.log(f"OpenAI_PineConeVector class getLookUP() Response::: \n{result}\tlen::: {len(result)}\t{type(result)}", "0")
-
-                id_list = [element["matches"][0]["id"] for element in result]
-                IdDescription_dict = dict(zip(self.queryList, id_list))
-                logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() IdDescription_dict::: \n{IdDescription_dict}\tlen::: {len(IdDescription_dict)}\t{type(IdDescription_dict)}", "0")
+                logger.log(f"Pinecone execution START Time::: {datetime.datetime.now().strftime('%H:%M:%S')}","0")
+                for query in self.queryList:
+                    if query != "" and query != None:
+                        if self.index_name == 'item':
+                            result.append(self.my_index.query(vector=get_embedding(query, engine=self.engineName),filter={"enterprise": self.enterpriseName},top_k=1, include_metadata=True))
+                        else:
+                            pineConeResponse = self.my_index.query(vector=get_embedding(query, engine=self.engineName),filter={"enterprise": self.enterpriseName},top_k=10, include_metadata=True)
+                            result.append(pineConeResponse)
 
-                return str(IdDescription_dict)
+                logger.log(f"Pinecone execution END Time::: {datetime.datetime.now().strftime('%H:%M:%S')}","0")
+                logger.log(f"OpenAI_PineConeVector class getLookUP() Response::: \n{result}\tlen::: {len(result)}\t{type(result)}", "0")
+                
+                # filtering response 
+                if len(result[0]['matches']) > 0:
+                    if self.index_name == 'item':
+                        id_list = [element["matches"][0]["id"] for element in result]
+                        IdDescription_dict = dict(zip(self.queryList, id_list))
+                        finalResult = IdDescription_dict
+                        logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() 'ITEM' Index IdDescription_dict::: \n{finalResult}\tlen::: {len(finalResult)}\t{type(finalResult)}", "0")
+                    else :
+                        logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() 'DOCUMENT' Index result::: \n{result}\tlen::: {len(result)}\t{type(result)}", "0")
+                        for query in self.queryList:
+                            for matchJson in result:
+                                # logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() 'DOCUMENT' Index matchJson::: \n{matchJson}\t{type(matchJson)}", "0")
+                                for j in matchJson['matches']:
+                                    # logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() 'DOCUMENT' Index j::: \n{j}\t{type(j)}", "0")
+                                    if j['score']  >= 0.75 and query in j['metadata']['description']:
+                                        id_list = [k['id'] for k in matchJson['matches']]
+                        logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() 'DOCUMENT' Index id_list::: \n{id_list}\t\t{type(id_list)}", "0")
+                        finalResult = id_list
+                    return str(finalResult)
             
             else:
                 logger.log(f"OpenAI_PineConeVector class getLookUP()::: \nIndex_Name: {self.index_name} not found in pinecone_IndexList: {pinecone_IndexList}","0")
                 message = f"Index_Name: '{self.index_name}' not found in pinecone_IndexList: {pinecone_IndexList}"
                 errorXml = common.getErrorXml(message, "")
                 raise Exception(errorXml)
             
         except Exception as e:
             logger.log(f"OpenAI_PineConeVector class getLookUP() Issue::: \n{e}","0")
             trace = traceback.format_exc()
             descr = str(e)
             errorXml = common.getErrorXml(descr, trace)
             logger.log(f'\n OpenAI_PineConeVector class getLookUP() errorXml::: \n{errorXml}', "0")
             raise str(errorXml)
-
-
```

## Comparing `openAIInsight-0.0.7.dist-info/LICENCE.txt` & `openAIInsight-0.0.8.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `openAIInsight-0.0.7.dist-info/METADATA` & `openAIInsight-0.0.8.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openAIInsight
-Version: 0.0.7
+Version: 0.0.8
 Summary: Proteus openAI File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

## Comparing `openAIInsight-0.0.7.dist-info/RECORD` & `openAIInsight-0.0.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-openAIInsight/OpenAI_PineConeVector.py,sha256=wpq7-kfFQJkTGAhUWzbAGNb94GSST8QuTkMYWfB2ugA,9399
+openAIInsight/OpenAI_PineConeVector.py,sha256=HVfh_sDvFDWie_TgZ7zaQczeTSLszcNod3Jpa0FHawc,12218
 openAIInsight/__init__.py,sha256=xXImeaMgVuR6qaRZ8E4zbB4_kbGg4h2wOUfe9O4vrMI,84
 openAIInsight/openAI.py,sha256=PW6yUTyYZodcqibHiqEQu3IYZwD4h6u__IPSecF531g,3604
-openAIInsight-0.0.7.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
-openAIInsight-0.0.7.dist-info/METADATA,sha256=5zP8UCS1veuQxHKPasyX4ybCkMyRLBt8iS6Zo6sietg,609
-openAIInsight-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-openAIInsight-0.0.7.dist-info/top_level.txt,sha256=YzsKehORjpmF7-8r3ivEG7yh7VoqXMt2TfYbfHovmfg,14
-openAIInsight-0.0.7.dist-info/RECORD,,
+openAIInsight-0.0.8.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
+openAIInsight-0.0.8.dist-info/METADATA,sha256=vSmATxBDWjnZy7bESs-ckk0QILh4e_zWAG6NiJczkQ0,609
+openAIInsight-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+openAIInsight-0.0.8.dist-info/top_level.txt,sha256=YzsKehORjpmF7-8r3ivEG7yh7VoqXMt2TfYbfHovmfg,14
+openAIInsight-0.0.8.dist-info/RECORD,,
```

