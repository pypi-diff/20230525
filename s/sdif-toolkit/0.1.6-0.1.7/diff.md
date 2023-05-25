# Comparing `tmp/sdif_toolkit-0.1.6.tar.gz` & `tmp/sdif-toolkit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "sdif-toolkit-0.1.7.tar", last modified: Thu May 25 02:28:47 2023, max compression
```

## Comparing `sdif_toolkit-0.1.6.tar` & `sdif-toolkit-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,22 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/requirements.txt
--rw-r--r--   0        0        0    69120 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/sdifv3f.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/src/sdif_toolkit/__init__.py
--rw-r--r--   0        0        0    26055 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/src/sdif_toolkit/io.py
--rw-r--r--   0        0        0    20558 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/src/sdif_toolkit/records.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/src/sdif_toolkit/time.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/tests/test_records.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/tests/test_time.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 sdif_toolkit-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 02:28:47.154690 sdif-toolkit-0.1.7/
+-rw-rw-rw-   0        0        0     1094 2022-07-21 18:52:24.000000 sdif-toolkit-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-05-25 02:28:47.154188 sdif-toolkit-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2022-07-21 18:52:24.000000 sdif-toolkit-0.1.7/README.md
+-rw-rw-rw-   0        0        0      696 2022-09-09 20:36:20.000000 sdif-toolkit-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 02:28:47.155189 sdif-toolkit-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 02:28:47.079489 sdif-toolkit-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 02:28:47.119187 sdif-toolkit-0.1.7/src/sdif_toolkit/
+-rw-rw-rw-   0        0        0        0 2022-07-21 18:52:24.000000 sdif-toolkit-0.1.7/src/sdif_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    36452 2023-03-13 19:18:55.000000 sdif-toolkit-0.1.7/src/sdif_toolkit/io.py
+-rw-rw-rw-   0        0        0    20552 2022-09-09 20:36:20.000000 sdif-toolkit-0.1.7/src/sdif_toolkit/records.py
+-rw-rw-rw-   0        0        0     2244 2022-09-09 20:36:20.000000 sdif-toolkit-0.1.7/src/sdif_toolkit/time.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:28:47.135190 sdif-toolkit-0.1.7/src/sdif_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-05-25 02:28:47.000000 sdif-toolkit-0.1.7/src/sdif_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-25 02:28:47.000000 sdif-toolkit-0.1.7/src/sdif_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 02:28:47.000000 sdif-toolkit-0.1.7/src/sdif_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 02:28:47.000000 sdif-toolkit-0.1.7/src/sdif_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 02:28:47.000000 sdif-toolkit-0.1.7/src/sdif_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 02:28:47.152687 sdif-toolkit-0.1.7/tests/
+-rw-rw-rw-   0        0        0     6718 2023-02-05 08:46:19.000000 sdif-toolkit-0.1.7/tests/test_io.py
+-rw-rw-rw-   0        0        0     4707 2023-02-05 08:47:39.000000 sdif-toolkit-0.1.7/tests/test_records.py
+-rw-rw-rw-   0        0        0     4610 2022-09-09 20:36:20.000000 sdif-toolkit-0.1.7/tests/test_time.py
```

### Comparing `sdif_toolkit-0.1.6/src/sdif_toolkit/io.py` & `sdif-toolkit-0.1.7/src/sdif_toolkit/io.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,52 @@
-import argparse, os, re
-from audioop import add
-from datetime import date, datetime
+import argparse
+import os
+import re
+from datetime import date, datetime, timedelta
 from tkinter import filedialog
-from typing import Dict, List, Tuple, Type
-from sdif_toolkit.records import STROKES, RECORD_TYPES, MeetRecord, RelayNameRecord, TeamIDRecord, IndividualEventRecord, SplitsRecord, IndividualInformationRecord, RelayEventRecord
-from sdif_toolkit.time import Time
-from pyodbc import connect
+from typing import Any, Dict, List, Tuple, Type
+
+from pyodbc import Connection, Cursor, connect
+from .records import (RECORD_TYPES, STROKES,
+                                      IndividualEventRecord,
+                                      IndividualInformationRecord, MeetRecord,
+                                      RelayEventRecord, RelayNameRecord,
+                                      SplitsRecord, TeamIDRecord)
+from .time import Time
+
 
 RESULT_TYPES = {
     "p": "Prelims",
     "s": "Swim-Off",
     "f": "Finals"
 }
 
+
 GENDERS_BG = {
     "m": "Boys",
     "f": "Girls"
 }
 
+
 class Result:
     time: Time
     course: str
     type: str
     splits: Dict[int, Time]
     split_distance: int
     rank: int
     points: float
-
-    def __init__(self, time:Time=None, time_str:str=None, type=None, course=None, splits=[], split_distance=None, rank=None, points=None) -> None:
+    is_dq: bool
+    dq_code: int
+    is_dfs: bool
+
+    def __init__(self, time:Time=None, time_str:str=None,
+                 type:str=None, course:str=None, splits=[],
+                 split_distance=None, rank:int=None, points:float=None,
+                 is_dq:bool=False, dq_code:int=None, is_dfs:bool=False) -> None:
         if time is not None:
             self.time = time
         elif time_str is not None:
             self.time = Time(time_str)
         
         if type is not None:
             self.type = type
@@ -42,27 +57,53 @@
         if rank is not None:
             self.rank = int(rank)
         
         if points is not None:
             self.points = float(points)
         
         self.splits = {}
+
+        self.is_dq = is_dq
+        self.is_dfs = is_dfs
+
+        if dq_code is not None:
+            self.dq_code = dq_code
         
 
     def __repr__(self) -> str:
         return f"{self.time}"
 
+    def __eq__(self, __o: object) -> bool:
+        if type(__o) is not Result:
+            raise TypeError("Result object not equatable to objects of other types.")
+
+        if self.time != __o.time:
+            return False
+        if hasattr(self, "course") and self.course != __o.course:
+            return False
+        if hasattr(self, "split_distance") and self.split_distance != __o.split_distance:
+            return False
+        if hasattr(self, "splits") and self.splits != __o.splits:
+            return False
+        if hasattr(self, "rank") and self.rank != __o.rank:
+            return False
+        if hasattr(self, "points") and self.points != __o.points:
+            return False
+        
+        return True
+
+
 class Seed:
     time: Time
     course: str
     heat: int
     lane: int
     rank: int
 
-    def __init__(self, time:Time=None, time_str:str=None, course=None, heat=None, lane=None, rank=None) -> None:
+    def __init__(self, time:Time=None, time_str:str=None, course:str=None, heat:int=None, lane:int=None, rank:bool=None) -> None:
         if time is not None:
             self.time = time
         elif time_str is not None:
             self.time = Time(time_str)
 
         if course is not None:
             self.course = course
