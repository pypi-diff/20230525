# Comparing `tmp/s27a_jbq-1.0.1.tar.gz` & `tmp/s27a_jbq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s27a_jbq-1.0.1.tar", last modified: Sat May 20 13:07:16 2023, max compression
+gzip compressed data, was "s27a_jbq-1.0.2.tar", last modified: Thu May 25 12:45:15 2023, max compression
```

## Comparing `s27a_jbq-1.0.1.tar` & `s27a_jbq-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.835660 s27a_jbq-1.0.1/
--rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    11714 2023-05-20 13:07:16.835660 s27a_jbq-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11197 2023-05-20 10:36:24.000000 s27a_jbq-1.0.1/README.md
--rw-rw-rw-   0        0        0      597 2023-05-18 13:05:59.000000 s27a_jbq-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 13:07:16.837428 s27a_jbq-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.796029 s27a_jbq-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.817998 s27a_jbq-1.0.1/src/s27a_jbq/
--rw-rw-rw-   0        0        0      225 2023-05-20 12:22:46.000000 s27a_jbq-1.0.1/src/s27a_jbq/__constants__.py
--rw-rw-rw-   0        0        0      719 2023-05-20 12:21:22.000000 s27a_jbq-1.0.1/src/s27a_jbq/__init__.py
--rw-rw-rw-   0        0        0     3970 2023-05-16 13:59:35.000000 s27a_jbq-1.0.1/src/s27a_jbq/extension.py
--rw-rw-rw-   0        0        0    10275 2023-05-20 13:04:44.000000 s27a_jbq-1.0.1/src/s27a_jbq/game.py
--rw-rw-rw-   0        0        0     6379 2023-05-20 09:57:48.000000 s27a_jbq-1.0.1/src/s27a_jbq/map.py
--rw-rw-rw-   0        0        0     6817 2023-05-20 12:52:08.000000 s27a_jbq-1.0.1/src/s27a_jbq/static.py
--rw-rw-rw-   0        0        0    14907 2023-05-20 12:52:02.000000 s27a_jbq-1.0.1/src/s27a_jbq/window.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.832037 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/
--rw-rw-rw-   0        0        0    11714 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.573660 s27a_jbq-1.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    11851 2023-05-25 12:45:15.573660 s27a_jbq-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11334 2023-05-24 11:17:11.000000 s27a_jbq-1.0.2/README.md
+-rw-rw-rw-   0        0        0      597 2023-05-23 12:26:37.000000 s27a_jbq-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:45:15.581166 s27a_jbq-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.526142 s27a_jbq-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.561578 s27a_jbq-1.0.2/src/s27a_jbq/
+-rw-rw-rw-   0        0        0      177 2023-05-24 12:28:15.000000 s27a_jbq-1.0.2/src/s27a_jbq/__constants__.py
+-rw-rw-rw-   0        0        0       87 2023-05-24 13:02:51.000000 s27a_jbq-1.0.2/src/s27a_jbq/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-05-24 11:40:26.000000 s27a_jbq-1.0.2/src/s27a_jbq/__main__.py
+-rw-rw-rw-   0        0        0     3970 2023-05-16 13:59:35.000000 s27a_jbq-1.0.2/src/s27a_jbq/extension.py
+-rw-rw-rw-   0        0        0    10421 2023-05-22 12:26:11.000000 s27a_jbq-1.0.2/src/s27a_jbq/game.py
+-rw-rw-rw-   0        0        0     6599 2023-05-24 12:00:48.000000 s27a_jbq-1.0.2/src/s27a_jbq/map.py
+-rw-rw-rw-   0        0        0     6870 2023-05-24 12:24:33.000000 s27a_jbq-1.0.2/src/s27a_jbq/static.py
+-rw-rw-rw-   0        0        0    16681 2023-05-24 13:03:58.000000 s27a_jbq-1.0.2/src/s27a_jbq/window.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.573660 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/
+-rw-rw-rw-   0        0        0    11851 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/top_level.txt
```

### Comparing `s27a_jbq-1.0.1/LICENSE` & `s27a_jbq-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s27a_jbq-1.0.1/PKG-INFO` & `s27a_jbq-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: s27a_jbq
-Version: 1.0.1
+Version: 1.0.2
 Summary: A board game with high degrees of freedom
 Author-email: amf <xyf081202@163.com>
 Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
 Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.1-blue)
