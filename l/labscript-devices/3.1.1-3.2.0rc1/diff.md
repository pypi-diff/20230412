# Comparing `tmp/labscript-devices-3.1.1.tar.gz` & `tmp/labscript-devices-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labscript-devices-3.1.1.tar", last modified: Wed Dec 15 13:44:51 2021, max compression
+gzip compressed data, was "labscript-devices-3.2.0rc1.tar", last modified: Wed Apr 12 19:48:14 2023, max compression
```

## Comparing `labscript-devices-3.1.1.tar` & `labscript-devices-3.2.0rc1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.937421 labscript-devices-3.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.941421 labscript-devices-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     9106 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      929 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (121)     9659 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8669 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.941421 labscript-devices-3.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.941421 labscript-devices-3.1.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.941421 labscript-devices-3.1.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.941421 labscript-devices-3.1.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.941421 labscript-devices-3.1.1/docs/source/_templates/models/
--rw-r--r--   0 runner    (1001) docker     (121)      996 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/_templates/models/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/adding_devices.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10251 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.945421 labscript-devices-3.1.1/docs/source/devices/
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/IMAQdx.rst
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/alazartechboard.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/andorsolis.rst
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/dummyintermediate.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/dummypseudoclock.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/flycapture2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/functionrunner.rst
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/lightcrafterdmd.rst
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/ni_daq_models.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5747 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/ni_daqs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/novatechDDS9m.rst
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/opalkellyXEM3001.rst
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/phasematrixquicksyn.rst
--rw-r--r--   0 runner    (1001) docker     (121)      390 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/pineblaster.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/prawnblaster.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/pulseblaster.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/pulseblaster_no_dds.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6561 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/pylon.rst
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/rfblaster.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/spinnaker.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/tekscope.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/testdevice.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices/zaberstagecontroller.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/devices.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/ex_conn_tables.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.945421 labscript-devices-3.1.1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    98716 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/labscript.ico
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7413 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/labscript_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12665 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14435 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13201 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)    64143 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/docs/source/user_devices.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.949421 labscript-devices-3.1.1/labscript_devices/
--rw-r--r--   0 runner    (1001) docker     (121)    34928 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AlazarTechBoard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.949421 labscript-devices-3.1.1/labscript_devices/AndorSolis/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.949421 labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)     4195 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    64381 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_solis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    27658 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5214 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/AndorSolis/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    14617 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/Camera.py
--rw-r--r--   0 runner    (1001) docker     (121)    34845 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/CiceroOpalKellyXEM3001.py
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyIntermediateDevice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.949421 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5977 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/runviewer_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.949421 labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20501 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.953421 labscript-devices-3.1.1/labscript_devices/FunctionRunner/
--rw-r--r--   0 runner    (1001) docker     (121)      839 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4308 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.953421 labscript-devices-3.1.1/labscript_devices/FunctionRunner/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/testing/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/FunctionRunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.953421 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/attributes_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5686 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/blacs_tab.ui
--rw-r--r--   0 runner    (1001) docker     (121)    12811 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21859 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11313 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.953421 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      993 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/testing/test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16904 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/LightCrafterDMD.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.953421 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/
--rw-r--r--   0 runner    (1001) docker     (121)      839 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9746 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    40969 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5317 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/daqmx_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    28997 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/labscript_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6008.py
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6229.py
--rw-r--r--   0 runner    (1001) docker     (121)     3748 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6343.py
--rw-r--r--   0 runner    (1001) docker     (121)     3752 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6363.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6366.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/_subclass_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    43041 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/capabilities.json
--rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/generate_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)    24733 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/runviewer_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_DAQmx/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_PCI_6733.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_PCIe_6363.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NI_USB_6343.py
--rw-r--r--   0 runner    (1001) docker     (121)    32152 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/NovaTechDDS9M.py
--rw-r--r--   0 runner    (1001) docker     (121)    16193 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PhaseMatrixQuickSyn.py
--rw-r--r--   0 runner    (1001) docker     (121)    15427 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PineBlaster.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6052 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18525 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19713 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PrawnBlaster/runviewer_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    69933 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PulseBlaster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PulseBlasterESRPro200.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PulseBlasterESRPro500.py
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PulseBlasterUSB.py
--rw-r--r--   0 runner    (1001) docker     (121)    22696 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PulseBlaster_No_DDS.py
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PulseBlaster_SP2_24_100_32k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/PylonCamera/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PylonCamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PylonCamera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7922 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PylonCamera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PylonCamera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PylonCamera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/PylonCamera/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     5288 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PylonCamera/testing/ExposureTiming.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/PythonCamera.py
--rw-r--r--   0 runner    (1001) docker     (121)    25523 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/RFBlaster.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11349 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/TekScope/
--rw-r--r--   0 runner    (1001) docker     (121)     7246 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/TekScope/TekScope.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/TekScope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/TekScope/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/TekScope/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/TekScope/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/TekScope/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/ZaberStageController/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.957420 labscript-devices-3.1.1/labscript_devices/ZaberStageController/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/testing/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/ZaberStageController/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    44881 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/atsapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/camera.ui
--rw-r--r--   0 runner    (1001) docker     (121)    19575 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/imaqdx_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/phasematrixquicksyn.ui
--rw-r--r--   0 runner    (1001) docker     (121)     7307 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/pulseblaster.ui
--rw-r--r--   0 runner    (1001) docker     (121)      761 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/labscript_devices/test_device.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 13:44:51.949421 labscript-devices-3.1.1/labscript_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9659 2021-12-15 13:44:51.000000 labscript-devices-3.1.1/labscript_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7813 2021-12-15 13:44:51.000000 labscript-devices-3.1.1/labscript_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 13:44:51.000000 labscript-devices-3.1.1/labscript_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 13:44:51.000000 labscript-devices-3.1.1/labscript_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-12-15 13:44:51.000000 labscript-devices-3.1.1/labscript_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-15 13:44:51.000000 labscript-devices-3.1.1/labscript_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-12-15 13:44:51.961420 labscript-devices-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-12-15 13:44:46.000000 labscript-devices-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.654699 labscript-devices-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/_templates/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/_templates/models/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/adding_devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.662700 labscript-devices-3.2.0rc1/docs/source/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/IMAQdx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/alazartechboard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/andorsolis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/dummyintermediate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/dummypseudoclock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/flycapture2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/functionrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/lightcrafterdmd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/ni_daq_models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/ni_daqs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/novatechDDS9m.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/opalkellyXEM3001.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/phasematrixquicksyn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pineblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/prawnblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster_no_dds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pylon.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/rfblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/spinnaker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/tekscope.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/testdevice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/zaberstagecontroller.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/ex_conn_tables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.662700 labscript-devices-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/labscript.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/labscript_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/user_devices.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.666700 labscript-devices-3.2.0rc1/labscript_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    34928 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AlazarTechBoard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64381 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_solis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/Camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34845 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/CiceroOpalKellyXEM3001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyIntermediateDevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/runviewer_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/testing/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/attributes_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/testing/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/LightCrafterDMD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42192 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/daqmx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/labscript_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6229.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6343.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6366.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/_subclass_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43041 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/generate_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24733 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/runviewer_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_PCI_6733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_PCIe_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_USB_6343.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32545 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NovaTechDDS9M.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PhaseMatrixQuickSyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PineBlaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/runviewer_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69933 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterUSB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_No_DDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_SP2_24_100_32k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/testing/ExposureTiming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PythonCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25523 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/RFBlaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/TekScope/
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/TekScope.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/testing/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44881 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/atsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/camera.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/imaqdx_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/phasematrixquicksyn.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/pulseblaster.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/test_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.666700 labscript-devices-3.2.0rc1/labscript_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/setup.py
```

### Comparing `labscript-devices-3.1.1/.github/workflows/release.yml` & `labscript-devices-3.2.0rc1/.github/workflows/release.yml`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,14 @@
     branches:
       - master
       - maintenance/*
   create:
     tags:
       - 'v[0-9]+.[0-9]+.[0-9]+*'
 
-defaults:
-  run:
-    shell: bash
-
 env:
   PACKAGE_NAME: labscript-devices
   SCM_LOCAL_SCHEME: no-local-version
   ANACONDA_USER: labscript-suite
 
   # Configuration for a package with compiled extensions:
   # PURE: false
@@ -37,238 +33,224 @@
 jobs:
   build:
     name: Build
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
-          - { os: ubuntu-latest,   python: 3.8,  arch: x64 }
-          # - { os: ubuntu-latest,   python: 3.7,  arch: x64 }
-          # - { os: ubuntu-latest,   python: 3.6,  arch: x64 }
-
-          # - { os: macos-latest,    python: 3.8,  arch: x64 }
-          # - { os: macos-latest,    python: 3.7,  arch: x64 }
-          # - { os: macos-latest,    python: 3.6,  arch: x64 }
-
-          # - { os: windows-latest,  python: 3.8,  arch: x64 }
-          # - { os: windows-latest,  python: 3.7,  arch: x64 }
-          # - { os: windows-latest,  python: 3.6,  arch: x64 }
-
-          # - { os: windows-latest,  python: 3.8,  arch: x86 }
-          # - { os: windows-latest,  python: 3.7,  arch: x86 }
-          # - { os: windows-latest,  python: 3.6,  arch: x86 }
+          - { os: ubuntu-latest,   python: '3.11',  arch: x64, conda: true}
+          # - { os: ubuntu-latest,   python: '3.10',  arch: x64, conda: true }
+          # - { os: ubuntu-latest,   python: '3.9',  arch: x64, conda: true }
+          # - { os: ubuntu-latest,   python: '3.8',  arch: x64, conda: true }
+          # - { os: ubuntu-latest,   python: '3.7',  arch: x64, conda: true }
+
+          # - { os: macos-11,    python: '3.11',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.10',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.9',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.8',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.7',  arch: x64, conda: true }
+
+          # - { os: windows-latest,  python: '3.11',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.10',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.9',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.8',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.7',  arch: x64, conda: true }
+
+          # - { os: windows-latest,  python: '3.11',  arch: x86, conda: false } # conda not yet available
+          # - { os: windows-latest,  python: '3.10',  arch: x86, conda: true }
+          # - { os: windows-latest,  python: '3.9',  arch: x86, conda: true }
+          # - { os: windows-latest,  python: '3.8',  arch: x86, conda: true }
+          # - { os: windows-latest,  python: '3.7',  arch: x86, conda: true }
 
     if: github.repository == 'labscript-suite/labscript-devices' && (github.event_name != 'create' || github.event.ref_type != 'branch')
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Ignore Tags
         if: github.event.ref_type != 'tag'
         run: git tag -d $(git tag --points-at HEAD)
 
       - name: Install Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           architecture: ${{ matrix.arch }}
 
       - name: Source Distribution
         if: strategy.job-index == 0
         run: |
-          python -m pip install --upgrade pip setuptools wheel pep517
-          python -m pep517.build -s .
+          python -m pip install --upgrade pip setuptools wheel build
+          python -m build -s .
 
       - name: Wheel Distribution
         # Impure Linux wheels are built in the manylinux job.
         if: (env.PURE == 'true' && strategy.job-index == 0) || (env.PURE == 'false' && runner.os != 'Linux')
         run: |
-          python -m pip install --upgrade pip setuptools wheel pep517
-          python -m pep517.build -b .
+          python -m pip install --upgrade pip setuptools wheel build
+          python -m build -w .
 
       - name: Upload Artifact
         if: strategy.job-index == 0 || (env.PURE == 'false' && runner.os != 'Linux')
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
           path: ./dist
 
       - name: Set Variables for Conda Build
+        if: matrix.conda
+        shell: bash
         run: |
-          if [ $RUNNER_OS == Windows ] && [ ${{ matrix.arch }} == x64 ]; then
-              CONDA_INSTALLER=Miniconda3-latest-Windows-x86_64.exe
-          elif [ $RUNNER_OS == Windows ]; then
-              CONDA_INSTALLER=Miniconda3-latest-Windows-x86.exe
-          elif [ $RUNNER_OS == Linux ]; then
-              CONDA_INSTALLER=Miniconda3-latest-Linux-x86_64.sh
-          else
-              CONDA_INSTALLER=Miniconda3-latest-MacOSX-x86_64.sh
-          fi
           if [ $NOARCH == true ]; then
               CONDA_BUILD_ARGS="--noarch"
           else
               CONDA_BUILD_ARGS=""
           fi
-          echo "CONDA_INSTALLER=$CONDA_INSTALLER" >> $GITHUB_ENV
           echo "CONDA_BUILD_ARGS=$CONDA_BUILD_ARGS" >> $GITHUB_ENV
 
+      - name: Install Miniconda
+        if: matrix.conda
+        uses: conda-incubator/setup-miniconda@v2
+        with:
+          auto-update-conda: true
+          python-version: ${{ matrix.python }}
+          architecture: ${{ matrix.arch }}
+          miniconda-version: "latest"
+
+      - name: Workaround conda-build incompatibility with xcode 12+
+        if: runner.os == 'macOS'
+        uses: maxim-lobanov/setup-xcode@v1
+        with:
+          xcode-version: 11.7
+
       - name: Conda package (Unix)
-        if: runner.os != 'Windows'
+        if: (matrix.conda && runner.os != 'Windows')
+        shell: bash -l {0}
         run: |
-          curl -LO https://repo.continuum.io/miniconda/$CONDA_INSTALLER
-          bash "$CONDA_INSTALLER" -b -p .miniconda
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
-          conda update -n base -c defaults conda
-          conda create -n py${{ matrix.python }} python=${{ matrix.python }}
-          conda activate py${{ matrix.python }}
-          conda install -c cbillington setuptools-conda
-          pip install --upgrade setuptools_scm
+          conda install -c labscript-suite setuptools-conda
           setuptools-conda build $CONDA_BUILD_ARGS .
 
       - name: Conda Package (Windows)
-        if: runner.os == 'Windows'
-        shell: cmd
+        if: (matrix.conda && runner.os == 'Windows')
+        shell: cmd /C CALL {0}
         run: |
-          curl -LO https://repo.continuum.io/miniconda/%CONDA_INSTALLER%
-          %CONDA_INSTALLER% /S /D=%CD%\.miniconda && ^
-          .miniconda\Scripts\activate && ^
-          conda update -n base -c defaults conda && ^
-          conda create -n py${{ matrix.python }} python=${{ matrix.python }} && ^
-          conda activate py${{ matrix.python }} && ^
-          conda install -c cbillington setuptools-conda && ^
-          pip install --upgrade setuptools_scm && ^
-          setuptools-conda build %CONDA_BUILD_ARGS% .
+          conda install -c labscript-suite setuptools-conda && ^
+          setuptools-conda build %CONDA_BUILD_ARGS% --croot ${{ runner.temp }}\cb .
 
       - name: Upload Artifact
-        uses: actions/upload-artifact@v2
+        if: matrix.conda
+        uses: actions/upload-artifact@v3
         with:
           name: conda_packages
           path: ./conda_packages
 
 
   manylinux:
     name: Build Manylinux
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        include:
-          - { python: 'cp36-cp36m cp37-cp37m cp38-cp38' }
-
     if: github.repository == 'labscript-suite/labscript-devices' && (github.event_name != 'create' || github.event.ref_type != 'branch')
     steps:
       - name: Checkout
         if: env.PURE == 'false'
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Ignore Tags
         if: github.event.ref_type != 'tag' && env.PURE == 'false'
         run: git tag -d $(git tag --points-at HEAD)
 
       - name: Build Manylinux Wheels
         if: env.PURE == 'false'
-        uses: RalfG/python-wheels-manylinux-build@v0.2.2-manylinux2010_x86_64
+        uses: RalfG/python-wheels-manylinux-build@v0.4.2
         with:
-          python-versions: ${{ matrix.python }}
+          python-versions: 'cp37-cp37m cp38-cp38 cp39-cp39 cp310-cp310 cp311-cp311'
+          pre-build-command: 'git config --global --add safe.directory "*"'
 
       - name: Upload Artifact
         if: env.PURE == 'false'
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
-          path: wheelhouse/*manylinux*.whl
+          path: dist/*manylinux*.whl
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: [build, manylinux]
     steps:
 
       - name: Download Artifact
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: dist
           path: ./dist
 
       - name: Download Artifact
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: conda_packages
           path: ./conda_packages
 
-      - name: Publish on TestPyPI
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          user: __token__
-          password: ${{ secrets.testpypi }}
-          repository_url: https://test.pypi.org/legacy/
-
       - name: Get Version Number
         if: github.event.ref_type == 'tag'
         run: |
           VERSION="${GITHUB_REF/refs\/tags\/v/}"
           echo "VERSION=$VERSION" >> $GITHUB_ENV
 
-      - name: Create GitHub Release
+      - name: Create GitHub Release and Upload Release Asset
         if: github.event.ref_type == 'tag'
-        id: create_release
-        uses: actions/create-release@latest
+        uses: softprops/action-gh-release@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: ${{ github.event.ref }}
-          release_name: ${{ env.PACKAGE_NAME }} ${{ env.VERSION }}
+          name: ${{ env.PACKAGE_NAME }} ${{ env.VERSION }}
           draft: true
           prerelease: ${{ contains(github.event.ref, 'rc') }}
+          files: ./dist/${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
 
-      - name: Upload Release Asset
-        if: github.event.ref_type == 'tag'
-        uses: actions/upload-release-asset@v1
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      - name: Publish on TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          upload_url: ${{ steps.create_release.outputs.upload_url }}
-          asset_path: ./dist/${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
-          asset_name: ${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
-          asset_content_type: application/gzip
+          user: __token__
+          password: ${{ secrets.testpypi }}
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish on PyPI
         if: github.event.ref_type == 'tag'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi }}
 
-      - name: Install Miniconda and cloud client
-        run: |
-          curl -LO https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh 
-          bash Miniconda3-latest-Linux-x86_64.sh -b -p .miniconda
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
-          conda install anaconda-client
+      - name: Install Miniconda
+        uses: conda-incubator/setup-miniconda@v2
+        with:
+          auto-update-conda: true
+
+      - name: Install Anaconda cloud client
+        shell: bash -l {0}
+        run: conda install anaconda-client
 
       - name: Publish to Anaconda test label
         if: github.event.ref_type != 'tag'
+        shell: bash -l {0}
         run: |
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
           anaconda \
             --token ${{ secrets.ANACONDA_API_TOKEN }} \
             upload \
             --user $ANACONDA_USER \
             --label test \
             conda_packages/*/*
 
       - name: Publish to Anaconda main label
+        shell: bash -l {0}
         if: github.event.ref_type == 'tag'
         run: |
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
           anaconda \
             --token ${{ secrets.ANACONDA_API_TOKEN }} \
             upload \
             --user $ANACONDA_USER \
             conda_packages/*/*
```

