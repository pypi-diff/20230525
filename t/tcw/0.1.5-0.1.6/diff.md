# Comparing `tmp/tcw-0.1.5.tar.gz` & `tmp/tcw-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcw-0.1.5.tar", last modified: Thu May  4 17:56:08 2023, max compression
+gzip compressed data, was "tcw-0.1.6.tar", last modified: Thu May 25 15:40:07 2023, max compression
```

## Comparing `tcw-0.1.5.tar` & `tcw-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.679538 tcw-0.1.5/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.5/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-04 17:56:08.679538 tcw-0.1.5/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.5/README.md
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-05-04 17:56:08.679538 tcw-0.1.5/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      596 2023-05-04 17:55:48.000000 tcw-0.1.5/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.671538 tcw-0.1.5/tcw/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.5/tcw/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.675538 tcw-0.1.5/tcw/apps/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.675538 tcw-0.1.5/tcw/apps/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.1.5/tcw/apps/contest/forms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3534 2023-01-01 20:54:30.000000 tcw-0.1.5/tcw/apps/contest/models.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.675538 tcw-0.1.5/tcw/apps/contest/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/templates/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.679538 tcw-0.1.5/tcw/apps/contest/templates/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1547 2023-04-04 23:59:46.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/about.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5820 2023-04-13 13:07:38.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/animation.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2078 2023-04-05 05:32:34.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/form.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      303 2023-04-06 18:51:38.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/index.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2222 2023-04-07 12:49:55.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/privacy.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2304 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/signup.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1735 2023-04-13 13:03:09.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/slide1.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      562 2023-04-13 13:03:16.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/slide2.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      219 2023-04-13 13:03:04.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/slide3.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/sorry.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2569 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/success.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      408 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/apps/contest/templates/contest/thanks.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3313 2023-01-21 12:31:08.000000 tcw-0.1.5/tcw/apps/contest/views.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.1.5/tcw/config.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-04-14 11:51:00.000000 tcw-0.1.5/tcw/run.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.679538 tcw-0.1.5/tcw/static/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/static/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.679538 tcw-0.1.5/tcw/static/images/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/static/images/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.679538 tcw-0.1.5/tcw/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1971 2023-04-04 18:51:43.000000 tcw-0.1.5/tcw/templates/404.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1960 2023-04-05 14:13:22.000000 tcw-0.1.5/tcw/templates/410.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.5/tcw/templates/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2476 2023-05-04 17:55:39.000000 tcw-0.1.5/tcw/templates/base.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.1.5/tcw/utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      186 2023-04-14 11:50:36.000000 tcw-0.1.5/tcw/wsgi.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 17:56:08.675538 tcw-0.1.5/tcw.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-04 17:56:08.000000 tcw-0.1.5/tcw.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1170 2023-05-04 17:56:08.000000 tcw-0.1.5/tcw.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-05-04 17:56:08.000000 tcw-0.1.5/tcw.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-05-04 17:56:08.000000 tcw-0.1.5/tcw.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-05-04 17:56:08.000000 tcw-0.1.5/tcw.egg-info/top_level.txt
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.290183 tcw-0.1.6/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.6/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-25 15:40:07.290183 tcw-0.1.6/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.6/README.md
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-05-25 15:40:07.290183 tcw-0.1.6/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      596 2023-05-25 14:54:23.000000 tcw-0.1.6/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.282183 tcw-0.1.6/tcw/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.6/tcw/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.286183 tcw-0.1.6/tcw/apps/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.286183 tcw-0.1.6/tcw/apps/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1208 2023-05-25 14:21:10.000000 tcw-0.1.6/tcw/apps/contest/forms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3853 2023-05-25 15:11:54.000000 tcw-0.1.6/tcw/apps/contest/models.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.286183 tcw-0.1.6/tcw/apps/contest/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/contest/templates/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.290183 tcw-0.1.6/tcw/apps/contest/templates/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1547 2023-04-04 23:59:46.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/about.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5820 2023-04-13 13:07:38.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/animation.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2078 2023-04-05 05:32:34.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/form.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      303 2023-04-06 18:51:38.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/index.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2222 2023-04-07 12:49:55.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/privacy.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2302 2023-05-12 04:16:15.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/signup.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1735 2023-04-13 13:03:09.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/slide1.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      562 2023-04-13 13:03:16.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/slide2.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      219 2023-04-13 13:03:04.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/slide3.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/sorry.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2569 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/success.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      408 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/apps/contest/templates/contest/thanks.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3533 2023-05-25 14:59:11.000000 tcw-0.1.6/tcw/apps/contest/views.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1245 2023-05-25 14:53:59.000000 tcw-0.1.6/tcw/config.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1065 2023-05-25 14:47:10.000000 tcw-0.1.6/tcw/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-05-25 14:48:34.000000 tcw-0.1.6/tcw/exc.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      159 2023-05-25 14:57:02.000000 tcw-0.1.6/tcw/run.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.290183 tcw-0.1.6/tcw/static/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/static/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.290183 tcw-0.1.6/tcw/static/images/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/static/images/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.290183 tcw-0.1.6/tcw/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1971 2023-04-04 18:51:43.000000 tcw-0.1.6/tcw/templates/404.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1960 2023-04-05 14:13:22.000000 tcw-0.1.6/tcw/templates/410.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.6/tcw/templates/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2476 2023-05-04 17:55:39.000000 tcw-0.1.6/tcw/templates/base.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1606 2023-05-25 14:39:49.000000 tcw-0.1.6/tcw/utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-05-25 14:27:27.000000 tcw-0.1.6/tcw/wsgi.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-25 15:40:07.286183 tcw-0.1.6/tcw.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-25 15:40:07.000000 tcw-0.1.6/tcw.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-05-25 15:40:07.000000 tcw-0.1.6/tcw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-05-25 15:40:07.000000 tcw-0.1.6/tcw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-05-25 15:40:07.000000 tcw-0.1.6/tcw.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-05-25 15:40:07.000000 tcw-0.1.6/tcw.egg-info/top_level.txt
```

### Comparing `tcw-0.1.5/LICENSE` & `tcw-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/PKG-INFO` & `tcw-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.5
+Version: 0.1.6
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.5/README.md` & `tcw-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/setup.py` & `tcw-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tcw',
-    version='0.1.5',
+    version='0.1.6',
     author='J Leary',
     author_email='tinycontestwinners@gmail.com',
     description='tiny contest winners application',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(),
