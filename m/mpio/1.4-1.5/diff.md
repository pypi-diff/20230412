# Comparing `tmp/mpio-1.4.tar.gz` & `tmp/mpio-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpio-1.4.tar", last modified: Wed Jul  6 13:28:38 2022, max compression
+gzip compressed data, was "mpio-1.5.tar", last modified: Wed Apr 12 16:19:59 2023, max compression
```

## Comparing `mpio-1.4.tar` & `mpio-1.5.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2022-07-06 13:28:38.576577 mpio-1.4/
--rw-r--r--   0 nferre    (1002) nferre    (1002)    11358 2020-02-12 10:59:53.000000 mpio-1.4/LICENSE
--rw-r--r--   0 nferre    (1002) nferre    (1002)     1099 2020-02-12 10:59:53.000000 mpio-1.4/LICENSE.MIT
--rw-r--r--   0 nferre    (1002) nferre    (1002)       88 2020-02-12 10:59:53.000000 mpio-1.4/MANIFEST.in
--rw-r--r--   0 nferre    (1002) nferre    (1002)      422 2020-02-12 10:59:53.000000 mpio-1.4/Makefile
--rw-rw-r--   0 nferre    (1002) nferre    (1002)     2388 2022-07-06 13:28:38.576577 mpio-1.4/PKG-INFO
--rw-rw-r--   0 nferre    (1002) nferre    (1002)     1471 2022-07-06 10:21:24.000000 mpio-1.4/README.md
-drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2022-07-06 13:28:38.576577 mpio-1.4/mpio/
--rw-r--r--   0 nferre    (1002) nferre    (1002)     1073 2022-07-06 10:06:41.000000 mpio-1.4/mpio/__init__.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)    10390 2020-02-12 10:59:53.000000 mpio-1.4/mpio/adc.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     6088 2020-02-18 16:22:28.000000 mpio-1.4/mpio/devmem.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)    14456 2020-02-18 16:22:28.000000 mpio-1.4/mpio/gpio.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     7646 2020-02-12 10:59:53.000000 mpio-1.4/mpio/i2c.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     5230 2020-02-12 10:59:53.000000 mpio-1.4/mpio/input.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     1984 2020-02-12 10:59:53.000000 mpio-1.4/mpio/ioctl.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     4205 2020-02-12 10:59:53.000000 mpio-1.4/mpio/led.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     9744 2020-02-18 16:22:28.000000 mpio-1.4/mpio/pwm.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)    18689 2020-02-12 10:59:53.000000 mpio-1.4/mpio/serial.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)     4128 2020-02-12 10:59:53.000000 mpio-1.4/mpio/smbus.py
--rw-r--r--   0 nferre    (1002) nferre    (1002)    13398 2020-02-12 10:59:53.000000 mpio-1.4/mpio/spi.py
--rw-rw-r--   0 nferre    (1002) nferre    (1002)     3506 2022-07-06 09:48:11.000000 mpio-1.4/mpio/utils.py
-drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2022-07-06 13:28:38.576577 mpio-1.4/mpio.egg-info/
--rw-r--r--   0 nferre    (1002) nferre    (1002)     2388 2022-07-06 13:28:38.000000 mpio-1.4/mpio.egg-info/PKG-INFO
--rw-r--r--   0 nferre    (1002) nferre    (1002)      366 2022-07-06 13:28:38.000000 mpio-1.4/mpio.egg-info/SOURCES.txt
--rw-r--r--   0 nferre    (1002) nferre    (1002)        1 2022-07-06 13:28:38.000000 mpio-1.4/mpio.egg-info/dependency_links.txt
--rw-r--r--   0 nferre    (1002) nferre    (1002)        5 2022-07-06 13:28:38.000000 mpio-1.4/mpio.egg-info/top_level.txt
--rw-r--r--   0 nferre    (1002) nferre    (1002)    12509 2020-02-12 10:59:53.000000 mpio-1.4/pylintrc
--rw-r--r--   0 nferre    (1002) nferre    (1002)      133 2022-07-06 13:28:38.576577 mpio-1.4/setup.cfg
--rw-r--r--   0 nferre    (1002) nferre    (1002)     1927 2022-07-06 13:28:35.000000 mpio-1.4/setup.py
+drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2023-04-12 16:19:59.424191 mpio-1.5/
+-rw-r--r--   0 nferre    (1002) nferre    (1002)    11358 2020-02-12 10:59:53.000000 mpio-1.5/LICENSE
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1099 2020-02-12 10:59:53.000000 mpio-1.5/LICENSE.MIT
+-rw-r--r--   0 nferre    (1002) nferre    (1002)       88 2020-02-12 10:59:53.000000 mpio-1.5/MANIFEST.in
+-rw-r--r--   0 nferre    (1002) nferre    (1002)      422 2020-02-12 10:59:53.000000 mpio-1.5/Makefile
+-rw-rw-r--   0 nferre    (1002) nferre    (1002)     2385 2023-04-12 16:19:59.424191 mpio-1.5/PKG-INFO
+-rw-rw-r--   0 nferre    (1002) nferre    (1002)     1468 2022-07-06 13:43:27.000000 mpio-1.5/README.md
+drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2023-04-12 16:19:59.420191 mpio-1.5/mpio/
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1073 2023-04-12 16:10:43.000000 mpio-1.5/mpio/__init__.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)    10390 2020-02-12 10:59:53.000000 mpio-1.5/mpio/adc.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     6088 2020-02-18 16:22:28.000000 mpio-1.5/mpio/devmem.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)    14456 2020-02-18 16:22:28.000000 mpio-1.5/mpio/gpio.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     7646 2020-02-12 10:59:53.000000 mpio-1.5/mpio/i2c.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     5230 2020-02-12 10:59:53.000000 mpio-1.5/mpio/input.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1984 2020-02-12 10:59:53.000000 mpio-1.5/mpio/ioctl.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     4205 2020-02-12 10:59:53.000000 mpio-1.5/mpio/led.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     9744 2020-02-18 16:22:28.000000 mpio-1.5/mpio/pwm.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)    18689 2020-02-12 10:59:53.000000 mpio-1.5/mpio/serial.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     4128 2020-02-12 10:59:53.000000 mpio-1.5/mpio/smbus.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)    13398 2020-02-12 10:59:53.000000 mpio-1.5/mpio/spi.py
+-rw-rw-r--   0 nferre    (1002) nferre    (1002)     3568 2022-07-15 16:18:15.000000 mpio-1.5/mpio/utils.py
+drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2023-04-12 16:19:59.420191 mpio-1.5/mpio.egg-info/
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     2385 2023-04-12 16:19:59.000000 mpio-1.5/mpio.egg-info/PKG-INFO
+-rw-r--r--   0 nferre    (1002) nferre    (1002)      557 2023-04-12 16:19:59.000000 mpio-1.5/mpio.egg-info/SOURCES.txt
+-rw-r--r--   0 nferre    (1002) nferre    (1002)        1 2023-04-12 16:19:59.000000 mpio-1.5/mpio.egg-info/dependency_links.txt
+-rw-r--r--   0 nferre    (1002) nferre    (1002)        5 2023-04-12 16:19:59.000000 mpio-1.5/mpio.egg-info/top_level.txt
+-rw-r--r--   0 nferre    (1002) nferre    (1002)    12509 2020-02-12 10:59:53.000000 mpio-1.5/pylintrc
+-rw-r--r--   0 nferre    (1002) nferre    (1002)      133 2023-04-12 16:19:59.424191 mpio-1.5/setup.cfg
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1927 2022-07-06 13:28:35.000000 mpio-1.5/setup.py
+drwxrwxr-x   0 nferre    (1002) nferre    (1002)        0 2023-04-12 16:19:59.424191 mpio-1.5/tests/
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1584 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_adc.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1234 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_devmem.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     4168 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_gpio.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     2822 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_i2c.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1725 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_input.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     2367 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_led.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     2019 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_pwm.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     2031 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_serial.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     2126 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_smbus.py
+-rw-r--r--   0 nferre    (1002) nferre    (1002)     1903 2020-02-12 10:59:53.000000 mpio-1.5/tests/test_spi.py
```

### Comparing `mpio-1.4/LICENSE` & `mpio-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mpio-1.4/LICENSE.MIT` & `mpio-1.5/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `mpio-1.4/PKG-INFO` & `mpio-1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpio
-Version: 1.4
+Version: 1.5
 Summary: Hardware access for Microchip boards
 Author: Joshua Henderson
 Author-email: joshua.henderson@microchip.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
@@ -23,18 +23,18 @@
 
    Microchip
 
 Microchip Peripheral I/O Python Package
 =======================================
 
 This package provides easy access to various hardware peripherals found
-on Microchip AT91/SAMA5 processors and Xplained boards running Linux.
-The API is clean, consistent, flexible, documented, and well tested to
-make navigating and exercising even the most complex hardware
-peripherals a trivial task.
+on Microchip AT91/SAMA5/SAMA7 processors and boards running Linux. The
+API is clean, consistent, flexible, documented, and well tested to make
+navigating and exercising even the most complex hardware peripherals a
+trivial task.
 
 Supported Interfaces
 --------------------
 
 -  ADC - Analog-to-Digital Converter
 -  DevMem - Read and Write System Memory
 -  GPIO - General Purpose I/O
```

