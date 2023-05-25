# Comparing `tmp/FreeTVG-karjakak-3.2.8.tar.gz` & `tmp/FreeTVG-karjakak-3.2.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.8.tar", last modified: Thu May 25 07:09:15 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.8rc1.tar", last modified: Mon May 22 07:21:13 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.8.tar` & `FreeTVG-karjakak-3.2.8rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-25 07:09:15.768934 FreeTVG-karjakak-3.2.8/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-25 07:09:15.765194 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-25 07:09:15.000000 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-25 07:09:15.000000 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-25 07:09:15.000000 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-25 07:09:15.000000 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      151 2023-05-25 07:09:15.000000 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-25 07:09:15.000000 FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.8/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-25 07:09:15.769039 FreeTVG-karjakak-3.2.8/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.8/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-25 07:09:15.767195 FreeTVG-karjakak-3.2.8/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   142093 2023-05-25 06:08:21.000000 FreeTVG-karjakak-3.2.8/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   361457 2023-05-25 07:07:46.000000 FreeTVG-karjakak-3.2.8/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.8/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-25 07:09:15.767704 FreeTVG-karjakak-3.2.8/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.8/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.8/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-25 07:09:15.768615 FreeTVG-karjakak-3.2.8/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.8/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.8/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     6528 2023-05-25 06:01:26.000000 FreeTVG-karjakak-3.2.8/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.8/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      976 2023-05-25 07:09:15.769359 FreeTVG-karjakak-3.2.8/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.925195 FreeTVG-karjakak-3.2.8rc1/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.919670 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      151 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.8rc1/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-22 07:21:13.925277 FreeTVG-karjakak-3.2.8rc1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.8rc1/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.921853 FreeTVG-karjakak-3.2.8rc1/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   146320 2023-05-22 01:33:43.000000 FreeTVG-karjakak-3.2.8rc1/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   360883 2023-05-17 06:38:49.000000 FreeTVG-karjakak-3.2.8rc1/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.8rc1/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.923122 FreeTVG-karjakak-3.2.8rc1/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.8rc1/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.8rc1/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.924897 FreeTVG-karjakak-3.2.8rc1/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.8rc1/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.8rc1/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     7090 2023-05-22 07:20:50.000000 FreeTVG-karjakak-3.2.8rc1/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.8rc1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      979 2023-05-22 07:21:13.925567 FreeTVG-karjakak-3.2.8rc1/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.8/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.8
+Version: 3.2.8rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.8/LICENSE.txt` & `FreeTVG-karjakak-3.2.8rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8/PKG-INFO` & `FreeTVG-karjakak-3.2.8rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.8
+Version: 3.2.8rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.8/README.md` & `FreeTVG-karjakak-3.2.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.8rc1/TVG/FreeTVG.py`

 * *Files 2% similar despite different names*

```diff
@@ -2527,48 +2527,14 @@
                 i.destroy()
                 del i
             self.mdframe.destroy()
             self.__delattr__("mdb")
             self.__delattr__("mdframe")
             self.frb3.pack_forget()
 
-    def _compile_editor(self, rows: int):
-        self.store = tuple(i for i in self.text.get("0.0", END)[:-1].split("\n") if i)
-        ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
-        compiled = {}
-        et = rows
-        for i in self.store:
-            et += 1
-            if "s:" == i.lower()[:2]:
-                compiled[et] = ("space", "\n")
-            elif "p:" == i.lower()[:2]:
-                if i.partition(":")[2].isspace() or not bool(i.partition(":")[2]):
-                    raise Exception("Parent cannot be empty!")
-                else:
-                    compiled[et] = (
-                        "parent",
-                        i[2:].removeprefix(" "),
-                    )
-            elif i.lower().partition(":")[0] in list(ckc):
-                if i.partition(":")[2].isspace():
-                    compiled[et] = (
-                        ckc[i.partition(":")[0].lower()],
-                        i.partition(":")[2],
-                    )
-                elif bool(i.partition(":")[2]):
-                    compiled[et] = (
-                        ckc[i.partition(":")[0].lower()],
-                        i.partition(":")[2].removeprefix(" "),
-                    )
-        if len(self.store) != len(compiled):
-            raise Exception("Not Editable!")
-        self.store = None
-        del ckc
-        return compiled, et
-
     def editor(self):
         """This is direct editor on text window.
         FORMAT:
         "s:" for 'space'
         "p:" for 'parent'
         "c1:" - "c50:" for 'child1' to 'child50'
         """