### Comparing `labscript-devices-3.1.1/.gitignore` & `labscript-devices-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/BSD-2-CLAUSE-LICENSE.txt` & `labscript-devices-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/BSD-3-CLAUSE-LICENSE.txt` & `labscript-devices-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/LICENSE.txt` & `labscript-devices-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/NEWS.md` & `labscript-devices-3.2.0rc1/NEWS.md`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/PKG-INFO` & `labscript-devices-3.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: labscript-devices
-Version: 3.1.1
+Version: 3.2.0rc1
 Summary: Device drivers for hardware controlled by the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-devices
 Project-URL: Download, https://github.com/labscript-suite/labscript-devices/releases
 Project-URL: Tracker, https://github.com/labscript-suite/labscript-devices/issues
 Keywords: experiment control automation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite" align="right">
 
@@ -94,9 +95,7 @@
 
 † We do not endorse the use of any particular hardware.
 
 
 ## Installation
 
 labscript-devices is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `labscript-devices-3.1.1/README.md` & `labscript-devices-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/Makefile` & `labscript-devices-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/make.bat` & `labscript-devices-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/_static/custom.css` & `labscript-devices-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/_templates/components.rst` & `labscript-devices-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/_templates/models/package.rst_t` & `labscript-devices-3.2.0rc1/docs/source/_templates/models/package.rst_t`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/adding_devices.rst` & `labscript-devices-3.2.0rc1/docs/source/adding_devices.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 ~~~~~~~~~~~~~~~~
 
 As a general rule, it is best to model new hardware implementations off of a currently implemented device that has similar functionality.
 If the functionality is similar enough, it may even be possible to simply sub-class the currently implemented device, which is likely preferrable.
 
 Barring the above simple solution, one must work from scratch.
 It is best to begin by determining the **labscript** device class to inherit from: `Psuedoclock`, `Device`, `IntermediateDevice`.
