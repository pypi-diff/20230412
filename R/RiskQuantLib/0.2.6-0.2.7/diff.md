# Comparing `tmp/RiskQuantLib-0.2.6.tar.gz` & `tmp/RiskQuantLib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskQuantLib-0.2.6.tar", last modified: Fri Mar 31 08:18:56 2023, max compression
+gzip compressed data, was "RiskQuantLib-0.2.7.tar", last modified: Wed Apr 12 02:24:20 2023, max compression
```

## Comparing `RiskQuantLib-0.2.6.tar` & `RiskQuantLib-0.2.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:56.079257 RiskQuantLib-0.2.6/
--rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.2.6/LICENSE
--rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1120 2023-03-31 08:18:56.081024 RiskQuantLib-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.2.6/README.md
--rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-31 08:18:56.081024 RiskQuantLib-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1932 2023-03-31 08:17:43.000000 RiskQuantLib-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.438203 RiskQuantLib-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.486049 RiskQuantLib-0.2.6/src/RiskQuantLib/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.517723 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.533373 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/Instrument/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/Instrument/__init__.py
--rw-rw-rw-   0        0        0      388 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.535085 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/InstrumentList/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0      409 2023-01-11 09:39:05.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Auto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.597869 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.622271 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.659294 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
--rw-rw-rw-   0        0        0     2677 2022-12-29 14:06:46.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
--rw-rw-rw-   0        0        0      351 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
--rw-rw-rw-   0        0        0      355 2022-12-29 14:55:03.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
--rw-rw-rw-   0        0        0      402 2022-12-29 14:55:03.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.730008 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
--rw-rw-rw-   0        0        0     1474 2023-01-11 09:39:05.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
--rw-rw-rw-   0        0        0     2151 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
--rw-rw-rw-   0        0        0     1515 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
--rw-rw-rw-   0        0        0     1101 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.740428 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/__pycache__/
--rw-rw-rw-   0        0        0      180 2022-12-14 06:06:02.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    14083 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/macro.pyt
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/__init__.py
--rw-rw-rw-   0        0        0    43577 2023-03-21 00:45:45.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/builder.py
--rw-rw-rw-   0        0        0     1640 2023-01-11 02:34:10.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/render.py
--rw-rw-rw-   0        0        0     8835 2023-03-21 00:45:45.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/router.py
--rw-rw-rw-   0        0        0     4736 2023-01-10 08:01:22.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Build/tree.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.753284 RiskQuantLib-0.2.6/src/RiskQuantLib/Instrument/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Instrument/__init__.py
--rw-rw-rw-   0        0        0      935 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.768960 RiskQuantLib-0.2.6/src/RiskQuantLib/InstrumentList/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/InstrumentList/instrumentList.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.784902 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.808634 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/Copula/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/Copula/__init__.py
--rw-rw-rw-   0        0        0     1207 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/Copula/copula.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.823219 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/KMV/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/KMV/__init__.py
--rw-rw-rw-   0        0        0     2181 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/KMV/kmv.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/__init__.py
--rw-rw-rw-   0        0        0      274 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Model/model.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.868274 RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/iloc.py
--rw-rw-rw-   0        0        0     1107 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/loc.py
--rw-rw-rw-   0        0        0    60946 2023-03-21 05:30:23.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/operation.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.883421 RiskQuantLib-0.2.6/src/RiskQuantLib/Property/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Property/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-01-11 10:25:57.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Property/property.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:56.076796 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/
--rw-rw-rw-   0        0        0     4368 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/GUITool.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/__init__.py
--rw-rw-rw-   0        0        0     6514 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/codeBuilderTool.py
--rw-rw-rw-   0        0        0    10263 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/databaseTool.py
--rw-rw-rw-   0        0        0     1593 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/excelTool.py
--rw-rw-rw-   0        0        0    19343 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/fileTool.py
--rw-rw-rw-   0        0        0     4862 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/githubTool.py
--rw-rw-rw-   0        0        0     2817 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/mathTool.py
--rw-rw-rw-   0        0        0     1158 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/multiThreadTool.py
--rw-rw-rw-   0        0        0     4705 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/outlookTool.py
--rw-rw-rw-   0        0        0     4487 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/plotTool.py
--rw-rw-rw-   0        0        0     9707 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/pptTool.py
--rw-rw-rw-   0        0        0     9605 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/strTool.py
--rw-rw-rw-   0        0        0     6111 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/wordTool.py
--rw-rw-rw-   0        0        0    34006 2023-03-31 08:08:38.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib/module.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:18:55.517723 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-03-31 08:18:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2773 2023-03-31 08:18:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 08:18:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      619 2023-03-31 08:18:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-03-31 08:18:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-31 08:18:55.000000 RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.495383 RiskQuantLib-0.2.7/
+-rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1120 2023-04-12 02:24:20.495383 RiskQuantLib-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.2.7/README.md
+-rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:24:20.496382 RiskQuantLib-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1932 2023-04-12 02:18:48.000000 RiskQuantLib-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.358344 RiskQuantLib-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.378347 RiskQuantLib-0.2.7/src/RiskQuantLib/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.407348 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.410388 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/Instrument/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      388 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.413385 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-01-11 09:39:05.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Auto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.423386 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.426385 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.435397 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
+-rw-rw-rw-   0        0        0     2677 2022-12-29 14:06:46.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
+-rw-rw-rw-   0        0        0      351 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
+-rw-rw-rw-   0        0        0      355 2022-12-29 14:55:03.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
+-rw-rw-rw-   0        0        0      402 2022-12-29 14:55:03.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.447383 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
+-rw-rw-rw-   0        0        0     1474 2023-01-11 09:39:05.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
+-rw-rw-rw-   0        0        0     2151 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
+-rw-rw-rw-   0        0        0     1515 2023-01-11 09:39:04.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
+-rw-rw-rw-   0        0        0     1101 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.449385 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/__pycache__/
+-rw-rw-rw-   0        0        0      180 2022-12-14 06:06:02.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14083 2023-01-11 10:09:16.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/macro.pyt
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/__init__.py
+-rw-rw-rw-   0        0        0    43577 2023-03-21 00:45:45.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/builder.py
+-rw-rw-rw-   0        0        0     1640 2023-01-11 02:34:10.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/render.py
+-rw-rw-rw-   0        0        0     8835 2023-03-21 00:45:45.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/router.py
+-rw-rw-rw-   0        0        0     4736 2023-01-10 08:01:22.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Build/tree.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.452409 RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      935 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.455395 RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/instrumentList.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.458390 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.460384 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/__init__.py
+-rw-rw-rw-   0        0        0     1207 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/copula.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.462384 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/__init__.py
+-rw-rw-rw-   0        0        0     2181 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/kmv.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/__init__.py
+-rw-rw-rw-   0        0        0      274 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Model/model.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.469385 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/iloc.py
+-rw-rw-rw-   0        0        0     1107 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/loc.py
+-rw-rw-rw-   0        0        0    60946 2023-03-21 05:30:23.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/operation.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.472401 RiskQuantLib-0.2.7/src/RiskQuantLib/Property/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Property/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-01-11 10:25:57.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Property/property.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.494397 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/
+-rw-rw-rw-   0        0        0     4368 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/GUITool.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/__init__.py
+-rw-rw-rw-   0        0        0     6514 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/codeBuilderTool.py
+-rw-rw-rw-   0        0        0    10785 2023-04-12 02:00:01.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/databaseTool.py
+-rw-rw-rw-   0        0        0     1593 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/excelTool.py
+-rw-rw-rw-   0        0        0    19343 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/fileTool.py
+-rw-rw-rw-   0        0        0     4862 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/githubTool.py
+-rw-rw-rw-   0        0        0     2817 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/mathTool.py
+-rw-rw-rw-   0        0        0     1158 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/multiThreadTool.py
+-rw-rw-rw-   0        0        0     4705 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/outlookTool.py
+-rw-rw-rw-   0        0        0     4487 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/plotTool.py
+-rw-rw-rw-   0        0        0     9707 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/pptTool.py
+-rw-rw-rw-   0        0        0     9605 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/strTool.py
+-rw-rw-rw-   0        0        0     6111 2023-01-11 09:52:54.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/wordTool.py
+-rw-rw-rw-   0        0        0    34418 2023-04-12 02:03:48.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-11 09:52:55.000000 RiskQuantLib-0.2.7/src/RiskQuantLib/module.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:24:20.405365 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2773 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      619 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 02:24:20.000000 RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/top_level.txt
```

### Comparing `RiskQuantLib-0.2.6/LICENSE` & `RiskQuantLib-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/PKG-INFO` & `RiskQuantLib-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.2.6
+Version: 0.2.7
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.2.6/README.md` & `RiskQuantLib-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/setup.py` & `RiskQuantLib-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="RiskQuantLib",
-    version="0.2.6",
+    version="0.2.7",
     author="Syuya_Murakami",
     author_email="wxy135@mail.ustc.edu.cn",
     description="RiskQuantLib is a QuantLib derivative to evaluate risk.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://riskquantlib-doc.readthedocs.io/en/latest/index.html",
     project_urls={
```

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/Component/macro.pyt` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/Component/macro.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/builder.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/builder.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/render.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/render.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/router.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/router.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Build/tree.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Build/tree.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Instrument/instrument.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/InstrumentList/instrumentList.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/InstrumentList/instrumentList.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Model/Copula/copula.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Model/Copula/copula.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Model/KMV/kmv.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Model/KMV/kmv.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/iloc.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/iloc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/loc.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/loc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Operation/operation.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Operation/operation.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Property/property.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Property/property.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/GUITool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/GUITool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/codeBuilderTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/codeBuilderTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/databaseTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/databaseTool.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,30 @@
     def readSql(self,sql:str):
         data = pd.read_sql(sql,con=self.engine)
         return data
 
     #<oracleTool>
     #</oracleTool>
 
+class sqlServerTool(object):
+    """
+    This is the API to connect with sql server database.
+    """
+    def __init__(self,databaseNameString:str,hostAddress:str,userName:str,passWord:str):
+        import pymssql
+        self.engine = pymssql.connect(hostAddress,userName,passWord,databaseNameString,charset='cp936')
+        self.cursor = self.engine.cursor()
+
+    def readSql(self,sql:str):
+        data = pd.read_sql(sql,con=self.engine)
+        return data
+
+    #<sqlServerTool>
+    #</sqlServerTool>
+
 class neo4jTool(object):
     """
     This is the API to connect with neo4j database.
     """
 
     def __init__(self, hostAddress:str,port:int,userName:str,password:str):
         from py2neo import Graph
```

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/excelTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/excelTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/fileTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/fileTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/githubTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/githubTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/mathTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/mathTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/multiThreadTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/multiThreadTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/outlookTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/outlookTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/plotTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/plotTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/pptTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/pptTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/strTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/strTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/Tool/wordTool.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/Tool/wordTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/__init__.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,14 +401,22 @@
         parser = argparse.ArgumentParser()
         parser.add_argument("template", type=str, help="the name of saved RiskQuantLib project")
         parser.add_argument("target", type=str, help="the path where you want to unpack the template project into")
         args = parser.parse_args()
         templateName = args.template
         targetPath = args.target
 
+    # use index number to locate template
+    if str.isdigit(templateName):
+        import os
+        sourcePath = checkAndCreateTemplatePath()
+        projectNameDict = {idx:i.replace('.zip', '') for idx, i in enumerate(os.listdir(sourcePath))}
+        templateIndex = int(templateName)
+        templateName = projectNameDict[templateIndex] if templateIndex in projectNameDict else templateName
+
     import sys,os,shutil
     RiskQuantLibDictionary = os.path.abspath(__file__).split('RiskQuantLib'+os.sep+'__init__')[0]
     sourcePath = os.path.abspath(RiskQuantLibDictionary)+os.sep+r'RQLTemplate'
     shutil.unpack_archive(sourcePath+os.sep+templateName+'.zip',targetPath,"zip")
     if os.path.exists(targetPath+os.sep+templateName+'.zip'):
         os.remove(targetPath+os.sep+templateName+'.zip')
     print('RiskQuantLib project template '+templateName+' unpack finished!')
@@ -423,15 +431,16 @@
     -------
     None
     """
     import os
     sourcePath = checkAndCreateTemplatePath()
     projectNameList = [i.replace('.zip','') for i in os.listdir(sourcePath)]
     hints = "Show all RiskQuantLib template projects:"
-    print(hints,'\n',"".join(['-' for i in range(len(hints))]))
+    print(hints)
+    print("".join(['-' for i in range(len(hints))]))
     [print(index,"->",name) for index,name in enumerate(projectNameList)]
 
 def delProjectTemplate(targetName:str = ''):
     """
     delProject() is a function to delete a RiskQuantLib project from library.
 
     Use terminal command 'delRQL' to use this function.
```

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib/module.py` & `RiskQuantLib-0.2.7/src/RiskQuantLib/module.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/PKG-INFO` & `RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.2.6
+Version: 0.2.7
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/SOURCES.txt` & `RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.6/src/RiskQuantLib.egg-info/entry_points.txt` & `RiskQuantLib-0.2.7/src/RiskQuantLib.egg-info/entry_points.txt`

 * *Files identical despite different names*

