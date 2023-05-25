# Comparing `tmp/ifd_python-10.1.5.tar.gz` & `tmp/ifd_python-10.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-10.1.5.tar", max compression
+gzip compressed data, was "ifd_python-10.1.6.tar", max compression
```

## Comparing `ifd_python-10.1.5.tar` & `ifd_python-10.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1093 2023-05-16 13:28:13.433655 ifd_python-10.1.5/LICENSE
--rw-r--r--   0        0        0      551 2023-05-16 13:28:13.433655 ifd_python-10.1.5/README.md
--rw-r--r--   0        0        0      283 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      630 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/BodyTicket.py
--rw-r--r--   0        0        0      734 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Image.py
--rw-r--r--   0        0        0      730 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Intervention.py
--rw-r--r--   0        0        0     1428 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      741 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Malfacon.py
--rw-r--r--   0        0        0      477 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Modele.py
--rw-r--r--   0        0        0      794 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/OCR.py
--rw-r--r--   0        0        0      529 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0     1033 2023-05-17 09:32:12.521357 ifd_python-10.1.5/ifd/entities/Tag.py
--rw-r--r--   0        0        0      423 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/Ticket.py
--rw-r--r--   0        0        0      400 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2161 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0     2215 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/repository/RestTicketRepository.py
--rw-r--r--   0        0        0     1039 2023-05-17 15:23:08.904378 ifd_python-10.1.5/ifd/repository/SqlLogRepository.py
--rw-r--r--   0        0        0     1742 2023-05-24 16:30:58.812249 ifd_python-10.1.5/ifd/repository/SqlTicketRepository.py
--rw-r--r--   0        0        0      210 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/repository/__init__.py
--rw-r--r--   0        0        0      940 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/repository/abstract/AbsSqlRepository.py
--rw-r--r--   0        0        0       46 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/repository/abstract/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/spec.py
--rw-r--r--   0        0        0      526 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-05-16 13:28:13.433655 ifd_python-10.1.5/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 16:30:58.832249 ifd_python-10.1.5/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      407 2023-05-24 16:31:08.048218 ifd_python-10.1.5/pyproject.toml
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-16 13:28:13.433655 ifd_python-10.1.6/LICENSE
+-rw-r--r--   0        0        0      551 2023-05-16 13:28:13.433655 ifd_python-10.1.6/README.md
+-rw-r--r--   0        0        0      283 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/BodyTicket.py
+-rw-r--r--   0        0        0      734 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Image.py
+-rw-r--r--   0        0        0      730 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Intervention.py
+-rw-r--r--   0        0        0     1428 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      741 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Malfacon.py
+-rw-r--r--   0        0        0      477 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      794 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      529 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0     1033 2023-05-17 09:32:12.521357 ifd_python-10.1.6/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      449 2023-05-25 07:06:16.414795 ifd_python-10.1.6/ifd/entities/Ticket.py
+-rw-r--r--   0        0        0      400 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2161 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0     2215 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/repository/RestTicketRepository.py
+-rw-r--r--   0        0        0     1039 2023-05-17 15:23:08.904378 ifd_python-10.1.6/ifd/repository/SqlLogRepository.py
+-rw-r--r--   0        0        0     1742 2023-05-24 16:30:58.812249 ifd_python-10.1.6/ifd/repository/SqlTicketRepository.py
+-rw-r--r--   0        0        0      210 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/repository/abstract/AbsSqlRepository.py
+-rw-r--r--   0        0        0       46 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/repository/abstract/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/spec.py
+-rw-r--r--   0        0        0      831 2023-05-25 07:06:16.414795 ifd_python-10.1.6/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-05-16 13:28:13.433655 ifd_python-10.1.6/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 07:06:16.434795 ifd_python-10.1.6/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-25 07:06:25.842712 ifd_python-10.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.1.6/PKG-INFO
```

### Comparing `ifd_python-10.1.5/LICENSE` & `ifd_python-10.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/README.md` & `ifd_python-10.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Abstract/ADetection.py` & `ifd_python-10.1.6/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/BodyTicket.py` & `ifd_python-10.1.6/ifd/entities/BodyTicket.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Classification.py` & `ifd_python-10.1.6/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Detection.py` & `ifd_python-10.1.6/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Image.py` & `ifd_python-10.1.6/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Intervention.py` & `ifd_python-10.1.6/ifd/entities/Intervention.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/LogResult.py` & `ifd_python-10.1.6/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Malfacon.py` & `ifd_python-10.1.6/ifd/entities/Malfacon.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/OCR.py` & `ifd_python-10.1.6/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/RabbitMqMessage.py` & `ifd_python-10.1.6/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/Tag.py` & `ifd_python-10.1.6/ifd/entities/Tag.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/entities/bbox.py` & `ifd_python-10.1.6/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/repository/AmqpImageRepository.py` & `ifd_python-10.1.6/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/repository/RestTicketRepository.py` & `ifd_python-10.1.6/ifd/repository/RestTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/repository/SqlLogRepository.py` & `ifd_python-10.1.6/ifd/repository/SqlLogRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/repository/SqlTicketRepository.py` & `ifd_python-10.1.6/ifd/repository/SqlTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/repository/abstract/AbsSqlRepository.py` & `ifd_python-10.1.6/ifd/repository/abstract/AbsSqlRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/ifd/spec.py` & `ifd_python-10.1.6/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.5/PKG-INFO` & `ifd_python-10.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 10.1.5
+Version: 10.1.6
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

