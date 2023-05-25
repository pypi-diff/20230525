# Comparing `tmp/Adafruit_PureIO-1.1.8.tar.gz` & `tmp/Adafruit_PureIO-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Adafruit_PureIO-1.1.8.tar", last modified: Mon Dec  7 13:52:37 2020, max compression
+gzip compressed data, was "Adafruit_PureIO-1.1.9.tar", last modified: Mon Jun 14 15:03:08 2021, max compression
```

## Comparing `Adafruit_PureIO-1.1.8.tar` & `Adafruit_PureIO-1.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (116)     2668 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (116)     1415 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1467 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)      944 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      788 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    16166 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/Adafruit_PureIO/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15671 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO/smbus.py
--rw-r--r--   0 runner    (1001) docker     (116)    12558 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO/spi.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3469 2020-12-07 13:52:36.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      517 2020-12-07 13:52:37.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 13:52:36.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-12-07 13:52:36.000000 Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5987 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1115 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3469 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1944 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5356 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      842 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1916 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 13:52:37.404827 Adafruit_PureIO-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2020-12-07 13:52:22.000000 Adafruit_PureIO-1.1.8/tests/test_I2C.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.004585 Adafruit_PureIO-1.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.004585 Adafruit_PureIO-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    16166 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/Adafruit_PureIO/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15796 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO/smbus.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12432 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO/spi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-06-14 15:03:07.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2021-06-14 15:03:07.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-14 15:03:07.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-06-14 15:03:07.000000 Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5987 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5356 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 15:03:08.008585 Adafruit_PureIO-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2021-06-14 15:02:58.000000 Adafruit_PureIO-1.1.9/tests/test_I2C.py
```

### Comparing `Adafruit_PureIO-1.1.8/.github/ISSUE_TEMPLATE.md` & `Adafruit_PureIO-1.1.9/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/.github/PULL_REQUEST_TEMPLATE.md` & `Adafruit_PureIO-1.1.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/.github/workflows/build.yml` & `Adafruit_PureIO-1.1.9/.github/workflows/build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         path: actions-ci
     - name: Install dependencies
       # (e.g. - apt-get: gettext, etc; pip: circuitpython-build-tools, requirements.txt; etc.)
       run: |
         source actions-ci/install.sh
     - name: Pip install pylint, black, & Sphinx
       run: |
-        pip install --force-reinstall pylint black==19.10b0 Sphinx sphinx-rtd-theme
+        pip install --force-reinstall pylint black Sphinx sphinx-rtd-theme
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Check formatting
       run: |
         black --check --target-version=py35 .
     - name: PyLint
       run: |
```

### Comparing `Adafruit_PureIO-1.1.8/.github/workflows/release.yml` & `Adafruit_PureIO-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/.gitignore` & `Adafruit_PureIO-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/.pylintrc` & `Adafruit_PureIO-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/Adafruit_PureIO/smbus.py` & `Adafruit_PureIO-1.1.9/Adafruit_PureIO/smbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,17 @@
     def open(self, bus):
         """Open the smbus interface on the specified bus."""
         # Close the device if it's already open.
         if self._device is not None:
             self.close()
         # Try to open the file for the specified bus.  Must turn off buffering
         # or else Python 3 fails (see: https://bugs.python.org/issue20074)
+        # pylint: disable=consider-using-with
         self._device = open("/dev/i2c-{0}".format(bus), "r+b", buffering=0)
+        # pylint: enable=consider-using-with
         # TODO: Catch IOError and throw a better error message that describes
         # what's wrong (i.e. I2C may not be enabled or the bus doesn't exist).
 
     def close(self):
         """Close the smbus connection.  You cannot make any other function
         calls on the bus unless open is called!"""
         if self._device is not None:
@@ -281,15 +283,19 @@
         # just write a single byte that initiates a write to the specified device
         # address (but writes no data!).  The functionality is duplicated below
         # but the actual use case for this is unknown.
         assert (
             self._device is not None
         ), "Bus must be opened before operations are made against it!"
         # Build ioctl request.