@@ -75,14 +116,26 @@
 
         if rank is not None:
             self.rank = int(rank)
 
     def __repr__(self) -> str:
         return f"{self.time}"
 
+    def __eq__(self, __o: object) -> bool:
+        if type(__o) is not Seed:
+            return TypeError("Seed object not equatable to obejcts of other types.")
+
+        if self.time != __o.time:
+            return False
+        if hasattr(self, "course") and self.course != __o.course:
+            return False
+        
+        return True
+        
+
 class AgeGroup:
     lower_age: int
     upper_age: int
 
     def __init__(self, lower_age:int, upper_age:int) -> None:
         self.lower_age = lower_age
         self.upper_age = upper_age
@@ -93,70 +146,109 @@
         elif self.lower_age <= 0 and self.upper_age < 100:
             return f"{self.upper_age} & Under"
         elif self.lower_age > 0 and self.upper_age >= 100:
             return f"{self.lower_age} & Over"
         else:
             return "Open"
 
+
 class Event:
-    number: str
+    number: int
+    letter: str
     distance: int
     stroke: str
     age_group: AgeGroup
     gender: str
+    is_relay: bool
 
-    def __init__(self, number:str, distance:int|str|float, stroke:str, age_group:AgeGroup, gender:str) -> None:
+    def __init__(self, number:int, letter:str, distance:int|str|float, stroke:str, age_group:AgeGroup, gender:str, is_relay:bool=False) -> None:
         self.number = number
+        self.letter = letter
         if type(distance) is str or type(distance) is float:
             self.distance = int(distance)
         elif type(distance) is int:
             self.distance = distance
         self.stroke= stroke
         self.age_group = age_group
         self.gender = gender.lower()
+        self.is_relay = is_relay
 
     def __repr__(self) -> str:
-        return f"{GENDERS_BG[self.gender]} {self.age_group} {self.distance} {self.stroke}"
+        relay = " Relay" if self.is_relay else ""
+        return f"{GENDERS_BG[self.gender]} {self.age_group} {self.distance} {self.stroke}{relay}"
+
+
+def calculate_usas_id(first_name: str, middle_name: str, last_name: str, birthday: date):
+    """Calculates the USA Swimming ID for the given values. i.e. Thomas Andrew Smith, 05/11/00 => 051100THOASMIT."""
+
+    def format(string: str, num_chars: int):
+        return re.sub(r"\W", "", string)[0:num_chars].ljust(num_chars,"*").upper()
+
+    bd = birthday.strftime("%m%d%y")
+    first = format(first_name, 3)
+    middle = format(middle_name, 1)
+    last = format(last_name, 4)
+
+    return f"{bd}{first}{middle}{last}"
 
 
 class Swimmer:
     first_name: str
     pref_name: str
     middle_name: str
     last_name: str
-    birthdate: str
+    birthday: str
     age: int
+    gender: str
+    desync_id: str
 
-    def __init__(self, full_name, age=None, birthdate=None, pref_name=None) -> None:
+    def __init__(self, full_name: str, age: int|str = None, birthday:str = None, pref_name: str = None, gender: str = None, id: str = None) -> None:
         name = parse_name(full_name)
         self.first_name = name["first_name"]
         if "middle_name" in name.keys():
             self.middle_name = name["middle_name"]
         else:
             self.middle_name = ""
         self.last_name = name["last_name"]
 
         if type(age) is str:
             self.age = int(age)
         elif type(age) is int:
             self.age = age
         
-        if birthdate is not None:
-            self.birthdate = birthdate
+        if birthday is not None:
+            self.birthday = birthday
+
+        if gender is not None:
+            self.gender = gender.lower()
 
         if pref_name is not None:
             self.pref_name = pref_name
 
+        if id is not None:
+            id = id.upper()
+            if self.middle_name == "" and id[9:10] != "*":
+                self.middle_name = id[9:10]
+            
+            if id != self.id:
+                self.desync_id = id
+                print(f"For swimmer: {full_name} USAS ID does not match given name and birthday. Given: {id}, Calculated: {self.id}")
+
     @property
     def id(self):
-        birthdate = self.birthdate
-        first = self.first_name[0:3].ljust(3,"*").upper()
-        middle = self.middle_name[0:1].ljust(1,"*").upper()
-        last = self.last_name[0:4].ljust(4,"*").upper()
-        return f"{birthdate}{first}{middle}{last}" 
+        try:
+            return calculate_usas_id(
+                first_name=self.first_name,
+                middle_name=self.middle_name,
+                last_name=self.last_name,
+                birthday=self.birthday
+            )
+        except:
+            print(f"Swimmer: {self.last_name}, {self.first_name} {self.middle_name} ")
+            return ""
 
     def __repr__(self) -> str:
         return self.full_pref_name
 
     @property
     def full_name(self):
         if hasattr(self, "middle_name"):
@@ -169,27 +261,36 @@
         first = self.pref_name if hasattr(self, "pref_name") else self.first_name
         return f"{self.last_name}, {first}"
 
 class IndividualEntry:
     event: Event
     swimmer: Swimmer
     seeds: Dict[str, Seed]
+    """Seeds keyed by event round character:
+    'p': Prelims
+    's': Swim Off
+    'f': Finals"""
     results: Dict[str, Result]
+    """Results keyed by event round character:
+    'p': Prelims
+    's': Swim Off
+    'f': Finals"""
 
     def __init__(self) -> None:
         self.seeds = {}
         self.results = {}
 
     def __repr__(self) -> str:
         return f"{self.swimmer} - {self.event}"
 
 class RelayEntry:
     event: Event
     identifier: str
     swimmers: Dict[str, Dict[int,Swimmer]]
+    """Swimmers keyed by relay order"""
     seeds: Dict[str, Seed]
     results: Dict[str, Result]
 
     def __init__(self) -> None:
         self.swimmers = {}
         self.seeds = {}
         self.results = {}
@@ -198,14 +299,15 @@
         return f"{self.event} - {self.identifier}"
 
 class Team:
     name: str
     code: str
     lsc: str
     swimmers: Dict[str, Swimmer]
+    """Swimmers keyed by USAS Id Number"""
 
     @property
     def points(self) -> float:
         individual_points = [entry.results["f"].points for entry in self.entries if "f" in entry.results and hasattr(entry.results["f"], "points")]
         ind_total = sum(individual_points)
         relay_points = [relay.results["f"].points for relay in self.relays if "f" in relay.results and hasattr(relay.results["f"], "points")]
         relay_total = sum(relay_points)
@@ -222,20 +324,25 @@
         self.relays = []
 
     def __repr__(self) -> str:
         return f"{self.name}"
 
 class Session:
     name: str
