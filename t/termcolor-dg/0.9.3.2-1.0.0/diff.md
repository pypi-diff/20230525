# Comparing `tmp/termcolor_dg-0.9.3.2.tar.gz` & `tmp/termcolor_dg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termcolor_dg-0.9.3.2.tar", last modified: Wed Jan 11 11:11:02 2023, max compression
+gzip compressed data, was "termcolor_dg-1.0.0.tar", last modified: Wed May 24 22:39:02 2023, max compression
```

## Comparing `termcolor_dg-0.9.3.2.tar` & `termcolor_dg-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-01-11 11:11:02.346923 termcolor_dg-0.9.3.2/
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      323 2022-11-20 23:08:37.000000 termcolor_dg-0.9.3.2/.pylintrc
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1875 2022-02-14 09:33:23.000000 termcolor_dg-0.9.3.2/CHANGES.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      504 2023-01-11 11:09:09.000000 termcolor_dg-0.9.3.2/INSTALL.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1073 2022-02-05 13:13:56.000000 termcolor_dg-0.9.3.2/LICENSE
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      300 2023-01-11 10:23:58.000000 termcolor_dg-0.9.3.2/MANIFEST.in
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     2854 2023-01-11 11:10:09.000000 termcolor_dg-0.9.3.2/Makefile
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    11663 2023-01-11 11:11:02.347923 termcolor_dg-0.9.3.2/PKG-INFO
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     8842 2023-01-11 11:11:00.000000 termcolor_dg-0.9.3.2/README.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      119 2022-02-22 22:00:05.000000 termcolor_dg-0.9.3.2/TODO.md
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   113637 2022-02-10 07:54:40.000000 termcolor_dg-0.9.3.2/color_logs.png
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   158505 2022-02-05 13:13:56.000000 termcolor_dg-0.9.3.2/colors.png
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      106 2022-02-05 13:13:56.000000 termcolor_dg-0.9.3.2/pyproject.toml
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1873 2023-01-11 11:11:02.347923 termcolor_dg-0.9.3.2/setup.cfg
--rwxrwxr-x   0 dgunchev  (1000) dgunchev  (1000)      809 2022-03-21 14:32:23.000000 termcolor_dg-0.9.3.2/setup.py
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-01-11 11:11:02.346923 termcolor_dg-0.9.3.2/src/
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-01-11 11:11:02.346923 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    11663 2023-01-11 11:11:02.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/PKG-INFO
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      452 2023-01-11 11:11:02.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/SOURCES.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-01-11 11:11:02.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/dependency_links.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      118 2023-01-11 11:11:02.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/entry_points.txt
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-01-11 11:11:02.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/not-zip-safe
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)       13 2023-01-11 11:11:02.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.egg-info/top_level.txt
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)    20128 2023-01-11 11:00:11.000000 termcolor_dg-0.9.3.2/src/termcolor_dg.py
--rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2082 2023-01-11 11:00:51.000000 termcolor_dg-0.9.3.2/termcolor_dg.spec
-drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-01-11 11:11:02.346923 termcolor_dg-0.9.3.2/test/
--rwxrwxr-x   0 dgunchev  (1000) dgunchev  (1000)    13304 2023-01-11 10:05:05.000000 termcolor_dg-0.9.3.2/test/test_termcolor_dg.py
--rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1728 2022-02-09 11:53:16.000000 termcolor_dg-0.9.3.2/tox.ini
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      302 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/.pylintrc
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2208 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/CHANGES.md
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      512 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/INSTALL.md
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)     1073 2022-02-05 13:13:56.000000 termcolor_dg-1.0.0/LICENSE
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      300 2023-01-11 10:23:58.000000 termcolor_dg-1.0.0/MANIFEST.in
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     3046 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/Makefile
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    12208 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/PKG-INFO
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     8908 2023-05-24 22:38:59.000000 termcolor_dg-1.0.0/README.md
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      119 2022-02-22 22:00:05.000000 termcolor_dg-1.0.0/TODO.md
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   113637 2022-02-10 07:54:40.000000 termcolor_dg-1.0.0/color_logs.png
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)   158505 2022-02-05 13:13:56.000000 termcolor_dg-1.0.0/colors.png
+-rw-rw-r--   0 dgunchev  (1000) dgunchev  (1000)      106 2022-02-05 13:13:56.000000 termcolor_dg-1.0.0/pyproject.toml
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     1999 2023-05-24 22:39:02.113514 termcolor_dg-1.0.0/setup.cfg
+-rwxrwxr-x   0 dgunchev  (1000) dgunchev  (1000)      809 2022-03-21 14:32:23.000000 termcolor_dg-1.0.0/setup.py
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.111514 termcolor_dg-1.0.0/src/
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    12208 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/PKG-INFO
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      452 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/SOURCES.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/dependency_links.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)      118 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/entry_points.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)        1 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/not-zip-safe
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)       13 2023-05-24 22:39:02.000000 termcolor_dg-1.0.0/src/termcolor_dg.egg-info/top_level.txt
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)    20170 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/src/termcolor_dg.py
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2723 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/termcolor_dg.spec
+drwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)        0 2023-05-24 22:39:02.112514 termcolor_dg-1.0.0/test/
+-rwxr-xr-x   0 dgunchev  (1000) dgunchev  (1000)    13743 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/test/test_termcolor_dg.py
+-rw-r--r--   0 dgunchev  (1000) dgunchev  (1000)     2285 2023-05-24 22:28:57.000000 termcolor_dg-1.0.0/tox.ini
```

### Comparing `termcolor_dg-0.9.3.2/CHANGES.md` & `termcolor_dg-1.0.0/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,104 @@
 termcolor_dg changes
 ====================
 
+1.0.0 (2023-05-25)
+------------------
+
+- fix DISABLED detection
+- logging.basicConfig has no disable_existing_loggers argument.
+- move back to GitHub, workflows does work and is free.
+
+0.9.3.1 (2022-02-14)
+--------------------
+
+- Adjust the log color scheme.
+- pylint fixes in the color demo.
+
 0.9.3 (2022-02-14)
 ------------------
+
 - Adjust the log color scheme.
 - pylint fixes in the color demo.
 
 0.9.2 (2022-02-07)
 ------------------
-- Combine color, background and attributes in single escape sequence
-- minor enhancements
+
+- Combine color, background and attributes in a single escape sequence.
+- Minor enhancements.
 
 0.9.1 (2022-02-05)
 ------------------
-- rename to termcolor_dg (termcolor2 is taken)
+
+- Rename to termcolor_dg (termcolor2 is taken).
 
 0.9.0 (2022-02-05)
 ------------------
-- fork to termcolor2
-- add 24-bit colors support
-- add logging and color demos
-- add ANSI_COLORS_DISABLED and ANSI_COLORS_FORCE environment variables
-- add always_colored, rainbow_color
-- add monkey_patch_logging and logging_basic_color_config utility functions
-- better cprint and print compatibility (no arguments = new line)
-- drop 'gray' and 'on_gray' (it was an alias for black, bad idea?)
-- make trailing reset sequence optional for colored
-- `python -m build` to build the project
-- remove regex usage, the following would have not been stripped but works: `echo -e '(\e[01;32mx\e[1;0033mx\e[m)'`
-- remove PKG-INFO
-- README.md instead of README.rst
+
+- Fork to termcolor2.
+- Add 24-bit colors support.
+- Add logging and color demos.
+- Add ANSI_COLORS_DISABLED and ANSI_COLORS_FORCE environment variables.
+- Add always_colored, rainbow_color.
+- Add monkey_patch_logging and logging_basic_color_config utility functions.
+- Better cprint and print compatibility (no arguments = new line).
+- Drop 'gray' and 'on_gray' (it was an alias for black, bad idea?).
+- Make the trailing reset sequence optional for colored.
+- Use `python -m build` to build the project.
+- Remove regex usage, the following would have not been stripped but works: `echo -e '(\e[01;32mx\e[1;0033mx\e[m)'`.
+- Remove PKG-INFO.
+- README.md instead of README.rst.
 - ... unit tests, INSTALL ...
 
 ---
 
 termcolor changes
 =================
 
 1.9.1 (2021-12-15)
 ------------------
