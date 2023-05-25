# Comparing `tmp/fastgedcom-0.0.2.tar.gz` & `tmp/fastgedcom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-0.0.2.tar", last modified: Tue May 23 21:05:03 2023, max compression
+gzip compressed data, was "fastgedcom-0.0.3.tar", last modified: Thu May 25 16:56:48 2023, max compression
```

## Comparing `fastgedcom-0.0.2.tar` & `fastgedcom-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 21:05:03.158081 fastgedcom-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5060 2023-05-23 21:05:03.150546 fastgedcom-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4212 2023-05-23 20:58:09.000000 fastgedcom-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 21:05:03.129924 fastgedcom-0.0.2/fastgedcom/
--rw-rw-rw-   0        0        0      234 2023-05-20 15:25:33.000000 fastgedcom-0.0.2/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0     8857 2023-05-23 20:37:12.000000 fastgedcom-0.0.2/fastgedcom/base.py
--rw-rw-rw-   0        0        0     1415 2023-05-23 18:17:44.000000 fastgedcom-0.0.2/fastgedcom/future.py
--rw-rw-rw-   0        0        0     5796 2023-05-23 20:54:07.000000 fastgedcom-0.0.2/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     3612 2023-05-23 20:14:32.000000 fastgedcom-0.0.2/fastgedcom/parser.py
--rw-rw-rw-   0        0        0     1541 2023-05-22 20:56:29.000000 fastgedcom-0.0.2/fastgedcom/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-23 21:05:03.150546 fastgedcom-0.0.2/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     5060 2023-05-23 21:05:02.000000 fastgedcom-0.0.2/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-23 21:05:03.000000 fastgedcom-0.0.2/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 21:05:02.000000 fastgedcom-0.0.2/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-23 21:05:02.000000 fastgedcom-0.0.2/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-23 21:05:02.000000 fastgedcom-0.0.2/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 21:05:03.158620 fastgedcom-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-05-23 21:03:55.000000 fastgedcom-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:56:48.632524 fastgedcom-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5000 2023-05-25 16:56:48.632524 fastgedcom-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4152 2023-05-25 16:53:48.000000 fastgedcom-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 16:56:48.592493 fastgedcom-0.0.3/fastgedcom/
+-rw-rw-rw-   0        0        0      234 2023-05-20 15:25:33.000000 fastgedcom-0.0.3/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0     9254 2023-05-24 23:22:27.000000 fastgedcom-0.0.3/fastgedcom/base.py
+-rw-rw-rw-   0        0        0     1415 2023-05-24 17:51:16.000000 fastgedcom-0.0.3/fastgedcom/future.py
+-rw-rw-rw-   0        0        0     5336 2023-05-24 22:45:41.000000 fastgedcom-0.0.3/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     3689 2023-05-24 22:13:35.000000 fastgedcom-0.0.3/fastgedcom/parser.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.3/fastgedcom/py.typed
+-rw-rw-rw-   0        0        0     1436 2023-05-25 16:44:01.000000 fastgedcom-0.0.3/fastgedcom/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:56:48.624522 fastgedcom-0.0.3/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     5000 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 16:52:11.000000 fastgedcom-0.0.3/fastgedcom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 16:56:48.632524 fastgedcom-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2023-05-25 16:47:45.000000 fastgedcom-0.0.3/setup.py
```

### Comparing `fastgedcom-0.0.2/LICENSE` & `fastgedcom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.2/PKG-INFO` & `fastgedcom-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.2
+Version: 0.0.3
 Summary: A gedcom tool to parse, browse and modify gedcom files
 Home-page: https://github.com/GatienBouyer/fastgedcom
 Author: Gatien Bouyer
 Author-email: gatien.bouyer.dev@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
@@ -86,40 +86,40 @@
 
 print(f"Number of generations above root: {number_generations_above_root}")
 ```
 
 In the following example, we find the oldest deceased person. Then, we print his name and all his gedcom information using the `fastgedcom.helpers` module
 ```python
 from fastgedcom.helpers import (extract_int_year, extract_year, format_name,
-                                get_gedcom_data)
+                                get_gedcom_source)
 from fastgedcom.parser import guess_encoding, parse
 
 gedcom_file = YOUR_GEDCOM_FILE
 with open(gedcom_file, "r", encoding=guess_encoding(gedcom_file)) as f:
 	gedcom, _ = parse(f)
 
