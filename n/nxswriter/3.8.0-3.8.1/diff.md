# Comparing `tmp/nxswriter-3.8.0.tar.gz` & `tmp/nxswriter-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxswriter-3.8.0.tar", last modified: Wed Mar  8 09:00:50 2023, max compression
+gzip compressed data, was "dist/nxswriter-3.8.1.tar", last modified: Thu Mar  9 13:19:26 2023, max compression
```

## Comparing `nxswriter-3.8.0.tar` & `nxswriter-3.8.1.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian10_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3518 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian10_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian10_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3593 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian10_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian11_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3587 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian11_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian8_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2554 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian8_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian8_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2763 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian8_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian9_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3521 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian9_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/debian9_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3524 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/debian9_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) irc         (39)     3208 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/install.sh
--rw-r--r--   0 jkotan   (15949) irc         (39)      432 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/run.sh
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/ubuntu16.04_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2598 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/ubuntu16.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/ubuntu16.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2603 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/ubuntu16.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/ubuntu18.04_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3273 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/ubuntu18.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/ubuntu18.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3326 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/ubuntu18.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.ci/ubuntu20.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3737 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.ci/ubuntu20.04_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) irc         (39)      175 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.flake8
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.github/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/.github/workflows/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2022-11-22 20:26:35.000000 nxswriter-3.8.0/.github/workflows/tests.yml
--rw-r--r--   0 jkotan   (15949) irc         (39)       83 2018-09-14 10:01:58.000000 nxswriter-3.8.0/.gitignore
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-09-14 10:01:58.000000 nxswriter-3.8.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)    17273 2023-03-08 09:00:26.000000 nxswriter-3.8.0/ChangeLog
--rw-r--r--   0 jkotan   (15949) irc         (39)      114 2022-11-22 20:26:35.000000 nxswriter-3.8.0/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      918 2022-11-22 20:26:35.000000 nxswriter-3.8.0/NXSDataWriter
--rw-r--r--   0 jkotan   (15949) irc         (39)    18110 2023-03-02 11:49:55.000000 nxswriter-3.8.0/NXSDataWriter.xmi
--rw-r--r--   0 jkotan   (15949) irc         (39)    10763 2023-03-08 09:00:50.000000 nxswriter-3.8.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     7593 2022-11-22 20:26:35.000000 nxswriter-3.8.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/XMLExamples/
--rw-r--r--   0 jkotan   (15949) irc         (39)   104154 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/MNI.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      915 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/encodedImage.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      904 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/encodedImage4.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1593 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/scan.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1645 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/scan2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1594 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/scan3.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     7606 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/test.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     7539 2018-09-14 10:01:58.000000 nxswriter-3.8.0/XMLExamples/trigger.xml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/doc/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6774 2022-11-22 20:26:35.000000 nxswriter-3.8.0/doc/Makefile
--rw-r--r--   0 jkotan   (15949) irc         (39)    14053 2022-11-22 20:26:35.000000 nxswriter-3.8.0/doc/conf.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      448 2022-11-22 20:26:35.000000 nxswriter-3.8.0/doc/index.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     6707 2022-11-22 20:26:35.000000 nxswriter-3.8.0/doc/make.bat
--rw-r--r--   0 jkotan   (15949) irc         (39)     4318 2022-11-22 20:26:35.000000 nxswriter-3.8.0/doc/nxswriter.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/doc_html/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3757 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrCanFail.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3732 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrCurrentFileId.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3656 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrErrors.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3956 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrFileName.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3882 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrJSONRecord.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3839 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrSkipAcquisition.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3968 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrStepsPerFile.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3914 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/AttrXMLSettings.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3053 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/Attributes.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1861 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/ClassDescription.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1249 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdCloseEntry.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1288 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdCloseEntryAsynch.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1231 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdCloseFile.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1272 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdOpenEntry.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1311 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdOpenEntryAsynch.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1232 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdOpenFile.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1292 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdRecord.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1331 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdRecordAsynch.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1253 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdState.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1266 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/CmdStatus.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     2701 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/Commands.html
--rw-r--r--   0 jkotan   (15949) irc         (39)    51672 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/FullDocument.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1758 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/Properties.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1003 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/States.html
--rw-r--r--   0 jkotan   (15949) irc         (39)      903 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/TitleBanner.html
--rw-r--r--   0 jkotan   (15949) irc         (39)      979 2023-03-02 11:49:57.000000 nxswriter-3.8.0/doc_html/index.html
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      991 2022-11-22 20:26:35.000000 nxswriter-3.8.0/man/NXSDataWriter.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     2209 2023-02-28 13:19:57.000000 nxswriter-3.8.0/man/nxsfromxml.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    86849 2023-03-08 09:00:26.000000 nxswriter-3.8.0/man/nxswriter.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       74 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxsfromxml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3889 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/ClientSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9068 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/DBaseSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6156 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/DataHolder.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4683 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/DataSourceFactory.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4574 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/DataSourcePool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5295 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/DataSources.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15052 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/DecoderPool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8599 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/EAttribute.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    26261 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/EField.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/EGroup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8817 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/ELink.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4000 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/EStrategy.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3011 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/Element.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2099 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/ElementThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1660 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/Errors.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20455 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/FElement.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6821 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/FetchNameHandler.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6035 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/H5Elements.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4493 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/InnerXMLParser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3668 2022-12-12 12:16:40.000000 nxswriter-3.8.0/nxswriter/Metadata.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9077 2023-02-28 13:17:59.000000 nxswriter-3.8.0/nxswriter/NXSFromXML.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    31313 2023-03-02 11:51:13.000000 nxswriter-3.8.0/nxswriter/NXSWriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    13805 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/NexusXMLHandler.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11230 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/PyEvalSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-03-08 09:00:26.000000 nxswriter-3.8.0/nxswriter/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5473 2023-03-08 09:00:26.000000 nxswriter-3.8.0/nxswriter/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    27784 2023-03-08 09:00:26.000000 nxswriter-3.8.0/nxswriter/TangoDataWriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29400 2023-03-02 09:03:40.000000 nxswriter-3.8.0/nxswriter/TangoSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6031 2023-03-08 09:00:26.000000 nxswriter-3.8.0/nxswriter/ThreadPool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7676 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/Types.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1760 2022-11-22 20:26:35.000000 nxswriter-3.8.0/nxswriter/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)    10763 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     5577 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 20:30:29.000000 nxswriter-3.8.0/nxswriter.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       42 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       10 2023-03-08 09:00:50.000000 nxswriter-3.8.0/nxswriter.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      203 2023-03-08 09:00:50.000000 nxswriter-3.8.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4117 2022-11-22 20:26:35.000000 nxswriter-3.8.0/setup.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-08 09:00:50.000000 nxswriter-3.8.0/test/
--rw-r--r--   0 jkotan   (15949) irc         (39)    52501 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/Checkers.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5501 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ClientFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5490 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ClientFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4684 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ClientFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4771 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ClientFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   105723 2023-03-02 07:45:36.000000 nxswriter-3.8.0/test/ClientFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   105064 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ClientFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20281 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ClientSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5954 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/Converters_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5612 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5598 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4882 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    87899 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    87520 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16850 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DBaseSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    30489 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DataHolder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10182 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DataSourceDecoders_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15976 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DataSourceFactory_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10560 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DataSourcePool_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5859 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DataSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12848 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/DecoderPool_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   108465 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EAttributeH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   107896 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EAttributeH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    18366 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EDimH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    18395 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EDimH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7839 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EDimensionsH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7832 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EDimensionsH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6412 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EDocH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6409 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EDocH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   285119 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EFieldH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   285230 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EFieldH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   171438 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EFieldReshapeH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   170929 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EFieldReshapeH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5329 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EFileH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5321 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EFileH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    42448 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EGroupH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    42416 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EGroupH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    72155 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ELinkH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    71822 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ELinkH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11340 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EStrategyH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11349 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/EStrategyH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7030 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ESymbolH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7120 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ESymbolH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3208 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ElementH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3204 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ElementH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5386 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ElementThread_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3629 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/Element_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4471 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/Errors_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45152 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FElementH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45164 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FElementH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    34938 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FElementWithAttrH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35205 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FElementWithAttrH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22964 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FetchNameHandler_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   344148 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FileWriterH5CppH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   179717 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FileWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/FileWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   215225 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/H5CppWriter_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   178444 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/H5PYWriter_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15547 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/InnerXMLParser_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15418 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/MYSQLSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    46174 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/NTP_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   211886 2023-02-28 12:37:21.000000 nxswriter-3.8.0/test/NXSDataWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   211039 2023-02-28 12:37:21.000000 nxswriter-3.8.0/test/NXSDataWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    41359 2023-02-28 13:17:59.000000 nxswriter-3.8.0/test/NXSFromXMLH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    41371 2023-02-28 13:17:59.000000 nxswriter-3.8.0/test/NXSFromXMLH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   125101 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/NexusXMLHandlerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   125171 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/NexusXMLHandlerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    14694 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ORACLESource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    13061 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/PGSQLSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1652 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ProxyHelper.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5053 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ProxyTools_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    25478 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/PyEvalSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    54033 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/PyEvalTangoSourceH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    53808 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/PyEvalTangoSourceH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4886 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    52123 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/SimpleServer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5851 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/SimpleServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    21200 2023-03-08 09:00:26.000000 nxswriter-3.8.0/test/StreamSet_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7488 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TNObject_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      252 2018-09-14 10:01:58.000000 nxswriter-3.8.0/test/TangoClassID.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)    35756 2023-03-02 09:03:40.000000 nxswriter-3.8.0/test/TangoDataWriterH5CppH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   250238 2023-02-28 12:37:21.000000 nxswriter-3.8.0/test/TangoDataWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   250237 2023-02-28 12:37:21.000000 nxswriter-3.8.0/test/TangoDataWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5627 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TangoFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5618 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TangoFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4851 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TangoFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4841 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TangoFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   112661 2023-03-02 09:03:40.000000 nxswriter-3.8.0/test/TangoFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   112655 2023-03-02 09:03:40.000000 nxswriter-3.8.0/test/TangoFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   161008 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TangoSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11581 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TgDevice_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    33398 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TgGroup_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    27676 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TgMember_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10508 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/ThreadPool_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4264 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/TstDataSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8163 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/UINT32decoder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5434 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/UTF8decoder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9237 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/VDEOdecoder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5365 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/XMLFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5354 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/XMLFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4712 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/XMLFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4702 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/XMLFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35614 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/XMLFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35619 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/XMLFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      923 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      945 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/__main__.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    20511 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/main.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1458 2018-09-14 10:01:58.000000 nxswriter-3.8.0/test/mydb.pgsql
--rw-r--r--   0 jkotan   (15949) irc         (39)     1646 2022-11-22 20:26:35.000000 nxswriter-3.8.0/test/sttest.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian10_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3518 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian10_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian10_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3593 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian10_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian11_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3587 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian11_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian8_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2554 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian8_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian8_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2763 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian8_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian9_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3521 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian9_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/debian9_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3524 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/debian9_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3208 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/install.sh
+-rw-r--r--   0 jkotan   (15949) irc         (39)      432 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/run.sh
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/ubuntu16.04_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2598 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/ubuntu16.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/ubuntu16.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2603 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/ubuntu16.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/ubuntu18.04_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3273 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/ubuntu18.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/ubuntu18.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3326 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/ubuntu18.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.ci/ubuntu20.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3737 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.ci/ubuntu20.04_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)      175 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.flake8
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.github/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/.github/workflows/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2022-11-22 20:26:35.000000 nxswriter-3.8.1/.github/workflows/tests.yml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       83 2018-09-14 10:01:58.000000 nxswriter-3.8.1/.gitignore
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-09-14 10:01:58.000000 nxswriter-3.8.1/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)    17389 2023-03-09 13:11:43.000000 nxswriter-3.8.1/ChangeLog
+-rw-r--r--   0 jkotan   (15949) irc         (39)      114 2022-11-22 20:26:35.000000 nxswriter-3.8.1/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      918 2022-11-22 20:26:35.000000 nxswriter-3.8.1/NXSDataWriter
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18108 2023-03-08 10:18:04.000000 nxswriter-3.8.1/NXSDataWriter.xmi
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10763 2023-03-09 13:19:26.000000 nxswriter-3.8.1/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7593 2022-11-22 20:26:35.000000 nxswriter-3.8.1/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/XMLExamples/
+-rw-r--r--   0 jkotan   (15949) irc         (39)   104154 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/MNI.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      915 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/encodedImage.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      904 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/encodedImage4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1593 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/scan.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1645 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/scan2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1594 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/scan3.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7606 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/test.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7539 2018-09-14 10:01:58.000000 nxswriter-3.8.1/XMLExamples/trigger.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/doc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6774 2022-11-22 20:26:35.000000 nxswriter-3.8.1/doc/Makefile
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14053 2022-11-22 20:26:35.000000 nxswriter-3.8.1/doc/conf.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      448 2022-11-22 20:26:35.000000 nxswriter-3.8.1/doc/index.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6707 2022-11-22 20:26:35.000000 nxswriter-3.8.1/doc/make.bat
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4318 2022-11-22 20:26:35.000000 nxswriter-3.8.1/doc/nxswriter.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/doc_html/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3757 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrCanFail.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3732 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrCurrentFileId.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3656 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrErrors.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3956 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrFileName.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3882 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrJSONRecord.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3839 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrSkipAcquisition.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3968 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrStepsPerFile.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3914 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/AttrXMLSettings.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3053 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/Attributes.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1861 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/ClassDescription.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1249 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdCloseEntry.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1288 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdCloseEntryAsynch.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1231 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdCloseFile.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1272 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdOpenEntry.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1311 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdOpenEntryAsynch.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1232 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdOpenFile.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1292 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdRecord.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1331 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdRecordAsynch.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1253 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdState.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1266 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/CmdStatus.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2701 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/Commands.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)    51670 2023-03-08 10:18:44.000000 nxswriter-3.8.1/doc_html/FullDocument.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1756 2023-03-08 10:18:53.000000 nxswriter-3.8.1/doc_html/Properties.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1003 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/States.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)      903 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/TitleBanner.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)      979 2023-03-02 11:49:57.000000 nxswriter-3.8.1/doc_html/index.html
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      991 2022-11-22 20:26:35.000000 nxswriter-3.8.1/man/NXSDataWriter.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2209 2023-02-28 13:19:57.000000 nxswriter-3.8.1/man/nxsfromxml.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    86849 2023-03-08 09:00:26.000000 nxswriter-3.8.1/man/nxswriter.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       74 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxsfromxml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3889 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/ClientSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9068 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/DBaseSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6156 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/DataHolder.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4683 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/DataSourceFactory.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4574 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/DataSourcePool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5295 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/DataSources.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15052 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/DecoderPool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8599 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/EAttribute.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    26261 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/EField.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/EGroup.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8817 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/ELink.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4000 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/EStrategy.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3011 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/Element.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2099 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/ElementThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1660 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/Errors.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20455 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/FElement.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6821 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/FetchNameHandler.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6035 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/H5Elements.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4493 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/InnerXMLParser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3668 2022-12-12 12:16:40.000000 nxswriter-3.8.1/nxswriter/Metadata.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9077 2023-02-28 13:17:59.000000 nxswriter-3.8.1/nxswriter/NXSFromXML.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    31313 2023-03-02 11:51:13.000000 nxswriter-3.8.1/nxswriter/NXSWriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13805 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/NexusXMLHandler.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11230 2023-03-02 09:03:40.000000 nxswriter-3.8.1/nxswriter/PyEvalSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-03-09 13:11:43.000000 nxswriter-3.8.1/nxswriter/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 13:11:43.000000 nxswriter-3.8.1/nxswriter/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27784 2023-03-08 09:00:26.000000 nxswriter-3.8.1/nxswriter/TangoDataWriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29378 2023-03-09 13:11:43.000000 nxswriter-3.8.1/nxswriter/TangoSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6031 2023-03-08 09:00:26.000000 nxswriter-3.8.1/nxswriter/ThreadPool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7676 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/Types.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1760 2022-11-22 20:26:35.000000 nxswriter-3.8.1/nxswriter/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10763 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5577 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 20:30:29.000000 nxswriter-3.8.1/nxswriter.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       42 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       10 2023-03-09 13:19:26.000000 nxswriter-3.8.1/nxswriter.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      203 2023-03-09 13:19:26.000000 nxswriter-3.8.1/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4117 2022-11-22 20:26:35.000000 nxswriter-3.8.1/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-09 13:19:26.000000 nxswriter-3.8.1/test/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    52501 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/Checkers.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5501 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ClientFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5490 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ClientFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4684 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ClientFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4771 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ClientFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   105723 2023-03-02 07:45:36.000000 nxswriter-3.8.1/test/ClientFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   105064 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ClientFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20281 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ClientSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5954 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/Converters_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5612 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5598 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4882 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    87899 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    87520 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16850 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DBaseSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    30489 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DataHolder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10182 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DataSourceDecoders_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15976 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DataSourceFactory_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10560 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DataSourcePool_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5859 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DataSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12848 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/DecoderPool_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   108465 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EAttributeH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   107896 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EAttributeH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18366 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EDimH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18395 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EDimH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7839 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EDimensionsH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7832 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EDimensionsH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6412 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EDocH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6409 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EDocH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   285119 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EFieldH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   285230 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EFieldH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   171438 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EFieldReshapeH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   170929 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EFieldReshapeH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5329 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EFileH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5321 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EFileH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    42448 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EGroupH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    42416 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EGroupH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    72155 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ELinkH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    71822 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ELinkH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11340 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EStrategyH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11349 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/EStrategyH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7030 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ESymbolH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7120 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ESymbolH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3208 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ElementH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3204 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ElementH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5386 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ElementThread_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3629 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/Element_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4471 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/Errors_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45152 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FElementH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45164 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FElementH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    34938 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FElementWithAttrH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35205 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FElementWithAttrH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22964 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FetchNameHandler_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   344148 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FileWriterH5CppH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   179717 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FileWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/FileWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   215225 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/H5CppWriter_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   178444 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/H5PYWriter_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15547 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/InnerXMLParser_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15418 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/MYSQLSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46174 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/NTP_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   211886 2023-02-28 12:37:21.000000 nxswriter-3.8.1/test/NXSDataWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   211039 2023-02-28 12:37:21.000000 nxswriter-3.8.1/test/NXSDataWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    41359 2023-02-28 13:17:59.000000 nxswriter-3.8.1/test/NXSFromXMLH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    41371 2023-02-28 13:17:59.000000 nxswriter-3.8.1/test/NXSFromXMLH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   125101 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/NexusXMLHandlerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   125171 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/NexusXMLHandlerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14694 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ORACLESource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13061 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/PGSQLSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1652 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ProxyHelper.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5053 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ProxyTools_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    25478 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/PyEvalSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    54033 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/PyEvalTangoSourceH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    53808 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/PyEvalTangoSourceH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4886 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    52123 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/SimpleServer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5851 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/SimpleServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    21946 2023-03-09 13:11:43.000000 nxswriter-3.8.1/test/StreamSet_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7488 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TNObject_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      252 2018-09-14 10:01:58.000000 nxswriter-3.8.1/test/TangoClassID.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35756 2023-03-02 09:03:40.000000 nxswriter-3.8.1/test/TangoDataWriterH5CppH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   250238 2023-02-28 12:37:21.000000 nxswriter-3.8.1/test/TangoDataWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   250237 2023-02-28 12:37:21.000000 nxswriter-3.8.1/test/TangoDataWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5627 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TangoFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5618 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TangoFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4851 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TangoFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4841 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TangoFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   112661 2023-03-02 09:03:40.000000 nxswriter-3.8.1/test/TangoFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   112655 2023-03-02 09:03:40.000000 nxswriter-3.8.1/test/TangoFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   161008 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TangoSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11581 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TgDevice_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    33398 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TgGroup_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27676 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TgMember_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10508 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/ThreadPool_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4264 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/TstDataSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8163 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/UINT32decoder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5434 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/UTF8decoder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9237 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/VDEOdecoder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5365 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/XMLFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5354 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/XMLFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4712 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/XMLFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4702 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/XMLFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35614 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/XMLFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35619 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/XMLFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      923 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      945 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/__main__.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    20511 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/main.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1458 2018-09-14 10:01:58.000000 nxswriter-3.8.1/test/mydb.pgsql
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1646 2022-11-22 20:26:35.000000 nxswriter-3.8.1/test/sttest.py
```

### Comparing `nxswriter-3.8.0/.ci/debian10_py2/Dockerfile` & `nxswriter-3.8.1/.ci/debian10_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/debian10_py3/Dockerfile` & `nxswriter-3.8.1/.ci/debian10_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/debian11_py3/Dockerfile` & `nxswriter-3.8.1/.ci/debian11_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/debian8_py2/Dockerfile` & `nxswriter-3.8.1/.ci/debian8_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/debian8_py3/Dockerfile` & `nxswriter-3.8.1/.ci/debian8_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/debian9_py2/Dockerfile` & `nxswriter-3.8.1/.ci/debian9_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/debian9_py3/Dockerfile` & `nxswriter-3.8.1/.ci/debian9_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/install.sh` & `nxswriter-3.8.1/.ci/install.sh`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/ubuntu16.04_py2/Dockerfile` & `nxswriter-3.8.1/.ci/ubuntu16.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/ubuntu16.04_py3/Dockerfile` & `nxswriter-3.8.1/.ci/ubuntu16.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/ubuntu18.04_py2/Dockerfile` & `nxswriter-3.8.1/.ci/ubuntu18.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/ubuntu18.04_py3/Dockerfile` & `nxswriter-3.8.1/.ci/ubuntu18.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.ci/ubuntu20.04_py3/Dockerfile` & `nxswriter-3.8.1/.ci/ubuntu20.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/.github/workflows/tests.yml` & `nxswriter-3.8.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/COPYRIGHT` & `nxswriter-3.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/ChangeLog` & `nxswriter-3.8.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 2023-03-07 Jan Kotanski <jankotan@gmail.com>
+	* add timestamps to stderr and stdout logs (#142)
+	* tagged as 3.8.1
+
+2023-03-07 Jan Kotanski <jankotan@gmail.com>
 	* send WARNING, ERROR, FATAL to stderr by default (#139)
 	* tagged as 3.8.0
 
 2023-03-01 Jan Kotanski <jankotan@gmail.com>
 	* add MaxRecordRuntime and MaxElementRuntime tango server properties (#136)
 	* use datasource name as a keyword for Tango datasources (#136)
 	* tagged as 3.7.0
```

