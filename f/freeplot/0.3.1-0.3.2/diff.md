# Comparing `tmp/freeplot-0.3.1.tar.gz` & `tmp/freeplot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplot-0.3.1.tar", last modified: Sun Apr  9 12:09:27 2023, max compression
+gzip compressed data, was "freeplot-0.3.2.tar", last modified: Thu May 25 01:53:50 2023, max compression
```

## Comparing `freeplot-0.3.1.tar` & `freeplot-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 12:09:27.919465 freeplot-0.3.1/
--rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     7420 2023-04-09 12:09:27.918464 freeplot-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 12:09:27.894497 freeplot-0.3.1/freeplot/
--rw-rw-rw-   0        0        0       51 2023-04-09 12:08:20.000000 freeplot-0.3.1/freeplot/__init__.py
--rw-rw-rw-   0        0        0    17958 2023-02-17 05:04:04.000000 freeplot-0.3.1/freeplot/base.py
--rw-rw-rw-   0        0        0     3682 2023-02-17 05:04:08.000000 freeplot-0.3.1/freeplot/config.py
--rw-rw-rw-   0        0        0    23929 2023-02-21 12:02:26.000000 freeplot-0.3.1/freeplot/unit.py
--rw-rw-rw-   0        0        0     2303 2023-02-17 05:04:16.000000 freeplot-0.3.1/freeplot/utils.py
--rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.3.1/freeplot/zoo.py
-drwxrwxrwx   0        0        0        0 2023-04-09 12:09:27.918464 freeplot-0.3.1/freeplot.egg-info/
--rw-rw-rw-   0        0        0     7420 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 12:09:27.919465 freeplot-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-04-09 12:08:12.000000 freeplot-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:53:50.796381 freeplot-0.3.2/
+-rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     7420 2023-05-25 01:53:50.795380 freeplot-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 01:53:50.756380 freeplot-0.3.2/freeplot/
+-rw-rw-rw-   0        0        0       51 2023-05-25 01:53:10.000000 freeplot-0.3.2/freeplot/__init__.py
+-rw-rw-rw-   0        0        0    17958 2023-02-17 05:04:04.000000 freeplot-0.3.2/freeplot/base.py
+-rw-rw-rw-   0        0        0     3682 2023-04-20 05:14:16.000000 freeplot-0.3.2/freeplot/config.py
+-rw-rw-rw-   0        0        0    25144 2023-04-17 13:09:51.000000 freeplot-0.3.2/freeplot/unit.py
+-rw-rw-rw-   0        0        0     2303 2023-02-17 05:04:16.000000 freeplot-0.3.2/freeplot/utils.py
+-rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.3.2/freeplot/zoo.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:53:50.794381 freeplot-0.3.2/freeplot.egg-info/
+-rw-rw-rw-   0        0        0     7420 2023-05-25 01:53:50.000000 freeplot-0.3.2/freeplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-25 01:53:50.000000 freeplot-0.3.2/freeplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:53:50.000000 freeplot-0.3.2/freeplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-25 01:53:50.000000 freeplot-0.3.2/freeplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 01:53:50.000000 freeplot-0.3.2/freeplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 01:53:50.797380 freeplot-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-04-30 02:42:02.000000 freeplot-0.3.2/setup.py
```

### Comparing `freeplot-0.3.1/LICENSE` & `freeplot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.1/PKG-INFO` & `freeplot-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.3.1
+Version: 0.3.2
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freeplot-0.3.1/README.md` & `freeplot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.1/freeplot/base.py` & `freeplot-0.3.2/freeplot/base.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.1/freeplot/config.py` & `freeplot-0.3.2/freeplot/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         super(Config, self).__setitem__(key, value)
         self.__setattr__(key, value)
 
 
 
 COLORS = (
     "#2D2C40",
-    "#B3002A",
     "#0050C2",
+    "#B3002A",
     "#006058",
     "#3A4E8C",
     "#D99F6C",
     "#BF3F34",
 )
 
 MARKERS = (
```

### Comparing `freeplot-0.3.1/freeplot/unit.py` & `freeplot-0.3.2/freeplot/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,28 @@
 
         Examples:
 
         >>> fp.set_text(0.5, 0.5, s='GoGoGo', fontsize='big)
         """
         return self[index].text(x, y, s, fontdict, **kwargs)
 
+    def set_arrow(
+        self, 
+        x: float, y: float,
+        dx: float, dy: float,
+        width: float, head_width: float,
+        index = (0, 0), color: str = 'r', alpha: float = 0.5,
+        **kwargs
+    ):
+        return self[index].arrow(
+            x, y, dx, dy,
+            width=width, head_width=head_width,
+            color=color, alpha=alpha, **kwargs
+        )
+
     def set_title(self, y: float = .99) -> None:
         """Set titles for Axes.
         
         Parameters:
         ---
 
         y: The height from the bottom.
@@ -385,14 +399,44 @@
         labels = [fmt%value for value in values]
         kwargs = dict()
         kwargs['index'] = index
         kwargs[axis + 'ticks'] = values
         kwargs[axis + 'ticklabels'] = labels
         return self.set(**kwargs)
 
+    def fill_between(
+        self,
+        x: Iterable,
+        lower: Iterable, upper: Iterable,
+        alpha: float = 0.5, linewidth: float = 0.,
+        index = (0, 0),
+        **kwargs
+    ):
+        """
+        Fill between lower and upper.
+
+        Parameters:
+        -----------
+
+        x: array
+            The x coordinates of the nodes defining the curves.
+        lower: array or scalar
+            The y coordinates of the nodes defining the first curve.
+        upper: array or scalar
+            The y coordinates of the nodes defining the second curve.
+        
+        Returns:
+        --------
+
+        PolyCollection
+        """
+        return self[index].fill_between(
+            x, lower, upper, alpha=alpha, linewidth=linewidth,
+            **kwargs
+        )
     
     def ticklabel_format(
         self, style: str = 'sci', scilimits: Iterable[int] = (0, 0),
         index: Union[Axes, str, Iterable[int], slice, None] = (0, 0), 
         axis: str = 'y', **kwargs
     ):
         """Configure the ScalarFormatter used by default for linear Axes.
```

### Comparing `freeplot-0.3.1/freeplot/utils.py` & `freeplot-0.3.2/freeplot/utils.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.1/freeplot/zoo.py` & `freeplot-0.3.2/freeplot/zoo.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.1/freeplot.egg-info/PKG-INFO` & `freeplot-0.3.2/freeplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.3.1
+Version: 0.3.2
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freeplot-0.3.1/setup.py` & `freeplot-0.3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,16 @@
   long_description = fh.read()
 
 requires = [
     'numpy>=1.18.1',
     'pandas>=1.0.1',
     'scipy>=1.4.1',
     'scikit-learn>=0.23.2',
-    'matplotlib>=3.1.3',
-    'seaborn>=0.10.0',
+    'matplotlib==3.1.3',
+    'seaborn==0.10.0',
     'SciencePlots==1.0.9'
 ]
 
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
```