+    number: int
+    letter: str
     start: datetime
-    events: List[Event]
+    events: Dict[int, Event]
+    """Events keyed by numerical order within session"""
     course: str
 
-    def __init__(self, name, start, course) -> None:
+    def __init__(self, name, number, letter, start, course) -> None:
         self.name = name
+        self.number = number
+        self.letter = letter
         self.start = start
         self.course = course
         self.events = {}
 
     def __repr__(self) -> str:
         return self.name
 
@@ -243,40 +350,75 @@
     name: str
     address1: str
     address2: str
     city: str
     state: str
     zip: str
 
-    def __init__(self, name, address1, address2, city, state, zip) -> None:
+    def __init__(self, name, address1=None, address2=None, city=None, state=None, zip=None) -> None:
         self.name = name
-        self.address1 = address1
-        self.address2 = address2
-        self.city = city
-        self.state = state
-        self.zip = zip
+        if address1 is not None:
+            self.address1 = address1
+        if address2 is not None:
+            self.address2 = address2
+        if city is not None:
+            self.city = city
+        if state is not None:
+            self.state = state
+        if zip is not None:
+            self.zip = zip
 
     def __repr__(self) -> str:
         return f"{self.name}"
 
 class Meet:
     name: str
     facility: Facility
     start_date: date
     end_date: date
-    sessions: List[Session]
-    events: Dict[str, Event]
+    sessions: Dict[Tuple[int,str], Session]
+    """Session keyed by:
+    
+    (Session.number, Session.letter)"""
+    events: Dict[Tuple[int,str], Event]
+    """Events keyed by:
+    
+    (Event.number, Event.letter)"""
+    rounds: Dict[Tuple[int,str,int,str,str], Event]
+    """Session/Event relationships. Events keyed by:
+    
+    (Session.number, Session.letter, Event.number, Event.letter, round_type)
+    
+    round_type:
+    'p': Prelims
+    's': Swim Off
+    'f': Finals"""
     teams: Dict[str, Team]
-    entries: Dict[Tuple[str,str], IndividualEntry]
+    """Teams keyed by:
+    
+    (Team.code, Team.lsc)"""
+    swimmers: Dict[Tuple[str, str], Swimmer]
+    """Swimmers keyed by:
+    
+    (Swimmer.id, Team.code)"""
+    entries: Dict[Tuple[int,str,str], IndividualEntry]
+    """Individual Entries keyed by:
+    
+    (Event.number, Event.letter, Swimmer.id)"""
     relays: Dict[Tuple[str,str,str], RelayEntry]
+    """Relay Entries keyed by:
+    
+    (Event.number, Event.letter, Team.code, RelayEntry.identifier)"""
 
     def __init__(self) -> None:
         self.sessions = {}
         self.events = {}
+        self.rounds = {}
         self.teams = {}
+        self.swimmers = {}
         self.entries = {}
         self.relays = {}
 
     def __repr__(self) -> str:
         return self.name
 
 
@@ -288,15 +430,15 @@
     m = re.match(r"^(?P<last_name>.*), (?P<first_name>.*)$", name)
     if m is not None:
         return m.groupdict()
 
     raise ValueError("Name not properly formatted")   
     
 
-def read(input):
+def read_cl2(input):
     """Read .cl2 file into Meet object"""
     if type(input) is str:
         lines = input.split("\n")
     elif type(input) is list:
         lines = input
     elif type(input) is bytes:
         lines = input.decode("utf-8").split("\n")
@@ -325,15 +467,15 @@
         
         if type(active_record) is TeamIDRecord:
             active_team = Team(name=active_record.team_name, code=active_record.team_code, lsc=active_record.lsc_code)
             meet.teams[active_team.code] = active_team
 
         elif type(active_record) is IndividualEventRecord:
             if active_swimmer is None or active_record.swimmer_name != active_swimmer.full_name:
-                active_swimmer = Swimmer(full_name=active_record.swimmer_name, age=active_record.swimmer_age, birthdate=active_record.swimmer_birthdate)
+                active_swimmer = Swimmer(full_name=active_record.swimmer_name, age=active_record.swimmer_age, birthday=active_record.swimmer_birthday, gender=active_record.swimmer_sex)
 
                 if active_swimmer.id in active_team.swimmers:
                     active_swimmer = active_team.swimmers[active_swimmer.id]
                 else:
                     active_team.swimmers[active_swimmer.id] = active_swimmer
             
             active_entry = IndividualEntry()
@@ -409,15 +551,15 @@
                     active_entry.seeds["f"] = Seed(time_str=active_record.prelim_time, rank=active_record.prelim_rank, course=active_record.prelim_course, heat=active_record.final_heat, lane=active_record.final_lane)
             
             if hasattr(active_record, "final_time") and active_record.final_time != "NS" and active_record.final_time != "DQ":
                 points = active_record.points if hasattr(active_record, "points") else None
                 active_entry.results["f"]= Result(type="f", rank=active_record.final_rank, points=points, time_str=active_record.final_time, course=active_record.final_course)
 
         elif type(active_record) is RelayNameRecord:
-            active_swimmer = Swimmer(full_name=active_record.swimmer_name, birthdate=active_record.swimmer_birthdate, age=active_record.swimmer_birthdate)
+            active_swimmer = Swimmer(full_name=active_record.swimmer_name, birthday=active_record.swimmer_birthday, age=active_record.swimmer_birthdate)
             if active_swimmer.id in active_team.swimmers:
                 active_swimmer = active_team.swimmers[active_swimmer.id]
             
             active_entry.swimmers.append(active_swimmer)
         
         elif type(active_record) is SplitsRecord:
             try:
@@ -429,141 +571,409 @@
                 if hasattr(active_record, f"time_{i + 1}"):
                     time = getattr(active_record, f"time_{i + 1}")
                     if active_record.swim_code.lower() in active_entry.results:
                         active_entry.results[active_record.swim_code.lower()].splits.append(Time(time)) 
 
     return meet
 
-def process_result(cursor, query):
+_CONDITIONS = {
+    lambda _, val: type(val) is str: lambda x: str.rstrip(x),
+    lambda key, _: key in [
+        "Sess_rnd",
+        "Event_round",
+        "Rnd_ltr",
+    ]: lambda x: str.lower(x),
+    lambda key, _: key in [
+        "Reg_no",
+    ]: lambda x: str.upper(x)
+}
+
+def sanitize(key, value):
+    for condition in _CONDITIONS:
+        if condition(key, value):
+            value = _CONDITIONS[condition](value)
+    return value
+
+def process_result(cursor: Cursor, query: str) -> Dict[str, Any]:
     cursor.execute(query)
     result = cursor.fetchone()
     columns = [column[0] for column in cursor.description]