### Comparing `nxswriter-3.8.0/NXSDataWriter` & `nxswriter-3.8.1/NXSDataWriter`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/NXSDataWriter.xmi` & `nxswriter-3.8.1/NXSDataWriter.xmi`

 * *Files 0% similar despite different names*

#### Comparing `nxswriter-3.8.0/NXSDataWriter.xmi` & `nxswriter-3.8.1/NXSDataWriter.xmi`

```diff
@@ -26,15 +26,15 @@
       <status abstract="false" inherited="false" concrete="true" concreteHere="true"/>
     </deviceProperties>
     <deviceProperties name="DefaultCanFail" description="Default value of CanFail attribute">
       <type xsi:type="pogoDsl:BooleanType"/>
       <status abstract="false" inherited="false" concrete="true" concreteHere="true"/>
       <DefaultPropValue>True</DefaultPropValue>
     </deviceProperties>
-    <deviceProperties name="AddingLogs" description="Add XML logs  in nexus_logs of NXscollection">
+    <deviceProperties name="AddingLogs" description="Add XML logs in nexus_logs of NXcollection">
       <type xsi:type="pogoDsl:BooleanType"/>
       <status abstract="false" inherited="false" concrete="true" concreteHere="true"/>
       <DefaultPropValue>True</DefaultPropValue>
     </deviceProperties>
     <deviceProperties name="MaxRecordRuntime" description="maximal runtime for a record command in seconds">
       <type xsi:type="pogoDsl:DoubleType"/>
       <status abstract="false" inherited="false" concrete="true" concreteHere="true"/>
```

