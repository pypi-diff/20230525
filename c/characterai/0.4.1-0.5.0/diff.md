# Comparing `tmp/characterai-0.4.1.tar.gz` & `tmp/characterai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.4.1.tar", last modified: Tue May 16 20:11:17 2023, max compression
+gzip compressed data, was "dist\characterai-0.5.0.tar", last modified: Wed May 24 22:23:09 2023, max compression
```

## Comparing `characterai-0.4.1.tar` & `characterai-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:11:17.812631 characterai-0.4.1/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1873 2023-05-16 20:11:17.807631 characterai-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 20:11:17.736160 characterai-0.4.1/characterai/
--rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.4.1/characterai/__init__.py
--rw-rw-rw-   0        0        0     6548 2023-05-16 20:04:21.000000 characterai-0.4.1/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.4.1/characterai/errors.py
--rw-rw-rw-   0        0        0     6879 2023-05-16 20:02:20.000000 characterai-0.4.1/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:11:17.801631 characterai-0.4.1/characterai.egg-info/
--rw-rw-rw-   0        0        0     1873 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 20:11:17.813634 characterai-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-05-16 20:11:12.000000 characterai-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 22:23:09.325900 characterai-0.5.0/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1873 2023-05-24 22:23:09.323901 characterai-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 22:23:09.259431 characterai-0.5.0/characterai/
+-rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.5.0/characterai/__init__.py
+-rw-rw-rw-   0        0        0     8871 2023-05-24 22:17:50.000000 characterai-0.5.0/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.5.0/characterai/errors.py
+-rw-rw-rw-   0        0        0     9177 2023-05-24 22:17:56.000000 characterai-0.5.0/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-05-24 22:23:09.318900 characterai-0.5.0/characterai.egg-info/
+-rw-rw-rw-   0        0        0     1873 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-24 22:23:09.000000 characterai-0.5.0/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-24 22:23:08.000000 characterai-0.5.0/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 22:23:09.325900 characterai-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-05-24 22:19:52.000000 characterai-0.5.0/setup.py
```

### Comparing `characterai-0.4.1/LICENSE` & `characterai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.4.1/PKG-INFO` & `characterai-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 0.4.1
+Version: 0.5.0
 Summary: An unofficial API for character.ai for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `characterai-0.4.1/README.md` & `characterai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `characterai-0.4.1/characterai/characterai.py` & `characterai-0.5.0/characterai/characterai.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,41 +4,50 @@
 from playwright.sync_api import sync_playwright
 
 from characterai import errors
 from characterai.pyasynccai import pyAsyncCAI
 
 __all__ = ['pyCAI', 'pyAsyncCAI']
 
-page = None
-
 def goto(link: str, *, wait: bool = False, token: str = None):
     if token != None:
         page.set_extra_http_headers({"Authorization": f"Token {token}"})
 
     page.goto(link)
 
     if page.title() != 'Waiting Room powered by Cloudflare':
