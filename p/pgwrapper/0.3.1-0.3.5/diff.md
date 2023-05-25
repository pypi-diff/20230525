# Comparing `tmp/pgwrapper-0.3.1.tar.gz` & `tmp/pgwrapper-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgwrapper-0.3.1.tar", last modified: Tue Mar 14 04:32:19 2023, max compression
+gzip compressed data, was "pgwrapper-0.3.5.tar", last modified: Thu May 25 14:30:37 2023, max compression
```

## Comparing `pgwrapper-0.3.1.tar` & `pgwrapper-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lyuande  (1059746653) mts        (201)        0 2023-03-14 04:32:19.205132 pgwrapper-0.3.1/
--rw-r--r--   0 lyuande  (1059746653) mts        (201)    35108 2023-03-14 03:07:16.000000 pgwrapper-0.3.1/LICENSE
--rw-r--r--   0 lyuande  (1059746653) mts        (201)       43 2023-03-14 03:07:16.000000 pgwrapper-0.3.1/MANIFEST.in
--rw-r--r--   0 lyuande  (1059746653) mts        (201)     3109 2023-03-14 04:32:19.205132 pgwrapper-0.3.1/PKG-INFO
--rw-r--r--   0 lyuande  (1059746653) mts        (201)     2456 2023-03-14 03:22:50.000000 pgwrapper-0.3.1/README.md
-drwxr-xr-x   0 lyuande  (1059746653) mts        (201)        0 2023-03-14 04:32:19.201146 pgwrapper-0.3.1/pgwrapper/
--rw-r--r--   0 lyuande  (1059746653) mts        (201)      127 2023-03-14 03:07:16.000000 pgwrapper-0.3.1/pgwrapper/__init__.py
--rw-r--r--   0 lyuande  (1059746653) mts        (201)     4805 2023-03-14 03:07:16.000000 pgwrapper-0.3.1/pgwrapper/pgpool.py
--rw-r--r--   0 lyuande  (1059746653) mts        (201)     9234 2023-03-14 03:22:56.000000 pgwrapper-0.3.1/pgwrapper/pgwrap.py
-drwxr-xr-x   0 lyuande  (1059746653) mts        (201)        0 2023-03-14 04:32:19.205132 pgwrapper-0.3.1/pgwrapper.egg-info/
--rw-r--r--   0 lyuande  (1059746653) mts        (201)     3109 2023-03-14 04:32:19.000000 pgwrapper-0.3.1/pgwrapper.egg-info/PKG-INFO
--rw-r--r--   0 lyuande  (1059746653) mts        (201)      264 2023-03-14 04:32:19.000000 pgwrapper-0.3.1/pgwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 lyuande  (1059746653) mts        (201)        1 2023-03-14 04:32:19.000000 pgwrapper-0.3.1/pgwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 lyuande  (1059746653) mts        (201)       16 2023-03-14 04:32:19.000000 pgwrapper-0.3.1/pgwrapper.egg-info/requires.txt
--rw-r--r--   0 lyuande  (1059746653) mts        (201)       10 2023-03-14 04:32:19.000000 pgwrapper-0.3.1/pgwrapper.egg-info/top_level.txt
--rw-r--r--   0 lyuande  (1059746653) mts        (201)       38 2023-03-14 04:32:19.205132 pgwrapper-0.3.1/setup.cfg
--rw-r--r--   0 lyuande  (1059746653) mts        (201)     1116 2023-03-14 04:32:15.000000 pgwrapper-0.3.1/setup.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-05-25 14:30:37.410358 pgwrapper-0.3.5/
+-rw-r--r--   0 richard    (501) staff       (20)    35108 2023-05-25 13:08:55.000000 pgwrapper-0.3.5/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)       43 2023-05-25 13:08:55.000000 pgwrapper-0.3.5/MANIFEST.in
+-rw-r--r--   0 richard    (501) staff       (20)     3404 2023-05-25 14:30:37.409776 pgwrapper-0.3.5/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)     2750 2023-05-25 13:08:55.000000 pgwrapper-0.3.5/README.md
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-05-25 14:30:37.406087 pgwrapper-0.3.5/pgwrapper/
+-rw-r--r--   0 richard    (501) staff       (20)      127 2023-05-25 13:08:55.000000 pgwrapper-0.3.5/pgwrapper/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)     4987 2023-05-25 13:40:12.000000 pgwrapper-0.3.5/pgwrapper/pgpool.py
+-rw-r--r--   0 richard    (501) staff       (20)     9005 2023-05-25 14:28:32.000000 pgwrapper-0.3.5/pgwrapper/pgwrap.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-05-25 14:30:37.409034 pgwrapper-0.3.5/pgwrapper.egg-info/
+-rw-r--r--   0 richard    (501) staff       (20)     3404 2023-05-25 14:30:37.000000 pgwrapper-0.3.5/pgwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)      264 2023-05-25 14:30:37.000000 pgwrapper-0.3.5/pgwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 richard    (501) staff       (20)        1 2023-05-25 14:30:37.000000 pgwrapper-0.3.5/pgwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 richard    (501) staff       (20)       16 2023-05-25 14:30:37.000000 pgwrapper-0.3.5/pgwrapper.egg-info/requires.txt
+-rw-r--r--   0 richard    (501) staff       (20)       10 2023-05-25 14:30:37.000000 pgwrapper-0.3.5/pgwrapper.egg-info/top_level.txt
+-rw-r--r--   0 richard    (501) staff       (20)       38 2023-05-25 14:30:37.410542 pgwrapper-0.3.5/setup.cfg
+-rw-r--r--   0 richard    (501) staff       (20)     1117 2023-05-25 14:28:43.000000 pgwrapper-0.3.5/setup.py
```

### Comparing `pgwrapper-0.3.1/LICENSE` & `pgwrapper-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgwrapper-0.3.1/PKG-INFO` & `pgwrapper-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pgwrapper
-Version: 0.3.1
+Version: 0.3.5
 Summary: A simple, fast way to access postgresql
 Home-page: https://github.com/LaoLiulaoliu/pgwrapper
 Author: Richard Liu
 Author-email: miraclecome@gmail.com
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
@@ -31,14 +31,27 @@
 
 ### Install
 pip install pgwrapper
 
 
 ### Usage
 