```

### Comparing `tcw-0.1.5/tcw/__init__.py` & `tcw-0.1.6/tcw/__init__.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/forms.py` & `tcw-0.1.6/tcw/apps/contest/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import datetime
 from flask_wtf import FlaskForm, RecaptchaField
-from wtforms import (StringField, IntegerField, HiddenField, TextAreaField,
-    DateTimeField, SubmitField, SelectField)
+from wtforms import (StringField, IntegerField, TextAreaField, SubmitField,
+    SelectField)
 from wtforms.validators import DataRequired
 from wtforms.fields import EmailField
 
 
 class ContestForm(FlaskForm):
+    """
+    Form definition class for new contest    
+    """
+
     title = StringField('contest title', validators=[DataRequired()],)
     instructions = TextAreaField('sign-up instructions', validators=[DataRequired()])
     email = EmailField('contest owner email', validators=[DataRequired()])
     winners = IntegerField('number of winners (1-50)', validators=[DataRequired()])
     maximum = IntegerField('max number of entrants (1-500)', validators=[DataRequired()])
     hours = SelectField('contest expires after', choices=[
         ('1', '1 hour'),
@@ -21,9 +24,13 @@
         ('120', '5 days'),
         ],  validators=[DataRequired()])
     recaptcha = RecaptchaField()
     submit = SubmitField('submit')
 
 
 class SignupForm(FlaskForm):
+    """
+    Form definition for user signup form
+    """
+
     name = StringField('sign up!')
     submit = SubmitField('submit')
```

### Comparing `tcw-0.1.5/tcw/apps/contest/models.py` & `tcw-0.1.6/tcw/apps/contest/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,59 +7,73 @@
     Boolean, ForeignKey, func)
 from sqlalchemy.orm import relationship
 from sqlalchemy.schema import UniqueConstraint
 from tcw.database import Base
 
 
 class JSONEncodedDict(TypeDecorator):
+    """
+    Store json text as a varchar
+    """
+
     impl = VARCHAR
 
     def process_bind_param(self, value, dialect):
         if value is not None:
             value = json.dumps(value)
         return value
 
     def process_result_variable(self, value, dialect):
         if value is not None:
             value = json.dumps(value)
         return value
 
 
 class MutableDict(Mutable, dict):