### Comparing `mpio-1.4/README.md` & `mpio-1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ![Microchip](https://raw.githubusercontent.com/linux4sam/mpio/master/docs/_static/microchip_logo.png)
 
 # Microchip Peripheral I/O Python Package
 
 This package provides easy access to various hardware peripherals found on
-Microchip AT91/SAMA5 processors and Xplained boards running Linux.  The API is
+Microchip AT91/SAMA5/SAMA7 processors and boards running Linux.  The API is
 clean, consistent, flexible, documented, and well tested to make navigating and
 exercising even the most complex hardware peripherals a trivial task.
 
 
 ## Supported Interfaces
 
 * ADC - Analog-to-Digital Converter
```

### Comparing `mpio-1.4/mpio/__init__.py` & `mpio-1.5/mpio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 from .input import Input
 from .i2c import I2C
 from .spi import SPI
 from .serial import Serial
 from .devmem import DevMem
 from .smbus import SMBus
 
-__version__ = '1.4'
+__version__ = '1.5'
 "mpio module version string."
```

### Comparing `mpio-1.4/mpio/adc.py` & `mpio-1.5/mpio/adc.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/devmem.py` & `mpio-1.5/mpio/devmem.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/gpio.py` & `mpio-1.5/mpio/gpio.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/i2c.py` & `mpio-1.5/mpio/i2c.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/input.py` & `mpio-1.5/mpio/input.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/ioctl.py` & `mpio-1.5/mpio/ioctl.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/led.py` & `mpio-1.5/mpio/led.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/pwm.py` & `mpio-1.5/mpio/pwm.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/serial.py` & `mpio-1.5/mpio/serial.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/smbus.py` & `mpio-1.5/mpio/smbus.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/spi.py` & `mpio-1.5/mpio/spi.py`

 * *Files identical despite different names*

### Comparing `mpio-1.4/mpio/utils.py` & `mpio-1.5/mpio/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     """
 
     fixed = os.environ.get('MPIO_BOARD')
     if fixed:
         return fixed
 
     boards = [
+        ("sam9x60-curiosity", "microchip,sam9x60-curiosity"),
         ("sam9x60-ek", "microchip,sam9x60ek"),
         ("sam9x75-eb", "microchip,sam9x75eb"),
         ("sama5d3-xplained", "atmel,sama5d3-xplained"),
         ("sama5d4-xplained", "atmel,sama5d4-xplained"),
         ("sama5d2-xplained", "atmel,sama5d2-xplained"),
         ("sama5d27-som1-ek", "atmel,sama5d27-som1-ek"),
         ("sama5d27-wlsom1-ek", "microchip,sama5d27-wlsom1-ek"),
```

### Comparing `mpio-1.4/mpio.egg-info/PKG-INFO` & `mpio-1.5/mpio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpio
-Version: 1.4
+Version: 1.5
 Summary: Hardware access for Microchip boards
 Author: Joshua Henderson
 Author-email: joshua.henderson@microchip.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
@@ -23,18 +23,18 @@
 
    Microchip
 
 Microchip Peripheral I/O Python Package
 =======================================
 
 This package provides easy access to various hardware peripherals found
-on Microchip AT91/SAMA5 processors and Xplained boards running Linux.
-The API is clean, consistent, flexible, documented, and well tested to
-make navigating and exercising even the most complex hardware
-peripherals a trivial task.
+on Microchip AT91/SAMA5/SAMA7 processors and boards running Linux. The
+API is clean, consistent, flexible, documented, and well tested to make
+navigating and exercising even the most complex hardware peripherals a
+trivial task.
 
 Supported Interfaces
 --------------------
 
 -  ADC - Analog-to-Digital Converter
 -  DevMem - Read and Write System Memory
 -  GPIO - General Purpose I/O
```

### Comparing `mpio-1.4/pylintrc` & `mpio-1.5/pylintrc`

 * *Files identical despite different names*

### Comparing `mpio-1.4/setup.py` & `mpio-1.5/setup.py`

 * *Files identical despite different names*

