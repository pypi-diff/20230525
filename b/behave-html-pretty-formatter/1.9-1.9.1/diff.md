# Comparing `tmp/behave-html-pretty-formatter-1.9.tar.gz` & `tmp/behave-html-pretty-formatter-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behave-html-pretty-formatter-1.9.tar", last modified: Wed May 24 10:41:00 2023, max compression
+gzip compressed data, was "behave-html-pretty-formatter-1.9.1.tar", last modified: Thu May 25 09:04:02 2023, max compression
```

## Comparing `behave-html-pretty-formatter-1.9.tar` & `behave-html-pretty-formatter-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.css
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.js
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39409 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/html_pretty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 10:41:00.000000 behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 10:41:00.928940 behave-html-pretty-formatter-1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-24 10:40:41.000000 behave-html-pretty-formatter-1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:02.864025 behave-html-pretty-formatter-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-25 09:04:02.864025 behave-html-pretty-formatter-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:02.864025 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39409 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/html_pretty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:02.864025 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-25 09:04:02.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-25 09:04:02.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:02.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:04:02.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 09:04:02.000000 behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:04:02.864025 behave-html-pretty-formatter-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-25 09:03:43.000000 behave-html-pretty-formatter-1.9.1/setup.py
```

### Comparing `behave-html-pretty-formatter-1.9/LICENSE` & `behave-html-pretty-formatter-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.9/PKG-INFO` & `behave-html-pretty-formatter-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-html-pretty-formatter
-Version: 1.9
+Version: 1.9.1
 Summary: Pretty HTML Formatter for Behave
 Home-page: https://github.com/behave-contrib/behave-html-pretty-formatter
 Author: Michal Odehnal
 Author-email: modehnal@redhat.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `behave-html-pretty-formatter-1.9/README.md` & `behave-html-pretty-formatter-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.css` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.css`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.js` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 1% similar despite different names*

