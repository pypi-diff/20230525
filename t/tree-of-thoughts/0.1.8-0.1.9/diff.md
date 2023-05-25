# Comparing `tmp/tree-of-thoughts-0.1.8.tar.gz` & `tmp/tree-of-thoughts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.1.8.tar", last modified: Tue May 23 20:02:58 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.1.9.tar", last modified: Thu May 25 15:16:19 2023, max compression
```

## Comparing `tree-of-thoughts-0.1.8.tar` & `tree-of-thoughts-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:02:58.883048 tree-of-thoughts-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 20:02:45.000000 tree-of-thoughts-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 20:02:58.883048 tree-of-thoughts-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-05-23 20:02:45.000000 tree-of-thoughts-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:02:58.883048 tree-of-thoughts-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 20:02:45.000000 tree-of-thoughts-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:02:58.883048 tree-of-thoughts-0.1.8/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 20:02:46.000000 tree-of-thoughts-0.1.8/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-05-23 20:02:46.000000 tree-of-thoughts-0.1.8/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:02:58.883048 tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 20:02:58.000000 tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 20:02:58.000000 tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:02:58.000000 tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 20:02:58.000000 tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 20:02:58.000000 tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:16:19.594643 tree-of-thoughts-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 15:16:07.000000 tree-of-thoughts-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-25 15:16:19.594643 tree-of-thoughts-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-05-25 15:16:07.000000 tree-of-thoughts-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:16:19.594643 tree-of-thoughts-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-25 15:16:07.000000 tree-of-thoughts-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:16:19.594643 tree-of-thoughts-0.1.9/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 15:16:07.000000 tree-of-thoughts-0.1.9/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-05-25 15:16:07.000000 tree-of-thoughts-0.1.9/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:16:19.594643 tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-25 15:16:19.000000 tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 15:16:19.000000 tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:16:19.000000 tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 15:16:19.000000 tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 15:16:19.000000 tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.1.8/LICENSE` & `tree-of-thoughts-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.8/PKG-INFO` & `tree-of-thoughts-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.1.8/README.md` & `tree-of-thoughts-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,33 +21,35 @@
 Clone this repository with ```git clone https://github.com/kyegomez/tree-of-thoughts```
 
 or:
 
 ```pip install tree-of-thoughts ```
 
 
-Navigate to the repository folder: ``` cd tree-of-thoughts```
+Navigate to the repository folder: ```cd tree-of-thoughts```
 
 ```pip install openai```
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
 from tree_of_thoughts.treeofthoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts
 
 use_v2 = False
 api_key=""
 api_base= "" # leave it blank if you simply use default openai api url
 
 if not use_v2:
     #v1
-    model = OpenAILanguageModel(api_key=api_key, api_base=api_base)
+    model = OpenAILanguageModel(api_key=api_key, api_base=api_base # api_model="gpt4" # for higher performance base model is not smart
+    ) 
 else:
     #v2 parallel execution, caching, adaptive temperature
-    model = OptimizedOpenAILanguageModel(api_key=api_key, api_base=api_base)
+    model = OptimizedOpenAILanguageModel(api_key=api_key, api_base=api_base, # api_model="gpt4" # for higher performance base model is not smart
+    )
 
 #choose search algorithm('BFS' or 'DFS')
 search_algorithm = "BFS"
 
 #cot or propose
 strategy="cot"
 
@@ -57,23 +59,23 @@
 if not use_v2:
     #create an instance of the tree of thoughts class v1
     tree_of_thoughts = TreeofThoughts(model, search_algorithm)
 else:
     #or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts
     tree_of_thoughts= OptimizedTreeofThoughts(model, search_algorithm)
 
-input_problem = "use 4 numbers and basic arithmetic operations (+-*/) to obtain 24"
+input_problem = "use 4 numbers and basic arithmetic operations (+-*/) to obtain 24" #note for super intelligent responses you'll have to be more explicit in your prompt and select a better model
     
 k = 5
 T = 3
 b = 5
 vth = 0.5
 timeout = 10
 confidence = 1.0 #cmodel is confident on performance
-max_iterations = 40 #tree branh nodes 
+max_iterations = 40 #tree branch nodes 
 convergence_threshold = 0.01
 convergence_count = 5
 
 
 
 
 solution = tree_of_thoughts.solve(input_problem, k, T, b, vth, timeout, confidence_threshold=confidence, max_iterations=max_iterations, convergence_threshold=convergence_threshold, convergence_count=convergence_count)
```

### Comparing `tree-of-thoughts-0.1.8/setup.py` & `tree-of-thoughts-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.1.8',
+  version = '0.1.9',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.1.8/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.1.9/tree_of_thoughts/treeofthoughts.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         #implement the thought generation logic using self.model
         pass
 
     def evaluate_states(self, states):
         #implement state evaluation logic using self.model
         pass
 class OpenAILanguageModel(AbstractLanguageModel):
-    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=True):
+    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=False):
         if api_key == "" or api_key == None:
             api_key = os.environ.get("OPENAI_API_KEY", "")
         if api_key != "":
             openai.api_key = api_key
         else:
             raise Exception("Please provide OpenAI API key")
 
