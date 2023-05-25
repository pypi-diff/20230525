# Comparing `tmp/VisionFive.gpio-1.2.8.tar.gz` & `tmp/VisionFive.gpio-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionFive.gpio-1.2.8.tar", last modified: Thu Apr 20 07:21:45 2023, max compression
+gzip compressed data, was "VisionFive.gpio-1.2.9.tar", last modified: Tue May 16 01:48:32 2023, max compression
```

## Comparing `VisionFive.gpio-1.2.8.tar` & `VisionFive.gpio-1.2.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/
--rw-r--r--   0 sz        (1000) sz        (1000)     1003 2023-04-20 07:12:09.000000 VisionFive.gpio-1.2.8/CHANGELOG.txt
--rw-r--r--   0 sz        (1000) sz        (1000)      430 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/INSTALL.txt
--rw-r--r--   0 sz        (1000) sz        (1000)     1060 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/LICENCE.txt
--rw-r--r--   0 sz        (1000) sz        (1000)       50 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/MANIFEST.in
--rw-rw-r--   0 sz        (1000) sz        (1000)     2510 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/PKG-INFO
--rw-r--r--   0 sz        (1000) sz        (1000)      757 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/README.txt
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/boardtype/
--rw-r--r--   0 sz        (1000) sz        (1000)     1241 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/boardtype/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/gpio/
--rw-r--r--   0 sz        (1000) sz        (1000)     1226 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/gpio/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive/i2c/
--rw-r--r--   0 sz        (1000) sz        (1000)     1225 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/i2c/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.913627 VisionFive.gpio-1.2.8/VisionFive/sample-code/
--rw-r--r--   0 sz        (1000) sz        (1000)     3760 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/I2C_Sense_Hat.py
--rw-r--r--   0 sz        (1000) sz        (1000)     2569 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/LED_Matrix.py
--rw-r--r--   0 sz        (1000) sz        (1000)      946 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py
--rw-r--r--   0 sz        (1000) sz        (1000)      826 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/__init__.py
--rw-r--r--   0 sz        (1000) sz        (1000)     2156 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/basic_edge_detection.py
--rw-r--r--   0 sz        (1000) sz        (1000)     1730 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/buzzer.py
--rw-r--r--   0 sz        (1000) sz        (1000)     4829 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_LED_Matrix.py
--rw-r--r--   0 sz        (1000) sz        (1000)     2817 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_waiting_time.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.913627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/
--rw-r--r--   0 sz        (1000) sz        (1000)       86 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/READEME.txt
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.913627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/
--rw-r--r--   0 sz        (1000) sz        (1000)     2598 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py
--rw-r--r--   0 sz        (1000) sz        (1000)    31487 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg
--rw-r--r--   0 sz        (1000) sz        (1000)   153656 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/__init__.py
--rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive.bmp
--rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive2.bmp
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/
--rw-r--r--   0 sz        (1000) sz        (1000)     7733 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py
--rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/example/
--rw-r--r--   0 sz        (1000) sz        (1000)      417 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/example/LCD_2intest.py
--rw-r--r--   0 sz        (1000) sz        (1000)      925 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/led.py
--rw-r--r--   0 sz        (1000) sz        (1000)     1390 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/pud_test.py
--rw-r--r--   0 sz        (1000) sz        (1000)     1150 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/pwm_led.py
--rw-r--r--   0 sz        (1000) sz        (1000)     8642 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/sample-code/uart_gps_demo.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/VisionFive/spi/
--rw-r--r--   0 sz        (1000) sz        (1000)     1225 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/VisionFive/spi/__init__.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.909627 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/
--rw-rw-r--   0 sz        (1000) sz        (1000)     2510 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/PKG-INFO
--rw-rw-r--   0 sz        (1000) sz        (1000)     2019 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/SOURCES.txt
--rw-rw-r--   0 sz        (1000) sz        (1000)        1 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/dependency_links.txt
--rw-rw-r--   0 sz        (1000) sz        (1000)       11 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/top_level.txt
--rw-r--r--   0 sz        (1000) sz        (1000)       38 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/setup.cfg
--rw-r--r--   0 sz        (1000) sz        (1000)     3747 2023-04-20 07:21:22.000000 VisionFive.gpio-1.2.8/setup.py
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.905627 VisionFive.gpio-1.2.8/source/
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/source/boardtype/
--rw-r--r--   0 sz        (1000) sz        (1000)     1340 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/boardtype/py_boardtype.c
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/source/gpio/
--rw-r--r--   0 sz        (1000) sz        (1000)    10302 2023-04-20 07:19:24.000000 VisionFive.gpio-1.2.8/source/gpio/c_gpio.c
--rw-r--r--   0 sz        (1000) sz        (1000)    21693 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/c_gpio.h
--rw-r--r--   0 sz        (1000) sz        (1000)     1510 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/cpuinfo.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1394 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/cpuinfo.h
--rw-r--r--   0 sz        (1000) sz        (1000)    15109 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/event_gpio.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1703 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/event_gpio.h
--rw-r--r--   0 sz        (1000) sz        (1000)     9596 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/gpio-utils.c
--rw-r--r--   0 sz        (1000) sz        (1000)     2097 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/gpio-utils.h
--rw-r--r--   0 sz        (1000) sz        (1000)     2866 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/py_constants.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1615 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/py_constants.h
--rw-r--r--   0 sz        (1000) sz        (1000)    22867 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/gpio/py_gpio.c
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.917627 VisionFive.gpio-1.2.8/source/i2c/
--rw-r--r--   0 sz        (1000) sz        (1000)     1845 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/i2c/c_i2c.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1345 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/i2c/c_i2c.h
--rw-r--r--   0 sz        (1000) sz        (1000)     4369 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/i2c/py_i2c.c
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/source/pwm/
--rw-r--r--   0 sz        (1000) sz        (1000)     6174 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/py_pwm.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1190 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/py_pwm.h
--rw-r--r--   0 sz        (1000) sz        (1000)     5188 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/soft_pwm.c
--rw-r--r--   0 sz        (1000) sz        (1000)     1334 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/pwm/soft_pwm.h
-drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.921627 VisionFive.gpio-1.2.8/source/spi/
--rw-r--r--   0 sz        (1000) sz        (1000)     6105 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/spi/py_spi.c
--rw-r--r--   0 sz        (1000) sz        (1000)     3831 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/spi/spi_dev.c
--rw-r--r--   0 sz        (1000) sz        (1000)      407 2023-04-06 06:31:47.000000 VisionFive.gpio-1.2.8/source/spi/spi_dev.h
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.284421 VisionFive.gpio-1.2.9/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1060 2023-05-16 01:38:33.000000 VisionFive.gpio-1.2.9/CHANGELOG.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)      430 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/INSTALL.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)     1060 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/LICENCE.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)       50 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/MANIFEST.in
+-rw-rw-r--   0 sz        (1000) sz        (1000)     4313 2023-05-16 01:48:32.284421 VisionFive.gpio-1.2.9/PKG-INFO
+-rw-r--r--   0 sz        (1000) sz        (1000)     2503 2023-05-16 01:47:10.000000 VisionFive.gpio-1.2.9/README.txt
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.244430 VisionFive.gpio-1.2.9/VisionFive/
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.244430 VisionFive.gpio-1.2.9/VisionFive/boardtype/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1241 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/boardtype/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.244430 VisionFive.gpio-1.2.9/VisionFive/gpio/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1226 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/gpio/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.244430 VisionFive.gpio-1.2.9/VisionFive/i2c/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1231 2023-05-12 08:28:40.000000 VisionFive.gpio-1.2.9/VisionFive/i2c/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.248429 VisionFive.gpio-1.2.9/VisionFive/sample-code/
+-rw-r--r--   0 sz        (1000) sz        (1000)     3760 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/I2C_Sense_Hat.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     2569 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/LED_Matrix.py
+-rw-r--r--   0 sz        (1000) sz        (1000)      946 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py
+-rw-r--r--   0 sz        (1000) sz        (1000)      826 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/__init__.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     2156 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/basic_edge_detection.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     1730 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/buzzer.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     4829 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/edge_detection_with_LED_Matrix.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     2817 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/edge_detection_with_waiting_time.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.248429 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/
+-rw-r--r--   0 sz        (1000) sz        (1000)       86 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/READEME.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.252428 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/
+-rw-r--r--   0 sz        (1000) sz        (1000)     2598 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py
+-rw-r--r--   0 sz        (1000) sz        (1000)    31487 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg
+-rw-r--r--   0 sz        (1000) sz        (1000)   153656 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/__init__.py
+-rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/visionfive.bmp
+-rw-r--r--   0 sz        (1000) sz        (1000)   230454 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/visionfive2.bmp
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.252428 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/lib/
+-rw-r--r--   0 sz        (1000) sz        (1000)     7733 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py
+-rw-r--r--   0 sz        (1000) sz        (1000)        0 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/lib/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.252428 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/lib/example/
+-rw-r--r--   0 sz        (1000) sz        (1000)      417 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/lib/example/LCD_2intest.py
+-rw-r--r--   0 sz        (1000) sz        (1000)      925 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/led.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     1390 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/pud_test.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     1150 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/pwm_led.py
+-rw-r--r--   0 sz        (1000) sz        (1000)     8642 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/VisionFive/sample-code/uart_gps_demo.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.252428 VisionFive.gpio-1.2.9/VisionFive/spi/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1231 2023-05-12 08:28:53.000000 VisionFive.gpio-1.2.9/VisionFive/spi/__init__.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.244430 VisionFive.gpio-1.2.9/VisionFive.gpio.egg-info/
+-rw-rw-r--   0 sz        (1000) sz        (1000)     4313 2023-05-16 01:48:32.000000 VisionFive.gpio-1.2.9/VisionFive.gpio.egg-info/PKG-INFO
+-rw-rw-r--   0 sz        (1000) sz        (1000)     2019 2023-05-16 01:48:32.000000 VisionFive.gpio-1.2.9/VisionFive.gpio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sz        (1000) sz        (1000)        1 2023-05-16 01:48:32.000000 VisionFive.gpio-1.2.9/VisionFive.gpio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sz        (1000) sz        (1000)       11 2023-05-16 01:48:32.000000 VisionFive.gpio-1.2.9/VisionFive.gpio.egg-info/top_level.txt
+-rw-r--r--   0 sz        (1000) sz        (1000)       38 2023-05-16 01:48:32.292420 VisionFive.gpio-1.2.9/setup.cfg
+-rw-r--r--   0 sz        (1000) sz        (1000)     3747 2023-05-12 09:02:47.000000 VisionFive.gpio-1.2.9/setup.py
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.240431 VisionFive.gpio-1.2.9/source/
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.252428 VisionFive.gpio-1.2.9/source/boardtype/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1340 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/boardtype/py_boardtype.c
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.260427 VisionFive.gpio-1.2.9/source/gpio/
+-rw-r--r--   0 sz        (1000) sz        (1000)    10302 2023-05-15 06:09:11.000000 VisionFive.gpio-1.2.9/source/gpio/c_gpio.c
+-rw-r--r--   0 sz        (1000) sz        (1000)    21693 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/c_gpio.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     1510 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/cpuinfo.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1394 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/cpuinfo.h
+-rw-r--r--   0 sz        (1000) sz        (1000)    15109 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/event_gpio.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1703 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/event_gpio.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     9596 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/gpio-utils.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     2097 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/gpio-utils.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     2866 2023-05-15 02:02:43.000000 VisionFive.gpio-1.2.9/source/gpio/py_constants.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1615 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/gpio/py_constants.h
+-rw-r--r--   0 sz        (1000) sz        (1000)    29340 2023-05-15 11:16:58.000000 VisionFive.gpio-1.2.9/source/gpio/py_gpio.c
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.260427 VisionFive.gpio-1.2.9/source/i2c/
+-rw-r--r--   0 sz        (1000) sz        (1000)     1845 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/i2c/c_i2c.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1345 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/i2c/c_i2c.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     6119 2023-05-12 06:55:26.000000 VisionFive.gpio-1.2.9/source/i2c/py_i2c.c
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.280422 VisionFive.gpio-1.2.9/source/pwm/
+-rw-r--r--   0 sz        (1000) sz        (1000)     8179 2023-05-12 08:21:45.000000 VisionFive.gpio-1.2.9/source/pwm/py_pwm.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1190 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/pwm/py_pwm.h
+-rw-r--r--   0 sz        (1000) sz        (1000)     5188 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/pwm/soft_pwm.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     1334 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/pwm/soft_pwm.h
+drwxrwxr-x   0 sz        (1000) sz        (1000)        0 2023-05-16 01:48:32.280422 VisionFive.gpio-1.2.9/source/spi/
+-rw-r--r--   0 sz        (1000) sz        (1000)     8345 2023-05-15 01:24:20.000000 VisionFive.gpio-1.2.9/source/spi/py_spi.c
+-rw-r--r--   0 sz        (1000) sz        (1000)     3870 2023-05-12 08:40:52.000000 VisionFive.gpio-1.2.9/source/spi/spi_dev.c
+-rw-r--r--   0 sz        (1000) sz        (1000)      407 2023-04-20 07:21:45.000000 VisionFive.gpio-1.2.9/source/spi/spi_dev.h
```

### Comparing `VisionFive.gpio-1.2.8/CHANGELOG.txt` & `VisionFive.gpio-1.2.9/CHANGELOG.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 Change Log
 ==========