+    """
+    Convert plain dictionaries to MutableDict
+    """
+
     @classmethod
     def coerce(cls, key, value):
-        "Convert plain dictionaries to MutableDict."
+        """
+        Coerce to dict
+        """
 
         if not isinstance(value, MutableDict):
             if isinstance(value, dict):
                 return MutableDict(value)
 
             return Mutable.coerce(key, value)
         else:
             return value
 
     def __setitem__(self, key, value):
-        "Detect dictionary set events and emit change events."
+        """
+        Detect dictionary set events and emit change events.
+        """
 
         dict.__setitem__(self, key, value)
         self.changed()
 
     def __delitem__(self, key):
-        "Detect dictionary del events and emit change events."
+        """
+        Detect dictionary del events and emit change events.
+        """
 
         dict.__delitem__(self, key)
         self.changed()
 
 
 class Contest(Base):
-    '''
+    """
     NOTE: Do not use the attributes field for ANYTHING.
     If you do, it will break the sqlalchemy subqueries that check for
     expired contests, and tcw-tasks will break.
-    '''
+    """
 
     __tablename__ = 'contests'
 
     id = Column(Integer, primary_key=True)
     name = Column(Unicode(48), nullable=False, unique=True)
     title = Column(Unicode(128), nullable=False)
     instructions = Column(UnicodeText, nullable=True)
@@ -88,34 +102,43 @@
         if len(self.entrants) == 0:
             return []
 
         if len(self.entrants) < self.winners:
             nwinners = len(self.entrants)
 
         choices = [e.name for e in self.entrants]
-        while len(results) < self.winners:
+        while len(results) < nwinners:
             name = secrets.choice(choices)
             if name not in results:
                 results.append(name)
 
         return results
 
 
 class Entrant(Base):
+    """
+    Entrant class definition
+    """
+
     __tablename__ = 'entrants'
 
     id = Column(Integer, primary_key=True)
     name = Column(Unicode, nullable=False, unique=False)
     contest_id = Column(Integer, ForeignKey('contests.id'))
 
     # ensure only one name sign-up per contest.
     __table_args__ = (
         UniqueConstraint('name', 'contest_id', name='_name_id_uc'),)
 
 
 class Fossil(Base):
+    """
+    Fossil class definition. This is used only to keep a bare bones crumb
+    of info about expired contests
+    """
+
     __tablename__ = 'fossils'
 
     id = Column(Integer, primary_key=True)
     name = Column(Unicode(48), nullable=False, unique=True)
     expired = Column(DateTime, nullable=False, default=func.now())
     attributes = Column(MutableDict.as_mutable(JSONEncodedDict), nullable=True)
```

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/about.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/about.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/animation.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/animation.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/form.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/form.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/privacy.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/privacy.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/signup.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/signup.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             const e = document.getElementById('expires');
             const d = new Date(e.innerText);
             e.innerText = d.toDateString() + " " + d.toLocaleTimeString();
         }
     </script>
     <h4 class="text-center mb-4">Raffle Sign Up!</h4>
     <div class="card">
-        <div class="card-header text-center bg-warning">
+        <div class="card-header text-center bg-light">
             <h6>{{ contest.title }}</h6>
             <div class="small">
                 contest expires <span id="expires">{{ contest.expires.isoformat() + "Z" }}</span>
             </div>
         </div>
         <div class="card-body">
             <p class="text-center">{{ contest.instructions | markdown | safe }}</p>
```

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/slide1.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/slide1.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/slide2.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/slide2.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/templates/contest/success.html` & `tcw-0.1.6/tcw/apps/contest/templates/contest/success.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/apps/contest/views.py` & `tcw-0.1.6/tcw/apps/contest/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,56 @@
-import datetime
 import logging
 from flask import (Blueprint, render_template, redirect, request, abort,
-    url_for, Response)
+    url_for)
 from sqlalchemy.exc import IntegrityError
 from tcw.database import session
 from tcw.utils import (contest_by_name, fossil_by_name, random_name,
     expires_time)
+from tcw.exc import ContestNotFound, FossilNotFound
 from .forms import ContestForm, SignupForm
 from .models import Contest, Entrant
 
 
 logger = logging.getLogger(__name__)
 bp = Blueprint('contest', __name__, template_folder='templates')
 
 
 @bp.route('/', methods=['GET'])
 def index():
+    """
+    Main page
+    """
+
     return render_template('contest/index.html')
 
 
 @bp.route('/about', methods=['GET'])
 def about():
+    """
+    About page
+    """
+
     return render_template('contest/about.html')
 
 
 @bp.route('/privacy', methods=['GET'])
 def privacy():
+    """
+    Privacy document
+    """
+
     return render_template('contest/privacy.html')
 
 
 @bp.route('/contest', methods=['GET', 'POST'])
 def new():
+    """
+    Create a new contest
+    """
+
     form = ContestForm()
     if form.validate_on_submit():
         unique = random_name()
         options = {
             'name': unique,
             'title': form.title.data,
             'instructions': form.instructions.data,
@@ -45,39 +61,40 @@
         }
 
         try:
             obj = Contest(**options)
             session.add(obj)
             session.commit()
             options['expires'] = options['expires'].isoformat() + "Z"
-        except Exception as x:
-            logger.warning(x)
+        except:
             abort(404)
 
         return redirect(url_for('contest.success', **options))
 
     return render_template('contest/form.html', form=form)
 
 
 @bp.route('/signup', methods=['GET', 'POST'])
 def signup():
-    form = SignupForm()
+    """
+    User signup for existing contest
+    """
 
+    form = SignupForm()
     try:
         name = request.args.get('name')
-    except Exception as x:
-        logger.warning(x)
+    except:
         abort(404)
 
     try:
         contest = contest_by_name(name)
-    except:
+    except ContestNotFound:
         try:
             fossil = fossil_by_name(name)
-        except:
+        except FossilNotFound:
             abort(404)
         abort(410)
 
     if form.validate_on_submit():
         if len(contest.entrants) >= contest.max_entrants:
             return render_template('contest/signup.html',
                 data=contest, form=form)
@@ -93,26 +110,33 @@
                 url_for('contest.thanks',
                     contest=contest.title,
                     entrant=form.name.data), code=303)
         except IntegrityError:
             session.rollback()
             return render_template('contest/sorry.html',
                 contest=contest, form=form)
-        except Exception as x:
-            logg
+        except:
             abort(404)
-    else:
-        return render_template('contest/signup.html',
-            contest=contest, form=form)
+
+    return render_template('contest/signup.html',
+        contest=contest, form=form)
 
 
 @bp.route('/success', methods=['GET'])
 def success():
+    """
+    Contest was successfully created
+    """
+
     return render_template('contest/success.html', data=request.args)
 
 
 @bp.route('/thanks', methods=['GET'])
 def thanks():
+    """
+    Thanks for signing up!    
+    """
+
     contest = request.args.get('contest')
     entrant = request.args.get('entrant')
     return render_template('contest/thanks.html',
         contest=contest, name=entrant)
```

### Comparing `tcw-0.1.5/tcw/config.py` & `tcw-0.1.6/tcw/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 import os
 
 class BaseConfig:
+    """
+    Parent class
+    """
+
     ## flask options ##
     PROJECT = 'tiny contest winners'
     DEBUG = False
     TESTING = False
     PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
     SECRET_KEY = os.getenv('FLASK_SECRET', 'TerribleLifeChoices')
     WFT_SECRET_KEY = os.getenv('FLASK_SECRET', 'TerribleLifeChoices')
     WTF_CSRF_ENABLED = True
     CSRF_ENABLED = True
 
     ## database options ##
     SQLALCHEMY_DATABASE_URI = os.getenv('SQLALCHEMY_DATABASE_URI', 'sqlite:////tmp/test.db')
-    SQLALCHEMY_ECHO = os.getenv('SQLALCHEMY_ECHO', False)
+    SQLALCHEMY_ECHO = False
     SQLALCHEMY_TRACK_MODIFICATIONS = False
 
     ## recaptcha options ##
-    RECAPTCHA_USE_SSL = os.getenv('RECAPTCHA_USE_SSL', True)
+    RECAPTCHA_USE_SSL = True
     RECAPTCHA_PUBLIC_KEY = os.getenv('RECAPTCHA_PUBLIC_KEY', None)
     RECAPTCHA_PRIVATE_KEY = os.getenv('RECAPTCHA_PRIVATE_KEY', None)
-    RECAPTCHA_OPTIONS = os.getenv('RECAPTCHA_OPTIONS', {'theme': 'white'})
+    RECAPTCHA_OPTIONS = {'theme': 'white'}
 
 
 class Development(BaseConfig):
+    """
+    For development environment only
+    """
+
     DEBUG = True
     TESTING = True
     CSRF_ENABLED = False
     WTF_CSRF_ENABLED = False
     SQLALCHEMY_ECHO = True
     SQLALCHEMY_TRACK_MODIFICATIONS = True
 
 
 class Production(BaseConfig):
+    """
+    For production environment only
+    """
+
     # SERVER_NAME = os.getenv('FLASK_SERVER_NAME', 'localhost')
     pass
```

### Comparing `tcw-0.1.5/tcw/database.py` & `tcw-0.1.6/tcw/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from sqlalchemy import create_engine
-from sqlalchemy.orm import scoped_session, sessionmaker, create_session
+from sqlalchemy.orm import scoped_session, create_session
 from sqlalchemy.ext.declarative import declarative_base
+from tcw.apps.contest.models import Contest, Fossil, Entrant
+
 
 # globals #
 engine = None
 session = scoped_session(lambda: create_session( bind=engine,
                                                     autocommit=False,
                                                     autoflush=False ))
 
@@ -21,15 +23,15 @@
         - sqlalchemy echo?
     """
 
     init_engine(uri, echo=echo)
     init_tables()
 
 
