# Comparing `tmp/hvcc-0.6.3.tar.gz` & `tmp/hvcc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvcc-0.6.3.tar", last modified: Mon Jan  9 20:01:24 2023, max compression
+gzip compressed data, was "hvcc-0.7.0.tar", last modified: Wed Apr 12 14:10:04 2023, max compression
```

## Comparing `hvcc-0.6.3.tar` & `hvcc-0.7.0.tar`

### file list

```diff
@@ -1,567 +1,556 @@
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.084050 hvcc-0.6.3/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    32005 2021-04-14 08:50:26.000000 hvcc-0.6.3/LICENSE
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      291 2022-08-20 00:37:38.000000 hvcc-0.6.3/MANIFEST.in
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-01-09 20:01:24.084050 hvcc-0.6.3/PKG-INFO
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6500 2023-01-09 19:58:43.000000 hvcc-0.6.3/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.968050 hvcc-0.6.3/hvcc/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14688 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.968050 hvcc-0.6.3/hvcc/core/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.972050 hvcc-0.6.3/hvcc/core/hv2ir/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4023 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/BufferPool.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2693 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/Connection.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1370 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrConvolution.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1664 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrInlet.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      996 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrLorenz.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1209 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrOutlet.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1067 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrPack.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1423 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrReceive.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1962 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrSend.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1214 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrSwitchcase.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1386 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrTabhead.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1420 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrTabread.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1402 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HIrTabwrite.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1976 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangAdc.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10517 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangBinop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1763 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangBiquad.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1964 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangDac.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1317 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangDelay.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2010 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangIf.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1563 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangLine.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1309 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangMessage.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1704 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangNoise.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1360 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangPhasor.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1301 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangPrint.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1392 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangRandom.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1920 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangReceive.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2207 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangSend.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3140 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangSequence.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1301 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangSlice.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1305 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangSystem.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1965 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangTable.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3829 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangUnop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2695 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangVar.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2174 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/HLangVario.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      934 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/core/hv2ir/HeavyException.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    41429 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HeavyGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9594 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HeavyIrObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15784 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/core/hv2ir/HeavyLangObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11351 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/core/hv2ir/HeavyParser.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3651 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/LocalVars.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/hv2ir/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5319 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/core/hv2ir/hv2ir.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.972050 hvcc-0.6.3/hvcc/core/json/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49675 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/json/heavy.ir.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    42899 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/core/json/heavy.lang.json
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.972050 hvcc-0.6.3/hvcc/generators/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.972050 hvcc-0.6.3/hvcc/generators/buildjson/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/buildjson/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3008 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/buildjson/buildjson.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.976050 hvcc-0.6.3/hvcc/generators/c2bela/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      181 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2bela/SETUP.md
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2bela/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3364 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2bela/c2bela.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2bela/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.976050 hvcc-0.6.3/hvcc/generators/c2bela/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1048 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2bela/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.976050 hvcc-0.6.3/hvcc/generators/c2daisy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2daisy/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.976050 hvcc-0.6.3/hvcc/generators/c2daisy/boards/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      888 2021-09-24 15:16:41.000000 hvcc-0.6.3/hvcc/generators/c2daisy/boards/pod.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1604 2021-09-24 15:16:52.000000 hvcc-0.6.3/hvcc/generators/c2daisy/boards/versio.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4902 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2daisy/c2daisy.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8943 2022-10-11 17:59:25.000000 hvcc-0.6.3/hvcc/generators/c2daisy/parameters.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.976050 hvcc-0.6.3/hvcc/generators/c2daisy/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7851 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/c2daisy/static/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.976050 hvcc-0.6.3/hvcc/generators/c2daisy/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5101 2022-10-11 19:05:31.000000 hvcc-0.6.3/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      418 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/c2daisy/templates/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2dpf/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2dpf/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6474 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2dpf/c2dpf.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2dpf/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      862 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2dpf/static/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2dpf/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1239 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13944 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/HeavyDPF.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3461 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/HeavyDPF.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      515 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/Makefile
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      882 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/Makefile.project
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      968 2021-08-19 11:55:10.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/Makefile_project
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      557 2021-11-02 18:48:51.000000 hvcc-0.6.3/hvcc/generators/c2dpf/templates/x42_clock_ticks.txt
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2fabric/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6206 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2fabric/c2fabric.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2fabric/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2fabric/templates/android/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2fabric/templates/android/jni/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1036 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/android/jni/Android.mk
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      104 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/android/jni/Application.mk
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2fabric/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      843 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2fabric/templates/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2fabric/templates/source/fabric/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5095 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3293 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2fabric/templates/vs2015/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1879 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12034 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2fabric/templates/xcode/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11773 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.980050 hvcc-0.6.3/hvcc/generators/c2js/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2js/README.md
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2js/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9892 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2js/c2js.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2js/template/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6364 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2js/template/hv_worklet.js
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      323 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2js/template/hv_worklet_start.js
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8674 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2js/template/hv_wrapper.js
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5094 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2js/template/index.html
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2owl/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/c2owl/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6607 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2owl/c2owl.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2owl/deps/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7309 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/c2owl/deps/HvMessage.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10738 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/c2owl/deps/HvUtils.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2owl/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7536 2023-01-09 09:40:06.000000 hvcc-0.6.3/hvcc/generators/c2owl/templates/HeavyOwl.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      511 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/c2owl/templates/HeavyOwlConstants.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2pdext/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2pdext/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5254 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2pdext/c2pdext.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2pdext/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    28387 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2pdext/static/m_pd.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2pdext/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5138 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2pdext/templates/pd_external.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9581 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2pdext/templates/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2rack/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2rack/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      862 2021-09-30 10:53:08.000000 hvcc-0.6.3/hvcc/generators/c2rack/static/README.md
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.984050 hvcc-0.6.3/hvcc/generators/c2unity/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6114 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2unity/c2unity.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2unity/static/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2unity/static/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.988050 hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11516 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5538 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1399 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.988050 hvcc-0.6.3/hvcc/generators/c2unity/static/xcode/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1269 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/static/xcode/Info.plist
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2unity/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2unity/templates/android/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.988050 hvcc-0.6.3/hvcc/generators/c2unity/templates/android/jni/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1745 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/android/jni/Android.mk
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      132 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/android/jni/Application.mk
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.988050 hvcc-0.6.3/hvcc/generators/c2unity/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1451 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2unity/templates/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.988050 hvcc-0.6.3/hvcc/generators/c2unity/templates/source/unity/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15663 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4128 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       64 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/source/unity/PluginList.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.988050 hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10393 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10411 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2079 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.960049 hvcc-0.6.3/hvcc/generators/c2unity/templates/xcode/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.992050 hvcc-0.6.3/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    26264 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.992050 hvcc-0.6.3/hvcc/generators/c2wwise/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10051 2022-12-17 19:58:59.000000 hvcc-0.6.3/hvcc/generators/c2wwise/c2wwise.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.992050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/linux/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1584 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/linux/Makefile
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.992050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/resources/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4603 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.996050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9669 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      182 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.def
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2866 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6266 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      481 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1261 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.996050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2162 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2470 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9180 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2231 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.996050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      530 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      345 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_Wwise{{type}}PluginFactory.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.996050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2939 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8432 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1994 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5019 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1816 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3015 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7157 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4129 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2234 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/stdafx.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.996050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4601 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7351 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2691 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8485 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14466 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.996050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/runtime/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      475 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/runtime/Hv_{{name}}_WwisePluginRegister.cpp
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.000050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    27569 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18316 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4208 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    24299 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.000050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      889 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/Info.plist
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.000050 hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    25293 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       82 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/wwise.xcconfig
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.000050 hvcc-0.6.3/hvcc/generators/copyright/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/copyright/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1972 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/copyright/copyright_manager.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1570 2022-10-02 01:32:33.000000 hvcc-0.6.3/hvcc/generators/copyright/default_template.txt
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.004050 hvcc-0.6.3/hvcc/generators/ir2c/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4365 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlBinop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1408 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlCast.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2251 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlDelay.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1641 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlIf.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3138 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlMessage.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1614 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlPack.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1560 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlPrint.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1600 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlRandom.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      963 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlReceive.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2023 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlSend.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1619 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlSlice.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2536 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlSwitchcase.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1259 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlSystem.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1579 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlTabhead.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1633 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlTabread.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1644 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlTabwrite.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2452 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlUnop.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1980 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/ControlVar.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5871 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/HeavyObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2528 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/HeavyTable.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1512 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/PrettyfyC.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3032 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalBiquad.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2184 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalCPole.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1901 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalConvolution.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1718 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalDel1.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1581 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalEnvelope.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1732 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalLine.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2105 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalLorenz.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3535 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalMath.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2920 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalPhasor.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1937 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalRPole.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1791 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalSamphold.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1887 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalSample.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1807 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalTabhead.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3132 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalTabread.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2354 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalTabwrite.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4353 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/SignalVar.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/__init__.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12622 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/generators/ir2c/ir2c.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3616 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/generators/ir2c/ir2c_perf.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.012050 hvcc-0.6.3/hvcc/generators/ir2c/static/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9339 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HeavyContext.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4262 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HeavyContext.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11622 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HeavyContextInterface.hpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4072 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlBinop.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2033 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlBinop.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2040 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlCast.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1256 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlCast.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3597 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlDelay.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1494 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlDelay.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1405 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlIf.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1250 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlIf.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2505 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPack.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPack.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1035 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPrint.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1094 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPrint.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1697 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlRandom.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1300 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlRandom.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2151 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSlice.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSlice.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSystem.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1167 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSystem.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1577 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabhead.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabhead.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1675 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabread.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabread.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1750 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabwrite.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1354 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabwrite.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2367 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlUnop.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1538 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlUnop.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2525 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlVar.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1401 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlVar.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9062 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvHeavy.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15439 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvHeavy.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1412 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvHeavyInternal.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4803 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvLightPipe.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3274 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvLightPipe.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    21501 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMath.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7317 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessage.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessage.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4680 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessagePool.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2623 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessagePool.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6071 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessageQueue.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3270 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessageQueue.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9283 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalBiquad.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7085 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalBiquad.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2412 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalCPole.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11740 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalCPole.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4821 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalConvolution.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1429 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalConvolution.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1386 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalDel1.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1769 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalDel1.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5852 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalEnvelope.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1392 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalEnvelope.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4974 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLine.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2891 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLine.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1189 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLorenz.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4976 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLorenz.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4917 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalPhasor.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5679 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalPhasor.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1724 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalRPole.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3743 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalRPole.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1537 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSamphold.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9492 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSamphold.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1753 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSample.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1379 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSample.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2427 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabread.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6188 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabread.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1783 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabwrite.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5551 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabwrite.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2890 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalVar.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalVar.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4251 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvTable.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2625 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvTable.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1653 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvUtils.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9710 2022-10-01 22:57:41.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/HvUtils.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4553 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/cpuid.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2319 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/static/cpuid.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.012050 hvcc-0.6.3/hvcc/generators/ir2c/templates/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11759 2022-10-11 07:11:20.000000 hvcc-0.6.3/hvcc/generators/ir2c/templates/Heavy_NAME.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2517 2022-10-11 07:11:20.000000 hvcc-0.6.3/hvcc/generators/ir2c/templates/Heavy_NAME.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2720 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/ir2c/templates/Heavy_NAME.hpp
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/vs2015/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.012050 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1263 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/Heavy.sln
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13015 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/Heavy.vcxproj
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9467 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2527 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/main.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/stdafx.cpp
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      305 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/stdafx.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      306 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/vs2015/Heavy/targetver.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/xcode/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.016050 hvcc-0.6.3/hvcc/generators/xcode/Heavy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2492 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy/main.c
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.016050 hvcc-0.6.3/hvcc/generators/xcode/Heavy.xcodeproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    81361 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.020050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      934 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1141 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1626 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9797 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.020050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Base.lproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49663 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      170 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Prefix.pch
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.020050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      903 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1662 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/MainViewController.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2902 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/MainViewController.m
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16216 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Views/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.020050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18184 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.020050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/en.lproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      436 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/en.lproj/Credits.rtf
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       45 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/en.lproj/InfoPlist.strings
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      809 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/main.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.020050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/tinywav/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4493 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1956 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      842 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2761 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Base.lproj/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3702 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1575 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      921 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13635 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1077 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1576 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Info.plist
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5995 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7428 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      777 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/ViewController.h
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1049 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/ViewController.m
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      901 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/main.m
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/interpreters/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/interpreters/pd2hv/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2126 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/Connection.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2848 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/HeavyGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8156 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/HeavyObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1481 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/HvSwitchcase.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2327 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/NotificationEnum.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1754 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdAudioIoObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5382 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdBinopObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8021 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1011 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdLetObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2548 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdLibSignalGraph.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2252 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdMessageObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6480 2022-12-17 00:45:53.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1733 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdPackObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    28837 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdParser.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2789 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdRaw.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5446 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdReceiveObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6007 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdRouteObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5294 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdSelectObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3618 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdSendObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2014 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdTableObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2027 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdTriggerObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3337 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/PdUnpackObject.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/__init__.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.964050 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      798 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      761 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.024050 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy_converted/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6569 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:24.084050 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/abs.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/abs~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/atan.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/atan2.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/b.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bang.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      872 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bendin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      413 2022-10-01 22:57:41.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bendout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2107 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bng.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bp~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      627 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/change.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      372 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/clip.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      376 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/clip~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      117 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/cnv.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/cos.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      817 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/cos~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      573 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2291 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      523 2022-10-01 22:57:41.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      981 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      979 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/czero~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      694 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/dbtopow~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      692 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/dbtorms~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       61 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/declare.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/del.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      657 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delay.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delread~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1339 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      343 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/div.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/env~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      268 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/exp.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      228 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/exp~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/f.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/float.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/floatatom.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1082 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ftom.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      369 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ftom~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1239 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/hip~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/hradio.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/hsl.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      212 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/i.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      867 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/int.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2724 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/line.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      299 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/line~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      147 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/loadbang.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/log.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1088 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/lop~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1043 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/makenote.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1185 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/metro.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      250 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/midiin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      378 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/midiout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      258 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/midirealtimein.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      502 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/moses.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      492 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/mtof.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      366 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/mtof~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/nbx.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1234 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/noise~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      918 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/notein.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      422 2022-10-01 22:57:41.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/noteout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      489 2021-10-18 07:21:36.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/noteout.pd-test
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1156 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/osc~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      914 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      451 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/pgmout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      351 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/phasor~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/pipe.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12790 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/poly.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      919 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      430 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/polytouchout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/powtodb~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      215 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/print.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/q8_rsqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      226 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/q8_sqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      835 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/random.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rmstodb~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      337 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rpole~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      907 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      367 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rzero_rev~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      417 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rzero~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      615 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      269 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/samplerate~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      267 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/sig~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/sin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      411 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/snapshot~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      359 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/spigot.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/sqrt.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      909 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2022-12-17 19:43:48.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/stripnote.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      585 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/swap.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      332 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/symbol.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      179 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/symbolatom.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2361 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      292 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabplay~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      796 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabread.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2494 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1497 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      440 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabwrite.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tan.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      188 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tgl.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      869 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/timer.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      875 2023-01-09 19:58:43.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/touchin.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      373 2022-10-01 22:57:41.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/touchout.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      946 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/until.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2709 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      243 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/vd~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/vradio.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/vsl.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      497 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/wrap.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      288 2022-08-20 00:37:38.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/wrap~.pd
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5020 2022-10-11 07:11:14.000000 hvcc-0.6.3/hvcc/interpreters/pd2hv/pd2hv.py
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1906 2022-12-17 19:59:13.000000 hvcc-0.6.3/hvcc/utils.py
-drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-01-09 20:01:23.968050 hvcc-0.6.3/hvcc.egg-info/
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-01-09 20:01:23.000000 hvcc-0.6.3/hvcc.egg-info/PKG-INFO
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)    20949 2023-01-09 20:01:23.000000 hvcc-0.6.3/hvcc.egg-info/SOURCES.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)        1 2023-01-09 20:01:23.000000 hvcc-0.6.3/hvcc.egg-info/dependency_links.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       60 2023-01-09 20:01:23.000000 hvcc-0.6.3/hvcc.egg-info/entry_points.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       56 2023-01-09 20:01:23.000000 hvcc-0.6.3/hvcc.egg-info/requires.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       11 2023-01-09 20:01:23.000000 hvcc-0.6.3/hvcc.egg-info/top_level.txt
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1047 2023-01-09 20:01:24.084050 hvcc-0.6.3/setup.cfg
--rw-r--r--   0 dreamer   (1000) dreamer   (1000)       38 2022-08-20 00:37:38.000000 hvcc-0.6.3/setup.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.475034 hvcc-0.7.0/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    32005 2023-03-23 00:02:12.000000 hvcc-0.7.0/LICENSE
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      291 2023-03-23 00:02:12.000000 hvcc-0.7.0/MANIFEST.in
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-04-12 14:10:04.475034 hvcc-0.7.0/PKG-INFO
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6431 2023-04-12 13:45:43.000000 hvcc-0.7.0/README.md
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.355033 hvcc-0.7.0/hvcc/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14778 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.355033 hvcc-0.7.0/hvcc/core/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/core/hv2ir/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4237 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/BufferPool.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/Connection.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1688 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrConvolution.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1998 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrInlet.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1207 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrLorenz.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1486 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrOutlet.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1367 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrPack.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1695 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrReceive.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2345 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrSend.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1499 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrSwitchcase.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1705 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrTabhead.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1738 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrTabread.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1720 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HIrTabwrite.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2221 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangAdc.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10864 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangBinop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2055 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangBiquad.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2128 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangDac.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1523 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangDelay.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2010 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangIf.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1735 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangLine.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1481 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangMessage.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1704 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangNoise.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1592 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangPhasor.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1473 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangPrint.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1563 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangRandom.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2186 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangReceive.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2497 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSend.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3325 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSequence.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1473 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSlice.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1477 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangSystem.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2161 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangTable.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4041 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangUnop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2927 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangVar.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2604 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HLangVario.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1039 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyException.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    43580 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10293 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyIrObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16786 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyLangObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11713 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/HeavyParser.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3954 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/LocalVars.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/hv2ir/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5472 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/hv2ir/hv2ir.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/core/json/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49936 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/core/json/heavy.ir.json
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    42899 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/core/json/heavy.lang.json
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/generators/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.363033 hvcc-0.7.0/hvcc/generators/buildjson/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/buildjson/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3191 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/buildjson/buildjson.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2daisy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5107 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2daisy/c2daisy.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9377 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2daisy/parameters.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2daisy/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7851 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/static/README.md
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2daisy/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5101 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      418 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2daisy/templates/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2dpf/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2dpf/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7591 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/c2dpf.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2dpf/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1071 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/static/README.md
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.367033 hvcc-0.7.0/hvcc/generators/c2dpf/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2442 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6924 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4070 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4468 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3430 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2243 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3543 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1218 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_plugin
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      882 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_project
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5625 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2fabric/c2fabric.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1036 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/Android.mk
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      104 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/Application.mk
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/linux/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      843 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/linux/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5095 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3293 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1879 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12034 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.343032 hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11773 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/project.pbxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.371033 hvcc-0.7.0/hvcc/generators/c2js/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/README.md
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10301 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2js/c2js.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2js/template/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6364 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/hv_worklet.js
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      323 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/hv_worklet_start.js
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8674 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/hv_wrapper.js
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5094 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2js/template/index.html
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2owl/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6825 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2owl/c2owl.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2owl/deps/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7309 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/deps/HvMessage.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10738 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/deps/HvUtils.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2owl/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7536 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/templates/HeavyOwl.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      511 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2owl/templates/HeavyOwlConstants.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2pdext/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4826 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2pdext/c2pdext.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.375033 hvcc-0.7.0/hvcc/generators/c2pdext/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    28387 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/static/m_pd.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2pdext/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5138 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/templates/pd_external.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9581 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2pdext/templates/project.pbxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5509 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2unity/c2unity.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/static/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/static/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11516 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5538 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1399 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/static/xcode/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1269 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/static/xcode/Info.plist
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1745 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/Android.mk
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      132 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/Application.mk
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.379033 hvcc-0.7.0/hvcc/generators/c2unity/templates/linux/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1451 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/linux/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15663 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4128 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       64 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/PluginList.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10393 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    10411 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2079 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    26264 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2wwise/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9537 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/c2wwise/c2wwise.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2wwise/templates/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/linux/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1584 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/linux/Makefile
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.383033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/resources/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4603 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.347032 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.387033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9669 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      182 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.def
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2866 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6266 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      481 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1261 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.387033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2162 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2470 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9180 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2231 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.391033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      530 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      345 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_Wwise{{type}}PluginFactory.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.391033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2939 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8432 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1994 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5019 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1816 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3015 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7157 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4129 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2234 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/stdafx.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4601 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7351 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2691 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8485 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    14466 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/runtime/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      475 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/runtime/Hv_{{name}}_WwisePluginRegister.cpp
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    27569 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18316 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4208 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    24299 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      889 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Info.plist
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.395033 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    25293 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       82 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/wwise.xcconfig
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.399033 hvcc-0.7.0/hvcc/generators/copyright/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/copyright/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/copyright/copyright_manager.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1570 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/copyright/default_template.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2285 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/filters.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.407033 hvcc-0.7.0/hvcc/generators/ir2c/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4509 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlBinop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1507 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlCast.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2507 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlDelay.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1798 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlIf.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3341 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlMessage.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1748 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlPack.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1863 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlPrint.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1757 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlRandom.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1060 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlReceive.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2209 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSend.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1740 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSlice.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2787 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSwitchcase.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1299 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlSystem.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1648 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlTabhead.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1794 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlTabread.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1805 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlTabwrite.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2608 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlUnop.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2141 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ControlVar.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6610 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/HeavyObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2479 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/HeavyTable.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1721 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/PrettyfyC.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3271 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalBiquad.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2301 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalCPole.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalConvolution.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1867 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalDel1.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1708 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalEnvelope.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1918 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalLine.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalLorenz.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3650 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalMath.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2819 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalPhasor.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2078 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalRPole.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1952 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalSamphold.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2038 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalSample.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1926 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalTabhead.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3188 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalTabread.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2389 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalTabwrite.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4561 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/SignalVar.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/__init__.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12893 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ir2c.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3740 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/ir2c_perf.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.423033 hvcc-0.7.0/hvcc/generators/ir2c/static/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9339 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4262 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11622 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContextInterface.hpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4072 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2033 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2040 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1256 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3597 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1494 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1405 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1250 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2505 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1035 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1094 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1697 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1300 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2151 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2283 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1167 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1577 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1325 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1675 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1318 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1750 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1354 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2367 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1538 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2525 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1401 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9062 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    15439 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavyInternal.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4803 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3274 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    21847 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMath.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7317 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4680 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2623 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6071 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3270 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9283 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7085 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11740 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4821 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1429 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1386 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1769 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5852 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1392 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4974 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2891 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1189 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4976 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4917 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5679 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1724 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3743 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1537 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9492 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1753 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1379 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2427 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6188 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1783 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5551 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2890 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3211 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4251 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2625 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1653 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9710 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4553 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2319 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/ir2c/templates/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    11759 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2517 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2720 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.hpp
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/vs2015/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1263 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.sln
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13015 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9467 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2527 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/main.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/stdafx.cpp
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      305 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/stdafx.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      306 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/vs2015/Heavy/targetver.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/xcode/Heavy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2492 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy/main.c
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.427033 hvcc-0.7.0/hvcc/generators/xcode/Heavy.xcodeproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    81361 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      934 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1141 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1626 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9797 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    49663 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1080 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      170 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Prefix.pch
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      903 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1662 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2902 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.m
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    16216 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    18184 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      436 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/Credits.rtf
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       45 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/en.lproj/InfoPlist.strings
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      809 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/main.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.435033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     4493 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1956 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.439033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      842 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2761 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.439033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3702 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1575 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      921 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    13635 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.439033 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1077 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1576 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Info.plist
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5995 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     7428 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      777 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.h
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1049 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.m
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      901 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/main.m
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.443034 hvcc-0.7.0/hvcc/interpreters/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.447034 hvcc-0.7.0/hvcc/interpreters/pd2hv/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2581 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/Connection.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2977 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     8422 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1664 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/HvSwitchcase.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2327 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/NotificationEnum.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1929 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdAudioIoObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5676 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdBinopObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     9128 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1838 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLetObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3461 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLibSignalGraph.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3078 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdMessageObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6952 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1900 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdPackObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    29733 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdParser.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2856 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRaw.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5686 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdReceiveObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6302 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRouteObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5537 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSelectObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3805 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSendObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2179 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTableObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2230 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTriggerObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3510 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/PdUnpackObject.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        0 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/__init__.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.351032 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.447034 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      798 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      761 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.447034 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy_converted/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     6569 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.475034 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/abs.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/abs~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/atan.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      284 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/atan2.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/b.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bang.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      872 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bendin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      413 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bendout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2107 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bng.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2052 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bp~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      627 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/change.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      372 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/clip.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      376 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/clip~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      117 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cnv.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cos.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      817 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cos~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      573 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2291 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      523 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      981 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      979 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      694 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      692 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      229 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       61 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/declare.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/del.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      657 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delay.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1339 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      343 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/div.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/env~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      268 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/exp.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      228 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/exp~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/f.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      336 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/float.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      173 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/floatatom.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1082 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ftom.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      369 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ftom~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1239 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hip~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hradio.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hsl.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      212 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/i.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      867 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/int.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2724 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/line.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      299 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/line~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      147 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/loadbang.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/log.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1088 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/lop~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1043 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/makenote.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1185 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/metro.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      250 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/midiin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      378 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/midiout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      258 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/midirealtimein.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      502 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/moses.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      492 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/mtof.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      366 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/mtof~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/nbx.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1234 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/noise~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      918 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/notein.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      422 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/noteout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1156 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/osc~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      914 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      451 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pgmout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      351 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/phasor~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pipe.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    12790 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/poly.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      919 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      430 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/polytouchout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/powtodb~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      215 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/print.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      227 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/q8_rsqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      226 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/q8_sqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      835 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/random.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      680 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      412 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      337 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rpole~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      907 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      367 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rzero_rev~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      417 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rzero~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      615 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      269 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/samplerate~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      267 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sig~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      411 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/snapshot~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      359 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/spigot.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      222 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sqrt.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      909 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      342 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/stripnote.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      585 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/swap.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      332 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/symbol.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      179 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/symbolatom.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2361 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      292 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabplay~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      796 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2494 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1497 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      440 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2619 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      221 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tan.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      188 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tgl.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      869 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/timer.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      875 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/touchin.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      373 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/touchout.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      946 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/until.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     2709 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     3340 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vd~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vradio.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      131 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vsl.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      497 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/wrap.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      288 2023-03-23 00:02:12.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/wrap~.pd
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     5213 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/interpreters/pd2hv/pd2hv.py
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1889 2023-04-12 13:45:43.000000 hvcc-0.7.0/hvcc/utils.py
+drwxr-xr-x   0 dreamer   (1000) dreamer   (1000)        0 2023-04-12 14:10:04.355033 hvcc-0.7.0/hvcc.egg-info/
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)      896 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/PKG-INFO
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)    20780 2023-04-12 14:10:04.000000 hvcc-0.7.0/hvcc.egg-info/SOURCES.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)        1 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/dependency_links.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       60 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/entry_points.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       56 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/requires.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       11 2023-04-12 14:10:03.000000 hvcc-0.7.0/hvcc.egg-info/top_level.txt
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)     1047 2023-04-12 14:10:04.475034 hvcc-0.7.0/setup.cfg
+-rw-r--r--   0 dreamer   (1000) dreamer   (1000)       38 2023-03-23 00:02:12.000000 hvcc-0.7.0/setup.py
```

### Comparing `hvcc-0.6.3/LICENSE` & `hvcc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/PKG-INFO` & `hvcc-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hvcc
-Version: 0.6.3
+Version: 0.7.0
 Summary: `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 Home-page: https://github.com/Wasted-Audio/hvcc
-Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.6.3.tar.gz
+Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.7.0.tar.gz
 Author: Enzien Audio, Wasted Audio
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Compilers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hvcc-0.6.3/README.md` & `hvcc-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-[![Build Status](https://github.com/Wasted-Audio/hvcc/actions/workflows/build.yml/badge.svg)](https://github.com/Wasted-Audio/hvcc/actions)
-
-This is an attempt to modernize `hvcc` to work with `python3` and add some additional targets.
-
-Not all functionality is being tested. Bugreports and feedback are appreciated.
-
 # Heavy Compiler Collection (hvcc)
 
+[![Build Status](https://github.com/Wasted-Audio/hvcc/actions/workflows/build.yml/badge.svg)](https://github.com/Wasted-Audio/hvcc/actions)
+
 `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 
 ## Background
 
-The original need for `hvcc` arose from running against performance limitations while creating interactive music and sound products for the iPhone. [Pure Data](https://puredata.info) (libpd) was the only real choice for a design tool as it was embeddable and provided a high enough abstraction level that musicians or sound designers could be creative.
+Originaly created by Enzien Audio, the need for `hvcc` arose from running against performance limitations while creating interactive music and sound products for the iPhone. [Pure Data](https://puredata.info) (libpd) was the only real choice for a design tool as it was embeddable and provided a high enough abstraction level that musicians or sound designers could be creative.
 
 The goal was to leverage Pure Data as a design interface and statically interpret the resultant patches to generate a low-level, portable and optimised C/C++ program that would be structured to take advantage of modern hardware whilst still generating the same behaviour and audio output as Pure Data.
 
-It has since then been expanded to provide further support for many different platforms and frameworks, targeting game audio design, daw plugins and embedded production tools.
+It has since then been expanded to provide further support for many different platforms and frameworks, targeting game audio design, daw plugins and embedded production tools. In 2021 Wasted Audio took over maintenance of the project.
 
 ## Requirements
 
 * python 3.7 or higher
-    - `jinja2` (for generator templating)
-    - `importlib_resources` (for reading static resources)
-    - `json2daisy` (for daisy integration)
-    - `tox` (for tests, optional)
-    - `clang/clang++` (for building tests, optional)
+  * `jinja2` (for generator templating)
+  * `importlib_resources` (for reading static resources)
+  * `json2daisy` (for daisy integration)
+  * `tox` (for tests, optional)
+  * `clang/clang++` (for building tests, optional)
 
 ## Installation
+
 hvcc is available from pypi.org and can be installed using python3 pip:
 
 `$ pip3 install hvcc`
 
 If you want to develop hvcc you can install it from the source directory:
 
 `$ git clone https://github.com/Wasted-Audio/hvcc.git`
@@ -86,21 +83,22 @@
 
 A list of available generator options can be found [here](/docs/03.generators.md)
 
 ### `-p` Search Paths
 
 `hvcc` will iterate through various directories when resolving patch objects and abstractions. The `-p` or `--search_paths` argument can be used to add additional folders for `hvcc` to look in. Note that this argument is not needed for abstractions in the same folder as the top-level patch.
 
-This can be handy when using a third-party patch library for example https://github.com/Wasted-Audio/heavylib.
+This can be handy when using a third-party patch library like [heavylib](https://github.com/Wasted-Audio/heavylib) for example.
 
 Simply append any folder paths after the `-p` flag like so:
 
 `$ hvcc ~/myProject/_main.pd -o ~/Desktop/somewhere/else/ -n mySynth -p ~/Workspace/Projects/Enzien/heavylib/ ~/Desktop/myLib/`
 
 ### `-m` Meta Data
+
 `hvcc` can take extra meta-data via a supplied json file. It depends on the generator which fields are supported.
 
 ### `--copyright` User Copyright
 
 By default all the generated source files via `hvcc` will have the following copyright text applied to the top of the file:
 
 `Copyright (c) 2018 Enzien Audio, Ltd.`
@@ -112,33 +110,35 @@
 ### `--help`
 
 Displays all the available parameters and options for hvcc.
 
 ## Documentation
 
 * [Introduction](/docs/01.introduction.md)
-  - [What is heavy?](/docs/01.introduction.md#what-is-heavy)
-  - [Supported patch formats](/docs/01.introduction.md#supported-patch-formats)
-  - [Supported platforms](/docs/01.introduction.md#supported-platforms)
-  - [Supported frameworks](/docs/01.introduction.md#supported-frameworks)
-  - [Licensing](/docs/01.introduction.md#licensing)
+  * [What is heavy?](/docs/01.introduction.md#what-is-heavy)
+  * [Supported patch formats](/docs/01.introduction.md#supported-patch-formats)
+  * [Supported platforms](/docs/01.introduction.md#supported-platforms)
+  * [Supported frameworks](/docs/01.introduction.md#supported-frameworks)
+  * [Licensing](/docs/01.introduction.md#licensing)
 * [Getting Started](/docs/02.getting_started.md)
 * [Generators](/docs/03.generators.md)
 * [MIDI](/docs/04.midi.md)
 * [C API](/docs/05.c.md)
 * [C++ API](/docs/06.cpp.md)
 * [Heavy Lang Info](/docs/07.heavy_lang.md)
 * [Heavy IR Info](/docs/08.heavy_ir_lang.md)
 * [Supported vanilla objects](/docs/09.supported_vanilla_objects.md)
 * [Unsupported vanilla objects](/docs/10.unsupported_vanilla_objects.md)
 
 ## Contact
+
 There are several places where heavy/hvcc conversation is happening:
+
 * [Discord](https://discord.gg/fmxJveg)
 * [IRC](https://web.libera.chat/#hvcc)
 * A number of forums:
   * [Bela](https://forum.bela.io/?q=hvcc)
   * [Rebel Technology](https://community.rebeltech.org/tags/puredata)
-  * [Daisy](https://forum.electro-smith.com/t/pure-data/110)
+  * [Daisy](https://forum.electro-smith.com/c/integrations/pure-data/32)
   * [MOD](https://forum.moddevices.com/c/developers/pure-data/56)
 
 Or you can use the [discussions](https://github.com/Wasted-Audio/hvcc/discussions) tab of this repository
```

### Comparing `hvcc-0.6.3/hvcc/__init__.py` & `hvcc-0.7.0/hvcc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2021-2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,20 +17,20 @@
 import argparse
 from collections import OrderedDict
 import json
 import os
 import re
 import time
 import sys
+from typing import List, Dict, Optional
 
 from hvcc.interpreters.pd2hv import pd2hv
 from hvcc.core.hv2ir import hv2ir
 from hvcc.generators.ir2c import ir2c
 from hvcc.generators.ir2c import ir2c_perf
-from hvcc.generators.c2bela import c2bela
 from hvcc.generators.c2fabric import c2fabric
 from hvcc.generators.c2js import c2js
 from hvcc.generators.c2daisy import c2daisy
 from hvcc.generators.c2dpf import c2dpf
 from hvcc.generators.c2owl import c2owl
 from hvcc.generators.c2pdext import c2pdext
 from hvcc.generators.c2wwise import c2wwise
@@ -45,15 +46,15 @@
     yellow = "\033[93m"
     red = "\033[91m"
     bold = "\033[1m"
     underline = "\033[4m"
     end = "\033[0m"
 
 
-def add_error(results, error):
+def add_error(results: OrderedDict, error: str) -> OrderedDict:
     if "hvcc" in results:
         results["hvcc"]["notifs"]["errors"].append({"message": error})
     else:
         results["hvcc"] = {
             "stage": "hvcc",
             "notifs": {
                 "has_error": True,
@@ -61,30 +62,30 @@
                 "errors": [{"message": error}],
                 "warnings": []
             }
         }
     return results
 
 
-def check_extern_name_conflicts(extern_type, extern_list, results):
+def check_extern_name_conflicts(extern_type: str, extern_list: List, results: OrderedDict) -> None:
     """ In most of the generator code extern names become capitalised when used
         as enums. This method makes sure that there are no cases where two unique
         keys become the same after being capitalised.
         Note(joe): hvcc is probably the best place to check as at this point we
         have a list of all extern names.
     """
     for i, v in enumerate(extern_list):
         for j, u in enumerate(extern_list[i + 1:]):
             if v[0].upper() == u[0].upper():
                 add_error(results,
                           f"Conflicting {extern_type} names '{v[0]}' and '{u[0]}', make sure that "
                           "capital letters are not the only difference.")
 
 
-def generate_extern_info(hvir, results):
+def generate_extern_info(hvir: Dict, results: OrderedDict) -> Dict:
     """ Simplifies the receiver/send and table lists by only containing values
         externed with @hv_param, @hv_event or @hv_table
     """
     # Exposed input parameters
     in_parameter_list = [(k, v) for k, v in hvir["control"]["receivers"].items() if v.get("extern", None) == "param"]
     in_parameter_list.sort(key=lambda x: x[0])
     check_extern_name_conflicts("input parameter", in_parameter_list, results)
@@ -128,43 +129,49 @@
             "internal": 10,  # TODO(joe): should this increase if there are a lot of internal connections?
             "inputQueue": max(2, int(len(in_parameter_list) + len(in_event_list) / 4)),
             "outputQueue": max(2, int(len(out_parameter_list) + len(out_event_list) / 4)),
         }
     }
 
 
-def compile_dataflow(in_path, out_dir, patch_name=None, patch_meta_file=None,
-                     search_paths=None, generators=None, verbose=False,
-                     copyright=None, hvir=None):
+def compile_dataflow(
+    in_path: str,
+    out_dir: str,
+    patch_name: str = "heavy",
+    patch_meta_file: Optional[str] = None,
+    search_paths: Optional[List] = None,
+    generators: Optional[List] = None,
+    verbose: bool = False,
+    copyright: Optional[str] = None
+) -> OrderedDict:
 
-    results = OrderedDict()  # default value, empty dictionary
+    results: OrderedDict = OrderedDict()  # default value, empty dictionary
+    patch_meta = {}
 
     # basic error checking on input
     if os.path.isfile(in_path):
-        if not in_path.endswith((".pd", ".maxpat")):
-            return add_error(results, "Can only process Pd or Max files.")
+        if not in_path.endswith((".pd")):
+            return add_error(results, "Can only process Pd files.")
     elif os.path.isdir(in_path):
         if not os.path.basename("c"):
             return add_error(results, "Can only process c directories.")
     else:
         return add_error(results, f"Unknown input path {in_path}")
 
     # meta-data file
     if patch_meta_file:
         if os.path.isfile(patch_meta_file):
             with open(patch_meta_file) as json_file:
                 try:
                     patch_meta = json.load(json_file)
                 except Exception as e:
                     return add_error(results, f"Unable to open json_file: {e}")
-    else:
-        patch_meta = {}
 
-    patch_name = patch_name or "heavy"
-    generators = generators or {"c"}
+    patch_name = patch_meta.get("name", patch_name)
+    generators = ["c"] if generators is None else [x.lower() for x in generators]
 
     if in_path.endswith((".pd")):
         if verbose:
             print("--> Generating C")
         results["pd2hv"] = pd2hv.pd2hv.compile(
             pd_path=in_path,
             hv_dir=os.path.join(out_dir, "hv"),
@@ -247,19 +254,14 @@
         'num_input_channels': num_input_channels,
         'num_output_channels': num_output_channels,
         'externs': externs,
         'copyright': copyright,
         'verbose': verbose
     }
 
-    if "bela" in generators:
-        if verbose:
-            print("--> Generating Bela plugin")
-        results["c2bela"] = c2bela.c2bela.compile(**gen_args)
-
     if "fabric" in generators:
         if verbose:
             print("--> Generating Fabric plugin")
         results["c2fabric"] = c2fabric.c2fabric.compile(**gen_args)
 
     if "js" in generators:
         if verbose:
@@ -295,15 +297,15 @@
         if verbose:
             print("--> Generating Wwise plugin")
         results["c2wwise"] = c2wwise.c2wwise.compile(**gen_args)
 
     return results
 
 
-def main():
+def main() -> bool:
     tick = time.time()
 
     parser = argparse.ArgumentParser(
         description="This is the Enzien Audio Heavy compiler. It compiles supported dataflow languages into C,"
                     " and other supported frameworks.")
     parser.add_argument(
         "in_path",
@@ -316,26 +318,25 @@
         "-p",
         "--search_paths",
         nargs="+",
         help="Add a list of directories to search through for abstractions.")
     parser.add_argument(
         "-n",
         "--name",
-        default="heavy",
         help="Provides a name for the generated Heavy context.")
     parser.add_argument(
         "-m",
         "--meta",
         help="Provide metadata file (json) for generator")
     parser.add_argument(
         "-g",
         "--gen",
         nargs="+",
         default=["c"],
-        help="List of generator outputs: c, unity, wwise, js, pdext, daisy, dpf, fabric")
+        help="List of generator outputs: c, unity, wwise, js, pdext, daisy, dpf, fabric, owl")
     parser.add_argument(
         "--results_path",
         help="Write results dictionary to the given path as a JSON-formatted string."
              " Target directory will be created if it does not exist.")
     parser.add_argument(
         "-v",
         "--verbose",
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/BufferPool.py` & `hvcc-0.7.0/hvcc/core/hv2ir/BufferPool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,41 +11,42 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from collections import defaultdict
+from typing import Dict, List, Optional, Tuple
 
 from .HeavyException import HeavyException
 
 
 class BufferPool:
 
-    def __init__(self):
+    def __init__(self) -> None:
         # the idea is that the same buffer is reused as quickly as possible so that it doesn't need
         # to be moved around in the cache. It does not give substantially different results
         # from a Counter-based implementation, but it is more consistent and predictable.
-        self.pool = {
+        self.pool: Dict = {
             "~f>": defaultdict(list),
             "~i>": defaultdict(list)
         }
 
-    def num_buffers(self, connection_type=None):
+    def num_buffers(self, connection_type: Optional[str] = None) -> int:
         """ Returns the number of buffers with the given retain count. By default returns
             the size of the entire pool. Number of buffers per connection type can also be retrieved.
         """
         if connection_type is None:
             return self.num_buffers("~f>") + self.num_buffers("~i>")
         elif connection_type in self.pool:
             return sum(len(v) for v in self.pool[connection_type].values())
         else:
             raise HeavyException(f"Unknown connection type: \"{connection_type}\"")
 
-    def get_buffer(self, connection_type, count=1, excludeSet=None):
+    def get_buffer(self, connection_type: str, count: int = 1, excludeSet: Optional[set] = None) -> Tuple[str, int]:
         """ Returns a currently unused buffer. The buffer can be assigned a retain count. An optional
             exclude set can also be supplied, ensuring that the returned buffer is not one of them.
         """
         excludeSet = excludeSet if excludeSet is not None else set()
 
         pool = self.pool[connection_type]
 
@@ -54,30 +56,30 @@
             pool[0].remove(b)
         else:
             # if we get here, then no available buffer was found. Create a new one.
             b = (connection_type, self.num_buffers(connection_type))  # new buffer index for the given type
         pool[count].append(b)
         return b
 
-    def retain_buffer(self, b, count=1):
+    def retain_buffer(self, b: List, count: int = 1) -> int:
         """ Increases the retain count of the buffer. Returns the new count.
         """
         # adc~ and ZERO_BUFFER are special. They cannot be retained.
         if b[0] in {"zero", "input"}:
             return 0
         else:
             pool = self.pool[b[0]]
             for k, v in pool.items():
                 if b in v:
                     v.remove(b)
                     pool[k + count].append(b)
                     return k + count  # return the new retain count
             raise HeavyException(f"{b} not found in BufferPool!")
 
-    def release_buffer(self, b, count=1):
+    def release_buffer(self, b: List, count: int = 1) -> int:
         """ Reduces the retain count of the buffer. Returns the new count.
         """
         # adc~, ZERO_BUFFER, send~ buffers are special. They can not be released.
         # if the buffer is otherwise unknown (as may be in the case that objects provide their own),
         # they cannot be released
         if b[0] in {"zero", "input"}:
             return 0
@@ -86,9 +88,9 @@
             for k, v in pool.items():
                 if b in v:
                     v.remove(b)
                     pool[k - count].append(b)
                     return k - count  # return the new retain count
             raise HeavyException(f"{b} not found in BufferPool!")
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.pool["~f>"].__repr__() + self.pool["~i>"].__repr__()
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/Connection.py` & `hvcc-0.7.0/hvcc/core/hv2ir/Connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,94 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .HeavyIrObject import HeavyIrObject
+
+
 class Connection:
     """ A Connection describes a connection between two objects.
     """
 
-    def __init__(self, from_object, outlet_index, to_object, inlet_index, conn_type):
+    def __init__(
+        self,
+        from_object: 'HeavyIrObject',
+        outlet_index: int,
+        to_object: 'HeavyIrObject',
+        inlet_index: int,
+        conn_type: str
+    ) -> None:
         self.from_object = from_object
         self.outlet_index = outlet_index
         self.to_object = to_object
         self.inlet_index = inlet_index
         self.type = conn_type
 
         # cache the hash of this object
         self.__hash = hash((
             self.from_object, self.outlet_index,
             self.to_object, self.inlet_index,
             self.type))
 
-    def copy(self, from_object=None, outlet_index=None, to_object=None, inlet_index=None, type=None):
+    def copy(
+        self,
+        from_object: Optional['HeavyIrObject'] = None,
+        outlet_index: Optional[int] = None,
+        to_object: Optional['HeavyIrObject'] = None,
+        inlet_index: Optional[int] = None,
+        type: Optional[str] = None
+    ) -> 'Connection':
         """ Create a new connection based on the existing one, changing the given values.
         """
         return Connection(from_object=self.from_object if from_object is None else from_object,
                           outlet_index=self.outlet_index if outlet_index is None else outlet_index,
                           to_object=self.to_object if to_object is None else to_object,
                           inlet_index=self.inlet_index if inlet_index is None else inlet_index,
                           conn_type=self.type if type is None else type)
 
     @property
-    def is_signal(self):
-        return Connection.is_signal_type(self.type)
+    def is_signal(self) -> bool:
+        return self.is_signal_type(self.type)
 
     @property
-    def is_control(self):
+    def is_control(self) -> bool:
         return self.type == "-->"
 
     @property
-    def is_float_signal(self):
+    def is_float_signal(self) -> bool:
         return self.type == "~f>"
 
     @property
-    def is_integer_signal(self):
+    def is_integer_signal(self) -> bool:
         return self.type == "~i>"
 
     @property
-    def is_mixed(self):
+    def is_mixed(self) -> bool:
         return self.type == "-~>"
 
     @classmethod
-    def is_signal_type(clazz, type):
+    def is_signal_type(cls, type: Optional[str]) -> bool:
         return type in {"~i>", "~f>"}
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return self.__hash == other.__hash__() if isinstance(other, Connection) else False
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return self.__hash
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"[{self.from_object}:{self.outlet_index}] {self.type} [{self.to_object}:{self.inlet_index}]"
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrConvolution.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrTabread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HIrConvolution(HeavyIrObject):
-    """ __conv~f
+class HIrTabread(HeavyIrObject):
+    """ __tabread~if
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        assert obj_type == "__conv~f"
-        HeavyIrObject.__init__(self, obj_type, args=args, graph=graph, annotations=annotations)
-
-    def reduce(self):
-        table_obj = self.graph.resolve_object_for_name(
-            self.args["table"],
-            ["table", "__table"])
-        if table_obj is not None:
-            self.args["table_id"] = table_obj.id
-            return ({self}, [])
-        else:
-            self.add_error(f"Cannot find table named \"{self.args['table']}\" for object {self}.")
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type in {"__tabread~if", "__tabread~f", "__tabreadu~f", "__tabread"}
+        super().__init__(obj_type, args=args, graph=graph, annotations=annotations)
+
+    def reduce(self) -> Optional[tuple]:
+        if self.graph is not None:
+            table_obj = self.graph.resolve_object_for_name(
+                self.args["table"],
+                ["table", "__table"])
+            if table_obj is not None:
+                self.args["table_id"] = table_obj.id
+                return ({self}, [])
+            else:
+                self.add_error(f"Cannot find table named \"{self.args['table']}\" for object {self}.")
+
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrInlet.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrInlet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
 from .HeavyException import HeavyException
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HIrInlet(HeavyIrObject):
     """ A specific implementation of the inlet object.
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        HeavyIrObject.__init__(self, "__inlet", args=args, graph=graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        super().__init__("__inlet", args=args, graph=graph, annotations=annotations)
 
-    def _resolved_outlet_type(self, outlet_index=0):
-        connections = self.graph.inlet_connections[self.args["index"]]
-        connection_type_set = {c.type for c in connections}
-        if len(connection_type_set) == 0:
-            # object has no incident connections.
-            return "-->"  # outlet type defaults to control (-->)
-        elif len(connection_type_set) == 1:
-            return list(connection_type_set)[0]
-        else:
-            raise HeavyException(
-                f"{self} has multiple incident connections of differing type. "
-                "The outlet type cannot be explicitly resolved.")
+    def _resolved_outlet_type(self, outlet_index: int = 0) -> Optional[str]:
+        if self.graph is not None:
+            connections = self.graph.inlet_connections[self.args["index"]]
+            connection_type_set = {c.type for c in connections}
+            if len(connection_type_set) == 0:
+                # object has no incident connections.
+                return "-->"  # outlet type defaults to control (-->)
+            elif len(connection_type_set) == 1:
+                return list(connection_type_set)[0]
+            else:
+                raise HeavyException(
+                    f"{self} has multiple incident connections of differing type. "
+                    "The outlet type cannot be explicitly resolved.")
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrLorenz.py` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-# Copyright (C) 2014-2018 Enzien Audio, Ltd.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from .HeavyIrObject import HeavyIrObject
-
-
-class HIrLorenz(HeavyIrObject):
-    """ __lorenz~f
-    """
-
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        assert obj_type == "__lorenz~f"
-        HeavyIrObject.__init__(self, obj_type, args=args, graph=graph, annotations=annotations)
+/**
+ * Copyright (C) 2014-2018 Enzien Audio, Ltd.
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <http://www.gnu.org/licenses/>.
+ */
+
+#import <Foundation/Foundation.h>
+
+@interface HeavyAudio : NSObject
+
+- (void)initialiseAudioSession;
+- (void)initialiseAudioUnit;
+
+- (void)play;
+- (void)pause;
+
+- (void)overrideOutputToSpeaker:(BOOL)shouldOverride;
+
+@end
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrOutlet.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangRandom.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import random
+from typing import Optional, Dict
+
+from .HeavyLangObject import HeavyLangObject
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HIrOutlet(HeavyIrObject):
-    """ A specific implementation of the outlet object.
+class HLangRandom(HeavyLangObject):
+    """ Handles the HeavyLang "print" object.
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        HeavyIrObject.__init__(self, "__outlet", args=args, graph=graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "random"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=2,
+                         num_outlets=1,
+                         annotations=annotations)
 
-    def get_ir_on_message(self, inlet_index):
-        x = []
-        for c in self.graph.outlet_connections[self.args["index"]]:
-            x.extend(c.to_object.get_ir_on_message(c.inlet_index))
-        return x
+    def reduce(self) -> tuple:
+        self.args["seed"] = int(random.uniform(-2147483647, 2147483648))
+        x = HeavyIrObject("__random", self.args)
+        return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrPack.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrPack.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HIrPack(HeavyIrObject):
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        HeavyIrObject.__init__(self, "__pack", args=args, graph=graph,
-                               num_inlets=len(args["values"]),
-                               num_outlets=1,
-                               annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        if args is not None:
+            num_inlets = len(args["values"])
+        else:
+            num_inlets = 0
+
+        super().__init__("__pack", args=args, graph=graph,
+                         num_inlets=num_inlets,
+                         num_outlets=1,
+                         annotations=annotations)
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrReceive.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangMessage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
+from typing import Optional, Dict
+
+from .HeavyLangObject import HeavyLangObject
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HIrReceive(HeavyIrObject):
-    """ A specific implementation of the __receive object.
+class HLangMessage(HeavyLangObject):
+    """ Handles the HeavyLang "message" object.
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        HeavyIrObject.__init__(self, "__receive", args=args, graph=graph, annotations=annotations)
-        if args["extern"]:
-            # externed receivers must contain only alphanumeric characters or underscores,
-            # so that the names can be easily and transparently turned into code
-            if re.search(r"\W", args["name"]):
-                self.add_error("Parameter and Event names may only contain"
-                               f"alphanumeric characters or underscore: '{args['name']}'")
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "message"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=1,
+                         num_outlets=1,
+                         annotations=annotations)
+
+    def reduce(self) -> tuple:
+        x = HeavyIrObject("__message", self.args)
+        return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrSend.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrSend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,34 +11,46 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
+from typing import Dict, List, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HIrSend(HeavyIrObject):
     """ A specific implementation of the __send object.
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        HeavyIrObject.__init__(self, "__send", args=args, graph=graph, annotations=annotations)
-        if args["extern"]:
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        super().__init__("__send", args=args, graph=graph, annotations=annotations)
+        if args is not None and args["extern"]:
             # output parameters must contain only alphanumeric characters or underscores,
             # so that the names can be easily and transparently turned into code
             if re.search(r"\W", args["name"]):
                 self.add_error(f"Parameter and Event names may only contain \
                                 alphanumeric characters or underscore: '{args['name']}'")
 
-    def get_ir_control_list(self):
-        receive_objs = self.graph.resolve_objects_for_name(self.name, "__receive")
-        on_message_list = [x for o in receive_objs for x in o.get_ir_on_message(inlet_index=0)]
-        return [{
-            "id": self.id,
-            "onMessage": [on_message_list],
-            "extern": self.args["extern"],
-            "hash": self.args["hash"],
-            "display": self.args["name"],
-            "name": ((f"_{self.args['name']}") if re.match(r"\d", self.args["name"]) else self.args["name"])
-        }]
+    def get_ir_control_list(self) -> List:
+        if self.graph is not None and self.name is not None:
+            receive_objs = self.graph.resolve_objects_for_name(self.name, "__receive")
+            on_message_list = [x for o in receive_objs for x in o.get_ir_on_message(inlet_index=0)]
+            return [{
+                "id": self.id,
+                "onMessage": [on_message_list],
+                "extern": self.args["extern"],
+                "hash": self.args["hash"],
+                "display": self.args["name"],
+                "name": ((f"_{self.args['name']}") if re.match(r"\d", self.args["name"]) else self.args["name"])
+            }]
+        else:
+            return []
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrSwitchcase.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrSwitchcase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HIrSwitchcase(HeavyIrObject):
     """ A specific implementation of the __switchcase object.
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        HeavyIrObject.__init__(self, "__switchcase",
-                               args=args,
-                               graph=graph,
-                               num_inlets=1,
-                               num_outlets=len(args["cases"]) + 1,
-                               annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        if args is not None:
+            num_cases = len(args["cases"])
+        else:
+            num_cases = 0
+
+        super().__init__("__switchcase",
+                         args=args,
+                         graph=graph,
+                         num_inlets=1,
+                         num_outlets=num_cases + 1,
+                         annotations=annotations)
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrTabhead.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrTabhead.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HIrTabhead(HeavyIrObject):
     """ __tabhead~f and __tabhead
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
         assert obj_type in {"__tabhead~f", "__tabhead"}
-        HeavyIrObject.__init__(self, obj_type, args=args, graph=graph, annotations=annotations)
+        super().__init__(obj_type, args=args, graph=graph, annotations=annotations)
+
+    def reduce(self) -> Optional[tuple]:
+        if self.graph is not None:
+            table_obj = self.graph.resolve_object_for_name(
+                self.args["table"],
+                ["table", "__table"])
+            if table_obj is not None:
+                self.args["table_id"] = table_obj.id
+                return ({self}, [])
+            else:
+                self.add_error(f"Can't find table with name \"{self.args['table']}\".")
 
-    def reduce(self):
-        table_obj = self.graph.resolve_object_for_name(
-            self.args["table"],
-            ["table", "__table"])
-        if table_obj is not None:
-            self.args["table_id"] = table_obj.id
-            return ({self}, [])
-        else:
-            self.add_error(f"Can't find table with name \"{self.args['table']}\".")
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrTabread.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrConvolution.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HIrTabread(HeavyIrObject):
-    """ __tabread~if
+class HIrConvolution(HeavyIrObject):
+    """ __conv~f
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
-        assert obj_type in {"__tabread~if", "__tabread~f", "__tabreadu~f", "__tabread"}
-        HeavyIrObject.__init__(self, obj_type, args=args, graph=graph, annotations=annotations)
-
-    def reduce(self):
-        table_obj = self.graph.resolve_object_for_name(
-            self.args["table"],
-            ["table", "__table"])
-        if table_obj is not None:
-            self.args["table_id"] = table_obj.id
-            return ({self}, [])
-        else:
-            self.add_error(f"Cannot find table named \"{self.args['table']}\" for object {self}.")
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "__conv~f"
+        super().__init__(obj_type, args=args, graph=graph, annotations=annotations)
+
+    def reduce(self) -> Optional[tuple]:
+        if self.graph is not None:
+            table_obj = self.graph.resolve_object_for_name(
+                self.args["table"],
+                ["table", "__table"])
+            if table_obj is not None:
+                self.args["table_id"] = table_obj.id
+                return ({self}, [])
+            else:
+                self.add_error(f"Cannot find table named \"{self.args['table']}\" for object {self}.")
+
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HIrTabwrite.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrTabwrite.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HIrTabwrite(HeavyIrObject):
     """ __tabwrite~f
     """
 
-    def __init__(self, obj_type, args=None, graph=None, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
         assert obj_type in {"__tabwrite~f", "__tabwrite_stoppable~f", "__tabwrite"}
-        HeavyIrObject.__init__(self, obj_type, args=args, graph=graph, annotations=annotations)
+        super().__init__(obj_type, args=args, graph=graph, annotations=annotations)
+
+    def reduce(self) -> Optional[tuple]:
+        if self.graph is not None:
+            table_obj = self.graph.resolve_object_for_name(
+                self.args["table"],
+                ["table", "__table"])
+            if table_obj is not None:
+                self.args["table_id"] = table_obj.id
+                return ({self}, [])
+            else:
+                self.add_error(f"Can't find table with name \"{self.args['table']}\".")
 
-    def reduce(self):
-        table_obj = self.graph.resolve_object_for_name(
-            self.args["table"],
-            ["table", "__table"])
-        if table_obj is not None:
-            self.args["table_id"] = table_obj.id
-            return ({self}, [])
-        else:
-            self.add_error(f"Can't find table with name \"{self.args['table']}\".")
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangAdc.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangAdc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangAdc(HeavyLangObject):
     """ adc
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(
-            self,
-            obj_type,
-            args, graph,
-            num_inlets=0,
-            num_outlets=len(args[HeavyLangObject._HEAVY_LANG_DICT[obj_type]["args"][0]["name"]]),
-            annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "adc"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=0,
+                         num_outlets=len(args[HeavyLangObject._HEAVY_LANG_DICT[obj_type]["args"][0]["name"]]),
+                         annotations=annotations)
 
-    def _resolved_outlet_type(self, outlet_index=0):
+    def _resolved_outlet_type(self, outlet_index: int = 0) -> str:
         return "~f>"
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         objects = set()
         connections = []
 
         # reduce a HeavyLang adc to a number of individual HeavyIR __inlet objects
         for i, channel_index in enumerate(self.args["channels"]):
             if len(self.outlet_connections[i]) > 0:  # if there are any connections to this inlet
                 x = HeavyIrObject("__inlet", args={
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangBinop.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangBinop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .Connection import Connection
 from .HeavyLangObject import HeavyLangObject
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangBinop(HeavyLangObject):
 
     __HEAVY_DICT = {
         "+": ["__add", "__add_k", "__add~f", "__add~i"],
         "-": ["__sub", "__sub_k", "__sub~f", "__sub~i"],
@@ -42,24 +46,33 @@
         "atan2": ["__atan2", "__atan2_k", "__atan2~f"],
         "mod": ["__unimod", "__unimod_k"],
         "%": ["__bimod", "__bimod_k"],
         ">>": ["__shiftright", "__shiftright_k"],  # binary right shift
         "<<": ["__shiftleft", "__shiftleft_k"]  # binary left shift
     }
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, obj_type, args, graph, num_inlets=2, num_outlets=1, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional['HeavyGraph'] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        super().__init__(obj_type, args, graph,
+                         num_inlets=2,
+                         num_outlets=1,
+                         annotations=annotations)
 
     @classmethod
-    def handles_type(clazz, obj_type):
+    def handles_type(cls, obj_type: str) -> bool:
         """Returns True if this class handles the given object type. False otherwise.
         """
         return obj_type in HLangBinop.__HEAVY_DICT
 
-    def reduce(self):
+    def reduce(self) -> Optional[tuple]:
         if self.has_inlet_connection_format("__") or \
                 self.has_inlet_connection_format("_c") or \
                 self.has_inlet_connection_format("_f") or \
                 self.has_outlet_connection_format("_"):
             # binary operator objects must have a left inlet or outlet connection.
             return (set(), [])  # remove this object
 
@@ -203,7 +216,9 @@
             fmt = self._get_connection_format(self.inlet_connections)
             if "m" in fmt:
                 self.add_error(
                     "A binary operator cannot have both a signal and control "
                     f"connection to the same inlet: {fmt}")
             else:
                 self.add_error(f"Unknown inlet configuration: {fmt}")
+
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangBiquad.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangBiquad.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,36 +11,48 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
+from typing import Optional, Dict
 
 from .HeavyException import HeavyException
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangBiquad(HeavyLangObject):
     """ Translates HeavyLang object biquad to HeavyIR biquad~.
     """
 
     # used to detect valid connection configuration formats
     __re_fmt_k = re.compile("[f_][c_]+")
     __re_fmt_f = re.compile("[f_]+")
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "biquad", args, graph, num_inlets=6, num_outlets=1, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "biquad"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=6,
+                         num_outlets=1,
+                         annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         fmt = self._get_connection_format(self.inlet_connections)
-        if HLangBiquad.__re_fmt_k.search(fmt):
+        if self.__re_fmt_k.search(fmt):
             x = HeavyIrObject("__biquad_k~f", self.args)
             return {x}, self.get_connection_move_list(x)
 
-        elif HLangBiquad.__re_fmt_f.search(fmt):
+        elif self.__re_fmt_f.search(fmt):
             x = HeavyIrObject("__biquad~f", self.args)
             return {x}, self.get_connection_move_list(x)
 
         else:
             raise HeavyException(f"Unsupported connection format to biquad: {fmt}")
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangDac.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangDac.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangDac(HeavyLangObject):
     """ Translates HeavyLang [dac] to HeavyIR [__add~f].
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
         assert obj_type == "dac"
-        HeavyLangObject.__init__(
-            self,
-            obj_type,
-            args, graph,
-            num_inlets=len(args[HeavyLangObject._HEAVY_LANG_DICT["dac"]["args"][0]["name"]]),
-            num_outlets=0,
-            annotations=annotations)
+        super().__init__(obj_type, args, graph,
+                         num_inlets=len(args[HeavyLangObject._HEAVY_LANG_DICT["dac"]["args"][0]["name"]]),
+                         num_outlets=0,
+                         annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         objects = set()
         connections = []
 
         # reduce a HeavyLang dac to a number of individual HeavyIR __add~f objects
         for i, channel_index in enumerate(self.args["channels"]):
             if len(self.inlet_connections[i]) > 0:  # if there are any connections to this inlet
                 x = HeavyIrObject("__add~f")
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangDelay.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangSystem.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyIrObject import HeavyIrObject
+from typing import Optional, Dict
+
 from .HeavyLangObject import HeavyLangObject
+from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HLangDelay(HeavyLangObject):
-    """ Handle the delay object.
+class HLangSystem(HeavyLangObject):
+    """ Handles the HeavyLang "system" object.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "delay"
-        HeavyLangObject.__init__(self, "delay", args, graph,
-                                 num_inlets=2,
-                                 num_outlets=1,
-                                 annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "system"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=1,
+                         num_outlets=1,
+                         annotations=annotations)
 
-    def reduce(self):
-        x = HeavyIrObject("__delay", self.args, annotations=self.annotations)
+    def reduce(self) -> tuple:
+        x = HeavyIrObject("__system", self.args)
         return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangIf.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangIf.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangLine.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangPhasor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
-class HLangLine(HeavyLangObject):
-    """ Translates HeavyLang object [line] to HeavyIR [__line] or [__line~f].
+class HLangPhasor(HeavyLangObject):
+    """ Translates HeavyLang object [phasor] to HeavyIR [phasor~].
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "line"
-        HeavyLangObject.__init__(self, "line", args, graph,
-                                 num_inlets=2,
-                                 num_outlets=1,
-                                 annotations=annotations)
-
-    def reduce(self):
-        if self.has_outlet_connection_format("f"):
-            x = HeavyIrObject("__line~f", self.args)
-        elif self.has_outlet_connection_format("c"):
-            x = HeavyIrObject("__line", self.args)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "phasor"
+        super().__init__(obj_type, args, graph, annotations=annotations)
+
+    def reduce(self) -> tuple:
+        if self.has_inlet_connection_format(["f_", "fc"]):
+            x = HeavyIrObject("__phasor~f", self.args)
+            return ({x}, self.get_connection_move_list(x))
         else:
-            self.add_error("Unknown inlet configuration.")
-
-        return ({x}, self.get_connection_move_list(x))
+            x = HeavyIrObject("__phasor_k~f", self.args)
+            return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangMessage.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrLorenz.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyLangObject import HeavyLangObject
+from typing import Dict, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HLangMessage(HeavyLangObject):
-    """ Handles the HeavyLang "message" object.
+class HIrLorenz(HeavyIrObject):
+    """ __lorenz~f
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "message"
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=1,
-                                 num_outlets=1,
-                                 annotations=annotations)
-
-    def reduce(self):
-        x = HeavyIrObject("__message", self.args)
-        return ({x}, self.get_connection_move_list(x))
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "__lorenz~f"
+        super().__init__(obj_type, args=args, graph=graph, annotations=annotations)
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangNoise.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangNoise.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangPhasor.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangDelay.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
-class HLangPhasor(HeavyLangObject):
-    """ Translates HeavyLang object [phasor] to HeavyIR [phasor~].
+class HLangDelay(HeavyLangObject):
+    """ Handle the delay object.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "phasor", args, graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional['HeavyGraph'] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "delay"
+        super().__init__("delay", args, graph,
+                         num_inlets=2,
+                         num_outlets=1,
+                         annotations=annotations)
 
-    def reduce(self):
-        if self.has_inlet_connection_format(["f_", "fc"]):
-            x = HeavyIrObject("__phasor~f", self.args)
-            return ({x}, self.get_connection_move_list(x))
-        else:
-            x = HeavyIrObject("__phasor_k~f", self.args)
-            return ({x}, self.get_connection_move_list(x))
+    def reduce(self) -> tuple:
+        x = HeavyIrObject("__delay", self.args, annotations=self.annotations)
+        return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangPrint.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HeavyException.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyLangObject import HeavyLangObject
-from .HeavyIrObject import HeavyIrObject
+from typing import Dict
 
 
-class HLangPrint(HeavyLangObject):
-    """ Handles the HeavyLang "print" object.
+class HeavyException(Exception):
+    """ This exception is raised if anything goes wrong during the hv2ir compilation process.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "print"
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=1,
-                                 num_outlets=0,
-                                 annotations=annotations)
-
-    def reduce(self):
-        x = HeavyIrObject("__print", self.args)
-        return ({x}, self.get_connection_move_list(x))
+    def __init__(self, message: str = "") -> None:
+        super(Exception, self).__init__(message)
+        self.message = message
+        self.notes: Dict = {}
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangRandom.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangPrint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import random
+from typing import Optional, Dict
 
 from .HeavyLangObject import HeavyLangObject
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HLangRandom(HeavyLangObject):
+class HLangPrint(HeavyLangObject):
     """ Handles the HeavyLang "print" object.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "random"
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=2,
-                                 num_outlets=1,
-                                 annotations=annotations)
-
-    def reduce(self):
-        self.args["seed"] = int(random.uniform(-2147483647, 2147483648))
-        x = HeavyIrObject("__random", self.args)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "print"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=1,
+                         num_outlets=0,
+                         annotations=annotations)
+
+    def reduce(self) -> tuple:
+        x = HeavyIrObject("__print", self.args)
         return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangReceive.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangReceive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyLangObject import HeavyLangObject
 from .HIrReceive import HIrReceive
+from .HeavyGraph import HeavyGraph
 
 
 class HLangReceive(HeavyLangObject):
     """ Translates HeavyLang object [receive] to HeavyIR [__receive if control,
         otherwise for signal connections it will remove the send~/receive~ objects
         and reorder the graph.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "receive", args, graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "receive"
+        super().__init__(obj_type, args, graph, annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> Optional[tuple]:
         if self.has_outlet_connection_format(["c"]):
             x = HIrReceive("__receive", self.args, annotations=self.annotations)
             return ({x}, self.get_connection_move_list(x))
 
         elif self.has_outlet_connection_format(["f"]):
             # this case should be handled already in HeavyGraph.remap_send_receive()
             # clean up just in case
@@ -39,7 +50,8 @@
         elif self.has_outlet_connection_format("_"):
             self.add_warning("receive~ object doesn't have any outputs, this one is being removed.")
             return (set(), [])
 
         else:
             fmt = self._get_connection_format(self.outlet_connections)
             self.add_error(f"Unknown outlet configuration: {fmt}")
+            return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangSend.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangSend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyLangObject import HeavyLangObject
 from .HIrSend import HIrSend
+from .HeavyGraph import HeavyGraph
 
 
 class HLangSend(HeavyLangObject):
     """ Translates HeavyLang object [send] to HeavyIR [__send] if control,
         otherwise for signal connections it will remove the send~/receive~ objects
         and reorder the graph.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "send", args, graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "send"
+        super().__init__(obj_type, args, graph, annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> Optional[tuple]:
         if self.has_inlet_connection_format("c"):
             ir_args = dict(self.args)
             ir_args["hash"] = f"0x{HeavyLangObject.get_hash(ir_args['name']):X}"
             x = HIrSend("__send", ir_args, annotations=self.annotations)
             return ({x}, self.get_connection_move_list(x))
 
         elif self.has_inlet_connection_format("f"):
@@ -42,11 +53,13 @@
             self.add_warning("send~ object doesn't have any inputs, this one is being removed.")
             return (set(), [])
 
         elif self.has_inlet_connection_format("m"):
             self.add_error(
                 "Inlet can support either control or signal connections, "
                 "but not both at the same time.")
+            return None
 
         else:
             fmt = self._get_connection_format(self.inlet_connections)
             self.add_error(f"Unknown inlet configuration: {fmt}")
+            return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangSequence.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangSequence.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict, List
+
 from .Connection import Connection
 from .HeavyException import HeavyException
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangSequence(HeavyLangObject):
-    def __init__(self, obj_type, args, graph, annotations=None):
+
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
         # get the number of outlets that this object has
         num_outlets = len(args[HeavyLangObject._HEAVY_LANG_DICT[obj_type]["args"][0]["name"]])
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=1,
-                                 num_outlets=num_outlets,
-                                 annotations=annotations)
+        super().__init__(obj_type, args, graph,
+                         num_inlets=1,
+                         num_outlets=num_outlets,
+                         annotations=annotations)
 
-    def reduce(self):
-        cast_objs = []
+    def reduce(self) -> tuple:
+        cast_objs: List = []
         for a in self.args[self.name_for_arg()]:
             if a in {"a", "anything", "l", "list"}:
                 cast_objs.append(None)  # pass through
             elif a in {"b", "bang"}:
                 cast_objs.append(HeavyIrObject("__cast_b", {}))
             elif a in {"f", "float"}:
                 cast_objs.append(HeavyIrObject("__cast_f", {}))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangSlice.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrOutlet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyLangObject import HeavyLangObject
+from typing import Dict, List, Optional
+
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
-class HLangSlice(HeavyLangObject):
-    """ Handles the HeavyLang "slice" object.
+class HIrOutlet(HeavyIrObject):
+    """ A specific implementation of the outlet object.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "slice"
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=3,
-                                 num_outlets=2,
-                                 annotations=annotations)
-
-    def reduce(self):
-        x = HeavyIrObject("__slice", self.args)
-        return ({x}, self.get_connection_move_list(x))
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional[HeavyGraph] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        super().__init__("__outlet", args=args, graph=graph, annotations=annotations)
+
+    def get_ir_on_message(self, inlet_index: int = 0) -> List:
+        x = []
+        if self.graph is not None:
+            for c in self.graph.outlet_connections[self.args["index"]]:
+                x.extend(c.to_object.get_ir_on_message(c.inlet_index))
+        return x
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangSystem.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlTabread.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyLangObject import HeavyLangObject
-from .HeavyIrObject import HeavyIrObject
+from typing import Dict, List
 
+from .HeavyObject import HeavyObject
 
-class HLangSystem(HeavyLangObject):
-    """ Handles the HeavyLang "system" object.
-    """
-
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert obj_type == "system"
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=1,
-                                 num_outlets=1,
-                                 annotations=annotations)
-
-    def reduce(self):
-        x = HeavyIrObject("__system", self.args)
-        return ({x}, self.get_connection_move_list(x))
+
+class ControlTabread(HeavyObject):
+
+    c_struct = "ControlTabread"
+    preamble = "cTabread"
+
+    @classmethod
+    def get_C_header_set(cls) -> set:
+        return {"HvControlTabread.h"}
+
+    @classmethod
+    def get_C_file_set(cls) -> set:
+        return {"HvControlTabread.h", "HvControlTabread.c"}
+
+    @classmethod
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [
+            "cTabread_init(&cTabread_{0}, &hTable_{1}); // {2}".format(
+                obj_id,
+                args["table_id"],
+                args["table"])
+        ]
+
+    @classmethod
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
+
+    @classmethod
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return [
+            "cTabread_onMessage(_c, &Context(_c)->cTabread_{0}, {1}, m, &cTabread_{0}_sendMessage);".format(
+                obj_id,
+                inlet_index)
+        ]
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangTable.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangTable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,37 +11,46 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
+from typing import Optional, Dict
+
 from .HeavyLangObject import HeavyLangObject
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangTable(HeavyLangObject):
     """ Handles the HeavyLang "table" object.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
         assert obj_type == "table"
-        HeavyLangObject.__init__(self, obj_type, args, graph, annotations=annotations)
+        super().__init__(obj_type, args, graph, annotations=annotations)
 
         # the values argument overrides the size argument
         if len(self.args.get("values", [])) > 0:
             self.args["size"] = len(self.args["values"])
 
         if self.args["extern"]:
             # externed tables must contain only alphanumeric characters or underscores,
             # so that the names can be easily and transparently turned into code
             if re.search(r"\W", args["name"]):
                 self.add_error("Table names may only contain alphanumeric characters"
                                f"or underscore: '{args['name']}'")
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         x = HeavyIrObject("__table", self.args)
         # ensure that __table object maintains the same id as the original
         # table object. The latter is referenced by id from other objects.
         # Consistency must be maintained.
         x.id = self.id
         return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangUnop.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangUnop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyLangObject import HeavyLangObject
 from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangUnop(HeavyLangObject):
 
     __HEAVY_DICT = {
         "log": ["__log"],
         "log10": ["__log10"],
@@ -40,28 +44,34 @@
         "abs": ["__abs", "__abs~f", "__abs~i"],
         "floor": ["__floor", "__floor~f"],
         "ceil": ["__ceil", "__ceil~f"],
         "cast_fi": ["__cast~fi"],
         "cast_if": ["__cast~if"]
     }
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        assert HLangUnop.handles_type(obj_type)
-        HeavyLangObject.__init__(self, obj_type, args, graph,
-                                 num_inlets=1,
-                                 num_outlets=1,
-                                 annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert self.handles_type(obj_type)
+        super().__init__(obj_type, args, graph,
+                         num_inlets=1,
+                         num_outlets=1,
+                         annotations=annotations)
 
     @classmethod
-    def handles_type(clazz, obj_type):
+    def handles_type(cls, obj_type: str) -> bool:
         """ Returns True if this class handles the given object type. False otherwise.
         """
         return obj_type in HLangUnop.__HEAVY_DICT
 
-    def reduce(self):
+    def reduce(self) -> Optional[tuple]:
         if len(self.inlet_connections[0]) == 0:
             self.add_error("Unary operator objects must have an input.")
 
         # TODO(mhroth): there is no general consensus on how to handle incoming
         # and outgoing connections of different types, given the local let-type
         # definitions.
 
@@ -84,7 +94,8 @@
         elif self.has_inlet_connection_format("c"):
             ir_type = f"__{self.type}"
             assert ir_type in HLangUnop.__HEAVY_DICT[self.type]
             x = HeavyIrObject(ir_type)
             return ({x}, self.get_connection_move_list(x, "-->"))
         else:
             self.add_error("Unknown inlet configuration.")
+            return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangVar.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangVar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangVar(HeavyLangObject):
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "var", args, graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "var"
+        super().__init__(obj_type, args, graph, annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         if self.has_inlet_connection_format("_") and self.has_outlet_connection_format("f"):
             x = HeavyIrObject("__var_k~f", self.args)
         elif self.has_inlet_connection_format("_") and self.has_outlet_connection_format("i"):
             x = HeavyIrObject("__var_k~i", self.args)
         elif self.has_inlet_connection_format(["_", "c"]) and self.has_outlet_connection_format("f"):
             x = HeavyIrObject("__var~f", self.args)
             x.id = self.id
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HLangVario.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangVario.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,64 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, Dict
+
 from .HeavyException import HeavyException
 from .HeavyIrObject import HeavyIrObject
 from .HeavyLangObject import HeavyLangObject
+from .HeavyGraph import HeavyGraph
 
 
 class HLangVario(HeavyLangObject):
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "vario", args, graph, annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "vario"
+        super().__init__(obj_type, args, graph, annotations=annotations)
+
+    def reduce(self) -> Optional[tuple]:
+        if self.graph is not None and self.name is not None:
+            var_obj = self.graph.resolve_object_for_name(self.name, "var")
+            if var_obj is None:
+                raise HeavyException(
+                    f"No corresponding \"var\" object found for object {self} in file {self.graph.file}"
+                )
+
+            if self.has_inlet_connection_format("f") and self.has_outlet_connection_format("_"):
+                x = HeavyIrObject("__varwrite~f", {"var_id": var_obj.id})
+                return {x}, self.get_connection_move_list(x)
+
+            elif self.has_inlet_connection_format("i") and self.has_outlet_connection_format("_"):
+                x = HeavyIrObject("__varwrite~i", {"var_id": var_obj.id})
+                return {x}, self.get_connection_move_list(x)
+
+            elif self.has_inlet_connection_format("_") and self.has_outlet_connection_format("f"):
+                x = HeavyIrObject("__varread~f", {"var_id": var_obj.id})
+                return {x}, self.get_connection_move_list(x)
+
+            elif self.has_inlet_connection_format("_") and self.has_outlet_connection_format("i"):
+                x = HeavyIrObject("__varread~i", {"var_id": var_obj.id})
+                return {x}, self.get_connection_move_list(x)
 
-    def reduce(self):
-        var_obj = self.graph.resolve_object_for_name(self.name, "var")
-        if var_obj is None:
-            raise HeavyException(f"No corresponding \"var\" object found for object {self} in file {self.graph.file}")
-
-        if self.has_inlet_connection_format("f") and self.has_outlet_connection_format("_"):
-            x = HeavyIrObject("__varwrite~f", {"var_id": var_obj.id})
-            return {x}, self.get_connection_move_list(x)
-
-        elif self.has_inlet_connection_format("i") and self.has_outlet_connection_format("_"):
-            x = HeavyIrObject("__varwrite~i", {"var_id": var_obj.id})
-            return {x}, self.get_connection_move_list(x)
-
-        elif self.has_inlet_connection_format("_") and self.has_outlet_connection_format("f"):
-            x = HeavyIrObject("__varread~f", {"var_id": var_obj.id})
-            return {x}, self.get_connection_move_list(x)
-
-        elif self.has_inlet_connection_format("_") and self.has_outlet_connection_format("i"):
-            x = HeavyIrObject("__varread~i", {"var_id": var_obj.id})
-            return {x}, self.get_connection_move_list(x)
+            else:
+                raise Exception()
 
-        else:
-            raise Exception()
+        return None
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HeavyGraph.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HeavyGraph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from collections import Counter
 import os
 import re
+from collections import Counter
+from typing import Optional, Union, Dict, List
 
 from .BufferPool import BufferPool
 from .Connection import Connection
 from .LocalVars import LocalVars
 from .HeavyException import HeavyException
 from .HeavyIrObject import HeavyIrObject
 from .HIrReceive import HIrReceive
@@ -28,49 +30,58 @@
 
 class HeavyGraph(HeavyIrObject):
     """ Represents a graph. Subclasses HeavyIrObject for functionality.
         "__graph" does exist as a HeavyIR object, though it has no functionality
         and should not appear in any IR output.
     """
 
-    def __init__(self, graph=None, graph_args=None, file=None, xname=None):
+    def __init__(
+        self,
+        graph: Optional['HeavyGraph'] = None,
+        graph_args: Optional[Dict] = None,
+        file: str = "",
+        xname: str = "heavy"
+    ) -> None:
         # zero inlets and outlets until inlet/outlet objects are declared
-        HeavyIrObject.__init__(self, "__graph", graph_args, graph, 0, 0)
+        super().__init__("__graph", graph_args, graph, 0, 0)
 
         # the heavy file which defines this graph
         self.file = file
 
         # a user-defined name of this graph
-        self.xname = xname or "heavy"
+        self.xname = xname
 
         # the dictionary of all objects in the graph
-        self.objs = {}
+        self.objs: Dict = {}
 
         # set the local arguments
-        self.args = graph_args or {}
+        if graph_args is not None:
+            self.args = graph_args
+        else:
+            self.args = {}
 
         # initialise the local variables
         self.local_vars = LocalVars()
 
         # the list of all constituent inlet and outlet objects
         # graphs always start with no inlet/outlets
-        self.inlet_objs = []
-        self.outlet_objs = []
+        self.inlet_objs: List = []
+        self.outlet_objs: List = []
 
         # the set of input/output channels that this graph writes to
-        self.input_channel_set = set()
-        self.output_channel_set = set()
+        self.input_channel_set: set = set()
+        self.output_channel_set: set = set()
 
         # an ordered list of signal objects to process
-        self.signal_order = []
+        self.signal_order: List = []
 
         # a pool of signal buffers for use during signal ordering and buffer assignment
-        self.buffer_pool = None
+        self.buffer_pool: Optional[BufferPool] = None
 
-    def resolve_arguments(self, obj_args):
+    def resolve_arguments(self, obj_args: Dict) -> Dict:
         """ Resolves the object arguments based on values from the local graph.
         """
         args = dict(obj_args)  # make a copy of the input arguments
         for key, value in args.items():
             # do any of them reference a variable input?
             if isinstance(value, str):
                 if value.find("$") > -1:
@@ -95,39 +106,39 @@
                         # removed from the argument dictionary
                         args.pop(key, None)
                         self.add_warning(f"Variable \"{key}\":\"{value}\" could not be resolved.")
                     else:
                         args[key] = value
         return args
 
-    def connect_objects(self, c, require_intra_graph_connection=True):
+    def connect_objects(self, c: Connection, require_intra_graph_connection: bool = True) -> None:
         """ Establish a connection from one object to another.
             Typically a connection must be made within a single graph, though
             this requirement may be subpressed.
         """
         if require_intra_graph_connection:
             assert c.from_object.graph is c.to_object.graph, \
                 f"Conection established between two objects not in the same graph: {c}"
 
         # add the connection from the parent to the child
         c.from_object.add_connection(c)
 
         # add the connection to the child from the parent
         c.to_object.add_connection(c)
 
-    def disconnect_objects(self, c):
+    def disconnect_objects(self, c: Connection) -> None:
         """ Remove a connection from one object to another.
         """
         # remove the connection from the parent to the child
         c.from_object.remove_connection(c)
 
         # remove the connection to the child from the parent
         c.to_object.remove_connection(c)
 
-    def update_connection(self, c, n_list):
+    def update_connection(self, c: Connection, n_list: List) -> None:
         """ Update the old connection (c) with the new connections (n_list).
             Connection order is maintained. If c is None, this method acts
             as connect_objects(). If n is empty, this method acts as disconnect_objects().
         """
         if c is not None and len(n_list) > 0:
             if all([c.from_object is n.from_object for n in n_list]):
                 # connections start at the same point
@@ -145,15 +156,19 @@
                 raise HeavyException(f"Connections must have a common endpoint: {c} / {n_list}")
         elif c is not None and len(n_list) == 0:
             self.disconnect_objects(c)  # remove connection c
         elif c is None and len(n_list) > 0:
             for n in n_list:
                 self.connect_objects(n)  # add connection n
 
-    def add_object(self, obj, obj_id=None):
+    def add_object(
+        self,
+        obj: HeavyIrObject,
+        obj_id: Optional[Union[int, str]] = None
+    ) -> None:
         """ Add an object to the graph based on the given id.
             Per-object bookkeeping is performed.
         """
 
         obj_id = obj_id or obj.id
         if obj_id not in self.objs:
             obj.graph = self
@@ -190,48 +205,71 @@
                     obj,
                     obj.name,
                     static=obj.static,
                     unique=True)
         else:
             self.add_error(f"Duplicate object id {obj_id} found in graph.")
 
-    def __register_named_object(self, obj, name=None, static=False, unique=False):
+    def __register_named_object(
+        self,
+        obj: HeavyIrObject,
+        name: Optional[str] = None,
+        static: bool = False,
+        unique: bool = False
+    ) -> None:
         """ Register a named object at the appropriate graph level.
         """
 
         name = name or obj.name
-        if obj.scope == "private" and not static:
-            # stay at this level
-            self.local_vars.register_object(obj, name, static, unique)
-        elif obj.scope == "protected":
-            # go up one level
-            g = self.graph if self.graph is not None else self
-            g.local_vars.register_object(obj, name, static, unique)
-        elif obj.scope == "public" or static:
-            self.get_root_graph().local_vars.register_object(obj, name, static, unique)
+        if name is not None:
+            if obj.scope == "private" and not static:
+                # stay at this level
+                self.local_vars.register_object(obj, name, static, unique)
+            elif obj.scope == "protected":
+                # go up one level
+                g = self.graph if self.graph is not None else self
+                g.local_vars.register_object(obj, name, static, unique)
+            elif obj.scope == "public" or static:
+                self.get_root_graph().local_vars.register_object(obj, name, static, unique)
+            else:
+                raise HeavyException(f"Unknown scope \"{obj.scope}\" for object {obj}.")
         else:
             raise HeavyException(f"Unknown scope \"{obj.scope}\" for object {obj}.")
 
-    def __unregister_named_object(self, obj, name=None, static=False, unique=False):
+    def __unregister_named_object(
+        self,
+        obj: HeavyIrObject,
+        name: Optional[str] = None,
+        static: bool = False,
+        unique: bool = False
+    ) -> None:
         """ Unregister a named object at the appropriate graph level.
         """
 
         name = name or obj.name
-        if obj.scope == "private" and not static:
-            self.local_vars.unregister_object(obj, name)
-        elif obj.scope == "protected":
-            # go up one level
-            g = self.graph if self.graph is not None else self
-            g.local_vars.unregister_object(obj, name)
-        elif obj.scope == "public" or static:
-            self.get_root_graph().local_vars.unregister_object(obj, name)
+        if name is not None:
+            if obj.scope == "private" and not static:
+                self.local_vars.unregister_object(obj, name)
+            elif obj.scope == "protected":
+                # go up one level
+                g = self.graph if self.graph is not None else self
+                g.local_vars.unregister_object(obj, name)
+            elif obj.scope == "public" or static:
+                self.get_root_graph().local_vars.unregister_object(obj, name)
+            else:
+                raise HeavyException(f"Unknown scope \"{obj.scope}\" for object {obj}.")
         else:
             raise HeavyException(f"Unknown scope \"{obj.scope}\" for object {obj}.")
 
-    def resolve_objects_for_name(self, name, obj_types, local_graph=None):
+    def resolve_objects_for_name(
+        self,
+        name: str,
+        obj_types: Union[List, str],
+        local_graph: Optional['HeavyGraph'] = None
+    ) -> List:
         """ Returns all objects with the given name and type that are visible
             from this graph. Returns an empty list if no objects could be found.
             The results are otherwise ordered from most local/private first,
             and the most global last.
         """
 
         obj_types = obj_types if isinstance(obj_types, list) else [obj_types]
@@ -242,44 +280,55 @@
 
         if self.graph is not None:
             obj_list_from_super_graph = self.graph.resolve_objects_for_name(name, obj_types, local_graph)
             obj_list.extend(obj_list_from_super_graph)
 
         return obj_list
 
-    def resolve_object_for_name(self, name, obj_types, local_graph=None):
+    def resolve_object_for_name(
+        self,
+        name: str,
+        obj_types: Union[List, str],
+        local_graph: Optional['HeavyGraph'] = None
+    ) -> Optional[HeavyIrObject]:
         """ Returns the first object with the given name and type that is visible
             from this graph. Returns None if no objects are available.
             This is a convenience method.
         """
 
         objs = self.resolve_objects_for_name(name, obj_types, local_graph)
         return objs[0] if len(objs) > 0 else None
 
-    def is_root_graph(self):
+    def is_root_graph(self) -> bool:
         """ Returns true if this is the top-level (i.e. root) graph. False otherwise.
         """
         return self.graph is None
 
-    def get_root_graph(self):
+    def get_root_graph(self) -> 'HeavyGraph':
         """Returns the top-level graph.
         """
-        return self if self.is_root_graph() else self.graph.get_root_graph()
+        if self.is_root_graph():
+            return self
+        elif self.graph is not None:
+            return self.graph.get_root_graph()
+        else:
+            # NOTE(dromer): we should never get here
+            raise Exception
 
-    def find_path_for_abstraction(self, obj_type):
+    def find_path_for_abstraction(self, obj_type: str) -> Optional[str]:
         """ Travels up the graph heirarchy looking for a file path to an abstraction.
             Returns None if no abstraction is found.
         """
         file_path = self.local_vars.find_path_for_abstraction(obj_type)
         if file_path is not None:
             return file_path
         else:
             return self.graph.find_path_for_abstraction(obj_type) if self.graph is not None else None
 
-    def remove_object(self, o, obj_id=None):
+    def remove_object(self, o: HeavyIrObject, obj_id: Optional[str] = None) -> None:
         """ Removes an object and all of its connections from the graph.
             A custom id for the object to be removed can be given.
         """
         for connections in o.inlet_connections:
             for c in list(connections):  # make copy of connections as it will be mutated
                 self.disconnect_objects(c)
         for connections in o.outlet_connections:
@@ -290,85 +339,85 @@
             if o is v:
                 del self.objs[k]
                 break
 
         if o.type in {"receive", "__receive", "send", "__send"}:
             self.__unregister_named_object(o, o.name)
 
-    def get_inlet_object(self, index):
+    def get_inlet_object(self, index: int) -> HeavyIrObject:
         """ Returns the indexed inlet object of this graph.
         """
         return self.inlet_objs[index]
 
-    def get_outlet_object(self, index):
+    def get_outlet_object(self, index: int) -> HeavyIrObject:
         """ Returns the indexed outlet object of this graph.
         """
         return self.outlet_objs[index]
 
-    def get_input_channel_set(self, recursive=False):
+    def get_input_channel_set(self, recursive: bool = False) -> set:
         """ Returns the set of input channels that this graph writes to.
             Optionally includes all subgraphs as well.
         """
         if recursive:
             channels = set(self.input_channel_set)  # copy the output channel set
             for o in [o for o in self.objs.values() if o.type == "__graph"]:
                 channels.update(o.get_input_channel_set(recursive=True))
             return channels
         else:
             return self.input_channel_set
 
-    def get_output_channel_set(self, recursive=False):
+    def get_output_channel_set(self, recursive: bool = False) -> set:
         """ Returns the set of output channels that this graph writes to.
             Optionally includes all subgraphs as well.
         """
         if recursive:
             channels = set(self.output_channel_set)  # copy the output channel set
             for o in [o for o in self.objs.values() if o.type == "__graph"]:
                 channels.update(o.get_output_channel_set(recursive=True))
             return channels
         else:
             return self.output_channel_set
 
-    def get_notices(self):
+    def get_notices(self) -> Dict:
         notices = HeavyLangObject.get_notices(self)
         for o in self.objs.values():
             n = o.get_notices()
             notices["warnings"].extend(n["warnings"])
             notices["errors"].extend(n["errors"])
         return notices
 
-    def get_objects_for_type(self, obj_type, recursive=False):
+    def get_objects_for_type(self, obj_type: str, recursive: bool = False) -> List:
         """ Returns a list of all objects of a given type in this graph.
             The optional parameter "recursive" also includes all objects from subgraphs.
         """
         obj_list = []
         for o in self.objs.values():
             if o.type == "__graph" and recursive:
                 obj_list.extend(o.get_objects_for_type(obj_type, recursive))
             elif o.type == obj_type:
                 obj_list.append(o)
         return obj_list
 
-    def get_object_counter(self, recursive=False):
+    def get_object_counter(self, recursive: bool = False) -> Counter:
         """ Returns a counter of all object types in this graph.
             Graph objects are explicitly removed. "__inlet" and "__outlet"
             objects are renamed to "inlet" and "outlet", for clarity.
             An optional recursive argument includes all subgraphs.
         """
-        c = Counter()
+        c: Counter = Counter()
         for o in self.objs.values():
             if o.type == "__graph" and recursive:
                 c += o.get_object_counter(recursive=True)
             elif o.type in {"__inlet", "__outlet"}:
                 c[o.type[2:]] += 1  # remove leading "__"
             else:
                 c[o.type] += 1
         return c
 
-    def prepare(self):
+    def prepare(self) -> None:
         """ Prepares a graph to be exported. Must be called from a root graph.
         """
         assert self.is_root_graph()
 
         try:
             # apply graph transformations when all graphs have been read
             # All transformations must be recursive.
@@ -411,15 +460,15 @@
             self.assign_signal_buffers()
         except HeavyException as e:
             e.notes = self.get_notices()
             e.notes["has_error"] = True
             e.notes["exception"] = e
             raise e
 
-    def _remove_unused_inlet_connections(self):
+    def _remove_unused_inlet_connections(self) -> None:
         """ Remove connections from inlet object, if there are no incoming
             connections to it. This is a basic approach to pruning unused or
             unnecessary connections, which allow further optimisation later
             in the pipeline.
         """
         for i, cc in enumerate(self.inlet_connections):
             if len(cc) == 0:
@@ -427,27 +476,27 @@
                 for c in list(self.inlet_objs[i].outlet_connections[0]):
                     self.disconnect_objects(c)
 
         # the recursive bit
         for o in [o for o in self.objs.values() if (o.type == "__graph")]:
             o._remove_unused_inlet_connections()
 
-    def _resolved_outlet_type(self, outlet_index=0):
+    def _resolved_outlet_type(self, outlet_index: int = 0) -> str:
         # a graph's outlet type depends on the connections incident on the
         # corresponding outlet object
         connection_type_set = {c.type for c in self.outlet_objs[outlet_index].inlet_connections[0]}
         if len(connection_type_set) == 0:
             return "-->"  # object has no incident connections, default to -->
         elif len(connection_type_set) == 1:
             return list(connection_type_set)[0]
         else:
             raise HeavyException(f"{self} has multiple incident connections of differing type.\
                                   The outlet type cannot be explicitly resolved.")
 
-    def _resolve_connection_types(self, obj_stack=None):
+    def _resolve_connection_types(self, obj_stack: Optional[set] = None) -> Optional[None]:
         """ Resolves the type of all connections before reduction to IR object types.
             If connections incident on an object are incompatible, they are either
             resolved, potentially by inserting conversion objects, or pruned.
             If a viable resolution cannot be found, an exception may be raised.
         """
         obj_stack = obj_stack or set()
         if self in obj_stack:
@@ -464,15 +513,15 @@
         for c in [c for cc in self.outlet_connections for c in cc]:
             if c.is_mixed:
                 # resolve connection type and update it
                 connection_type = self._resolved_outlet_type(c.outlet_index)
                 self.update_connection(c, [c.copy(type=connection_type)])
             c.to_object._resolve_connection_types(obj_stack)  # turtle on down
 
-    def remap_send_receive(self):
+    def remap_send_receive(self) -> None:
         """ Recursively finds all signal send/receive objects and for each unique
             send name, get all of the sends, and all of the corresponding receives.
             Reconnect all incoming connections to a __add~f, and fan out the results
             to all of receivers' connections. At most one __add~f must
             be added, and a lot of connections remapped.
         """
 
@@ -542,15 +591,15 @@
 
             # when all is said and done, remove the send and receive objects
             for o in s_list:
                 o.graph.remove_object(o)
             for o in r_list:
                 o.graph.remove_object(o)
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         """ Breaks this object into low-level objects. This method returns either
             the object that it is called on, or a graph. In case of a graph, it contains
             only low-level objects. Unnecessary connections are pruned. Because
             this method is called on graphs while they are being constructed, returned
             graphs contains no sub-graphs. Thus this method does not process subgraphs.
         """
         # refactor all constituent objects
@@ -582,15 +631,15 @@
             # remove the old object (and any remaining connections) from the graph
             self.remove_object(o, obj_id=obj_id)
             # o.id may not be the same as obj_id if the object comes from an abstraction
 
         # a graph is reduced in-place and does not change any connections
         return ({self}, [])
 
-    def cascade_expansion(self):
+    def cascade_expansion(self) -> None:
         """ Turns implicit +~ into explicit cascading +~ trees.
             It is assumed that this simplification operation is run on a reduced graph.
         """
         for o in self.objs.copy().values():  # all items in the graph
             for i in range(len(o.inlet_connections)):  # for each inlet
                 # if there is more than one signal connection
                 # get all of the signal connections to an object at this inlet
@@ -629,15 +678,15 @@
                         to_object=o,
                         inlet_index=i,
                         conn_type="~f>"))
 
             if o.type == "__graph":
                 o.cascade_expansion()
 
-    def fma_replacement(self):
+    def fma_replacement(self) -> None:
         """ Replace:
             [__mul~f] ~f> [__add~f] with [__fma~f] or
             [__mul~f] ~f> [__sub~f] with [__fms~f]
         """
         # for all __mul~f objects
         for o in self.objs.copy().values():
             if o.type == "__mul~f" \
@@ -679,15 +728,15 @@
                 # (along with any remaining connections)
                 o.graph.remove_object(o)  # *~
                 o_add.graph.remove_object(o_add)  # +~
 
             elif o.type == "__graph":
                 o.fma_replacement()  # recurse through all subgraphs
 
-    def group_control_receivers(self):
+    def group_control_receivers(self) -> None:
         """ Group all control receivers with the same name under one receiver
             with that name. This way only one message must be scheduled to hit
             all receivers.
         """
 
         for name, receivers in self.local_vars.get_registered_objects_for_type("__receive").items():
 
@@ -725,34 +774,38 @@
                     self.connect_objects(c.copy(from_object=recv), require_intra_graph_connection=False)
 
             # remove old receivers
             for r in receivers:
                 r.graph.remove_object(r)
 
     @property
-    def does_process_signal(self):
+    def does_process_signal(self) -> bool:
         # this graph processes a signal if it contains any adc~ (__inlet
         # objects with index > 127)
         return any(o.does_process_signal for o in self.objs.values()) or \
             any(o.args["index"] > 127 for o in self.inlet_objs)
 
-    def order_signal_objects(self):
+    def order_signal_objects(self) -> None:
         """ Places the signal objects in the correct order to be processed.
             Only the objects in this graph are ordered, stopping at the inlet objects.
         """
         # for all leaves of graph, get the parent objects and combine the lists
         self.signal_order = []  # ordered objects
         for o in [o for o in self.objs.values() if o.is_leaf()]:
             self.signal_order.extend(o.get_parent_order())
 
         # retain only objects that process a signal
         self.signal_order = [o for o in self.signal_order if o.does_process_signal]
 
-    def assign_signal_buffers(self, buffer_pool=None):
-        self.buffer_pool = buffer_pool or BufferPool()  # the top-level graph owns the buffer pool
+    def assign_signal_buffers(self, buffer_pool: Optional[BufferPool] = None) -> None:
+        # the top-level graph owns the buffer pool
+        if buffer_pool is not None:
+            self.buffer_pool = buffer_pool
+        else:
+            self.buffer_pool = BufferPool()
 
         # before signal buffers can be assigned, the objects must be ordered
         self.order_signal_objects()
 
         for c_list in self.inlet_connections:
             c_list = [c for c in c_list if c.is_signal]  # only consider signal connections to inlet
             if len(c_list) == 0:
@@ -790,90 +843,94 @@
                 buf = c.from_object.outlet_buffers[c.outlet_index]
                 self.outlet_buffers[i] = buf
                 self.buffer_pool.retain_buffer(buf, len(self.outlet_connections[i]) - 1)
             else:
                 raise HeavyException(
                     f"Object {outlet_obj} in graph {outlet_obj.graph.file} has {len(c_list)} (> 1) signal inputs.")
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self.xname is not None:
             # TODO(mhroth): does not handle nested subgraph
             return f"__graph.{self.id}({os.path.basename(self.file)}/{self.xname})"
         else:
             return f"__graph.{self.id}({os.path.basename(self.file)})"
 
     #
     # Intermediate Representation generators
     #
 
-    def to_ir(self):
+    def to_ir(self) -> Optional[Dict]:
         """ Returns Heavy intermediate representation.
         """
 
         # the set of all input/output signal channels used by the graph
         input_channel_set = self.get_input_channel_set(recursive=True)
         output_channel_set = self.get_output_channel_set(recursive=True)
 
-        return {
-            "name": {
-                "escaped": re.sub(r"\W", "_", self.xname),
-                "display": self.xname
-            },
-            "objects": self.get_object_dict(),
-            "init": {
-                "order": self.get_ir_init_list()
-            },
-            "tables": self.get_ir_table_dict(),
-            "control": {
-                "receivers": self.get_ir_receiver_dict(),
-                "sendMessage": self.get_ir_control_list()
-            },
-            "signal": {
-                "numInputBuffers": max(input_channel_set) if len(input_channel_set) > 0 else 0,
-                "numOutputBuffers": max(output_channel_set) if len(output_channel_set) > 0 else 0,
-                "numTemporaryBuffers": {
-                    "float": self.buffer_pool.num_buffers("~f>"),
-                    "integer": self.buffer_pool.num_buffers("~i>")
+        if self.buffer_pool is not None:
+            return {
+                "name": {
+                    "escaped": re.sub(r"\W", "_", self.xname),
+                    "display": self.xname
+                },
+                "objects": self.get_object_dict(),
+                "init": {
+                    "order": self.get_ir_init_list()
+                },
+                "tables": self.get_ir_table_dict(),
+                "control": {
+                    "receivers": self.get_ir_receiver_dict(),
+                    "sendMessage": self.get_ir_control_list()
                 },
-                "processOrder": self.get_ir_signal_list()
+                "signal": {
+                    "numInputBuffers": max(input_channel_set) if len(input_channel_set) > 0 else 0,
+                    "numOutputBuffers": max(output_channel_set) if len(output_channel_set) > 0 else 0,
+                    "numTemporaryBuffers": {
+                        "float": self.buffer_pool.num_buffers("~f>"),
+                        "integer": self.buffer_pool.num_buffers("~i>")
+                    },
+                    "processOrder": self.get_ir_signal_list()
+                }
             }
-        }
+        else:
+            # we should never get here
+            raise Exception
 
-    def get_object_dict(self):
+    def get_object_dict(self) -> Dict:
         # d = {o.id: o.get_object_dict() for o in self.objs.values() if o.type not in
         # ["inlet", "__inlet", "outlet", "__outlet"]}
         d = {}
         for o in self.objs.values():
             # NOTE(mhroth): a bit of a hack to remove unnecessary inlet and outlet ir objects
             if o.type not in ["inlet", "__inlet", "outlet", "__outlet"]:
                 d.update(o.get_object_dict())
         return d
 
-    def get_ir_init_list(self):
+    def get_ir_init_list(self) -> List:
         """ Init list is returned with all signal objects at the front,
             in the order that they are processed. This is to reduce cache misses
             on the signal object state as the process function is executed.
         """
         init_list = [x for o in self.objs.values() for x in o.get_ir_init_list()]
         signal_list = self.get_ir_signal_list()
         s_init_list = [x["id"] for x in signal_list if x["id"] in init_list]
         i_init_list = [o_id for o_id in init_list if o_id not in s_init_list]
         ordered_init_list = s_init_list + i_init_list
         # ordered_init_list = list(OrderedDict.fromkeys(s_init_list + i_init_list))
         return ordered_init_list
 
-    def get_ir_on_message(self, inlet_index):
+    def get_ir_on_message(self, inlet_index: int = 0) -> List:
         # pass the method through the inlet object, but only follow control connections
         x = []
         for c in self.inlet_objs[inlet_index].outlet_connections[0]:
             if c.is_control:
                 x.extend(c.to_object.get_ir_on_message(c.inlet_index))
         return x
 
-    def get_ir_table_dict(self):
+    def get_ir_table_dict(self) -> Dict:
         """ Returns a dictionary of all publicly visible tables at the root graph
             and their ids.
         """
         assert self.is_root_graph(), "This function should only be called from the root graph."
         d = self.local_vars.get_registered_objects_for_type("__table")
         # update(), because tables can be registered either as Heavy tables
         # or HeavyIr __tables. We need to be able to handle them both.
@@ -888,25 +945,25 @@
                     "id": v[0].id,
                     "display": k,
                     "hash": f"0x{HeavyLangObject.get_hash(k):X}",
                     "extern": v[0].args["extern"]
                 }
         return e
 
-    def get_ir_control_list(self):
+    def get_ir_control_list(self) -> List:
         return [x for o in self.objs.values() for x in o.get_ir_control_list()]
 
-    def get_ir_receiver_dict(self):
+    def get_ir_receiver_dict(self) -> Dict:
         # NOTE(mhroth): this code assumes that v is always an array of length 1,
         # as the grouping of control receivers should have grouped all same-named
         # receivers into one logical receiver.
         # NOTE(mhroth): a code-compatible name is only necessary for externed receivers
         return {((f"_{k}") if re.match(r"\d", k) else k): {
             "display": k,
             "hash": f"0x{HeavyLangObject.get_hash(k):X}",
             "extern": v[0].args["extern"],
             "attributes": v[0].args["attributes"],
             "ids": [v[0].id]
         } for k, v in self.local_vars.get_registered_objects_for_type("__receive").items()}
 
-    def get_ir_signal_list(self):
+    def get_ir_signal_list(self) -> List:
         return [x for o in self.signal_order for x in o.get_ir_signal_list()]
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HeavyIrObject.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HeavyIrObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,49 +13,63 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import os
 
-from hvcc.core.hv2ir.Connection import Connection
-from hvcc.core.hv2ir.HeavyException import HeavyException
-from hvcc.core.hv2ir.HeavyLangObject import HeavyLangObject
+from typing import Dict, List, Optional, TYPE_CHECKING
+
+from .Connection import Connection
+from .HeavyException import HeavyException
+from .HeavyLangObject import HeavyLangObject
+from .BufferPool import BufferPool
+
+if TYPE_CHECKING:
+    from .HeavyGraph import HeavyGraph
 
 
 class HeavyIrObject(HeavyLangObject):
     """ Intermediate Representation (IR) objects are atomic and have
         strictly defined interfaces and types. These are generally defined in
         the file heavy.ir.json.
     """
 
     # load the HeavyIR object definitions
     with open(os.path.join(os.path.dirname(__file__), "../json/heavy.ir.json"), "r") as f:
         __HEAVY_OBJS_IR_DICT = json.load(f)
 
-    def __init__(self, obj_type, args=None, graph=None, num_inlets=-1, num_outlets=-1, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional['HeavyGraph'] = None,
+        num_inlets: int = -1,
+        num_outlets: int = -1,
+        annotations: Optional[Dict] = None
+    ) -> None:
         # allow the number of inlets and outlets to be overridden
         num_inlets = len(HeavyIrObject.__HEAVY_OBJS_IR_DICT[obj_type]["inlets"]) if num_inlets < 0 else num_inlets
 
         num_outlets = len(HeavyIrObject.__HEAVY_OBJS_IR_DICT[obj_type]["outlets"]) if num_outlets < 0 else num_outlets
 
-        HeavyLangObject.__init__(self, obj_type, args, graph, num_inlets, num_outlets, annotations)
+        super().__init__(obj_type, args, graph, num_inlets, num_outlets, annotations)
 
         # resolve arguments and fill in missing defaults for HeavyIR objects
         self.__resolve_default_ir_args()
 
         # the list of signal buffers at the inlets and outlets
         # these are filled in by HeavyGraph.assign_signal_buffers()
         self.inlet_buffers = [("zero", 0)] * self.num_inlets
         self.outlet_buffers = [("zero", 0)] * self.num_outlets
 
         # True if this object has already been ordered in the signal chain
         self.__is_ordered = False
 
-    def __resolve_default_ir_args(self):
+    def __resolve_default_ir_args(self) -> None:
         """ Resolves missing default arguments. Also checks to make sure that all
             required arguments are present.
         """
         if self.type in HeavyIrObject.__HEAVY_OBJS_IR_DICT:
             for arg in self.__obj_desc.get("args", []):
                 if arg["name"] not in self.args:
                     # if a defined argument is not in the argument dictionary
@@ -69,46 +84,46 @@
                     if arg["default"] is not None:
                         self.args[arg["name"]] = HeavyLangObject.force_arg_type(
                             self.args[arg["name"]],
                             arg["value_type"],
                             self.graph)
 
     @classmethod
-    def is_ir(clazz, obj_type):
+    def is_ir(cls, obj_type: str) -> bool:
         """Returns true if the type is an IR object. False otherwise.
         """
         return obj_type in HeavyIrObject.__HEAVY_OBJS_IR_DICT
 
     @property
-    def does_process_signal(self):
+    def does_process_signal(self) -> bool:
         """Returns True if this object processes a signal. False otherwise.
         """
         return self.__obj_desc["ir"]["signal"]
 
     @property
-    def __obj_desc(self):
+    def __obj_desc(self) -> Dict:
         """ Returns the original HeavyIR object description.
         """
         return HeavyIrObject.__HEAVY_OBJS_IR_DICT[self.type]
 
-    def inlet_requires_signal(self, inlet_index=0):
+    def inlet_requires_signal(self, inlet_index: int = 0) -> bool:
         """ Returns True if the indexed inlet requires a signal connection. False otherwise.
         """
         return self.__obj_desc["inlets"][inlet_index] in {"~i>", "~f>"}
 
-    def outlet_requires_signal(self, inlet_index=0):
+    def outlet_requires_signal(self, inlet_index: int = 0) -> bool:
         """ Returns True if the indexed outlet requires a signal connection. False otherwise.
         """
         return self.__obj_desc["outlets"][inlet_index] in {"~i>", "~f>"}
 
-    def reduce(self):
+    def reduce(self) -> Optional[tuple]:
         # A Heavy IR object is already reduced. Returns itself and no connection changes.
         return ({self}, [])
 
-    def get_parent_order(self):
+    def get_parent_order(self) -> List:
         """ Returns a list of all objects in process order, with this object at the end.
         """
         if self.__is_ordered:
             return []
         else:
             self.__is_ordered = True
             if self.is_root():
@@ -116,92 +131,94 @@
             else:
                 order_list = []
                 for c in [c for inlet in self.inlet_connections for c in inlet]:
                     order_list.extend(c.from_object.get_parent_order())
                 order_list.append(self)
                 return order_list
 
-    def assign_signal_buffers(self, buffer_pool):
-        # assign the inlet buffers
-        for cc in self.inlet_connections:
-            cc = [c for c in cc if c.is_signal]  # only need to deal with signal connections
-            if len(cc) == 0:
-                continue
-            if len(cc) == 1:
-                c = cc[0]  # get the connection
+    def assign_signal_buffers(self, buffer_pool: Optional[BufferPool]) -> None:
+        if buffer_pool is not None:
+            # assign the inlet buffers
+            for cc in self.inlet_connections:
+                cc = [c for c in cc if c.is_signal]  # only need to deal with signal connections
+                if len(cc) == 0:
+                    continue
+                if len(cc) == 1:
+                    c = cc[0]  # get the connection
 
-                # get the buffer at the outlet of the connected object
-                buf = c.from_object.outlet_buffers[c.outlet_index]
+                    # get the buffer at the outlet of the connected object
+                    buf = c.from_object.outlet_buffers[c.outlet_index]
 
-                # assign the buffer to the inlet of this object
-                self.inlet_buffers[c.inlet_index] = buf
+                    # assign the buffer to the inlet of this object
+                    self.inlet_buffers[c.inlet_index] = buf
 
-                # decrease the retain count of the buffer
-                buffer_pool.release_buffer(buf)
-            else:
-                raise HeavyException(f"This object has {len(cc)} (> 1) signal inputs.")
+                    # decrease the retain count of the buffer
+                    buffer_pool.release_buffer(buf)
+                else:
+                    raise HeavyException(f"This object has {len(cc)} (> 1) signal inputs.")
 
-        # assign the output buffers
-        exclude_set = set()
+            # assign the output buffers
+            exclude_set: set = set()
 
-        for i in range(self.num_outlets):
-            # buffers are assigned even if the outlet has no connections.
-            # The buffer will still be filled. However, if the buffer has already
-            # been set (i.e. non-zero) (e.g. in the case of dac~),
-            # then we skip this set
-
-            connection_type = self._resolved_outlet_type(outlet_index=i)
-            if Connection.is_signal_type(connection_type) and self.outlet_buffers[i][0] == "zero":
-                b = buffer_pool.get_buffer(
-                    connection_type,
-                    len(self.outlet_connections[i]),
-                    exclude_set)
-                self.outlet_buffers[i] = b
-
-                # if the buffer has no dependencies, make sure that it isn't reused
-                # right away. All outlets should have independent buffers.
-                if len(self.outlet_connections[i]) == 0:
-                    exclude_set.add(b)
+            for i in range(self.num_outlets):
+                # buffers are assigned even if the outlet has no connections.
+                # The buffer will still be filled. However, if the buffer has already
+                # been set (i.e. non-zero) (e.g. in the case of dac~),
+                # then we skip this set
+
+                connection_type = self._resolved_outlet_type(outlet_index=i)
+                if Connection.is_signal_type(connection_type) and self.outlet_buffers[i][0] == "zero" \
+                        and connection_type is not None:
+                    b = buffer_pool.get_buffer(
+                        connection_type,
+                        len(self.outlet_connections[i]),
+                        exclude_set)
+                    self.outlet_buffers[i] = b
+
+                    # if the buffer has no dependencies, make sure that it isn't reused
+                    # right away. All outlets should have independent buffers.
+                    if len(self.outlet_connections[i]) == 0:
+                        exclude_set.add(b)
 
-    def _resolved_outlet_type(self, outlet_index=0):
+    def _resolved_outlet_type(self, outlet_index: int = 0) -> Optional[str]:
         """ Returns the connection type at the given outlet.
             This information is always well-defined for IR objects.
         """
         return self.__obj_desc["outlets"][outlet_index]
 
     #
     # Intermediate Representation generators
     #
 
-    def get_object_dict(self):
+    def get_object_dict(self) -> Dict:
         """ Returns a dictionary of all constituent low-level objects,
             indexed by id, including their arguments and type.
         """
         return {
             self.id: {
                 "args": self.args,
                 "type": self.type
             }
         }
 
-    def get_ir_init_list(self):
+    def get_ir_init_list(self) -> List:
         """ Returns a list of all object id for obejcts that need initialisation.
         """
         return [self.id] if self.__obj_desc["ir"]["init"] else []
 
-    def get_ir_on_message(self, inlet_index=0):
+    def get_ir_on_message(self, inlet_index: int = 0) -> List:
         """ Returns an array of dictionaries containing the information for the
             corresponding on_message call.
         """
         return [{
             "id": self.id,
             "inletIndex": inlet_index
         }]
 
-    def get_ir_control_list(self):
+    def get_ir_control_list(self) -> List:
         """ Returns the intermediate representation for object control functions.
             Basically, does sendMessage() need to be written?
         """
         if self.__obj_desc["ir"]["control"]:
             on_message_list = []
             for connections in self.outlet_connections:
                 on_messages_let = []
@@ -212,15 +229,15 @@
             return [{
                 "id": self.id,
                 "onMessage": on_message_list
             }]
         else:
             return []
 
-    def get_ir_signal_list(self):
+    def get_ir_signal_list(self) -> List:
         """ Returns the intermediate representation for object process functions.
             Only outputs buffer information for lets that require a signal.
         """
         # we assume that this method will only be called on signal objects
         assert self.__obj_desc["ir"]["signal"]
 
         return [{
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HeavyLangObject.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HeavyLangObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,125 +14,140 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import decimal
 import json
 import os
 import random
-from struct import unpack, pack
 import string
 
-from hvcc.core.hv2ir.HeavyException import HeavyException
+from struct import unpack, pack
+from typing import Optional, Union, List, Dict, Any, TYPE_CHECKING
+
+from .Connection import Connection
+from .HeavyException import HeavyException
+
+if TYPE_CHECKING:
+    from .HeavyGraph import HeavyGraph
+    from .HeavyIrObject import HeavyIrObject
 
 
 class HeavyLangObject:
     """ This is the base Heavy object class.
     """
 
     __RANDOM = random.Random()
     __ID_CHARS = string.ascii_letters + string.digits
 
     # load the Heavy object definitions
     with open(os.path.join(os.path.dirname(__file__), "../json/heavy.lang.json"), "r") as f:
         _HEAVY_LANG_DICT = json.load(f)
 
-    def __init__(self, obj_type, args=None, graph=None, num_inlets=-1, num_outlets=-1, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional['HeavyGraph'] = None,
+        num_inlets: int = -1,
+        num_outlets: int = -1,
+        annotations: Optional[Dict] = None
+    ) -> None:
         # set the object type
         self.type = obj_type
 
         # generate a unique id for this object
-        self.id = "".join(HeavyLangObject.__RANDOM.choice(HeavyLangObject.__ID_CHARS) for _ in range(8))
+        self.id = "".join(self.__RANDOM.choice(self.__ID_CHARS) for _ in range(8))
 
         # assign the parent graph
         self.graph = graph
 
         # set local arguments
-        self.args = args or {}
+        self.args: Dict = args or {}
 
         # set local annotations
-        self.annotations = annotations or {}
+        self.annotations: Dict = annotations or {}
 
         # a list of locally generated warnings and errors (notifications)
-        self.warnings = []
-        self.errors = []
+        self.warnings: List = []
+        self.errors: List = []
 
         # resolve arguments and fill in missing defaults for HeavyLang objects
         self.__resolve_default_lang_args()
 
         # the list of connections at each inlet
         num_inlets = num_inlets if num_inlets >= 0 else len(self._obj_desc["inlets"])
-        self.inlet_connections = [[] for _ in range(num_inlets)]
+        self.inlet_connections: List = [[] for _ in range(num_inlets)]
 
         # the list of connections at each outlet
         num_outlets = num_outlets if num_outlets >= 0 else len(self._obj_desc["outlets"])
-        self.outlet_connections = [[] for _ in range(num_outlets)]
+        self.outlet_connections: List = [[] for _ in range(num_outlets)]
 
     @property
-    def scope(self):
+    def scope(self) -> str:
         """ Returns the scope of this object, private by default.
             Scope may be public, protected, private.
         """
         return self.annotations.get("scope", "private")
 
     @property
-    def static(self):
+    def static(self) -> bool:
         """ Returns true of this object is marked as static. False by default.
         """
         return self.annotations.get("static", False)
 
     @property
-    def const(self):
+    def const(self) -> bool:
         """ Returns true of this object is marked as constant. False by default.
         """
         return self.annotations.get("const", False)
 
     @property
-    def name(self):
+    def name(self) -> Optional[str]:
         """ Returns the name of this object. Returns None if there is no name.
         """
         return self.args.get("name", None)
 
     @property
-    def _obj_desc(self):
+    def _obj_desc(self) -> Dict:
         """ Returns the HeavyLang object description.
         """
-        return HeavyLangObject._HEAVY_LANG_DICT[self.type]
+        return self._HEAVY_LANG_DICT[self.type]
 
-    def inlet_connection_type(self, index):
+    def inlet_connection_type(self, index: int) -> Dict:
         return self._obj_desc["inlets"][index]
 
-    def outlet_connection_type(self, index):
+    def outlet_connection_type(self, index: int) -> Dict:
         return self._obj_desc["outlets"][index]
 
-    def name_for_arg(self, index=0):
+    def name_for_arg(self, index: int = 0) -> str:
         """ Returns the name of the argument at the given index.
         """
         return self._obj_desc["args"][index]["name"]
 
-    def add_warning(self, warning):
+    def add_warning(self, warning: str) -> None:
         """ Add a warning to this object.
         """
         self.warnings.append({"message": warning})
 
-    def add_error(self, error):
+    def add_error(self, error: str) -> None:
         """ Add an error to this object and raise an exception.
         """
         self.errors.append({"message": error})
         raise HeavyException(error)
 
-    def get_notices(self):
+    def get_notices(self) -> Dict:
         """ Returns a dictionary of all warnings and errors at this object.
         """
         return {
             "warnings": [{"message": f"{self}: {n['message']}"} for n in self.warnings],
             "errors": [{"message": f"{self}: {n['message']}"} for n in self.errors],
         }
 
     @classmethod
-    def force_arg_type(clazz, value, value_type, graph=None):
+    def force_arg_type(cls, value: Any, value_type: str, graph: Optional['HeavyGraph'] = None) -> Any:
         """ Attempts to convert a value to a given value type. Raises an Exception otherwise.
             If the value_type is unknown and a graph is provided, a warning will be registered.
         """
         if value_type == "float":
             try:
                 return float(value)
             except Exception:
@@ -171,15 +187,15 @@
             # not necessarily an error. It may simply be that the value should
             # not be resolved to anything other than what it already is.
             # This happens most often with message objects.
             # if graph is not None:
             #     graph.add_warning(f"Unknown value type \"{value_type}\" for value: {value}")
             return value
 
-    def __resolve_default_lang_args(self):
+    def __resolve_default_lang_args(self) -> None:
         """ Resolves missing default arguments. Also checks to make sure that all
             required arguments are present. Does nothing if the object is IR.
         """
         if self.type in HeavyLangObject._HEAVY_LANG_DICT:
             for arg in self._obj_desc["args"]:
                 if arg["name"] not in self.args:
                     # if a defined argument is not in the argument dictionary
@@ -192,45 +208,45 @@
                     # enforce argument types
                     self.args[arg["name"]] = HeavyLangObject.force_arg_type(
                         self.args[arg["name"]],
                         arg["value_type"],
                         self.graph)
 
     @property
-    def num_inlets(self):
+    def num_inlets(self) -> int:
         return len(self.inlet_connections)
 
     @property
-    def num_outlets(self):
+    def num_outlets(self) -> int:
         return len(self.outlet_connections)
 
-    def add_connection(self, c):
+    def add_connection(self, c: Connection) -> None:
         """ Add a connection to this object.
         """
         try:
             if c.to_object is self:
                 self.inlet_connections[c.inlet_index].append(c)
             elif c.from_object is self:
                 self.outlet_connections[c.outlet_index].append(c)
             else:
                 raise HeavyException(f"Connection {c} does not connect to this object {self}.")
         except Exception:
             raise HeavyException(f"Connection {c} connects to out-of-range let.")
 
-    def remove_connection(self, c):
+    def remove_connection(self, c: Connection) -> None:
         """ Remove a connection to this object.
         """
         if c.to_object is self:
             self.inlet_connections[c.inlet_index].remove(c)
         elif c.from_object is self:
             self.outlet_connections[c.outlet_index].remove(c)
         else:
             raise HeavyException(f"Connection {c} does not connect to this object {self}.")
 
-    def replace_connection(self, c, n_list):
+    def replace_connection(self, c: Connection, n_list: list) -> None:
         """ Replaces connection c with connection list n_list, maintaining connection order
         """
         if c.from_object is self:
             cc = self.outlet_connections[c.outlet_index]
             # NOTE(mhroth): this will throw an exception if c does not exist
             # if a heavy object connects to itself, such as through a [t a]
             # or directly, there may be an error here,
@@ -239,26 +255,26 @@
         elif c.to_object is self:
             # connection order doesn't matter at the inlet
             self.inlet_connections[c.inlet_index].remove(c)
             self.inlet_connections[c.inlet_index].extend(n_list)
         else:
             raise HeavyException(f"Connections must have a common endpoint: {c} / {n_list}")
 
-    def get_connection_move_list(self, o, connection_type_filter="-~>"):
+    def get_connection_move_list(self, o: 'HeavyIrObject', connection_type_filter: str = "-~>") -> List:
         """ Create a list of commands to move all connections from this object
             to the given object o.
         """
         m = []
         for c in [c for cc in self.inlet_connections for c in cc]:
             m.append((c, [c.copy(to_object=o)]))
         for c in [c for cc in self.outlet_connections for c in cc]:
             m.append((c, [c.copy(from_object=o)]))
         return m
 
-    def _get_connection_format(self, connections_list):
+    def _get_connection_format(self, connections_list: List) -> str:
         fmt = []
         for cc in connections_list:
             s = {c.type for c in cc}
             if len(s) == 0:
                 fmt.append("_")
             elif len(s) == 1:
                 if "-->" in s:
@@ -271,44 +287,44 @@
                     raise Exception(f"Unknown connection type in set {cc} in file {cc[0].from_object.graph.file}.")
             elif s in [{"~f>", "-->"}, {"~i>", "-->"}]:
                 fmt.append("m")
             else:
                 fmt.append("m")
         return "".join(fmt)
 
-    def has_inlet_connection_format(self, fmts=None):
+    def has_inlet_connection_format(self, fmts: Optional[Union[str, List]] = None) -> bool:
         """ Returns true if the object has given format at its inlets.
         """
         fmts = fmts if isinstance(fmts, list) else [fmts]
         return self._get_connection_format(self.inlet_connections) in fmts
 
-    def has_outlet_connection_format(self, fmts=None):
+    def has_outlet_connection_format(self, fmts: Optional[Union[str, List]] = None) -> bool:
         """ Returns true if the object has given format at its outlets.
             Take either litteral or list as input.
         """
         fmts = fmts if isinstance(fmts, list) else [fmts]
         return self._get_connection_format(self.outlet_connections) in fmts
 
-    def is_leaf(self):
+    def is_leaf(self) -> bool:
         """ Returns True if this object is a leaf in the graph. False otherwise.
         """
         return all(len(c) == 0 for c in self.outlet_connections)
 
-    def is_root(self):
+    def is_root(self) -> bool:
         """ Returns True if this object is a root in the graph. False otherwise.
         """
         return all(len(c) == 0 for c in self.inlet_connections)
 
-    def _resolved_outlet_type(self, outlet_index=0):
+    def _resolved_outlet_type(self, outlet_index: int = 0) -> Optional[str]:
         """ Returns the connection type expected at the given outlet.
             The result may be influenced by the state of the input connections.
         """
         # get the defined connection type
         connection_type = self._obj_desc["outlets"][outlet_index]["connectionType"]
-        if connection_type == "-~>":
+        if connection_type == "-~>" and self.graph is not None:
             # if the connection type is defined as mixed,
             # use the default approach to resolve it
             connection_type_set = {c.type for c in self.inlet_connections[0]}
             if len(connection_type_set) == 0:
                 return "-->"
             elif len(connection_type_set) == 1:
                 return list(connection_type_set)[0]
@@ -319,38 +335,42 @@
                     return "~i>"
             # if the connection type cannot be resolved to a well-defined type
             self.graph.add_error("Connection type cannot be resolved."
                                  f"Unknown inlet connection type configuration: {connection_type_set}")
         else:
             return connection_type
 
-    def _resolve_connection_types(self, obj_stack):
+        return None
+
+    def _resolve_connection_types(self, obj_stack: Optional[set] = None) -> Optional[None]:
         """ Resolves the type of all connections before reduction to IR object types.
             If connections incident on an object are incompatible, they are either
             resolved, potentially by inserting conversion objects, or pruned.
             If a viable resolution cannot be found, an exception may be raised.
         """
+        obj_stack = obj_stack or set()
         if self in obj_stack:
             return
         else:
             obj_stack.add(self)
 
         # for all outgoing connections
-        for c in [c for cc in self.outlet_connections for c in cc]:
-            if c.is_mixed:
-                connection_type = self._resolved_outlet_type(outlet_index=c.outlet_index)
-                if connection_type == "-~>":
-                    self.graph.add_error("Cannot resolve connection type from -~>.")
-                else:
-                    self.graph.update_connection(c, [c.copy(type=connection_type)])
+        if self.graph is not None:
+            for c in [c for cc in self.outlet_connections for c in cc]:
+                if c.is_mixed:
+                    connection_type = self._resolved_outlet_type(outlet_index=c.outlet_index)
+                    if connection_type == "-~>":
+                        self.graph.add_error("Cannot resolve connection type from -~>.")
+                    else:
+                        self.graph.update_connection(c, [c.copy(type=connection_type)])
 
-            c.to_object._resolve_connection_types(obj_stack)  # turtle all the way down
+                c.to_object._resolve_connection_types(obj_stack)  # turtle all the way down
 
     @classmethod
-    def get_hash(clazz, x):
+    def get_hash(cls, x: str) -> int:
         """ Compute the message element hash used by msg_getHash(). Returns a 32-bit integer.
         """
         if isinstance(x, float) or isinstance(x, int):
             # interpret the float bytes as an unsigned integer
             return unpack("@I", pack("@f", float(x)))[0]
         elif x == "bang":
             return 0xFFFFFFFF
@@ -385,10 +405,10 @@
             h ^= h >> 13
             h = (h * m) & 0xFFFFFFFF
             h ^= h >> 15
             return h
         else:
             raise Exception("Message element hashes can only be computed for float and string types.")
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         arg_str = " ".join([f"{k}:{o}" for (k, o) in self.args.items()])
         return f"{self.type} {{{arg_str}}}" if len(arg_str) > 0 else self.type
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/HeavyParser.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HeavyParser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,14 +14,16 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import random
 import os
 
+from typing import Any, Dict, Optional
+
 from .HIrConvolution import HIrConvolution
 from .HIrInlet import HIrInlet
 from .HIrLorenz import HIrLorenz
 from .HIrOutlet import HIrOutlet
 from .HIrPack import HIrPack
 from .HIrSwitchcase import HIrSwitchcase
 from .HIrTabhead import HIrTabhead
@@ -55,15 +58,22 @@
 from .HeavyGraph import HeavyGraph
 from .Connection import Connection
 
 
 class HeavyParser:
 
     @classmethod
-    def graph_from_file(clazz, hv_file, graph=None, graph_args=None, path_stack=None, xname=None):
+    def graph_from_file(
+        cls,
+        hv_file: str,
+        graph: Optional[HeavyGraph] = None,
+        graph_args: Optional[Dict] = None,
+        path_stack: Optional[set] = None,
+        xname: Optional[str] = None
+    ) -> HeavyGraph:
         """ Read a graph object from a file.
 
             @param graph  The parent graph of this graph.
             @param graph_args  The arguments to this graph, in the form of a completely
             resolved dictionary.
             @param path_stack  The path_stack is the current stack of resolved abstractions.
             It prevents infinite recursion when reading many abstractions deep.
@@ -78,18 +88,27 @@
         else:
             path_stack.add(hv_file)
 
         # open and parse the heavy file
         with open(hv_file, "r") as f:
             json_heavy = json.load(f)
 
-        return HeavyParser.graph_from_object(json_heavy, graph, graph_args, hv_file, path_stack, xname)
+        return cls.graph_from_object(hv_file, json_heavy, path_stack, graph, graph_args, xname)
 
     @classmethod
-    def graph_from_object(clazz, json_heavy, graph=None, graph_args=None, hv_file=None, path_stack=None, xname=None):
+    def graph_from_object(
+        cls,
+        hv_file: str,
+        json_heavy: Dict,
+        path_stack: set,
+        graph: Optional[HeavyGraph] = None,
+        graph_args: Optional[Dict] = None,
+        xname: Optional[str] = None
+    ) -> HeavyGraph:
+
         """ Parse a graph object.
 
             @param graph  The parent graph.
             @param graph_args  The resolved arguments to this graph, in the form of a dictionary.
             @param hv_file  The Heavy file where this graph can be found.
         """
         # resolve default graph arguments
@@ -121,37 +140,37 @@
             for obj_id, o in json_heavy["objects"].items():
                 if o["type"] == "comment":
                     continue  # first and foremost, ignore comment objects
 
                 elif o["type"] == "graph":
                     # inline HeavyGraph objects (i.e. subgraphs)
                     # require a different set of initialisation arguments
-                    x = HeavyParser.graph_from_object(o, g, g.args, hv_file, path_stack, xname)
+                    x: Any = cls.graph_from_object(hv_file, o, path_stack, g, g.args, xname)
 
                 else:
                     # resolve the arguments dictionary based on the graph args
                     args = g.resolve_arguments(o["args"])
 
                     # before anything, search for an abstraction
                     # in case we want to override default functionality
                     # However, if we are in an abstraction that has the same
                     # name as the type that we are looking for, don't recurse!
                     abs_path = g.find_path_for_abstraction(o["type"])
                     if abs_path is not None and abs_path not in path_stack:
-                        x = HeavyParser.graph_from_file(
+                        x = cls.graph_from_file(
                             hv_file=abs_path,
                             graph=g,
                             graph_args=args,
                             path_stack=path_stack)
 
                     # if we know how to handle this object type natively
                     # either as a custom type or as a generic IR object
                     elif HeavyParser.get_class_for_type(o["type"]) is not None:
-                        obj_clazz = HeavyParser.get_class_for_type(o["type"])
-                        x = obj_clazz(o["type"], args, g, o.get("annotations", {}))
+                        obj_cls = HeavyParser.get_class_for_type(o["type"])
+                        x = obj_cls(o["type"], args, g, o.get("annotations", {}))
 
                     # handle generic IR objects
                     elif HeavyIrObject.is_ir(o["type"]):
                         x = HeavyIrObject(o["type"], args, g, annotations=o.get("annotations", {}))
 
                     # an object definition can't be found
                     else:
@@ -183,15 +202,15 @@
             # remove this graph from the stack when finished.
             # Subpatches should not remove themselves.
             path_stack.remove(g.file)
 
         return g
 
     @classmethod
-    def get_class_for_type(clazz, obj_type):
+    def get_class_for_type(cls, obj_type: str) -> Any:
         """ Returns the class which can handle the given object type.
         """
         if HLangUnop.handles_type(obj_type):
             return HLangUnop
         elif HLangBinop.handles_type(obj_type):
             return HLangBinop
         elif obj_type in LANG_CLASS_DICT:
@@ -200,21 +219,25 @@
             return None
 
 
 class HLangIf(HeavyLangObject):
     """ Translates HeavyLang object [if] to HeavyIR [if] or [if~].
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
-        HeavyLangObject.__init__(self, "if", args, graph,
-                                 num_inlets=2,
-                                 num_outlets=2,
-                                 annotations=annotations)
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: HeavyGraph,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "if"
+        super().__init__("if", args, graph, num_inlets=2, num_outlets=2, annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         if self.has_inlet_connection_format(["cc", "_c", "c_", "__"]):
             x = HeavyIrObject("__if", self.args)
         elif self.has_inlet_connection_format("ff"):
             # TODO(mhroth): implement this
             x = HeavyParser.graph_from_file("./hvlib/if~f.hv.json")
         elif self.has_inlet_connection_format("ii"):
             # TODO(mhroth): implement this
@@ -226,22 +249,25 @@
         return ({x}, self.get_connection_move_list(x))
 
 
 class HLangNoise(HeavyLangObject):
     """ Handles the HeavyLang "noise" object.
     """
 
-    def __init__(self, obj_type, args, graph, annotations=None):
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: HeavyGraph,
+        annotations: Optional[Dict] = None
+    ) -> None:
         assert obj_type == "noise"
-        HeavyLangObject.__init__(self, "noise", args, graph,
-                                 num_inlets=1,
-                                 num_outlets=1,
-                                 annotations=annotations)
+        super().__init__("noise", args, graph, num_inlets=1, num_outlets=1, annotations=annotations)
 
-    def reduce(self):
+    def reduce(self) -> tuple:
         seed = int(random.uniform(1, 2147483647))  # assign a random 32-bit seed
         noise_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "./hvlib/noise.hv.json")
         x = HeavyParser.graph_from_file(noise_path, graph_args={"seed": seed})
         x.reduce()
         # TODO(mhroth): deal with control input
         return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/LocalVars.py` & `hvcc-0.7.0/hvcc/core/hv2ir/LocalVars.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from collections import defaultdict
 import os
+from collections import defaultdict
+from typing import Optional, Union, Dict, List
 
 from .HeavyException import HeavyException
+from .HeavyLangObject import HeavyLangObject
 
 
 class LocalVars:
     """ A set of scoped objects.
     """
 
-    def __init__(self, stdlib_dir="./"):
+    def __init__(self, stdlib_dir: str = "./") -> None:
         # a dictionary of name-registered objects
         # the data structure is a list map
         # key is the name under which the object is registered, value is a
         # list of all objects who are registered with that name
-        self.__REGISTERED_OBJ_DICT = defaultdict(list)
+        self.__REGISTERED_OBJ_DICT: Dict = defaultdict(list)
 
         # the list of globally declared paths
         self.declared_paths = [stdlib_dir]  # initialise with the standard library directory
 
-    def find_path_for_abstraction(self, name):
+    def find_path_for_abstraction(self, name: str) -> Optional[str]:
         # the file name based on the abstraction name
         file_name = f"{name}.hv.json"
 
         # iterate in order through the declared paths in order to find the file
         for d in self.declared_paths:
             file_path = os.path.join(d, file_name)
             if os.path.exists(file_path):
                 return file_path  # if a matching abstraction is found, return the path
         return None  # otherwise return None
 
-    def add_import_paths(self, path_list):
+    def add_import_paths(self, path_list: List) -> None:
         """ Add import paths. Paths are expanded and made as explicit as possible.
         """
         self.declared_paths.extend([os.path.abspath(os.path.expanduser(p)) for p in path_list])
 
-    def register_object(self, obj, name, static=False, unique=False):
+    def register_object(self, obj: HeavyLangObject, name: str, static: bool = False, unique: bool = False) -> None:
         """ Registers a named object.
         """
 
         objs = self.get_objects_for_name(name, obj.type)
         if (unique and len(objs) > 0) or (static and len(objs) > 1):
             # if there is already a registered object of this type and the new
             # object is not declared as static, throw an error
             raise HeavyException(f"Object {obj} with name \"{name}\" already exists, "
                                  "and the new object is static or unique.")
         elif len(objs) == 1 and static:
             pass  # the static object has already been registered, move on
         else:
             self.__REGISTERED_OBJ_DICT[name].append(obj)
 
-    def unregister_object(self, obj, name):
+    def unregister_object(self, obj: HeavyLangObject, name: str) -> None:
         """ Unregisters a named object.
         """
 
         self.__REGISTERED_OBJ_DICT[name].remove(obj)
 
-    def get_objects_for_name(self, name, obj_types):
+    def get_objects_for_name(self, name: str, obj_types: Union[str, List]) -> List:
         """ Returns a list of objects registered under a name in this scope.
         """
 
         obj_types = obj_types if isinstance(obj_types, list) else [obj_types]
         return [o for o in self.__REGISTERED_OBJ_DICT[name] if o.type in obj_types]
 
-    def get_registered_objects_for_type(self, obj_type):
+    def get_registered_objects_for_type(self, obj_type: str) -> Dict:
         """ Returns a list-dictionary for all objects of the given type, indexed by name.
         """
 
         d = defaultdict(list)
         for k, v in self.__REGISTERED_OBJ_DICT.items():
             x = [o for o in v if o.type == obj_type]
             if len(x) > 0:  # only return names that actually have associated objects
```

### Comparing `hvcc-0.6.3/hvcc/core/hv2ir/hv2ir.py` & `hvcc-0.7.0/hvcc/core/hv2ir/hv2ir.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -14,22 +15,30 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import json
 import os
 import time
 
-from hvcc.core.hv2ir.HeavyException import HeavyException
-from hvcc.core.hv2ir.HeavyParser import HeavyParser
+from typing import Optional, Dict
+
+from .HeavyException import HeavyException
+from .HeavyParser import HeavyParser
 
 
 class hv2ir:
 
     @classmethod
-    def compile(clazz, hv_file, ir_file, patch_name=None, verbose=False):
+    def compile(
+        cls,
+        hv_file: str,
+        ir_file: str,
+        patch_name: Optional[str] = None,
+        verbose: bool = False
+    ) -> Dict:
         """ Compiles a HeavyLang file into a HeavyIR file.
             Returns a tuple of compile time in seconds, a notification dictionary,
             and a heavy object counter.
         """
 
         # keep track of the total compile time
         tick = time.time()
@@ -95,15 +104,15 @@
                     f,
                     sort_keys=True,
                     indent=2,
                     separators=(",", ": "))
             else:
                 json.dump(ir, f)
 
-        if verbose:
+        if verbose and ir is not None:
             if len(ir["signal"]["processOrder"]) > 0:
                 print("")
                 print("=== Signal Order ===")
                 for so in ir["signal"]["processOrder"]:
                     o = ir["objects"][so["id"]]
                     if len(o["args"]) > 0:
                         print("{0} {{{1}}}".format(
@@ -121,15 +130,15 @@
             "in_dir": os.path.dirname(hv_file),
             "out_file": os.path.basename(ir_file),
             "out_dir": os.path.dirname(ir_file),
             "ir": ir
         }
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         description="A C-language compiler for the Heavy audio programming language.")
     parser.add_argument(
         "hv_path",
         help="The patch to the top-level patch to compile.")
     parser.add_argument(
         "--hv_ir_path",
```

### Comparing `hvcc-0.6.3/hvcc/core/json/heavy.ir.json` & `hvcc-0.7.0/hvcc/core/json/heavy.ir.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939024390243902%*

 * *Differences: {"'__eq~f'": "OrderedDict([('inlets', ['~f>', '~f>']), ('ir', OrderedDict([('control', False), "*

 * *             "('signal', True), ('init', False)])), ('outlets', ['~f>']), ('args', []), ('perf', "*

 * *             "OrderedDict([('avx', 3), ('sse', 3)]))])"}*

```diff
@@ -972,14 +972,33 @@
             "init": true,
             "signal": false
         },
         "outlets": [
             "-->"
         ]
     },
+    "__eq~f": {
+        "args": [],
+        "inlets": [
+            "~f>",
+            "~f>"
+        ],
+        "ir": {
+            "control": false,
+            "init": false,
+            "signal": true
+        },
+        "outlets": [
+            "~f>"
+        ],
+        "perf": {
+            "avx": 3,
+            "sse": 3
+        }
+    },
     "__exp": {
         "args": [],
         "inlets": [
             "-->"
         ],
         "ir": {
             "control": true,
```

### Comparing `hvcc-0.6.3/hvcc/core/json/heavy.lang.json` & `hvcc-0.7.0/hvcc/core/json/heavy.lang.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/buildjson/buildjson.py` & `hvcc-0.7.0/hvcc/generators/buildjson/buildjson.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,35 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from collections import defaultdict
 import json
 import os
+from typing import Dict, List, Optional
 
 # generate build configuration files for use with https://github.com/enzienaudio/courtesan
 # Example arguments:
 #   macos_x64_args=["-project", "Hv_test_WwiseSourcePlugin.xcodeproj", "-arch", "x86_64", "-alltargets"]
 #   android_armv7a_args=["APP_ABI=armeabi-v7a", "-j"]
 #   win_x64_args=["/property:Configuration=Release", "/property:Platform=x64",
 #                 "/t:Rebuild", "Hv_{0}_Unity.sln".format(patch_name), "/m"]
 
 
-def generate_json(out_dir, android_armv7a_args=None, ios_armv7a_args=None,
-                  linux_armv7a_args=None, linux_x64_args=None, macos_x64_args=None,
-                  win_x64_args=None, win_x86_args=None):
-    build_json = defaultdict(dict)
+def generate_json(
+    out_dir: str,
+    android_armv7a_args: Optional[List] = None,
+    ios_armv7a_args: Optional[List] = None,
+    linux_armv7a_args: Optional[List] = None,
+    linux_x64_args: Optional[List] = None,
+    macos_x64_args: Optional[List] = None,
+    win_x64_args: Optional[List] = None,
+    win_x86_args: Optional[List] = None
+) -> None:
+    build_json: Dict = defaultdict(dict)
 
     if android_armv7a_args:
         build_json["android"]["armv7a"] = {
             "args": [android_armv7a_args],
             "projectDir": ["android", "jni"],
             "binaryDir": ["android", "libs", "armeabi-v7a"]
         }
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2daisy/c2daisy.py` & `hvcc-0.7.0/hvcc/generators/c2daisy/c2daisy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-# import datetime
 import jinja2
 import os
 import shutil
 import time
+import json2daisy  # type: ignore
+
+from typing import Dict, Optional
+
 from ..buildjson import buildjson
 from ..copyright import copyright_manager
-import json2daisy
 from . import parameters
 
 
 class c2daisy:
     """ Generates a Daisy wrapper for a given patch.
     """
 
     @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         out_dir = os.path.join(out_dir, "daisy")
 
         if patch_meta:
             patch_name = patch_meta.get("name", patch_name)
-            daisy_meta = patch_meta.get("daisy")
+            daisy_meta = patch_meta.get("daisy", {})
         else:
             daisy_meta = {}
 
-        board = daisy_meta.get("board", "seed")
+        board = daisy_meta.get("board", "pod")
 
         copyright_c = copyright_manager.get_copyright_for_c(copyright)
         # copyright_plist = copyright or u"Copyright {0} Enzien Audio, Ltd." \
         #     " All Rights Reserved.".format(datetime.datetime.now().year)
 
         try:
             # ensure that the output directory does not exist
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2daisy/parameters.py` & `hvcc-0.7.0/hvcc/generators/c2daisy/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 
 from copy import deepcopy
+from typing import Any, Dict, Optional
 
 
-def filter_match(set, key, match, key_exclude=None, match_exclude=None):
+def filter_match(
+    set: Dict,
+    key: str,
+    match: str,
+    key_exclude: Optional[str] = None,
+    match_exclude: Optional[str] = None
+) -> filter:
     if (key_exclude is not None and match_exclude is not None):
         return filter(lambda x: x.get(key, '') == match and x.get(key_exclude, '') != match_exclude, set)
     else:
         return filter(lambda x: x.get(key, '') == match, set)
 
 
-def verify_param_exists(name, original_name, components, input=True):
+def verify_param_exists(name: str, original_name: str, components: Dict, input: bool = True) -> Any:
     for comp in components:
 
         # Dealing with the cvouts the way we have it set up is really annoying
         if comp['component'] == 'CVOuts':
 
             if name == comp['name']:
                 if input:
@@ -28,63 +35,80 @@
                     raise TypeError(
                         f'Parameter "{original_name}" cannot be used as an {"input" if input else "output"}')
                 return
 
     raise NameError(f'Unknown parameter "{original_name}"')
 
 
-def verify_param_direction(name, components):
+def verify_param_direction(name: str, components: Dict) -> bool:
     for comp in components:
         if comp['component'] == 'CVOuts':
             if name == comp['name']:
                 return True
         else:
             variants = [mapping['name'].format_map(
                 {'name': comp['name']}) for mapping in comp['mapping']]
             if name in variants:
                 return True
+    return False
 
 
-def get_root_component(variant, original_name, components):
+def get_root_component(variant: str, original_name: str, components: Dict) -> str:
     for comp in components:
         if comp['component'] == 'CVOuts':
             if variant == comp['name']:
                 return variant
         else:
             variants = [mapping['name'].format_map(
                 {'name': comp['name']}) for mapping in comp['mapping']]
             if variant in variants:
                 return comp['name']
     raise NameError(f'Unknown parameter "{original_name}"')
 
 
-def get_component_mapping(component_variant, original_name, component, components):
+def get_component_mapping(
+    component_variant: str,
+    original_name: str,
+    component: Dict,
+    components: Dict
+) -> Dict:
     for variant in component['mapping']:
         if component['component'] == 'CVOuts':
             stripped = variant['name'].format_map({'name': ''})
             if stripped in component['name']:
                 return variant
         elif variant['name'].format_map({'name': component['name']}) == component_variant:
             return variant
     raise NameError(f'Unknown parameter "{original_name}"')
 
 
-def verify_param_used(component, params_in, params_out, params_in_original_name, params_out_original_name, components):
+def verify_param_used(
+    component: Dict,
+    params_in: Dict,
+    params_out: Dict,
+    params_in_original_name: Dict,
+    params_out_original_name: Dict,
+    components: Dict
+) -> bool:
     # Exclude parents, since they don't have 1-1 i/o mapping
     if component.get('is_parent', False):
         return True
     for param in {**params_in, **params_out}:
         root = get_root_component(
             param, ({**params_in_original_name, **params_out_original_name})[param], components)
         if root == component['name']:
             return True
     return False
 
 
-def de_alias(name, aliases, components):
+def de_alias(
+    name: str,
+    aliases: Dict,
+    components: Dict
+) -> str:
     low = name.lower()
     # simple case
     if low in aliases:
         return aliases[low]
     # aliased variant
     potential_aliases = list(filter(lambda x: x in low, aliases))
     for alias in potential_aliases:
@@ -99,26 +123,31 @@
         except IndexError:
             # No matching alias from filter
             pass
     # otherwise, it's a direct parameter or unkown one
     return low
 
 
-def parse_parameters(parameters, components, aliases, object_name):
+def parse_parameters(
+    parameters: Dict,
+    components: Dict,
+    aliases: Dict,
+    object_name: str
+) -> Dict:
     """
     Parses the `parameters` passed from hvcc and generates getters and setters
     according to the info in `components`. The `aliases` help disambiguate parameters
     and the `object_name` sets the identifier for the generated Daisy hardware class,
     in this case `hardware`.
     """
 
     # Verify that the params are valid and remove unused components
-    replacements = {}
-    params_in = {}
-    params_in_original_names = {}
+    replacements: Dict = {}
+    params_in: Dict = {}
+    params_in_original_names: Dict = {}
     for key, item in parameters['in']:
         de_aliased = de_alias(key, aliases, components)
         params_in[de_aliased] = item
         params_in_original_names[de_aliased] = key
 
     params_out = {}
     params_out_original_names = {}
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2daisy/static/README.md` & `hvcc-0.7.0/hvcc/generators/c2daisy/static/README.md`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp` & `hvcc-0.7.0/hvcc/generators/c2daisy/templates/HeavyDaisy.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2dpf/c2dpf.py` & `hvcc-0.7.0/hvcc/generators/c2dpf/c2dpf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,85 @@
-# import datetime
-import hashlib
+# Copyright (C) 2021-2023 Wasted Audio
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import os
 import shutil
 import time
 import jinja2
+from typing import Dict, Optional
+
 from ..buildjson import buildjson
 from ..copyright import copyright_manager
+from ..filters import filter_uniqueid
 
 
 class c2dpf:
     """ Generates a DPF wrapper for a given patch.
     """
 
     @classmethod
-    def filter_uniqueid(clazz, s):
-        """ Return a unique id (in hexadecimal) for the Plugin interface.
-        """
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:8]
-        s = f"0x{s}"
-        return s
-
-    @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         out_dir = os.path.join(out_dir, "plugin")
         receiver_list = externs['parameters']['in']
 
         if patch_meta:
             patch_name = patch_meta.get("name", patch_name)
             dpf_meta = patch_meta.get("dpf", {})
         else:
             dpf_meta = {}
 
-        dpf_project = dpf_meta.get('project')
         dpf_path = dpf_meta.get('dpf_path', '')
 
         copyright_c = copyright_manager.get_copyright_for_c(copyright)
         # copyright_plist = copyright or u"Copyright {0} Enzien Audio, Ltd." \
         #     " All Rights Reserved.".format(datetime.datetime.now().year)
 
         try:
             # ensure that the output directory does not exist
             out_dir = os.path.abspath(out_dir)
             if os.path.exists(out_dir):
                 shutil.rmtree(out_dir)
 
             # copy over static files
             shutil.copytree(os.path.join(os.path.dirname(__file__), "static"), out_dir)
-
-            if dpf_project:
-                shutil.copy(os.path.join(os.path.dirname(__file__), "static/README.md"), f'{out_dir}/../')
+            shutil.copy(os.path.join(os.path.dirname(__file__), "static/README.md"), f'{out_dir}/../')
 
             # copy over generated C source files
             source_dir = os.path.join(out_dir, "source")
             shutil.copytree(c_src_dir, source_dir)
 
             # initialize the jinja template environment
             env = jinja2.Environment()
-            env.filters["uniqueid"] = c2dpf.filter_uniqueid
+            env.filters["uniqueid"] = filter_uniqueid
 
             env.loader = jinja2.FileSystemLoader(
                 os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates"))
 
             # generate DPF wrapper from template
             dpf_h_path = os.path.join(source_dir, f"HeavyDPF_{patch_name}.hpp")
             with open(dpf_h_path, "w") as f:
@@ -84,14 +98,25 @@
                     meta=dpf_meta,
                     class_name=f"HeavyDPF_{patch_name}",
                     num_input_channels=num_input_channels,
                     num_output_channels=num_output_channels,
                     receivers=receiver_list,
                     pool_sizes_kb=externs["memoryPoolSizesKb"],
                     copyright=copyright_c))
+            if dpf_meta.get("enable_ui"):
+                dpf_ui_path = os.path.join(source_dir, f"HeavyDPF_{patch_name}_UI.cpp")
+                with open(dpf_ui_path, "w") as f:
+                    f.write(env.get_template("HeavyDPF_UI.cpp").render(
+                        name=patch_name,
+                        meta=dpf_meta,
+                        class_name=f"HeavyDPF_{patch_name}",
+                        num_input_channels=num_input_channels,
+                        num_output_channels=num_output_channels,
+                        receivers=receiver_list,
+                        copyright=copyright_c))
             dpf_h_path = os.path.join(source_dir, "DistrhoPluginInfo.h")
             with open(dpf_h_path, "w") as f:
                 f.write(env.get_template("DistrhoPluginInfo.h").render(
                     name=patch_name,
                     meta=dpf_meta,
                     class_name=f"HeavyDPF_{patch_name}",
                     num_input_channels=num_input_channels,
@@ -104,26 +129,25 @@
             # files = os.listdir(source_dir)
 
             # ======================================================================================
             # Linux
 
             # plugin makefile
             with open(os.path.join(source_dir, "Makefile"), "w") as f:
-                f.write(env.get_template("Makefile").render(
+                f.write(env.get_template("Makefile_plugin").render(
                     name=patch_name,
                     meta=dpf_meta,
                     dpf_path=dpf_path))
 
             # project makefile
-            if dpf_project:
-                with open(os.path.join(source_dir, "../../Makefile"), "w") as f:
-                    f.write(env.get_template("Makefile.project").render(
-                        name=patch_name,
-                        meta=dpf_meta,
-                        dpf_path=dpf_path))
+            with open(os.path.join(source_dir, "../../Makefile"), "w") as f:
+                f.write(env.get_template("Makefile_project").render(
+                    name=patch_name,
+                    meta=dpf_meta,
+                    dpf_path=dpf_path))
 
             buildjson.generate_json(
                 out_dir,
                 linux_x64_args=["-j"])
             # macos_x64_args=["-project", "{0}.xcodeproj".format(patch_name), "-arch",
             #                 "x86_64", "-alltargets"],
             # win_x64_args=["/property:Configuration=Release", "/property:Platform=x64",
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2dpf/templates/HeavyDPF.hpp` & `hvcc-0.7.0/hvcc/generators/c2dpf/templates/HeavyDPF.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,31 @@
   enum Parameters
   {
     {% for k, v in receivers -%}
       param{{v.display}},
     {% endfor %}
   };
 
+{% if meta.port_groups is defined %}
+  enum PortGroups
+  {
+{%- if meta.port_groups.input|length %}
+  {%- for group, value in meta.port_groups.input.items() %}
+    kPortGroup{{group}},
+  {%- endfor %}
+{%- endif %}
+{%- if meta.port_groups.output|length %}
+  {%- for group, value in meta.port_groups.output.items() %}
+    kPortGroup{{group}},
+  {%- endfor %}
+{%- endif %}
+    kPortGroupCount
+  };
+{%- endif %}
+
   {{class_name}}();
   ~{{class_name}}() override;
 
   void handleMidiInput(uint32_t frames, const MidiEvent* midiEvents, uint32_t midiEventCount);
   void handleMidiSend(uint32_t sendHash, const HvMessage *m);
 
 protected:
@@ -83,14 +100,18 @@
     return int64_t( {{class_name|uniqueid}} );
   }
 
   // -------------------------------------------------------------------
   // Init
 
   void initParameter(uint32_t index, Parameter& parameter) override;
+  {% if meta.port_groups is defined %}
+  void initAudioPort(bool input, uint32_t index, AudioPort& port) override;
+  void initPortGroup(uint32_t groupId, PortGroup& portGroup) override;
+  {%- endif %}
 
   // -------------------------------------------------------------------
   // Internal data
 
   float getParameterValue(uint32_t index) const override;
   void  setParameterValue(uint32_t index, float value) override;
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2dpf/templates/Makefile.project` & `hvcc-0.7.0/hvcc/generators/c2dpf/templates/Makefile_project`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/c2fabric.py` & `hvcc-0.7.0/hvcc/generators/c2fabric/c2fabric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,51 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2021-2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import hashlib
 import jinja2
 import os
 import shutil
 import time
+from typing import Dict, Optional
+
 from ..buildjson import buildjson
 from ..copyright import copyright_manager
+from ..filters import filter_templates, filter_xcode_build, filter_xcode_copy, filter_xcode_fileref
 
 
 class c2fabric:
     """Generates a DSP component for Fabric.
     """
 
     @classmethod
-    def filter_xcode_copy(clazz, s):
-        """Return a copyref hash suitable for use in an Xcode project file.
-        """
-        s = hashlib.md5(f"{s}_copy".encode('utf-8'))
-        return s.hexdigest().upper()[0:24]
-
-    @classmethod
-    def filter_xcode_build(clazz, s):
-        """Return a build hash suitable for use in an Xcode project file.
-        """
-        s = hashlib.md5(f"{s}_build".encode('utf-8'))
-        return s.hexdigest().upper()[0:24]
-
-    @classmethod
-    def filter_xcode_fileref(clazz, s):
-        """Return a fileref hash suitable for use in an Xcode project file.
-        """
-        s = hashlib.md5(f"{s}_fileref".encode('utf-8'))
-        return s.hexdigest().upper()[0:24]
-
-    @classmethod
-    def filter_templates(clazz, template_name):
-        return False if os.path.basename(template_name) in [".DS_Store"] else True
-
-    @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         in_parameter_list = externs["parameters"]["in"]
         out_parameter_list = externs["parameters"]["out"]
         in_event_list = externs["events"]["in"]
         out_event_list = externs["events"]["out"]
@@ -65,17 +53,17 @@
         out_dir = os.path.join(out_dir, "fabric")
         patch_name = patch_name or "heavy"
 
         copyright = copyright_manager.get_copyright_for_c(copyright)
 
         # initialise the jinja template environment
         env = jinja2.Environment()
-        env.filters["xcode_build"] = c2fabric.filter_xcode_build
-        env.filters["xcode_fileref"] = c2fabric.filter_xcode_fileref
-        env.filters["xcode_copy"] = c2fabric.filter_xcode_copy
+        env.filters["xcode_build"] = filter_xcode_build
+        env.filters["xcode_copy"] = filter_xcode_copy
+        env.filters["xcode_fileref"] = filter_xcode_fileref
         env.loader = jinja2.FileSystemLoader(
             encoding="utf-8-sig",
             searchpath=[os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates")])
 
         src_out_dir = os.path.join(out_dir, "source")
 
         try:
@@ -87,15 +75,15 @@
             # copy over generated C source files
             src_out_dir = os.path.join(out_dir, "source", "heavy")
             shutil.copytree(c_src_dir, src_out_dir)
 
             files_to_copy = [f"Hv_{patch_name}_FabricDSP.cs", f"Hv_{patch_name}_FabricDSPEditor.cs"]
 
             # generate files from templates
-            for f in env.list_templates(filter_func=c2fabric.filter_templates):
+            for f in env.list_templates(filter_func=filter_templates):
                 file_path = os.path.join(out_dir, f)
                 file_path = file_path.replace("{{name}}", patch_name)
 
                 if not os.path.exists(os.path.dirname(file_path)):
                     os.makedirs(os.path.dirname(file_path))
 
                 with open(file_path, "w") as g:
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/android/jni/Android.mk` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/linux/Makefile` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/linux/Makefile`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/Hv_{{name}}_Fabric.sln`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/vs2015/lib{{name}}.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/project.pbxproj` & `hvcc-0.7.0/hvcc/generators/c2fabric/templates/xcode/Hv_{{name}}_Fabric.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2js/c2js.py` & `hvcc-0.7.0/hvcc/generators/c2js/c2js.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2021-2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -15,14 +16,15 @@
 
 import os
 import subprocess
 import time
 import jinja2
 
 from shutil import which
+from typing import Dict, Optional
 
 from hvcc.core.hv2ir.HeavyException import HeavyException
 from ..copyright import copyright_manager
 
 
 class c2js:
     """Compiles a directory of C source files into javascript. Requires the
@@ -53,22 +55,32 @@
         "_hv_table_setLength",
         "_hv_table_getBuffer",
         "_hv_sendMessageToReceiverV",
         "_malloc"  # Rationale: https://github.com/emscripten-core/emscripten/issues/6882#issuecomment-406745898
     ]
 
     @classmethod
-    def run_emscripten(clazz, c_src_dir, out_dir, patch_name, output_name, post_js_path, should_modularize,
-                       environment, pre_js_path="", binaryen_async=1):
+    def run_emscripten(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        patch_name: str,
+        output_name: str,
+        post_js_path: str,
+        should_modularize: int,
+        environment: str,
+        pre_js_path: str = "",
+        binaryen_async: int = 1
+    ) -> str:
         """Run the emcc command to compile C source files to a javascript library.
         """
 
         emcc_path = which("emcc")
 
-        if not emcc_path:
+        if emcc_path is None:
             raise HeavyException("emcc is not in the PATH")
 
         c_flags = [
             f"-I {c_src_dir}",
             "-DHV_SIMD_NONE",
             "-ffast-math",
             "-DNDEBUG",
@@ -79,27 +91,27 @@
         cpp_src_paths = [os.path.join(c_src_dir, cpp) for cpp in os.listdir(c_src_dir) if cpp.endswith((".cpp"))]
         obj_paths = []
         cmd = ""
 
         # compile C files
         for c in c_src_paths:
             obj_path = f"{os.path.splitext(c)[0]}.o"
-            cmd = [emcc_path] + c_flags + ["-c", "-o", obj_path, c]
+            cmd = [emcc_path] + c_flags + ["-c", "-o", obj_path, c]  # type: ignore
             subprocess.check_output(cmd)  # run emscripten
             obj_paths += [obj_path]
 
         # compile C++ files
         for cpp in cpp_src_paths:
             obj_path = f"{os.path.splitext(cpp)[0]}.o"
-            cmd = [emcc_path] + c_flags + ["-std=c++11"] + ["-c", "-o", obj_path, cpp]
+            cmd = [emcc_path] + c_flags + ["-std=c++11"] + ["-c", "-o", obj_path, cpp]  # type: ignore
             subprocess.check_output(cmd)  # run emscripten
             obj_paths += [obj_path]
 
         # exported heavy api methods
-        hv_api_defs = ", ".join([f"\"{x.format(patch_name)}\"" for x in c2js.__HV_API])
+        hv_api_defs = ", ".join([f"\"{x.format(patch_name)}\"" for x in cls.__HV_API])
 
         # output path
         wasm_js_path = os.path.join(out_dir, f"{output_name}.js")
 
         linker_flags = [
             "-O3",
             "--memory-init-file", "0",
@@ -118,31 +130,41 @@
 
         if len(pre_js_path):
             linker_flags = linker_flags + [
                 "--pre-js", pre_js_path
             ]
 
         # include C/C++ obj files in js library
-        cmd = [emcc_path] + obj_paths + linker_flags
+        cmd = [emcc_path] + obj_paths + linker_flags  # type: ignore
         subprocess.check_output(  # WASM
-            cmd + [
+            cmd + [  # type: ignore
                 "-s", "WASM=1",
                 "-s", f"EXPORT_NAME='{output_name}_Module'",
                 "-o", wasm_js_path
             ])
 
         # clean up
         for o in obj_paths:
             os.remove(o)
 
         return wasm_js_path
 
     @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         parameter_list = externs["parameters"]["in"]
         event_list = externs["events"]["in"]
 
         out_dir = os.path.join(out_dir, "js")
@@ -169,21 +191,21 @@
             with open(post_js_path, "w") as f:
                 f.write(env.get_template("hv_wrapper.js").render(
                     name=patch_name,
                     copyright=copyright_js,
                     externs=externs,
                     pool_sizes_kb=externs["memoryPoolSizesKb"]))
 
-            js_path = c2js.run_emscripten(c_src_dir=c_src_dir,
-                                          out_dir=out_dir,
-                                          patch_name=patch_name,
-                                          output_name=patch_name,
-                                          post_js_path=post_js_path,
-                                          should_modularize=1,
-                                          environment="web")
+            js_path = cls.run_emscripten(c_src_dir=c_src_dir,
+                                         out_dir=out_dir,
+                                         patch_name=patch_name,
+                                         output_name=patch_name,
+                                         post_js_path=post_js_path,
+                                         should_modularize=1,
+                                         environment="web")
 
             # delete temporary files
             os.remove(post_js_path)
 
             js_out_file = os.path.basename(js_path)
 
             # generate index.html from template
@@ -210,23 +232,23 @@
             with open(pre_js_path, "w") as f:
                 f.write(env.get_template("hv_worklet_start.js").render(
                     name=patch_name,
                     copyright=copyright_js,
                     externs=externs,
                     pool_sizes_kb=externs["memoryPoolSizesKb"]))
 
-            js_path = c2js.run_emscripten(c_src_dir=c_src_dir,
-                                          out_dir=out_dir,
-                                          patch_name=patch_name,
-                                          output_name=f"{patch_name}_AudioLibWorklet",
-                                          post_js_path=post_js_path,
-                                          should_modularize=0,
-                                          environment="worker",
-                                          pre_js_path=pre_js_path,
-                                          binaryen_async=0)
+            js_path = cls.run_emscripten(c_src_dir=c_src_dir,
+                                         out_dir=out_dir,
+                                         patch_name=patch_name,
+                                         output_name=f"{patch_name}_AudioLibWorklet",
+                                         post_js_path=post_js_path,
+                                         should_modularize=0,
+                                         environment="worker",
+                                         pre_js_path=pre_js_path,
+                                         binaryen_async=0)
 
             # delete temporary files
             os.remove(post_js_path)
             os.remove(pre_js_path)
 
             return {
                 "stage": "c2js",
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2js/template/hv_worklet.js` & `hvcc-0.7.0/hvcc/generators/c2js/template/hv_worklet.js`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2js/template/hv_wrapper.js` & `hvcc-0.7.0/hvcc/generators/c2js/template/hv_wrapper.js`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2js/template/index.html` & `hvcc-0.7.0/hvcc/generators/c2js/template/index.html`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2owl/c2owl.py` & `hvcc-0.7.0/hvcc/generators/c2owl/c2owl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # import datetime
 import os
 import shutil
 import time
 import jinja2
 import json
+from typing import Dict, List, Optional
 from ..buildjson import buildjson
 from ..copyright import copyright_manager
+
 import hvcc.core.hv2ir.HeavyLangObject as HeavyLangObject
 
 
 heavy_hash = HeavyLangObject.HeavyLangObject.get_hash
 OWL_BUTTONS = ['Push', 'B1', 'B2', 'B3', 'B4', 'B5', 'B6', 'B7', 'B8']
 
 
 class c2owl:
     """ Generates a OWL wrapper for a given patch.
     """
 
     @classmethod
-    def make_jdata(clazz, patch_ir):
+    def make_jdata(cls, patch_ir: str) -> List:
         jdata = list()
 
         with open(patch_ir, mode="r") as f:
             ir = json.load(f)
 
             for name, v in ir['control']['receivers'].items():
                 # skip __hv_init and similar
@@ -60,16 +62,26 @@
                                           0, 1, None, key in OWL_BUTTONS))
                 except Exception:
                     pass
 
             return jdata
 
     @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         out_dir = os.path.join(out_dir, "Source")
         patch_name = patch_name or "heavy"
         copyright_c = copyright_manager.get_copyright_for_c(copyright)
 
@@ -90,15 +102,15 @@
 
             env.loader = jinja2.FileSystemLoader(
                 os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates"))
 
             # construct jdata from ir
             ir_dir = os.path.join(c_src_dir, "../ir")
             patch_ir = os.path.join(ir_dir, f"{patch_name}.heavy.ir.json")
-            jdata = c2owl.make_jdata(patch_ir)
+            jdata = cls.make_jdata(patch_ir)
 
             # generate OWL wrapper from template
             owl_hpp_path = os.path.join(out_dir, f"HeavyOWL_{patch_name}.hpp")
             with open(owl_hpp_path, "w") as f:
                 f.write(env.get_template("HeavyOwl.hpp").render(
                     jdata=jdata,
                     name=patch_name,
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2owl/deps/HvMessage.c` & `hvcc-0.7.0/hvcc/generators/c2owl/deps/HvMessage.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2owl/deps/HvUtils.h` & `hvcc-0.7.0/hvcc/generators/c2owl/deps/HvUtils.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2owl/templates/HeavyOwl.hpp` & `hvcc-0.7.0/hvcc/generators/c2owl/templates/HeavyOwl.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2pdext/c2pdext.py` & `hvcc-0.7.0/hvcc/generators/c2pdext/c2pdext.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2021-2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import hashlib
 import os
 import shutil
 import time
 import jinja2
+from typing import Dict, Optional
+
 from ..copyright import copyright_manager
+from ..filters import filter_max, filter_xcode_build, filter_xcode_fileref
 
 
 class c2pdext:
     """Generates a Pure Data external wrapper for a given patch.
     """
 
     @classmethod
-    def filter_max(clazz, i, j):
-        """Calculate the maximum of two integers.
-        """
-        return max(int(i), int(j))
-
-    @classmethod
-    def filter_xcode_build(clazz, s):
-        """Return a build hash suitable for use in an Xcode project file.
-        """
-        s = f"{s}_build"
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:24]
-        return s
-
-    @classmethod
-    def filter_xcode_fileref(clazz, s):
-        """Return a fileref hash suitable for use in an Xcode project file.
-        """
-        s = f"{s}_fileref"
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:24]
-        return s
-
-    @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         out_dir = os.path.join(out_dir, "pdext")
         receiver_list = externs["parameters"]["in"]
 
         copyright = copyright_manager.get_copyright_for_c(copyright)
@@ -76,34 +65,34 @@
         shutil.copy(
             os.path.join(os.path.dirname(os.path.abspath(__file__)), "static", "m_pd.h"),
             out_dir)
 
         try:
             # initialise the jinja template environment
             env = jinja2.Environment()
-            env.filters["max"] = c2pdext.filter_max
-            env.filters["xcode_build"] = c2pdext.filter_xcode_build
-            env.filters["xcode_fileref"] = c2pdext.filter_xcode_fileref
+            env.filters["max"] = filter_max
+            env.filters["xcode_build"] = filter_xcode_build
+            env.filters["xcode_fileref"] = filter_xcode_fileref
             env.loader = jinja2.FileSystemLoader(
                 os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates"))
 
             # generate Pd external wrapper from template
-            pdext_path = os.path.join(out_dir, "{0}.c".format(struct_name))
+            pdext_path = os.path.join(out_dir, f"{struct_name}.c")
             with open(pdext_path, "w") as f:
                 f.write(env.get_template("pd_external.c").render(
                     name=patch_name,
                     struct_name=struct_name,
                     display_name=ext_name,
                     num_input_channels=num_input_channels,
                     num_output_channels=num_output_channels,
                     receivers=receiver_list,
                     copyright=copyright))
 
             # generate Xcode project
-            xcode_path = os.path.join(out_dir, "{0}.xcodeproj".format(struct_name))
+            xcode_path = os.path.join(out_dir, f"{struct_name}.xcodeproj")
             os.mkdir(xcode_path)  # create the xcode project bundle
             pbxproj_path = os.path.join(xcode_path, "project.pbxproj")
 
             # generate list of source files
             files = [g for g in os.listdir(out_dir) if g.endswith((".h", ".hpp", ".c", ".cpp"))]
 
             # render the pbxproj file
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2pdext/static/m_pd.h` & `hvcc-0.7.0/hvcc/generators/c2pdext/static/m_pd.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2pdext/templates/pd_external.c` & `hvcc-0.7.0/hvcc/generators/c2pdext/templates/pd_external.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2pdext/templates/project.pbxproj` & `hvcc-0.7.0/hvcc/generators/c2pdext/templates/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/c2unity.py` & `hvcc-0.7.0/hvcc/generators/c2unity/c2unity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,68 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2021-2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import hashlib
 import jinja2
 import os
 import shutil
 import time
+from typing import Dict, Optional
+
 from ..copyright import copyright_manager
 from ..buildjson import buildjson
+from ..filters import filter_string_cap, filter_templates, filter_xcode_build, filter_xcode_fileref
 
 
 class c2unity:
     """Generates a Audio Native Plugin wrapper for Unity 5.
     """
 
     @classmethod
-    def filter_xcode_build(clazz, s):
-        """Return a build hash suitable for use in an Xcode project file.
-        """
-        s = f"{s}_build"
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:24]
-        return s
-
-    @classmethod
-    def filter_xcode_fileref(clazz, s):
-        """Return a fileref hash suitable for use in an Xcode project file.
-        """
-        f"{s}_fileref"
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:24]
-        return s
-
-    @classmethod
-    def filter_string_cap(clazz, s, li):
-        """Returns a truncated string with ellipsis if it exceeds a certain length.
-        """
-        return s if (len(s) <= li) else f"{s[0:li - 3]}..."
-
-    @classmethod
-    def filter_templates(clazz, template_name):
-        return False if os.path.basename(template_name) in [".DS_Store"] else True
-
-    @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         parameter_list = externs["parameters"]["in"]
         event_list = externs["events"]["in"]
         table_list = externs["tables"]
 
         out_dir = os.path.join(out_dir, "unity")
         patch_name = patch_name or "heavy"
 
         copyright = copyright_manager.get_copyright_for_c(copyright)
 
         # initialise the jinja template environment
         env = jinja2.Environment()
-        env.filters["xcode_build"] = c2unity.filter_xcode_build
-        env.filters["xcode_fileref"] = c2unity.filter_xcode_fileref
-        env.filters["cap"] = c2unity.filter_string_cap
+        env.filters["xcode_build"] = filter_xcode_build
+        env.filters["xcode_fileref"] = filter_xcode_fileref
+        env.filters["cap"] = filter_string_cap
         env.loader = jinja2.FileSystemLoader(
             encoding="utf-8-sig",
             searchpath=[os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates")])
 
         static_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "static")
         src_out_dir = os.path.join(out_dir, "source")
 
@@ -91,15 +76,15 @@
             shutil.copytree(static_dir, out_dir)
 
             # copy over generated C source files
             src_out_dir = os.path.join(out_dir, "source", "heavy")
             shutil.copytree(c_src_dir, src_out_dir)
 
             # generate files from templates
-            for f in env.list_templates(filter_func=c2unity.filter_templates):
+            for f in env.list_templates(filter_func=filter_templates):
                 file_path = os.path.join(out_dir, f)
                 file_path = file_path.replace("{{name}}", patch_name)
 
                 if not os.path.exists(os.path.dirname(file_path)):
                     os.makedirs(os.path.dirname(file_path))
 
                 with open(file_path, "w") as g:
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h` & `hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp` & `hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h` & `hvcc-0.7.0/hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/static/xcode/Info.plist` & `hvcc-0.7.0/hvcc/generators/c2unity/static/xcode/Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/android/jni/Android.mk` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/linux/Makefile` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/linux/Makefile`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioLib.cs`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/source/unity/Hv_{{name}}_AudioPlugin.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/AudioPlugin_Hv_{{name}}.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_AudioLib.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/vs2015/Hv_{{name}}_Unity.sln`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj` & `hvcc-0.7.0/hvcc/generators/c2unity/templates/xcode/Hv_{{name}}_Unity.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/c2wwise.py` & `hvcc-0.7.0/hvcc/generators/c2wwise/c2wwise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,52 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2021-2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import hashlib
 import os
 import shutil
 import time
 import jinja2
+from typing import Dict, Optional
+
 from ..buildjson import buildjson
 from ..copyright import copyright_manager
+from ..filters import filter_plugin_id, filter_xcode_build, filter_xcode_fileref
 
 
 class c2wwise:
     """Generates a plugin wrapper for Audiokinetic's Wwise game audio middleware
     platform.
     """
 
     @classmethod
-    def filter_xcode_build(clazz, s):
-        """Return a build hash suitable for use in an Xcode project file.
-        """
-        s = f"{s}_build"
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:24]
-        return s
-
-    @classmethod
-    def filter_xcode_fileref(clazz, s):
-        """Return a fileref hash suitable for use in an Xcode project file.
-        """
-        s = f"{s}_fileref"
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest().upper()[0:24]
-        return s
-
-    @classmethod
-    def filter_plugin_id(clazz, s):
-        """ Return a unique id from patch name
-            [0...32767
-        """
-        s = hashlib.md5(s.encode('utf-8'))
-        s = s.hexdigest()[:4]
-        s = int(s, 16) & 0x7FFF
-        return s
-
-    @classmethod
-    def compile(clazz, c_src_dir, out_dir, externs, patch_name=None, patch_meta: dict = None,
-                num_input_channels=0, num_output_channels=0, copyright=None, verbose=False):
+    def compile(
+        cls,
+        c_src_dir: str,
+        out_dir: str,
+        externs: Dict,
+        patch_name: Optional[str] = None,
+        patch_meta: Optional[Dict] = None,
+        num_input_channels: int = 0,
+        num_output_channels: int = 0,
+        copyright: Optional[str] = None,
+        verbose: Optional[bool] = False
+    ) -> Dict:
 
         tick = time.time()
 
         in_parameter_list = externs["parameters"]["in"]
         out_parameter_list = externs["parameters"]["out"]
         event_list = externs["events"]["in"]
         table_list = externs["tables"]
@@ -75,19 +60,19 @@
         wwise_sdk_version = "2017.2.2.6553"
 
         if not os.path.exists(out_dir):
             os.makedirs(out_dir)
 
         templates_dir = os.path.join(os.path.dirname(__file__), "templates")
         plugin_type = "Source" if num_input_channels == 0 else "FX"
-        plugin_id = c2wwise.filter_plugin_id(patch_name)
+        plugin_id = filter_plugin_id(patch_name)
 
         env = jinja2.Environment()
-        env.filters["xcode_build"] = c2wwise.filter_xcode_build
-        env.filters["xcode_fileref"] = c2wwise.filter_xcode_fileref
+        env.filters["xcode_build"] = filter_xcode_build
+        env.filters["xcode_fileref"] = filter_xcode_fileref
         env.loader = jinja2.FileSystemLoader(
             encoding="utf-8-sig",
             searchpath=[templates_dir])
 
         try:
             if plugin_type == "FX":
                 if num_input_channels > 2:
```

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/linux/Makefile` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/linux/Makefile`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/resources/Hv_{{name}}_Wwise{{type}}AuthPlugin.xml`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPlugin.rc`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseAuthoringPluginApp.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/authoring/Hv_{{name}}_WwiseResource.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_WwisePluginEngineParams.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/engine/Hv_{{name}}_Wwise{{type}}PluginEngine.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/Hv_{{name}}_WwisePluginIDs.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/AudioDecoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Common.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/Dither.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/IMA4Util.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/ModplugDecoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/PostProcess.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/RiffUtils.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavDecoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/libnyquist/WavEncoder.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/include/stdafx.h` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/include/stdafx.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/AudioDecoder.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/Common.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/RiffUtils.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavDecoder.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/source/libnyquist/WavEncoder.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}AuthPlugin.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Engine.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}Plugin.sln`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/vs2015/Hv_{{name}}_Wwise{{type}}RuntimePlugin.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/Info.plist` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj` & `hvcc-0.7.0/hvcc/generators/c2wwise/templates/xcode/Plugin.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/copyright/default_template.txt` & `hvcc-0.7.0/hvcc/generators/copyright/default_template.txt`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlBinop.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlBinop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
 from .HeavyObject import HeavyObject
 
 
 class ControlBinop(HeavyObject):
     # a dictionary translating from the operation argument to the C case
     __OPERATION_DICT = {
         "__add": "HV_BINOP_ADD",
@@ -70,49 +72,49 @@
         "__bimod_k": "HV_BINOP_MOD_BIPOLAR"
     }
 
     c_struct = "ControlBinop"
     preamble = "cBinop"
 
     @classmethod
-    def handles_type(clazz, obj_type):
+    def handles_type(cls, obj_type: str) -> bool:
         """Returns true if the object type can be handled by this class
         """
-        return obj_type in ControlBinop.__OPERATION_DICT
+        return obj_type in cls.__OPERATION_DICT
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlBinop.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlBinop.h", "HvControlBinop.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if obj_type.endswith("_k"):
             return []
         else:
             obj_arg = float(list(args.values())[0])
             return [f"cBinop_init(&cBinop_{obj_id}, {obj_arg}f); // {obj_type}"]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []  # no need to free any control binop objects
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         if obj_type.endswith("_k"):
             return [
                 "cBinop_k_onMessage(_c, NULL, {0}, {1}f, {2}, m, &cBinop_{3}_sendMessage);".format(
-                    ControlBinop.__OPERATION_DICT[obj_type[:-2]],
+                    cls.__OPERATION_DICT[obj_type[:-2]],
                     float(args["k"]),
                     inlet_index,
                     obj_id)
             ]
         else:
             return [
                 "cBinop_onMessage(_c, &Context(_c)->cBinop_{0}, {1}, {2}, m, &cBinop_{0}_sendMessage);".format(
                     obj_id,
-                    ControlBinop.__OPERATION_DICT[obj_type],
+                    cls.__OPERATION_DICT[obj_type],
                     inlet_index)
             ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlCast.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlCast.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlCast(HeavyObject):
     __OPERATION_DICT = {
         "__cast_b": "HV_CAST_BANG",
         "__cast_f": "HV_CAST_FLOAT",
         "__cast_s": "HV_CAST_SYMBOL"
     }
 
     c_struct = "ControlCast"
     preamble = "cCast"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlCast.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlCast.h", "HvControlCast.c"}
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
             "cCast_onMessage(_c, {1}, 0, m, &cCast_{0}_sendMessage);".format(
                 obj_id,
-                ControlCast.__OPERATION_DICT[obj_type])
+                cls.__OPERATION_DICT[obj_type])
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlDelay.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlDelay.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Callable, Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlDelay(HeavyObject):
 
     c_struct = "ControlDelay"
     preamble = "cDelay"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlDelay.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlDelay.h", "HvControlDelay.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "{0}_init(this, &{0}_{1}, {2}f);".format(
-                clazz.preamble,
+                cls.preamble,
                 obj_id,
                 float(args["delay"]))
         ]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []  # no need to free any control binop objects
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
             "{0}_onMessage(_c, &Context(_c)->{0}_{1}, {2}, m, "
             "&{0}_{1}_sendMessage);".format(
-                clazz.preamble,
+                cls.preamble,
                 obj_id,
                 inlet_index)
         ]
 
     @classmethod
-    def get_C_impl(clazz, obj_type, obj_id, on_message_list, get_obj_class, objects):
+    def get_C_impl(
+        cls,
+        obj_type: str,
+        obj_id: int,
+        on_message_list: List,
+        get_obj_class: Callable,
+        objects: Dict
+    ) -> List[str]:
         send_message_list = [
             f"cDelay_{obj_id}_sendMessage(HeavyContextInterface *_c, int letIn, const HvMessage *const m) {{"
         ]
         send_message_list.append(f"cDelay_clearExecutingMessage(&Context(_c)->cDelay_{obj_id}, m);")
         send_message_list.extend(
-            HeavyObject._get_on_message_list(on_message_list[0], get_obj_class, objects))
+            cls._get_on_message_list(on_message_list[0], get_obj_class, objects))
         send_message_list.append("}")  # end function
         return send_message_list
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlIf.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlIf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlIf(HeavyObject):
 
     c_struct = "ControlIf"
     preamble = "cIf"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlIf.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlIf.h", "HvControlIf.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "{0}_init(&{0}_{1}, {2});".format(
-                clazz.preamble,
+                cls.preamble,
                 obj_id,
                 "true" if float(args["k"]) != 0.0 else "false"
             )]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []  # no need to free any control binop objects
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
             "{0}_onMessage(_c, &Context(_c)->{0}_{1}, {2}, m, "
-            "&{0}_{1}_sendMessage);".format(clazz.preamble, obj_id, inlet_index)
+            "&{0}_{1}_sendMessage);".format(cls.preamble, obj_id, inlet_index)
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlMessage.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlMessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,28 +11,36 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
+from typing import Callable, Dict, List
 
 from .HeavyObject import HeavyObject
 
 
 class ControlMessage(HeavyObject):
 
     preamble = "cMsg"
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [f"cMsg_{obj_id}_sendMessage(_c, 0, m);"]
 
     @classmethod
-    def get_C_impl(clazz, obj_type, obj_id, on_message_list, get_obj_class, objects):
+    def get_C_impl(
+        cls,
+        obj_type: str,
+        obj_id: int,
+        on_message_list: List,
+        get_obj_class: Callable,
+        objects: Dict
+    ) -> List[str]:
         send_message_list = [
             f"cMsg_{obj_id}_sendMessage(HeavyContextInterface *_c, int letIn, const HvMessage *const n) {{"
         ]
 
         if len(objects[obj_id]["args"]["local"]) > 0:
             # declare the outgoing messages (if there are any)
             send_message_list.append("HvMessage *m = nullptr;")
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlPack.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalDel1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class ControlPack(HeavyObject):
-    """Prints the first value in a message to the console"""
+class SignalDel1(HeavyObject):
+    """Handles the __del1~f object.
+    """
 
-    c_struct = "ControlPack"
-    preamble = "cPack"
+    c_struct = "SignalDel1"
+    preamble = "sDel1"
 
     @classmethod
-    def get_C_header_set(clazz):
-        return {"HvControlPack.h"}
+    def get_C_header_set(cls) -> set:
+        return {"HvSignalDel1.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvControlPack.h", "HvControlPack.c"}
+    def get_C_file_set(cls) -> set:
+        return {"HvSignalDel1.h", "HvSignalDel1.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return [
-            "cPack_init(&cPack_{0}, {1}, {2});".format(
-                obj_id,
-                len(args["values"]),
-                ", ".join(["{0}f".format(float(x)) for x in args["values"]]))
-        ]
+    def get_C_def(cls, obj_type: str, obj_id: int) -> List[str]:
+        return [f"SignalDel1 sDel1_{obj_id};"]
+
+    @classmethod
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [f"sDel1_init(&sDel1_{obj_id});"]
+
+    @classmethod
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "cPack_onMessage(_c, &Context(_c)->cPack_{0}, {1}, m, &cPack_{0}_sendMessage);".format(
-                obj_id,
-                inlet_index)
-        ]
+            "__hv_del1_f(&sDel1_{0}, VIf({1}), VOf({2}));".format(
+                process_dict["id"],
+                cls._c_buffer(process_dict["inputBuffers"][0]),
+                cls._c_buffer(process_dict["outputBuffers"][0]))]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlPrint.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlTabhead.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyObject import HeavyObject
+from typing import Dict, List
 
+from .HeavyObject import HeavyObject
 
-class ControlPrint(HeavyObject):
-    """Prints the first value in a message to the console"""
 
-    preamble = "cPrint"
+class ControlTabhead(HeavyObject):
+    """Handles __tabhead
+    """
 
-    @classmethod
-    def get_C_header_set(clazz):
-        return {"HvControlPrint.h"}
+    c_struct = "ControlTabhead"
+    preamble = "cTabhead"
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvControlPrint.h", "HvControlPrint.c"}
+    def get_C_header_set(cls) -> set:
+        return {"HvControlTabhead.h"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return []
+    def get_C_file_set(cls) -> set:
+        return {"HvControlTabhead.h", "HvControlTabhead.c"}
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [f"cPrint_onMessage(_c, m, \"{args['label']}\");"]
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [f"cTabhead_init(&cTabhead_{obj_id}, &hTable_{args['table_id']});"]
 
     @classmethod
-    def get_C_decl(clazz, obj_type, obj_id, args):
-        return []
-
-    @classmethod
-    def get_C_impl(clazz, obj_type, obj_id, on_message_list, obj_class_dict):
-        return []
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return [f"cTabhead_onMessage(_c, &Context(_c)->cTabhead_{obj_id}, 0, m, &cTabhead_{obj_id}_sendMessage);"]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlRandom.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlRandom.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlRandom(HeavyObject):
 
     c_struct = "ControlRandom"
     preamble = "cRandom"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlRandom.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlRandom.h", "HvControlRandom.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "{0}_init(&{0}_{1}, {2});".format(
-                clazz.preamble, obj_id, int(args["seed"]))
+                cls.preamble, obj_id, int(args["seed"]))
         ]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []  # no need to free any control binop objects
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
             "{0}_onMessage(_c, &Context(_c)->{0}_{1}, {2}, m, "
-            "&{0}_{1}_sendMessage);".format(clazz.preamble, obj_id, inlet_index)
+            "&{0}_{1}_sendMessage);".format(cls.preamble, obj_id, inlet_index)
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlReceive.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HIrReceive.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyObject import HeavyObject
+import re
+from typing import Dict, Optional, TYPE_CHECKING
 
+from .HeavyIrObject import HeavyIrObject
 
-class ControlReceive(HeavyObject):
+if TYPE_CHECKING:
+    from .HeavyGraph import HeavyGraph
 
-    c_struct = "ControlReceive"
-    preamble = "cReceive"
 
-    @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [f"cReceive_{obj_id}_sendMessage(_c, 0, m);"]
+class HIrReceive(HeavyIrObject):
+    """ A specific implementation of the __receive object.
+    """
+
+    def __init__(
+        self,
+        obj_type: str,
+        args: Optional[Dict] = None,
+        graph: Optional['HeavyGraph'] = None,
+        annotations: Optional[Dict] = None
+    ) -> None:
+        super().__init__("__receive", args=args, graph=graph, annotations=annotations)
+        if args is not None and args["extern"]:
+            # externed receivers must contain only alphanumeric characters or underscores,
+            # so that the names can be easily and transparently turned into code
+            if re.search(r"\W", args["name"]):
+                self.add_error("Parameter and Event names may only contain"
+                               f"alphanumeric characters or underscore: '{args['name']}'")
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlSend.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlSend.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Callable, Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlSend(HeavyObject):
 
     c_struct = "ControlSend"
     preamble = "cSend"
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [f"cSend_{obj_id}_sendMessage(_c, 0, m);"]
 
     @classmethod
-    def get_C_impl(clazz, obj_type, obj_id, on_message_list, get_obj_class, objects):
+    def get_C_impl(
+        cls,
+        obj_type: str,
+        obj_id: int,
+        on_message_list: List,
+        get_obj_class: Callable,
+        objects: Dict
+    ) -> List[str]:
         # Note(joe): if no corresponding receivers exist and there's no extern indicator
         # then there is not much need to generate code stub
         send_message_list = [
             "{0}_{1}_sendMessage(HeavyContextInterface *_c, int letIn, const HvMessage *m) {{".format(
-                clazz.get_preamble(obj_type),
+                cls.get_preamble(obj_type),
                 obj_id)]
 
         if objects[obj_id]["args"].get("extern", False):
             # call the send hook
             send_name = objects[obj_id]["args"]["name"]
             send_message_list.append("if (_c->getSendHook() != nullptr) _c->getSendHook()(_c, \"{0}\", {1}, m);".format(
                 send_name,
-                HeavyObject.get_hash_string(send_name)))
+                cls.get_hash_string(send_name)))
 
         # a send has only one (implicit!) outlet
         send_message_list.extend(
-            HeavyObject._get_on_message_list(on_message_list[0], get_obj_class, objects))
+            cls._get_on_message_list(on_message_list[0], get_obj_class, objects))
 
         send_message_list.append("}")  # end function
 
         return send_message_list
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlSlice.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlSlice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlSlice(HeavyObject):
 
     c_struct = "ControlSlice"
     preamble = "cSlice"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlSlice.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlSlice.h", "HvControlSlice.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "cSlice_init(&cSlice_{0}, {1}, {2});".format(
                 obj_id,
                 int(args["index"]),
                 int(args["length"]))]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []  # nothing to free
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
-            "cSlice_onMessage(_c, &Context(_c)->cSlice_{0}, {1}, m, &cSlice_{0}_sendMessage);".format(
-                obj_id,
-                inlet_index)
+            f"cSlice_onMessage(_c, &Context(_c)->cSlice_{obj_id}, {inlet_index}, m, &cSlice_{obj_id}_sendMessage);"
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlSwitchcase.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlUnop.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class ControlSwitchcase(HeavyObject):
+class ControlUnop(HeavyObject):
+    # a dictionary translating from the operation argument to the C case
+    __OPERATION_DICT = {
+        "__cos": "HV_UNOP_COS",
+        "__acos": "HV_UNOP_ACOS",
+        "__cosh": "HV_UNOP_COSH",
+        "__acosh": "HV_UNOP_ACOSH",
+        "__sin": "HV_UNOP_SIN",
+        "__asin": "HV_UNOP_ASIN",
+        "__sinh": "HV_UNOP_SINH",
+        "__asinh": "HV_UNOP_ASINH",
+        "__tan": "HV_UNOP_TAN",
+        "__atan": "HV_UNOP_ATAN",
+        "__tanh": "HV_UNOP_TANH",
+        "__atanh": "HV_UNOP_ATANH",
+        "__log": "HV_UNOP_LOG",
+        "__log10": "HV_UNOP_LOG10",
+        "__log2": "HV_UNOP_LOG2",
+        "__exp": "HV_UNOP_EXP",
+        "__abs": "HV_UNOP_ABS",
+        "__sqrt": "HV_UNOP_SQRT",
+        "__ceil": "HV_UNOP_CEIL",
+        "__floor": "HV_UNOP_FLOOR",
+        "__round": "HV_UNOP_ROUND"
+    }
 
-    c_struct = "ControlSwitchase"
-    preamble = "cSwichcase"
+    c_struct = "ControlUnop"
+    preamble = "cUnop"
 
     @classmethod
-    def get_C_def(clazz, obj_type, obj_id):
-        return []
+    def handles_type(cls, obj_type: str) -> bool:
+        """Returns true if the object type can be handled by this class
+        """
+        return obj_type in cls.__OPERATION_DICT
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
-        return []
+    def get_C_header_set(cls) -> set:
+        return {"HvControlUnop.h"}
 
     @classmethod
-    def get_C_decl(clazz, obj_type, obj_id, args):
-        return [
-            f"cSwitchcase_{obj_id}_onMessage(HeavyContextInterface *, void *, int letIn, "
-            "const HvMessage *const, void *);"
-        ]
+    def get_C_file_set(cls) -> set:
+        return {"HvControlUnop.h", "HvControlUnop.c"}
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [f"cSwitchcase_{obj_id}_onMessage(_c, NULL, {inlet_index}, m, NULL);"]
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
 
     @classmethod
-    def get_C_impl(clazz, obj_type, obj_id, on_message_list, obj_class_dict, objects):
-        # generate the onMessage implementation
-        out_list = [
-            f"cSwitchcase_{obj_id}_onMessage(HeavyContextInterface *_c, void *o, int letIn, "
-            f"const HvMessage *const m, void *sendMessage) {{"
-        ]
-        out_list.append("switch (msg_getHash(m, 0)) {")
-        cases = objects[obj_id]["args"]["cases"]
-        for i, c in enumerate(cases):
-            hv_hash = HeavyObject.get_hash_string(c)
-            out_list.append(f"case {hv_hash}: {{ // \"{c}\"")
-            out_list.extend(
-                HeavyObject._get_on_message_list(on_message_list[i], obj_class_dict, objects))
-            out_list.append("break;")
-            out_list.append("}")
-        out_list.append("default: {")
-        out_list.extend(
-            HeavyObject._get_on_message_list(on_message_list[-1], obj_class_dict, objects))
-        out_list.append("break;")
-        out_list.append("}")  # end default
-        out_list.append("}")  # end switch
-        out_list.append("}")  # end function
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
 
-        return out_list
+    @classmethod
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return [
+            "cUnop_onMessage(_c, {1}, m, &cUnop_{0}_sendMessage);".format(
+                obj_id,
+                cls.__OPERATION_DICT[obj_type])
+        ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlSystem.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlSystem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlSystem(HeavyObject):
 
     c_struct = "ControlSystem"
     preamble = "cSystem"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlSystem.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlSystem.h", "HvControlSystem.c"}
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [
-            "cSystem_onMessage(_c, NULL, {1}, m, &cSystem_{0}_sendMessage);".format(
-                obj_id,
-                inlet_index)
-        ]
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return [f"cSystem_onMessage(_c, NULL, {inlet_index}, m, &cSystem_{obj_id}_sendMessage);"]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlTabhead.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalTabhead.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class ControlTabhead(HeavyObject):
-    """Handles __tabhead
+class SignalTabhead(HeavyObject):
+    """Handles __tabhead~f
     """
 
-    c_struct = "ControlTabhead"
-    preamble = "cTabhead"
+    c_struct = "SignalTabhead"
+    preamble = "sTabhead"
 
     @classmethod
-    def get_C_header_set(clazz):
-        return {"HvControlTabhead.h"}
+    def get_C_header_set(cls) -> set:
+        return {"HvSignalTabread.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvControlTabhead.h", "HvControlTabhead.c"}
+    def get_C_file_set(cls) -> set:
+        return {"HvSignalTabread.h", "HvSignalTabread.c"}
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return [
-            "cTabhead_init(&cTabhead_{0}, &hTable_{1});".format(
-                obj_id,
-                args["table_id"])]
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [f"sTabhead_init(&sTabhead_{obj_id}, &hTable_{args['table_id']});"]
+
+    @classmethod
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return []  # TODO(mhroth): deal with this later
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "cTabhead_onMessage(_c, &Context(_c)->cTabhead_{0}, 0, m, &cTabhead_{0}_sendMessage);".format(
-                obj_id)]
+            "__hv_tabhead_f(&sTabhead_{0}, {1});".format(
+                process_dict["id"],
+                ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
+            )]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlTabwrite.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalTabwrite.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class ControlTabwrite(HeavyObject):
+class SignalTabwrite(HeavyObject):
+    """Handles __tabwrite~f
+    """
 
-    c_struct = "ControlTabwrite"
-    preamble = "cTabwrite"
+    c_struct = "SignalTabwrite"
+    preamble = "sTabwrite"
 
     @classmethod
-    def get_C_header_set(clazz):
-        return {"HvControlTabwrite.h"}
+    def get_C_header_set(cls) -> set:
+        return {"HvSignalTabwrite.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvControlTabwrite.h", "HvControlTabwrite.c"}
+    def get_C_file_set(cls) -> set:
+        return {"HvSignalTabwrite.h", "HvSignalTabwrite.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return [
-            "cTabwrite_init(&cTabwrite_{0}, &hTable_{1}); // {2}".format(
-                obj_id,
-                args["table_id"],
-                args["table"])
-        ]
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
-        return []
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [f"sTabwrite_init(&sTabwrite_{obj_id}, &hTable_{args['table_id']});"]
+
+    @classmethod
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return [f"sTabwrite_onMessage(_c, &Context(_c)->sTabwrite_{obj_id}, {inlet_index}, m, NULL);"]
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [
-            "cTabwrite_onMessage(_c, &Context(_c)->cTabwrite_{0}, {1}, m, &cTabwrite_{0}_sendMessage);".format(
-                obj_id,
-                inlet_index)
-        ]
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        if obj_type == "__tabwrite~f":
+            return [
+                "__hv_tabwrite_f(&sTabwrite_{0}, {1});".format(
+                    process_dict["id"],
+                    ", ".join([f"VIf({cls._c_buffer(b)})" for b in process_dict["inputBuffers"]])
+                )]
+        elif obj_type == "__tabwrite_stoppable~f":
+            return [
+                "__hv_tabwrite_stoppable_f(&sTabwrite_{0}, {1});".format(
+                    process_dict["id"],
+                    ", ".join([f"VIf({cls._c_buffer(b)})" for b in process_dict["inputBuffers"]])
+                )]
+        else:
+            raise Exception()
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ControlVar.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlVar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class ControlVar(HeavyObject):
     """An object which holds a variable. In this case only a float.
     NOTE(mhroth): maybe in the future this can hold any data structure, such as
     a generic message. At the moment, the memory churn is deemed unnecessary.
     """
 
     c_struct = "ControlVar"
     preamble = "cVar"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvControlVar.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvControlVar.h", "HvControlVar.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if isinstance(args["k"], str):
             return [
                 "cVar_init_s(&cVar_{0}, \"{1}\");".format(
                     obj_id,
                     args["k"])]
         else:
             return [
                 "cVar_init_f(&cVar_{0}, {1}f);".format(
                     obj_id,
                     float(args["k"]))]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
             "cVar_onMessage(_c, &Context(_c)->cVar_{0}, {1}, m, &cVar_{0}_sendMessage);".format(
                 obj_id,
                 inlet_index)
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/HeavyObject.py` & `hvcc-0.7.0/hvcc/generators/ir2c/HeavyObject.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,14 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from struct import unpack, pack
+from typing import Callable, Dict, List, Union
 
 
 class HeavyObject:
 
     c_struct = ""
     preamble = ""
 
@@ -26,104 +28,119 @@
         "~i>": "Bi",
         "input": "I",
         "output": "O",
         "zero": "ZERO"
     }
 
     @classmethod
-    def get_c_struct(clazz, obj_type=""):
-        return clazz.c_struct
+    def get_C_struct(cls, obj_type: str = "") -> str:
+        return cls.c_struct
 
     @classmethod
-    def get_preamble(clazz, obj_type):
-        return clazz.preamble
+    def get_preamble(cls, obj_type: str) -> str:
+        return cls.preamble
 
     @classmethod
-    def get_C_header_set(self):
+    def get_C_header_set(self) -> set:
         return set()
 
     @classmethod
-    def get_C_file_set(self):
+    def get_C_file_set(self) -> set:
         return set()
 
     @classmethod
-    def get_C_def(clazz, obj_type, obj_id):
+    def get_C_def(cls, obj_type: str, obj_id: int) -> List[str]:
         return ["{0} {1}_{2};".format(
-            clazz.get_c_struct(obj_type),
-            clazz.get_preamble(obj_type),
+            cls.get_C_struct(obj_type),
+            cls.get_preamble(obj_type),
             obj_id)]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return ["{0}_free(&{0}_{1});".format(
-            clazz.get_preamble(obj_type),
+            cls.get_preamble(obj_type),
             obj_id)]
 
     @classmethod
-    def get_C_decl(clazz, obj_type, obj_id, args):
+    def get_C_decl(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return ["{0}_{1}_sendMessage(HeavyContextInterface *, int, const HvMessage *);".format(
-                clazz.get_preamble(obj_type),
+                cls.get_preamble(obj_type),
                 obj_id)]
 
     @classmethod
-    def get_C_impl(clazz, obj_type, obj_id, on_message_list, get_obj_class, objects):
+    def get_C_impl(
+        cls,
+        obj_type: str,
+        obj_id: int,
+        on_message_list: List,
+        get_obj_class: Callable,
+        objects: Dict
+    ) -> List[str]:
         send_message_list = [
             "{0}_{1}_sendMessage(HeavyContextInterface *_c, int letIn, const HvMessage *m) {{".format(
-                clazz.get_preamble(obj_type),
+                cls.get_preamble(obj_type),
                 obj_id)]
         if len(on_message_list) == 1:
             # if there is only one outlet, skip the switch-case template
             send_message_list.extend(
-                HeavyObject._get_on_message_list(on_message_list[0], get_obj_class, objects))
+                cls._get_on_message_list(on_message_list[0], get_obj_class, objects))
         else:
             send_message_list.append("switch (letIn) {")
             for i in range(len(on_message_list)):
                 send_message_list.append(f"case {i}: {{")
                 send_message_list.extend(
-                    HeavyObject._get_on_message_list(on_message_list[i], get_obj_class, objects))
+                    cls._get_on_message_list(on_message_list[i], get_obj_class, objects))
                 send_message_list.append("break;")
                 send_message_list.append("}")  # end case
             send_message_list.append("default: return;")
             send_message_list.append("}")  # end switch
         send_message_list.append("}")  # end function
         return send_message_list
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
-        raise NotImplementedError("method get_C_process not implemented")
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        raise NotImplementedError("method get_C_init not implemented")
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         raise NotImplementedError("method get_C_onMessage not implemented")
 
     @classmethod
-    def _get_on_message_list(clazz, on_message_list, get_obj_class, objects):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        raise NotImplementedError("method get_C_process not implemented")
+
+    @classmethod
+    def get_table_data_decl(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        raise NotImplementedError("method get_table_data_decl not implemented")
+
+    @classmethod
+    def _get_on_message_list(cls, on_message_list: List, get_obj_class: Callable, objects: Dict) -> List:
         out_list = []
         for om in on_message_list:
             out_list.extend(
                 get_obj_class(objects[om["id"]]["type"]).get_C_onMessage(
                     objects[om["id"]]["type"],
                     om["id"],
                     om["inletIndex"],
                     objects[om["id"]]["args"]))
         return out_list
 
     @classmethod
-    def _c_buffer(clazz, buffer_dict):
+    def _c_buffer(cls, buffer_dict: Dict) -> str:
         """ Returns the C represenation of the given buffer.
         """
         if buffer_dict["type"] == "zero":
-            return HeavyObject.__C_BUFFER_DICT[buffer_dict["type"]]
+            return cls.__C_BUFFER_DICT[buffer_dict["type"]]
         else:
             return "{0}{1}".format(
-                HeavyObject.__C_BUFFER_DICT[buffer_dict["type"]],
+                cls.__C_BUFFER_DICT[buffer_dict["type"]],
                 buffer_dict["index"])
 
     @classmethod
-    def get_hash(clazz, x):
+    def get_hash(cls, x: Union[float, str]) -> int:
         """ Compute the message element hash used by msg_getHash().
         Returns a 32-bit integer.
         """
         if isinstance(x, float) or isinstance(x, int):
             # interpret the float bytes as an unsigned integer
             return unpack("@I", pack("@f", float(x)))[0]
         elif x == "bang":
@@ -160,11 +177,11 @@
             h = (h * m) & 0xFFFFFFFF
             h ^= h >> 15
             return h
         else:
             raise Exception("Message element hashes can only be computed for float and string types.")
 
     @classmethod
-    def get_hash_string(clazz, x):
+    def get_hash_string(cls, x: Union[float, str]) -> str:
         """ Returns the hash as a hex string.
         """
-        return f"0x{HeavyObject.get_hash(x):X}"
+        return f"0x{cls.get_hash(x):X}"
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/HeavyTable.py` & `hvcc-0.7.0/hvcc/generators/ir2c/HeavyTable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,71 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class HeavyTable(HeavyObject):
     """Outputs code for the table object.
     """
 
     c_struct = "HvTable"
     preamble = "hTable"
 
     @classmethod
-    def get_C_header_set(self):
+    def get_C_header_set(self) -> set:
         return {"HvTable.h"}
 
     @classmethod
-    def get_C_file_set(self):
+    def get_C_file_set(self) -> set:
         return {"HvTable.h", "HvTable.c"}
 
     @classmethod
-    def get_C_decl(clazz, obj_type, obj_id, args):
-        return [
-            f"{clazz.preamble}_{obj_id}_sendMessage(HeavyContextInterface *, int, const HvMessage *);"
-        ]
-
-    @classmethod
-    def get_table_data_decl(clazz, obj_type, obj_id, args):
+    def get_table_data_decl(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if len(args.get("values", [])) > 0:
             return [
                 "float hTable_{0}_data[{1}] = {{{2}}};".format(
                     obj_id,
                     len(args["values"]),
                     ", ".join([f"{float(v)}f" for v in args["values"]]))]
         else:
             return []
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if len(args.get("values", [])) > 0:
             return [
                 "hTable_initWithData(&hTable_{0}, {1}, hTable_{0}_data);".format(
                     obj_id,
                     len(args["values"]))]
         else:
             return [
                 "hTable_init(&hTable_{0}, {1});".format(
                     obj_id,
                     int(args.get("size", 256)))]  # 1KB default memory allocation
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return ["{0}_free(&{0}_{1});".format(
-            clazz.preamble,
+            cls.preamble,
             obj_id)]
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
-            "hTable_onMessage(_c, &Context(_c)->hTable_{0}, {1}, m, &hTable_{0}_sendMessage);".format(
-                obj_id,
-                inlet_index)
+            f"hTable_onMessage(_c, &Context(_c)->hTable_{obj_id}, {inlet_index}, m, &hTable_{obj_id}_sendMessage);"
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/PrettyfyC.py` & `hvcc-0.7.0/hvcc/generators/ir2c/PrettyfyC.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,33 +11,46 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
+from typing import List
 
 
 class PrettyfyC:
 
     @classmethod
-    def prettyfy_file(clazz, file_in, file_out, indent=0, step=2, delete_input_on_finish=False):
+    def prettyfy_file(
+        cls,
+        file_in: str,
+        file_out: str,
+        indent: int = 0,
+        step: int = 2,
+        delete_input_on_finish: bool = False
+    ) -> None:
         with open(file_in, "r") as f:
             with open(file_out, "w") as g:
                 for line in f:
                     indent -= line.count("}")
                     new_line = (" " * (step * indent)) + line
                     g.write(new_line + os.linesep)
                     indent += line.count("{")
 
         if delete_input_on_finish:
-            os.path.delete(file_in)
+            os.remove(file_in)
 
     @classmethod
-    def prettyfy_list(clazz, list_in, indent=0, step=2):
+    def prettyfy_list(
+        cls,
+        list_in: List,
+        indent: int = 0,
+        step: int = 2
+    ) -> List:
         g = []
         for line in list_in:
             indent -= line.count("}")
             new_line = (" " * (step * indent)) + line
             g.append(new_line)
             indent += line.count("{")
         return g
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalBiquad.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalBiquad.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,86 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalBiquad(HeavyObject):
     """Handles the biquad~ object.
     """
 
     c_struct = "SignalBiquad"
     preamble = "sBiquad"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvSignalBiquad.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvSignalBiquad.h", "HvSignalBiquad.c"}
 
     @classmethod
-    def get_C_def(clazz, obj_type, obj_id):
+    def get_C_def(cls, obj_type: str, obj_id: int) -> List[str]:
         if obj_type == "__biquad_k~f":
             return [f"SignalBiquad_k sBiquad_k_{obj_id};"]
         elif obj_type == "__biquad~f":
             return [f"SignalBiquad sBiquad_s_{obj_id};"]
         else:
             raise Exception()
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if obj_type == "__biquad_k~f":
             return ["sBiquad_k_init(&sBiquad_k_{0}, {1}f, {2}f, {3}f, {4}f, {5}f);".format(
                 obj_id,
                 float(args["ff0"]),
                 float(args["ff1"]),
                 float(args["ff2"]),
                 float(args["fb1"]),
                 float(args["fb2"]))]
         elif obj_type == "__biquad~f":
             return [f"sBiquad_init(&sBiquad_s_{obj_id});"]
         else:
             raise Exception()
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return ["sBiquad_k_onMessage(&Context(_c)->sBiquad_k_{0}, {1}, m);".format(
-            obj_id,
-            inlet_index)]
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
+        return [f"sBiquad_k_onMessage(&Context(_c)->sBiquad_k_{obj_id}, {inlet_index}, m);"]
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if obj_type == "__biquad_k~f":
             return [
                 "__hv_biquad_k_f(&sBiquad_k_{0}, VIf({1}), VOf({2}));".format(
                     process_dict["id"],
-                    HeavyObject._c_buffer(process_dict["inputBuffers"][0]),
-                    HeavyObject._c_buffer(process_dict["outputBuffers"][0])
+                    cls._c_buffer(process_dict["inputBuffers"][0]),
+                    cls._c_buffer(process_dict["outputBuffers"][0])
                 )]
         elif obj_type == "__biquad~f":
             return [
                 "__hv_biquad_f(&sBiquad_s_{0}, {1}, {2});".format(
                     process_dict["id"],
-                    ", ".join([f"VIf({HeavyObject._c_buffer(b)})" for b in process_dict["inputBuffers"]]),
-                    ", ".join([f"VOf({HeavyObject._c_buffer(b)})" for b in process_dict["outputBuffers"]])
+                    ", ".join([f"VIf({cls._c_buffer(b)})" for b in process_dict["inputBuffers"]]),
+                    ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
                 )]
+        else:
+            raise Exception(f"Incorrect obj_type {obj_type} for SignalBiquad")
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalCPole.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalCPole.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalCPole(HeavyObject):
     """Handles the __cpole~f object.
     """
 
     c_struct = "SignalCPole"
     preamble = "sCPole"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvSignalCPole.h", "HvSignalDel1.h", "HvMath.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {
             "HvSignalCPole.h", "HvSignalCPole.c",
             "HvSignalDel1.h", "HvSignalDel1.c",
             "HvMath.h"
         }
 
     @classmethod
-    def get_C_def(clazz, obj_type, obj_id):
-        return ["SignalCPole sCPole_{0};".format(obj_id)]
+    def get_C_def(cls, obj_type: str, obj_id: int) -> List[str]:
+        return [f"SignalCPole sCPole_{obj_id};"]
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return ["sCPole_init(&sCPole_{0});".format(obj_id)]
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [f"sCPole_init(&sCPole_{obj_id});"]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "__hv_cpole_f(&sCPole_{0}, VIf({1}), VIf({2}), VIf({3}), VIf({4}), VOf({5}), VOf({6}));".format(
                 process_dict["id"],
-                HeavyObject._c_buffer(process_dict["inputBuffers"][0]),
-                HeavyObject._c_buffer(process_dict["inputBuffers"][1]),
-                HeavyObject._c_buffer(process_dict["inputBuffers"][2]),
-                HeavyObject._c_buffer(process_dict["inputBuffers"][3]),
-                HeavyObject._c_buffer(process_dict["outputBuffers"][0]),
-                HeavyObject._c_buffer(process_dict["outputBuffers"][1]))]
+                cls._c_buffer(process_dict["inputBuffers"][0]),
+                cls._c_buffer(process_dict["inputBuffers"][1]),
+                cls._c_buffer(process_dict["inputBuffers"][2]),
+                cls._c_buffer(process_dict["inputBuffers"][3]),
+                cls._c_buffer(process_dict["outputBuffers"][0]),
+                cls._c_buffer(process_dict["outputBuffers"][1]))]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalConvolution.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlPack.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class SignalConvolution(HeavyObject):
+class ControlPack(HeavyObject):
+    """Prints the first value in a message to the console"""
 
-    c_struct = "SignalConvolution"
-    preamble = "sConv"
+    c_struct = "ControlPack"
+    preamble = "cPack"
 
     @classmethod
-    def get_C_header_set(clazz):
-        return {"HvSignalConvolution.h"}
+    def get_C_header_set(cls) -> set:
+        return {"HvControlPack.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvSignalConvolution.h", "HvSignalConvolution.c"}
+    def get_C_file_set(cls) -> set:
+        return {"HvControlPack.h", "HvControlPack.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "sConv_init(&sConv_{0}, &hTable_{1}, {2});".format(
+            "cPack_init(&cPack_{0}, {1}, {2});".format(
                 obj_id,
-                args["table_id"],
-                int(args["size"]))
+                len(args["values"]),
+                ", ".join(["{0}f".format(float(x)) for x in args["values"]]))
         ]
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
-            "sConv_onMessage(_c, &Context(_c)->sConv_{0}, {1}, m, NULL);".format(
+            "cPack_onMessage(_c, &Context(_c)->cPack_{0}, {1}, m, &cPack_{0}_sendMessage);".format(
                 obj_id,
                 inlet_index)
         ]
-
-    @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
-        return [
-            "__hv_conv_f(&sConv_{0}, VIf({1}), VOf({2}));".format(
-                process_dict["id"],
-                HeavyObject._c_buffer(process_dict["inputBuffers"][0]),
-                HeavyObject._c_buffer(process_dict["outputBuffers"][0])
-            )
-        ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalLine.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalRPole.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class SignalLine(HeavyObject):
+class SignalRPole(HeavyObject):
+    """Handles the __rpole~f object.
+    """
 
-    c_struct = "SignalLine"
-    preamble = "sLine"
+    c_struct = "SignalRpole"
+    preamble = "sRPole"
 
     @classmethod
-    def get_C_header_set(clazz):
-        return {"HvSignalLine.h"}
+    def get_C_header_set(cls) -> set:
+        return {"HvSignalRPole.h", "HvSignalDel1.h", "HvMath.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvSignalLine.h", "HvSignalLine.c"}
+    def get_C_file_set(cls) -> set:
+        return {
+            "HvSignalRPole.h", "HvSignalRPole.c",
+            "HvSignalDel1.h", "HvSignalDel1.c",
+            "HvMath.h"
+        }
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return [
-            f"sLine_init(&sLine_{obj_id});"
-        ]
+    def get_C_def(cls, obj_type: str, obj_id: int) -> List[str]:
+        return [f"SignalRPole sRPole_{obj_id};"]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
-        return []  # nothing to free
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return [f"sRPole_init(&sRPole_{obj_id});"]
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [
-            f"sLine_onMessage(_c, &Context(_c)->sLine_{obj_id}, {inlet_index}, m, NULL);"
-        ]
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "__hv_line_f(&sLine_{0}, VOf({1}));".format(
+            "__hv_rpole_f(&sRPole_{0}, VIf({1}), VIf({2}), VOf({3}));".format(
                 process_dict["id"],
-                HeavyObject._c_buffer(process_dict["outputBuffers"][0])
-            )
-        ]
+                cls._c_buffer(process_dict["inputBuffers"][0]),
+                cls._c_buffer(process_dict["inputBuffers"][1]),
+                cls._c_buffer(process_dict["outputBuffers"][0]))]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalLorenz.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalLorenz.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalLorenz(HeavyObject):
 
     c_struct = "SignalLorenz"
     preamble = "sLorenz"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvSignalLorenz.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvSignalLorenz.h", "HvSignalLorenz.c", "HvMath.h"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "sLorenz_init(&sLorenz_{0}, {1}f, {2}f, {3}f);".format(
                 obj_id,
                 float(args["x"]),
                 float(args["y"]),
                 float(args["z"]))
         ]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []  # nothing to free
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
             "sLorenz_onMessage(_c, &Context(_c)->sLorenz_{0}, {1}, m);".format(
                 obj_id,
                 inlet_index)
         ]
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "__hv_lorenz_f(&sLorenz_{0}, {1}, {2});".format(
                 process_dict["id"],
-                ", ".join(["VIf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["inputBuffers"]]),
-                ", ".join(["VOf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["outputBuffers"]])
+                ", ".join(["VIf({0})".format(cls._c_buffer(b)) for b in process_dict["inputBuffers"]]),
+                ", ".join(["VOf({0})".format(cls._c_buffer(b)) for b in process_dict["outputBuffers"]])
             )
         ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalMath.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalMath.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalMath(HeavyObject):
     """Handles the math objects.
     """
 
@@ -60,41 +63,42 @@
         "__gt~i": "__hv_gt_i",
         "__gte~f": "__hv_gte_f",
         "__gte~i": "__hv_gte_i",
         "__lt~f": "__hv_lt_f",
         "__lt~i": "__hv_lt_i",
         "__lte~f": "__hv_lte_f",
         "__lte~i": "__hv_lte_i",
+        "__eq~f": "__hv_eq_f",
         "__neq~f": "__hv_neq_f",
         "__fma~f": "__hv_fma_f",
         "__fms~f": "__hv_fms_f",
         "__floor~f": "__hv_floor_f",
         "__ceil~f": "__hv_ceil_f",
         "__cast~fi": "__hv_cast_fi",
         "__cast~if": "__hv_cast_if",
         "__and~f": "__hv_and_f",  # binary and
         "__andnot~f": "__hv_andnot_f",
         "__or~f": "__hv_or_f",  # binary or
     }
 
     @classmethod
-    def handles_type(clazz, obj_type):
+    def handles_type(cls, obj_type: str) -> bool:
         """Returns true if the object type can be handled by this class
         """
-        return obj_type in SignalMath.__OPERATION_DICT
+        return obj_type in cls.__OPERATION_DICT
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvMath.h"}
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "{0}({1}, {2});".format(
-                SignalMath.__OPERATION_DICT[obj_type],
+                cls.__OPERATION_DICT[obj_type],
                 ", ".join(["VI{0}({1})".format(
                     "i" if b["type"] == "~i>" else "f",
-                    HeavyObject._c_buffer(b)) for b in process_dict["inputBuffers"]]),
+                    cls._c_buffer(b)) for b in process_dict["inputBuffers"]]),
                 ", ".join(["VO{0}({1})".format(
                     "i" if b["type"] == "~i>" else "f",
-                    HeavyObject._c_buffer(b)) for b in process_dict["outputBuffers"]])
+                    cls._c_buffer(b)) for b in process_dict["outputBuffers"]])
             )]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalPhasor.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalPhasor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,75 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalPhasor(HeavyObject):
 
     c_struct = "SignalPhasor"
     preamble = "sPhasor"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvSignalPhasor.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvSignalPhasor.h", "HvSignalPhasor.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if obj_type == "__phasor~f":
-            return [
-                "sPhasor_init(&sPhasor_{0}, sampleRate);".format(obj_id)
-            ]
+            return [f"sPhasor_init(&sPhasor_{obj_id}, sampleRate);"]
         elif obj_type == "__phasor_k~f":
-            return [
-                "sPhasor_k_init(&sPhasor_{0}, {1}f, sampleRate);".format(
-                    obj_id,
-                    args["frequency"])
-            ]
+            return [f"sPhasor_k_init(&sPhasor_{obj_id}, {args['frequency']}f, sampleRate);"]
         else:
             raise Exception()
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         if obj_type == "__phasor~f":
-            return [
-                "sPhasor_onMessage(_c, &Context(_c)->sPhasor_{0}, {1}, m);".format(
-                    obj_id,
-                    inlet_index)]
+            return [f"sPhasor_onMessage(_c, &Context(_c)->sPhasor_{obj_id}, {inlet_index}, m);"]
         elif obj_type == "__phasor_k~f":
-            return [
-                "sPhasor_k_onMessage(_c, &Context(_c)->sPhasor_{0}, {1}, m);".format(
-                    obj_id,
-                    inlet_index)]
+            return [f"sPhasor_k_onMessage(_c, &Context(_c)->sPhasor_{obj_id}, {inlet_index}, m);"]
         else:
             raise Exception()
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if obj_type == "__phasor~f":
             return [
                 "__hv_phasor_f(&sPhasor_{0}, VIf({1}), VOf({2}));".format(
                     process_dict["id"],
-                    HeavyObject._c_buffer(process_dict["inputBuffers"][0]),
-                    HeavyObject._c_buffer(process_dict["outputBuffers"][0])
+                    cls._c_buffer(process_dict["inputBuffers"][0]),
+                    cls._c_buffer(process_dict["outputBuffers"][0])
                 )
             ]
         elif obj_type == "__phasor_k~f":
             return [
                 "__hv_phasor_k_f(&sPhasor_{0}, VOf({1}));".format(
                     process_dict["id"],
-                    HeavyObject._c_buffer(process_dict["outputBuffers"][0])
+                    cls._c_buffer(process_dict["outputBuffers"][0])
                 )
             ]
         else:
-            raise Exception("Unknown object type \"{0}\".".format(obj_type))
+            raise Exception(f"Unknown object type \"{obj_type}\".")
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalSample.py` & `hvcc-0.7.0/hvcc/core/hv2ir/HLangSlice.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,43 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyObject import HeavyObject
+from typing import Optional, Dict
 
-
-class SignalSample(HeavyObject):
-
-    c_struct = "SignalSample"
-    preamble = "sSample"
-
-    @classmethod
-    def get_C_header_set(clazz):
-        return {"HvSignalSample.h"}
-
-    @classmethod
-    def get_C_file_set(clazz):
-        return {"HvSignalSample.h", "HvSignalSample.c"}
-
-    @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
-        return [
-            "sSample_init(&sSample_{0});".format(obj_id)
-        ]
-
-    @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
-        return []  # nothing to free
-
-    @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return [
-            "{0}_onMessage(_c, &Context(_c)->{0}_{1}, {2}, m);".format(
-                clazz.preamble,
-                obj_id,
-                inlet_index)
-        ]
-
-    @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
-        return [
-            "__hv_sample_f(this, &sSample_{0}, VIf({1}), &{2}_{0}_sendMessage);".format(
-                process_dict["id"],
-                HeavyObject._c_buffer(process_dict["inputBuffers"][0]),
-                clazz.preamble
-            )
-        ]
+from .HeavyLangObject import HeavyLangObject
+from .HeavyIrObject import HeavyIrObject
+from .HeavyGraph import HeavyGraph
+
+
+class HLangSlice(HeavyLangObject):
+    """ Handles the HeavyLang "slice" object.
+    """
+
+    def __init__(
+        self,
+        obj_type: str,
+        args: Dict,
+        graph: 'HeavyGraph',
+        annotations: Optional[Dict] = None
+    ) -> None:
+        assert obj_type == "slice"
+        super().__init__(obj_type, args, graph,
+                         num_inlets=3,
+                         num_outlets=2,
+                         annotations=annotations)
+
+    def reduce(self) -> tuple:
+        x = HeavyIrObject("__slice", self.args)
+        return ({x}, self.get_connection_move_list(x))
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalTabhead.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalEnvelope.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .HeavyObject import HeavyObject
+from typing import Dict, List
 
+from .HeavyObject import HeavyObject
 
-class SignalTabhead(HeavyObject):
-    """Handles __tabhead~f
-    """
 
-    c_struct = "SignalTabhead"
-    preamble = "sTabhead"
+class SignalEnvelope(HeavyObject):
 
-    @classmethod
-    def get_C_header_set(clazz):
-        return {"HvSignalTabread.h"}
+    c_struct = "SignalEnvelope"
+    preamble = "sEnv"
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvSignalTabread.h", "HvSignalTabread.c"}
+    def get_C_header_set(cls) -> set:
+        return {"HvSignalEnvelope.h"}
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
-        return []
+    def get_C_file_set(cls) -> set:
+        return {"HvSignalEnvelope.h", "HvSignalEnvelope.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "sTabhead_init(&sTabhead_{0}, &hTable_{1});".format(
+            "sEnv_init(&sEnv_{0}, {1}, {2});".format(
                 obj_id,
-                args["table_id"])]
-
-    @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
-        return []  # TODO(mhroth): deal with this later
+                int(args["windowSize"]),
+                int(args["period"]))
+        ]
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "__hv_tabhead_f(&sTabhead_{0}, {1});".format(
+            "sEnv_process(this, &sEnv_{0}, VIf({1}), &sEnv_{0}_sendMessage);".format(
                 process_dict["id"],
-                ", ".join(["VOf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["outputBuffers"]])
-            )]
+                cls._c_buffer(process_dict["inputBuffers"][0])
+            )
+        ]
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalTabread.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalTabread.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalTabread(HeavyObject):
     """Handles __tabread~if, __tabread~f, __tabreadu~f
     """
 
     c_struct = "SignalTabread"
     preamble = "sTabread"
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvSignalTabread.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvSignalTabread.h", "HvSignalTabread.c"}
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
             "sTabread_init(&sTabread_{0}, &hTable_{1}, {2});".format(
                 obj_id,
                 args["table_id"],
                 "true" if obj_type == "__tabread~f" else "false")]
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         if obj_type in ["__tabread~f", "__tabreadu~f"]:
             return [
                 "sTabread_onMessage(_c, &Context(_c)->sTabread_{0}, {1}, m, &sTabread_{0}_sendMessage);".format(
                     obj_id,
                     inlet_index)]
         else:  # "__tabread~if"
-            return [
-                "sTabread_onMessage(_c, &Context(_c)->sTabread_{0}, {1}, m, NULL);".format(
-                    obj_id,
-                    inlet_index)]
+            return [f"sTabread_onMessage(_c, &Context(_c)->sTabread_{obj_id}, {inlet_index}, m, NULL);"]
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         if obj_type == "__tabread~if":
             return [
                 "__hv_tabread_if(&sTabread_{0}, {1}, {2});".format(
                     process_dict["id"],
-                    ", ".join(["VIi({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["inputBuffers"]]),
-                    ", ".join(["VOf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["outputBuffers"]])
+                    ", ".join([f"VIi({cls._c_buffer(b)})" for b in process_dict["inputBuffers"]]),
+                    ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
                 )]
         elif obj_type == "__tabread~f":
             return [
                 "__hv_tabread_f(&sTabread_{0}, {1});".format(
                     process_dict["id"],
-                    ", ".join(["VOf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["outputBuffers"]])
+                    ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
                 )]
         elif obj_type == "__tabreadu~f":
             return [
                 "__hv_tabreadu_f(&sTabread_{0}, {1});".format(
                     process_dict["id"],
-                    ", ".join(["VOf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["outputBuffers"]])
+                    ", ".join([f"VOf({cls._c_buffer(b)})" for b in process_dict["outputBuffers"]])
                 )]
         else:
             raise Exception()
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalTabwrite.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ControlTabwrite.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,54 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
-class SignalTabwrite(HeavyObject):
-    """Handles __tabwrite~f
-    """
+class ControlTabwrite(HeavyObject):
 
-    c_struct = "SignalTabwrite"
-    preamble = "sTabwrite"
+    c_struct = "ControlTabwrite"
+    preamble = "cTabwrite"
 
     @classmethod
-    def get_C_header_set(clazz):
-        return {"HvSignalTabwrite.h"}
+    def get_C_header_set(cls) -> set:
+        return {"HvControlTabwrite.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
-        return {"HvSignalTabwrite.h", "HvSignalTabwrite.c"}
+    def get_C_file_set(cls) -> set:
+        return {"HvControlTabwrite.h", "HvControlTabwrite.c"}
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
-        return []
-
-    @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return [
-            "sTabwrite_init(&sTabwrite_{0}, &hTable_{1});".format(
+            "cTabwrite_init(&cTabwrite_{0}, &hTable_{1}); // {2}".format(
                 obj_id,
-                args["table_id"])]
+                args["table_id"],
+                args["table"])
+        ]
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
+        return []
+
+    @classmethod
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         return [
-            "sTabwrite_onMessage(_c, &Context(_c)->sTabwrite_{0}, {1}, m, NULL);".format(
+            "cTabwrite_onMessage(_c, &Context(_c)->cTabwrite_{0}, {1}, m, &cTabwrite_{0}_sendMessage);".format(
                 obj_id,
                 inlet_index)
         ]
-
-    @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
-        if obj_type == "__tabwrite~f":
-            return [
-                "__hv_tabwrite_f(&sTabwrite_{0}, {1});".format(
-                    process_dict["id"],
-                    ", ".join(["VIf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["inputBuffers"]])
-                )]
-        elif obj_type == "__tabwrite_stoppable~f":
-            return [
-                "__hv_tabwrite_stoppable_f(&sTabwrite_{0}, {1});".format(
-                    process_dict["id"],
-                    ", ".join(["VIf({0})".format(HeavyObject._c_buffer(b)) for b in process_dict["inputBuffers"]])
-                )]
-        else:
-            raise Exception()
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/SignalVar.py` & `hvcc-0.7.0/hvcc/generators/ir2c/SignalVar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, List
+
 from .HeavyObject import HeavyObject
 
 
 class SignalVar(HeavyObject):
 
     __OPERATION_DICT = {
         "__var~f": "sVarf",
@@ -26,89 +29,91 @@
         "__varwrite~f": "__hv_varwrite_f",
         "__varwrite~i": "__hv_varwrite_i",
         "__varread~f": "__hv_varread_f",
         "__varread~i": "__hv_varread_i"
     }
 
     @classmethod
-    def get_c_struct(clazz, obj_type):
+    def get_C_struct(cls, obj_type: str = "") -> str:
         if obj_type == "__var~f":
             return "SignalVarf"
         elif obj_type == "__var~i":
             return "SignalVari"
         else:
             raise Exception()
 
     @classmethod
-    def get_preamble(clazz, obj_type):
-        return SignalVar.__OPERATION_DICT[obj_type]
+    def get_preamble(cls, obj_type: str) -> str:
+        return cls.__OPERATION_DICT[obj_type]
 
     @classmethod
-    def handles_type(clazz, obj_type):
+    def handles_type(cls, obj_type: str) -> bool:
         """Returns true if the object type can be handled by this class
         """
-        return obj_type in SignalVar.__OPERATION_DICT
+        return obj_type in cls.__OPERATION_DICT
 
     @classmethod
-    def get_C_header_set(clazz):
+    def get_C_header_set(cls) -> set:
         return {"HvSignalVar.h"}
 
     @classmethod
-    def get_C_file_set(clazz):
+    def get_C_file_set(cls) -> set:
         return {"HvSignalVar.h", "HvSignalVar.c"}
 
     @classmethod
-    def get_C_init(clazz, obj_type, obj_id, args):
+    def get_C_init(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         assert obj_type in ["__var~f", "__var~i"], obj_type
         return [
             "{0}_init(&{0}_{1}, {2}, {3}, {4});".format(
                 SignalVar.__OPERATION_DICT[obj_type],
                 obj_id,
-                "{0}f".format(float(args["k"])) if obj_type.endswith("f") else int(args["k"]),
-                "{0}f".format(float(args["step"])) if obj_type.endswith("f") else int(args["step"]),
+                f"{float(args['k'])}f" if obj_type.endswith("f") else int(args["k"]),
+                f"{float(args['step'])}f" if obj_type.endswith("f") else int(args["step"]),
                 "true" if args["reverse"] else "false")]
 
     @classmethod
-    def get_C_free(clazz, obj_type, obj_id, args):
+    def get_C_free(cls, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         return []
 
     @classmethod
-    def get_C_onMessage(clazz, obj_type, obj_id, inlet_index, args):
+    def get_C_onMessage(cls, obj_type: str, obj_id: int, inlet_index: int, args: Dict) -> List[str]:
         assert obj_type in ["__var~f", "__var~i"]
         return [
             "{0}_onMessage(_c, &Context(_c)->{0}_{1}, m);".format(
-                SignalVar.__OPERATION_DICT[obj_type],
+                cls.__OPERATION_DICT[obj_type],
                 obj_id)]
 
     @classmethod
-    def get_C_process(clazz, process_dict, obj_type, obj_id, args):
+    def get_C_process(cls, process_dict: Dict, obj_type: str, obj_id: int, args: Dict) -> List[str]:
         fmt = obj_type[-1]
         if obj_type in ["__var~f", "__var~i"]:
             # NOTE(mhroth): signal rate variables do not process anything
             return []
         elif obj_type in ["__varwrite~f", "__varwrite~i"]:
             return [
                 "__hv_varwrite_{1}(&sVar{1}_{0}, VI{1}({2}));".format(
                     args["var_id"],
                     fmt,
-                    HeavyObject._c_buffer(process_dict["inputBuffers"][0])
+                    cls._c_buffer(process_dict["inputBuffers"][0])
                 )]
         elif obj_type in ["__var_k~f", "__var_k~i"]:
             if args["k"] == 0.0 and args.get("step", 0.0) == 0.0:
                 return ["__hv_zero_{0}(VO{0}({1}));".format(
                     fmt,
-                    HeavyObject._c_buffer(process_dict["outputBuffers"][0]))]
+                    cls._c_buffer(process_dict["outputBuffers"][0]))]
             else:
                 c = [float(args["k"] + i * args.get("step", 0.0)) for i in range(8)]
                 cx = ", ".join(["{0}f".format(f) for f in c]) if fmt == "f" else ", ".join([str(int(i)) for i in c])
                 return ["__hv_var_k_{0}{3}(VO{0}({1}), {2});".format(
                     fmt,
-                    HeavyObject._c_buffer(process_dict["outputBuffers"][0]),
+                    cls._c_buffer(process_dict["outputBuffers"][0]),
                     cx,
                     "_r" if args.get("reverse", False) else "")]
         elif obj_type in ["__varread~f", "__varread~i"]:
             return [
                 "__hv_varread_{1}(&sVar{1}_{0}, VO{1}({2}));".format(
                     args["var_id"],
                     fmt,
-                    HeavyObject._c_buffer(process_dict["outputBuffers"][0])
+                    cls._c_buffer(process_dict["outputBuffers"][0])
                 )]
+        else:
+            raise Exception("")
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ir2c.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ir2c.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,22 +11,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
-from collections import Counter
-from collections import OrderedDict
 import jinja2
 import json
 import os
 import shutil
 import time
 
+from collections import Counter
+from collections import OrderedDict
+from typing import Dict, List, Optional, Type, Union
+
 from hvcc.generators.ir2c.PrettyfyC import PrettyfyC
 from hvcc.generators.copyright import copyright_manager
 
 from hvcc.generators.ir2c.ControlBinop import ControlBinop
 from hvcc.generators.ir2c.ControlCast import ControlCast
 from hvcc.generators.ir2c.ControlDelay import ControlDelay
 from hvcc.generators.ir2c.ControlIf import ControlIf
@@ -116,54 +119,61 @@
         "HvMessagePool.h", "HvMessagePool.c",
         "HvTable.h", "HvTable.c",
         "HvMessage.h", "HvMessage.c",
         "HvLightPipe.h", "HvLightPipe.c"
     }
 
     @classmethod
-    def filter_hvhash(clazz, x):
+    def filter_hvhash(cls, x: Union[float, str]) -> str:
         """ Return the hash string of an object.
         """
         return HeavyObject.get_hash_string(x)
 
     @classmethod
-    def filter_extern(clazz, d):
+    def filter_extern(cls, d: Dict) -> Dict:
         """ Return a dictionary of objects that are externed.
         """
         return {k: v for k, v in d.items() if v["extern"]}
 
     @classmethod
-    def get_class(clazz, obj_type):
+    def get_class(cls, obj_type: str) -> Type[HeavyObject]:
         if SignalMath.handles_type(obj_type):
             return SignalMath
         elif ControlBinop.handles_type(obj_type):
             return ControlBinop
         elif ControlUnop.handles_type(obj_type):
             return ControlUnop
         elif SignalVar.handles_type(obj_type):
             return SignalVar
         elif obj_type in ir2c.__OBJECT_CLASS_DICT:
             return ir2c.__OBJECT_CLASS_DICT[obj_type]
         else:
-            raise Exception("No class found for object type \"{0}\".".format(obj_type))
+            raise Exception(f"No class found for object type \"{obj_type}\".")
 
     @classmethod
-    def compile(clazz, hv_ir_path, static_dir, output_dir, externs, copyright=None):
+    def compile(
+        cls,
+        hv_ir_path: str,
+        static_dir: str,
+        output_dir: str,
+        externs: Dict,
+        copyright: Optional[str] = None
+    ) -> Dict:
         """ Compiles a HeavyIR file into a C.
             Returns a tuple of compile time in seconds, a notification dictionary,
             and a HeavyIR object counter.
         """
 
         # keep track of the total compile time
         tick = time.time()
 
         # establish the jinja environment
         env = jinja2.Environment()
-        env.filters["hvhash"] = ir2c.filter_hvhash
-        env.filters["extern"] = ir2c.filter_extern
+        env.filters["hvhash"] = cls.filter_hvhash
+        env.filters["extern"] = cls.filter_extern
         env.loader = jinja2.FileSystemLoader(
             os.path.join(os.path.dirname(__file__), "templates"))
 
         # read the hv.ir.json file
         with open(hv_ir_path, "r") as f:
             ir = json.load(f)
 
@@ -178,15 +188,15 @@
         include_set = set([x for o in ir["objects"].values() for x in ir2c.get_class(o["type"]).get_C_header_set()])
 
         # generate set of files to add to project
         file_set = set([x for o in ir["objects"].values() for x in ir2c.get_class(o["type"]).get_C_file_set()])
         file_set.update(ir2c.__BASE_FILE_SET)
 
         # generate object definition and initialisation list
-        init_list = []
+        init_list: List = []
         free_list = []
         def_list = []
         decl_list = []
         for obj_id in ir["init"]["order"]:
             o = ir["objects"][obj_id]
             obj_class = ir2c.get_class(o["type"])
             init_list.extend(obj_class.get_C_init(o["type"], obj_id, o["args"]))
@@ -204,25 +214,25 @@
                 x["onMessage"],
                 ir2c.get_class,
                 ir["objects"])
             impl_list.append("\n".join(PrettyfyC.prettyfy_list(impl)))
             decl_list.extend(obj_class.get_C_decl(o["type"], obj_id, o["args"]))
 
         # generate static table data initialisers
-        table_data_list = []
+        table_data_list: List = []
         for k, v in ir["tables"].items():
             o = ir["objects"][v["id"]]
             obj_class = ir2c.get_class(o["type"])
             table_data_list.extend(obj_class.get_table_data_decl(
                 o["type"],
                 v["id"],
                 o["args"]))
 
         # generate the list of functions to process
-        process_list = []
+        process_list: List = []
         for x in ir["signal"]["processOrder"]:
             obj_id = x["id"]
             o = ir["objects"][obj_id]
             process_list.extend(ir2c.get_class(o["type"]).get_C_process(
                 x,
                 o["type"],
                 obj_id,
@@ -273,16 +283,16 @@
                 name=name,
                 copyright=copyright,
                 externs=externs))
 
         # copy static files to output directory
         for f in file_set:
             shutil.copy2(
-                src=os.path.join(static_dir, f),
-                dst=os.path.join(output_dir, f))
+                src=os.path.join(static_dir, str(f)),
+                dst=os.path.join(output_dir, str(f)))
 
         # generate HeavyIR object counter
         ir_counter = Counter([obj["type"] for obj in ir["objects"].values()])
 
         return {
             "stage": "ir2c",
             "notifs": {
@@ -295,15 +305,15 @@
             "out_dir": output_dir,
             "out_file": "",
             "compile_time": (time.time() - tick),
             "obj_counter": ir_counter
         }
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         description="A Heavy.IR to C-language translator.")
     parser.add_argument(
         "hv_ir_path",
         help="The path to the Heavy.IR file to read.")
     parser.add_argument(
         "--static_dir",
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/ir2c_perf.py` & `hvcc-0.7.0/hvcc/generators/ir2c/ir2c_perf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,31 +11,32 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
-from collections import Counter
-from collections import defaultdict
 import json
 import os
+from collections import Counter
+from collections import defaultdict
+from typing import Dict
 
 
 class ir2c_perf:
 
     @classmethod
-    def perf(clazz, ir, blocksize=512, mhz=1000, verbose=False):
+    def perf(cls, ir: Dict, blocksize: int = 512, mhz: int = 1000, verbose: bool = False) -> Dict:
         # read the hv.ir.json file
         with open(os.path.join(os.path.dirname(__file__), "../../core/json/heavy.ir.json"), "r") as f:
             HEAVY_IR_JSON = json.load(f)
 
-        objects = Counter()
-        perf = Counter()
-        per_object_perf = defaultdict(Counter)
+        objects: Counter = Counter()
+        perf: Counter = Counter()
+        per_object_perf: Dict = defaultdict(Counter)
         for o in ir["signal"]["processOrder"]:
             obj_id = o["id"]
             obj_type = ir["objects"][obj_id]["type"]
             if obj_type in HEAVY_IR_JSON:
                 objects[obj_type] += 1
                 if "perf" in HEAVY_IR_JSON[obj_type]:
                     c = Counter(HEAVY_IR_JSON[obj_type]["perf"])
@@ -70,15 +72,15 @@
             # items.sort(key=lambda o: o[1]["avx"], reverse=True)
             for k, v in items:
                 print("{2:>2.2g}%  {3:<5} {0:<16} {1}".format(k, v, int(100.0 * v["avx"] / perf["avx"]), objects[k]))
 
         return per_object_perf
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         description="A Heavy.IR to C-language translator.")
     parser.add_argument(
         "hv_ir_path",
         help="The path to the Heavy.IR file to read.")
     parser.add_argument("--mhz", default=1000, type=float, help="the CPU clock frequency in MHz")
     parser.add_argument("--blocksize", default=64, type=int, help="the number of frames per block")
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HeavyContext.cpp` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HeavyContext.hpp` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContext.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HeavyContextInterface.hpp` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HeavyContextInterface.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlBinop.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlBinop.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlBinop.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlCast.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlCast.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlCast.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlDelay.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlDelay.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlDelay.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlIf.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlIf.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlIf.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPack.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPack.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPack.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPrint.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlPrint.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlPrint.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlRandom.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlRandom.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlRandom.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSlice.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSlice.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSlice.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSystem.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlSystem.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlSystem.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabhead.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabhead.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabhead.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabread.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabread.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabread.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabwrite.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlTabwrite.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlTabwrite.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlUnop.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlUnop.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlUnop.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlVar.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvControlVar.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvControlVar.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvHeavy.cpp` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvHeavy.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavy.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvHeavyInternal.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvHeavyInternal.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvLightPipe.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvLightPipe.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvLightPipe.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMath.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMath.h`

 * *Files 1% similar despite different names*

```diff
@@ -611,14 +611,26 @@
 #elif HV_SIMD_NEON
   *bOut = vreinterpretq_f32_u32(vcleq_f32(bIn0, bIn1));
 #else // HV_SIMD_NONE
   *bOut = (bIn0 <= bIn1) ? 1.0f : 0.0f;
 #endif
 }
 
+static inline void __hv_eq_f(hv_bInf_t bIn0, hv_bInf_t bIn1, hv_bOutf_t bOut) {
+#if HV_SIMD_AVX
+  *bOut = _mm256_cmp_ps(bIn0, bIn1, _CMP_EQ_OQ);
+#elif HV_SIMD_SSE
+  *bOut = _mm_cmpeq_ps(bIn0, bIn1);
+#elif HV_SIMD_NEON
+  *bOut = vreinterpretq_f32_u32(vceqq_f32(bIn0, bIn1));
+#else // HV_SIMD_NONE
+  *bOut = (bIn0 == bIn1) ? 1.0f : 0.0f;
+#endif
+}
+
 static inline void __hv_neq_f(hv_bInf_t bIn0, hv_bInf_t bIn1, hv_bOutf_t bOut) {
 #if HV_SIMD_AVX
   *bOut = _mm256_cmp_ps(bIn0, bIn1, _CMP_NEQ_OQ);
 #elif HV_SIMD_SSE
   *bOut = _mm_cmpneq_ps(bIn0, bIn1);
 #elif HV_SIMD_NEON
   *bOut = vreinterpretq_f32_u32(vmvnq_u32(vceqq_f32(bIn0, bIn1)));
```

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessage.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessage.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessage.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessagePool.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessagePool.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessagePool.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessageQueue.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvMessageQueue.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvMessageQueue.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalBiquad.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalBiquad.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalBiquad.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalCPole.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalCPole.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalCPole.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalConvolution.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalConvolution.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalConvolution.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalDel1.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalDel1.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalDel1.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalEnvelope.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalEnvelope.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalEnvelope.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLine.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLine.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLine.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLorenz.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalLorenz.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalLorenz.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalPhasor.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalPhasor.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalPhasor.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalRPole.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalRPole.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalRPole.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSamphold.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSamphold.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSamphold.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSample.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalSample.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalSample.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabread.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabread.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabread.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabwrite.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalTabwrite.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalTabwrite.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalVar.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvSignalVar.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvSignalVar.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvTable.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvTable.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvTable.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvUtils.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/HvUtils.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/HvUtils.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/cpuid.c` & `hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/static/cpuid.h` & `hvcc-0.7.0/hvcc/generators/ir2c/static/cpuid.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/templates/Heavy_NAME.cpp` & `hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.cpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/templates/Heavy_NAME.h` & `hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/ir2c/templates/Heavy_NAME.hpp` & `hvcc-0.7.0/hvcc/generators/ir2c/templates/Heavy_NAME.hpp`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/vs2015/Heavy/Heavy.sln` & `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.sln`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/vs2015/Heavy/Heavy.vcxproj` & `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters` & `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/Heavy.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/vs2015/Heavy/main.c` & `hvcc-0.7.0/hvcc/generators/vs2015/Heavy/main.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy/main.c` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy/main.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/AudioEngine.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Base.lproj/MainMenu.xib`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Heavy_OSX-Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Images.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/MainViewController.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/MainViewController.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/MainViewController.xib`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/Views/nuklear/nuklear_glfw_gl3.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/main.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/main.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_OSX/tinywav/tinywav.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/LaunchScreen.xib`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.m`

 * *Files 17% similar despite different names*

```diff
@@ -11,20 +11,26 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
 
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#import <Foundation/Foundation.h>
+#import "ViewController.h"
 
-@interface HeavyAudio : NSObject
+@interface ViewController ()
 
-- (void)initialiseAudioSession;
-- (void)initialiseAudioUnit;
+@end
 
-- (void)play;
-- (void)pause;
+@implementation ViewController
 
-- (void)overrideOutputToSpeaker:(BOOL)shouldOverride;
+- (void)viewDidLoad {
+  [super viewDidLoad];
+  // Do any additional setup after loading the view, typically from a nib.
+}
+
+- (void)didReceiveMemoryWarning {
+  [super didReceiveMemoryWarning];
+  // Dispose of any resources that can be recreated.
+}
 
 @end
```

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/HeavyAudio.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Images.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/Info.plist` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/Info.plist`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.c`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/TPCircularBuffer.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/ViewController.h` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/ViewController.h`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/generators/xcode/Heavy_iOS/main.m` & `hvcc-0.7.0/hvcc/generators/xcode/Heavy_iOS/main.m`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/HeavyGraph.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyGraph.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,26 +12,29 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import os
+from typing import Optional, List, Dict
 
 from .PdObject import PdObject
 from .HeavyObject import HeavyObject
 
 
 class HeavyGraph(PdObject):
-    def __init__(self, hv_path, obj_args=None, pos_x=0, pos_y=0):
-        PdObject.__init__(
-            self,
-            os.path.basename(hv_path).split(".")[0],
-            obj_args,
-            pos_x, pos_y)
+    def __init__(
+        self,
+        hv_path: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        super().__init__(os.path.basename(hv_path).split(".")[0], obj_args, pos_x, pos_y)
 
         # read the heavy graph
         with open(hv_path, "r") as f:
             self.hv_json = json.load(f)
 
         # parse the heavy data structure to determine the outlet connection type
         outlets = [o for o in self.hv_json["objects"].values() if o["type"] == "outlet"]
@@ -62,12 +66,12 @@
                         o["args"][k] = arg_value
 
         # reset all arguments, as they have all been resolved
         # any required arguments would break hv2ir as they will no longer
         # be supplied (because they are resolved)
         self.hv_json["args"] = []
 
-    def get_outlet_connection_type(self, outlet_index):
+    def get_outlet_connection_type(self, outlet_index: int) -> str:
         return self.__outlet_connection_types[outlet_index]
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return self.hv_json
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/HeavyObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/HeavyObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,50 +13,58 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import decimal
 import json
 import importlib_resources
+from typing import Optional, List, Dict, Any
 
+from .Connection import Connection
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
 class HeavyObject(PdObject):
 
     heavy_lang_json = importlib_resources.files('hvcc') / 'core/json/heavy.lang.json'
     with open(heavy_lang_json, "r") as f:
         __HEAVY_LANG_OBJS = json.load(f)
 
     heavy_ir_json = importlib_resources.files('hvcc') / 'core/json/heavy.ir.json'
     with open(heavy_ir_json, "r") as f:
         __HEAVY_IR_OBJS = json.load(f)
 
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
         # get the object dictionary (note that it is NOT a copy)
         if self.is_hvlang:
-            self.__obj_dict = HeavyObject.__HEAVY_LANG_OBJS[obj_type]
+            self.__obj_dict = self.__HEAVY_LANG_OBJS[obj_type]
         elif self.is_hvir:
-            self.__obj_dict = HeavyObject.__HEAVY_IR_OBJS[obj_type]
+            self.__obj_dict = self.__HEAVY_IR_OBJS[obj_type]
         else:
             assert False, f"{obj_type} is not a Heavy Lang or IR object."
 
         # resolve arguments
         obj_args = obj_args or []
-        self.obj_args = {}
+        self.obj_dict = {}
         for i, a in enumerate(self.__obj_dict["args"]):
             # if the argument exists (and has been correctly resolved)
             if i < len(obj_args) and obj_args[i] is not None:
                 # force the Heavy argument type
                 # Catch type errors as early as possible
                 try:
-                    self.obj_args[a["name"]] = HeavyObject.force_arg_type(
+                    self.obj_dict[a["name"]] = self.force_arg_type(
                         obj_args[i],
                         a["value_type"])
                 except Exception as e:
                     self.add_error(
                         f"Heavy {obj_type} cannot convert argument \"{a['name']}\""
                         f" with value \"{obj_args[i]}\" to type {a['value_type']}: {e}")
             else:
@@ -74,15 +83,15 @@
 
         # send/receive, table, etc. must have public scope
         # TODO(mhroth): dirty
         if obj_type in ["table", "__table", "send", "__send", "receive", "__receive"]:
             self.__annotations["scope"] = "public"
 
     @classmethod
-    def force_arg_type(clazz, value, value_type):
+    def force_arg_type(cls, value: str, value_type: str) -> Any:
         # TODO(mhroth): add support for mixedarray?
         if value_type == "auto":
             try:
                 return float(value)
             except Exception:
                 return str(value)
         elif value_type == "float":
@@ -121,22 +130,22 @@
             # NOTE(mhroth): if value_type is not a known type or None, that is
             # not necessarily an error. It may simply be that the value should
             # not be resolved to anything other than what it already is.
             # This happens most often with message objects.
             return value
 
     @property
-    def is_hvlang(self):
-        return self.obj_type in HeavyObject.__HEAVY_LANG_OBJS
+    def is_hvlang(self) -> bool:
+        return self.obj_type in self.__HEAVY_LANG_OBJS
 
     @property
-    def is_hvir(self):
-        return self.obj_type in HeavyObject.__HEAVY_IR_OBJS
+    def is_hvir(self) -> bool:
+        return self.obj_type in self.__HEAVY_IR_OBJS
 
-    def get_inlet_connection_type(self, inlet_index):
+    def get_inlet_connection_type(self, inlet_index: int) -> Optional[str]:
         """ Returns the inlet connection type, None if the inlet does not exist.
         """
         # TODO(mhroth): it's stupid that hvlang and hvir json have different data formats here
         if self.is_hvlang:
             if len(self.__obj_dict["inlets"]) > inlet_index:
                 return self.__obj_dict["inlets"][inlet_index]["connectionType"]
             else:
@@ -145,15 +154,15 @@
             if len(self.__obj_dict["inlets"]) > inlet_index:
                 return self.__obj_dict["inlets"][inlet_index]
             else:
                 return None
         else:
             return None
 
-    def get_outlet_connection_type(self, outlet_index):
+    def get_outlet_connection_type(self, outlet_index: int) -> Optional[str]:
         """ Returns the outlet connection type, None if the inlet does not exist.
         """
         # TODO(mhroth): it's stupid that hvlang and hvir json have different data formats here
         if self.is_hvlang:
             if len(self.__obj_dict["outlets"]) > outlet_index:
                 return self.__obj_dict["outlets"][outlet_index]["connectionType"]
             else:
@@ -162,37 +171,37 @@
             if len(self.__obj_dict["outlets"]) > outlet_index:
                 return self.__obj_dict["outlets"][outlet_index]
             else:
                 return None
         else:
             return None
 
-    def add_connection(self, c):
+    def add_connection(self, c: Connection) -> None:
         """ Adds a connection, either inlet or outlet, to this object.
         """
         if c.from_id == self.obj_id:
             if self.get_outlet_connection_type(c.outlet_index) is not None:
                 self._outlet_connections[str(c.outlet_index)].append(c)
             else:
                 self.add_error(
                     f"Connection made from non-existent outlet at {self.obj_type}:{c.outlet_index}.",
                     enum=NotificationEnum.ERROR_UNABLE_TO_CONNECT_OBJECTS)
         elif c.to_id == self.obj_id:
             if self.get_inlet_connection_type(c.inlet_index) is not None:
                 self._inlet_connections[str(c.inlet_index)].append(c)
             else:
                 self.add_error(
-                    f"Connection made to non-existent inlet at [{self.obj_type} {self.obj_args}]:{c.inlet_index}.",
+                    f"Connection made to non-existent inlet at [{self.obj_type} {self.obj_dict}]:{c.inlet_index}.",
                     enum=NotificationEnum.ERROR_UNABLE_TO_CONNECT_OBJECTS)
         else:
             raise Exception("Adding a connection to the wrong object!")
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return {
             "type": self.obj_type,
-            "args": self.obj_args,
+            "args": self.obj_dict,
             "properties": {
                 "x": self.pos_x,
                 "y": self.pos_y
             },
             "annotations": self.__annotations
         }
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/HvSwitchcase.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTriggerObject.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,66 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
+from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
-class HvSwitchcase(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
-        assert obj_type == "__switchcase"
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+class PdTriggerObject(PdObject):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        assert obj_type in {"trigger", "t"}
+        super().__init__("trigger", obj_args, pos_x, pos_y)
 
-        # ensure that correct case hashes are generated
+        # convert all numeric casts to "f"
         for i, a in enumerate(self.obj_args):
-            try:
-                self.obj_args[i] = float(a)
-            except Exception:
-                pass
+            self.obj_args[i] = "f" if PdTriggerObject.__is_float(a) else a
 
-    def get_outlet_connection_type(self, outlet_index):
-        return "-->"
+        if len(self.obj_args) == 0:
+            self.obj_args = ["b", "b"]
+            self.add_warning("A trigger with no arguments defualts to [t b b].")
+        if obj_args is not None and not (set(obj_args) <= set(["a", "f", "s", "b"])):
+            self.add_error(
+                "Heavy only supports arguments 'a', 'f', 's', and 'b'.",
+                NotificationEnum.ERROR_TRIGGER_ABFS)
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return {
-            "type": "__switchcase",
+            "type": "sequence",
             "args": {
-                "cases": self.obj_args
+                "casts": self.obj_args
             },
             "properties": {
                 "x": self.pos_x,
                 "y": self.pos_y
             }
         }
+
+    @classmethod
+    def __is_float(cls, x: int) -> bool:
+        """ Returns True if the input can be converted to a float. False otherwise.
+        """
+        try:
+            float(x)
+            return True
+        except Exception:
+            return False
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/NotificationEnum.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/NotificationEnum.py`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdAudioIoObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdAudioIoObject.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
 class PdAudioIoObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert obj_type in {"adc~", "dac~"}
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         # ensure that only signal connections are made to the dac
         for i, connections in self._inlet_connections.items():
             if any(c.conn_type == "-->" for c in connections):
                 self.add_error(
                     f"{self.obj_type} does not support control connections (inlet {i}). They should be removed.",
                     NotificationEnum.ERROR_UNSUPPORTED_CONNECTION)
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return {
             "type": self.obj_type.strip("~"),
             "args": {
                 "channels": [1, 2] if len(self.obj_args) == 0 else [int(a) for a in self.obj_args]
             },
             "properties": {
                 "x": self.pos_x,
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdBinopObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdBinopObject.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .Connection import Connection
-from .PdObject import PdObject
 from .HeavyObject import HeavyObject
+from .PdObject import PdObject
 
 
 class PdBinopObject(PdObject):
     # a translation dictionary from a Pd object to corresponding heavy object
     __PD_HEAVY_DICT = {
         "+": "+",
         "+~": "+",
@@ -47,27 +50,33 @@
         ">=": ">=",
         "pow": "pow",
         "pow~": "pow",
         ">>": ">>",
         "<<": "<<"
     }
 
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
-        assert PdBinopObject.is_binop(obj_type)
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        assert self.is_binop(obj_type)
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
     @classmethod
-    def is_binop(clazz, obj_type):
-        return obj_type in PdBinopObject.__PD_HEAVY_DICT
+    def is_binop(cls, obj_type: str) -> bool:
+        return obj_type in cls.__PD_HEAVY_DICT
 
     @classmethod
-    def get_supported_objects(clazz):
-        return set(PdBinopObject.__PD_HEAVY_DICT.keys())
+    def get_supported_objects(cls) -> set:
+        return set(cls.__PD_HEAVY_DICT.keys())
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         # check signal objects for control connections and auto insert
         # heavy var objects where necessary
         if self.obj_type.endswith("~"):
 
             # left inlet check
             conns_left = self._inlet_connections.get("0", [])
 
@@ -96,52 +105,53 @@
                 self.__k = float(self.obj_args[0])
             except Exception:
                 self.add_warning(f"\"{self.obj_args[0]}\" cannot be resolved to a number. Defaulting to zero.")
                 self.__k = 0.0
         else:
             self.__k = 0.0
 
-    def convert_ctrl_to_sig_connections_at_inlet(self, connection_list, inlet_index):
+    def convert_ctrl_to_sig_connections_at_inlet(self, connection_list: List, inlet_index: int) -> None:
         """ Auto insert heavy var object inbetween control connections.
         """
         sig_obj = HeavyObject(obj_type="var",
                               obj_args=[0],
                               pos_x=int(self.pos_x),
                               pos_y=int(self.pos_y - 5))  # shift upwards a few points
 
         # add sig~ object to parent graph
-        self.parent_graph.add_object(sig_obj)
+        if self.parent_graph is not None:
+            self.parent_graph.add_object(sig_obj)
 
-        # add connection from sig~ to this object
-        c = Connection(sig_obj, 0, self, inlet_index, "~f>")
-        self.parent_graph._PdGraph__connections.append(c)  # update the local connections list
-        sig_obj.add_connection(c)
-        self.add_connection(c)
-
-        # retrieve all control connections
-        control_conns = [c for c in connection_list if c.conn_type == "-->"]
-
-        for old_conn in control_conns:
-            # get from obj
-            from_obj = old_conn.from_obj
-
-            # add connection from fromobj to new sig
-            new_conn = Connection(from_obj, old_conn.outlet_index, sig_obj, 0, "-->")
-            self.parent_graph._PdGraph__connections.append(new_conn)
-            sig_obj.add_connection(new_conn)
-            from_obj.add_connection(new_conn)
-
-            # remove connection from fromobj
-            self.parent_graph._PdGraph__connections.remove(old_conn)
-            from_obj.remove_connection(old_conn)
-            self.remove_connection(old_conn)
+            # add connection from sig~ to this object
+            c = Connection(sig_obj, 0, self, inlet_index, "~f>")
+            self.parent_graph._PdGraph__connections.append(c)  # update the local connections list
+            sig_obj.add_connection(c)
+            self.add_connection(c)
+
+            # retrieve all control connections
+            control_conns = [c for c in connection_list if c.conn_type == "-->"]
+
+            for old_conn in control_conns:
+                # get from obj
+                from_obj = old_conn.from_obj
+
+                # add connection from fromobj to new sig
+                new_conn = Connection(from_obj, old_conn.outlet_index, sig_obj, 0, "-->")
+                self.parent_graph._PdGraph__connections.append(new_conn)
+                sig_obj.add_connection(new_conn)
+                from_obj.add_connection(new_conn)
+
+                # remove connection from fromobj
+                self.parent_graph._PdGraph__connections.remove(old_conn)
+                from_obj.remove_connection(old_conn)
+                self.remove_connection(old_conn)
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return {
-            "type": PdBinopObject.__PD_HEAVY_DICT[self.obj_type],
+            "type": self.__PD_HEAVY_DICT[self.obj_type],
             "args": {
                 "k": self.__k
             },
             "properties": {
                 "x": self.pos_x,
                 "y": self.pos_y
             }
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdGraph.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdGraph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,58 +11,72 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
+from typing import Optional, List, Dict
 
 from .Connection import Connection
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
 class PdGraph(PdObject):
 
-    def __init__(self, obj_args, pd_path, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_args: List,
+        pd_path: str,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert len(obj_args) > 0, "PdGraph arguments must contain at least dollar zero."
-        PdObject.__init__(self, "graph", obj_args, pos_x, pos_y)
+        super().__init__("graph", obj_args, pos_x, pos_y)
 
         # file location of this graph
         self.__pd_path = pd_path
 
-        self.__objs = []
-        self.__connections = []
+        self.__objs: List = []
+        self.__connections: List = []
 
-        self.__inlet_objects = []
-        self.__outlet_objects = []
+        self.__inlet_objects: List = []
+        self.__outlet_objects: List = []
 
         # the first search path is always the directory of this graph
-        self.__declared_paths = [os.path.dirname(pd_path)]
+        self.__declared_paths: List = [os.path.dirname(pd_path)]
 
         # heavy graph arguments (added via @hv_arg flag in #X text)
-        self.hv_args = []
+        self.hv_args: List = []
 
         # the subpatch name of this graph
         # only used is this graph is actually a subpatch
-        self.subpatch_name = None
+        self.subpatch_name: Optional[str] = None
+
+        # TODO(dromer) these are virtual attributes that are only instantiated with internal representation
+        self._PdGraph__connections: List[Connection] = []
+        self._PdGraph__pd_path: str = ""
 
     @property
-    def dollar_zero(self):
+    def dollar_zero(self) -> str:
         return self.obj_args[0]
 
     @property
-    def is_root(self):
+    def is_root(self) -> bool:
         return self.parent_graph is None
 
     @property
-    def is_subpatch(self):
-        return self.parent_graph.__pd_path == self.__pd_path if not self.is_root else False
+    def is_subpatch(self) -> bool:
+        if self.parent_graph is None:
+            return False
+        else:
+            return self.parent_graph.__pd_path == self.__pd_path if not self.is_root else False
 
-    def add_object(self, obj):
+    def add_object(self, obj: PdObject) -> None:
         obj.parent_graph = self
         self.__objs.append(obj)
 
         if obj.obj_type in ["inlet", "inlet~"]:
             self.__inlet_objects.append(obj)
             # set correct let index by sorting on x position
             self.__inlet_objects.sort(key=lambda o: o.pos_x)
@@ -69,15 +84,15 @@
                 o.let_index = i
         elif obj.obj_type in ["outlet", "outlet~"]:
             self.__outlet_objects.append(obj)
             self.__outlet_objects.sort(key=lambda o: o.pos_x)
             for i, o in enumerate(self.__outlet_objects):
                 o.let_index = i
 
-    def add_parsed_connection(self, from_index, from_outlet, to_index, to_inlet):
+    def add_parsed_connection(self, from_index: int, from_outlet: int, to_index: int, to_inlet: int) -> None:
         """ Add a connection to the graph which has been parsed externally.
         """
         try:
             # when connecting a Heavy object that allows mixed connection types,
             # try to immediately resolve to a non-mixed type based on the
             # object that it is connected to.
             connection_type = self.__objs[from_index].get_outlet_connection_type(from_outlet)
@@ -97,15 +112,15 @@
             self.__objs[to_index].add_connection(c)
         except Exception:
             self.add_error("There was an error while connecting two objects. "
                            "Have all objects been correctly instantiated? "
                            "Have all inlets and outlets been declared?",
                            NotificationEnum.ERROR_UNABLE_TO_CONNECT_OBJECTS)
 
-    def add_hv_arg(self, arg_index, name, value_type, default_value, required):
+    def add_hv_arg(self, arg_index: int, name: str, value_type: str, default_value: str, required: bool) -> None:
         """ Add a Heavy argument to the graph. Indicies are from zero (not one, like Pd).
         """
         # ensure that self.hv_args is big enough, as heavy arguments are not
         # necessarily added in the natural order
         while arg_index >= len(self.hv_args):
             self.hv_args.append(None)
 
@@ -113,21 +128,21 @@
             "name": name,
             "description": "",
             "value_type": value_type,
             "default": default_value,
             "required": required
         }
 
-    def get_inlet_connection_type(self, inlet_index):
-        return self.__inlet_objects[inlet_index].get_inlet_connection_type()
+    def get_inlet_connection_type(self, inlet_index: int) -> str:
+        return self.__inlet_objects[inlet_index].get_inlet_connection_type(inlet_index)
 
-    def get_outlet_connection_type(self, outlet_index):
-        return self.__outlet_objects[outlet_index].get_outlet_connection_type()
+    def get_outlet_connection_type(self, outlet_index: int) -> str:
+        return self.__outlet_objects[outlet_index].get_outlet_connection_type(outlet_index)
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         if self.is_root:
             if any((o.obj_type in {"inlet~", "outlet~"}) for o in self.__objs):
                 self.add_error(
                     "Top-level graphs may not contain inlet~ or outlet~ objects. "
                     "Use adc~ and dac~.",
                     NotificationEnum.ERROR_NO_TOPLEVEL_SIGNAL_LETS)
             if any((o.obj_type in {"inlet", "outlet"}) for o in self.__objs):
@@ -135,53 +150,64 @@
                     "Control inlets and outlets in top-level graphs don't do "
                     "anything. Use receive and send objects.")
 
         # validate all object recursively
         for o in self.__objs:
             o.validate_configuration()
 
-    def is_abstraction_on_call_stack(self, abs_path):
+    def is_abstraction_on_call_stack(self, abs_path: str) -> bool:
         """ Returns True if the given abstraction name is already on the call
             stack (i.e. it is currently being parsed). This function is used to
             detect recursion within abstractions.
         """
         if self.__pd_path == abs_path:
             return True
-        elif not self.is_root:
+        elif not self.is_root and self.parent_graph:
             return self.parent_graph.is_abstraction_on_call_stack(abs_path)
         else:
             return False
 
-    def get_notices(self):
+    def get_notices(self) -> Dict:
         notices = PdObject.get_notices(self)
         for o in self.__objs:
             n = o.get_notices()
             notices["warnings"].extend(n["warnings"])
             notices["errors"].extend(n["errors"])
 
         # remove ERROR_EXCEPTION if there are already other errors.
         # The exception is always a result of some other error
         if any((n["enum"] != NotificationEnum.ERROR_EXCEPTION) for n in notices["errors"]):
             notices["errors"] = [n for n in notices["errors"] if n["enum"] != NotificationEnum.ERROR_EXCEPTION]
 
         return notices
 
-    def get_graph_heirarchy(self):
+    def get_graph_heirarchy(self) -> List:
         """ Returns the "path" of this graph, indicating where it is in the
             graph heirarchy (i.e. with file names, etc.)
         """
-        return [str(self)] if self.is_root else \
-            self.parent_graph.get_graph_heirarchy() + [str(self)]
+        if self.is_root:
+            return [str(self)]
+        elif self.parent_graph is not None:
+            return self.parent_graph.get_graph_heirarchy() + [str(self)]
+        else:
+            # NOTE(dromer): we should never get here
+            raise Exception("parent_graph argument is None")
 
-    def get_depth(self):
+    def get_depth(self) -> int:
         """ Returns the depth of this graph, with the root being at 1.
         """
-        return 1 if self.is_root else (1 + self.parent_graph.get_depth())
+        if self.is_root:
+            return 1
+        elif self.parent_graph is not None:
+            return 1 + self.parent_graph.get_depth()
+        else:
+            # NOTE(dromer): we should never get here
+            raise Exception("parent_graph argument is None")
 
-    def to_hv(self, export_args=False):
+    def to_hv(self, export_args: bool = False) -> Dict:
         # NOTE(mhroth): hv_args are not returned. Because all arguments have
         # been resolved, no arguments are otherwise passed. hv2ir would break
         # on required arguments that are not passed to the graph
         assert all(a is not None for a in self.hv_args), "Graph is missing a @hv_arg."
         return {
             "type": "graph",
             "imports": [],
@@ -190,9 +216,9 @@
             "connections": [c.to_hv() for c in self.__connections],
             "properties": {
                 "x": self.pos_x,
                 "y": self.pos_y
             }
         }
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.subpatch_name or os.path.basename(self.__pd_path)
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdLibSignalGraph.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdLibSignalGraph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,87 @@
-# Copyright 2018 Enzien Audio, Ltd. All Rights Reserved.
+# Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
+from typing import List
 
 from .Connection import Connection
-from .PdGraph import PdGraph
 from .HeavyObject import HeavyObject
+from .PdGraph import PdGraph
 
 
 class PdLibSignalGraph(PdGraph):
 
-    def __init__(self, obj_args, pd_path, pos_x=0, pos_y=0):
-        PdGraph.__init__(self, obj_args, pd_path, pos_x, pos_y)
+    def __init__(
+        self,
+        obj_args: List,
+        pd_path: str,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        super().__init__(obj_args, pd_path, pos_x, pos_y)
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         """ Auto-detect control only connections to expected signal inlets and
             insert a sig~ (var) object inbetween to ensure it doesn't break.
         """
+
         # Note(joe): only checking first inlet, should we check all inlets by
         # default? i.e. samphold~ has a 2nd inlet that requires checking
         conns = self._inlet_connections.get("0", [])
 
         # only do this if no signal connections are present
         if (len([c for c in conns if c.conn_type == "~f>"]) == 0) and len(conns) > 0:
 
             # add sig~ object to parent graph
-            sig_obj = HeavyObject(
-                obj_type="var",
-                obj_args=[0],
-                pos_x=int(self.pos_x),
-                pos_y=int(self.pos_y - 5))  # shift upwards a few points
-            self.parent_graph.add_object(sig_obj)
-
-            # add connection from sig~ to this abstraction
-            c = Connection(sig_obj, 0, self, 0, "~f>")
-            self.parent_graph._PdGraph__connections.append(c)  # update the local connections list
-            sig_obj.add_connection(c)
-            self.add_connection(c)
-
-            # retrieve all control connections
-            control_conns = [c for c in conns if c.conn_type == "-->"]
-
-            for old_conn in control_conns:
-                # get from obj
-                from_obj = old_conn.from_obj
-
-                # add connection from fromobj to new sig
-                new_conn = Connection(from_obj, old_conn.outlet_index, sig_obj, 0, "-->")
-                self.parent_graph._PdGraph__connections.append(new_conn)
-                sig_obj.add_connection(new_conn)
-                from_obj.add_connection(new_conn)
-
-                # remove connection from fromobj
-                self.parent_graph._PdGraph__connections.remove(old_conn)
-                from_obj.remove_connection(old_conn)
-                self.remove_connection(old_conn)
+            if self.parent_graph is not None:
+                sig_obj = HeavyObject(
+                    obj_type="var",
+                    obj_args=[0],
+                    pos_x=int(self.pos_x),
+                    pos_y=int(self.pos_y - 5))  # shift upwards a few points
+                self.parent_graph.add_object(sig_obj)
+
+                # add connection from sig~ to this abstraction
+                c = Connection(sig_obj, 0, self, 0, "~f>")
+                self.parent_graph._PdGraph__connections.append(c)  # update the local connections list
+                sig_obj.add_connection(c)
+                self.add_connection(c)
+
+                # retrieve all control connections
+                control_conns = [c for c in conns if c.conn_type == "-->"]
+
+                for old_conn in control_conns:
+                    # get from obj
+                    from_obj = old_conn.from_obj
+
+                    # add connection from fromobj to new sig
+                    new_conn = Connection(from_obj, old_conn.outlet_index, sig_obj, 0, "-->")
+                    self.parent_graph._PdGraph__connections.append(new_conn)
+                    sig_obj.add_connection(new_conn)
+                    from_obj.add_connection(new_conn)
+
+                    # remove connection from fromobj
+                    self.parent_graph._PdGraph__connections.remove(old_conn)
+                    from_obj.remove_connection(old_conn)
+                    self.remove_connection(old_conn)
 
         # make sure to call parent validate_configuration()
-        PdGraph.validate_configuration(self)
+        super().validate_configuration()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "[{0} {1}]".format(
             os.path.splitext(os.path.basename(self._PdGraph__pd_path))[0],
             " ".join(self.obj_args[1:]))
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdObject.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,52 +14,64 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from collections import defaultdict
 import random
 import string
 
-from hvcc.interpreters.pd2hv.NotificationEnum import NotificationEnum
+from typing import Optional, List, Dict, TYPE_CHECKING
+
+from .Connection import Connection
+from .NotificationEnum import NotificationEnum
+
+if TYPE_CHECKING:
+    from .PdGraph import PdGraph
 
 
 class PdObject:
 
     __RANDOM = random.Random()
     __ID_CHARS = string.ascii_letters + string.digits
 
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         self.obj_type = obj_type
         # all arguments should be resolved when passed to a PdObject
         self.obj_args = obj_args or []
         self.obj_id = "{0}_{1}".format(
             obj_type,
-            "".join(PdObject.__RANDOM.choice(PdObject.__ID_CHARS) for _ in range(8)))
+            "".join(self.__RANDOM.choice(self.__ID_CHARS) for _ in range(8)))
         self.pos_x = pos_x
         self.pos_y = pos_y
 
         # this is set when the object is added to a graph
-        self.parent_graph = None
+        self.parent_graph: Optional['PdGraph'] = None
 
-        self._inlet_connections = defaultdict(list)
-        self._outlet_connections = defaultdict(list)
+        self._inlet_connections: Dict = defaultdict(list)
+        self._outlet_connections: Dict = defaultdict(list)
 
-        self._warnings = []
-        self._errors = []
+        self._warnings: List = []
+        self._errors: List = []
 
-    def add_warning(self, warning, enum=NotificationEnum.WARNING_GENERIC):
+    def add_warning(self, warning: str, enum: NotificationEnum = NotificationEnum.WARNING_GENERIC) -> None:
         """ Add a warning regarding this object.
         """
         self._warnings.append({"enum": enum, "message": warning})
 
-    def add_error(self, error, enum=NotificationEnum.ERROR_GENERIC):
+    def add_error(self, error: str, enum: NotificationEnum = NotificationEnum.ERROR_GENERIC) -> None:
         """ Add an error regarding this object.
         """
         self._errors.append({"enum": enum, "message": error})
 
-    def get_notices(self):
+    def get_notices(self) -> Dict:
         """ Returns a dictionary of all warnings and errors at this object.
         """
         # TODO(mhroth): we might want to consider moving to a more expressive format.
         # {
         #     "objectType": "trigger",
         #     "objectString": "t l l",
         #     "graphs": ["_main", "hello"],
@@ -95,77 +108,77 @@
                     "enum": n["enum"],
                     "message": "{0} in \"{1}\" @ (x:{2}, y:{3}): {4}".format(
                         self, "/".join(self.get_graph_heirarchy()), self.pos_x, self.pos_y, n["message"])
                 } for n in self._errors
             ]
         }
 
-    def get_inlet_connection_type(self, inlet_index=0):
+    def get_inlet_connection_type(self, inlet_index: int) -> Optional[str]:
         """ Returns the inlet connection type of this Pd object.
             For the sake of convenience, the connection type is reported in
             Heavy's format.
         """
         return "~f>" if self.obj_type.endswith("~") else "-->"
 
-    def get_outlet_connection_type(self, outlet_index=0):
+    def get_outlet_connection_type(self, outlet_index: int) -> Optional[str]:
         """ Returns the outlet connection type of this Pd object.
             For the sake of convenience, the connection type is reported in
             Heavy's format.
         """
         return "~f>" if self.obj_type.endswith("~") else "-->"
 
-    def add_connection(self, c):
+    def add_connection(self, c: Connection) -> None:
         """ Adds a connection, either inlet or outlet, to this object.
         """
         if c.from_id == self.obj_id:
             self._outlet_connections[str(c.outlet_index)].append(c)
         elif c.to_id == self.obj_id:
             self._inlet_connections[str(c.inlet_index)].append(c)
         else:
             raise Exception("Adding a connection to the wrong object!")
 
-    def remove_connection(self, c):
+    def remove_connection(self, c: Connection) -> None:
         """ Remove a connection to this object.
         """
         if c.to_obj is self:
             self._inlet_connections[str(c.inlet_index)].remove(c)
         elif c.from_obj is self:
             self._outlet_connections[str(c.outlet_index)].remove(c)
         else:
             raise Exception(f"Connection {c} does not connect to this object {self}.")
 
-    def get_graph_heirarchy(self):
+    def get_graph_heirarchy(self) -> List:
         """ Returns an indication of the graph "path" of this object.
         It only includes unique graphs (not subpatches) E.g. _main/tabosc4~
         The check for None is in case the object is somehow not yet attached.
         """
         return self.parent_graph.get_graph_heirarchy() \
             if self.parent_graph is not None else ["unattached"]
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         """ Called when all graphs are finished parsing, from the root.
             Gives each object the chance to validate it's configuration,
             including connections.
             In general this function does nothing, though it may add warnings and
             errors.
             Note that object validation occurs when the entire patch is finished
             parsing and before it is returned to the user. The program may assume
             that all parameters and variables have been set.
         """
         pass
 
     @classmethod
-    def get_supported_objects(clazz):
+    def get_supported_objects(cls) -> set:
         """ Returns a list of Pd objects that this class can parse.
         """
         raise NotImplementedError()
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         """ Returns the HeavyLang JSON representation of this object.
         """
         raise NotImplementedError()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if len(self.obj_args) == 0:
             return f"[{self.obj_type}]"
         else:
             return f"[{self.obj_type} {' '.join([str(o) for o in self.obj_args])}]"
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdPackObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/HvSwitchcase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from .NotificationEnum import NotificationEnum
-from .PdObject import PdObject
-
+from typing import Optional, List, Dict
 
-class PdPackObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
-        assert obj_type == "pack"
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+from .PdObject import PdObject
 
-        self.values = []
 
-        if len(self.obj_args) == 0:
-            self.values = [0.0, 0.0]
+class HvSwitchcase(PdObject):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        assert obj_type == "__switchcase"
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
-        for x in self.obj_args:
+        # ensure that correct case hashes are generated
+        for i, a in enumerate(self.obj_args):
             try:
-                self.values.append(float(x))
+                self.obj_args[i] = float(a)
             except Exception:
-                if x in {"f", "float"}:
-                    self.values.append(0.0)
-                else:
-                    self.add_error(
-                        f"\"{x}\" argument to [pack] object not supported.",
-                        NotificationEnum.ERROR_PACK_FLOAT_ARGUMENTS)
+                pass
+
+    def get_outlet_connection_type(self, outlet_index: int = 0) -> str:
+        return "-->"
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return {
-            "type": "__pack",
+            "type": "__switchcase",
             "args": {
-                "values": self.values
+                "cases": self.obj_args
             },
             "properties": {
                 "x": self.pos_x,
                 "y": self.pos_y
             }
         }
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdParser.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdParser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from collections import Counter
-from collections import OrderedDict
 import decimal
 import os
 import re
+from collections import Counter
+from collections import OrderedDict
+from typing import List, Dict, Optional, Type, Any, Generator
 
 from .HeavyObject import HeavyObject
 from .HeavyGraph import HeavyGraph              # pre-converted Heavy graphs
 from .HvSwitchcase import HvSwitchcase          # __switchcase
 from .PdAudioIoObject import PdAudioIoObject    # adc~/dac~
 from .PdBinopObject import PdBinopObject        # binary arithmatic operators
 from .PdGraph import PdGraph                    # canvas
@@ -50,84 +52,84 @@
 
     # detect a dollar argument in a string
     __RE_DOLLAR = re.compile(r"\$(\d+)")
 
     # detect width parameter e.g. "#X obj 172 79 t b b, f 22;"
     __RE_WIDTH = re.compile(r", f \d+$")
 
-    def __init__(self):
+    def __init__(self) -> None:
         # the current global value of $0
         # Note(joe): set a high starting value to avoid potential user naming conflicts
         self.__DOLLAR_ZERO = 1000
 
         # a counter of all Pd objects in the graph
-        self.obj_counter = Counter()
+        self.obj_counter: Counter = Counter()
 
         # search paths at this graph level
-        self.__search_paths = []
+        self.__search_paths: List = []
 
     @classmethod
-    def get_supported_objects(clazz):
+    def get_supported_objects(cls) -> List:
         """ Returns a set of all pd objects names supported by the parser.
         """
-        pd_objects = [os.path.splitext(f)[0] for f in os.listdir(clazz.__PDLIB_DIR) if f.endswith(".pd")]
-        pd_objects.extend(PdParser.__PD_CLASSES.keys())
+        pd_objects = [os.path.splitext(f)[0] for f in os.listdir(cls.__PDLIB_DIR) if f.endswith(".pd")]
+        pd_objects.extend(cls.__PD_CLASSES.keys())
         return pd_objects
 
     @classmethod
-    def __get_hv_args(clazz, pd_path):
+    def __get_hv_args(cls, pd_path: str) -> OrderedDict:
         """ Pre-parse the file for Heavy arguments, such that they are available
             as soon as a graph is created.
         """
         num_canvas = -1
         hv_arg_dict = OrderedDict()
-        hv_arg_list = None
+        hv_arg_list: Optional[List] = None
         with open(pd_path, "r") as f:
             for li in f:
                 if li.startswith("#N canvas"):
                     hv_arg_list = []
                     hv_arg_dict[li.rstrip(";\r\n")] = hv_arg_list
                     num_canvas += 1
-                elif "@hv_arg" in li:
+                elif "@hv_arg" in li and hv_arg_list is not None:
                     hv_arg_list.append(li.rstrip(";\r\n"))
                 elif li.startswith("#X restore"):
                     num_canvas -= 1
                     hv_arg_list = list(hv_arg_dict.values())[num_canvas]
         return hv_arg_dict
 
     @classmethod
-    def __get_pd_line(clazz, pd_path):
+    def __get_pd_line(cls, pd_path: str) -> Generator:
         concat = ""  # concatination state
         with open(pd_path, "r") as f:
             for li in f:
                 # concatenate split lines in the Pd file here
                 li = li.rstrip("\r\n")  # account for windows CRLF
                 if li.endswith(";") and not li.endswith(r"\;"):
                     out = li[:-1]  # remove single ";"
                     if len(concat) > 0:
                         out = f'{concat} {out}'
                         concat = ""  # reset concatenation state
                     yield out
                 else:
                     concat = (f'{concat} {li}') if len(concat) > 0 else f'{li}'
 
-    def add_absolute_search_directory(self, search_dir):
+    def add_absolute_search_directory(self, search_dir: str) -> bool:
         if os.path.isdir(search_dir):
             self.__search_paths.append(search_dir)
             return True
         else:
             return False
 
-    def add_relative_search_directory(self, search_dir):
+    def add_relative_search_directory(self, search_dir: str) -> bool:
         search_dir = os.path.abspath(os.path.join(
             self.__search_paths[0],
             search_dir))
         return self.add_absolute_search_directory(search_dir)
 
-    def find_abstraction_path(self, local_dir, abs_name):
+    def find_abstraction_path(self, local_dir: str, abs_name: str) -> Optional[str]:
         """ Finds the full path for an abstraction.
             Checks the local directory first, then all declared paths.
         """
 
         abs_filename = f'{abs_name}.pd'
 
         # check local directory first
@@ -139,27 +141,35 @@
         for d in reversed(self.__search_paths):
             abs_path = os.path.join(d, abs_filename)
             if os.path.isfile(abs_path):
                 return abs_path
 
         return None
 
-    def graph_from_file(self, file_path, obj_args=None, pos_x=0, pos_y=0, is_root=True, pd_graph_class=PdGraph):
+    def graph_from_file(
+        self,
+        file_path: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0,
+        is_root: bool = True,
+        pd_graph_class: Type[PdGraph] = PdGraph
+    ) -> Any:
         """ Instantiate a PdGraph from a file.
             Note that obj_args does not include $0.
             @param pd_graph_class  The python class to handle specific graph types
         """
         # add main patch directory. The first entry of self.__search_paths is
         # assumed to be the root path of the whole system
 
         if is_root:
             self.__search_paths.append(os.path.dirname(file_path))
 
-        file_hv_arg_dict = PdParser.__get_hv_args(file_path)
-        file_iterator = PdParser.__get_pd_line(file_path)
+        file_hv_arg_dict = self.__get_hv_args(file_path)
+        file_iterator = self.__get_pd_line(file_path)
         canvas_line = file_iterator.__next__()
 
         self.__DOLLAR_ZERO += 1  # increment $0
         graph_args = [self.__DOLLAR_ZERO] + (obj_args or [])
 
         if not canvas_line.startswith("#N canvas"):
             g = pd_graph_class(graph_args, file_path, pos_x, pos_y)
@@ -181,24 +191,34 @@
                 # return the graph early here as there are already errors and it is
                 # clearly invalid, avoids triggering unrelated errors in validation
                 return g
             g.validate_configuration()
 
         return g
 
-    def graph_from_canvas(self, file_iterator, file_hv_arg_dict, canvas_line, graph_args,
-                          pd_path, pos_x=0, pos_y=0, is_root=False, pd_graph_class=PdGraph):
+    def graph_from_canvas(
+        self,
+        file_iterator: Generator,
+        file_hv_arg_dict: Dict,
+        canvas_line: str,
+        graph_args: List,
+        pd_path: str,
+        pos_x: int = 0,
+        pos_y: int = 0,
+        is_root: bool = False,
+        pd_graph_class: Type[PdGraph] = PdGraph
+    ) -> Any:
         """ Instantiate a PdGraph from an existing canvas.
             Note that graph_args includes $0.
             @param file_hv_arg_dict  A dictionary containing all Heavy argument lines
             for each "#N canvas" in this file.
             @param canvas_line  The "#N canvas" which initiates this canvas.
             @param pd_graph_class  The python class to handle specific graph types
         """
-        obj_array = None  # an #A (table) object which is currently being parsed
+        obj_array: Optional[HeavyObject] = None  # an #A (table) object which is currently being parsed
 
         g = pd_graph_class(graph_args, pd_path, pos_x, pos_y)
 
         # parse and add all Heavy arguments to the graph
         for li in file_hv_arg_dict[canvas_line]:
             line = li.split()
             assert line[4] == "@hv_arg"
@@ -211,15 +231,15 @@
                 value_type=line[7],
                 default_value=default_value,
                 required=is_required)
 
         try:  # this try will capture any critical errors
             for li in file_iterator:
                 # remove width parameter
-                line = PdParser.__RE_WIDTH.sub("", li).split()
+                line = self.__RE_WIDTH.sub("", li).split()
 
                 if line[0] == "#N":
                     if line[1] == "canvas":
                         x = self.graph_from_canvas(
                             file_iterator,
                             file_hv_arg_dict,
                             canvas_line=li,
@@ -228,15 +248,15 @@
                             pos_x=int(line[2]),
                             pos_y=int(line[3]))
                         g.add_object(x)
 
                 elif line[0] == "#X":
                     if line[1] == "restore":
                         if len(line) > 5 and line[5] == "@hv_obj":
-                            obj_args = PdParser.__resolve_object_args(
+                            obj_args = self.__resolve_object_args(
                                 obj_type=line[6],
                                 obj_args=line[7:],
                                 graph=g,
                                 raise_on_failure=False,
                                 is_root=is_root)
                             if line[6] == "__switchcase":
                                 x = HvSwitchcase(
@@ -251,31 +271,31 @@
                                     pos_x=int(line[2]),
                                     pos_y=int(line[3]))
                             return x  # return a Heavy object instead of a graph
                         else:
                             # are we restoring an array object?
                             # do some final sanity checks
                             if obj_array is not None:
-                                declared_size = obj_array.obj_args["size"]
-                                values_size = len(obj_array.obj_args["values"])
+                                declared_size = obj_array.obj_dict["size"]
+                                values_size = len(obj_array.obj_dict["values"])
                                 if declared_size != values_size:
                                     new_size = max(declared_size, values_size)
                                     obj_array.add_warning(
                                         "Table \"{0}\" was declared as having {1} values, "
                                         "but {2} were supplied. It will be resized to {3} "
                                         "values (any unsupplied values will be zeroed).".format(
-                                            obj_array.obj_args["name"],
+                                            obj_array.obj_dict["name"],
                                             declared_size,
                                             values_size,
                                             new_size))
-                                    obj_array.obj_args["size"] = new_size
+                                    obj_array.obj_dict["size"] = new_size
                                     if new_size < declared_size:
-                                        obj_array.obj_args["values"] = obj_args["values"][:new_size]
+                                        obj_array.obj_dict["values"] = obj_args["values"][:new_size]
                                     else:
-                                        obj_array.obj_args["values"].extend([0.0 for _ in
+                                        obj_array.obj_dict["values"].extend([0.0 for _ in
                                                                              range(new_size - declared_size)])
                                 obj_array = None  # done parsing the array
 
                             # set the subpatch name
                             g.subpatch_name = " ".join(line[5:]) if len(line) > 5 else "subpatch"
                             return g  # pop the graph
 
@@ -291,20 +311,20 @@
                             pos_y=int(line[3])))
 
                     elif line[1] == "obj":
                         x = None  # a PdObject
                         if len(line) > 4:
                             obj_type = line[4]
                             # sometimes objects have $ arguments in them as well
-                            obj_type = PdParser.__resolve_object_args(
+                            obj_type = self.__resolve_object_args(
                                 obj_type=obj_type,
                                 obj_args=[obj_type],
                                 graph=g,
                                 is_root=is_root)[0]
-                            obj_args = PdParser.__resolve_object_args(
+                            obj_args = self.__resolve_object_args(
                                 obj_type=obj_type,
                                 obj_args=line[5:],
                                 graph=g,
                                 is_root=is_root)
                         else:
                             g.add_warning(
                                 "This graph contains an empty object. "
@@ -324,39 +344,39 @@
                             x = self.graph_from_file(
                                 file_path=abs_path,
                                 obj_args=obj_args,
                                 pos_x=int(line[2]), pos_y=int(line[3]),
                                 is_root=False)
 
                         # is this object in lib/pd_converted?
-                        elif os.path.isfile(os.path.join(PdParser.__PDLIB_CONVERTED_DIR, f"{obj_type}.hv.json")):
+                        elif os.path.isfile(os.path.join(self.__PDLIB_CONVERTED_DIR, f"{obj_type}.hv.json")):
                             self.obj_counter[obj_type] += 1
-                            hv_path = os.path.join(PdParser.__PDLIB_CONVERTED_DIR, f"{obj_type}.hv.json")
+                            hv_path = os.path.join(self.__PDLIB_CONVERTED_DIR, f"{obj_type}.hv.json")
                             x = HeavyGraph(
                                 hv_path=hv_path,
                                 obj_args=obj_args,
                                 pos_x=int(line[2]), pos_y=int(line[3]))
 
                         # is this object in lib/heavy_converted?
-                        elif os.path.isfile(os.path.join(PdParser.__HVLIB_CONVERTED_DIR, f"{obj_type}.hv.json")):
+                        elif os.path.isfile(os.path.join(self.__HVLIB_CONVERTED_DIR, f"{obj_type}.hv.json")):
                             self.obj_counter[obj_type] += 1
-                            hv_path = os.path.join(PdParser.__HVLIB_CONVERTED_DIR, f"{obj_type}.hv.json")
+                            hv_path = os.path.join(self.__HVLIB_CONVERTED_DIR, f"{obj_type}.hv.json")
                             x = HeavyGraph(
                                 hv_path=hv_path,
                                 obj_args=obj_args,
                                 pos_x=int(line[2]), pos_y=int(line[3]))
 
                         # is this object in lib/pd?
-                        elif os.path.isfile(os.path.join(PdParser.__PDLIB_DIR, f"{obj_type}.pd")):
+                        elif os.path.isfile(os.path.join(self.__PDLIB_DIR, f"{obj_type}.pd")):
                             self.obj_counter[obj_type] += 1
-                            pdlib_path = os.path.join(PdParser.__PDLIB_DIR, f"{obj_type}.pd")
+                            pdlib_path = os.path.join(self.__PDLIB_DIR, f"{obj_type}.pd")
 
                             # mapping of pd/lib abstraction objects to classes
                             # for checking connection validity
-                            clazz = {
+                            pd_class = {
                                 "abs~": PdLibSignalGraph,
                                 "clip~": PdLibSignalGraph,
                                 "cos~": PdLibSignalGraph,
                                 "dbtopow~": PdLibSignalGraph,
                                 "dbtorms~": PdLibSignalGraph,
                                 "exp~": PdLibSignalGraph,
                                 "ftom~": PdLibSignalGraph,
@@ -373,42 +393,42 @@
                             }.get(obj_type, PdGraph)
 
                             x = self.graph_from_file(
                                 file_path=pdlib_path,
                                 obj_args=obj_args,
                                 pos_x=int(line[2]), pos_y=int(line[3]),
                                 is_root=False,
-                                pd_graph_class=clazz)
+                                pd_graph_class=pd_class)
 
                             # register any object-specific warnings or errors
                             if obj_type in {"rzero~", "rzero_rev~", "czero~", "czero_rev~"}:
                                 g.add_warning(
                                     f"[{obj_type}] accepts only signal input. "
                                     "Arguments and control connections are ignored.")
 
                         # is this object in lib/heavy?
-                        elif os.path.isfile(os.path.join(PdParser.__HVLIB_DIR, f"{obj_type}.pd")):
+                        elif os.path.isfile(os.path.join(self.__HVLIB_DIR, f"{obj_type}.pd")):
                             self.obj_counter[obj_type] += 1
-                            hvlib_path = os.path.join(PdParser.__HVLIB_DIR, f"{obj_type}.pd")
+                            hvlib_path = os.path.join(self.__HVLIB_DIR, f"{obj_type}.pd")
                             x = self.graph_from_file(
                                 file_path=hvlib_path,
                                 obj_args=obj_args,
                                 pos_x=int(line[2]), pos_y=int(line[3]),
                                 is_root=False)
 
                         # is this an object that must be programatically parsed?
-                        elif obj_type in PdParser.__PD_CLASSES:
+                        elif obj_type in self.__PD_CLASSES:
                             self.obj_counter[obj_type] += 1
-                            obj_class = PdParser.__PD_CLASSES[obj_type]
+                            obj_class = self.__PD_CLASSES[obj_type]
                             x = obj_class(
                                 obj_type,
                                 obj_args,
                                 pos_x=int(line[2]), pos_y=int(line[3]))
 
-                        elif PdParser.__is_float(obj_type):
+                        elif self.__is_float(obj_type):
                             # parse float literals
                             self.obj_counter["float"] += 1
                             x = HeavyObject(
                                 obj_type="__var",
                                 obj_args=[float(obj_type)],
                                 pos_x=int(line[2]), pos_y=int(line[3]))
 
@@ -423,25 +443,25 @@
                                 obj_args=[f"null object placeholder ({obj_type})"])
 
                         g.add_object(x)
 
                     elif line[1] in {"floatatom", "symbolatom"}:
                         self.obj_counter[line[1]] += 1
                         x = self.graph_from_file(
-                            file_path=os.path.join(PdParser.__PDLIB_DIR, f"{line[1]}.pd"),
+                            file_path=os.path.join(self.__PDLIB_DIR, f"{line[1]}.pd"),
                             obj_args=[],
                             pos_x=int(line[2]), pos_y=int(line[3]),
                             is_root=False)
                         g.add_object(x)
 
                     elif line[1] == "array":
                         assert obj_array is None, "#X array object is already being parsed."
                         # array names can have dollar arguments in them.
                         # ensure that they are resolved
-                        table_name = PdParser.__resolve_object_args(
+                        table_name = self.__resolve_object_args(
                             obj_type="array",
                             obj_args=[line[2]],
                             graph=g)[0]
                         # Pd encodes arrays with length greater than 999,999 with
                         # scientific notatation (e.g. 1e6) which Python's int() can't parse
                         table_size = int(decimal.Decimal(line[3]))
                         obj_array = HeavyObject(
@@ -482,20 +502,25 @@
                             g.add_warning(
                                 "Heavy only supports the -path flag for the "
                                 "declare object.",
                                 NotificationEnum.WARNING_DECLARE_PATH)
 
                     elif line[1] == "coords":
                         pass  # don't do anything with this command
+                    elif line[1] == "f":
+                        # A line such as "#X f 123"
+                        # is found after a "#X restore" when the [pd afasdfasd]
+                        # object's box has been resized
+                        pass  # don't do anything with this command
 
                     else:
                         g.add_error(f"Don't know how to parse line: {' '.join(line)}")
 
-                elif line[0] == "#A":
-                    obj_array.obj_args["values"].extend([float(f) for f in line[2:]])
+                elif line[0] == "#A" and obj_array is not None:
+                    obj_array.obj_dict["values"].extend([float(f) for f in line[2:]])
 
                 else:
                     g.add_error(f"Don't know how to parse line: {' '.join(line)}")
 
         except Exception as e:
             # bubble the Exception back to the root graph where the graph
             # will be returned
@@ -505,27 +530,34 @@
                 # NOTE(mhroth): should the exception be added as an error?
                 # Sometimes it's all that we have, so perhaps it's a good idea.
                 g.add_error(str(e), NotificationEnum.ERROR_EXCEPTION)
 
         return g
 
     @classmethod
-    def __resolve_object_args(clazz, obj_type, obj_args, graph, raise_on_failure=True, is_root=False):
+    def __resolve_object_args(
+        cls,
+        obj_type: str,
+        obj_args: List,
+        graph: PdGraph,
+        raise_on_failure: bool = True,
+        is_root: bool = False
+    ) -> Any:
         """ Resolve object arguments against the given graph arguments.
             By default this function raises an Exception if it cannot resolve an
             argument.
             This behaviour may be disabled, in which case the unresolved argument
             is replaced with None (which is an otherwise invalid value). A value of
             None typically indicates to a HeavyObject that the default value
             may be used.
         """
         # TODO(mhroth): can this be done more elegantly?
         resolved_obj_args = list(obj_args)  # make a copy of the original obj_args
         for i, a in enumerate(obj_args):
-            for m in set(PdParser.__RE_DOLLAR.findall(a)):
+            for m in set(cls.__RE_DOLLAR.findall(a)):
                 x = int(m)  # the dollar index (i.e. $x)
                 if len(graph.obj_args) > x:
                     a = a.replace(fr"\${m}", str(graph.obj_args[x]))
 
                 # check if hv_args can be used to supply a default value
                 elif len(graph.hv_args) > (x - 1):  # heavy args are zero-indexed
                     if not graph.hv_args[x - 1]["required"]:
@@ -588,15 +620,15 @@
     }
 
     # fill in as much of __PD_CLASSES programmatically as possible
     for o in PdBinopObject.get_supported_objects():
         __PD_CLASSES[o] = PdBinopObject
 
     @classmethod
-    def __is_float(clazz, x):
+    def __is_float(cls, x: int) -> bool:
         """ Returns True if the input can be converted to a float. False otherwise.
         """
         try:
             float(x)
             return True
         except Exception:
             return False
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdRaw.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRaw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import List, Dict
+
+
 class PdRawException(Exception):
     pass
 
 
-def replace_owl(args):
+def replace_owl(args: List) -> List:
     new_args = []
     for arg in args:
         new_arg = arg.replace('owl', 'raw')
         new_args.append(new_arg)
     return new_args
 
 
-def parse_pd_raw_args(args):
+def parse_pd_raw_args(args: List) -> Dict:
     """Parses a list of puredata send or receive objects looking for @raw and legacy @owl*
     annotations, parsing everything and throwing errors when syntax is not
     correct or values are of incorrect type"""
 
     attrdict = {}
 
     # define default values
     attrdict["min"] = 0.0
     attrdict["max"] = 1.0
-    attrdict["default"] = None
 
     args = replace_owl(args)  # TODO(dromer): deprecate @owl on next stable release
 
     for raw_param in {'@raw', '@raw_min', '@raw_max', '@raw_default', '@raw_param'}:
         if raw_param not in args:
             continue
 
@@ -64,11 +67,11 @@
             try:
                 attrdict[raw_param.split('@raw_')[1]] = float(args[i + 1])
             except ValueError:
                 raise PdRawException(f"{raw_param} annotation value '{args[i + 1]}' is not numeric")
             except IndexError:
                 raise PdRawException(f"{raw_param} annotation is missing its value")
 
-    if attrdict["default"] is None:
+    if attrdict.get("default") is None:
         attrdict["default"] = (attrdict["max"] - attrdict["min"]) / 2.0
 
     return attrdict
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdReceiveObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdReceiveObject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .PdObject import PdObject
 from .PdRaw import parse_pd_raw_args, PdRawException
 
 
 class PdReceiveObject(PdObject):
 
     __INSTANCE_COUNTER = 0
 
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert obj_type in {"r", "r~", "receive", "receive~", "catch~"}
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
         self.__receiver_name = ""
         self.__extern_type = None
-        self.__attributes = {}
+        self.__attributes: Dict = {}
         self.__priority = None  # priority is not set
 
         PdReceiveObject.__INSTANCE_COUNTER += 1
         self.__instance = PdReceiveObject.__INSTANCE_COUNTER
 
         try:
             # receive objects don't necessarily need to have a name
@@ -83,34 +92,35 @@
 
         if '@raw' in self.obj_args or '@owl' in self.obj_args:  # TODO(dromer): deprecate @owl on next stable release
             try:
                 pd_raw_args = parse_pd_raw_args(self.obj_args)
                 self.__attributes.update(pd_raw_args)
                 self.__extern_type = "param"  # make sure output code is generated
             except PdRawException as e:
-                self.add_error(e)
+                self.add_error(str(e))
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         if self.obj_type in {"r~", "receive~"}:
             if len(self._inlet_connections.get("0", [])) > 0:
                 self.add_error("[receive~] inlet connections are not supported.")
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         # note: control rate send objects should not modify their name argument
         names = {
             "r": "",
             "receive": "",
             "r~": "sndrcv_sig_",
             "receive~": "sndrcv_sig_",
             "catch~": "thrwctch_sig_"
         }
 
         # NOTE(mhroth): we follow Pd's execution rule: deeper receivers fire first.
         # Receivers on the same level fire in the order of instantiation.
-        if (self.__priority is None) or (self.__receiver_name == "__hv_init" and self.__priority == 0):
+        if self.parent_graph is not None and \
+                ((self.__priority is None) or (self.__receiver_name == "__hv_init" and self.__priority == 0)):
             self.__priority = (self.parent_graph.get_depth() * 1000) - self.__instance
 
         return {
             "type": "receive",
             "args": {
                 "name": f"{names[self.obj_type]}{self.__receiver_name}",
                 "extern": self.__extern_type,
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdRouteObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdRouteObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,62 +11,72 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from collections import Counter
+from typing import Optional, List, Dict
+
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
 class PdRouteObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert obj_type == "route"
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
-        if len(obj_args) == 0:
-            self.add_error("At least one argument is required.")
-        # NOTE(joe): disabling this warning as it can be quite annoying.
-        # if len(set(obj_args) & set(["bang", "list", "float", "symbol"])) > 0:
-        #     self.add_warning(
-        #         "Heavy interprets route arguments such as \"bang\", \"list\", \"float\", "
-        #         "and \"symbol\" literally. They cannot be used to filter generic "
-        #         "messages as in Pd.")
-        if len(set(obj_args)) != len(obj_args):
-            c = Counter(obj_args).most_common(1)
-            self.add_error(
-                f"All arguments to [route] must be unique. Argument \"{c[0][0]}\" is repeated {c[0][1]} times.",
-                NotificationEnum.ERROR_UNIQUE_ARGUMENTS_REQUIRED)
-
-        # convert to obj_args to mixedarray, such that correct switchcase hash
-        # is generated
-        for i, a in enumerate(self.obj_args):
-            try:
-                self.obj_args[i] = float(a)
-            except Exception:
-                pass
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
+
+        if obj_args is not None:
+            if len(obj_args) == 0:
+                self.add_error("At least one argument is required.")
+            # NOTE(joe): disabling this warning as it can be quite annoying.
+            # if len(set(obj_args) & set(["bang", "list", "float", "symbol"])) > 0:
+            #     self.add_warning(
+            #         "Heavy interprets route arguments such as \"bang\", \"list\", \"float\", "
+            #         "and \"symbol\" literally. They cannot be used to filter generic "
+            #         "messages as in Pd.")
+            if len(set(obj_args)) != len(obj_args):
+                c = Counter(obj_args).most_common(1)
+                self.add_error(
+                    f"All arguments to [route] must be unique. Argument \"{c[0][0]}\" is repeated {c[0][1]} times.",
+                    NotificationEnum.ERROR_UNIQUE_ARGUMENTS_REQUIRED)
+
+            # convert to obj_args to mixedarray, such that correct switchcase hash
+            # is generated
+            for i, a in enumerate(self.obj_args):
+                try:
+                    self.obj_args[i] = float(a)
+                except Exception:
+                    pass
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         if len(self._inlet_connections.get("1", [])) > 0:
             self.add_warning("The right inlet of route is not supported. It will not do anything.")
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         """Creates a graph dynamically based on the number of arguments.
             An unconnected right inlet is added.
 
             [inlet]                                         [inlet]
             |
             [@hv_obj switchcase [arg list (N elements)]           ]
             |                             |                       |
             [@hv_obj __slice 1 -1]        [@hv_obj __slice 1 -1]  |
             |        |                    |          |            |
             [outlet_0]                    [outlet_N-1]            [outlet_right]
         """
 
-        route_graph = {
+        route_graph: Dict = {
             "type": "graph",
             "imports": [],
             "args": [],
             "objects": {
                 "inlet": {
                     "type": "inlet",
                     "args": {
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdSelectObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSelectObject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,57 +11,68 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from collections import Counter
+from typing import Optional, List, Dict
+
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
 class PdSelectObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert obj_type in {"select", "sel"}
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
+
+        if not obj_args:
+            obj_args = []
 
-        if len(obj_args) == 0:
+        if len(self.obj_args) == 0:
             self.add_error("At least one argument is required.")
-        if len(set(obj_args)) != len(obj_args):
+        if len(set(self.obj_args)) != len(obj_args):
             c = Counter(obj_args).most_common(1)
             self.add_error(
                 f"All arguments to [select] must be unique. Argument \"{c[0][0]}\" is repeated {c[0][1]} times.",
                 NotificationEnum.ERROR_UNIQUE_ARGUMENTS_REQUIRED)
 
         # convert to obj_args to mixedarray, such that correct switchcase hash
         # is generated
         for i, a in enumerate(self.obj_args):
             try:
                 self.obj_args[i] = float(a)
             except Exception:
                 pass
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         if len(self._inlet_connections.get("1", [])) > 0:
             self.add_warning("The right inlet of select is not supported. It will not do anything.")
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         """ Creates a graph dynamically based on the number of arguments.
             An unconnected right inlet is added.
 
             [inlet]                                         [inlet]
             |
             [@hv_obj switchcase [arg list (N elements)]           ]
             |                             |                       |
             [@hv_obj __cast_b]            [@hv_obj __cast_b]      |
             |                             |                       |
             [outlet_0]                    [outlet_N-1]            [outlet_right]
         """
 
-        route_graph = {
+        route_graph: Dict = {
             "type": "graph",
             "imports": [],
             "args": [],
             "objects": {
                 "inlet": {
                     "type": "inlet",
                     "args": {
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdSendObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdSendObject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 from .PdRaw import parse_pd_raw_args, PdRawException
 
 
 class PdSendObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert obj_type in {"s", "send", "s~", "send~", "throw~"}
         PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
 
         self.__send_name = ""
         self.__extern_type = None
         self.__attributes = {}
 
@@ -42,17 +51,17 @@
 
         if '@raw' in self.obj_args or '@owl' in self.obj_args:  # TODO(dromer): deprecate @owl on next stable release
             try:
                 pd_raw_args = parse_pd_raw_args(self.obj_args)
                 self.__attributes.update(pd_raw_args)
                 self.__extern_type = "param"  # make sure output code is generated
             except PdRawException as e:
-                self.add_error(e)
+                self.add_error(str(e))
 
-    def validate_configuration(self):
+    def validate_configuration(self) -> None:
         if len(self.obj_args) == 0:
             self.add_warning(
                 f"No name was given to this {self.obj_type} object. "
                 "It should have a name to reduce the risk of errors.",
                 NotificationEnum.WARNING_USELESS_OBJECT)
         if len(self._inlet_connections.get("0", [])) == 0:
             self.add_warning(
@@ -61,15 +70,15 @@
                 NotificationEnum.WARNING_USELESS_OBJECT)
         if self.obj_type in {"s", "send"} and len(self._inlet_connections.get("1", [])) > 0:
             self.add_error(
                 "Connections to the right inlet of a send object "
                 "are not supported. A name should be given.",
                 NotificationEnum.ERROR_MISSING_REQUIRED_ARGUMENT)
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         # note: control rate send/receive objects should not modify their name argument
         names = {
             "s": "",
             "send": "",
             "s~": "sndrcv_sig_",
             "send~": "sndrcv_sig_",
             "throw~": "thrwctch_sig_"
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdTableObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdTableObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
 class PdTableObject(PdObject):
 
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
-        assert obj_type in {"table"}
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        assert obj_type == "table"
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
         self.__table_name = ""
         self.__size = 0
         self.__extern = False
 
         try:
             self.__table_name = self.obj_args[0]
@@ -40,15 +49,15 @@
                 self.__size = int(self.obj_args[1])
                 self.__extern = (self.obj_args[2] == "@hv_table")
             except Exception:
                 pass
         except Exception:
             pass
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         return {
             "type": "table",
             "args": {
                 "name": self.__table_name,
                 "size": self.__size,
                 "values": [],
                 "extern": self.__extern
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdTriggerObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdPackObject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .NotificationEnum import NotificationEnum
 from .PdObject import PdObject
 
 
-class PdTriggerObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
-        assert obj_type in {"trigger", "t"}
-        PdObject.__init__(self, "trigger", obj_args, pos_x, pos_y)
-
-        # convert all numeric casts to "f"
-        for i, a in enumerate(self.obj_args):
-            self.obj_args[i] = "f" if PdTriggerObject.__is_float(a) else a
+class PdPackObject(PdObject):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
+        assert obj_type == "pack"
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
+
+        self.values = []
 
         if len(self.obj_args) == 0:
-            self.obj_args = ["b", "b"]
-            self.add_warning("A trigger with no arguments defualts to [t b b].")
-        if not (set(obj_args) <= set(["a", "f", "s", "b"])):
-            self.add_error(
-                "Heavy only supports arguments 'a', 'f', 's', and 'b'.",
-                NotificationEnum.ERROR_TRIGGER_ABFS)
+            self.values = [0.0, 0.0]
 
-    def to_hv(self):
+        for x in self.obj_args:
+            try:
+                self.values.append(float(x))
+            except Exception:
+                if x in {"f", "float"}:
+                    self.values.append(0.0)
+                else:
+                    self.add_error(
+                        f"\"{x}\" argument to [pack] object not supported.",
+                        NotificationEnum.ERROR_PACK_FLOAT_ARGUMENTS)
+
+    def to_hv(self) -> Dict:
         return {
-            "type": "sequence",
+            "type": "__pack",
             "args": {
-                "casts": self.obj_args
+                "values": self.values
             },
             "properties": {
                 "x": self.pos_x,
                 "y": self.pos_y
             }
         }
-
-    @classmethod
-    def __is_float(clazz, x):
-        """ Returns True if the input can be converted to a float. False otherwise.
-        """
-        try:
-            float(x)
-            return True
-        except Exception:
-            return False
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/PdUnpackObject.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/PdUnpackObject.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Optional, List, Dict
+
 from .PdObject import PdObject
 
 
 class PdUnpackObject(PdObject):
-    def __init__(self, obj_type, obj_args=None, pos_x=0, pos_y=0):
+    def __init__(
+        self,
+        obj_type: str,
+        obj_args: Optional[List] = None,
+        pos_x: int = 0,
+        pos_y: int = 0
+    ) -> None:
         assert obj_type == "unpack"
-        PdObject.__init__(self, obj_type, obj_args, pos_x, pos_y)
+        super().__init__(obj_type, obj_args, pos_x, pos_y)
 
         if len(self.obj_args) == 0:
             self.add_error("Unpack requires at least one argument.")
         if not (set(self.obj_args) <= set(["f", "s"])):
             self.add_warning("Heavy only supports arguments 'f' and 's' to unpack.")
 
-    def to_hv(self):
+    def to_hv(self) -> Dict:
         """ Creates a graph dynamically based on the number of arguments.
 
             [inlet                                                ]
             |                        |      |
             [@hv_obj __slice 0 1]    ...    [@hv_obj __slice N-1 1]
             |                        |      |
             [outlet_0]               ...    [outlet_N-1]
         """
 
-        hv_graph = {
+        hv_graph: Dict = {
             "type": "graph",
             "imports": [],
             "args": [],
             "objects": {
                 "inlet": {
                     "type": "inlet",
                     "args": {
```

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/conv~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy/lorenz~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/heavy_converted/lorenz~.hv.json`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bendin.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bendin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/biquad~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/bp~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/bp~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/change.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/change.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/cos~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cos~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/cpole~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ctlout.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero_rev~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/czero~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/czero~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtopow.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/dbtorms.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delay.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delay.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread4~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delread~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delread~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/delwrite~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/ftom.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/ftom.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/hip~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/hip~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/int.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/int.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/line.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/line.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/lop~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/lop~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/makenote.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/makenote.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/metro.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/metro.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/noise~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/noise~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/notein.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/notein.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/osc~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/osc~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/pgmin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/poly.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/poly.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/powtodb.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/random.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/random.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rmstodb.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/rsqrt~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/samphold~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/sqrt~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/swap.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/swap.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabosc4~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabread.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread4~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabread~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/tabwrite~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/timer.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/timer.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/touchin.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/touchin.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/until.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/until.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/libs/pd/vcf~.pd`

 * *Files identical despite different names*

### Comparing `hvcc-0.6.3/hvcc/interpreters/pd2hv/pd2hv.py` & `hvcc-0.7.0/hvcc/interpreters/pd2hv/pd2hv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (C) 2014-2018 Enzien Audio, Ltd.
+# Copyright (C) 2023 Wasted Audio
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,14 +14,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import json
 import os
 import time
+from typing import Dict, List, Optional
 
 from hvcc.interpreters.pd2hv.PdParser import PdParser
 
 
 class Colours:
     purple = "\033[95m"
     cyan = "\033[96m"
@@ -33,19 +35,27 @@
     underline = "\033[4m"
     end = "\033[0m"
 
 
 class pd2hv:
 
     @classmethod
-    def get_supported_objects(clazz):
+    def get_supported_objects(cls) -> List:
         return PdParser.get_supported_objects()
 
     @classmethod
-    def compile(clazz, pd_path, hv_dir, search_paths=None, verbose=False, export_args=False):
+    def compile(
+        cls,
+        pd_path: str,
+        hv_dir: str,
+        search_paths: Optional[List] = None,
+        verbose: bool = False,
+        export_args: bool = False
+    ) -> Dict:
+
         tick = time.time()
 
         parser = PdParser()  # create parser state
         if search_paths is not None:
             for p in search_paths:
                 parser.add_absolute_search_directory(p)
 
@@ -98,15 +108,15 @@
             "in_file": os.path.basename(pd_path),
             "out_dir": hv_dir,
             "out_file": hv_file,
             "compile_time": (time.time() - tick)
         }
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         description="Converts a Pd patch into the Heavy language format.")
     parser.add_argument(
         "pd_path",
         help="The Pd patch to convert to Heavy.")
     parser.add_argument(
         "hv_dir",
```

### Comparing `hvcc-0.6.3/hvcc/utils.py` & `hvcc-0.7.0/hvcc/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import sys
 import argparse
 import json
 
-import hvcc.core.hv2ir.HeavyLangObject as HeavyLangObject
-import hvcc.interpreters.pd2hv.PdParser as PdParser
+from hvcc.core.hv2ir.HeavyLangObject import HeavyLangObject
+from hvcc.interpreters.pd2hv.PdParser import PdParser
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         description="Some separate heavy utilities, wrapped into a single app")
     subparsers = parser.add_subparsers(dest="command")
     subparsers.add_parser("pdobjects", help="list supported Pure Data objects")
     subparser_hvhash = subparsers.add_parser("hvhash", help="print the heavy hash of the input string")
     subparser_hvhash.add_argument("string")
 
     parsed_args = parser.parse_args(args=None if sys.argv[1:] else ['--help'])
     args = vars(parsed_args)
 
     command = args.pop("command")
     if command == "pdobjects":
-        obj_list = PdParser.PdParser.get_supported_objects()
+        obj_list = PdParser.get_supported_objects()
         obj_list.sort()
 
         obj_dict = {
             "Message Objects": [k for k in obj_list if '~' not in k],
             "Signal Objects": [k for k in obj_list if '~' in k]
         }
         print(json.dumps(obj_dict, indent=4))
     elif command == "hvhash":
-        print("0x{0:X}".format(HeavyLangObject.HeavyLangObject.get_hash(args.get('string'))))
+        print("0x{0:X}".format(HeavyLangObject.get_hash(args['string'])))
     else:
         pass
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hvcc-0.6.3/hvcc.egg-info/PKG-INFO` & `hvcc-0.7.0/hvcc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hvcc
-Version: 0.6.3
+Version: 0.7.0
 Summary: `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 Home-page: https://github.com/Wasted-Audio/hvcc
-Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.6.3.tar.gz
+Download-URL: https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.7.0.tar.gz
 Author: Enzien Audio, Wasted Audio
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Compilers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hvcc-0.6.3/hvcc.egg-info/SOURCES.txt` & `hvcc-0.7.0/hvcc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,38 +53,35 @@
 hvcc/core/hv2ir/HeavyParser.py
 hvcc/core/hv2ir/LocalVars.py
 hvcc/core/hv2ir/__init__.py
 hvcc/core/hv2ir/hv2ir.py
 hvcc/core/json/heavy.ir.json
 hvcc/core/json/heavy.lang.json
 hvcc/generators/__init__.py
+hvcc/generators/filters.py
 hvcc/generators/buildjson/__init__.py
 hvcc/generators/buildjson/buildjson.py
-hvcc/generators/c2bela/SETUP.md
-hvcc/generators/c2bela/__init__.py
-hvcc/generators/c2bela/c2bela.py
-hvcc/generators/c2bela/templates/linux/Makefile
 hvcc/generators/c2daisy/__init__.py
 hvcc/generators/c2daisy/c2daisy.py
 hvcc/generators/c2daisy/parameters.py
-hvcc/generators/c2daisy/boards/pod.json
-hvcc/generators/c2daisy/boards/versio.json
 hvcc/generators/c2daisy/static/README.md
 hvcc/generators/c2daisy/templates/HeavyDaisy.cpp
 hvcc/generators/c2daisy/templates/Makefile
 hvcc/generators/c2dpf/__init__.py
 hvcc/generators/c2dpf/c2dpf.py
 hvcc/generators/c2dpf/static/README.md
 hvcc/generators/c2dpf/templates/DistrhoPluginInfo.h
 hvcc/generators/c2dpf/templates/HeavyDPF.cpp
 hvcc/generators/c2dpf/templates/HeavyDPF.hpp
-hvcc/generators/c2dpf/templates/Makefile
-hvcc/generators/c2dpf/templates/Makefile.project
+hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Input.cpp
+hvcc/generators/c2dpf/templates/HeavyDPF_MIDI_Output.cpp
+hvcc/generators/c2dpf/templates/HeavyDPF_PortGroups.cpp
+hvcc/generators/c2dpf/templates/HeavyDPF_UI.cpp
+hvcc/generators/c2dpf/templates/Makefile_plugin
 hvcc/generators/c2dpf/templates/Makefile_project
-hvcc/generators/c2dpf/templates/x42_clock_ticks.txt
 hvcc/generators/c2fabric/__init__.py
 hvcc/generators/c2fabric/c2fabric.py
 hvcc/generators/c2fabric/templates/android/jni/Android.mk
 hvcc/generators/c2fabric/templates/android/jni/Application.mk
 hvcc/generators/c2fabric/templates/linux/Makefile
 hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSP.cs
 hvcc/generators/c2fabric/templates/source/fabric/Hv_{{name}}_FabricDSPEditor.cs
@@ -105,15 +102,14 @@
 hvcc/generators/c2owl/templates/HeavyOwl.hpp
 hvcc/generators/c2owl/templates/HeavyOwlConstants.h
 hvcc/generators/c2pdext/__init__.py
 hvcc/generators/c2pdext/c2pdext.py
 hvcc/generators/c2pdext/static/m_pd.h
 hvcc/generators/c2pdext/templates/pd_external.c
 hvcc/generators/c2pdext/templates/project.pbxproj
-hvcc/generators/c2rack/static/README.md
 hvcc/generators/c2unity/__init__.py
 hvcc/generators/c2unity/c2unity.py
 hvcc/generators/c2unity/static/source/unity/AudioPluginInterface.h
 hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.cpp
 hvcc/generators/c2unity/static/source/unity/AudioPluginUtil.h
 hvcc/generators/c2unity/static/xcode/Info.plist
 hvcc/generators/c2unity/templates/android/jni/Android.mk
@@ -415,15 +411,14 @@
 hvcc/interpreters/pd2hv/libs/pd/moses.pd
 hvcc/interpreters/pd2hv/libs/pd/mtof.pd
 hvcc/interpreters/pd2hv/libs/pd/mtof~.pd
 hvcc/interpreters/pd2hv/libs/pd/nbx.pd
 hvcc/interpreters/pd2hv/libs/pd/noise~.pd
 hvcc/interpreters/pd2hv/libs/pd/notein.pd
 hvcc/interpreters/pd2hv/libs/pd/noteout.pd
-hvcc/interpreters/pd2hv/libs/pd/noteout.pd-test
 hvcc/interpreters/pd2hv/libs/pd/osc~.pd
 hvcc/interpreters/pd2hv/libs/pd/pgmin.pd
 hvcc/interpreters/pd2hv/libs/pd/pgmout.pd
 hvcc/interpreters/pd2hv/libs/pd/phasor~.pd
 hvcc/interpreters/pd2hv/libs/pd/pipe.pd
 hvcc/interpreters/pd2hv/libs/pd/poly.pd
 hvcc/interpreters/pd2hv/libs/pd/polytouchin.pd
```

### Comparing `hvcc-0.6.3/setup.cfg` & `hvcc-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = hvcc
-version = 0.6.3
+version = 0.7.0
 license = GPLv3
 author = Enzien Audio, Wasted Audio
 description = `hvcc` is a python-based dataflow audio programming language compiler that generates C/C++ code and a variety of specific framework wrappers.
 url = https://github.com/Wasted-Audio/hvcc
-download_url = https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.6.3.tar.gz
+download_url = https://github.com/Wasted-Audio/hvcc/archive/refs/tags/v0.7.0.tar.gz
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Topic :: Software Development :: Compilers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

