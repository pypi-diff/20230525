# Comparing `tmp/types-circuitpython-8.1.0rc0.tar.gz` & `tmp/types-circuitpython-8.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-circuitpython-8.1.0rc0.tar", last modified: Wed May 24 01:40:16 2023, max compression
+gzip compressed data, was "types-circuitpython-8.2.0b0.tar", last modified: Thu May 25 14:27:54 2023, max compression
```

## Comparing `types-circuitpython-8.1.0rc0.tar` & `types-circuitpython-8.2.0b0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.192585 types-circuitpython-8.1.0rc0/
--rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.1.0rc0/LICENSE
--rw-r--r--   0 timon      (501) staff       (20)     3860 2023-05-24 01:40:16.192232 types-circuitpython-8.1.0rc0/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-23 18:25:46.000000 types-circuitpython-8.1.0rc0/README.md
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.144021 types-circuitpython-8.1.0rc0/bindings/
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.145897 types-circuitpython-8.1.0rc0/bindings/__future__/
--rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-24 01:40:06.000000 types-circuitpython-8.1.0rc0/bindings/__future__/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.146202 types-circuitpython-8.1.0rc0/bindings/_bleio/
--rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_bleio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.146573 types-circuitpython-8.1.0rc0/bindings/_eve/
--rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_eve/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.146931 types-circuitpython-8.1.0rc0/bindings/_pew/
--rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_pew/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.147247 types-circuitpython-8.1.0rc0/bindings/_pixelmap/
--rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_pixelmap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.147555 types-circuitpython-8.1.0rc0/bindings/_stage/
--rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/_stage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.147854 types-circuitpython-8.1.0rc0/bindings/adafruit_bus_device/
--rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.148168 types-circuitpython-8.1.0rc0/bindings/adafruit_pixelbuf/
--rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.148486 types-circuitpython-8.1.0rc0/bindings/aesio/
--rw-r--r--   0 timon      (501) staff       (20)     2602 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/aesio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.148788 types-circuitpython-8.1.0rc0/bindings/alarm/
--rw-r--r--   0 timon      (501) staff       (20)     7021 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/alarm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.149096 types-circuitpython-8.1.0rc0/bindings/analogbufio/
--rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/analogbufio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.149412 types-circuitpython-8.1.0rc0/bindings/analogio/
--rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/analogio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.149731 types-circuitpython-8.1.0rc0/bindings/atexit/
--rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/atexit/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150041 types-circuitpython-8.1.0rc0/bindings/audiobusio/
--rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiobusio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150352 types-circuitpython-8.1.0rc0/bindings/audiocore/
--rw-r--r--   0 timon      (501) staff       (20)     4607 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiocore/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150657 types-circuitpython-8.1.0rc0/bindings/audioio/
--rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.150962 types-circuitpython-8.1.0rc0/bindings/audiomixer/
--rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiomixer/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.151274 types-circuitpython-8.1.0rc0/bindings/audiomp3/
--rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiomp3/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.151583 types-circuitpython-8.1.0rc0/bindings/audiopwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4448 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/audiopwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.151885 types-circuitpython-8.1.0rc0/bindings/bitbangio/
--rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/bitbangio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.152192 types-circuitpython-8.1.0rc0/bindings/bitmaptools/
--rw-r--r--   0 timon      (501) staff       (20)    13492 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/bitmaptools/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.152503 types-circuitpython-8.1.0rc0/bindings/bitops/
--rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/bitops/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.152800 types-circuitpython-8.1.0rc0/bindings/board/
--rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/board/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.153097 types-circuitpython-8.1.0rc0/bindings/busio/
--rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/busio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.153545 types-circuitpython-8.1.0rc0/bindings/camera/
--rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/camera/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.153998 types-circuitpython-8.1.0rc0/bindings/canio/
--rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/canio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.154558 types-circuitpython-8.1.0rc0/bindings/countio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/countio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.155128 types-circuitpython-8.1.0rc0/bindings/digitalio/
--rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/digitalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.155684 types-circuitpython-8.1.0rc0/bindings/displayio/
--rw-r--r--   0 timon      (501) staff       (20)    40361 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/displayio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.156365 types-circuitpython-8.1.0rc0/bindings/dualbank/
--rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/dualbank/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.156800 types-circuitpython-8.1.0rc0/bindings/floppyio/
--rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/floppyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.157205 types-circuitpython-8.1.0rc0/bindings/fontio/
--rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/fontio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.157808 types-circuitpython-8.1.0rc0/bindings/framebufferio/
--rw-r--r--   0 timon      (501) staff       (20)     3743 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/framebufferio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.158419 types-circuitpython-8.1.0rc0/bindings/frequencyio/
--rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-24 01:40:07.000000 types-circuitpython-8.1.0rc0/bindings/frequencyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.159003 types-circuitpython-8.1.0rc0/bindings/getpass/
--rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/getpass/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.159346 types-circuitpython-8.1.0rc0/bindings/gifio/
--rw-r--r--   0 timon      (501) staff       (20)     5691 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/gifio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.159690 types-circuitpython-8.1.0rc0/bindings/gnss/
--rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/gnss/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.160233 types-circuitpython-8.1.0rc0/bindings/hashlib/
--rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/hashlib/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.160852 types-circuitpython-8.1.0rc0/bindings/i2ctarget/
--rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/i2ctarget/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.161607 types-circuitpython-8.1.0rc0/bindings/imagecapture/
--rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/imagecapture/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.162309 types-circuitpython-8.1.0rc0/bindings/ipaddress/
--rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/ipaddress/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.163048 types-circuitpython-8.1.0rc0/bindings/is31fl3741/
--rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/is31fl3741/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.163845 types-circuitpython-8.1.0rc0/bindings/keypad/
--rw-r--r--   0 timon      (501) staff       (20)    13080 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/keypad/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.164674 types-circuitpython-8.1.0rc0/bindings/math/
--rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/math/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.165378 types-circuitpython-8.1.0rc0/bindings/mdns/
--rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/mdns/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.166235 types-circuitpython-8.1.0rc0/bindings/memorymap/
--rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/memorymap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.166853 types-circuitpython-8.1.0rc0/bindings/memorymonitor/
--rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/memorymonitor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.167517 types-circuitpython-8.1.0rc0/bindings/microcontroller/
--rw-r--r--   0 timon      (501) staff       (20)     6388 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/microcontroller/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.168136 types-circuitpython-8.1.0rc0/bindings/msgpack/
--rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/msgpack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.168713 types-circuitpython-8.1.0rc0/bindings/neopixel_write/
--rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/neopixel_write/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.169263 types-circuitpython-8.1.0rc0/bindings/nvm/
--rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/nvm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.169811 types-circuitpython-8.1.0rc0/bindings/onewireio/
--rw-r--r--   0 timon      (501) staff       (20)     1671 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/onewireio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.170389 types-circuitpython-8.1.0rc0/bindings/os/
--rw-r--r--   0 timon      (501) staff       (20)     3750 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/os/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.170961 types-circuitpython-8.1.0rc0/bindings/paralleldisplay/
--rw-r--r--   0 timon      (501) staff       (20)     2416 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.171520 types-circuitpython-8.1.0rc0/bindings/ps2io/
--rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/ps2io/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.172108 types-circuitpython-8.1.0rc0/bindings/pulseio/
--rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/pulseio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.172726 types-circuitpython-8.1.0rc0/bindings/pwmio/
--rw-r--r--   0 timon      (501) staff       (20)     5906 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/pwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.173317 types-circuitpython-8.1.0rc0/bindings/qrio/
--rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/qrio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.174270 types-circuitpython-8.1.0rc0/bindings/rainbowio/
--rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rainbowio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.175290 types-circuitpython-8.1.0rc0/bindings/random/
--rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/random/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.176109 types-circuitpython-8.1.0rc0/bindings/rgbmatrix/
--rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.176762 types-circuitpython-8.1.0rc0/bindings/rotaryio/
--rw-r--r--   0 timon      (501) staff       (20)     2660 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rotaryio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.177428 types-circuitpython-8.1.0rc0/bindings/rtc/
--rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/rtc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.178088 types-circuitpython-8.1.0rc0/bindings/sdcardio/
--rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/sdcardio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.178710 types-circuitpython-8.1.0rc0/bindings/sdioio/
--rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/sdioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.179349 types-circuitpython-8.1.0rc0/bindings/sharpdisplay/
--rw-r--r--   0 timon      (501) staff       (20)     1763 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.180000 types-circuitpython-8.1.0rc0/bindings/socketpool/
--rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/socketpool/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.180572 types-circuitpython-8.1.0rc0/bindings/ssl/
--rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/ssl/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.181147 types-circuitpython-8.1.0rc0/bindings/storage/
--rw-r--r--   0 timon      (501) staff       (20)     5949 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/storage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.181657 types-circuitpython-8.1.0rc0/bindings/struct/
--rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/struct/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.182206 types-circuitpython-8.1.0rc0/bindings/supervisor/
--rw-r--r--   0 timon      (501) staff       (20)    10934 2023-05-24 01:40:08.000000 types-circuitpython-8.1.0rc0/bindings/supervisor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.182748 types-circuitpython-8.1.0rc0/bindings/synthio/
--rw-r--r--   0 timon      (501) staff       (20)    14321 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/synthio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.183292 types-circuitpython-8.1.0rc0/bindings/terminalio/
--rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/terminalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.183807 types-circuitpython-8.1.0rc0/bindings/time/
--rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/time/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.184332 types-circuitpython-8.1.0rc0/bindings/touchio/
--rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/touchio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.184840 types-circuitpython-8.1.0rc0/bindings/traceback/
--rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/traceback/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.185356 types-circuitpython-8.1.0rc0/bindings/uheap/
--rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/uheap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.185894 types-circuitpython-8.1.0rc0/bindings/usb/
--rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.186444 types-circuitpython-8.1.0rc0/bindings/usb_cdc/
--rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_cdc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.186950 types-circuitpython-8.1.0rc0/bindings/usb_hid/
--rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_hid/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.187466 types-circuitpython-8.1.0rc0/bindings/usb_host/
--rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_host/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.188066 types-circuitpython-8.1.0rc0/bindings/usb_midi/
--rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/usb_midi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.188513 types-circuitpython-8.1.0rc0/bindings/ustack/
--rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/ustack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.188879 types-circuitpython-8.1.0rc0/bindings/vectorio/
--rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/vectorio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.189215 types-circuitpython-8.1.0rc0/bindings/watchdog/
--rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/watchdog/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.189555 types-circuitpython-8.1.0rc0/bindings/wifi/
--rw-r--r--   0 timon      (501) staff       (20)    10381 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/wifi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.189881 types-circuitpython-8.1.0rc0/bindings/zlib/
--rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/bindings/zlib/__init__.pyi
--rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.1.0rc0/pyproject.toml
--rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-24 01:40:16.192689 types-circuitpython-8.1.0rc0/setup.cfg
--rw-r--r--   0 timon      (501) staff       (20)     2179 2023-05-24 01:40:09.000000 types-circuitpython-8.1.0rc0/setup.py
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-24 01:40:16.191753 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/
--rw-r--r--   0 timon      (501) staff       (20)     3860 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/SOURCES.txt
--rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/dependency_links.txt
--rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/requires.txt
--rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-24 01:40:16.000000 types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/top_level.txt
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.413269 types-circuitpython-8.2.0b0/
+-rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.2.0b0/LICENSE
+-rw-r--r--   0 timon      (501) staff       (20)     2501 2023-05-25 14:27:54.412923 types-circuitpython-8.2.0b0/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     1444 2023-05-24 02:15:14.000000 types-circuitpython-8.2.0b0/README.md
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.357413 types-circuitpython-8.2.0b0/bindings/
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.360300 types-circuitpython-8.2.0b0/bindings/__future__/
+-rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/__future__/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.360628 types-circuitpython-8.2.0b0/bindings/_bleio/
+-rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/_bleio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.361793 types-circuitpython-8.2.0b0/bindings/_eve/
+-rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/_eve/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.362302 types-circuitpython-8.2.0b0/bindings/_pew/
+-rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/_pew/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.362745 types-circuitpython-8.2.0b0/bindings/_pixelmap/
+-rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/_pixelmap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.363139 types-circuitpython-8.2.0b0/bindings/_stage/
+-rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/_stage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.363583 types-circuitpython-8.2.0b0/bindings/adafruit_bus_device/
+-rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.363987 types-circuitpython-8.2.0b0/bindings/adafruit_pixelbuf/
+-rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.364395 types-circuitpython-8.2.0b0/bindings/aesio/
+-rw-r--r--   0 timon      (501) staff       (20)     2602 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/aesio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.364784 types-circuitpython-8.2.0b0/bindings/alarm/
+-rw-r--r--   0 timon      (501) staff       (20)     7021 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/alarm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.365125 types-circuitpython-8.2.0b0/bindings/analogbufio/
+-rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/analogbufio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.365433 types-circuitpython-8.2.0b0/bindings/analogio/
+-rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/analogio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.365746 types-circuitpython-8.2.0b0/bindings/atexit/
+-rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/atexit/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.366061 types-circuitpython-8.2.0b0/bindings/audiobusio/
+-rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/audiobusio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.366380 types-circuitpython-8.2.0b0/bindings/audiocore/
+-rw-r--r--   0 timon      (501) staff       (20)     4607 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/audiocore/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.366703 types-circuitpython-8.2.0b0/bindings/audioio/
+-rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/audioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.367007 types-circuitpython-8.2.0b0/bindings/audiomixer/
+-rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/audiomixer/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.367322 types-circuitpython-8.2.0b0/bindings/audiomp3/
+-rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/audiomp3/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.367623 types-circuitpython-8.2.0b0/bindings/audiopwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4448 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/audiopwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.367926 types-circuitpython-8.2.0b0/bindings/bitbangio/
+-rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/bitbangio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.368224 types-circuitpython-8.2.0b0/bindings/bitmaptools/
+-rw-r--r--   0 timon      (501) staff       (20)    13492 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/bitmaptools/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.368535 types-circuitpython-8.2.0b0/bindings/bitops/
+-rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/bitops/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.368847 types-circuitpython-8.2.0b0/bindings/board/
+-rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/board/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.369157 types-circuitpython-8.2.0b0/bindings/busio/
+-rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/busio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.369518 types-circuitpython-8.2.0b0/bindings/camera/
+-rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/camera/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.369816 types-circuitpython-8.2.0b0/bindings/canio/
+-rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/canio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.370135 types-circuitpython-8.2.0b0/bindings/countio/
+-rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/countio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.370443 types-circuitpython-8.2.0b0/bindings/digitalio/
+-rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/digitalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.370746 types-circuitpython-8.2.0b0/bindings/displayio/
+-rw-r--r--   0 timon      (501) staff       (20)    40361 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/displayio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.371128 types-circuitpython-8.2.0b0/bindings/dualbank/
+-rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/dualbank/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.371602 types-circuitpython-8.2.0b0/bindings/floppyio/
+-rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-25 14:27:48.000000 types-circuitpython-8.2.0b0/bindings/floppyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.372148 types-circuitpython-8.2.0b0/bindings/fontio/
+-rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/fontio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.373266 types-circuitpython-8.2.0b0/bindings/framebufferio/
+-rw-r--r--   0 timon      (501) staff       (20)     3743 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/framebufferio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.374324 types-circuitpython-8.2.0b0/bindings/frequencyio/
+-rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/frequencyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.375117 types-circuitpython-8.2.0b0/bindings/getpass/
+-rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/getpass/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.376349 types-circuitpython-8.2.0b0/bindings/gifio/
+-rw-r--r--   0 timon      (501) staff       (20)     5691 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/gifio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.377435 types-circuitpython-8.2.0b0/bindings/gnss/
+-rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/gnss/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.378569 types-circuitpython-8.2.0b0/bindings/hashlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/hashlib/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.379575 types-circuitpython-8.2.0b0/bindings/i2ctarget/
+-rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/i2ctarget/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.381401 types-circuitpython-8.2.0b0/bindings/imagecapture/
+-rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/imagecapture/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.382060 types-circuitpython-8.2.0b0/bindings/ipaddress/
+-rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/ipaddress/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.382735 types-circuitpython-8.2.0b0/bindings/is31fl3741/
+-rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/is31fl3741/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.383471 types-circuitpython-8.2.0b0/bindings/keypad/
+-rw-r--r--   0 timon      (501) staff       (20)    13080 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/keypad/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.384123 types-circuitpython-8.2.0b0/bindings/math/
+-rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/math/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.384699 types-circuitpython-8.2.0b0/bindings/mdns/
+-rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/mdns/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.385275 types-circuitpython-8.2.0b0/bindings/memorymap/
+-rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/memorymap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.385871 types-circuitpython-8.2.0b0/bindings/memorymonitor/
+-rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/memorymonitor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.386507 types-circuitpython-8.2.0b0/bindings/microcontroller/
+-rw-r--r--   0 timon      (501) staff       (20)     6388 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/microcontroller/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.387153 types-circuitpython-8.2.0b0/bindings/msgpack/
+-rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/msgpack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.387865 types-circuitpython-8.2.0b0/bindings/neopixel_write/
+-rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/neopixel_write/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.388530 types-circuitpython-8.2.0b0/bindings/nvm/
+-rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/nvm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.389126 types-circuitpython-8.2.0b0/bindings/onewireio/
+-rw-r--r--   0 timon      (501) staff       (20)     1671 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/onewireio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.389690 types-circuitpython-8.2.0b0/bindings/os/
+-rw-r--r--   0 timon      (501) staff       (20)     3750 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/os/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.390293 types-circuitpython-8.2.0b0/bindings/paralleldisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     2416 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.390928 types-circuitpython-8.2.0b0/bindings/ps2io/
+-rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/ps2io/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.391538 types-circuitpython-8.2.0b0/bindings/pulseio/
+-rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/pulseio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.392142 types-circuitpython-8.2.0b0/bindings/pwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     5906 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/pwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.392805 types-circuitpython-8.2.0b0/bindings/qrio/
+-rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/qrio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.393490 types-circuitpython-8.2.0b0/bindings/rainbowio/
+-rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/rainbowio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.394042 types-circuitpython-8.2.0b0/bindings/random/
+-rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/random/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.394600 types-circuitpython-8.2.0b0/bindings/rgbmatrix/
+-rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.395171 types-circuitpython-8.2.0b0/bindings/rotaryio/
+-rw-r--r--   0 timon      (501) staff       (20)     2660 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/rotaryio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.395751 types-circuitpython-8.2.0b0/bindings/rtc/
+-rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/rtc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.396313 types-circuitpython-8.2.0b0/bindings/sdcardio/
+-rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/sdcardio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.396896 types-circuitpython-8.2.0b0/bindings/sdioio/
+-rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/sdioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.397446 types-circuitpython-8.2.0b0/bindings/sharpdisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     1763 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.398002 types-circuitpython-8.2.0b0/bindings/socketpool/
+-rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/socketpool/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.398555 types-circuitpython-8.2.0b0/bindings/ssl/
+-rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/ssl/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.399074 types-circuitpython-8.2.0b0/bindings/storage/
+-rw-r--r--   0 timon      (501) staff       (20)     5949 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/storage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.399613 types-circuitpython-8.2.0b0/bindings/struct/
+-rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/struct/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.400178 types-circuitpython-8.2.0b0/bindings/supervisor/
+-rw-r--r--   0 timon      (501) staff       (20)    10934 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/supervisor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.400753 types-circuitpython-8.2.0b0/bindings/synthio/
+-rw-r--r--   0 timon      (501) staff       (20)    20705 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/synthio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.401365 types-circuitpython-8.2.0b0/bindings/terminalio/
+-rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-25 14:27:49.000000 types-circuitpython-8.2.0b0/bindings/terminalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.401896 types-circuitpython-8.2.0b0/bindings/time/
+-rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/time/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.402426 types-circuitpython-8.2.0b0/bindings/touchio/
+-rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/touchio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.403006 types-circuitpython-8.2.0b0/bindings/traceback/
+-rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/traceback/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.403559 types-circuitpython-8.2.0b0/bindings/uheap/
+-rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/uheap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.404066 types-circuitpython-8.2.0b0/bindings/usb/
+-rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/usb/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.404554 types-circuitpython-8.2.0b0/bindings/usb_cdc/
+-rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/usb_cdc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.405050 types-circuitpython-8.2.0b0/bindings/usb_hid/
+-rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/usb_hid/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.405608 types-circuitpython-8.2.0b0/bindings/usb_host/
+-rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/usb_host/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.406274 types-circuitpython-8.2.0b0/bindings/usb_midi/
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/usb_midi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.407013 types-circuitpython-8.2.0b0/bindings/ustack/
+-rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/ustack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.407750 types-circuitpython-8.2.0b0/bindings/vectorio/
+-rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/vectorio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.408549 types-circuitpython-8.2.0b0/bindings/watchdog/
+-rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/watchdog/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.409296 types-circuitpython-8.2.0b0/bindings/wifi/
+-rw-r--r--   0 timon      (501) staff       (20)    10381 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/wifi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.410093 types-circuitpython-8.2.0b0/bindings/zlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/bindings/zlib/__init__.pyi
+-rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.2.0b0/pyproject.toml
+-rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-25 14:27:54.413375 types-circuitpython-8.2.0b0/setup.cfg
+-rw-r--r--   0 timon      (501) staff       (20)     2181 2023-05-25 14:27:50.000000 types-circuitpython-8.2.0b0/setup.py
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-25 14:27:54.412501 types-circuitpython-8.2.0b0/types_circuitpython.egg-info/
+-rw-r--r--   0 timon      (501) staff       (20)     2501 2023-05-25 14:27:54.000000 types-circuitpython-8.2.0b0/types_circuitpython.egg-info/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-25 14:27:54.000000 types-circuitpython-8.2.0b0/types_circuitpython.egg-info/SOURCES.txt
+-rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-25 14:27:54.000000 types-circuitpython-8.2.0b0/types_circuitpython.egg-info/dependency_links.txt
+-rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-25 14:27:54.000000 types-circuitpython-8.2.0b0/types_circuitpython.egg-info/requires.txt
+-rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-25 14:27:54.000000 types-circuitpython-8.2.0b0/types_circuitpython.egg-info/top_level.txt
```

### Comparing `types-circuitpython-8.1.0rc0/LICENSE` & `types-circuitpython-8.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/__future__/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/__future__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/_bleio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/_eve/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/_pew/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/_pixelmap/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/_stage/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/adafruit_pixelbuf/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/aesio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/alarm/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/analogbufio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/analogio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/atexit/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/audiobusio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/audiocore/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/audioio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/audiomixer/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/audiomp3/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/audiopwmio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/bitbangio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/bitmaptools/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/bitops/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/board/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/busio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/camera/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/canio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/countio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/digitalio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/displayio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/dualbank/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/floppyio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/fontio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/framebufferio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/frequencyio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/getpass/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/gifio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/gnss/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/hashlib/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/i2ctarget/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/imagecapture/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/ipaddress/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/is31fl3741/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/keypad/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/math/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/mdns/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/memorymap/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/memorymonitor/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/microcontroller/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/msgpack/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/neopixel_write/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/nvm/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/onewireio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/os/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/paralleldisplay/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/ps2io/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/pulseio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/pwmio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/qrio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/random/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/rgbmatrix/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/rotaryio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/rtc/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/sdcardio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/sdioio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/sharpdisplay/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/socketpool/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/ssl/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/storage/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/struct/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/supervisor/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/synthio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/synthio/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Support for multi-channel audio synthesis
 
 At least 2 simultaneous notes are supported.  samd5x, mimxrt10xx and rp2040 platforms support up to 12 notes.