@@ -137,39 +137,39 @@
         return thoughts
 
     def evaluate_states(self, states):
         if self.evaluation_strategy == 'value':
             state_values = {}
             for state in states:
                 state_text = ' '.join(state)
-                prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1, and NOTHING ELSE:"
+                prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1, on the probability of this state of reasoning achieveing {prompt} and NOTHING ELSE:"
                 response = self.openai_api_call_handler(prompt, 10, 1)
                 try:
                     value_text = self.openai_choice2text_handler(response.choices[0])
                     value = float(value_text)
                     print(f"value: {value}")
                 except ValueError:
                     value = 0  # Assign a default value if the conversion fails
                 state_values[state] = value
             return state_values
 
         elif self.evaluation_strategy == 'vote':
             states_text = '\n'.join([' '.join(state) for state in states])
-            prompt = f"Given the following states of reasoning, vote for the best state:\n{states_text}\n\nVote, and NOTHING ELSE:"
+            prompt = f"Given the following states of reasoning, vote for the best state:\n{states_text}\n\nVote, on the probability of this state of reasoning achieveing {prompt} and NOTHING ELSE"
             response = self.openai_api_call_handler(prompt, 50, 1)
             best_state_text = self.openai_choice2text_handler(response.choices[0])
             print(f"Best state text: {best_state_text}")
             best_state = tuple(best_state_text.split())
             return {state: 1 if state == best_state else 0 for state in states}
 
         else:
             raise ValueError("Invalid evaluation strategy. Choose 'value' or 'vote'.")
 
 class OptimizedOpenAILanguageModel(OpenAILanguageModel):
-    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", cache_enabled=True, api_base="", api_model="", enable_ReAct_prompting=True):
+    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", cache_enabled=True, api_base="", api_model="", enable_ReAct_prompting=False):
         super().__init__(api_key, strategy, evaluation_strategy, api_base, api_model, enable_ReAct_prompting)
         self.cache_enabled = cache_enabled
         self.thought_cache = {}
         self.state_evaluation_cache = {}
 
     def parallel_generate_thoughts(self, states, k):
         with concurrent.futures.ThreadPoolExecutor() as executor:
@@ -180,28 +180,130 @@
     def parallel_evaluate_states(self, states):
         with concurrent.futures.ThreadPoolExecutor() as executor:
             state_values = list(executor.map(self.evaluate_states, states))
             print(f"Parallel evaluated state values: {state_values}")
         return state_values
     
 class GuidanceLanguageModel(AbstractLanguageModel):
-    def __init__(self, model, strategy="cot", evaluation_strategy="value"):
-        # guidance.llms.OpenAI("gpt-4")
+    def __init__(self, model, strategy="cot", evaluation_strategy="value", enable_ReAct_prompting=False):
+        # gpt4 = guidance.llms.OpenAI("gpt-4")
+        # vicuna = guidance.llms.transformers.Vicuna("your_path/vicuna_13B", device_map="auto")
         self.model = model
+        
+        # reference : https://www.promptingguide.ai/techniques/react
+        self.ReAct_prompt = ''
+        if enable_ReAct_prompting:
+            self.ReAct_prompt = '''{{#assistant~}}
+            {{gen 'Observation' temperature=0.5 max_tokens=50}}
+            {{~/assistant}}'''
+        
+        self.strategy = strategy
+        self.evaluation_strategy = evaluation_strategy
+        
+        self.thoughts_program = guidance('''
+            {{#system~}}
+            You are a logical and rational assistant.
+            {{~/system}}
+
+            {{#user~}}
+            Given the current state of reasoning:
+            {{state_text}}
+            Generate {{k}} coherent thoughts as short as possible to continue the reasoning process.
+            Don't answer the question yet.
+            {{~/user}}
+
+            %s
+            
+            {{#assistant~}}
+            {{gen 'Thoughts' temperature=0.5 max_tokens=50}}
+            {{~/assistant}}
+            ''' % self.ReAct_prompt, llm=self.model)
+        
+        self.value_program = guidance('''
+            {{#system~}}
+            You are a logical and rational assistant.
+            {{~/system}}
+
+            {{#user~}}
+            Given the current state of reasoning:
+            {{state_text}}
+            Evaluate its value as a float between 0 and 1, and NOTHING ELSE
+            Don't answer the question yet.
+            {{~/user}}
+
+            {{#assistant~}}
+            {{gen 'Value' temperature=1 max_tokens=10}}
+            {{~/assistant}}
+            ''', llm=self.model)
+        
+        self.vote_program = guidance('''
+            {{#system~}}
+            You are a logical and rational assistant.
+            {{~/system}}
+
+            {{#user~}}
+            Given the following states of reasoning, vote for the best state:
+            {{states_text}}
+            Give the index of your voted best state(the 1st state has index 0), and NOTHING ELSE
+            Don't answer the question yet.
+            {{~/user}}
+
+            {{#assistant~}}
+            {{gen 'Vote' temperature=1 max_tokens=10}}
+            {{~/assistant}}
+            ''', llm=self.model)
+        
+    def model_response_handler(self, program, **kargs):
+        print("Calling guidance model(Modify Me to handle specific LLM response excpetions!)")
+        reponse = program(**kargs)
+        return reponse
 
     def generate_thoughts(self, state, k):
         #implement the thought generation logic using self.model
