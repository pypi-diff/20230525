# Comparing `tmp/dsmltf-0.0.3.tar.gz` & `tmp/dsmltf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dsmltf-0.0.3.tar", last modified: Mon May 15 20:15:21 2023, max compression
+gzip compressed data, was "dsmltf-0.0.5.tar", last modified: Thu May 25 13:14:05 2023, max compression
```

## Comparing `dsmltf-0.0.3.tar` & `dsmltf-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-15 20:15:21.000000 dsmltf-0.0.3/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-15 20:15:21.000000 dsmltf-0.0.3/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 dsmltf-0.0.3/README.md
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-15 20:15:21.000000 dsmltf-0.0.3/dsmltf/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 dsmltf-0.0.3/dsmltf/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    33332 2023-05-15 19:12:42.000000 dsmltf-0.0.3/dsmltf/main.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-15 20:15:21.000000 dsmltf-0.0.3/dsmltf.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-15 20:15:21.000000 dsmltf-0.0.3/dsmltf.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      182 2023-05-15 20:15:21.000000 dsmltf-0.0.3/dsmltf.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-15 20:15:21.000000 dsmltf-0.0.3/dsmltf.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-15 20:15:21.000000 dsmltf-0.0.3/dsmltf.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-15 20:15:21.000000 dsmltf-0.0.3/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      623 2023-05-15 20:15:11.000000 dsmltf-0.0.3/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 13:14:05.897046 dsmltf-0.0.5/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    35201 2023-05-14 06:35:21.000000 dsmltf-0.0.5/LICENSE
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      618 2023-05-25 13:14:05.897321 dsmltf-0.0.5/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 dsmltf-0.0.5/README.md
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 13:14:05.893300 dsmltf-0.0.5/dsmltf/
+-rwxr-xr-x   0 sergejzuev   (501) staff       (20)       19 2023-05-15 20:13:28.000000 dsmltf-0.0.5/dsmltf/__init__.py
+-rw-r--r--   0 sergejzuev   (501) staff       (20)    30600 2023-05-25 12:55:41.000000 dsmltf-0.0.5/dsmltf/main.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-25 13:14:05.896027 dsmltf-0.0.5/dsmltf.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      618 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      190 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-25 13:14:05.000000 dsmltf-0.0.5/dsmltf.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-25 13:14:05.898828 dsmltf-0.0.5/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      623 2023-05-25 13:13:45.000000 dsmltf-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dsmltf-0.0.3/PKG-INFO` & `dsmltf-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: dsmltf
-Version: 0.0.3
+Version: 0.0.5
 Summary: A set of functions to study Data Science
-Home-page: UNKNOWN
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
-License: UNKNOWN
-Description: The dsmltf (Data Science and Machine Learning Training Functions) contains 
-        a set of functions to be used for educational purposes during study the  
-        Data Science course. Most of functions are described in the textbook 
-        available from the author by request on email shoukhov@mail.ru.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+The dsmltf (Data Science and Machine Learning Training Functions) contains 
+a set of functions to be used for educational purposes during study the  
+Data Science course. Most of functions are described in the textbook 
+available from the author by request on email shoukhov@mail.ru.
```

### Comparing `dsmltf-0.0.3/dsmltf/main.py` & `dsmltf-0.0.5/dsmltf/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -371,15 +371,15 @@
             return (matrix[i][j] - means[j])/stdevs[j]
         else:
             return matrix[i][j]
     return make_matrix(rows,cols,res)
 def de_mean_matrix(A):
     r, c = shape(A)
     columns_means = [mean(get_column(A,i)) for i in range(c)]
-    return make_matrix(r, c, lambda i, j: A[i][j] - columns_means[j])
+    return make_matrix(r, c, lambda i, j: A[i][j] - column_means[j])
 def direction(w):
     return [w_i/magnitude(w) for w_i in w]
 def dir_variance(X,w):
     return sum(dot(x_i, direction(w))**2 for x_i in X)
 def the_first_priciple_comp(data):
     n = len(data[0])
     init_w = [random.random() for _ in range(n)]
@@ -630,15 +630,15 @@
     B.append(b)
     if len(layers) == 1:
         return WW, B
     else:
         for s,ls in enumerate(layers[1:]):
             W, b = [], []
             for lj in range(ls):
-                W.append([random()-1/2 for _ in range(layers[s])])
+                W.append([random.random()-1/2 for _ in range(layers[s])])
                 b.append(0)
             WW.append(W)
             B.append(b)
         return WW, B
 def forward(data, WW, B): # data не содержат метки
     layer_outputs = [[] for _ in B]
     for d in data:
@@ -813,75 +813,7 @@
     while True:
         candidates = trans[(first, second)]
         next_word = random.choice(candidates)
         first, second = second, next_word
         result.append(second)
         if second == '.':
             return " ".join(result)