+```
+>>> import pgwrapper
+>>> pg = pgwrapper.PGWrapper(
+        dbname='postgres',
+        user='postgres',
+        password='',
+        host='127.0.0.1',
+        port=5432)
+>>> r = pg.select('company', 'id, name', 'address is not null', 'limit 2')
+>>> print(r)
+
+[(12, 'sun'), (34, 'moon')]
+```
 
 ###### select
 ```
     >>> select('hospital', 'id, city', control='limit 1')
     select id, city from hospital limit 1;
```

### Comparing `pgwrapper-0.3.1/README.md` & `pgwrapper-0.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,27 @@
 
 ### Install
 pip install pgwrapper
 
 
 ### Usage
 
+```
+>>> import pgwrapper
+>>> pg = pgwrapper.PGWrapper(
+        dbname='postgres',
+        user='postgres',
+        password='',
+        host='127.0.0.1',
+        port=5432)
+>>> r = pg.select('company', 'id, name', 'address is not null', 'limit 2')
+>>> print(r)
+
+[(12, 'sun'), (34, 'moon')]
+```
 
 ###### select
 ```
     >>> select('hospital', 'id, city', control='limit 1')
     select id, city from hospital limit 1;
```

### Comparing `pgwrapper-0.3.1/pgwrapper/pgpool.py` & `pgwrapper-0.3.5/pgwrapper/pgpool.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,73 +67,76 @@
                               user=self.user, password=self.password,
                               host=self.host, port=self.port)
         if 'psycopg2.extras' in sys.modules:
             psycopg2.extras.register_hstore(db)
         return db
 
     @contextmanager
