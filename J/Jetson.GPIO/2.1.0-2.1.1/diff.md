# Comparing `tmp/Jetson.GPIO-2.1.0.tar.gz` & `tmp/Jetson.GPIO-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jetson.GPIO-2.1.0.tar", last modified: Tue Feb 21 20:15:30 2023, max compression
+gzip compressed data, was "Jetson.GPIO-2.1.1.tar", last modified: Wed Apr 12 19:18:31 2023, max compression
```

## Comparing `Jetson.GPIO-2.1.0.tar` & `Jetson.GPIO-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.381009 Jetson.GPIO-2.1.0/
--rw-------   0 lhoang    (1000) lhoang    (1000)     1178 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.0/LICENSE.txt
--rw-------   0 lhoang    (1000) lhoang    (1000)       83 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.0/MANIFEST.in
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15864 2023-02-21 20:15:30.381009 Jetson.GPIO-2.1.0/PKG-INFO
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15229 2023-02-16 01:46:24.000000 Jetson.GPIO-2.1.0/README.md
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.377009 Jetson.GPIO-2.1.0/lib/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.377009 Jetson.GPIO-2.1.0/lib/python/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.377009 Jetson.GPIO-2.1.0/lib/python/Jetson/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.381009 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     1749 2023-02-16 01:46:24.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/99-gpio.rules
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-02-15 21:10:07.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/__init__.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    19821 2023-02-16 01:46:24.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     8300 2023-02-15 20:57:35.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio_cdev.py
--rw-------   0 lhoang    (1000) lhoang    (1000)    11205 2022-12-07 00:50:45.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio_event.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    28593 2023-02-15 21:10:29.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio_pin_data.py
--rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.0/lib/python/Jetson/__init__.py
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.377009 Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15864 2023-02-21 20:15:30.000000 Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/PKG-INFO
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)      531 2023-02-21 20:15:30.000000 Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/SOURCES.txt
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)        1 2023-02-21 20:15:30.000000 Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/dependency_links.txt
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       11 2023-02-21 20:15:30.000000 Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/top_level.txt
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.381009 Jetson.GPIO-2.1.0/lib/python/RPi/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-02-21 20:15:30.381009 Jetson.GPIO-2.1.0/lib/python/RPi/GPIO/
--rw-------   0 lhoang    (1000) lhoang    (1000)       44 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.0/lib/python/RPi/GPIO/__init__.py
--rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.0/lib/python/RPi/__init__.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-02-21 20:15:30.381009 Jetson.GPIO-2.1.0/setup.cfg
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     2432 2023-02-16 01:46:24.000000 Jetson.GPIO-2.1.0/setup.py
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/
+-rw-------   0 lhoang    (1000) lhoang    (1000)     1178 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/LICENSE.txt
+-rw-------   0 lhoang    (1000) lhoang    (1000)       83 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/MANIFEST.in
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15864 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/PKG-INFO
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15229 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/README.md
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/python/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/python/Jetson/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     1749 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/99-gpio.rules
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/__init__.py
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    19821 2023-04-12 19:17:23.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio.py
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     8300 2023-04-12 19:17:23.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_cdev.py
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    11205 2023-04-12 19:17:13.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_event.py
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    29648 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_pin_data.py
+-rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/__init__.py
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15864 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/PKG-INFO
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)      531 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)        1 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       11 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/top_level.txt
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/lib/python/RPi/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/lib/python/RPi/GPIO/
+-rw-------   0 lhoang    (1000) lhoang    (1000)       44 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/lib/python/RPi/GPIO/__init__.py
+-rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/lib/python/RPi/__init__.py
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/setup.cfg
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     2432 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/setup.py
```

### Comparing `Jetson.GPIO-2.1.0/LICENSE.txt` & `Jetson.GPIO-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/PKG-INFO` & `Jetson.GPIO-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jetson.GPIO
-Version: 2.1.0
+Version: 2.1.1
 Summary: A module to control Jetson GPIO channels
 Home-page: https://github.com/NVIDIA/jetson-gpio
 Author: NVIDIA
 Author-email: linux-tegra-bugs@nvidia.com
 License: MIT
 Keywords: Jetson GPIO
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `Jetson.GPIO-2.1.0/README.md` & `Jetson.GPIO-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/99-gpio.rules` & `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/99-gpio.rules`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio.py` & `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio.py`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio_cdev.py` & `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_cdev.py`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio_event.py` & `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_event.py`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson/GPIO/gpio_pin_data.py` & `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_pin_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2022, NVIDIA CORPORATION. All rights reserved.
+# Copyright (c) 2018-2023, NVIDIA CORPORATION. All rights reserved.
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
 #
@@ -26,16 +26,17 @@
 JETSON_XAVIER = 'JETSON_XAVIER'
 JETSON_TX2 = 'JETSON_TX2'
 JETSON_TX1 = 'JETSON_TX1'
 JETSON_NANO = 'JETSON_NANO'
 JETSON_TX2_NX='JETSON_TX2_NX'
 JETSON_ORIN='JETSON_ORIN'
 JETSON_ORIN_NX='JETSON_ORIN_NX'
+JETSON_ORIN_NANO='JETSON_ORIN_NANO'
 
-JETSON_MODELS = [JETSON_TX1, JETSON_TX2, CLARA_AGX_XAVIER, JETSON_TX2_NX, JETSON_XAVIER, JETSON_NANO, JETSON_NX, JETSON_ORIN, JETSON_ORIN_NX]
+JETSON_MODELS = [JETSON_TX1, JETSON_TX2, CLARA_AGX_XAVIER, JETSON_TX2_NX, JETSON_XAVIER, JETSON_NANO, JETSON_NX, JETSON_ORIN, JETSON_ORIN_NX, JETSON_ORIN_NANO]
 
 # These arrays contain tuples of all the relevant GPIO data for each Jetson
 # Platform. The fields are:
 # - Linux GPIO pin number (line offset inside chip, not global),
 # - Linux exported GPIO name,
 #   (map from chip GPIO count to value, to cater for different naming schemes)
 #   (entries omitted if exported filename is gpio%i)
@@ -72,14 +73,26 @@
     (124, 'PY.02', "tegra234-gpio", 37, 26, 'SPI1_MOSI', 'GP38_SPI3_MOSI', None, None),
     (52, 'PI.01', "tegra234-gpio", 38, 20, 'I2S0_SDIN', 'GP124', None, None),
     (51, 'PI.00', "tegra234-gpio", 40, 21, 'I2S0_SDOUT', 'GP123', None, None)
 ]
 
 compats_jetson_orins_nx = (
     "nvidia,p3509-0000+p3767-0000",
+    "nvidia,p3768-0000+p3767-0000",
+    "nvidia,p3509-0000+p3767-0001",
+    "nvidia,p3768-0000+p3767-0001",
+)
+
+compats_jetson_orins_nano = (
+    "nvidia,p3509-0000+p3767-0003",
+    "nvidia,p3768-0000+p3767-0003",
+    "nvidia,p3509-0000+p3767-0004",
+    "nvidia,p3768-0000+p3767-0004",
+    "nvidia,p3509-0000+p3767-0005",
+    "nvidia,p3768-0000+p3767-0005",
 )
 
 JETSON_ORIN_PIN_DEFS = [
     (106, 'PQ.06', "tegra234-gpio", 7, 4, 'MCLK05', 'GP66', None, None),
     # Output-only (due to base board)
     (112, 'PR.04', "tegra234-gpio", 11, 17, 'UART1_RTS', 'GP72_UART1_RTS_N', None, None),
     (50, 'PH.07', "tegra234-gpio", 12, 18, 'I2S2_CLK', 'GP122', None, None),
@@ -270,70 +283,70 @@
     'nvidia,p3489-0000',
     'nvidia,lightning',
     'nvidia,quill',
     'nvidia,storm',
 )
 
 JETSON_TX1_PIN_DEFS = [
-    (216, "tegra-gpio", 7, 4, 'AUDIO_MCLK', 'AUD_MCLK', None, None),
+    (216, '', "tegra-gpio", 7, 4, 'AUDIO_MCLK', 'AUD_MCLK', None, None),
     # Output-only (due to base board)
-    (162, "tegra-gpio", 11, 17, 'UART0_RTS', 'UART1_RTS', None, None),
-    (11, "tegra-gpio", 12, 18, 'I2S0_CLK', 'DAP1_SCLK', None, None),
-    (38, "tegra-gpio", 13, 27, 'GPIO20_AUD_INT', 'GPIO_PE6', None, None),
-    (15, "tca9539", 15, 22, 'GPIO_EXP_P17', 'GPIO_EXP_P17', None, None),
-    (37, "tegra-gpio", 16, 23, 'AO_DMIC_IN_DAT', 'DMIC3_DAT', None, None),
-    (184, "tegra-gpio", 18, 24, 'GPIO16_MDM_WAKE_AP', 'MODEM_WAKE_AP', None, None),
-    (16, "tegra-gpio", 19, 10, 'SPI1_MOSI', 'SPI1_MOSI', None, None),
-    (17, "tegra-gpio", 21, 9, 'SPI1_MISO', 'SPI1_MISO', None, None),
-    (14, "tca9539", 22, 25, 'GPIO_EXP_P16', 'GPIO_EXP_P16', None, None),
-    (18, "tegra-gpio", 23, 11, 'SPI1_CLK', 'SPI1_SCK', None, None),
-    (19, "tegra-gpio", 24, 8, 'SPI1_CS0', 'SPI1_CS0', None, None),
-    (20, "tegra-gpio", 26, 7, 'SPI1_CS1', 'SPI1_CS1', None, None),
-    (219, "tegra-gpio", 29, 5, 'GPIO19_AUD_RST', 'GPIO_X1_AUD', None, None),
-    (186, "tegra-gpio", 31, 6, 'GPIO9_MOTION_INT', 'MOTION_INT', None, None),
-    (36, "tegra-gpio", 32, 12, 'AO_DMIC_IN_CLK', 'DMIC3_CLK', None, None),
-    (63, "tegra-gpio", 33, 13, 'GPIO11_AP_WAKE_BT', 'AP_WAKE_NFC', None, None),
-    (8, "tegra-gpio", 35, 19, 'I2S0_LRCLK', 'DAP1_FS', None, None),
+    (162, '', "tegra-gpio", 11, 17, 'UART0_RTS', 'UART1_RTS', None, None),
+    (11, '',  "tegra-gpio", 12, 18, 'I2S0_CLK', 'DAP1_SCLK', None, None),
+    (38, '', "tegra-gpio", 13, 27, 'GPIO20_AUD_INT', 'GPIO_PE6', None, None),
+    (15, '', "tca9539", 15, 22, 'GPIO_EXP_P17', 'GPIO_EXP_P17', None, None),
+    (37, '', "tegra-gpio", 16, 23, 'AO_DMIC_IN_DAT', 'DMIC3_DAT', None, None),
+    (184, '', "tegra-gpio", 18, 24, 'GPIO16_MDM_WAKE_AP', 'MODEM_WAKE_AP', None, None),
+    (16, '', "tegra-gpio", 19, 10, 'SPI1_MOSI', 'SPI1_MOSI', None, None),
+    (17, '', "tegra-gpio", 21, 9, 'SPI1_MISO', 'SPI1_MISO', None, None),
+    (14, '', "tca9539", 22, 25, 'GPIO_EXP_P16', 'GPIO_EXP_P16', None, None),
+    (18, '', "tegra-gpio", 23, 11, 'SPI1_CLK', 'SPI1_SCK', None, None),
+    (19, '', "tegra-gpio", 24, 8, 'SPI1_CS0', 'SPI1_CS0', None, None),
+    (20, '', "tegra-gpio", 26, 7, 'SPI1_CS1', 'SPI1_CS1', None, None),
+    (219, '', "tegra-gpio", 29, 5, 'GPIO19_AUD_RST', 'GPIO_X1_AUD', None, None),
+    (186, '', "tegra-gpio", 31, 6, 'GPIO9_MOTION_INT', 'MOTION_INT', None, None),
+    (36, '', "tegra-gpio", 32, 12, 'AO_DMIC_IN_CLK', 'DMIC3_CLK', None, None),
+    (63, '', "tegra-gpio", 33, 13, 'GPIO11_AP_WAKE_BT', 'AP_WAKE_NFC', None, None),
+    (8, '', "tegra-gpio", 35, 19, 'I2S0_LRCLK', 'DAP1_FS', None, None),
     # Input-only (due to base board) IF NVIDIA debug card NOT plugged in
     # Input-only (due to base board) (always reads fixed value) IF NVIDIA debug card plugged in
-    (163, "tegra-gpio", 36, 16, 'UART0_CTS', 'UART1_CTS', None, None),
-    (187, "tegra-gpio", 37, 26, 'GPIO8_ALS_PROX_INT', 'ALS_PROX_INT', None, None),
-    (9, "tegra-gpio", 38, 20, 'I2S0_SDIN', 'DAP1_DIN', None, None),
-    (10, "tegra-gpio", 40, 21, 'I2S0_SDOUT', 'DAP1_DOUT', None, None)
+    (163, '', "tegra-gpio", 36, 16, 'UART0_CTS', 'UART1_CTS', None, None),
+    (187, '',  "tegra-gpio", 37, 26, 'GPIO8_ALS_PROX_INT', 'ALS_PROX_INT', None, None),
+    (9, '', "tegra-gpio", 38, 20, 'I2S0_SDIN', 'DAP1_DIN', None, None),
+    (10, '', "tegra-gpio", 40, 21, 'I2S0_SDOUT', 'DAP1_DOUT', None, None)
 ]
 compats_tx1 = (
     'nvidia,p2371-2180',
     'nvidia,jetson-cv',
 )
 
 JETSON_NANO_PIN_DEFS = [
-    (216, "tegra-gpio", 7, 4, 'GPIO9', 'AUD_MCLK', None, None),
-    (50, "tegra-gpio", 11, 17, 'UART1_RTS', 'UART2_RTS', None, None),
-    (79, "tegra-gpio", 12, 18, 'I2S0_SCLK', 'DAP4_SCLK', None, None),
-    (14, "tegra-gpio", 13, 27, 'SPI1_SCK', 'SPI2_SCK', None, None),
-    (194, "tegra-gpio", 15, 22, 'GPIO12', 'LCD_TE', None, None),
-    (232, "tegra-gpio", 16, 23, 'SPI1_CS1', 'SPI2_CS1', None, None),
-    (15, "tegra-gpio", 18, 24, 'SPI1_CS0', 'SPI2_CS0', None, None),
-    (16, "tegra-gpio", 19, 10, 'SPI0_MOSI', 'SPI1_MOSI', None, None),
-    (17, "tegra-gpio", 21, 9, 'SPI0_MISO', 'SPI1_MISO', None, None),
-    (13, "tegra-gpio", 22, 25, 'SPI1_MISO', 'SPI2_MISO', None, None),
-    (18, "tegra-gpio", 23, 11, 'SPI0_SCK', 'SPI1_SCK', None, None),
-    (19, "tegra-gpio", 24, 8, 'SPI0_CS0', 'SPI1_CS0', None, None),
-    (20, "tegra-gpio", 26, 7, 'SPI0_CS1', 'SPI1_CS1', None, None),
-    (149, "tegra-gpio", 29, 5, 'GPIO01', 'CAM_AF_EN', None, None),
-    (200, "tegra-gpio", 31, 6, 'GPIO11', 'GPIO_PZ0', None, None),
+    (216,  '', "tegra-gpio", 7, 4, 'GPIO9', 'AUD_MCLK', None, None),
+    (50,  '', "tegra-gpio", 11, 17, 'UART1_RTS', 'UART2_RTS', None, None),
+    (79, '',  "tegra-gpio", 12, 18, 'I2S0_SCLK', 'DAP4_SCLK', None, None),
+    (14,  '', "tegra-gpio", 13, 27, 'SPI1_SCK', 'SPI2_SCK', None, None),
+    (194,  '', "tegra-gpio", 15, 22, 'GPIO12', 'LCD_TE', None, None),
+    (232,  '', "tegra-gpio", 16, 23, 'SPI1_CS1', 'SPI2_CS1', None, None),
+    (15,  '', "tegra-gpio", 18, 24, 'SPI1_CS0', 'SPI2_CS0', None, None),
+    (16,  '', "tegra-gpio", 19, 10, 'SPI0_MOSI', 'SPI1_MOSI', None, None),
+    (17,  '', "tegra-gpio", 21, 9, 'SPI0_MISO', 'SPI1_MISO', None, None),
+    (13,  '', "tegra-gpio", 22, 25, 'SPI1_MISO', 'SPI2_MISO', None, None),
+    (18,  '', "tegra-gpio", 23, 11, 'SPI0_SCK', 'SPI1_SCK', None, None),
+    (19,  '', "tegra-gpio", 24, 8, 'SPI0_CS0', 'SPI1_CS0', None, None),
+    (20,  '', "tegra-gpio", 26, 7, 'SPI0_CS1', 'SPI1_CS1', None, None),
+    (149,  '', "tegra-gpio", 29, 5, 'GPIO01', 'CAM_AF_EN', None, None),
+    (200,  '', "tegra-gpio", 31, 6, 'GPIO11', 'GPIO_PZ0', None, None),
     # Older versions of L4T have a DT bug which instantiates a bogus device
     # which prevents this library from using this PWM channel.
-    (168, "tegra-gpio", 32, 12, 'GPIO07', 'LCD_BL_PW', '7000a000.pwm', 0),
-    (38, "tegra-gpio", 33, 13, 'GPIO13', 'GPIO_PE6', '7000a000.pwm', 2),
-    (76, "tegra-gpio", 35, 19, 'I2S0_FS', 'DAP4_FS', None, None),
-    (51, "tegra-gpio", 36, 16, 'UART1_CTS', 'UART2_CTS', None, None),
-    (12, "tegra-gpio", 37, 26, 'SPI1_MOSI', 'SPI2_MOSI', None, None),
-    (77, "tegra-gpio", 38, 20, 'I2S0_DIN', 'DAP4_DIN', None, None),
-    (78, "tegra-gpio", 40, 21, 'I2S0_DOUT', 'DAP4_DOUT', None, None)
+    (168,  '', "tegra-gpio", 32, 12, 'GPIO07', 'LCD_BL_PW', '7000a000.pwm', 0),
+    (38,  '', "tegra-gpio", 33, 13, 'GPIO13', 'GPIO_PE6', '7000a000.pwm', 2),
+    (76,  '', "tegra-gpio", 35, 19, 'I2S0_FS', 'DAP4_FS', None, None),
+    (51,  '', "tegra-gpio", 36, 16, 'UART1_CTS', 'UART2_CTS', None, None),
+    (12,  '', "tegra-gpio", 37, 26, 'SPI1_MOSI', 'SPI2_MOSI', None, None),
+    (77,  '', "tegra-gpio", 38, 20, 'I2S0_DIN', 'DAP4_DIN', None, None),
+    (78,  '', "tegra-gpio", 40, 21, 'I2S0_DOUT', 'DAP4_DOUT', None, None)
 ]
 compats_nano = (
     'nvidia,p3450-0000',
     'nvidia,p3450-0002',
     'nvidia,jetson-nano',
 )
 
@@ -345,14 +358,25 @@
             'RAM': '32768M, 65536M',
             'REVISION': 'Unknown',
             'TYPE': 'JETSON_ORIN_NX',
             'MANUFACTURER': 'NVIDIA',
             'PROCESSOR': 'A78AE'
         }
     ),
+    JETSON_ORIN_NANO: (
+        JETSON_ORIN_NX_PIN_DEFS,
+        {
+            'P1_REVISION': 1,
+            'RAM': '32768M, 65536M',
+            'REVISION': 'Unknown',
+            'TYPE': 'JETSON_ORIN_NANO',
+            'MANUFACTURER': 'NVIDIA',
+            'PROCESSOR': 'A78AE'
+        }
+    ),
     JETSON_ORIN: (
         JETSON_ORIN_PIN_DEFS,
         {
             'P1_REVISION': 1,
             'RAM': '32768M, 65536M',
             'REVISION': 'Unknown',
             'TYPE': 'JETSON_ORIN',
@@ -543,16 +567,19 @@
         elif matches(compats_nx):
             warn_if_not_carrier_board('3509', '3449')
             return JETSON_NX
         elif matches(compats_jetson_orins):
             warn_if_not_carrier_board('3737')
             return JETSON_ORIN
         elif matches(compats_jetson_orins_nx):
-            warn_if_not_carrier_board('3509')
+            warn_if_not_carrier_board('3509', '3768')
             return JETSON_ORIN_NX
+        elif matches(compats_jetson_orins_nano):
+            warn_if_not_carrier_board('3509', '3768')
+            return JETSON_ORIN_NANO
 
     # get model info from the environment variables for docker containers
     model_name = os.environ.get("JETSON_MODEL_NAME")
     if model_name is not None:
         model_name = model_name.strip()
         if model_name in JETSON_MODELS:
             return model_name
```

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/PKG-INFO` & `Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jetson.GPIO
-Version: 2.1.0
+Version: 2.1.1
 Summary: A module to control Jetson GPIO channels
 Home-page: https://github.com/NVIDIA/jetson-gpio
 Author: NVIDIA
 Author-email: linux-tegra-bugs@nvidia.com
 License: MIT
 Keywords: Jetson GPIO
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `Jetson.GPIO-2.1.0/lib/python/Jetson.GPIO.egg-info/SOURCES.txt` & `Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.0/setup.py` & `Jetson.GPIO-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                'Intended Audience :: Developers',
                'Programming Language :: Python :: 2.7',
                'Programming Language :: Python :: 3',
                'Topic :: Software Development',
                'Topic :: System :: Hardware']
 
 setup(name                          = 'Jetson.GPIO',
-      version                       = '2.1.0',
+      version                       = '2.1.1',
       author                        = 'NVIDIA',
       author_email                  = 'linux-tegra-bugs@nvidia.com',
       description                   = 'A module to control Jetson GPIO channels',
       long_description              = open('README.md').read(),
       long_description_content_type = 'text/markdown',
       license                       = 'MIT',
       keywords                      = 'Jetson GPIO',
```