-
 """
 
 from __future__ import annotations
 
 import typing
-from typing import Optional, Sequence, Union
+from typing import List, Optional, Sequence, Union
 
 from circuitpython_typing import ReadableBuffer
 
+BlockInput = Union["Math", "LFO", float, None]
+"""Blocks and Notes can take any of these types as inputs on certain attributes
+
+A BlockInput can be any of the following types: `Math`, `LFO`, `builtins.float`, `None` (treated same as 0).
+"""
+
 class Envelope:
     def __init__(
         self,
         *,
         attack_time: Optional[float] = 0.1,
         decay_time: Optional[float] = 0.05,
         release_time: Optional[float] = 0.2,
@@ -81,33 +86,168 @@
             pass
           print("stopped")"""
     ...
 
 def midi_to_hz(midi_note: float) -> float:
     """Converts the given midi note (60 = middle C, 69 = concert A) to Hz"""
 
-def onevo_to_hz(ctrl: float) -> float:
+def voct_to_hz(ctrl: float) -> float:
     """Converts a 1v/octave signal to Hz.
 
-    60/12 (5.0) corresponds to middle C, 69/12 is concert A."""
+    24/12 (2.0) corresponds to middle C, 33/12 (2.75) is concert A."""
+
+class LFO:
+    """A low-frequency oscillator block
+
+    Every `rate` seconds, the output of the LFO cycles through its `waveform`.
+    The output at any particular moment is ``waveform[idx] * scale + offset``.
+
+    If `waveform` is None, a triangle waveform is used.
+
+    `rate`, `phase_offset`, `offset`, `scale`, and `once` can be changed at run-time. `waveform` may be mutated.
+
+    `waveform` must be a ``ReadableBuffer`` with elements of type ``'h'``
+    (16-bit signed integer).  Internally, the elements of `waveform` are scaled
+    so that the input range ``[-32768,32767]`` maps to ``[-1.0, 0.99996]``.
+
+    An LFO only updates if it is actually associated with a playing `Synthesizer`,
+    including indirectly via a `Note` or another intermediate LFO.
+
+    Using the same LFO as an input to multiple other LFOs or Notes is OK, but
+    the result if an LFO is tied to multiple Synthtesizer objects is undefined.
+
+    In the current implementation, LFOs are updated every 256 samples. This
+    should be considered an implementation detail, though it affects how LFOs
+    behave for instance when used to implement an integrator (``l.offset = l``).
+    """
+
+    def __init__(
+        self,
+        waveform: ReadableBuffer = None,
+        *,
+        rate: BlockInput = 1.0,
+        scale: BlockInput = 1.0,
+        offset: BlockInput = 0.0,
+        phase_offset: BlockInput = 0.0,
+        once=False,
+        interpolate=True,
+    ):
+        pass
+    waveform: Optional[ReadableBuffer]
+    """The waveform of this lfo. (read-only, but the values in the buffer may be modified dynamically)"""
+    rate: BlockInput
+    """The rate (in Hz) at which the LFO cycles through its waveform"""
+    offset: BlockInput
+    """An additive value applied to the LFO's output"""
+    phase_offset: BlockInput
+    """An additive value applied to the LFO's phase"""
+    scale: BlockInput
+    """An multiplier value applied to the LFO's output"""
+
+    once: bool
+    """True if the waveform should stop when it reaches its last output value, false if it should re-start at the beginning of its waveform
+
+    This applies to the ``phase`` *before* the addition of any ``phase_offset`` """
+
+    interpolate: bool
+    """True if the waveform should perform linear interpolation between values"""
+
+    phase: float
+    """The phase of the oscillator, in the range 0 to 1 (read-only)"""
+
+    value: float
+    """The value of the oscillator (read-only)"""
+
+    def retrigger(self):
+        """Reset the LFO's internal index to the start of the waveform. Most useful when it its `once` property is `True`."""
+
+class MathOperation:
+    """Operation for a Math block"""
+
+    def __call__(self, a: BlockInput, b: BlockInput = 0.0, c: BlockInput = 1.0) -> Math:
+        """A MathOperation enumeration value can be called to construct a Math block that performs that operation"""
+    SUM: "MathOperation"
+    """Computes ``a+b+c``. For 2-input sum, set one argument to ``0.0``. To hold a control value for multiple subscribers, set two arguments to ``0.0``."""
+
+    ADD_SUB: "MathOperation"
+    """Computes ``a+b-c``. For 2-input subtraction, set ``b`` to ``0.0``."""
+
+    PRODUCT: "MathOperation"
+    """Computes ``a*b*c``. For 2-input product, set one argument to ``1.0``."""
+
+    MUL_DIV: "MathOperation"
+    """Computes ``a*b/c``. If ``c`` is zero, the output is ``1.0``."""
 