-The first is for implementing Psuedoclock devices, the second is for generic devices that are not hardware timed by a pseudoclock, and the last is for hardware timed device that are connected to another device controlled via labscript.
+The first is for implementing Psuedoclock devices, the second is for generic devices that are not hardware timed by a pseudoclock, and the last is for hardware timed devices that are connected to another device controlled via labscript.
 
 The `labscript_device` implements general configuration parameters, many of which are passed to the `BLACS_worker`.
 It also implements the `generate_code` method which converts **labscript** high-level instructions and saves them to the h5 file.
 
 The `BLACS_tab` defines the GUI widgets that control the device.
-This typically takes the form of using standard widgets provided by **labscript** for controlling **labscript** output primitives (ie `AnalogOut`, `DigitalOut`,`DDS`, etc).
+This typically takes the form of using standard widgets provided by **labscript** for controlling **labscript** output primitives (ie `AnalogOut`, `DigitalOut`, `DDS`, etc).
 This configuration is done in the `initialiseGUI` method.
-This also links directly to the appropriate BLACS workers.
+This also specifies which BLACS workers to use and provides necessary instantiation arguments.
 
 The `BLACS_worker` handles communication with the hardware itself and often represents the bulk of the work required to implement a new labscript device.
 In general, it should provide five different methods:
 