@@ -2591,51 +2557,138 @@
                 self._mdbuttons()
                 if not self.plat.startswith("win"):
                     self.root.clipboard_clear()
                 del ckb
             else:
                 try:
                     if self.text.count("1.0", END, "chars")[0] > 1:
-                        stor = None
-                        if self.editorsel or (stor := self.listb.curselection()):
-                            stor = (
-                                self.editorsel if self.editorsel else (stor[0], stor[0])
-                            )
-                            p2 = self._compile_editor(stor[0])
-                            p1 = None
-                            p3 = None
-                            with tv(self.filename) as tvg:
-                                p1 = islice(tvg.insighttree(), 0, stor[0])
-                                if stor[1] <= tvg.getdatanum() - 1:
-                                    p3 = islice(
-                                        tvg.insighttree(),
-                                        stor[1],
-                                        tvg.getdatanum(),
-                                    )
-                                if p3:
-                                    p3 = tuple(v for v in dict(p3).values())
-                                    p3 = {p2[1] + j + 1: p3[j] for j in range(len(p3))}
-                                    combi = iter((dict(p1) | p2[0] | p3).values())
-                                else:
-                                    combi = iter((dict(p1) | p2[0]).values())
-                                tvg.fileread(combi)
-                            del tvg, p1, p2, combi, p3
-                        else:
-                            p2 = self._compile_editor(self.listb.size())
-                            with tv(self.filename) as tvg:
-                                if not self.nonetype():
-                                    tvg.fileread(iter(p2[0].values()))
-                                else:
+                        self.store = self.text.get("1.0", END)
+                        if self.nonetype():
+                            if self.editorsel:
+                                stor = self.editorsel
+                                ed = tuple(i for i in self.store[:-1].split("\n") if i)
+                                ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
+                                et = stor[0]
+                                p2 = {}
+                                p1 = None
+                                p3 = None
+                                for i in ed:
+                                    et += 1
+                                    if "s:" == i.lower()[:2]:
+                                        p2[et] = ("space", "\n")
+                                    elif "p:" == i.lower()[:2]:
+                                        if i.partition(":")[2].isspace() or not bool(
+                                            i.partition(":")[2]
+                                        ):
+                                            raise Exception("Parent cannot be empty!")
+                                        else:
+                                            p2[et] = (
+                                                "parent",
+                                                i[2:].removeprefix(" "),
+                                            )
+                                    elif i.lower().partition(":")[0] in list(ckc):
+                                        if i.partition(":")[2].isspace():
+                                            p2[et] = (
+                                                ckc[i.partition(":")[0].lower()],
+                                                i.partition(":")[2],
+                                            )
+                                        elif bool(i.partition(":")[2]):
+                                            p2[et] = (
+                                                ckc[i.partition(":")[0].lower()],
+                                                i.partition(":")[2].removeprefix(" "),
+                                            )
+                                if len(ed) != len(p2):
+                                    raise Exception("Not Editable!")
+                                with tv(self.filename) as tvg:
+                                    p1 = islice(tvg.insighttree(), 0, stor[0])
+                                    if stor[1] < tvg.getdatanum() - 1:
+                                        p3 = islice(
+                                            tvg.insighttree(),
+                                            stor[1],
+                                            tvg.getdatanum(),
+                                        )
+                                    if p3:
+                                        p3 = tuple(v for v in dict(p3).values())
+                                        p3 = {et + j + 1: p3[j] for j in range(len(p3))}
+                                        combi = iter((dict(p1) | p2 | p3).values())
+                                    else:
+                                        combi = iter((dict(p1) | p2).values())
+                                    tvg.fileread(combi)
+                                del stor, tvg, p1, ed, ckc, et, p2, combi, p3
+                            else:
+                                et = self.listb.size()
+                                ed = tuple(i for i in self.store[:-1].split("\n") if i)
+                                ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
+                                p2 = {}
+                                for i in ed:
+                                    et += 1
+                                    if "s:" == i.lower()[:2]:
+                                        p2[et] = ("space", "\n")
+                                    elif "p:" == i.lower()[:2]:
+                                        if i.partition(":")[2].isspace() or not bool(
+                                            i.partition(":")[2]
+                                        ):
+                                            raise Exception("Parent cannot be empty!")
+                                        else:
+                                            p2[et] = (
+                                                "parent",
+                                                i[2:].removeprefix(" "),
+                                            )
+                                    elif i.lower().partition(":")[0] in list(ckc):
+                                        if i.partition(":")[2].isspace():
+                                            p2[et] = (
+                                                ckc[i.partition(":")[0].lower()],
+                                                i.partition(":")[2],
+                                            )
+                                        elif bool(i.partition(":")[2]):
+                                            p2[et] = (
+                                                ckc[i.partition(":")[0].lower()],
+                                                i.partition(":")[2].removeprefix(" "),
+                                            )
+                                if len(ed) != len(p2):
+                                    raise Exception("Not Editable!")
+                                with tv(self.filename) as tvg:
                                     combi = iter(
-                                        (dict(tvg.insighttree()) | p2[0]).values()
+                                        (dict(tvg.insighttree()) | p2).values()
                                     )
                                     tvg.fileread(combi)