+![](https://img.shields.io/badge/release-1.0.2-blue)
 ![](https://img.shields.io/badge/last%20commit-may-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
 精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
@@ -32,61 +32,71 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您可以从[这里](https://github.com/amf14151/s27a_jbq/archive/refs/heads/main.zip)直接下载文件并自行安装，或使用以下指令来安装
+您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包，也可以按照下面的步骤安装模块并使用
+
+## 安装模块
+
+*若想通过模块的方式运行精班棋，您需要Python解释器*
+
+使用以下命令来安装模块
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装`s27a_jbq`模块后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
+在安装`s27a_jbq`模块后，使用以下命令来构建游戏文件夹
 
-``` python
-from s27a_jbq import generate_game
+```
+python.exe -m s27a_jbq generate_game {游戏文件夹路径} {游戏运行方式}
+```
+
+其中，游戏运行方式有以下选择：
+
+- `window`：窗口模式
 
-generate_game(
-   game_path = "JBQ", # 游戏文件夹位置
-   record_path = None, # 棋局记录位置，格式为.csv，使用相对路径时根目录为游戏文件夹路径
-   display = "window" # 游戏打开方式，'window'为窗口模式
-)
+示例：
+
+```
+python.exe -m s27a_jbq generate_game C:/JBQ window
 ```
 
+上方的代码在C盘根目录中创建名为`JBQ`的游戏文件夹
+
 您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
 
 ``` python
 from s27a_jbq.game import App
 
 def main():
    app = App()
    app.run()
 ```
 
 在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
-另有`map`文件夹，该文件夹用于存储地图，地图是进行游戏的关键文件
-
 # 使用方法
 
 [(返回目录)](#目录)
 
 ## 游戏过程
 
 在设置好地图及扩展（具体方法请参见下文）后，点击开始游戏即可
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
 
 一些棋子在不同的位置会有不同的可移动格子，每个棋子的具体可移动格子根据地图、扩展决定
 
-在对局结束后，如果设置了`record_path`，则会在文件夹中创建同名文件，格式为`.csv`
+在对局结束后，如果在设置中设置了棋局记录路径，则会对棋局进行记录
 
 ## 地图
 
 地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
 
 地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
@@ -110,33 +120,29 @@
 
 1. 棋盘位置规则
 
    - 单个棋盘位置规则表示为`M[a|b|c]`的形式，其中`M`为规则名，为大写，`a`、`b`、`c`等为参数，为整数，用`|`隔开
    - 可使用的规则名：
      - `X[m|n|...]`，当棋子所在的行数等于任意一个参数（`m`、`n`等）时，该规则的值为`true`，否则为`false`
      - `Y[m|n|...]`，当棋子所在的列数等于任意一个参数（`m`、`n`等）时，该规则的值为`true`，否则为`false`
-     - `P[x|y]`，当棋子所在的位置等于`(x,y)`时，该规则的值为`true`，否则为`false`
+     - `P[x1|y1|x2|y2|...]`，当棋子所在的位置等于`(xn,yn)`时，该规则的值为`true`，否则为`false`
    - 其他规则名返回值为`false`
    - 多个棋盘位置规则间用`&`连接（`&`表示**或**，即棋子位置只要有一项满足该棋盘位置规则则返回值为`true`）
    - 示例：`X[1|-1]&Y[1|-1]`表示棋盘边缘区域
 
 2. 可移动规则
 
    - 该语法规则分为两部分，第一部分为可以向某方向移动一格，第二部分为可以向某方向移动无限格。两部分语法相同，两部分间用`;`隔开
    - 在每一部分中，用`,`分隔开所有可移动方向，这些方向按**左上、上、右上、左、右、左下、下、右下**分别对应1-8
    - 如果这一方向上是否可以移动有位置限制，可以在方向编号后加上`()`，并在内部填入*棋盘位置规则*
    - 在第二部分中出现的可移动方向可以不出现在第一部分中
    - 如果没有第二部分（或第一部分）也需要在后面（或前面）加上`;`
    - 示例：`1(Y[4|5|6]),3(Y[2|3|4]),4(Y[7]),5(Y[1]);2`
 
-棋子表的每一列内容依次是：
-
-```
-编号 名称 归属 首领 可移动 升变条件 升变后可移动
-```
+棋子表的每一列内容依次是`编号`、`名称`、`归属`、`首领`、`可移动`、`升变条件`、`升变后可移动`、`其他`
 
 这些内容必须**按序**排列，具体填写规则如下：
 
 1. 编号
 
    - 每个棋子独立的不同的编号
    - 按照顺序由1递增
@@ -167,14 +173,17 @@
    - 当棋子位置符合升变条件时，其可移动规则永久变为*升变后可移动*
 
 7. 升变后可移动
 
    - 填入*可移动规则*
    - 该角色无法升变时仍需填写`;`
 
+8. 其他
+
+   - 可以有多列，每列标题、填写规则由扩展而定
 
 ### 棋盘表
 
 棋盘表的名称为`map`
 
 棋盘表由两部分组成：棋盘行列数、棋盘布局
```

### Comparing `s27a_jbq-1.0.1/README.md` & `s27a_jbq-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.1-blue)
+![](https://img.shields.io/badge/release-1.0.2-blue)
 ![](https://img.shields.io/badge/last%20commit-may-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
 精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
@@ -18,61 +18,71 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您可以从[这里](https://github.com/amf14151/s27a_jbq/archive/refs/heads/main.zip)直接下载文件并自行安装，或使用以下指令来安装
+您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包，也可以按照下面的步骤安装模块并使用
+
+## 安装模块
+
+*若想通过模块的方式运行精班棋，您需要Python解释器*
+
+使用以下命令来安装模块
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装`s27a_jbq`模块后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
+在安装`s27a_jbq`模块后，使用以下命令来构建游戏文件夹
 
-``` python
-from s27a_jbq import generate_game
+```
+python.exe -m s27a_jbq generate_game {游戏文件夹路径} {游戏运行方式}
+```
+
+其中，游戏运行方式有以下选择：
+
+- `window`：窗口模式
 
-generate_game(
-   game_path = "JBQ", # 游戏文件夹位置
-   record_path = None, # 棋局记录位置，格式为.csv，使用相对路径时根目录为游戏文件夹路径
-   display = "window" # 游戏打开方式，'window'为窗口模式
-)
+示例：
+
+```
+python.exe -m s27a_jbq generate_game C:/JBQ window
 ```
 
+上方的代码在C盘根目录中创建名为`JBQ`的游戏文件夹
+
 您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
 
 ``` python
 from s27a_jbq.game import App
 
 def main():
    app = App()
    app.run()
 ```
 
 在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
-另有`map`文件夹，该文件夹用于存储地图，地图是进行游戏的关键文件
-
 # 使用方法
 
 [(返回目录)](#目录)
 
 ## 游戏过程
 
 在设置好地图及扩展（具体方法请参见下文）后，点击开始游戏即可
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
 
 一些棋子在不同的位置会有不同的可移动格子，每个棋子的具体可移动格子根据地图、扩展决定
 
-在对局结束后，如果设置了`record_path`，则会在文件夹中创建同名文件，格式为`.csv`
+在对局结束后，如果在设置中设置了棋局记录路径，则会对棋局进行记录
 
 ## 地图
 
 地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
 
 地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
@@ -96,33 +106,29 @@
 
 1. 棋盘位置规则
 
    - 单个棋盘位置规则表示为`M[a|b|c]`的形式，其中`M`为规则名，为大写，`a`、`b`、`c`等为参数，为整数，用`|`隔开
    - 可使用的规则名：
      - `X[m|n|...]`，当棋子所在的行数等于任意一个参数（`m`、`n`等）时，该规则的值为`true`，否则为`false`
      - `Y[m|n|...]`，当棋子所在的列数等于任意一个参数（`m`、`n`等）时，该规则的值为`true`，否则为`false`
-     - `P[x|y]`，当棋子所在的位置等于`(x,y)`时，该规则的值为`true`，否则为`false`
+     - `P[x1|y1|x2|y2|...]`，当棋子所在的位置等于`(xn,yn)`时，该规则的值为`true`，否则为`false`
    - 其他规则名返回值为`false`
    - 多个棋盘位置规则间用`&`连接（`&`表示**或**，即棋子位置只要有一项满足该棋盘位置规则则返回值为`true`）
    - 示例：`X[1|-1]&Y[1|-1]`表示棋盘边缘区域
 
 2. 可移动规则
 
    - 该语法规则分为两部分，第一部分为可以向某方向移动一格，第二部分为可以向某方向移动无限格。两部分语法相同，两部分间用`;`隔开
    - 在每一部分中，用`,`分隔开所有可移动方向，这些方向按**左上、上、右上、左、右、左下、下、右下**分别对应1-8
    - 如果这一方向上是否可以移动有位置限制，可以在方向编号后加上`()`，并在内部填入*棋盘位置规则*
    - 在第二部分中出现的可移动方向可以不出现在第一部分中
    - 如果没有第二部分（或第一部分）也需要在后面（或前面）加上`;`
    - 示例：`1(Y[4|5|6]),3(Y[2|3|4]),4(Y[7]),5(Y[1]);2`
 
-棋子表的每一列内容依次是：
-
-```
-编号 名称 归属 首领 可移动 升变条件 升变后可移动
-```
+棋子表的每一列内容依次是`编号`、`名称`、`归属`、`首领`、`可移动`、`升变条件`、`升变后可移动`、`其他`
 
 这些内容必须**按序**排列，具体填写规则如下：
 
 1. 编号
 
    - 每个棋子独立的不同的编号
    - 按照顺序由1递增
@@ -153,14 +159,17 @@
    - 当棋子位置符合升变条件时，其可移动规则永久变为*升变后可移动*
 
 7. 升变后可移动
 
    - 填入*可移动规则*
    - 该角色无法升变时仍需填写`;`
 
+8. 其他
+
+   - 可以有多列，每列标题、填写规则由扩展而定
 
 ### 棋盘表
 
 棋盘表的名称为`map`
 
 棋盘表由两部分组成：棋盘行列数、棋盘布局
```

### Comparing `s27a_jbq-1.0.1/pyproject.toml` & `s27a_jbq-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s27a_jbq"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="amf", email="xyf081202@163.com" },
 ]
 description = "A board game with high degrees of freedom"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `s27a_jbq-1.0.1/src/s27a_jbq/extension.py` & `s27a_jbq-1.0.2/src/s27a_jbq/extension.py`

 * *Files identical despite different names*

### Comparing `s27a_jbq-1.0.1/src/s27a_jbq/game.py` & `s27a_jbq-1.0.2/src/s27a_jbq/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 from .static import ARR,MapViewer,static_data,save_record
 from .map import Chess,Map,HistoryRecorder
 from .window import MainWindow,GameWindow,SettingWindow
 from .extension import ExtAPI,ExtensionManager
 
 class App:
-    def __init__(self,record_path:str = None):
+    RUNNING = False
+    def __init__(self):
+        if App.RUNNING:
+            raise RuntimeError("App只能有一个实例")
+        App.RUNNING = True
         self.map_data = None
         self.map_path = None
-        if record_path and not record_path.endswith(".csv"):
-            record_path += ".csv"
-        self.record_path = record_path 
+        self.open_setting = False
 
     def run(self,debug:bool = False):
         self.debug = debug
         self.extension_manager = ExtensionManager(self)
         self.window = MainWindow({
             # 主窗口调用的函数
             "get_map":self.get_map,
@@ -54,44 +56,51 @@
                 return
         if success_prompt:
             showinfo("提示","地图文件加载成功")
         self.map_path = filename
         self.window.set_map(self.map_path)
 
     def start_game(self):
+        if self.open_setting:
+            return
         if not self.map_data:
             showinfo("提示","暂未选择地图")
             return
         self.window.withdraw()
         if self.debug:
-            game = Game(self.map_data,self.record_path,self.debug)
+            game = Game(self.map_data,self.debug)
             game.start()
         else:
             try:
-                game = Game(self.map_data,self.record_path,self.debug)
+                game = Game(self.map_data,self.debug)
                 game.start()
             except Exception as e:
                 showerror("错误",f"游戏运行错误：{e}")
         self.window.deiconify()
 
     def add_extension(self):
         filename = self.window.choose_extension_file()
         self.extension_manager.add_extension(filename)
         self.window.refresh_extension()
 
     def setting(self):
-        setting_window = SettingWindow(self.add_extension,self.window.refresh_extension)
-        setting_window.mainloop()
+        if not self.open_setting:
+            self.open_setting = True
+            setting_window = SettingWindow(self.close_setting_window,self.add_extension,self.window.refresh_extension)
+            setting_window.mainloop()
+
+    def close_setting_window(self,window:SettingWindow):
+        self.open_setting = False
+        window.destroy()
 
 # 游戏类
 # 每场创建一个新的Game对象
 class Game:
-    def __init__(self,map_data:Map,record_path:str,debug:bool):
+    def __init__(self,map_data:Map,debug:bool):
         self.map_data = map_data
-        self.record_path = record_path
         self.debug = debug
         self.map_data.init_chessboard(self.win)
         self.history_recorder = HistoryRecorder(self.map_data)
         game_api = {
             "click":self.click,
             "info":self.get_info,
             "back":self.back,
@@ -247,10 +256,9 @@
     # 和棋
     # 只能由扩展触发
     def stalemate(self):
         showinfo("提示","双方和棋")
         self.stop()
 
     def stop(self):
-        if self.record_path:
-            save_record(self.record_path,self.history_recorder.history) # 记录棋局
+        save_record(self.history_recorder.history) # 记录棋局
         self.running = False
```

### Comparing `s27a_jbq-1.0.1/src/s27a_jbq/map.py` & `s27a_jbq-1.0.2/src/s27a_jbq/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,14 @@
                 if len(j) == 1: # 没有判断条件
                     move[-1].append(j[0])
                 elif len(j) == 2:
                     if self.map_data.is_in_position(arr,j[1]):
                         move[-1].append(j[0])
         return move
 
-    # 升变条件检测
-    def tran(self,arr:ARR):
-        if self.is_tran:
-            return
-        if self.map_data.is_in_position(arr,self.tran_con):
-            self.is_tran = True
-
 class Map:
     def __init__(self,chesses:list,map:list[list[int]],rules:dict):
         self.chesses = chesses
         self.map = map
         self.rules = rules
         self.rl = len(self.map) # 地图行数
         self.cl = len(self.map[0]) # 地图列数
@@ -108,16 +101,17 @@
                     if arr[0] == get_abs_pos(j,self.rl):
                         return True
             elif command == "Y": # 函数Y（列）
                 for j in i[1:]:
                     if arr[1] == get_abs_pos(j,self.cl):
                         return True
             elif command == "P": # 函数P（点）
-                if arr == (get_abs_pos(i[1],self.rl),get_abs_pos(i[2],self.cl)):
-                    return True
+                for j in range(1,len(i),2):
+                    if arr == (get_abs_pos(i[j],self.rl),get_abs_pos(i[j + 1],self.cl)):
+                        return True
             for j in ExtensionManager.Ext.loc_rules: # 扩展中的函数
                 if command == j:
                     if ExtensionManager.Ext.loc_rules[j](i[1:],arr):
                         return True
         return False
 
     # 移动棋子
@@ -132,15 +126,27 @@
                 self.red_move_ne = 0
             else:
                 self.blue_move_ne = 0
         if arr1 != arr2 and self.chessboard[arr2[0]][arr2[1]] and self.chessboard[arr2[0]][arr2[1]].is_captain:
             self.win(turn)
         self.chessboard[arr1[0]][arr1[1]],self.chessboard[arr2[0]][arr2[1]] = None,self.chessboard[arr1[0]][arr1[1]]
         if self.rules["tran"]:
-            self.chessboard[arr2[0]][arr2[1]].tran(arr2)
+            self.tran()
+
+    # 棋子升变
+    def tran(self):
+        for i in range(self.rl):
+            for j in range(self.cl):
+                chess = self.chessboard[i][j]
+                if not chess:
+                    continue
+                if chess.is_tran:
+                    continue
+                if self.is_in_position((i,j),chess.tran_con):
+                    chess.is_tran = True
 
 class HistoryRecorder:
     def __init__(self,map_data:Map):
         self.history = list[tuple[list[list[Chess]],str]]()
         self.history.append((self.copy_chessboard(map_data.chessboard),1)) # 初始也在其中，走完后立即add
         self.now = 1 # 当前位置（不含）
```

### Comparing `s27a_jbq-1.0.1/src/s27a_jbq/static.py` & `s27a_jbq-1.0.2/src/s27a_jbq/static.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 import os
 import sys
 import csv
 import json
 
-from tkinter.messagebox import showerror
+from openpyxl import load_workbook
 
-# 导入第三方模块openpyxl并进行版本判断
-try:
-    from openpyxl import load_workbook
-except ModuleNotFoundError:
-    showerror("提示","未安装openpyxl")
-    sys.exit()
-
-RELEASE_DATE = "2023-05-20"
+RELEASE_DATE = "2023-05-25"
 COLOR_STYLES = {
     "normal":{
         "name":"标准",
         "colors":{
             "chessboard":"khaki",
             "red-label":"pink",
             "blue-label":"skyblue",
@@ -52,20 +45,16 @@
         "relief":"groove",
         "bg":"snow"
     },
     "label-style":{
         "relief":"groove"
     }
 }
-static = {
-    "color-styles":1,
-    "shape-style":COMPONENT_STYLE
-}
 
-setting_path = "setting.json"
+SETTING_PATH = "setting.json"
 
 ARR = tuple[int,int] # 棋子位置数组
 
 def load(path:str):
     with open(path,encoding = "utf-8") as rfile:
         return json.load(rfile)
 
@@ -83,16 +72,16 @@
         [('X',1),('Y',2),('P',2,3),('T',7)]
         """
         data = data.split("&")
         loc = list[tuple]()
         for i in data:
             if not i:
                 continue
-            command = i[0]
-            args = [int(j) for j in i[2:-1].split("|")]
+            command = i.split("[")[0]
+            args = [int(j) for j in i[len(command) + 1:-1].split("|")]
             loc.append(tuple([command] + args))
         return loc
 
     # 解析移动规则
     @staticmethod
     def parse_move(data:str):
         """
@@ -145,61 +134,71 @@
         # 处理特殊规则
         rules_sheet = wb.get_sheet_by_name("rules")
         rules = {}
         rules["tran"] = rules_sheet[2][2].value == "c" # 启用升变
         rules["back"] = rules_sheet[3][2].value == "c" # 启用悔棋
         rules["restrict_move_ne"] = rules_sheet[4][2].value == "c" # 限制连续3步以上移动中立棋子
         # 将打开的棋盘文件保存到设置中
-        setting = load(setting_path)
+        setting = load(SETTING_PATH)
         setting["lastly-load-map"] = filename
-        write(setting_path,setting)
+        write(SETTING_PATH,setting)
         return (chesses,map,rules)
 
-def load_data():
-    if os.path.exists(setting_path):
-        setting = load(setting_path)
-    else:
-        setting = {
-            "color-styles":"normal",
-            "lastly-load-map":"",
-            "used-extensions":[]
-        }
-        write(setting_path,setting)
-    static_data = {}
-    static_data["color-styles"] = [(i,COLOR_STYLES[i]["name"]) for i in COLOR_STYLES]
-    static_data["color-style-name"] = setting["color-styles"]
-    static_data["colors"] = COLOR_STYLES[setting["color-styles"]]["colors"]
-    static_data["shape-style"] = COMPONENT_STYLE
-    static_data["lastly-load-map"] = setting["lastly-load-map"]
-    static_data["used-extensions"] = setting["used-extensions"]
-    return static_data
-
 def refresh_extension(extensions):
-    setting = load(setting_path)
+    setting = load(SETTING_PATH)
     setting["used-extensions"] = []
     for i in extensions:
         if i.use:
             setting["used-extensions"].append(i.name)
-    write(setting_path,setting)
+    write(SETTING_PATH,setting)
     static_data["used-extensions"] = setting["used-extensions"]
 
 def refresh_color(value:str):
-    setting = load(setting_path)
+    setting = load(SETTING_PATH)
     setting["color-styles"] = value
-    write(setting_path,setting)
+    write(SETTING_PATH,setting)
     static_data["color-style-name"] = value
     static_data["colors"] = COLOR_STYLES[value]["colors"]
 
-def save_record(record_path:str,history:list[tuple[list[list],str]]):
+def set_record_path(path:str):
+    setting = load(SETTING_PATH)
+    setting["record-path"] = path
+    write(SETTING_PATH,setting)
+    static_data["record-path"] = path
+
+def save_record(history:list[tuple[list[list],str]]):
+    if not static_data["record-path"]:
+        return
     print_chessboard = []
     for index,i in enumerate(history):
         print_chessboard.append([f"回合{index + 1}"])
         print_chessboard.extend([[k.name if k else " " for k in j] for j in i[0]])
-    with open(record_path,"w",newline = "") as wfile:
+    with open(static_data["record-path"],"w",newline = "") as wfile:
         writer = csv.writer(wfile)
         writer.writerows(print_chessboard)
 
-try:
-    static_data = load_data()
-except (FileNotFoundError,KeyError):
-    showerror("错误","配置文件错误, 请尝试删除setting文件或重新下载static文件")
-    sys.exit()
+def load_data():
+    if os.path.exists(SETTING_PATH):
+        setting = load(SETTING_PATH)
+    else:
+        setting = {
+            "color-styles":"normal",
+            "lastly-load-map":"",
+            "record-path":"",
+            "used-extensions":[]
+        }
+        write(SETTING_PATH,setting)
+    static_data = {}
+    try:
+        static_data["color-styles"] = [(i,COLOR_STYLES[i]["name"]) for i in COLOR_STYLES]
+        static_data["color-style-name"] = setting["color-styles"]
+        static_data["colors"] = COLOR_STYLES[setting["color-styles"]]["colors"]
+        static_data["shape-style"] = COMPONENT_STYLE
+        static_data["lastly-load-map"] = setting["lastly-load-map"]
+        static_data["record-path"] = setting["record-path"]
+        static_data["used-extensions"] = setting["used-extensions"]
+    except: # setting文件格式错误
+        os.remove(SETTING_PATH)
+        static_data = load_data()
+    return static_data
+
+static_data = load_data()
```

### Comparing `s27a_jbq-1.0.1/src/s27a_jbq/window.py` & `s27a_jbq-1.0.2/src/s27a_jbq/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import tkinter as tk
 import webbrowser
 
 from tkinter.messagebox import showinfo
-from tkinter.filedialog import askopenfilename
+from tkinter.filedialog import askopenfilename,asksaveasfilename
 
 from .__constants__ import __version__
-from .static import ARR,RELEASE_DATE,static_data,refresh_extension,refresh_color
-from .map import Map
+from .static import ARR,RELEASE_DATE,static_data,refresh_extension,refresh_color,set_record_path
+from .map import Chess,Map
 from .extension import Extension,ExtensionManager
 
 class MainWindow(tk.Tk):
     def __init__(self,app_api:dict,debug:bool):
         super().__init__()
         self.app_api = app_api
         self.title(f"精班棋 {__version__}{' [debug mode]' if debug else ''}")
@@ -86,15 +86,16 @@
 
 class GameWindow(tk.Tk):
     def __init__(self,belong:int,map_data:Map,game_api:dict):
         super().__init__()
         self.belong = belong
         self.map_data = map_data
         self.game_api = game_api
-        self.can_go_prompt_list = ["·","*","o","x"]
+        self.can_go_prompt_list = ["·","*","o","x","%"]
+        self.show_can_go_prompt = True
         self.title("红方" if self.belong == 1 else "蓝方")
         self.resizable(width = False,height = False)
         self.protocol("WM_DELETE_WINDOW",self.game_api["stop"])
         self.init_menu()
         self.init_chessboard()
         self.refresh_map()
 
@@ -115,14 +116,15 @@
         self.func_menu = tk.Menu(self.menu,tearoff = False)
         self.menu.add_cascade(label = "功能(F)",underline = 3,menu = self.func_menu)
         if True and self.map_data.rules["back"]: # 仅在单人模式下生效
             self.func_menu.add_command(label = "悔棋",command = lambda:self.game_api["back"](1))
             self.func_menu.add_command(label = "撤销悔棋",command = lambda:self.game_api["back"](-1))
             self.func_menu.add_separator()
         self.func_menu.add_command(label = "切换棋子大小",command = self.change_chess_height)
+        self.func_menu.add_command(label = "显示/隐藏可行走提示",command = self.change_show_prompt)
 
     def map_info(self):
         rules = {
             "tran":"启用升变",
             "back":"启用悔棋",
             "restrict_move_ne":"限制连续3步以上移动中立棋子"
         }
@@ -142,14 +144,18 @@
                 if j["height"] == 3: # 大棋子
                     j["height"] = 2
                     j["width"] = 5
                 else:
                     j["height"] = 3
                     j["width"] = 8
 
+    def change_show_prompt(self):
+        self.show_can_go_prompt = not self.show_can_go_prompt
+        self.refresh_map()
+
     #反方棋盘渲染反转横纵坐标
     def getx(self,x:int):
         return x if self.belong == 1 else self.map_data.rl - x - 1
 
     def gety(self,y:int):
         return y if self.belong == 1 else self.map_data.cl - y - 1
 
@@ -165,14 +171,15 @@
                 self.chess_btn[-1][-1].bind("<Button 3>",self.click(i,j,3))
                 self.chess_btn[-1][-1].grid(row = i,column = j,padx = 1,pady = 1)
         self.chess_frame.pack()
         self.mess_label = tk.Label(self,height = 3,width = 24)
         self.mess_label.pack()
         if len(self.chess_btn) > 8 or len(self.chess_btn[0]) > 12:
             self.change_chess_height()
+            self.change_show_prompt()
 
     # 点击棋子回调中转函数
     def click(self,x:int,y:int,key:int):
         def wrapper(event = None):
             if key == 1:
                 self.game_api["click"]((self.getx(x),self.gety(y)),self.belong)
             else:
@@ -199,45 +206,49 @@
                     self.chess_btn[i][j]["text"] = text
                     self.chess_btn[i][j]["fg"] = fg
                 else:
                     self.chess_btn[i][j]["text"] = ""
                 self.chess_btn[i][j]["bg"] = static_data["colors"]["chess-bg"]
 
     # 在按钮上显示的文字及颜色
-    def get_chess_text(self,chess):
-        can_go_prompt = list[str]()
-        now_move = chess.now_move # 先赋值中间变量，避免调用self.now_move属性时重新计算
-        for i in range(1,9):
-            is_add = False
-            for j,k in enumerate(now_move):
-                if i in k:
-                    can_go_prompt.append(self.can_go_prompt_list[j])
-                    is_add = True
-                    break
-            if not is_add:
-                can_go_prompt.append(" ")
-        if self.belong == 2: # 反方棋盘
-            can_go_prompt.reverse()
-        # 生成名字
-        name_withspace = chess.name
-        name_length = len(chess.name.encode(encoding = "gbk"))
-        side = True # True为右侧
-        while name_length < 6:
-            if side:
-                name_withspace += " "
-            else:
-                name_withspace = " " + name_withspace
-            side = not side
-            name_length += 1
-        can_go_prompt.insert(4,name_withspace)
-        # 合并空格
-        text = ""
-        whitespace = ["   ","   ","\n","","","\n","   ","   ",""]
-        for i in range(9):
-            text += (can_go_prompt[i] + whitespace[i])
+    def get_chess_text(self,chess:Chess) -> tuple[str,str]:
+        if self.show_can_go_prompt:
+            can_go_prompt = list[str]()
+            now_move = chess.now_move # 先赋值中间变量，避免调用self.now_move属性时重新计算
+            for i in range(1,9):
+                is_add = False
+                for j,k in enumerate(now_move):
+                    if i in k:
+                        if is_add: # 仅保留最后一项
+                            del can_go_prompt[-1]
+                        can_go_prompt.append(self.can_go_prompt_list[j])
+                        is_add = True
+                if not is_add:
+                    can_go_prompt.append(" ")
+            if self.belong == 2: # 反方棋盘
+                can_go_prompt.reverse()
+            # 生成名字
+            name_withspace = chess.name
+            name_length = len(chess.name.encode(encoding = "gbk"))
+            side = True # True为右侧
+            while name_length < 6:
+                if side:
+                    name_withspace += " "
+                else:
+                    name_withspace = " " + name_withspace
+                side = not side
+                name_length += 1
+            can_go_prompt.insert(4,name_withspace)
+            # 合并空格
+            text = ""
+            whitespace = ["   ","   ","\n","","","\n","   ","   ",""]
+            for i in range(9):
+                text += (can_go_prompt[i] + whitespace[i])
+        else:
+            text = chess.name
         # 设置颜色
         if chess.belong == 1:
             if chess.is_tran or not chess.tran_con:
                 fg = "red-tran-chess-fg"
             else:
                 fg = "red-chess-fg"
         elif chess.belong == 2:
@@ -246,49 +257,64 @@
             else:
                 fg = "blue-chess-fg"
         else:
             fg = "neutral-chess-fg"
         return text,static_data["colors"][fg]
 
 class SettingWindow(tk.Tk):
-    def __init__(self,add_ext_func,refresh_ext_func):
+    def __init__(self,close_func,add_ext_func,refresh_ext_func):
         super().__init__()
         self.title("设置")
         self.minsize(480,360)
         self.resizable(width = False,height = False)
+        self.protocol("WM_DELETE_WINDOW",lambda:close_func(self))
         self.main_frame = tk.Frame(self) # 解决布局分布在两侧的问题
         self.main_frame.pack()
+
+        self.left_frame = tk.Frame(self.main_frame)
+        self.left_frame.pack(side = "left",fill = "y",padx = 18)
         # 扩展
-        self.extension_frame = tk.Frame(self.main_frame)
-        self.extension_frame.pack(side = "left",fill = "y",padx = 18)
-        self.extension_label = tk.Label(self.extension_frame,text = "已加载扩展",width = 24,height = 2,**static_data["shape-style"]["label-style"])
+        self.extension_label = tk.Label(self.left_frame,text = "已加载扩展",width = 24,height = 2,**static_data["shape-style"]["label-style"])
         self.extension_label.pack(pady = 5)
         self.extension_btns = list[tk.Button]()
         for i in ExtensionManager.Ext.extensions:
-            self.extension_btns.append(tk.Button(self.extension_frame,text = i.text(),width = 20,**static_data["shape-style"]["btn-style"]))
+            self.extension_btns.append(tk.Button(self.left_frame,text = i.text(),width = 20,**static_data["shape-style"]["btn-style"]))
             self.extension_btns[-1]["bg"] = "lightgreen" if i.use else "pink"
             self.extension_btns[-1]["command"] = self.use_extension(self.extension_btns[-1],i,refresh_ext_func)
             self.extension_btns[-1].pack(pady = 5)
-        self.add_extension_btn = tk.Button(self.extension_frame,text = "添加扩展",width = 16,height = 2,**static_data["shape-style"]["btn-style"],command = add_ext_func)
+        self.add_extension_btn = tk.Button(self.left_frame,text = "添加扩展",width = 16,height = 2,**static_data["shape-style"]["btn-style"],command = add_ext_func)
         self.add_extension_btn.pack(pady = 5)
+
+        self.right_frame = tk.Frame(self.main_frame)
+        self.right_frame.pack(side = "right",fill = "y",padx = 18)
         # 颜色样式
-        self.color_style_frame = tk.Frame(self.main_frame)
-        self.color_style_frame.pack(side = "right",fill = "y",padx = 18)
-        self.set_color_style_label = tk.Label(self.color_style_frame,text = "设置颜色样式",width = 24,height = 2,**static_data["shape-style"]["label-style"])
+        self.set_color_style_label = tk.Label(self.right_frame,text = "设置颜色样式",width = 24,height = 2,**static_data["shape-style"]["label-style"])
         self.set_color_style_label.pack(pady = 5)
         self.set_color_style_var = tk.StringVar()
         self.set_color_style_radius = list[tk.Radiobutton]()
         for i in static_data["color-styles"]:
-            self.set_color_style_radius.append(tk.Radiobutton(self.color_style_frame,text = i[1],variable = self.set_color_style_var,value = i[0],command = self.set_color(i[0])))
+            self.set_color_style_radius.append(tk.Radiobutton(self.right_frame,text = i[1],variable = self.set_color_style_var,value = i[0],command = self.set_color(i[0])))
             if i[0] == static_data["color-style-name"]:
                 self.set_color_style_radius[-1].select()
             self.set_color_style_radius[-1].pack(pady = 5)
+        # 棋局记录文件
+        self.record_path_label1 = tk.Label(self.right_frame,text = "棋局记录文件",width = 24,height = 2,**static_data["shape-style"]["label-style"])
+        self.record_path_label1.pack(pady = 5)
+        self.record_path_label2 = tk.Label(self.right_frame,text = static_data["record-path"] if static_data["record-path"] else "不进行记录",height = 2,**static_data["shape-style"]["label-style"])
+        self.record_path_label2.pack(pady = 5)
+        self.set_record_path_btn = tk.Button(self.right_frame,text = "选择棋局记录文件",width = 16,height = 2,**static_data["shape-style"]["btn-style"],command = self.set_record)
+        self.set_record_path_btn.pack(pady = 5)
 
     def use_extension(self,button:tk.Button,extension:Extension,refresh_ext_func):
         def wrapper():
             extension.use = not extension.use
             button["bg"] = "lightgreen" if extension.use else "pink"
             refresh_ext_func()
         return wrapper
 
     def set_color(self,value:str):
         return lambda:refresh_color(value)
+
+    def set_record(self):
+        filename = asksaveasfilename(filetypes = [("CSV Files","*.csv"),("All Files","*.*")],initialfile = "游戏记录.csv",title = "选择棋局记录文件")
+        set_record_path(filename)
+        self.record_path_label2["text"] = static_data["record-path"] if static_data["record-path"] else "不进行记录"
```

### Comparing `s27a_jbq-1.0.1/src/s27a_jbq.egg-info/PKG-INFO` & `s27a_jbq-1.0.2/src/s27a_jbq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: s27a-jbq
-Version: 1.0.1
+Version: 1.0.2
 Summary: A board game with high degrees of freedom
 Author-email: amf <xyf081202@163.com>
 Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
 Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.1-blue)
+![](https://img.shields.io/badge/release-1.0.2-blue)
 ![](https://img.shields.io/badge/last%20commit-may-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
 精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
@@ -32,61 +32,71 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您可以从[这里](https://github.com/amf14151/s27a_jbq/archive/refs/heads/main.zip)直接下载文件并自行安装，或使用以下指令来安装
+您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包，也可以按照下面的步骤安装模块并使用
+
+## 安装模块
+
+*若想通过模块的方式运行精班棋，您需要Python解释器*
+
+使用以下命令来安装模块
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装`s27a_jbq`模块后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
+在安装`s27a_jbq`模块后，使用以下命令来构建游戏文件夹
 
-``` python
-from s27a_jbq import generate_game
+```
+python.exe -m s27a_jbq generate_game {游戏文件夹路径} {游戏运行方式}
+```
+
+其中，游戏运行方式有以下选择：
+
+- `window`：窗口模式
 
-generate_game(
-   game_path = "JBQ", # 游戏文件夹位置
-   record_path = None, # 棋局记录位置，格式为.csv，使用相对路径时根目录为游戏文件夹路径
-   display = "window" # 游戏打开方式，'window'为窗口模式
-)
+示例：
+
+```
+python.exe -m s27a_jbq generate_game C:/JBQ window
 ```
 
+上方的代码在C盘根目录中创建名为`JBQ`的游戏文件夹
+
 您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
 
 ``` python
 from s27a_jbq.game import App
 
 def main():
    app = App()
    app.run()
 ```
 
 在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
-另有`map`文件夹，该文件夹用于存储地图，地图是进行游戏的关键文件
-
 # 使用方法
 
 [(返回目录)](#目录)
 
 ## 游戏过程
 
 在设置好地图及扩展（具体方法请参见下文）后，点击开始游戏即可
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
 
 一些棋子在不同的位置会有不同的可移动格子，每个棋子的具体可移动格子根据地图、扩展决定
 
-在对局结束后，如果设置了`record_path`，则会在文件夹中创建同名文件，格式为`.csv`
+在对局结束后，如果在设置中设置了棋局记录路径，则会对棋局进行记录
 
 ## 地图
 
 地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
 
 地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
@@ -110,33 +120,29 @@
 
 1. 棋盘位置规则
 
    - 单个棋盘位置规则表示为`M[a|b|c]`的形式，其中`M`为规则名，为大写，`a`、`b`、`c`等为参数，为整数，用`|`隔开
    - 可使用的规则名：
      - `X[m|n|...]`，当棋子所在的行数等于任意一个参数（`m`、`n`等）时，该规则的值为`true`，否则为`false`
      - `Y[m|n|...]`，当棋子所在的列数等于任意一个参数（`m`、`n`等）时，该规则的值为`true`，否则为`false`
-     - `P[x|y]`，当棋子所在的位置等于`(x,y)`时，该规则的值为`true`，否则为`false`
+     - `P[x1|y1|x2|y2|...]`，当棋子所在的位置等于`(xn,yn)`时，该规则的值为`true`，否则为`false`
    - 其他规则名返回值为`false`
    - 多个棋盘位置规则间用`&`连接（`&`表示**或**，即棋子位置只要有一项满足该棋盘位置规则则返回值为`true`）
    - 示例：`X[1|-1]&Y[1|-1]`表示棋盘边缘区域
 
 2. 可移动规则
 
    - 该语法规则分为两部分，第一部分为可以向某方向移动一格，第二部分为可以向某方向移动无限格。两部分语法相同，两部分间用`;`隔开
    - 在每一部分中，用`,`分隔开所有可移动方向，这些方向按**左上、上、右上、左、右、左下、下、右下**分别对应1-8
    - 如果这一方向上是否可以移动有位置限制，可以在方向编号后加上`()`，并在内部填入*棋盘位置规则*
    - 在第二部分中出现的可移动方向可以不出现在第一部分中
    - 如果没有第二部分（或第一部分）也需要在后面（或前面）加上`;`
    - 示例：`1(Y[4|5|6]),3(Y[2|3|4]),4(Y[7]),5(Y[1]);2`
 
-棋子表的每一列内容依次是：
-
-```
-编号 名称 归属 首领 可移动 升变条件 升变后可移动
-```
+棋子表的每一列内容依次是`编号`、`名称`、`归属`、`首领`、`可移动`、`升变条件`、`升变后可移动`、`其他`
 
 这些内容必须**按序**排列，具体填写规则如下：
 
 1. 编号
 
    - 每个棋子独立的不同的编号
    - 按照顺序由1递增
@@ -167,14 +173,17 @@
    - 当棋子位置符合升变条件时，其可移动规则永久变为*升变后可移动*
 
 7. 升变后可移动
 
    - 填入*可移动规则*
    - 该角色无法升变时仍需填写`;`
 
+8. 其他
+
+   - 可以有多列，每列标题、填写规则由扩展而定
 
 ### 棋盘表
 
 棋盘表的名称为`map`
 
 棋盘表由两部分组成：棋盘行列数、棋盘布局
```