-* `init`: This method initialised communications with the device. Not to be confused with the standard python class `__init__` method.
+* `init`: This method initialises communications with the device. Not to be confused with the standard python class `__init__` method.
 * `program_manual`: This method allows for user control of the device via the `BLACS_tab`, setting outputs to the values set in the `BLACS_tab` widgets.
 * `check_remote_values`: This method reads the current settings of the device, updating the `BLACS_tab` widgets to reflect these values.
 * `transition_to_buffered`: This method transitions the device to buffered shot mode, reading the shot h5 file and taking the saved instructions from `labscript_device.generate_code` and sending the appropriate commands to the hardware.
-* `transition_to_manual`: This method transitions the device from buffered to manual mode. It does any necessary configuration to take the device out of buffered mode and is used to read an measurements and save them to the shot h5 file as results.
+* `transition_to_manual`: This method transitions the device from buffered to manual mode. It does any necessary configuration to take the device out of buffered mode and is used to read any measurements and save them to the shot h5 file as results.
 
 The `runviewer_parser` takes shot h5 files, reads the saved instructions, and allows you to view them in **runviewer** in order to visualise experiment timing.
 
 Code Organization
 ~~~~~~~~~~~~~~~~~
 
 There are currently two supported file organization styles for a labscript-device. 
 
 The old style has the `labscript_device`, `BLACS_tab`, `BLACS_worker`, and `runviewer_parser` all in the same file, which typically has the same name as the `labscript_device` class name.
 
 The new style allows for arbitrary code organization, but typically has a folder named after the `labscript_device` with each device component in a different file (ie `labscript_devices.py`, `BLACS_workers.py`, etc).
 With this style, the folder requires an `__init__.py` file (which can be empty) as well as a `register_classes.py` file.
-This file imports :obj:`<labscript-utils:labscript_utils.device_registry>` via
+This file imports :mod:`labscript-utils:labscript_utils.device_registry` via
 
 .. code-block:: python
 
 	from labscript_devices import register_classes
 
 This function informs **labscript** where to find the necessary classes during import. An example for the `NI_DAQmx` device is
```

### Comparing `labscript-devices-3.1.1/docs/source/conf.py` & `labscript-devices-3.2.0rc1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     "sphinx.ext.viewcode",
     "sphinx_rtd_theme",
     "recommonmark",
 ]
 
 autodoc_typehints = 'description'
 autoclass_content = 'both'  # options: 'both', 'class', 'init'
-autodoc_mock_imports = ['PyDAQmx']
+autodoc_mock_imports = ['PyDAQmx','labscript_utils']
 
 # Prefix each autosectionlabel with the name of the document it is in and a colon
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -71,23 +71,23 @@
 master_doc = 'index'
 
 # intersphinx allows us to link directly to other repos sphinxdocs.
 # https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