-        pass
+        state_text = ' '.join(state)
+        
+        thoughts = []
+        for _ in range(k):
+            response = self.model_response_handler(self.thoughts_program, state_text=state_text, k=1)
+            text = response['Thoughts']
+            thoughts += [text]
+        # print(thoughts)
+        print(f"Generated thoughts: {thoughts}")
+        return thoughts
 
     def evaluate_states(self, states):
         #implement state evaluation logic using self.model
-        pass
+        if self.evaluation_strategy == 'value':
+            state_values = {}
+            for state in states:
+                state_text = ' '.join(state)
+                response = self.model_response_handler(self.value_program, state_text=state_text)
+                try:
+                    value_text = response['Value']
+                    print(f"Value text {value_text}")
+                    value = float(value_text)
+                    print(f"value: {value}")
+                except ValueError:
+                    value = 0  # Assign a default value if the conversion fails
+                state_values[state] = value
+            return state_values
+
+        elif self.evaluation_strategy == 'vote':
+            states_text = '\n'.join([' '.join(state) for state in states])
+            response = self.model_response_handler(self.vote_program, states_text=states_text)
+            best_state_text = response['Vote']
+            print(f"Best state text: {best_state_text}")
+            best_state = int(best_state_text)
+            return {state: 1 if i == best_state else 0 for i in range(len(states))}
+
+        else:
+            raise ValueError("Invalid evaluation strategy. Choose 'value' or 'vote'.")
 
 class GuidanceOpenAILanguageModel(GuidanceLanguageModel):
-    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model=""):
+    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=False):
         if api_key == "" or api_key == None:
             api_key = os.environ.get("OPENAI_API_KEY", "")
         if api_key != "":
             openai.api_key = api_key
         else:
             raise Exception("Please provide OpenAI API key")
 
@@ -215,16 +317,39 @@
         if api_model == "" or api_model == None:
             api_model = os.environ.get("OPENAI_API_MODEL", "")
         if api_model != "":
             self.api_model = api_model
         else:
             self.api_model = "text-davinci-003"
         print(f'Using api_model {self.api_model}')
+
+        super().__init__(guidance.llms.OpenAI(self.api_model), strategy, evaluation_strategy, enable_ReAct_prompting)
         
-        super.__init__(guidance.llms.OpenAI(self.api_model), strategy, evaluation_strategy)
+    
+    def model_response_handler(self, program, **kargs):
+        error_msg = ''
+        while True:
+            try:
+                program.llm.max_retries = 60
+                guidance.llms.OpenAI.cache.clear()
+                response = program(**kargs)
+                return response
+            except openai.error.RateLimitError as e:
+                sleep_duratoin = os.environ.get("OPENAI_RATE_TIMEOUT", 30)
+                print(f'{str(e)}, sleep for {sleep_duratoin}s, set it by env OPENAI_RATE_TIMEOUT')
+                time.sleep(sleep_duratoin)
+            except Exception as e:
+                if str(e) == f'''Too many (more than {guidance.llm.max_retries}) OpenAI API RateLimitError's in a row!''':
+                    sleep_duratoin = os.environ.get("OPENAI_RATE_TIMEOUT", 30)
+                    print(f'{str(e)}, sleep for {sleep_duratoin}s, set it by env OPENAI_RATE_TIMEOUT')
+                    time.sleep(sleep_duratoin)
+                else:
+                    error_msg = str(e)
+                    break
+        raise Exception(error_msg)
 
 class TreeofThoughts:
     """
     1. Thought Decomposition --> based on problem properties
 
     2. Thought Generator -> create a thought generator function G(p0, s, k) with 2 strategies a sample iid thoughts from a cot prompt b. propose thoughts
     sequentially using a propose prompt
@@ -254,15 +379,15 @@
     execute the chosen search algo with the input problem, thought generator, and state evaluator, and other required params
     """
 
     def __init__(self, model, search_algorithm):
         self.model = model
         self.search_algorithm = search_algorithm
 
-    def solve(self, x, k, T, b, vth, timeout=None):
+    def solve(self, x, k=None, T=None, b=None, vth=None, timeout=None, confidence_threshold=None, max_iterations=None, convergence_threshold=None, convergence_count=None):
         start_time = time.time()
         if self.search_algorithm == 'BFS':
             while timeout is None or time.time() - start_time < timeout:
                 result = self.tot_bfs(x, k, T, b)
                 if result:
                     return result
         elif self.search_algorithm == 'DFS':
@@ -394,8 +519,8 @@
     0.7
     ['By utilizing these methods, we can continue to advance large language models by improving their accuracy and performance. We can also use these methods to identify weaknesses in the models and make modifications to address them. Additionally, these methods can help us to develop']
     0.7
     0.7
     
     
     """
-    
+
```

### Comparing `tree-of-thoughts-0.1.8/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.1.9/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

