# Comparing `tmp/doFolder-0.0.1.tar.gz` & `tmp/doFolder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.1.tar", last modified: Mon May 22 13:38:30 2023, max compression
+gzip compressed data, was "doFolder-0.0.2.tar", last modified: Thu May 25 15:23:20 2023, max compression
```

## Comparing `doFolder-0.0.1.tar` & `doFolder-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 13:38:30.271960 doFolder-0.0.1/
--rw-rw-rw-   0        0        0     3213 2023-05-22 13:38:30.269959 doFolder-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2521 2023-05-22 13:21:30.000000 doFolder-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-22 13:38:30.263960 doFolder-0.0.1/doFolder/
--rw-rw-rw-   0        0        0    16922 2023-05-22 12:46:47.000000 doFolder-0.0.1/doFolder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:38:30.268962 doFolder-0.0.1/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3213 2023-05-22 13:38:30.000000 doFolder-0.0.1/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-22 13:38:30.000000 doFolder-0.0.1/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 13:38:30.000000 doFolder-0.0.1/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 13:38:30.000000 doFolder-0.0.1/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 13:38:30.000000 doFolder-0.0.1/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 13:38:30.271960 doFolder-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-05-22 13:37:48.000000 doFolder-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:23:20.874165 doFolder-0.0.2/
+-rw-rw-rw-   0        0        0     3132 2023-05-25 15:23:20.874165 doFolder-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2440 2023-05-25 15:16:05.000000 doFolder-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 15:23:20.865164 doFolder-0.0.2/doFolder/
+-rw-rw-rw-   0        0        0       63 2023-05-25 15:20:42.000000 doFolder-0.0.2/doFolder/__init__.py
+-rw-rw-rw-   0        0        0     8382 2023-05-25 15:18:43.000000 doFolder-0.0.2/doFolder/compare.py
+-rw-rw-rw-   0        0        0    17480 2023-05-25 14:42:53.000000 doFolder-0.0.2/doFolder/main.py
+-rw-rw-rw-   0        0        0    13042 2023-05-25 15:18:16.000000 doFolder-0.0.2/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:23:20.873165 doFolder-0.0.2/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3132 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 15:23:20.000000 doFolder-0.0.2/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:23:20.874165 doFolder-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2023-05-25 15:16:41.000000 doFolder-0.0.2/setup.py
```

### Comparing `doFolder-0.0.1/PKG-INFO` & `doFolder-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.1
+Version: 0.0.2
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -17,17 +17,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 
 文件夹管理(doFolder)
 ====================
 
-::
+.. code:: bash
 
-   pip install import doFolder
+   pip install doFolder
 
 使用方法
 --------
 
 导入
 ~~~~
 
@@ -40,16 +40,16 @@
 
 -  ``Folder`` 指一个文件夹
 
    -  *参数* ``path`` 文件夹路径:``str|doFolder.Path``
    -  *参数* ``onlisten`` 是否监听比同步文件夹变动:``bool``
    -  *属性* ``files`` 文件夹中的文件列表:``FileList``
    -  *属性* ``subfolder`` 文件夹中的子文件夹:``FolderList``
-   -  *方法* ``hasFolder,hasFile``
-      是否包括某个文件/文件夹,参数为\ ``str``\ 时默认匹配\ ``.name``\ 属性
+   -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
+      ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
       -  *参数* ``condition`` 搜索条件:``List[UnformattedMatching]``
       -  *参数* ``aim`` 目标: ``"file"|"folder"|"both"``
       -  *返回* 搜索结果:``SearchResult``
 
@@ -62,33 +62,46 @@
 -  ``Path`` 指一个路径
 
    -  *参数* ``path`` 路径(绝对或相对):``str``
    -  *属性* ``partition`` 将路径(不包含驱动器)切片
    -  *方法* ``add`` 将内容加载路径后面
    -  *方法* ``findRest`` 去除两个路径的共同部分
 
--  ``FolderList,FileList`` 模拟列表
+-  ``compare``\ 提供比较文件夹的API
 
-   -  支持遍历,用index(``str``\ 或\ ``int``)获取值
-   -  in 运算符可以针对\ ``str``\ 使用，代表匹配\ ``.name``\ 属性
+   -  *函数* ``compare`` 比较两个文件夹
 
--  ``UnformattedMatching`` 搜索条件,可能的类型和意义如下
+      -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
+      -  *参数* ``compareContent`` 文件内容的比较方法
 
