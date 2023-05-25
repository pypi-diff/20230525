# Comparing `tmp/vizad-0.0.4.tar.gz` & `tmp/vizad-0.1.tar.gz`

## Comparing `vizad-0.0.4.tar` & `vizad-0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.4/.DS_Store
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/eda.iml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vizad-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.4/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.0.4/src/vizad/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vizad-0.0.4/src/vizad/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 vizad-0.0.4/src/vizad/bivariate.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 vizad-0.0.4/src/vizad/univariate.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 vizad-0.0.4/LICENSE
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 vizad-0.0.4/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 vizad-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 vizad-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.1/.DS_Store
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vizad-0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 vizad-0.1/.idea/eda.iml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 vizad-0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 vizad-0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vizad-0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 vizad-0.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vizad-0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vizad-0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.1/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 vizad-0.1/src/vizad/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vizad-0.1/src/vizad/__init__.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 vizad-0.1/src/vizad/bivariate.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 vizad-0.1/src/vizad/univariate.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 vizad-0.1/LICENSE
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 vizad-0.1/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 vizad-0.1/pyproject.toml
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 vizad-0.1/PKG-INFO
```

### Comparing `vizad-0.0.4/.idea/workspace.xml` & `vizad-0.1/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `vizad-0.0.4/.idea/inspectionProfiles/Project_Default.xml` & `vizad-0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `vizad-0.0.4/src/.DS_Store` & `vizad-0.1/src/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 00000280: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
 00000290: 7208 0908 095f 1018 7b7b 3433 362c 2033  r...._..{{436, 3
 000002a0: 3736 7d2c 207b 3932 302c 2034 3336 7d7d  76}, {920, 436}}
 000002b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 000002c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000002d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000002e0: 0005 0076 0069 007a 0061 0064 6473 636c  ...v.i.z.a.ddscl
-000002f0: 626f 6f6c 0100 0000 0500 7600 6900 7a00  bool......v.i.z.
-00000300: 6100 6466 6473 6362 6f6f 6c00 0000 0005  a.dfdscbool.....
+000002f0: 626f 6f6c 0000 0000 0500 7600 6900 7a00  bool......v.i.z.
+00000300: 6100 6466 6473 6362 6f6f 6c01 0000 0005  a.dfdscbool.....
 00000310: 0076 0069 007a 0061 0064 7653 726e 6c6f  .v.i.z.a.dvSrnlo
 00000320: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `vizad-0.0.4/src/vizad/.DS_Store` & `vizad-0.1/src/vizad/.DS_Store`

 * *Files identical despite different names*

### Comparing `vizad-0.0.4/src/vizad/bivariate.py` & `vizad-0.1/src/vizad/bivariate.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # using the plot type specified in the kind parameter
 # diag_kind and corner parameters to be ignored if kind is heatmap
 
 def plot_bivariate_numeric(data,
                            numcol_names,
                            kind='pairplot',
                            diag_kind='kde',
-                           corner=True):
+                           corner=True,
+                           figsize=None):
     """
     This function takes a pandas dataframe and a list of column names containing the names of
 numeric columns and plots bivariate distribution of each column vs. each other column. The
 user can choose the kind of plot to be displayed using the 'kind' parameter. The function
 does not return anything.
 
 Parameters:
@@ -33,42 +34,51 @@
     The kind of plot to be displayed. Possible values are 'pairplot', 'heatmap'. Default is
     'pairplot'.
 diag_kind : str (default=None)
     The kind of plot for the diagonal subplots. Possible values are 'hist', 'kde'. Default is
     "kde". This parameter is ignored if kind is 'heatmap'.
 corner : bool (default=True)
     If True, the corner subplots are not shown. This parameter is ignored if kind is 'heatmap'.
-figsize : tuple of int (default=(15,15))
-    The size of the figure to be displayed.
+figsize : tuple of int (default=None)
+    The size of the figure to be displayed. If None, the figsize is set to (max(3*len(numcol_names),10),
+    max(3*len(numcol_names),10)).
 
     """
+    if figsize is None:
+        figsize = (max(3*len(numcol_names),10),max(3*len(numcol_names),10))
+
     
     if kind == 'pairplot':
         # plot the pairplot with size the figsize parameter
         
         sns.pairplot(data[numcol_names],
                         diag_kind=diag_kind,
                         corner=corner)
         
         # add a title to the figure containing the plot
         plt.suptitle("Bivariate Analysis of numeric features", fontsize='xx-large')
+        plt.tight_layout()
     elif kind == 'heatmap':
         corel = data[numcol_names].corr().round(2)
+        # create a figure with size the figsize parameter
+        fig, axes = plt.subplots(figsize=figsize)
         sns.heatmap(corel,
                     annot=True,
                     cmap='plasma',
                     vmin=-1,
                     vmax=1,
                     linewidths=1,
                     linecolor='white',
-                    mask=np.triu(corel, 1))
+                    mask=np.triu(corel, 1),
+                    ax=axes)
         # add a title to the figure
         plt.title("Bivariate Analysis of numeric features-Correlation Heatmap", fontsize='xx-large')
         plt.xticks(rotation=45)
         plt.yticks(rotation=0)