-oldest = next(gedcom.get_records("INDI")).tag
+oldest = next(gedcom.get_records("INDI"))
 age_oldest = 0.0 # the age is a float to handle all type of date
 # A date such as between 2001 and 2002 returns 2001.5
 for individual in gedcom.get_records("INDI"):
-	birth_date = (gedcom[individual.tag] > "BIRT") >= "DATE"
-	death_date = (gedcom[individual.tag] > "DEAT") >= "DATE"
+	birth_date = (individual > "BIRT") >= "DATE"
+	death_date = (individual > "DEAT") >= "DATE"
 	birth_year = extract_int_year(birth_date)
 	death_year = extract_int_year(death_date)
 	if birth_year is None or death_year is None: continue
 	age = death_year - birth_year
 	if age > age_oldest:
-		oldest = individual.tag
+		oldest = individual
 		age_oldest = age
 
-print("Oldest person:", format_name(gedcom[oldest] >= "NAME"))
-print("Year of birth:", extract_year((gedcom[oldest] > "BIRT") >= "DATE"))
-print("Year of death:", extract_year((gedcom[oldest] > "DEAT") >= "DATE"))
+print("Oldest person:", format_name(oldest >= "NAME"))
+print("Year of birth:", extract_year((oldest > "BIRT") >= "DATE"))
+print("Year of death:", extract_year((oldest > "DEAT") >= "DATE"))
 print("Age:", age_oldest)
-print("All the information:", get_gedcom_data(gedcom, oldest))
+print("All the information:", get_gedcom_source(oldest))
 ```
 
 
 ## Contributing
 
 Contributions are welcome, and they will be greatly appreciated!
```

### Comparing `fastgedcom-0.0.2/README.md` & `fastgedcom-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,40 +64,40 @@
 
 print(f"Number of generations above root: {number_generations_above_root}")
 ```
 
 In the following example, we find the oldest deceased person. Then, we print his name and all his gedcom information using the `fastgedcom.helpers` module
 ```python
 from fastgedcom.helpers import (extract_int_year, extract_year, format_name,
-                                get_gedcom_data)
+                                get_gedcom_source)
 from fastgedcom.parser import guess_encoding, parse
 
 gedcom_file = YOUR_GEDCOM_FILE
 with open(gedcom_file, "r", encoding=guess_encoding(gedcom_file)) as f:
 	gedcom, _ = parse(f)
 
-oldest = next(gedcom.get_records("INDI")).tag
+oldest = next(gedcom.get_records("INDI"))
 age_oldest = 0.0 # the age is a float to handle all type of date
 # A date such as between 2001 and 2002 returns 2001.5
 for individual in gedcom.get_records("INDI"):
-	birth_date = (gedcom[individual.tag] > "BIRT") >= "DATE"
-	death_date = (gedcom[individual.tag] > "DEAT") >= "DATE"
+	birth_date = (individual > "BIRT") >= "DATE"
+	death_date = (individual > "DEAT") >= "DATE"
 	birth_year = extract_int_year(birth_date)
 	death_year = extract_int_year(death_date)
 	if birth_year is None or death_year is None: continue
 	age = death_year - birth_year
 	if age > age_oldest:
-		oldest = individual.tag
+		oldest = individual
 		age_oldest = age
 
-print("Oldest person:", format_name(gedcom[oldest] >= "NAME"))
-print("Year of birth:", extract_year((gedcom[oldest] > "BIRT") >= "DATE"))
-print("Year of death:", extract_year((gedcom[oldest] > "DEAT") >= "DATE"))
+print("Oldest person:", format_name(oldest >= "NAME"))
+print("Year of birth:", extract_year((oldest > "BIRT") >= "DATE"))
+print("Year of death:", extract_year((oldest > "DEAT") >= "DATE"))
 print("Age:", age_oldest)
-print("All the information:", get_gedcom_data(gedcom, oldest))
+print("All the information:", get_gedcom_source(oldest))
 ```
 
 
 ## Contributing
 
 Contributions are welcome, and they will be greatly appreciated!
```

### Comparing `fastgedcom-0.0.2/fastgedcom/base.py` & `fastgedcom-0.0.3/fastgedcom/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,132 +1,150 @@
+from typing import Iterator, TypeGuard, Union
 from abc import ABC, abstractmethod
