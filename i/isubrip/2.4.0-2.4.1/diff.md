# Comparing `tmp/isubrip-2.4.0.tar.gz` & `tmp/isubrip-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isubrip-2.4.0.tar", last modified: Tue May 23 20:01:56 2023, max compression
+gzip compressed data, was "isubrip-2.4.1.tar", last modified: Thu May 25 09:09:54 2023, max compression
```

## Comparing `isubrip-2.4.0.tar` & `isubrip-2.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.316877 isubrip-2.4.0/
--rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     3536 2023-05-23 20:01:56.315875 isubrip-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2411 2023-05-23 20:01:27.000000 isubrip-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.303876 isubrip-2.4.0/isubrip/
--rw-rw-rw-   0        0        0       23 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/__init__.py
--rw-rw-rw-   0        0        0    12753 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/__main__.py
--rw-rw-rw-   0        0        0    11798 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/config.py
--rw-rw-rw-   0        0        0     2178 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/constants.py
--rw-rw-rw-   0        0        0     6053 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/data_structures.py
-drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.309880 isubrip-2.4.0/isubrip/resources/
--rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/resources/default_config.toml
-drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.312875 isubrip-2.4.0/isubrip/scrapers/
--rw-rw-rw-   0        0        0        0 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/__init__.py
--rw-rw-rw-   0        0        0    15845 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/appletv_scraper.py
--rw-rw-rw-   0        0        0     4375 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/itunes_scraper.py
--rw-rw-rw-   0        0        0    22230 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.315875 isubrip-2.4.0/isubrip/subtitle_formats/
--rw-rw-rw-   0        0        0        0 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/subrip.py
--rw-rw-rw-   0        0        0     7909 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/subtitles.py
--rw-rw-rw-   0        0        0     9220 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/webvtt.py
--rw-rw-rw-   0        0        0    13341 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.308879 isubrip-2.4.0/isubrip.egg-info/
--rw-rw-rw-   0        0        0     3536 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       83 2023-05-23 20:01:27.000000 isubrip-2.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 20:01:56.316877 isubrip-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2815 2023-05-23 20:01:27.000000 isubrip-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.720051 isubrip-2.4.1/
+-rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3536 2023-05-25 09:09:54.719053 isubrip-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2411 2023-05-25 08:44:47.000000 isubrip-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.704043 isubrip-2.4.1/isubrip/
+-rw-rw-rw-   0        0        0       23 2023-05-25 08:44:47.000000 isubrip-2.4.1/isubrip/__init__.py
+-rw-rw-rw-   0        0        0    12873 2023-05-25 08:19:55.000000 isubrip-2.4.1/isubrip/__main__.py
+-rw-rw-rw-   0        0        0    11798 2023-05-25 08:19:55.000000 isubrip-2.4.1/isubrip/config.py
+-rw-rw-rw-   0        0        0     2178 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/constants.py
+-rw-rw-rw-   0        0        0     6053 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.710051 isubrip-2.4.1/isubrip/resources/
+-rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.1/isubrip/resources/default_config.toml
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.714050 isubrip-2.4.1/isubrip/scrapers/
+-rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/__init__.py
+-rw-rw-rw-   0        0        0    15845 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/appletv_scraper.py
+-rw-rw-rw-   0        0        0     4375 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/itunes_scraper.py
+-rw-rw-rw-   0        0        0    22230 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.718051 isubrip-2.4.1/isubrip/subtitle_formats/
+-rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/subrip.py
+-rw-rw-rw-   0        0        0     7909 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/subtitles.py
+-rw-rw-rw-   0        0        0     9220 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/webvtt.py
+-rw-rw-rw-   0        0        0    13341 2023-05-25 08:19:55.000000 isubrip-2.4.1/isubrip/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.709051 isubrip-2.4.1/isubrip.egg-info/
+-rw-rw-rw-   0        0        0     3536 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       83 2023-05-24 22:34:46.000000 isubrip-2.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:09:54.720051 isubrip-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2815 2023-05-24 22:34:46.000000 isubrip-2.4.1/setup.py
```

### Comparing `isubrip-2.4.0/LICENSE` & `isubrip-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/PKG-INFO` & `isubrip-2.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.0 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.1 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.4.0 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.1 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
-downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.0
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.1
 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
