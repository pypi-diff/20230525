# Comparing `tmp/sinol-make-0.0.1.tar.gz` & `tmp/sinol-make-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-0.0.1.tar", last modified: Mon May 22 16:18:21 2023, max compression
+gzip compressed data, was "sinol-make-1.0.0.tar", last modified: Thu May 25 10:51:32 2023, max compression
```

## Comparing `sinol-make-0.0.1.tar` & `sinol-make-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.804607 sinol-make-0.0.1/
--rw-r--r--   0 planeg    (1000) planeg    (1000)    35147 2023-05-22 16:14:31.000000 sinol-make-0.0.1/LICENSE
--rw-r--r--   0 planeg    (1000) planeg    (1000)      915 2023-05-22 16:18:21.804607 sinol-make-0.0.1/PKG-INFO
--rw-r--r--   0 planeg    (1000) planeg    (1000)      306 2023-05-22 16:14:31.000000 sinol-make-0.0.1/README.md
--rw-r--r--   0 planeg    (1000) planeg    (1000)      856 2023-05-22 16:14:31.000000 sinol-make-0.0.1/pyproject.toml
--rw-r--r--   0 planeg    (1000) planeg    (1000)       38 2023-05-22 16:18:21.804607 sinol-make-0.0.1/setup.cfg
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.801273 sinol-make-0.0.1/src/
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.804607 sinol-make-0.0.1/src/sinol_make/
--rw-r--r--   0 planeg    (1000) planeg    (1000)      823 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/__init__.py
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.801273 sinol-make-0.0.1/src/sinol_make/commands/
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.804607 sinol-make-0.0.1/src/sinol_make/commands/run/
--rw-r--r--   0 planeg    (1000) planeg    (1000)    25781 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 planeg    (1000) planeg    (1000)      348 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.804607 sinol-make-0.0.1/src/sinol_make/helpers/
--rw-r--r--   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 planeg    (1000) planeg    (1000)     1783 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/helpers/compile.py
--rw-r--r--   0 planeg    (1000) planeg    (1000)     1344 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/helpers/compiler.py
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.804607 sinol-make-0.0.1/src/sinol_make/interfaces/
--rw-r--r--   0 planeg    (1000) planeg    (1000)      272 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 planeg    (1000) planeg    (1000)      133 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/interfaces/__init__.py
--rw-r--r--   0 planeg    (1000) planeg    (1000)     4525 2023-05-22 16:14:31.000000 sinol-make-0.0.1/src/sinol_make/util.py
-drwxr-xr-x   0 planeg    (1000) planeg    (1000)        0 2023-05-22 16:18:21.804607 sinol-make-0.0.1/src/sinol_make.egg-info/
--rw-r--r--   0 planeg    (1000) planeg    (1000)      915 2023-05-22 16:18:21.000000 sinol-make-0.0.1/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 planeg    (1000) planeg    (1000)      610 2023-05-22 16:18:21.000000 sinol-make-0.0.1/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 planeg    (1000) planeg    (1000)        1 2023-05-22 16:18:21.000000 sinol-make-0.0.1/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 planeg    (1000) planeg    (1000)       47 2023-05-22 16:18:21.000000 sinol-make-0.0.1/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 planeg    (1000) planeg    (1000)       52 2023-05-22 16:18:21.000000 sinol-make-0.0.1/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 planeg    (1000) planeg    (1000)       11 2023-05-22 16:18:21.000000 sinol-make-0.0.1/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.174860 sinol-make-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 10:51:21.000000 sinol-make-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 10:51:32.174860 sinol-make-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-25 10:51:21.000000 sinol-make-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 10:51:21.000000 sinol-make-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:51:32.174860 sinol-make-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/helpers/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.174860 sinol-make-1.0.0/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/top_level.txt
```

### Comparing `sinol-make-0.0.1/LICENSE` & `sinol-make-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-0.0.1/PKG-INFO` & `sinol-make-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 0.0.1
+Version: 1.0.0
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # sinol-make
 CLI tool for creating sio2 task packages. \
 Currently in development and not yet ready to be used.
