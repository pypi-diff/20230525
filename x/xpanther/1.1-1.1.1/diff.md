# Comparing `tmp/xpanther-1.1.tar.gz` & `tmp/xpanther-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.1.tar", last modified: Tue May 23 12:09:09 2023, max compression
+gzip compressed data, was "xpanther-1.1.1.tar", last modified: Thu May 25 14:47:49 2023, max compression
```

## Comparing `xpanther-1.1.tar` & `xpanther-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 12:09:09.205768 xpanther-1.1/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.1/LICENSE
--rw-rw-rw-   0        0        0     5537 2023-05-23 12:09:09.205768 xpanther-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5071 2023-05-20 14:06:27.000000 xpanther-1.1/README.md
--rw-rw-rw-   0        0        0      648 2023-05-23 12:08:35.000000 xpanther-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 12:09:09.205768 xpanther-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 12:09:09.144827 xpanther-1.1/xpanther/
--rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.1/xpanther/__init__.py
--rw-rw-rw-   0        0        0    19990 2023-05-22 18:16:20.000000 xpanther-1.1/xpanther/main.py
--rw-rw-rw-   0        0        0     5464 2023-05-23 11:57:10.000000 xpanther-1.1/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:09:09.205768 xpanther-1.1/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5537 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 14:47:49.173689 xpanther-1.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5539 2023-05-25 14:47:49.173689 xpanther-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5071 2023-05-20 14:06:27.000000 xpanther-1.1.1/README.md
+-rw-rw-rw-   0        0        0      650 2023-05-25 14:47:11.000000 xpanther-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:47:49.173689 xpanther-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 14:47:49.123041 xpanther-1.1.1/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.1.1/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    20899 2023-05-25 12:52:00.000000 xpanther-1.1.1/xpanther/main.py
+-rw-rw-rw-   0        0        0     5109 2023-05-25 14:46:29.000000 xpanther-1.1.1/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:47:49.172671 xpanther-1.1.1/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5539 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 14:47:49.000000 xpanther-1.1.1/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.1/LICENSE` & `xpanther-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.1/PKG-INFO` & `xpanther-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.1
+Version: 1.1.1
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `xpanther-1.1/README.md` & `xpanther-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xpanther-1.1/pyproject.toml` & `xpanther-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpanther"
-version = "1.1"
+version = "1.1.1"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Find Unique Xpath of any HTML/XML element"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xpanther-1.1/xpanther/main.py` & `xpanther-1.1.1/xpanther/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.__no_digits = no_digits
         self.__url_input = url_input
         self.__show_all = show_all
         self.__print_output = print_output
         self.__speed = speed
 
     def capture(self, target):
-        program_return = []
+        program_return = [False]
         formatted_HTML = self.__format_html(self.__dom)
         element_regex, attr_regex, closing_tag_regex = self.__regex_distributor(formatted_HTML)
 
         self.__process_html(formatted_HTML, element_regex, attr_regex, closing_tag_regex)
 
         if type(target) == str and re.match(element_regex, target):
             list_of_occurrences = []
@@ -77,14 +77,15 @@
             else:
                 indexes_of_element = [0]
             outerHTML_input = re.findall(element_regex, formatted_element[0])
             outerHTML_input = re.findall(attr_regex, str(outerHTML_input))
             occurrences = [i for i, x in enumerate(self.__keys) if Counter(x[0]) == Counter(outerHTML_input)]
             self.__separate_classes_into_subclasses()
             if occurrences:
+                program_return = []
                 for index_of_element in indexes_of_element:
                     row_index = occurrences[index_of_element]
                     self.__target = self.__keys[row_index]
                     self.__original_target = self.__target
                     rarity = 'Unique'
                     if self.__identical:
                         rarity = 'Duplicate'
@@ -99,14 +100,15 @@
                         program_return.append(element_xpath)
                     else:
                         self.__print('Xpath couldn\'t be found ...')
                         program_return.append(False)
                 return program_return
             else:
                 self.__print('Program couldn\'t find this element, make sure it is inputted correctly !')
+                return program_return
 
         elif type(target) == int:
             if target <= len(self.__keys):
                 self.__separate_classes_into_subclasses()
                 self.__target = self.__keys[target - 1]
                 self.__original_target = self.__target
                 self.__print("\033[94m {}\033[00m".format(f'Index #{target}/{len(self.__keys)} | '), newline=False)
@@ -282,14 +284,15 @@
         elif type(self.__speed) == int and int(self.__speed) <= 50:
             speed = self.__speed
         else:
             speed = 25
         return [elements[0][:speed], elements[1], elements[2]]
 
     def __format_xpath(self, unique_elements, all_elements):
+        all_ = []
         combination = False
         if self.__identifier_method == 'combination':
             combination = True
 
         child_index_xpath = ''
         parent_hierarchy = ''
         tag = all_elements[0][0]
@@ -308,48 +311,58 @@
                 if not self.__xml:
                     attr_type = (tag == unique_element)
                 else:
                     attr_type = (tag in unique_element)
                 if attr_type:
                     XPATH = f'//{tag}'
                     final_Xpath = XPATH + child_index_xpath + parent_hierarchy
+                    all_.append(final_Xpath)
                     self.__print(final_Xpath)
                     if not self.__show_all:
                         return final_Xpath
                 else:
-                    XPATH = f'//{tag}[@{unique_element}]'
+                    if f_class := self.__merge_classes(unique_element):
+                        XPATH = f'//{tag}[{f_class}]'
+                    else:
+                        XPATH = f'//{tag}[@{unique_element}]'
                     final_Xpath = XPATH + child_index_xpath + parent_hierarchy
+                    all_.append(final_Xpath)
                     self.__print(final_Xpath)
                     self.__children_index = []
                     self.__gen = []
                     if not self.__show_all:
                         return final_Xpath
-            return True
+            return all_
         elif combination:
             for unique_element in unique_elements:
                 if classes := self.__merge_classes(unique_element):
                     unique_element = [x for x in unique_element if 'class="' not in x]
                     unique_element.append(classes)
                 for element in unique_element:
                     if not self.__xml:
                         if tag == element:
                             unique_element.remove(element)
                     else:
                         if tag in element:
                             unique_element.remove(element)
                 XPATH = f'//{tag}'
                 for element in unique_element:
-                    XPATH += f'[@{element}]'
+                    if element is not classes:
+                        XPATH += f'[@{element}]'
+                    else:
+                        XPATH += f'[{element}]'
                 final_Xpath = XPATH + child_index_xpath + parent_hierarchy
+                all_.append(final_Xpath)
                 self.__print(final_Xpath)
                 self.__children_index = []
                 self.__gen = []
+
                 if not self.__show_all:
                     return final_Xpath
-            return True
+            return all_
         else:
             self.__print(f'Element\'s --{all_elements[0]}-- format is not normal !')
             return False
 
     def __find_xpath(self, unique_elements, target_elements):
         if result := self.__format_xpath(unique_elements, target_elements):
             self.__gen = []
@@ -437,23 +450,29 @@
         if classes:
             return classes[0]
         else:
             return False
 
     @staticmethod
     def __merge_classes(unique_elements):
-        class_merge = [x for x in unique_elements if 'class="' in x]
+        if type(unique_elements) == list:
+            class_merge = [x for x in unique_elements if 'class="' in x]
+        else:
+            class_merge = unique_elements if 'class="' in unique_elements else False
         if class_merge:
-            combined_class = 'class="'
-            for classes in class_merge:
-                combined_class += classes[7:][:-1] + ' '
+            if type(class_merge) == str:
+                class_merge = [class_merge]
+            new_format = 'contains(concat(" ", normalize-space(@class), " "), " {} ")'
+            combined_class = ''
+            for index, classes in enumerate(class_merge):
+                if index != 0:
+                    combined_class += ' and '
+                combined_class += new_format.format(classes[7:][:-1])
             combined_class = list(combined_class)
-            combined_class[-1] = '"'
             combined_class = ''.join(combined_class)
-
             return combined_class
         return False
 
     def __print(self, text, newline=True):
         if self.__print_output:
             if newline:
                 print(text)
```

### Comparing `xpanther-1.1/xpanther.egg-info/PKG-INFO` & `xpanther-1.1.1/xpanther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.1
+Version: 1.1.1
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