-    return dict(zip(columns, result))
+    out = dict(zip(columns, result))
+    return {key: sanitize(key, out[key]) for key in out}
 
-def process_results(cursor, query):
+def process_results(cursor: Cursor, query: str) -> Dict[str, Any]:
     cursor.execute(query)
     results = cursor.fetchall()
     columns = [column[0] for column in cursor.description]
-    return [dict(zip(columns, result)) for result in results]
+    outs = [dict(zip(columns, result)) for result in results]
+    return [{key: sanitize(key, out[key]) for key in out} for out in outs]
 
-def create_entry(props, type:Type):
+def create_entry(props: Dict[str, Any], type: Type) -> IndividualEntry | RelayEntry:
+    """Creates an entry object from the properties returned in a valid entry query"""
     entry_obj = type()
 
-    if props["ActualSeed_time"] is not None:
-        seed_time = Time(int(round(props["ActualSeed_time"]*100)))
-        if props["Pre_heat"] != 0:
-            entry_obj.seeds["p"] = Seed(time=seed_time, course=props["ActSeed_course"], heat=props["Pre_heat"], lane=props["Pre_lane"])
-        elif props["Fin_heat"] != 0:
-            entry_obj.seeds["f"] = Seed(time=seed_time, course=props["ActSeed_course"], heat=props["Fin_heat"], lane=props["Fin_lane"])
-
-    if props["Pre_Time"] is not None:
-        prelim_time = Time(int(round(props["Pre_Time"]*100)))
-        entry_obj.results["p"] = Result(time=prelim_time, type="p", course=props["Pre_course"], rank=props["Pre_place"])
-        if props["Pre_heat"] != 0 and props["Fin_heat"] != 0:
-            entry_obj.seeds["f"] = Seed(time=prelim_time, course=props["Pre_course"], heat=props["Fin_heat"], lane=props["Fin_lane"])
-    
-    #TODO: Process DQ information
-    if props["Fin_Time"] is not None:
-        final_time = Time(int(round(props["Fin_Time"]*100)))
-        entry_obj.results["f"] = Result(time=final_time, type="f", course=props["Fin_course"], rank=props["Fin_place"])
+    def is_valid(time):
+        return time is not None and time != 0
+
+    if is_valid(props["Pre_heat"]):
+        if is_valid(props["ActualSeed_time"]):
+            seed_time = Time(props["ActualSeed_time"])
+        else:
+            seed_time = Time(0)
+
+        entry_obj.seeds["p"] = Seed(
+            time=seed_time,
+            course=props["ActSeed_course"],
+            heat=props["Pre_heat"],
+            lane=props["Pre_lane"]
+        )
+
+    if is_valid(props["Fin_heat"]):
+        if is_valid(props["Pre_Time"]):
+            seed_time = Time(props["Pre_Time"])
+        elif is_valid(props["ActualSeed_time"]):
+            seed_time = Time(props["ActualSeed_time"])
+        else:
+            seed_time = Time(0)
+
+        entry_obj.seeds["f"] = Seed(
+            time=seed_time,
+            course=props["ActSeed_course"],
+            heat=props["Fin_heat"],
+            lane=props["Fin_lane"]
+        )
+
+    if "p" in entry_obj.seeds:
+        prelim_time = Time(0)
+        prelim_dq = False
+        
+        if is_valid(props["Pre_Time"]):
+            prelim_time = Time(props["Pre_Time"])
+
+        if hasattr(props, "Pre_stat"):
+            prelim_dq = props["Pre_stat"] == "Q"
+
+        entry_obj.results["p"] = Result(
+            time=prelim_time,
+            type="p",
+            course=props["Pre_course"],
+            rank=props["Pre_place"],
+            is_dq=prelim_dq,
+        )
+    
+    if "f" in entry_obj.seeds:
+        final_time = Time(0)
+        final_dq = False
+
+        if is_valid(props["Fin_Time"]):
+            final_time = Time(props["Fin_Time"])
+
+        if hasattr(props, "Fin_stat"):
+            final_dq = props["Fin_stat"] == "Q"
+        
+
+        entry_obj.results["f"] = Result(
+            time=final_time,
+            type="f",
+            course=props["Fin_course"],
+            rank=props["Fin_place"],
+            points=props["Ev_score"],
+            is_dq=final_dq,
+        )
 
     return entry_obj
 
 MDB_STROKES = {
     "A": "Free", 
     "B": "Back",
     "C": "Breast",
     "D": "Fly",
     "E": "Medley",
 }
 
-def read_mdb(path):
+def read_mdb(path: str) -> Meet:
+    """Reads a MeetManager formatted .mdb file into memory as a Meet object"""
     if not os.path.isfile(path) or not os.path.splitext(path)[1] == ".mdb":
         return
     
     connection_string = "Driver={Microsoft Access Driver (*.mdb, *.accdb)};Dbq=" + path + ";Uid=Admin;Pwd=TeP69s)lAd_mW-(J_72u"
     connection = connect(connection_string)
     cursor = connection.cursor()
 
     meet = Meet()
+    desync_ids = {}
 
     # Meet
-    query = "SELECT Meet_name1, Meet_location, Meet_addr1, Meet_addr2, Meet_city, Meet_state from Meet"
+    query = """
+            SELECT
+                Meet_name1, Meet_location, Meet_addr1,
+                Meet_addr2, Meet_city, Meet_state,
+                Meet_zip, Meet_start, Meet_end
+            from Meet
+            """
     result = process_result(cursor, query)
-    meet.name = result["Meet_name1"].rstrip()
-    meet.facility = Facility(name=result["Meet_location"], address1=result["Meet_addr1"], city=result["Meet_city"], state=result["Meet_state"], zip=result["Meet_zip"])
-    
+    meet.name = result["Meet_name1"]
+    meet.facility = Facility(
+        name=result["Meet_location"],
+        address1=result["Meet_addr1"],
+        city=result["Meet_city"],
+        state=result["Meet_state"],
+        zip=result["Meet_zip"],
+    )
+    meet.start_date = result["Meet_start"]
+    meet.end_date = result["Meet_end"]
+
     # Sessions
-    query = "SELECT Sess_no, Sess_name, Sess_starttime, Sess_course FROM Session"
+    query = """
+            SELECT
+                Sess_no, Sess_ltr, Sess_name,
+                Sess_day, Sess_starttime, Sess_course
+            FROM Session
+            """
     for result in process_results(cursor, query):