```

### Comparing `isubrip-2.4.0/README.md` & `isubrip-2.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.0 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.1 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # iSubRip A Python package for scraping and downloading subtitles from AppleTV
-/ iTunes movie pages. Latest version: 2.4.0 ([changelog](https://github.com/
+/ iTunes movie pages. Latest version: 2.4.1 ([changelog](https://github.com/
 MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
```

### Comparing `isubrip-2.4.0/isubrip/__main__.py` & `isubrip-2.4.1/isubrip/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
             try:
                 scraper = scraper_factory.get_scraper_instance(url=url, config_data=config.data.get("scrapers"))
                 atexit.register(scraper.close)
                 scraper.config.check()
 
                 media_data: MovieData = scraper.get_data(url=url)
+                media_items: list[MovieData] = single_to_list(media_data)
 
-                print(f"Found movie: {media_data.name} ({media_data.release_date.year})")
+                print(f"Found movie: {media_items[0].name} ({media_items[0].release_date.year})")
 
                 if not media_data:
                     print(f"Error: No supported media data was found for {url}.")
                     continue
 
                 download_media_subtitles_args = {
                     "download_path": Path(config.downloads["folder"]),
                     "language_filter": config.downloads.get("languages"),
                     "convert_to_srt": config.subtitles.get("convert-to-srt", False),
                     "overwrite_existing": config.downloads.get("overwrite-existing", False),
                     "zip_files": config.downloads.get("zip", False),
                 }
 
-                media_items: list[MovieData] = single_to_list(media_data)
                 multiple_media_items = len(media_items) > 1
                 if multiple_media_items:
                     print(f"{len(media_items)} media items were found.")
 
                 for media_item in media_items:
                     media_id = media_item.id or media_item.alt_id or media_item.name
 
@@ -99,16 +99,15 @@
                         else:
                             failed_count = len(results.failed_subtitles)
                             print(f"\n{success_count}/{success_count + failed_count} matching subtitles "
                                   f"have been successfully downloaded.", sep='')
 
                     except Exception as e:
                         if multiple_media_items:
-                            print(f"Error: Encountered an error while scraping playlist for "
-                                  f"{media_id}: {e}")
+                            print(f"Error: Encountered an error while scraping playlist for {media_id}: {e}")
                             continue
 
                         else:
                             raise e
 
             except Exception as e:
                 if multiple_urls:
@@ -204,18 +203,21 @@
         except Exception:
             failed_downloads.append(subtitles_data)
             continue
 
     if not zip_files or len(temp_downloads) == 1:
         for file_path in temp_downloads:
             if overwrite_existing:
-                file_path.replace(download_path / file_path.name)
+                new_path = download_path / file_path.name
 
             else:
-                file_path.replace(generate_non_conflicting_path(download_path / file_path.name))
+                new_path = generate_non_conflicting_path(download_path / file_path.name)
+
+            # str conversion needed only for Python 3.8 - https://github.com/python/cpython/issues/76870
+            shutil.move(src=str(file_path), dst=new_path)
 
     else:
         archive_path = Path(shutil.make_archive(
             base_name=str(temp_download_path.parent / temp_download_path.name),
             format=ARCHIVE_FORMAT,
             root_dir=temp_download_path,
         ))
```

### Comparing `isubrip-2.4.0/isubrip/config.py` & `isubrip-2.4.1/isubrip/config.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/constants.py` & `isubrip-2.4.1/isubrip/constants.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/data_structures.py` & `isubrip-2.4.1/isubrip/data_structures.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/resources/default_config.toml` & `isubrip-2.4.1/isubrip/resources/default_config.toml`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/scrapers/appletv_scraper.py` & `isubrip-2.4.1/isubrip/scrapers/appletv_scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/scrapers/itunes_scraper.py` & `isubrip-2.4.1/isubrip/scrapers/itunes_scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/scrapers/scraper.py` & `isubrip-2.4.1/isubrip/scrapers/scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/subtitle_formats/subrip.py` & `isubrip-2.4.1/isubrip/subtitle_formats/subrip.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/subtitle_formats/subtitles.py` & `isubrip-2.4.1/isubrip/subtitle_formats/subtitles.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/subtitle_formats/webvtt.py` & `isubrip-2.4.1/isubrip/subtitle_formats/webvtt.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip/utils.py` & `isubrip-2.4.1/isubrip/utils.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/isubrip.egg-info/PKG-INFO` & `isubrip-2.4.1/isubrip.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.0 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.1 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.4.0 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.1 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
-downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.0
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.1
 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
```

### Comparing `isubrip-2.4.0/isubrip.egg-info/SOURCES.txt` & `isubrip-2.4.1/isubrip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.0/setup.py` & `isubrip-2.4.1/setup.py`

 * *Files identical despite different names*