### Comparing `nxswriter-3.8.0/PKG-INFO` & `nxswriter-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxswriter
-Version: 3.8.0
+Version: 3.8.1
 Summary: Nexus Data writer implemented as a Tango Server
 Home-page: https://github.com/nexdatas/nxsdatawriter
 Author: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: Welcome to NXSDataWriter's documentation!
         =========================================
```

### Comparing `nxswriter-3.8.0/README.rst` & `nxswriter-3.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/MNI.xml` & `nxswriter-3.8.1/XMLExamples/MNI.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/encodedImage.xml` & `nxswriter-3.8.1/XMLExamples/encodedImage.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/encodedImage4.xml` & `nxswriter-3.8.1/XMLExamples/encodedImage4.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/scan.xml` & `nxswriter-3.8.1/XMLExamples/scan.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/scan2.xml` & `nxswriter-3.8.1/XMLExamples/scan2.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/scan3.xml` & `nxswriter-3.8.1/XMLExamples/scan3.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/test.xml` & `nxswriter-3.8.1/XMLExamples/test.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/XMLExamples/trigger.xml` & `nxswriter-3.8.1/XMLExamples/trigger.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc/Makefile` & `nxswriter-3.8.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc/conf.py` & `nxswriter-3.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc/make.bat` & `nxswriter-3.8.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc/nxswriter.rst` & `nxswriter-3.8.1/doc/nxswriter.rst`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrCanFail.html` & `nxswriter-3.8.1/doc_html/AttrCanFail.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrCurrentFileId.html` & `nxswriter-3.8.1/doc_html/AttrCurrentFileId.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrErrors.html` & `nxswriter-3.8.1/doc_html/AttrErrors.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrFileName.html` & `nxswriter-3.8.1/doc_html/AttrFileName.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrJSONRecord.html` & `nxswriter-3.8.1/doc_html/AttrJSONRecord.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrSkipAcquisition.html` & `nxswriter-3.8.1/doc_html/AttrSkipAcquisition.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrStepsPerFile.html` & `nxswriter-3.8.1/doc_html/AttrStepsPerFile.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/AttrXMLSettings.html` & `nxswriter-3.8.1/doc_html/AttrXMLSettings.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/Attributes.html` & `nxswriter-3.8.1/doc_html/Attributes.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/ClassDescription.html` & `nxswriter-3.8.1/doc_html/ClassDescription.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdCloseEntry.html` & `nxswriter-3.8.1/doc_html/CmdCloseEntry.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdCloseEntryAsynch.html` & `nxswriter-3.8.1/doc_html/CmdCloseEntryAsynch.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdCloseFile.html` & `nxswriter-3.8.1/doc_html/CmdCloseFile.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdOpenEntry.html` & `nxswriter-3.8.1/doc_html/CmdOpenEntry.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdOpenEntryAsynch.html` & `nxswriter-3.8.1/doc_html/CmdOpenEntryAsynch.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdOpenFile.html` & `nxswriter-3.8.1/doc_html/CmdOpenFile.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdRecord.html` & `nxswriter-3.8.1/doc_html/CmdRecord.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdRecordAsynch.html` & `nxswriter-3.8.1/doc_html/CmdRecordAsynch.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdState.html` & `nxswriter-3.8.1/doc_html/CmdState.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/CmdStatus.html` & `nxswriter-3.8.1/doc_html/CmdStatus.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/Commands.html` & `nxswriter-3.8.1/doc_html/Commands.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/FullDocument.html` & `nxswriter-3.8.1/doc_html/FullDocument.html`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 		<td> DefaultCanFail </td>
 		<td> Default value of CanFail attribute </td>
 		<td> boolean </td>
 		<td> True <br> </td>
 	</tr>
 	<tr>
 		<td> AddingLogs </td>