-        request = make_i2c_rdwr_data([(addr, 0, 0, None),])  # Write with no data.
+        request = make_i2c_rdwr_data(
+            [
+                (addr, 0, 0, None),
+            ]
+        )  # Write with no data.
         # Make ioctl call and return result data.
         ioctl(self._device.fileno(), I2C_RDWR, request)
 
     def write_byte(self, addr, val):
         """Write a single byte to the specified device."""
         assert (
             self._device is not None
@@ -304,16 +310,15 @@
         assert (
             self._device is not None
         ), "Bus must be opened before operations are made against it!"
         self._select_device(addr)
         self._device.write(buf)
 
     def write_byte_data(self, addr, cmd, val):
-        """Write a byte of data to the specified cmd register of the device.
-        """
+        """Write a byte of data to the specified cmd register of the device."""
         assert (
             self._device is not None
         ), "Bus must be opened before operations are made against it!"
         # Construct a string of data to send with the command register and byte value.
         data = bytearray(2)
         data[0] = cmd & 0xFF
         data[1] = val & 0xFF
@@ -345,16 +350,15 @@
         # their length as the first byte.
         data = bytearray(len(vals) + 1)
         data[0] = len(vals) & 0xFF
         data[1:] = vals[0:]
         self.write_i2c_block_data(addr, cmd, data)
 
     def write_i2c_block_data(self, addr, cmd, vals):
-        """Write a buffer of data to the specified cmd register of the device.
-        """
+        """Write a buffer of data to the specified cmd register of the device."""
         assert (
             self._device is not None
         ), "Bus must be opened before operations are made against it!"
         # Construct a string of data to send, including room for the command register.
         data = bytearray(len(vals) + 1)
         data[0] = cmd & 0xFF  # Command register at the start.
         data[1:] = vals[0:]  # Copy in the block data (ugly but necessary to ensure
```

### Comparing `Adafruit_PureIO-1.1.8/Adafruit_PureIO/spi.py` & `Adafruit_PureIO-1.1.9/Adafruit_PureIO/spi.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,102 +221,92 @@
             return arg[0]
 
         arg = struct.pack("=" + structure, data)
         ioctl(self.handle, ioctl_bytes, arg)
         return None
 
     def _get_mode_field(self, field):
-        """Helper function to get specific spidev mode bits
-        """
+        """Helper function to get specific spidev mode bits"""
         return bool(self._ioctl(SPI._IOC_RD_MODE) & field)
 
     def _set_mode_field(self, field, value):
-        """Helper function to set a spidev mode bit
-        """
+        """Helper function to set a spidev mode bit"""
         mode = self._ioctl(SPI._IOC_RD_MODE)
         if value:
             mode |= field
         else:
             mode &= ~field
         self._ioctl(SPI._IOC_WR_MODE, mode)
 
     @property
     def phase(self):
-        """SPI clock phase bit
-        """
+        """SPI clock phase bit"""
         return self._get_mode_field(SPI_CPHA)
 
     @phase.setter
     def phase(self, phase):
         self._set_mode_field(SPI_CPHA, phase)
 
     @property
     def polarity(self):
-        """SPI polarity bit
-        """
+        """SPI polarity bit"""
         return self._get_mode_field(SPI_CPOL)
 
     @polarity.setter
     def polarity(self, polarity):
         self._set_mode_field(SPI_CPOL, polarity)
 
     @property
     def cs_high(self):
-        """SPI chip select active level
-        """
+        """SPI chip select active level"""
         return self._get_mode_field(SPI_CS_HIGH)
 
     @cs_high.setter
     def cs_high(self, cs_high):
         self._set_mode_field(SPI_CS_HIGH, cs_high)
 
     @property
     def lsb_first(self):
-        """Bit order of SPI word transfers
-        """
+        """Bit order of SPI word transfers"""
         return self._get_mode_field(SPI_LSB_FIRST)
 
     @lsb_first.setter
     def lsb_first(self, lsb_first):
         self._set_mode_field(SPI_LSB_FIRST, lsb_first)
 
     @property
     def three_wire(self):
-        """SPI 3-wire mode
-        """
+        """SPI 3-wire mode"""
         return self._get_mode_field(SPI_THREE_WIRE)
 
     @three_wire.setter
     def three_wire(self, three_wire):
         self._set_mode_field(SPI_THREE_WIRE, three_wire)
 
     @property
     def loop(self):
-        """SPI loopback mode
-        """
+        """SPI loopback mode"""
         return self._get_mode_field(SPI_LOOP)
 
     @loop.setter
     def loop(self, loop):
         self._set_mode_field(SPI_LOOP, loop)
 
     @property
     def no_cs(self):
-        """No chipselect. Single device on bus.
-        """
+        """No chipselect. Single device on bus."""
         return self._get_mode_field(SPI_NO_CS)
 
     @no_cs.setter
     def no_cs(self, no_cs):
         self._set_mode_field(SPI_NO_CS, no_cs)
 
     @property
     def ready(self):
-        """Slave pulls low to pause
-        """
+        """Slave pulls low to pause"""
         return self._get_mode_field(SPI_READY)
 
     @ready.setter
     def ready(self, ready):
         self._set_mode_field(SPI_READY, ready)
 
     @property
@@ -342,25 +332,23 @@
 
     @bits_per_word.setter
     def bits_per_word(self, bits_per_word):
         self._ioctl(SPI._IOC_WR_BITS_PER_WORD, bits_per_word)
 
     @property
     def mode(self):
-        """Mode that SPI is currently running in
-        """
+        """Mode that SPI is currently running in"""
         return self._ioctl(SPI._IOC_RD_MODE)
 
     @mode.setter
     def mode(self, mode):
         self._ioctl(SPI._IOC_WR_MODE, mode)
 
     def writebytes(self, data, max_speed_hz=0, bits_per_word=0, delay=0):
-        """Perform half-duplex SPI write.
-        """
+        """Perform half-duplex SPI write."""
         data = array.array("B", data).tobytes()
         # length = len(data)
         chunks = [
             data[i : i + self.chunk_size] for i in range(0, len(data), self.chunk_size)
         ]
         for chunk in chunks:
             length = len(chunk)
@@ -382,16 +370,15 @@
                 ioctl(self.handle, SPI._IOC_MESSAGE, spi_ioc_transfer)
             except TimeoutError as e:
                 raise Exception(
                     "ioctl timeout. Please try a different SPI frequency or less data."
                 ) from e
 
     def readbytes(self, length, max_speed_hz=0, bits_per_word=0, delay=0):
-        """Perform half-duplex SPI read as a binary string
-        """
+        """Perform half-duplex SPI read as a binary string"""
         receive_buffer = create_string_buffer(length)
         spi_ioc_transfer = struct.pack(
             SPI._IOC_TRANSFER_FORMAT,
             0,
             addressof(receive_buffer),
             length,
             max_speed_hz,
@@ -402,16 +389,15 @@
             0,
             0,
         )
         ioctl(self.handle, SPI._IOC_MESSAGE, spi_ioc_transfer)
         return string_at(receive_buffer, length)
 
     def transfer(self, data, max_speed_hz=0, bits_per_word=0, delay=0):
-        """Perform full-duplex SPI transfer
-        """
+        """Perform full-duplex SPI transfer"""
         data = array.array("B", data).tobytes()
         receive_data = []
 
         chunks = [
             data[i : i + self.chunk_size] for i in range(0, len(data), self.chunk_size)
         ]
         for chunk in chunks:
```

### Comparing `Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/PKG-INFO` & `Adafruit_PureIO-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Adafruit-PureIO
-Version: 1.1.8
+Name: Adafruit_PureIO
+Version: 1.1.9
 Summary: Pure python (i.e. no native extensions) access to Linux IO    including I2C and SPI. Drop in replacement for smbus and spidev modules.
 Home-page: https://github.com/adafruit/Adafruit_Python_PureIO
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `Adafruit_PureIO-1.1.8/Adafruit_PureIO.egg-info/SOURCES.txt` & `Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/CODE_OF_CONDUCT.md` & `Adafruit_PureIO-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/LICENSE` & `Adafruit_PureIO-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/PKG-INFO` & `Adafruit_PureIO-1.1.9/Adafruit_PureIO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Adafruit_PureIO
-Version: 1.1.8
+Name: Adafruit-PureIO
+Version: 1.1.9
 Summary: Pure python (i.e. no native extensions) access to Linux IO    including I2C and SPI. Drop in replacement for smbus and spidev modules.
 Home-page: https://github.com/adafruit/Adafruit_Python_PureIO
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `Adafruit_PureIO-1.1.8/README.rst` & `Adafruit_PureIO-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/docs/_static/favicon.ico` & `Adafruit_PureIO-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/docs/conf.py` & `Adafruit_PureIO-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/docs/index.rst` & `Adafruit_PureIO-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/setup.py` & `Adafruit_PureIO-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `Adafruit_PureIO-1.1.8/tests/test_I2C.py` & `Adafruit_PureIO-1.1.9/tests/test_I2C.py`

 * *Files identical despite different names*