-                                    del combi
-                            del tvg, p2
-                        del stor
+                                del tvg, et, ed, ckc, p2, combi
+                        else:
+                            ed = tuple(i for i in self.store[:-1].split("\n") if i)
+                            et = -1
+                            ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
+                            p2 = {}
+                            for i in ed:
+                                et += 1
+                                if "s:" == i.lower()[:2]:
+                                    p2[et] = ("space", "\n")
+                                elif "p:" == i.lower()[:2]:
+                                    if i.partition(":")[2].isspace() or not bool(
+                                        i.partition(":")[2]
+                                    ):
+                                        raise Exception("Parent cannot be empty!")
+                                    else:
+                                        p2[et] = ("parent", i[2:].removeprefix(" "))
+                                elif i.lower().partition(":")[0] in list(ckc):
+                                    if i.partition(":")[2].isspace():
+                                        p2[et] = (
+                                            ckc[i.partition(":")[0].lower()],
+                                            i.partition(":")[2],
+                                        )
+                                    elif bool(i.partition(":")[2]):
+                                        p2[et] = (
+                                            ckc[i.partition(":")[0].lower()],
+                                            i.partition(":")[2].removeprefix(" "),
+                                        )
+                            if len(ed) != len(p2):
+                                raise Exception("Not Editable!")
+                            with tv(self.filename) as tvg:
+                                tvg.fileread(iter(p2.values()))
+                            del tvg, ed, et, ckc, p2
+                        self.store = None
                         self.text.config(state=DISABLED)
                         self.disab(dis=False)
                         self.spaces()
                         if self.editorsel:
                             self.text.see(f"{self.editorsel[0]}.0")
                             self.editorsel = None
                     else:
@@ -2644,14 +2697,15 @@
                         self.spaces()
                         if self.editorsel:
                             self.editorsel = None
                 except Exception as a:
                     messagebox.showerror("TreeViewGui", f"{a}", parent=self.root)
                 if self.text.cget("state") == DISABLED:
                     self._mdbuttons()
+            self.store = None
             self.text.edit_reset()
             self.infobar()
 
     def tvgexit(self, event=None):
         """Exit mode for TVG and setting everything back to default"""
 
         if self.FREEZE is False:
```

### Comparing `FreeTVG-karjakak-3.2.8/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.2.8rc1/TVG/Tutorial TVG.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -29,24 +29,24 @@
 if child, you can choose which position of child
 you want to put under parent.
 Ctrl + B
 
 = BackUp button
 
 Backing up the file.
-
-Max 10.
+Max 10.
 When reach 10, the next one will replace the
 oldest one.
 Ctrl + L
 
 = Load button
 
 Load backup file.
-Write a number that represent the position of a
+
+Write a number that represent the position of a
 backup file.
 Ctrl + D
 
 = Delete button
 
 Delete a row on the text window.
 Choose a row in list box first.
@@ -58,134 +58,104 @@
 Choose a child in child box first and choose a child
 row in list box.
 if smaller to the left, and if bigger to the right.
 Ctrl + S
 
 = Insight button
 