-    def connection(self):
+    def connection(self, dryrun=False):
         yielded = False
         retry = 0
         while yielded is False and retry < self.maxretries:
             try:
                 conn = self.get()
                 cur = conn.cursor()
                 yield cur
             except Exception as e:
                 conn = None
                 retry += 1
                 print(e)
             else:
                 yielded = True
                 retry = 0
-                conn.commit()  # commit `insert`, `update` and `delete`
+                if not dryrun:
+                    conn.commit()  # commit `insert`, `update` and `delete`
             finally:
-                if conn is not None:
+                if cur:
                     cur.close()
+                if conn:
                     self.put(conn)
 
         if yielded is False:
             raise Exception('Could not obtain cursor, max retry {} reached.'.format(retry))
 
-    def execute(self, query, vars=None, result=False):
+    def execute(self, query, vars=None, result=False, dryrun=False):
         """.. :py:method::
 
         :param bool result: whether query return result
-        :rtype: bool
+        :param bool dryrun: whether just return sql
+        :rtype: sql str for dryrun, QueryResult for result
 
         .. note::
             True for `select`, False for `insert` and `update`
         """
-        with self.connection() as cur:
-            if self.debug:
-                print(cur.mogrify(query, vars))
+        with self.connection(dryrun) as cur:
+            if dryrun:
+                return cur.mogrify(query, vars)
 
             resp = cur.execute(query, vars)
 
             if result == False:
                 return resp
 
             else:
                 columns = [i[0] for i in cur.description]
                 results = cur.fetchall()
                 return QueryResult(columns, results)
 
-    def execute_generator(self, query, vars=None, result=False):
+    def execute_generator(self, query, vars=None, result=False, dryrun=False):
         """.. :py:method::
 
         :param bool result: whether query return result
         :rtype: bool
 
         .. note::
             True for `select`, False for `insert` and `update`
         """
-        with self.connection() as cur:
-            if self.debug:
-                print(cur.mogrify(query, vars))
+        with self.connection(dryrun) as cur:
+            if dryrun:
+                return cur.mogrify(query, vars)
 
             resp = cur.execute(query, vars)
 
             if result == True:
                 columns = [i[0] for i in cur.description]
                 results = cur.fetchmany(1000)
                 while results:
@@ -160,8 +163,7 @@
         with self.connection() as cur:
             for sql in sqls:
 
                 if isinstance(sql, tuple):
                     cur.execute(sql[0], sql[1])
                 else:
                     cur.execute(sql)
-
```

### Comparing `pgwrapper-0.3.1/pgwrapper/pgwrap.py` & `pgwrapper-0.3.5/pgwrapper/pgwrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,21 +31,20 @@
             select id, city from hospital limit 1;
 
 
             >>> select('hospital', 'id', 'address is null')
             select id from hospital where address is null;
 
         """
-        sql = 'select {} from {}'.format(args, table)
-        sql += self.parse_condition(condition) + (' {};'.format(control) if control else ';')
+        sql = f'select {args} from {table}'
+        sql += self.parse_condition(condition) + (f' {control};' if control else ';')
         if dryrun:
             return sql
         return super(PGWrapper, self).execute(sql, result=True).results
 
-
     def update(self, table, kwargs, condition=None, dryrun=False):
         """.. :py:method:: update
 
             All module update can user this function.
             condition only support string and dictionary.
 
         Usage::
