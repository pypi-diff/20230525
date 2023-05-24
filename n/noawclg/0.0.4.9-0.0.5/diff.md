# Comparing `tmp/noawclg-0.0.4.9-py3-none-any.whl.zip` & `tmp/noawclg-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 18227 bytes, number of entries: 8
+Zip file size: 18353 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx      140 b- defN 23-Jan-13 03:41 noawclg/__init__.py
--rw-rw-r--  2.0 unx     5095 b- defN 23-Jan-13 03:55 noawclg/main.py
--rw-rw-r--  2.0 unx     1968 b- defN 23-Jan-13 03:37 noawclg/plot.py
--rw-rw-r--  2.0 unx    35148 b- defN 23-Jan-13 05:01 noawclg-0.0.4.9.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4106 b- defN 23-Jan-13 05:01 noawclg-0.0.4.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-13 05:01 noawclg-0.0.4.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-13 05:01 noawclg-0.0.4.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      615 b- defN 23-Jan-13 05:01 noawclg-0.0.4.9.dist-info/RECORD
-8 files, 47172 bytes uncompressed, 17161 bytes compressed:  63.6%
+-rw-rw-r--  2.0 unx     5147 b- defN 23-May-24 23:15 noawclg/main.py
+-rw-rw-r--  2.0 unx     1978 b- defN 23-May-24 23:13 noawclg/plot.py
+-rw-rw-r--  2.0 unx    35148 b- defN 23-May-24 23:20 noawclg-0.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4343 b- defN 23-May-24 23:20 noawclg-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-24 23:20 noawclg-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-24 23:20 noawclg-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      605 b- defN 23-May-24 23:20 noawclg-0.0.5.dist-info/RECORD
+8 files, 47461 bytes uncompressed, 17307 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: noawclg/main.py
 Comment: 
 
 Filename: noawclg/plot.py
 Comment: 
 
-Filename: noawclg-0.0.4.9.dist-info/LICENSE
+Filename: noawclg-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: noawclg-0.0.4.9.dist-info/METADATA
+Filename: noawclg-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: noawclg-0.0.4.9.dist-info/WHEEL
+Filename: noawclg-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: noawclg-0.0.4.9.dist-info/top_level.txt
+Filename: noawclg-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: noawclg-0.0.4.9.dist-info/RECORD
+Filename: noawclg-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## noawclg/main.py

```diff
@@ -52,15 +52,16 @@
 
 
 
 date_base = None
 def set_date(date:str):
     global date_base
     date_base = date #'08/01/2023'
-print(xr.__version__)
+
+print(xr.__version__) # need just and only from 0.20.1 version of xarray
 
 
 
 __date_now = datetime.now
 date_base_param = __date_now().strftime('%d/%m/%Y')
 
 
@@ -77,15 +78,15 @@
         '''
             params:
                 date: str
                     input a date in mode day/moth/year
                     ex: 08/01/2022
         '''
         if date_base:
-            print('i fun')
+            #print('i fun')
             date=date_base
 
         elif not date:
             date=date_base_param
         
 
         self.date = date
@@ -97,39 +98,39 @@
         self.url_data = url_data
         self.hour = hour
         
         date_input=date
         date=date.split('/')
         date=''.join(date)
         #print(date)
-        # url base from the data noaa in GFS 0.25 or GFS 1.00
+        #url base from the data noaa in GFS 0.25 or GFS 1.00
         #url_cdf=f'https://nomads.ncep.noaa.gov/dods/gfs_0p25/gfs{date}/gfs_0p25_{hour}z'
         url_cdf=f'https://nomads.ncep.noaa.gov/dods/gfs_{gfs}/gfs{date}/gfs_{gfs}_{hour}z'#'https://nomads.ncep.noaa.gov/dods/gfs_0p25/gfs20230103/gfs_0p25_00z'
        
         
         if url_data:
             print('hmm, url_data, its a urgency?..')
             url_cdf=url_data
     
         #self.date = date
         self.gfs = gfs
         self.url_data = url_data
         self.hour = hour
         print(f'url_data: {url_cdf}')
-        # reading the data required in the param's
+        #reading the data required in the param's
         file = xr.open_dataset(url_cdf)
         
         self.file_noaa = file
         
     
     def __getitem__(self,key:str):
         data_get = self.file_noaa.variables[key]
         return data_get
     
-    # getting the list data present in the data noaa GFS 0.25
+    #getting the list data present in the data noaa GFS 0.25
     def get_noaa_keys(self):
         '''
         '''
 
         keys = self.file_noaa.variables.keys()
         keys_about = {}
         for key in keys:
@@ -142,15 +143,15 @@
     def get_data_from_point(self,point:tuple):
         '''
         '''
         #new_data = self.file #get_noaa_data(hour=self.hour,date=self.date,gfs=self.gfs,url_data=self.url_data)
         #data = self.file.variables
         
         lat,lon = point[0],360+(point[1]) if point[1]<0 else point[1]
-        print(f"never print it!! just get the your need data's. ")
+        #print(f"never print it!! just get the your need data's. ")
         data_point = self.file_noaa.sel(lon=lon,lat=lat,method='nearest')
         # data_point = {'time':data_point.variables['time'],'data':data_point.variables[data_key]}
         
         return data_point
     
     
     def get_data_from_place(self,place:str):
@@ -158,8 +159,8 @@
         point = (location.latitude, location.longitude)
         #print(point)
 
         data_point = self.get_data_from_point(point=point)
 
         return data_point
     
-    
+
```

## noawclg/plot.py