-Will show you exactly which row that represent the
-text in text window.
+Will show you exactly which row that represent the text
+in text window.
 When rows created many, is advise to use Insight.
 Ctrl + U
 
 = Up button
 
-To move a row up that chosen on the list box up to the
+To move a row up that chosen on the list box up to the
 next row by 1
 If you want to move few more, just keep pressing
 [Control+u].
 Ctrl + O
 
 = Down button
 
-To move a row down that chosen on the list box down
-to the next row by 1.
+To move a row down that chosen on the list box down to
+the next row by 1.
 Ctrl + P
 
 = Printing button
 
 Can save as pdf in printing mode in browser.
 The font that you choose in TVG will implement on
 the html [not all font is applicable].
-Ctrl + H
+
+Ctrl + H
 
 = Hide Parent button
 
 To hide any parent row and all it's child rows in reverse
 mode (selected parents are not hid).
 Just display mode in TVG for send note and printing
 purpose.
-A json file is created for remembering the rows
-that are hidden.
+A json file is created for remembering the rows that
+are hidden.
 As long as the json file is not deleted, most
 functions are locked [unable to edit].
 Ctrl + A
 
 = radios button (parent, child)
 
 Switching between Parent and Child radio button for
 positioning.
-
-Ctrl + E
+Ctrl + E
 
 = Paste button
 
-Choose a row and paste the words to entry box to be
-fix.
+Choose a row and paste the words to entry box to be fix.
 Press
 Ctrl + Y
 
 Ctrl + W
 
 to write back to its position.
 
 = Checked button
 
 To give checked mark (for finished a task).
 WARNING:
-Not all computer has same encoding system; if
-it's not 'utf-8', the Checked button will print
-'Done' instead.
+Not all computer has same encoding system; if it's
+not 'utf-8', the Checked button will print 'Done'
+instead.
 Ctrl + 0
 
 = Arrange button
 
 The function mostly used on background for arranging
 display.
-Helpful for clearing chosen higlighted row in list
-box.
+Helpful for clearing chosen higlighted row in list box.
 Helpful for avoiding any mistaken editing.
-Ctrl + -
+
+Ctrl + -
 
 = Clear Hide
 
 Unhide collections of hidden parent one at a time.
 Can delete the whole json file so that all hidden
 appear at once.
-Win
-
-Ctrl + Left
-
-/
-
-Ctrl + Right
-
-/
-
-Ctrl + Up
-
-/
-
-Ctrl + Down
-
-|| Mac
-
-Ctrl + Shift + Left
-
-Ctrl + Shift + Up
-
-/
-
-/
-
-Ctrl + Shift + Right
-
-/
-
-Ctrl + Shift + Down
-
+Win Ctrl + Left / Ctrl + Right / Ctrl + Up / Ctrl + Down ||
+Mac Ctrl + Shift + Left / Ctrl + Shift + Right /
+Ctrl + Shift + Up / Ctrl + Shift + Down
 To move the app windows to user's liking position.
 Shift + Up
 
 /
 
 Shift + Down
 
-To scrolling up and down the text window and list box
-at the same time.
+To scrolling up and down the text window and list box at
+the same time.
 Win
 
 Ctrl + N
 
 || Mac
 
 Cmd + N
@@ -229,47 +199,43 @@
 Ctrl + 7
 
 = Editor
 
 To be able write and edit on the big screen of TVG.
 Need to use formats that will apply for editing.
 For how to use Editor visit for tutorials.
-Editor now can write at any row that has been selected
-Select any row before Editor Mode begin
 Ctrl + 9
 
 = Un/Wrap
 
 Wrapping or Unwrapping the tvg text note for better
 viewing on long sentences.
 Ctrl + [
 
 = Ex
 
 To convert the tvg text note to editor's format for easy
 editing.
-
-Usually for long rows is adviceable.
-Can choose a parent only, and edited all with its child
-in editor mode.
+Usually for long rows is adviceable.
+Can choose a parent only, and edited all with its child in
+editor mode.
 TAKE NOTE:
 Do backup in case want to revert back.
 Ctrl + ]
 
 = Template
 