-   -  ``str`` 表示完全匹配文件名/文件夹名
-   -  ``re.Pattern`` 用正则表达式匹配文件名/文件夹名
-   -  ``Callable[[Union["File","Folder"]],bool]`` 自定义匹配函数
-   -  ``FormattedMatching`` 意义如下所示
+         -  ``ignore`` 忽略文件内容
+         -  ``hash`` 比较文件哈希值
+         -  ``content`` 比较文件内容
+         -  ``size`` 比较文件大小
 
--  ``FormattedMatching`` 针对\ ``UnformattedMatching``\ 归一化的结果
-   类型为\ ``Tuple``,长度为3
+      -  *返回* 比较结果:``CompareResult``
 
-   1. ``Callable[[Union["File","Folder"]],bool]`` 匹配函数
-   2. ``int`` 最小重复次数(默认1)
-   3. ``int|None`` 最大重复次数|正无穷(默认为1) ## 关于作者
+命令行使用
+~~~~~~~~~~
+
+.. code:: bash
+
+   compare Folder1 Folder2 [-c ignore|hash|content|size]
+
+具体作用参见
+
+.. code:: bash
+
+   compare -h
+
+关于作者
+--------
 
 作者主页\ `宽宽2007 <https://kuankuan2007.gitee.io>`__
 
 本项目在\ `苟浩铭/文件夹管理
 (gitee.com) <https://gitee.com/kuankuan2007/do-folder>`__\ 上开源
 
 帮助文档参见\ `宽宽的帮助文档
 (gitee.io) <https://kuankuan2007.gitee.io/docs/do-folder/>`__
+
+pypi官网项目地址\ `Pypi <https://pypi.org/project/doFolder/>`__
```

### Comparing `doFolder-0.0.1/README.rst` & `doFolder-0.0.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 文件夹管理(doFolder)
 ====================
 
-::
+.. code:: bash
 
-   pip install import doFolder
+   pip install doFolder
 
 使用方法
 --------
 
 导入
 ~~~~
 
@@ -20,16 +20,16 @@
 
 -  ``Folder`` 指一个文件夹
 
    -  *参数* ``path`` 文件夹路径:``str|doFolder.Path``
    -  *参数* ``onlisten`` 是否监听比同步文件夹变动:``bool``
    -  *属性* ``files`` 文件夹中的文件列表:``FileList``
    -  *属性* ``subfolder`` 文件夹中的子文件夹:``FolderList``
-   -  *方法* ``hasFolder,hasFile``
-      是否包括某个文件/文件夹,参数为\ ``str``\ 时默认匹配\ ``.name``\ 属性
+   -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
+      ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
       -  *参数* ``condition`` 搜索条件:``List[UnformattedMatching]``
       -  *参数* ``aim`` 目标: ``"file"|"folder"|"both"``
       -  *返回* 搜索结果:``SearchResult``
 
@@ -42,33 +42,46 @@
 -  ``Path`` 指一个路径
 
    -  *参数* ``path`` 路径(绝对或相对):``str``
    -  *属性* ``partition`` 将路径(不包含驱动器)切片
    -  *方法* ``add`` 将内容加载路径后面
    -  *方法* ``findRest`` 去除两个路径的共同部分
 
--  ``FolderList,FileList`` 模拟列表
+-  ``compare``\ 提供比较文件夹的API
 
-   -  支持遍历,用index(``str``\ 或\ ``int``)获取值
-   -  in 运算符可以针对\ ``str``\ 使用，代表匹配\ ``.name``\ 属性
+   -  *函数* ``compare`` 比较两个文件夹
 
--  ``UnformattedMatching`` 搜索条件,可能的类型和意义如下
+      -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
+      -  *参数* ``compareContent`` 文件内容的比较方法
 
-   -  ``str`` 表示完全匹配文件名/文件夹名
-   -  ``re.Pattern`` 用正则表达式匹配文件名/文件夹名
-   -  ``Callable[[Union["File","Folder"]],bool]`` 自定义匹配函数
-   -  ``FormattedMatching`` 意义如下所示
+         -  ``ignore`` 忽略文件内容
+         -  ``hash`` 比较文件哈希值
+         -  ``content`` 比较文件内容
+         -  ``size`` 比较文件大小
 
--  ``FormattedMatching`` 针对\ ``UnformattedMatching``\ 归一化的结果
-   类型为\ ``Tuple``,长度为3
+      -  *返回* 比较结果:``CompareResult``
 