+        plt.tight_layout()
     else:
         print("Invalid kind parameter value for plot type. Allowed values are 'pairplot', 'heatmap'")
 
 
 
 # write a function that takes the following as input:
 # - a pandas dataframe
```

### Comparing `vizad-0.0.4/src/vizad/univariate.py` & `vizad-0.1/src/vizad/univariate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 
-def plot_univariate_numeric(df, numcols_name, subplot_cols=3, kind="box"):
+def plot_univariate_numeric(df, numcols_name, subplot_cols=3, kind="box",figsize=(10,3)):
     """
     This function takes a pandas dataframe and a list of column names containing
     numeric values and plots univariate distribution of each column. The user can
     choose the kind of plot to be displayed using the 'kind' parameter. The function
     returns a matplotlib figure object.
 
     Parameters:
@@ -17,30 +17,34 @@
     numcols_name : list of str
         The list of column names containing numeric values.
     subplot_cols : int (default=3)
         The number of subplots columns to display.
     kind : str (default='box')
         The kind of plot to be displayed. Possible values are 'box', 'hist', and
         'density'.
+    figsize : tuple of int (default=(10,3))
 
     Returns:
     --------
     None
     """
     numcols_len = len(numcols_name)
     subplot_rows = 1
     # handle edge case when subplot_cols > numcols_len
     if subplot_cols >= numcols_len:
         subplot_cols = numcols_len
     else:
         subplot_rows = int(np.ceil(numcols_len/subplot_cols))
 
         
-    fig, axes = plt.subplots(subplot_rows,subplot_cols,figsize=(subplot_cols*3,subplot_rows*3))
-
+    fig, axes = plt.subplots(subplot_rows,
+                             subplot_cols,
+                             figsize=(max(subplot_cols*3,figsize[0]),
+                                      max(subplot_rows*3,figsize[1])))
+    
 
     # if subplot_rows == 1 or subplot_cols==1 then the axes object will be a 1D array
     # so we need to handle this case differently
     if (subplot_rows == 1) | (subplot_cols == 1):
         for i in range(numcols_len):
             if kind == "box":
                 sns.boxplot(x=numcols_name[i],data=df,ax=axes[i])
@@ -55,14 +59,17 @@
                 raise ValueError("kind parameter can only take values 'box', 'hist', or 'density'")
         
         # remove the excess axes
         excess_plots = subplot_rows*subplot_cols - numcols_len
         if excess_plots > 0:
             for i in range(numcols_len,subplot_rows*subplot_cols):
                 fig.delaxes(axes[i//subplot_cols,i%subplot_cols])
+        # add suptitle
+        fig.suptitle("Univariate Analysis: Numeric Features",fontsize=20)
+        plt.subplots_adjust(top=0.85) # adjust top spacing
         plt.tight_layout()
     else: # if subplot_rows > 1 then the axes object will be a 2D array
         for i in range(numcols_len):
             if kind == "box":
                 sns.boxplot(x=numcols_name[i],data=df,ax=axes[i//subplot_cols,i%subplot_cols])
             elif kind == "hist":
                 sns.histplot(x=numcols_name[i],data=df,ax=axes[i//subplot_cols,i%subplot_cols])
@@ -75,18 +82,16 @@
                 raise ValueError("kind parameter can only take values 'box', 'hist', or 'density'")
         
         # remove the excess axes
         excess_plots = subplot_rows*subplot_cols - numcols_len
         if excess_plots > 0:
             for i in range(numcols_len,subplot_rows*subplot_cols):
                 fig.delaxes(axes[i//subplot_cols,i%subplot_cols])
-        plt.tight_layout()
-    # add suptitle
-    fig.suptitle("Univariate Analysis: Numeric Features",fontsize=20)
-    plt.tight_layout()
+        
+        plt.tight_layout()    
 
 
 
 def plot_univariate_categorical(df, catcols_name, subplot_cols=3, kind="count",figsize=(10,10)):
     """
     This function takes a pandas dataframe and a list of column names containing
     categorical values and plots univariate distribution of each column. The user
```

### Comparing `vizad-0.0.4/LICENSE` & `vizad-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vizad-0.0.4/pyproject.toml` & `vizad-0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vizad"
-version = "0.0.4"
+version = "0.1"
 authors = [
     {name = "Balaji Sundararaman", email = "bala@python4u.in"},
 ]
 description = "A simple visualization library for univariate and bivariate analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vizad-0.0.4/PKG-INFO` & `vizad-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizad
-Version: 0.0.4
+Version: 0.1
 Summary: A simple visualization library for univariate and bivariate analysis
 Project-URL: Homepage, https://github.com/bala-srm/eda
 Project-URL: Bug Tracker, https://github.com/bala-srm/eda/issues
 Author-email: Balaji Sundararaman <bala@python4u.in>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