+1.2.9
+-------
+- Add help description for gpio, i2c, spi
+
 1.2.8
 -------
 -Fix gpio issue
 
 1.2.7
 -------
 -Fix pud issue
```

### Comparing `VisionFive.gpio-1.2.8/LICENCE.txt` & `VisionFive.gpio-1.2.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/boardtype/__init__.py` & `VisionFive.gpio-1.2.9/VisionFive/boardtype/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/gpio/__init__.py` & `VisionFive.gpio-1.2.9/VisionFive/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/i2c/__init__.py` & `VisionFive.gpio-1.2.9/VisionFive/i2c/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-"""This package provides a Python module to control the GPIO on a VisionFive"""
+"""This package provides a Python module to control the I2C device on a VisionFive"""
 
 from VisionFive._i2c import *
 
 VERSION = '1.0.0'
```

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/I2C_Sense_Hat.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/I2C_Sense_Hat.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/LED_Matrix.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/LED_Matrix.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/RPi_demo_#GPIO_basic#_run_on_VisionFive.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/RPi_demo_#PWM#_run_on_VisionFive.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/basic_edge_detection.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/basic_edge_detection.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/buzzer.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/buzzer.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_LED_Matrix.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/edge_detection_with_LED_Matrix.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/edge_detection_with_waiting_time.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/edge_detection_with_waiting_time.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/2.4inch_LCD_demo.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/LCD_2inch.jpg`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/LCD_2inch4_parrot.bmp`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive.bmp` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/visionfive.bmp`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/example/visionfive2.bmp` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/example/visionfive2.bmp`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/lcddemo/lib/LCD2inch4_lib.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/led.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/led.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/pud_test.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/pud_test.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/pwm_led.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/pwm_led.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/sample-code/uart_gps_demo.py` & `VisionFive.gpio-1.2.9/VisionFive/sample-code/uart_gps_demo.py`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/VisionFive/spi/__init__.py` & `VisionFive.gpio-1.2.9/VisionFive/spi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-"""This package provides a Python module to control the GPIO on a VisionFive"""
+"""This package provides a Python module to control the SPI device on a VisionFive"""
 
 from VisionFive._spi import *
 
 VERSION = '1.0.0'
