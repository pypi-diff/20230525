# Comparing `tmp/google-chad-3.5.tar.gz` & `tmp/google-chad-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-chad-3.5.tar", last modified: Fri May  5 18:32:07 2023, max compression
+gzip compressed data, was "google-chad-3.6.tar", last modified: Thu May 25 10:39:58 2023, max compression
```

## Comparing `google-chad-3.5.tar` & `google-chad-3.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.572549 google-chad-3.5/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:13:40.000000 google-chad-3.5/LICENSE
--rwxrwx---   0 root         (0) root         (0)      111 2023-04-28 13:13:40.000000 google-chad-3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10618 2023-05-05 18:32:07.572549 google-chad-3.5/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    10515 2023-05-05 18:31:23.000000 google-chad-3.5/README.md
--rwxrwx---   0 root         (0) root         (0)      912 2023-05-05 18:23:13.000000 google-chad-3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:32:07.572549 google-chad-3.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.568549 google-chad-3.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.572549 google-chad-3.5/src/chad/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.5/src/chad/__init__.py
--rwxrwx---   0 root         (0) root         (0)    20062 2023-05-05 16:31:19.000000 google-chad-3.5/src/chad/chad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.572549 google-chad-3.5/src/chad_extractor/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.5/src/chad_extractor/__init__.py
--rwxrwx---   0 root         (0) root         (0)    23152 2023-05-05 16:31:29.000000 google-chad-3.5/src/chad_extractor/chad_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.572549 google-chad-3.5/src/dorks/
--rwxrwx---   0 root         (0) root         (0)      237 2023-04-28 13:13:40.000000 google-chad-3.5/src/dorks/social_media_dorks.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.572549 google-chad-3.5/src/google_chad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10618 2023-05-05 18:32:07.000000 google-chad-3.5/src/google_chad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-05 18:32:07.000000 google-chad-3.5/src/google_chad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:32:07.000000 google-chad-3.5/src/google_chad.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-05-05 18:32:07.000000 google-chad-3.5/src/google_chad.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-05-05 18:32:07.000000 google-chad-3.5/src/google_chad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-05 18:32:07.000000 google-chad-3.5/src/google_chad.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:32:07.572549 google-chad-3.5/src/templates/
--rwxrwx---   0 root         (0) root         (0)     1739 2023-04-28 13:13:40.000000 google-chad-3.5/src/templates/social_media_template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.779649 google-chad-3.6/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-05-25 09:39:19.000000 google-chad-3.6/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      111 2023-05-25 09:39:19.000000 google-chad-3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10626 2023-05-25 10:39:58.775647 google-chad-3.6/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    10523 2023-05-25 09:55:01.000000 google-chad-3.6/README.md
+-rwxrwx---   0 root         (0) root         (0)      912 2023-05-25 09:54:31.000000 google-chad-3.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:39:58.779649 google-chad-3.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/chad/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-05-25 09:39:19.000000 google-chad-3.6/src/chad/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    20062 2023-05-25 09:54:20.000000 google-chad-3.6/src/chad/chad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/chad_extractor/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-05-25 09:39:19.000000 google-chad-3.6/src/chad_extractor/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    23026 2023-05-25 10:37:05.000000 google-chad-3.6/src/chad_extractor/chad_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/dorks/
+-rwxrwx---   0 root         (0) root         (0)      237 2023-05-25 09:39:19.000000 google-chad-3.6/src/dorks/social_media_dorks.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/google_chad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10626 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/templates/
+-rwxrwx---   0 root         (0) root         (0)     1747 2023-05-25 09:55:11.000000 google-chad-3.6/src/templates/social_media_template.json
```

### Comparing `google-chad-3.5/LICENSE` & `google-chad-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `google-chad-3.5/PKG-INFO` & `google-chad-3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.5
+Version: 3.6
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
@@ -52,15 +52,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.5-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.6-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -124,15 +124,15 @@
    },
    "twitter":{
       "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
    "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
    "facebook":{
       "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
@@ -201,15 +201,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.5 ( github.com/ivan-sincek/chad )
+Chad v3.6 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -268,15 +268,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.5 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.6 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.5/README.md` & `google-chad-3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.5-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.6-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -111,15 +111,15 @@
    },
    "twitter":{
       "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
    "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
    "facebook":{
       "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
@@ -188,15 +188,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.5 ( github.com/ivan-sincek/chad )
+Chad v3.6 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -255,15 +255,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.5 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.6 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.5/pyproject.toml` & `google-chad-3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "google-chad"
-version = "3.5"
+version = "3.6"
 authors = [{ name = "Ivan Sincek" }]
 description = "Not another Google Dorking tool."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `google-chad-3.5/src/chad/chad.py` & `google-chad-3.6/src/chad/chad.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 colorama.init(autoreset = True)
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Chad v3.5 ( github.com/ivan-sincek/chad )")
+	print("Chad v3.6 ( github.com/ivan-sincek/chad )")
 	print("")
 	print("Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]")
 	print("Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -526,15 +526,15 @@
 			error("Missing a mandatory option (-q) and/or optional (-s, -t, -tr, -pr, -min-q, -max-q, -min-p, -max-p, -a, -p, -th, -d, -o, -sos, -dbg)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                                Chad v3.5                                #")
+		print("#                                Chad v3.6                                #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Search Google Dorks like Chad.                                          #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `google-chad-3.5/src/chad_extractor/chad_extractor.py` & `google-chad-3.6/src/chad_extractor/chad_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Chad Extractor v3.5 ( github.com/ivan-sincek/chad )")
+	print("Chad Extractor v3.6 ( github.com/ivan-sincek/chad )")
 	print("")
 	print("Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]")
 	print("Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]")
 
 def advanced():
 	basic()
 	print("")
@@ -297,16 +297,19 @@
 def split(records, threads = 4):
 	if threads > 1:
 		k, m = divmod(len(records), threads)
 		return (records[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(threads))
 	else:
 		return [records]
 
-def parse_response(skey, template, record, response):
+def parse_response(skey, template, record, response, excludes = []):
 	tmp = {}
+	if excludes:
+		for exclude in excludes:
+			response = re.sub(exclude, "", response, flags = re.MULTILINE | re.IGNORECASE)
 	if skey == "extracted":
 		for key in template:
 			try:
 				matches = re.findall(template[key]["extract"], response, re.MULTILINE | re.IGNORECASE)
 				if matches:
 					if "extract_prepend" in template[key] or "extract_append" in template[key]:
 						prepend = ""
@@ -326,49 +329,43 @@
 	elif skey == "validated" and re.search(template[record["id"]]["validate"], response, re.MULTILINE | re.IGNORECASE):
 		tmp = True
 	return tmp
 
 async def block(route):
 	await route.abort() if route.request.resource_type in ["stylesheet", "image", "media", "font", "ping"] else await route.continue_()
 
-async def page_get(context, url, excludes = [], wait = 4):
+async def page_get(context, url, wait = 4):
 	tmp = {"response": None, "error": False}
 	page = None
 	try:
 		page = await context.new_page()
 		await page.route("**/*", block) # ignore unnecessary requests
 		await page.goto(url, wait_until = "load")
 		if wait:
 			time.sleep(wait)
 		try:
 			await page.wait_for_load_state(state = "networkidle") # wait until network is idle for 500ms within 30s
 		except PlaywrightTimeoutError: # in case of a live stream, suppress and continue
 			pass
 		tmp["response"] = await page.content()
-		if excludes:
-			for exclude in excludes:
-				tmp["response"] = re.sub(exclude, "", tmp["response"], re.MULTILINE | re.IGNORECASE)
 	except PlaywrightTimeoutError:
 		pass
 	except Exception: # in case of a file or invalid domain, fallback
 		tmp["error"] = True
 	finally:
 		if page:
 			await page.close()
 	return tmp
 
-async def request_get(context, url, excludes = []):
+async def request_get(context, url):
 	tmp = {"response": None, "error": False}
 	try:
 		response = await context.request.get(url)
 		response = await response.body()
 		tmp["response"] = response.decode("ISO-8859-1")
-		if excludes:
-			for exclude in excludes:
-				tmp["response"] = re.sub(exclude, "", tmp["response"], re.MULTILINE | re.IGNORECASE)
 	except PlaywrightTimeoutError:
 		pass
 	except Exception: # in case of an invalid domain, break
 		tmp["error"] = True
 	return tmp
 
 def get_headers(agents = None):
@@ -390,23 +387,23 @@
 		# context.set_default_timeout(60000)
 		for record in records:
 			entry = {"files": record["files"], "url": record["url"], "results": {}}
 			count = retries + 1
 			while count > 0:
 				await context.set_extra_http_headers(get_headers(agents)) # anti-bot evasion 2
 				# --------------------
-				tmp = await page_get(context, record["url"], excludes, wait)
+				tmp = await page_get(context, record["url"], wait)
 				if tmp["error"]:
-					tmp = await request_get(context, record["url"], excludes)
+					tmp = await request_get(context, record["url"])
 					if tmp["error"]:
 						count = 0
 				# --------------------
 				if not tmp["error"] and tmp["response"]:
 					count = 0
-					entry["results"] = parse_response(skey, template, record, tmp["response"])
+					entry["results"] = parse_response(skey, template, record, tmp["response"], excludes)
 					if entry["results"]:
 						succeeded.append(entry)
 				else:
 					count -= 1
 					if count <= 0:
 						failed.append(entry)
 				# --------------------
@@ -432,24 +429,24 @@
 				tmp[key] = template[key]
 	else:
 		for key in template:
 			if "validate" in template[key]:
 				tmp[key] = template[key]
 	return tmp
 
-def parse_input(template, results, extract = True, plaintext = False):
+def parse_input(template, results, extract = True, plaintext = False, excludes = []):
 	global data
 	tmp = []
 	if extract:
 		for file in results:
 			for url in jquery(read_json(file), queries["get_urls"]):
 				tmp.append({"file": file, "url": url})
 	elif plaintext:
 		for file in results:
-			result = parse_response("extracted", template, None, read_file(file, False, True)) # passing a file content instead of a web content
+			result = parse_response("extracted", template, None, read_file(file, False, True), excludes) # passing a file content instead of a web content
 			data["extracted"]["data"].append({"file": file, "results": result})
 			for key in result:
 				if key in template:
 					for url in result[key]:
 						tmp.append({"file": file, "url": url, "id": key})
 	else:
 		for result in results:
@@ -542,15 +539,15 @@
 			error("Missing a mandatory option (-t, -res, -o) and/or optional (-pt, -e, -th, -r, -w, -a, -v)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                           Chad Extractor v3.5                           #")
+		print("#                           Chad Extractor v3.6                           #")
 		print("#                                   by Ivan Sincek                        #")
 		print("#                                                                         #")
 		print("# Extract and validate data from Chad results.                            #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
@@ -563,15 +560,15 @@
 			args["wait"] = 4
 		# --------------------
 		if args["plaintext"]:
 			args["template"] = parse_template(args["template"], True)
 			if not args["template"]:
 				print("No extraction entries were found in the template file")
 			else:
-				args["results"] = parse_input(args["template"], args["results"], False, True)
+				args["results"] = parse_input(args["template"], args["results"], False, True, args["excludes"])
 				if not data["extracted"]["data"]:
 					print("No data was extracted")
 				else:
 					args["template"] = parse_template(args["template"], False)
 					if not args["template"]:
 						print("No validation entries were found in the template file")
 					else:
```

### Comparing `google-chad-3.5/src/google_chad.egg-info/PKG-INFO` & `google-chad-3.6/src/google_chad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.5
+Version: 3.6
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
@@ -52,15 +52,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.5-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.6-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -124,15 +124,15 @@
    },
    "twitter":{
       "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
    "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
    "facebook":{
       "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
       "extract_prepend":"https://",
@@ -201,15 +201,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.5 ( github.com/ivan-sincek/chad )
+Chad v3.6 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -268,15 +268,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.5 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.6 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.5/src/templates/social_media_template.json` & `google-chad-3.6/src/templates/social_media_template.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'instagram'": "{'extract': "*

 * *                "'instagram\\\\.com\\\\/(?:(?!(?:p|accounts|explore)(?:\\\\/|\\\\?)[^\\\\s]+)[\\\\w\\\\d\\\\-\\\\+\\\\.]+)(?<!\\\\.)'}"}*

```diff
@@ -6,15 +6,15 @@
     },
     "facebook": {
         "extract": "facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
         "extract_prepend": "https://",
         "validate": "This page isn't available"
     },
     "instagram": {
-        "extract": "instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+        "extract": "instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
         "extract_append": "/",
         "extract_prepend": "https://",
         "validate": "Sorry, this page isn't available\\."
     },
     "linkedin-company": {
         "extract": "linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
         "extract_prepend": "https://hr.",
```