-For saving collections of often use format in Editor
-mode.
-Can load back in Editor mode to be use againandagain.
+For saving collections of often use format in Editor mode.
+
+Can load back in Editor mode to be use againandagain.
 Ctrl + ,
 
 = Select font style
 
-Change font style on TVG screen and the listbox as
-well.
+Change font style on TVG screen and the listbox as well.
 Ctrl + .
 
 = Select background color
 
 To change color of TVG screen and the listbox as well.
 Ctrl + /
 
@@ -282,30 +248,30 @@
 
 Win
 
 Ctrl + Shift + Z
 
 Shift + Enter
 
-focus
-
 || Mac
 
+= Undo in Editor Mode.
+
 Cmd + Z
 
 || Mac
 
-= Undo in Editor Mode.
 Cmd + Y
 
 = Redo in Editor Mode.
 
 = To invoke buttons and radios call while in
 
-Press tab to run over the focus.
+focus
+Press tab to run over the focus.
 Ctrl + F1
 
 = Call TVG tutorial pdf
 
 The pdf will open in default browser.
 Ctrl + F2
 
@@ -320,29 +286,28 @@
 
 Sending the text by mail.
 Or copied formatted text for sending with chat app.
 Ctrl + Shift + F
 
 = Fold all childs
 
-All childs are folded.
+All childs are folded.
 Ctrl + Shift + S
 
 = Fold selected childs
 
 Only selected childs are folded.
 Folded childs are retain even after changing file.
 Ctrl + Shift + U
 
 = Unfolded all childs
 
 All childs are unfolded
 Add-On TVG:
-
-Ctrl + 1
+Ctrl + 1
 
 = Sum-Up Function
 
 Summing up all parent with sign "+"
 Every each parent will has addition child that state
 "TOTAL ..." sum
 Ctrl + 4
@@ -355,31 +320,31 @@
 = Del-Total
 
 Clear all sums "TOTAL ..."
 Ctrl + F4
 
 /
 
-= Expression Calculator
-
 Fn + F4
 
+= Expression Calculator
+
 Simple calculator
-The paste button formating the numbers and insert
-to the editor at the end of a row's line
+The paste button formating the numbers and insert to
+the editor at the end of a row's line
 Markdown shortcuts:
 Ctrl + Shift + 1
 
 = Bold
 
 Ctrl + Shift + 2
 
 = Italic
 
-Ctrl + Shift + 3
+Ctrl + Shift + 3
 
 = Underline
 
 Ctrl + Shift + 4
 
 = Strikethrough
 
@@ -387,40 +352,40 @@
 
 = Mark Highlight
 
 Ctrl + Shift + 6
 
 =
 
+Ctrl + Shift + 7
+
+= TVG link
+
+Ctrl + Shift + 8
+
+= superscript
+
+Ctrl + Shift + 9
+
+= subscript
+
 S
 
 P
 
 E
 
 C
 
 I
 
 A
 
 L
 
-Ctrl + Shift + 7
-
-= TVG link
-
-Ctrl + Shift + 8
-
-= superscript
-
-Ctrl + Shift + 9
-
-= subscript
-
 = Checked markdown that can be checkedoff by clicking on the check-box in html
 Ctrl + Shift + 0
 
 Win
 
 Ctrl + Shift + Q
 
@@ -464,20 +429,20 @@
 Select massively with Shift key and select or
 unselect individually with Ctrl key.
 
 With multiple, selection or unselect individually one by
 one (not massively).
 unreverse = For Hidden selection mode
 By default is reverse selection.
-Selected parents are not hid, and unselected ones
-are hid.
+Selected parents are not hid, and unselected ones are
+hid.
 With unreverse, only selected parents hid.
 word = For Wrap
 By default words text are not wrapped.
 With word, words text are wrapped from beginning.
 Can use Wrap function to unwrapped.
 on = For Checked
 By default will insert ✔ or >>[DONE]<<.
-With on will insert checked-box [x] at beginning of a
-text line.
+With on will insert checked-box [x] at beginning of a text
+line.
```

### Comparing `FreeTVG-karjakak-3.2.8/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.8rc1/TVG/structure/frame_layouts.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.8rc1/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.8rc1/TVG/utility/mdh.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,44 +28,14 @@
     "pymdownx.keys": {"strict": True},
     "pymdownx.tasklist": {
         "clickable_checkbox": True,
     },
 }
 
 