-		<td> Add XML logs  in nexus_logs of NXscollection </td>
+		<td> Add XML logs in nexus_logs of NXcollection </td>
 		<td> boolean </td>
 		<td> True <br> </td>
 	</tr>
 	<tr>
 		<td> MaxRecordRuntime </td>
 		<td> maximal runtime for a record command in seconds </td>
 		<td> double </td>
```

#### html2text {}

```diff
@@ -82,15 +82,15 @@
 |_________________|or_`h5py`_or_`h5cpp`|____________|___________________|
 |MetadataOutput   |metadata output:    |String      |none               |
 |_________________|`file`______________|____________|___________________|
 |DefaultCanFail   |Default value of    |boolean     |True               |
 |_________________|CanFail_attribute___|____________|___________________|
 |                 |Add XML logs in     |            |                   |
 |AddingLogs       |nexus_logs of       |boolean     |True               |
-|_________________|NXscollection_______|____________|___________________|
+|_________________|NXcollection________|____________|___________________|
 |                 |maximal runtime for |            |                   |
 |MaxRecordRuntime |a record command in |double      |0.0                |
 |_________________|seconds_____________|____________|___________________|
 |                 |maximal runtime for |            |                   |
 |MaxElementRuntime|a thread element in |double      |0.0                |
 |_________________|seconds_____________|____________|___________________|