+    'scipy': ('https://docs.scipy.org/doc/scipy/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
     'qtutils': ('https://qtutils.readthedocs.io/en/stable/', None),
     'pyqtgraph': (
         'https://pyqtgraph.readthedocs.io/en/latest/',
         None,
     ),  # change to stable once v0.11 is published
-    'matplotlib': ('https://matplotlib.org/', None),
-    'h5py': ('http://docs.h5py.org/en/stable/', None),
+    'matplotlib': ('https://matplotlib.org/stable/', None),
+    'h5py': ('https://docs.h5py.org/en/stable/', None),
     'pydaqmx': ('https://pythonhosted.org/PyDAQmx/', None),
     'qt': (
         '',
         'pyqt5-modified-objects.inv',
     )  # from https://github.com/MSLNZ/msl-qt/blob/master/docs/create_pyqt_objects.py
     # under MIT License
     # TODO
```

### Comparing `labscript-devices-3.1.1/docs/source/devices/IMAQdx.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/IMAQdx.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/alazartechboard.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/alazartechboard.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/andorsolis.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/andorsolis.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/dummypseudoclock.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/dummypseudoclock.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/flycapture2.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/flycapture2.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/functionrunner.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/functionrunner.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/opalkellyXEM3001.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/opalkellyXEM3001.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/prawnblaster.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/prawnblaster.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/pulseblaster.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/pulseblaster_no_dds.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster_no_dds.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/pylon.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/pylon.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/spinnaker.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/spinnaker.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/tekscope.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/tekscope.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices/zaberstagecontroller.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/zaberstagecontroller.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/devices.rst` & `labscript-devices-3.2.0rc1/docs/source/devices.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/ex_conn_tables.rst` & `labscript-devices-3.2.0rc1/docs/source/ex_conn_tables.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/blacs_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/labscript.ico` & `labscript-devices-3.2.0rc1/docs/source/img/labscript.ico`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/labscript_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/labscript_64x64.svg` & `labscript-devices-3.2.0rc1/docs/source/img/labscript_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/lyse_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/runmanager_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/img/runviewer_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/index.rst` & `labscript-devices-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/introduction.rst` & `labscript-devices-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/pyqt5-modified-objects.inv` & `labscript-devices-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/docs/source/user_devices.rst` & `labscript-devices-3.2.0rc1/docs/source/user_devices.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AlazarTechBoard.py` & `labscript-devices-3.2.0rc1/labscript_devices/AlazarTechBoard.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_solis.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_solis.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_structures.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_structures.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/andor_utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/andor_sdk/status_codes.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/status_codes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class AndorCamera(object):
 
     def __init__(self):
         global AndorCam
         from .andor_sdk.andor_utils import AndorCam
         self.camera = AndorCam()
         self.attributes = self.camera.default_acquisition_attrs
+        self.exception_on_failed_shot = True
 
     def set_attributes(self, attr_dict):
         self.attributes.update(attr_dict)
         
     def set_attribute(self, name, value):
         self.attributes[name] = value
```

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/AndorSolis/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/Camera.py` & `labscript-devices-3.2.0rc1/labscript_devices/Camera.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/CiceroOpalKellyXEM3001.py` & `labscript-devices-3.2.0rc1/labscript_devices/CiceroOpalKellyXEM3001.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyIntermediateDevice.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyIntermediateDevice.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/DummyPseudoclock/runviewer_parsers.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/runviewer_parsers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_workers.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,16 @@
         fmts = {prop:getattr(PyCapture2.PIXEL_FORMAT,prop) 
                 for prop in dir(PyCapture2.PIXEL_FORMAT) 
                 if not prop.startswith('_')}
                 
         self.pixel_formats = IntEnum('pixel_formats',fmts)
 
         self._abort_acquisition = False
-        
+        self.exception_on_failed_shot = True
+
         # check if GigE camera. If so, ensure max packet size is used
         cam_info = self.camera.getCameraInfo()
         if cam_info.interfaceType == PyCapture2.INTERFACE_TYPE.GIGE:
             # need to close generic camera first to avoid strange interactions
             print('Checking Packet size for GigE Camera...')
             self.camera.disconnect()
             gige_camera = PyCapture2.GigECamera()
```

### Comparing `labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FlyCapture2Camera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/testing/test.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/testing/test.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/FunctionRunner/utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/attributes_dialog.ui` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/attributes_dialog.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/blacs_tab.ui` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tab.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         # priority to ensure all other occur before our next call to self.handler()
         # runs. This may be because the CallEvents used by qtutils.invoke_in_main have
         # their own event handler (qtutils.invoke_in_main.Caller), perhaps posted event
         # priorities are only meaningful within the context of a single event handler,
         # and not for the Qt event loop as a whole. In any case, this seems to fix it.
         # Manually calling this is usually a sign of bad coding, but I think it is the
         # right solution to this problem. This solves issue #36.
-        QtGui.QApplication.instance().sendPostedEvents()
+        QtWidgets.QApplication.instance().sendPostedEvents()
         return self.NO_RESPONSE
 
 
 class IMAQdxCameraTab(DeviceTab):
     # Subclasses may override this if all they do is replace the worker class with a
     # different one:
     worker_class = 'labscript_devices.IMAQdxCamera.blacs_workers.IMAQdxCameraWorker' 
@@ -138,15 +138,15 @@
             self.on_attr_visibility_level_changed
         )
         self.ui.doubleSpinBox_maxrate.valueChanged.connect(self.on_max_rate_changed)
 
         layout.addWidget(self.ui)
         self.image = pg.ImageView()
         self.image.setSizePolicy(
-            QtGui.QSizePolicy.Expanding, QtGui.QSizePolicy.Expanding
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding
         )
         self.ui.horizontalLayout.addWidget(self.image)
         self.ui.pushButton_stop.hide()
         self.ui.doubleSpinBox_maxrate.hide()
         self.ui.toolButton_nomax.hide()
         self.ui.label_fps.hide()