-   1. ``Callable[[Union["File","Folder"]],bool]`` 匹配函数
-   2. ``int`` 最小重复次数(默认1)
-   3. ``int|None`` 最大重复次数|正无穷(默认为1) ## 关于作者
+命令行使用
+~~~~~~~~~~
+
+.. code:: bash
+
+   compare Folder1 Folder2 [-c ignore|hash|content|size]
+
+具体作用参见
+
+.. code:: bash
+
+   compare -h
+
+关于作者
+--------
 
 作者主页\ `宽宽2007 <https://kuankuan2007.gitee.io>`__
 
 本项目在\ `苟浩铭/文件夹管理
 (gitee.com) <https://gitee.com/kuankuan2007/do-folder>`__\ 上开源
 
 帮助文档参见\ `宽宽的帮助文档
 (gitee.io) <https://kuankuan2007.gitee.io/docs/do-folder/>`__
+
+pypi官网项目地址\ `Pypi <https://pypi.org/project/doFolder/>`__
```

### Comparing `doFolder-0.0.1/doFolder/__init__.py` & `doFolder-0.0.2/doFolder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import re
 from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,Protocol
 import shutil
 import copy
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler,FileSystemEvent,FileSystemMovedEvent,EVENT_TYPE_CREATED,EVENT_TYPE_DELETED,EVENT_TYPE_MOVED,EVENT_TYPE_MODIFIED
+import hashlib
+
+__all__=["File","Folder","Path"]
+
 pathTester=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)/(?:[^/\\\*\?]+/?)*$")
 driverFinder=re.compile(r"^((?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+))/(?:[^/\\\*\?]+/?)*$")
 pathFinder=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)(/(?:[^/\\\*\?]+/?)*)$")
 SearchCondition=Union[str,re.Pattern[str],Callable[[Union["File","Folder"]],bool]]
 FormatedMatching=Tuple[Callable[[Union["File","Folder"]],bool],int,Union[int,None]]
 UnformattedMatching=Union[SearchCondition,Tuple[SearchCondition,int,Union[int,None]]]
 _T=TypeVar("_T",bound="_HasName")
@@ -77,23 +81,23 @@
     def __contains__(self,var:_T|str)->bool:
         if var in self.values :
             return True
         for i in range(len(self.values)):
             if  self.values[i].name == var:
                 return True
         return False
-    def __getitem__(self,key:Union[int,str],e:_U)->Union[_T,_U]:
+    def __getitem__(self,key:Union[int,str])->Union[_T,None]:
         if type(key)==str:
             for i in self.values:
                 if i.name == key:
                     return i
-            return e
+            return None
         elif type(key)==int:
             return  self.values[key]
-        return e
+        return None
     def __getattribute__(self,key:str)->Any:
         try:
             return super().__getattribute__(key)
         except AttributeError:
             for i in self.values:
                 if i.name == key:
                     return i
@@ -132,25 +136,31 @@
         super().__init__()
         self.driver:str=driverFinder.findall(self)[0]
         self.path:str=pathFinder.findall(self)[0]
     @property
     def partition(self)->List[str]:
         """split the path into list"""
         li=self.path.split("/")
-        li.remove("")
+        while "" in li:
+            li.remove("")
         return li
     @property
     def name(self)->str:
         """The name of the path points to"""
         return self.partition[-1]
     def add(self, value:str):
         """add another dir name after the path"""
         if self[-1]!="/":
             return Path(self+"/"+value)
         return Path(self+value)
+    def adds(self, value:List[str])->"Path":
+        new=copy.deepcopy(self)
+        for i in value:
+            new=new.add(i)
+        return new
     def findRest(self,other:"Path",error:Literal["strict","ignore"]="strict"):
         """Find the same ancestor node of them
         :param error:"strict" means if other path not exactly the parent directory of this path, raise ValueError.
         """
         if error=="strict" and self.driver!=other.driver:
             raise ValueError(f"\"{self}\" and \"{other}\" has different driver")
         retsult=copy.deepcopy(self.partition)
@@ -178,24 +188,35 @@
         self.dev=state.st_dev
         self.uid=state.st_uid
         self.gid=state.st_gid
         self.size=state.st_size
         self.mtime=state.st_mtime
         self.ctime=state.st_ctime
         self.atime=state.st_atime
+        self._hash:Union[None,str]=None
     @property
     def name(self)->str:
         return self.path.name
     def open(self,*args,**kw):
         """open the file by function open"""
         return open(self.path,*args,**kw)
     def __str__(self)->str:
         return f"<File \"{self.name}\">"
     def __repr__(self) -> str:
         return f"<File \"{self.name}\">"
+    @property
+    def content(self)->bytes:
+        with self.open("rb") as f:
+            return f.read()
+    @property
+    def hash(self)->str:
+        if self._hash:
+            return self._hash
+        self._hash=hashlib.md5(self.content).hexdigest()
+        return self._hash
     def remove(self):
         os.remove(self.path)
     def copy(self,path:str):
         shutil.copy(self.path,path)
     def move(self,path:str):
         shutil.move(self.path,path)
 class Folder(_HasName):