```diff
@@ -153,354 +153,354 @@
 00000980: 6765 2075 7569 6420 6c69 7374 0a20 2020  ge uuid list.   
 00000990: 2069 6620 2868 6173 685f 7575 6964 5f6c   if (hash_uuid_l
 000009a0: 6973 742e 696e 636c 7564 6573 2869 6429  ist.includes(id)
 000009b0: 2920 7b0a 2020 2020 2020 2020 6861 7368  ) {.        hash
 000009c0: 5f75 7569 645f 6c69 7374 2e73 706c 6963  _uuid_list.splic
 000009d0: 6528 6861 7368 5f75 7569 645f 6c69 7374  e(hash_uuid_list
 000009e0: 2e69 6e64 6578 4f66 2869 6429 2c20 3129  .indexOf(id), 1)
-000009f0: 3b0a 2020 2020 7d0a 2020 2020 656c 7365  ;.    }.    else
-00000a00: 207b 0a20 2020 2020 2020 2068 6173 685f   {.        hash_
-00000a10: 7575 6964 5f6c 6973 742e 7075 7368 2869  uuid_list.push(i
-00000a20: 6429 3b0a 2020 2020 7d0a 2020 2020 2f2f  d);.    }.    //
-00000a30: 2055 7064 6174 6520 5552 4c20 6861 7368   Update URL hash
-00000a40: 0a20 2020 2076 6172 2068 6173 6820 3d20  .    var hash = 
-00000a50: 2223 223b 0a20 2020 2069 6620 2868 6173  "#";.    if (has
-00000a60: 685f 7575 6964 5f6c 6973 742e 6c65 6e67  h_uuid_list.leng
-00000a70: 7468 2021 3d20 3029 207b 0a20 2020 2020  th != 0) {.     
-00000a80: 2020 2068 6173 6820 3d20 746f 6767 6c65     hash = toggle
-00000a90: 5f6e 6f6e 5f65 6d70 7479 5f73 7472 696e  _non_empty_strin
-00000aa0: 6720 2b20 6861 7368 5f75 7569 645f 6c69  g + hash_uuid_li
-00000ab0: 7374 2e74 6f53 7472 696e 6728 290a 2020  st.toString().  
-00000ac0: 2020 7d0a 2020 2020 636f 6e73 6f6c 652e    }.    console.
-00000ad0: 6c6f 6728 224e 6577 2068 6173 683a 2022  log("New hash: "
-00000ae0: 202b 2068 6173 6829 3b0a 2020 2020 6869   + hash);.    hi
-00000af0: 7374 6f72 792e 7265 706c 6163 6553 7461  story.replaceSta
-00000b00: 7465 2875 6e64 6566 696e 6564 2c20 756e  te(undefined, un
-00000b10: 6465 6669 6e65 642c 2068 6173 6829 3b0a  defined, hash);.
-00000b20: 2020 2020 2f2f 204e 6565 6420 746f 2063      // Need to c
-00000b30: 616c 6c20 6861 7368 5f74 6f5f 7374 6174  all hash_to_stat
-00000b40: 652c 2065 7665 6e74 2069 7320 6e6f 7420  e, event is not 
-00000b50: 7472 6967 6765 7265 6420 666f 7220 736f  triggered for so
-00000b60: 6d65 2072 6561 736f 6e0a 2020 2020 6861  me reason.    ha
-00000b70: 7368 5f74 6f5f 7374 6174 6528 293b 0a7d  sh_to_state();.}
-00000b80: 0a0a 6675 6e63 7469 6f6e 2063 6f6c 6c61  ..function colla
-00000b90: 7073 6962 6c65 5f74 6f67 676c 6528 6964  psible_toggle(id
-00000ba0: 2920 7b0a 2020 2020 636f 6e73 6f6c 652e  ) {.    console.
-00000bb0: 6c6f 6728 2254 6f67 676c 6520 656d 6265  log("Toggle embe
-00000bc0: 643a 2022 202b 2069 6429 3b0a 2020 2020  d: " + id);.    
-00000bd0: 7661 7220 656d 6265 645f 6275 7474 6f6e  var embed_button
-00000be0: 5f69 6420 3d20 2265 6d62 6564 5f62 7574  _id = "embed_but
-00000bf0: 746f 6e5f 2220 2b20 6964 0a20 2020 2076  ton_" + id.    v
-00000c00: 6172 2070 6172 656e 7420 3d20 646f 6375  ar parent = docu
-00000c10: 6d65 6e74 2e67 6574 456c 656d 656e 7442  ment.getElementB
-00000c20: 7949 6428 656d 6265 645f 6275 7474 6f6e  yId(embed_button
-00000c30: 5f69 6429 3b0a 2020 2020 6966 2028 7061  _id);.    if (pa
-00000c40: 7265 6e74 203d 3d3d 206e 756c 6c29 207b  rent === null) {
-00000c50: 0a20 2020 2020 2020 2072 6574 7572 6e3b  .        return;
-00000c60: 0a20 2020 207d 0a20 2020 2077 6869 6c65  .    }.    while
-00000c70: 2028 7061 7265 6e74 2021 3d3d 2075 6e64   (parent !== und
-00000c80: 6566 696e 6564 2026 2620 2170 6172 656e  efined && !paren
-00000c90: 742e 636c 6173 734c 6973 742e 636f 6e74  t.classList.cont
-00000ca0: 6169 6e73 2822 656d 6265 645f 6275 7474  ains("embed_butt
-00000cb0: 6f6e 2229 2920 7b0a 2020 2020 2020 2020  on")) {.        
-00000cc0: 7061 7265 6e74 203d 2070 6172 656e 742e  parent = parent.
-00000cd0: 7061 7265 6e74 456c 656d 656e 743b 0a20  parentElement;. 
-00000ce0: 2020 207d 0a20 2020 2069 6620 2870 6172     }.    if (par
-00000cf0: 656e 7420 213d 3d20 756e 6465 6669 6e65  ent !== undefine
-00000d00: 6429 207b 0a20 2020 2020 2020 2074 6f67  d) {.        tog
-00000d10: 676c 655f 636c 6173 7328 7061 7265 6e74  gle_class(parent
-00000d20: 2c20 2263 6f6c 6c61 7073 6522 293b 0a20  , "collapse");. 
-00000d30: 2020 207d 0a0a 2020 2020 7661 7220 656d     }..    var em
-00000d40: 6265 645f 636f 6e74 656e 745f 6964 203d  bed_content_id =
-00000d50: 2022 656d 6265 645f 2220 2b20 6964 0a20   "embed_" + id. 
-00000d60: 2020 2076 6172 2065 6c65 6d20 3d20 646f     var elem = do
-00000d70: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
-00000d80: 7442 7949 6428 656d 6265 645f 636f 6e74  tById(embed_cont
-00000d90: 656e 745f 6964 293b 0a20 2020 2074 6f67  ent_id);.    tog
-00000da0: 676c 655f 636c 6173 7328 656c 656d 2c20  gle_class(elem, 
-00000db0: 2263 6f6c 6c61 7073 6522 293b 0a7d 3b0a  "collapse");.};.
-00000dc0: 0a66 756e 6374 696f 6e20 636f 6c6c 6170  .function collap
-00000dd0: 7369 626c 655f 7375 6d6d 6172 7928 636c  sible_summary(cl
-00000de0: 6173 736e 616d 6529 207b 0a20 2020 2076  assname) {.    v
-00000df0: 6172 2065 6c65 6d20 3d20 646f 6375 6d65  ar elem = docume
-00000e00: 6e74 2e67 6574 456c 656d 656e 7473 4279  nt.getElementsBy
-00000e10: 436c 6173 734e 616d 6528 636c 6173 736e  ClassName(classn
-00000e20: 616d 6529 3b0a 2020 2020 666f 7220 2876  ame);.    for (v
-00000e30: 6172 2069 203d 2030 3b20 6920 3c20 656c  ar i = 0; i < el
-00000e40: 656d 2e6c 656e 6774 683b 2069 2b2b 2920  em.length; i++) 
-00000e50: 7b0a 2020 2020 2020 2020 746f 6767 6c65  {.        toggle
-00000e60: 5f63 6c61 7373 2865 6c65 6d5b 695d 2c20  _class(elem[i], 
-00000e70: 2263 6f6c 6c61 7073 6522 293b 0a20 2020  "collapse");.   
-00000e80: 207d 0a7d 3b0a 0a66 756e 6374 696f 6e20   }.};..function 
-00000e90: 6578 7061 6e64 6572 2861 6374 696f 6e2c  expander(action,
-00000ea0: 2073 756d 6d61 7279 5f62 6c6f 636b 2920   summary_block) 
-00000eb0: 7b0a 2020 2020 7661 7220 656c 656d 203d  {.    var elem =
-00000ec0: 2041 7272 6179 2e66 726f 6d28 646f 6375   Array.from(docu
-00000ed0: 6d65 6e74 2e67 6574 456c 656d 656e 7473  ment.getElements
-00000ee0: 4279 436c 6173 734e 616d 6528 2273 6365  ByClassName("sce
-00000ef0: 6e61 7269 6f2d 6361 7073 756c 6522 2929  nario-capsule"))
-00000f00: 3b0a 2020 2020 656c 656d 203d 2065 6c65  ;.    elem = ele
-00000f10: 6d2e 636f 6e63 6174 2841 7272 6179 2e66  m.concat(Array.f
-00000f20: 726f 6d28 646f 6375 6d65 6e74 2e67 6574  rom(document.get
-00000f30: 456c 656d 656e 7473 4279 436c 6173 734e  ElementsByClassN
-00000f40: 616d 6528 2273 6365 6e61 7269 6f2d 6865  ame("scenario-he
-00000f50: 6164 6572 2229 2929 3b0a 2020 2020 7661  ader")));.    va
-00000f60: 7220 6665 6174 7572 655f 6964 203d 2073  r feature_id = s
-00000f70: 756d 6d61 7279 5f62 6c6f 636b 2e70 6172  ummary_block.par
-00000f80: 656e 7445 6c65 6d65 6e74 2e70 6172 656e  entElement.paren
-00000f90: 7445 6c65 6d65 6e74 2e69 640a 2020 2020  tElement.id.    
-00000fa0: 666f 7220 2876 6172 2069 203d 2030 3b20  for (var i = 0; 
-00000fb0: 6920 3c20 656c 656d 2e6c 656e 6774 683b  i < elem.length;
-00000fc0: 2069 2b2b 2920 7b0a 2020 2020 2020 2020   i++) {.        
-00000fd0: 6966 2028 6665 6174 7572 655f 6964 2021  if (feature_id !
-00000fe0: 3d20 656c 656d 5b69 5d2e 7061 7265 6e74  = elem[i].parent
-00000ff0: 456c 656d 656e 742e 6964 2920 7b0a 2020  Element.id) {.  
-00001000: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00001010: 7565 0a20 2020 2020 2020 207d 0a20 2020  ue.        }.   
-00001020: 2020 2020 2069 6620 2861 6374 696f 6e20       if (action 
-00001030: 3d3d 2022 6578 7061 6e64 5f61 6c6c 2229  == "expand_all")
-00001040: 207b 0a20 2020 2020 2020 2020 2020 2065   {.            e
-00001050: 6c65 6d5b 695d 2e63 6c61 7373 4c69 7374  lem[i].classList
-00001060: 2e72 656d 6f76 6528 2263 6f6c 6c61 7073  .remove("collaps
-00001070: 6522 290a 2020 2020 2020 2020 7d20 656c  e").        } el
-00001080: 7365 2069 6620 2861 6374 696f 6e20 3d3d  se if (action ==
-00001090: 2022 636f 6c6c 6170 7365 5f61 6c6c 2229   "collapse_all")
-000010a0: 207b 0a20 2020 2020 2020 2020 2020 2069   {.            i
-000010b0: 6620 2821 656c 656d 5b69 5d2e 636c 6173  f (!elem[i].clas
-000010c0: 734c 6973 742e 636f 6e74 6169 6e73 2822  sList.contains("
-000010d0: 636f 6c6c 6170 7365 2229 2920 7b0a 2020  collapse")) {.  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000010f0: 656d 5b69 5d2e 636c 6173 734c 6973 742e  em[i].classList.
-00001100: 6164 6428 2263 6f6c 6c61 7073 6522 293b  add("collapse");
-00001110: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00001120: 2020 2020 2020 207d 2065 6c73 6520 6966         } else if
-00001130: 2028 6163 7469 6f6e 203d 3d20 2265 7870   (action == "exp
-00001140: 616e 645f 616c 6c5f 6661 696c 6564 2229  and_all_failed")
-00001150: 207b 0a20 2020 2020 2020 2020 2020 2069   {.            i
-00001160: 6620 2821 656c 656d 5b69 5d2e 636c 6173  f (!elem[i].clas
-00001170: 734c 6973 742e 636f 6e74 6169 6e73 2822  sList.contains("
-00001180: 7061 7373 6564 2229 2920 7b0a 2020 2020  passed")) {.    
-00001190: 2020 2020 2020 2020 2020 2020 656c 656d              elem
-000011a0: 5b69 5d2e 636c 6173 734c 6973 742e 7265  [i].classList.re
-000011b0: 6d6f 7665 2822 636f 6c6c 6170 7365 2229  move("collapse")
-000011c0: 3b0a 2020 2020 2020 2020 2020 2020 7d20  ;.            } 
-000011d0: 656c 7365 207b 0a20 2020 2020 2020 2020  else {.         
-000011e0: 2020 2020 2020 2069 6620 2821 656c 656d         if (!elem
-000011f0: 5b69 5d2e 636c 6173 734c 6973 742e 636f  [i].classList.co
-00001200: 6e74 6169 6e73 2822 636f 6c6c 6170 7365  ntains("collapse
-00001210: 2229 2920 7b0a 2020 2020 2020 2020 2020  ")) {.          
-00001220: 2020 2020 2020 2020 2020 656c 656d 5b69            elem[i
-00001230: 5d2e 636c 6173 734c 6973 742e 6164 6428  ].classList.add(
-00001240: 2263 6f6c 6c61 7073 6522 293b 0a20 2020  "collapse");.   
-00001250: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00001260: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00001270: 2020 2020 207d 0a20 2020 207d 0a7d 3b0a       }.    }.};.
-00001280: 0a0a 6675 6e63 7469 6f6e 2065 7870 616e  ..function expan
-00001290: 645f 7468 6973 5f6f 6e6c 7928 6e61 6d65  d_this_only(name
-000012a0: 2920 7b0a 2020 2020 7661 7220 6964 203d  ) {.    var id =
-000012b0: 206e 616d 652e 6964 3b0a 2020 2020 7661   name.id;.    va
-000012c0: 7220 6361 7073 756c 6520 3d20 646f 6375  r capsule = docu
-000012d0: 6d65 6e74 2e67 6574 456c 656d 656e 7442  ment.getElementB
-000012e0: 7949 6428 6964 202b 2022 2d63 2229 3b0a  yId(id + "-c");.
-000012f0: 2020 2020 7661 7220 6865 6164 6572 203d      var header =
-00001300: 2064 6f63 756d 656e 742e 6765 7445 6c65   document.getEle
-00001310: 6d65 6e74 4279 4964 2869 6420 2b20 222d  mentById(id + "-
-00001320: 6822 293b 0a20 2020 2069 6620 2868 6561  h");.    if (hea
-00001330: 6465 722e 636c 6173 734c 6973 742e 636f  der.classList.co
-00001340: 6e74 6169 6e73 2822 636f 6c6c 6170 7365  ntains("collapse
-00001350: 2229 2920 7b0a 2020 2020 2020 2020 6865  ")) {.        he
-00001360: 6164 6572 2e63 6c61 7373 4c69 7374 2e72  ader.classList.r
-00001370: 656d 6f76 6528 2263 6f6c 6c61 7073 6522  emove("collapse"
-00001380: 293b 0a20 2020 2020 2020 2063 6170 7375  );.        capsu
-00001390: 6c65 2e63 6c61 7373 4c69 7374 2e72 656d  le.classList.rem
-000013a0: 6f76 6528 2263 6f6c 6c61 7073 6522 293b  ove("collapse");
-000013b0: 0a20 2020 207d 2065 6c73 6520 7b0a 2020  .    } else {.  
-000013c0: 2020 2020 2020 6865 6164 6572 2e63 6c61        header.cla
-000013d0: 7373 4c69 7374 2e61 6464 2822 636f 6c6c  ssList.add("coll
-000013e0: 6170 7365 2229 3b0a 2020 2020 2020 2020  apse");.        
-000013f0: 6361 7073 756c 652e 636c 6173 734c 6973  capsule.classLis
-00001400: 742e 6164 6428 2263 6f6c 6c61 7073 6522  t.add("collapse"
-00001410: 293b 0a20 2020 207d 0a7d 3b0a 0a2f 2f20  );.    }.};..// 
-00001420: 4865 6c70 6572 2066 756e 6374 696f 6e20  Helper function 
-00001430: 746f 2074 6f67 676c 6520 636c 6173 7320  to toggle class 
-00001440: 666f 7220 656c 656d 656e 740a 6675 6e63  for element.func
-00001450: 7469 6f6e 2074 6f67 676c 655f 636c 6173  tion toggle_clas
-00001460: 7328 656c 656d 2c20 636c 6173 735f 6e61  s(elem, class_na
-00001470: 6d65 2920 7b0a 2020 2020 6966 2028 656c  me) {.    if (el
-00001480: 656d 2e63 6c61 7373 4c69 7374 2e63 6f6e  em.classList.con
-00001490: 7461 696e 7328 636c 6173 735f 6e61 6d65  tains(class_name
-000014a0: 2929 207b 0a20 2020 2020 2020 2065 6c65  )) {.        ele
-000014b0: 6d2e 636c 6173 734c 6973 742e 7265 6d6f  m.classList.remo
-000014c0: 7665 2863 6c61 7373 5f6e 616d 6529 3b0a  ve(class_name);.
-000014d0: 2020 2020 7d0a 2020 2020 656c 7365 207b      }.    else {
-000014e0: 0a20 2020 2020 2020 2065 6c65 6d2e 636c  .        elem.cl
-000014f0: 6173 734c 6973 742e 6164 6428 636c 6173  assList.add(clas
-00001500: 735f 6e61 6d65 290a 2020 2020 7d0a 7d0a  s_name).    }.}.
-00001510: 0a0a 6675 6e63 7469 6f6e 2074 6f67 676c  ..function toggl
-00001520: 655f 636f 6e74 7261 7374 5f66 6f72 2874  e_contrast_for(t
-00001530: 6172 6765 745f 636c 6173 7329 207b 0a20  arget_class) {. 
-00001540: 2020 2076 6172 2065 6c65 6d65 6e74 7320     var elements 
-00001550: 3d20 646f 6375 6d65 6e74 2e67 6574 456c  = document.getEl
-00001560: 656d 656e 7473 4279 436c 6173 734e 616d  ementsByClassNam
-00001570: 6528 7461 7267 6574 5f63 6c61 7373 293b  e(target_class);
-00001580: 0a20 2020 2066 6f72 2028 7661 7220 6920  .    for (var i 
-00001590: 3d20 303b 2069 203c 2065 6c65 6d65 6e74  = 0; i < element
-000015a0: 732e 6c65 6e67 7468 3b20 692b 2b29 207b  s.length; i++) {
-000015b0: 0a20 2020 2020 2020 2074 6f67 676c 655f  .        toggle_
-000015c0: 636c 6173 7328 656c 656d 656e 7473 5b69  class(elements[i
-000015d0: 5d2c 2022 636f 6e74 7261 7374 2229 3b0a  ], "contrast");.
-000015e0: 2020 2020 7d0a 7d3b 0a0a 6675 6e63 7469      }.};..functi
-000015f0: 6f6e 2074 6f67 676c 655f 636f 6e74 7261  on toggle_contra
-00001600: 7374 2829 207b 0a20 2020 2076 6172 2073  st() {.    var s
-00001610: 7465 705f 7374 6174 7573 5f69 7465 6d73  tep_status_items
-00001620: 203d 2064 6f63 756d 656e 742e 6765 7445   = document.getE
-00001630: 6c65 6d65 6e74 7342 7943 6c61 7373 4e61  lementsByClassNa
-00001640: 6d65 2822 7374 6570 2d73 7461 7475 7322  me("step-status"
-00001650: 293b 0a20 2020 2066 6f72 2028 7661 7220  );.    for (var 
-00001660: 6920 3d20 303b 2069 203c 2073 7465 705f  i = 0; i < step_
-00001670: 7374 6174 7573 5f69 7465 6d73 2e6c 656e  status_items.len
-00001680: 6774 683b 2069 2b2b 2920 7b0a 2020 2020  gth; i++) {.    
-00001690: 2020 2020 7374 6570 5f73 7461 7475 735f      step_status_
-000016a0: 6974 656d 735b 695d 2e73 7479 6c65 2e64  items[i].style.d
-000016b0: 6973 706c 6179 203d 2028 7374 6570 5f73  isplay = (step_s
-000016c0: 7461 7475 735f 6974 656d 735b 695d 2e73  tatus_items[i].s
-000016d0: 7479 6c65 2e64 6973 706c 6179 203d 3d20  tyle.display == 
-000016e0: 2262 6c6f 636b 2220 3f20 226e 6f6e 6522  "block" ? "none"
-000016f0: 203a 2022 626c 6f63 6b22 293b 0a20 2020   : "block");.   
-00001700: 207d 3b0a 0a20 2020 2063 6f6e 7374 2063   };..    const c
-00001710: 6f6e 7472 6173 745f 636c 6173 7365 7320  ontrast_classes 
-00001720: 3d20 5b0a 2020 2020 2020 2020 2266 6561  = [.        "fea
-00001730: 7475 7265 2d74 6974 6c65 222c 0a20 2020  ture-title",.   
-00001740: 2020 2020 2022 6665 6174 7572 652d 7375       "feature-su
-00001750: 6d6d 6172 792d 636f 6d6d 656e 7461 7279  mmary-commentary
-00001760: 222c 0a20 2020 2020 2020 2022 6665 6174  ",.        "feat
-00001770: 7572 652d 7375 6d6d 6172 792d 636f 6e74  ure-summary-cont
-00001780: 6169 6e65 7222 2c0a 2020 2020 2020 2020  ainer",.        
-00001790: 2266 6561 7475 7265 2d73 756d 6d61 7279  "feature-summary
-000017a0: 2d72 6f77 222c 0a20 2020 2020 2020 2022  -row",.        "
-000017b0: 6665 6174 7572 652d 6963 6f6e 222c 0a0a  feature-icon",..
-000017c0: 2020 2020 2020 2020 2273 6365 6e61 7269          "scenari
-000017d0: 6f2d 6865 6164 6572 222c 0a20 2020 2020  o-header",.     
-000017e0: 2020 2022 7363 656e 6172 696f 2d63 6170     "scenario-cap
-000017f0: 7375 6c65 222c 0a20 2020 2020 2020 2022  sule",.        "
-00001800: 7363 656e 6172 696f 2d74 6167 7322 2c0a  scenario-tags",.
-00001810: 2020 2020 2020 2020 2273 6365 6e61 7269          "scenari
-00001820: 6f2d 6475 7261 7469 6f6e 222c 0a0a 2020  o-duration",..  
-00001830: 2020 2020 2020 2273 7465 702d 6361 7073        "step-caps
-00001840: 756c 6522 2c0a 2020 2020 2020 2020 2273  ule",.        "s
-00001850: 7465 702d 7374 6174 7573 222c 0a20 2020  tep-status",.   
-00001860: 2020 2020 2022 7374 6570 2d64 7572 6174       "step-durat
-00001870: 696f 6e22 2c0a 0a20 2020 2020 2020 2022  ion",..        "
-00001880: 6d65 7373 6167 6573 222c 0a20 2020 2020  messages",.     
-00001890: 2020 2022 656d 6265 645f 6275 7474 6f6e     "embed_button
-000018a0: 222c 0a20 2020 2020 2020 2022 6c69 6e6b  ",.        "link
-000018b0: 222c 0a20 2020 2020 2020 2022 7461 626c  ",.        "tabl
-000018c0: 6522 2c0a 0a20 2020 205d 3b0a 2020 2020  e",..    ];.    
-000018d0: 636f 6e74 7261 7374 5f63 6c61 7373 6573  contrast_classes
-000018e0: 2e66 6f72 4561 6368 2874 6f67 676c 655f  .forEach(toggle_
-000018f0: 636f 6e74 7261 7374 5f66 6f72 293b 0a7d  contrast_for);.}
-00001900: 3b0a 0a66 756e 6374 696f 6e20 6465 7465  ;..function dete
-00001910: 6374 5f63 6f6e 7472 6173 7428 2920 7b0a  ct_contrast() {.
-00001920: 2020 2020 7661 7220 6f62 6a5f 6469 7620      var obj_div 
-00001930: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
-00001940: 6545 6c65 6d65 6e74 2822 6469 7622 293b  eElement("div");
-00001950: 0a20 2020 206f 626a 5f64 6976 2e73 7479  .    obj_div.sty
-00001960: 6c65 2e63 6f6c 6f72 203d 2022 7267 6228  le.color = "rgb(
-00001970: 3331 2c20 3431 2c20 3539 2922 0a20 2020  31, 41, 59)".   
-00001980: 2064 6f63 756d 656e 742e 626f 6479 2e61   document.body.a
-00001990: 7070 656e 6443 6869 6c64 286f 626a 5f64  ppendChild(obj_d
-000019a0: 6976 293b 0a20 2020 2076 6172 2063 6f6c  iv);.    var col
-000019b0: 203d 2064 6f63 756d 656e 742e 6465 6661   = document.defa
-000019c0: 756c 7456 6965 7720 3f20 646f 6375 6d65  ultView ? docume
-000019d0: 6e74 2e64 6566 6175 6c74 5669 6577 2e67  nt.defaultView.g
-000019e0: 6574 436f 6d70 7574 6564 5374 796c 6528  etComputedStyle(
-000019f0: 6f62 6a5f 6469 762c 206e 756c 6c29 2e63  obj_div, null).c
-00001a00: 6f6c 6f72 203a 206f 626a 5f64 6976 2e63  olor : obj_div.c
-00001a10: 7572 7265 6e74 5374 796c 652e 636f 6c6f  urrentStyle.colo
-00001a20: 723b 0a20 2020 2064 6f63 756d 656e 742e  r;.    document.
-00001a30: 626f 6479 2e72 656d 6f76 6543 6869 6c64  body.removeChild
-00001a40: 286f 626a 5f64 6976 293b 0a20 2020 2063  (obj_div);.    c
-00001a50: 6f6c 203d 2063 6f6c 2e72 6570 6c61 6365  ol = col.replace
-00001a60: 282f 202f 672c 2022 2229 3b0a 2020 2020  (/ /g, "");.    
-00001a70: 6966 2028 636f 6c20 213d 3d20 2272 6762  if (col !== "rgb
-00001a80: 2833 312c 3431 2c35 3929 2229 207b 0a20  (31,41,59)") {. 
-00001a90: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
-00001aa0: 6f67 2822 4869 6768 2043 6f6e 7472 6173  og("High Contras
-00001ab0: 7420 7468 656d 6520 6465 7465 6374 6564  t theme detected
-00001ac0: 2e22 290a 2020 2020 2020 2020 746f 6767  .").        togg
-00001ad0: 6c65 5f63 6f6e 7472 6173 7428 293b 0a20  le_contrast();. 
-00001ae0: 2020 207d 0a7d 0a0a 7661 7220 656c 656d     }.}..var elem
-00001af0: 656e 7420 3d20 646f 6375 6d65 6e74 2e63  ent = document.c
-00001b00: 7265 6174 6545 6c65 6d65 6e74 2827 6469  reateElement('di
-00001b10: 7627 293b 0a76 6172 2065 6e74 6974 7920  v');.var entity 
-00001b20: 3d20 2f26 283f 3a23 785b 612d 6630 2d39  = /&(?:#x[a-f0-9
-00001b30: 5d2b 7c23 5b30 2d39 5d2b 7c5b 612d 7a30  ]+|#[0-9]+|[a-z0
-00001b40: 2d39 5d2b 293b 3f2f 6967 3b0a 0a66 756e  -9]+);?/ig;..fun
-00001b50: 6374 696f 6e20 6465 636f 6465 4854 4d4c  ction decodeHTML
-00001b60: 456e 7469 7469 6573 2873 7472 2920 7b0a  Entities(str) {.
-00001b70: 2020 2020 7374 7220 3d20 7374 722e 7265      str = str.re
-00001b80: 706c 6163 6528 656e 7469 7479 2c20 6675  place(entity, fu
-00001b90: 6e63 7469 6f6e 2028 6d29 207b 0a20 2020  nction (m) {.   
-00001ba0: 2020 2020 2065 6c65 6d65 6e74 2e69 6e6e       element.inn
-00001bb0: 6572 4854 4d4c 203d 206d 3b0a 2020 2020  erHTML = m;.    
-00001bc0: 2020 2020 7265 7475 726e 2065 6c65 6d65      return eleme
-00001bd0: 6e74 2e74 6578 7443 6f6e 7465 6e74 3b0a  nt.textContent;.
-00001be0: 2020 2020 7d29 3b0a 2020 2020 656c 656d      });.    elem
-00001bf0: 656e 742e 7465 7874 436f 6e74 656e 7420  ent.textContent 
-00001c00: 3d20 2727 3b0a 2020 2020 7265 7475 726e  = '';.    return
-00001c10: 2073 7472 3b0a 7d0a 0a66 756e 6374 696f   str;.}..functio
-00001c20: 6e20 646f 776e 6c6f 6164 5f65 6d62 6564  n download_embed
-00001c30: 2869 642c 2066 696c 656e 616d 6529 207b  (id, filename) {
-00001c40: 0a20 2020 2076 6172 2065 6c65 6d20 3d20  .    var elem = 
-00001c50: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
-00001c60: 656e 7442 7949 6428 6964 293b 0a20 2020  entById(id);.   
-00001c70: 2076 6172 2063 6869 6c64 203d 2065 6c65   var child = ele
-00001c80: 6d2e 6368 696c 6472 656e 5b31 5d3b 0a20  m.children[1];. 
-00001c90: 2020 2076 6172 2076 616c 7565 203d 2022     var value = "
-00001ca0: 223b 0a20 2020 2076 6172 2074 6167 203d  ";.    var tag =
-00001cb0: 2063 6869 6c64 2e74 6167 4e61 6d65 2e74   child.tagName.t
-00001cc0: 6f4c 6f77 6572 4361 7365 2829 3b0a 2020  oLowerCase();.  
-00001cd0: 2020 6966 2028 7461 6720 3d3d 3d20 2273    if (tag === "s
-00001ce0: 7061 6e22 2920 7b0a 2020 2020 2020 2020  pan") {.        
-00001cf0: 6669 6c65 6e61 6d65 202b 3d20 222e 7478  filename += ".tx
-00001d00: 7422 3b0a 2020 2020 2020 2020 7661 6c75  t";.        valu
-00001d10: 6520 3d20 2264 6174 613a 7465 7874 2f70  e = "data:text/p
-00001d20: 6c61 696e 2c22 202b 2065 6e63 6f64 6555  lain," + encodeU
-00001d30: 5249 436f 6d70 6f6e 656e 7428 6465 636f  RIComponent(deco
-00001d40: 6465 4854 4d4c 456e 7469 7469 6573 2863  deHTMLEntities(c
-00001d50: 6869 6c64 2e69 6e6e 6572 4854 4d4c 2929  hild.innerHTML))
-00001d60: 3b0a 2020 2020 7d20 656c 7365 2069 6620  ;.    } else if 
-00001d70: 2874 6167 203d 3d20 2276 6964 656f 2229  (tag == "video")
-00001d80: 207b 0a20 2020 2020 2020 2066 696c 656e   {.        filen
-00001d90: 616d 6520 2b3d 2022 2e77 6562 6d22 3b0a  ame += ".webm";.
-00001da0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00001db0: 6368 696c 642e 6368 696c 6472 656e 5b30  child.children[0
-00001dc0: 5d2e 7372 633b 0a20 2020 207d 2065 6c73  ].src;.    } els
-00001dd0: 6520 6966 2028 7461 6720 3d3d 2022 696d  e if (tag == "im
-00001de0: 6722 2920 7b0a 2020 2020 2020 2020 6669  g") {.        fi
-00001df0: 6c65 6e61 6d65 202b 3d20 222e 706e 6722  lename += ".png"
-00001e00: 3b0a 2020 2020 2020 2020 7661 6c75 6520  ;.        value 
-00001e10: 3d20 6368 696c 642e 7372 633b 0a20 2020  = child.src;.   
-00001e20: 207d 2065 6c73 6520 7b0a 2020 2020 2020   } else {.      
-00001e30: 2020 6669 6c65 6e61 6d65 202b 3d20 222e    filename += ".
-00001e40: 6874 6d6c 223b 0a20 2020 2020 2020 2076  html";.        v
-00001e50: 616c 7565 203d 2064 6563 6f64 6548 544d  alue = decodeHTM
-00001e60: 4c45 6e74 6974 6965 7328 6368 696c 642e  LEntities(child.
-00001e70: 696e 6e65 7248 544d 4c29 3b0a 2020 2020  innerHTML);.    
-00001e80: 7d0a 2020 2020 7661 7220 6c69 6e6b 203d  }.    var link =
-00001e90: 2064 6f63 756d 656e 742e 6372 6561 7465   document.create
-00001ea0: 456c 656d 656e 7428 2261 2229 3b0a 2020  Element("a");.  
-00001eb0: 2020 6c69 6e6b 2e73 7479 6c65 2e64 6973    link.style.dis
-00001ec0: 706c 6179 203d 2022 6e6f 6e65 223b 0a20  play = "none";. 
-00001ed0: 2020 206c 696e 6b2e 6872 6566 203d 2076     link.href = v
-00001ee0: 616c 7565 3b0a 2020 2020 6c69 6e6b 2e64  alue;.    link.d
-00001ef0: 6f77 6e6c 6f61 6420 3d20 6669 6c65 6e61  ownload = filena
-00001f00: 6d65 3b0a 2020 2020 646f 6375 6d65 6e74  me;.    document
-00001f10: 2e62 6f64 792e 6170 7065 6e64 4368 696c  .body.appendChil
-00001f20: 6428 6c69 6e6b 293b 0a20 2020 206c 696e  d(link);.    lin
-00001f30: 6b2e 636c 6963 6b28 290a 2020 2020 2f2a  k.click().    /*
-00001f40: 2066 6978 2072 6163 6520 696e 2046 4620   fix race in FF 
-00001f50: 2a2f 0a20 2020 2073 6574 5469 6d65 6f75  */.    setTimeou
-00001f60: 7428 6675 6e63 7469 6f6e 2028 2920 7b20  t(function () { 
-00001f70: 646f 6375 6d65 6e74 2e62 6f64 792e 7265  document.body.re
-00001f80: 6d6f 7665 4368 696c 6428 6c69 6e6b 293b  moveChild(link);
-00001f90: 207d 2c20 3230 3030 293b 0a7d 3b          }, 2000);.};
+000009f0: 3b0a 2020 2020 7d20 656c 7365 207b 0a20  ;.    } else {. 
+00000a00: 2020 2020 2020 2068 6173 685f 7575 6964         hash_uuid
+00000a10: 5f6c 6973 742e 7075 7368 2869 6429 3b0a  _list.push(id);.
+00000a20: 2020 2020 7d0a 2020 2020 2f2f 2055 7064      }.    // Upd
+00000a30: 6174 6520 5552 4c20 6861 7368 0a20 2020  ate URL hash.   
+00000a40: 2076 6172 2068 6173 6820 3d20 2223 223b   var hash = "#";
+00000a50: 0a20 2020 2069 6620 2868 6173 685f 7575  .    if (hash_uu
+00000a60: 6964 5f6c 6973 742e 6c65 6e67 7468 2021  id_list.length !
+00000a70: 3d20 3029 207b 0a20 2020 2020 2020 2068  = 0) {.        h
+00000a80: 6173 6820 3d20 746f 6767 6c65 5f6e 6f6e  ash = toggle_non
+00000a90: 5f65 6d70 7479 5f73 7472 696e 6720 2b20  _empty_string + 
+00000aa0: 6861 7368 5f75 7569 645f 6c69 7374 2e74  hash_uuid_list.t
+00000ab0: 6f53 7472 696e 6728 290a 2020 2020 7d0a  oString().    }.
+00000ac0: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00000ad0: 224e 6577 2068 6173 683a 2022 202b 2068  "New hash: " + h
+00000ae0: 6173 6829 3b0a 2020 2020 6869 7374 6f72  ash);.    histor
+00000af0: 792e 7265 706c 6163 6553 7461 7465 2875  y.replaceState(u
+00000b00: 6e64 6566 696e 6564 2c20 756e 6465 6669  ndefined, undefi
+00000b10: 6e65 642c 2068 6173 6829 3b0a 2020 2020  ned, hash);.    
+00000b20: 2f2f 204e 6565 6420 746f 2063 616c 6c20  // Need to call 
+00000b30: 6861 7368 5f74 6f5f 7374 6174 652c 2065  hash_to_state, e
+00000b40: 7665 6e74 2069 7320 6e6f 7420 7472 6967  vent is not trig
+00000b50: 6765 7265 6420 666f 7220 736f 6d65 2072  gered for some r
+00000b60: 6561 736f 6e0a 2020 2020 6861 7368 5f74  eason.    hash_t
+00000b70: 6f5f 7374 6174 6528 293b 0a7d 0a0a 6675  o_state();.}..fu
+00000b80: 6e63 7469 6f6e 2063 6f6c 6c61 7073 6962  nction collapsib
+00000b90: 6c65 5f74 6f67 676c 6528 6964 2920 7b0a  le_toggle(id) {.
+00000ba0: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00000bb0: 2254 6f67 676c 6520 656d 6265 643a 2022  "Toggle embed: "
+00000bc0: 202b 2069 6429 3b0a 2020 2020 7661 7220   + id);.    var 
+00000bd0: 656d 6265 645f 6275 7474 6f6e 5f69 6420  embed_button_id 
+00000be0: 3d20 2265 6d62 6564 5f62 7574 746f 6e5f  = "embed_button_
+00000bf0: 2220 2b20 6964 0a20 2020 2076 6172 2070  " + id.    var p
+00000c00: 6172 656e 7420 3d20 646f 6375 6d65 6e74  arent = document
+00000c10: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
+00000c20: 656d 6265 645f 6275 7474 6f6e 5f69 6429  embed_button_id)
+00000c30: 3b0a 2020 2020 6966 2028 7061 7265 6e74  ;.    if (parent
+00000c40: 203d 3d3d 206e 756c 6c29 207b 0a20 2020   === null) {.   
+00000c50: 2020 2020 2072 6574 7572 6e3b 0a20 2020       return;.   
+00000c60: 207d 0a20 2020 2077 6869 6c65 2028 7061   }.    while (pa
+00000c70: 7265 6e74 2021 3d3d 2075 6e64 6566 696e  rent !== undefin
+00000c80: 6564 2026 2620 2170 6172 656e 742e 636c  ed && !parent.cl
+00000c90: 6173 734c 6973 742e 636f 6e74 6169 6e73  assList.contains
+00000ca0: 2822 656d 6265 645f 6275 7474 6f6e 2229  ("embed_button")
+00000cb0: 2920 7b0a 2020 2020 2020 2020 7061 7265  ) {.        pare
+00000cc0: 6e74 203d 2070 6172 656e 742e 7061 7265  nt = parent.pare
+00000cd0: 6e74 456c 656d 656e 743b 0a20 2020 207d  ntElement;.    }
+00000ce0: 0a20 2020 2069 6620 2870 6172 656e 7420  .    if (parent 
+00000cf0: 213d 3d20 756e 6465 6669 6e65 6429 207b  !== undefined) {
+00000d00: 0a20 2020 2020 2020 2074 6f67 676c 655f  .        toggle_
+00000d10: 636c 6173 7328 7061 7265 6e74 2c20 2263  class(parent, "c
+00000d20: 6f6c 6c61 7073 6522 293b 0a20 2020 207d  ollapse");.    }
+00000d30: 0a0a 2020 2020 7661 7220 656d 6265 645f  ..    var embed_
+00000d40: 636f 6e74 656e 745f 6964 203d 2022 656d  content_id = "em
+00000d50: 6265 645f 2220 2b20 6964 0a20 2020 2076  bed_" + id.    v
+00000d60: 6172 2065 6c65 6d20 3d20 646f 6375 6d65  ar elem = docume
+00000d70: 6e74 2e67 6574 456c 656d 656e 7442 7949  nt.getElementByI
+00000d80: 6428 656d 6265 645f 636f 6e74 656e 745f  d(embed_content_
+00000d90: 6964 293b 0a20 2020 2074 6f67 676c 655f  id);.    toggle_
+00000da0: 636c 6173 7328 656c 656d 2c20 2263 6f6c  class(elem, "col
+00000db0: 6c61 7073 6522 293b 0a7d 3b0a 0a66 756e  lapse");.};..fun
+00000dc0: 6374 696f 6e20 636f 6c6c 6170 7369 626c  ction collapsibl
+00000dd0: 655f 7375 6d6d 6172 7928 636c 6173 736e  e_summary(classn
+00000de0: 616d 6529 207b 0a20 2020 2076 6172 2065  ame) {.    var e
+00000df0: 6c65 6d20 3d20 646f 6375 6d65 6e74 2e67  lem = document.g
+00000e00: 6574 456c 656d 656e 7473 4279 436c 6173  etElementsByClas
+00000e10: 734e 616d 6528 636c 6173 736e 616d 6529  sName(classname)
+00000e20: 3b0a 2020 2020 666f 7220 2876 6172 2069  ;.    for (var i
+00000e30: 203d 2030 3b20 6920 3c20 656c 656d 2e6c   = 0; i < elem.l
+00000e40: 656e 6774 683b 2069 2b2b 2920 7b0a 2020  ength; i++) {.  
+00000e50: 2020 2020 2020 746f 6767 6c65 5f63 6c61        toggle_cla
+00000e60: 7373 2865 6c65 6d5b 695d 2c20 2263 6f6c  ss(elem[i], "col
+00000e70: 6c61 7073 6522 293b 0a20 2020 207d 0a7d  lapse");.    }.}
+00000e80: 3b0a 0a66 756e 6374 696f 6e20 6578 7061  ;..function expa
+00000e90: 6e64 6572 2861 6374 696f 6e2c 2073 756d  nder(action, sum
+00000ea0: 6d61 7279 5f62 6c6f 636b 2920 7b0a 2020  mary_block) {.  
+00000eb0: 2020 7661 7220 656c 656d 203d 2041 7272    var elem = Arr
+00000ec0: 6179 2e66 726f 6d28 646f 6375 6d65 6e74  ay.from(document
+00000ed0: 2e67 6574 456c 656d 656e 7473 4279 436c  .getElementsByCl
+00000ee0: 6173 734e 616d 6528 2273 6365 6e61 7269  assName("scenari
+00000ef0: 6f2d 6361 7073 756c 6522 2929 3b0a 2020  o-capsule"));.  
+00000f00: 2020 656c 656d 203d 2065 6c65 6d2e 636f    elem = elem.co
+00000f10: 6e63 6174 2841 7272 6179 2e66 726f 6d28  ncat(Array.from(
+00000f20: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
+00000f30: 656e 7473 4279 436c 6173 734e 616d 6528  entsByClassName(
+00000f40: 2273 6365 6e61 7269 6f2d 6865 6164 6572  "scenario-header
+00000f50: 2229 2929 3b0a 2020 2020 7661 7220 6665  ")));.    var fe
+00000f60: 6174 7572 655f 6964 203d 2073 756d 6d61  ature_id = summa
+00000f70: 7279 5f62 6c6f 636b 2e70 6172 656e 7445  ry_block.parentE
+00000f80: 6c65 6d65 6e74 2e70 6172 656e 7445 6c65  lement.parentEle
+00000f90: 6d65 6e74 2e69 640a 2020 2020 666f 7220  ment.id.    for 
+00000fa0: 2876 6172 2069 203d 2030 3b20 6920 3c20  (var i = 0; i < 
+00000fb0: 656c 656d 2e6c 656e 6774 683b 2069 2b2b  elem.length; i++
+00000fc0: 2920 7b0a 2020 2020 2020 2020 6966 2028  ) {.        if (
+00000fd0: 6665 6174 7572 655f 6964 2021 3d20 656c  feature_id != el
+00000fe0: 656d 5b69 5d2e 7061 7265 6e74 456c 656d  em[i].parentElem
+00000ff0: 656e 742e 6964 2920 7b0a 2020 2020 2020  ent.id) {.      
+00001000: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00001010: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001020: 2069 6620 2861 6374 696f 6e20 3d3d 2022   if (action == "
+00001030: 6578 7061 6e64 5f61 6c6c 2229 207b 0a20  expand_all") {. 
+00001040: 2020 2020 2020 2020 2020 2065 6c65 6d5b             elem[
+00001050: 695d 2e63 6c61 7373 4c69 7374 2e72 656d  i].classList.rem
+00001060: 6f76 6528 2263 6f6c 6c61 7073 6522 290a  ove("collapse").
+00001070: 2020 2020 2020 2020 7d20 656c 7365 2069          } else i
+00001080: 6620 2861 6374 696f 6e20 3d3d 2022 636f  f (action == "co
+00001090: 6c6c 6170 7365 5f61 6c6c 2229 207b 0a20  llapse_all") {. 
+000010a0: 2020 2020 2020 2020 2020 2069 6620 2821             if (!
+000010b0: 656c 656d 5b69 5d2e 636c 6173 734c 6973  elem[i].classLis
+000010c0: 742e 636f 6e74 6169 6e73 2822 636f 6c6c  t.contains("coll
+000010d0: 6170 7365 2229 2920 7b0a 2020 2020 2020  apse")) {.      
+000010e0: 2020 2020 2020 2020 2020 656c 656d 5b69            elem[i
+000010f0: 5d2e 636c 6173 734c 6973 742e 6164 6428  ].classList.add(
+00001100: 2263 6f6c 6c61 7073 6522 293b 0a20 2020  "collapse");.   
+00001110: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001120: 2020 207d 2065 6c73 6520 6966 2028 6163     } else if (ac
+00001130: 7469 6f6e 203d 3d20 2265 7870 616e 645f  tion == "expand_
+00001140: 616c 6c5f 6661 696c 6564 2229 207b 0a20  all_failed") {. 
+00001150: 2020 2020 2020 2020 2020 2069 6620 2821             if (!
+00001160: 656c 656d 5b69 5d2e 636c 6173 734c 6973  elem[i].classLis
+00001170: 742e 636f 6e74 6169 6e73 2822 7061 7373  t.contains("pass
+00001180: 6564 2229 2920 7b0a 2020 2020 2020 2020  ed")) {.        
+00001190: 2020 2020 2020 2020 656c 656d 5b69 5d2e          elem[i].
+000011a0: 636c 6173 734c 6973 742e 7265 6d6f 7665  classList.remove
+000011b0: 2822 636f 6c6c 6170 7365 2229 3b0a 2020  ("collapse");.  
+000011c0: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
+000011d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000011e0: 2020 2069 6620 2821 656c 656d 5b69 5d2e     if (!elem[i].
+000011f0: 636c 6173 734c 6973 742e 636f 6e74 6169  classList.contai
+00001200: 6e73 2822 636f 6c6c 6170 7365 2229 2920  ns("collapse")) 
+00001210: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001220: 2020 2020 2020 656c 656d 5b69 5d2e 636c        elem[i].cl
+00001230: 6173 734c 6973 742e 6164 6428 2263 6f6c  assList.add("col
+00001240: 6c61 7073 6522 293b 0a20 2020 2020 2020  lapse");.       
+00001250: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001260: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001270: 207d 0a20 2020 207d 0a7d 3b0a 0a0a 6675   }.    }.};...fu
+00001280: 6e63 7469 6f6e 2065 7870 616e 645f 7468  nction expand_th
+00001290: 6973 5f6f 6e6c 7928 6e61 6d65 2920 7b0a  is_only(name) {.
+000012a0: 2020 2020 7661 7220 6964 203d 206e 616d      var id = nam
+000012b0: 652e 6964 3b0a 2020 2020 7661 7220 6361  e.id;.    var ca
+000012c0: 7073 756c 6520 3d20 646f 6375 6d65 6e74  psule = document
+000012d0: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
+000012e0: 6964 202b 2022 2d63 2229 3b0a 2020 2020  id + "-c");.    
+000012f0: 7661 7220 6865 6164 6572 203d 2064 6f63  var header = doc
+00001300: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
+00001310: 4279 4964 2869 6420 2b20 222d 6822 293b  ById(id + "-h");
+00001320: 0a20 2020 2069 6620 2868 6561 6465 722e  .    if (header.
+00001330: 636c 6173 734c 6973 742e 636f 6e74 6169  classList.contai
+00001340: 6e73 2822 636f 6c6c 6170 7365 2229 2920  ns("collapse")) 
+00001350: 7b0a 2020 2020 2020 2020 6865 6164 6572  {.        header
+00001360: 2e63 6c61 7373 4c69 7374 2e72 656d 6f76  .classList.remov
+00001370: 6528 2263 6f6c 6c61 7073 6522 293b 0a20  e("collapse");. 
+00001380: 2020 2020 2020 2063 6170 7375 6c65 2e63         capsule.c
+00001390: 6c61 7373 4c69 7374 2e72 656d 6f76 6528  lassList.remove(
+000013a0: 2263 6f6c 6c61 7073 6522 293b 0a20 2020  "collapse");.   
+000013b0: 207d 2065 6c73 6520 7b0a 2020 2020 2020   } else {.      
+000013c0: 2020 6865 6164 6572 2e63 6c61 7373 4c69    header.classLi
+000013d0: 7374 2e61 6464 2822 636f 6c6c 6170 7365  st.add("collapse
+000013e0: 2229 3b0a 2020 2020 2020 2020 6361 7073  ");.        caps
+000013f0: 756c 652e 636c 6173 734c 6973 742e 6164  ule.classList.ad
+00001400: 6428 2263 6f6c 6c61 7073 6522 293b 0a20  d("collapse");. 
+00001410: 2020 207d 0a7d 3b0a 0a2f 2f20 4865 6c70     }.};..// Help
+00001420: 6572 2066 756e 6374 696f 6e20 746f 2074  er function to t
+00001430: 6f67 676c 6520 636c 6173 7320 666f 7220  oggle class for 
+00001440: 656c 656d 656e 740a 6675 6e63 7469 6f6e  element.function
+00001450: 2074 6f67 676c 655f 636c 6173 7328 656c   toggle_class(el
+00001460: 656d 2c20 636c 6173 735f 6e61 6d65 2920  em, class_name) 
+00001470: 7b0a 2020 2020 6966 2028 656c 656d 2e63  {.    if (elem.c
+00001480: 6c61 7373 4c69 7374 2e63 6f6e 7461 696e  lassList.contain
+00001490: 7328 636c 6173 735f 6e61 6d65 2929 207b  s(class_name)) {
+000014a0: 0a20 2020 2020 2020 2065 6c65 6d2e 636c  .        elem.cl
+000014b0: 6173 734c 6973 742e 7265 6d6f 7665 2863  assList.remove(c
+000014c0: 6c61 7373 5f6e 616d 6529 3b0a 2020 2020  lass_name);.    
+000014d0: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
+000014e0: 2065 6c65 6d2e 636c 6173 734c 6973 742e   elem.classList.
+000014f0: 6164 6428 636c 6173 735f 6e61 6d65 290a  add(class_name).
+00001500: 2020 2020 7d0a 7d0a 0a0a 6675 6e63 7469      }.}...functi
+00001510: 6f6e 2074 6f67 676c 655f 636f 6e74 7261  on toggle_contra
+00001520: 7374 5f66 6f72 2874 6172 6765 745f 636c  st_for(target_cl
+00001530: 6173 7329 207b 0a20 2020 2076 6172 2065  ass) {.    var e
+00001540: 6c65 6d65 6e74 7320 3d20 646f 6375 6d65  lements = docume
+00001550: 6e74 2e67 6574 456c 656d 656e 7473 4279  nt.getElementsBy
+00001560: 436c 6173 734e 616d 6528 7461 7267 6574  ClassName(target
+00001570: 5f63 6c61 7373 293b 0a20 2020 2066 6f72  _class);.    for
+00001580: 2028 7661 7220 6920 3d20 303b 2069 203c   (var i = 0; i <
+00001590: 2065 6c65 6d65 6e74 732e 6c65 6e67 7468   elements.length
+000015a0: 3b20 692b 2b29 207b 0a20 2020 2020 2020  ; i++) {.       
+000015b0: 2074 6f67 676c 655f 636c 6173 7328 656c   toggle_class(el
+000015c0: 656d 656e 7473 5b69 5d2c 2022 636f 6e74  ements[i], "cont
+000015d0: 7261 7374 2229 3b0a 2020 2020 7d0a 7d3b  rast");.    }.};
+000015e0: 0a0a 6675 6e63 7469 6f6e 2074 6f67 676c  ..function toggl
+000015f0: 655f 636f 6e74 7261 7374 2829 207b 0a20  e_contrast() {. 
+00001600: 2020 2076 6172 2073 7465 705f 7374 6174     var step_stat
+00001610: 7573 5f69 7465 6d73 203d 2064 6f63 756d  us_items = docum
+00001620: 656e 742e 6765 7445 6c65 6d65 6e74 7342  ent.getElementsB
+00001630: 7943 6c61 7373 4e61 6d65 2822 7374 6570  yClassName("step
+00001640: 2d73 7461 7475 7322 293b 0a20 2020 2066  -status");.    f
+00001650: 6f72 2028 7661 7220 6920 3d20 303b 2069  or (var i = 0; i
+00001660: 203c 2073 7465 705f 7374 6174 7573 5f69   < step_status_i
+00001670: 7465 6d73 2e6c 656e 6774 683b 2069 2b2b  tems.length; i++
+00001680: 2920 7b0a 2020 2020 2020 2020 7374 6570  ) {.        step
+00001690: 5f73 7461 7475 735f 6974 656d 735b 695d  _status_items[i]
+000016a0: 2e73 7479 6c65 2e64 6973 706c 6179 203d  .style.display =
+000016b0: 2028 7374 6570 5f73 7461 7475 735f 6974   (step_status_it
+000016c0: 656d 735b 695d 2e73 7479 6c65 2e64 6973  ems[i].style.dis
+000016d0: 706c 6179 203d 3d20 2262 6c6f 636b 2220  play == "block" 
+000016e0: 3f20 226e 6f6e 6522 203a 2022 626c 6f63  ? "none" : "bloc
+000016f0: 6b22 293b 0a20 2020 207d 3b0a 0a20 2020  k");.    };..   
+00001700: 2063 6f6e 7374 2063 6f6e 7472 6173 745f   const contrast_
+00001710: 636c 6173 7365 7320 3d20 5b0a 2020 2020  classes = [.    
+00001720: 2020 2020 2266 6561 7475 7265 2d74 6974      "feature-tit
+00001730: 6c65 222c 0a20 2020 2020 2020 2022 6665  le",.        "fe
+00001740: 6174 7572 652d 7375 6d6d 6172 792d 636f  ature-summary-co
+00001750: 6d6d 656e 7461 7279 222c 0a20 2020 2020  mmentary",.     
+00001760: 2020 2022 6665 6174 7572 652d 7375 6d6d     "feature-summ
+00001770: 6172 792d 636f 6e74 6169 6e65 7222 2c0a  ary-container",.
+00001780: 2020 2020 2020 2020 2266 6561 7475 7265          "feature
+00001790: 2d73 756d 6d61 7279 2d72 6f77 222c 0a20  -summary-row",. 
+000017a0: 2020 2020 2020 2022 6665 6174 7572 652d         "feature-
+000017b0: 6963 6f6e 222c 0a0a 2020 2020 2020 2020  icon",..        
+000017c0: 2273 6365 6e61 7269 6f2d 6865 6164 6572  "scenario-header
+000017d0: 222c 0a20 2020 2020 2020 2022 7363 656e  ",.        "scen
+000017e0: 6172 696f 2d63 6170 7375 6c65 222c 0a20  ario-capsule",. 
+000017f0: 2020 2020 2020 2022 7363 656e 6172 696f         "scenario
+00001800: 2d74 6167 7322 2c0a 2020 2020 2020 2020  -tags",.        
+00001810: 2273 6365 6e61 7269 6f2d 6475 7261 7469  "scenario-durati
+00001820: 6f6e 222c 0a0a 2020 2020 2020 2020 2273  on",..        "s
+00001830: 7465 702d 6361 7073 756c 6522 2c0a 2020  tep-capsule",.  
+00001840: 2020 2020 2020 2273 7465 702d 7374 6174        "step-stat
+00001850: 7573 222c 0a20 2020 2020 2020 2022 7374  us",.        "st
+00001860: 6570 2d64 7572 6174 696f 6e22 2c0a 0a20  ep-duration",.. 
+00001870: 2020 2020 2020 2022 6d65 7373 6167 6573         "messages
+00001880: 222c 0a20 2020 2020 2020 2022 656d 6265  ",.        "embe
+00001890: 645f 6275 7474 6f6e 222c 0a20 2020 2020  d_button",.     
+000018a0: 2020 2022 6c69 6e6b 222c 0a20 2020 2020     "link",.     
+000018b0: 2020 2022 7461 626c 6522 2c0a 0a20 2020     "table",..   
+000018c0: 205d 3b0a 2020 2020 636f 6e74 7261 7374   ];.    contrast
+000018d0: 5f63 6c61 7373 6573 2e66 6f72 4561 6368  _classes.forEach
+000018e0: 2874 6f67 676c 655f 636f 6e74 7261 7374  (toggle_contrast
+000018f0: 5f66 6f72 293b 0a7d 3b0a 0a66 756e 6374  _for);.};..funct
+00001900: 696f 6e20 6465 7465 6374 5f63 6f6e 7472  ion detect_contr
+00001910: 6173 7428 2920 7b0a 2020 2020 7661 7220  ast() {.    var 
+00001920: 6f62 6a5f 6469 7620 3d20 646f 6375 6d65  obj_div = docume
+00001930: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
+00001940: 2822 6469 7622 293b 0a20 2020 206f 626a  ("div");.    obj
+00001950: 5f64 6976 2e73 7479 6c65 2e63 6f6c 6f72  _div.style.color
+00001960: 203d 2022 7267 6228 3331 2c20 3431 2c20   = "rgb(31, 41, 
+00001970: 3539 2922 0a20 2020 2064 6f63 756d 656e  59)".    documen
+00001980: 742e 626f 6479 2e61 7070 656e 6443 6869  t.body.appendChi
+00001990: 6c64 286f 626a 5f64 6976 293b 0a20 2020  ld(obj_div);.   
+000019a0: 2076 6172 2063 6f6c 203d 2064 6f63 756d   var col = docum
+000019b0: 656e 742e 6465 6661 756c 7456 6965 7720  ent.defaultView 
+000019c0: 3f20 646f 6375 6d65 6e74 2e64 6566 6175  ? document.defau
+000019d0: 6c74 5669 6577 2e67 6574 436f 6d70 7574  ltView.getComput
+000019e0: 6564 5374 796c 6528 6f62 6a5f 6469 762c  edStyle(obj_div,
+000019f0: 206e 756c 6c29 2e63 6f6c 6f72 203a 206f   null).color : o
+00001a00: 626a 5f64 6976 2e63 7572 7265 6e74 5374  bj_div.currentSt
+00001a10: 796c 652e 636f 6c6f 723b 0a20 2020 2064  yle.color;.    d
+00001a20: 6f63 756d 656e 742e 626f 6479 2e72 656d  ocument.body.rem
+00001a30: 6f76 6543 6869 6c64 286f 626a 5f64 6976  oveChild(obj_div
+00001a40: 293b 0a20 2020 2063 6f6c 203d 2063 6f6c  );.    col = col
+00001a50: 2e72 6570 6c61 6365 282f 202f 672c 2022  .replace(/ /g, "
+00001a60: 2229 3b0a 2020 2020 6966 2028 636f 6c20  ");.    if (col 
+00001a70: 213d 3d20 2272 6762 2833 312c 3431 2c35  !== "rgb(31,41,5
+00001a80: 3929 2229 207b 0a20 2020 2020 2020 2063  9)") {.        c
+00001a90: 6f6e 736f 6c65 2e6c 6f67 2822 4869 6768  onsole.log("High
+00001aa0: 2043 6f6e 7472 6173 7420 7468 656d 6520   Contrast theme 
+00001ab0: 6465 7465 6374 6564 2e22 290a 2020 2020  detected.").    
+00001ac0: 2020 2020 746f 6767 6c65 5f63 6f6e 7472      toggle_contr
+00001ad0: 6173 7428 293b 0a20 2020 207d 0a7d 0a0a  ast();.    }.}..
+00001ae0: 7661 7220 656c 656d 656e 7420 3d20 646f  var element = do
+00001af0: 6375 6d65 6e74 2e63 7265 6174 6545 6c65  cument.createEle
+00001b00: 6d65 6e74 2827 6469 7627 293b 0a76 6172  ment('div');.var
+00001b10: 2065 6e74 6974 7920 3d20 2f26 283f 3a23   entity = /&(?:#
+00001b20: 785b 612d 6630 2d39 5d2b 7c23 5b30 2d39  x[a-f0-9]+|#[0-9
+00001b30: 5d2b 7c5b 612d 7a30 2d39 5d2b 293b 3f2f  ]+|[a-z0-9]+);?/
+00001b40: 6967 3b0a 0a66 756e 6374 696f 6e20 6465  ig;..function de
+00001b50: 636f 6465 4854 4d4c 456e 7469 7469 6573  codeHTMLEntities
+00001b60: 2873 7472 2920 7b0a 2020 2020 7374 7220  (str) {.    str 
+00001b70: 3d20 7374 722e 7265 706c 6163 6528 656e  = str.replace(en
+00001b80: 7469 7479 2c20 6675 6e63 7469 6f6e 2028  tity, function (
+00001b90: 6d29 207b 0a20 2020 2020 2020 2065 6c65  m) {.        ele
+00001ba0: 6d65 6e74 2e69 6e6e 6572 4854 4d4c 203d  ment.innerHTML =
+00001bb0: 206d 3b0a 2020 2020 2020 2020 7265 7475   m;.        retu
+00001bc0: 726e 2065 6c65 6d65 6e74 2e74 6578 7443  rn element.textC
+00001bd0: 6f6e 7465 6e74 3b0a 2020 2020 7d29 3b0a  ontent;.    });.
+00001be0: 2020 2020 656c 656d 656e 742e 7465 7874      element.text
+00001bf0: 436f 6e74 656e 7420 3d20 2727 3b0a 2020  Content = '';.  
+00001c00: 2020 7265 7475 726e 2073 7472 3b0a 7d0a    return str;.}.
+00001c10: 0a66 756e 6374 696f 6e20 646f 776e 6c6f  .function downlo
+00001c20: 6164 5f65 6d62 6564 2869 642c 2066 696c  ad_embed(id, fil
+00001c30: 656e 616d 6529 207b 0a20 2020 2076 6172  ename) {.    var
+00001c40: 2065 6c65 6d20 3d20 646f 6375 6d65 6e74   elem = document
+00001c50: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
+00001c60: 6964 293b 0a20 2020 2076 6172 2063 6869  id);.    var chi
+00001c70: 6c64 203d 2065 6c65 6d2e 6368 696c 6472  ld = elem.childr
+00001c80: 656e 5b31 5d3b 0a20 2020 2076 6172 2076  en[1];.    var v
+00001c90: 616c 7565 203d 2022 223b 0a20 2020 2076  alue = "";.    v
+00001ca0: 6172 2074 6167 203d 2063 6869 6c64 2e74  ar tag = child.t
+00001cb0: 6167 4e61 6d65 2e74 6f4c 6f77 6572 4361  agName.toLowerCa
+00001cc0: 7365 2829 3b0a 2020 2020 6966 2028 7461  se();.    if (ta
+00001cd0: 6720 3d3d 3d20 2273 7061 6e22 2920 7b0a  g === "span") {.
+00001ce0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+00001cf0: 202b 3d20 222e 7478 7422 3b0a 2020 2020   += ".txt";.    
+00001d00: 2020 2020 7661 6c75 6520 3d20 2264 6174      value = "dat
+00001d10: 613a 7465 7874 2f70 6c61 696e 2c22 202b  a:text/plain," +
+00001d20: 2065 6e63 6f64 6555 5249 436f 6d70 6f6e   encodeURICompon
+00001d30: 656e 7428 6465 636f 6465 4854 4d4c 456e  ent(decodeHTMLEn
+00001d40: 7469 7469 6573 2863 6869 6c64 2e69 6e6e  tities(child.inn
+00001d50: 6572 4854 4d4c 2929 3b0a 2020 2020 7d20  erHTML));.    } 
+00001d60: 656c 7365 2069 6620 2874 6167 203d 3d20  else if (tag == 
+00001d70: 2276 6964 656f 2229 207b 0a20 2020 2020  "video") {.     
+00001d80: 2020 2066 696c 656e 616d 6520 2b3d 2022     filename += "
+00001d90: 2e77 6562 6d22 3b0a 2020 2020 2020 2020  .webm";.        
+00001da0: 7661 6c75 6520 3d20 6368 696c 642e 6368  value = child.ch
+00001db0: 696c 6472 656e 5b30 5d2e 7372 633b 0a20  ildren[0].src;. 
+00001dc0: 2020 207d 2065 6c73 6520 6966 2028 7461     } else if (ta
+00001dd0: 6720 3d3d 2022 696d 6722 2920 7b0a 2020  g == "img") {.  
+00001de0: 2020 2020 2020 6669 6c65 6e61 6d65 202b        filename +
+00001df0: 3d20 222e 706e 6722 3b0a 2020 2020 2020  = ".png";.      
+00001e00: 2020 7661 6c75 6520 3d20 6368 696c 642e    value = child.
+00001e10: 7372 633b 0a20 2020 207d 2065 6c73 6520  src;.    } else 
+00001e20: 7b0a 2020 2020 2020 2020 6669 6c65 6e61  {.        filena
+00001e30: 6d65 202b 3d20 222e 6874 6d6c 223b 0a20  me += ".html";. 
+00001e40: 2020 2020 2020 2076 616c 7565 203d 2064         value = d
+00001e50: 6563 6f64 6548 544d 4c45 6e74 6974 6965  ecodeHTMLEntitie
+00001e60: 7328 6368 696c 642e 696e 6e65 7248 544d  s(child.innerHTM
+00001e70: 4c29 3b0a 2020 2020 7d0a 2020 2020 7661  L);.    }.    va
+00001e80: 7220 6c69 6e6b 203d 2064 6f63 756d 656e  r link = documen
+00001e90: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
+00001ea0: 2261 2229 3b0a 2020 2020 6c69 6e6b 2e73  "a");.    link.s
+00001eb0: 7479 6c65 2e64 6973 706c 6179 203d 2022  tyle.display = "
+00001ec0: 6e6f 6e65 223b 0a20 2020 206c 696e 6b2e  none";.    link.
+00001ed0: 6872 6566 203d 2076 616c 7565 3b0a 2020  href = value;.  
+00001ee0: 2020 6c69 6e6b 2e64 6f77 6e6c 6f61 6420    link.download 
+00001ef0: 3d20 6669 6c65 6e61 6d65 3b0a 2020 2020  = filename;.    
+00001f00: 646f 6375 6d65 6e74 2e62 6f64 792e 6170  document.body.ap
+00001f10: 7065 6e64 4368 696c 6428 6c69 6e6b 293b  pendChild(link);
+00001f20: 0a20 2020 206c 696e 6b2e 636c 6963 6b28  .    link.click(
+00001f30: 290a 2020 2020 2f2a 2066 6978 2072 6163  ).    /* fix rac
+00001f40: 6520 696e 2046 4620 2a2f 0a20 2020 2073  e in FF */.    s
+00001f50: 6574 5469 6d65 6f75 7428 6675 6e63 7469  etTimeout(functi
+00001f60: 6f6e 2028 2920 7b20 646f 6375 6d65 6e74  on () { document
+00001f70: 2e62 6f64 792e 7265 6d6f 7665 4368 696c  .body.removeChil
+00001f80: 6428 6c69 6e6b 293b 207d 2c20 3230 3030  d(link); }, 2000
+00001f90: 293b 0a7d 3b                             );.};
```

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.css` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.min.css`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/behave.min.js` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/behave.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -37,16 +37,15 @@
 window.onhashchange = hash_to_state;
 
 function toggle_hash(id) {
     console.log("Toggle ID: " + id);
     hash_uuid_list_change.push(id);
     if (hash_uuid_list.includes(id)) {
         hash_uuid_list.splice(hash_uuid_list.indexOf(id), 1);
-    };
-    else {
+    } else {
         hash_uuid_list.push(id);
     };
     var hash = "#";
     if (hash_uuid_list.length != 0) {
         hash = toggle_non_empty_string + hash_uuid_list.toString()
     };
     console.log("New hash: " + hash);
@@ -117,16 +116,15 @@
         capsule.classList.add("collapse");
     }
 };
 
 function toggle_class(elem, class_name) {
     if (elem.classList.contains(class_name)) {
         elem.classList.remove(class_name);
-    };
-    else {
+    } else {
         elem.classList.add(class_name)
     }
 };
 
 function toggle_contrast_for(target_class) {
     var elements = document.getElementsByClassName(target_class);
     for (var i = 0; i < elements.length; i++) {
```

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter/html_pretty.py` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter/html_pretty.py`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/PKG-INFO` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-html-pretty-formatter
-Version: 1.9
+Version: 1.9.1
 Summary: Pretty HTML Formatter for Behave
 Home-page: https://github.com/behave-contrib/behave-html-pretty-formatter
 Author: Michal Odehnal
 Author-email: modehnal@redhat.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `behave-html-pretty-formatter-1.9/behave_html_pretty_formatter.egg-info/SOURCES.txt` & `behave-html-pretty-formatter-1.9.1/behave_html_pretty_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.9/setup.py` & `behave-html-pretty-formatter-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Return the content of a file."""
     with open(filename, "r", encoding="utf-8") as file:
         return file.read()
 
 
 setuptools.setup(
     name="behave-html-pretty-formatter",
-    version="1.9",
+    version="1.9.1",
     author="Michal Odehnal",
     author_email="modehnal@redhat.com",
     description="""
 Pretty HTML Formatter for Behave
 
 Authors:
 Michal Odehnal <modehnal@redhat.com>,
```