-
-def gs_step_down(data, powers = {}): # just non-negative integers in data
-    pwrs = getpower(data, powers)
-    smallest = dict(sorted(pwrs.items(), key=lambda item: item[1])[:2])
-    n1,n2 = tuple(smallest.keys())
-    newdata = []
-    for d in data:
-        nd = [di if i not in [n1,n2] else d[n1] + smallest[n1]*d[n2] for i,di in enumerate(d) if i!= n2]
-        newdata.append(nd)
-    return newdata, n1,n2,smallest[n1],smallest[n2] # features number n1 and n2 are unified into n1, number n2 is dropped in newdata
-def gs_step_downback(newdata, n1,n2,N1): #performs backward from down transformation of the newdata to data
-    data = []
-    for nd in newdata:
-        d = [ndi if i!=n1 else ndi%N1 for i,ndi in enumerate(nd[:n2])] + [nd[n1]//N1] + [ndi if i!=n1-1 else ndi%N1 for i,ndi in enumerate(nd[n2:])]
-        data.append(d)
-    return data
-
-def gs_step_up(data, powers = {}): # just non-negative integers in data
-    pwrs = getpower(data, powers)
-    biggest = dict(sorted(pwrs.items(), key=lambda item: item[1], reverse = True)[:1])
-    n1 = list(biggest.keys())[0]
-    B = biggest[n1]
-    N1 = int(B**(1/2))
-    N2 = (B//N1 if not B%N1 else B//N1 + 1) 
-    newdata = []
-    for d in data:
-        nd = (d[:n1] + [d[n1]%N1] + d[n1+1:] + [d[n1]//N1]) if n1<len(d)-1 else (d[:n1] + [d[n1]%N1] + [d[n1]//N1])
-        newdata.append(nd)
-    return newdata, n1, N1, N2 # feature number n1 is splited onto feature number n1 with power N1 and the last feature powered N2 in newdata 
-def gs_step_upback(newdata, n1, N1): #performs backward from up transformation of the newdata to data
-    n = len(newdata[0]) - 1
-    data = []
-    for nd in newdata:
-        d = [ndi if i!=n1 else ndi+N1*nd[-1] for i,ndi in enumerate(nd[:-1])]
-        data.append(d)
-    return data
-def getpower(data, powers = {}):
-    n = len(data[0])
-    for k in range(n):
-        if k in powers.keys():
-            continue
-        else:
-            powers[k] = max([d[k] for d in data])+1
-    return powers
-
-def genser(data,m, powers = {}): # transforms data to newdata of dimension m, keeps parameters saved in stat_dict (for backward transformation)
-    stat_dict = {}
-    n = len(data[0])
-    newdata = copy(data)
-    pwrs = dict(powers)
-    if m<n:
-        for k in range(n-m):
-            newdata,n1,n2,N1,N2 = gs_step_down(newdata, pwrs)
-            stat_dict[-k-1] = [n1,n2,N1,N2]
-            pwrs[n1] = N1*N2
-            del pwrs[n2]
-            pwrs = getpower(newdata,pwrs)
-    elif m>n:
-        for k in range(m-n):
-            newdata, n1, N1, N2 = gs_step_up(newdata, pwrs)
-            stat_dict[k+1] = [n1,N1,N2]
-            pwrs[n1] = N1
-            pwrs[len(pwrs)] = N2
-            pwrs = getpower(newdata,pwrs)
-    return newdata, stat_dict
-
-
-
```

### Comparing `dsmltf-0.0.3/dsmltf.egg-info/PKG-INFO` & `dsmltf-0.0.5/dsmltf.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: dsmltf
-Version: 0.0.3
+Version: 0.0.5
 Summary: A set of functions to study Data Science
-Home-page: UNKNOWN
 Author: Sergei Zuev
 Author-email: shoukhov@mail.ru
-License: UNKNOWN
-Description: The dsmltf (Data Science and Machine Learning Training Functions) contains 
-        a set of functions to be used for educational purposes during study the  
-        Data Science course. Most of functions are described in the textbook 
-        available from the author by request on email shoukhov@mail.ru.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+The dsmltf (Data Science and Machine Learning Training Functions) contains 
+a set of functions to be used for educational purposes during study the  
+Data Science course. Most of functions are described in the textbook 
+available from the author by request on email shoukhov@mail.ru.
```

### Comparing `dsmltf-0.0.3/setup.py` & `dsmltf-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 #requirements = ["requests<=2.21.0"]
 
 setuptools.setup(name="dsmltf",
-	version="0.0.3",
+	version="0.0.5",
 	author="Sergei Zuev",
 	author_email="shoukhov@mail.ru",
 	description="A set of functions to study Data Science",
 	packages=setuptools.find_packages(),
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	classifiers=[
```