```

### Comparing `VisionFive.gpio-1.2.8/VisionFive.gpio.egg-info/SOURCES.txt` & `VisionFive.gpio-1.2.9/VisionFive.gpio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/setup.py` & `VisionFive.gpio-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 module_boardtype = Extension('VisionFive._boardtype',
                            [
                             'source/gpio/cpuinfo.c',
                             'source/boardtype/py_boardtype.c'])
 
 setup(name             = 'VisionFive.gpio',
-      version          = '1.2.8',
+      version          = '1.2.9',
       author           = 'VisionFive',
       author_email     = 'support@starfivetech.com',
       description      = 'A module to control VisionFive GPIO ports',
       long_description = open('README.txt').read() + open('CHANGELOG.txt').read(),
       license          = 'MIT',
       keywords         = 'VisionFive GPIO',
       url              = 'http://gitlab.starfivetech.com/Product/Software AE/VisionFive-python-gpio/starfive_gpio',
```

### Comparing `VisionFive.gpio-1.2.8/source/boardtype/py_boardtype.c` & `VisionFive.gpio-1.2.9/source/boardtype/py_boardtype.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/c_gpio.c` & `VisionFive.gpio-1.2.9/source/gpio/c_gpio.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/c_gpio.h` & `VisionFive.gpio-1.2.9/source/gpio/c_gpio.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/cpuinfo.c` & `VisionFive.gpio-1.2.9/source/gpio/cpuinfo.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/cpuinfo.h` & `VisionFive.gpio-1.2.9/source/gpio/cpuinfo.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/event_gpio.c` & `VisionFive.gpio-1.2.9/source/gpio/event_gpio.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/event_gpio.h` & `VisionFive.gpio-1.2.9/source/gpio/event_gpio.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/gpio-utils.c` & `VisionFive.gpio-1.2.9/source/gpio/gpio-utils.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/gpio-utils.h` & `VisionFive.gpio-1.2.9/source/gpio/gpio-utils.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/py_constants.c` & `VisionFive.gpio-1.2.9/source/gpio/py_constants.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/py_constants.h` & `VisionFive.gpio-1.2.9/source/gpio/py_constants.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/gpio/py_gpio.c` & `VisionFive.gpio-1.2.9/source/gpio/py_gpio.c`

 * *Files 26% similar despite different names*

```diff
@@ -36,14 +36,37 @@
    int gpio;
    PyObject *py_cb;
    struct py_callback *next;
 };
 static struct py_callback *py_callbacks = NULL;
 
 