```

### Comparing `nxswriter-3.8.0/doc_html/Properties.html` & `nxswriter-3.8.1/doc_html/Properties.html`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 		<td> DefaultCanFail </td>
 		<td> Default value of CanFail attribute </td>
 		<td> boolean </td>
 		<td> True <br> </td>
 	</tr>
 	<tr>
 		<td> AddingLogs </td>
-		<td> Add XML logs  in nexus_logs of NXscollection </td>
+		<td> Add XML logs in nexus_logs of NXcollection </td>
 		<td> boolean </td>
 		<td> True <br> </td>
 	</tr>
 	<tr>
 		<td> MaxRecordRuntime </td>
 		<td> maximal runtime for a record command in seconds </td>
 		<td> double </td>
```

#### html2text {}

```diff
@@ -16,14 +16,14 @@
 |_________________|or_`h5py`_or_`h5cpp`|____________|___________________|
 |MetadataOutput   |metadata output:    |String      |none               |
 |_________________|`file`______________|____________|___________________|
 |DefaultCanFail   |Default value of    |boolean     |True               |
 |_________________|CanFail_attribute___|____________|___________________|
 |                 |Add XML logs in     |            |                   |
 |AddingLogs       |nexus_logs of       |boolean     |True               |
-|_________________|NXscollection_______|____________|___________________|
+|_________________|NXcollection________|____________|___________________|
 |                 |maximal runtime for |            |                   |
 |MaxRecordRuntime |a record command in |double      |0.0                |
 |_________________|seconds_____________|____________|___________________|
 |                 |maximal runtime for |            |                   |
 |MaxElementRuntime|a thread element in |double      |0.0                |
 |_________________|seconds_____________|____________|___________________|
```

### Comparing `nxswriter-3.8.0/doc_html/States.html` & `nxswriter-3.8.1/doc_html/States.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/TitleBanner.html` & `nxswriter-3.8.1/doc_html/TitleBanner.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/doc_html/index.html` & `nxswriter-3.8.1/doc_html/index.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/man/NXSDataWriter.1` & `nxswriter-3.8.1/man/NXSDataWriter.1`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/man/nxsfromxml.1` & `nxswriter-3.8.1/man/nxsfromxml.1`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/man/nxswriter.1` & `nxswriter-3.8.1/man/nxswriter.1`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/ClientSource.py` & `nxswriter-3.8.1/nxswriter/ClientSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/DBaseSource.py` & `nxswriter-3.8.1/nxswriter/DBaseSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/DataHolder.py` & `nxswriter-3.8.1/nxswriter/DataHolder.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/DataSourceFactory.py` & `nxswriter-3.8.1/nxswriter/DataSourceFactory.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/DataSourcePool.py` & `nxswriter-3.8.1/nxswriter/DataSourcePool.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/DataSources.py` & `nxswriter-3.8.1/nxswriter/DataSources.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/DecoderPool.py` & `nxswriter-3.8.1/nxswriter/DecoderPool.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/EAttribute.py` & `nxswriter-3.8.1/nxswriter/EAttribute.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/EField.py` & `nxswriter-3.8.1/nxswriter/EField.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/EGroup.py` & `nxswriter-3.8.1/nxswriter/EGroup.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/ELink.py` & `nxswriter-3.8.1/nxswriter/ELink.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/EStrategy.py` & `nxswriter-3.8.1/nxswriter/EStrategy.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/Element.py` & `nxswriter-3.8.1/nxswriter/Element.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/ElementThread.py` & `nxswriter-3.8.1/nxswriter/ElementThread.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/Errors.py` & `nxswriter-3.8.1/nxswriter/Errors.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/FElement.py` & `nxswriter-3.8.1/nxswriter/FElement.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/FetchNameHandler.py` & `nxswriter-3.8.1/nxswriter/FetchNameHandler.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/H5Elements.py` & `nxswriter-3.8.1/nxswriter/H5Elements.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/InnerXMLParser.py` & `nxswriter-3.8.1/nxswriter/InnerXMLParser.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/Metadata.py` & `nxswriter-3.8.1/nxswriter/Metadata.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/NXSFromXML.py` & `nxswriter-3.8.1/nxswriter/NXSFromXML.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/NXSWriter.py` & `nxswriter-3.8.1/nxswriter/NXSWriter.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/NexusXMLHandler.py` & `nxswriter-3.8.1/nxswriter/NexusXMLHandler.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/PyEvalSource.py` & `nxswriter-3.8.1/nxswriter/PyEvalSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/Release.py` & `nxswriter-3.8.1/test/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,12 @@
 #    nexdatas is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
-#
-
-""" Tango Data Writer realease"""
-
+# \package nxswriter nexdatas
+# \file __init__.py
+# package constructor
 
-#: package version
-__version__ = "3.8.0"
+""" Tango Data Writer tests"""
```

### Comparing `nxswriter-3.8.0/nxswriter/StreamSet.py` & `nxswriter-3.8.1/nxswriter/StreamSet.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """ labels to Tango Streams """
 
 import sys
 import weakref
+import datetime
 
 
 # (:obj:`bool`) write stream to stdout
 stdoutflag = False
 
 # (:obj:`bool`) write stream to stderrr
 stderrflag = True
@@ -77,15 +78,16 @@
         """
         if std is None:
             std = stderrflag
         try:
             if self.log_fatal:
                 self.log_fatal.write(message + '\n')
             if std:
-                sys.stderr.write(message + '\n')
+                sys.stderr.write(
+                    "%s: FATAL: %s\n" % (datetime.datetime.now(), message))
                 sys.stderr.flush()
         except Exception:
             print(message)
 
     def error(self, message, std=None):
         """ writes error message
 
