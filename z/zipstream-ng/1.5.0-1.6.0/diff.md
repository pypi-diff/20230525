# Comparing `tmp/zipstream-ng-1.5.0.tar.gz` & `tmp/zipstream-ng-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipstream-ng-1.5.0.tar", last modified: Fri Mar 31 14:27:33 2023, max compression
+gzip compressed data, was "zipstream-ng-1.6.0.tar", last modified: Thu May 25 01:37:07 2023, max compression
```

## Comparing `zipstream-ng-1.5.0.tar` & `zipstream-ng-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-31 14:27:33.009654 zipstream-ng-1.5.0/
--rw-r--r--   0 carey      (501) staff       (20)     7652 2021-12-13 03:37:00.000000 zipstream-ng-1.5.0/LICENSE
--rw-r--r--   0 carey      (501) staff       (20)     9191 2023-03-31 14:27:33.009315 zipstream-ng-1.5.0/PKG-INFO
--rw-r--r--   0 carey      (501) staff       (20)     8162 2023-03-31 13:43:52.000000 zipstream-ng-1.5.0/README.md
--rw-r--r--   0 carey      (501) staff       (20)       38 2023-03-31 14:27:33.009792 zipstream-ng-1.5.0/setup.cfg
--rw-r--r--   0 carey      (501) staff       (20)     1561 2023-03-31 14:26:10.000000 zipstream-ng-1.5.0/setup.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-31 14:27:33.005914 zipstream-ng-1.5.0/tests/
--rw-r--r--   0 carey      (501) staff       (20)    39009 2023-03-31 13:43:52.000000 zipstream-ng-1.5.0/tests/test_zipstream.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-31 14:27:33.007332 zipstream-ng-1.5.0/zipstream/
--rw-r--r--   0 carey      (501) staff       (20)      161 2023-03-31 13:40:52.000000 zipstream-ng-1.5.0/zipstream/__init__.py
--rw-r--r--   0 carey      (501) staff       (20)    41832 2023-03-31 14:17:45.000000 zipstream-ng-1.5.0/zipstream/ng.py
--rwxr-xr-x   0 carey      (501) staff       (20)     6886 2022-12-28 20:48:01.000000 zipstream-ng-1.5.0/zipstream/server.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-03-31 14:27:33.008993 zipstream-ng-1.5.0/zipstream_ng.egg-info/
--rw-r--r--   0 carey      (501) staff       (20)     9191 2023-03-31 14:27:32.000000 zipstream-ng-1.5.0/zipstream_ng.egg-info/PKG-INFO
--rw-r--r--   0 carey      (501) staff       (20)      326 2023-03-31 14:27:33.000000 zipstream-ng-1.5.0/zipstream_ng.egg-info/SOURCES.txt
--rw-r--r--   0 carey      (501) staff       (20)        1 2023-03-31 14:27:32.000000 zipstream-ng-1.5.0/zipstream_ng.egg-info/dependency_links.txt
--rw-r--r--   0 carey      (501) staff       (20)       52 2023-03-31 14:27:32.000000 zipstream-ng-1.5.0/zipstream_ng.egg-info/entry_points.txt
--rw-r--r--   0 carey      (501) staff       (20)       27 2023-03-31 14:27:32.000000 zipstream-ng-1.5.0/zipstream_ng.egg-info/requires.txt
--rw-r--r--   0 carey      (501) staff       (20)       10 2023-03-31 14:27:32.000000 zipstream-ng-1.5.0/zipstream_ng.egg-info/top_level.txt
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-05-25 01:37:07.958326 zipstream-ng-1.6.0/
+-rw-r--r--   0 carey      (501) staff       (20)     7652 2021-12-13 03:37:00.000000 zipstream-ng-1.6.0/LICENSE
+-rw-r--r--   0 carey      (501) staff       (20)    10060 2023-05-25 01:37:07.957924 zipstream-ng-1.6.0/PKG-INFO
+-rw-r--r--   0 carey      (501) staff       (20)     9031 2023-04-25 20:12:41.000000 zipstream-ng-1.6.0/README.md
+-rw-r--r--   0 carey      (501) staff       (20)       38 2023-05-25 01:37:07.958393 zipstream-ng-1.6.0/setup.cfg
+-rw-r--r--   0 carey      (501) staff       (20)     1561 2023-05-25 01:13:49.000000 zipstream-ng-1.6.0/setup.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-05-25 01:37:07.953745 zipstream-ng-1.6.0/tests/
+-rw-r--r--   0 carey      (501) staff       (20)    45016 2023-04-25 20:12:41.000000 zipstream-ng-1.6.0/tests/test_zipstream.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-05-25 01:37:07.955465 zipstream-ng-1.6.0/zipstream/
+-rw-r--r--   0 carey      (501) staff       (20)      161 2023-03-31 13:40:52.000000 zipstream-ng-1.6.0/zipstream/__init__.py
+-rw-r--r--   0 carey      (501) staff       (20)    43790 2023-04-28 00:23:41.000000 zipstream-ng-1.6.0/zipstream/ng.py
+-rwxr-xr-x   0 carey      (501) staff       (20)     6886 2022-12-28 20:48:01.000000 zipstream-ng-1.6.0/zipstream/server.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-05-25 01:37:07.957467 zipstream-ng-1.6.0/zipstream_ng.egg-info/
+-rw-r--r--   0 carey      (501) staff       (20)    10060 2023-05-25 01:37:07.000000 zipstream-ng-1.6.0/zipstream_ng.egg-info/PKG-INFO
+-rw-r--r--   0 carey      (501) staff       (20)      326 2023-05-25 01:37:07.000000 zipstream-ng-1.6.0/zipstream_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 carey      (501) staff       (20)        1 2023-05-25 01:37:07.000000 zipstream-ng-1.6.0/zipstream_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 carey      (501) staff       (20)       52 2023-05-25 01:37:07.000000 zipstream-ng-1.6.0/zipstream_ng.egg-info/entry_points.txt
+-rw-r--r--   0 carey      (501) staff       (20)       27 2023-05-25 01:37:07.000000 zipstream-ng-1.6.0/zipstream_ng.egg-info/requires.txt
+-rw-r--r--   0 carey      (501) staff       (20)       10 2023-05-25 01:37:07.000000 zipstream-ng-1.6.0/zipstream_ng.egg-info/top_level.txt
```

### Comparing `zipstream-ng-1.5.0/LICENSE` & `zipstream-ng-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zipstream-ng-1.5.0/PKG-INFO` & `zipstream-ng-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipstream-ng
-Version: 1.5.0
+Version: 1.6.0
 Summary: A modern and easy to use streamable zip file generator
 Home-page: https://github.com/pR0Ps/zipstream-ng
 License: LGPLv3
 Project-URL: Source, https://github.com/pR0Ps/zipstream-ng
 Project-URL: Changelog, https://github.com/pR0Ps/zipstream-ng/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -25,32 +25,45 @@
 zipstream-ng
 ============
 [![Status](https://github.com/pR0Ps/zipstream-ng/workflows/tests/badge.svg)](https://github.com/pR0Ps/zipstream-ng/actions/workflows/tests.yml)
 [![Version](https://img.shields.io/pypi/v/zipstream-ng.svg)](https://pypi.org/project/zipstream-ng/)
 ![Python](https://img.shields.io/pypi/pyversions/zipstream-ng.svg)
 
 A modern and easy to use streamable zip file generator. It can package and stream many files and
-folders on the fly without needing temporary files or excessive memory.
+folders into a zip on the fly without needing temporary files or excessive memory. It can also
+calculate the final size of the zip file before streaming it.
 
-Includes the ability to calculate the total size of the stream before any data is actually added
-(provided no compression is used). This makes it ideal for use in web applications since the total
-size can be used to set the `Content-Length` header without having to generate the entire file first
-(see examples below).
 
-Features:
+### Features:
  - Generates zip data on the fly as it's requested.
  - Can calculate the total size of the resulting zip file before generation even begins.
+ - Low memory usage: Since the zip is generated as it's requested, very little has to be kept in
+   memory (peak usage of less than 20MB is typical, even for TBs of files).
  - Flexible API: Typical use cases are simple, complicated ones are possible.
  - Supports zipping data from files, bytes, strings, and any other iterable objects.
- - Threadsafe: Won't mangle data if multiple threads concurrently add/read data to/from the same stream.
+ - Keeps track of the date of the most recently modified file added to the zip file.
+ - Threadsafe: Won't mangle data if multiple threads concurrently add data to the same stream.
  - Includes a clone of Python's `http.server` module with zip support added. Try `python -m zipstream.server`.
  - Automatically uses Zip64 extensions, but only if they are required.
  - No external dependencies.
 
 
+### Ideal for web backends:
+ - Generating zip data on the fly requires very little memory, no disk usage, and starts producing
+   data with less latency than creating the entire zip up-front. This means faster responses, no
+   temporary files, and very low memory usage.
+ - The ability to calculate the total size of the stream before any data is actually generated
+   (provided no compression is used) means web backends can provide a `Content-Length` header in
+   their responses. This allows clients to show a progress bar as the stream is transferred.
+ - By keeping track of the date of the most recently modified file added to the zip, web
+   backends can provide a `Last-Modified` header. This allows clients to check if they have the most
+   up-to-date version of the zip with just a HEAD request instead of having to download the entire
+   thing.
+
+
 Installation
 ------------
 ```
 pip install zipstream-ng
 ```
 
 
@@ -100,15 +113,15 @@
 zs.add(random_data(), "random.bin")
 
 # Add a file containing some static text.
 # Will automatically be encoded to bytes before being added (uses utf-8).
 zs.add("This is some text", "README.txt")
 
 # Write out the zip file as it's being generated.
-# At this point the data in the files files will be read in and the generator
+# At this point the data in the files will be read in and the generator
 # will be iterated over.
 with open("files.zip", "wb") as f:
     f.writelines(zs)
 ```
 
 
 ### zipserver (included)
```

### Comparing `zipstream-ng-1.5.0/README.md` & `zipstream-ng-1.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 zipstream-ng
 ============
 [![Status](https://github.com/pR0Ps/zipstream-ng/workflows/tests/badge.svg)](https://github.com/pR0Ps/zipstream-ng/actions/workflows/tests.yml)
 [![Version](https://img.shields.io/pypi/v/zipstream-ng.svg)](https://pypi.org/project/zipstream-ng/)
 ![Python](https://img.shields.io/pypi/pyversions/zipstream-ng.svg)
 
 A modern and easy to use streamable zip file generator. It can package and stream many files and
-folders on the fly without needing temporary files or excessive memory.
+folders into a zip on the fly without needing temporary files or excessive memory. It can also
+calculate the final size of the zip file before streaming it.
 
-Includes the ability to calculate the total size of the stream before any data is actually added
-(provided no compression is used). This makes it ideal for use in web applications since the total
-size can be used to set the `Content-Length` header without having to generate the entire file first
-(see examples below).
 
-Features:
+### Features:
  - Generates zip data on the fly as it's requested.
  - Can calculate the total size of the resulting zip file before generation even begins.
+ - Low memory usage: Since the zip is generated as it's requested, very little has to be kept in
+   memory (peak usage of less than 20MB is typical, even for TBs of files).
  - Flexible API: Typical use cases are simple, complicated ones are possible.
  - Supports zipping data from files, bytes, strings, and any other iterable objects.
- - Threadsafe: Won't mangle data if multiple threads concurrently add/read data to/from the same stream.
+ - Keeps track of the date of the most recently modified file added to the zip file.
+ - Threadsafe: Won't mangle data if multiple threads concurrently add data to the same stream.
  - Includes a clone of Python's `http.server` module with zip support added. Try `python -m zipstream.server`.
  - Automatically uses Zip64 extensions, but only if they are required.
  - No external dependencies.
 
 
+### Ideal for web backends:
+ - Generating zip data on the fly requires very little memory, no disk usage, and starts producing
+   data with less latency than creating the entire zip up-front. This means faster responses, no
+   temporary files, and very low memory usage.
+ - The ability to calculate the total size of the stream before any data is actually generated
+   (provided no compression is used) means web backends can provide a `Content-Length` header in
+   their responses. This allows clients to show a progress bar as the stream is transferred.
+ - By keeping track of the date of the most recently modified file added to the zip, web
+   backends can provide a `Last-Modified` header. This allows clients to check if they have the most
+   up-to-date version of the zip with just a HEAD request instead of having to download the entire
+   thing.
+
+
 Installation
 ------------
 ```
 pip install zipstream-ng
 ```
 
 
@@ -76,15 +89,15 @@
 zs.add(random_data(), "random.bin")
 
 # Add a file containing some static text.
 # Will automatically be encoded to bytes before being added (uses utf-8).
 zs.add("This is some text", "README.txt")
 
 # Write out the zip file as it's being generated.
-# At this point the data in the files files will be read in and the generator
+# At this point the data in the files will be read in and the generator
 # will be iterated over.
 with open("files.zip", "wb") as f:
     f.writelines(zs)
 ```
 
 
 ### zipserver (included)
```

### Comparing `zipstream-ng-1.5.0/setup.py` & `zipstream-ng-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         long_description = f.read()
 except Exception:
     long_description=None
 
 
 setup(
     name="zipstream-ng",
-    version="1.5.0",
+    version="1.6.0",
     description="A modern and easy to use streamable zip file generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pR0Ps/zipstream-ng",
     project_urls={
         "Source": "https://github.com/pR0Ps/zipstream-ng",
         "Changelog": "https://github.com/pR0Ps/zipstream-ng/blob/master/CHANGELOG.md",
```

### Comparing `zipstream-ng-1.5.0/tests/test_zipstream.py` & `zipstream-ng-1.6.0/tests/test_zipstream.py`

 * *Files 3% similar despite different names*

```diff
@@ -471,14 +471,17 @@
         assert zinfos[i].file_size == 0
         assert zinfos[i].compress_size == 0
 
 
 def test_mkdir():
     zs = ZipStream(sized=True)
 
+    with pytest.raises(ValueError, match="A valid arcname .* is required"):
+        zs.mkdir("")
+
     PATHS = (
         "folder0",  # no trailing slash
         "folder1",
         "folder1/sub",  # into existing dir
         "folder2/sub/sub/sub/",  # new path
     )
 
@@ -575,14 +578,101 @@
     assert len(zinfos) == 1
     assert zinfos[0].filename == "top/"
     assert zinfos[0].is_dir()
     assert zinfos[0].file_size == 0
     assert zinfos[0].compress_size == 0
 
 
+@pytest.mark.parametrize("preserve_empty", [True, False])
+@pytest.mark.parametrize("followlinks", [True, False])
+def test_zipstream_walk(tmpdir, preserve_empty, followlinks):
+    """Test the zipstream's walk walks the walk it talks"""
+
+    # Create directory structure
+    t = tmpdir.mkdir("top")
+    t.mkdir("empty")
+    t.join("empty.txt").write("")
+    t.join("test.txt").write("test")
+    f = t.mkdir("filled")
+    f.join("file.bin").write_binary(b"\x00\x01\xFF")
+
+    # Can't make symlinks on some platforms
+    symlink_support = hasattr(t, "mksymlinkto")
+    if symlink_support:
+        f.join("file2.bin").mksymlinkto("file.bin")
+
+        o = tmpdir.mkdir("othertop")
+        o.join("other.txt").write("other")
+        f.join("notevil").mksymlinkto("../../othertop")
+        f.join("evil").mksymlinkto("../")
+
+    def walk(path):
+        yield from zipstream.walk(
+            path,
+            preserve_empty=preserve_empty,
+            followlinks=followlinks
+        )
+
+    zs = ZipStream.from_path(t, recurse=walk)
+    data = bytes(zs)
+    assert len(data) == len(zs)
+
+    contents = {
+        x.filename: x.is_dir()
+        for x in _get_zip(data).infolist()
+    }
+
+    for name, is_dir in contents.items():
+        assert (name == "top/empty/") == is_dir
+
+    names = set(contents)
+    assert "top/empty.txt" in names
+    assert symlink_support == ("top/filled/file2.bin" in names)
+    assert "top/filled/file.bin" in names
+    assert "top/test.txt" in names
+    assert preserve_empty == ("top/empty/" in names)
+    assert (symlink_support and followlinks) == ("top/filled/notevil/other.txt" in names)
+
+
+def test_custom_walk(tmpdir):
+    """Test that custom walk functions are supported"""
+
+    t = tmpdir.mkdir("top")
+    t.join("1.txt").write("1")
+    t.join("2.txt").write("22")
+    t.join("3.bin").write("333")
+    t.join("4.txt").write("4444")
+    t.join("5.txt").write("55555")
+    t.mkdir("empty")
+
+    def custom_walk(path):
+        for dirpath, dirnames, files in os.walk(path):
+            for f in files:
+                if f.endswith(".bin"):
+                    continue
+                fullpath = os.path.join(dirpath, f)
+                if os.path.getsize(fullpath) > 4:
+                    continue
+                yield fullpath
+
+            if not files and not dirnames:
+                yield dirpath  # no trailing pathsep
+
+    zs = ZipStream.from_path(t, recurse=custom_walk)
+    data = bytes(zs)
+    assert len(data) == len(zs)
+    zf = _get_zip(data)
+    assert zf.getinfo("top/empty/").is_dir()
+
+    names = sorted(x.filename for x in zf.infolist())
+    assert len(names) == 4
+    assert "top/3.bin" not in names
+    assert "top/5.txt" not in names
+
+
 @pytest.mark.parametrize("data", [
     "this is a string",
     b"these are some bytes",
     bytearray(b"this is a bytearray"),
     [b"a", b"list", b"of", b"bytes"],
     _gen_rand()
 ])
@@ -605,17 +695,17 @@
     elif not isinstance(data, (bytes, str, bytearray)):
         # tee the iterator and get the contents from it so they can be checked
         # against what's put into the stream
         tostore, data = itertools.tee(data)
         data = b"".join(data)
 
     # Test arcname is required
-    with pytest.raises(ValueError, match="An arcname to store the data in is required"):
+    with pytest.raises(ValueError, match="A valid arcname .* is required"):
         zs.add(tostore, None)
-    with pytest.raises(ValueError, match="An arcname to store the data in is required"):
+    with pytest.raises(ValueError, match="A valid arcname .* is required"):
         zs.add(tostore, "")
     with pytest.raises(ValueError, match="Can't store .* as a directory"):
         zs.add(tostore, "directory/")
 
     zs.add(tostore, "data.bin")
     zf = _get_zip(zs)
 
@@ -633,14 +723,32 @@
 @pytest.mark.parametrize("data", [0, 1, object(), type(None)])
 def test_adding_invalid_data(data):
     zs = ZipStream()
     with pytest.raises(TypeError):
         zs.add(data, "test")
 
 
+@pytest.mark.parametrize("name", ["file", "directory/"])
+def test_adding_broken_symlinks(tmpdir, name):
+    """Test that adding a broken symlink will raise a FileNotFoundError"""
+
+    t = tmpdir.mkdir("top")
+    if not hasattr(t, "mksymlinkto"):
+        pytest.skip("mksymlinkto not supported - can't test broken links")
+
+    l = t.join(name)
+    l.mksymlinkto("nothing")
+
+    zs = ZipStream()
+    with pytest.raises(FileNotFoundError):
+        zs.add_path(l)
+    with pytest.raises(FileNotFoundError):
+        zs.add_path(t)
+
+
 @pytest.mark.parametrize("data", [
     ["strs", "cannot", "be", "added"],
     range(10),
     ZipStream,
 ])
 def test_adding_undetectable_invalid_data(data):
     """Test iterables that yield bad data are only detected at generation time"""
@@ -686,15 +794,15 @@
         else:
             assert x.is_dir()
             assert x.file_size == 0
             assert x.compress_size == 0
 
 
 def test_adding_missing_path(tmpdir):
-    with pytest.raises(ValueError):
+    with pytest.raises(FileNotFoundError):
         ZipStream.from_path(tmpdir.join("doesntexist"))
 
 
 def test_adding_deleted_path(tmpdir):
     zs = ZipStream(sized=True)
     f = tmpdir.join("file")
     f.write(b"this is some data")
@@ -713,14 +821,41 @@
     zs = ZipStream(sized=True)
     with pytest.raises(ValueError, match="No arcname for path"):
         zs.add_path(tmpdir)
     with pytest.raises(ValueError, match="No arcname for path"):
         zs.add_path(tmpdir, arcname="")
 
 
+def test_adding_null_byte_name():
+    zs = ZipStream(sized=True)
+
+    zs.add(b"data", "file.txt\x00and more")
+    with pytest.raises(ValueError, match="A valid arcname .* is required"):
+        zs.add(b"otherdata", "\x00nofilename")
+
+    zs.mkdir("directory\x00and more")
+    with pytest.raises(ValueError, match="A valid arcname .* is required"):
+        zs.mkdir("\x00nodirectory")
+
+    expected_len = len(zs)
+    data = bytes(zs)
+    assert len(data) == expected_len
+
+    zinfos = sorted(_get_zip(data).infolist(), key=lambda x: x.filename)
+    assert len(zinfos) == 2
+
+    assert zinfos[0].filename == "directory/"
+    assert zinfos[0].file_size == 0
+    assert zinfos[0].is_dir()
+
+    assert zinfos[1].filename == "file.txt"
+    assert zinfos[1].file_size == 4
+    assert not zinfos[1].is_dir()
+
+
 @pytest.mark.parametrize("data", [
     ("short text", "then longer text"),
     ("first longer text", "then shorter"),
 ])
 @pytest.mark.parametrize("sized", (True, False))
 def test_adding_changed_path(caplog, tmpdir, sized, data):
     caplog.set_level(logging.WARNING)
@@ -756,18 +891,63 @@
     zs = ZipStream(sized=sized)
     zs.add(_gen_rand(), "rand.txt", size=size)
 
     assert not caplog.text
     if sized and size is not None:
         with pytest.raises(RuntimeError, match="Error adding 'rand.txt' to sized ZipStream"):
             bytes(zs)
-        assert "Size mismatch when adding data for 'rand.txt'" in caplog.text
     else:
         bytes(zs)
-        assert "Size mismatch" not in caplog.text
+
+    # only emits a warning when size was specfied
+    assert (size is not None) == ("Size mismatch when adding data for 'rand.txt'" in caplog.text)
+
+
+def test_adding_iterator_invalid_size_underestimate_zip64(monkeypatch):
+    """Make sure that if an iterator size that doesn't require zip64 is given
+    and the data from it does, a RuntimeError is raised"""
+    monkeypatch.setattr(zipfile, "ZIP64_LIMIT", 100)
+    monkeypatch.setattr(zipstream.ng, "ZIP64_LIMIT", 100)
+
+    zs = ZipStream(sized=False)
+    zs.add(_gen_rand(), "rand.txt", size=1)
+
+    with pytest.raises(RuntimeError, match="Adding file 'rand.txt' unexpectedly required using Zip64 extensions"):
+        bytes(zs)
+
+
+def test_underestimate_zip64_via_compression(monkeypatch):
+    """Test that underestimating compresed size raises a RuntimeError"""
+
+    # compressed data can be bigger than uncompressed data. This generally only
+    # happens with small amounts of data but can with large amounts of data as
+    # well. This is less of a test and more of a demonstration of why the
+    # estimation factor is needed
+    monkeypatch.setattr(zipfile, "ZIP64_LIMIT", 10)
+    monkeypatch.setattr(zipstream.ng, "ZIP64_LIMIT", 10)
+
+    ZEROS = "0" * 10
+    NUMS = "0123456789"
+
+    def _make_zip(content):
+        zs = ZipStream(compress_type=zipfile.ZIP_DEFLATED)
+        zs.add(content, "file.txt")
+        bytes(zs)
+
+    assert len(ZEROS) == len(NUMS)
+
+    _make_zip(ZEROS)
+    _make_zip(NUMS)
+
+    # remove overestimation
+    monkeypatch.setattr(zipstream.ng, "ZIP64_ESTIMATE_FACTOR", 1)
+
+    _make_zip(ZEROS)
+    with pytest.raises(RuntimeError, match="Adding file 'file.txt' unexpectedly required using Zip64 extensions"):
+        _make_zip(NUMS)
 
 
 def test_adding_comment(caplog):
     caplog.set_level(logging.WARNING)
 
     zs = ZipStream()
     zs.comment = "test"
@@ -1107,29 +1287,36 @@
 
     with pytest.raises(TypeError):
         len(ZipStream(sized=False))
 
 
 @pytest.mark.parametrize("zip64", [False, True])
 @pytest.mark.parametrize("sized", [False, True])
-def test_proper_zip64_min_version(monkeypatch, zip64, sized):
-    """Ensure that the min version is set properly"""
+@pytest.mark.parametrize("known_size", [False, True])
+def test_proper_zip64_min_version(monkeypatch, zip64, sized, known_size):
+    """Ensure that the zip64 extensions are used when needed and the min
+    version is set accordingly
+    """
     if zip64:
         monkeypatch.setattr(zipfile, "ZIP64_LIMIT", 100)
         monkeypatch.setattr(zipstream.ng, "ZIP64_LIMIT", 100)
 
     zs = ZipStream(sized=sized)
-    zs.add(_gen_rand(), "rand.txt")
+    size = None if not known_size else len(b"".join(_gen_rand()))
+
+    zs.add(_gen_rand(), "rand.txt", size=size)
 
     zi = _get_zip(zs).infolist()[0]
-    # A sized zipstream will pull the entire iterator into memory and realize
-    # that zip64 is not required.
+    # A sized zipstream will always pull the entire iterator into memory and
+    # realize that zip64 is not required. Likewise if the size of the iterator
+    # is known.
     # An unsized zipstream will not pull it into memory and be forced to use
-    # zip64 extensions since the size could be too big
-    expected_version = (zipfile.DEFAULT_VERSION if sized and not zip64 else zipfile.ZIP64_VERSION)
+    # zip64 extensions if the size of the iterator is unknown since the size
+    # could be too big.
+    expected_version = (zipfile.DEFAULT_VERSION if not zip64 and (sized or known_size) else zipfile.ZIP64_VERSION)
 
     assert zi.create_version == expected_version
     assert zi.extract_version == expected_version
 
 
 @pytest.mark.parametrize("sized", [False, True])
 @pytest.mark.parametrize("known_size", [False, True])
@@ -1246,15 +1433,15 @@
     # check contents
     zf = _get_zip(data)
     assert len(zf.infolist()) == len(files)
     for f in files:
         _verify_zip_contains(zf, f)
 
 
-# Warning: skippped because it creates a 4GB+ temp file
+# Warning: skipped because it creates a 4GB+ temp file
 @pytest.mark.skip
 def test_zip64_real(tmpdir):
     """Test compressing a large file using Zip64 extensions works"""
     large_file = tmpdir.join("large.bin")
     zip_file = tmpdir.join("out.zip")
 
     # Generate a big empty file that requires Zip64 extensions to handle
```

### Comparing `zipstream-ng-1.5.0/zipstream/ng.py` & `zipstream-ng-1.6.0/zipstream/ng.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 """A modern and easy to use streamable zip file generator"""
 
 import collections
 import datetime
+import errno
 import functools
 import logging
 import os
 import stat
 import struct
 import sys
 import time
@@ -55,14 +56,16 @@
 
 
 __all__ = [
     # Defined classes
     "ZipStream", "ZipStreamInfo",
     # Compression constants (imported from zipfile)
     "ZIP_STORED", "ZIP_DEFLATED", "BZIP2_VERSION", "ZIP_BZIP2", "LZMA_VERSION", "ZIP_LZMA",
+    # Helper functions
+    "walk"
 ]
 
 __log__ = logging.getLogger(__name__)
 
 
 def _check_compression(compress_type, compress_level):
     """Check the specified compression type and level are valid"""
@@ -257,17 +260,21 @@
             compress_size = file_size
 
         # Update the CRC and filesize info
         self.CRC = crc
         self.file_size = file_size
         self.compress_size = compress_size
 
-        if not zip64 and max(file_size, compress_size) > ZIP64_LIMIT:  # pragma: no cover
+        if not zip64 and max(file_size, compress_size) > ZIP64_LIMIT:
             # Didn't estimate correctly :(
-            raise RuntimeError("Adding file unexpectedly required using Zip64")
+            raise RuntimeError(
+                "Adding file '{}' unexpectedly required using Zip64 extensions".format(
+                    self.filename
+                )
+            )
 
         # Yield the data descriptor with the now-valid CRC and file size info
         yield self.DataDescriptor(zip64)
 
     def _central_directory_header_data(self):
         """Yield a central directory file header for this file"""
         # Based on code in zipfile.ZipFile._write_end_record
@@ -408,39 +415,100 @@
             compress_level=compress_level,
             **kwargs
         )
 
     return wrapper
 
 
+def _sanitize_arcname(arcname):
+    """Terminate the arcname at the first null byte"""
+    # based on zipfile._sanitize_filename
+
+    if arcname:
+        # trim the arcname to the first null byte
+        null_byte = arcname.find(chr(0))
+        if null_byte >= 0:
+            arcname = arcname[:null_byte]
+
+    if not arcname:
+        raise ValueError(
+            "A valid arcname (name of the entry in the zip file) is required"
+        )
+
+    # Ensure paths in the zip always use forward slashes as the directory
+    # separator
+    for sep in PATH_SEPARATORS:
+        if sep != "/":
+            arcname = arcname.replace(sep, "/")
+
+    return arcname
+
+
 def _iter_file(path):
     """Yield data from a file"""
     with open(path, "rb") as fp:
         while True:
             buf = fp.read(READ_BUFFER)
             if not buf:
                 break
             yield buf
 
 
+def walk(path, preserve_empty=True, followlinks=True):
+    """Recursively walk the given the path and yield files/folders under it.
+
+    preserve_empty:
+        If True (the default), empty directories will be included in the
+        output. The paths of these directories will be yielded with a trailing
+        path separator.
+
+    followlinks:
+        If True (the default), symlinks to folders will be resolved and
+        followed unless this would result in infinite recursion (symlinks to
+        files are always resolved)
+    """
+
+    # Define a function to return the device and inode for a path.
+    # Will be used to deduplicate folders to avoid infinite recursion
+    def _getkey(path):
+        st = os.stat(path)
+        return (st.st_dev, st.st_ino)
+
+    visited = {_getkey(path)}
+    for dirpath, dirnames, files in os.walk(path, followlinks=followlinks):
+
+        if followlinks:
+            # Prevent infinite recursion by removing previously-visited
+            # directories from dirnames.
+            for i in reversed(range(len(dirnames))):
+                k = _getkey(os.path.join(dirpath, dirnames[i]))
+                if k in visited:
+                    dirnames.pop(i)
+                else:
+                    visited.add(k)
+
+        # Preserve empty directories
+        if preserve_empty and not files and not dirnames:
+            files = [""]
+
+        for f in files:
+            yield os.path.join(dirpath, f)
+
+
 class ZipStream:
     """A write-only zip that is generated from source files/data as it's
     iterated over.
 
     Ideal for situations where a zip file needs to be dynamically generated
     without using temporary files (ie: web applications).
     """
 
-    def __init__(self, *, comment=None, compress_type=ZIP_STORED, compress_level=None, sized=False):
+    def __init__(self, *, compress_type=ZIP_STORED, compress_level=None, sized=False):
         """Create a ZipStream
 
-        comment:
-            The comment to set on the ZipStream. This can be modified later by
-            setting the `.comment` property.
-
         compress_type:
             The ZIP compression method to use when writing the archive, and
             should be ZIP_STORED, ZIP_DEFLATED, ZIP_BZIP2 or ZIP_LZMA;
             unrecognized values will cause NotImplementedError to be raised. If
             ZIP_DEFLATED, ZIP_BZIP2 or ZIP_LZMA is specified but the
             corresponding module (zlib, bz2 or lzma) is not available,
             RuntimeError is raised. The default is ZIP_STORED.
@@ -491,16 +559,14 @@
         self._size_lock = threading.Lock()
 
         # For generating
         self._gen_lock = threading.Lock()
         self._pos = 0
         self._final = False
 
-        self.comment = comment
-
     def __iter__(self):
         """Generate zipped data from the added files/data"""
         return self.finalize()
 
     def __bool__(self):
         """A ZipStream is considered truthy if any files have been added to it"""
         return not self.is_empty()
@@ -568,99 +634,94 @@
         yield from self.footer()
 
     @_validate_final
     @_validate_compression
     def add_path(self, path, arcname=None, *, recurse=True, compress_type=None, compress_level=None):
         """Queue up a path to be added to the ZipStream
 
-        Queues the `path` up to to be written to the archive, giving it the name
-        provided by `arcname`. If `arcname` is not provided, it is assumed to be
-        the last component of the `path` (Ex: "/path/to/files/" --> "files").
-
-        If `recurse` is `True` (the default), and the `path` is a directory, all
-        files and folders under the `path` will be added to ZipStream. Symlinks
-        to files and folders will be resolved and followed unless this would
-        result in infinite recursion.
+        Queues the `path` up to to be written to the archive, giving it the
+        name provided by `arcname`. If `arcname` is not provided, it is assumed
+        to be the last component of the `path` (Ex: "/path/to/files/" -->
+        "files").
+
+        if `recurse` is `True` (the default), and the `path` is a directory,
+        all contents under the `path` will also be added. By default, this is
+        done using the `walk` function in this module, which will preserve
+        empty directories as well as follow symlinks to files and folders
+        unless this would result in infinite recursion.
+
+        If more control over directory walking is required, a function that
+        takes a `path` and returns an iterable of paths can also be passed in
+        as `recurse`. Alternatively, the directory can be walked in external
+        code while calling `add_path(path, arcname, recurse=False)` for each
+        discovered entry.
 
         If recurse is `False`, only the specified path (file or directory) will
         be added.
 
-        If more control over directory walking is required, walk the directory
-        normally and call `add_path(path, arcname, recurse=False)` for each
-        discovered path.
+        If given, `compress_type` and `compress_level` override the settings
+        the ZipStream was initialized with.
 
-        If given, `compress_type` and `compress_level` override the settings the
-        ZipStream was initialized with.
-
-        Raises a ValueError if the path does not exist or an arcname isn't
-        provided and the assumed one is empty.
+        Raises a FileNotFoundError if the path does not exist
+        Raises a ValueError if an arcname isn't provided and the assumed
+        one is empty.
         Raises a RuntimeError if the ZipStream has already been finalized.
         """
         # Resolve path objects to strings on Python 3.5
         if PY35_COMPAT and hasattr(path, "__fspath__"):  # pragma no cover
             path = path.__fspath__()
 
         if not os.path.exists(path):
-            raise ValueError("Path '{}' not found".format(path))
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
 
         path = os.path.normpath(path)
 
+        # special case - discover the arcname from the path
         if not arcname:
             arcname = os.path.basename(path)
             if not arcname:
                 raise ValueError(
                     "No arcname for path '{}' could be assumed".format(path)
                 )
+        arcname = _sanitize_arcname(arcname)
 
         # Not recursing - just add the path
         if not recurse or not os.path.isdir(path):
             self._enqueue(
                 path=path,
                 arcname=arcname,
                 compress_type=compress_type,
                 compress_level=compress_level
             )
             return
 
-        # Define a function to return the device and inode for a path.
-        # Will be used to deduplicate folders to avoid infinite recursion
-        def _getkey(path):
-            s = os.stat(path)
-            return (s.st_dev, s.st_ino)
-
-        visited = {_getkey(path)}
-        for dirpath, dirnames, files in os.walk(path, followlinks=True):
+        if recurse is True:
+            recurse = walk
 
-            # Prevent infinite recursion by removing previously-visited
-            # directories from dirnames.
-            for i in reversed(range(len(dirnames))):
-                k = _getkey(os.path.join(dirpath, dirnames[i]))
-                if k in visited:
-                    dirnames.pop(i)
-                else:
-                    visited.add(k)
+        for filepath in recurse(path):
+            filename = os.path.relpath(filepath, path)
+            filearcname = os.path.normpath(os.path.join(arcname, filename))
+
+            # Check if adding a directory, and if so, add a trailing slash
+            # (normpath will remove it). Also set the size since we're doing
+            # the stat anyway
+            st = os.stat(filepath)
+            if stat.S_ISDIR(st.st_mode):
+                filearcname += "/"
+                size = 0
+            else:
+                size = st.st_size
 
-            # Preserve empty directories
-            if not files and not dirnames:
-                files = [""]
-
-            for f in files:
-                filepath = os.path.join(dirpath, f)
-                filename = os.path.relpath(filepath, path)
-                filearcname = os.path.normpath(os.path.join(arcname, filename))
-                if not f:
-                    # adding an empty directory - make sure it has a trailing slash
-                    filearcname += "/"
-
-                self._enqueue(
-                    path=filepath,
-                    arcname=filearcname,
-                    compress_type=compress_type,
-                    compress_level=compress_level
-                )
+            self._enqueue(
+                path=filepath,
+                arcname=filearcname,
+                size=size,
+                compress_type=compress_type,
+                compress_level=compress_level
+            )
 
     @_validate_final
     @_validate_compression
     def add(self, data, arcname, *, size=None, compress_type=None, compress_level=None):
         """Queue up data to be added to the ZipStream
 
         `data` can be bytes, a string (encoded to bytes using utf-8), or any
@@ -671,32 +732,30 @@
         file or a directory)
 
         `arcname` (required) is the name of the file to store the data in. If
         any `data` is provided then the `arcname` cannot end with a "/" as this
         would create a directory (which can't contain content).
 
         `size` (optional) specifies the size of the `data` ONLY in the case
-        where it is an iterator and the ZipStream is sized. It is ignored in
-        all other cases.
+        where it is an iterator. It is ignored in all other cases.
 
         Note that the data provided will not be used until the file is actually
         encoded in the ZipStream. This means that strings and bytes will be held
         in memory and iterables will not be iterated over until then. For this
         reason it's a good idea to use `add_path()` wherever possible.
 
         If given, `compress_type` and `compress_level` override the settings the
         ZipStream was initialized with.
 
         Raises a ValueError if an arcname is not provided or ends with a "/"
         when data is given.
         Raises a TypeError if the data is not str, bytes, or an iterator.
         Raises a RuntimeError if the ZipStream has already been finalized.
         """
-        if not arcname:
-            raise ValueError("An arcname to store the data in is required")
+        arcname = _sanitize_arcname(arcname)
 
         if data is None:
             data = b""
         elif isinstance(data, str):
             data = data.encode("utf-8")
         elif isinstance(data, bytearray):
             # bytearrays are mutable - need to store a copy so it doesn't
@@ -717,26 +776,28 @@
             )
         elif hasattr(data, "__iter__"):
             if is_directory:
                 raise ValueError("Can't store an iterable as a directory")
 
             self._enqueue(
                 iterable=data,
-                size=size if self._sized else None,
+                size=size,
                 arcname=arcname,
                 compress_type=compress_type,
                 compress_level=compress_level,
             )
         else:
             raise TypeError(
                 "Data to add must be str, bytes, or an iterable of bytes"
             )
 
     def mkdir(self, arcname):
         """Create a directory inside the ZipStream"""
+        arcname = _sanitize_arcname(arcname)
+
         if arcname[-1] not in PATH_SEPARATORS:
             arcname += "/"
 
         self.add(data=None, arcname=arcname)
 
     @property
     def sized(self):
@@ -846,29 +907,34 @@
     def _enqueue(self, **kwargs):
         """Internal method to enqueue files, data, and iterables to be streamed"""
 
         path = kwargs.get("path")
         data = kwargs.get("data")
         size = kwargs.get("size")
 
+        if path:
+            st = os.stat(path)
+        else:
+            st = None
+
         # Get the modified time of the added path (use current time for
         # non-paths) and use it to update the last_modified property
-        mtime = time.localtime(os.stat(path).st_mtime if path else None)[0:6]
+        mtime = time.localtime(st.st_mtime if path else None)[0:6]
         if self._last_modified is None or self._last_modified < mtime:
             self._last_modified = mtime
 
         # Get the expected size of the data where not specified and possible
         if size is None:
             if data is not None:
                 kwargs["size"] = len(data)
             elif path is not None:
-                if os.path.isdir(path):
+                if stat.S_ISDIR(st.st_mode):
                     kwargs["size"] = 0
                 else:
-                    kwargs["size"] = os.path.getsize(path)
+                    kwargs["size"] = st.st_size
 
         # If the ZipStream is sized then it will look at what is being added and
         # queue up some information for _get_size to use to compute the total
         # length of the stream. It will also read any iterables fully into
         # memory so their size is known.
         if self._sized:
             if kwargs.get("compress_type"):
@@ -909,29 +975,31 @@
                 zinfo.external_attr = 0o40775 << 16  # drwxrwxr-x
                 zinfo.external_attr |= 0x10  # MS-DOS directory flag
             else:
                 zinfo.external_attr = 0o600 << 16  # ?rw-------
 
             if data is not None:
                 zinfo.file_size = len(data)
+            elif size is not None:
+                zinfo.file_size = size
 
         zinfo.compress_type = compress_type if compress_type is not None else self._compress_type
         if not PY36_COMPAT:
             if zinfo.compress_type in (ZIP_STORED, ZIP_LZMA):
                 # Make sure the zinfo properties are accurate for get_info
                 zinfo._compresslevel = None
             else:
                 zinfo._compresslevel = compress_level if compress_level is not None else self._compress_level
 
         # Store the position of the header
         zinfo.header_offset = self._pos
 
-        # We need to force using zip64 extensions for iterables since we don't
-        # know how big they'll end up being.
-        force_zip64 = bool(iterable)
+        # We need to force using zip64 extensions for unsized iterables since
+        # we don't know how big they'll end up being.
+        force_zip64 = bool(iterable) and size is None
 
         # Convert paths and data into iterables
         if path:
             if zinfo.is_dir():
                 iterable = None
             else:
                 iterable = _iter_file(path)
```

### Comparing `zipstream-ng-1.5.0/zipstream/server.py` & `zipstream-ng-1.6.0/zipstream/server.py`

 * *Files identical despite different names*

### Comparing `zipstream-ng-1.5.0/zipstream_ng.egg-info/PKG-INFO` & `zipstream-ng-1.6.0/zipstream_ng.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipstream-ng
-Version: 1.5.0
+Version: 1.6.0
 Summary: A modern and easy to use streamable zip file generator
 Home-page: https://github.com/pR0Ps/zipstream-ng
 License: LGPLv3
 Project-URL: Source, https://github.com/pR0Ps/zipstream-ng
 Project-URL: Changelog, https://github.com/pR0Ps/zipstream-ng/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -25,32 +25,45 @@
 zipstream-ng
 ============
 [![Status](https://github.com/pR0Ps/zipstream-ng/workflows/tests/badge.svg)](https://github.com/pR0Ps/zipstream-ng/actions/workflows/tests.yml)
 [![Version](https://img.shields.io/pypi/v/zipstream-ng.svg)](https://pypi.org/project/zipstream-ng/)
 ![Python](https://img.shields.io/pypi/pyversions/zipstream-ng.svg)
 
 A modern and easy to use streamable zip file generator. It can package and stream many files and
-folders on the fly without needing temporary files or excessive memory.
+folders into a zip on the fly without needing temporary files or excessive memory. It can also
+calculate the final size of the zip file before streaming it.
 
-Includes the ability to calculate the total size of the stream before any data is actually added
-(provided no compression is used). This makes it ideal for use in web applications since the total
-size can be used to set the `Content-Length` header without having to generate the entire file first
-(see examples below).
 
-Features:
+### Features:
  - Generates zip data on the fly as it's requested.
  - Can calculate the total size of the resulting zip file before generation even begins.
+ - Low memory usage: Since the zip is generated as it's requested, very little has to be kept in
+   memory (peak usage of less than 20MB is typical, even for TBs of files).
  - Flexible API: Typical use cases are simple, complicated ones are possible.
  - Supports zipping data from files, bytes, strings, and any other iterable objects.
- - Threadsafe: Won't mangle data if multiple threads concurrently add/read data to/from the same stream.
+ - Keeps track of the date of the most recently modified file added to the zip file.
+ - Threadsafe: Won't mangle data if multiple threads concurrently add data to the same stream.
  - Includes a clone of Python's `http.server` module with zip support added. Try `python -m zipstream.server`.
  - Automatically uses Zip64 extensions, but only if they are required.
  - No external dependencies.
 
 
+### Ideal for web backends:
+ - Generating zip data on the fly requires very little memory, no disk usage, and starts producing
+   data with less latency than creating the entire zip up-front. This means faster responses, no
+   temporary files, and very low memory usage.
+ - The ability to calculate the total size of the stream before any data is actually generated
+   (provided no compression is used) means web backends can provide a `Content-Length` header in
+   their responses. This allows clients to show a progress bar as the stream is transferred.
+ - By keeping track of the date of the most recently modified file added to the zip, web
+   backends can provide a `Last-Modified` header. This allows clients to check if they have the most
+   up-to-date version of the zip with just a HEAD request instead of having to download the entire
+   thing.
+
+
 Installation
 ------------
 ```
 pip install zipstream-ng
 ```
 
 
@@ -100,15 +113,15 @@
 zs.add(random_data(), "random.bin")
 
 # Add a file containing some static text.
 # Will automatically be encoded to bytes before being added (uses utf-8).
 zs.add("This is some text", "README.txt")
 
 # Write out the zip file as it's being generated.
-# At this point the data in the files files will be read in and the generator
+# At this point the data in the files will be read in and the generator
 # will be iterated over.
 with open("files.zip", "wb") as f:
     f.writelines(zs)
 ```
 
 
 ### zipserver (included)
```