-from typing import Iterator, Union
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from .structure import FamRef, IndiRef, XRef
 
 
 class Line(ABC):
 	"""Abstract base class for gedcom lines.
 	(see GedcomLine for more information)
 	This class is for syntactic sugar. It defines operator
 	as alias of standard methods and allows the chaining of
-	operations thanks to the FakeLine implemantation.
+	operations thanks to the FakeLine implementation.
 	
 	Example:
 	```python
 	# With standard methods:
 	indi = gedcom.get_record("@I1@")
 	birth_date = indi.get_sub_record("BIRT").get_sub_record_value("DATE")
 	sources = indi.get_sub_record("BIRT").get_sub_records("SOUR").
 	
 	# With magic methods:
 	indi = gedcom["@I1@"]
 	birth_date = indi > "BIRT" >= "DATE"
 	sources = indi > "BIRT" >> "SOUR"
 	```
-
-	In general, the use of `get_sub_record_payload` (or `>=`) is preferable
-	rather than the use of isinstance(line, FakeLine).
 	"""
+	@property
 	@abstractmethod
-	def get_sub_records(self, tag: str) -> list['GedcomLine']:
-		raise NotImplementedError
+	def payload(self) -> str: ...
+	
+	@property
 	@abstractmethod
-	def get_sub_record(self, tag: str) -> Union['GedcomLine', 'FakeLine']:
-		raise NotImplementedError
+	def payload_with_cont(self) -> str: ...
+
+	@abstractmethod
+	def get_sub_records(self, tag: str) -> list['GedcomLine']: ...
+	
+	@abstractmethod
+	def get_sub_record(self, tag: str) -> Union['GedcomLine', 'FakeLine']: ...
+	
 	@abstractmethod
-	def get_sub_record_payload(self, tag: str) -> str | None:
-		# TODO Check if checking for CONT in sub_rec here doesn't hurt performance
-		raise NotImplementedError
+	def get_sub_record_payload(self, tag: str) -> str: ...
+
 	__gt__ = get_sub_record # operator >
 	__ge__ = get_sub_record_payload # operator >=
 	__rshift__ = get_sub_records # operator >>
 
 class FakeLine(Line):
-	"""Dummy Line that allows the chaining of get_sub_record.
+	"""Dummy Line that allows the chaining of operators.
 
 	To differenciate a FakeLine from a GedcomLine a simple boolean test is
 	enough: `if line: line.payload`. However to tell typecheckers that after
-	the test it can't be FakeLine, I found nothing else than the use of
-	isinstance: `if not isinstance(line, FakeLine): line.payload`  
+	the test it the type is narrowed, you should use the line_exists
+	function.
 
 	In general, the use of `get_sub_record_payload` (or `>=`) is preferable.
 
 	Example:
 	```python
+	# Instead of:
 	indi_birth_date = (gedcom.get_record("@I1@") > "BIRT") > "DATE"
-	if not isinstance(line, FakeLine):
-		print("We know the birth date of @I1@ !")
+	if line_exists(indi_birth_date):
+		print(indi_birth_date.payload)
+
+	# Prefere the use of:
+	indi_birth_date = (gedcom.get_record("@I1@") > "BIRT") >= "DATE"
+	print(indi_birth_date)
 	```
 	"""
+	payload = ""
+	payload_with_cont = ""
+	
 	def get_sub_records(self, tag: str) -> list['GedcomLine']:
 		return []
 	
 	def get_sub_record(self, tag: str) -> Union['GedcomLine', 'FakeLine']:
 		return fake_line
 	
-	def get_sub_record_payload(self, tag: str) -> str | None:
-		return None
+	def get_sub_record_payload(self, tag: str) -> str:
+		return ""
 	
 	__gt__ = get_sub_record # operator >
 	__ge__ = get_sub_record_payload # operator >=
 	__rshift__ = get_sub_records # operator >>
 	
 	def __repr__(self) -> str:
 		return f"<{self.__class__.__qualname__}>"
 	
 	def __bool__(self) -> bool:
 		return False
 
 
-fake_line = FakeLine()
-
-
 @dataclass(slots=True)
 class GedcomLine(Line):
 	"""Represent a line of a gedcom document and contains the sub-lines
 	to traverse the gedcom tree structure.
 