```diff
@@ -25,15 +25,16 @@
     
     def render(self):
         if self.cla:
             plt.cla()
             plt.clf()
         data_point = self.data.get_data_from_place(self.place)
         temp = self.fmt_data(data_point[self.key_noaa])
-        print('getted data..')
+        #print('getted data..')
+        
         temp = temp.to_pandas()
 
         m_temp = temp.rolling(8).mean()
         max_temp = temp.rolling(8).max()
         min_temp = temp.rolling(8).min()
 
         ax2 = max_temp.plot(label=self.max_label)
@@ -42,15 +43,15 @@
 
         plt.title(self.title,fontweight='bold')
         plt.legend()
         #plt.annotate(self.author,xy=(temp.index[10],20))
         plt.text(0.14, 0.07, self.author, fontsize=10, fontweight='bold', transform=plt.gcf().transFigure)
         about_key=self.data.get_noaa_keys()[self.key_noaa]
         key_about = f'{self.key_noaa}:\n {about_key}'
-        plt.text(0.65, 0.07, key_about, fontsize=8, transform=plt.gcf().transFigure)
+        plt.text(0.65, 0.06, key_about, fontsize=8, transform=plt.gcf().transFigure)
         plt.text(0.65, 0.04, f'data: GFS{self.data.gfs} NOMADS-OpenDAP',color='gray', fontsize=8, transform=plt.gcf().transFigure)
         plt.text(0.19, 0.04, 'NOAA/NASA',color='gray',fontweight='bold', fontsize=9, transform=plt.gcf().transFigure)
 
         plt.xlabel(self.xlabel)
         plt.ylabel(self.ylabel)
 
         plt.tight_layout()
```

## Comparing `noawclg-0.0.4.9.dist-info/LICENSE` & `noawclg-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `noawclg-0.0.4.9.dist-info/METADATA` & `noawclg-0.0.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noawclg
-Version: 0.0.4.9
+Version: 0.0.5
 Summary: Library for getting dataset from noaa site
 Home-page: https://github.com/reinanbr/noawclg
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: GPLv3
 Keywords: climate weather noaa
 Description-Content-Type: text/markdown
@@ -135,7 +135,11 @@
 ```
 result:
 <img src='https://raw.githubusercontent.com/reinanbr/noawclg/main/plot_wind100m.png'/>
 
 
 
 <!-- the truest Reinan 13/01/23 01:58 :siga a rotina criada -->
+<!-- N se molde por ninguem e pra ninguem -->
+<!-- se precisar, abndone todos os complexos-->
+<!-- fique com qualquer uma, transe com quiem quiser transar ctg 10:15 14/01/23-->
+<!-- e demonstre isso em suas redes sociais, para vim mais-->
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: noawclg Version: 0.0.4.9 Summary: Library for
-getting dataset from noaa site Home-page: https://github.com/reinanbr/noawclg
-Author: Reinan Br Author-email: slimchatuba@gmail.com License: GPLv3 Keywords:
-climate weather noaa Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy Requires-Dist: xarray (<=0.20.1) Requires-Dist:
-netCDF4 (<=1.5.7) Requires-Dist: matplotlib Requires-Dist: geopy Requires-Dist:
+Metadata-Version: 2.1 Name: noawclg Version: 0.0.5 Summary: Library for getting
+dataset from noaa site Home-page: https://github.com/reinanbr/noawclg Author:
+Reinan Br Author-email: slimchatuba@gmail.com License: GPLv3 Keywords: climate
+weather noaa Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: numpy Requires-Dist: xarray (<=0.20.1) Requires-Dist: netCDF4
+(<=1.5.7) Requires-Dist: matplotlib Requires-Dist: geopy Requires-Dist:
 openpyxl
                              ****** NOAWClg ******
 
      [https://img.shields.io/badge/Autor-reinan_br-blue.svg?style=for-the-
                               badge&logo=github]
   [https://img.shields.io/pypi/v/noawclg] [https://img.shields.io/pypi/wheel/
                  noawclg] [PyPI_-_Downloads] [PyPI - License]
```

## Comparing `noawclg-0.0.4.9.dist-info/RECORD` & `noawclg-0.0.5.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noawclg/__init__.py,sha256=qvAaEJdlJbmUyNeroucZAvzewARgDoz7_npijrUzXsg,140
-noawclg/main.py,sha256=baBvTynp5xdGYiX--9FHyfSeTodCuXlOuL25huFyGTE,5095
-noawclg/plot.py,sha256=JXfYWv8kGG4_K8fh1S6GG4mvavUq62aWDkzNcXi1_78,1968
-noawclg-0.0.4.9.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-noawclg-0.0.4.9.dist-info/METADATA,sha256=bqVJtSPehfODZXYgpnRZcELZ2epX0Ff3_7OgtcOuq6M,4106
-noawclg-0.0.4.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-noawclg-0.0.4.9.dist-info/top_level.txt,sha256=3Mlxg6t9Z9-P7IrGjhe0cbDep3gT0zE9kxDQsLBDk6U,8
-noawclg-0.0.4.9.dist-info/RECORD,,
+noawclg/main.py,sha256=HbJ3v89B9wSP4CT4IG1DgOl27lOt4-kJanDvRk_h72g,5147
+noawclg/plot.py,sha256=WIYCgo-deFQsnwr3LNBCRcrXwrkz3Rsm10X4D7N9_2w,1978
+noawclg-0.0.5.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+noawclg-0.0.5.dist-info/METADATA,sha256=wJExcV-jkr-UzSEgMI6riLe4suI46hvEjQxfcYFmDi0,4343
+noawclg-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+noawclg-0.0.5.dist-info/top_level.txt,sha256=3Mlxg6t9Z9-P7IrGjhe0cbDep3gT0zE9kxDQsLBDk6U,8
+noawclg-0.0.5.dist-info/RECORD,,
```