@@ -225,15 +246,15 @@
                 self.subfolder.append(Folder(newPath,parent=self))
     @property
     def name(self)->str:
         return self.path.name
     def __str__(self)->str:
         return f"<Folder \"{self.name}\">"
     def __repr__(self) -> str:
-        return f"<Folder \"{self.name}\">"
+        return self.__str__()
     def __contains__(self,item:Union[str,"Folder","File"]) -> bool:
         if type(item)==str:
             return item in self.dir
         elif type(item)==Folder:
             return item in self.subfolder
         elif type(item)==File:
             return item in self.files
```

### Comparing `doFolder-0.0.1/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.2/doFolder.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.1
+Version: 0.0.2
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -17,17 +17,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 
 文件夹管理(doFolder)
 ====================
 
-::
+.. code:: bash
 
-   pip install import doFolder
+   pip install doFolder
 
 使用方法
 --------
 
 导入
 ~~~~
 
@@ -40,16 +40,16 @@
 
 -  ``Folder`` 指一个文件夹
 
    -  *参数* ``path`` 文件夹路径:``str|doFolder.Path``
    -  *参数* ``onlisten`` 是否监听比同步文件夹变动:``bool``
    -  *属性* ``files`` 文件夹中的文件列表:``FileList``
    -  *属性* ``subfolder`` 文件夹中的子文件夹:``FolderList``
-   -  *方法* ``hasFolder,hasFile``
-      是否包括某个文件/文件夹,参数为\ ``str``\ 时默认匹配\ ``.name``\ 属性
+   -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
+      ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
       -  *参数* ``condition`` 搜索条件:``List[UnformattedMatching]``
       -  *参数* ``aim`` 目标: ``"file"|"folder"|"both"``
       -  *返回* 搜索结果:``SearchResult``
 
@@ -62,33 +62,46 @@
 -  ``Path`` 指一个路径
 
    -  *参数* ``path`` 路径(绝对或相对):``str``
    -  *属性* ``partition`` 将路径(不包含驱动器)切片
    -  *方法* ``add`` 将内容加载路径后面
    -  *方法* ``findRest`` 去除两个路径的共同部分
 
--  ``FolderList,FileList`` 模拟列表
+-  ``compare``\ 提供比较文件夹的API
 
-   -  支持遍历,用index(``str``\ 或\ ``int``)获取值
-   -  in 运算符可以针对\ ``str``\ 使用，代表匹配\ ``.name``\ 属性
+   -  *函数* ``compare`` 比较两个文件夹
 
--  ``UnformattedMatching`` 搜索条件,可能的类型和意义如下
+      -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
+      -  *参数* ``compareContent`` 文件内容的比较方法
 
-   -  ``str`` 表示完全匹配文件名/文件夹名
-   -  ``re.Pattern`` 用正则表达式匹配文件名/文件夹名
-   -  ``Callable[[Union["File","Folder"]],bool]`` 自定义匹配函数
-   -  ``FormattedMatching`` 意义如下所示
+         -  ``ignore`` 忽略文件内容
+         -  ``hash`` 比较文件哈希值
+         -  ``content`` 比较文件内容
+         -  ``size`` 比较文件大小
 
--  ``FormattedMatching`` 针对\ ``UnformattedMatching``\ 归一化的结果
-   类型为\ ``Tuple``,长度为3
+      -  *返回* 比较结果:``CompareResult``
 
-   1. ``Callable[[Union["File","Folder"]],bool]`` 匹配函数
-   2. ``int`` 最小重复次数(默认1)
-   3. ``int|None`` 最大重复次数|正无穷(默认为1) ## 关于作者
+命令行使用
+~~~~~~~~~~
+
+.. code:: bash
+
+   compare Folder1 Folder2 [-c ignore|hash|content|size]
+
+具体作用参见
+
+.. code:: bash
+
+   compare -h
+
+关于作者
+--------
 
 作者主页\ `宽宽2007 <https://kuankuan2007.gitee.io>`__
 
 本项目在\ `苟浩铭/文件夹管理
 (gitee.com) <https://gitee.com/kuankuan2007/do-folder>`__\ 上开源
 
 帮助文档参见\ `宽宽的帮助文档
 (gitee.io) <https://kuankuan2007.gitee.io/docs/do-folder/>`__
+
+pypi官网项目地址\ `Pypi <https://pypi.org/project/doFolder/>`__
```