```

### Comparing `sinol-make-0.0.1/pyproject.toml` & `sinol-make-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sinol-make"
-version = "0.0.1"
+dynamic = ["version"]
 authors = [
   { name="Mateusz Masiarz", email="m.masiarz@fri.edu.pl" }
 ]
 maintainers = [
   { name="Tomasz Nowak", email="tomasz.nowak@tonowak.com" }
 ]
 description = "CLI tool for creating sio2 task packages"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
 	"argparse",
 	"requests",
 	"PyYAML",
 	"dictdiffer"
 ]
 
 [project.optional-dependencies]
 tests = [
-  "pytest"
+  "pytest",
+  "pytest-cov"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sio2project/sinol-make"
 "Bug Tracker" = "https://github.com/sio2project/sinol-make/issues"
 
 [project.scripts]
 sinol-make = "sinol_make:main"
+
+[tool.setuptools.dynamic]
+version = { attr = "sinol_make.__version__" }
```

### Comparing `sinol-make-0.0.1/src/sinol_make/__init__.py` & `sinol-make-1.0.0/src/sinol_make/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import argparse, pkg_resources
+import argparse
 from sinol_make import util
 
+__version__ = "1.0.0"
+
 def configure_parsers():
 	parser = argparse.ArgumentParser(
 		prog='sinol-make',
 		description='Tool for creating and testing sio2 tasks',
 	)
-	parser.add_argument("-v", "--version", action="version", version="%(prog)s " + pkg_resources.get_distribution('sinol_make').version)
+	parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
 	subparsers = parser.add_subparsers(
 		title='commands',
 		description='sinol-make commands',
 		dest='command',
 	)
 	subparsers.required = False
```

### Comparing `sinol-make-0.0.1/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.0.0/src/sinol_make/commands/run/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,46 +252,50 @@
 				for test in self.tests:
 					all_results[name][self.get_group(test)][test] = {"Status": "CE"}
 		print()
 		executions.sort(key = lambda x: (self.get_executable_key(x[1]), x[2]))
 		program_groups_scores = collections.defaultdict(dict)
 
 		def print_view(output_file=None):
+			def print_stream(*values, end='\n'):
+				if output_file is not None:
+					print(*values, end=end, file=output_file)
+				else:
+					print(*values, end=end)
+
 			if i != 0 and output_file is None:
 				# TODO: always display both tables
 				# if self.args.verbose:
 				# 	cursor_delta = len(self.tests) + len(self.groups)+ 9
 				# 	if not self.args.hide_memory:
 				# 		cursor_delta += len(self.tests)
 				# else:
 				cursor_delta = len(self.groups) + 7
 				number_of_rows = (len(solutions) + self.PROGRAMS_IN_ROW - 1) // self.PROGRAMS_IN_ROW
 				sys.stdout.write('\033[%dA' % (cursor_delta * number_of_rows + 1))
 			program_scores = collections.defaultdict(int)
 			program_times = collections.defaultdict(lambda: -1)
 			program_memory = collections.defaultdict(lambda: -1)
-			if output_file is not None:
-				sys.stdout = open(output_file, 'w')
-			else:
+			if output_file is None:
 				time_remaining = (len(executions) - i - 1) * 2 * self.time_limit / self.cpus / 1000.0
-				print('Done %4d/%4d. Time remaining (in the worst case): %5d seconds.'
+				print_stream('Done %4d/%4d. Time remaining (in the worst case): %5d seconds.'
 					% (i+1, len(executions), time_remaining))
 			for program_ix in range(0, len(names), self.PROGRAMS_IN_ROW):
 				# how to jump one line up
 				program_group = names[program_ix:program_ix + self.PROGRAMS_IN_ROW]
-				print("groups", end=" | ")
+				print_stream("groups", end=" | ")
 				for program in program_group:
-					print("%10s" % program, end=" | ")
-				print()
-				print(6*"-", end=" | ")
+					print_stream("%10s" % program, end=" | ")
+				print_stream()
+				print_stream(6*"-", end=" | ")
 				for program in program_group:
-					print(10*"-", end=" | ")
-				print()
+					print_stream(10*"-", end=" | ")
+				print_stream()
 				for group in self.groups:
-					print("%6s" % group, end=" | ")
+					print_stream("%6s" % group, end=" | ")
 					for program in program_group:
 						results = all_results[program][group]
 						group_status = "OK"
 						for test in results:
 							status = results[test]["Status"]
 							if "Time" in results[test].keys():
 								program_times[program] = max(
@@ -302,67 +306,67 @@
 								program_memory[program] = max(
 									program_memory[program], results[test]["Memory"])
 							elif status == "ML":
 								program_memory[program] = 2 * self.memory_limit
 							if status != "OK":
 								group_status = status
 								break
-						print("%3s" % util.bold(util.color_green(group_status)) if group_status == "OK" else util.bold(util.color_red(group_status)),
+						print_stream("%3s" % util.bold(util.color_green(group_status)) if group_status == "OK" else util.bold(util.color_red(group_status)),
 							"%3s/%3s" % (self.scores[group] if group_status == "OK" else "---", self.scores[group]),
 							end=" | ")
 						program_scores[program] += self.scores[group] if group_status == "OK" else 0
 						program_groups_scores[program][group] = group_status
-					print()
-				print(6*" ", end=" | ")
+					print_stream()
+				print_stream(6*" ", end=" | ")
 				for program in program_group:
-					print(10*" ", end=" | ")
-				print()
-				print("points", end=" | ")
+					print_stream(10*" ", end=" | ")
+				print_stream()
+				print_stream("points", end=" | ")
 				for program in program_group:
-					print(util.bold("   %3s/%3s" % (program_scores[program], self.possible_score)), end=" | ")
-				print()
-				print("  time", end=" | ")
+					print_stream(util.bold("   %3s/%3s" % (program_scores[program], self.possible_score)), end=" | ")
+				print_stream()
+				print_stream("  time", end=" | ")
 				for program in program_group:
 					program_time = program_times[program]
-					print(util.bold(("%20s" % self.color_time(program_time, self.time_limit))
+					print_stream(util.bold(("%20s" % self.color_time(program_time, self.time_limit))
 						if program_time < 2 * self.time_limit and program_time >= 0
 						else "   "+7*'-'), end=" | ")
-				print()
-				print("memory", end=" | ")
+				print_stream()
+				print_stream("memory", end=" | ")
 				for program in program_group:
 					program_mem = program_memory[program]
-					print(util.bold(("%20s" % self.color_memory(program_mem, self.memory_limit))
+					print_stream(util.bold(("%20s" % self.color_memory(program_mem, self.memory_limit))
 						if program_mem < 2 * self.memory_limit and program_mem >= 0
 						else "   "+7*'-'), end=" | ")
-				print()
+				print_stream()
 				# TODO: always display both tables
 				# if self.args.verbose:
-				# 	print(6*" ", end=" | ")
+				# 	print_stream(6*" ", end=" | ")
 				# 	for program in program_group:
-				# 		print(10*" ", end=" | ")
-				# 	print()
+				# 		print_stream(10*" ", end=" | ")
+				# 	print_stream()
 				# 	for test in self.tests:
-				# 		print("%6s" % self.extract_test_no(test), end=" | ")
+				# 		print_stream("%6s" % self.extract_test_no(test), end=" | ")
 				# 		for program in program_group:
 				# 			result = all_results[program][self.get_group(test)][test]
 				# 			status = result["Status"]
-				# 			if status == "  ": print(10*' ', end=" | ")
+				# 			if status == "  ": print_stream(10*' ', end=" | ")
 				# 			else:
-				# 				print("%3s" % self.colorize_status(status),
+				# 				print_stream("%3s" % self.colorize_status(status),
 				# 					("%17s" % self.color_time(result["Time"], self.time_limit)) if "Time" in result.keys() else 7*" ", end=" | ")
-				# 		print()
+				# 		print_stream()
 				# 		if not self.args.hide_memory:
-				# 			print(6*" ", end=" | ")
+				# 			print_stream(6*" ", end=" | ")
 				# 			for program in program_group:
 				# 				result = all_results[program][self.get_group(test)][test]
-				# 				print(("%20s" % self.color_memory(result["Memory"], self.memory_limit))  if "Memory" in result.keys() else 10*" ", end=" | ")
-				# 			print()
-				# 	print()
-				print(10*len(program_group)*' ')
-			sys.stdout = sys.__stdout__
+				# 				print_stream(("%20s" % self.color_memory(result["Memory"], self.memory_limit))  if "Memory" in result.keys() else 10*" ", end=" | ")
+				# 			print_stream()
+				# 	print_stream()
+				print_stream(10*len(program_group)*' ')
+
 			if output_file is not None:
 				os.system('sed -i -r "s/\x1B\[([0-9]{1,3}(;[0-9]{1,2})?)?[mGK]//g" %s' % output_file) # TODO: make this work on Windows
 				print("Report has been saved to", util.bold(output_file))
 				print()
 
 		print("Performing %d executions..." % len(executions))
 		with mp.Pool(self.cpus) as pool:
@@ -470,15 +474,15 @@
 						removed_groups.add(group[0])
 			elif type == "change":
 				if field[1] == "expected": # Results for at least one group has changed
 					solution = field[0]
 					group = field[2]
 					old_result = change[0]
 					result = change[1]
-					changes.append(ResultChange(solution, group, result, old_result))
+					changes.append(ResultChange(solution, group, old_result, result))
 
 		return ValidationResult(
 			added_solutions,
 			removed_solutions,
 			added_groups,
 			removed_groups,
 			changes,
@@ -569,22 +573,14 @@
 		if not 'time_limit' in self.config.keys():
 			util.exit_with_error('Time limit was not defined in config.yml.')
 		if not 'memory_limit' in self.config.keys():
 			util.exit_with_error('Memory limit was not defined in config.yml.')
 		if not 'scores' in self.config.keys():
 			util.exit_with_error('Scores were not defined in config.yml.')
 
-		self.ID = os.path.split(os.getcwd())[-1]
-		self.TMP_DIR = os.path.join(os.getcwd(), "cache")
-		self.COMPILATION_DIR = os.path.join(self.TMP_DIR, "compilation")
-		self.EXECUTIONS_DIR = os.path.join(self.TMP_DIR, "executions")
-		self.EXECUTABLES_DIR = os.path.join(self.TMP_DIR, "executables")
-		self.SOURCE_EXTENSIONS = ['.c', '.cpp', '.py', '.java']
-		self.PROGRAMS_IN_ROW = 8
-
 		for solution in self.get_solutions(None):
 			ext = os.path.splitext(solution)[1]
 			compiler = ""
 			tried = ""
 			flag = ""
 			if ext == '.c' and args.c_compiler_path is None:
 				compiler = 'C compiler'
```

### Comparing `sinol-make-0.0.1/src/sinol_make/helpers/compile.py` & `sinol-make-1.0.0/src/sinol_make/helpers/compile.py`

 * *Files identical despite different names*

### Comparing `sinol-make-0.0.1/src/sinol_make/helpers/compiler.py` & `sinol-make-1.0.0/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol-make-0.0.1/src/sinol_make/util.py` & `sinol-make-1.0.0/src/sinol_make/util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-0.0.1/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.0.0/src/sinol_make.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 0.0.1
+Version: 1.0.0
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # sinol-make
 CLI tool for creating sio2 task packages. \
 Currently in development and not yet ready to be used.
```

### Comparing `sinol-make-0.0.1/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.0.0/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