@@ -56,60 +55,57 @@
             >>> update('dept', {'name': 'design', 'quantity': 3}, 'introduction is null')
             update dept set name='design', quantity=3 where introduction is null;
 
             >>> update('physician', {'$inc': {'status': -10}, 'present': 0}, {'id': 'someid'})
             update physician set status=status+-10, present=0 where id='someid';
 
         """
-        sql = "update {} set {}"
         equations = []
         values = []
         for k, v in kwargs.items():
             if k == '$inc' and isinstance(v, dict):
                 for ik, iv in v.items():
-                    equations.append("{field}={field}+{value}".format(field=ik, value=iv))
+                    equations.append(f'{ik}={ik}+{iv}')
             else:
-                equations.append("{}=%s".format(k))
+                equations.append(f'{k}=%s')
                 values.append(v)
 
-        sql = sql.format(table, ', '.join(equations))
-        sql += self.parse_condition(condition) + ";"
+        sql = (f"update {table} set {', '.join(equations)}"
+               f"{self.parse_condition(condition)};")
         if dryrun:
             return sql, values
         super(PGWrapper, self).execute(sql, values, result=False)
 
-
     def insert(self, table, kwargs, returning=False, dryrun=False):
         """.. :py:method::
 
         Usage::
 
             >>> insert('hospital', {'id': '12de3wrv', 'province': 'shanghai'})
             insert into hospital (id, province) values ('12de3wrv', 'shanghai');
 
         :param string table: table name
         :param dict kwargs: name and value
         :param bool dryrun: if dryrun, return sql and variables
         :rtype: tuple
 
         """
-        sql = "insert into " + table + " ({}) values ({});"
         keys, values = [], []
         [(keys.append(k), values.append(v)) for k, v in kwargs.items()]
-        sql = sql.format(', '.join(keys), ', '.join(['%s'] * len(values)))
+        sql = (f"insert into {table} ({', '.join(keys)}) values "
+               f"({', '.join(['%s'] * len(values))});")
         sql = sql[:-1] + ' returning *;' if returning else sql
         if dryrun:
             return sql, values
 
         if returning:
             return super(PGWrapper, self).execute(sql, values, result=True)
         else:
             super(PGWrapper, self).execute(sql, values, result=False)
 
-
     def insert_list(self, table, names, values, returning=False, dryrun=False):
         """.. :py:method::
 
         Usage::
 
             >>> insert_list('hospital', ['id', 'province'], ['12de3wrv', 'shanghai'])
             insert into hospital (id, province) values ('12de3wrv', 'shanghai');
@@ -117,86 +113,81 @@
         :param string table: table name
         :param list names: name
         :param list values: value
         :param bool dryrun: if dryrun, return sql and variables
         :rtype: tuple
 
         """
-        sql = "insert into " + table + " ({}) values ({});"
-        sql = sql.format(', '.join(names), ', '.join(['%s'] * len(values)))
+        sql = (f"insert into {table} ({', '.join(names)}) values "
+               f"({', '.join(['%s'] * len(values))});")
         sql = sql[:-1] + ' returning *;' if returning else sql
         if dryrun:
             return sql, values
 
         if returning:
             return super(PGWrapper, self).execute(sql, values, result=True)
         else:
             super(PGWrapper, self).execute(sql, values, result=False)
 
-
     def delete(self, table, condition, dryrun=False):
         """.. :py:method::
 
         Usage::
 
             >>> delete('hospital', {'id': '12de3wrv'})
             delete from hospital where id='12de3wrv';
 
         """
-        sql = "delete from {}".format(table)
-        sql += self.parse_condition(condition) + ";"
+        sql = f'delete from {table}{self.parse_condition(condition)};'
         if dryrun:
             return sql
         super(PGWrapper, self).execute(sql, result=False)
 
-
     def insert_inexistence(self, table, kwargs, condition, returning=False, dryrun=False):
         """.. :py:method::
 
         Usage::
 
             >>> insert_inexistence('hospital', {'id': '12de3wrv', 'province': 'shanghai'}, {'id': '12de3wrv'})
             insert into hospital (id, province) select '12de3wrv', 'shanghai' where not exists (select 1 from hospital where id='12de3wrv' limit 1);
 
         """
-        sql = "insert into " + table + " ({}) "
-        select = "select {} "
-        condition = "where not exists (select 1 from " + table + "{} limit 1);".format(self.parse_condition(condition))
         keys, values = [], []
         [(keys.append(k), values.append(v)) for k, v in kwargs.items()]
-        sql = sql.format(', '.join(keys)) + select.format(', '.join(['%s'] * len(values))) + condition
+        sql = (f"insert into {table} ({', '.join(keys)}) "
+               f"select {', '.join(['%s'] * len(values))} "
+               f"where not exists (select 1 from {table}"
+               f"{self.parse_condition(condition)} limit 1);")
         sql = sql[:-1] + ' returning *;' if returning else sql
 
         if dryrun:
             return sql, values
 
         if returning:
             return super(PGWrapper, self).execute(sql, values, result=True)
         else:
             super(PGWrapper, self).execute(sql, values, result=False)
 
-
     def parse_condition(self, condition):
         """.. :py:method::
 
             parse the condition, support string and dictonary
         """
         if isinstance(condition, str):
-            sql = " where {}".format(condition)
+            sql = f' where {condition}'
         elif isinstance(condition, dict):
             conditions = []
             for k, v in condition.items():
-                s = "{}='{}'".format(k, v) if isinstance(v, str) else "{}={}".format(k, v)
+                s = f"{k}='{v}'" if isinstance(v, str) else f'{k}={v}'
                 conditions.append(s)
-            sql = " where {}".format(' and '.join(conditions))
+            sql = f" where {' and '.join(conditions)}"
         else:
-            sql = ""
+            sql = ''
         return sql
 
-
     def select_join(self, table, field, join_table, join_field, dryrun=False):
         """.. :py:method::
 
         Usage::
 
             >>> select_join('hospital', 'id', 'department', 'hospid')
             select hospital.id from hospital left join department on hospital.id=department.hospid where department.hospid is null;
