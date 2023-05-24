# Comparing `tmp/surv_ai-0.1.8.tar.gz` & `tmp/surv_ai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surv_ai-0.1.8.tar", max compression
+gzip compressed data, was "surv_ai-0.1.9.tar", max compression
```

## Comparing `surv_ai-0.1.8.tar` & `surv_ai-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.8/LICENSE
--rw-r--r--   0        0        0    21368 2023-05-23 14:20:46.224165 surv_ai-0.1.8/README.md
--rw-r--r--   0        0        0     1447 2023-05-23 14:20:58.843859 surv_ai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.8/surv_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.8/surv_ai/core/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.8/surv_ai/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.8/surv_ai/core/agents/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.8/surv_ai/core/agents/binary.py
--rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.8/surv_ai/core/agents/reasoning.py
--rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.8/surv_ai/core/interfaces.py
--rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.8/surv_ai/core/model.py
--rw-r--r--   0        0        0     4722 2023-05-23 14:20:48.841757 surv_ai-0.1.8/surv_ai/core/survey.py
--rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.8/surv_ai/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.8/surv_ai/lib/conversation/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.8/surv_ai/lib/conversation/conversation.py
--rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.8/surv_ai/lib/conversation/interfaces.py
--rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.8/surv_ai/lib/knowledge_store/__init__.py
--rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.8/surv_ai/lib/knowledge_store/interfaces.py
--rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.8/surv_ai/lib/knowledge_store/local.py
--rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.8/surv_ai/lib/llm/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.8/surv_ai/lib/llm/anthropic.py
--rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.8/surv_ai/lib/llm/gpt.py
--rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.8/surv_ai/lib/llm/interfaces.py
--rw-r--r--   0        0        0     2005 2023-05-23 04:29:11.574974 surv_ai-0.1.8/surv_ai/lib/log.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.8/surv_ai/lib/tools/__init__.py
--rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.8/surv_ai/lib/tools/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.8/surv_ai/lib/tools/query/__init__.py
--rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.8/surv_ai/lib/tools/query/google_custom_search.py
--rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.8/surv_ai/lib/tools/query/interfaces.py
--rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.8/surv_ai/lib/tools/query/wikipedia.py
--rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.8/surv_ai/lib/tools/tool_belt.py
--rw-r--r--   0        0        0    22718 1970-01-01 00:00:00.000000 surv_ai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.9/LICENSE
+-rw-r--r--   0        0        0    21457 2023-05-24 16:07:15.155665 surv_ai-0.1.9/README.md
+-rw-r--r--   0        0        0     1449 2023-05-24 22:03:59.026252 surv_ai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.9/surv_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.9/surv_ai/core/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.9/surv_ai/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.9/surv_ai/core/agents/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.9/surv_ai/core/agents/binary.py
+-rw-r--r--   0        0        0     6959 2023-05-24 22:03:59.026585 surv_ai-0.1.9/surv_ai/core/agents/reasoning.py
+-rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.9/surv_ai/core/interfaces.py
+-rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.9/surv_ai/core/model.py
+-rw-r--r--   0        0        0     4800 2023-05-24 17:10:39.143388 surv_ai-0.1.9/surv_ai/core/survey.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.9/surv_ai/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.9/surv_ai/lib/conversation/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.9/surv_ai/lib/conversation/conversation.py
+-rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.9/surv_ai/lib/conversation/interfaces.py
+-rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.9/surv_ai/lib/knowledge_store/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.9/surv_ai/lib/knowledge_store/interfaces.py
+-rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.9/surv_ai/lib/knowledge_store/local.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.9/surv_ai/lib/llm/__init__.py
+-rw-r--r--   0        0        0     3926 2023-05-24 19:57:13.306950 surv_ai-0.1.9/surv_ai/lib/llm/anthropic.py
+-rw-r--r--   0        0        0     4427 2023-05-24 22:03:59.026889 surv_ai-0.1.9/surv_ai/lib/llm/gpt.py
+-rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.9/surv_ai/lib/llm/interfaces.py
+-rw-r--r--   0        0        0     2005 2023-05-24 03:24:35.670699 surv_ai-0.1.9/surv_ai/lib/log.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.9/surv_ai/lib/tools/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-24 15:30:01.272295 surv_ai-0.1.9/surv_ai/lib/tools/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.9/surv_ai/lib/tools/query/__init__.py
+-rw-r--r--   0        0        0     7697 2023-05-24 22:03:59.027208 surv_ai-0.1.9/surv_ai/lib/tools/query/google_custom_search.py
+-rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.9/surv_ai/lib/tools/query/interfaces.py
+-rw-r--r--   0        0        0     6326 2023-05-24 16:07:49.258939 surv_ai-0.1.9/surv_ai/lib/tools/query/wikipedia.py
+-rw-r--r--   0        0        0     3229 2023-05-24 16:07:49.215788 surv_ai-0.1.9/surv_ai/lib/tools/tool_belt.py
+-rw-r--r--   0        0        0    22809 1970-01-01 00:00:00.000000 surv_ai-0.1.9/PKG-INFO
```

### Comparing `surv_ai-0.1.8/LICENSE` & `surv_ai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/README.md` & `surv_ai-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: surv-ai
+Version: 0.1.9
+Summary: A framework for multi-agent modeling using large language models
+Home-page: https://github.com/DanielBalsam/surv_ai
+License: MIT
+Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
+Author: Daniel Balsam
+Author-email: daniel.balsam@survai.org
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
+Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
+Description-Content-Type: text/markdown
+
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![PyPi](https://shields.io/pypi/v/surv-ai)](https://pypi.org/project/surv-ai/)
 [![PyPi](https://shields.io/pypi/pyversions/surv-ai)](https://pypi.org/project/surv-ai/)
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
@@ -100,43 +128,45 @@
 
 Let's start by establishing the system's ability to figure out if information is true.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
-    ToolBelt,x
+    ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
-survey = Survey(
-    client,
-    tool_belt=ToolBelt(
-        client,
-        tools=[
-            GoogleCustomSearchTool(
-                client,
-                os.environ["GOOGLE_API_KEY"],
-                os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                start_date="2023-01-01",
-                end_date="2023-05-01",
-                n_pages=10,
-            )
-        ]
+tool_belt = ToolBelt(
+    tools=[
+        GoogleCustomSearchTool(
+            google_api_key=os.environ["GOOGLE_API_KEY"],
+            google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+            start_date="2023-01-01",
+            end_date="2023-05-01",
+            n_pages=10,
+        )
+    ]
+)
+base_knowledge = [
+    Knowledge(
+        text="It is currently 2023/05/01, all the articles are from 2023.",
+        source="Additional context",
     ),
+]
+
+survey = Survey(
+    client=client,
+    tool_belt=tool_belt,
+    base_knowledge=base_knowledge,
+    max_knowledge_per_agent=3,
     n_agents=10,
-    base_knowledge=[
-        Knowledge(
-            text="It is currently 2023/05/01, all the articles are from 2023.",
-            source="Additional context",
-        ),
-    ],
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
@@ -153,36 +183,38 @@
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
-survey = Survey(
-    client,
-    tool_belt=ToolBelt(
-        client,
-        tools=[
-            GoogleCustomSearchTool(
-                client,
-                os.environ["GOOGLE_API_KEY"],
-                os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                n_pages=10,
-                start_date="2023-01-01",
-                end_date="2023-05-01",
-            )
-        ]
+tool_belt = ToolBelt(
+    tools=[
+        GoogleCustomSearchTool(
+            google_api_key=os.environ["GOOGLE_API_KEY"],
+            google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+            start_date="2023-01-01",
+            end_date="2023-05-01",
+            n_pages=10,
+        )
+    ]
+)
+base_knowledge = [
+    Knowledge(
+        text="It is currently 2023/05/01, all the articles are from 2023.",
+        source="Additional context",
     ),
+]
+
+survey = Survey(
+    client=client,
+    tool_belt=tool_belt,
+    base_knowledge=base_knowledge,
+    max_knowledge_per_agent=3,
     n_agents=10,
-    base_knowledge=[
-        Knowledge(
-            text="It is currently 2023/05/01, all the articles are from 2023.",
-            source="Additional context",
-        ),
-    ],
 )
 
 await survey.conduct(
     "California experienced little rainfall this winter.",
 )  # This should always returns a high confidence disagreement.
 ```
 
@@ -197,60 +229,63 @@
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge,
+    Survey,
     SurveyParameter
 )
 
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
+def build_parameter(date_range: tuple[str, str]):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date=date_range[0],
+                end_date=date_range[1]
+            ),
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently {date_range[0]}. The included articles were published between {date_range[0]} and {date_range[1]}",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=date_range[1],
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":20,
+            "max_concurrency": 10,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
 date_ranges = [
     ('2022-05-01', '2022-06-01'),
     ('2022-06-01', '2022-07-01'),
     ('2022-07-01', '2022-08-01'),
     ('2022-08-01', '2022-09-01'),
     ('2022-09-01', '2022-10-01'),
     ('2022-10-01', '2022-11-05'),
 ]
 
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=range[1],
-            parameters={
-                "n_agents": 100,
-                "max_concurrency": 10,
-                "tool_belt": ToolBelt(
-                    client,
-                    [
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=20,
-                            start_date=range[0],
-                            end_date=range[1]
-                        ),
-                    ],
-                ),
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently {range[0]}. The included articles were published between {range[0]} and {range[1]}",
-                        source="Additional context",
-                    ),
-                ],
-            },
-        )
-        for range in date_ranges
-    ],
+    parameters=[build_parameter(date_range) for date_range in date_ranges],
 )
 
 results = await model.build(
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
@@ -270,55 +305,57 @@
     GoogleCustomSearchTool,
     Knowledge,
     Survey,
     SurveyParameter
 )
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
+def build_parameter(date_range: tuple[str, str]):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date=date_range[0],
+                end_date=date_range[1]
+            ),
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently {date_range[0]}. The included articles were published between {date_range[0]} and {date_range[1]}",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=date_range[1],
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":20,
+            "max_concurrency": 10,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
 date_ranges = [
     ('2021-09-01', '2022-01-01'),
     ('2022-01-01', '2022-03-01'),
     ('2022-03-01', '2022-06-01'),
     ('2022-06-01', '2022-09-01'),
     ('2022-09-01', '2023-01-01'),
     ('2023-01-01', '2023-03-01'),
     ('2023-03-01', '2023-06-01'),
 ]
 
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=range[1],
-            parameters={
-                "n_agents": 100,
-                "max_concurrency": 5,
-                "tool_belt": ToolBelt(
-                    client,
-                    [
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=10,
-                            start_date=range[0],
-                            end_date=range[1]
-                        ),
-                    ],
-                ),
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently {range[0]}. The included articles were published between {range[0]} and {range[1]}",
-                        source="Additional context",
-                    ),
-                ],
-            },
-        )
-        for range in date_ranges
-    ],
+    parameters=[build_parameter(date_range) for date_range in date_ranges],
 )
 
 results = await model.build(
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
@@ -339,53 +376,57 @@
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge,
     Survey,
     SurveyParameter
 )
 
-sources = [
+client = GPTClient(os.environ["OPEN_AI_API_KEY"])
+
+def build_parameter(news_source: str):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date="2023-05-01",
+                end_date="2023-06-01",
+                only_include_sources=[news_source]
+            ),
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently 2023-06-01. The included articles were published between 2023-05-01 and 2023-06-01",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=news_source,
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":10,
+            "max_concurrency": 10,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
+news_sources = [
     "nytimes.com",
     "cnn.com",
     "wsj.com",
     "foxnews.com",
 ]
 
-client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=source,
-            parameters={
-                "tool_belt": ToolBelt(
-                    client,
-                    tools=[
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=10,
-                            start_date="2023-05-01",
-                            end_date="2023-06-01",
-                            only_include_sources=[source]
-                        )
-                    ]
-                ),
-                "n_agents": 100,
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently 2023-06-01. The included articles were published between 2023-05-01 and 2023-06-01",
-                        source="Additional context",
-                    ),
-                ],
-            }
-        )
-        for source in sources
-    ],
+    parameters=[build_parameter(news_source) for news_source in news_sources],
 )
 results = await model.build(
     "Republicans are responsible for the impending debt ceiling crisis."
 )
 ```
 
 This provides us with a scatter plot representing the above-mentioned news sources:
@@ -403,52 +444,54 @@
     GPTClient,
     AnthropicClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge,
     Survey,
-    SurveyParameter
+    SurveyParameter,
+    LargeLanguageModelClientInterface
 )
 
-
 clients = [AnthropicClient(os.environ["ANTHROPIC_API_KEY"]), GPTClient(os.environ["OPEN_AI_API_KEY"])]
+
+def build_parameter(client: LargeLanguageModelClientInterface):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date="2023-01-01",
+                end_date="2024-05-01",
+                max_concurrency=3,
+            )
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently 2023-06-01. The included articles were published between 2023-01-01 and 2023-06-01",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=client.__class__.__name__,
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":20,
+            "max_concurrency": 3,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=client.__class__.__name__,
-            kwargs={
-                "client": client,
-                "tool_belt": ToolBelt(
-                    client,
-                    tools=[
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=10,
-                            start_date="2023-01-01",
-                            end_date="2023-06-01",
-                            max_concurrency=3,
-                        )
-                    ]
-                ),
-                "n_agents": 100,
-                "max_concurrency": 3,
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently 2023-06-01. The included articles were published between 2023-01-01 and 2023-06-01",
-                        source="Additional context",
-                    ),
-                ],
-            }
-        )
-        for client in clients
-    ],
+    parameters=[build_parameter(client) for client in clients],
 )
 results = await model.build(
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
 When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
@@ -473,36 +516,38 @@
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
-survey = Survey(
-    client,
-    tool_belt=ToolBelt(
-        client,
-        tools=[
-            GoogleCustomSearchTool(
-                client,
-                os.environ["GOOGLE_API_KEY"],
-                os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                start_date="2023-01-01",
-                end_date="2023-05-01",
-                n_pages=10,
-            )
-        ]
+tool_belt = ToolBelt(
+    tools=[
+        GoogleCustomSearchTool(
+            google_api_key=os.environ["GOOGLE_API_KEY"],
+            google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+            start_date="2023-01-01",
+            end_date="2023-05-01",
+            n_pages=10,
+        )
+    ]
+)
+base_knowledge = [
+    Knowledge(
+        text="It is currently 2023/05/01, all the articles are from 2023.",
+        source="Additional context",
     ),
+]
+
+survey = Survey(
+    client=client,
+    tool_belt=tool_belt,
+    base_knowledge=base_knowledge,
+    max_knowledge_per_agent=3,
     n_agents=10,
-    base_knowledge=[
-        Knowledge(
-            text="It is currently 2023/05/01, all the articles are from 2023.",
-            source="Additional context",
-        ),
-    ],
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
@@ -562,7 +607,8 @@
 4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection with the multi-agent models.
 5. More documentation and use guides!
 
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
+
```

### Comparing `surv_ai-0.1.8/pyproject.toml` & `surv_ai-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surv_ai"
-version = "0.1.8"
+version = "0.1.9"
 description = "A framework for multi-agent modeling using large language models"
 authors = ["Daniel Balsam <daniel.balsam@survai.org>"]
 license = "MIT"
 readme = "README.md"
 keywords=[
     "ai",
     "artificial intelligence",
@@ -40,20 +40,20 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiohttp = "^3.8.4"
 pydantic = "^1.10.7"
 python-dotenv = "^1.0.0"
 beautifulsoup4 = "^4.12.2"
 colorama = "^0.4.6"
 exceptiongroup = "^1.1.1"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.22.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 matplotlib = "^3.7.1"
```

### Comparing `surv_ai-0.1.8/surv_ai/__init__.py` & `surv_ai-0.1.9/surv_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/core/agent.py` & `surv_ai-0.1.9/surv_ai/core/agent.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/core/agents/binary.py` & `surv_ai-0.1.9/surv_ai/core/agents/binary.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/core/agents/reasoning.py` & `surv_ai-0.1.9/surv_ai/core/agents/reasoning.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,23 +43,19 @@
 
     def _get_plan_prompt_text(self, prompt: str):
         return f"""     
         You are a decisive agent who is concerned with whether this statement is more likely to be true or false:
 
         {prompt}
            
-        You must decide whether you think the statement is more likely to be true or false.
-
-        The next set of messages will be a series of articles that you can use to help you make your decision.
+        The next set of messages will be a series of articles a user has provided that you can use to help you make your decision.
 
         In your response please construct a plan for how you will approach the problem.
 
-        Make sure your plan includes offering specific citations.
-
-        You must make the best decision possible with the information you have. You cannot be undecided.
+        You may only use the information the user has provided.
         """
 
     async def _get_plan(self, prompt: str, relevant_knowledge: list[Knowledge]):
         messages = [
             PromptMessage(
                 role="system",
                 content=self._get_plan_prompt_text(
@@ -154,15 +150,18 @@
             n_knowledge_items=self.n_knowledge_items_per_prompt,
         )
 
         plan = await self._get_plan(prompt, relevant_knowledge)
         logger.log_internal(f"{self.name} plans: {plan}")
 
         argument_in_favor = await self._get_argument_in_favor(prompt, relevant_knowledge)
+        logger.log_internal(f"{self.name} argues in favor: {argument_in_favor}")
+
         argument_against = await self._get_argument_against(prompt, relevant_knowledge)
+        logger.log_internal(f"{self.name} argues against: {argument_against}")
 
         messages = [
             PromptMessage(
                 role="system",
                 content=self._get_completion_prompt_text(
                     prompt,
                 ),
```

### Comparing `surv_ai-0.1.8/surv_ai/core/interfaces.py` & `surv_ai-0.1.9/surv_ai/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/core/model.py` & `surv_ai-0.1.9/surv_ai/core/model.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/core/survey.py` & `surv_ai-0.1.9/surv_ai/core/survey.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,19 @@
         self,
         statement: str,
         summaries: Conversation,
         relevant_articles: list[Knowledge],
         index: int,
     ):
         try:
+            agent_name = f"ReasoningAgent #{index + 1}"
             reasoning_agent = ReasoningAgent(
                 self.client,
                 n_knowledge_items_per_prompt=self.max_knowledge_per_agent,
+                name=agent_name,
                 _hyperparameters={"temperature": 0.6},
             )
 
             for article in sample(
                 relevant_articles,
                 min(len(relevant_articles), self.max_knowledge_per_agent),
             ):
@@ -60,18 +62,18 @@
             binary_agent = BinaryAgent(
                 self.client,
                 _hyperparameters={"temperature": 0.2, "max_tokens": 5},
             )
             binary_agent.teach_text(statement, "Assertion")
 
             response_conversation = Conversation()
-            response_conversation.add(response, f"Researcher #{index}", reasoning_agent.color)
+            response_conversation.add(response, agent_name, reasoning_agent.color)
 
             decision = await binary_agent.prompt(response_conversation)
-            summaries.add(decision, f"Researcher #{index}", reasoning_agent.color)
+            summaries.add(decision, agent_name, reasoning_agent.color)
 
             true_in_decision = "true" in decision.lower()
             false_in_decision = "false" in decision.lower()
 
             if true_in_decision and not false_in_decision:
                 return "true"
             elif false_in_decision and not true_in_decision:
@@ -87,15 +89,15 @@
     async def conduct(self, hypothesis: str):
         results = {"true": 0, "false": 0, "undecided": 0, "error": 0}
 
         summaries = Conversation()
         agents = 0
 
         try:
-            relevant_articles = await self.tool_belt.inspect(hypothesis, self.base_knowledge or [])
+            relevant_articles = await self.tool_belt.inspect(self.client, hypothesis, self.base_knowledge or [])
         except NoMemoriesFoundException:
             return SurveyResponse(
                 in_favor=0,
                 against=0,
                 undecided=0,
                 error=self.n_agents,
                 percent_in_favor=0,
```

### Comparing `surv_ai-0.1.8/surv_ai/lib/conversation/conversation.py` & `surv_ai-0.1.9/surv_ai/lib/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/lib/knowledge_store/interfaces.py` & `surv_ai-0.1.9/surv_ai/lib/knowledge_store/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/lib/knowledge_store/local.py` & `surv_ai-0.1.9/surv_ai/lib/knowledge_store/local.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/lib/llm/anthropic.py` & `surv_ai-0.1.9/surv_ai/lib/llm/anthropic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from enum import Enum
 
-from aiohttp import ClientSession
+import requests
 
 from surv_ai.lib.log import logger
 
 from .interfaces import LargeLanguageModelClientInterface, Prompt
 
 
 class AnthropicModel(str, Enum):
@@ -20,15 +20,14 @@
         self,
         api_key: str,
     ):
         self.api_key = api_key
 
     async def _get_completion(
         self,
-        session: ClientSession,
         prompt: Prompt,
         attempt=1,
         presence_penalty=0,
         frequency_penalty=0,
         temperature=1,
         top_p=1,
         max_tokens: int = 800,
@@ -55,72 +54,76 @@
                 "prompt": messages,
                 "temperature": temperature,
                 "top_p": top_p,
                 "max_tokens_to_sample": max_tokens,
                 "stop_sequences": ["\n\nUser:"],
             }
 
-            response = await session.post(
-                "https://api.anthropic.com/v1/complete",
-                json=request,
-                headers={
-                    "Content-Type": "application/json",
-                    "x-api-key": f"{self.api_key}",
-                },
+            loop = asyncio.get_event_loop()
+            response = await loop.run_in_executor(
+                None,
+                lambda: requests.post(
+                    "https://api.anthropic.com/v1/complete",
+                    json=request,
+                    headers={
+                        "Content-Type": "application/json",
+                        "x-api-key": f"{self.api_key}",
+                    },
+                ),
             )
 
             try:
-                response_body = await response.json()
+                response_body = response.json()
             except Exception:
-                response_body = await response.text()
+                response_body = response.text
 
             response.raise_for_status()
         except Exception as e:
-            logger.log_exception(e)
-
-            if not response or response.status == 429 or response.status == 502:
-                await asyncio.sleep(0.5)
+            if not response or response.status_code == 429 or response.status_code == 502:
+                seconds_to_wait = 0.5 * attempt
+                logger.log_internal("Exceeded model rate limit: attempting backoff...")
+                await asyncio.sleep(seconds_to_wait)
 
                 if attempt < 5:
-                    return await self._get_completion(session, prompt, attempt + 1)
-            elif response.status == 400:
+                    return await self._get_completion(prompt, attempt + 1)
+            elif response.status_code == 400:
                 if attempt < 5:
+                    logger.log_internal("Exceeded model context length limit: attempting to reduce prompt size...")
+
                     return await self._get_completion(
-                        session,
                         prompt,
                         attempt + 1,
                         token_multiplier=token_multiplier - 0.2,
                     )
-            else:
-                raise Exception(
-                    f"Call to GPT API failed with status {response.status}.",
-                    response_body,
-                )
+
+            logger.log_exception(e)
+            raise Exception(
+                f"Call to Anthropic API failed with status {response.status_code}.",
+                response_body,
+            )
 
         return response_body["completion"]
 
     async def get_completions(
         self,
         prompts: list[Prompt],
         presence_penalty=0,
         frequency_penalty=0,
         temperature=1,
         top_p=1,
         max_tokens: int = 800,
         model=AnthropicModel.CLAUDE_V1,
     ) -> list[str]:
-        async with ClientSession() as session:
-            return await asyncio.gather(
-                *[
-                    self._get_completion(
-                        session,
-                        prompt,
-                        presence_penalty=presence_penalty,
-                        frequency_penalty=frequency_penalty,
-                        temperature=temperature,
-                        top_p=top_p,
-                        max_tokens=max_tokens,
-                        model=model,
-                    )
-                    for prompt in prompts
-                ],
-            )
+        return await asyncio.gather(
+            *[
+                self._get_completion(
+                    prompt,
+                    presence_penalty=presence_penalty,
+                    frequency_penalty=frequency_penalty,
+                    temperature=temperature,
+                    top_p=top_p,
+                    max_tokens=max_tokens,
+                    model=model,
+                )
+                for prompt in prompts
+            ],
+        )
```

### Comparing `surv_ai-0.1.8/surv_ai/lib/llm/gpt.py` & `surv_ai-0.1.9/surv_ai/lib/llm/gpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from enum import Enum
 
-from aiohttp import ClientSession
+import requests
 
 from surv_ai.lib.log import logger
 
 from .interfaces import LargeLanguageModelClientInterface, Prompt
 
 
 class GPTModel(str, Enum):
@@ -21,15 +21,14 @@
         self,
         api_key: str,
     ):
         self.api_key = api_key
 
     async def _get_completion(
         self,
-        session: ClientSession,
         prompt: Prompt,
         attempt=1,
         presence_penalty=0,
         frequency_penalty=0,
         temperature=1,
         top_p=1,
         max_tokens: int = 800,
@@ -71,71 +70,76 @@
                 "temperature": temperature,
                 "top_p": top_p,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "max_tokens": max_tokens,
             }
 
-            response = await session.post(
-                "https://api.openai.com/v1/chat/completions",
-                json=request,
-                headers={
-                    "Content-Type": "application/json",
-                    "Authorization": f"Bearer {self.api_key}",
-                },
+            loop = asyncio.get_event_loop()
+            response = await loop.run_in_executor(
+                None,
+                lambda: requests.post(
+                    "https://api.openai.com/v1/chat/completions",
+                    json=request,
+                    headers={
+                        "Content-Type": "application/json",
+                        "Authorization": f"Bearer {self.api_key}",
+                    },
+                ),
             )
 
             try:
-                response_body = await response.json()
+                response_body = response.json()
             except Exception:
-                response_body = await response.text()
+                response_body = response.text
 
             response.raise_for_status()
         except Exception as e:
-            logger.log_exception(e)
-            if not response or response.status == 429 or response.status == 502:
-                await asyncio.sleep(0.5)
+            if not response or response.status_code == 429 or response.status_code == 502:
+                seconds_to_wait = 0.5 * attempt
+                logger.log_internal("Exceeded model rate limit: attempting backoff...")
+                await asyncio.sleep(seconds_to_wait)
 
                 if attempt < 5:
-                    return await self._get_completion(session, prompt, attempt + 1)
-            elif response.status == 400:
+                    return await self._get_completion(prompt, attempt + 1)
+            elif response.status_code == 400:
                 if attempt < 5:
+                    logger.log_internal("Exceeded model context length limit: attempting to reduce prompt size...")
+
                     return await self._get_completion(
-                        session,
                         prompt,
                         attempt + 1,
                         token_multiplier=token_multiplier - 0.2,
                     )
-            else:
-                raise Exception(
-                    f"Call to GPT API failed with status {response.status}.",
-                    response_body,
-                )
+
+            logger.log_exception(e)
+            raise Exception(
+                f"Call to GPT API failed with status {response.status_code}.",
+                response_body,
+            )
 
         return response_body["choices"][0]["message"]["content"]
 
     async def get_completions(
         self,
         prompts: list[Prompt],
         presence_penalty=0,
         frequency_penalty=0,
         temperature=1,
         top_p=1,
         max_tokens: int = 800,
         model=GPTModel.TURBO,
     ) -> list[str]:
-        async with ClientSession() as session:
-            return await asyncio.gather(
-                *[
-                    self._get_completion(
-                        session,
-                        prompt,
-                        presence_penalty=presence_penalty,
-                        frequency_penalty=frequency_penalty,
-                        temperature=temperature,
-                        top_p=top_p,
-                        max_tokens=max_tokens,
-                        model=model,
-                    )
-                    for prompt in prompts
-                ],
-            )
+        return await asyncio.gather(
+            *[
+                self._get_completion(
+                    prompt,
+                    presence_penalty=presence_penalty,
+                    frequency_penalty=frequency_penalty,
+                    temperature=temperature,
+                    top_p=top_p,
+                    max_tokens=max_tokens,
+                    model=model,
+                )
+                for prompt in prompts
+            ],
+        )
```

### Comparing `surv_ai-0.1.8/surv_ai/lib/log.py` & `surv_ai-0.1.9/surv_ai/lib/log.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.8/surv_ai/lib/tools/query/google_custom_search.py` & `surv_ai-0.1.9/surv_ai/lib/tools/query/google_custom_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import re
+from typing import Optional
 
-from aiohttp import ClientSession
+import requests
 from bs4 import BeautifulSoup
 
 from surv_ai.lib.knowledge_store.interfaces import Knowledge
 from surv_ai.lib.llm.interfaces import (
     LargeLanguageModelClientInterface,
     Prompt,
     PromptMessage,
@@ -21,40 +22,48 @@
     """
     command = r"SEARCH\((.+)\)"
 
     _base_url = "https://www.googleapis.com/customsearch/v1/siterestrict"
 
     def __init__(
         self,
-        llm_client: LargeLanguageModelClientInterface,
-        google_api_key: str,
-        google_search_engine_id: str,
+        llm_client: Optional[LargeLanguageModelClientInterface] = None,
+        google_api_key: str = "",
+        google_search_engine_id: str = "",
         start_date=None,
         end_date=None,
         n_pages=1,
         max_percent_per_source=1.0,
         max_concurrency=10,
         only_include_sources=None,
     ):
-        self.client = llm_client
+        if llm_client:
+            logger.log_warning(
+                "Deprecation warning: LargeLanguageModelClient no longer should be passed into tools on init."
+            )
+
+        if not google_api_key:
+            raise ValueError("google_api_key is required for GoogleCustomSearchTool")
+        elif not google_search_engine_id:
+            raise ValueError("google_search_engine_id is required for GoogleCustomSearchTool")
 
         self.google_api_key = google_api_key
         self.google_search_engine_id = google_search_engine_id
 
         self.n_pages = n_pages
 
         self.start_date = start_date
         self.end_date = end_date
 
         self.max_percent_per_source = max_percent_per_source
         self.max_concurrency = max_concurrency
 
         self.only_include_sources = only_include_sources
 
-    async def _search(self, session, query: str) -> list[str]:
+    async def _search(self, query: str) -> list[str]:
         start = 1
         results = []
 
         seen_sources = {}
 
         while len(results) < self.n_pages:
             params = {
@@ -67,16 +76,17 @@
 
             if self.start_date:
                 params["q"] += f" after:{self.start_date}"
 
             if self.end_date:
                 params["q"] += f" before:{self.end_date}"
 
-            async with session.get(self._base_url, params=params) as response:
-                data = await response.json()
+            loop = asyncio.get_event_loop()
+            response = await loop.run_in_executor(None, lambda: requests.get(self._base_url, params=params))
+            data = response.json()
 
             try:
                 new_records = data["items"]
             except Exception:
                 logger.log_exception("Could not retrieve all articles.")
 
                 return results
@@ -109,117 +119,119 @@
                 new_records = records_to_return
 
             results += new_records
             start += 10
 
         return results
 
-    async def _get_page_text(self, session: ClientSession, web_url: str) -> str:
-        response = await session.get(
-            web_url,
-            headers={"User-Agent": "Mozilla/5.0"},
+    async def _get_page_text(self, web_url: str) -> str:
+        loop = asyncio.get_event_loop()
+        response = await loop.run_in_executor(
+            None,
+            lambda: requests.get(web_url, headers={"User-Agent": "Mozilla/5.0"}),
         )
 
-        data = await response.text()
+        data = response.text
 
         soup = BeautifulSoup(data, "html.parser")
 
         results = []
         for paragraph in soup.find_all("p"):
             results.append(paragraph.text)
 
         return results
 
     async def _ingest_page_information(
         self,
-        session,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         title: str,
         publication: str,
         web_url: str,
     ):
-        paragraphs = await self._get_page_text(session, web_url)
+        paragraphs = await self._get_page_text(web_url)
 
         prompt = Prompt(
             messages=[
                 PromptMessage(
-                    content=f"""A user has asked you some questions:
+                    content=f"""A user has presented you with a hypothesis:
                     
                     {original_prompt}
 
                     All subsequent messages will be paragraphs from a {publication} article titled "{title}."
 
-                    Your job is to extract any useful information that might help someone answer these questions.
+                    Your job is to extract any useful information that might help someone evaluate this hypothesis.
 
                     Remember to include as much data and concrete examples as possible from the article.
 
-                    For each useful piece of information you extract, please state why it relates to the original questions.
+                    For each useful piece of information you extract, please state why it relates to the original hypothesis.
                     """,
                     role="system",
                 ),
                 *[PromptMessage(content=paragraph, role="user", name="Article") for paragraph in paragraphs],
                 PromptMessage(
                     role="assistant",
-                    content=f"I have read the Wikpedia article entitled {title} and some useful information is:",
+                    content=f"I have read the {publication} article entitled {title} and some useful information is:",
                 ),
             ],
         )
-        response = await self.client.get_completions([prompt])
+        response = await llm_client.get_completions([prompt])
 
         return response[0]
 
     async def _ingest_pages(
         self,
-        session: ClientSession,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         result: dict,
     ):
         try:
             metatags = result["pagemap"]["metatags"][0]
 
             publication = metatags.get("og:site_name", result["displayLink"])
             title = metatags.get("og:title", result["title"])
 
             logger.log_context(f"......Retrieving {publication} article with title {title}......")
             page_summary = await self._ingest_page_information(
-                session,
+                llm_client,
                 original_prompt,
                 title,
                 publication,
                 result["link"],
             )
+            logger.log_internal(f"Summary of {publication} article with title {title}: {page_summary}")
 
             return Knowledge(
                 text=f'{publication} article entitled "{title}": {page_summary}',
                 source=result["link"],
             )
         except Exception as e:
             logger.log_exception(e)
             return None
 
     async def use(
         self,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         search_query: str,
     ) -> list[Knowledge]:
-        async with ClientSession() as session:
-            search_results = await self._search(session, search_query)
+        search_results = await self._search(search_query)
+
+        if len(search_results) == 0:
+            return []
 
-            if len(search_results) == 0:
-                return []
+        response = []
 
-            response = []
+        while len(response) < len(search_results[: self.n_pages]):
+            results_to_fetch = min(
+                self.max_concurrency,
+                len(search_results[: self.n_pages]) - len(response),
+            )
 
-            while len(response) < len(search_results[: self.n_pages]):
-                results_to_fetch = min(
-                    self.max_concurrency,
-                    len(search_results[: self.n_pages]) - len(response),
-                )
-
-                response += await asyncio.gather(
-                    *[
-                        self._ingest_pages(session, original_prompt, result)
-                        for result in search_results[len(response) : len(response) + results_to_fetch]
-                    ]
-                )
+            response += await asyncio.gather(
+                *[
+                    self._ingest_pages(llm_client, original_prompt, result)
+                    for result in search_results[len(response) : len(response) + results_to_fetch]
+                ]
+            )
 
-            return [r for r in response if r]
+        return [r for r in response if r]
```

### Comparing `surv_ai-0.1.8/surv_ai/lib/tools/query/wikipedia.py` & `surv_ai-0.1.9/surv_ai/lib/tools/query/wikipedia.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import re
+from typing import Optional
 
-from aiohttp import ClientSession
+import requests
 from bs4 import BeautifulSoup
 
 from surv_ai.lib.knowledge_store.interfaces import Knowledge
 from surv_ai.lib.llm.interfaces import (
     LargeLanguageModelClientInterface,
     Prompt,
     PromptMessage,
@@ -21,72 +22,78 @@
     """
     command = r"WIKIPEDIA\((.+)\)"
 
     _base_url = "https://en.wikipedia.org/w/api.php"
 
     def __init__(
         self,
-        llm_client: LargeLanguageModelClientInterface,
+        llm_client: Optional[LargeLanguageModelClientInterface] = None,
         n_articles=1,
     ):
-        self.client = llm_client
+        if llm_client:
+            logger.log_warning(
+                "Deprecation warning: LargeLanguageModelClient no longer should be passed into tools on init."
+            )
+
         self.n_articles = n_articles
 
         self._already_searched = dict()
 
-    async def _search(self, session, query: str) -> list[str]:
+    async def _search(self, query: str) -> list[str]:
         params = {
             "action": "query",
             "format": "json",
             "list": "search",
             "srsearch": re.sub(r"[^A-Za-z0-9 ]+", "", query),
         }
-        async with session.get(self._base_url, params=params) as response:
-            data = await response.json()
-            return [result["title"] for result in data["query"]["search"]]
+        loop = asyncio.get_event_loop()
+        response = await loop.run_in_executor(None, lambda: requests.get(self._base_url, params=params))
+        data = response.json()
+        return [result["title"] for result in data["query"]["search"]]
 
-    async def _get_page_text(self, session, page_title: str) -> str:
+    async def _get_page_text(self, page_title: str) -> str:
         if page_title in self._already_searched:
             return self._already_searched[page_title]
 
         params = {
             "action": "parse",
             "format": "json",
             "page": page_title,
             "prop": "text",
         }
 
-        async with session.get(self._base_url, params=params) as response:
-            data = await response.json()
+        loop = asyncio.get_event_loop()
+        response = await loop.run_in_executor(None, lambda: requests.get(self._base_url, params=params))
+        data = response.json()
 
-            try:
-                html_content = data["parse"]["text"]["*"]
+        try:
+            html_content = data["parse"]["text"]["*"]
 
-                soup = BeautifulSoup(html_content, "html.parser")
+            soup = BeautifulSoup(html_content, "html.parser")
 
-                results = []
-                for paragraph in soup.find_all("p"):
-                    paragraph_text = paragraph.text.strip()
+            results = []
+            for paragraph in soup.find_all("p"):
+                paragraph_text = paragraph.text.strip()
 
-                    if paragraph_text:
-                        results.append(paragraph_text)
+                if paragraph_text:
+                    results.append(paragraph_text)
 
-                self._already_searched[page_title] = results
-            except Exception:
-                return ""
+            self._already_searched[page_title] = results
+        except Exception:
+            return ""
 
-            return results
+        return results
 
     async def _ingest_page_information(
         self,
-        session,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         page_title: str,
     ):
-        paragraphs = await self._get_page_text(session, page_title)
+        paragraphs = await self._get_page_text(page_title)
 
         prompt = Prompt(
             messages=[
                 PromptMessage(
                     content=f"""A user has asked you some questions:
                     
                     {original_prompt}
@@ -104,40 +111,42 @@
                 *[PromptMessage(content=paragraph, role="user", name="Article") for paragraph in paragraphs],
                 PromptMessage(
                     role="assistant",
                     content=f"I have read the Wikpedia article entitled {page_title} and some useful information is:",
                 ),
             ],
         )
-        response = await self.client.get_completions([prompt], **{"temperature": 0.2})
+        response = await llm_client.get_completions([prompt], **{"temperature": 0.2})
 
         return response[0]
 
     async def _ingest_pages(
         self,
-        session: ClientSession,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         page_title: str,
     ):
         logger.log_context(f"......Learning Wikipedia page with title {page_title}......")
         page_summary = await self._ingest_page_information(
-            session,
+            llm_client,
             original_prompt,
             page_title,
         )
+        logger.log_internal(f"Summary of Wikipedia article with title {page_title}: {page_summary}")
 
         source = f"https://en.wikipedia.org/wiki/{page_title.replace(' ', '_')}"
 
         return Knowledge(
             text=f"Wikipedia page entitled {page_title}: {page_summary}",
             source=source,
         )
 
     async def _filter_relevant_pages(
         self,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         search_results: list[str],
     ):
         prompt = Prompt(
             messages=[
                 PromptMessage(
                     content=f"""Your job is to determine which, if any of the following article titles are relevant to a user's prompt.
@@ -154,30 +163,30 @@
                 ),
                 PromptMessage(
                     content=", ".join(search_results),
                     role="user",
                 ),
             ],
         )
-        response = (await self.client.get_completions([prompt]))[0]
+        response = (await llm_client.get_completions([prompt]))[0]
 
         return response
 
     async def use(
         self,
+        llm_client: LargeLanguageModelClientInterface,
         original_prompt: str,
         search_query: str,
     ) -> list[Knowledge]:
-        async with ClientSession() as session:
-            search_results = await self._search(session, search_query)
+        search_results = await self._search(search_query)
 
-            relevant_results = (await self._filter_relevant_pages(original_prompt, search_results)).split(", ")
+        relevant_results = (await self._filter_relevant_pages(llm_client, original_prompt, search_results)).split(", ")
 
-            if len(relevant_results) == 0:
-                return []
+        if len(relevant_results) == 0:
+            return []
 
-            return await asyncio.gather(
-                *[
-                    self._ingest_pages(session, original_prompt, page_title)
-                    for page_title in relevant_results[: self.n_articles]
-                ]
-            )
+        return await asyncio.gather(
+            *[
+                self._ingest_pages(llm_client, original_prompt, page_title)
+                for page_title in relevant_results[: self.n_articles]
+            ]
+        )
```

### Comparing `surv_ai-0.1.8/surv_ai/lib/tools/tool_belt.py` & `surv_ai-0.1.9/surv_ai/lib/tools/tool_belt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Optional
 
 from surv_ai.lib.knowledge_store.interfaces import Knowledge
 from surv_ai.lib.llm.interfaces import (
     LargeLanguageModelClientInterface,
     Prompt,
     PromptMessage,
 )
@@ -10,19 +11,23 @@
 
 from .interfaces import NoMemoriesFoundException, ToolBeltInterface, ToolInterface
 
 
 class ToolBelt(ToolBeltInterface):
     def __init__(
         self,
-        client: LargeLanguageModelClientInterface,
-        tools: list[ToolInterface],
+        llm_client: Optional[LargeLanguageModelClientInterface] = None,
+        tools: Optional[list[ToolInterface]] = None,
     ):
-        self.client = client
-        self.tools = tools
+        if llm_client:
+            logger.log_warning(
+                "Deprecation warning: LargeLanguageModelClient no longer should be passed into ToolBelt on init."
+            )
+
+        self.tools = tools or []
 
     @staticmethod
     def tools_as_list(tools: list[ToolInterface]) -> str:
         return "\n".join(f"{i + 1}. {t.instruction}" for i, t in enumerate(tools)) if tools else ""
 
     def _get_tool_belt_prompt(self, original_prompt: str, base_knowledge: list[Knowledge]) -> str:
         return Prompt(
@@ -58,33 +63,34 @@
                     """,
                 ),
             ]
         )
 
     async def inspect(
         self,
+        client: LargeLanguageModelClientInterface,
         original_prompt: str,
         base_knowledge: list[Knowledge],
         attempt=1,
     ):
         prompt = self._get_tool_belt_prompt(original_prompt, base_knowledge)
 
-        response = (await self.client.get_completions([prompt], **{"temperature": 0.7}))[0].strip()
+        response = (await client.get_completions([prompt], **{"temperature": 0.7}))[0].strip()
 
         for tool in self.tools:
             match = re.match(tool.command, response)
 
             if match:
                 knowledge = []
                 for args in match.groups():
                     logger.log_context(f"...Using tool: {response}...")
 
-                    knowledge += await tool.use(original_prompt, args)
+                    knowledge += await tool.use(client, original_prompt, args)
 
                     if not knowledge and attempt < 3:
-                        knowledge = await self.inspect(original_prompt, attempt=attempt + 1)
+                        knowledge = await self.inspect(client, original_prompt, base_knowledge, attempt=attempt + 1)
                     elif not knowledge:
                         raise NoMemoriesFoundException()
 
                 return knowledge
 
         return []
```

### Comparing `surv_ai-0.1.8/PKG-INFO` & `surv_ai-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: surv-ai
-Version: 0.1.8
-Summary: A framework for multi-agent modeling using large language models
-Home-page: https://github.com/DanielBalsam/surv_ai
-License: MIT
-Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
-Author: Daniel Balsam
-Author-email: daniel.balsam@survai.org
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
-Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
-Description-Content-Type: text/markdown
-
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![PyPi](https://shields.io/pypi/v/surv-ai)](https://pypi.org/project/surv-ai/)
 [![PyPi](https://shields.io/pypi/pyversions/surv-ai)](https://pypi.org/project/surv-ai/)
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
@@ -128,43 +100,45 @@
 
 Let's start by establishing the system's ability to figure out if information is true.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
-    ToolBelt,x
+    ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
-survey = Survey(
-    client,
-    tool_belt=ToolBelt(
-        client,
-        tools=[
-            GoogleCustomSearchTool(
-                client,
-                os.environ["GOOGLE_API_KEY"],
-                os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                start_date="2023-01-01",
-                end_date="2023-05-01",
-                n_pages=10,
-            )
-        ]
+tool_belt = ToolBelt(
+    tools=[
+        GoogleCustomSearchTool(
+            google_api_key=os.environ["GOOGLE_API_KEY"],
+            google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+            start_date="2023-01-01",
+            end_date="2023-05-01",
+            n_pages=10,
+        )
+    ]
+)
+base_knowledge = [
+    Knowledge(
+        text="It is currently 2023/05/01, all the articles are from 2023.",
+        source="Additional context",
     ),
+]
+
+survey = Survey(
+    client=client,
+    tool_belt=tool_belt,
+    base_knowledge=base_knowledge,
+    max_knowledge_per_agent=3,
     n_agents=10,
-    base_knowledge=[
-        Knowledge(
-            text="It is currently 2023/05/01, all the articles are from 2023.",
-            source="Additional context",
-        ),
-    ],
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
@@ -181,36 +155,38 @@
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
-survey = Survey(
-    client,
-    tool_belt=ToolBelt(
-        client,
-        tools=[
-            GoogleCustomSearchTool(
-                client,
-                os.environ["GOOGLE_API_KEY"],
-                os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                n_pages=10,
-                start_date="2023-01-01",
-                end_date="2023-05-01",
-            )
-        ]
+tool_belt = ToolBelt(
+    tools=[
+        GoogleCustomSearchTool(
+            google_api_key=os.environ["GOOGLE_API_KEY"],
+            google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+            start_date="2023-01-01",
+            end_date="2023-05-01",
+            n_pages=10,
+        )
+    ]
+)
+base_knowledge = [
+    Knowledge(
+        text="It is currently 2023/05/01, all the articles are from 2023.",
+        source="Additional context",
     ),
+]
+
+survey = Survey(
+    client=client,
+    tool_belt=tool_belt,
+    base_knowledge=base_knowledge,
+    max_knowledge_per_agent=3,
     n_agents=10,
-    base_knowledge=[
-        Knowledge(
-            text="It is currently 2023/05/01, all the articles are from 2023.",
-            source="Additional context",
-        ),
-    ],
 )
 
 await survey.conduct(
     "California experienced little rainfall this winter.",
 )  # This should always returns a high confidence disagreement.
 ```
 
@@ -225,60 +201,63 @@
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge,
+    Survey,
     SurveyParameter
 )
 
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
+def build_parameter(date_range: tuple[str, str]):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date=date_range[0],
+                end_date=date_range[1]
+            ),
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently {date_range[0]}. The included articles were published between {date_range[0]} and {date_range[1]}",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=date_range[1],
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":20,
+            "max_concurrency": 10,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
 date_ranges = [
     ('2022-05-01', '2022-06-01'),
     ('2022-06-01', '2022-07-01'),
     ('2022-07-01', '2022-08-01'),
     ('2022-08-01', '2022-09-01'),
     ('2022-09-01', '2022-10-01'),
     ('2022-10-01', '2022-11-05'),
 ]
 
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=range[1],
-            parameters={
-                "n_agents": 100,
-                "max_concurrency": 10,
-                "tool_belt": ToolBelt(
-                    client,
-                    [
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=20,
-                            start_date=range[0],
-                            end_date=range[1]
-                        ),
-                    ],
-                ),
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently {range[0]}. The included articles were published between {range[0]} and {range[1]}",
-                        source="Additional context",
-                    ),
-                ],
-            },
-        )
-        for range in date_ranges
-    ],
+    parameters=[build_parameter(date_range) for date_range in date_ranges],
 )
 
 results = await model.build(
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
@@ -298,55 +277,57 @@
     GoogleCustomSearchTool,
     Knowledge,
     Survey,
     SurveyParameter
 )
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
+def build_parameter(date_range: tuple[str, str]):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date=date_range[0],
+                end_date=date_range[1]
+            ),
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently {date_range[0]}. The included articles were published between {date_range[0]} and {date_range[1]}",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=date_range[1],
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":20,
+            "max_concurrency": 10,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
 date_ranges = [
     ('2021-09-01', '2022-01-01'),
     ('2022-01-01', '2022-03-01'),
     ('2022-03-01', '2022-06-01'),
     ('2022-06-01', '2022-09-01'),
     ('2022-09-01', '2023-01-01'),
     ('2023-01-01', '2023-03-01'),
     ('2023-03-01', '2023-06-01'),
 ]
 
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=range[1],
-            parameters={
-                "n_agents": 100,
-                "max_concurrency": 5,
-                "tool_belt": ToolBelt(
-                    client,
-                    [
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=10,
-                            start_date=range[0],
-                            end_date=range[1]
-                        ),
-                    ],
-                ),
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently {range[0]}. The included articles were published between {range[0]} and {range[1]}",
-                        source="Additional context",
-                    ),
-                ],
-            },
-        )
-        for range in date_ranges
-    ],
+    parameters=[build_parameter(date_range) for date_range in date_ranges],
 )
 
 results = await model.build(
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
@@ -367,53 +348,57 @@
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge,
     Survey,
     SurveyParameter
 )
 
-sources = [
+client = GPTClient(os.environ["OPEN_AI_API_KEY"])
+
+def build_parameter(news_source: str):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date="2023-05-01",
+                end_date="2023-06-01",
+                only_include_sources=[news_source]
+            ),
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently 2023-06-01. The included articles were published between 2023-05-01 and 2023-06-01",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=news_source,
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":10,
+            "max_concurrency": 10,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
+news_sources = [
     "nytimes.com",
     "cnn.com",
     "wsj.com",
     "foxnews.com",
 ]
 
-client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=source,
-            parameters={
-                "tool_belt": ToolBelt(
-                    client,
-                    tools=[
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=10,
-                            start_date="2023-05-01",
-                            end_date="2023-06-01",
-                            only_include_sources=[source]
-                        )
-                    ]
-                ),
-                "n_agents": 100,
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently 2023-06-01. The included articles were published between 2023-05-01 and 2023-06-01",
-                        source="Additional context",
-                    ),
-                ],
-            }
-        )
-        for source in sources
-    ],
+    parameters=[build_parameter(news_source) for news_source in news_sources],
 )
 results = await model.build(
     "Republicans are responsible for the impending debt ceiling crisis."
 )
 ```
 
 This provides us with a scatter plot representing the above-mentioned news sources:
@@ -431,52 +416,54 @@
     GPTClient,
     AnthropicClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge,
     Survey,
-    SurveyParameter
+    SurveyParameter,
+    LargeLanguageModelClientInterface
 )
 
-
 clients = [AnthropicClient(os.environ["ANTHROPIC_API_KEY"]), GPTClient(os.environ["OPEN_AI_API_KEY"])]
+
+def build_parameter(client: LargeLanguageModelClientInterface):
+    tool_belt = ToolBelt(
+        tools=[
+            GoogleCustomSearchTool(
+                google_api_key=os.environ["GOOGLE_API_KEY"],
+                google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+                n_pages=20,
+                start_date="2023-01-01",
+                end_date="2024-05-01",
+                max_concurrency=3,
+            )
+        ],
+    )
+    base_knowledge = [
+        Knowledge(
+            text=f"It is currently 2023-06-01. The included articles were published between 2023-01-01 and 2023-06-01",
+            source="Additional context",
+        ),
+    ]
+    return SurveyParameter(
+        independent_variable=client.__class__.__name__,
+        kwargs={
+            "client": client,
+            "n_agents": 100,
+            "max_knowledge_per_agent":20,
+            "max_concurrency": 3,
+            "tool_belt": tool_belt,
+            "base_knowledge": base_knowledge,
+        },
+    )
+
 model = Model(
     Survey,
-    parameters=[
-        SurveyParameter(
-            independent_variable=client.__class__.__name__,
-            kwargs={
-                "client": client,
-                "tool_belt": ToolBelt(
-                    client,
-                    tools=[
-                        GoogleCustomSearchTool(
-                            client,
-                            os.environ["GOOGLE_API_KEY"],
-                            os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                            n_pages=10,
-                            start_date="2023-01-01",
-                            end_date="2023-06-01",
-                            max_concurrency=3,
-                        )
-                    ]
-                ),
-                "n_agents": 100,
-                "max_concurrency": 3,
-                "base_knowledge": [
-                    Knowledge(
-                        text=f"It is currently 2023-06-01. The included articles were published between 2023-01-01 and 2023-06-01",
-                        source="Additional context",
-                    ),
-                ],
-            }
-        )
-        for client in clients
-    ],
+    parameters=[build_parameter(client) for client in clients],
 )
 results = await model.build(
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
 When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
@@ -501,36 +488,38 @@
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
-survey = Survey(
-    client,
-    tool_belt=ToolBelt(
-        client,
-        tools=[
-            GoogleCustomSearchTool(
-                client,
-                os.environ["GOOGLE_API_KEY"],
-                os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                start_date="2023-01-01",
-                end_date="2023-05-01",
-                n_pages=10,
-            )
-        ]
+tool_belt = ToolBelt(
+    tools=[
+        GoogleCustomSearchTool(
+            google_api_key=os.environ["GOOGLE_API_KEY"],
+            google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
+            start_date="2023-01-01",
+            end_date="2023-05-01",
+            n_pages=10,
+        )
+    ]
+)
+base_knowledge = [
+    Knowledge(
+        text="It is currently 2023/05/01, all the articles are from 2023.",
+        source="Additional context",
     ),
+]
+
+survey = Survey(
+    client=client,
+    tool_belt=tool_belt,
+    base_knowledge=base_knowledge,
+    max_knowledge_per_agent=3,
     n_agents=10,
-    base_knowledge=[
-        Knowledge(
-            text="It is currently 2023/05/01, all the articles are from 2023.",
-            source="Additional context",
-        ),
-    ],
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
@@ -590,8 +579,7 @@
 4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection with the multi-agent models.
 5. More documentation and use guides!
 
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
-
```

