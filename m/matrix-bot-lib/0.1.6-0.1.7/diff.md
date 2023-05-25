# Comparing `tmp/matrix-bot-lib-0.1.6.tar.gz` & `tmp/matrix_bot_lib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix-bot-lib-0.1.6.tar", max compression
+gzip compressed data, was "matrix_bot_lib-0.1.7.tar", max compression
```

## Comparing `matrix-bot-lib-0.1.6.tar` & `matrix_bot_lib-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1072 2022-09-14 11:39:06.687250 matrix-bot-lib-0.1.6/LICENSE
--rw-r--r--   0        0        0      183 2022-10-26 21:47:06.596290 matrix-bot-lib-0.1.6/matrix_bot_lib/__init__.py
--rw-r--r--   0        0        0    11072 2022-11-23 16:22:45.235089 matrix-bot-lib-0.1.6/matrix_bot_lib/botlib.py
--rw-r--r--   0        0        0     4460 2022-10-26 21:53:12.710803 matrix-bot-lib-0.1.6/matrix_bot_lib/models.py
--rw-r--r--   0        0        0      436 2022-11-16 17:37:52.674721 matrix-bot-lib-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 matrix-bot-lib-0.1.6/setup.py
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 matrix-bot-lib-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 23:56:04.134837 matrix_bot_lib-0.1.7/LICENSE
+-rw-r--r--   0        0        0      183 2023-05-24 23:56:04.134837 matrix_bot_lib-0.1.7/matrix_bot_lib/__init__.py
+-rw-r--r--   0        0        0    11125 2023-05-24 23:59:05.107318 matrix_bot_lib-0.1.7/matrix_bot_lib/botlib.py
+-rw-r--r--   0        0        0     4460 2023-05-24 23:56:04.134837 matrix_bot_lib-0.1.7/matrix_bot_lib/models.py
+-rw-r--r--   0        0        0      436 2023-05-24 23:56:04.134837 matrix_bot_lib-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 matrix_bot_lib-0.1.7/PKG-INFO
```

### Comparing `matrix-bot-lib-0.1.6/LICENSE` & `matrix_bot_lib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix-bot-lib-0.1.6/matrix_bot_lib/botlib.py` & `matrix_bot_lib-0.1.7/matrix_bot_lib/botlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                         logging.warning(f'{r.url}: {error}')
                         return Err(errcode)
                     case status_code, result:
                         logging.warning(f"Unknown: {status_code=}: {result=}. Sleeping {2**(retry_cnt-1)}s and retrying")
                 await asyncio.sleep(2**(retry_cnt-1))
             except Exception as ex:
                 logging.warning(f'Err {ex} Retrying.')
-
+                await asyncio.sleep(2**(retry_cnt-1))
         return Err(f"Did not manage to make request after {retry_cnt+1} retries")
 
     async def _POST(self, path: str, j, **kwargs) -> Result[dict, str]:
         async def aux():
             return await self.client.post(path, json=j, headers=self.get_auth(), **kwargs)
         return await self.process_body(aux)
 
@@ -187,16 +187,16 @@
                 else:
                     logging.info(f'No listeners for {typ=}.')
 
             case unknown:
                 logging.warning(f'Unknown event: {unknown}')
 
     async def run(self, full_sync=True) -> None:
-        if next_batch := await self.sync({'full_state': full_sync, 'timeout': 5_000}):
-            while (next_batch := await self.sync({'since': next_batch, 'timeout': 3_000})):
+        if next_batch := await self.sync({'full_state': full_sync, 'timeout': 7_000}):
+            while (next_batch := await self.sync({'since': next_batch, 'timeout': 5_000})):
                 logging.info("Syncing")
 
     def _save_tokens(self, tokens: TokenResponse):
         """ Given the result of login/RefreshTokenExchange this method will save the
         returned tokens.  Use `TokenResponse.from_dict` to turn a random dict into a TokenResponse.
         """
         if tokens.access_token:
```

### Comparing `matrix-bot-lib-0.1.6/matrix_bot_lib/models.py` & `matrix_bot_lib-0.1.7/matrix_bot_lib/models.py`

 * *Files identical despite different names*