+
 - python 2 and 3 compatibility, avoid KeyError
 - make pylint happy
 - fix character escapes
 - better .gitignore
 - fix __ALL__ to __all__
 
 1.1.0 (2011-01-13)
 ------------------
+
 - Added cprint function.
 
 1.0.1 (2011-01-13)
 ------------------
+
 - Updated README.rst.
 
 1.0.0 (2011-01-13)
 ------------------
+
 - Changed license to MIT.
 - Updated copyright.
 - Refactored source code.
 
 0.2 (2010-09-07)
 ------------------
-- Added support of Python 3.x.
+
+- Added support for Python 3.x.
 
 0.1.2 (2009-06-04)
 ------------------
+
 - Fixed bold characters. (Thanks Tibor Fekete)
 
 0.1.1 (2009-03-05)
 ------------------
+
 - Some refactoring.
 - Updated copyright.
 - Fixed reset colors.
 - Updated documentation.
 
 0.1 (2008-06-09)
 ----------------
+
 - Initial release.
```

### Comparing `termcolor_dg-0.9.3.2/LICENSE` & `termcolor_dg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termcolor_dg-0.9.3.2/Makefile` & `termcolor_dg-1.0.0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 TOP := $(shell dirname "$(abspath $(lastword $(MAKEFILE_LIST)))")
-
+PYLINT_RCFILE ?= .pylintrc
 
 .PHONY: help
 help:
 	@echo
 	@echo "▐ Help"
 	@echo "▝▀▀▀▀▀▀"
 	@echo
@@ -33,37 +33,39 @@
 
 .PHONY: test
 test:
 	coverage erase
 	PYTHONPATH=src coverage run -m unittest discover --verbose -s test
 	# coverage combine  # Will fail if only one run...
 	coverage report -m --skip-empty
-	# pylint2 $(shell git ls-files '*.py')
+	# pylint2 --rcfile .pylintrc2 $(shell git ls-files '*.py')
 	# pylint $(shell git ls-files '*.py')
-	pylint *.py */*.py
+	pylint --rcfile $(PYLINT_RCFILE) *.py */*.py
 
 
 .PHONY: clean
 clean:
 	coverage erase
 	rm -rf ./.tox ./.coverage* ./coverage.json ./coverage.xml ./htmlcov/ ./build/ ./dist/
 	rm -rf ./easy-install* ./easy_install* ./setuptools.pth ./*.egg-link termcolor_dg_demo termcolor_dg_demo_log
 	find . -depth -name '__pycache__' -exec rm -rf \{\} \;
 	find . -depth \( -name '*.pyc' -o -name '*.pyo' -o -name '*.egg-info' -o -name '*.py,cover'  \) -exec rm -rf \{\} \;
 
 
 .PHONY: build
 build: clean
-	# fix the image locations, version/tag detection would be nice
+	# https://stackoverflow.com/a/46875147 - Fix the image locations, version/tag detection would be nice.
 	# Remove URLs
-	sed -i 's#https://gitlab.com/dngunchev/termcolor_dg/.*/##g' README.md
-	sed -i 's#](\([a-zA-Z0-9/:_%]*\.png\)#](https://gitlab.com/dngunchev/termcolor_dg/-/raw/master/\1#g' README.md
+	sed -i 's#https://raw.githubusercontent.com/gunchev/termcolor_dg/.*/##g' README.md
+	# Redirect to github
+	sed -i 's#](\([a-zA-Z0-9/:_%]*\.png\)#](https://raw.githubusercontent.com/gunchev/termcolor_dg/master/\1#g' README.md
 	python -m build
-	sed -i 's#https://gitlab.com/dngunchev/termcolor_dg/.*/##g' README.md
-	# python setup.py sdist  # gives more source formats, but can't upload more than one anyways
+	# Remove URLs
+	sed -i 's#https://raw.githubusercontent.com/gunchev/termcolor_dg/.*/##g' README.md
+	# With "python setup.py sdist" we can get more source formats, but can't upload more than one anyways.
 
 
 .PHONY: test_install
 test_install:
 	pip install --user -i https://test.pypi.org/simple/ termcolor_dg