-def _pattern(wrd: str, pat: str):
-    try:
-        last = g = fx = pt = None
-        if "<p>" not in wrd:
-            last = -5
-        else:
-            last = -4
-        g = wrd.partition(pat)
-        g = g[0] + g[1]
-        pt = (
-            '<input type="checkbox" class="strikethrough" name="ck"/><span for="ck">'
-            if not "checked" in pat
-            else '<input type="checkbox" class="strikethrough" name="ck" checked/><span for="ck">'
-        )
-        fx = (
-            wrd[: len(g)]
-            + "<span>"
-            + wrd[len(g) : last]
-            + "</span>"
-            + wrd[last:]
-            + "\n"
-        ).replace(
-            f"{pat}<span>",
-            pt,
-        )
-        return fx
-    finally:
-        del last, g, fx, pt, wrd, pat
-
-
 def convhtml(
     text: str,
     filename: str,
     font: str,
     bg: str = None,
     fg: str = None,
     preview: bool = True,
@@ -179,39 +149,76 @@
 </html>
 """
 
         cssstyle = cssstyle + printed + nxt
         fcs = []
         if 'input type="checkbox"' in cssstyle:
             for i in cssstyle.split("\n"):
-                if '<input type="checkbox" checked/>' in i:
-                    fcs.append(_pattern(i, '<input type="checkbox" checked/>'))
-                elif '<input type="checkbox"/>' in i:
-                    fcs.append(_pattern(i, '<input type="checkbox"/>'))
+                if '<p><input type="checkbox"/>' in i:
+                    g = '<p><input type="checkbox"/>'
+                    fx = (
+                        i[: len(g)]
+                        + "<span>"
+                        + i[len(g) : -4]
+                        + "</span>"
+                        + i[-4:]
+                        + "\n"
+                    )
+                    fx = fx.replace(
+                        g + "<span>",
+                        '<p><input type="checkbox" class="strikethrough" name="ck"/><span for="ck">',
+                    )
+                    fcs.append(fx)
+                    del g, fx
+                elif '<p><input type="checkbox" checked/>' in i:
+                    g = '<p><input type="checkbox" checked/>'
+                    fx = (
+                        i[: len(g)]
+                        + "<span>"
+                        + i[len(g) : -4]
+                        + "</span>"
+                        + i[-4:]
+                        + "\n"
+                    )
+                    fx = fx.replace(
+                        g + "<span>",
+                        '<p><input type="checkbox" class="strikethrough" name="ck" checked/><span for="ck">',
+                    )
+                    fcs.append(fx)
+                    del g, fx
                 else:
                     fcs.append(f"{i}\n")
 
         if fcs:
             cssstyle = "".join(fcs)
         del fcs
         with open(f"{filename}.html", "w") as whtm:
             whtm.write(cssstyle)
         pro = None
         if platform.startswith("win"):
-            # ToDo: Preview for arm64 architecture
-            # In preview no interactive printing even it open on browser
-            pro = [
-                "powershell.exe",
-                "start",
-                "msedge",
-                f"'\"{Path(f'{filename}.html').absolute()}\"'",
-            ]
-            startupinfo = subprocess.STARTUPINFO()
-            startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-            subprocess.run(pro, startupinfo=startupinfo)
+            if preview:
+                window = webview.create_window(
+                    "TVG",
+                    html=cssstyle,
+                    resizable=False,
+                    width=width if width else 800,
+                    height=height if height else 600,
+                    on_top=True,
+                )
+                webview.start(gui="mshtml")
+            else:
+                pro = [
+                    "powershell.exe",
+                    "start",
+                    "msedge",
+                    f"'\"{Path(f'{filename}.html').absolute()}\"'",
+                ]
+                startupinfo = subprocess.STARTUPINFO()
+                startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+                subprocess.run(pro, startupinfo=startupinfo)
         else:
             if preview:
                 window = webview.create_window(
                     "TVG",
                     html=cssstyle,
                     resizable=False,
                     width=width if width else 800,
```

### Comparing `FreeTVG-karjakak-3.2.8/setup.cfg` & `FreeTVG-karjakak-3.2.8rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.8
+version = 3.2.8rc1
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
```

