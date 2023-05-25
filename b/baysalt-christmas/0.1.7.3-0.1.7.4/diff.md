# Comparing `tmp/baysalt_christmas-0.1.7.3.tar.gz` & `tmp/baysalt_christmas-0.1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.3.tar", last modified: Wed May 17 09:02:38 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.4.tar", last modified: Thu May 25 08:49:35 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.3.tar` & `baysalt_christmas-0.1.7.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.199330 baysalt_christmas-0.1.7.3/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-09 03:21:44.000000 baysalt_christmas-0.1.7.3/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.3/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-17 09:02:38.199168 baysalt_christmas-0.1.7.3/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.3/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.193191 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.196340 baysalt_christmas-0.1.7.3/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    20792 2023-05-10 02:26:31.000000 baysalt_christmas-0.1.7.3/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.3/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.3/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.3/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.3/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.197982 baysalt_christmas-0.1.7.3/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.198836 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.3/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.3/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.3/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.3/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-05-17 09:02:38.199396 baysalt_christmas-0.1.7.3/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-05-17 09:02:36.000000 baysalt_christmas-0.1.7.3/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.910997 baysalt_christmas-0.1.7.4/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.4/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.4/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-25 08:49:35.910856 baysalt_christmas-0.1.7.4/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.4/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.905585 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-05-25 08:49:35.000000 baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.907886 baysalt_christmas-0.1.7.4/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    20844 2023-05-25 08:49:22.000000 baysalt_christmas-0.1.7.4/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.4/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.4/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.4/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.4/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.909709 baysalt_christmas-0.1.7.4/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-25 08:49:35.910511 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.4/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.4/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.4/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.4/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.4/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-05-25 08:49:35.911051 baysalt_christmas-0.1.7.4/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-05-25 08:49:31.000000 baysalt_christmas-0.1.7.4/setup.py
```

### Comparing `baysalt_christmas-0.1.7.3/.DS_Store` & `baysalt_christmas-0.1.7.4/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -270,31 +270,31 @@
 000010d0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000010e0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000010f0: 0066 006f 6c67 3153 636f 6d70 0000 0000  .f.olg1Scomp....
 00001100: 0000 1301 0000 001a 0062 0061 0079 0073  .........b.a.y.s
 00001110: 0061 006c 0074 005f 0063 0068 0072 0069  .a.l.t._.c.h.r.i
 00001120: 0073 0074 006d 0061 0073 002e 0065 0067  .s.t.m.a.s...e.g
 00001130: 0067 002d 0069 006e 0066 006f 6d6f 4444  .g.-.i.n.f.omoDD
-00001140: 626c 6f62 0000 0008 745c 6dc3 6afc c441  blob....t\m.j..A
+00001140: 626c 6f62 0000 0008 a182 0dd7 670a c541  blob........g..A
 00001150: 0000 001a 0062 0061 0079 0073 0061 006c  .....b.a.y.s.a.l
 00001160: 0074 005f 0063 0068 0072 0069 0073 0074  .t._.c.h.r.i.s.t
 00001170: 006d 0061 0073 002e 0065 0067 0067 002d  .m.a.s...e.g.g.-
 00001180: 0069 006e 0066 006f 6d6f 6444 626c 6f62  .i.n.f.omodDblob
-00001190: 0000 0008 745c 6dc3 6afc c441 0000 001a  ....t\m.j..A....
+00001190: 0000 0008 a182 0dd7 670a c541 0000 001a  ........g..A....
 000011a0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000011b0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000011c0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000011d0: 0066 006f 7068 3153 636f 6d70 0000 0000  .f.oph1Scomp....
 000011e0: 0000 5000 0000 0005 0062 0075 0069 006c  ..P......b.u.i.l
 000011f0: 0064 6c67 3153 636f 6d70 0000 0000 0001  .dlg1Scomp......
-00001200: 9651 0000 0005 0062 0075 0069 006c 0064  .Q.....b.u.i.l.d
-00001210: 6d6f 4444 626c 6f62 0000 0008 3414 94c3  moDDblob....4...
-00001220: 6afc c441 0000 0005 0062 0075 0069 006c  j..A.....b.u.i.l
-00001230: 0064 6d6f 6444 626c 6f62 0000 0008 3414  .dmodDblob....4.
-00001240: 94c3 6afc c441 0000 0005 0062 0075 0069  ..j..A.....b.u.i
+00001200: 97f8 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
+00001210: 6d6f 4444 626c 6f62 0000 0008 b036 39d7  moDDblob.....69.
+00001220: 670a c541 0000 0005 0062 0075 0069 006c  g..A.....b.u.i.l
+00001230: 0064 6d6f 6444 626c 6f62 0000 0008 b036  .dmodDblob.....6
+00001240: 39d7 670a c541 0000 0005 0062 0075 0069  9.g..A.....b.u.i
 00001250: 006c 0064 7068 3153 636f 6d70 0000 0000  .l.dph1Scomp....
 00001260: 0002 4000 0000 0009 0063 0068 0072 0069  ..@......c.h.r.i
 00001270: 0073 0074 006d 0061 0073 6277 7370 626c  .s.t.m.a.sbwspbl
 00001280: 6f62 0000 00ba 6270 6c69 7374 3030 d601  ob....bplist00..
 00001290: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000012a0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000012b0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