```

### Comparing `termcolor_dg-0.9.3.2/PKG-INFO` & `termcolor_dg-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,93 @@
-Metadata-Version: 2.1
-Name: termcolor_dg
-Version: 0.9.3.2
-Summary: ANSI Color formatting for terminal output and log coloring
-Home-page: https://gitlab.com/dngunchev/termcolor_dg
-Author: Konstantin Lepa
-Author-email: konstantin.lepa@gmail.com
-Maintainer: Doncho N. Gunchev
-Maintainer-email: dgunchev@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://gitlab.com/dngunchev/termcolor_dg/-/issues
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Console
-Classifier: Topic :: Terminals
-Classifier: Topic :: Software Development
-Classifier: Intended Audience :: Developers
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 termcolor_dg
 ============
 
 📦 [pypi/termcolor_dg](https://pypi.python.org/pypi/termcolor_dg) |
 📑 [ANSI escape code](https://en.wikipedia.org/wiki/ANSI_escape_code) |
 📑 [Color codes cheatsheet](https://delameter.github.io/termcolor)
 
-ANSI Color formatting for terminal output and log coloring. Supports 16 color, 256 color and 24-bit color modes.
+ANSI Color formatting for terminal output and log coloring. Supports 16 colors, 256 colors and 24-bit color modes.
 
-Python 2 support is present for legacy projects and because it is not too much work and I have to use it for now.
+Python 2 support is present for legacy projects, and because it is not too much work and I have to use it for now.
 
 
 Example
 -------
 
 ```python
->>> from termcolor_dg import colored, cprint
->>>
->>> print(colored('Hello, World!', 'light_red', 'on_blue'))
->>> cprint('Hello, World!', 'blue', 'on_light_red', ['reverse', 'blink'])
->>>
->>> print_red_on_cyan = lambda x: cprint(x, 'red', 'on_cyan')
->>> print_red_on_cyan('Hello, World!')
->>>
->>> for i in range(10):
->>>     cprint(str(i), 'magenta', end=' ' if i != 9 else '\n')
->>>
->>> import sys
->>> cprint("Attention!", 196, attrs=('bold'), file=sys.stderr)  # 256 color mode
->>> cprint("Attention!", (255, 0, 0), attrs=('bold'), file=sys.stderr)  # 24 bit color mode
->>>
->>> import logging
->>> from termcolor_dg import logging_basic_color_config
->>> logging_basic_color_config()
->>> logging.log(logging.INFO, 'test')
+from termcolor_dg import colored, cprint
+
+print(colored('Hello, World!', 'light_red', 'on_blue'))
+cprint('Hello, World!', 'blue', 'on_light_red', ['reverse', 'blink'])
+print_red_on_cyan = lambda x: cprint(x, 'red', 'on_cyan')
+print_red_on_cyan('Hello, World!')
+for i in range(10):
+  cprint(str(i), 'magenta', end=' ' if i != 9 else '\n')
+import sys
+
+cprint("Attention!", 196, attrs='bold', file=sys.stderr)  # 256 color mode
+cprint("Attention!", (255, 0, 0), attrs='bold', file=sys.stderr)  # 24-bit color mode
+import logging
+from termcolor_dg import logging_basic_color_config
+
+logging_basic_color_config()
+logging.log(logging.INFO, 'test')
 ```
 
 
 Colors demo screenshot (`python -m termcolor_dg`):
 --------------------------------------------------
 
-![colors.png](https://gitlab.com/dngunchev/termcolor_dg/-/raw/master/colors.png "Colors demo")
+![colors.png](https://raw.githubusercontent.com/gunchev/termcolor_dg/master/colors.png "Colors demo")
 
 
 Colored logs demo screenshot (`python -m termcolor_dg logs`):
 -------------------------------------------------------------
 
-![color_logs.png](https://gitlab.com/dngunchev/termcolor_dg/-/raw/master/color_logs.png "Colorized logs demo")
+![color_logs.png](https://raw.githubusercontent.com/gunchev/termcolor_dg/master/color_logs.png "Colorized logs demo")
 
 
 Environment variables
 ---------------------
 
-**ANSI_COLORS_FORCE**
-  if set to anything, even empty string, color escape sequences will be added.
+- **ANSI_COLORS_FORCE**:
+  If set to anything, even empty string, color escape sequences will be added.
 
-**ANSI_COLORS_DISABLED**
-  if set to anything no coloring will be performed, overrides **ANSI_COLORS_FORCE**.
+- **ANSI_COLORS_DISABLED**:
+  If set to anything no coloring will be performed, overrides **ANSI_COLORS_FORCE**.
 
-**NO_COLOR**
-  if set to anything no coloring will be performed, overrides **ANSI_COLORS_FORCE**.
-  see https://no-color.org/
+- **NO_COLOR**:
+  If set to anything no coloring will be performed, overrides **ANSI_COLORS_FORCE**,
+  see https://no-color.org/.
 
 If none of the environment variables is set the colors are used
 only if the ``stdout`` is attached to a terminal: ``sys.stdout.isatty()``.
 
 
 Text properties
 ---------------
 
-| Text colors   | Text highlights | Alt Text highlights  | Attributes |
-| ------------- | --------------- | -------------------- | ---------- |
-| black         | black           | on_black             | bold       |
-| red           | red             | on_red               | dark       |
-| green         | green           | on_green             | underline  |
-| yellow        | yellow          | on_yellow            | blink      |
-| blue          | blue            | on_blue              | reverse    |
-| magenta       | magenta         | on_magenta           | concealed  |
-| cyan          | cyan            | on_cyan              |            |
-| light_grey    | light_grey      | on_light_grey        |            |
-| dark_grey     | dark_grey       | on_dark_grey         |            |
-| light_red     | light_red       | on_light_red         |            |
-| light_green   | light_green     | on_light_green       |            |
-| light_yellow  | light_yellow    | on_light_yellow      |            |
-| light_blue    | light_blue      | on_light_blue        |            |
-| light_magenta | light_magenta   | on_light_magenta     |            |
-| light_cyan    | light_cyan      | on_light_cyan        |            |
-| white         | white           | on_white             |            |
+| Text colors   | Text highlights | Alt Text highlights | Attributes |
+|---------------|-----------------|---------------------|------------|
+| black         | black           | on_black            | bold       |
+| red           | red             | on_red              | dark       |
+| green         | green           | on_green            | underline  |
+| yellow        | yellow          | on_yellow           | blink      |
+| blue          | blue            | on_blue             | reverse    |
+| magenta       | magenta         | on_magenta          | concealed  |
+| cyan          | cyan            | on_cyan             |            |
+| light_grey    | light_grey      | on_light_grey       |            |
+| dark_grey     | dark_grey       | on_dark_grey        |            |
+| light_red     | light_red       | on_light_red        |            |
+| light_green   | light_green     | on_light_green      |            |
+| light_yellow  | light_yellow    | on_light_yellow     |            |
+| light_blue    | light_blue      | on_light_blue       |            |
+| light_magenta | light_magenta   | on_light_magenta    |            |
+| light_cyan    | light_cyan      | on_light_cyan       |            |
+| white         | white           | on_white            |            |
 
 
 Functions
 ---------
 
 ### Adding ANSI colors
 
@@ -169,112 +141,31 @@
 - 📑 [MarkdownGuide - Basic Syntax](https://www.markdownguide.org/basic-syntax)
 
 
 Terminal properties support
 ---------------------------
 Assume this information is outdated.
 
-| Terminal         |  bold  | dark | underline |  blink  | reverse | concealed | 256 colors | 24-bit color |
-| :--------------- | :----: | :--: | :-------: | :-----: | :-----: | :-------: | :--------: | :----------: |
-| **linux**        | ❌[^3] |❌[^3]|   ✅[^3]  |  ✅[^3] |    ✅   |     ❌    |     ❌     |      ❌      |
-| **konsole**      |   ✅   |  ✅  |     ✅    |    ✅   |    ✅   |     ✅    |     ✅     |      ✅      |
-| **terminator**   |   ✅   |  ✅  |     ✅    |    ✅   |    ✅   |     ✅    |     ✅     |      ✅      |
-| **kitty**        |   ✅   |  ✅  |     ✅    |    ✅   |    ✅   |     ❌    |     ✅     |      ✅      |
-| **xterm**        |   ✅   |  ❌  |     ✅    |    ✅   |    ✅   |     ✅    |     ✅     |      ✅      |
-| **rxvt**         |   ✅   |  ❌  |     ✅    |    ✅   |    ✅   |     ❌    |     ✅     |      ❌      |
-| **dtterm**       |   ✅   |  ✅  |     ✅    | reverse |    ✅   |     ✅    |     ❓     |      ❓      |
-| **teraterm**     | reverse|  ❌  |     ✅    | rev/red |    ✅   |     ❌    |     ❓     |      ❓      |
-| **aixterm**      | normal |  ❌  |     ✅    |    ❌   |    ✅   |     ✅    |     ❓     |      ❓      |
-| **Windows**      |   ❌   |  ❌  |     ❌    |    ❌   |    ✅   |   ✅[^4]  |     ❓     |      ✅      |
-| **PuTTY**        | ✅[^2] |  ✅  |     ✅    |  ✅[^1] |    ✅   |     ❌    |     ✅     |      ✅      |
-| **Cygwin SSH**   |   ✅   |  ❌  |    color  |  color  |  color  |     ✅    |     ❓     |      ❓      |
-| **Mac Terminal** |   ✅   |  ❓  |     ✅    |    ✅   |    ✅   |     ✅    |     ✅     |      ❓      |
-| **iTerm2**       |   ✅   |  ❓  |     ✅    |    ✅   |    ✅   |     ✅    |     ✅     |      ✅      |
+| Terminal         |  bold   | dark  | underline |  blink  | reverse | concealed | 256 colors | 24-bit color |
+|:-----------------|:-------:|:-----:|:---------:|:-------:|:-------:|:---------:|:----------:|:------------:|
+| **linux**        |  ❌[^3]  | ❌[^3] |   ✅[^3]   |  ✅[^3]  |    ✅    |     ❌     |     ❌      |      ❌       |
+| **konsole**      |    ✅    |   ✅   |     ✅     |    ✅    |    ✅    |     ✅     |     ✅      |      ✅       |
+| **terminator**   |    ✅    |   ✅   |     ✅     |    ✅    |    ✅    |     ✅     |     ✅      |      ✅       |
+| **kitty**        |    ✅    |   ✅   |     ✅     |    ✅    |    ✅    |     ❌     |     ✅      |      ✅       |
+| **xterm**        |    ✅    |   ❌   |     ✅     |    ✅    |    ✅    |     ✅     |     ✅      |      ✅       |
+| **rxvt**         |    ✅    |   ❌   |     ✅     |    ✅    |    ✅    |     ❌     |     ✅      |      ❌       |
+| **dtterm**       |    ✅    |   ✅   |     ✅     | reverse |    ✅    |     ✅     |     ❓      |      ❓       |
+| **teraterm**     | reverse |   ❌   |     ✅     | rev/red |    ✅    |     ❌     |     ❓      |      ❓       |
+| **aixterm**      | normal  |   ❌   |     ✅     |    ❌    |    ✅    |     ✅     |     ❓      |      ❓       |
+| **Windows**      |    ❌    |   ❌   |     ❌     |    ❌    |    ✅    |   ✅[^4]   |     ❓      |      ✅       |
+| **PuTTY**        |  ✅[^2]  |   ✅   |     ✅     |  ✅[^1]  |    ✅    |     ❌     |     ✅      |      ✅       |
+| **Cygwin SSH**   |    ✅    |   ❌   |   color   |  color  |  color  |     ✅     |     ❓      |      ❓       |
+| **Mac Terminal** |    ✅    |   ❓   |     ✅     |    ✅    |    ✅    |     ✅     |     ✅      |      ❓       |
+| **iTerm2**       |    ✅    |   ❓   |     ✅     |    ✅    |    ✅    |     ✅     |     ✅      |      ✅       |
 
 [^1]: Disabled by default
 
 [^2]: Supports color change, bold text or both.
 
 [^3]: See [VGA text mode](https://en.wikipedia.org/wiki/VGA_text_mode)
 
 [^4]: See [Add support for the "concealed" graphic rendition attribute #6876 ](https://github.com/microsoft/terminal/issues/6876)
-
-
-termcolor_dg changes
-====================
-
-0.9.3 (2022-02-14)
-------------------
-- Adjust the log color scheme.
-- pylint fixes in the color demo.
-
-0.9.2 (2022-02-07)
-------------------
-- Combine color, background and attributes in single escape sequence
-- minor enhancements
-
-0.9.1 (2022-02-05)
-------------------
-- rename to termcolor_dg (termcolor2 is taken)
-
-0.9.0 (2022-02-05)
-------------------
-- fork to termcolor2
-- add 24-bit colors support
-- add logging and color demos
-- add ANSI_COLORS_DISABLED and ANSI_COLORS_FORCE environment variables
-- add always_colored, rainbow_color
-- add monkey_patch_logging and logging_basic_color_config utility functions
-- better cprint and print compatibility (no arguments = new line)
-- drop 'gray' and 'on_gray' (it was an alias for black, bad idea?)
-- make trailing reset sequence optional for colored
-- `python -m build` to build the project
-- remove regex usage, the following would have not been stripped but works: `echo -e '(\e[01;32mx\e[1;0033mx\e[m)'`
-- remove PKG-INFO
-- README.md instead of README.rst
-- ... unit tests, INSTALL ...
-
----
-
-termcolor changes
-=================
-
-1.9.1 (2021-12-15)
-------------------
-- python 2 and 3 compatibility, avoid KeyError
-- make pylint happy
-- fix character escapes
-- better .gitignore
-- fix __ALL__ to __all__
-
-1.1.0 (2011-01-13)
-------------------
-- Added cprint function.
-
-1.0.1 (2011-01-13)
-------------------
-- Updated README.rst.
-
-1.0.0 (2011-01-13)
-------------------
-- Changed license to MIT.
-- Updated copyright.
-- Refactored source code.
-
-0.2 (2010-09-07)
-------------------
-- Added support of Python 3.x.
-
-0.1.2 (2009-06-04)
-------------------
-- Fixed bold characters. (Thanks Tibor Fekete)
-
-0.1.1 (2009-03-05)
-------------------
-- Some refactoring.
-- Updated copyright.
-- Fixed reset colors.
-- Updated documentation.
-
-0.1 (2008-06-09)
-----------------
-- Initial release.
```

### Comparing `termcolor_dg-0.9.3.2/color_logs.png` & `termcolor_dg-1.0.0/color_logs.png`

 * *Files identical despite different names*

### Comparing `termcolor_dg-0.9.3.2/colors.png` & `termcolor_dg-1.0.0/colors.png`

 * *Files identical despite different names*

### Comparing `termcolor_dg-0.9.3.2/setup.cfg` & `termcolor_dg-1.0.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [metadata]
 name = termcolor_dg
 version = attr: termcolor_dg.__version__
-url = https://gitlab.com/dngunchev/termcolor_dg
+url = https://github.com/gunchev/termcolor_dg/
 project_urls = 
-	Bug Tracker = https://gitlab.com/dngunchev/termcolor_dg/-/issues
+	Source = https://github.com/gunchev/termcolor_dg/
+	Bug Tracker = https://github.com/gunchev/termcolor_dg/issues/
+	Documentation = https://github.com/gunchev/termcolor_dg/blob/master/README.md
 description = ANSI Color formatting for terminal output and log coloring
 long_description = file: README.md, CHANGES.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 platforms = any
 test_suite = test
```

### Comparing `termcolor_dg-0.9.3.2/setup.py` & `termcolor_dg-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `termcolor_dg-0.9.3.2/src/termcolor_dg.py` & `termcolor_dg-1.0.0/src/termcolor_dg.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 # Original author: Konstantin Lepa <konstantin.lepa@gmail.com>
 
-'''ANSI Color formatting for terminal output and logging coloring.
+"""ANSI Color formatting for terminal output and logging coloring.
 
 Run `python -m termcolor_dg` for color demo
 
 Run `python -m termcolor_dg logs` for colored logs demo
-'''
+"""
 
 from __future__ import absolute_import, print_function, division
 
 import logging
 import os
 import shutil
 import sys
 import time
 
 
 __all__ = ['always_colored', 'colored', 'cprint', 'rainbow_color', 'monkey_patch_logging', 'logging_basic_color_config',
            'COLOR_RESET_STR']
 
-__version__ = '0.9.3.2'
+__version__ = '1.0.0'
 __copyright__ = 'Copyright (c) 2008-2011 Volvox Development Team'
 __license__ = 'MIT'
 
 __author__ = 'Konstantin Lepa'
 __email__ = 'konstantin.lepa@gmail.com'
 
 __maintainer__ = 'Doncho N. Gunchev'
@@ -58,16 +58,16 @@
 # Python 2 and 3 compatibility
 if sys.version_info >= (3, 0):  # pragma: no cover
     # raw_input = input  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     # unicode = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     basestring = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     # long = int  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
 
-DISABLED = not (os.getenv('ANSI_COLORS_DISABLED') or os.getenv('NO_COLOR')) \
-    and (not sys.stdout.isatty() or os.getenv('ANSI_COLORS_FORCE'))
+DISABLED = (os.getenv('ANSI_COLORS_DISABLED') is not None or os.getenv('NO_COLOR') is not None) \
+           or (not sys.stdout.isatty() and os.getenv('ANSI_COLORS_FORCE') is None)
 
 COLOR_RESET_STR = '\033[0m'
 ERASE_EOL_STR = '\033[2K'
 RESET_STR = '\033c'
 
 ATTRIBUTES = {
     'bold': '1',
@@ -97,15 +97,15 @@
     'white': '97',
 }
 
 HIGHLIGHTS = dict((i[0], str(int(i[1]) + 10)) for i in COLORS.items())
 
 
 def color_fmt(color, colors16, cnum):
-    '''Format the color/background escape sequence chunk'''
+    """Format the color/background escape sequence chunk"""
     if isinstance(color, basestring):
         if color.startswith('on_'):  # backwards compatibility
             color = color[3:]
         if color in colors16:
             return colors16[color]
         raise ValueError("Invalid color %r" % color)
 
@@ -119,15 +119,15 @@
             return '%d;2;%d;%d;%d' % (cnum, color[0], color[1], color[2])
         raise ValueError("Invalid color %r" % (color,))
 
     raise TypeError("Unsupported color type %s" % type(color).__name__)
 
 
 def always_colored(text, color=None, on_color=None, attrs=None, reset=True):
-    '''Color text with ANSI escape codes
+    """Color text with ANSI escape codes
 
     color (text color): 'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'light_grey', 'dark_grey',
         'light_red', 'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan', 'white'.
 
     on_color (text background): same as color but with 'on_' or 'on ' prefix.
 
     attributes: 'bold', 'dark', 'underline', 'blink', 'reverse', 'concealed'.
@@ -137,15 +137,15 @@
     Additionally, if 256 colors are supported, any integer between 1 and 255 can be provided for both foreground
     and background. A tuple/list with three integers (R, G, B) can be provided for 24 bit color.
 
     Examples:
         always_colored('Hello, World!', 'red', 'on_black', ['bold', 'blink'])
         always_colored('Hello, World!', 191, 182)
         always_colored('24bit color!', (255, 127, 127), (127, 127, 255), ['bold'])
-    '''
+    """
     pfx = []
     if color is not None:
         pfx.append(color_fmt(color, COLORS, 38))
 
     if on_color is not None:
         pfx.append(color_fmt(on_color, HIGHLIGHTS, 48))
 
@@ -159,15 +159,15 @@
     if pfx:
         return '\033[' + ';'.join(pfx) + 'm' + text + (COLOR_RESET_STR if reset else '')
 
     return text
 
 
 def colored(text, color=None, on_color=None, attrs=None, reset=True):
-    '''Color text with ANSI escape codes if running on terminal (or overridden).
+    """Color text with ANSI escape codes if running on terminal (or overridden).
 
     Environment variables:
         - **ANSI_COLORS_FORCE**: any value (even empty) will force colorizing the text.
         - **ANSI_COLORS_DISABLED** any value (even empty) will disable colorization. Takes precedence.
 
     Available text colors:
         red, green, yellow, blue, magenta, cyan, white, black, light_grey, dark_grey, light_red, light_green,
@@ -183,32 +183,31 @@
     Available attributes:
         bold, dark, underline, blink, reverse, concealed.
 
     Examples:
         colored('Hello, World!', 'red', 'on_black', ['bold', 'blink'])
         colored('Hello, World!', 191, 182)
         colored('24bit color!', (255, 127, 127), (127, 127, 255), ['bold'])
-    '''
+    """
     if DISABLED:
         return text
 
     return always_colored(text, color, on_color, attrs, reset)
 
 
 def cprint(text='', color=None, on_color=None, attrs=None, reset=True, **kwargs):
-    '''
-    Print colorized text.
+    """Print colorized text.
 
     It accepts arguments of print function.
-    '''
+    """
     print(colored(text, color, on_color, attrs, reset), **kwargs)
 
 
 def rainbow_color(n, steps, nmax=255):
-    '''Calculate rainbow color'''
+    """Calculate rainbow color"""
     if not isinstance(n, int) and isinstance(steps, int):
         raise TypeError('Arguments must be integers')
     if steps < 6:
         raise ValueError('Total must be at least 6')
 
     n %= steps
     progress = float(n) / steps
@@ -222,63 +221,64 @@
     progress = float(n) / steps
     b_value = max(0, min(nmax, abs(3 * nmax - 6 * progress * nmax) - nmax))
 
     return round(r_value), round(g_value), round(b_value)
 
 
 def monkey_patch_logging_format():
-    '''Monkey patches the logging module format error report'''
+    """Monkey patches the logging module format error report"""
     if getattr(logging.LogRecord, 'distGetMessage', None) is not None:
         return
 
     logging.LogRecord.distGetMessage = logging.LogRecord.getMessage
 
     def print_log_record_on_error(func):
-        '''Monkeypatch for logging.LogRecord.getMessage
+        """Monkeypatch for logging.LogRecord.getMessage
 
-        Credits: https://stackoverflow.com/questions/2477934/'''
+        Credits: https://stackoverflow.com/questions/2477934/"""
 
         def wrap(self, *args, **kwargs):
-            '''Generate wrapper function for logging.LogRecord.getMessage'''
+            """Generate wrapper function for logging.LogRecord.getMessage"""
             try:
                 return func(self, *args, **kwargs)
             except Exception as exc:  # pylint: disable=broad-except
                 return 'Error logging msg=%r, args=%r: %r' \
                     % (getattr(self, 'msg', '?'), getattr(self, 'args', '?'), exc)
 
         return wrap
 
     # Monkeypatch the logging library for more informative formatting errors
     logging.LogRecord.getMessage = print_log_record_on_error(logging.LogRecord.getMessage)
 
 
 def monkey_unpatch_logging_format():
-    '''Undo monkey_patch_logging_format'''
+    """Undo monkey_patch_logging_format"""
     if getattr(logging.LogRecord, 'distGetMessage', None) is None:
         return
+    # noinspection PyUnresolvedReferences
     logging.LogRecord.getMessage = logging.LogRecord.distGetMessage  # @UndefinedVariable
     delattr(logging.LogRecord, 'distGetMessage')
 
 
 def monkey_patch_logging(color_on_terminal=True):
-    '''Monkey patches the logging module and add colors if enabled'''
+    """Monkey patches the logging module and add colors if enabled"""
 
     if getattr(logging, 'DistFormatter', None) is not None:
         return True
 
     monkey_patch_logging_format()
 
     if color_on_terminal and not DISABLED:
         # Monkey patches the logging module to print in color'
 
         def get_formatter(logging_formatter=logging.Formatter):
-            '''Get it? ;-)'''
+            """Get it? ;-)"""
 
             class ColoredFormatter(logging_formatter):
-                '''Color console formatter'''
+                """Color console formatter"""
 
                 def format(self, record):
                     output = logging_formatter.format(self, record)
                     tail = None
                     comment_pos = output.find('  # ')  # Intentionally require two spaces before
                     if comment_pos >= 0:
                         output, tail = output[:comment_pos], output[comment_pos:]
@@ -295,57 +295,55 @@
                         output = colored(text=output, color='red', on_color=None, attrs=['bold'])
                     elif record.levelno <= logging.CRITICAL:
                         output = colored(text=output, color='white', on_color='on_red', attrs=['bold'])
                     else:
                         output = colored(text=output, color='yellow', on_color='on_red',
                                          attrs=['bold', 'underline'])
                     if tail:
-                        output += colored(text=tail, color='black', attrs=['dark'])
+                        output += colored(text=tail, color='black', attrs='dark')
 
                     return output
 
                 def formatException(self, ei):
-                    '''Format and return the specified exception information as a string.'''
+                    """Format and return the specified exception information as a string."""
                     text = logging_formatter.formatException(self, ei)
                     text = '\n'.join(ERASE_EOL_STR + i for i in text.splitlines())
-                    return colored(text=text, color='white', on_color='on_magenta', attrs=('bold'))
+                    return colored(text=text, color='white', on_color='on_magenta', attrs='bold')
 
             return ColoredFormatter
 
         logging.DistFormatter = logging.Formatter
         logging.Formatter = get_formatter()
 
     return True
 
 
 def monkey_unpatch_logging():
-    '''Undo monkey_patch_logging'''
+    """Undo monkey_patch_logging"""
 
     monkey_unpatch_logging_format()
 
     if getattr(logging, 'DistFormatter', None) is not None:
+        # noinspection PyUnresolvedReferences
         logging.Formatter = logging.DistFormatter  # @UndefinedVariable
         delattr(logging, 'DistFormatter')
 
 
 def logging_basic_color_config(level='DEBUG', fmt='%(asctime)s %(message)s  # %(filename)s:%(lineno)d %(name)s',
                                color_on_terminal=True):
-    '''Setup basic logging with fancy format and colors if running on terminal
+    """Setup basic logging with fancy format and colors if running on terminal
 
     a very fancy fmt would be "%(asctime)s %(levelname)-8s: %(message)s  # %(filename)s:%(lineno)d %(name)s"
-    '''
+    """
     monkey_patch_logging(color_on_terminal=color_on_terminal)
-    try:
-        logging.basicConfig(level=level, format=fmt, disable_existing_loggers=False)
-    except ValueError:
-        logging.basicConfig(level=level, format=fmt)
+    logging.basicConfig(level=level, format=fmt)
 
 
 def termcolor_demo_16():
-    '''Base 16 color demo'''
+    """Base 16 color demo"""
     colors = ('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'light_grey', 'dark_grey', 'light_red',
               'light_green', 'light_yellow', 'light_blue', 'light_magenta', 'light_cyan', 'white')
     max_len = max(len(color) for color in colors)
 
     print(RESET_STR, end='')
     print(('--- 16 color mode test on TERM=%r ' % os.getenv('TERM')).ljust(119, '-'))
 
@@ -387,15 +385,15 @@
     print(' [' + colored('Dark blink concealed white', 'white', attrs=['dark', 'blink', 'concealed']), end=']\n')
     print(' [' + '      Reversed blue       ', end=']')
     print(' [' + '    Concealed Magenta     ', end=']')
     print(' [' + 'Bold underline reverse red', end=']')
     print(' [' + 'Dark blink concealed white', end=']\n')
 
     def all_combos(values):
-        '''Generate all combinations'''
+        """Generate all combinations"""
         values = tuple(values)
         if values:
             for i in all_combos(values[1:]):
                 yield i
                 yield [values[0]] + i
         else:
             yield []
@@ -408,15 +406,15 @@
         code += 'K' if 'blink' in attrs else 'k'
         code += 'R' if 'reverse' in attrs else 'r'
         code += 'C' if 'concealed' in attrs else 'c'
         print(' [' if idx % 16 == 0 else ' ' + colored(code, attrs=attrs), end='' if idx % 16 != 15 else ' ]\n')
 
 
 def termcolor_demo_256():
-    '''256 color demo'''
+    """256 color demo"""
     print('\n--- 256 color mode test '.ljust(120, '-'))
     print(' First 16: [', end='')
     for i in range(16):
         cprint('%3d ' % i, color=15 - i, on_color=i, end='', reset=i == 15)
     print(']')
 
     print()
@@ -436,15 +434,15 @@
     for i in range(232, 256):
         # cprint('%4d' % i, color='white' if i < 244 else 'black', on_color=i, end='')
         cprint('%4d' % i, color=(232 + 255) - i, on_color=i, end='')
     print(']\n')
 
 
 def termcolor_demo_24bit():
-    '''24 bit color demo'''
+    """24 bit color demo"""
     data = '=== 24 bit color mode test '.ljust(114, '=')
     for i in range(2 * len(data), -1, -1):
         print('\r   ', end='')
         grey = abs(i * 8 % 510 - 255)
         print(
             colored(
                 ''.join(colored(char, on_color=rainbow_color(step + i, len(data)), reset=False)
@@ -464,40 +462,41 @@
         time.sleep(0.02)
         print(COLOR_RESET_STR, end='')
 
     print()
 
 
 def get_term_width():
-    '''Get terminal width, there is https://gist.github.com/mr700/c73af70357ff8bcfc3250ee6c84e164d but it is overkill'''
+    """Get terminal width, https://gist.github.com/mr700/c73af70357ff8bcfc3250ee6c84e164d, is an overkill."""
     try:
         return shutil.get_terminal_size(fallback=(80, 32)).columns  # @UndefinedVariable
     except AttributeError:  # pragma: no cover
-        return 120          # pragma: no cover
+        return 120  # pragma: no cover
 
 
 def termcolor_demo():
-    '''Demonstrate this module's capabilities'''
+    """Demonstrate this module's capabilities"""
     termcolor_demo_16()
     termcolor_demo_256()
-    if get_term_width() >= 120:
+    if get_term_width() >= 120 or os.getenv('ANSI_COLORS_FORCE') is not None:
         termcolor_demo_24bit()
     else:
         print("Need terminal width of 120 or more for this part...")  # pragma: no cover
 
 
 def color_log_demo():
-    '''Test color logging on terminal and logging format error'''
+    """Test color logging on terminal and logging format error"""
     # monkey_patch_logging(color_on_terminal=True)
     logging_basic_color_config()
 
     log = logging.getLogger('logger')
     print('Logging test... levels and exception:')
 
     # Hack to skip the log level test
+    # noinspection PyTypeChecker
     log._log(logging.NOTSET, 'Not set, below DEBUG, normally not show...', [])  # pylint: disable=W0212
     log.debug('Debug')
     log.info('Info')
     log.warning('Warning')
     log.error('Error')
     log.critical('Critical')
     log.error('x', 1)  # the mistake is intentional pylint: disable=logging-too-many-args
@@ -508,15 +507,15 @@
     except TypeError:
         log.exception('Exception')
     log.log(51, 'ABOVE CRITICAL!')
     log.info('Done.')
 
 
 def main():
-    '''Main demo entry point, if no arguments - color demo, if any - colored logs demo'''
-    if len(sys.argv) == 1:       # pragma: no cover
+    """Main demo entry point, if no arguments - color demo, if any - colored logs demo"""
+    if len(sys.argv) == 1:  # pragma: no cover
         return termcolor_demo()  # pragma: no cover
-    return color_log_demo()      # pragma: no cover
+    return color_log_demo()  # pragma: no cover
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `termcolor_dg-0.9.3.2/termcolor_dg.spec` & `termcolor_dg-1.0.0/termcolor_dg.spec`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 %{?!python3_pkgversion:%global python3_pkgversion 3}
 
 %global srcname termcolor_dg
 
 Name:           python-%{srcname}
-Version:        0.9.3.2
+Version:        1.0.0
 Release:        0%{?dist}
 Summary:        ANSI Color formatting for terminal output and log coloring.
 License:        MIT
-URL:            https://gitlab.com/dngunchev/%{srcname}
-Source0:        https://gitlab.com/dngunchev/%{srcname}/-/archive/v%{version}/%{srcname}-%{version}.tar.gz
+URL:            https://github.com/gunchev/termcolor_dg/%{srcname}
+Source0:        https://github.com/gunchev/%{srcname}/archive/refs/tags/v%{version}.tar.gz?name=%{srcname}-%{version}.tar.gz
 
 BuildArch:      noarch
 
 BuildRequires:  python%{python3_pkgversion}-devel
 BuildRequires:  python%{python3_pkgversion}-setuptools
 BuildRequires:  python%{python3_pkgversion}-check-manifest >= 0.42
 BuildRequires:  python%{python3_pkgversion}-coverage
@@ -40,39 +40,62 @@
 ANSI Color formatting for terminal output and log coloring.
 Supports 16 color, 256 color and 24-bit color modes.
 
 Python 2 support is present for legacy projects and because
 it is not too much work and I have to use it for now.
 
 
+%package -n python%{python3_pkgversion}-%{srcname}-bin
+Summary:  %{summary}
+Requires: python%{python3_pkgversion}-%{srcname}
+
+%description -n python%{python3_pkgversion}-%{srcname}-bin
+binary files for %{srcname}, you can simply:
+
+    python -m termcolor_dg
+
+or
+
+    python -m termcolor_dg logs
+
+
 %prep
 %autosetup -p1 -n %{srcname}-%{version}
 
 
 %build
 %py3_build
 
 
 %install
-rm -rf $RPM_BUILD_ROOT
+rm -rf "$RPM_BUILD_ROOT"
 %py3_install
 
 
 %check
 make test
 
 
 %files -n  python%{python3_pkgversion}-%{srcname}
 %license LICENSE
 %doc CHANGES.md README.md INSTALL.md TODO.md
-# binaries
-%{_bindir}/termcolor_dg_demo
-%{_bindir}/termcolor_dg_demo_log
-# For noarch packages: sitelib
 %{python3_sitelib}/%{srcname}.py
 %{python3_sitelib}/%{srcname}-%{version}-py%{python3_version}.egg-info/
 %{python3_sitelib}/__pycache__/%{srcname}*
 
 
+%files -n  python%{python3_pkgversion}-%{srcname}-bin
+# binaries
+%{_bindir}/termcolor_dg_demo
+%{_bindir}/termcolor_dg_demo_log
+
+
 %changelog
+* Thu May 25 2023 Doncho N. Gunchev <dgunchev@gmail.com> - 1.0.0-0
+- Fix logging.basicConfig has no disable_existing_loggers argument.
+- fix DISABLED detection
+
+* Wed Jan 11 2023 Doncho N. Gunchev <dgunchev@gmail.com> - 0.9.3.2-1
+- Move the executables to -bin subpackage. Not too useful.
+
 * Wed Jan 11 2023 Doncho N. Gunchev <dgunchev@gmail.com> - 0.9.3.2-0
 - Initial package
```

### Comparing `termcolor_dg-0.9.3.2/test/test_termcolor_dg.py` & `termcolor_dg-1.0.0/test/test_termcolor_dg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-'''termcolor_dg unit tests'''
+"""termcolor_dg unit tests"""
 
 from __future__ import absolute_import, print_function, division
 
 import io
 import logging
+import os
 import re
 import sys
 import time
 import unittest
 
 import termcolor_dg
 
@@ -20,118 +21,126 @@
     raw_input = input  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     unicode = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     basestring = str  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
     long = int  # @ReservedAssignment pylint: disable=C0103,redefined-builtin
 
 
 class CapturedOutput:
-    '''Temporary replace sys.stdout and sys.stderr with io.StringIO or io.BytesIO'''
+    """Temporary replace sys.stdout and sys.stderr with io.StringIO or io.BytesIO"""
 
     def __init__(self):
         self._buf = io.BytesIO() if sys.version_info < (3, 0) else io.StringIO()
         self._stdout, self._stderr = sys.stdout, sys.stderr
 
     def __enter__(self):
         sys.stdout, sys.stderr = self._buf, self._buf
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):  # @UnusedVariable
         sys.stderr, sys.stdout = self._stderr, self._stdout
-        return False  # return True  # To stop any exception from propagating
+        return False  # return True # To stop any exception from propagating
 
     def get_output(self):
-        '''Get what was written so far'''
+        """Get what was written so far"""
         return self._buf.getvalue()
 
 
 class Coffeine:
-    '''Temporary replace time.sleep() with pass'''
+    """Temporary replace time.sleep() with pass"""
 
     def __init__(self):
         self._sleep = time.sleep
 
     def __enter__(self):
         time.sleep = lambda _: None
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):  # @UnusedVariable
         time.sleep = self._sleep
-        return False  # return True  # To stop any exception from propagating
+        return False  # return True # To stop any exception from propagating
 
 
 class TestTermcolorDg(unittest.TestCase):
-    '''Test the termcolor_dg module'''
+    """Test the termcolor_dg module"""
 
     def __init__(self, methodName='runTest'):
         unittest.TestCase.__init__(self, methodName=methodName)
         self._disabled = termcolor_dg.DISABLED
 
     def setUp(self):
         unittest.TestCase.setUp(self)
         termcolor_dg.DISABLED = False
 
+        def get_term_width():
+            """Return a fake width of the terminal"""
+            return 120
+
+        termcolor_dg.get_term_width = get_term_width
+
     def tearDown(self):
         unittest.TestCase.tearDown(self)
         termcolor_dg.DISABLED = self._disabled
 
     def test_main_exists(self):
-        '''Check if main is defined in the module'''
+        """Check if main is defined in the module"""
         for fname in ('always_colored', 'colored', 'cprint', 'rainbow_color', 'monkey_patch_logging',
                       'logging_basic_color_config', 'monkey_unpatch_logging', 'monkey_unpatch_logging_format'):
             self.assertIn(fname, termcolor_dg.__dict__.keys(), '%r not defined?!?' % fname)
 
     def test_cprint_no_color(self):
-        '''Check if main is printing the proper string'''
+        """Check if main is printing the proper string"""
         with CapturedOutput() as out:
             termcolor_dg.cprint('test')
             output = out.get_output()
         self.assertEqual(output, 'test\n')
 
     # @unittest.skipIf(not sys.stdout.isatty(), 'Not testing on non-tty')
     def test_cprint(self):
-        '''Check if main is printing the proper string'''
+        """Check if main is printing the proper string"""
         with CapturedOutput() as out:
             termcolor_dg.cprint('test')
             output = out.get_output()
         self.assertEqual(output, 'test\n')
 
     def test_colored(self):
-        '''Basics'''
+        """Basics"""
         self.assertEqual(termcolor_dg.colored('test', 'red'), '\x1b[31mtest\x1b[0m')
         self.assertEqual(termcolor_dg.colored('test', color='red'), '\x1b[31mtest\x1b[0m')
         self.assertEqual(termcolor_dg.colored('test', 2), '\x1b[38;5;2mtest\x1b[0m')
         self.assertEqual(termcolor_dg.colored('test', (0, 0, 255)), '\x1b[38;2;0;0;255mtest\x1b[0m')
 
         self.assertEqual(termcolor_dg.colored('test', on_color='on_red'), '\x1b[41mtest\x1b[0m')
         self.assertEqual(termcolor_dg.colored('test', on_color=2), '\x1b[48;5;2mtest\x1b[0m')
         self.assertEqual(termcolor_dg.colored('test', None, (0, 0, 255)), '\x1b[48;2;0;0;255mtest\x1b[0m')
 
         self.assertEqual(termcolor_dg.colored('test', 'red', 'on_blue', ['bold']), '\x1b[31;44;1mtest\x1b[0m')
         self.assertEqual(termcolor_dg.colored('test', 'red', 'on_blue', ['bold'], reset=False), '\x1b[31;44;1mtest')
 
         termcolor_dg.DISABLED = True
         self.assertEqual(termcolor_dg.colored('test', 'red'), 'test')
+        termcolor_dg.DISABLED = False
+        self.assertNotEqual(termcolor_dg.colored('test', 'red'), 'test')
 
     def test_always_colored(self):
-        '''Basics'''
+        """Basics"""
         self.assertEqual(termcolor_dg.always_colored('test', 'red'), '\x1b[31mtest\x1b[0m')
         self.assertEqual(termcolor_dg.always_colored('test', color='red'), '\x1b[31mtest\x1b[0m')
         self.assertEqual(termcolor_dg.always_colored('test', 2), '\x1b[38;5;2mtest\x1b[0m')
         self.assertEqual(termcolor_dg.always_colored('test', (0, 0, 255)), '\x1b[38;2;0;0;255mtest\x1b[0m')
 
         self.assertEqual(termcolor_dg.always_colored('test', on_color='on_red'), '\x1b[41mtest\x1b[0m')
         self.assertEqual(termcolor_dg.always_colored('test', on_color=2), '\x1b[48;5;2mtest\x1b[0m')
         self.assertEqual(termcolor_dg.always_colored('test', None, (0, 0, 255)), '\x1b[48;2;0;0;255mtest\x1b[0m')
 
         self.assertEqual(termcolor_dg.always_colored('test', 'red', 'on_blue', ['bold']), '\x1b[31;44;1mtest\x1b[0m')
         self.assertEqual(termcolor_dg.always_colored('test', 'red', 'on_blue', ['bold'], reset=False),
                          '\x1b[31;44;1mtest')
 
     def test_rainbow_color(self):
-        '''Test rainbow_color'''
+        """Test rainbow_color"""
         self.assertEqual(termcolor_dg.rainbow_color(0, 18), (255, 0, 0))
         self.assertEqual(termcolor_dg.rainbow_color(1, 18), (255, 85, 0))
         self.assertEqual(termcolor_dg.rainbow_color(2, 18), (255, 170, 0))
         self.assertEqual(termcolor_dg.rainbow_color(3, 18), (255, 255, 0))
         self.assertEqual(termcolor_dg.rainbow_color(4, 18), (170, 255, 0))
         self.assertEqual(termcolor_dg.rainbow_color(5, 18), (85, 255, 0))
         self.assertEqual(termcolor_dg.rainbow_color(6, 18), (0, 255, 0))
@@ -150,15 +159,15 @@
             termcolor_dg.rainbow_color('17', 18)
         with self.assertRaises(TypeError):
             termcolor_dg.rainbow_color(17, '18')
         with self.assertRaises(ValueError):
             termcolor_dg.rainbow_color(5, 2)
 
     def test_log_demo(self):
-        '''Check the log demo output'''
+        """Check the log demo output"""
         with CapturedOutput() as out:
             termcolor_dg.color_log_demo()
             output = out.get_output()
 
         self.assertTrue(termcolor_dg.monkey_patch_logging())
 
         head_expected = 'Logging test... levels and exception:\n\x1b[30;44;2m'
@@ -214,26 +223,30 @@
         termcolor_dg.monkey_unpatch_logging()
         termcolor_dg.DISABLED = True
         self.assertTrue(termcolor_dg.monkey_patch_logging())
         self.assertTrue(termcolor_dg.monkey_patch_logging())
         termcolor_dg.DISABLED = False
 
     def test_color_demo(self):
-        '''Check the log demo output'''
+        """Check the log demo output"""
+        os.environ['ANSI_COLORS_FORCE'] = '1'
         with CapturedOutput() as out, Coffeine() as a_stimulant:  # @UnusedVariable pylint: disable=unused-variable
             termcolor_dg.termcolor_demo()
             output = out.get_output()
 
+        if len(output) != 477595:
+            print("Bad output, len =", len(output))
+            print(output)
         self.assertEqual(len(output), 477595, "Unexpected output size")
         self.assertEqual(output[:33], '\x1bc--- 16 color mode test on TERM=', 'Bad output start')
         tail = ';40m=\x1b[0m\x1b[38;2;0;27;255;48;2;255;0;27m=\x1b[0m\x1b[38;2;0;13;255;48;2;255;0;13m=\x1b[0m\n'
         self.assertEqual(output[-80:], tail, 'Bad output tailing 80 chars')
 
     def test_errors(self):
-        '''Check exceptions are thrown'''
+        """Check exceptions are thrown"""
         # Color exceptions
         with self.assertRaises(ValueError):
             termcolor_dg.always_colored('', 'invalid_color')
         with self.assertRaises(ValueError):
             termcolor_dg.always_colored('', 256)
         with self.assertRaises(ValueError):
             termcolor_dg.always_colored('', -1)
```

### Comparing `termcolor_dg-0.9.3.2/tox.ini` & `termcolor_dg-1.0.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://tox.wiki/en/latest/example/basic.html
 # https://github.com/pypa/sampleproject/blob/main/tox.ini
 
 [tox]
-envlist = py3{10,6,7,8,9},py27,pypy{2,3}
+envlist = py27,py3{6,7,8,9,11},pypy{2,3}
 # At least this version is needed for PEP 517/518 support.
 minversion = 3.3.0
 # Activate isolated build environment. tox will use a virtual environment
 # to build a source distribution from the source tree. For build tools and
 # arguments use the pyproject.toml file as specified in PEP-517 and PEP-518.
 isolated_build = true
 
@@ -18,14 +18,36 @@
 deps =
     pylint
 commands =
     python -m unittest discover --verbose -s test {posargs}
     pylint setup.py src/termcolor_dg.py test/test_termcolor_dg.py
 
 
+# Python 2
+[testenv:py27]
+setenv =
+    PYTHONPATH = {toxinidir}{:}{toxinidir}/src{:}{toxinidir}/test
+deps =
+    pylint
+commands =
+    python -m unittest discover --verbose -s test {posargs}
+    pylint --rcfile .pylintrc2 setup.py src/termcolor_dg.py test/test_termcolor_dg.py
+
+
+# pypy 2
+[testenv:pypy2]
+setenv =
+    PYTHONPATH = {toxinidir}{:}{toxinidir}/src{:}{toxinidir}/test
+deps =
+    pylint
+commands =
+    python -m unittest discover --verbose -s test {posargs}
+    pylint --rcfile .pylintrc2 setup.py src/termcolor_dg.py test/test_termcolor_dg.py
+
+
 # Detailed with formatting and stuff - only on the latest
 [testenv:py310]
 setenv =
     PYTHONPATH = {toxinidir}{:}{toxinidir}/src{:}{toxinidir}/test
 deps =
     # check-manifest >= 0.42
     readme_renderer  # confirms your long_description will render correctly on PyPI.
@@ -43,8 +65,8 @@
     pylint setup.py src/termcolor_dg.py test/test_termcolor_dg.py
 
 
 [flake8]
 exclude = .tox, *.egg, build, data, .git, .eggs, __pycache__, test/, docs/, build/, dist/
 select = E,W,F
 max-line-length = 120
-ignore=E226, N818, E24, E704, E126, E123, W503, E121, W504, E241
+ignore = E226, N818, E24, E704, E126, E123, W503, E121, W504, E241
```

