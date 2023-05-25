# Comparing `tmp/huhangkai-1.1.5.tar.gz` & `tmp/huhangkai-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.5.tar", last modified: Tue May 23 08:46:19 2023, max compression
+gzip compressed data, was "huhangkai-1.1.6.tar", last modified: Thu May 25 08:35:35 2023, max compression
```

## Comparing `huhangkai-1.1.5.tar` & `huhangkai-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:46:19.553175 huhangkai-1.1.5/
--rw-rw-rw-   0        0        0      228 2023-05-23 08:46:19.552180 huhangkai-1.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 08:46:19.540985 huhangkai-1.1.5/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.5/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3475 2023-05-23 08:44:54.000000 huhangkai-1.1.5/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.5/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-16 11:14:52.000000 huhangkai-1.1.5/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:46:19.550183 huhangkai-1.1.5/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 08:46:19.553175 huhangkai-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-05-23 08:46:16.000000 huhangkai-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:35:35.342184 huhangkai-1.1.6/
+-rw-rw-rw-   0        0        0      228 2023-05-25 08:35:35.341192 huhangkai-1.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 08:35:35.330215 huhangkai-1.1.6/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.6/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3821 2023-05-25 08:05:21.000000 huhangkai-1.1.6/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.6/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.6/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-16 11:14:52.000000 huhangkai-1.1.6/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:35:35.339192 huhangkai-1.1.6/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 08:35:35.000000 huhangkai-1.1.6/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 08:35:35.342184 huhangkai-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-05-25 08:35:14.000000 huhangkai-1.1.6/setup.py
```

### Comparing `huhangkai-1.1.5/commen/__init__.py` & `huhangkai-1.1.6/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.5/commen/init_project.py` & `huhangkai-1.1.6/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.5/commen/unit_dict.py` & `huhangkai-1.1.6/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.5/commen/unit_encryption.py` & `huhangkai-1.1.6/commen/unit_encryption.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,16 +64,17 @@
         return b
 
 
 # ------------------------加密------------------------
 def rsa_encryption(text: str, public_key: bytes):
     # 字符串指定编码（转为bytes）
     text = text.encode('utf-8')
+    key = RSA.importKey(public_key)
     # 构建公钥对象
-    cipher_public = PKCS1_v1_5.new(RSA.importKey(public_key))
+    cipher_public = PKCS1_v1_5.new(key)
     # 加密（bytes）
     text_encrypted = cipher_public.encrypt(text)
     # base64编码，并转为字符串
     text_encrypted_base64 = base64.b64encode(text_encrypted).decode()
     return text_encrypted_base64
 
 
@@ -96,17 +97,20 @@
     # 生成密钥对
     # create_rsa_pair(is_save=True)
     # public_key = read_public_key()
     # private_key = read_private_key()
     public_key, private_key = create_rsa_pair(is_save=False)
 
     # 加密
-    text = '123456'
-    text_encrypted_base64 = des_encryption(text)
+    text = 'Pickup@123456'
+    public_key = """-----BEGIN PUBLIC KEY-----
+MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQCsGAZ1trFEvH3TdHSFPbxCkdJUVLFsOUHW9ePVCAKkG0az4oqyKPJMME4avemlRlkBaNIpBPpqvPb0xBJgCu13ARm2YMNw7OdbHUiDjqciyU/WS5C9GiDGelHnSWM2m2sYdwU9zJO0I2nXViCccHTy29BWWkjXJTyCbiX2PyMymQIDAQAB
+-----END PUBLIC KEY-----"""
+    text_encrypted_base64 = rsa_encryption(text, public_key)
     print('密文：', text_encrypted_base64)
 
     # 解密
-    text_decrypted = des_decryption(text_encrypted_base64)
-    print('明文：', text_decrypted)
+    # text_decrypted = rsa_decryption(text_encrypted_base64, private_key)
+    # print('明文：', text_decrypted)
```

### Comparing `huhangkai-1.1.5/commen/unit_fun.py` & `huhangkai-1.1.6/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.5/commen/unit_logger.py` & `huhangkai-1.1.6/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.5/commen/unit_request.py` & `huhangkai-1.1.6/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.5/commen/unit_tasks.py` & `huhangkai-1.1.6/commen/unit_tasks.py`

 * *Files identical despite different names*