@@ -306,15 +306,15 @@
 00001310: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8c  }}...#/;R_klmno.
 00001320: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001330: 0000 0000 0000 0000 0000 0000 0000 008d  ................
 00001340: 0000 0009 0063 0068 0072 0069 0073 0074  .....c.h.r.i.s.t
 00001350: 006d 0061 0073 6473 636c 626f 6f6c 0100  .m.a.sdsclbool..
 00001360: 0000 0900 6300 6800 7200 6900 7300 7400  ....c.h.r.i.s.t.
 00001370: 6d00 6100 736c 6731 5363 6f6d 7000 0000  m.a.slg1Scomp...
-00001380: 0000 0219 f200 0000 0900 6300 6800 7200  ..........c.h.r.
+00001380: 0000 0216 8f00 0000 0900 6300 6800 7200  ..........c.h.r.
 00001390: 6900 7300 7400 6d00 6100 736c 7376 4362  i.s.t.m.a.slsvCb
 000013a0: 6c6f 6200 0003 0062 706c 6973 7430 30d8  lob....bplist00.
 000013b0: 0102 0304 0506 0708 090a 0b16 5354 550a  ............STU.
 000013c0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
 000013d0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
 000013e0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
 000013f0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
@@ -400,20 +400,20 @@
 000018f0: 0169 0172 0174 0175 0176 017f 0181 0182  .i.r.t.u.v......
 00001900: 0184 0185 018e 0190 0191 0194 0195 019e  ................
 00001910: 01a0 01a1 01a2 01a3 01ac 01b9 01c2 0000  ................
 00001920: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001930: 0000 0000 0000 0000 0000 0000 01c3 0000  ................
 00001940: 0009 0063 0068 0072 0069 0073 0074 006d  ...c.h.r.i.s.t.m
 00001950: 0061 0073 6d6f 4444 626c 6f62 0000 0008  .a.smoDDblob....
-00001960: 29ca 80d6 f904 c541 0000 0009 0063 0068  )......A.....c.h
+00001960: 8fa1 18c9 670a c541 0000 0009 0063 0068  ....g..A.....c.h
 00001970: 0072 0069 0073 0074 006d 0061 0073 6d6f  .r.i.s.t.m.a.smo
-00001980: 6444 626c 6f62 0000 0008 29ca 80d6 f904  dDblob....).....
+00001980: 6444 626c 6f62 0000 0008 8fa1 18c9 670a  dDblob........g.
 00001990: c541 0000 0009 0063 0068 0072 0069 0073  .A.....c.h.r.i.s
 000019a0: 0074 006d 0061 0073 7068 3153 636f 6d70  .t.m.a.sph1Scomp
-000019b0: 0000 0000 0003 8000 0000 0009 0063 0068  .............c.h
+000019b0: 0000 0000 0003 1000 0000 0009 0063 0068  .............c.h
 000019c0: 0072 0069 0073 0074 006d 0061 0073 7653  .r.i.s.t.m.a.svS
 000019d0: 726e 6c6f 6e67 0000 0001 0000 0004 0064  rnlong.........d
 000019e0: 0069 0073 0074 6277 7370 626c 6f62 0000  .i.s.tbwspblob..
 000019f0: 00b9 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001a00: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001a10: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001a20: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
@@ -422,19 +422,19 @@
 00001a50: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
 00001a60: 095f 1019 7b7b 3430 342c 2034 3738 7d2c  ._..{{404, 478},
 00001a70: 207b 3132 3338 2c20 3436 377d 7d09 0815   {1238, 467}}...
 00001a80: 232f 3b52 5f6b 6c6d 6e6f 8b00 0000 0000  #/;R_klmno......
 00001a90: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 8c00 0000 0400  ................
 00001ab0: 6400 6900 7300 746c 6731 5363 6f6d 7000  d.i.s.tlg1Scomp.