-        meet.sessions[result["Sess_no"]] = Session(result["Sess_name"], result["Sess_starttime"], result["Sess_course"])
+        start_time = meet.start_date + timedelta(days=result["Sess_day"]-1, seconds=result["Sess_starttime"])
+
+        session = Session(
+            name=result["Sess_name"],
+            number=result["Sess_no"],
+            letter=result["Sess_ltr"],
+            start=start_time,
+            course=result["Sess_course"],
+        )
+
+        meet.sessions[result["Sess_no"], result["Sess_ltr"]] = session
 
     # Events
-    query = "SELECT Event_no, Event_dist, Event_stroke, Low_age, High_age, Event_gender FROM Event"
-    events = process_results(cursor, query)
-    for event in events:
-        meet.events[event["Event_no"]] = Event(event["Event_no"], event["Event_dist"], MDB_STROKES[event["Event_stroke"]], AgeGroup(int(event["Low_age"]),int(event["High_age"])), event["Event_gender"])
+    query = """
+            SELECT
+                Event_no, Event_ltr, Event_dist,
+                Event_stroke, Low_age, High_age,
+                Event_gender, Ind_rel
+            FROM Event
+            """
+    for result in process_results(cursor, query):
+
+        event = Event(
+            number=result["Event_no"],
+            letter=result["Event_ltr"],
+            distance=result["Event_dist"],
+            stroke=MDB_STROKES[result["Event_stroke"]],
+            age_group=AgeGroup(int(result["Low_age"]),int(result["High_age"])),
+            gender=result["Event_gender"],
+            is_relay=result["Ind_rel"] == "R"
+        )
+
+        meet.events[result["Event_no"], result["Event_ltr"]] = event
 
     # Session Events
-    query = "SELECT Sess_no, Sess_order, Event_no FROM (Sessitem LEFT JOIN Session ON Sessitem.Sess_ptr = Session.Sess_ptr) LEFT JOIN Event on Sessitem.Event_ptr = Event.Event_ptr"
+    query = """
+            SELECT
+                Sess_no, Sess_ltr, Sess_order,
+                Sess_rnd, Event_no, Event_ltr
+            FROM (Sessitem 
+            LEFT JOIN Session ON Sessitem.Sess_ptr = Session.Sess_ptr)
+            LEFT JOIN Event on Sessitem.Event_ptr = Event.Event_ptr
+            """
     for result in process_results(cursor, query):
-        meet.sessions[result["Sess_no"]].events[result["Sess_order"]] = meet.events[result["Event_no"]]
+
+        event = meet.events[(
+            result["Event_no"],
+            result["Event_ltr"],
+        )]
+
+        meet.rounds[
+            result["Sess_no"],
+            result["Sess_ltr"],
+            result["Event_no"],
+            result["Event_ltr"],
+            result["Sess_rnd"],
+        ] = event
+        meet.sessions[
+            result["Sess_no"],
+            result["Sess_ltr"],
+        ].events[result["Sess_order"]] = (
+            result["Sess_rnd"],
+            event
+        )
 
     # Teams
-    cursor.execute("SELECT Team_name, Team_abbr, Team_lsc from Team")
-    teams = cursor.fetchall()
-    meet.teams = {team[1].rstrip(): Team(name=team[0].rstrip(), code=team[1].rstrip(), lsc=team[2].rstrip()) for team in teams}
+    query = """
+            SELECT
+                Team_name, Team_abbr, Team_lsc
+            FROM Team
+            """
+    for result in process_results(cursor, query):
+        team = Team(
+            name=result["Team_name"],
+            code=result["Team_abbr"],
+            lsc=result["Team_lsc"],
+        )
+
+        meet.teams[result["Team_abbr"], result["Team_lsc"]] = team
 
     # Swimmers
-    query = "SELECT Team_abbr, Reg_no, Last_name, First_name, Initial, Pref_name FROM Athlete LEFT JOIN Team ON Athlete.Team_no = Team.Team_no"
-    swimmers = process_results(cursor, query)
-    for swimmer in swimmers:
-        full_name = f"{swimmer['Last_name'].rstrip()}, {swimmer['First_name'].rstrip()} {swimmer['Initial'].rstrip()}".rstrip()
-        pref_name = swimmer["Pref_name"].rstrip() if swimmer["Pref_name"].rstrip() != "" else None
+    query = """
+            SELECT 
+                Team_abbr, Team_lsc, Reg_no,
+                Last_name, First_name, Initial,
+                Pref_name, Birth_date, Ath_sex 
+            FROM Athlete 
+            LEFT JOIN Team ON Athlete.Team_no = Team.Team_no
+            """
+    for result in process_results(cursor, query):
+        full_name = f"{result['Last_name']}, {result['First_name']} {result['Initial']}"
+        pref_name = result["Pref_name"] if result["Pref_name"] != "" else None
+
+        swimmer = Swimmer(
+            full_name=full_name,
+            pref_name=pref_name,
+            birthday=result["Birth_date"],
+            gender=result["Ath_sex"],
+            id=result["Reg_no"],
+        )
+
+        if hasattr(swimmer, "desync_id"):
+            desync_ids[swimmer.desync_id] = swimmer.id
+
+        if result["Reg_no"] in desync_ids:
+            result["Reg_no"] = desync_ids[result["Reg_no"]]
+
+        meet.swimmers[result["Reg_no"]] = swimmer
+        meet.teams[result["Team_abbr"], result["Team_lsc"]].swimmers[result["Reg_no"]] = swimmer
 
-        meet.teams[swimmer["Team_abbr"].rstrip()].swimmers[swimmer["Reg_no"]] = Swimmer(full_name=full_name, pref_name=pref_name)
-    
     # Individual Entries/Results
-    query = "SELECT ActualSeed_time, ActSeed_course, Pre_heat, Pre_lane, Pre_Time, Pre_course, Pre_place, Fin_heat, Fin_lane, Fin_Time, Fin_course, Fin_place, Ev_score, Reg_no, Team_abbr, Event_no FROM ((Entry LEFT JOIN Athlete ON Entry.Ath_no = Athlete.Ath_no) LEFT JOIN Team ON Athlete.Team_no = Team.Team_no) LEFT JOIN Event ON Entry.Event_ptr = Event.Event_ptr"
-    entries = process_results(cursor, query)
-    for props in entries:
-        entry = create_entry(props, IndividualEntry)
-        entry.event = meet.events[props["Event_no"]]
-        entry.swimmer = meet.teams[props["Team_abbr"].rstrip()].swimmers[props["Reg_no"]]
+    query = """
+            SELECT
+                ActualSeed_time, ActSeed_course, Pre_heat,
+                Pre_lane, Pre_Time, Pre_course,
+                Pre_stat, Pre_place, Fin_heat,
+                Fin_lane, Fin_Time, Fin_course, Fin_stat,
+                Fin_place, fin_dqofficial, Ev_score,
+                Reg_no, Team_abbr, Team_lsc,
+                Event_no, Event_ltr
+            FROM ((Entry
+            LEFT JOIN Athlete ON Entry.Ath_no = Athlete.Ath_no)
+            LEFT JOIN Team ON Athlete.Team_no = Team.Team_no)
+            LEFT JOIN Event ON Entry.Event_ptr = Event.Event_ptr
+            """
+    for result in process_results(cursor, query):
 