-	This class use the simplified 'Level Tag Payload EOL' structure
-	(instead of the normalized 'Level [Xref] Tag [LineVal] EOL' structure).
+	This class use the simplified 'Level Tag Payload' structure,
+	instead of the normalized 'Level [Xref] Tag [LineVal]' gedcom structure.
 	In this structure, the Tag is either the normalized Tag or the optional Xref.
 	Hence, the Payload is the LineVal when the Xref is not present,
 	or the Payload is the normalized Tag plus the LineVal when the Xref is present.
-	When the line contains neither a Xref or a LineVal, the Payload is None."""
+	When the line contains neither a Xref or a LineVal, the Payload is an empty string.
+	"""
 	level: int
 	tag: str | XRef
-	payload: str | None
-	sub_rec: list['GedcomLine']
+	payload: str
+	sub_rec: list['GedcomLine'] = field(default_factory=list)
 
 	def get_sub_records(self, tag: str) -> list['GedcomLine']:
 		return [sub_record for sub_record in self.sub_rec if sub_record.tag == tag]
 
 	def get_sub_record(self, tag: str) -> Union['GedcomLine', 'FakeLine']:
 		for sub_record in self.sub_rec:
 			if sub_record.tag == tag:
 				return sub_record
 		return fake_line
 
-	def get_sub_record_payload(self, tag: str) -> str | None:
+	def get_sub_record_payload(self, tag: str) -> str:
 		for sub_record in self.sub_rec:
 			if sub_record.tag == tag:
 				return sub_record.payload
-		return None
+		return ""
 	
 	__gt__ = get_sub_record # operator >
 	__ge__ = get_sub_record_payload # operator >=
 	__rshift__ = get_sub_records # operator >>
 
 	def __str__(self) -> str:
-		return f"{self.level} {self.tag} {self.payload if self.payload else ''}"
+		return f"{self.level} {self.tag} {self.payload}"
 
 	def __repr__(self) -> str:
 		return f"<{self.__class__.__qualname__} {self.level} {self.tag} {self.payload} -> {len(self.sub_rec)}>"
 