-        if page.get_by_role("button", name="Accept").is_visible():
-            page.get_by_role("button", name="Accept").click()
-
-            return page
+        return page
 
     else:
         if wait:
             page.wait_for_selector('div#wrapper', state='detached', timeout=0)
             goto(link=link, wait=wait)
         else:
             raise errors.NoResponse('The Site is Overloaded')
 
 def GetResponse(link: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
     goto(f'https://beta.character.ai/{link}/', wait=wait, token=token)
     data = json.loads(page.locator('body').inner_text())
 
     return data
 
+def PostResponse(link: str, post_link: str, data: str, headers: str, *, json: bool = True, wait: bool = False) -> Dict[str, str]:
+    goto(link, wait=wait)
+
+    with page.expect_response(post_link) as response_info:
+        # From HearYourWaifu
+        page.evaluate("const {fetch: origFetch} = window;window.fetch = async (...args) => {const response = await origFetch(...args);const raw_text = await new Response(response.clone().body).text();return response;};")
+        
+        page.evaluate("fetch('" + post_link + "', {method: 'POST',body: JSON.stringify(" + str(data) + "),headers: new Headers(" + str(headers) + "),})")
+
+    if json:
+        return response_info.value.json()
+    else:
+        return response_info.value.text()
+
 
 class pyCAI:
     def __init__(self, token: str, *, headless: bool = True):
         global page
 
         self.token = token
         self.headless = headless
@@ -54,18 +63,30 @@
         self.chat = self.chat()
 
     class user:
         """
         Just a Responses from site for user info
 
         user.info()
+        user.posts()
+        user.followers()
+        user.following()
+        user.recent()
         """
-
-        def info(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return GetResponse(link='chat/user', wait=wait, token=token)
+        def info(self, username: str = None, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            if username == None:
+                return GetResponse('chat/user', wait=wait, token=token)
+            else:
+                return PostResponse(
+                    link=f'https://beta.character.ai/public-profile/?username={username}',
+                    post_link='https://beta.character.ai/chat/user/public/',
+                    data={'username': username},
+                    headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
+                    wait=wait
+                )
 
         def posts(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/posts/user/?scope=user&page=1&posts_to_load=5', wait=wait, token=token)
 
         def followers(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/user/followers', wait=wait, token=token)
 
@@ -76,38 +97,52 @@
             return GetResponse('chat/characters/recent/', wait=wait, token=token)
 
     class character:
         """
         Just a Responses from site for characters
 
         character.trending()
+        character.recommended()
+        character.categories()
         character.info('CHAR')
         character.search('SEARCH')
         """
         def trending(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/characters/trending', wait=wait, token=token)
 
         def recommended(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/characters/recommended', wait=wait, token=token)
 
         def categories(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/character/categories', wait=wait, token=token)
 
         def info(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            data = GetResponse(f'chat/character/info-cached/{char}/', wait=wait, token=token)
-
-            if data != "{'error': 'Server Error (500)'}":
-                return data
-            else:
-                raise errors.CharNotFound('Wrong Char')
+            return GetResponse(f'chat/character/info-cached/{char}/', wait=wait, token=token)
         
         def search(self, search, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(f'chat/characters/search/?query={search}', wait=wait, token=token)
 
     class chat:
+        def get_histories(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            """
+            Getting all character chat histories, return json response
+
+            chat.get_histories('CHAR')
+            """
+            return PostResponse(
+                link=f'https://beta.character.ai/chat?char={char}',
+                post_link='https://beta.character.ai/chat/character/histories/',
+                data={
+                    "external_id": char,
+                    "number": 50,
+                },
+                headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
+                wait=wait
+            )
+
         def get_history(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
             Getting character chat history, return json response
 
             chat.get_history('CHAR')
             """
             goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
@@ -117,44 +152,58 @@
                     goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
 
                 response = response_info.value.text()
                 return json.loads(response)
             else:
                 raise errors.CharNotFound('Wrong Char')
 
-        def send_message(self, char: str, message: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+        def send_message(self, char: str, message: str, *, history_external_id: str = None, tgt: str = None, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
             Sending a message, return json
 
             chat.send_message('CHAR', 'MESSAGE')
             """
-            goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
-            
-            # BIG THANKS - HearYourWaifu
-            page.evaluate("""
-            const { fetch: origFetch } = window;
-            window.fetch = async (...args) => {
-            const response = await origFetch(...args);
-            const raw_text = await new Response(response.clone().body).text();
-            return response;};""")
-            
-            with page.expect_response("https://beta.character.ai/chat/streaming/") as response_info:
-                page.get_by_placeholder("Type a message").fill(message)
-                page.get_by_role("button", name="Submit Message").click()
-
-            response = response_info.value.text()
-            return json.loads('{"replies": ' + response.split(r'{"replies": ')[-1])
+            # Get history_external_id and tgt
+            if history_external_id == None and tgt == None:
+                info = PostResponse(
+                    link=f'https://beta.character.ai/chat?char={char}',
+                    post_link='https://beta.character.ai/chat/history/continue/',
+                    data={'character_external_id': char},
+                    headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
+                    wait=wait
+                )
+
+                history_external_id = info['external_id']
+                tgt = info['participants'][1]['user']['username']
+
+            response = PostResponse(
+                link=f'https://beta.character.ai/chat?char={char}',
+                post_link='https://beta.character.ai/chat/streaming/',
+                data={
+                    "history_external_id": history_external_id,
+                    "character_external_id": char,
+                    "text": message,
+                    "tgt": tgt
+                },
+                headers={'Authorization': f'Token {token}','Content-Type': 'application/json'},
+                wait=wait,
+                json=False
+            )
+
+            try:
+                return json.loads('{"replies": ' + str(response.split('{"replies": ')[-1].split('\n')[0]))
+            except:
+                return response
 
         def new_chat(self, char: str, *, wait: bool = False, token: str = None) -> None:
             """
-            Starting new chat, return json
+            Starting new chat, return new chat history
 
             chat.new_chat('CHAR')
             """
-            goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
-
-            with page.expect_response("https://beta.character.ai/chat/history/create/") as response_info:
-                page.wait_for_selector('.col-auto.px-2.dropdown').click()
-                page.wait_for_selector('"Save and Start New Chat"').click()
-
-            response = response_info.value.text()
-            return json.loads(response)
+            return PostResponse(
+                link=f'https://beta.character.ai/chat?char={char}',
+                post_link='https://beta.character.ai/chat/history/create/',
+                data={'character_external_id': char},
+                headers={'Authorization': f'Token {token}', 'Content-Type': 'application/json'},
+                wait=wait
+            )
```

### Comparing `characterai-0.4.1/characterai.egg-info/PKG-INFO` & `characterai-0.5.0/characterai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 0.4.1
+Version: 0.5.0
 Summary: An unofficial API for character.ai for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `characterai-0.4.1/setup.py` & `characterai-0.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf8') as f:
     long_description = f.read()
 
 setup(
     name='characterai',
-    version='0.4.1',
+    version='0.5.0',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/characterai',
     packages=find_packages(),
     install_requires=["playwright>=1.32.1"],
```

