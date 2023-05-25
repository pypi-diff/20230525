# Comparing `tmp/EdgeGPT-0.6.2.tar.gz` & `tmp/EdgeGPT-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.2.tar", last modified: Sun May 21 14:19:13 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.3.tar", last modified: Wed May 24 16:31:19 2023, max compression
```

## Comparing `EdgeGPT-0.6.2.tar` & `EdgeGPT-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-21 14:19:12.000000 EdgeGPT-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.2/LICENSE` & `EdgeGPT-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.2/PKG-INFO` & `EdgeGPT-0.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: EdgeGPT
-Version: 0.6.2
-Summary: Reverse engineered Edge Chat API
-Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong
-Author-email: acheong@student.dalat.org
-License: GNU General Public License v2.0
-Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
@@ -54,16 +35,16 @@
 ```bash
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
-- A Microsoft Account with early access to <https://bing.com/chat> (Required)
-- Required in a supported country with New Bing (Chinese mainland VPN required)
+- A Microsoft Account with access to <https://bing.com/chat> (Optional)
+- Required in a supported country or region with New Bing (Chinese mainland VPN required)
 - [Selenium](https://pypi.org/project/selenium/) (for automatic cookie setup)
 
 <details>
 
 <summary>
 
 # Chatbot
@@ -71,14 +52,35 @@
 </summary>
 
 ## Authentication
 
 !!! NOT REQUIRED ANYMORE !!!
 Microsoft has made the chat feature available to everyone, so you can skip this step.
 
+1. Install the latest version of Microsoft Edge
+<details>
+
+2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+
+</details>
+
+3. Open [bing.com/chat](https://bing.com/chat)
+4. If you see a chat feature, you are good to continue...
+5. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+6. Go to [bing.com](https://bing.com)
+7. Open the extension
+8. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
+9. Paste your cookies into a file `cookies.json`
+
+### In code:
+```python
+cookies = json.loads(open("./path/to/cookies.json", encoding="utf-8").read())
+bot = await Chatbot.create(cookies=cookies)
+```
+
 ## Running from the Command Line
 
 ```
  $ python3 -m EdgeGPT -h
 
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
         Repo: github.com/acheong08/EdgeGPT
@@ -94,28 +96,29 @@
 options:
   -h, --help            show this help message and exit
   --enter-once
   --no-stream
   --rich
   --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
   --style {creative,balanced,precise}