+int pin_check(PyObject *tempobj, int *gpioport) {
+	unsigned int gpiooffset;
+
+#if PY_MAJOR_VERSION > 2
+		if (PyLong_Check(tempobj)) {
+			*gpioport = (int)PyLong_AsLong(tempobj);
+#else
+		if (PyInt_Check(tempobj)) {
+			*gpioport = (int)PyInt_AsLong(tempobj);
+#endif
+		if (PyErr_Occurred())
+			return 1;
+		} else {
+			PyErr_SetString(PyExc_ValueError, "gpioport must be an integer");
+			return 1;
+		}
+		if (pin_valid(gpioport))
+			return 1;
+
+		return 0;
+}
+
+
 int int_check(PyObject *tempobj, int *gpioport) {
 	unsigned int gpiooffset;
 
 #if PY_MAJOR_VERSION > 2
 		if (PyLong_Check(tempobj)) {
 			*gpioport = (int)PyLong_AsLong(tempobj);
 #else
@@ -717,26 +740,17 @@
 		return NULL;
 	} else {
 		return Py_BuildValue("i", gpio);
 	}
 
 }
 
-// python function value = gpio_function(gpio)
-static PyObject *py_gpio_function(PyObject *self, PyObject *args)
-{
-	int gpio, f = MODE_UNKNOWN;
-	PyObject *func;
-
-	if (!PyArg_ParseTuple(args, "i", &gpio))
-		return NULL;
-
-	if (pin_valid(&gpio))
-		return NULL;
-
+static int gpio_func_check(int gpio, unsigned char pn []) {
+	int f = MODE_UNKNOWN;
+	
 	switch (gpio)
 	{	case 7:
 		case 11:
 		case 12:
 		case 13:
 		case 15:
 		case 16:
@@ -748,68 +762,267 @@
 		case 29:
 		case 31:
 		case 35:
 		case 36:
 		case 37:
 		case 38:
 		case 40:
-				 if (OUTPUT == gpio_get_dir(gpio))
-				 	f = OUTPUT;
-				 else if (INPUT == gpio_get_dir(gpio))
-				 	f = INPUT;
-				 else if (gpio_get_dir(gpio) < 0)
-				 	f = MODE_UNKNOWN;
+				 if (OUTPUT == gpio_get_dir(gpio)) {
+					 f = OUTPUT;
+					 memcpy(pn, "gpio(input)", strlen("gpio(input)"));
+				 }
+				 else if (INPUT == gpio_get_dir(gpio)) {
+					f = INPUT;
+					memcpy(pn, "gpio(output)", strlen("gpio(output)"));
+				 }
+				 else if (gpio_get_dir(gpio) < 0) {
+					f = MODE_UNKNOWN;
+					memcpy(pn, "unkown", strlen("unkown"));
+				 }
 				 break;
 
 		case 3 :
-		case 5 : f = I2C; break;
-
+		case 5 : 
+					f = I2C; 
+					memcpy(pn, "i2c", strlen("i2c"));
+					break;
 		case 19 :
 		case 21 :
 		case 23 :
-		case 24 : f = SPI; break;
+		case 24 : 
+					f = SPI;
+					memcpy(pn, "spi", strlen("spi"));
+					break;
 
 		case 32 :
-		case 33 : f = PWM; break;
+		case 33 : 
+					f = PWM; 
+					memcpy(pn, "pwm", strlen("pwm"));
+					break;
 
 		case 8 :
-		case 10 : f = SERIAL; break;
+		case 10 : 
+					f = SERIAL;
+					memcpy(pn, "serial", strlen("serial"));
+					break;
+
+		default :
+					f = MODE_UNKNOWN;
+					memcpy(pn, "NA", strlen("NA"));
+					break;
+	}
 
-		default : f = MODE_UNKNOWN; break;
+	return f;
+}
+
+// python function value = gpio_function(gpio)
+static PyObject *py_gpio_function(PyObject *self, PyObject *args, PyObject *kwargs)
+{
+	int gpio, f = MODE_UNKNOWN;
+	int ret, i;
+	int gpiocount = -255;
+	int found = 0;
+	int gpioport = -255;
+	unsigned int gpiooffset;
+	PyObject *gpiolist = NULL;
+	PyObject *gpiotuple = NULL;
+	PyObject *tempobj;
+	PyObject *func;
+	static char *kwlist[] = {"channel", NULL};
+	unsigned char pn[20] = {0};
+
+	if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|O", kwlist, &gpiolist))
+		return NULL;
+
+	if (gpiolist == NULL) {  // gpioport kwarg not set
+	// do nothing
+	}
+	else {
+		ret = GPIO_Data_check(gpiolist, gpiotuple, &gpioport, &gpiocount);
+		if (ret == 1)
+			return NULL;
 	}
-	func = Py_BuildValue("i", f);
-	return func;
+
+	if (gpioport == -255 && gpiocount == -255) {
+		printf("pin\t\tfunc:\n");
+		for (i = 1; i < 41; i++) {
+			memset(pn, 0, 20);
+			f = gpio_func_check(i, pn);
+			printf("%d\t\t%s\n", i, pn);
+		}
+	} else if (gpioport != -255) {
+		if (pin_valid(&gpioport)) return NULL;
+		printf("pin\t\tfunc:\n");
+		memset(pn, 0, 20);
+		f = gpio_func_check(gpioport, pn);
+		printf("%d\t\t%s\n", gpioport, pn);
+	} else {  
+		// gpioport was a list/tuple
+		printf("pin\t\tfunc:\n");
+		for (i = 0; i < gpiocount; i++) {
+			if (gpiolist) {
+				if ((tempobj = PyList_GetItem(gpiolist, i)) == NULL) {
+					return NULL;
+				}
+			} else { // assume gpiotuple
+				if ((tempobj = PyTuple_GetItem(gpiotuple, i)) == NULL) {
+					return NULL;
+				}
+			}
+
+			ret = pin_check(tempobj, &gpioport);
+			if (ret == 1)
+				return NULL;
+			
+			memset(pn, 0, 20);
+			f = gpio_func_check(gpioport, pn);
+			printf("%d\t\t%s\n", gpioport, pn);
+		}
+	}
+
+	Py_RETURN_NONE;
 }
 
 // python function setwarnings(state)
 static PyObject *py_setwarnings(PyObject *self, PyObject *args)
 {
 	if (!PyArg_ParseTuple(args, "i", &gpio_warnings))
 		return NULL;
 
 	Py_RETURN_NONE;
 }
 
 static const char moduledocstring[] = "Python GPIO module for VisionFive";
 
 PyMethodDef sfv_gpio_methods[] = {
-	{"setup", (PyCFunction)py_setup_gpioport, METH_VARARGS | METH_KEYWORDS, "Setup direction"},
-	{"cleanup", (PyCFunction)py_cleanup, METH_VARARGS | METH_KEYWORDS, "set default."},
-	{"output", py_output_gpio, METH_VARARGS, "Output to a GPIO gpioport or list of gpioports\ngpioport - GPIO pin No.\nvalue   - 0/1 or False/True or LOW/HIGH"},
-	{"input", py_input_gpio, METH_VARARGS, "Input from a GPIO gpioport.	Returns HIGH=1=True or LOW=0=False\ngpioport - GPIO pin No."},
-	{"setmode", py_setmode, METH_VARARGS, "Just Compatible with RPI CMD"},
-	{"getmode", py_getmode, METH_VARARGS, "Just Compatible with RPI CMD"},
-	{"add_event_detect", (PyCFunction)py_add_event_detect, METH_VARARGS | METH_KEYWORDS, "Enable edge detection events for a particular GPIO port.\ngpio - GPIO pin No.\nedge		  - RISING, FALLING or BOTH\n[callback]   - A callback function for the event (optional)\n[bouncetime] - Switch bounce timeout in ms for callback"},
-	{"remove_event_detect", py_remove_event_detect, METH_VARARGS, "Remove edge detection for a particular GPIO pin\nGPIO - GPIO pin No."},
-	{"event_detected", py_event_detected, METH_VARARGS, "Returns 1 if an RISING_EDGE.\ngpio - GPIO pin No."},
-	{"get_detected_event", (PyCFunction)py_get_detected_event, METH_VARARGS | METH_KEYWORDS, "Returns 1 with RISING_EDGE detected, returns 2 with FALLING_EDGE detected, returns 0 with others..\ngpio - GPIO pin No.\n"},
-	{"add_event_callback", (PyCFunction)py_add_event_callback, METH_VARARGS | METH_KEYWORDS, "Add a callback for an event already defined using add_event_detect()\ngpio - GPIO pin No.\ncallback	   - a callback function"},
-	{"wait_for_edge", (PyCFunction)py_wait_for_edge, METH_VARARGS | METH_KEYWORDS, "Wait for an edge.  Returns the channel number or None on timeout.\ngpio - GPIO pin No.\nedge		  - RISING, FALLING or BOTH\n[bouncetime] - time allowed between calls to allow for switchbounce\n[timeout]    - timeout in ms"},
-	{"gpio_function", py_gpio_function, METH_VARARGS, "Return the current GPIO function (IN, OUT, PWM, SERIAL, I2C, SPI)\ngpio - GPIO pin No."},
-	{"setwarnings", py_setwarnings, METH_VARARGS, "Just Compatible with RPI CMD"},
+	{"setup", (PyCFunction)py_setup_gpioport, METH_VARARGS | METH_KEYWORDS,
+					"***************************************************************\n" \
+					"function: setup direction and pull-up pull-down of GPIO pin \n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n"\
+					"  GPIO.setup(pin, GPIO.OUT) \n" \
+					"  GPIO.setup(37, GPIO.IN, pull_up_down=GPIO.PUD_DOWN) \n" \
+					"  GPIO.setup(37, GPIO.IN, pull_up_down=GPIO.PUD_UP) \n" \
+					"***************************************************************\n"},
+
+	{"cleanup", (PyCFunction)py_cleanup, METH_VARARGS | METH_KEYWORDS,
+					"***************************************************************\n" \
+					"function: set default config to GPIO pin \n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n"\
+					"  GPIO.cleanup(37) \n" \
+					"  GPIO.cleanup() \n" \
+					"***************************************************************\n"},
+
+	{"output", py_output_gpio, METH_VARARGS, 
+					"***************************************************************\n"\
+					"function: set output level to GPIO pin \n" \
+					"usage: \n"	\
+					"  import VisionFive.gpio as GPIO \n"\
+					"  GPIO.setup(pin, GPIO.OUT) \n" \
+					"  GPIO.output(led_pin, GPIO.HIGH) \n" \
+					"  GPIO.output(led_pin, GPIO.LOW) \n" \
+					"***************************************************************\n"},
+
+	{"input", py_input_gpio, METH_VARARGS, 
+					"***************************************************************\n" \
+					"function: get input level from GPIO pin \n" \
+					"          returns 1, meaning HIGH level; or 0, meaning LOW level\n" \
+					"usage: \n"	\
+					"  import VisionFive.gpio as GPIO \n"\
+					"  IVAL = GPIO.input(pin) \n" \
+					"***************************************************************\n"},
+
+	{"setmode", py_setmode, METH_VARARGS, 
+					"function: just compatible with RPI CMD \n"},
+
+	{"getmode", py_getmode, METH_VARARGS, 
+					"function: just compatible with RPI CMD \n"},
+
+	{"add_event_detect", (PyCFunction)py_add_event_detect, METH_VARARGS | METH_KEYWORDS,
+					"***************************************************************\n" \
+					"function: enable edge detection for a GPIO pin.\n" \
+					"           [callback]   - a callback function for the event (optional)\n" \
+					"           [bouncetime] - set bouncetime(unit: millisecond) to avoid jitter \n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n"\
+					"  \n"
+					"  def detect(pin, edge_type): \n" \
+					"        if (1 == edge_type): \n" \
+					"           print('Rising edge is detected') \n" \
+					"        elif (2 == edge_type): \n" \
+					"           print('Failing edge is detected') \n" \
+					"        \n" \
+					"  GPIO.add_event_detect(37, GPIO.FALLING, callback=detect, bouncetime=2) \n" \
+					"  GPIO.remove_event_detect(37) \n" \
+					"  GPIO.add_event_detect(key_pin, GPIO.RISING, callback=detect, bouncetime=2) \n" \
+					"  GPIO.remove_event_detect(37) \n"\
+					"***************************************************************\n"},
+
+	{"remove_event_detect", py_remove_event_detect, METH_VARARGS,
+					"***************************************************************\n" \
+					"function: remove edge detection for a GPIO pin\n" \
+					"usage: \n" \
+					"  please see usage of API  add_event_detect() \n" \
+					"***************************************************************\n"},
+
+	{"event_detected", py_event_detected, METH_VARARGS, 
+					"***************************************************************\n" \
+					"function: query if edge event is detected \n" \
+					"          returns 1, meaning edge is detected; 0, meaning edge isn't detected.\n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n" \
+					"  edge_detected_flag = GPIO.event_detected(37) \n" \
+					"***************************************************************\n"},
+
+	{"get_detected_event", (PyCFunction)py_get_detected_event, METH_VARARGS | METH_KEYWORDS, 
+					"***************************************************************\n" \
+					"function: query the edge type after detecting edge \n" \ 
+					"          returns 1, meaning rising edge is detected; \n" \
+					"                  2, meaning failing edge is detected.\n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n" \
+					"  edge_type = GPIO.get_detected_event(37) \n" \
+					"***************************************************************\n"},
+
+	{"add_event_callback", (PyCFunction)py_add_event_callback, METH_VARARGS | METH_KEYWORDS,
+					"***************************************************************\n"\
+					"function: adding a callback for an event already defined using add_event_detect()\n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n" \
+					"  GPIO.add_event_detect(37, GPIO.FALLING, bouncetime=2) \n" \
+					"  GPIO.add_event_callback(37, callback=detect) \n" \
+					"***************************************************************\n"},
+
+	{"wait_for_edge", (PyCFunction)py_wait_for_edge, METH_VARARGS | METH_KEYWORDS,
+					"***************************************************************\n"\
+					"function: wait for an edge. \n" \
+					"          Returns the GPIO pin nubmer or None on timeout.\n" \
+					"          [bouncetime] - set bouncetime(unit: second) to avoid jitter \n" \
+					"          [timeout] - detecting edge event in a time window(unit: millisecond)  \n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n" \
+					"  GPIO.wait_for_edge(37, GPIO.FALLING, bouncetime=2, timeout=5000) \n" \
+					"  GPIO.wait_for_edge(37, GPIO.RISING, bouncetime=2) \n" \
+					"  Note: the default timeout is -1, meaning waiting until edge event is detected \n"
+					"***************************************************************\n"},
+
+	{"gpio_function", (PyCFunction)py_gpio_function, METH_VARARGS | METH_KEYWORDS,
+					"***************************************************************\n"\
+					"fucntion: query pin fuction (gpio, pwm, serial, i2c, spi)\n" \
+					"usage: \n" \
+					"  import VisionFive.gpio as GPIO \n" \
+					"  #query function of all pins \n"
+					"  GPIO.gpio_function() \n"
+					"  GPIO.gpio_function(37) \n"
+					"***************************************************************\n"},
+
+	{"setwarnings", py_setwarnings, METH_VARARGS, 
+					"just compatible with RPI CMD"},
+					
 	{NULL, NULL, 0, NULL}
 };
 
 #if PY_MAJOR_VERSION > 2
 static struct PyModuleDef sfvgpiomodule = {
 	PyModuleDef_HEAD_INIT,
 	"VisionFive._gpio",      // name of module
```

### Comparing `VisionFive.gpio-1.2.8/source/i2c/c_i2c.c` & `VisionFive.gpio-1.2.9/source/i2c/c_i2c.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/i2c/c_i2c.h` & `VisionFive.gpio-1.2.9/source/i2c/c_i2c.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/pwm/py_pwm.h` & `VisionFive.gpio-1.2.9/source/pwm/py_pwm.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/pwm/soft_pwm.c` & `VisionFive.gpio-1.2.9/source/pwm/soft_pwm.c`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/pwm/soft_pwm.h` & `VisionFive.gpio-1.2.9/source/pwm/soft_pwm.h`

 * *Files identical despite different names*

### Comparing `VisionFive.gpio-1.2.8/source/spi/spi_dev.c` & `VisionFive.gpio-1.2.9/source/spi/spi_dev.c`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 #define SPI_TX_OCTAL            0x2000      /* transmit with 8 wires */
 #define SPI_RX_OCTAL            0x4000      /* receive with 8 wires */
 #endif
 
 
 static int      fds    = 0;
 //static uint32_t mode  = 0;
-static uint32_t speed = 500000;
-static uint16_t delay = 0;
-static uint8_t  bits  = 8;
+static uint32_t gspeed = 500000;
+static uint16_t gdelay = 0;
+static uint8_t  gbits  = 8;
 static int      gmode  = 0;
 
 int spi_getdev(char *dev)
 {
 	fds = open(dev, O_RDWR);
 	if(fds < 0){
 		printf("open spi dev failed\n");
@@ -62,15 +62,14 @@
 	return 0;
 }
 
 int spi_setmode(int speed, int mode, int bits)
 {
 	int retval = 0;
 
-	gmode = mode;
 	retval = ioctl(fds, SPI_IOC_WR_MODE32, &mode);
 	if(retval < 0){
 		printf("set spi wr mode failed\n");
 		return -1;
 	}
 
 	retval = ioctl(fds, SPI_IOC_RD_MODE32, &mode);
@@ -99,14 +98,18 @@
 
 	retval = ioctl(fds, SPI_IOC_RD_MAX_SPEED_HZ, &speed);
 	if(retval < 0){
 		printf("set wrd speed failed\n");
 		return -1;
 	}
 
+	gmode = mode;
+	gspeed = speed;
+	gbits = bits;
+
 	printf("Set Spi mode successfully\n");
 	printf("spi mode: 0x%x\n", mode);
 	printf("bits per word: %u\n", bits);
 	printf("max speed: %u Hz (%u kHz)\n", speed, speed/1000);
 
 	return 0;
 
@@ -126,17 +129,17 @@
 		return -1;
 	}
 	memset(recv_data, 0, len);
 
 	tr.tx_buf        = (unsigned long)data;
 	tr.rx_buf        = (unsigned long)recv_data;
 	tr.len           = len;
-	tr.delay_usecs   = delay;
-	tr.speed_hz      = speed;
-	tr.bits_per_word = bits;
+	tr.delay_usecs   = gdelay;
+	tr.speed_hz      = gspeed;
+	tr.bits_per_word = gbits;
 
 	if(gmode & SPI_TX_OCTAL)
 		tr.tx_nbits = 8;
 	else if(gmode & SPI_TX_QUAD)
 		tr.tx_nbits = 4;
 	else if(gmode & SPI_TX_DUAL)
 		tr.tx_nbits = 2;
```

