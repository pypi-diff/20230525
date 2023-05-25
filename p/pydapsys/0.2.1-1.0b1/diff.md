# Comparing `tmp/pydapsys-0.2.1.tar.gz` & `tmp/pydapsys-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydapsys-0.2.1.tar", max compression
+gzip compressed data, was "pydapsys-1.0b1.tar", max compression
```

## Comparing `pydapsys-0.2.1.tar` & `pydapsys-1.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1580 2023-03-10 18:58:03.069491 pydapsys-0.2.1/LICENSE
--rw-r--r--   0        0        0     5594 2023-05-25 11:33:00.536213 pydapsys-0.2.1/README.md
--rw-r--r--   0        0        0      138 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/__init__.py
--rw-r--r--   0        0        0    11093 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/binaryreader.py
--rw-r--r--   0        0        0     3573 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/file.py
--rw-r--r--   0        0        0     1100 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/neo_converters/__init__.py
--rw-r--r--   0        0        0     9404 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/neo_converters/helper.py
--rw-r--r--   0        0        0      335 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/neo_converters/interface.py
--rw-r--r--   0        0        0     5395 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/neo_converters/ni_pulse_stim.py
--rw-r--r--   0        0        0     1823 2023-03-08 10:13:49.890995 pydapsys-0.2.1/pydapsys/page.py
--rw-r--r--   0        0        0     4931 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/read.py
--rw-r--r--   0        0        0       70 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/toc/__init__.py
--rw-r--r--   0        0        0      970 2023-05-25 09:19:37.677766 pydapsys-0.2.1/pydapsys/toc/display.py
--rw-r--r--   0        0        0     4332 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/toc/entry.py
--rw-r--r--   0        0        0     1072 2023-05-25 11:33:00.537213 pydapsys-0.2.1/pydapsys/toc/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-31 15:29:24.391135 pydapsys-0.2.1/pydapsys/util/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 11:38:36.522282 pydapsys-0.2.1/pydapsys/util/floats.py
--rw-r--r--   0        0        0     3287 2023-05-25 11:38:36.523282 pydapsys-0.2.1/pydapsys/util/structs.py
--rw-r--r--   0        0        0      804 2023-05-25 11:38:36.523282 pydapsys-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6684 1970-01-01 00:00:00.000000 pydapsys-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1580 2023-03-10 18:58:03.069491 pydapsys-1.0b1/LICENSE
+-rw-r--r--   0        0        0     5604 2023-04-04 15:18:26.917594 pydapsys-1.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-02-01 10:54:52.662661 pydapsys-1.0b1/pydapsys/__init__.py
+-rw-r--r--   0        0        0    11074 2023-04-02 10:57:22.614984 pydapsys-1.0b1/pydapsys/binaryreader.py
+-rw-r--r--   0        0        0     3106 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/file.py
+-rw-r--r--   0        0        0        0 2023-01-31 09:49:52.052722 pydapsys-1.0b1/pydapsys/neo_convert/__init__.py
+-rw-r--r--   0        0        0     9705 2023-04-04 14:25:22.974192 pydapsys-1.0b1/pydapsys/neo_convert/abstract_converter.py
+-rw-r--r--   0        0        0     5316 2023-03-19 09:37:53.746926 pydapsys-1.0b1/pydapsys/neo_convert/ni_pulse_stim.py
+-rw-r--r--   0        0        0     1823 2023-03-08 10:13:49.890995 pydapsys-1.0b1/pydapsys/page.py
+-rw-r--r--   0        0        0     4926 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/read.py
+-rw-r--r--   0        0        0        0 2023-01-13 15:03:45.620258 pydapsys-1.0b1/pydapsys/toc/__init__.py
+-rw-r--r--   0        0        0      970 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/toc/display.py
+-rw-r--r--   0        0        0     4326 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/toc/entry.py
+-rw-r--r--   0        0        0     1072 2023-04-04 14:48:28.559904 pydapsys-1.0b1/pydapsys/toc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-01-31 15:29:24.391135 pydapsys-1.0b1/pydapsys/util/__init__.py
+-rw-r--r--   0        0        0      342 2023-01-31 15:35:28.305695 pydapsys-1.0b1/pydapsys/util/floats.py
+-rw-r--r--   0        0        0     3286 2023-04-04 13:35:15.855031 pydapsys-1.0b1/pydapsys/util/structs.py
+-rw-r--r--   0        0        0      803 2023-04-04 14:53:29.208657 pydapsys-1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 pydapsys-1.0b1/setup.py
+-rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 pydapsys-1.0b1/PKG-INFO
```

### Comparing `pydapsys-0.2.1/LICENSE` & `pydapsys-1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.1/README.md` & `pydapsys-1.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PyDapsys - Read DAPSYS recordings with Python
 
 [![PyPI](https://img.shields.io/pypi/v/pydapsys?style=for-the-badge)](https://pypi.org/project/pydapsys/)
 
 PyDapsys is a package to read neurography recordings made with [DAPSYS](http://dapsys.net/) (Data Acquisition Processor System). It is based on a reverse-engineered specification of the binary data format used by the latest DAPSYS version.
 
-Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastructures, from where they can be exported into various other formats.
+Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastrucutres, from where they can be exported into various other formats.
 
 ## Installation
 
 Either download the wheel file for offline installation or use pypi.
 
 ### Basic functionalities
 
@@ -31,33 +31,33 @@
 ### Quickstart
 
 A DAPSYS file is made up of two parts: A sequential list of blocks or **pages**, which store either a text with a timestamp or a waveform with associated timestamps, and a table of contents (toc). The toc consists of **folders** and **streams**. Each page has an id unique in the context of the file. Streams in the toc have an array of ids of the pages belonging to the stream. A stream is either a text stream (referring only to text pages) or a data stream (referring only to recording pages).
 
 #### Load a file
 Use `File.from_binary` to read from a BinaryIO object.
 ```python
-from pydapsys import read_file
+from pydapsys.file import File
 from pathlib import Path
 MY_DAPSYS_FILE = Path(".")/"to"/"my"/"dapsys_file.dps"
 with open(MY_DAPSYS_FILE, 'rb') as file:
-    file = read_file(file)
+    file = File.from_binary(file)
 ```
 The `File` object has two fields, the root of the table of contents and a dictionary mapping the page ids to their respective pages.
 ##### Inspect file structure
 To inspect the ToC structure of a loaded file, use the `structure` property of the toc `Root`, preferable together with `pprint`:
 ```python
 import pprint
 pprint.PrettyPrinter(indent=4).pprint(file.toc.structure)
 ```
 This will print the structure, names and types of all elements in the table of contents. For Streams, the number of associated pages it also printed after their type.
 #### Access data from a file
 To access data, use the `File.get_data` method. The method takes a path from the toc structure (WITHOUT THE NAME OF THE ROOT!) and will return all associated pages.
 Please note, that the path is  case insensitive
 ```python
-from pydapsys.toc import StreamType
+from pydapsys.toc.entry import StreamType
 my_texts = list(file.get_data("myrecording/my text stream", stype=StreamType.Text))
 my_waveforms = list(file.get_data("myrecording/somewhere else/ my waveform stream", stype=StreamType.Waveform))
 ```
 ##### Text pages
 
 A text page consists of three fields:
 
@@ -91,18 +91,18 @@
 
 ### NI Pulse stimulator
 
 Converter class for Dapsys recording created using an NI Pulse stimulator. Puts everything into one neo sequence. 
 Waveform pages of the continuous recording are merged if the difference between a pair of consecutive pages is less than a specified threshold (`grouping_tolerance`).
 
 ```python
-from pydapsys.neo_converters import NIPulseStimRecordingConverter
+from pydapsys.neo_convert.ni_pulse_stim import NIPulseStimulatorToNeo
 
 # convert a recording to a neo block
-neo_block = NIPulseStimRecordingConverter(file, grouping_tolerance=1e-9).to_neo()
+neo_block = NIPulseStimulatorToNeo(file, grouping_tolerance=1e-9).to_neo()
 ```
 
 #### Expected file structure
 
 {stim_folder} must be one of "NI Puls Stimulator", "pulse stimulator", "NI Pulse stimulator", but can be changed by adding entries to `NIPulseStimulatorToNeo.stim_foler_names`
 
 * Root
```

### Comparing `pydapsys-0.2.1/pydapsys/binaryreader.py` & `pydapsys-1.0b1/pydapsys/binaryreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,27 @@
         """
         Reads a number of binary values "null aware": The function will check if the read bytes for each value are unitized.
 
         Will read x values and compare each bytes with 'CD' * length of block. If the block is unitilized, the value will be set to None.
         Else the bytes will be unpacked.
         Example: To read 8 32-bit ints, the function will read 4 bytes 8 times. Each 4-byte block will be compared with 'CDCDCDCD'.
         If the comparison is true, the value will be set to None. Else it will unpack the bytes to an int.
-
         :param type_fmt: Type fmt string
         :param count: Number of values to read
         :return: Tuple containing the read objects
         """
         struct_str = self.byte_order + type_fmt
         data_size = calcsize(struct_str)
         null_bytes = bytes.fromhex('CD' * data_size)
         return tuple(unpack(struct_str, read_bytes)[0] if read_bytes != null_bytes else None for read_bytes in
                      (self.binio.read(data_size) for _ in range(count)))
 
     def _read_direct(self, type_fmt: str, count: int) -> Tuple:
         """
         Will read a number of values specified by the type fmt from a binary reader
-
         :param type_fmt: Type fmt string of the data to read
         :param count: number of values to read
         :return: Tuple containing the read values
         """
         struct_str = self.byte_order + type_fmt * count
         return unpack(struct_str, self.binio.read(calcsize(struct_str)))
 
@@ -72,15 +70,14 @@
         ...
 
     def read_tuple(self, type_fmt: str, count: int,
                    check_null: bool = False) -> Union[
         Tuple[float, ...], Tuple[int, ...], Tuple[Optional[float], ...], Tuple[Optional[int]]]:
         """
         Will read a tuple of values according to type_fmt.
-
         :param type_fmt: Type fmt string
         :param count: Number of values to read
         :param check_null: If the function should check if each function is unitilized according to visual C++ (0xCDCDCDCD)
         :return:Tuple containig the read data
         """
         read_func = self._read_nullaware if check_null else self._read_direct
         unpacked_values = read_func(type_fmt, count)
@@ -114,15 +111,14 @@
         ...
 
     def read_single(self, type_fmt: str,
                     check_null: bool = False) -> \
             Optional[Union[float, int]]:
         """
         Will read a single value according to type_fmt.
-
         :param type_fmt: Type fmt string
         :param check_null: If the function should check if each function is unitilized according to visual C++ (0xCDCDCDCD)
         :return:Tuple containig the read data
         """
         return self.read_tuple(type_fmt, 1, check_null=check_null)[0]
 
     @overload
@@ -132,15 +128,14 @@
     @overload
     def read_u32(self, check_null: Literal[True] = ...) -> Optional[int]:
         ...
 
     def read_u32(self, check_null=False) -> Optional[int]:
         """
         Will read a single u32 value
-
         :param check_null: Wether to check for null
         :return: An int or none.
         """
         return self.read_single('I', check_null=check_null)
 
     @overload
     def read_f32(self, check_null: Literal[False] = ...) -> float:
@@ -149,15 +144,14 @@
     @overload
     def read_f32(self, check_null: Literal[True] = ...) -> Optional[float]:
         ...
 
     def read_f32(self, check_null=False) -> Optional[float]:
         """
         Will read a single f32 value
-
         :param check_null: Wether to check for null
         :return: A float or none.
         """
         return self.read_single('f', check_null=check_null)
 
     @overload
     def read_f64(self, check_null: Literal[False] = ...) -> float:
@@ -166,15 +160,14 @@
     @overload
     def read_f64(self, check_null: Literal[True] = ...) -> Optional[float]:
         ...
 
     def read_f64(self, check_null=False) -> Optional[float]:
         """
         Will read a single f64 value
-
         :param check_null: Wether to check for null
         :return: A float or none.
         """
         return self.read_single('d', check_null=check_null)
 
     def read_ubyte(self) -> int:
         """
@@ -182,46 +175,42 @@
         :return: An integer representing the value of the read byte
         """
         return self.read_single('B', check_null=False)
 
     def read_ubytes(self, count: int) -> Tuple[int, ...]:
         """
         Reads the multiple bytes as usigned value
-
         :param count: Number of bytes to read
         :return: A tuple of integer values representing the individual usnigned values of the read bytes
         """
         return self.read_tuple('B', count, check_null=False)
 
     def skip(self, byte_count: int):
         if self.binio.seekable():
             self.binio.seek(byte_count, SEEK_CUR)
         else:
             self.binio.read(byte_count)
 
     def skip_32(self, count=1):
         """
         Advances the reader in 32-bit steps
-
         :param count: Number of 32-bit blocks to skip, defaults to 1
         """
         self.skip(4 * count)
 
     def skip_64(self, count=1):
         """
         Advances the reader in 64-bit steps
-
         :param count: Number of 64-bit blocks to skip, defaults to 1
         """
         self.skip(8 * count)
 
     def read_bool(self) -> bool:
         """
         Reads a dapsys bool (reads 1 byte, then skips 3 additional bytes)
-
         :return: Value of the read bool
         """
         v = self.binio.read(1)
         self.skip(3)
         return v != 0
 
     @overload
@@ -231,15 +220,14 @@
     @overload
     def read_array(self, type_fmt: FLOAT_STRUCTS) -> Tuple[float, ...]:
         ...
 
     def read_array(self, type_fmt: str) -> Union[Tuple[int, ...], Tuple[float, ...]]:
         """
         Reads an u32 value as x and then the following x values according to type fmt
-
         :param type_fmt: Type fmt of the values
         :return: Tuple containing x values
         """
         value_counts = self.read_u32()
         return self.read_tuple(type_fmt, count=value_counts, check_null=False, )
 
     def read_u32_array(self) -> Tuple[int, ...]:
@@ -248,65 +236,58 @@
         :return: Tuple containing x int values
         """
         return self.read_array('I')
 
     def read_f32_array(self) -> Tuple[float, ...]:
         """
         Reads a single u32 value as x and then the following x f32 values as an array
-
         :return: Tuple containing x float values
         """
         return self.read_array('f')
 
     def read_f64_array(self) -> Tuple[float, ...]:
         """
         Reads a single u32 value as x and then the following x f64 values as an array
-
         :return: Tuple containing x float values
         """
         return self.read_array('d')
 
     def read_str(self, encoding='latin_1') -> str:
         """
         Reads a single u32 value as x and then the following x bytes and decodes them as string
-
         :param encoding: Encoding to use when decoding the bytes, defaults to 'latin_1'
         :return: The decoded string
         """
         length = self.read_u32()
         str_bytes = self.binio.read(length)
         return str_bytes.decode(encoding=encoding)
 
     def _read_nparray(self, dtype: np.dtype) -> npt.NDArray:
         """
         Reads an u32 value as x and then uses numpy fromfile to read x following values of the specified type
-
         :param dtype: Dtype of the values to read
         :return: Numpy array containing the values read
         """
         value_counts = self.read_u32()
         raw_data = self.binio.read(value_counts * dtype.itemsize)
         return np.frombuffer(raw_data, dtype=dtype.newbyteorder(self.byte_order))
 
     def read_f32_nparray(self) -> npt.NDArray[np.float32]:
         """
         Reads an u32 value as x and then uses numpy fromfile to read x following f32 values of the specified type
-
         :return: Numpy array containing the read np.float32 values
         """
         return self._read_nparray(np.dtype(np.float32))
 
     def read_f64_nparray(self) -> npt.NDArray[np.float64]:
         """
         Reads an u32 value as x and then uses numpy fromfile to read x following f64 values of the specified type
-
         :return: Numpy array containing the read np.float64 values
         """
         return self._read_nparray(np.dtype(np.float64))
 
     def read_u32_nparray(self) -> npt.NDArray[np.uint32]:
         """
         Reads an u32 value as x and then uses numpy fromfile to read x following u32 values of the specified type
-
         :return: Numpy array containing the read np.uint32 values
         """
         return self._read_nparray(np.dtype(np.uint32))
```

### Comparing `pydapsys-0.2.1/pydapsys/file.py` & `pydapsys-1.0b1/pydapsys/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     def get_data(self, path: str, stype: Literal[StreamType.Waveform] = ...) -> Iterable[WaveformPage]:
         ...
 
     def get_data(self, path: str, stype: Optional[StreamType] = None) -> Union[
         Iterable[DataPage], Iterable[TextPage], Iterable[WaveformPage]]:
         """
         Yields all pages associated with the given stream path. To check for sanity, the expected stream type can be passed to the method.
-
         :param path: path of the stream in the table of contents (without the root node)
         :param stype: The expected type of the stream. If the stream is of a different type, the function will raise an exception. None by default.
         :return: An iterable of all pages associated with the stream
         """
         entry = self.toc.path(path)
         if not isinstance(entry, Stream):
             raise ToCEEntryIsNotAStreamError(element=path)
@@ -58,24 +57,13 @@
             raise ToCInvalidStreamTypeError(element=path, is_type=entry.stream_type.name, expected_type=stype.name)
         for pid in entry.page_ids:
             yield self.pages[pid]
 
     @staticmethod
     def from_binary(binio: BinaryIO, byte_order='<') -> File:
         """Reads a DAPSYS file from the given binary io object and directly constructs a new File class from it.
-
         :param binio: BinaryIO object to read from
         :param byte_order: byte order to use when reading from the binary io object. Defaults to little endian.
         :return: The File object constructed from the contents of the io stream
         """
         toc_root, pages = read_from(binio, byte_order=byte_order)
         return File(toc_root, pages)
-
-
-def read_file(binio: BinaryIO, byte_order='<') -> File:
-    """Reads a DAPSYS file from the given binary io object and directly constructs a new File class from it.
-
-    :param binio: BinaryIO object to read from
-    :param byte_order: byte order to use when reading from the binary io object. Defaults to little endian.
-    :return: The File object constructed from the contents of the io stream
-    """
-    return File.from_binary(binio, byte_order=byte_order)
```

### Comparing `pydapsys-0.2.1/pydapsys/neo_converters/helper.py` & `pydapsys-1.0b1/pydapsys/neo_convert/abstract_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,38 @@
+from abc import ABC, abstractmethod
 from typing import Sequence, Union, Optional, Iterable, List, Dict
 
 import neo
 import numpy as np
 import numpy.typing as npt
 import quantities as pq
 
 from pydapsys.file import File
 from pydapsys.page import DataPage, WaveformPage, TextPage, PageType
 from pydapsys.toc.entry import Stream, StreamType
 from pydapsys.util.floats import float_comp
 
 
-class DapsysToNeoHelper:
-    """ Converter to put various Dapsys streams neo structures
+class DapsysToNeoConverter(ABC):
+    """ Converter to put Dapsys recordings into the neo structure
+
+    This abstract base class provides common functionalities to transform Dapsys streams into common neo structures
+    :param file: PyDapsys dapsys file
     """
 
     def __init__(self, file: File):
-        """
-        Initialize helper for a file.
+        self.file = file
 
-        :param file: the file the helper reads from
+    @abstractmethod
+    def to_neo(self) -> neo.Block:
         """
-        self.file = file
+        Create a neo structure based on the given recording
+        :return: A neo block containing the data from the recording
+        """
+        ...
 
     def _get_datapage_typechecked(self, pid: int, ptype: PageType) -> DataPage:
         """
         gets the page with the given id and checks if it is of the requested type.
         Throws an exception if the type doesn't match
         """
         page = self.file.pages[pid]
@@ -46,15 +53,14 @@
         Primarily serves as a convenience function for type hinting.
         """
         return self._get_datapage_typechecked(pid, PageType.Waveform)
 
     def _pageids_to_event(self, page_ids: Union[Sequence[int], npt.NDArray[np.uint32]], name: str = "") -> neo.Event:
         """Converts data from a sequence (or numpy array) of page ids to a neo event.
         The labels will be taken from the page text and the event times from the first timestamp (timestamp_a)
-
         :param page_ids: Page ids of the comment pages
         :param name: name of the returned neo event
         :return: A neo event containing the text of the comment pages as labels and their first timestamps as times
         """
         times = np.empty(len(page_ids), dtype=np.float64)
         comments = []
         for i, page in enumerate(self.get_textpage(pid) for pid in page_ids):
@@ -93,57 +99,53 @@
             copy=False)
 
     def textstream_to_spiketrain(self, stream: Stream, t_stop: float, name: Optional[str] = None) -> neo.SpikeTrain:
         """Puts data from a text stream into a spike train. Requires an additional parameter t_stop for the equally named,
          required parameter on :class:`neo.SpikeTrain`. t_stop must be greater than the last timestamp of the train.
 
          The times of the spike train will be taken from the timestamp_a of the streams comment pages.
-
         :param stream: The stream to convert
         :param t_stop: t_stop parameter to set on :class:`neo.SpikeTrain`
         :param name: Name of the spike train. Will default to the name of the stream
         :return: A spike train build from the given text stream
         """
         if stream.stream_type != StreamType.Text:
             raise ValueError(f"StreamType.Text required for this operation, not {stream.stream_type.name}")
         return self._pageids_to_spiketrain(stream.page_ids, t_stop, name=stream.name if name is None else name)
 
     def _pageids_to_events_by_comment_text(self, page_ids: Union[Sequence[int], npt.NDArray[np.uint32]]) -> Iterable[
         neo.Event]:
         """Orders a number of comment pages by their text and emits one event for each unique text.
         The times are loaded from the comment pages timestamp_a, will have no labels and the name of the events will be
         the unique text.
-
         :param page_ids: Ids of the comment pages
         :return: An iterable of neo events
         """
         comment_string_to_timestamps: Dict[str, List[float]] = dict()
         for comment in (self.get_textpage(pid) for pid in page_ids):
             comment_string_to_timestamps.setdefault(comment.text, list()).append(comment.timestamp_a)
         for comment_string, comment_timestamps in comment_string_to_timestamps.items():
             yield neo.Event(times=np.array(comment_timestamps, dtype=np.float64), units=pq.second, name=comment_string,
                             copy=False)
 
     def textstream_to_events_by_comment_text(self, stream: Stream) -> Iterable[neo.Event]:
         """Orders the comment pages of a text stream by their text and emits one event for each unique text.
         The times are loaded from the comment pages timestamp_a, will have no labels and the name of the events will be
         the unique text.
-
         :param stream: A text stream to convert
         :return: An iterable of neo events
         """
         if stream.stream_type != StreamType.Text:
             raise ValueError(f"StreamType.Text required for this operation, not {stream.stream_type.name}")
         return self._pageids_to_events_by_comment_text(stream.page_ids)
 
     def _group_recordingsegments(self, rec_pages: Iterable[WaveformPage], tolerance: float = 1e-5) -> Iterable[
         List[WaveformPage]]:
         """Groups consecutive recording pages into lists, if the difference between the end of the last page and the start
-        of the next one is less than the threshold and they have the same sampling interval.
-
+        of the next one is less than the threshold and they have the same sampling interval
         :param rec_pages: Recording pages to group. Must be in orderly sequence.
         :param tolerance: Tolerance for grouping, defaults to 1e-5
         :return: An iterable of lists containing grouped recording pages
         """
         page_iter = iter(rec_pages)
         current_set: List[WaveformPage] = [next(page_iter)]
         for page in page_iter:
```

### Comparing `pydapsys-0.2.1/pydapsys/neo_converters/ni_pulse_stim.py` & `pydapsys-1.0b1/pydapsys/neo_convert/ni_pulse_stim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import datetime
 from typing import Optional, Iterable
 
 import neo
 
 from pydapsys.file import File
-from pydapsys.neo_converters.helper import DapsysToNeoHelper
-from pydapsys.neo_converters.interface import INeoConverter
+from pydapsys.neo_convert.abstract_converter import DapsysToNeoConverter
 from pydapsys.toc.entry import Folder, Stream, StreamType
 
 
-class NIPulseStimRecordingConverter(DapsysToNeoHelper, INeoConverter):
+class NIPulseStimulatorToNeo(DapsysToNeoConverter):
     """Converter class for Dapsys recording created using an NI Pulse stimulator. Puts everything into one neo sequence.
     Waveform pages of continuous recording are merged if the difference between a pair of consecutive pages is less than a specified threshold.
 
 
     Expected structure is:
 
     - Root
@@ -39,52 +38,48 @@
 
     @property
     def stimulator_folder(self) -> Folder:
         """
         Returns the folder of the stimulator.
 
         Looks in :attr:`self.file` for a folder with one of the keys of :attr:`self.stim_folder_names` and returns the first match
-
         :return:The folder object of the stimulator
         """
         candidates = self.file.toc.folders
         for stim_name in self.stim_foler_names:
             if stim_name in candidates:
                 return candidates[stim_name]
         raise Exception(f"Could not find a fitting stimulator name: {self.file.toc.children.keys()}")
 
     @property
     def comment_stream(self) -> Stream:
         """
         Returns the stream containing the comments of the recording (root/comments)
-
         :return: Comment stream
         """
         return self.file.toc.s["comments"]
 
     @property
     def track_textstreams(self) -> Iterable[Stream]:
         """
         Yields the streams containing sorted tracks
 
         Looks in root/[stimulator]/responses/tracks for all responses/ for any streams and returns them.
         root/[stimulator]/responses must exist, the function will silently ignore missing "tracks for all responses".
-
         :return: Streams containing sorted tracks
         """
         if "tracks for all responses" in self.stimulator_folder.f["responses"].folders:
             for pulse_stream in self.stimulator_folder.f["responses"].f["tracks for all responses"].streams.values():
                 if pulse_stream.stream_type == StreamType.Text:
                     yield pulse_stream
 
     def to_neo(self, block_name="DAPSYS recording", segment_name="Main segment",
                file_datetime: Optional[datetime] = None, rec_datetime: Optional[datetime] = None) -> neo.Block:
         """
         Attemps to read the data of the recording into a neo structure.
-        
         :param block_name: Name of the neo Block that will be returned
         :param segment_name: Name of the sole sequence contained in the block
         :param file_datetime: File datetime to set on the neo block and sequence. If none, will be set to unix-epoch 0
         :param rec_datetime: Recording datetime to set on the neo block and sequence. If none, will be set to unix-epoch 0
         :return: A neo block structured according to classdoc.
         """
         file_datetime = datetime.fromtimestamp(0) if file_datetime is None else file_datetime
```

### Comparing `pydapsys-0.2.1/pydapsys/page.py` & `pydapsys-1.0b1/pydapsys/page.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.1/pydapsys/read.py` & `pydapsys-1.0b1/pydapsys/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 class UnknownPageTypeError(BinaryElementTypeError):
     ...
 
 
 def _read_display_properties(file: DapsysBinaryReader) -> DisplayProperties:
     """
     Reads a block of display properties from a binary file
-
     :param file: Opened binary file to read from
     :return: The read plot config object
     """
     plot_type = PlotType(file.read_u32())
     hist_interval = file.read_f64()
     latency_unit = LatencyPlotUnit(file.read_u32())
     latency_reference = file.read_u32()
@@ -38,15 +37,14 @@
                              RGBA8(r=r, g=g, b=b, a=a),
                              hist_begin)
 
 
 def _read_toc_entry(file: DapsysBinaryReader) -> Entry:
     """
     Reads an entry from the table of contents. Children will be read recursively.
-
     :param file: Opened binary file to read from
     :return: The entry, populated with its children (if any)
     """
     entry_type = EntryType(file.read_u32())
     name = file.read_str()
     file.skip_32()
     entry_id = file.read_u32()
@@ -66,15 +64,14 @@
     else:
         raise UnknownEntryTypeError(f"Unhandled entry type {entry_type}")
 
 
 def _read_toc(file: DapsysBinaryReader) -> Root:
     """
     Reads the Root of the table of contents and recursively all further elements of it.
-
     :param file: Opened binary file to read from
     :return: The root of the ToC
     """
     root_name = file.read_str()
     file.skip_64()
     element_count = file.read_u32()
     children = {entry.name: entry for entry in
@@ -82,15 +79,14 @@
     footer = file.read_str()
     return Root(name=root_name, footer=footer, children=CaseInsensitiveDict.from_dict(children))
 
 
 def _read_page(file: DapsysBinaryReader) -> DataPage:
     """
     Reads a page. Dynamically creates either a text page or a recording page, depending on the read page type.
-
     :param file: Opened binary file to read from
     :return: A DataPage, either a TextPage or a RecordingPage, depending on the read page type
     """
     page_type = PageType(file.read_u32())
     page_id = file.read_u32()
     ref = file.read_u32(check_null=True)
     if page_type == PageType.Text:
@@ -107,15 +103,14 @@
                             interval=tail)
     else:
         raise UnknownPageTypeError(f"Unhandled page type {page_type}")
 
 
 def read_from(binio: BinaryIO, byte_order='<') -> Tuple[Root, Dict[int, DataPage]]:
     """Reads a DAPSYS file from a readable binaryio object
-
     :param binio:  binary io to read from
     :param byte_order: Byte order to use when reading
     :returns: A tuple containing the Root of the table of contents and a dictionary mapping the page ids to their respective pages
     """
     dapsys_io = DapsysBinaryReader(binio, byte_order=byte_order)
     dapsys_io.skip(0x30)
     page_count = dapsys_io.read_u32()
```

### Comparing `pydapsys-0.2.1/pydapsys/toc/display.py` & `pydapsys-1.0b1/pydapsys/toc/display.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.1/pydapsys/toc/entry.py` & `pydapsys-1.0b1/pydapsys/toc/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         d = dict()
         for v in self.children.values():
             d[v.name] = v.structure if isinstance(v, ChildContainer) else f"{v.stream_type.name};{len(v.page_ids)}"
         return d
 
     def path(self, path: str) -> Entry:
         """Returns the Entry from the given relative path.
-
         :param path: Relative path to the target entry
         :returns: the target entry
         """
         splits = path.split('/', 1)
         selected_entry = self[splits[0]]
         if len(splits) == 1:
             return selected_entry
@@ -107,16 +106,15 @@
     def entry_type(self) -> EntryType:
         return EntryType.Folder
 
 
 @dataclass
 class Root(ChildContainer):
     """The root of the table of contents. It differentiates from a :class:`pydapsys.toc.entry.Folder`,
-    as it does not have a ToC id and contains the footer string of the file.
-    """
+    as it does not have a ToC id and contains the footer string of the file."""
     name: str
     """name of the root"""
     footer: str
     """footer string. Usually contains the version and serial number of the Dapsys program the recording was created from"""
 
 
 class StreamType(IntEnum):
```

### Comparing `pydapsys-0.2.1/pydapsys/toc/exceptions.py` & `pydapsys-1.0b1/pydapsys/toc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.1/pydapsys/util/structs.py` & `pydapsys-1.0b1/pydapsys/util/structs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
     def transform_key(self, __k: str) -> str:
         return __k.lower()
 
     def select(self, selector: Callable[[str, _VT], bool]) -> CaseInsensitiveDictView[_VT]:
         """
         Returns a view of the dictionary only containing the items for which selector returned true
-
         :param selector: Function for selecting items that should be present in the dict view
         :return: A dict view
         """
         return CaseInsensitiveDictView(self, {k for k, v in self.items() if selector(k, v)})
 
 
 class CaseInsensitiveDictView(MutableMapping[str, _VT], Generic[_VT]):
```

### Comparing `pydapsys-0.2.1/pyproject.toml` & `pydapsys-1.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "pydapsys"
-version = "0.2.1"
+version = "1.0b1"
 description = "Read recordings made with DAPSYS"
 authors = ["Peter Konradi <codingchipmunk@posteo.net>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/Digital-C-Fiber/PyDapsys"
 keywords = ["microneurography", "dapsys", "neurophysiology", "electrophysiology"]
 classifiers = ["Development Status :: 4 - Beta",
-    "Intended Audience :: Developers", "Intended Audience :: Science/Research",
+    "Intended Audience :: Developers","Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3 :: Only",
-]
+    ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21"
-neo = { version = ">=0.12, <1", optional = true }
+neo = { version = "^0.11.1", optional = true }
 
 [tool.poetry.extras]
 neo = ["neo"]
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydapsys-0.2.1/PKG-INFO` & `pydapsys-1.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydapsys
-Version: 0.2.1
+Version: 1.0b1
 Summary: Read recordings made with DAPSYS
 Home-page: https://github.com/Digital-C-Fiber/PyDapsys
 License: BSD-3-Clause
 Keywords: microneurography,dapsys,neurophysiology,electrophysiology
 Author: Peter Konradi
 Author-email: codingchipmunk@posteo.net
 Requires-Python: >=3.8,<4.0
@@ -13,29 +13,28 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: neo
-Requires-Dist: neo (>=0.12,<1) ; extra == "neo"
+Requires-Dist: neo (>=0.11.1,<0.12.0); extra == "neo"
 Requires-Dist: numpy (>=1.21,<2.0)
 Project-URL: Repository, https://github.com/Digital-C-Fiber/PyDapsys
 Description-Content-Type: text/markdown
 
 # PyDapsys - Read DAPSYS recordings with Python
 
 [![PyPI](https://img.shields.io/pypi/v/pydapsys?style=for-the-badge)](https://pypi.org/project/pydapsys/)
 
 PyDapsys is a package to read neurography recordings made with [DAPSYS](http://dapsys.net/) (Data Acquisition Processor System). It is based on a reverse-engineered specification of the binary data format used by the latest DAPSYS version.
 
-Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastructures, from where they can be exported into various other formats.
+Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastrucutres, from where they can be exported into various other formats.
 
 ## Installation
 
 Either download the wheel file for offline installation or use pypi.
 
 ### Basic functionalities
 
@@ -58,33 +57,33 @@
 ### Quickstart
 
 A DAPSYS file is made up of two parts: A sequential list of blocks or **pages**, which store either a text with a timestamp or a waveform with associated timestamps, and a table of contents (toc). The toc consists of **folders** and **streams**. Each page has an id unique in the context of the file. Streams in the toc have an array of ids of the pages belonging to the stream. A stream is either a text stream (referring only to text pages) or a data stream (referring only to recording pages).
 
 #### Load a file
 Use `File.from_binary` to read from a BinaryIO object.
 ```python
-from pydapsys import read_file
+from pydapsys.file import File
 from pathlib import Path
 MY_DAPSYS_FILE = Path(".")/"to"/"my"/"dapsys_file.dps"
 with open(MY_DAPSYS_FILE, 'rb') as file:
-    file = read_file(file)
+    file = File.from_binary(file)
 ```
 The `File` object has two fields, the root of the table of contents and a dictionary mapping the page ids to their respective pages.
 ##### Inspect file structure
 To inspect the ToC structure of a loaded file, use the `structure` property of the toc `Root`, preferable together with `pprint`:
 ```python
 import pprint
 pprint.PrettyPrinter(indent=4).pprint(file.toc.structure)
 ```
 This will print the structure, names and types of all elements in the table of contents. For Streams, the number of associated pages it also printed after their type.
 #### Access data from a file
 To access data, use the `File.get_data` method. The method takes a path from the toc structure (WITHOUT THE NAME OF THE ROOT!) and will return all associated pages.
 Please note, that the path is  case insensitive
 ```python
-from pydapsys.toc import StreamType
+from pydapsys.toc.entry import StreamType
 my_texts = list(file.get_data("myrecording/my text stream", stype=StreamType.Text))
 my_waveforms = list(file.get_data("myrecording/somewhere else/ my waveform stream", stype=StreamType.Waveform))
 ```
 ##### Text pages
 
 A text page consists of three fields:
 
@@ -118,18 +117,18 @@
 
 ### NI Pulse stimulator
 
 Converter class for Dapsys recording created using an NI Pulse stimulator. Puts everything into one neo sequence. 
 Waveform pages of the continuous recording are merged if the difference between a pair of consecutive pages is less than a specified threshold (`grouping_tolerance`).
 
 ```python
-from pydapsys.neo_converters import NIPulseStimRecordingConverter
+from pydapsys.neo_convert.ni_pulse_stim import NIPulseStimulatorToNeo
 
 # convert a recording to a neo block
-neo_block = NIPulseStimRecordingConverter(file, grouping_tolerance=1e-9).to_neo()
+neo_block = NIPulseStimulatorToNeo(file, grouping_tolerance=1e-9).to_neo()
 ```
 
 #### Expected file structure
 
 {stim_folder} must be one of "NI Puls Stimulator", "pulse stimulator", "NI Pulse stimulator", but can be changed by adding entries to `NIPulseStimulatorToNeo.stim_foler_names`
 
 * Root
```