-        meet.entries[(props["Event_no"],props["Reg_no"])] = entry
+        if result["Reg_no"] in desync_ids:
+            result["Reg_no"] = desync_ids[result["Reg_no"]]
+
+        entry = create_entry(result, IndividualEntry)
+        entry.event = meet.events[result["Event_no"], result["Event_ltr"]]
+        entry.swimmer = meet.teams[result["Team_abbr"], result["Team_lsc"]].swimmers[result["Reg_no"]]
+
+        meet.entries[result["Event_no"],result["Event_ltr"],result["Reg_no"]] = entry
 
     # Relay Entries/Results
-    query = "SELECT ActualSeed_time, ActSeed_course, Pre_heat, Pre_lane, Pre_Time, Pre_course, Pre_place, Fin_heat, Fin_lane, Fin_Time, Fin_course, Fin_place, Ev_score, Team_ltr, Team_abbr, Event_no FROM (Relay Left JOIN Team on Relay.Team_no = Team.Team_no) LEFT JOIN Event on Relay.Event_ptr = Event.Event_ptr"
-    relays = process_results(cursor, query)
-    for props in relays:
-        entry = create_entry(props, RelayEntry)
-        entry.event = meet.events[props["Event_no"]]
-        entry.identifier = props["Team_ltr"]
+    query = """
+            SELECT
+                ActualSeed_time, ActSeed_course, Pre_heat,
+                Pre_lane, Pre_Time, Pre_course,
+                Pre_stat, Pre_place, Fin_heat, Fin_lane,
+                Fin_Time, Fin_course, Fin_place,
+                Fin_stat, fin_dqofficial, Ev_score,
+                Team_ltr, Team_abbr, Event_no,
+                Event_ltr
+            FROM (Relay
+            LEFT JOIN Team on Relay.Team_no = Team.Team_no)
+            LEFT JOIN Event on Relay.Event_ptr = Event.Event_ptr
+            """
+    for result in process_results(cursor, query):
 
-        meet.relays[(props["Event_no"],props["Team_abbr"].rstrip(),props["Team_ltr"])] = entry
+        entry = create_entry(result, RelayEntry)
+        entry.event = meet.events[result["Event_no"], result["Event_ltr"]]
+        entry.identifier = result["Team_ltr"]
+
+        meet.relays[
+            result["Event_no"],
+            result["Event_ltr"],
+            result["Team_abbr"],
+            result["Team_ltr"],
+        ] = entry
 
     # Relay Swimmers
-    query = "SELECT Event_no, Team_abbr, RelayNames.Team_ltr, Reg_no, Event_round, Pos_no FROM (((RelayNames LEFT JOIN Relay ON RelayNames.Relay_no=Relay.Relay_no) LEFT JOIN Team ON RelayNames.Team_no = Team.Team_no) LEFT JOIN Athlete ON RelayNames.Ath_no=Athlete.Ath_no) LEFT JOIN Event on RelayNames.Event_ptr=Event.Event_ptr"
-    for props in process_results(cursor, query):
-        if props["Event_round"].lower() not in meet.relays[(props["Event_no"],props["Team_abbr"].rstrip(),props["Team_ltr"])].swimmers:
-            meet.relays[(props["Event_no"],props["Team_abbr"].rstrip(),props["Team_ltr"])].swimmers[props["Event_round"].lower()] = {}
-        meet.relays[(props["Event_no"],props["Team_abbr"].rstrip(),props["Team_ltr"])].swimmers[props["Event_round"].lower()][props["Pos_no"]] = meet.teams[props["Team_abbr"].rstrip()].swimmers[props["Reg_no"]]
+    query = """
+            SELECT
+                Event_no, Event_ltr, Team_abbr,
+                Team_lsc, RelayNames.Team_ltr, Reg_no,
+                Event_round, Pos_no
+            FROM (((RelayNames
+            LEFT JOIN Relay ON RelayNames.Relay_no=Relay.Relay_no)
+            LEFT JOIN Team ON RelayNames.Team_no = Team.Team_no)
+            LEFT JOIN Athlete ON RelayNames.Ath_no=Athlete.Ath_no)
+            LEFT JOIN Event on RelayNames.Event_ptr=Event.Event_ptr
+            """
+    for result in process_results(cursor, query):
+
+        if result["Reg_no"] in desync_ids:
+            result["Reg_no"] = desync_ids[result["Reg_no"]]
+
+        if result["Event_round"] not in meet.relays[(result["Event_no"],result["Event_ltr"],result["Team_abbr"],result["Team_ltr"])].swimmers:
+            meet.relays[
+                result["Event_no"],
+                result["Event_ltr"],
+                result["Team_abbr"],
+                result["Team_ltr"],
+            ].swimmers[result["Event_round"]] = {}
+
+        meet.relays[
+            result["Event_no"],
+            result["Event_ltr"],
+            result["Team_abbr"],
+            result["Team_ltr"],
+        ].swimmers[result["Event_round"]][result["Pos_no"]] = meet.teams[result["Team_abbr"], result["Team_lsc"]].swimmers[result["Reg_no"]]
 
     # Individual Splits
-    query = "SELECT Event_no, Reg_no, Team_abbr, Rnd_ltr, Split_no, Split_Time FROM ((Split LEFT JOIN Athlete ON Split.Ath_no=Athlete.Ath_no) LEFT JOIN Team ON Athlete.Team_no=Team.Team_no) LEFT JOIN Event ON Split.Event_ptr=Event.Event_ptr WHERE Split.Ath_no IS NOT NULL AND Split.Ath_no <> 0"
+    query = """
+            SELECT
+                Event_no, Event_ltr, Reg_no,
+                Team_abbr, Rnd_ltr, Split_no,
+                Split_Time
+            FROM ((Split
+            LEFT JOIN Athlete ON Split.Ath_no=Athlete.Ath_no)
+            LEFT JOIN Team ON Athlete.Team_no=Team.Team_no)
+            LEFT JOIN Event ON Split.Event_ptr=Event.Event_ptr
+                WHERE Split.Ath_no IS NOT NULL AND Split.Ath_no <> 0
+            """
     splits = process_results(cursor, query)