@@ -97,15 +99,16 @@
         """
         if std is None:
             std = stderrflag
         try:
             if self.log_error:
                 self.log_error.write(message + '\n')
             if std:
-                sys.stderr.write(message + '\n')
+                sys.stderr.write(
+                    "%s: ERROR: %s\n" % (datetime.datetime.now(), message))
                 sys.stderr.flush()
         except Exception:
             print(message)
 
     def warn(self, message, std=None):
         """ writes warning message
 
@@ -117,15 +120,16 @@
         """
         if std is None:
             std = stderrflag
         try:
             if self.log_warn:
                 self.log_warn.write(message + '\n')
             if std:
-                sys.stderr.write(message + '\n')
+                sys.stderr.write(
+                    "%s: WARNING: %s\n" % (datetime.datetime.now(), message))
                 sys.stderr.flush()
         except Exception:
             print(message)
 
     def info(self, message, std=None):
         """ writes info message
 
@@ -137,15 +141,16 @@
         """
         if std is None:
             std = stdoutflag
         try:
             if self.log_info:
                 self.log_info.write(message + '\n')
             elif std:
-                sys.stdout.write(message + '\n')
+                sys.stdout.write(
+                    "%s: INFO: %s\n" % (datetime.datetime.now(), message))
                 sys.stdout.flush()
         except Exception:
             print(message)
 
     def debug(self, message, std=None):
         """ writes debug message
 