+	@property
+	def payload_with_cont(self) -> str:
+		"""The ilne payload with the payload of the CONT sub-records."""
+		text = self.payload
+		for cont in self.get_sub_records('CONT'):
+			text += '\n' + cont.payload
+		return text
+
 
 class Gedcom():
 	"""Stores all the information of the gedcom document.
 	
 	All level 0 records are directly accessible and the higher level records
 	are accessible via GedcomLine.sub_rec of the parent record.
 	
@@ -167,14 +185,15 @@
 
 	def get_parent_family(self, child: IndiRef) -> FamRef | None:
 		"""Return the FamRef of the family with the parents of the person."""
 		record = self.level0_index.get(child, None)
 		if record is None: return None
 		for sub_record in record.sub_rec:
 			if sub_record.tag == "FAMC":
+				if sub_record.payload == "": return None
 				return sub_record.payload
 		return None
 
 	def get_parents(self, child: IndiRef) -> tuple[IndiRef | None, IndiRef | None]:
 		"""Return the IndiRef of the father and the IndiRef of the mother of the person.
 		Parameter is the IndiRef of the child.
 		Return the tuple (father, mother) with None in case of missing data."""
@@ -185,19 +204,22 @@
 		unions: list[FamRef]
 		if spouse is None: unions = self.unions.get(parent, [])
 		else: unions = self.get_unions(parent, spouse)
 		for fam in unions:
 			record = self.level0_index[fam]
 			for sub_record in record.sub_rec:
 				if sub_record.tag == "CHIL":
-					if sub_record.payload is None: continue
+					if sub_record.payload == "": continue
 					children.append(sub_record.payload)
 		return children
 
-	def get_unions(self, parent: IndiRef, spouse: IndiRef | None = None) -> list[FamRef]:
+	def get_unions(self,
+		parent: IndiRef,
+		spouse: IndiRef | None = None
+	) -> list[FamRef]:
 		if spouse is None:
 			return self.unions.get(parent, [])
 		unions: list[FamRef] = []
 		spouse_fams = self.unions.get(spouse, [])
 		for fam in self.unions.get(parent, []):
 			if fam in spouse_fams:
 				unions.append(fam)
@@ -205,26 +227,26 @@
 
 	def get_spouses(self, indi: IndiRef) -> list[IndiRef]:
 		spouses: list[IndiRef] = []
 		for fam in self.unions.get(indi, []):
 			record = self.level0_index[fam]
 			for sub_record in record.sub_rec:
 				if sub_record.payload != indi and (sub_record.tag == "HUSB" or sub_record.tag == "WIFE"):
-					if sub_record.payload is None: continue
+					if sub_record.payload == "": continue
 					spouses.append(sub_record.payload)
 		return spouses
 
 	def get_siblings(self, indi: IndiRef) -> list[IndiRef]:
 		fam = self.get_parent_family(indi)
 		if fam is None: return []
 		record = self.level0_index[fam]
 		siblings: list[IndiRef] = []
 		for sub_record in record.sub_rec:
 			if sub_record.payload != indi and sub_record.tag == "CHIL":
-				if sub_record.payload is None: continue
+				if sub_record.payload == "": continue
 				siblings.append(sub_record.payload)
 		return siblings
 
 	def get_stepsiblings(self, indi: IndiRef) -> list[IndiRef]:
 		father, mother = self.get_parents(indi)
 		stepsiblings: set[IndiRef] = set()
 		if father: stepsiblings.update(self.get_children(father))
@@ -238,13 +260,20 @@
 		unions: list[tuple[IndiRef | None, list[IndiRef]]] = []
 		for fam in self.unions.get(indi, []):
 			record = self.level0_index[fam]
 			spouse = None
 			children: list[IndiRef] = []
 			for sub_record in record.sub_rec:
 				if sub_record.tag == "CHIL":
-					if sub_record.payload is None: continue
+					if sub_record.payload == "": continue
 					children.append(sub_record.payload)
 				elif sub_record.payload != indi and (sub_record.tag == "HUSB" or sub_record.tag == "WIFE"):
+					if sub_record.payload == "": continue
 					spouse = sub_record.payload
 			unions.append((spouse, children))
 		return unions
+
+
+fake_line = FakeLine()
+
+def line_exists(line: Union[GedcomLine, FakeLine]) -> TypeGuard[GedcomLine]:
+	return bool(line)
```

### Comparing `fastgedcom-0.0.2/fastgedcom/future.py` & `fastgedcom-0.0.3/fastgedcom/future.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.2/fastgedcom/helpers.py` & `fastgedcom-0.0.3/fastgedcom/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 from typing import Any, Callable, Iterator, Literal
 
-from .base import FakeLine, Gedcom, GedcomLine
-from .structure import IndiRef, XRef
+from .base import FakeLine, Gedcom, GedcomLine, line_exists
+from .structure import IndiRef
 
-MINIMAL_DATE = -99999 # used to sort None dates
+MINIMAL_DATE = -99999
+"""Used to sort empty date fields"""
 
 def get_all_sub_records(line: GedcomLine) -> Iterator[GedcomLine]:
 	"""Recursively iterate on all lines under the given line."""
 	sub_records = list(line.sub_rec)
 	while len(sub_records) > 0:
 		record = sub_records.pop(0)
 		yield record
 		sub_records = record.sub_rec + sub_records
 
-def format_name(name: str | None) -> str:
+def get_gedcom_source(line: GedcomLine | FakeLine) -> str:
+	"""Return all the contents of the gedcom under this level 0 id (person id, family id, source id, ...)."""
+	if not line_exists(line): return ""
+	text = str(line) + "\n"
+	for sub_rec in get_all_sub_records(line):
+		text += str(sub_rec) + "\n"
+	return text
+
+def format_name(name: str) -> str:
 	"""Format the payload of the gedcom tag NAME.
 	Remove the backslash around the surname."""
-	if name is None: return ""
 	return name.replace("/", "")
 
 def gender_to_ascii(gender: Literal['M', 'F'] | Any) -> Literal['♂', '♀', '⚥']:
 	if gender == 'M': return '♂'
 	if gender == 'F': return '♀'
 	return '⚥'
 
-def format_date(date: str | None) -> str:
+def format_date(date: str) -> str:
 	"""Format the gedcom date into a shorter string.
 	Replace gedcom keywords by symbols.
 
 	Replacements:
 	- 'd BC' standing for before christ is replaced by '-d',
 	- 'd BCE' or before common era with '-d',
 	- 'ABT d' stading for about is replaced by '~ d',