-    for props in splits:
-        meet.entries[(props["Event_no"],props["Reg_no"])].results[props["Rnd_ltr"].lower()].splits[props["Split_no"]] = Time(int(round(props["Split_Time"]*100)))
+    for result in splits:
+
+        if result["Reg_no"] in desync_ids:
+            result["Reg_no"] = desync_ids[result["Reg_no"]]
+
+        if result["Rnd_ltr"] in meet.entries[result["Event_no"],result["Event_ltr"],result["Reg_no"]].results:
+            meet.entries[(
+                result["Event_no"],
+                result["Event_ltr"],
+                result["Reg_no"],
+            )].results[result["Rnd_ltr"]].splits[result["Split_no"]] = Time(result["Split_Time"])
 
     # Relay Splits
-    query = "SELECT Event_no, Team_abbr, Relay.Team_ltr, Rnd_ltr, Split_no, Split_Time FROM ((Split Left Join Relay ON Split.Relay_no=Relay.Relay_no) LEFT JOIN Team on Relay.Team_no=Team.Team_no) LEFT JOIN Event ON Split.Event_ptr=Event.Event_ptr WHERE Split.Relay_no IS NOT NULL AND Split.Relay_no <> 0"
+    query = """
+            SELECT
+                Event_no, Event_ltr, Team_abbr,
+                Relay.Team_ltr, Rnd_ltr, Split_no,
+                Split_Time
+            FROM ((Split
+            LEFT JOIN Relay ON Split.Relay_no=Relay.Relay_no)
+            LEFT JOIN Team on Relay.Team_no=Team.Team_no)
+            LEFT JOIN Event ON Split.Event_ptr=Event.Event_ptr
+                WHERE Split.Relay_no IS NOT NULL AND Split.Relay_no <> 0
+            """
     splits = process_results(cursor, query)
     for props in splits:
-        meet.relays[(props["Event_no"],props["Team_abbr"].rstrip(),props["Team_ltr"])].results[props["Rnd_ltr"].lower()].splits[props["Split_no"]] = Time(int(round(props["Split_Time"]*100)))
+        meet.relays[(
+            props["Event_no"],
+            props["Event_ltr"],
+            props["Team_abbr"],
+            props["Team_ltr"],
+        )].results[props["Rnd_ltr"]].splits[props["Split_no"]] = Time(props["Split_Time"])
 
     return meet
 
 
 def is_valid_path(path):
     """Validates path to ensure it is valid in the current file system"""
 
@@ -610,8 +1020,8 @@
     # print(meet.teams["FRST"].points)
     # team_scores = [{"team": team, "score": team.points} for team in meet.teams.values()]
     # team_scores.sort(key=lambda x: x["score"], reverse=True)
     print(meet)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `sdif_toolkit-0.1.6/src/sdif_toolkit/records.py` & `sdif-toolkit-0.1.7/src/sdif_toolkit/records.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     code: str
     org_code: str
     swimmer_name: str
     swimmer_id: str
     "Incomplete swimmer USAS ID, omits the final 2 characters"
     attach_code: str
     citizen_code: str
-    swimmer_birthdate: str
+    swimmer_birthday: str
     swimmer_age: str
     swimmer_sex: str
     event_sex: str
     event_distance: str
     event_stroke: str
     event_number: str
     event_lower_age: str
@@ -272,15 +272,15 @@
     encodings = {
         "code": (0,2),
         "org_code": (2,3),
         "swimmer_name": (11,39),
         "swimmer_id": (39,51),
         "attach_code": (51,52),
         "citizen_code": (52,55),
-        "swimmer_birthdate": (55,63),
+        "swimmer_birthday": (55,63),
         "swimmer_age": (63,65),
         "swimmer_sex": (65,66),
         "event_sex": (66,67),
         "event_distance": (67,71),
         "event_stroke": (71,72),
         "event_number": (72,76),
         "event_lower_age": (76,78),
@@ -342,15 +342,15 @@
     org_code: str
     team_code: str
     team_code_ext: str
     swimmer_name: str
     swimmer_id: str
     attach_code: str
     citizen_code: str
-    swimmer_birthdate: str
+    swimmer_birthday: str
     swimmer_age: str
     swimmer_sex: str
     admin_info_1: str
     admin_info_4: str
     swimmer_phone_1: str
     swimmer_phone_2: str
     swimmer_reg_date: str
@@ -361,15 +361,15 @@
         "org_code": (2,3),
         "team_code": (11,17),
         "team_code_ext": (17,18),
         "swimmer_name": (18,46),
         "swimmer_id": (47,59),
         "attach_code": (59,60),
         "citizen_code": (60,63),
-        "swimmer_birthdate": (63,71),
+        "swimmer_birthday": (63,71),
         "swimmer_age": (71,73),
         "swimmer_sex": (73,74),
         "admin_info_1": (74,104),
         "admin_info_4": (104,124),
         "swimmer_phone_1": (124,136),
         "swimmer_phone_2": (136,148),
         "swimmer_reg_date": (148,156),
@@ -581,15 +581,15 @@
     code: str
     org_code: str
     team_code: str
     realy_id: str
     swimmer_name: str
     swimmer_id: str
     citizen_code: str
-    swimmer_birthdate: str
+    swimmer_birthday: str
     swimmer_age: str
     event_sex: str
     prelim_order: str
     swimoff_order: str
     final_order: str
     split_time: str
     split_course: str
@@ -601,15 +601,15 @@
         "code": (0,2),
         "org_code": (2,3),
         "team_code": (15,21),
         "relay_id": (21,22),
         "swimmer_name": (22,50),
         "swimmer_id": (50,62),
         "citizen_code": (62,65),
-        "swimmer_birthdate": (65,73),
+        "swimmer_birthday": (65,73),
         "swimmer_age": (73,75),
         "event_sex": (75,76),
         "prelim_order": (76,77),
         "swimoff_order": (77,78),
         "final_order": (78,79),
         "split_time": (79,87),
         "split_course": (87,88),
```

### Comparing `sdif_toolkit-0.1.6/src/sdif_toolkit/time.py` & `sdif-toolkit-0.1.7/src/sdif_toolkit/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,30 @@
         return self.minutes * 6000 + self.seconds * 100 + self.hundredths
 
     def __init__(self, time) -> None:
         if type(time) is int:
             self.minutes  = time // 6000
             self.seconds = (time % 6000) // 100
             self.hundredths = time % 100
+        elif type(time) is float:
+            int_value = int(round(time*100))
+            self.minutes = int_value // 6000
+            self.seconds = (int_value % 6000) // 100
+            self.hundredths = int_value % 100
         elif type(time) is str:
             m = re.match(r"(?P<minutes>\d*)?:?(?P<seconds>\d{2})[\.:]?(?P<hundredths>\d{1,2})?$", time)
 
             if m is None:
-                raise ValueError(f"Invalid time string: {time}")
+                if time == "NT" or int(time) == 0:
+                    self.minutes = 0
+                    self.seconds = 0
+                    self.hundredths = 0
+                    return
+                else:
+                    raise ValueError(f"Invalid time string: {time}")
 
             minutes = m.group("minutes")
             if minutes is None or minutes == "":
                 self.minutes = 0
             else:
                 self.minutes = int(minutes)
 
@@ -35,10 +46,20 @@
                 self.hundredths = 0
             elif len(hundredths) == 1:
                 self.hundredths = int(hundredths) * 10
             else:
                 self.hundredths = int(hundredths)
 
     def __repr__(self) -> str:
-        minutes = f"{self.minutes}:" if self.minutes > 0 else ""
-        return f"{minutes}{self.seconds:02d}.{self.hundredths:02d}"
-            
+        if self.value == 0:
+            return "NT"
+        else:
+            minutes = f"{self.minutes}:" if self.minutes > 0 else ""
+            return f"{minutes}{self.seconds:02d}.{self.hundredths:02d}"
+
+    def __eq__(self, __o: object) -> bool:
+        if type(__o) is int or type(__o) is str:
+            return self.value == Time(__o).value
+        elif type(__o) is Time:
+            return self.value == __o.value
+        else:
+            raise TypeError(f"Equality undefined for given type: {type(__o)}")
```

### Comparing `sdif_toolkit-0.1.6/tests/test_records.py` & `sdif-toolkit-0.1.7/tests/test_records.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import unittest
-from sdif_toolkit.records import FileDescriptionRecord, MeetRecord, SDIFRecord, TeamIDRecord
+
+from src.sdif_toolkit.records import (FileDescriptionRecord, MeetRecord,
+                                      SDIFRecord, TeamIDRecord)
+
 
 class TestSDIFRecord(unittest.TestCase):
 
     def test_init(self):
         line = "A01V3      02Meet Results                  Hy-Tek, Ltd         WMM 7.0Fb Hy-Tek, Ltd         866-456-511103062022                                    MM40    N42"
         self.assertEqual(SDIFRecord(line).code, "A0")
 
+
 class TestFileDescriptionRecord(unittest.TestCase):
 
     def test_init(self):
         line = "A01V3      02Meet Results                  Hy-Tek, Ltd         WMM 7.0Fb Hy-Tek, Ltd         866-456-511103062022                                    MM40    N42"
         record = FileDescriptionRecord(line)
 
         self.assertEqual(SDIFRecord(line).code, "A0")
@@ -22,14 +26,15 @@
         self.assertEqual(record.software_version, "WMM 7.0Fb")
         self.assertEqual(record.contact_name, "Hy-Tek, Ltd")
         self.assertEqual(record.contact_phone, "866-456-5111")
         self.assertEqual(record.file_creation_date, "03062022")
         with self.assertRaises(AttributeError):
             record.submitted_by_lsc
 
+
 class TestMeetRecord(unittest.TestCase):
 
     def test_init(self):
         line = "B11        2022 SE Indiana Divisional Cha2717 S Morgantown Rd                        Greenwood           IN46143     USA 0304202203062022   0        Y 500   N28"
         record = MeetRecord(line)
 
         self.assertEqual(SDIFRecord(line).code, "B1")
@@ -43,81 +48,91 @@
         self.assertEqual(record.start_date, "03042022")
         self.assertEqual(record.end_date, "03062022")
         self.assertEqual(record.altitude, "0")
         self.assertEqual(record.course, "Y")
         with self.assertRaises(AttributeError):
             record.address_2
 
+
 class TestMeetHostRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestTeamIDRecord(unittest.TestCase):
 
     def test_init(self):
         line = "C11IN      INFRSTFranklin Regional Swim Team                   654 Walnut St.                              Franklin            IN46131                       N85"
         record = TeamIDRecord(line)
 
         self.assertEqual(SDIFRecord(line).code, "C1")
         self.assertEqual(record.code, "C1")
         self.assertEqual(record.org_code, "1")
-        self.assertEqual(record.team_code, "INFRST")
+        self.assertEqual(record.lsc_code, "IN")
+        self.assertEqual(record.team_code, "FRST")
         self.assertEqual(record.team_name, "Franklin Regional Swim Team")
         self.assertEqual(record.address_1, "654 Walnut St.")
         self.assertEqual(record.city, "Franklin")
         self.assertEqual(record.state, "IN")
         self.assertEqual(record.zip, "46131")
-        
+
         with self.assertRaises(AttributeError):
             record.team_name_abbr
         with self.assertRaises(AttributeError):
             record.address_2
         with self.assertRaises(AttributeError):
             record.region
         with self.assertRaises(AttributeError):
             record.team_code_ext
 
+
 class TestTeamEntryRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestIndividualEventRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestIndividualAdministrativeRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestIndividualContactRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestIndividualInformationRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestRelayEventRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestRelayNameRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
+
 class TestSplitsRecord(unittest.TestCase):
 
     def test_init(self):
         raise NotImplementedError
 
 
-
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `sdif_toolkit-0.1.6/LICENSE` & `sdif-toolkit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sdif_toolkit-0.1.6/pyproject.toml` & `sdif-toolkit-0.1.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdif-toolkit"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Colin Mothersead", email="cmothersead@gmail.com" },
 ]
 description = "Utility to read and process swimming data files"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "pyodbc"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/cmothersead/sdif-toolkit"
 "Bug Tracker" = "https://github.com/cmothersead/sdif-toolkit/issues"
```

### Comparing `sdif_toolkit-0.1.6/PKG-INFO` & `sdif-toolkit-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-Metadata-Version: 2.1
-Name: sdif-toolkit
-Version: 0.1.6
-Summary: Utility to read and process swimming data files
-Project-URL: Homepage, https://github.com/cmothersead/sdif-toolkit
-Project-URL: Bug Tracker, https://github.com/cmothersead/sdif-toolkit/issues
-Author-email: Colin Mothersead <cmothersead@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 Colin Mothersead
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
-# SDIF Tools
-
-SDIF reader provides a set of classes built from the Swimming Data Interchange Format V3. The specification document was pulled from the US Masters Swimming website and is provided in this repository for reference.
+Metadata-Version: 2.1
+Name: sdif-toolkit
+Version: 0.1.7
+Summary: Utility to read and process swimming data files
+Author-email: Colin Mothersead <cmothersead@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2022 Colin Mothersead
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/cmothersead/sdif-toolkit
+Project-URL: Bug Tracker, https://github.com/cmothersead/sdif-toolkit/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SDIF Tools
+
+SDIF reader provides a set of classes built from the Swimming Data Interchange Format V3. The specification document was pulled from the US Masters Swimming website and is provided in this repository for reference.
```