@@ -209,24 +200,23 @@
                                                                 join_table=join_table,
                                                                 join_field=join_field)
         if dryrun:
             return sql
 
         return super(PGWrapper, self).execute(sql, result=True).results
 
-
     def joint(self,
-            table,
-            fields,
-            join_table,
-            join_fields,
-            condition_field,
-            condition_join_field,
-            join_method='left_join',
-            dryrun=False):
+              table,
+              fields,
+              join_table,
+              join_fields,
+              condition_field,
+              condition_join_field,
+              join_method='left_join',
+              dryrun=False):
         """.. :py:method::
 
         Usage::
 
             >>> joint('user', 'name, id_number', 'medical_card', 'number', 'id', 'user_id', 'inner_join')
             select u.name, u.id_number, v.number from user as u inner join medical_card as v on u.id=v.user_id;
```

### Comparing `pgwrapper-0.3.1/pgwrapper.egg-info/PKG-INFO` & `pgwrapper-0.3.5/pgwrapper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pgwrapper
-Version: 0.3.1
+Version: 0.3.5
 Summary: A simple, fast way to access postgresql
 Home-page: https://github.com/LaoLiulaoliu/pgwrapper
 Author: Richard Liu
 Author-email: miraclecome@gmail.com
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
@@ -31,14 +31,27 @@
 
 ### Install
 pip install pgwrapper
 
 
 ### Usage
 
+```
+>>> import pgwrapper
+>>> pg = pgwrapper.PGWrapper(
+        dbname='postgres',
+        user='postgres',
+        password='',
+        host='127.0.0.1',
+        port=5432)
+>>> r = pg.select('company', 'id, name', 'address is not null', 'limit 2')
+>>> print(r)
+
+[(12, 'sun'), (34, 'moon')]
+```
 
 ###### select
 ```
     >>> select('hospital', 'id, city', control='limit 1')
     select id, city from hospital limit 1;
```

### Comparing `pgwrapper-0.3.1/setup.py` & `pgwrapper-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'pgwrapper',
-    version = '0.3.1',
+    version = '0.3.5',
     packages = ['pgwrapper'],
     author = 'Richard Liu',
     author_email = 'miraclecome@gmail.com',
     url = 'https://github.com/LaoLiulaoliu/pgwrapper',
-    install_requires=[ 'psycopg2 >= 2.8.5', ],
+    install_requires=[ 'psycopg2 >= 2.9.6', ],
     description = 'A simple, fast way to access postgresql',
     classifiers = [
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
         "Development Status :: 4 - Beta",
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         ],
```