+  --cookie-file [path/to/cookies.json]
 ```
 
 ## Running in Python
 
 ### 1. The `Chatbot` class and `asyncio` for more granular control
 
 Use Async for the best experience, for example:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
-    bot = await Chatbot.create()
+    bot = await Chatbot.create() # Passing cookies is optional
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `EdgeGPT-0.6.2/README.md` & `EdgeGPT-0.6.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,503 +1,635 @@
-00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0a20 203c 696d 6720 7372 633d  er">.  <img src=
-00000020: 2268 7474 7073 3a2f 2f73 6f63 6961 6c69  "https://sociali
-00000030: 6679 2e67 6974 2e63 692f 6163 6865 6f6e  fy.git.ci/acheon
-00000040: 6730 382f 4564 6765 4750 542f 696d 6167  g08/EdgeGPT/imag
-00000050: 653f 666f 6e74 3d49 6e74 6572 266c 616e  e?font=Inter&lan
-00000060: 6775 6167 653d 3126 6c6f 676f 3d68 7474  guage=1&logo=htt
-00000070: 7073 2533 4125 3246 2532 4675 706c 6f61  ps%3A%2F%2Fuploa
-00000080: 642e 7769 6b69 6d65 6469 612e 6f72 6725  d.wikimedia.org%
-00000090: 3246 7769 6b69 7065 6469 6125 3246 636f  2Fwikipedia%2Fco
-000000a0: 6d6d 6f6e 7325 3246 3925 3246 3963 2532  mmons%2F9%2F9c%2
-000000b0: 4642 696e 675f 466c 7565 6e74 5f4c 6f67  FBing_Fluent_Log
-000000c0: 6f2e 7376 6726 6f77 6e65 723d 3126 7061  o.svg&owner=1&pa
-000000d0: 7474 6572 6e3d 466c 6f61 7469 6e67 2532  ttern=Floating%2
-000000e0: 3043 6f67 7326 7468 656d 653d 4175 746f  0Cogs&theme=Auto
-000000f0: 2220 616c 743d 2245 6467 6547 5054 2220  " alt="EdgeGPT" 
-00000100: 7769 6474 683d 2236 3430 2220 6865 6967  width="640" heig
-00000110: 6874 3d22 3332 3022 202f 3e0a 0a23 2045  ht="320" />..# E
-00000120: 6467 6520 4750 540a 0a5f 5468 6520 7265  dge GPT.._The re
-00000130: 7665 7273 6520 656e 6769 6e65 6572 696e  verse engineerin
-00000140: 6720 7468 6520 6368 6174 2066 6561 7475  g the chat featu
-00000150: 7265 206f 6620 7468 6520 6e65 7720 7665  re of the new ve
-00000160: 7273 696f 6e20 6f66 2042 696e 675f 0a0a  rsion of Bing_..
-00000170: 3c61 3e45 6e67 6c69 7368 3c2f 613e 202d  <a>English</a> -
-00000180: 0a3c 6120 6872 6566 3d22 2e2f 5245 4144  .<a href="./READ
-00000190: 4d45 5f7a 682d 636e 2e6d 6422 3ee7 ae80  ME_zh-cn.md">...
-000001a0: e4bd 93e4 b8ad e696 873c 2f61 3e20 2d0a  .........</a> -.
-000001b0: 3c61 2068 7265 663d 222e 2f52 4541 444d  <a href="./READM
-000001c0: 455f 7a68 2d74 772e 6d64 223e e7b9 81e9  E_zh-tw.md">....
-000001d0: ab94 e4b8 ade6 9687 3c2f 613e 202d 0a3c  ........</a> -.<
-000001e0: 6120 6872 6566 3d22 2e2f 5245 4144 4d45  a href="./README
-000001f0: 5f65 732e 6d64 223e 4573 7061 c3b1 6f6c  _es.md">Espa..ol
-00000200: 3c2f 613e 202d 0a3c 6120 6872 6566 3d22  </a> -.<a href="
-00000210: 2e2f 5245 4144 4d45 5f6a 612e 6d64 223e  ./README_ja.md">
-00000220: e697 a5e6 9cac e8aa 9e3c 2f61 3e0a 0a3c  .........</a>..<
-00000230: 2f64 6976 3e0a 0a3c 7020 616c 6967 6e3d  /div>..<p align=
-00000240: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
-00000250: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000260: 6875 622e 636f 6d2f 6163 6865 6f6e 6730  hub.com/acheong0
-00000270: 382f 4564 6765 4750 5422 3e0a 2020 2020  8/EdgeGPT">.    
-00000280: 3c69 6d67 2061 6c74 3d22 5079 5049 2076  <img alt="PyPI v
-00000290: 6572 7369 6f6e 2220 7372 633d 2268 7474  ersion" src="htt
-000002a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000002b0: 2e69 6f2f 7079 7069 2f76 2f45 6467 6547  .io/pypi/v/EdgeG
-000002c0: 5054 223e 0a20 203c 2f61 3e0a 2020 3c69  PT">.  </a>.  <i
-000002d0: 6d67 2061 6c74 3d22 5079 7468 6f6e 2076  mg alt="Python v
-000002e0: 6572 7369 6f6e 2220 7372 633d 2268 7474  ersion" src="htt
-000002f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000300: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
-00000310: 2d33 2e38 2b2d 626c 7565 2e73 7667 223e  -3.8+-blue.svg">
-00000320: 0a20 203c 696d 6720 616c 743d 2254 6f74  .  <img alt="Tot
-00000330: 616c 2064 6f77 6e6c 6f61 6473 2220 7372  al downloads" sr
-00000340: 633d 2268 7474 7073 3a2f 2f73 7461 7469  c="https://stati
-00000350: 632e 7065 7079 2e74 6563 682f 6261 6467  c.pepy.tech/badg
-00000360: 652f 6564 6765 6770 7422 3e0a 0a3c 2f70  e/edgegpt">..</p
-00000370: 3e0a 0a3c 6465 7461 696c 733e 0a0a 3c73  >..<details>..<s
-00000380: 756d 6d61 7279 3e0a 0a23 2053 6574 7570  ummary>..# Setup
-00000390: 0a0a 3c2f 7375 6d6d 6172 793e 0a0a 2323  ..</summary>..##
-000003a0: 2320 496e 7374 616c 6c20 7061 636b 6167  # Install packag
-000003b0: 650a 0a60 6060 6261 7368 0a70 7974 686f  e..```bash.pytho
-000003c0: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-000003d0: 6c20 4564 6765 4750 5420 2d2d 7570 6772  l EdgeGPT --upgr
-000003e0: 6164 650a 6060 600a 0a23 2323 2052 6571  ade.```..### Req
-000003f0: 7569 7265 6d65 6e74 730a 0a2d 2070 7974  uirements..- pyt
-00000400: 686f 6e20 332e 382b 0a2d 2041 204d 6963  hon 3.8+.- A Mic
-00000410: 726f 736f 6674 2041 6363 6f75 6e74 2077  rosoft Account w
-00000420: 6974 6820 6561 726c 7920 6163 6365 7373  ith early access
-00000430: 2074 6f20 3c68 7474 7073 3a2f 2f62 696e   to <https://bin
-00000440: 672e 636f 6d2f 6368 6174 3e20 2852 6571  g.com/chat> (Req
-00000450: 7569 7265 6429 0a2d 2052 6571 7569 7265  uired).- Require
-00000460: 6420 696e 2061 2073 7570 706f 7274 6564  d in a supported
-00000470: 2063 6f75 6e74 7279 2077 6974 6820 4e65   country with Ne
-00000480: 7720 4269 6e67 2028 4368 696e 6573 6520  w Bing (Chinese 
-00000490: 6d61 696e 6c61 6e64 2056 504e 2072 6571  mainland VPN req
-000004a0: 7569 7265 6429 0a2d 205b 5365 6c65 6e69  uired).- [Seleni
-000004b0: 756d 5d28 6874 7470 733a 2f2f 7079 7069  um](https://pypi
-000004c0: 2e6f 7267 2f70 726f 6a65 6374 2f73 656c  .org/project/sel
-000004d0: 656e 6975 6d2f 2920 2866 6f72 2061 7574  enium/) (for aut
-000004e0: 6f6d 6174 6963 2063 6f6f 6b69 6520 7365  omatic cookie se
-000004f0: 7475 7029 0a0a 3c64 6574 6169 6c73 3e0a  tup)..<details>.
-00000500: 0a3c 7375 6d6d 6172 793e 0a0a 2320 4368  .<summary>..# Ch
-00000510: 6174 626f 740a 0a3c 2f73 756d 6d61 7279  atbot..</summary
-00000520: 3e0a 0a23 2320 4175 7468 656e 7469 6361  >..## Authentica
-00000530: 7469 6f6e 0a0a 2121 2120 4e4f 5420 5245  tion..!!! NOT RE
-00000540: 5155 4952 4544 2041 4e59 4d4f 5245 2021  QUIRED ANYMORE !
-00000550: 2121 0a4d 6963 726f 736f 6674 2068 6173  !!.Microsoft has
-00000560: 206d 6164 6520 7468 6520 6368 6174 2066   made the chat f
-00000570: 6561 7475 7265 2061 7661 696c 6162 6c65  eature available
-00000580: 2074 6f20 6576 6572 796f 6e65 2c20 736f   to everyone, so
-00000590: 2079 6f75 2063 616e 2073 6b69 7020 7468   you can skip th
-000005a0: 6973 2073 7465 702e 0a0a 2323 2052 756e  is step...## Run
-000005b0: 6e69 6e67 2066 726f 6d20 7468 6520 436f  ning from the Co
-000005c0: 6d6d 616e 6420 4c69 6e65 0a0a 6060 600a  mmand Line..```.
-000005d0: 2024 2070 7974 686f 6e33 202d 6d20 4564   $ python3 -m Ed
-000005e0: 6765 4750 5420 2d68 0a0a 2020 2020 2020  geGPT -h..      
-000005f0: 2020 4564 6765 4750 5420 2d20 4120 6465    EdgeGPT - A de
-00000600: 6d6f 206f 6620 7265 7665 7273 6520 656e  mo of reverse en
-00000610: 6769 6e65 6572 696e 6720 7468 6520 4269  gineering the Bi
-00000620: 6e67 2047 5054 2063 6861 7462 6f74 0a20  ng GPT chatbot. 
-00000630: 2020 2020 2020 2052 6570 6f3a 2067 6974         Repo: git
-00000640: 6875 622e 636f 6d2f 6163 6865 6f6e 6730  hub.com/acheong0
-00000650: 382f 4564 6765 4750 540a 2020 2020 2020  8/EdgeGPT.      
-00000660: 2020 4279 3a20 416e 746f 6e69 6f20 4368    By: Antonio Ch
-00000670: 656f 6e67 0a0a 2020 2020 2020 2020 2168  eong..        !h
-00000680: 656c 7020 666f 7220 6865 6c70 0a0a 2020  elp for help..  
-00000690: 2020 2020 2020 5479 7065 2021 6578 6974        Type !exit
-000006a0: 2074 6f20 6578 6974 0a20 2020 2020 2020   to exit.       
-000006b0: 2045 6e74 6572 2074 7769 6365 2074 6f20   Enter twice to 
-000006c0: 7365 6e64 206d 6573 7361 6765 206f 7220  send message or 
-000006d0: 7365 7420 2d2d 656e 7465 722d 6f6e 6365  set --enter-once
-000006e0: 2074 6f20 7365 6e64 206f 6e65 206c 696e   to send one lin
-000006f0: 6520 6d65 7373 6167 650a 0a75 7361 6765  e message..usage
-00000700: 3a20 4564 6765 4750 542e 7079 205b 2d68  : EdgeGPT.py [-h
-00000710: 5d20 5b2d 2d65 6e74 6572 2d6f 6e63 655d  ] [--enter-once]
-00000720: 205b 2d2d 6e6f 2d73 7472 6561 6d5d 205b   [--no-stream] [
-00000730: 2d2d 7269 6368 5d20 5b2d 2d70 726f 7879  --rich] [--proxy
-00000740: 2050 524f 5859 5d20 5b2d 2d73 7479 6c65   PROXY] [--style
-00000750: 207b 6372 6561 7469 7665 2c62 616c 616e   {creative,balan
-00000760: 6365 642c 7072 6563 6973 657d 5d0a 0a6f  ced,precise}]..o
-00000770: 7074 696f 6e73 3a0a 2020 2d68 2c20 2d2d  ptions:.  -h, --
-00000780: 6865 6c70 2020 2020 2020 2020 2020 2020  help            
-00000790: 7368 6f77 2074 6869 7320 6865 6c70 206d  show this help m
-000007a0: 6573 7361 6765 2061 6e64 2065 7869 740a  essage and exit.
-000007b0: 2020 2d2d 656e 7465 722d 6f6e 6365 0a20    --enter-once. 
-000007c0: 202d 2d6e 6f2d 7374 7265 616d 0a20 202d   --no-stream.  -
-000007d0: 2d72 6963 680a 2020 2d2d 7072 6f78 7920  -rich.  --proxy 
-000007e0: 5052 4f58 5920 2020 2020 2020 2020 5072  PROXY         Pr
-000007f0: 6f78 7920 5552 4c20 2865 2e67 2e20 736f  oxy URL (e.g. so
-00000800: 636b 7335 3a2f 2f31 3237 2e30 2e30 2e31  cks5://127.0.0.1
-00000810: 3a31 3038 3029 0a20 202d 2d73 7479 6c65  :1080).  --style
-00000820: 207b 6372 6561 7469 7665 2c62 616c 616e   {creative,balan
-00000830: 6365 642c 7072 6563 6973 657d 0a60 6060  ced,precise}.```
-00000840: 0a0a 2323 2052 756e 6e69 6e67 2069 6e20  ..## Running in 
-00000850: 5079 7468 6f6e 0a0a 2323 2320 312e 2054  Python..### 1. T
-00000860: 6865 2060 4368 6174 626f 7460 2063 6c61  he `Chatbot` cla
-00000870: 7373 2061 6e64 2060 6173 796e 6369 6f60  ss and `asyncio`
-00000880: 2066 6f72 206d 6f72 6520 6772 616e 756c   for more granul
-00000890: 6172 2063 6f6e 7472 6f6c 0a0a 5573 6520  ar control..Use 
-000008a0: 4173 796e 6320 666f 7220 7468 6520 6265  Async for the be
-000008b0: 7374 2065 7870 6572 6965 6e63 652c 2066  st experience, f
-000008c0: 6f72 2065 7861 6d70 6c65 3a0a 0a60 6060  or example:..```
-000008d0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6173  python.import as
-000008e0: 796e 6369 6f0a 6672 6f6d 2045 6467 6547  yncio.from EdgeG
-000008f0: 5054 2069 6d70 6f72 7420 4368 6174 626f  PT import Chatbo
-00000900: 742c 2043 6f6e 7665 7273 6174 696f 6e53  t, ConversationS
-00000910: 7479 6c65 0a0a 6173 796e 6320 6465 6620  tyle..async def 
-00000920: 6d61 696e 2829 3a0a 2020 2020 626f 7420  main():.    bot 
-00000930: 3d20 6177 6169 7420 4368 6174 626f 742e  = await Chatbot.
-00000940: 6372 6561 7465 2829 0a20 2020 2070 7269  create().    pri
-00000950: 6e74 2861 7761 6974 2062 6f74 2e61 736b  nt(await bot.ask
-00000960: 2870 726f 6d70 743d 2248 656c 6c6f 2077  (prompt="Hello w
-00000970: 6f72 6c64 222c 2063 6f6e 7665 7273 6174  orld", conversat
-00000980: 696f 6e5f 7374 796c 653d 436f 6e76 6572  ion_style=Conver
-00000990: 7361 7469 6f6e 5374 796c 652e 6372 6561  sationStyle.crea
-000009a0: 7469 7665 2929 0a20 2020 2061 7761 6974  tive)).    await
-000009b0: 2062 6f74 2e63 6c6f 7365 2829 0a0a 6966   bot.close()..if
-000009c0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-000009d0: 6d61 696e 5f5f 223a 0a20 2020 2061 7379  main__":.    asy
-000009e0: 6e63 696f 2e72 756e 286d 6169 6e28 2929  ncio.run(main())
-000009f0: 0a60 6060 0a0a 3c64 6574 6169 6c73 3e0a  .```..<details>.
-00000a00: 3c73 756d 6d61 7279 3e0a 0a23 2323 2032  <summary>..### 2
-00000a10: 2920 5468 6520 6051 7565 7279 6020 616e  ) The `Query` an
-00000a20: 6420 6043 6f6f 6b69 6560 2068 656c 7065  d `Cookie` helpe
-00000a30: 7220 636c 6173 7365 730a 0a20 203c 2f73  r classes..  </s
-00000a40: 756d 6d61 7279 3e0a 0a43 7265 6174 6520  ummary>..Create 
-00000a50: 6120 7369 6d70 6c65 2042 696e 6720 4368  a simple Bing Ch
-00000a60: 6174 2041 4920 7175 6572 7920 2875 7369  at AI query (usi
-00000a70: 6e67 2074 6865 2027 7072 6563 6973 6527  ng the 'precise'
-00000a80: 2063 6f6e 7665 7273 6174 696f 6e20 7374   conversation st
-00000a90: 796c 6520 6279 2064 6566 6175 6c74 2920  yle by default) 
-00000aa0: 616e 6420 7365 6520 6a75 7374 2074 6865  and see just the
-00000ab0: 206d 6169 6e20 7465 7874 206f 7574 7075   main text outpu
-00000ac0: 7420 7261 7468 6572 2074 6861 6e20 7468  t rather than th
-00000ad0: 6520 7768 6f6c 6520 4150 4920 7265 7370  e whole API resp
-00000ae0: 6f6e 7365 3a0a 0a60 6060 7079 7468 6f6e  onse:..```python
-00000af0: 0a66 726f 6d20 4564 6765 4750 5420 696d  .from EdgeGPT im
-00000b00: 706f 7274 2051 7565 7279 2c20 436f 6f6b  port Query, Cook
-00000b10: 6965 0a0a 7120 3d20 5175 6572 7928 2257  ie..q = Query("W
-00000b20: 6861 7420 6172 6520 796f 753f 2047 6976  hat are you? Giv
-00000b30: 6520 796f 7572 2061 6e73 7765 7220 6173  e your answer as
-00000b40: 2050 7974 686f 6e20 636f 6465 2229 0a70   Python code").p
-00000b50: 7269 6e74 2871 290a 6060 600a 0a4f 7220  rint(q).```..Or 
-00000b60: 6368 616e 6765 2074 6865 2063 6f6e 7665  change the conve
-00000b70: 7273 6174 696f 6e20 7374 796c 6520 6f72  rsation style or
-00000b80: 2063 6f6f 6b69 6520 6669 6c65 2074 6f20   cookie file to 
-00000b90: 6265 2075 7365 643a 0a0a 6060 6070 7974  be used:..```pyt
-00000ba0: 686f 6e0a 7120 3d20 5175 6572 7928 0a20  hon.q = Query(. 
-00000bb0: 2022 5768 6174 2061 7265 2079 6f75 3f20   "What are you? 
-00000bc0: 4769 7665 2079 6f75 7220 616e 7377 6572  Give your answer
-00000bd0: 2061 7320 5079 7468 6f6e 2063 6f64 6522   as Python code"
-00000be0: 2c0a 2020 7374 796c 653d 2263 7265 6174  ,.  style="creat
-00000bf0: 6976 6522 2c20 2023 206f 7220 2762 616c  ive",  # or 'bal
-00000c00: 616e 6365 6427 0a20 2063 6f6f 6b69 6573  anced'.  cookies
-00000c10: 3d22 2e2f 6269 6e67 5f63 6f6f 6b69 6573  ="./bing_cookies
-00000c20: 5f61 6c74 6572 6e61 7469 7665 2e6a 736f  _alternative.jso
-00000c30: 6e22 0a29 0a60 6060 0a0a 5175 6963 6b6c  n".).```..Quickl
-00000c40: 7920 6578 7472 6163 7420 7468 6520 7465  y extract the te
-00000c50: 7874 206f 7574 7075 742c 2063 6f64 6520  xt output, code 
-00000c60: 736e 6970 7065 7473 2c20 6c69 7374 206f  snippets, list o
-00000c70: 6620 736f 7572 6365 732f 7265 6665 7265  f sources/refere
-00000c80: 6e63 6573 2c20 6f72 2073 7567 6765 7374  nces, or suggest
-00000c90: 6564 2066 6f6c 6c6f 772d 6f6e 2071 7565  ed follow-on que
-00000ca0: 7374 696f 6e73 2075 7369 6e67 2074 6865  stions using the
-00000cb0: 2066 6f6c 6c6f 7769 6e67 2061 7474 7269   following attri
-00000cc0: 6275 7465 733a 0a0a 6060 6070 7974 686f  butes:..```pytho
-00000cd0: 6e0a 712e 6f75 7470 7574 0a71 2e63 6f64  n.q.output.q.cod
-00000ce0: 650a 712e 7375 6767 6573 7469 6f6e 730a  e.q.suggestions.
-00000cf0: 712e 736f 7572 6365 7320 2020 2020 2020  q.sources       
-00000d00: 2320 666f 7220 7468 6520 6675 6c6c 206a  # for the full j
-00000d10: 736f 6e20 6f75 7470 7574 0a71 2e73 6f75  son output.q.sou
-00000d20: 7263 6573 5f64 6963 7420 2023 2066 6f72  rces_dict  # for
-00000d30: 2061 2064 6963 7469 6f6e 6172 7920 6f66   a dictionary of
-00000d40: 2074 6974 6c65 7320 616e 6420 7572 6c73   titles and urls
-00000d50: 0a60 6060 0a0a 4765 7420 7468 6520 6f72  .```..Get the or
-00000d60: 6769 6e61 6c20 7072 6f6d 7074 2061 6e64  ginal prompt and
-00000d70: 2074 6865 2063 6f6e 7665 7273 6174 696f   the conversatio
-00000d80: 6e20 7374 796c 6520 796f 7520 7370 6563  n style you spec
-00000d90: 6966 6965 643a 0a0a 6060 6070 7974 686f  ified:..```pytho
-00000da0: 6e0a 712e 7072 6f6d 7074 0a71 2e73 7479  n.q.prompt.q.sty
-00000db0: 6c65 0a72 6570 7228 7129 0a60 6060 0a0a  le.repr(q).```..
-00000dc0: 4163 6365 7373 2070 7265 7669 6f75 7320  Access previous 
-00000dd0: 5175 6572 6965 7320 6d61 6465 2073 696e  Queries made sin
-00000de0: 6365 2069 6d70 6f72 7469 6e67 2060 5175  ce importing `Qu
-00000df0: 6572 7960 3a0a 0a60 6060 7079 7468 6f6e  ery`:..```python
-00000e00: 0a51 7565 7279 2e69 6e64 6578 2020 2320  .Query.index  # 
-00000e10: 4120 6c69 7374 206f 6620 5175 6572 7920  A list of Query 
-00000e20: 6f62 6a65 6374 733b 2075 7064 6174 6564  objects; updated
-00000e30: 2064 796e 616d 6963 616c 6c79 0a51 7565   dynamically.Que
-00000e40: 7279 2e72 6571 7565 7374 5f63 6f75 6e74  ry.request_count
-00000e50: 2020 2320 4120 7461 6c6c 7920 6f66 2072    # A tally of r
-00000e60: 6571 7565 7374 7320 6d61 6465 2075 7369  equests made usi
-00000e70: 6e67 2065 6163 6820 636f 6f6b 6965 2066  ng each cookie f
-00000e80: 696c 650a 6060 600a 0a41 6e64 2066 696e  ile.```..And fin
-00000e90: 616c 6c79 2c20 7468 6520 6043 6f6f 6b69  ally, the `Cooki
-00000ea0: 6560 2063 6c61 7373 2073 7570 706f 7274  e` class support
-00000eb0: 7320 6d75 6c74 6970 6c65 2063 6f6f 6b69  s multiple cooki
-00000ec0: 6520 6669 6c65 732c 2073 6f20 6966 2079  e files, so if y
-00000ed0: 6f75 2063 7265 6174 6520 6164 6469 7469  ou create additi
-00000ee0: 6f6e 616c 2063 6f6f 6b69 6520 6669 6c65  onal cookie file
-00000ef0: 7320 7769 7468 2074 6865 206e 616d 696e  s with the namin
-00000f00: 6720 636f 6e76 656e 7469 6f6e 2060 6269  g convention `bi
-00000f10: 6e67 5f63 6f6f 6b69 6573 5f2a 2e6a 736f  ng_cookies_*.jso
-00000f20: 6e60 2c20 796f 7572 2071 7565 7269 6573  n`, your queries
-00000f30: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
-00000f40: 6c6c 7920 7472 7920 7573 696e 6720 7468  lly try using th
-00000f50: 6520 6e65 7874 2066 696c 6520 2861 6c70  e next file (alp
-00000f60: 6861 6265 7469 6361 6c6c 7929 2069 6620  habetically) if 
-00000f70: 796f 7527 7665 2065 7863 6565 6465 6420  you've exceeded 
-00000f80: 796f 7572 2064 6169 6c79 2071 756f 7461  your daily quota
-00000f90: 206f 6620 7265 7175 6573 7473 2028 6375   of requests (cu
-00000fa0: 7272 656e 746c 7920 7365 7420 6174 2032  rrently set at 2
-00000fb0: 3030 292e 0a0a 4865 7265 2061 7265 2074  00)...Here are t
-00000fc0: 6865 206d 6169 6e20 6174 7472 6962 7574  he main attribut
-00000fd0: 6573 2077 6869 6368 2079 6f75 2063 616e  es which you can
-00000fe0: 2061 6363 6573 733a 0a0a 6060 6070 7974   access:..```pyt
-00000ff0: 686f 6e0a 436f 6f6b 6965 2e63 7572 7265  hon.Cookie.curre
-00001000: 6e74 5f66 696c 655f 696e 6465 780a 436f  nt_file_index.Co
-00001010: 6f6b 6965 2e64 6972 7061 7468 0a43 6f6f  okie.dirpath.Coo
-00001020: 6b69 652e 7365 6172 6368 5f70 6174 7465  kie.search_patte
-00001030: 726e 2020 2320 6465 6661 756c 7420 6973  rn  # default is
-00001040: 2060 6269 6e67 5f63 6f6f 6b69 6573 5f2a   `bing_cookies_*
-00001050: 2e6a 736f 6e60 0a43 6f6f 6b69 652e 6669  .json`.Cookie.fi
-00001060: 6c65 7328 2920 2023 206c 6973 7420 6173  les()  # list as
-00001070: 2066 696c 6573 2074 6861 7420 6d61 7463   files that matc
-00001080: 6820 2e73 6561 7263 685f 7061 7474 6572  h .search_patter
-00001090: 6e0a 436f 6f6b 6965 2e63 7572 7265 6e74  n.Cookie.current
-000010a0: 5f66 696c 6570 6174 680a 436f 6f6b 6965  _filepath.Cookie
-000010b0: 2e63 7572 7265 6e74 5f64 6174 610a 436f  .current_data.Co
-000010c0: 6f6b 6965 2e69 6d70 6f72 745f 6e65 7874  okie.import_next
-000010d0: 2829 0a43 6f6f 6b69 652e 696d 6167 655f  ().Cookie.image_
-000010e0: 746f 6b65 6e0a 436f 6f6b 6965 2e69 676e  token.Cookie.ign
-000010f0: 6f72 655f 6669 6c65 730a 6060 600a 0a3c  ore_files.```..<
-00001100: 2f64 6574 6169 6c73 3e0a 0a2d 2d2d 0a0a  /details>..---..
-00001110: 2323 2052 756e 6e69 6e67 2077 6974 6820  ## Running with 
-00001120: 446f 636b 6572 0a0a 5468 6973 2061 7373  Docker..This ass
-00001130: 756d 6573 2079 6f75 2068 6176 6520 6120  umes you have a 
-00001140: 6669 6c65 2063 6f6f 6b69 6573 2e6a 736f  file cookies.jso
-00001150: 6e20 696e 2079 6f75 7220 6375 7272 656e  n in your curren
-00001160: 7420 776f 726b 696e 6720 6469 7265 6374  t working direct
-00001170: 6f72 790a 0a60 6060 6261 7368 0a0a 646f  ory..```bash..do
-00001180: 636b 6572 2072 756e 202d 2d72 6d20 2d69  cker run --rm -i
-00001190: 7420 2d76 2024 2870 7764 292f 636f 6f6b  t -v $(pwd)/cook
-000011a0: 6965 732e 6a73 6f6e 3a2f 636f 6f6b 6965  ies.json:/cookie
-000011b0: 732e 6a73 6f6e 3a72 6f20 2d65 2043 4f4f  s.json:ro -e COO
-000011c0: 4b49 455f 4649 4c45 3d27 2f63 6f6f 6b69  KIE_FILE='/cooki
-000011d0: 6573 2e6a 736f 6e27 2067 6863 722e 696f  es.json' ghcr.io
-000011e0: 2f61 6368 656f 6e67 3038 2f65 6467 6567  /acheong08/edgeg
-000011f0: 7074 0a60 6060 0a0a 596f 7520 6361 6e20  pt.```..You can 
-00001200: 6164 6420 616e 7920 6578 7472 6120 666c  add any extra fl
-00001210: 6167 7320 6173 2066 6f6c 6c6f 7769 6e67  ags as following
-00001220: 0a0a 6060 6062 6173 680a 0a64 6f63 6b65  ..```bash..docke
-00001230: 7220 7275 6e20 2d2d 726d 202d 6974 202d  r run --rm -it -
-00001240: 7620 2428 7077 6429 2f63 6f6f 6b69 6573  v $(pwd)/cookies
-00001250: 2e6a 736f 6e3a 2f63 6f6f 6b69 6573 2e6a  .json:/cookies.j
-00001260: 736f 6e3a 726f 202d 6520 434f 4f4b 4945  son:ro -e COOKIE
-00001270: 5f46 494c 453d 272f 636f 6f6b 6965 732e  _FILE='/cookies.
-00001280: 6a73 6f6e 2720 6768 6372 2e69 6f2f 6163  json' ghcr.io/ac
-00001290: 6865 6f6e 6730 382f 6564 6765 6770 7420  heong08/edgegpt 
-000012a0: 2d2d 7269 6368 202d 2d73 7479 6c65 2063  --rich --style c
-000012b0: 7265 6174 6976 650a 6060 600a 0a3c 2f64  reative.```..</d
-000012c0: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
-000012d0: 733e 0a0a 3c73 756d 6d61 7279 3e0a 0a23  s>..<summary>..#
-000012e0: 2049 6d61 6765 2067 656e 6572 6174 6f72   Image generator
-000012f0: 0a0a 3c2f 7375 6d6d 6172 793e 0a0a 2323  ..</summary>..##
-00001300: 2052 756e 6e69 6e67 2066 726f 6d20 7468   Running from th
-00001310: 6520 436f 6d6d 616e 6420 4c69 6e65 0a0a  e Command Line..
-00001320: 6060 6062 6173 680a 2420 7079 7468 6f6e  ```bash.$ python
-00001330: 3320 2d6d 2049 6d61 6765 4765 6e20 2d68  3 -m ImageGen -h
-00001340: 0a75 7361 6765 3a20 496d 6167 6547 656e  .usage: ImageGen
-00001350: 2e70 7920 5b2d 685d 205b 2d55 2055 5d20  .py [-h] [-U U] 
-00001360: 5b2d 2d63 6f6f 6b69 652d 6669 6c65 2043  [--cookie-file C
-00001370: 4f4f 4b49 455f 4649 4c45 5d20 2d2d 7072  OOKIE_FILE] --pr
-00001380: 6f6d 7074 2050 524f 4d50 5420 5b2d 2d6f  ompt PROMPT [--o
-00001390: 7574 7075 742d 6469 7220 4f55 5450 5554  utput-dir OUTPUT
-000013a0: 5f44 4952 5d20 5b2d 2d71 7569 6574 5d20  _DIR] [--quiet] 
-000013b0: 5b2d 2d61 7379 6e63 696f 5d0a 0a6f 7074  [--asyncio]..opt
-000013c0: 696f 6e61 6c20 6172 6775 6d65 6e74 733a  ional arguments:
-000013d0: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
-000013e0: 2020 2020 2020 2020 2073 686f 7720 7468           show th
-000013f0: 6973 2068 656c 7020 6d65 7373 6167 6520  is help message 
-00001400: 616e 6420 6578 6974 0a20 202d 5520 5520  and exit.  -U U 
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 2041 7574 6820 636f 6f6b 6965 2066 726f   Auth cookie fro
-00001430: 6d20 6272 6f77 7365 720a 2020 2d2d 636f  m browser.  --co
-00001440: 6f6b 6965 2d66 696c 6520 434f 4f4b 4945  okie-file COOKIE
-00001450: 5f46 494c 450a 2020 2020 2020 2020 2020  _FILE.          
-00001460: 2020 2020 2020 2020 2020 2020 2020 4669                Fi
-00001470: 6c65 2063 6f6e 7461 696e 696e 6720 6175  le containing au
-00001480: 7468 2063 6f6f 6b69 650a 2020 2d2d 7072  th cookie.  --pr
-00001490: 6f6d 7074 2050 524f 4d50 5420 2020 2020  ompt PROMPT     
-000014a0: 2020 5072 6f6d 7074 2074 6f20 6765 6e65    Prompt to gene
-000014b0: 7261 7465 2069 6d61 6765 7320 666f 720a  rate images for.
-000014c0: 2020 2d2d 6f75 7470 7574 2d64 6972 204f    --output-dir O
-000014d0: 5554 5055 545f 4449 520a 2020 2020 2020  UTPUT_DIR.      
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 4f75 7470 7574 2064 6972 6563 746f    Output directo
-00001500: 7279 0a20 202d 2d71 7569 6574 2020 2020  ry.  --quiet    
-00001510: 2020 2020 2020 2020 2020 2044 6973 6162             Disab
-00001520: 6c65 2070 6970 656c 696e 6520 6d65 7373  le pipeline mess
-00001530: 6167 6573 0a20 202d 2d61 7379 6e63 696f  ages.  --asyncio
-00001540: 2020 2020 2020 2020 2020 2020 2052 756e               Run
-00001550: 2049 6d61 6765 4765 6e20 7573 696e 6720   ImageGen using 
-00001560: 6173 796e 6369 6f0a 6060 600a 0a23 2320  asyncio.```..## 
-00001570: 5275 6e6e 696e 6720 696e 2050 7974 686f  Running in Pytho
-00001580: 6e0a 0a23 2323 2031 2920 5468 6520 6049  n..### 1) The `I
-00001590: 6d61 6765 5175 6572 7960 2068 656c 7065  mageQuery` helpe
-000015a0: 7220 636c 6173 730a 0a47 656e 6572 6174  r class..Generat
-000015b0: 6520 696d 6167 6573 2062 6173 6564 206f  e images based o
-000015c0: 6e20 6120 7369 6d70 6c65 2070 726f 6d70  n a simple promp
-000015d0: 7420 616e 6420 646f 776e 6c6f 6164 2074  t and download t
-000015e0: 6f20 7468 6520 6375 7272 656e 7420 776f  o the current wo
-000015f0: 726b 696e 6720 6469 7265 6374 6f72 793a  rking directory:
-00001600: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00001610: 2045 6467 6547 5054 2069 6d70 6f72 7420   EdgeGPT import 
-00001620: 496d 6167 6551 7565 7279 0a0a 713d 496d  ImageQuery..q=Im
-00001630: 6167 6551 7565 7279 2822 4d65 6572 6b61  ageQuery("Meerka
-00001640: 7473 2061 7420 6120 6761 7264 656e 2070  ts at a garden p
-00001650: 6172 7479 2069 6e20 4465 766f 6e22 290a  arty in Devon").
-00001660: 6060 600a 0a43 6861 6e67 6520 7468 6520  ```..Change the 
-00001670: 646f 776e 6c6f 6164 2064 6972 6563 746f  download directo
-00001680: 7279 2066 6f72 2061 6c6c 2066 7574 7572  ry for all futur
-00001690: 6520 696d 6167 6573 2069 6e20 7468 6973  e images in this
-000016a0: 2073 6573 7369 6f6e 3a0a 0a60 6060 0a51   session:..```.Q
-000016b0: 7565 7279 2e69 6d61 6765 5f64 6972 7061  uery.image_dirpa
-000016c0: 7468 203d 2050 6174 6828 222e 2f74 6f5f  th = Path("./to_
-000016d0: 616e 6f74 6865 725f 666f 6c64 6572 2229  another_folder")
-000016e0: 0a60 6060 0a0a 2323 2320 3229 2054 6865  .```..### 2) The
-000016f0: 2060 496d 6167 6547 656e 6020 636c 6173   `ImageGen` clas
-00001700: 7320 616e 6420 6061 7379 6e63 696f 6020  s and `asyncio` 
-00001710: 666f 7220 6d6f 7265 2067 7261 6e75 6c61  for more granula
-00001720: 7220 636f 6e74 726f 6c0a 0a60 6060 7079  r control..```py
-00001730: 7468 6f6e 0a66 726f 6d20 496d 6167 6547  thon.from ImageG
-00001740: 656e 2069 6d70 6f72 7420 496d 6167 6547  en import ImageG
-00001750: 656e 0a69 6d70 6f72 7420 6172 6770 6172  en.import argpar
-00001760: 7365 0a69 6d70 6f72 7420 6a73 6f6e 0a0a  se.import json..
-00001770: 6173 796e 6320 6465 6620 6173 796e 635f  async def async_
-00001780: 696d 6167 655f 6765 6e28 6172 6773 2920  image_gen(args) 
-00001790: 2d3e 204e 6f6e 653a 0a20 2020 2061 7379  -> None:.    asy
-000017a0: 6e63 2077 6974 6820 496d 6167 6547 656e  nc with ImageGen
-000017b0: 4173 796e 6328 6172 6773 2e55 2c20 6172  Async(args.U, ar
-000017c0: 6773 2e71 7569 6574 2920 6173 2069 6d61  gs.quiet) as ima
-000017d0: 6765 5f67 656e 6572 6174 6f72 3a0a 2020  ge_generator:.  
-000017e0: 2020 2020 2020 696d 6167 6573 203d 2061        images = a
-000017f0: 7761 6974 2069 6d61 6765 5f67 656e 6572  wait image_gener
-00001800: 6174 6f72 2e67 6574 5f69 6d61 6765 7328  ator.get_images(
-00001810: 6172 6773 2e70 726f 6d70 7429 0a20 2020  args.prompt).   
-00001820: 2020 2020 2061 7761 6974 2069 6d61 6765       await image
-00001830: 5f67 656e 6572 6174 6f72 2e73 6176 655f  _generator.save_
-00001840: 696d 6167 6573 2869 6d61 6765 732c 206f  images(images, o
-00001850: 7574 7075 745f 6469 723d 6172 6773 2e6f  utput_dir=args.o
-00001860: 7574 7075 745f 6469 7229 0a0a 6966 205f  utput_dir)..if _
-00001870: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00001880: 696e 5f5f 223a 0a20 2020 2070 6172 7365  in__":.    parse
-00001890: 7220 3d20 6172 6770 6172 7365 2e41 7267  r = argparse.Arg
-000018a0: 756d 656e 7450 6172 7365 7228 290a 2020  umentParser().  
-000018b0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-000018c0: 756d 656e 7428 222d 5522 2c20 6865 6c70  ument("-U", help
-000018d0: 3d22 4175 7468 2063 6f6f 6b69 6520 6672  ="Auth cookie fr
-000018e0: 6f6d 2062 726f 7773 6572 222c 2074 7970  om browser", typ
-000018f0: 653d 7374 7229 0a20 2020 2070 6172 7365  e=str).    parse
-00001900: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
-00001910: 2d2d 636f 6f6b 6965 2d66 696c 6522 2c20  --cookie-file", 
-00001920: 6865 6c70 3d22 4669 6c65 2063 6f6e 7461  help="File conta
-00001930: 696e 696e 6720 6175 7468 2063 6f6f 6b69  ining auth cooki
-00001940: 6522 2c20 7479 7065 3d73 7472 290a 2020  e", type=str).  
-00001950: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00001960: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
-00001970: 2d2d 7072 6f6d 7074 222c 0a20 2020 2020  --prompt",.     
-00001980: 2020 2068 656c 703d 2250 726f 6d70 7420     help="Prompt 
-00001990: 746f 2067 656e 6572 6174 6520 696d 6167  to generate imag
-000019a0: 6573 2066 6f72 222c 0a20 2020 2020 2020  es for",.       
-000019b0: 2074 7970 653d 7374 722c 0a20 2020 2020   type=str,.     
-000019c0: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
-000019d0: 2c0a 2020 2020 290a 2020 2020 7061 7273  ,.    ).    pars
-000019e0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-000019f0: 0a20 2020 2020 2020 2022 2d2d 6f75 7470  .        "--outp
-00001a00: 7574 2d64 6972 222c 0a20 2020 2020 2020  ut-dir",.       
-00001a10: 2068 656c 703d 224f 7574 7075 7420 6469   help="Output di
-00001a20: 7265 6374 6f72 7922 2c0a 2020 2020 2020  rectory",.      
-00001a30: 2020 7479 7065 3d73 7472 2c0a 2020 2020    type=str,.    
-00001a40: 2020 2020 6465 6661 756c 743d 222e 2f6f      default="./o
-00001a50: 7574 7075 7422 2c0a 2020 2020 290a 2020  utput",.    ).  
-00001a60: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00001a70: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
-00001a80: 2d2d 7175 6965 7422 2c20 6865 6c70 3d22  --quiet", help="
-00001a90: 4469 7361 626c 6520 7069 7065 6c69 6e65  Disable pipeline
-00001aa0: 206d 6573 7361 6765 7322 2c20 6163 7469   messages", acti
-00001ab0: 6f6e 3d22 7374 6f72 655f 7472 7565 220a  on="store_true".
-00001ac0: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
-00001ad0: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
-00001ae0: 2020 2020 2020 2022 2d2d 6173 796e 6369         "--asynci
-00001af0: 6f22 2c20 6865 6c70 3d22 5275 6e20 496d  o", help="Run Im
-00001b00: 6167 6547 656e 2075 7369 6e67 2061 7379  ageGen using asy
-00001b10: 6e63 696f 222c 2061 6374 696f 6e3d 2273  ncio", action="s
-00001b20: 746f 7265 5f74 7275 6522 0a20 2020 2029  tore_true".    )
-00001b30: 0a20 2020 2061 7267 7320 3d20 7061 7273  .    args = pars
-00001b40: 6572 2e70 6172 7365 5f61 7267 7328 290a  er.parse_args().
-00001b50: 2020 2020 2320 4c6f 6164 2061 7574 6820      # Load auth 
-00001b60: 636f 6f6b 6965 0a20 2020 2077 6974 6820  cookie.    with 
-00001b70: 6f70 656e 2861 7267 732e 636f 6f6b 6965  open(args.cookie
-00001b80: 5f66 696c 652c 2065 6e63 6f64 696e 673d  _file, encoding=
-00001b90: 2275 7466 2d38 2229 2061 7320 6669 6c65  "utf-8") as file
-00001ba0: 3a0a 2020 2020 2020 2020 636f 6f6b 6965  :.        cookie
-00001bb0: 5f6a 736f 6e20 3d20 6a73 6f6e 2e6c 6f61  _json = json.loa
-00001bc0: 6428 6669 6c65 290a 2020 2020 2020 2020  d(file).        
-00001bd0: 666f 7220 636f 6f6b 6965 2069 6e20 636f  for cookie in co
-00001be0: 6f6b 6965 5f6a 736f 6e3a 0a20 2020 2020  okie_json:.     
-00001bf0: 2020 2020 2020 2069 6620 636f 6f6b 6965         if cookie
-00001c00: 2e67 6574 2822 6e61 6d65 2229 203d 3d20  .get("name") == 
-00001c10: 225f 5522 3a0a 2020 2020 2020 2020 2020  "_U":.          
-00001c20: 2020 2020 2020 6172 6773 2e55 203d 2063        args.U = c
-00001c30: 6f6f 6b69 652e 6765 7428 2276 616c 7565  ookie.get("value
-00001c40: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00001c50: 2020 2062 7265 616b 0a0a 2020 2020 6966     break..    if
-00001c60: 2061 7267 732e 5520 6973 204e 6f6e 653a   args.U is None:
-00001c70: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
-00001c80: 7863 6570 7469 6f6e 2822 436f 756c 6420  xception("Could 
-00001c90: 6e6f 7420 6669 6e64 2061 7574 6820 636f  not find auth co
-00001ca0: 6f6b 6965 2229 0a0a 2020 2020 6966 206e  okie")..    if n
-00001cb0: 6f74 2061 7267 732e 6173 796e 6369 6f3a  ot args.asyncio:
-00001cc0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-00001cd0: 6520 696d 6167 6520 6765 6e65 7261 746f  e image generato
-00001ce0: 720a 2020 2020 2020 2020 696d 6167 655f  r.        image_
-00001cf0: 6765 6e65 7261 746f 7220 3d20 496d 6167  generator = Imag
-00001d00: 6547 656e 2861 7267 732e 552c 2061 7267  eGen(args.U, arg
-00001d10: 732e 7175 6965 7429 0a20 2020 2020 2020  s.quiet).       
-00001d20: 2069 6d61 6765 5f67 656e 6572 6174 6f72   image_generator
-00001d30: 2e73 6176 655f 696d 6167 6573 280a 2020  .save_images(.  
-00001d40: 2020 2020 2020 2020 2020 696d 6167 655f            image_
-00001d50: 6765 6e65 7261 746f 722e 6765 745f 696d  generator.get_im
-00001d60: 6167 6573 2861 7267 732e 7072 6f6d 7074  ages(args.prompt
-00001d70: 292c 0a20 2020 2020 2020 2020 2020 206f  ),.            o
-00001d80: 7574 7075 745f 6469 723d 6172 6773 2e6f  utput_dir=args.o
-00001d90: 7574 7075 745f 6469 722c 0a20 2020 2020  utput_dir,.     
-00001da0: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
-00001db0: 2020 2020 2020 2061 7379 6e63 696f 2e72         asyncio.r
-00001dc0: 756e 2861 7379 6e63 5f69 6d61 6765 5f67  un(async_image_g
-00001dd0: 656e 2861 7267 7329 290a 0a60 6060 0a0a  en(args))..```..
-00001de0: 3c2f 6465 7461 696c 733e 0a0a 2320 5374  </details>..# St
-00001df0: 6172 2048 6973 746f 7279 0a0a 5b21 5b53  ar History..[![S
-00001e00: 7461 7220 4869 7374 6f72 7920 4368 6172  tar History Char
-00001e10: 745d 2868 7474 7073 3a2f 2f61 7069 2e73  t](https://api.s
-00001e20: 7461 722d 6869 7374 6f72 792e 636f 6d2f  tar-history.com/
-00001e30: 7376 673f 7265 706f 733d 6163 6865 6f6e  svg?repos=acheon
-00001e40: 6730 382f 4564 6765 4750 5426 7479 7065  g08/EdgeGPT&type
-00001e50: 3d44 6174 6529 5d28 6874 7470 733a 2f2f  =Date)](https://
-00001e60: 7374 6172 2d68 6973 746f 7279 2e63 6f6d  star-history.com
-00001e70: 2f23 6163 6865 6f6e 6730 382f 4564 6765  /#acheong08/Edge
-00001e80: 4750 5426 4461 7465 290a 0a23 2043 6f6e  GPT&Date)..# Con
-00001e90: 7472 6962 7574 6f72 730a 0a54 6869 7320  tributors..This 
-00001ea0: 7072 6f6a 6563 7420 6578 6973 7473 2074  project exists t
-00001eb0: 6861 6e6b 7320 746f 2061 6c6c 2074 6865  hanks to all the
-00001ec0: 2070 656f 706c 6520 7768 6f20 636f 6e74   people who cont
-00001ed0: 7269 6275 7465 2e0a 0a20 3c61 2068 7265  ribute... <a hre
-00001ee0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001ef0: 622e 636f 6d2f 6163 6865 6f6e 6730 382f  b.com/acheong08/
-00001f00: 4564 6765 4750 542f 6772 6170 6873 2f63  EdgeGPT/graphs/c
-00001f10: 6f6e 7472 6962 7574 6f72 7322 3e0a 2020  ontributors">.  
-00001f20: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001f30: 2f2f 636f 6e74 7269 622e 726f 636b 732f  //contrib.rocks/
-00001f40: 696d 6167 653f 7265 706f 3d61 6368 656f  image?repo=acheo
-00001f50: 6e67 3038 2f45 6467 6547 5054 2220 2f3e  ng08/EdgeGPT" />
-00001f60: 0a20 3c2f 613e 0a                        . </a>.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 4564 6765  : 2.1.Name: Edge
+00000020: 4750 540a 5665 7273 696f 6e3a 2030 2e36  GPT.Version: 0.6
+00000030: 2e33 0a53 756d 6d61 7279 3a20 5265 7665  .3.Summary: Reve
+00000040: 7273 6520 656e 6769 6e65 6572 6564 2045  rse engineered E
+00000050: 6467 6520 4368 6174 2041 5049 0a48 6f6d  dge Chat API.Hom
+00000060: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000070: 6769 7468 7562 2e63 6f6d 2f61 6368 656f  github.com/acheo
+00000080: 6e67 3038 2f45 6467 6547 5054 0a41 7574  ng08/EdgeGPT.Aut
+00000090: 686f 723a 2041 6e74 6f6e 696f 2043 6865  hor: Antonio Che
+000000a0: 6f6e 670a 4175 7468 6f72 2d65 6d61 696c  ong.Author-email
+000000b0: 3a20 6163 6865 6f6e 6740 7374 7564 656e  : acheong@studen
+000000c0: 742e 6461 6c61 742e 6f72 670a 4c69 6365  t.dalat.org.Lice
+000000d0: 6e73 653a 2047 4e55 2047 656e 6572 616c  nse: GNU General
+000000e0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000000f0: 7632 2e30 0a50 726f 6a65 6374 2d55 524c  v2.0.Project-URL
+00000100: 3a20 4275 6720 5265 706f 7274 2c20 6874  : Bug Report, ht
+00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000120: 2f61 6368 656f 6e67 3038 2f45 6467 6547  /acheong08/EdgeG
+00000130: 5054 2f69 7373 7565 732f 6e65 770a 436c  PT/issues/new.Cl
+00000140: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000150: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000160: 6420 3a3a 2054 6865 2055 6e6c 6963 656e  d :: The Unlicen
+00000170: 7365 2028 556e 6c69 6365 6e73 6529 0a43  se (Unlicense).C
+00000180: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00000190: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+000001a0: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
+000001b0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000001c0: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
+000001d0: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
+000001e0: 7320 3a3a 2050 7974 686f 6e20 4d6f 6475  s :: Python Modu
+000001f0: 6c65 730a 436c 6173 7369 6669 6572 3a20  les.Classifier: 
+00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000220: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+00000230: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000240: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000250: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000260: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000280: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000290: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002b0: 7974 686f 6e20 3a3a 2033 2e31 310a 4465  ython :: 3.11.De
+000002c0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000002d0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000002e0: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+000002f0: 6c65 3a20 4c49 4345 4e53 450a 0a3c 6469  le: LICENSE..<di
+00000300: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00000310: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
+00000320: 7470 733a 2f2f 736f 6369 616c 6966 792e  tps://socialify.
+00000330: 6769 742e 6369 2f61 6368 656f 6e67 3038  git.ci/acheong08
+00000340: 2f45 6467 6547 5054 2f69 6d61 6765 3f66  /EdgeGPT/image?f
+00000350: 6f6e 743d 496e 7465 7226 6c61 6e67 7561  ont=Inter&langua
+00000360: 6765 3d31 266c 6f67 6f3d 6874 7470 7325  ge=1&logo=https%
+00000370: 3341 2532 4625 3246 7570 6c6f 6164 2e77  3A%2F%2Fupload.w
+00000380: 696b 696d 6564 6961 2e6f 7267 2532 4677  ikimedia.org%2Fw
+00000390: 696b 6970 6564 6961 2532 4663 6f6d 6d6f  ikipedia%2Fcommo
+000003a0: 6e73 2532 4639 2532 4639 6325 3246 4269  ns%2F9%2F9c%2FBi
+000003b0: 6e67 5f46 6c75 656e 745f 4c6f 676f 2e73  ng_Fluent_Logo.s
+000003c0: 7667 266f 776e 6572 3d31 2670 6174 7465  vg&owner=1&patte
+000003d0: 726e 3d46 6c6f 6174 696e 6725 3230 436f  rn=Floating%20Co
+000003e0: 6773 2674 6865 6d65 3d41 7574 6f22 2061  gs&theme=Auto" a
+000003f0: 6c74 3d22 4564 6765 4750 5422 2077 6964  lt="EdgeGPT" wid
+00000400: 7468 3d22 3634 3022 2068 6569 6768 743d  th="640" height=
+00000410: 2233 3230 2220 2f3e 0a0a 2320 4564 6765  "320" />..# Edge
+00000420: 2047 5054 0a0a 5f54 6865 2072 6576 6572   GPT.._The rever
+00000430: 7365 2065 6e67 696e 6565 7269 6e67 2074  se engineering t
+00000440: 6865 2063 6861 7420 6665 6174 7572 6520  he chat feature 
+00000450: 6f66 2074 6865 206e 6577 2076 6572 7369  of the new versi
+00000460: 6f6e 206f 6620 4269 6e67 5f0a 0a3c 613e  on of Bing_..<a>
+00000470: 456e 676c 6973 683c 2f61 3e20 2d0a 3c61  English</a> -.<a
+00000480: 2068 7265 663d 222e 2f52 4541 444d 455f   href="./README_
+00000490: 7a68 2d63 6e2e 6d64 223e e7ae 80e4 bd93  zh-cn.md">......
+000004a0: e4b8 ade6 9687 3c2f 613e 202d 0a3c 6120  ......</a> -.<a 
+000004b0: 6872 6566 3d22 2e2f 5245 4144 4d45 5f7a  href="./README_z
+000004c0: 682d 7477 2e6d 6422 3ee7 b981 e9ab 94e4  h-tw.md">.......
+000004d0: b8ad e696 873c 2f61 3e20 2d0a 3c61 2068  .....</a> -.<a h
+000004e0: 7265 663d 222e 2f52 4541 444d 455f 6573  ref="./README_es
+000004f0: 2e6d 6422 3e45 7370 61c3 b16f 6c3c 2f61  .md">Espa..ol</a
+00000500: 3e20 2d0a 3c61 2068 7265 663d 222e 2f52  > -.<a href="./R
+00000510: 4541 444d 455f 6a61 2e6d 6422 3ee6 97a5  EADME_ja.md">...
+00000520: e69c ace8 aa9e 3c2f 613e 0a0a 3c2f 6469  ......</a>..</di
+00000530: 763e 0a0a 3c70 2061 6c69 676e 3d22 6365  v>..<p align="ce
+00000540: 6e74 6572 223e 0a20 203c 6120 6872 6566  nter">.  <a href
+00000550: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000560: 2e63 6f6d 2f61 6368 656f 6e67 3038 2f45  .com/acheong08/E
+00000570: 6467 6547 5054 223e 0a20 2020 203c 696d  dgeGPT">.    <im
+00000580: 6720 616c 743d 2250 7950 4920 7665 7273  g alt="PyPI vers
+00000590: 696f 6e22 2073 7263 3d22 6874 7470 733a  ion" src="https:
+000005a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000005b0: 2f70 7970 692f 762f 4564 6765 4750 5422  /pypi/v/EdgeGPT"
+000005c0: 3e0a 2020 3c2f 613e 0a20 203c 696d 6720  >.  </a>.  <img 
+000005d0: 616c 743d 2250 7974 686f 6e20 7665 7273  alt="Python vers
+000005e0: 696f 6e22 2073 7263 3d22 6874 7470 733a  ion" src="https:
+000005f0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000600: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
+00000610: 382b 2d62 6c75 652e 7376 6722 3e0a 2020  8+-blue.svg">.  
+00000620: 3c69 6d67 2061 6c74 3d22 546f 7461 6c20  <img alt="Total 
+00000630: 646f 776e 6c6f 6164 7322 2073 7263 3d22  downloads" src="
+00000640: 6874 7470 733a 2f2f 7374 6174 6963 2e70  https://static.p
+00000650: 6570 792e 7465 6368 2f62 6164 6765 2f65  epy.tech/badge/e
+00000660: 6467 6567 7074 223e 0a0a 3c2f 703e 0a0a  dgegpt">..</p>..
+00000670: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
+00000680: 6172 793e 0a0a 2320 5365 7475 700a 0a3c  ary>..# Setup..<
+00000690: 2f73 756d 6d61 7279 3e0a 0a23 2323 2049  /summary>..### I
+000006a0: 6e73 7461 6c6c 2070 6163 6b61 6765 0a0a  nstall package..
+000006b0: 6060 6062 6173 680a 7079 7468 6f6e 3320  ```bash.python3 
+000006c0: 2d6d 2070 6970 2069 6e73 7461 6c6c 2045  -m pip install E
+000006d0: 6467 6547 5054 202d 2d75 7067 7261 6465  dgeGPT --upgrade
+000006e0: 0a60 6060 0a0a 2323 2320 5265 7175 6972  .```..### Requir
+000006f0: 656d 656e 7473 0a0a 2d20 7079 7468 6f6e  ements..- python
+00000700: 2033 2e38 2b0a 2d20 4120 4d69 6372 6f73   3.8+.- A Micros
+00000710: 6f66 7420 4163 636f 756e 7420 7769 7468  oft Account with
+00000720: 2061 6363 6573 7320 746f 203c 6874 7470   access to <http
+00000730: 733a 2f2f 6269 6e67 2e63 6f6d 2f63 6861  s://bing.com/cha
+00000740: 743e 2028 4f70 7469 6f6e 616c 290a 2d20  t> (Optional).- 
+00000750: 5265 7175 6972 6564 2069 6e20 6120 7375  Required in a su
+00000760: 7070 6f72 7465 6420 636f 756e 7472 7920  pported country 
+00000770: 6f72 2072 6567 696f 6e20 7769 7468 204e  or region with N
+00000780: 6577 2042 696e 6720 2843 6869 6e65 7365  ew Bing (Chinese
+00000790: 206d 6169 6e6c 616e 6420 5650 4e20 7265   mainland VPN re
+000007a0: 7175 6972 6564 290a 2d20 5b53 656c 656e  quired).- [Selen
+000007b0: 6975 6d5d 2868 7474 7073 3a2f 2f70 7970  ium](https://pyp
+000007c0: 692e 6f72 672f 7072 6f6a 6563 742f 7365  i.org/project/se
+000007d0: 6c65 6e69 756d 2f29 2028 666f 7220 6175  lenium/) (for au
+000007e0: 746f 6d61 7469 6320 636f 6f6b 6965 2073  tomatic cookie s
+000007f0: 6574 7570 290a 0a3c 6465 7461 696c 733e  etup)..<details>
+00000800: 0a0a 3c73 756d 6d61 7279 3e0a 0a23 2043  ..<summary>..# C
+00000810: 6861 7462 6f74 0a0a 3c2f 7375 6d6d 6172  hatbot..</summar
+00000820: 793e 0a0a 2323 2041 7574 6865 6e74 6963  y>..## Authentic
+00000830: 6174 696f 6e0a 0a21 2121 204e 4f54 2052  ation..!!! NOT R
+00000840: 4551 5549 5245 4420 414e 594d 4f52 4520  EQUIRED ANYMORE 
+00000850: 2121 210a 4d69 6372 6f73 6f66 7420 6861  !!!.Microsoft ha
+00000860: 7320 6d61 6465 2074 6865 2063 6861 7420  s made the chat 
+00000870: 6665 6174 7572 6520 6176 6169 6c61 626c  feature availabl
+00000880: 6520 746f 2065 7665 7279 6f6e 652c 2073  e to everyone, s
+00000890: 6f20 796f 7520 6361 6e20 736b 6970 2074  o you can skip t
+000008a0: 6869 7320 7374 6570 2e0a 0a31 2e20 496e  his step...1. In
+000008b0: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
+000008c0: 2076 6572 7369 6f6e 206f 6620 4d69 6372   version of Micr
+000008d0: 6f73 6f66 7420 4564 6765 0a3c 6465 7461  osoft Edge.<deta
+000008e0: 696c 733e 0a0a 322e 2041 6c74 6572 6e61  ils>..2. Alterna
+000008f0: 7469 7665 6c79 2c20 796f 7520 6361 6e20  tively, you can 
+00000900: 7573 6520 616e 7920 6272 6f77 7365 7220  use any browser 
+00000910: 616e 6420 7365 7420 7468 6520 7573 6572  and set the user
+00000920: 2d61 6765 6e74 2074 6f20 6c6f 6f6b 206c  -agent to look l
+00000930: 696b 6520 796f 7527 7265 2075 7369 6e67  ike you're using
+00000940: 2045 6467 6520 2865 2e67 2e2c 2060 4d6f   Edge (e.g., `Mo
+00000950: 7a69 6c6c 612f 352e 3020 2857 696e 646f  zilla/5.0 (Windo
+00000960: 7773 204e 5420 3130 2e30 3b20 5769 6e36  ws NT 10.0; Win6
+00000970: 343b 2078 3634 2920 4170 706c 6557 6562  4; x64) AppleWeb
+00000980: 4b69 742f 3533 372e 3336 2028 4b48 544d  Kit/537.36 (KHTM
+00000990: 4c2c 206c 696b 6520 4765 636b 6f29 2043  L, like Gecko) C
+000009a0: 6872 6f6d 652f 3131 312e 302e 302e 3020  hrome/111.0.0.0 
+000009b0: 5361 6661 7269 2f35 3337 2e33 3620 4564  Safari/537.36 Ed
+000009c0: 672f 3131 312e 302e 3136 3631 2e35 3160  g/111.0.1661.51`
+000009d0: 292e 2059 6f75 2063 616e 2064 6f20 7468  ). You can do th
+000009e0: 6973 2065 6173 696c 7920 7769 7468 2061  is easily with a
+000009f0: 6e20 6578 7465 6e73 696f 6e20 6c69 6b65  n extension like
+00000a00: 2022 5573 6572 2d41 6765 6e74 2053 7769   "User-Agent Swi
+00000a10: 7463 6865 7220 616e 6420 4d61 6e61 6765  tcher and Manage
+00000a20: 7222 2066 6f72 205b 4368 726f 6d65 5d28  r" for [Chrome](
+00000a30: 6874 7470 733a 2f2f 6368 726f 6d65 2e67  https://chrome.g
+00000a40: 6f6f 676c 652e 636f 6d2f 7765 6273 746f  oogle.com/websto
+00000a50: 7265 2f64 6574 6169 6c2f 7573 6572 2d61  re/detail/user-a
+00000a60: 6765 6e74 2d73 7769 7463 6865 722d 616e  gent-switcher-an
+00000a70: 642d 6d2f 6268 6368 6463 656a 686f 6866  d-m/bhchdcejhohf
+00000a80: 6d69 676a 6166 6261 6d70 6f67 6d61 616e  migjafbampogmaan
+00000a90: 6266 6b67 2920 616e 6420 5b46 6972 6566  bfkg) and [Firef
+00000aa0: 6f78 5d28 6874 7470 733a 2f2f 6164 646f  ox](https://addo
+00000ab0: 6e73 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  ns.mozilla.org/e
+00000ac0: 6e2d 5553 2f66 6972 6566 6f78 2f61 6464  n-US/firefox/add
+00000ad0: 6f6e 2f75 7365 722d 6167 656e 742d 7374  on/user-agent-st
+00000ae0: 7269 6e67 2d73 7769 7463 6865 722f 292e  ring-switcher/).
+00000af0: 0a0a 3c2f 6465 7461 696c 733e 0a0a 332e  ..</details>..3.
+00000b00: 204f 7065 6e20 5b62 696e 672e 636f 6d2f   Open [bing.com/
+00000b10: 6368 6174 5d28 6874 7470 733a 2f2f 6269  chat](https://bi
+00000b20: 6e67 2e63 6f6d 2f63 6861 7429 0a34 2e20  ng.com/chat).4. 
+00000b30: 4966 2079 6f75 2073 6565 2061 2063 6861  If you see a cha
+00000b40: 7420 6665 6174 7572 652c 2079 6f75 2061  t feature, you a
+00000b50: 7265 2067 6f6f 6420 746f 2063 6f6e 7469  re good to conti
+00000b60: 6e75 652e 2e2e 0a35 2e20 496e 7374 616c  nue....5. Instal
+00000b70: 6c20 7468 6520 636f 6f6b 6965 2065 6469  l the cookie edi
+00000b80: 746f 7220 6578 7465 6e73 696f 6e20 666f  tor extension fo
+00000b90: 7220 5b43 6872 6f6d 655d 2868 7474 7073  r [Chrome](https
+00000ba0: 3a2f 2f63 6872 6f6d 652e 676f 6f67 6c65  ://chrome.google
+00000bb0: 2e63 6f6d 2f77 6562 7374 6f72 652f 6465  .com/webstore/de
+00000bc0: 7461 696c 2f63 6f6f 6b69 652d 6564 6974  tail/cookie-edit
+00000bd0: 6f72 2f68 6c6b 656e 6e64 6564 6e68 666b  or/hlkenndednhfk
+00000be0: 656b 6867 6364 6963 6466 6464 6e6b 616c  ekhgcdicdfddnkal
+00000bf0: 6d64 6d29 206f 7220 5b46 6972 6566 6f78  mdm) or [Firefox
+00000c00: 5d28 6874 7470 733a 2f2f 6164 646f 6e73  ](https://addons
+00000c10: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00000c20: 5553 2f66 6972 6566 6f78 2f61 6464 6f6e  US/firefox/addon
+00000c30: 2f63 6f6f 6b69 652d 6564 6974 6f72 2f29  /cookie-editor/)
+00000c40: 0a36 2e20 476f 2074 6f20 5b62 696e 672e  .6. Go to [bing.
+00000c50: 636f 6d5d 2868 7474 7073 3a2f 2f62 696e  com](https://bin
+00000c60: 672e 636f 6d29 0a37 2e20 4f70 656e 2074  g.com).7. Open t
+00000c70: 6865 2065 7874 656e 7369 6f6e 0a38 2e20  he extension.8. 
+00000c80: 436c 6963 6b20 2245 7870 6f72 7422 206f  Click "Export" o
+00000c90: 6e20 7468 6520 626f 7474 6f6d 2072 6967  n the bottom rig
+00000ca0: 6874 2c20 7468 656e 2022 4578 706f 7274  ht, then "Export
+00000cb0: 2061 7320 4a53 4f4e 2220 2854 6869 7320   as JSON" (This 
+00000cc0: 7361 7665 7320 796f 7572 2063 6f6f 6b69  saves your cooki
+00000cd0: 6573 2074 6f20 636c 6970 626f 6172 6429  es to clipboard)
+00000ce0: 0a39 2e20 5061 7374 6520 796f 7572 2063  .9. Paste your c
+00000cf0: 6f6f 6b69 6573 2069 6e74 6f20 6120 6669  ookies into a fi
+00000d00: 6c65 2060 636f 6f6b 6965 732e 6a73 6f6e  le `cookies.json
+00000d10: 600a 0a23 2323 2049 6e20 636f 6465 3a0a  `..### In code:.
+00000d20: 6060 6070 7974 686f 6e0a 636f 6f6b 6965  ```python.cookie
+00000d30: 7320 3d20 6a73 6f6e 2e6c 6f61 6473 286f  s = json.loads(o
+00000d40: 7065 6e28 222e 2f70 6174 682f 746f 2f63  pen("./path/to/c
+00000d50: 6f6f 6b69 6573 2e6a 736f 6e22 2c20 656e  ookies.json", en
+00000d60: 636f 6469 6e67 3d22 7574 662d 3822 292e  coding="utf-8").
+00000d70: 7265 6164 2829 290a 626f 7420 3d20 6177  read()).bot = aw
+00000d80: 6169 7420 4368 6174 626f 742e 6372 6561  ait Chatbot.crea
+00000d90: 7465 2863 6f6f 6b69 6573 3d63 6f6f 6b69  te(cookies=cooki
+00000da0: 6573 290a 6060 600a 0a23 2320 5275 6e6e  es).```..## Runn
+00000db0: 696e 6720 6672 6f6d 2074 6865 2043 6f6d  ing from the Com
+00000dc0: 6d61 6e64 204c 696e 650a 0a60 6060 0a20  mand Line..```. 
+00000dd0: 2420 7079 7468 6f6e 3320 2d6d 2045 6467  $ python3 -m Edg
+00000de0: 6547 5054 202d 680a 0a20 2020 2020 2020  eGPT -h..       
+00000df0: 2045 6467 6547 5054 202d 2041 2064 656d   EdgeGPT - A dem
+00000e00: 6f20 6f66 2072 6576 6572 7365 2065 6e67  o of reverse eng
+00000e10: 696e 6565 7269 6e67 2074 6865 2042 696e  ineering the Bin
+00000e20: 6720 4750 5420 6368 6174 626f 740a 2020  g GPT chatbot.  
+00000e30: 2020 2020 2020 5265 706f 3a20 6769 7468        Repo: gith
+00000e40: 7562 2e63 6f6d 2f61 6368 656f 6e67 3038  ub.com/acheong08
+00000e50: 2f45 6467 6547 5054 0a20 2020 2020 2020  /EdgeGPT.       
+00000e60: 2042 793a 2041 6e74 6f6e 696f 2043 6865   By: Antonio Che
+00000e70: 6f6e 670a 0a20 2020 2020 2020 2021 6865  ong..        !he
+00000e80: 6c70 2066 6f72 2068 656c 700a 0a20 2020  lp for help..   
+00000e90: 2020 2020 2054 7970 6520 2165 7869 7420       Type !exit 
+00000ea0: 746f 2065 7869 740a 2020 2020 2020 2020  to exit.        
+00000eb0: 456e 7465 7220 7477 6963 6520 746f 2073  Enter twice to s
+00000ec0: 656e 6420 6d65 7373 6167 6520 6f72 2073  end message or s
+00000ed0: 6574 202d 2d65 6e74 6572 2d6f 6e63 6520  et --enter-once 
+00000ee0: 746f 2073 656e 6420 6f6e 6520 6c69 6e65  to send one line
+00000ef0: 206d 6573 7361 6765 0a0a 7573 6167 653a   message..usage:
+00000f00: 2045 6467 6547 5054 2e70 7920 5b2d 685d   EdgeGPT.py [-h]
+00000f10: 205b 2d2d 656e 7465 722d 6f6e 6365 5d20   [--enter-once] 
+00000f20: 5b2d 2d6e 6f2d 7374 7265 616d 5d20 5b2d  [--no-stream] [-
+00000f30: 2d72 6963 685d 205b 2d2d 7072 6f78 7920  -rich] [--proxy 
+00000f40: 5052 4f58 595d 205b 2d2d 7374 796c 6520  PROXY] [--style 
+00000f50: 7b63 7265 6174 6976 652c 6261 6c61 6e63  {creative,balanc
+00000f60: 6564 2c70 7265 6369 7365 7d5d 0a0a 6f70  ed,precise}]..op
+00000f70: 7469 6f6e 733a 0a20 202d 682c 202d 2d68  tions:.  -h, --h
+00000f80: 656c 7020 2020 2020 2020 2020 2020 2073  elp            s
+00000f90: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+00000fa0: 7373 6167 6520 616e 6420 6578 6974 0a20  ssage and exit. 
+00000fb0: 202d 2d65 6e74 6572 2d6f 6e63 650a 2020   --enter-once.  
+00000fc0: 2d2d 6e6f 2d73 7472 6561 6d0a 2020 2d2d  --no-stream.  --
+00000fd0: 7269 6368 0a20 202d 2d70 726f 7879 2050  rich.  --proxy P
+00000fe0: 524f 5859 2020 2020 2020 2020 2050 726f  ROXY         Pro
+00000ff0: 7879 2055 524c 2028 652e 672e 2073 6f63  xy URL (e.g. soc
+00001000: 6b73 353a 2f2f 3132 372e 302e 302e 313a  ks5://127.0.0.1:
+00001010: 3130 3830 290a 2020 2d2d 7374 796c 6520  1080).  --style 
+00001020: 7b63 7265 6174 6976 652c 6261 6c61 6e63  {creative,balanc
+00001030: 6564 2c70 7265 6369 7365 7d0a 2020 2d2d  ed,precise}.  --
+00001040: 636f 6f6b 6965 2d66 696c 6520 5b70 6174  cookie-file [pat
+00001050: 682f 746f 2f63 6f6f 6b69 6573 2e6a 736f  h/to/cookies.jso
+00001060: 6e5d 0a60 6060 0a0a 2323 2052 756e 6e69  n].```..## Runni
+00001070: 6e67 2069 6e20 5079 7468 6f6e 0a0a 2323  ng in Python..##
+00001080: 2320 312e 2054 6865 2060 4368 6174 626f  # 1. The `Chatbo
+00001090: 7460 2063 6c61 7373 2061 6e64 2060 6173  t` class and `as
+000010a0: 796e 6369 6f60 2066 6f72 206d 6f72 6520  yncio` for more 
+000010b0: 6772 616e 756c 6172 2063 6f6e 7472 6f6c  granular control
+000010c0: 0a0a 5573 6520 4173 796e 6320 666f 7220  ..Use Async for 
+000010d0: 7468 6520 6265 7374 2065 7870 6572 6965  the best experie
+000010e0: 6e63 652c 2066 6f72 2065 7861 6d70 6c65  nce, for example
+000010f0: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
+00001100: 6f72 7420 6173 796e 6369 6f0a 6672 6f6d  ort asyncio.from
+00001110: 2045 6467 6547 5054 2069 6d70 6f72 7420   EdgeGPT import 
+00001120: 4368 6174 626f 742c 2043 6f6e 7665 7273  Chatbot, Convers
+00001130: 6174 696f 6e53 7479 6c65 0a0a 6173 796e  ationStyle..asyn
+00001140: 6320 6465 6620 6d61 696e 2829 3a0a 2020  c def main():.  
+00001150: 2020 626f 7420 3d20 6177 6169 7420 4368    bot = await Ch
+00001160: 6174 626f 742e 6372 6561 7465 2829 2023  atbot.create() #
+00001170: 2050 6173 7369 6e67 2063 6f6f 6b69 6573   Passing cookies
+00001180: 2069 7320 6f70 7469 6f6e 616c 0a20 2020   is optional.   
+00001190: 2070 7269 6e74 2861 7761 6974 2062 6f74   print(await bot
+000011a0: 2e61 736b 2870 726f 6d70 743d 2248 656c  .ask(prompt="Hel
+000011b0: 6c6f 2077 6f72 6c64 222c 2063 6f6e 7665  lo world", conve
+000011c0: 7273 6174 696f 6e5f 7374 796c 653d 436f  rsation_style=Co
+000011d0: 6e76 6572 7361 7469 6f6e 5374 796c 652e  nversationStyle.
+000011e0: 6372 6561 7469 7665 2929 0a20 2020 2061  creative)).    a
+000011f0: 7761 6974 2062 6f74 2e63 6c6f 7365 2829  wait bot.close()
+00001200: 0a0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00001210: 2022 5f5f 6d61 696e 5f5f 223a 0a20 2020   "__main__":.   
+00001220: 2061 7379 6e63 696f 2e72 756e 286d 6169   asyncio.run(mai
+00001230: 6e28 2929 0a60 6060 0a0a 3c64 6574 6169  n()).```..<detai
+00001240: 6c73 3e0a 3c73 756d 6d61 7279 3e0a 0a23  ls>.<summary>..#
+00001250: 2323 2032 2920 5468 6520 6051 7565 7279  ## 2) The `Query
+00001260: 6020 616e 6420 6043 6f6f 6b69 6560 2068  ` and `Cookie` h
+00001270: 656c 7065 7220 636c 6173 7365 730a 0a20  elper classes.. 
+00001280: 203c 2f73 756d 6d61 7279 3e0a 0a43 7265   </summary>..Cre
+00001290: 6174 6520 6120 7369 6d70 6c65 2042 696e  ate a simple Bin
+000012a0: 6720 4368 6174 2041 4920 7175 6572 7920  g Chat AI query 
+000012b0: 2875 7369 6e67 2074 6865 2027 7072 6563  (using the 'prec
+000012c0: 6973 6527 2063 6f6e 7665 7273 6174 696f  ise' conversatio
+000012d0: 6e20 7374 796c 6520 6279 2064 6566 6175  n style by defau
+000012e0: 6c74 2920 616e 6420 7365 6520 6a75 7374  lt) and see just
+000012f0: 2074 6865 206d 6169 6e20 7465 7874 206f   the main text o
+00001300: 7574 7075 7420 7261 7468 6572 2074 6861  utput rather tha
+00001310: 6e20 7468 6520 7768 6f6c 6520 4150 4920  n the whole API 
+00001320: 7265 7370 6f6e 7365 3a0a 0a60 6060 7079  response:..```py
+00001330: 7468 6f6e 0a66 726f 6d20 4564 6765 4750  thon.from EdgeGP
+00001340: 5420 696d 706f 7274 2051 7565 7279 2c20  T import Query, 
+00001350: 436f 6f6b 6965 0a0a 7120 3d20 5175 6572  Cookie..q = Quer
+00001360: 7928 2257 6861 7420 6172 6520 796f 753f  y("What are you?
+00001370: 2047 6976 6520 796f 7572 2061 6e73 7765   Give your answe
+00001380: 7220 6173 2050 7974 686f 6e20 636f 6465  r as Python code
+00001390: 2229 0a70 7269 6e74 2871 290a 6060 600a  ").print(q).```.
+000013a0: 0a4f 7220 6368 616e 6765 2074 6865 2063  .Or change the c
+000013b0: 6f6e 7665 7273 6174 696f 6e20 7374 796c  onversation styl
+000013c0: 6520 6f72 2063 6f6f 6b69 6520 6669 6c65  e or cookie file
+000013d0: 2074 6f20 6265 2075 7365 643a 0a0a 6060   to be used:..``
+000013e0: 6070 7974 686f 6e0a 7120 3d20 5175 6572  `python.q = Quer
+000013f0: 7928 0a20 2022 5768 6174 2061 7265 2079  y(.  "What are y
+00001400: 6f75 3f20 4769 7665 2079 6f75 7220 616e  ou? Give your an
+00001410: 7377 6572 2061 7320 5079 7468 6f6e 2063  swer as Python c
+00001420: 6f64 6522 2c0a 2020 7374 796c 653d 2263  ode",.  style="c
+00001430: 7265 6174 6976 6522 2c20 2023 206f 7220  reative",  # or 
+00001440: 2762 616c 616e 6365 6427 0a20 2063 6f6f  'balanced'.  coo
+00001450: 6b69 6573 3d22 2e2f 6269 6e67 5f63 6f6f  kies="./bing_coo
+00001460: 6b69 6573 5f61 6c74 6572 6e61 7469 7665  kies_alternative
+00001470: 2e6a 736f 6e22 0a29 0a60 6060 0a0a 5175  .json".).```..Qu
+00001480: 6963 6b6c 7920 6578 7472 6163 7420 7468  ickly extract th
+00001490: 6520 7465 7874 206f 7574 7075 742c 2063  e text output, c
+000014a0: 6f64 6520 736e 6970 7065 7473 2c20 6c69  ode snippets, li
+000014b0: 7374 206f 6620 736f 7572 6365 732f 7265  st of sources/re
+000014c0: 6665 7265 6e63 6573 2c20 6f72 2073 7567  ferences, or sug
+000014d0: 6765 7374 6564 2066 6f6c 6c6f 772d 6f6e  gested follow-on
+000014e0: 2071 7565 7374 696f 6e73 2075 7369 6e67   questions using
+000014f0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2061   the following a
+00001500: 7474 7269 6275 7465 733a 0a0a 6060 6070  ttributes:..```p
+00001510: 7974 686f 6e0a 712e 6f75 7470 7574 0a71  ython.q.output.q
+00001520: 2e63 6f64 650a 712e 7375 6767 6573 7469  .code.q.suggesti
+00001530: 6f6e 730a 712e 736f 7572 6365 7320 2020  ons.q.sources   
+00001540: 2020 2020 2320 666f 7220 7468 6520 6675      # for the fu
+00001550: 6c6c 206a 736f 6e20 6f75 7470 7574 0a71  ll json output.q
+00001560: 2e73 6f75 7263 6573 5f64 6963 7420 2023  .sources_dict  #
+00001570: 2066 6f72 2061 2064 6963 7469 6f6e 6172   for a dictionar
+00001580: 7920 6f66 2074 6974 6c65 7320 616e 6420  y of titles and 
+00001590: 7572 6c73 0a60 6060 0a0a 4765 7420 7468  urls.```..Get th
+000015a0: 6520 6f72 6769 6e61 6c20 7072 6f6d 7074  e orginal prompt
+000015b0: 2061 6e64 2074 6865 2063 6f6e 7665 7273   and the convers
+000015c0: 6174 696f 6e20 7374 796c 6520 796f 7520  ation style you 
+000015d0: 7370 6563 6966 6965 643a 0a0a 6060 6070  specified:..```p
+000015e0: 7974 686f 6e0a 712e 7072 6f6d 7074 0a71  ython.q.prompt.q
+000015f0: 2e73 7479 6c65 0a72 6570 7228 7129 0a60  .style.repr(q).`
+00001600: 6060 0a0a 4163 6365 7373 2070 7265 7669  ``..Access previ
+00001610: 6f75 7320 5175 6572 6965 7320 6d61 6465  ous Queries made
+00001620: 2073 696e 6365 2069 6d70 6f72 7469 6e67   since importing
+00001630: 2060 5175 6572 7960 3a0a 0a60 6060 7079   `Query`:..```py
+00001640: 7468 6f6e 0a51 7565 7279 2e69 6e64 6578  thon.Query.index
+00001650: 2020 2320 4120 6c69 7374 206f 6620 5175    # A list of Qu
+00001660: 6572 7920 6f62 6a65 6374 733b 2075 7064  ery objects; upd
+00001670: 6174 6564 2064 796e 616d 6963 616c 6c79  ated dynamically
+00001680: 0a51 7565 7279 2e72 6571 7565 7374 5f63  .Query.request_c
+00001690: 6f75 6e74 2020 2320 4120 7461 6c6c 7920  ount  # A tally 
+000016a0: 6f66 2072 6571 7565 7374 7320 6d61 6465  of requests made
+000016b0: 2075 7369 6e67 2065 6163 6820 636f 6f6b   using each cook
+000016c0: 6965 2066 696c 650a 6060 600a 0a41 6e64  ie file.```..And
+000016d0: 2066 696e 616c 6c79 2c20 7468 6520 6043   finally, the `C
+000016e0: 6f6f 6b69 6560 2063 6c61 7373 2073 7570  ookie` class sup
+000016f0: 706f 7274 7320 6d75 6c74 6970 6c65 2063  ports multiple c
+00001700: 6f6f 6b69 6520 6669 6c65 732c 2073 6f20  ookie files, so 
+00001710: 6966 2079 6f75 2063 7265 6174 6520 6164  if you create ad
+00001720: 6469 7469 6f6e 616c 2063 6f6f 6b69 6520  ditional cookie 
+00001730: 6669 6c65 7320 7769 7468 2074 6865 206e  files with the n
+00001740: 616d 696e 6720 636f 6e76 656e 7469 6f6e  aming convention
+00001750: 2060 6269 6e67 5f63 6f6f 6b69 6573 5f2a   `bing_cookies_*
+00001760: 2e6a 736f 6e60 2c20 796f 7572 2071 7565  .json`, your que
+00001770: 7269 6573 2077 696c 6c20 6175 746f 6d61  ries will automa
+00001780: 7469 6361 6c6c 7920 7472 7920 7573 696e  tically try usin
+00001790: 6720 7468 6520 6e65 7874 2066 696c 6520  g the next file 
+000017a0: 2861 6c70 6861 6265 7469 6361 6c6c 7929  (alphabetically)
+000017b0: 2069 6620 796f 7527 7665 2065 7863 6565   if you've excee
+000017c0: 6465 6420 796f 7572 2064 6169 6c79 2071  ded your daily q
+000017d0: 756f 7461 206f 6620 7265 7175 6573 7473  uota of requests
+000017e0: 2028 6375 7272 656e 746c 7920 7365 7420   (currently set 
+000017f0: 6174 2032 3030 292e 0a0a 4865 7265 2061  at 200)...Here a
+00001800: 7265 2074 6865 206d 6169 6e20 6174 7472  re the main attr
+00001810: 6962 7574 6573 2077 6869 6368 2079 6f75  ibutes which you
+00001820: 2063 616e 2061 6363 6573 733a 0a0a 6060   can access:..``
+00001830: 6070 7974 686f 6e0a 436f 6f6b 6965 2e63  `python.Cookie.c
+00001840: 7572 7265 6e74 5f66 696c 655f 696e 6465  urrent_file_inde
+00001850: 780a 436f 6f6b 6965 2e64 6972 7061 7468  x.Cookie.dirpath
+00001860: 0a43 6f6f 6b69 652e 7365 6172 6368 5f70  .Cookie.search_p
+00001870: 6174 7465 726e 2020 2320 6465 6661 756c  attern  # defaul
+00001880: 7420 6973 2060 6269 6e67 5f63 6f6f 6b69  t is `bing_cooki
+00001890: 6573 5f2a 2e6a 736f 6e60 0a43 6f6f 6b69  es_*.json`.Cooki
+000018a0: 652e 6669 6c65 7328 2920 2023 206c 6973  e.files()  # lis
+000018b0: 7420 6173 2066 696c 6573 2074 6861 7420  t as files that 
+000018c0: 6d61 7463 6820 2e73 6561 7263 685f 7061  match .search_pa
+000018d0: 7474 6572 6e0a 436f 6f6b 6965 2e63 7572  ttern.Cookie.cur
+000018e0: 7265 6e74 5f66 696c 6570 6174 680a 436f  rent_filepath.Co
+000018f0: 6f6b 6965 2e63 7572 7265 6e74 5f64 6174  okie.current_dat
+00001900: 610a 436f 6f6b 6965 2e69 6d70 6f72 745f  a.Cookie.import_
+00001910: 6e65 7874 2829 0a43 6f6f 6b69 652e 696d  next().Cookie.im
+00001920: 6167 655f 746f 6b65 6e0a 436f 6f6b 6965  age_token.Cookie
+00001930: 2e69 676e 6f72 655f 6669 6c65 730a 6060  .ignore_files.``
+00001940: 600a 0a3c 2f64 6574 6169 6c73 3e0a 0a2d  `..</details>..-
+00001950: 2d2d 0a0a 2323 2052 756e 6e69 6e67 2077  --..## Running w
+00001960: 6974 6820 446f 636b 6572 0a0a 5468 6973  ith Docker..This
+00001970: 2061 7373 756d 6573 2079 6f75 2068 6176   assumes you hav
+00001980: 6520 6120 6669 6c65 2063 6f6f 6b69 6573  e a file cookies
+00001990: 2e6a 736f 6e20 696e 2079 6f75 7220 6375  .json in your cu
+000019a0: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
+000019b0: 7265 6374 6f72 790a 0a60 6060 6261 7368  rectory..```bash
+000019c0: 0a0a 646f 636b 6572 2072 756e 202d 2d72  ..docker run --r
+000019d0: 6d20 2d69 7420 2d76 2024 2870 7764 292f  m -it -v $(pwd)/
+000019e0: 636f 6f6b 6965 732e 6a73 6f6e 3a2f 636f  cookies.json:/co
+000019f0: 6f6b 6965 732e 6a73 6f6e 3a72 6f20 2d65  okies.json:ro -e
+00001a00: 2043 4f4f 4b49 455f 4649 4c45 3d27 2f63   COOKIE_FILE='/c
+00001a10: 6f6f 6b69 6573 2e6a 736f 6e27 2067 6863  ookies.json' ghc
+00001a20: 722e 696f 2f61 6368 656f 6e67 3038 2f65  r.io/acheong08/e
+00001a30: 6467 6567 7074 0a60 6060 0a0a 596f 7520  dgegpt.```..You 
+00001a40: 6361 6e20 6164 6420 616e 7920 6578 7472  can add any extr
+00001a50: 6120 666c 6167 7320 6173 2066 6f6c 6c6f  a flags as follo
+00001a60: 7769 6e67 0a0a 6060 6062 6173 680a 0a64  wing..```bash..d
+00001a70: 6f63 6b65 7220 7275 6e20 2d2d 726d 202d  ocker run --rm -
+00001a80: 6974 202d 7620 2428 7077 6429 2f63 6f6f  it -v $(pwd)/coo
+00001a90: 6b69 6573 2e6a 736f 6e3a 2f63 6f6f 6b69  kies.json:/cooki
+00001aa0: 6573 2e6a 736f 6e3a 726f 202d 6520 434f  es.json:ro -e CO
+00001ab0: 4f4b 4945 5f46 494c 453d 272f 636f 6f6b  OKIE_FILE='/cook
+00001ac0: 6965 732e 6a73 6f6e 2720 6768 6372 2e69  ies.json' ghcr.i
+00001ad0: 6f2f 6163 6865 6f6e 6730 382f 6564 6765  o/acheong08/edge
+00001ae0: 6770 7420 2d2d 7269 6368 202d 2d73 7479  gpt --rich --sty
+00001af0: 6c65 2063 7265 6174 6976 650a 6060 600a  le creative.```.
+00001b00: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00001b10: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
+00001b20: 3e0a 0a23 2049 6d61 6765 2067 656e 6572  >..# Image gener
+00001b30: 6174 6f72 0a0a 3c2f 7375 6d6d 6172 793e  ator..</summary>
+00001b40: 0a0a 2323 2052 756e 6e69 6e67 2066 726f  ..## Running fro
+00001b50: 6d20 7468 6520 436f 6d6d 616e 6420 4c69  m the Command Li
+00001b60: 6e65 0a0a 6060 6062 6173 680a 2420 7079  ne..```bash.$ py
+00001b70: 7468 6f6e 3320 2d6d 2049 6d61 6765 4765  thon3 -m ImageGe
+00001b80: 6e20 2d68 0a75 7361 6765 3a20 496d 6167  n -h.usage: Imag
+00001b90: 6547 656e 2e70 7920 5b2d 685d 205b 2d55  eGen.py [-h] [-U
+00001ba0: 2055 5d20 5b2d 2d63 6f6f 6b69 652d 6669   U] [--cookie-fi
+00001bb0: 6c65 2043 4f4f 4b49 455f 4649 4c45 5d20  le COOKIE_FILE] 
+00001bc0: 2d2d 7072 6f6d 7074 2050 524f 4d50 5420  --prompt PROMPT 
+00001bd0: 5b2d 2d6f 7574 7075 742d 6469 7220 4f55  [--output-dir OU
+00001be0: 5450 5554 5f44 4952 5d20 5b2d 2d71 7569  TPUT_DIR] [--qui
+00001bf0: 6574 5d20 5b2d 2d61 7379 6e63 696f 5d0a  et] [--asyncio].
+00001c00: 0a6f 7074 696f 6e61 6c20 6172 6775 6d65  .optional argume
+00001c10: 6e74 733a 0a20 202d 682c 202d 2d68 656c  nts:.  -h, --hel
+00001c20: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
+00001c30: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
+00001c40: 6167 6520 616e 6420 6578 6974 0a20 202d  age and exit.  -
+00001c50: 5520 5520 2020 2020 2020 2020 2020 2020  U U             
+00001c60: 2020 2020 2041 7574 6820 636f 6f6b 6965       Auth cookie
+00001c70: 2066 726f 6d20 6272 6f77 7365 720a 2020   from browser.  
+00001c80: 2d2d 636f 6f6b 6965 2d66 696c 6520 434f  --cookie-file CO
+00001c90: 4f4b 4945 5f46 494c 450a 2020 2020 2020  OKIE_FILE.      
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 2020 4669 6c65 2063 6f6e 7461 696e 696e    File containin
+00001cc0: 6720 6175 7468 2063 6f6f 6b69 650a 2020  g auth cookie.  
+00001cd0: 2d2d 7072 6f6d 7074 2050 524f 4d50 5420  --prompt PROMPT 
+00001ce0: 2020 2020 2020 5072 6f6d 7074 2074 6f20        Prompt to 
+00001cf0: 6765 6e65 7261 7465 2069 6d61 6765 7320  generate images 
+00001d00: 666f 720a 2020 2d2d 6f75 7470 7574 2d64  for.  --output-d
+00001d10: 6972 204f 5554 5055 545f 4449 520a 2020  ir OUTPUT_DIR.  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2020 4f75 7470 7574 2064 6972        Output dir
+00001d40: 6563 746f 7279 0a20 202d 2d71 7569 6574  ectory.  --quiet
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00001d60: 6973 6162 6c65 2070 6970 656c 696e 6520  isable pipeline 
+00001d70: 6d65 7373 6167 6573 0a20 202d 2d61 7379  messages.  --asy
+00001d80: 6e63 696f 2020 2020 2020 2020 2020 2020  ncio            
+00001d90: 2052 756e 2049 6d61 6765 4765 6e20 7573   Run ImageGen us
+00001da0: 696e 6720 6173 796e 6369 6f0a 6060 600a  ing asyncio.```.
+00001db0: 0a23 2320 5275 6e6e 696e 6720 696e 2050  .## Running in P
+00001dc0: 7974 686f 6e0a 0a23 2323 2031 2920 5468  ython..### 1) Th
+00001dd0: 6520 6049 6d61 6765 5175 6572 7960 2068  e `ImageQuery` h
+00001de0: 656c 7065 7220 636c 6173 730a 0a47 656e  elper class..Gen
+00001df0: 6572 6174 6520 696d 6167 6573 2062 6173  erate images bas
+00001e00: 6564 206f 6e20 6120 7369 6d70 6c65 2070  ed on a simple p
+00001e10: 726f 6d70 7420 616e 6420 646f 776e 6c6f  rompt and downlo
+00001e20: 6164 2074 6f20 7468 6520 6375 7272 656e  ad to the curren
+00001e30: 7420 776f 726b 696e 6720 6469 7265 6374  t working direct
+00001e40: 6f72 793a 0a0a 6060 6070 7974 686f 6e0a  ory:..```python.
+00001e50: 6672 6f6d 2045 6467 6547 5054 2069 6d70  from EdgeGPT imp
+00001e60: 6f72 7420 496d 6167 6551 7565 7279 0a0a  ort ImageQuery..
+00001e70: 713d 496d 6167 6551 7565 7279 2822 4d65  q=ImageQuery("Me
+00001e80: 6572 6b61 7473 2061 7420 6120 6761 7264  erkats at a gard
+00001e90: 656e 2070 6172 7479 2069 6e20 4465 766f  en party in Devo
+00001ea0: 6e22 290a 6060 600a 0a43 6861 6e67 6520  n").```..Change 
+00001eb0: 7468 6520 646f 776e 6c6f 6164 2064 6972  the download dir
+00001ec0: 6563 746f 7279 2066 6f72 2061 6c6c 2066  ectory for all f
+00001ed0: 7574 7572 6520 696d 6167 6573 2069 6e20  uture images in 
+00001ee0: 7468 6973 2073 6573 7369 6f6e 3a0a 0a60  this session:..`
+00001ef0: 6060 0a51 7565 7279 2e69 6d61 6765 5f64  ``.Query.image_d
+00001f00: 6972 7061 7468 203d 2050 6174 6828 222e  irpath = Path(".
+00001f10: 2f74 6f5f 616e 6f74 6865 725f 666f 6c64  /to_another_fold
+00001f20: 6572 2229 0a60 6060 0a0a 2323 2320 3229  er").```..### 2)
+00001f30: 2054 6865 2060 496d 6167 6547 656e 6020   The `ImageGen` 
+00001f40: 636c 6173 7320 616e 6420 6061 7379 6e63  class and `async
+00001f50: 696f 6020 666f 7220 6d6f 7265 2067 7261  io` for more gra
+00001f60: 6e75 6c61 7220 636f 6e74 726f 6c0a 0a60  nular control..`
+00001f70: 6060 7079 7468 6f6e 0a66 726f 6d20 496d  ``python.from Im
+00001f80: 6167 6547 656e 2069 6d70 6f72 7420 496d  ageGen import Im
+00001f90: 6167 6547 656e 0a69 6d70 6f72 7420 6172  ageGen.import ar
+00001fa0: 6770 6172 7365 0a69 6d70 6f72 7420 6a73  gparse.import js
+00001fb0: 6f6e 0a0a 6173 796e 6320 6465 6620 6173  on..async def as
+00001fc0: 796e 635f 696d 6167 655f 6765 6e28 6172  ync_image_gen(ar
+00001fd0: 6773 2920 2d3e 204e 6f6e 653a 0a20 2020  gs) -> None:.   
+00001fe0: 2061 7379 6e63 2077 6974 6820 496d 6167   async with Imag
+00001ff0: 6547 656e 4173 796e 6328 6172 6773 2e55  eGenAsync(args.U
+00002000: 2c20 6172 6773 2e71 7569 6574 2920 6173  , args.quiet) as
+00002010: 2069 6d61 6765 5f67 656e 6572 6174 6f72   image_generator
+00002020: 3a0a 2020 2020 2020 2020 696d 6167 6573  :.        images
+00002030: 203d 2061 7761 6974 2069 6d61 6765 5f67   = await image_g
+00002040: 656e 6572 6174 6f72 2e67 6574 5f69 6d61  enerator.get_ima
+00002050: 6765 7328 6172 6773 2e70 726f 6d70 7429  ges(args.prompt)
+00002060: 0a20 2020 2020 2020 2061 7761 6974 2069  .        await i
+00002070: 6d61 6765 5f67 656e 6572 6174 6f72 2e73  mage_generator.s
+00002080: 6176 655f 696d 6167 6573 2869 6d61 6765  ave_images(image
+00002090: 732c 206f 7574 7075 745f 6469 723d 6172  s, output_dir=ar
+000020a0: 6773 2e6f 7574 7075 745f 6469 7229 0a0a  gs.output_dir)..
+000020b0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
+000020c0: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2070  __main__":.    p
+000020d0: 6172 7365 7220 3d20 6172 6770 6172 7365  arser = argparse
+000020e0: 2e41 7267 756d 656e 7450 6172 7365 7228  .ArgumentParser(
+000020f0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00002100: 5f61 7267 756d 656e 7428 222d 5522 2c20  _argument("-U", 
+00002110: 6865 6c70 3d22 4175 7468 2063 6f6f 6b69  help="Auth cooki
+00002120: 6520 6672 6f6d 2062 726f 7773 6572 222c  e from browser",
+00002130: 2074 7970 653d 7374 7229 0a20 2020 2070   type=str).    p
+00002140: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00002150: 6e74 2822 2d2d 636f 6f6b 6965 2d66 696c  nt("--cookie-fil
+00002160: 6522 2c20 6865 6c70 3d22 4669 6c65 2063  e", help="File c
+00002170: 6f6e 7461 696e 696e 6720 6175 7468 2063  ontaining auth c
+00002180: 6f6f 6b69 6522 2c20 7479 7065 3d73 7472  ookie", type=str
+00002190: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+000021a0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+000021b0: 2020 2022 2d2d 7072 6f6d 7074 222c 0a20     "--prompt",. 
+000021c0: 2020 2020 2020 2068 656c 703d 2250 726f         help="Pro
+000021d0: 6d70 7420 746f 2067 656e 6572 6174 6520  mpt to generate 
+000021e0: 696d 6167 6573 2066 6f72 222c 0a20 2020  images for",.   
+000021f0: 2020 2020 2074 7970 653d 7374 722c 0a20       type=str,. 
+00002200: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00002210: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+00002220: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00002230: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
+00002240: 6f75 7470 7574 2d64 6972 222c 0a20 2020  output-dir",.   
+00002250: 2020 2020 2068 656c 703d 224f 7574 7075       help="Outpu
+00002260: 7420 6469 7265 6374 6f72 7922 2c0a 2020  t directory",.  
+00002270: 2020 2020 2020 7479 7065 3d73 7472 2c0a        type=str,.
+00002280: 2020 2020 2020 2020 6465 6661 756c 743d          default=
+00002290: 222e 2f6f 7574 7075 7422 2c0a 2020 2020  "./output",.    
+000022a0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+000022b0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+000022c0: 2020 2022 2d2d 7175 6965 7422 2c20 6865     "--quiet", he
+000022d0: 6c70 3d22 4469 7361 626c 6520 7069 7065  lp="Disable pipe
+000022e0: 6c69 6e65 206d 6573 7361 6765 7322 2c20  line messages", 
+000022f0: 6163 7469 6f6e 3d22 7374 6f72 655f 7472  action="store_tr
+00002300: 7565 220a 2020 2020 290a 2020 2020 7061  ue".    ).    pa
+00002310: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00002320: 7428 0a20 2020 2020 2020 2022 2d2d 6173  t(.        "--as
+00002330: 796e 6369 6f22 2c20 6865 6c70 3d22 5275  yncio", help="Ru
+00002340: 6e20 496d 6167 6547 656e 2075 7369 6e67  n ImageGen using
+00002350: 2061 7379 6e63 696f 222c 2061 6374 696f   asyncio", actio
+00002360: 6e3d 2273 746f 7265 5f74 7275 6522 0a20  n="store_true". 
+00002370: 2020 2029 0a20 2020 2061 7267 7320 3d20     ).    args = 
+00002380: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00002390: 7328 290a 2020 2020 2320 4c6f 6164 2061  s().    # Load a
+000023a0: 7574 6820 636f 6f6b 6965 0a20 2020 2077  uth cookie.    w
+000023b0: 6974 6820 6f70 656e 2861 7267 732e 636f  ith open(args.co
+000023c0: 6f6b 6965 5f66 696c 652c 2065 6e63 6f64  okie_file, encod
+000023d0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+000023e0: 6669 6c65 3a0a 2020 2020 2020 2020 636f  file:.        co
+000023f0: 6f6b 6965 5f6a 736f 6e20 3d20 6a73 6f6e  okie_json = json
+00002400: 2e6c 6f61 6428 6669 6c65 290a 2020 2020  .load(file).    
+00002410: 2020 2020 666f 7220 636f 6f6b 6965 2069      for cookie i
+00002420: 6e20 636f 6f6b 6965 5f6a 736f 6e3a 0a20  n cookie_json:. 
+00002430: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00002440: 6f6b 6965 2e67 6574 2822 6e61 6d65 2229  okie.get("name")
+00002450: 203d 3d20 225f 5522 3a0a 2020 2020 2020   == "_U":.      
+00002460: 2020 2020 2020 2020 2020 6172 6773 2e55            args.U
+00002470: 203d 2063 6f6f 6b69 652e 6765 7428 2276   = cookie.get("v
+00002480: 616c 7565 2229 0a20 2020 2020 2020 2020  alue").         
+00002490: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+000024a0: 2020 6966 2061 7267 732e 5520 6973 204e    if args.U is N
+000024b0: 6f6e 653a 0a20 2020 2020 2020 2072 6169  one:.        rai
+000024c0: 7365 2045 7863 6570 7469 6f6e 2822 436f  se Exception("Co
+000024d0: 756c 6420 6e6f 7420 6669 6e64 2061 7574  uld not find aut
+000024e0: 6820 636f 6f6b 6965 2229 0a0a 2020 2020  h cookie")..    
+000024f0: 6966 206e 6f74 2061 7267 732e 6173 796e  if not args.asyn
+00002500: 6369 6f3a 0a20 2020 2020 2020 2023 2043  cio:.        # C
+00002510: 7265 6174 6520 696d 6167 6520 6765 6e65  reate image gene
+00002520: 7261 746f 720a 2020 2020 2020 2020 696d  rator.        im
+00002530: 6167 655f 6765 6e65 7261 746f 7220 3d20  age_generator = 
+00002540: 496d 6167 6547 656e 2861 7267 732e 552c  ImageGen(args.U,
+00002550: 2061 7267 732e 7175 6965 7429 0a20 2020   args.quiet).   
+00002560: 2020 2020 2069 6d61 6765 5f67 656e 6572       image_gener
+00002570: 6174 6f72 2e73 6176 655f 696d 6167 6573  ator.save_images
+00002580: 280a 2020 2020 2020 2020 2020 2020 696d  (.            im
+00002590: 6167 655f 6765 6e65 7261 746f 722e 6765  age_generator.ge
+000025a0: 745f 696d 6167 6573 2861 7267 732e 7072  t_images(args.pr
+000025b0: 6f6d 7074 292c 0a20 2020 2020 2020 2020  ompt),.         
+000025c0: 2020 206f 7574 7075 745f 6469 723d 6172     output_dir=ar
+000025d0: 6773 2e6f 7574 7075 745f 6469 722c 0a20  gs.output_dir,. 
+000025e0: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
+000025f0: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
+00002600: 696f 2e72 756e 2861 7379 6e63 5f69 6d61  io.run(async_ima
+00002610: 6765 5f67 656e 2861 7267 7329 290a 0a60  ge_gen(args))..`
+00002620: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00002630: 2320 5374 6172 2048 6973 746f 7279 0a0a  # Star History..
+00002640: 5b21 5b53 7461 7220 4869 7374 6f72 7920  [![Star History 
+00002650: 4368 6172 745d 2868 7474 7073 3a2f 2f61  Chart](https://a
+00002660: 7069 2e73 7461 722d 6869 7374 6f72 792e  pi.star-history.
+00002670: 636f 6d2f 7376 673f 7265 706f 733d 6163  com/svg?repos=ac
+00002680: 6865 6f6e 6730 382f 4564 6765 4750 5426  heong08/EdgeGPT&
+00002690: 7479 7065 3d44 6174 6529 5d28 6874 7470  type=Date)](http
+000026a0: 733a 2f2f 7374 6172 2d68 6973 746f 7279  s://star-history
+000026b0: 2e63 6f6d 2f23 6163 6865 6f6e 6730 382f  .com/#acheong08/
+000026c0: 4564 6765 4750 5426 4461 7465 290a 0a23  EdgeGPT&Date)..#
+000026d0: 2043 6f6e 7472 6962 7574 6f72 730a 0a54   Contributors..T
+000026e0: 6869 7320 7072 6f6a 6563 7420 6578 6973  his project exis
+000026f0: 7473 2074 6861 6e6b 7320 746f 2061 6c6c  ts thanks to all
+00002700: 2074 6865 2070 656f 706c 6520 7768 6f20   the people who 
+00002710: 636f 6e74 7269 6275 7465 2e0a 0a20 3c61  contribute... <a
+00002720: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002730: 6974 6875 622e 636f 6d2f 6163 6865 6f6e  ithub.com/acheon
+00002740: 6730 382f 4564 6765 4750 542f 6772 6170  g08/EdgeGPT/grap
+00002750: 6873 2f63 6f6e 7472 6962 7574 6f72 7322  hs/contributors"
+00002760: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
+00002770: 7470 733a 2f2f 636f 6e74 7269 622e 726f  tps://contrib.ro
+00002780: 636b 732f 696d 6167 653f 7265 706f 3d61  cks/image?repo=a
+00002790: 6368 656f 6e67 3038 2f45 6467 6547 5054  cheong08/EdgeGPT
+000027a0: 2220 2f3e 0a20 3c2f 613e 0a              " />. </a>.
```

### Comparing `EdgeGPT-0.6.2/setup.py` & `EdgeGPT-0.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.2",
+    version="0.6.3",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -30,15 +30,15 @@
     install_requires=[
         "httpx",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
         "requests",
-        "BingImageCreator>=0.1.2.1",
+        "BingImageCreator>=0.3.0",
     ],
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
```

### Comparing `EdgeGPT-0.6.2/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.3/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4564 6765  : 2.1.Name: Edge
 00000020: 4750 540a 5665 7273 696f 6e3a 2030 2e36  GPT.Version: 0.6
-00000030: 2e32 0a53 756d 6d61 7279 3a20 5265 7665  .2.Summary: Reve
+00000030: 2e33 0a53 756d 6d61 7279 3a20 5265 7665  .3.Summary: Reve
 00000040: 7273 6520 656e 6769 6e65 6572 6564 2045  rse engineered E
 00000050: 6467 6520 4368 6174 2041 5049 0a48 6f6d  dge Chat API.Hom
 00000060: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000070: 6769 7468 7562 2e63 6f6d 2f61 6368 656f  github.com/acheo
 00000080: 6e67 3038 2f45 6467 6547 5054 0a41 7574  ng08/EdgeGPT.Aut
 00000090: 686f 723a 2041 6e74 6f6e 696f 2043 6865  hor: Antonio Che
 000000a0: 6f6e 670a 4175 7468 6f72 2d65 6d61 696c  ong.Author-email
@@ -108,444 +108,528 @@
 000006b0: 6060 6062 6173 680a 7079 7468 6f6e 3320  ```bash.python3 
 000006c0: 2d6d 2070 6970 2069 6e73 7461 6c6c 2045  -m pip install E
 000006d0: 6467 6547 5054 202d 2d75 7067 7261 6465  dgeGPT --upgrade
 000006e0: 0a60 6060 0a0a 2323 2320 5265 7175 6972  .```..### Requir
 000006f0: 656d 656e 7473 0a0a 2d20 7079 7468 6f6e  ements..- python
 00000700: 2033 2e38 2b0a 2d20 4120 4d69 6372 6f73   3.8+.- A Micros
 00000710: 6f66 7420 4163 636f 756e 7420 7769 7468  oft Account with
-00000720: 2065 6172 6c79 2061 6363 6573 7320 746f   early access to
-00000730: 203c 6874 7470 733a 2f2f 6269 6e67 2e63   <https://bing.c
-00000740: 6f6d 2f63 6861 743e 2028 5265 7175 6972  om/chat> (Requir
-00000750: 6564 290a 2d20 5265 7175 6972 6564 2069  ed).- Required i
-00000760: 6e20 6120 7375 7070 6f72 7465 6420 636f  n a supported co
-00000770: 756e 7472 7920 7769 7468 204e 6577 2042  untry with New B
-00000780: 696e 6720 2843 6869 6e65 7365 206d 6169  ing (Chinese mai
-00000790: 6e6c 616e 6420 5650 4e20 7265 7175 6972  nland VPN requir
-000007a0: 6564 290a 2d20 5b53 656c 656e 6975 6d5d  ed).- [Selenium]
-000007b0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-000007c0: 672f 7072 6f6a 6563 742f 7365 6c65 6e69  g/project/seleni
-000007d0: 756d 2f29 2028 666f 7220 6175 746f 6d61  um/) (for automa
-000007e0: 7469 6320 636f 6f6b 6965 2073 6574 7570  tic cookie setup
-000007f0: 290a 0a3c 6465 7461 696c 733e 0a0a 3c73  )..<details>..<s
-00000800: 756d 6d61 7279 3e0a 0a23 2043 6861 7462  ummary>..# Chatb
-00000810: 6f74 0a0a 3c2f 7375 6d6d 6172 793e 0a0a  ot..</summary>..
-00000820: 2323 2041 7574 6865 6e74 6963 6174 696f  ## Authenticatio
-00000830: 6e0a 0a21 2121 204e 4f54 2052 4551 5549  n..!!! NOT REQUI
-00000840: 5245 4420 414e 594d 4f52 4520 2121 210a  RED ANYMORE !!!.
-00000850: 4d69 6372 6f73 6f66 7420 6861 7320 6d61  Microsoft has ma
-00000860: 6465 2074 6865 2063 6861 7420 6665 6174  de the chat feat
-00000870: 7572 6520 6176 6169 6c61 626c 6520 746f  ure available to
-00000880: 2065 7665 7279 6f6e 652c 2073 6f20 796f   everyone, so yo
-00000890: 7520 6361 6e20 736b 6970 2074 6869 7320  u can skip this 
-000008a0: 7374 6570 2e0a 0a23 2320 5275 6e6e 696e  step...## Runnin
-000008b0: 6720 6672 6f6d 2074 6865 2043 6f6d 6d61  g from the Comma
-000008c0: 6e64 204c 696e 650a 0a60 6060 0a20 2420  nd Line..```. $ 
-000008d0: 7079 7468 6f6e 3320 2d6d 2045 6467 6547  python3 -m EdgeG
-000008e0: 5054 202d 680a 0a20 2020 2020 2020 2045  PT -h..        E
-000008f0: 6467 6547 5054 202d 2041 2064 656d 6f20  dgeGPT - A demo 
-00000900: 6f66 2072 6576 6572 7365 2065 6e67 696e  of reverse engin
-00000910: 6565 7269 6e67 2074 6865 2042 696e 6720  eering the Bing 
-00000920: 4750 5420 6368 6174 626f 740a 2020 2020  GPT chatbot.    
-00000930: 2020 2020 5265 706f 3a20 6769 7468 7562      Repo: github
-00000940: 2e63 6f6d 2f61 6368 656f 6e67 3038 2f45  .com/acheong08/E
-00000950: 6467 6547 5054 0a20 2020 2020 2020 2042  dgeGPT.        B
-00000960: 793a 2041 6e74 6f6e 696f 2043 6865 6f6e  y: Antonio Cheon
-00000970: 670a 0a20 2020 2020 2020 2021 6865 6c70  g..        !help
-00000980: 2066 6f72 2068 656c 700a 0a20 2020 2020   for help..     
-00000990: 2020 2054 7970 6520 2165 7869 7420 746f     Type !exit to
-000009a0: 2065 7869 740a 2020 2020 2020 2020 456e   exit.        En
-000009b0: 7465 7220 7477 6963 6520 746f 2073 656e  ter twice to sen
-000009c0: 6420 6d65 7373 6167 6520 6f72 2073 6574  d message or set
-000009d0: 202d 2d65 6e74 6572 2d6f 6e63 6520 746f   --enter-once to
-000009e0: 2073 656e 6420 6f6e 6520 6c69 6e65 206d   send one line m
-000009f0: 6573 7361 6765 0a0a 7573 6167 653a 2045  essage..usage: E
-00000a00: 6467 6547 5054 2e70 7920 5b2d 685d 205b  dgeGPT.py [-h] [
-00000a10: 2d2d 656e 7465 722d 6f6e 6365 5d20 5b2d  --enter-once] [-
-00000a20: 2d6e 6f2d 7374 7265 616d 5d20 5b2d 2d72  -no-stream] [--r
-00000a30: 6963 685d 205b 2d2d 7072 6f78 7920 5052  ich] [--proxy PR
-00000a40: 4f58 595d 205b 2d2d 7374 796c 6520 7b63  OXY] [--style {c
-00000a50: 7265 6174 6976 652c 6261 6c61 6e63 6564  reative,balanced
-00000a60: 2c70 7265 6369 7365 7d5d 0a0a 6f70 7469  ,precise}]..opti
-00000a70: 6f6e 733a 0a20 202d 682c 202d 2d68 656c  ons:.  -h, --hel
-00000a80: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
-00000a90: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
-00000aa0: 6167 6520 616e 6420 6578 6974 0a20 202d  age and exit.  -
-00000ab0: 2d65 6e74 6572 2d6f 6e63 650a 2020 2d2d  -enter-once.  --
-00000ac0: 6e6f 2d73 7472 6561 6d0a 2020 2d2d 7269  no-stream.  --ri
-00000ad0: 6368 0a20 202d 2d70 726f 7879 2050 524f  ch.  --proxy PRO
-00000ae0: 5859 2020 2020 2020 2020 2050 726f 7879  XY         Proxy
-00000af0: 2055 524c 2028 652e 672e 2073 6f63 6b73   URL (e.g. socks
-00000b00: 353a 2f2f 3132 372e 302e 302e 313a 3130  5://127.0.0.1:10
-00000b10: 3830 290a 2020 2d2d 7374 796c 6520 7b63  80).  --style {c
-00000b20: 7265 6174 6976 652c 6261 6c61 6e63 6564  reative,balanced
-00000b30: 2c70 7265 6369 7365 7d0a 6060 600a 0a23  ,precise}.```..#
-00000b40: 2320 5275 6e6e 696e 6720 696e 2050 7974  # Running in Pyt
-00000b50: 686f 6e0a 0a23 2323 2031 2e20 5468 6520  hon..### 1. The 
-00000b60: 6043 6861 7462 6f74 6020 636c 6173 7320  `Chatbot` class 
-00000b70: 616e 6420 6061 7379 6e63 696f 6020 666f  and `asyncio` fo
-00000b80: 7220 6d6f 7265 2067 7261 6e75 6c61 7220  r more granular 
-00000b90: 636f 6e74 726f 6c0a 0a55 7365 2041 7379  control..Use Asy
-00000ba0: 6e63 2066 6f72 2074 6865 2062 6573 7420  nc for the best 
-00000bb0: 6578 7065 7269 656e 6365 2c20 666f 7220  experience, for 
-00000bc0: 6578 616d 706c 653a 0a0a 6060 6070 7974  example:..```pyt
-00000bd0: 686f 6e0a 696d 706f 7274 2061 7379 6e63  hon.import async
-00000be0: 696f 0a66 726f 6d20 4564 6765 4750 5420  io.from EdgeGPT 
-00000bf0: 696d 706f 7274 2043 6861 7462 6f74 2c20  import Chatbot, 
-00000c00: 436f 6e76 6572 7361 7469 6f6e 5374 796c  ConversationStyl
-00000c10: 650a 0a61 7379 6e63 2064 6566 206d 6169  e..async def mai
-00000c20: 6e28 293a 0a20 2020 2062 6f74 203d 2061  n():.    bot = a
-00000c30: 7761 6974 2043 6861 7462 6f74 2e63 7265  wait Chatbot.cre
-00000c40: 6174 6528 290a 2020 2020 7072 696e 7428  ate().    print(
-00000c50: 6177 6169 7420 626f 742e 6173 6b28 7072  await bot.ask(pr
-00000c60: 6f6d 7074 3d22 4865 6c6c 6f20 776f 726c  ompt="Hello worl
-00000c70: 6422 2c20 636f 6e76 6572 7361 7469 6f6e  d", conversation
-00000c80: 5f73 7479 6c65 3d43 6f6e 7665 7273 6174  _style=Conversat
-00000c90: 696f 6e53 7479 6c65 2e63 7265 6174 6976  ionStyle.creativ
-00000ca0: 6529 290a 2020 2020 6177 6169 7420 626f  e)).    await bo
-00000cb0: 742e 636c 6f73 6528 290a 0a69 6620 5f5f  t.close()..if __
-00000cc0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
-00000cd0: 6e5f 5f22 3a0a 2020 2020 6173 796e 6369  n__":.    asynci
-00000ce0: 6f2e 7275 6e28 6d61 696e 2829 290a 6060  o.run(main()).``
-00000cf0: 600a 0a3c 6465 7461 696c 733e 0a3c 7375  `..<details>.<su
-00000d00: 6d6d 6172 793e 0a0a 2323 2320 3229 2054  mmary>..### 2) T
-00000d10: 6865 2060 5175 6572 7960 2061 6e64 2060  he `Query` and `
-00000d20: 436f 6f6b 6965 6020 6865 6c70 6572 2063  Cookie` helper c
-00000d30: 6c61 7373 6573 0a0a 2020 3c2f 7375 6d6d  lasses..  </summ
-00000d40: 6172 793e 0a0a 4372 6561 7465 2061 2073  ary>..Create a s
-00000d50: 696d 706c 6520 4269 6e67 2043 6861 7420  imple Bing Chat 
-00000d60: 4149 2071 7565 7279 2028 7573 696e 6720  AI query (using 
-00000d70: 7468 6520 2770 7265 6369 7365 2720 636f  the 'precise' co
-00000d80: 6e76 6572 7361 7469 6f6e 2073 7479 6c65  nversation style
-00000d90: 2062 7920 6465 6661 756c 7429 2061 6e64   by default) and
-00000da0: 2073 6565 206a 7573 7420 7468 6520 6d61   see just the ma
-00000db0: 696e 2074 6578 7420 6f75 7470 7574 2072  in text output r
-00000dc0: 6174 6865 7220 7468 616e 2074 6865 2077  ather than the w
-00000dd0: 686f 6c65 2041 5049 2072 6573 706f 6e73  hole API respons
-00000de0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-00000df0: 6f6d 2045 6467 6547 5054 2069 6d70 6f72  om EdgeGPT impor
-00000e00: 7420 5175 6572 792c 2043 6f6f 6b69 650a  t Query, Cookie.
-00000e10: 0a71 203d 2051 7565 7279 2822 5768 6174  .q = Query("What
-00000e20: 2061 7265 2079 6f75 3f20 4769 7665 2079   are you? Give y
-00000e30: 6f75 7220 616e 7377 6572 2061 7320 5079  our answer as Py
-00000e40: 7468 6f6e 2063 6f64 6522 290a 7072 696e  thon code").prin
-00000e50: 7428 7129 0a60 6060 0a0a 4f72 2063 6861  t(q).```..Or cha
-00000e60: 6e67 6520 7468 6520 636f 6e76 6572 7361  nge the conversa
-00000e70: 7469 6f6e 2073 7479 6c65 206f 7220 636f  tion style or co
-00000e80: 6f6b 6965 2066 696c 6520 746f 2062 6520  okie file to be 
-00000e90: 7573 6564 3a0a 0a60 6060 7079 7468 6f6e  used:..```python
-00000ea0: 0a71 203d 2051 7565 7279 280a 2020 2257  .q = Query(.  "W
-00000eb0: 6861 7420 6172 6520 796f 753f 2047 6976  hat are you? Giv
-00000ec0: 6520 796f 7572 2061 6e73 7765 7220 6173  e your answer as
-00000ed0: 2050 7974 686f 6e20 636f 6465 222c 0a20   Python code",. 
-00000ee0: 2073 7479 6c65 3d22 6372 6561 7469 7665   style="creative
-00000ef0: 222c 2020 2320 6f72 2027 6261 6c61 6e63  ",  # or 'balanc
-00000f00: 6564 270a 2020 636f 6f6b 6965 733d 222e  ed'.  cookies=".
-00000f10: 2f62 696e 675f 636f 6f6b 6965 735f 616c  /bing_cookies_al
-00000f20: 7465 726e 6174 6976 652e 6a73 6f6e 220a  ternative.json".
-00000f30: 290a 6060 600a 0a51 7569 636b 6c79 2065  ).```..Quickly e
-00000f40: 7874 7261 6374 2074 6865 2074 6578 7420  xtract the text 
-00000f50: 6f75 7470 7574 2c20 636f 6465 2073 6e69  output, code sni
-00000f60: 7070 6574 732c 206c 6973 7420 6f66 2073  ppets, list of s
-00000f70: 6f75 7263 6573 2f72 6566 6572 656e 6365  ources/reference
-00000f80: 732c 206f 7220 7375 6767 6573 7465 6420  s, or suggested 
-00000f90: 666f 6c6c 6f77 2d6f 6e20 7175 6573 7469  follow-on questi
-00000fa0: 6f6e 7320 7573 696e 6720 7468 6520 666f  ons using the fo
-00000fb0: 6c6c 6f77 696e 6720 6174 7472 6962 7574  llowing attribut
-00000fc0: 6573 3a0a 0a60 6060 7079 7468 6f6e 0a71  es:..```python.q
-00000fd0: 2e6f 7574 7075 740a 712e 636f 6465 0a71  .output.q.code.q
-00000fe0: 2e73 7567 6765 7374 696f 6e73 0a71 2e73  .suggestions.q.s
-00000ff0: 6f75 7263 6573 2020 2020 2020 2023 2066  ources       # f
-00001000: 6f72 2074 6865 2066 756c 6c20 6a73 6f6e  or the full json
-00001010: 206f 7574 7075 740a 712e 736f 7572 6365   output.q.source
-00001020: 735f 6469 6374 2020 2320 666f 7220 6120  s_dict  # for a 
-00001030: 6469 6374 696f 6e61 7279 206f 6620 7469  dictionary of ti
-00001040: 746c 6573 2061 6e64 2075 726c 730a 6060  tles and urls.``
-00001050: 600a 0a47 6574 2074 6865 206f 7267 696e  `..Get the orgin
-00001060: 616c 2070 726f 6d70 7420 616e 6420 7468  al prompt and th
-00001070: 6520 636f 6e76 6572 7361 7469 6f6e 2073  e conversation s
-00001080: 7479 6c65 2079 6f75 2073 7065 6369 6669  tyle you specifi
-00001090: 6564 3a0a 0a60 6060 7079 7468 6f6e 0a71  ed:..```python.q
-000010a0: 2e70 726f 6d70 740a 712e 7374 796c 650a  .prompt.q.style.
-000010b0: 7265 7072 2871 290a 6060 600a 0a41 6363  repr(q).```..Acc
-000010c0: 6573 7320 7072 6576 696f 7573 2051 7565  ess previous Que
-000010d0: 7269 6573 206d 6164 6520 7369 6e63 6520  ries made since 
-000010e0: 696d 706f 7274 696e 6720 6051 7565 7279  importing `Query
-000010f0: 603a 0a0a 6060 6070 7974 686f 6e0a 5175  `:..```python.Qu
-00001100: 6572 792e 696e 6465 7820 2023 2041 206c  ery.index  # A l
-00001110: 6973 7420 6f66 2051 7565 7279 206f 626a  ist of Query obj
-00001120: 6563 7473 3b20 7570 6461 7465 6420 6479  ects; updated dy
-00001130: 6e61 6d69 6361 6c6c 790a 5175 6572 792e  namically.Query.
-00001140: 7265 7175 6573 745f 636f 756e 7420 2023  request_count  #
-00001150: 2041 2074 616c 6c79 206f 6620 7265 7175   A tally of requ
-00001160: 6573 7473 206d 6164 6520 7573 696e 6720  ests made using 
-00001170: 6561 6368 2063 6f6f 6b69 6520 6669 6c65  each cookie file
-00001180: 0a60 6060 0a0a 416e 6420 6669 6e61 6c6c  .```..And finall
-00001190: 792c 2074 6865 2060 436f 6f6b 6965 6020  y, the `Cookie` 
-000011a0: 636c 6173 7320 7375 7070 6f72 7473 206d  class supports m
-000011b0: 756c 7469 706c 6520 636f 6f6b 6965 2066  ultiple cookie f
-000011c0: 696c 6573 2c20 736f 2069 6620 796f 7520  iles, so if you 
-000011d0: 6372 6561 7465 2061 6464 6974 696f 6e61  create additiona
-000011e0: 6c20 636f 6f6b 6965 2066 696c 6573 2077  l cookie files w
-000011f0: 6974 6820 7468 6520 6e61 6d69 6e67 2063  ith the naming c
-00001200: 6f6e 7665 6e74 696f 6e20 6062 696e 675f  onvention `bing_
-00001210: 636f 6f6b 6965 735f 2a2e 6a73 6f6e 602c  cookies_*.json`,
-00001220: 2079 6f75 7220 7175 6572 6965 7320 7769   your queries wi
-00001230: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
-00001240: 2074 7279 2075 7369 6e67 2074 6865 206e   try using the n
-00001250: 6578 7420 6669 6c65 2028 616c 7068 6162  ext file (alphab
-00001260: 6574 6963 616c 6c79 2920 6966 2079 6f75  etically) if you
-00001270: 2776 6520 6578 6365 6564 6564 2079 6f75  've exceeded you
-00001280: 7220 6461 696c 7920 7175 6f74 6120 6f66  r daily quota of
-00001290: 2072 6571 7565 7374 7320 2863 7572 7265   requests (curre
-000012a0: 6e74 6c79 2073 6574 2061 7420 3230 3029  ntly set at 200)
-000012b0: 2e0a 0a48 6572 6520 6172 6520 7468 6520  ...Here are the 
-000012c0: 6d61 696e 2061 7474 7269 6275 7465 7320  main attributes 
-000012d0: 7768 6963 6820 796f 7520 6361 6e20 6163  which you can ac
-000012e0: 6365 7373 3a0a 0a60 6060 7079 7468 6f6e  cess:..```python
-000012f0: 0a43 6f6f 6b69 652e 6375 7272 656e 745f  .Cookie.current_
-00001300: 6669 6c65 5f69 6e64 6578 0a43 6f6f 6b69  file_index.Cooki
-00001310: 652e 6469 7270 6174 680a 436f 6f6b 6965  e.dirpath.Cookie
-00001320: 2e73 6561 7263 685f 7061 7474 6572 6e20  .search_pattern 
-00001330: 2023 2064 6566 6175 6c74 2069 7320 6062   # default is `b
-00001340: 696e 675f 636f 6f6b 6965 735f 2a2e 6a73  ing_cookies_*.js
-00001350: 6f6e 600a 436f 6f6b 6965 2e66 696c 6573  on`.Cookie.files
-00001360: 2829 2020 2320 6c69 7374 2061 7320 6669  ()  # list as fi
-00001370: 6c65 7320 7468 6174 206d 6174 6368 202e  les that match .
-00001380: 7365 6172 6368 5f70 6174 7465 726e 0a43  search_pattern.C
-00001390: 6f6f 6b69 652e 6375 7272 656e 745f 6669  ookie.current_fi
-000013a0: 6c65 7061 7468 0a43 6f6f 6b69 652e 6375  lepath.Cookie.cu
-000013b0: 7272 656e 745f 6461 7461 0a43 6f6f 6b69  rrent_data.Cooki
-000013c0: 652e 696d 706f 7274 5f6e 6578 7428 290a  e.import_next().
-000013d0: 436f 6f6b 6965 2e69 6d61 6765 5f74 6f6b  Cookie.image_tok
-000013e0: 656e 0a43 6f6f 6b69 652e 6967 6e6f 7265  en.Cookie.ignore
-000013f0: 5f66 696c 6573 0a60 6060 0a0a 3c2f 6465  _files.```..</de
-00001400: 7461 696c 733e 0a0a 2d2d 2d0a 0a23 2320  tails>..---..## 
-00001410: 5275 6e6e 696e 6720 7769 7468 2044 6f63  Running with Doc
-00001420: 6b65 720a 0a54 6869 7320 6173 7375 6d65  ker..This assume
-00001430: 7320 796f 7520 6861 7665 2061 2066 696c  s you have a fil
-00001440: 6520 636f 6f6b 6965 732e 6a73 6f6e 2069  e cookies.json i
-00001450: 6e20 796f 7572 2063 7572 7265 6e74 2077  n your current w
-00001460: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
-00001470: 0a0a 6060 6062 6173 680a 0a64 6f63 6b65  ..```bash..docke
-00001480: 7220 7275 6e20 2d2d 726d 202d 6974 202d  r run --rm -it -
-00001490: 7620 2428 7077 6429 2f63 6f6f 6b69 6573  v $(pwd)/cookies
-000014a0: 2e6a 736f 6e3a 2f63 6f6f 6b69 6573 2e6a  .json:/cookies.j
-000014b0: 736f 6e3a 726f 202d 6520 434f 4f4b 4945  son:ro -e COOKIE
-000014c0: 5f46 494c 453d 272f 636f 6f6b 6965 732e  _FILE='/cookies.
-000014d0: 6a73 6f6e 2720 6768 6372 2e69 6f2f 6163  json' ghcr.io/ac
-000014e0: 6865 6f6e 6730 382f 6564 6765 6770 740a  heong08/edgegpt.
-000014f0: 6060 600a 0a59 6f75 2063 616e 2061 6464  ```..You can add
-00001500: 2061 6e79 2065 7874 7261 2066 6c61 6773   any extra flags
-00001510: 2061 7320 666f 6c6c 6f77 696e 670a 0a60   as following..`
-00001520: 6060 6261 7368 0a0a 646f 636b 6572 2072  ``bash..docker r
-00001530: 756e 202d 2d72 6d20 2d69 7420 2d76 2024  un --rm -it -v $
-00001540: 2870 7764 292f 636f 6f6b 6965 732e 6a73  (pwd)/cookies.js
-00001550: 6f6e 3a2f 636f 6f6b 6965 732e 6a73 6f6e  on:/cookies.json
-00001560: 3a72 6f20 2d65 2043 4f4f 4b49 455f 4649  :ro -e COOKIE_FI
-00001570: 4c45 3d27 2f63 6f6f 6b69 6573 2e6a 736f  LE='/cookies.jso
-00001580: 6e27 2067 6863 722e 696f 2f61 6368 656f  n' ghcr.io/acheo
-00001590: 6e67 3038 2f65 6467 6567 7074 202d 2d72  ng08/edgegpt --r
-000015a0: 6963 6820 2d2d 7374 796c 6520 6372 6561  ich --style crea
-000015b0: 7469 7665 0a60 6060 0a0a 3c2f 6465 7461  tive.```..</deta
-000015c0: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
-000015d0: 0a3c 7375 6d6d 6172 793e 0a0a 2320 496d  .<summary>..# Im
-000015e0: 6167 6520 6765 6e65 7261 746f 720a 0a3c  age generator..<
-000015f0: 2f73 756d 6d61 7279 3e0a 0a23 2320 5275  /summary>..## Ru
-00001600: 6e6e 696e 6720 6672 6f6d 2074 6865 2043  nning from the C
-00001610: 6f6d 6d61 6e64 204c 696e 650a 0a60 6060  ommand Line..```
-00001620: 6261 7368 0a24 2070 7974 686f 6e33 202d  bash.$ python3 -
-00001630: 6d20 496d 6167 6547 656e 202d 680a 7573  m ImageGen -h.us
-00001640: 6167 653a 2049 6d61 6765 4765 6e2e 7079  age: ImageGen.py
-00001650: 205b 2d68 5d20 5b2d 5520 555d 205b 2d2d   [-h] [-U U] [--
-00001660: 636f 6f6b 6965 2d66 696c 6520 434f 4f4b  cookie-file COOK
-00001670: 4945 5f46 494c 455d 202d 2d70 726f 6d70  IE_FILE] --promp
-00001680: 7420 5052 4f4d 5054 205b 2d2d 6f75 7470  t PROMPT [--outp
-00001690: 7574 2d64 6972 204f 5554 5055 545f 4449  ut-dir OUTPUT_DI
-000016a0: 525d 205b 2d2d 7175 6965 745d 205b 2d2d  R] [--quiet] [--
-000016b0: 6173 796e 6369 6f5d 0a0a 6f70 7469 6f6e  asyncio]..option
-000016c0: 616c 2061 7267 756d 656e 7473 3a0a 2020  al arguments:.  
-000016d0: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
-000016e0: 2020 2020 2020 7368 6f77 2074 6869 7320        show this 
-000016f0: 6865 6c70 206d 6573 7361 6765 2061 6e64  help message and
-00001700: 2065 7869 740a 2020 2d55 2055 2020 2020   exit.  -U U    
-00001710: 2020 2020 2020 2020 2020 2020 2020 4175                Au
-00001720: 7468 2063 6f6f 6b69 6520 6672 6f6d 2062  th cookie from b
-00001730: 726f 7773 6572 0a20 202d 2d63 6f6f 6b69  rowser.  --cooki
-00001740: 652d 6669 6c65 2043 4f4f 4b49 455f 4649  e-file COOKIE_FI
-00001750: 4c45 0a20 2020 2020 2020 2020 2020 2020  LE.             
-00001760: 2020 2020 2020 2020 2020 2046 696c 6520             File 
-00001770: 636f 6e74 6169 6e69 6e67 2061 7574 6820  containing auth 
-00001780: 636f 6f6b 6965 0a20 202d 2d70 726f 6d70  cookie.  --promp
-00001790: 7420 5052 4f4d 5054 2020 2020 2020 2050  t PROMPT       P
-000017a0: 726f 6d70 7420 746f 2067 656e 6572 6174  rompt to generat
-000017b0: 6520 696d 6167 6573 2066 6f72 0a20 202d  e images for.  -
-000017c0: 2d6f 7574 7075 742d 6469 7220 4f55 5450  -output-dir OUTP
-000017d0: 5554 5f44 4952 0a20 2020 2020 2020 2020  UT_DIR.         
-000017e0: 2020 2020 2020 2020 2020 2020 2020 204f                 O
-000017f0: 7574 7075 7420 6469 7265 6374 6f72 790a  utput directory.
-00001800: 2020 2d2d 7175 6965 7420 2020 2020 2020    --quiet       
-00001810: 2020 2020 2020 2020 4469 7361 626c 6520          Disable 
-00001820: 7069 7065 6c69 6e65 206d 6573 7361 6765  pipeline message
-00001830: 730a 2020 2d2d 6173 796e 6369 6f20 2020  s.  --asyncio   
-00001840: 2020 2020 2020 2020 2020 5275 6e20 496d            Run Im
-00001850: 6167 6547 656e 2075 7369 6e67 2061 7379  ageGen using asy
-00001860: 6e63 696f 0a60 6060 0a0a 2323 2052 756e  ncio.```..## Run
-00001870: 6e69 6e67 2069 6e20 5079 7468 6f6e 0a0a  ning in Python..
-00001880: 2323 2320 3129 2054 6865 2060 496d 6167  ### 1) The `Imag
-00001890: 6551 7565 7279 6020 6865 6c70 6572 2063  eQuery` helper c
-000018a0: 6c61 7373 0a0a 4765 6e65 7261 7465 2069  lass..Generate i
-000018b0: 6d61 6765 7320 6261 7365 6420 6f6e 2061  mages based on a
-000018c0: 2073 696d 706c 6520 7072 6f6d 7074 2061   simple prompt a
-000018d0: 6e64 2064 6f77 6e6c 6f61 6420 746f 2074  nd download to t
-000018e0: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
-000018f0: 6e67 2064 6972 6563 746f 7279 3a0a 0a60  ng directory:..`
-00001900: 6060 7079 7468 6f6e 0a66 726f 6d20 4564  ``python.from Ed
-00001910: 6765 4750 5420 696d 706f 7274 2049 6d61  geGPT import Ima
-00001920: 6765 5175 6572 790a 0a71 3d49 6d61 6765  geQuery..q=Image
-00001930: 5175 6572 7928 224d 6565 726b 6174 7320  Query("Meerkats 
-00001940: 6174 2061 2067 6172 6465 6e20 7061 7274  at a garden part
-00001950: 7920 696e 2044 6576 6f6e 2229 0a60 6060  y in Devon").```
-00001960: 0a0a 4368 616e 6765 2074 6865 2064 6f77  ..Change the dow
-00001970: 6e6c 6f61 6420 6469 7265 6374 6f72 7920  nload directory 
-00001980: 666f 7220 616c 6c20 6675 7475 7265 2069  for all future i
-00001990: 6d61 6765 7320 696e 2074 6869 7320 7365  mages in this se
-000019a0: 7373 696f 6e3a 0a0a 6060 600a 5175 6572  ssion:..```.Quer
-000019b0: 792e 696d 6167 655f 6469 7270 6174 6820  y.image_dirpath 
-000019c0: 3d20 5061 7468 2822 2e2f 746f 5f61 6e6f  = Path("./to_ano
-000019d0: 7468 6572 5f66 6f6c 6465 7222 290a 6060  ther_folder").``
-000019e0: 600a 0a23 2323 2032 2920 5468 6520 6049  `..### 2) The `I
-000019f0: 6d61 6765 4765 6e60 2063 6c61 7373 2061  mageGen` class a
-00001a00: 6e64 2060 6173 796e 6369 6f60 2066 6f72  nd `asyncio` for
-00001a10: 206d 6f72 6520 6772 616e 756c 6172 2063   more granular c
-00001a20: 6f6e 7472 6f6c 0a0a 6060 6070 7974 686f  ontrol..```pytho
-00001a30: 6e0a 6672 6f6d 2049 6d61 6765 4765 6e20  n.from ImageGen 
-00001a40: 696d 706f 7274 2049 6d61 6765 4765 6e0a  import ImageGen.
-00001a50: 696d 706f 7274 2061 7267 7061 7273 650a  import argparse.
-00001a60: 696d 706f 7274 206a 736f 6e0a 0a61 7379  import json..asy
-00001a70: 6e63 2064 6566 2061 7379 6e63 5f69 6d61  nc def async_ima
-00001a80: 6765 5f67 656e 2861 7267 7329 202d 3e20  ge_gen(args) -> 
-00001a90: 4e6f 6e65 3a0a 2020 2020 6173 796e 6320  None:.    async 
-00001aa0: 7769 7468 2049 6d61 6765 4765 6e41 7379  with ImageGenAsy
-00001ab0: 6e63 2861 7267 732e 552c 2061 7267 732e  nc(args.U, args.
-00001ac0: 7175 6965 7429 2061 7320 696d 6167 655f  quiet) as image_
-00001ad0: 6765 6e65 7261 746f 723a 0a20 2020 2020  generator:.     
-00001ae0: 2020 2069 6d61 6765 7320 3d20 6177 6169     images = awai
-00001af0: 7420 696d 6167 655f 6765 6e65 7261 746f  t image_generato
-00001b00: 722e 6765 745f 696d 6167 6573 2861 7267  r.get_images(arg
-00001b10: 732e 7072 6f6d 7074 290a 2020 2020 2020  s.prompt).      
-00001b20: 2020 6177 6169 7420 696d 6167 655f 6765    await image_ge
-00001b30: 6e65 7261 746f 722e 7361 7665 5f69 6d61  nerator.save_ima
-00001b40: 6765 7328 696d 6167 6573 2c20 6f75 7470  ges(images, outp
-00001b50: 7574 5f64 6972 3d61 7267 732e 6f75 7470  ut_dir=args.outp
-00001b60: 7574 5f64 6972 290a 0a69 6620 5f5f 6e61  ut_dir)..if __na
-00001b70: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
-00001b80: 5f22 3a0a 2020 2020 7061 7273 6572 203d  _":.    parser =
-00001b90: 2061 7267 7061 7273 652e 4172 6775 6d65   argparse.Argume
-00001ba0: 6e74 5061 7273 6572 2829 0a20 2020 2070  ntParser().    p
-00001bb0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00001bc0: 6e74 2822 2d55 222c 2068 656c 703d 2241  nt("-U", help="A
-00001bd0: 7574 6820 636f 6f6b 6965 2066 726f 6d20  uth cookie from 
-00001be0: 6272 6f77 7365 7222 2c20 7479 7065 3d73  browser", type=s
-00001bf0: 7472 290a 2020 2020 7061 7273 6572 2e61  tr).    parser.a
-00001c00: 6464 5f61 7267 756d 656e 7428 222d 2d63  dd_argument("--c
-00001c10: 6f6f 6b69 652d 6669 6c65 222c 2068 656c  ookie-file", hel
-00001c20: 703d 2246 696c 6520 636f 6e74 6169 6e69  p="File containi
-00001c30: 6e67 2061 7574 6820 636f 6f6b 6965 222c  ng auth cookie",
-00001c40: 2074 7970 653d 7374 7229 0a20 2020 2070   type=str).    p
-00001c50: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00001c60: 6e74 280a 2020 2020 2020 2020 222d 2d70  nt(.        "--p
-00001c70: 726f 6d70 7422 2c0a 2020 2020 2020 2020  rompt",.        
-00001c80: 6865 6c70 3d22 5072 6f6d 7074 2074 6f20  help="Prompt to 
-00001c90: 6765 6e65 7261 7465 2069 6d61 6765 7320  generate images 
-00001ca0: 666f 7222 2c0a 2020 2020 2020 2020 7479  for",.        ty
-00001cb0: 7065 3d73 7472 2c0a 2020 2020 2020 2020  pe=str,.        
-00001cc0: 7265 7175 6972 6564 3d54 7275 652c 0a20  required=True,. 
-00001cd0: 2020 2029 0a20 2020 2070 6172 7365 722e     ).    parser.
-00001ce0: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00001cf0: 2020 2020 2020 222d 2d6f 7574 7075 742d        "--output-
-00001d00: 6469 7222 2c0a 2020 2020 2020 2020 6865  dir",.        he
-00001d10: 6c70 3d22 4f75 7470 7574 2064 6972 6563  lp="Output direc
-00001d20: 746f 7279 222c 0a20 2020 2020 2020 2074  tory",.        t
-00001d30: 7970 653d 7374 722c 0a20 2020 2020 2020  ype=str,.       
-00001d40: 2064 6566 6175 6c74 3d22 2e2f 6f75 7470   default="./outp
-00001d50: 7574 222c 0a20 2020 2029 0a20 2020 2070  ut",.    ).    p
-00001d60: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00001d70: 6e74 280a 2020 2020 2020 2020 222d 2d71  nt(.        "--q
-00001d80: 7569 6574 222c 2068 656c 703d 2244 6973  uiet", help="Dis
-00001d90: 6162 6c65 2070 6970 656c 696e 6520 6d65  able pipeline me
-00001da0: 7373 6167 6573 222c 2061 6374 696f 6e3d  ssages", action=
-00001db0: 2273 746f 7265 5f74 7275 6522 0a20 2020  "store_true".   
-00001dc0: 2029 0a20 2020 2070 6172 7365 722e 6164   ).    parser.ad
-00001dd0: 645f 6172 6775 6d65 6e74 280a 2020 2020  d_argument(.    
-00001de0: 2020 2020 222d 2d61 7379 6e63 696f 222c      "--asyncio",
-00001df0: 2068 656c 703d 2252 756e 2049 6d61 6765   help="Run Image
-00001e00: 4765 6e20 7573 696e 6720 6173 796e 6369  Gen using asynci
-00001e10: 6f22 2c20 6163 7469 6f6e 3d22 7374 6f72  o", action="stor
-00001e20: 655f 7472 7565 220a 2020 2020 290a 2020  e_true".    ).  
-00001e30: 2020 6172 6773 203d 2070 6172 7365 722e    args = parser.
-00001e40: 7061 7273 655f 6172 6773 2829 0a20 2020  parse_args().   
-00001e50: 2023 204c 6f61 6420 6175 7468 2063 6f6f   # Load auth coo
-00001e60: 6b69 650a 2020 2020 7769 7468 206f 7065  kie.    with ope
-00001e70: 6e28 6172 6773 2e63 6f6f 6b69 655f 6669  n(args.cookie_fi
-00001e80: 6c65 2c20 656e 636f 6469 6e67 3d22 7574  le, encoding="ut
-00001e90: 662d 3822 2920 6173 2066 696c 653a 0a20  f-8") as file:. 
-00001ea0: 2020 2020 2020 2063 6f6f 6b69 655f 6a73         cookie_js
-00001eb0: 6f6e 203d 206a 736f 6e2e 6c6f 6164 2866  on = json.load(f
-00001ec0: 696c 6529 0a20 2020 2020 2020 2066 6f72  ile).        for
-00001ed0: 2063 6f6f 6b69 6520 696e 2063 6f6f 6b69   cookie in cooki
-00001ee0: 655f 6a73 6f6e 3a0a 2020 2020 2020 2020  e_json:.        
-00001ef0: 2020 2020 6966 2063 6f6f 6b69 652e 6765      if cookie.ge
-00001f00: 7428 226e 616d 6522 2920 3d3d 2022 5f55  t("name") == "_U
-00001f10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00001f20: 2020 2061 7267 732e 5520 3d20 636f 6f6b     args.U = cook
-00001f30: 6965 2e67 6574 2822 7661 6c75 6522 290a  ie.get("value").
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 6272 6561 6b0a 0a20 2020 2069 6620 6172  break..    if ar
-00001f60: 6773 2e55 2069 7320 4e6f 6e65 3a0a 2020  gs.U is None:.  
-00001f70: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-00001f80: 7074 696f 6e28 2243 6f75 6c64 206e 6f74  ption("Could not
-00001f90: 2066 696e 6420 6175 7468 2063 6f6f 6b69   find auth cooki
-00001fa0: 6522 290a 0a20 2020 2069 6620 6e6f 7420  e")..    if not 
-00001fb0: 6172 6773 2e61 7379 6e63 696f 3a0a 2020  args.asyncio:.  
-00001fc0: 2020 2020 2020 2320 4372 6561 7465 2069        # Create i
-00001fd0: 6d61 6765 2067 656e 6572 6174 6f72 0a20  mage generator. 
-00001fe0: 2020 2020 2020 2069 6d61 6765 5f67 656e         image_gen
-00001ff0: 6572 6174 6f72 203d 2049 6d61 6765 4765  erator = ImageGe
-00002000: 6e28 6172 6773 2e55 2c20 6172 6773 2e71  n(args.U, args.q
-00002010: 7569 6574 290a 2020 2020 2020 2020 696d  uiet).        im
-00002020: 6167 655f 6765 6e65 7261 746f 722e 7361  age_generator.sa
-00002030: 7665 5f69 6d61 6765 7328 0a20 2020 2020  ve_images(.     
-00002040: 2020 2020 2020 2069 6d61 6765 5f67 656e         image_gen
-00002050: 6572 6174 6f72 2e67 6574 5f69 6d61 6765  erator.get_image
-00002060: 7328 6172 6773 2e70 726f 6d70 7429 2c0a  s(args.prompt),.
-00002070: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00002080: 7574 5f64 6972 3d61 7267 732e 6f75 7470  ut_dir=args.outp
-00002090: 7574 5f64 6972 2c0a 2020 2020 2020 2020  ut_dir,.        
-000020a0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-000020b0: 2020 2020 6173 796e 6369 6f2e 7275 6e28      asyncio.run(
-000020c0: 6173 796e 635f 696d 6167 655f 6765 6e28  async_image_gen(
-000020d0: 6172 6773 2929 0a0a 6060 600a 0a3c 2f64  args))..```..</d
-000020e0: 6574 6169 6c73 3e0a 0a23 2053 7461 7220  etails>..# Star 
-000020f0: 4869 7374 6f72 790a 0a5b 215b 5374 6172  History..[![Star
-00002100: 2048 6973 746f 7279 2043 6861 7274 5d28   History Chart](
-00002110: 6874 7470 733a 2f2f 6170 692e 7374 6172  https://api.star
-00002120: 2d68 6973 746f 7279 2e63 6f6d 2f73 7667  -history.com/svg
-00002130: 3f72 6570 6f73 3d61 6368 656f 6e67 3038  ?repos=acheong08
-00002140: 2f45 6467 6547 5054 2674 7970 653d 4461  /EdgeGPT&type=Da
-00002150: 7465 295d 2868 7474 7073 3a2f 2f73 7461  te)](https://sta
-00002160: 722d 6869 7374 6f72 792e 636f 6d2f 2361  r-history.com/#a
-00002170: 6368 656f 6e67 3038 2f45 6467 6547 5054  cheong08/EdgeGPT
-00002180: 2644 6174 6529 0a0a 2320 436f 6e74 7269  &Date)..# Contri
-00002190: 6275 746f 7273 0a0a 5468 6973 2070 726f  butors..This pro
-000021a0: 6a65 6374 2065 7869 7374 7320 7468 616e  ject exists than
-000021b0: 6b73 2074 6f20 616c 6c20 7468 6520 7065  ks to all the pe
-000021c0: 6f70 6c65 2077 686f 2063 6f6e 7472 6962  ople who contrib
-000021d0: 7574 652e 0a0a 203c 6120 6872 6566 3d22  ute... <a href="
-000021e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000021f0: 6f6d 2f61 6368 656f 6e67 3038 2f45 6467  om/acheong08/Edg
-00002200: 6547 5054 2f67 7261 7068 732f 636f 6e74  eGPT/graphs/cont
-00002210: 7269 6275 746f 7273 223e 0a20 203c 696d  ributors">.  <im
-00002220: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
-00002230: 6f6e 7472 6962 2e72 6f63 6b73 2f69 6d61  ontrib.rocks/ima
-00002240: 6765 3f72 6570 6f3d 6163 6865 6f6e 6730  ge?repo=acheong0
-00002250: 382f 4564 6765 4750 5422 202f 3e0a 203c  8/EdgeGPT" />. <
-00002260: 2f61 3e0a                                /a>.
+00000720: 2061 6363 6573 7320 746f 203c 6874 7470   access to <http
+00000730: 733a 2f2f 6269 6e67 2e63 6f6d 2f63 6861  s://bing.com/cha
+00000740: 743e 2028 4f70 7469 6f6e 616c 290a 2d20  t> (Optional).- 
+00000750: 5265 7175 6972 6564 2069 6e20 6120 7375  Required in a su
+00000760: 7070 6f72 7465 6420 636f 756e 7472 7920  pported country 
+00000770: 6f72 2072 6567 696f 6e20 7769 7468 204e  or region with N
+00000780: 6577 2042 696e 6720 2843 6869 6e65 7365  ew Bing (Chinese
+00000790: 206d 6169 6e6c 616e 6420 5650 4e20 7265   mainland VPN re
+000007a0: 7175 6972 6564 290a 2d20 5b53 656c 656e  quired).- [Selen
+000007b0: 6975 6d5d 2868 7474 7073 3a2f 2f70 7970  ium](https://pyp
+000007c0: 692e 6f72 672f 7072 6f6a 6563 742f 7365  i.org/project/se
+000007d0: 6c65 6e69 756d 2f29 2028 666f 7220 6175  lenium/) (for au
+000007e0: 746f 6d61 7469 6320 636f 6f6b 6965 2073  tomatic cookie s
+000007f0: 6574 7570 290a 0a3c 6465 7461 696c 733e  etup)..<details>
+00000800: 0a0a 3c73 756d 6d61 7279 3e0a 0a23 2043  ..<summary>..# C
+00000810: 6861 7462 6f74 0a0a 3c2f 7375 6d6d 6172  hatbot..</summar
+00000820: 793e 0a0a 2323 2041 7574 6865 6e74 6963  y>..## Authentic
+00000830: 6174 696f 6e0a 0a21 2121 204e 4f54 2052  ation..!!! NOT R
+00000840: 4551 5549 5245 4420 414e 594d 4f52 4520  EQUIRED ANYMORE 
+00000850: 2121 210a 4d69 6372 6f73 6f66 7420 6861  !!!.Microsoft ha
+00000860: 7320 6d61 6465 2074 6865 2063 6861 7420  s made the chat 
+00000870: 6665 6174 7572 6520 6176 6169 6c61 626c  feature availabl
+00000880: 6520 746f 2065 7665 7279 6f6e 652c 2073  e to everyone, s
+00000890: 6f20 796f 7520 6361 6e20 736b 6970 2074  o you can skip t
+000008a0: 6869 7320 7374 6570 2e0a 0a31 2e20 496e  his step...1. In
+000008b0: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
+000008c0: 2076 6572 7369 6f6e 206f 6620 4d69 6372   version of Micr
+000008d0: 6f73 6f66 7420 4564 6765 0a3c 6465 7461  osoft Edge.<deta
+000008e0: 696c 733e 0a0a 322e 2041 6c74 6572 6e61  ils>..2. Alterna
+000008f0: 7469 7665 6c79 2c20 796f 7520 6361 6e20  tively, you can 
+00000900: 7573 6520 616e 7920 6272 6f77 7365 7220  use any browser 
+00000910: 616e 6420 7365 7420 7468 6520 7573 6572  and set the user
+00000920: 2d61 6765 6e74 2074 6f20 6c6f 6f6b 206c  -agent to look l
+00000930: 696b 6520 796f 7527 7265 2075 7369 6e67  ike you're using
+00000940: 2045 6467 6520 2865 2e67 2e2c 2060 4d6f   Edge (e.g., `Mo
+00000950: 7a69 6c6c 612f 352e 3020 2857 696e 646f  zilla/5.0 (Windo
+00000960: 7773 204e 5420 3130 2e30 3b20 5769 6e36  ws NT 10.0; Win6
+00000970: 343b 2078 3634 2920 4170 706c 6557 6562  4; x64) AppleWeb
+00000980: 4b69 742f 3533 372e 3336 2028 4b48 544d  Kit/537.36 (KHTM
+00000990: 4c2c 206c 696b 6520 4765 636b 6f29 2043  L, like Gecko) C
+000009a0: 6872 6f6d 652f 3131 312e 302e 302e 3020  hrome/111.0.0.0 
+000009b0: 5361 6661 7269 2f35 3337 2e33 3620 4564  Safari/537.36 Ed
+000009c0: 672f 3131 312e 302e 3136 3631 2e35 3160  g/111.0.1661.51`
+000009d0: 292e 2059 6f75 2063 616e 2064 6f20 7468  ). You can do th
+000009e0: 6973 2065 6173 696c 7920 7769 7468 2061  is easily with a
+000009f0: 6e20 6578 7465 6e73 696f 6e20 6c69 6b65  n extension like
+00000a00: 2022 5573 6572 2d41 6765 6e74 2053 7769   "User-Agent Swi
+00000a10: 7463 6865 7220 616e 6420 4d61 6e61 6765  tcher and Manage
+00000a20: 7222 2066 6f72 205b 4368 726f 6d65 5d28  r" for [Chrome](
+00000a30: 6874 7470 733a 2f2f 6368 726f 6d65 2e67  https://chrome.g
+00000a40: 6f6f 676c 652e 636f 6d2f 7765 6273 746f  oogle.com/websto
+00000a50: 7265 2f64 6574 6169 6c2f 7573 6572 2d61  re/detail/user-a
+00000a60: 6765 6e74 2d73 7769 7463 6865 722d 616e  gent-switcher-an
+00000a70: 642d 6d2f 6268 6368 6463 656a 686f 6866  d-m/bhchdcejhohf
+00000a80: 6d69 676a 6166 6261 6d70 6f67 6d61 616e  migjafbampogmaan
+00000a90: 6266 6b67 2920 616e 6420 5b46 6972 6566  bfkg) and [Firef
+00000aa0: 6f78 5d28 6874 7470 733a 2f2f 6164 646f  ox](https://addo
+00000ab0: 6e73 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  ns.mozilla.org/e
+00000ac0: 6e2d 5553 2f66 6972 6566 6f78 2f61 6464  n-US/firefox/add
+00000ad0: 6f6e 2f75 7365 722d 6167 656e 742d 7374  on/user-agent-st
+00000ae0: 7269 6e67 2d73 7769 7463 6865 722f 292e  ring-switcher/).
+00000af0: 0a0a 3c2f 6465 7461 696c 733e 0a0a 332e  ..</details>..3.
+00000b00: 204f 7065 6e20 5b62 696e 672e 636f 6d2f   Open [bing.com/
+00000b10: 6368 6174 5d28 6874 7470 733a 2f2f 6269  chat](https://bi
+00000b20: 6e67 2e63 6f6d 2f63 6861 7429 0a34 2e20  ng.com/chat).4. 
+00000b30: 4966 2079 6f75 2073 6565 2061 2063 6861  If you see a cha
+00000b40: 7420 6665 6174 7572 652c 2079 6f75 2061  t feature, you a
+00000b50: 7265 2067 6f6f 6420 746f 2063 6f6e 7469  re good to conti
+00000b60: 6e75 652e 2e2e 0a35 2e20 496e 7374 616c  nue....5. Instal
+00000b70: 6c20 7468 6520 636f 6f6b 6965 2065 6469  l the cookie edi
+00000b80: 746f 7220 6578 7465 6e73 696f 6e20 666f  tor extension fo
+00000b90: 7220 5b43 6872 6f6d 655d 2868 7474 7073  r [Chrome](https
+00000ba0: 3a2f 2f63 6872 6f6d 652e 676f 6f67 6c65  ://chrome.google
+00000bb0: 2e63 6f6d 2f77 6562 7374 6f72 652f 6465  .com/webstore/de
+00000bc0: 7461 696c 2f63 6f6f 6b69 652d 6564 6974  tail/cookie-edit
+00000bd0: 6f72 2f68 6c6b 656e 6e64 6564 6e68 666b  or/hlkenndednhfk
+00000be0: 656b 6867 6364 6963 6466 6464 6e6b 616c  ekhgcdicdfddnkal
+00000bf0: 6d64 6d29 206f 7220 5b46 6972 6566 6f78  mdm) or [Firefox
+00000c00: 5d28 6874 7470 733a 2f2f 6164 646f 6e73  ](https://addons
+00000c10: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00000c20: 5553 2f66 6972 6566 6f78 2f61 6464 6f6e  US/firefox/addon
+00000c30: 2f63 6f6f 6b69 652d 6564 6974 6f72 2f29  /cookie-editor/)
+00000c40: 0a36 2e20 476f 2074 6f20 5b62 696e 672e  .6. Go to [bing.
+00000c50: 636f 6d5d 2868 7474 7073 3a2f 2f62 696e  com](https://bin
+00000c60: 672e 636f 6d29 0a37 2e20 4f70 656e 2074  g.com).7. Open t
+00000c70: 6865 2065 7874 656e 7369 6f6e 0a38 2e20  he extension.8. 
+00000c80: 436c 6963 6b20 2245 7870 6f72 7422 206f  Click "Export" o
+00000c90: 6e20 7468 6520 626f 7474 6f6d 2072 6967  n the bottom rig
+00000ca0: 6874 2c20 7468 656e 2022 4578 706f 7274  ht, then "Export
+00000cb0: 2061 7320 4a53 4f4e 2220 2854 6869 7320   as JSON" (This 
+00000cc0: 7361 7665 7320 796f 7572 2063 6f6f 6b69  saves your cooki
+00000cd0: 6573 2074 6f20 636c 6970 626f 6172 6429  es to clipboard)
+00000ce0: 0a39 2e20 5061 7374 6520 796f 7572 2063  .9. Paste your c
+00000cf0: 6f6f 6b69 6573 2069 6e74 6f20 6120 6669  ookies into a fi
+00000d00: 6c65 2060 636f 6f6b 6965 732e 6a73 6f6e  le `cookies.json
+00000d10: 600a 0a23 2323 2049 6e20 636f 6465 3a0a  `..### In code:.
+00000d20: 6060 6070 7974 686f 6e0a 636f 6f6b 6965  ```python.cookie
+00000d30: 7320 3d20 6a73 6f6e 2e6c 6f61 6473 286f  s = json.loads(o
+00000d40: 7065 6e28 222e 2f70 6174 682f 746f 2f63  pen("./path/to/c
+00000d50: 6f6f 6b69 6573 2e6a 736f 6e22 2c20 656e  ookies.json", en
+00000d60: 636f 6469 6e67 3d22 7574 662d 3822 292e  coding="utf-8").
+00000d70: 7265 6164 2829 290a 626f 7420 3d20 6177  read()).bot = aw
+00000d80: 6169 7420 4368 6174 626f 742e 6372 6561  ait Chatbot.crea
+00000d90: 7465 2863 6f6f 6b69 6573 3d63 6f6f 6b69  te(cookies=cooki
+00000da0: 6573 290a 6060 600a 0a23 2320 5275 6e6e  es).```..## Runn
+00000db0: 696e 6720 6672 6f6d 2074 6865 2043 6f6d  ing from the Com
+00000dc0: 6d61 6e64 204c 696e 650a 0a60 6060 0a20  mand Line..```. 
+00000dd0: 2420 7079 7468 6f6e 3320 2d6d 2045 6467  $ python3 -m Edg
+00000de0: 6547 5054 202d 680a 0a20 2020 2020 2020  eGPT -h..       
+00000df0: 2045 6467 6547 5054 202d 2041 2064 656d   EdgeGPT - A dem
+00000e00: 6f20 6f66 2072 6576 6572 7365 2065 6e67  o of reverse eng
+00000e10: 696e 6565 7269 6e67 2074 6865 2042 696e  ineering the Bin
+00000e20: 6720 4750 5420 6368 6174 626f 740a 2020  g GPT chatbot.  
+00000e30: 2020 2020 2020 5265 706f 3a20 6769 7468        Repo: gith
+00000e40: 7562 2e63 6f6d 2f61 6368 656f 6e67 3038  ub.com/acheong08
+00000e50: 2f45 6467 6547 5054 0a20 2020 2020 2020  /EdgeGPT.       
+00000e60: 2042 793a 2041 6e74 6f6e 696f 2043 6865   By: Antonio Che
+00000e70: 6f6e 670a 0a20 2020 2020 2020 2021 6865  ong..        !he
+00000e80: 6c70 2066 6f72 2068 656c 700a 0a20 2020  lp for help..   
+00000e90: 2020 2020 2054 7970 6520 2165 7869 7420       Type !exit 
+00000ea0: 746f 2065 7869 740a 2020 2020 2020 2020  to exit.        
+00000eb0: 456e 7465 7220 7477 6963 6520 746f 2073  Enter twice to s
+00000ec0: 656e 6420 6d65 7373 6167 6520 6f72 2073  end message or s
+00000ed0: 6574 202d 2d65 6e74 6572 2d6f 6e63 6520  et --enter-once 
+00000ee0: 746f 2073 656e 6420 6f6e 6520 6c69 6e65  to send one line
+00000ef0: 206d 6573 7361 6765 0a0a 7573 6167 653a   message..usage:
+00000f00: 2045 6467 6547 5054 2e70 7920 5b2d 685d   EdgeGPT.py [-h]
+00000f10: 205b 2d2d 656e 7465 722d 6f6e 6365 5d20   [--enter-once] 
+00000f20: 5b2d 2d6e 6f2d 7374 7265 616d 5d20 5b2d  [--no-stream] [-
+00000f30: 2d72 6963 685d 205b 2d2d 7072 6f78 7920  -rich] [--proxy 
+00000f40: 5052 4f58 595d 205b 2d2d 7374 796c 6520  PROXY] [--style 
+00000f50: 7b63 7265 6174 6976 652c 6261 6c61 6e63  {creative,balanc
+00000f60: 6564 2c70 7265 6369 7365 7d5d 0a0a 6f70  ed,precise}]..op
+00000f70: 7469 6f6e 733a 0a20 202d 682c 202d 2d68  tions:.  -h, --h
+00000f80: 656c 7020 2020 2020 2020 2020 2020 2073  elp            s
+00000f90: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+00000fa0: 7373 6167 6520 616e 6420 6578 6974 0a20  ssage and exit. 
+00000fb0: 202d 2d65 6e74 6572 2d6f 6e63 650a 2020   --enter-once.  
+00000fc0: 2d2d 6e6f 2d73 7472 6561 6d0a 2020 2d2d  --no-stream.  --
+00000fd0: 7269 6368 0a20 202d 2d70 726f 7879 2050  rich.  --proxy P
+00000fe0: 524f 5859 2020 2020 2020 2020 2050 726f  ROXY         Pro
+00000ff0: 7879 2055 524c 2028 652e 672e 2073 6f63  xy URL (e.g. soc
+00001000: 6b73 353a 2f2f 3132 372e 302e 302e 313a  ks5://127.0.0.1:
+00001010: 3130 3830 290a 2020 2d2d 7374 796c 6520  1080).  --style 
+00001020: 7b63 7265 6174 6976 652c 6261 6c61 6e63  {creative,balanc
+00001030: 6564 2c70 7265 6369 7365 7d0a 2020 2d2d  ed,precise}.  --
+00001040: 636f 6f6b 6965 2d66 696c 6520 5b70 6174  cookie-file [pat
+00001050: 682f 746f 2f63 6f6f 6b69 6573 2e6a 736f  h/to/cookies.jso
+00001060: 6e5d 0a60 6060 0a0a 2323 2052 756e 6e69  n].```..## Runni
+00001070: 6e67 2069 6e20 5079 7468 6f6e 0a0a 2323  ng in Python..##
+00001080: 2320 312e 2054 6865 2060 4368 6174 626f  # 1. The `Chatbo
+00001090: 7460 2063 6c61 7373 2061 6e64 2060 6173  t` class and `as
+000010a0: 796e 6369 6f60 2066 6f72 206d 6f72 6520  yncio` for more 
+000010b0: 6772 616e 756c 6172 2063 6f6e 7472 6f6c  granular control
+000010c0: 0a0a 5573 6520 4173 796e 6320 666f 7220  ..Use Async for 
+000010d0: 7468 6520 6265 7374 2065 7870 6572 6965  the best experie
+000010e0: 6e63 652c 2066 6f72 2065 7861 6d70 6c65  nce, for example
+000010f0: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
+00001100: 6f72 7420 6173 796e 6369 6f0a 6672 6f6d  ort asyncio.from
+00001110: 2045 6467 6547 5054 2069 6d70 6f72 7420   EdgeGPT import 
+00001120: 4368 6174 626f 742c 2043 6f6e 7665 7273  Chatbot, Convers
+00001130: 6174 696f 6e53 7479 6c65 0a0a 6173 796e  ationStyle..asyn
+00001140: 6320 6465 6620 6d61 696e 2829 3a0a 2020  c def main():.  
+00001150: 2020 626f 7420 3d20 6177 6169 7420 4368    bot = await Ch
+00001160: 6174 626f 742e 6372 6561 7465 2829 2023  atbot.create() #
+00001170: 2050 6173 7369 6e67 2063 6f6f 6b69 6573   Passing cookies
+00001180: 2069 7320 6f70 7469 6f6e 616c 0a20 2020   is optional.   
+00001190: 2070 7269 6e74 2861 7761 6974 2062 6f74   print(await bot
+000011a0: 2e61 736b 2870 726f 6d70 743d 2248 656c  .ask(prompt="Hel
+000011b0: 6c6f 2077 6f72 6c64 222c 2063 6f6e 7665  lo world", conve
+000011c0: 7273 6174 696f 6e5f 7374 796c 653d 436f  rsation_style=Co
+000011d0: 6e76 6572 7361 7469 6f6e 5374 796c 652e  nversationStyle.
+000011e0: 6372 6561 7469 7665 2929 0a20 2020 2061  creative)).    a
+000011f0: 7761 6974 2062 6f74 2e63 6c6f 7365 2829  wait bot.close()
+00001200: 0a0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00001210: 2022 5f5f 6d61 696e 5f5f 223a 0a20 2020   "__main__":.   
+00001220: 2061 7379 6e63 696f 2e72 756e 286d 6169   asyncio.run(mai
+00001230: 6e28 2929 0a60 6060 0a0a 3c64 6574 6169  n()).```..<detai
+00001240: 6c73 3e0a 3c73 756d 6d61 7279 3e0a 0a23  ls>.<summary>..#
+00001250: 2323 2032 2920 5468 6520 6051 7565 7279  ## 2) The `Query
+00001260: 6020 616e 6420 6043 6f6f 6b69 6560 2068  ` and `Cookie` h
+00001270: 656c 7065 7220 636c 6173 7365 730a 0a20  elper classes.. 
+00001280: 203c 2f73 756d 6d61 7279 3e0a 0a43 7265   </summary>..Cre
+00001290: 6174 6520 6120 7369 6d70 6c65 2042 696e  ate a simple Bin
+000012a0: 6720 4368 6174 2041 4920 7175 6572 7920  g Chat AI query 
+000012b0: 2875 7369 6e67 2074 6865 2027 7072 6563  (using the 'prec
+000012c0: 6973 6527 2063 6f6e 7665 7273 6174 696f  ise' conversatio
+000012d0: 6e20 7374 796c 6520 6279 2064 6566 6175  n style by defau
+000012e0: 6c74 2920 616e 6420 7365 6520 6a75 7374  lt) and see just
+000012f0: 2074 6865 206d 6169 6e20 7465 7874 206f   the main text o
+00001300: 7574 7075 7420 7261 7468 6572 2074 6861  utput rather tha
+00001310: 6e20 7468 6520 7768 6f6c 6520 4150 4920  n the whole API 
+00001320: 7265 7370 6f6e 7365 3a0a 0a60 6060 7079  response:..```py
+00001330: 7468 6f6e 0a66 726f 6d20 4564 6765 4750  thon.from EdgeGP
+00001340: 5420 696d 706f 7274 2051 7565 7279 2c20  T import Query, 
+00001350: 436f 6f6b 6965 0a0a 7120 3d20 5175 6572  Cookie..q = Quer
+00001360: 7928 2257 6861 7420 6172 6520 796f 753f  y("What are you?
+00001370: 2047 6976 6520 796f 7572 2061 6e73 7765   Give your answe
+00001380: 7220 6173 2050 7974 686f 6e20 636f 6465  r as Python code
+00001390: 2229 0a70 7269 6e74 2871 290a 6060 600a  ").print(q).```.
+000013a0: 0a4f 7220 6368 616e 6765 2074 6865 2063  .Or change the c
+000013b0: 6f6e 7665 7273 6174 696f 6e20 7374 796c  onversation styl
+000013c0: 6520 6f72 2063 6f6f 6b69 6520 6669 6c65  e or cookie file
+000013d0: 2074 6f20 6265 2075 7365 643a 0a0a 6060   to be used:..``
+000013e0: 6070 7974 686f 6e0a 7120 3d20 5175 6572  `python.q = Quer
+000013f0: 7928 0a20 2022 5768 6174 2061 7265 2079  y(.  "What are y
+00001400: 6f75 3f20 4769 7665 2079 6f75 7220 616e  ou? Give your an
+00001410: 7377 6572 2061 7320 5079 7468 6f6e 2063  swer as Python c
+00001420: 6f64 6522 2c0a 2020 7374 796c 653d 2263  ode",.  style="c
+00001430: 7265 6174 6976 6522 2c20 2023 206f 7220  reative",  # or 
+00001440: 2762 616c 616e 6365 6427 0a20 2063 6f6f  'balanced'.  coo
+00001450: 6b69 6573 3d22 2e2f 6269 6e67 5f63 6f6f  kies="./bing_coo
+00001460: 6b69 6573 5f61 6c74 6572 6e61 7469 7665  kies_alternative
+00001470: 2e6a 736f 6e22 0a29 0a60 6060 0a0a 5175  .json".).```..Qu
+00001480: 6963 6b6c 7920 6578 7472 6163 7420 7468  ickly extract th
+00001490: 6520 7465 7874 206f 7574 7075 742c 2063  e text output, c
+000014a0: 6f64 6520 736e 6970 7065 7473 2c20 6c69  ode snippets, li
+000014b0: 7374 206f 6620 736f 7572 6365 732f 7265  st of sources/re
+000014c0: 6665 7265 6e63 6573 2c20 6f72 2073 7567  ferences, or sug
+000014d0: 6765 7374 6564 2066 6f6c 6c6f 772d 6f6e  gested follow-on
+000014e0: 2071 7565 7374 696f 6e73 2075 7369 6e67   questions using
+000014f0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2061   the following a
+00001500: 7474 7269 6275 7465 733a 0a0a 6060 6070  ttributes:..```p
+00001510: 7974 686f 6e0a 712e 6f75 7470 7574 0a71  ython.q.output.q
+00001520: 2e63 6f64 650a 712e 7375 6767 6573 7469  .code.q.suggesti
+00001530: 6f6e 730a 712e 736f 7572 6365 7320 2020  ons.q.sources   
+00001540: 2020 2020 2320 666f 7220 7468 6520 6675      # for the fu
+00001550: 6c6c 206a 736f 6e20 6f75 7470 7574 0a71  ll json output.q
+00001560: 2e73 6f75 7263 6573 5f64 6963 7420 2023  .sources_dict  #
+00001570: 2066 6f72 2061 2064 6963 7469 6f6e 6172   for a dictionar
+00001580: 7920 6f66 2074 6974 6c65 7320 616e 6420  y of titles and 
+00001590: 7572 6c73 0a60 6060 0a0a 4765 7420 7468  urls.```..Get th
+000015a0: 6520 6f72 6769 6e61 6c20 7072 6f6d 7074  e orginal prompt
+000015b0: 2061 6e64 2074 6865 2063 6f6e 7665 7273   and the convers
+000015c0: 6174 696f 6e20 7374 796c 6520 796f 7520  ation style you 
+000015d0: 7370 6563 6966 6965 643a 0a0a 6060 6070  specified:..```p
+000015e0: 7974 686f 6e0a 712e 7072 6f6d 7074 0a71  ython.q.prompt.q
+000015f0: 2e73 7479 6c65 0a72 6570 7228 7129 0a60  .style.repr(q).`
+00001600: 6060 0a0a 4163 6365 7373 2070 7265 7669  ``..Access previ
+00001610: 6f75 7320 5175 6572 6965 7320 6d61 6465  ous Queries made
+00001620: 2073 696e 6365 2069 6d70 6f72 7469 6e67   since importing
+00001630: 2060 5175 6572 7960 3a0a 0a60 6060 7079   `Query`:..```py
+00001640: 7468 6f6e 0a51 7565 7279 2e69 6e64 6578  thon.Query.index
+00001650: 2020 2320 4120 6c69 7374 206f 6620 5175    # A list of Qu
+00001660: 6572 7920 6f62 6a65 6374 733b 2075 7064  ery objects; upd
+00001670: 6174 6564 2064 796e 616d 6963 616c 6c79  ated dynamically
+00001680: 0a51 7565 7279 2e72 6571 7565 7374 5f63  .Query.request_c
+00001690: 6f75 6e74 2020 2320 4120 7461 6c6c 7920  ount  # A tally 
+000016a0: 6f66 2072 6571 7565 7374 7320 6d61 6465  of requests made
+000016b0: 2075 7369 6e67 2065 6163 6820 636f 6f6b   using each cook
+000016c0: 6965 2066 696c 650a 6060 600a 0a41 6e64  ie file.```..And
+000016d0: 2066 696e 616c 6c79 2c20 7468 6520 6043   finally, the `C
+000016e0: 6f6f 6b69 6560 2063 6c61 7373 2073 7570  ookie` class sup
+000016f0: 706f 7274 7320 6d75 6c74 6970 6c65 2063  ports multiple c
+00001700: 6f6f 6b69 6520 6669 6c65 732c 2073 6f20  ookie files, so 
+00001710: 6966 2079 6f75 2063 7265 6174 6520 6164  if you create ad
+00001720: 6469 7469 6f6e 616c 2063 6f6f 6b69 6520  ditional cookie 
+00001730: 6669 6c65 7320 7769 7468 2074 6865 206e  files with the n
+00001740: 616d 696e 6720 636f 6e76 656e 7469 6f6e  aming convention
+00001750: 2060 6269 6e67 5f63 6f6f 6b69 6573 5f2a   `bing_cookies_*
+00001760: 2e6a 736f 6e60 2c20 796f 7572 2071 7565  .json`, your que
+00001770: 7269 6573 2077 696c 6c20 6175 746f 6d61  ries will automa
+00001780: 7469 6361 6c6c 7920 7472 7920 7573 696e  tically try usin
+00001790: 6720 7468 6520 6e65 7874 2066 696c 6520  g the next file 
+000017a0: 2861 6c70 6861 6265 7469 6361 6c6c 7929  (alphabetically)
+000017b0: 2069 6620 796f 7527 7665 2065 7863 6565   if you've excee
+000017c0: 6465 6420 796f 7572 2064 6169 6c79 2071  ded your daily q
+000017d0: 756f 7461 206f 6620 7265 7175 6573 7473  uota of requests
+000017e0: 2028 6375 7272 656e 746c 7920 7365 7420   (currently set 
+000017f0: 6174 2032 3030 292e 0a0a 4865 7265 2061  at 200)...Here a
+00001800: 7265 2074 6865 206d 6169 6e20 6174 7472  re the main attr
+00001810: 6962 7574 6573 2077 6869 6368 2079 6f75  ibutes which you
+00001820: 2063 616e 2061 6363 6573 733a 0a0a 6060   can access:..``
+00001830: 6070 7974 686f 6e0a 436f 6f6b 6965 2e63  `python.Cookie.c
+00001840: 7572 7265 6e74 5f66 696c 655f 696e 6465  urrent_file_inde
+00001850: 780a 436f 6f6b 6965 2e64 6972 7061 7468  x.Cookie.dirpath
+00001860: 0a43 6f6f 6b69 652e 7365 6172 6368 5f70  .Cookie.search_p
+00001870: 6174 7465 726e 2020 2320 6465 6661 756c  attern  # defaul
+00001880: 7420 6973 2060 6269 6e67 5f63 6f6f 6b69  t is `bing_cooki
+00001890: 6573 5f2a 2e6a 736f 6e60 0a43 6f6f 6b69  es_*.json`.Cooki
+000018a0: 652e 6669 6c65 7328 2920 2023 206c 6973  e.files()  # lis
+000018b0: 7420 6173 2066 696c 6573 2074 6861 7420  t as files that 
+000018c0: 6d61 7463 6820 2e73 6561 7263 685f 7061  match .search_pa
+000018d0: 7474 6572 6e0a 436f 6f6b 6965 2e63 7572  ttern.Cookie.cur
+000018e0: 7265 6e74 5f66 696c 6570 6174 680a 436f  rent_filepath.Co
+000018f0: 6f6b 6965 2e63 7572 7265 6e74 5f64 6174  okie.current_dat
+00001900: 610a 436f 6f6b 6965 2e69 6d70 6f72 745f  a.Cookie.import_
+00001910: 6e65 7874 2829 0a43 6f6f 6b69 652e 696d  next().Cookie.im
+00001920: 6167 655f 746f 6b65 6e0a 436f 6f6b 6965  age_token.Cookie
+00001930: 2e69 676e 6f72 655f 6669 6c65 730a 6060  .ignore_files.``
+00001940: 600a 0a3c 2f64 6574 6169 6c73 3e0a 0a2d  `..</details>..-
+00001950: 2d2d 0a0a 2323 2052 756e 6e69 6e67 2077  --..## Running w
+00001960: 6974 6820 446f 636b 6572 0a0a 5468 6973  ith Docker..This
+00001970: 2061 7373 756d 6573 2079 6f75 2068 6176   assumes you hav
+00001980: 6520 6120 6669 6c65 2063 6f6f 6b69 6573  e a file cookies
+00001990: 2e6a 736f 6e20 696e 2079 6f75 7220 6375  .json in your cu
+000019a0: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
+000019b0: 7265 6374 6f72 790a 0a60 6060 6261 7368  rectory..```bash
+000019c0: 0a0a 646f 636b 6572 2072 756e 202d 2d72  ..docker run --r
+000019d0: 6d20 2d69 7420 2d76 2024 2870 7764 292f  m -it -v $(pwd)/
+000019e0: 636f 6f6b 6965 732e 6a73 6f6e 3a2f 636f  cookies.json:/co
+000019f0: 6f6b 6965 732e 6a73 6f6e 3a72 6f20 2d65  okies.json:ro -e
+00001a00: 2043 4f4f 4b49 455f 4649 4c45 3d27 2f63   COOKIE_FILE='/c
+00001a10: 6f6f 6b69 6573 2e6a 736f 6e27 2067 6863  ookies.json' ghc
+00001a20: 722e 696f 2f61 6368 656f 6e67 3038 2f65  r.io/acheong08/e
+00001a30: 6467 6567 7074 0a60 6060 0a0a 596f 7520  dgegpt.```..You 
+00001a40: 6361 6e20 6164 6420 616e 7920 6578 7472  can add any extr
+00001a50: 6120 666c 6167 7320 6173 2066 6f6c 6c6f  a flags as follo
+00001a60: 7769 6e67 0a0a 6060 6062 6173 680a 0a64  wing..```bash..d
+00001a70: 6f63 6b65 7220 7275 6e20 2d2d 726d 202d  ocker run --rm -
+00001a80: 6974 202d 7620 2428 7077 6429 2f63 6f6f  it -v $(pwd)/coo
+00001a90: 6b69 6573 2e6a 736f 6e3a 2f63 6f6f 6b69  kies.json:/cooki
+00001aa0: 6573 2e6a 736f 6e3a 726f 202d 6520 434f  es.json:ro -e CO
+00001ab0: 4f4b 4945 5f46 494c 453d 272f 636f 6f6b  OKIE_FILE='/cook
+00001ac0: 6965 732e 6a73 6f6e 2720 6768 6372 2e69  ies.json' ghcr.i
+00001ad0: 6f2f 6163 6865 6f6e 6730 382f 6564 6765  o/acheong08/edge
+00001ae0: 6770 7420 2d2d 7269 6368 202d 2d73 7479  gpt --rich --sty
+00001af0: 6c65 2063 7265 6174 6976 650a 6060 600a  le creative.```.
+00001b00: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00001b10: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
+00001b20: 3e0a 0a23 2049 6d61 6765 2067 656e 6572  >..# Image gener
+00001b30: 6174 6f72 0a0a 3c2f 7375 6d6d 6172 793e  ator..</summary>
+00001b40: 0a0a 2323 2052 756e 6e69 6e67 2066 726f  ..## Running fro
+00001b50: 6d20 7468 6520 436f 6d6d 616e 6420 4c69  m the Command Li
+00001b60: 6e65 0a0a 6060 6062 6173 680a 2420 7079  ne..```bash.$ py
+00001b70: 7468 6f6e 3320 2d6d 2049 6d61 6765 4765  thon3 -m ImageGe
+00001b80: 6e20 2d68 0a75 7361 6765 3a20 496d 6167  n -h.usage: Imag
+00001b90: 6547 656e 2e70 7920 5b2d 685d 205b 2d55  eGen.py [-h] [-U
+00001ba0: 2055 5d20 5b2d 2d63 6f6f 6b69 652d 6669   U] [--cookie-fi
+00001bb0: 6c65 2043 4f4f 4b49 455f 4649 4c45 5d20  le COOKIE_FILE] 
+00001bc0: 2d2d 7072 6f6d 7074 2050 524f 4d50 5420  --prompt PROMPT 
+00001bd0: 5b2d 2d6f 7574 7075 742d 6469 7220 4f55  [--output-dir OU
+00001be0: 5450 5554 5f44 4952 5d20 5b2d 2d71 7569  TPUT_DIR] [--qui
+00001bf0: 6574 5d20 5b2d 2d61 7379 6e63 696f 5d0a  et] [--asyncio].
+00001c00: 0a6f 7074 696f 6e61 6c20 6172 6775 6d65  .optional argume
+00001c10: 6e74 733a 0a20 202d 682c 202d 2d68 656c  nts:.  -h, --hel
+00001c20: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
+00001c30: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
+00001c40: 6167 6520 616e 6420 6578 6974 0a20 202d  age and exit.  -
+00001c50: 5520 5520 2020 2020 2020 2020 2020 2020  U U             
+00001c60: 2020 2020 2041 7574 6820 636f 6f6b 6965       Auth cookie
+00001c70: 2066 726f 6d20 6272 6f77 7365 720a 2020   from browser.  
+00001c80: 2d2d 636f 6f6b 6965 2d66 696c 6520 434f  --cookie-file CO
+00001c90: 4f4b 4945 5f46 494c 450a 2020 2020 2020  OKIE_FILE.      
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 2020 4669 6c65 2063 6f6e 7461 696e 696e    File containin
+00001cc0: 6720 6175 7468 2063 6f6f 6b69 650a 2020  g auth cookie.  
+00001cd0: 2d2d 7072 6f6d 7074 2050 524f 4d50 5420  --prompt PROMPT 
+00001ce0: 2020 2020 2020 5072 6f6d 7074 2074 6f20        Prompt to 
+00001cf0: 6765 6e65 7261 7465 2069 6d61 6765 7320  generate images 
+00001d00: 666f 720a 2020 2d2d 6f75 7470 7574 2d64  for.  --output-d
+00001d10: 6972 204f 5554 5055 545f 4449 520a 2020  ir OUTPUT_DIR.  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2020 4f75 7470 7574 2064 6972        Output dir
+00001d40: 6563 746f 7279 0a20 202d 2d71 7569 6574  ectory.  --quiet
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00001d60: 6973 6162 6c65 2070 6970 656c 696e 6520  isable pipeline 
+00001d70: 6d65 7373 6167 6573 0a20 202d 2d61 7379  messages.  --asy
+00001d80: 6e63 696f 2020 2020 2020 2020 2020 2020  ncio            
+00001d90: 2052 756e 2049 6d61 6765 4765 6e20 7573   Run ImageGen us
+00001da0: 696e 6720 6173 796e 6369 6f0a 6060 600a  ing asyncio.```.
+00001db0: 0a23 2320 5275 6e6e 696e 6720 696e 2050  .## Running in P
+00001dc0: 7974 686f 6e0a 0a23 2323 2031 2920 5468  ython..### 1) Th
+00001dd0: 6520 6049 6d61 6765 5175 6572 7960 2068  e `ImageQuery` h
+00001de0: 656c 7065 7220 636c 6173 730a 0a47 656e  elper class..Gen
+00001df0: 6572 6174 6520 696d 6167 6573 2062 6173  erate images bas
+00001e00: 6564 206f 6e20 6120 7369 6d70 6c65 2070  ed on a simple p
+00001e10: 726f 6d70 7420 616e 6420 646f 776e 6c6f  rompt and downlo
+00001e20: 6164 2074 6f20 7468 6520 6375 7272 656e  ad to the curren
+00001e30: 7420 776f 726b 696e 6720 6469 7265 6374  t working direct
+00001e40: 6f72 793a 0a0a 6060 6070 7974 686f 6e0a  ory:..```python.
+00001e50: 6672 6f6d 2045 6467 6547 5054 2069 6d70  from EdgeGPT imp
+00001e60: 6f72 7420 496d 6167 6551 7565 7279 0a0a  ort ImageQuery..
+00001e70: 713d 496d 6167 6551 7565 7279 2822 4d65  q=ImageQuery("Me
+00001e80: 6572 6b61 7473 2061 7420 6120 6761 7264  erkats at a gard
+00001e90: 656e 2070 6172 7479 2069 6e20 4465 766f  en party in Devo
+00001ea0: 6e22 290a 6060 600a 0a43 6861 6e67 6520  n").```..Change 
+00001eb0: 7468 6520 646f 776e 6c6f 6164 2064 6972  the download dir
+00001ec0: 6563 746f 7279 2066 6f72 2061 6c6c 2066  ectory for all f
+00001ed0: 7574 7572 6520 696d 6167 6573 2069 6e20  uture images in 
+00001ee0: 7468 6973 2073 6573 7369 6f6e 3a0a 0a60  this session:..`
+00001ef0: 6060 0a51 7565 7279 2e69 6d61 6765 5f64  ``.Query.image_d
+00001f00: 6972 7061 7468 203d 2050 6174 6828 222e  irpath = Path(".
+00001f10: 2f74 6f5f 616e 6f74 6865 725f 666f 6c64  /to_another_fold
+00001f20: 6572 2229 0a60 6060 0a0a 2323 2320 3229  er").```..### 2)
+00001f30: 2054 6865 2060 496d 6167 6547 656e 6020   The `ImageGen` 
+00001f40: 636c 6173 7320 616e 6420 6061 7379 6e63  class and `async
+00001f50: 696f 6020 666f 7220 6d6f 7265 2067 7261  io` for more gra
+00001f60: 6e75 6c61 7220 636f 6e74 726f 6c0a 0a60  nular control..`
+00001f70: 6060 7079 7468 6f6e 0a66 726f 6d20 496d  ``python.from Im
+00001f80: 6167 6547 656e 2069 6d70 6f72 7420 496d  ageGen import Im
+00001f90: 6167 6547 656e 0a69 6d70 6f72 7420 6172  ageGen.import ar
+00001fa0: 6770 6172 7365 0a69 6d70 6f72 7420 6a73  gparse.import js
+00001fb0: 6f6e 0a0a 6173 796e 6320 6465 6620 6173  on..async def as
+00001fc0: 796e 635f 696d 6167 655f 6765 6e28 6172  ync_image_gen(ar
+00001fd0: 6773 2920 2d3e 204e 6f6e 653a 0a20 2020  gs) -> None:.   
+00001fe0: 2061 7379 6e63 2077 6974 6820 496d 6167   async with Imag
+00001ff0: 6547 656e 4173 796e 6328 6172 6773 2e55  eGenAsync(args.U
+00002000: 2c20 6172 6773 2e71 7569 6574 2920 6173  , args.quiet) as
+00002010: 2069 6d61 6765 5f67 656e 6572 6174 6f72   image_generator
+00002020: 3a0a 2020 2020 2020 2020 696d 6167 6573  :.        images
+00002030: 203d 2061 7761 6974 2069 6d61 6765 5f67   = await image_g
+00002040: 656e 6572 6174 6f72 2e67 6574 5f69 6d61  enerator.get_ima
+00002050: 6765 7328 6172 6773 2e70 726f 6d70 7429  ges(args.prompt)
+00002060: 0a20 2020 2020 2020 2061 7761 6974 2069  .        await i
+00002070: 6d61 6765 5f67 656e 6572 6174 6f72 2e73  mage_generator.s
+00002080: 6176 655f 696d 6167 6573 2869 6d61 6765  ave_images(image
+00002090: 732c 206f 7574 7075 745f 6469 723d 6172  s, output_dir=ar
+000020a0: 6773 2e6f 7574 7075 745f 6469 7229 0a0a  gs.output_dir)..
+000020b0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
+000020c0: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2070  __main__":.    p
+000020d0: 6172 7365 7220 3d20 6172 6770 6172 7365  arser = argparse
+000020e0: 2e41 7267 756d 656e 7450 6172 7365 7228  .ArgumentParser(
+000020f0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00002100: 5f61 7267 756d 656e 7428 222d 5522 2c20  _argument("-U", 
+00002110: 6865 6c70 3d22 4175 7468 2063 6f6f 6b69  help="Auth cooki
+00002120: 6520 6672 6f6d 2062 726f 7773 6572 222c  e from browser",
+00002130: 2074 7970 653d 7374 7229 0a20 2020 2070   type=str).    p
+00002140: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00002150: 6e74 2822 2d2d 636f 6f6b 6965 2d66 696c  nt("--cookie-fil
+00002160: 6522 2c20 6865 6c70 3d22 4669 6c65 2063  e", help="File c
+00002170: 6f6e 7461 696e 696e 6720 6175 7468 2063  ontaining auth c
+00002180: 6f6f 6b69 6522 2c20 7479 7065 3d73 7472  ookie", type=str
+00002190: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+000021a0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+000021b0: 2020 2022 2d2d 7072 6f6d 7074 222c 0a20     "--prompt",. 
+000021c0: 2020 2020 2020 2068 656c 703d 2250 726f         help="Pro
+000021d0: 6d70 7420 746f 2067 656e 6572 6174 6520  mpt to generate 
+000021e0: 696d 6167 6573 2066 6f72 222c 0a20 2020  images for",.   
+000021f0: 2020 2020 2074 7970 653d 7374 722c 0a20       type=str,. 
+00002200: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00002210: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+00002220: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00002230: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
+00002240: 6f75 7470 7574 2d64 6972 222c 0a20 2020  output-dir",.   
+00002250: 2020 2020 2068 656c 703d 224f 7574 7075       help="Outpu
+00002260: 7420 6469 7265 6374 6f72 7922 2c0a 2020  t directory",.  
+00002270: 2020 2020 2020 7479 7065 3d73 7472 2c0a        type=str,.
+00002280: 2020 2020 2020 2020 6465 6661 756c 743d          default=
+00002290: 222e 2f6f 7574 7075 7422 2c0a 2020 2020  "./output",.    
+000022a0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+000022b0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+000022c0: 2020 2022 2d2d 7175 6965 7422 2c20 6865     "--quiet", he
+000022d0: 6c70 3d22 4469 7361 626c 6520 7069 7065  lp="Disable pipe
+000022e0: 6c69 6e65 206d 6573 7361 6765 7322 2c20  line messages", 
+000022f0: 6163 7469 6f6e 3d22 7374 6f72 655f 7472  action="store_tr
+00002300: 7565 220a 2020 2020 290a 2020 2020 7061  ue".    ).    pa
+00002310: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00002320: 7428 0a20 2020 2020 2020 2022 2d2d 6173  t(.        "--as
+00002330: 796e 6369 6f22 2c20 6865 6c70 3d22 5275  yncio", help="Ru
+00002340: 6e20 496d 6167 6547 656e 2075 7369 6e67  n ImageGen using
+00002350: 2061 7379 6e63 696f 222c 2061 6374 696f   asyncio", actio
+00002360: 6e3d 2273 746f 7265 5f74 7275 6522 0a20  n="store_true". 
+00002370: 2020 2029 0a20 2020 2061 7267 7320 3d20     ).    args = 
+00002380: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00002390: 7328 290a 2020 2020 2320 4c6f 6164 2061  s().    # Load a
+000023a0: 7574 6820 636f 6f6b 6965 0a20 2020 2077  uth cookie.    w
+000023b0: 6974 6820 6f70 656e 2861 7267 732e 636f  ith open(args.co
+000023c0: 6f6b 6965 5f66 696c 652c 2065 6e63 6f64  okie_file, encod
+000023d0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+000023e0: 6669 6c65 3a0a 2020 2020 2020 2020 636f  file:.        co
+000023f0: 6f6b 6965 5f6a 736f 6e20 3d20 6a73 6f6e  okie_json = json
+00002400: 2e6c 6f61 6428 6669 6c65 290a 2020 2020  .load(file).    
+00002410: 2020 2020 666f 7220 636f 6f6b 6965 2069      for cookie i
+00002420: 6e20 636f 6f6b 6965 5f6a 736f 6e3a 0a20  n cookie_json:. 
+00002430: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00002440: 6f6b 6965 2e67 6574 2822 6e61 6d65 2229  okie.get("name")
+00002450: 203d 3d20 225f 5522 3a0a 2020 2020 2020   == "_U":.      
+00002460: 2020 2020 2020 2020 2020 6172 6773 2e55            args.U
+00002470: 203d 2063 6f6f 6b69 652e 6765 7428 2276   = cookie.get("v
+00002480: 616c 7565 2229 0a20 2020 2020 2020 2020  alue").         
+00002490: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+000024a0: 2020 6966 2061 7267 732e 5520 6973 204e    if args.U is N
+000024b0: 6f6e 653a 0a20 2020 2020 2020 2072 6169  one:.        rai
+000024c0: 7365 2045 7863 6570 7469 6f6e 2822 436f  se Exception("Co
+000024d0: 756c 6420 6e6f 7420 6669 6e64 2061 7574  uld not find aut
+000024e0: 6820 636f 6f6b 6965 2229 0a0a 2020 2020  h cookie")..    
+000024f0: 6966 206e 6f74 2061 7267 732e 6173 796e  if not args.asyn
+00002500: 6369 6f3a 0a20 2020 2020 2020 2023 2043  cio:.        # C
+00002510: 7265 6174 6520 696d 6167 6520 6765 6e65  reate image gene
+00002520: 7261 746f 720a 2020 2020 2020 2020 696d  rator.        im
+00002530: 6167 655f 6765 6e65 7261 746f 7220 3d20  age_generator = 
+00002540: 496d 6167 6547 656e 2861 7267 732e 552c  ImageGen(args.U,
+00002550: 2061 7267 732e 7175 6965 7429 0a20 2020   args.quiet).   
+00002560: 2020 2020 2069 6d61 6765 5f67 656e 6572       image_gener
+00002570: 6174 6f72 2e73 6176 655f 696d 6167 6573  ator.save_images
+00002580: 280a 2020 2020 2020 2020 2020 2020 696d  (.            im
+00002590: 6167 655f 6765 6e65 7261 746f 722e 6765  age_generator.ge
+000025a0: 745f 696d 6167 6573 2861 7267 732e 7072  t_images(args.pr
+000025b0: 6f6d 7074 292c 0a20 2020 2020 2020 2020  ompt),.         
+000025c0: 2020 206f 7574 7075 745f 6469 723d 6172     output_dir=ar
+000025d0: 6773 2e6f 7574 7075 745f 6469 722c 0a20  gs.output_dir,. 
+000025e0: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
+000025f0: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
+00002600: 696f 2e72 756e 2861 7379 6e63 5f69 6d61  io.run(async_ima
+00002610: 6765 5f67 656e 2861 7267 7329 290a 0a60  ge_gen(args))..`
+00002620: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00002630: 2320 5374 6172 2048 6973 746f 7279 0a0a  # Star History..
+00002640: 5b21 5b53 7461 7220 4869 7374 6f72 7920  [![Star History 
+00002650: 4368 6172 745d 2868 7474 7073 3a2f 2f61  Chart](https://a
+00002660: 7069 2e73 7461 722d 6869 7374 6f72 792e  pi.star-history.
+00002670: 636f 6d2f 7376 673f 7265 706f 733d 6163  com/svg?repos=ac
+00002680: 6865 6f6e 6730 382f 4564 6765 4750 5426  heong08/EdgeGPT&
+00002690: 7479 7065 3d44 6174 6529 5d28 6874 7470  type=Date)](http
+000026a0: 733a 2f2f 7374 6172 2d68 6973 746f 7279  s://star-history
+000026b0: 2e63 6f6d 2f23 6163 6865 6f6e 6730 382f  .com/#acheong08/
+000026c0: 4564 6765 4750 5426 4461 7465 290a 0a23  EdgeGPT&Date)..#
+000026d0: 2043 6f6e 7472 6962 7574 6f72 730a 0a54   Contributors..T
+000026e0: 6869 7320 7072 6f6a 6563 7420 6578 6973  his project exis
+000026f0: 7473 2074 6861 6e6b 7320 746f 2061 6c6c  ts thanks to all
+00002700: 2074 6865 2070 656f 706c 6520 7768 6f20   the people who 
+00002710: 636f 6e74 7269 6275 7465 2e0a 0a20 3c61  contribute... <a
+00002720: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002730: 6974 6875 622e 636f 6d2f 6163 6865 6f6e  ithub.com/acheon
+00002740: 6730 382f 4564 6765 4750 542f 6772 6170  g08/EdgeGPT/grap
+00002750: 6873 2f63 6f6e 7472 6962 7574 6f72 7322  hs/contributors"
+00002760: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
+00002770: 7470 733a 2f2f 636f 6e74 7269 622e 726f  tps://contrib.ro
+00002780: 636b 732f 696d 6167 653f 7265 706f 3d61  cks/image?repo=a
+00002790: 6368 656f 6e67 3038 2f45 6467 6547 5054  cheong08/EdgeGPT
+000027a0: 2220 2f3e 0a20 3c2f 613e 0a              " />. </a>.
```

### Comparing `EdgeGPT-0.6.2/src/EdgeGPT.py` & `EdgeGPT-0.6.3/src/EdgeGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import ssl
 import sys
 import time
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
-from typing import Literal
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 from typing import Optional
 from typing import Union
 
 import aiohttp
 import certifi
 import httpx
 from BingImageCreator import ImageGen
@@ -1020,15 +1023,15 @@
     async def send_to_bing(self, echo=True, echo_prompt=False):
         """Creat, submit, then close a Chatbot instance.  Return the response"""
         retries = len(Cookie.files())
         while retries:
             try:
                 bot = await Chatbot.create()
                 if echo_prompt:
-                    print(f"> {self.prompt=}")
+                    print(f"> {self.prompt}=")
                 if echo:
                     print("> Waiting for response...")
                 if self.style.lower() not in "creative balanced precise".split():
                     self.style = "precise"
                 response = await bot.ask(
                     prompt=self.prompt,
                     conversation_style=getattr(ConversationStyle, self.style),
```