```

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 class MockCamera(object):
     """Mock camera class that returns fake image data."""
 
     def __init__(self):
         print("Starting device worker as a mock device")
         self.attributes = {}
+        self.exception_on_failed_shot = True
 
     def set_attributes(self, attributes):
         self.attributes.update(attributes)
 
     def get_attribute(self, name):
         return self.attributes[name]
 
@@ -135,14 +136,15 @@
         # Connect to the camera:
         print("Connecting to camera...")
         self.imaqdx = nv.IMAQdxOpenCamera(
             self.camera.InterfaceName, nv.IMAQdxCameraControlModeController
         )
         # Keep an img attribute so we don't have to create it every time
         self.img = nv.imaqCreateImage(nv.IMAQ_IMAGE_U16)
+        self.exception_on_failed_shot = True
         self._abort_acquisition = False
 
     def set_attributes(self, attr_dict):
         for k, v in attr_dict.items():
             self.set_attribute(k, v)
 
     def set_attribute(self, name, value):
@@ -169,15 +171,15 @@
         attributes = []
         for a in nv.IMAQdxEnumerateAttributes2(self.imaqdx, b'', visibility_level):
             if writeable_only and not a.Writable:
                 continue
             if not a.Readable:
                 continue
             attributes.append(a.Name.decode('utf8'))
-        return sorted(attributes)
+        return attributes
 
     def get_attribute(self, name):
         """Return current value of attribute of the given name"""
         try:
             value = nv.IMAQdxGetAttribute(self.imaqdx, name.encode('utf8'))
             if isinstance(value, nv.core.IMAQdxEnumItem):
                 value = value.Name
@@ -215,15 +217,24 @@
                     images.append(self.grab(waitForNextBuffer))
                     print(f"Got image {i+1} of {n_images}.")
                     break
                 except nv.ImaqDxError as e:
                     if e.code == nv.IMAQdxErrorTimeout.value:
                         print('.', end='')
                         continue
-                    raise
+                    
+                    if self.exception_on_failed_shot:
+                        raise
+                    else:
+                        # stop acquisition
+                        print(e, file=sys.stderr)
+                        break
+                    
+                    
+                    
         print(f"Got {len(images)} of {n_images} images.")
 
     def stop_acquisition(self):
         nv.IMAQdxStopAcquisition(self.imaqdx)
         nv.IMAQdxUnconfigureAcquisition(self.imaqdx)
 
     def abort_acquisition(self):
@@ -381,14 +392,15 @@
             properties = labscript_utils.properties.get(
                 f, self.device_name, 'device_properties'
             )
             camera_attributes = properties['camera_attributes']
             self.stop_acquisition_timeout = properties['stop_acquisition_timeout']
             self.exception_on_failed_shot = properties['exception_on_failed_shot']
             saved_attr_level = properties['saved_attribute_visibility_level']
+            self.camera.exception_on_failed_shot = self.exception_on_failed_shot
         # Only reprogram attributes that differ from those last programmed in, or all of
         # them if a fresh reprogramming was requested:
         if fresh:
             self.smart_cache = {}
         self.set_attributes_smart(camera_attributes)
         # Get the camera attributes, so that we can save them to the H5 file:
         if saved_attr_level is not None:
```

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/labscript_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     description = 'IMAQdx Camera'
 
     @set_passed_properties(
         property_names={
             "connection_table_properties": [
                 "serial_number",
                 "orientation",
+                "pixel_size",
+                "magnification",
                 "manual_mode_camera_attributes",
                 "mock",
             ],
             "device_properties": [
                 "camera_attributes",
                 "stop_acquisition_timeout",
                 "exception_on_failed_shot",
@@ -40,14 +42,16 @@
     def __init__(
         self,
         name,
         parent_device,
         connection,
         serial_number,
         orientation=None,
+        pixel_size=[1.0,1.0],
+        magnification=1.0,
         trigger_edge_type='rising',
         trigger_duration=None,
         minimum_recovery_time=0.0,
         camera_attributes=None,
         manual_mode_camera_attributes=None,
         stop_acquisition_timeout=5.0,
         exception_on_failed_shot=True,
@@ -72,14 +76,22 @@
                 camera's serial number. This will be used to idenitfy the camera.
 
             orientation (str, optional), default: `<name>`
                 Description of the camera's location or orientation. This will be used
                 to determine the location in the shot file where the images will be
                 saved. If not given, the device name will be used instead.
 
+            pixel_size ([float,float], optional), default: `[1.0, 1.0]`
+                The x and y size of the pixels in micrometers.  This can be used 
+                in setting the scale in the blacs image display as well as 
+                extracted in lyse for analysis.
+
+            magnification (float, optional), default: `1.0`
+                Imaging system magnification.
+
             trigger_edge_type (str), default: `'rising'`
                 The direction of the desired edges to be generated on the parent
                 devices's digital output used for triggering. Must be 'rising' or
                 'falling'. Note that this only determines the edges created on the
                 parent device, it does not program the camera to expect this type of
                 edge. If required, one must configure the camera separately via
                 `camera_attributes` to ensure it expects the type of edge being
@@ -141,14 +153,16 @@
             **kwargs: Further keyword arguments to be passed to the `__init__` method of
                 the parent class (TriggerableDevice).
         """
         self.trigger_edge_type = trigger_edge_type
         self.minimum_recovery_time = minimum_recovery_time
         self.trigger_duration = trigger_duration
         self.orientation = orientation
+        self.pixel_size = pixel_size
+        self.magnification = magnification
         if isinstance(serial_number, (str, bytes)):
             serial_number = int(serial_number, 16)
         self.serial_number = serial_number
         self.BLACS_connection = hex(self.serial_number)[2:].upper()
         if camera_attributes is None:
             camera_attributes = {}
         if manual_mode_camera_attributes is None:
```

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/IMAQdxCamera/testing/test.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/testing/test.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/LightCrafterDMD.py` & `labscript-devices-3.2.0rc1/labscript_devices/LightCrafterDMD.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_tabs.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         else:
             AO_base_min, AO_base_max = None, None
         AO_base_step = 0.1
         AO_base_decimals = 3
 
         clock_terminal = properties['clock_terminal']
         clock_mirror_terminal = properties['clock_mirror_terminal']
+        # get to avoid error on older connection tables
+        connected_terminals = properties.get('connected_terminals', None)
         static_AO = properties['static_AO']
         static_DO = properties['static_DO']
         clock_limit = properties['clock_limit']
         min_semiperiod_measurement = properties['min_semiperiod_measurement']
 
         # And the Measurement and Automation Explorer (MAX) name we will need to
         # communicate with the device:
@@ -200,14 +202,16 @@
                     'MAX_name': self.MAX_name,
                     'num_AI': num_AI,
                     'AI_chans': AI_chans,
                     'AI_term': properties['AI_term'],
                     'AI_range': properties['AI_range'],
                     'AI_start_delay': properties['AI_start_delay'],
                     'AI_start_delay_ticks': properties['AI_start_delay_ticks'],
+                    'AI_timebase_terminal': properties.get('AI_timebase_terminal',None),
+                    'AI_timebase_rate': properties.get('AI_timebase_rate',None),
                     'clock_terminal': clock_terminal,
                 },
             )
             self.add_secondary_worker("acquisition_worker")
 
         # Set the capabilities of this device
         self.supports_remote_value_check(False)
```

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_workers.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,14 +159,31 @@
                 self.clock_terminal,
                 self.clock_mirror_terminal,
                 DAQmx_Val_DoNotInvertPolarity,
             )
         else:
             DAQmxDisconnectTerms(self.clock_terminal, self.clock_mirror_terminal)
 
+    def set_connected_terminals_connected(self, connected):
+        """Connect the terminals in the connected terminals list.
+        Allows on daisy chaining of the clock line to/from other devices
+        that do not have a direct route (see Device Routes in NI MAX)."""
+        if self.connected_terminals is None:
+            return
+        if connected:
+            for terminal_pair in self.connected_terminals:
+                DAQmxConnectTerms(
+                    terminal_pair[0],
+                    terminal_pair[1],
+                    DAQmx_Val_DoNotInvertPolarity,
+                )
+        else:
+            for terminal_pair in self.connected_terminals:
+                DAQmxDisconnectTerms(terminal_pair[0], terminal_pair[1])
+
     def program_buffered_DO(self, DO_table):
         """Create the DO task and program in the DO table for a shot. Return a
         dictionary of the final values of each channel in use"""
         if DO_table is None:
             return {}
         self.DO_task = Task()
         written = int32()
@@ -316,14 +333,17 @@
 
         # Get the data to be programmed into the output tasks:
         AO_table, DO_table = self.get_output_tables(h5file, device_name)
 
         # Mirror the clock terminal, if applicable:
         self.set_mirror_clock_terminal_connected(True)
 
+        # Mirror other terminals, if applicable
+        self.set_connected_terminals_connected(True)
+
         # Program the output tasks and retrieve the final values of each output:
         DO_final_values = self.program_buffered_DO(DO_table)
         AO_final_values = self.program_buffered_AO(AO_table)
 
         final_values = {}
         final_values.update(DO_final_values)
         final_values.update(AO_final_values)
@@ -368,14 +388,17 @@
                         self.logger.info(msg, name, current, total)
                 task.StopTask()
             task.ClearTask()
 
         # Remove the mirroring of the clock terminal, if applicable:
         self.set_mirror_clock_terminal_connected(False)
 
+        # Remove connections between other terminals, if applicable:
+        self.set_connected_terminals_connected(False)
+
         # Set up manual mode tasks again:
         self.start_manual_mode_tasks()
         if abort:
             # Reprogram the initial states:
             self.program_manual(self.initial_values)
 
         return True
@@ -487,14 +510,21 @@
                 term,
                 self.AI_range[0],
                 self.AI_range[1],
                 DAQmx_Val_Volts,
                 None,
             )
 
+        if self.AI_timebase_terminal is None:
+            # use internal default
+            pass
+        else:
+            self.task.SetSampClkTimebaseSrc(self.AI_timebase_terminal)
+            self.task.SetSampClkTimebaseRate(self.AI_timebase_rate)
+
         self.task.CfgSampClkTiming(
             "", rate, DAQmx_Val_Rising, DAQmx_Val_ContSamps, num_samples
         )
         if self.buffered_mode:
             self.task.CfgDigEdgeStartTrig(self.clock_terminal, DAQmx_Val_Rising)
 
         # This must not be garbage collected until the task is:
```

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/daqmx_utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/daqmx_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/labscript_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # This file is part of the module labscript_devices, in the         #
 # labscript suite (see http://labscriptsuite.org), and is           #
 # licensed under the Simplified BSD License. See the license.txt    #
 # file in the root of the project for the full license.             #
 #                                                                   #
 #####################################################################
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 
 from labscript import (
     IntermediateDevice,
     AnalogOut,
     DigitalOut,
     StaticAnalogOut,
@@ -54,19 +54,22 @@
         property_names={
             "connection_table_properties": [
                 "clock_terminal",
                 "MAX_name",
                 "static_AO",
                 "static_DO",
                 "clock_mirror_terminal",
+                "connected_terminals",
                 "AI_range",
                 "AI_start_delay",
                 "AI_start_delay_ticks",
                 "AI_term",
                 "AI_chans",
+                "AI_timebase_terminal",
+                "AI_timebase_rate",
                 "AO_range",
                 "max_AI_multi_chan_rate",
                 "max_AI_single_chan_rate",
                 "max_AO_sample_rate",
                 "max_DO_sample_rate",
                 "min_semiperiod_measurement",
                 "num_AI",
@@ -89,21 +92,24 @@
         name,
         parent_device=None,
         clock_terminal=None,
         MAX_name=None,
         static_AO=None,
         static_DO=None,
         clock_mirror_terminal=None,
+        connected_terminals=None,
         acquisition_rate=None,
         AI_range=None,
         AI_range_Diff=None,
         AI_start_delay=0,
         AI_start_delay_ticks=None,
         AI_term='RSE',
         AI_term_cfg=None,
+        AI_timebase_terminal=None,
+        AI_timebase_rate=None,
         AO_range=None,
         max_AI_multi_chan_rate=None,
         max_AI_single_chan_rate=None,
         max_AO_sample_rate=None,
         max_DO_sample_rate=None,
         min_semiperiod_measurement=None,
         num_AI=0,
@@ -128,14 +134,17 @@
             clock_terminal (str): What input on the DAQ is used for the clockline
             MAX_name (str): NI-MAX device name
             static_AO (int, optional): Number of static analog output channels.
             static_DO (int, optional): Number of static digital output channels.
             clock_mirror_terminal (str, optional): Channel string of digital output
                 that mirrors the input clock. Useful for daisy-chaning DAQs on the same
                 clockline.
+            connected_terminals (list, optional): List of pairs of strings of digital inputs
+                and digital outputs that will be connected. Useful for daisy-chaining DAQs
+                on the same clockline when they do not have direct routes (see Device Routes in NI MAX).
             acquisiton_rate (float, optional): Default sample rate of inputs.
             AI_range (iterable, optional): A `[Vmin, Vmax]` pair that sets the analog
                 input voltage range for all analog inputs.
             AI_range_Diff (iterable, optional): A `[Vmin, Vmax]` pair that sets the analog
                 input voltage range for all analog inputs when using Differential termination.
             AI_start_delay (float, optional): Time in seconds between start of an
                 analog input task starting and the first sample.
@@ -145,14 +154,20 @@
                 for DAQs that employ delta ADCs.
             AI_term (str, optional): Configures the analog input termination for all
                 analog inputs. Must be supported by the device. Supported options are
                 `'RSE'`, `'NRSE'` `'Diff'`, and '`PseudoDiff'`.
             AI_term_cfg (dict, optional): Dictionary of analog input channels and their
                 supported terminations. Best to use `get_capabilities.py` to introspect
                 these.
+            AI_timebase_terminal (str, optional): Channel string that specifies what
+                channel to use for the Sample Clock Timebase signal.
+                If None, use default internal clocks.
+                Must also specify the rate when not using the internal sources.
+            AI_timebase_rate (float, optional): Supplied clock frequency for the AI timebase.
+                Only specify if using an external clock source.
             AO_range (iterable, optional): A `[Vmin, Vmax]` pair that sets the analog
                 output voltage range for all analog outputs.
             max_AI_multi_chan_rate (float, optional): Max supported analog input 
                 sampling rate when using multiple channels.
             max_AI_single_chan_rate (float, optional): Max supported analog input
                 sampling rate when only using a single channel.
             max_AO_sample_rate (float, optional): Max supported analog output
@@ -241,14 +256,21 @@
             else:
                 # Tells blacs_worker to use AI_start_delay to define delay
                 self.start_delay_ticks = False
         else:
             # no analog inputs
             self.AI_chans = []
             self.start_delay_ticks = None
+        # special AI timebase handling
+        if num_AI > 0:
+            if (AI_timebase_rate is None) ^ (AI_timebase_terminal is None):
+                raise LabscriptError("You must specify terminal and rate when using an external AI timebase")
+            self.AI_timebase_terminal = AI_timebase_terminal
+            self.AI_timebease_rate = AI_timebase_rate
+                
         self.num_AO = num_AO
         self.num_CI = num_CI
         self.ports = ports if ports is not None else {}
         self.supports_buffered_AO = supports_buffered_AO
         self.supports_buffered_DO = supports_buffered_DO
         self.supports_semiperiod_measurement = supports_semiperiod_measurement
         self.supports_simultaneous_AI_sampling = supports_simultaneous_AI_sampling
```

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6008.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6008.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6229.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6229.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6343.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6343.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/NI_USB_6366.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6366.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/README.txt` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/README.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/_subclass_template.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/_subclass_template.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/capabilities.json` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/capabilities.json`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/generate_subclasses.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/generate_subclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 Called from the command line via
 
 .. code-block:: shell
 
     python generate_subclasses.py
 
+For proper formatting of the code, you will need to install the `black` python package.
 """
 import os
 import warnings
 import json
 from string import Template
 
 from labscript_utils import dedent
```

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/models/get_capabilities.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/get_capabilities.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/runviewer_parsers.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/runviewer_parsers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_DAQmx/utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_PCI_6733.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_PCI_6733.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_PCIe_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_PCIe_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NI_USB_6343.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_USB_6343.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/NovaTechDDS9M.py` & `labscript-devices-3.2.0rc1/labscript_devices/NovaTechDDS9M.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,21 @@
     'baud_rate',  -- operating baud rate
     'default_baud_rate' -- assumed baud rate at startup
     """
     description = 'NT-DDS9M'
     allowed_children = [DDS, StaticDDS]
     clock_limit = 9990 # This is a realistic estimate of the max clock rate (100us for TS/pin10 processing to load next value into buffer and 100ns pipeline delay on pin 14 edge to update output values)
 
+    # This is longer than the technical requirement on the NovaTech. However, I
+    # suspect the tri-state buffer or similar electronics that some groups have
+    # in front of their NovaTech clock inputs might limit how fast this can be.
+    # 1us should be a good compromise, but can always be overridden by a
+    # subclass of monkey-patched if needed.
+    minimum_clock_high_time = 1e-6
+
     @set_passed_properties(
         property_names={
             'connection_table_properties': [
                 'com_port',
                 'baud_rate',
                 'default_baud_rate',
                 'update_mode',
```

### Comparing `labscript-devices-3.1.1/labscript_devices/PhaseMatrixQuickSyn.py` & `labscript-devices-3.2.0rc1/labscript_devices/PhaseMatrixQuickSyn.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PineBlaster.py` & `labscript-devices-3.2.0rc1/labscript_devices/PineBlaster.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PrawnBlaster/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PrawnBlaster/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PrawnBlaster/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PrawnBlaster/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PrawnBlaster/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PrawnBlaster/runviewer_parsers.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/runviewer_parsers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PulseBlaster.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PulseBlasterESRPro200.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro200.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PulseBlasterESRPro500.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro500.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PulseBlasterUSB.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterUSB.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PulseBlaster_No_DDS.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_No_DDS.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PulseBlaster_SP2_24_100_32k.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_SP2_24_100_32k.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PylonCamera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PylonCamera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         self.camera.Open()
         self.timeout = 1000 # in ms
         self.camera.RegisterConfiguration(pylon.SoftwareTriggerConfiguration(),
                         pylon.RegistrationMode_ReplaceAll, pylon.Cleanup_Delete)
         # Keep a nodeMap reference so we don't have to re-create a lot
         self.nodeMap = self.camera.GetNodeMap()
         self._abort_acquisition = False
+        self.exception_on_failed_shot = True
+
 
     def set_attributes(self, attributes_dict):
         """Sets all attribues in attr_dict.
         Pylon cameras require that ROI settings be done in correct order,
         so we do them separately."""
         # make a copy of dict so we can pop off already handled values
         attr_dict = attributes_dict.copy()
```

### Comparing `labscript-devices-3.1.1/labscript_devices/PylonCamera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PylonCamera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PylonCamera/testing/ExposureTiming.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/testing/ExposureTiming.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/PythonCamera.py` & `labscript-devices-3.2.0rc1/labscript_devices/PythonCamera.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/RFBlaster.py` & `labscript-devices-3.2.0rc1/labscript_devices/RFBlaster.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         camList.Clear()
 
         # Set the timeout to 5 s:
         self.timeout = 5000 # in ms
 
         # Set the abort acquisition thingy:
         self._abort_acquisition = False
+        self.exception_on_failed_shot = True
 
     def get_attribute_names(self, visibility):
         names = []
         def get_node_names_in_category(node_category, prefix=''):
             for node_feature in node_category.GetFeatures():
                 # Ensure node is available and readable
                 if (not PySpin.IsAvailable(node_feature) or not
```

### Comparing `labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/SpinnakerCamera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/TekScope/TekScope.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/TekScope.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/TekScope/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/TekScope/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/TekScope/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/ZaberStageController/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/ZaberStageController/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/ZaberStageController/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/ZaberStageController/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/ZaberStageController/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/ZaberStageController/utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/__version__.py` & `labscript-devices-3.2.0rc1/labscript_devices/__version__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/atsapi.py` & `labscript-devices-3.2.0rc1/labscript_devices/atsapi.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/camera.ui` & `labscript-devices-3.2.0rc1/labscript_devices/camera.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/imaqdx_server.py` & `labscript-devices-3.2.0rc1/labscript_devices/imaqdx_server.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/phasematrixquicksyn.ui` & `labscript-devices-3.2.0rc1/labscript_devices/phasematrixquicksyn.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/pulseblaster.ui` & `labscript-devices-3.2.0rc1/labscript_devices/pulseblaster.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices/test_device.py` & `labscript-devices-3.2.0rc1/labscript_devices/test_device.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/labscript_devices.egg-info/PKG-INFO` & `labscript-devices-3.2.0rc1/labscript_devices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: labscript-devices
-Version: 3.1.1
+Version: 3.2.0rc1
 Summary: Device drivers for hardware controlled by the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-devices
 Project-URL: Download, https://github.com/labscript-suite/labscript-devices/releases
 Project-URL: Tracker, https://github.com/labscript-suite/labscript-devices/issues
 Keywords: experiment control automation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite" align="right">
 
@@ -94,9 +95,7 @@
 
 † We do not endorse the use of any particular hardware.
 
 
 ## Installation
 
 labscript-devices is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `labscript-devices-3.1.1/labscript_devices.egg-info/SOURCES.txt` & `labscript-devices-3.2.0rc1/labscript_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/readthedocs.yaml` & `labscript-devices-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.1.1/setup.cfg` & `labscript-devices-3.2.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.6
 install_requires = 
@@ -41,16 +43,17 @@
 	qtutils>=2.2.3
 	spinapi
 	zprocess>=2.18.0
 
 [options.extras_require]
 docs = 
 	PyQt5
-	Sphinx==3.5.3
+	Sphinx==4.4.0
 	sphinx-rtd-theme==0.5.2
 	recommonmark==0.6.0
 	m2r==0.2.1
+	mistune<2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