-class BendMode:
-    """Controls the way the ``Note.pitch_bend_depth`` and ``Note.pitch_bend_rate`` properties are interpreted."""
+    SCALE_OFFSET: "MathOperation"
+    """Computes ``(a*b)+c``."""
 
-    STATIC: "BendMode"
-    """The Note's pitch is modified by its ``pitch_bend_depth``. ``pitch_bend_rate`` is ignored."""
+    OFFSET_SCALE: "MathOperation"
+    """Computes ``(a+b)*c``. For 2-input multiplication, set ``b`` to 0."""
 
-    VIBRATO: "BendMode"
-    """The Note's pitch varies by ``±pitch_bend_depth`` at a rate of ``pitch_bend_rate`` Hz."""
+    LERP: "MathOperation"
+    """Computes ``a * (1-c) + b * c``."""
 
-    SWEEP: "BendMode"
-    """The Note's pitch starts at ``Note.frequency`` then sweeps up or down by ``pitch_bend_depth`` over ``1/pitch_bend_rate`` seconds."""
+    CONSTRAINED_LERP: "MathOperation"
+    """Computes ``a * (1-c') + b * c'``, where ``c'`` is constrained to be between ``0.0`` and ``1.0``."""
 
-    SWEEP_IN: "BendMode"
-    """The Note's pitch sweep is the reverse of ``SWEEP`` mode, starting at the bent pitch and arriving at the tuned pitch."""
+    DIV_ADD: "MathOperation"
+    """Computes ``a/b+c``.  If ``b`` is zero, the output is ``c``."""
+
+    ADD_DIV: "MathOperation"
+    """Computes ``(a+b)/c``.  For 2-input product, set ``b`` to ``0.0``."""
+
+    MID: "MathOperation"
+    """Returns the middle of the 3 input values."""
+
+    MAX: "MathOperation"
+    """Returns the biggest of the 3 input values."""
+
+    MIN: "MathOperation"
+    """Returns the smallest of the 3 input values."""
+
+    ABS: "MathOperation"
+    """Returns the absolute value of ``a``."""
+
+class Math:
+    """An arithmetic block
+
+    Performs an arithmetic operation on up to 3 inputs. See the
+    documentation of ``MathOperation`` for the specific functions available.
+
+    The properties can all be changed at run-time.
+
+    An Math only updates if it is actually associated with a playing `Synthesizer`,
+    including indirectly via a `Note` or another intermediate Math.
+
+    Using the same Math as an input to multiple other Maths or Notes is OK, but
+    the result if an Math is tied to multiple Synthtesizer objects is undefined.
+
+    In the current implementation, Maths are updated every 256 samples. This
+    should be considered an implementation detail.
+    """
+
+    def __init__(
+        self,
+        operation: MathOperation,
+        a: BlockInput,
+        b: BlockInput = 0.0,
+        c: BlockInput = 1.0,
+    ):
+        pass
+    a: BlockInput
+    """The first input to the operation"""
+    b: BlockInput
+    """The second input to the operation"""
+    c: BlockInput
+    """The third input to the operation"""
+    operation: MathOperation
+    """The function to compute"""
+
+    value: float
+    """The value of the oscillator (read-only)"""
 
 class MidiTrack:
     """Simple MIDI synth"""
 
     def __init__(
         self,
         buffer: ReadableBuffer,
@@ -160,87 +300,96 @@
     """Offset, in bytes within the midi data, of a decoding error"""
 
 class Note:
     def __init__(
         self,
         *,
         frequency: float,
-        panning: float = 0.0,
+        panning: BlockInput = 0.0,
         waveform: Optional[ReadableBuffer] = None,
         envelope: Optional[Envelope] = None,
-        tremolo_depth: float = 0.0,
-        tremolo_rate: float = 0.0,
-        bend_depth: float = 0.0,
-        bend_rate: float = 0.0,
-        bend_mode: "BendMode" = BendMode.VIBRATO,
+        amplitude: BlockInput = 0.0,
+        bend: BlockInput = 0.0,
+        ring_frequency: float = 0.0,
+        ring_bend: float = 0.0,
+        ring_waveform: Optional[ReadableBuffer] = 0.0,
     ) -> None:
         """Construct a Note object, with a frequency in Hz, and optional panning, waveform, envelope, tremolo (volume change) and bend (frequency change).
 
         If waveform or envelope are `None` the synthesizer object's default waveform or envelope are used.
 
         If the same Note object is played on multiple Synthesizer objects, the result is undefined.
         """
     frequency: float
     """The base frequency of the note, in Hz."""
     filter: bool
     """True if the note should be processed via the synthesizer's FIR filter."""
-    panning: float
+    panning: BlockInput
     """Defines the channel(s) in which the note appears.
 
     -1 is left channel only, 0 is both channels, and 1 is right channel.
     For fractional values, the note plays at full amplitude in one channel
     and partial amplitude in the other channel. For instance -.5 plays at full
     amplitude in the left channel and 1/2 amplitude in the right channel."""
-    tremolo_depth: float
-    """The tremolo depth of the note, from 0 to 1
+    amplitude: BlockInput
+    """The relative amplitude of the note, from 0 to 1
 
-    A depth of 0 disables tremolo. A nonzero value enables tremolo,
-    with the maximum decrease in amplitude being equal to the tremolo
-    depth. A note with a tremolo depth of 1 will fade out to nothing, while
-    a tremolo depth of 0.1 will give a minimum amplitude of 0.9."""
-    tremolo_rate: float
-    """The tremolo rate of the note, in Hz."""
+    An amplitude of 0 makes the note inaudible. It is combined multiplicatively with
+    the value from the note's envelope.
 
-    bend_mode: BendMode
-    """The type of bend operation"""
+    To achieve a tremolo effect, attach an LFO here."""
 
-    bend_depth: float
-    """The bend depth of the note, from -1 to +1
+    bend: BlockInput
+    """The pitch bend depth of the note, from -12 to +12
 
-    A depth of 0 disables bend. A depth of 1 corresponds to a bend of 1
-    octave.  A depth of (1/12) = 0.833 corresponds to a bend of 1 semitone,
+    A depth of 0 plays the programmed frequency. A depth of 1 corresponds to a bend of 1
+    octave.  A depth of (1/12) = 0.0833 corresponds to a bend of 1 semitone,
     and a depth of .00833 corresponds to one musical cent.
+
+    To achieve a vibrato or sweep effect, attach an LFO here.
     """
-    bend_rate: float
-    """The bend rate of the note, in Hz."""
     waveform: Optional[ReadableBuffer]
     """The waveform of this note. Setting the waveform to a buffer of a different size resets the note's phase."""
     envelope: Envelope
     """The envelope of this note"""
 
     ring_frequency: float
     """The ring frequency of the note, in Hz. Zero disables.
 
     For ring to take effect, both ``ring_frequency`` and ``ring_waveform`` must be set."""
+    ring_bend: float
+    """The pitch bend depth of the note's ring waveform, from -12 to +12
+
+    A depth of 0 plays the programmed frequency. A depth of 1 corresponds to a bend of 1
+    octave.  A depth of (1/12) = 0.0833 corresponds to a bend of 1 semitone,
+    and a depth of .00833 corresponds to one musical cent.
+
+    To achieve a vibrato or sweep effect on the ring waveform, attach an LFO here.
+    """
     ring_waveform: Optional[ReadableBuffer]
     """The ring waveform of this note. Setting the ring_waveform to a buffer of a different size resets the note's phase.
 
     For ring to take effect, both ``ring_frequency`` and ``ring_waveform`` must be set."""
 
 NoteSequence = Sequence[Union[int, Note]]
-"""A sequence of notes, which can each be integer MIDI notes or `Note` objects"""
+"""A sequence of notes, which can each be integer MIDI note numbers or `Note` objects"""
+NoteOrNoteSequence = Union[int, Note, NoteSequence]
+"""A note or sequence of notes"""
+LFOOrLFOSequence = Union["LFO", Sequence["LFO"]]
+"""An LFO or a sequence of LFOs"""
 
 class Synthesizer:
     def __init__(
         self,
         *,
         sample_rate: int = 11025,
         channel_count: int = 1,
         waveform: Optional[ReadableBuffer] = None,
         envelope: Optional[Envelope] = None,
+        filter: Optional[ReadableBuffer] = None,
     ) -> None:
         """Create a synthesizer object.
 
         This API is experimental.
 
         Integer notes use MIDI note numbering, with 60 being C4 or Middle C,
         approximately 262Hz. Integer notes use the given waveform & envelope,
@@ -248,47 +397,58 @@
 
         :param int sample_rate: The desired playback sample rate; higher sample rate requires more memory
         :param int channel_count: The number of output channels (1=mono, 2=stereo)
         :param ReadableBuffer waveform: A single-cycle waveform. Default is a 50% duty cycle square wave. If specified, must be a ReadableBuffer of type 'h' (signed 16 bit)
         :param ReadableBuffer filter: Coefficients of an FIR filter to apply to notes with ``filter=True``. If specified, must be a ReadableBuffer of type 'h' (signed 16 bit)
         :param Optional[Envelope] envelope: An object that defines the loudness of a note over time. The default envelope, `None` provides no ramping, voices turn instantly on and off.
         """
-    def press(self, /, press: NoteSequence = ()) -> None:
+    def press(self, /, press: NoteOrNoteSequence = ()) -> None:
         """Turn some notes on.
 
         Pressing a note that was already pressed has no effect.
 
-        :param NoteSequence press: Any sequence of notes."""
-    def release(self, /, release: NoteSequence = ()) -> None:
+        :param NoteOrNoteSequence press: Any sequence of notes."""
+    def release(self, /, release: NoteOrNoteSequence = ()) -> None:
         """Turn some notes off.
 
         Releasing a note that was already released has no effect.
 
-        :param NoteSequence release: Any sequence of notes."""
-    def release_then_press(
-        self, release: NoteSequence = (), press: NoteSequence = ()
+        :param NoteOrNoteSequence release: Any sequence of notes."""
+    def change(
+        self,
+        release: NoteOrNoteSequence = (),
+        press: NoteOrNoteSequence = (),
+        retrigger=LFOOrLFOSequence,
     ) -> None:
-        """Turn some notes on and/or off.
+        """Start notes, stop them, and/or re-trigger some LFOs.
 
-        It is OK to release note that was not actually turned on.
-
-        Pressing a note that was already pressed has no effect.
+        The changes all happen atomically with respect to output generation.
 
-        Releasing and pressing the note again has little effect, but does reset the phase
-        of the note, which may be perceptible as a small glitch.
+        It is OK to release note that was not actually turned on.
 
-        :param NoteSequence release: Any sequence of notes.
-        :param NoteSequence press: Any sequence of notes."""
-    def release_all_then_press(self, /, press: NoteSequence) -> None:
+        Pressing a note that was already pressed returns it to the attack phase
+        but without resetting its amplitude. Releasing a note and immediately
+        pressing it again returns it to the attack phase with an initial
+        amplitude of 0.
+
+        At the same time, the passed LFOs (if any) are retriggered.
+
+        :param NoteOrNoteSequence release: Any sequence of notes.
+        :param NoteOrNoteSequence press: Any sequence of notes.
+        :param LFOOrLFOSequence retrigger: Any sequence of LFOs.
+
+        Note: for compatibility, ``release_then_press`` may be used as an alias
+        for this function. This compatibility name will be removed in 9.0."""
+    def release_all_then_press(self, /, press: NoteOrNoteSequence) -> None:
         """Turn any currently-playing notes off, then turn on the given notes
 
-        Releasing and pressing the note again has little effect, but does reset the phase
-        of the note, which may be perceptible as a small glitch.
+        Releasing a note and immediately pressing it again returns it to the
+        attack phase with an initial amplitude of 0.
 
-        :param NoteSequence press: Any sequence of notes."""
+        :param NoteOrNoteSequence press: Any sequence of notes."""
     def release_all(self) -> None:
         """Turn any currently-playing notes off"""
     def deinit(self) -> None:
         """Deinitialises the object and releases any memory resources for reuse."""
         ...
     def __enter__(self) -> Synthesizer:
         """No-op used by Context Managers."""
@@ -300,9 +460,16 @@
     envelope: Optional[Envelope]
     """The envelope to apply to all notes. `None`, the default envelope, instantly turns notes on and off. The envelope may be changed dynamically, but it affects all notes (even currently playing notes)"""
     sample_rate: int
     """32 bit value that tells how quickly samples are played in Hertz (cycles per second)."""
     pressed: NoteSequence
     """A sequence of the currently pressed notes (read-only property)"""
 
+    blocks: List[BlockInput]
+    """A list of blocks to advance whether or not they are associated with a playing note.
+
+    This can be used to implement 'free-running' LFOs. LFOs associated with playing notes are advanced whether or not they are in this list.
+
+    This property is read-only but its contents may be modified by e.g., calling ``synth.blocks.append()`` or ``synth.blocks.remove()``. It is initially an empty list."""
+
     max_polyphony: int
     """Maximum polyphony of the synthesizer (read-only class property)"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `types-circuitpython-8.1.0rc0/bindings/terminalio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/time/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/touchio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/traceback/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/usb_cdc/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/usb_hid/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/usb_host/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/usb_midi/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/vectorio/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/watchdog/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/wifi/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/wifi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/bindings/zlib/__init__.pyi` & `types-circuitpython-8.2.0b0/bindings/zlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/setup.py` & `types-circuitpython-8.2.0b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir, path
 
 from setuptools import setup
 
 __name__ = "types-circuitpython"
-__version__ = "8.1.0-rc.0"
+__version__ = "8.2.0-beta.0"
 __repo__ = "https://github.com/hardfury-labs/types-circuitpython"
 __author__ = "HardFury"
 
 
 HERE = path.abspath(path.dirname(__file__))
 BINDINGS_DIR = path.join(HERE, "bindings")
```

### Comparing `types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/SOURCES.txt` & `types-circuitpython-8.2.0b0/types_circuitpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.1.0rc0/types_circuitpython.egg-info/top_level.txt` & `types-circuitpython-8.2.0b0/types_circuitpython.egg-info/top_level.txt`

 * *Files identical despite different names*