@@ -157,11 +162,12 @@
        """
         if std is None:
             std = stdoutflag
         try:
             if self.log_debug:
                 self.log_debug.write(message + '\n')
             elif std:
-                sys.stdout.write(message + '\n')
+                sys.stdout.write(
+                    "%s: DEBUG: %s\n" % (datetime.datetime.now(), message))
                 sys.stdout.flush()
         except Exception:
             print(message)
```

### Comparing `nxswriter-3.8.0/nxswriter/TangoDataWriter.py` & `nxswriter-3.8.1/nxswriter/TangoDataWriter.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/TangoSource.py` & `nxswriter-3.8.1/nxswriter/TangoSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,22 +246,22 @@
             self.__proxy = ProxyTools.proxySetup(
                 self.device, streams=self._streams)
         except Exception:
             if self._streams:
                 self._streams.error(
                     "TangoSource::setup() - "
                     "Cannot connect to: %s \ndefined by %s"
-                    % (self.device, xml), std=False)
+                    % (self.device, xml))
 
         if not self.__proxy:
             if self._streams:
                 self._streams.error(
                     "TangoSource::setup() - "
                     "Cannot connect to: %s \ndefined by %s"
-                    % (self.device, xml), std=False)
+                    % (self.device, xml))
             # to make canfail works
             # raise DataSourceSetupError(
             #     "Cannot connect to: %s \ndefined by %s" % (self.device, xml))
         host = None
         if port and device and client:
             try:
                 host = self.__proxy.get_db_host().split(".")[0]
```

### Comparing `nxswriter-3.8.0/nxswriter/ThreadPool.py` & `nxswriter-3.8.1/nxswriter/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/Types.py` & `nxswriter-3.8.1/nxswriter/Types.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter/__init__.py` & `nxswriter-3.8.1/nxswriter/__init__.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/nxswriter.egg-info/PKG-INFO` & `nxswriter-3.8.1/nxswriter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxswriter
-Version: 3.8.0
+Version: 3.8.1
 Summary: Nexus Data writer implemented as a Tango Server
 Home-page: https://github.com/nexdatas/nxsdatawriter
 Author: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: Welcome to NXSDataWriter's documentation!
         =========================================
```

### Comparing `nxswriter-3.8.0/nxswriter.egg-info/SOURCES.txt` & `nxswriter-3.8.1/nxswriter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/setup.py` & `nxswriter-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/Checkers.py` & `nxswriter-3.8.1/test/Checkers.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.8.1/test/ClientFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientFieldTagAsynchH5PY_test.py` & `nxswriter-3.8.1/test/ClientFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientFieldTagServerH5Cpp_test.py` & `nxswriter-3.8.1/test/ClientFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientFieldTagServerH5PY_test.py` & `nxswriter-3.8.1/test/ClientFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientFieldTagWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/ClientFieldTagWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientFieldTagWriterH5PY_test.py` & `nxswriter-3.8.1/test/ClientFieldTagWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ClientSource_test.py` & `nxswriter-3.8.1/test/ClientSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/Converters_test.py` & `nxswriter-3.8.1/test/Converters_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.8.1/test/DBFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBFieldTagAsynchH5PY_test.py` & `nxswriter-3.8.1/test/DBFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBFieldTagServerH5Cpp_test.py` & `nxswriter-3.8.1/test/DBFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBFieldTagServerH5PY_test.py` & `nxswriter-3.8.1/test/DBFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBFieldTagWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/DBFieldTagWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBFieldTagWriterH5PY_test.py` & `nxswriter-3.8.1/test/DBFieldTagWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DBaseSource_test.py` & `nxswriter-3.8.1/test/DBaseSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DataHolder_test.py` & `nxswriter-3.8.1/test/DataHolder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DataSourceDecoders_test.py` & `nxswriter-3.8.1/test/DataSourceDecoders_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DataSourceFactory_test.py` & `nxswriter-3.8.1/test/DataSourceFactory_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DataSourcePool_test.py` & `nxswriter-3.8.1/test/DataSourcePool_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DataSource_test.py` & `nxswriter-3.8.1/test/DataSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/DecoderPool_test.py` & `nxswriter-3.8.1/test/DecoderPool_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EAttributeH5Cpp_test.py` & `nxswriter-3.8.1/test/EAttributeH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EAttributeH5PY_test.py` & `nxswriter-3.8.1/test/EAttributeH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EDimH5Cpp_test.py` & `nxswriter-3.8.1/test/EDimH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EDimH5PY_test.py` & `nxswriter-3.8.1/test/EDimH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EDimensionsH5Cpp_test.py` & `nxswriter-3.8.1/test/EDimensionsH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EDimensionsH5PY_test.py` & `nxswriter-3.8.1/test/EDimensionsH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EDocH5Cpp_test.py` & `nxswriter-3.8.1/test/EDocH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EDocH5PY_test.py` & `nxswriter-3.8.1/test/EDocH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EFieldH5Cpp_test.py` & `nxswriter-3.8.1/test/EFieldH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EFieldH5PY_test.py` & `nxswriter-3.8.1/test/EFieldH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EFieldReshapeH5Cpp_test.py` & `nxswriter-3.8.1/test/EFieldReshapeH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EFieldReshapeH5PY_test.py` & `nxswriter-3.8.1/test/EFieldReshapeH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EFileH5Cpp_test.py` & `nxswriter-3.8.1/test/EFileH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EFileH5PY_test.py` & `nxswriter-3.8.1/test/EFileH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EGroupH5Cpp_test.py` & `nxswriter-3.8.1/test/EGroupH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EGroupH5PY_test.py` & `nxswriter-3.8.1/test/EGroupH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ELinkH5Cpp_test.py` & `nxswriter-3.8.1/test/ELinkH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ELinkH5PY_test.py` & `nxswriter-3.8.1/test/ELinkH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EStrategyH5Cpp_test.py` & `nxswriter-3.8.1/test/EStrategyH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/EStrategyH5PY_test.py` & `nxswriter-3.8.1/test/EStrategyH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ESymbolH5Cpp_test.py` & `nxswriter-3.8.1/test/ESymbolH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ESymbolH5PY_test.py` & `nxswriter-3.8.1/test/ESymbolH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ElementH5Cpp_test.py` & `nxswriter-3.8.1/test/ElementH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ElementH5PY_test.py` & `nxswriter-3.8.1/test/ElementH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ElementThread_test.py` & `nxswriter-3.8.1/test/ElementThread_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/Element_test.py` & `nxswriter-3.8.1/test/Element_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/Errors_test.py` & `nxswriter-3.8.1/test/Errors_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FElementH5Cpp_test.py` & `nxswriter-3.8.1/test/FElementH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FElementH5PY_test.py` & `nxswriter-3.8.1/test/FElementH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FElementWithAttrH5Cpp_test.py` & `nxswriter-3.8.1/test/FElementWithAttrH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FElementWithAttrH5PY_test.py` & `nxswriter-3.8.1/test/FElementWithAttrH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FetchNameHandler_test.py` & `nxswriter-3.8.1/test/FetchNameHandler_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FileWriterH5CppH5PY_test.py` & `nxswriter-3.8.1/test/FileWriterH5CppH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FileWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/FileWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/FileWriterH5PY_test.py` & `nxswriter-3.8.1/test/FileWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/H5CppWriter_test.py` & `nxswriter-3.8.1/test/H5CppWriter_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/H5PYWriter_test.py` & `nxswriter-3.8.1/test/H5PYWriter_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/InnerXMLParser_test.py` & `nxswriter-3.8.1/test/InnerXMLParser_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/MYSQLSource_test.py` & `nxswriter-3.8.1/test/MYSQLSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NTP_test.py` & `nxswriter-3.8.1/test/NTP_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NXSDataWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/NXSDataWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NXSDataWriterH5PY_test.py` & `nxswriter-3.8.1/test/NXSDataWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NXSFromXMLH5Cpp_test.py` & `nxswriter-3.8.1/test/NXSFromXMLH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NXSFromXMLH5PY_test.py` & `nxswriter-3.8.1/test/NXSFromXMLH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NexusXMLHandlerH5Cpp_test.py` & `nxswriter-3.8.1/test/NexusXMLHandlerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/NexusXMLHandlerH5PY_test.py` & `nxswriter-3.8.1/test/NexusXMLHandlerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ORACLESource_test.py` & `nxswriter-3.8.1/test/ORACLESource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/PGSQLSource_test.py` & `nxswriter-3.8.1/test/PGSQLSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ProxyHelper.py` & `nxswriter-3.8.1/test/ProxyHelper.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ProxyTools_test.py` & `nxswriter-3.8.1/test/ProxyTools_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/PyEvalSource_test.py` & `nxswriter-3.8.1/test/PyEvalSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/PyEvalTangoSourceH5Cpp_test.py` & `nxswriter-3.8.1/test/PyEvalTangoSourceH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/PyEvalTangoSourceH5PY_test.py` & `nxswriter-3.8.1/test/PyEvalTangoSourceH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ServerSetUp.py` & `nxswriter-3.8.1/test/ServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/SimpleServer.py` & `nxswriter-3.8.1/test/SimpleServer.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/SimpleServerSetUp.py` & `nxswriter-3.8.1/test/SimpleServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/StreamSet_test.py` & `nxswriter-3.8.1/test/StreamSet_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,17 @@
                 self.streams.fatal(name, std=True)
             self.assertEqual(self.streams.log_fatal, None)
             self.assertEqual(self.streams.log_error, None)
             self.assertEqual(self.streams.log_warn, None)
             self.assertEqual(self.streams.log_info, None)
             self.assertEqual(self.streams.log_debug, None)
             self.assertEqual(self.mystdout.getvalue(), "")
-            self.assertEqual(self.mystderr.getvalue(), name + '\n')
+            self.assertEqual(
+                self.mystderr.getvalue().split(" ", 2)[-1],
+                "FATAL: " + name + '\n')
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_fatal_nostd(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
         for i in range(20):
@@ -182,19 +184,23 @@
             self.assertEqual(self.streams.log_fatal.getvalue(), name + '\n')
             self.assertEqual(self.streams.log_error.getvalue(), "")
             self.assertEqual(self.streams.log_warn.getvalue(), "")
             self.assertEqual(self.streams.log_info.getvalue(), "")
             self.assertEqual(self.streams.log_debug.getvalue(), "")
             self.assertEqual(self.mystdout.getvalue(), "")
             if i % 3 == 0:
-                self.assertEqual(self.mystderr.getvalue(), name + '\n')
+                self.assertEqual(
+                    self.mystderr.getvalue().split(" ", 2)[-1],
+                    "FATAL: " + name + '\n')
             elif i % 3 == 1:
                 self.assertEqual(self.mystderr.getvalue(), '')
             elif i % 3 == 2:
-                self.assertEqual(self.mystderr.getvalue(), name + '\n')
+                self.assertEqual(
+                    self.mystderr.getvalue().split(" ", 2)[-1],
+                    "FATAL: " + name + '\n')
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_error(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
         for i in range(20):
@@ -207,15 +213,17 @@
                 self.streams.error(name, std=True)
             self.assertEqual(self.streams.log_fatal, None)
             self.assertEqual(self.streams.log_error, None)
             self.assertEqual(self.streams.log_warn, None)
             self.assertEqual(self.streams.log_info, None)
             self.assertEqual(self.streams.log_debug, None)
             self.assertEqual(self.mystdout.getvalue(), "")
-            self.assertEqual(self.mystderr.getvalue(), name + '\n')
+            self.assertEqual(
+                self.mystderr.getvalue().split(" ", 2)[-1],
+                "ERROR: " + name + '\n')
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_error_nostd(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
         for i in range(20):
@@ -256,19 +264,23 @@
             self.assertEqual(self.streams.log_fatal.getvalue(), "")
             self.assertEqual(self.streams.log_error.getvalue(), name + '\n')
             self.assertEqual(self.streams.log_warn.getvalue(), "")
             self.assertEqual(self.streams.log_info.getvalue(), "")
             self.assertEqual(self.streams.log_debug.getvalue(), "")
             self.assertEqual(self.mystdout.getvalue(), "")
             if i % 3 == 0:
-                self.assertEqual(self.mystderr.getvalue(), name + '\n')
+                self.assertEqual(
+                    self.mystderr.getvalue().split(" ", 2)[-1],
+                    "ERROR: " + name + '\n')
             elif i % 3 == 1:
                 self.assertEqual(self.mystderr.getvalue(), '')
             elif i % 3 == 2:
-                self.assertEqual(self.mystderr.getvalue(), name + '\n')
+                self.assertEqual(
+                    self.mystderr.getvalue().split(" ", 2)[-1],
+                    "ERROR: " + name + '\n')
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_warn(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
         for i in range(20):
@@ -281,15 +293,17 @@
                 self.streams.warn(name, std=True)
             self.assertEqual(self.streams.log_fatal, None)
             self.assertEqual(self.streams.log_error, None)
             self.assertEqual(self.streams.log_warn, None)
             self.assertEqual(self.streams.log_info, None)
             self.assertEqual(self.streams.log_debug, None)
             self.assertEqual(self.mystdout.getvalue(), "")
-            self.assertEqual(self.mystderr.getvalue(), name + '\n')
+            self.assertEqual(
+                self.mystderr.getvalue().split(" ", 2)[-1],
+                "WARNING: " + name + '\n')
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_warn_nostd(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
         for i in range(20):
@@ -328,19 +342,23 @@
             self.assertEqual(self.streams.log_fatal.getvalue(), "")
             self.assertEqual(self.streams.log_error.getvalue(), "")
             self.assertEqual(self.streams.log_warn.getvalue(), name + '\n')
             self.assertEqual(self.streams.log_info.getvalue(), "")
             self.assertEqual(self.streams.log_debug.getvalue(), "")
             self.assertEqual(self.mystdout.getvalue(), "")
             if i % 3 == 0:
-                self.assertEqual(self.mystderr.getvalue(), name + '\n')
+                self.assertEqual(
+                    self.mystderr.getvalue().split(" ", 2)[-1],
+                    "WARNING: " + name + '\n')
             elif i % 3 == 1:
                 self.assertEqual(self.mystderr.getvalue(), '')
             elif i % 3 == 2:
-                self.assertEqual(self.mystderr.getvalue(), name + '\n')
+                self.assertEqual(
+                    self.mystderr.getvalue().split(" ", 2)[-1],
+                    "WARNING: " + name + '\n')
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_info(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
         for i in range(20):
@@ -349,15 +367,17 @@
             sys.stderr = self.mystderr = StringIO()
             self.streams.info(name, std=True)
             self.assertEqual(self.streams.log_fatal, None)
             self.assertEqual(self.streams.log_error, None)
             self.assertEqual(self.streams.log_warn, None)
             self.assertEqual(self.streams.log_info, None)
             self.assertEqual(self.streams.log_debug, None)
-            self.assertEqual(self.mystdout.getvalue(), name + '\n')
+            self.assertEqual(
+                self.mystdout.getvalue().split(" ", 2)[-1],
+                "INFO: " + name + '\n')
             self.assertEqual(self.mystderr.getvalue(), "")
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_info_nostd(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
@@ -418,15 +438,17 @@
             sys.stderr = self.mystderr = StringIO()
             self.streams.debug(name, std=True)
             self.assertEqual(self.streams.log_fatal, None)
             self.assertEqual(self.streams.log_error, None)
             self.assertEqual(self.streams.log_warn, None)
             self.assertEqual(self.streams.log_info, None)
             self.assertEqual(self.streams.log_debug, None)
-            self.assertEqual(self.mystdout.getvalue(), name + '\n')
+            self.assertEqual(
+                self.mystdout.getvalue().split(" ", 2)[-1],
+                "DEBUG: " + name + '\n')
             self.assertEqual(self.mystderr.getvalue(), "")
             sys.stdout = self.old_stdout
             sys.stderr = self.old_stderr
 
     def test_debug_nostd(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
```

### Comparing `nxswriter-3.8.0/test/TNObject_test.py` & `nxswriter-3.8.1/test/TNObject_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoDataWriterH5CppH5PY_test.py` & `nxswriter-3.8.1/test/TangoDataWriterH5CppH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoDataWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/TangoDataWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoDataWriterH5PY_test.py` & `nxswriter-3.8.1/test/TangoDataWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.8.1/test/TangoFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoFieldTagAsynchH5PY_test.py` & `nxswriter-3.8.1/test/TangoFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoFieldTagServerH5Cpp_test.py` & `nxswriter-3.8.1/test/TangoFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoFieldTagServerH5PY_test.py` & `nxswriter-3.8.1/test/TangoFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoFieldTagWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/TangoFieldTagWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoFieldTagWriterH5PY_test.py` & `nxswriter-3.8.1/test/TangoFieldTagWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TangoSource_test.py` & `nxswriter-3.8.1/test/TangoSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TgDevice_test.py` & `nxswriter-3.8.1/test/TgDevice_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TgGroup_test.py` & `nxswriter-3.8.1/test/TgGroup_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TgMember_test.py` & `nxswriter-3.8.1/test/TgMember_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/ThreadPool_test.py` & `nxswriter-3.8.1/test/ThreadPool_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/TstDataSource.py` & `nxswriter-3.8.1/test/TstDataSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/UINT32decoder_test.py` & `nxswriter-3.8.1/test/UINT32decoder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/UTF8decoder_test.py` & `nxswriter-3.8.1/test/UTF8decoder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/VDEOdecoder_test.py` & `nxswriter-3.8.1/test/VDEOdecoder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/XMLFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.8.1/test/XMLFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/XMLFieldTagAsynchH5PY_test.py` & `nxswriter-3.8.1/test/XMLFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/XMLFieldTagServerH5Cpp_test.py` & `nxswriter-3.8.1/test/XMLFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/XMLFieldTagServerH5PY_test.py` & `nxswriter-3.8.1/test/XMLFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/XMLFieldTagWriterH5Cpp_test.py` & `nxswriter-3.8.1/test/XMLFieldTagWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/XMLFieldTagWriterH5PY_test.py` & `nxswriter-3.8.1/test/XMLFieldTagWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/__init__.py` & `nxswriter-3.8.1/test/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
-#    Copyright (C) 2012-2017 DESY, Jan Kotanski <jkotan@mail.desy.de>
+#    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 #
 #    nexdatas is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
-# \package nxswriter nexdatas
-# \file __init__.py
-# package constructor
+# \package test nexdatas
+# \file runtest.py
+# the unittest runner
+#
+
+import main
+
 
-""" Tango Data Writer tests"""
+if __name__ == "__main__":
+    main.main()
```

### Comparing `nxswriter-3.8.0/test/__main__.py` & `nxswriter-3.8.1/nxswriter/Release.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
-#    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
+#    Copyright (C) 2012-2017 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 #
 #    nexdatas is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
-# \package test nexdatas
-# \file runtest.py
-# the unittest runner
 #
 
-import main
+""" Tango Data Writer realease"""
 
 
-if __name__ == "__main__":
-    main.main()
+#: package version
+__version__ = "3.8.1"
```

### Comparing `nxswriter-3.8.0/test/main.py` & `nxswriter-3.8.1/test/main.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/mydb.pgsql` & `nxswriter-3.8.1/test/mydb.pgsql`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.0/test/sttest.py` & `nxswriter-3.8.1/test/sttest.py`

 * *Files identical despite different names*