-00001ac0: 0000 0000 0139 1c00 0000 0400 6400 6900  .....9......d.i.
-00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 08d7  s.tmoDDblob.....
-00001ae0: 0398 c36a fcc4 4100 0000 0400 6400 6900  ...j..A.....d.i.
-00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 08d7  s.tmodDblob.....
-00001b00: 0398 c36a fcc4 4100 0000 0400 6400 6900  ...j..A.....d.i.
+00001ac0: 0000 0000 013a 3400 0000 0400 6400 6900  .....:4.....d.i.
+00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 08c3  s.tmoDDblob.....
+00001ae0: 703d d767 0ac5 4100 0000 0400 6400 6900  p=.g..A.....d.i.
+00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 08c3  s.tmodDblob.....
+00001b00: 703d d767 0ac5 4100 0000 0400 6400 6900  p=.g..A.....d.i.
 00001b10: 7300 7470 6831 5363 6f6d 7000 0000 0000  s.tph1Scomp.....
 00001b20: 0150 0000 0000 0400 6400 6900 7300 7476  .P......d.i.s.tv
 00001b30: 5372 6e6c 6f6e 6700 0000 0100 0000 0000  Srnlong.........
 00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `baysalt_christmas-0.1.7.3/PKG-INFO` & `baysalt_christmas-0.1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.3
+Version: 0.1.7.4
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.3/README.md` & `baysalt_christmas-0.1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.3
+Version: 0.1.7.4
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.4/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/Blogging.py` & `baysalt_christmas-0.1.7.4/christmas/Blogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             self.PARA_DEFAULT['debug_log_filename'] = f'{self.logfile_name}_debug.log'
             self.PARA_DEFAULT['info_log_filename'] = f'{self.logfile_name}_info.log'
             self.PARA_DEFAULT['warning_log_filename'] = f'{self.logfile_name}_warning.log'
             self.PARA_DEFAULT['error_log_filename'] = f'{self.logfile_name}_error.log'
             self.PARA_DEFAULT['critical_log_filename'] = f'{self.logfile_name}_critical.log'
         
         self.PARA = self.PARA_DEFAULT
+        self.setup_Blog()
         self.console()
     
     def setup_Blog(self, **kwargs):
         
         self.PARA.update(kwargs)
         self.maxBytes = self.PARA['maxBytes']
         self.backupCount = self.PARA['backupCount']
@@ -139,14 +140,15 @@
             rmfiles(self.__all_log_path,
                     self.__error_plus_log_path,
                     self.debug_log_filename,
                     self.info_log_filename,
                     self.warning_log_filename,
                     self.error_log_filename,
                     self.critical_log_filename)
+        self.console()
     
     def __init_logger_handler(self, logfile_path, Rotating='time', when='H', interval=1):
         # sourcery skip: inline-immediately-returned-variable
         """
         创建日志记录器handler，用于收集日志
         :param logfile_path: 日志文件路径
         :return: 日志记录器
@@ -251,15 +253,15 @@
         关闭日志记录器
         :param logger_handler: 日志记录器
         """
         logger_handler.close()
     
     def console(self):
         """构造日志收集器"""
-        self.setup_Blog()  # 初始化
+        # self.setup_Blog()  # 初始化
         self.logger.setLevel(self.log_level)  # 设置日志收集器级别
 
         if self.logger.hasHandlers():  # 如果已经有日志记录器，先关闭
             self.logger.handlers.clear()
         if self.logger.filters:  # 如果已经有日志过滤器，先关闭
             self.logger.filters.clear()
         if self.switch_write_all_log:  # 是否写入全部日志
@@ -295,15 +297,15 @@
         self.__set_log_formatter(error_logger_handler)  # 设置日志输出格式-error日志文件
         self.__set_log_handler(error_logger_handler, level=logging.ERROR)  # 设置handler级别并添加到logger收集器
         self.__close_log_handler(error_logger_handler)  # 关闭handler
     
     def __print_log(self):
         console_handle = colorlog.StreamHandler()  # 创建终端日志记录器handler，用于输出到控制台
         self.__set_color_formatter(console_handle, self.colors_config)  # 设置输出格式-控制台
-        self.__set_log_handler(console_handle, level=logging.DEBUG)  # 设置handler级别并添加到终端logger收集器
+        self.__set_log_handler(console_handle, level=self.log_level)  # 设置handler级别并添加到终端logger收集器
         self.__close_log_handler(console_handle)  # 关闭handler
     
     def __write_random_log(self, level=logging.ERROR, _level_log_name='all.log'):  # 日志单独输出
         random_logger_handler = self.__init_logger_handler(_level_log_name, Rotating=self.Rotating, when=self.when,
                                                            interval=self.interval)  # 收集随机日志信息文件
         self.__set_log_formatter(random_logger_handler)  # 设置日志输出格式-random日志文件
         self.__set_log_Filter(random_logger_handler, level)  # 设置过滤器
```

### Comparing `baysalt_christmas-0.1.7.3/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.4/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/commonCode.py` & `baysalt_christmas-0.1.7.4/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/cprintf.py` & `baysalt_christmas-0.1.7.4/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.4/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.4/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.4/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.4/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/processBar.py` & `baysalt_christmas-0.1.7.4/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/read_conf.py` & `baysalt_christmas-0.1.7.4/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/christmas/server_info.py` & `baysalt_christmas-0.1.7.4/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.3/setup.py` & `baysalt_christmas-0.1.7.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.3",
+    version="0.1.7.4",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