@@ -37,15 +45,14 @@
 	- 'BEF d' standing for before is replaced by '< d',
 	- 'AFT d' standing for after is replaced by '> d',
 	- 'BET d AND d' standing for between is replaced by 'd -- d',
 	- 'FROM d TO d' is replace by 'd -- d',
 	- 'FROM d' is replaced by 'd',
 	- 'TO d' is replaced by 'd'.
 	"""
-	if date is None: return ""
 	date = remove_trailing_zeros(date)
 	if date[:4]=='BET ' and 'AND' in date:
 		date = date[4:]
 		date1, date2 = date.split(' AND ', 1)
 		return format_date(date1) + ' -- ' + format_date(date2)
 	elif date[:5]=='FROM ' and 'TO' in date:
 		date = date[5:]
@@ -70,15 +77,15 @@
 	while k+1 < len(date):
 		if date[k]=='0' and (k==0 or (k>0 and (date[k-1].isspace() or date[k-1] == '-'))):
 			date = date[:k] + date[k+1:]
 		else:
 			k += 1
 	return date
 
-def extract_year(date: str | None) -> str:
+def extract_year(date: str) -> str:
 	"""Return the only year of the date.
 	The parameter is the gedcom date or the formatted date string.
 	Keep the context of the date: '-', '~', '<', '>' and '--'."""
 	formated_date = format_date(date)
 	if ' -- ' in formated_date:
 		first_date, second_date = formated_date.split(' -- ', 1)
 		first_year = extract_year(first_date)
@@ -91,15 +98,15 @@
 		return ""
 	year = numeric_parts[-1]
 	if '~' in formated_date: year = '~ '+year
 	if '<' in formated_date: year = '< '+year
 	if '>' in formated_date: year = '> '+year
 	return year
 
-def extract_int_year(date: str | None) -> float | None:
+def extract_int_year(date: str) -> float | None:
 	"""Return the year of the date as an integer.
 	Keep the context: A date BCE returns a negative number.
 	A date range of type `between` or `from-to` returns the median number of the range."""
 	year = extract_year(date)
 	if ' -- ' in year:
 		str_year1, str_year2 = year.split(' -- ', 1)
 		year1 = extract_int_year(str_year1)
@@ -108,43 +115,24 @@
 		elif year2 is None: return year1
 		return (year1 + year2) / 2
 	year_without_context = ''.join(filter(lambda c: c.isdecimal() or c=='-', year))
 	if year_without_context == "": return None
 	return int(year_without_context)
 
 
-def sorting_key_indi_birth(gedcom: Gedcom) -> Callable[[IndiRef], float]:
-	def get_sorting_key_indi_birth(indi: IndiRef) -> float:
+def sorting_key_indi_birth(gedcom: Gedcom) -> Callable[[IndiRef | None], float]:
+	def get_sorting_key_indi_birth(indi: IndiRef | None) -> float:
+		if indi is None: return MINIMAL_DATE
 		birth_year = extract_int_year((gedcom[indi] > "BIRT") >= "DATE")
-		return -MINIMAL_DATE if birth_year is None else birth_year
+		return MINIMAL_DATE if birth_year is None else birth_year
 	return get_sorting_key_indi_birth
 
-def sorting_key_indi_union(gedcom: Gedcom, ref_indi: IndiRef) -> Callable[[IndiRef], float]:
-	def get_sorting_key_indi_union(indi: IndiRef) -> float:
+def sorting_key_indi_union(
+	gedcom: Gedcom, ref_indi: IndiRef
+) -> Callable[[IndiRef | None], float]:
+	def get_sorting_key_indi_union(indi: IndiRef | None) -> float:
+		if indi is None: return MINIMAL_DATE
 		unions = gedcom.get_unions(ref_indi, indi)
-		if len(unions) == 0: return -MINIMAL_DATE
+		if len(unions) == 0: return MINIMAL_DATE
 		union_year = extract_int_year(gedcom[unions[0]] >= "DATE")
-		return -MINIMAL_DATE if union_year is None else union_year
+		return MINIMAL_DATE if union_year is None else union_year
 	return get_sorting_key_indi_union
-
-def get_note(gedcom: Gedcom, xref: IndiRef) -> str:
-	"""Return the content of the NOTE tag of the person. None if nothing."""
-	indi = gedcom.get_record(xref)
-	if indi is None: return ""
-	note = indi.get_sub_record('NOTE')
-	if isinstance(note, FakeLine): return ""
-	text = note.payload
-	if text is None: text = ""
-	for cont in note.get_sub_records('CONT'):
-		text += '\n'
-		text_part = cont.payload
-		if text_part is not None: text += text_part
-	return text
-
-def get_gedcom_data(gedcom: Gedcom, xref: XRef) -> str:
-	"""Return all the contents of the gedcom under this level 0 id (person id, family id, source id, ...)."""
-	rec = gedcom.get_record(xref)
-	if isinstance(rec, FakeLine): return ""
-	text = str(rec) + "\n"
-	for sub_rec in get_all_sub_records(rec):
-		text += str(sub_rec) + "\n"
-	return text
```

### Comparing `fastgedcom-0.0.2/fastgedcom/parser.py` & `fastgedcom-0.0.3/fastgedcom/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,45 +24,48 @@
 	"""Warn about a level 0 reference that is present twice."""
 	def __init__(self, xref: XRef) -> None:
 		self.xref = xref
 	def __repr__(self) -> str:
 		return f"<{self.__class__.__qualname__} xref={self.xref}>"
 
 def parse(readable_lines: IO[str]) -> tuple[Gedcom, list[ParsingWarning]]:
-	"""Parser for gedcom documents to create the Gedcom class."""
+	"""Parse the text input to create the Gedcom class.
+	
+	Return the Gedcom based on the input and the warnings about
+	input lines that can't be put into the Gedcom class.
+	
+	Raise ParsingError on failure."""
 	gedcom = Gedcom()
 	warnings: list[ParsingWarning] = []
 	line_number = 0
 	try:
 		parent_lines: list[GedcomLine] = []
 		for line in readable_lines:
 			line_number += 1
 			line_info = line.rstrip().split(' ', 2)
 			if len(line_info) == 3:
 				parsed_line = GedcomLine(int(line_info[0]), line_info[1], line_info[2], [])
 			elif len(line_info) == 2:
-				parsed_line = GedcomLine(int(line_info[0]), line_info[1], None, [])
+				parsed_line = GedcomLine(int(line_info[0]), line_info[1], "", [])
 			else:
 				warnings.append(LineParsingWarning(line_number, line))
 				continue
 			if parsed_line.level == 0:
 				parent_lines = [parsed_line]
 				if parsed_line.tag in gedcom.level0_index:
 					warnings.append(DuplicateParsingWarning(parsed_line.tag))
 				gedcom.level0_index[parsed_line.tag] = parsed_line
 			else:
 				while parent_lines and parsed_line.level <= parent_lines[-1].level:
 					parent_lines.pop(-1)
 				if len(parent_lines) == 0: raise ParsingError("Inconsistent use of line levels")
 				parent_lines[-1].sub_rec.append(parsed_line)
 				parent_lines.append(parsed_line)
-	except UnicodeDecodeError:
-		raise ParsingError(line_number, "UnicodeDecodeError")
-	except ValueError: # raised on int parsing error
-		raise ParsingError(line_number, "Line parsing failed")
+	except ValueError as err: # raised on int parsing error
+		raise ParsingError(line_number, "Line parsing failed") from err
 	__build_parents(gedcom)
 	return (gedcom, warnings)
 
 def __build_parents(gedcom: Gedcom) -> None:
 	for fam_record in gedcom.level0_index.values():
 		if fam_record.payload != "FAM": continue
 		father = mother = None
```

### Comparing `fastgedcom-0.0.2/fastgedcom/structure.py` & `fastgedcom-0.0.3/fastgedcom/structure.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,9 +23,7 @@
 VoidRef: TypeAlias = Literal['@VOID@']
 """A pointer used for unknown value and to have something in the payload.
 e.g.: in a family record, a line '2 CHIL @VOID@' indicates a placeholder for an unknown child."""
 
 Pointer: TypeAlias = XRef | VoidRef
 """Generic pointer that is used in the payload to reference an existing record or a non-existing one."""
 
-# TODO add tag macros ref: https://gedcom.io/specifications/FamilySearchGEDCOMv7.html#structure-types
-
```

### Comparing `fastgedcom-0.0.2/fastgedcom.egg-info/PKG-INFO` & `fastgedcom-0.0.3/fastgedcom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.2
+Version: 0.0.3
 Summary: A gedcom tool to parse, browse and modify gedcom files
 Home-page: https://github.com/GatienBouyer/fastgedcom
 Author: Gatien Bouyer
 Author-email: gatien.bouyer.dev@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
@@ -86,40 +86,40 @@
 
 print(f"Number of generations above root: {number_generations_above_root}")
 ```
 
 In the following example, we find the oldest deceased person. Then, we print his name and all his gedcom information using the `fastgedcom.helpers` module
 ```python
 from fastgedcom.helpers import (extract_int_year, extract_year, format_name,
-                                get_gedcom_data)
+                                get_gedcom_source)
 from fastgedcom.parser import guess_encoding, parse
 
 gedcom_file = YOUR_GEDCOM_FILE
 with open(gedcom_file, "r", encoding=guess_encoding(gedcom_file)) as f:
 	gedcom, _ = parse(f)
 
-oldest = next(gedcom.get_records("INDI")).tag
+oldest = next(gedcom.get_records("INDI"))
 age_oldest = 0.0 # the age is a float to handle all type of date
 # A date such as between 2001 and 2002 returns 2001.5
 for individual in gedcom.get_records("INDI"):
-	birth_date = (gedcom[individual.tag] > "BIRT") >= "DATE"
-	death_date = (gedcom[individual.tag] > "DEAT") >= "DATE"
+	birth_date = (individual > "BIRT") >= "DATE"
+	death_date = (individual > "DEAT") >= "DATE"
 	birth_year = extract_int_year(birth_date)
 	death_year = extract_int_year(death_date)
 	if birth_year is None or death_year is None: continue
 	age = death_year - birth_year
 	if age > age_oldest:
-		oldest = individual.tag
+		oldest = individual
 		age_oldest = age
 
-print("Oldest person:", format_name(gedcom[oldest] >= "NAME"))
-print("Year of birth:", extract_year((gedcom[oldest] > "BIRT") >= "DATE"))
-print("Year of death:", extract_year((gedcom[oldest] > "DEAT") >= "DATE"))
+print("Oldest person:", format_name(oldest >= "NAME"))
+print("Year of birth:", extract_year((oldest > "BIRT") >= "DATE"))
+print("Year of death:", extract_year((oldest > "DEAT") >= "DATE"))
 print("Age:", age_oldest)
-print("All the information:", get_gedcom_data(gedcom, oldest))
+print("All the information:", get_gedcom_source(oldest))
 ```
 
 
 ## Contributing
 
 Contributions are welcome, and they will be greatly appreciated!
```

### Comparing `fastgedcom-0.0.2/setup.py` & `fastgedcom-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from setuptools import find_packages, setup
+from setuptools import setup
 
 with open("Readme.md", "r") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setup(
     name="fastgedcom",
-    version="0.0.2",
+    version="0.0.3",
     description="A gedcom tool to parse, browse and modify gedcom files",
-    packages=find_packages(exclude=['fastgedcom.test']),
+    packages=["fastgedcom"],
+    package_data={"fastgedcom": ["py.typed"]},
     long_description=long_description,
     long_description_content_type="text/markdown",
+    zip_safe=False,
+    install_requires=requirements,
+    extras_require={
+        "dev": ["mypy", "twine"],
+	},
+    python_requires=">=3.11",
     url="https://github.com/GatienBouyer/fastgedcom",
     author="Gatien Bouyer",
     author_email="gatien.bouyer.dev@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.11",
         "Topic :: Sociology :: Genealogy",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Development Status :: 2 - Pre-Alpha",
     ],
     keywords='fastgedcom gedcom parser genealogy',
-    install_requires=requirements,
-    extras_require={
-        "dev": ["mypy", "twine"],
-	},
-    python_requires=">=3.11",
 	project_urls={
         'Bug Reports': 'https://github.com/GatienBouyer/fastgedcom/issues',
         'Source': 'https://github.com/GatienBouyer/fastgedcom',
     },
 )
```