-def init_engine(uri, *args, **kwargs):
+def init_engine(uri, **kwargs):
     """
     initialize the global engine for sessions.
 
     args:
         - db uri
         - keyword args (see sqlalchemy create_engine() docs)
     """
@@ -39,9 +41,8 @@
 
 
 def init_tables():
     """
     Initialize database tables for app models.
     """
 
-    from tcw.apps.contest.models import Contest, Entrant
     Base.metadata.create_all(bind=engine)
```

### Comparing `tcw-0.1.5/tcw/templates/404.html` & `tcw-0.1.6/tcw/templates/404.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/templates/410.html` & `tcw-0.1.6/tcw/templates/410.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/templates/base.html` & `tcw-0.1.6/tcw/templates/base.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.5/tcw/utils.py` & `tcw-0.1.6/tcw/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import string
 import secrets
 import datetime
 import markdown
+from tcw.apps.contest.models import Contest, Fossil
 from .database import session
-from tcw.apps.contest.models import Contest, Entrant, Fossil
+from .exc import ContestNotFound, FossilNotFound
 
 
 def contest_by_name(name):
+    """
+    Get contest object by name
+    """
+
     contest = session.query(Contest).filter(Contest.name == name).one()
     if not contest:
-        raise Exception("No contest with name %s" % name)
+        raise ContestNotFound(f"No contest with name {name}")
 
     return contest
 
 
 def fossil_by_name(name):
+    """
+    Get fossil object by name
+    """
+
     fossil = session.query(Fossil).filter(Fossil.name == name).one()
     if not fossil:
-        raise Exception("No fossil with name %s" % name)
+        raise FossilNotFound(f"No fossil with name {name}")
 
     return fossil
 
 
 def random_name(length=24):
     """
     create random name for contests. a mix of alphanum chars.
@@ -50,32 +59,24 @@
     args:
         - float hours into the future
     returns:
         - datateime object, None on  error
     """
 
     now = datetime.datetime.utcnow().replace(second=0, microsecond=0)
-    later = None
-
-    try:
-        later = now + datetime.timedelta(hours=hours)
-    except:
-        pass
+    later = now + datetime.timedelta(hours=hours)
 
     return later
 
 
 def md_to_html(txt):
     """
     Convert markdown text to HTML.
 
     args:
         - str (markdown text)
     returns:
         str (html text)
     """
 
-    try:
-        html = markdown.markdown(txt)
-        return html
-    except:
-        return txt
+    html = markdown.markdown(txt)
+    return html
```

### Comparing `tcw-0.1.5/tcw.egg-info/PKG-INFO` & `tcw-0.1.6/tcw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.5
+Version: 0.1.6
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.5/tcw.egg-info/SOURCES.txt` & `tcw-0.1.6/tcw.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 tcw/__init__.py
 tcw/config.py
 tcw/database.py
+tcw/exc.py
 tcw/run.py
 tcw/utils.py
 tcw/wsgi.py
 tcw.egg-info/PKG-INFO
 tcw.egg-info/SOURCES.txt
 tcw.egg-info/dependency_links.txt
 tcw.egg-info/requires.txt
```

