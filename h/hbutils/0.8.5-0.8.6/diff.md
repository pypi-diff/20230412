# Comparing `tmp/hbutils-0.8.5.tar.gz` & `tmp/hbutils-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbutils-0.8.5.tar", last modified: Sun Apr  9 07:05:29 2023, max compression
+gzip compressed data, was "hbutils-0.8.6.tar", last modified: Wed Apr 12 11:05:23 2023, max compression
```

## Comparing `hbutils-0.8.5.tar` & `hbutils-0.8.6.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.412520 hbutils-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 07:03:11.000000 hbutils-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-09 07:05:29.412520 hbutils-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-09 07:03:11.000000 hbutils-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.380519 hbutils-0.8.5/hbutils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.384520 hbutils-0.8.5/hbutils/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/algorithm/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/algorithm/topological.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.384520 hbutils-0.8.5/hbutils/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/binary/uint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.388520 hbutils-0.8.5/hbutils/collection/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/collection/structural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.388520 hbutils-0.8.5/hbutils/color/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/color/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/color/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/color/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.388520 hbutils-0.8.5/hbutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.388520 hbutils-0.8.5/hbutils/design/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/design/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/design/final.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/design/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/design/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.392520 hbutils-0.8.5/hbutils/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/encoding/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/encoding/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/encoding/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/encoding/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.392520 hbutils-0.8.5/hbutils/expression/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.392520 hbutils-0.8.5/hbutils/expression/native/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/expression/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/expression/native/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/expression/native/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/expression/native/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.392520 hbutils-0.8.5/hbutils/file/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/file/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.396520 hbutils-0.8.5/hbutils/model/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/clazz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/model/repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.396520 hbutils-0.8.5/hbutils/random/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/random/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/random/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/random/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/random/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.396520 hbutils-0.8.5/hbutils/reflection/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/clazz.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/reflection/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.400520 hbutils-0.8.5/hbutils/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/scale/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/scale/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.400520 hbutils-0.8.5/hbutils/string/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/string/inflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/string/plural.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/string/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/string/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/string/trunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.400520 hbutils-0.8.5/hbutils/system/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.400520 hbutils-0.8.5/hbutils/system/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/filesystem/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/filesystem/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/filesystem/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/filesystem/tempfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.404520 hbutils-0.8.5/hbutils/system/network/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/network/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/network/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/network/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.404520 hbutils-0.8.5/hbutils/system/os/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/os/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/os/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.404520 hbutils-0.8.5/hbutils/system/python/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/python/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/system/python/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.404520 hbutils-0.8.5/hbutils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.404520 hbutils-0.8.5/hbutils/testing/capture/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/capture/exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/capture/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.408520 hbutils-0.8.5/hbutils/testing/compare/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/compare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/compare/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.408520 hbutils-0.8.5/hbutils/testing/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/generator/aetg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/generator/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/generator/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.408520 hbutils-0.8.5/hbutils/testing/isolated/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/isolated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/isolated/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/isolated/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/isolated/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/isolated/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.412520 hbutils-0.8.5/hbutils/testing/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/requires/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/requires/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/requires/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.412520 hbutils-0.8.5/hbutils/testing/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-09 07:03:11.000000 hbutils-0.8.5/hbutils/testing/simulate/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:29.380519 hbutils-0.8.5/hbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-09 07:05:29.000000 hbutils-0.8.5/hbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-09 07:05:29.000000 hbutils-0.8.5/hbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:05:29.000000 hbutils-0.8.5/hbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 07:05:29.000000 hbutils-0.8.5/hbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 07:05:29.000000 hbutils-0.8.5/hbutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 07:05:29.412520 hbutils-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-09 07:03:11.000000 hbutils-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.657892 hbutils-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 11:03:12.000000 hbutils-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-12 11:05:23.657892 hbutils-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-12 11:03:12.000000 hbutils-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.621891 hbutils-0.8.6/hbutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.621891 hbutils-0.8.6/hbutils/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/algorithm/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/algorithm/topological.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.625891 hbutils-0.8.6/hbutils/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/binary/uint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.629891 hbutils-0.8.6/hbutils/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/collection/structural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.629891 hbutils-0.8.6/hbutils/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/color/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/color/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/color/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.633891 hbutils-0.8.6/hbutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.633891 hbutils-0.8.6/hbutils/design/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/design/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/design/final.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/design/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/design/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.633891 hbutils-0.8.6/hbutils/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/encoding/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/encoding/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/encoding/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/encoding/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.633891 hbutils-0.8.6/hbutils/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.637891 hbutils-0.8.6/hbutils/expression/native/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/expression/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/expression/native/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/expression/native/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/expression/native/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.637891 hbutils-0.8.6/hbutils/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/file/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.637891 hbutils-0.8.6/hbutils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/model/repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.637891 hbutils-0.8.6/hbutils/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/random/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/random/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/random/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/random/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.641891 hbutils-0.8.6/hbutils/reflection/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/reflection/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.641891 hbutils-0.8.6/hbutils/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/scale/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/scale/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.645892 hbutils-0.8.6/hbutils/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/string/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/string/plural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/string/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/string/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/string/trunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.645892 hbutils-0.8.6/hbutils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.645892 hbutils-0.8.6/hbutils/system/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/filesystem/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/filesystem/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/filesystem/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/filesystem/tempfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.649891 hbutils-0.8.6/hbutils/system/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/network/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/network/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/network/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.649891 hbutils-0.8.6/hbutils/system/os/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/os/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/os/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.649891 hbutils-0.8.6/hbutils/system/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/python/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/system/python/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.649891 hbutils-0.8.6/hbutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.649891 hbutils-0.8.6/hbutils/testing/capture/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/capture/exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/capture/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.649891 hbutils-0.8.6/hbutils/testing/compare/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/compare/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.653892 hbutils-0.8.6/hbutils/testing/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/generator/aetg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/generator/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/generator/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.653892 hbutils-0.8.6/hbutils/testing/isolated/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/isolated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/isolated/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/isolated/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/isolated/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/isolated/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.653892 hbutils-0.8.6/hbutils/testing/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/requires/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/requires/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/requires/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.653892 hbutils-0.8.6/hbutils/testing/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-12 11:03:12.000000 hbutils-0.8.6/hbutils/testing/simulate/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:05:23.621891 hbutils-0.8.6/hbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-12 11:05:23.000000 hbutils-0.8.6/hbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-12 11:05:23.000000 hbutils-0.8.6/hbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:05:23.000000 hbutils-0.8.6/hbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-12 11:05:23.000000 hbutils-0.8.6/hbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 11:05:23.000000 hbutils-0.8.6/hbutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:05:23.657892 hbutils-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-12 11:03:12.000000 hbutils-0.8.6/setup.py
```

### Comparing `hbutils-0.8.5/LICENSE` & `hbutils-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/PKG-INFO` & `hbutils-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbutils
-Version: 0.8.5
+Version: 0.8.6
 Summary: Some useful functions and classes in Python infrastructure development.
 Home-page: https://github.com/hansbug/hbutils
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hbutils-0.8.5/README.md` & `hbutils-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/algorithm/linear.py` & `hbutils-0.8.6/hbutils/algorithm/linear.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/algorithm/topological.py` & `hbutils-0.8.6/hbutils/algorithm/topological.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/base.py` & `hbutils-0.8.6/hbutils/binary/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/bool.py` & `hbutils-0.8.6/hbutils/binary/bool.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/buffer.py` & `hbutils-0.8.6/hbutils/binary/buffer.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/float.py` & `hbutils-0.8.6/hbutils/binary/float.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/int.py` & `hbutils-0.8.6/hbutils/binary/int.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/str.py` & `hbutils-0.8.6/hbutils/binary/str.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/binary/uint.py` & `hbutils-0.8.6/hbutils/binary/uint.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/collection/dimension.py` & `hbutils-0.8.6/hbutils/collection/dimension.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/collection/functional.py` & `hbutils-0.8.6/hbutils/collection/functional.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/collection/recover.py` & `hbutils-0.8.6/hbutils/collection/recover.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/collection/sequence.py` & `hbutils-0.8.6/hbutils/collection/sequence.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/collection/stacked.py` & `hbutils-0.8.6/hbutils/collection/stacked.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/collection/structural.py` & `hbutils-0.8.6/hbutils/collection/structural.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/color/base.py` & `hbutils-0.8.6/hbutils/color/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/color/model.py` & `hbutils-0.8.6/hbutils/color/model.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/color/utils.py` & `hbutils-0.8.6/hbutils/color/utils.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/design/decorator.py` & `hbutils-0.8.6/hbutils/design/decorator.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/design/final.py` & `hbutils-0.8.6/hbutils/design/final.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/design/observer.py` & `hbutils-0.8.6/hbutils/design/observer.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/design/singleton.py` & `hbutils-0.8.6/hbutils/design/singleton.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/encoding/ansi.py` & `hbutils-0.8.6/hbutils/encoding/ansi.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/encoding/base64.py` & `hbutils-0.8.6/hbutils/encoding/base64.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/encoding/decode.py` & `hbutils-0.8.6/hbutils/encoding/decode.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/encoding/hash.py` & `hbutils-0.8.6/hbutils/encoding/hash.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/expression/native/base.py` & `hbutils-0.8.6/hbutils/expression/native/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/expression/native/feature.py` & `hbutils-0.8.6/hbutils/expression/native/feature.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/expression/native/general.py` & `hbutils-0.8.6/hbutils/expression/native/general.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/file/stream.py` & `hbutils-0.8.6/hbutils/file/stream.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/model/clazz.py` & `hbutils-0.8.6/hbutils/model/clazz.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/model/compare.py` & `hbutils-0.8.6/hbutils/model/compare.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/model/enum.py` & `hbutils-0.8.6/hbutils/model/enum.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/model/raw.py` & `hbutils-0.8.6/hbutils/model/raw.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/model/repr.py` & `hbutils-0.8.6/hbutils/model/repr.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/random/binary.py` & `hbutils-0.8.6/hbutils/random/binary.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/random/sequence.py` & `hbutils-0.8.6/hbutils/random/sequence.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/random/state.py` & `hbutils-0.8.6/hbutils/random/state.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/random/string.py` & `hbutils-0.8.6/hbutils/random/string.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/clazz.py` & `hbutils-0.8.6/hbutils/reflection/clazz.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/context.py` & `hbutils-0.8.6/hbutils/reflection/context.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/exception.py` & `hbutils-0.8.6/hbutils/reflection/exception.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/func.py` & `hbutils-0.8.6/hbutils/reflection/func.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/imports.py` & `hbutils-0.8.6/hbutils/reflection/imports.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/iter.py` & `hbutils-0.8.6/hbutils/reflection/iter.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/reflection/module.py` & `hbutils-0.8.6/hbutils/reflection/module.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/scale/size.py` & `hbutils-0.8.6/hbutils/scale/size.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/scale/time.py` & `hbutils-0.8.6/hbutils/scale/time.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/string/inflection.py` & `hbutils-0.8.6/hbutils/string/inflection.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/string/plural.py` & `hbutils-0.8.6/hbutils/string/plural.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/string/template.py` & `hbutils-0.8.6/hbutils/string/template.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/string/tree.py` & `hbutils-0.8.6/hbutils/string/tree.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/string/trunc.py` & `hbutils-0.8.6/hbutils/string/trunc.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/filesystem/binary.py` & `hbutils-0.8.6/hbutils/system/filesystem/binary.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/filesystem/directory.py` & `hbutils-0.8.6/hbutils/system/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/filesystem/file.py` & `hbutils-0.8.6/hbutils/system/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/filesystem/tempfile.py` & `hbutils-0.8.6/hbutils/system/filesystem/tempfile.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/network/hosts.py` & `hbutils-0.8.6/hbutils/system/network/hosts.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/network/port.py` & `hbutils-0.8.6/hbutils/system/network/port.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/network/url.py` & `hbutils-0.8.6/hbutils/system/network/url.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/os/executable.py` & `hbutils-0.8.6/hbutils/system/os/executable.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/os/type.py` & `hbutils-0.8.6/hbutils/system/os/type.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/python/implementation.py` & `hbutils-0.8.6/hbutils/system/python/implementation.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/system/python/package.py` & `hbutils-0.8.6/hbutils/system/python/package.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/capture/exit.py` & `hbutils-0.8.6/hbutils/testing/capture/exit.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/capture/output.py` & `hbutils-0.8.6/hbutils/testing/capture/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,23 +127,25 @@
     """
     mock_func = _capture_via_memory if mem else _capture_via_tempfile
     with mock_func() as co:
         yield co
 
 
 @contextmanager
-def disable_output() -> ContextManager[OutputCaptureResult]:
+def disable_output(encoding='utf-8') -> ContextManager[OutputCaptureResult]:
     """
     Overview:
         Disable all the output to ``sys.stdout`` and ``sys.stderr`` in this ``with`` block.
 
+    :param encoding: Encoding of null file, default is ``utf-8``.
+
     Examples::
         >>> import sys
         >>> from hbutils.testing import disable_output
         >>>
         >>> with disable_output():  # no output will be shown
         ...     print('this is stdout')
         ...     print('this is stderr', file=sys.stderr)
     """
-    with open(os.devnull, 'w') as sout:
+    with open(os.devnull, 'w', encoding=encoding) as sout:
         with redirect_stdout(sout), redirect_stderr(sout):
             yield
```

### Comparing `hbutils-0.8.5/hbutils/testing/compare/text.py` & `hbutils-0.8.6/hbutils/testing/compare/text.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/generator/aetg.py` & `hbutils-0.8.6/hbutils/testing/generator/aetg.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/generator/base.py` & `hbutils-0.8.6/hbutils/testing/generator/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/generator/func.py` & `hbutils-0.8.6/hbutils/testing/generator/func.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/generator/matrix.py` & `hbutils-0.8.6/hbutils/testing/generator/matrix.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/isolated/directory.py` & `hbutils-0.8.6/hbutils/testing/isolated/directory.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/isolated/entry_point.py` & `hbutils-0.8.6/hbutils/testing/isolated/entry_point.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/isolated/input.py` & `hbutils-0.8.6/hbutils/testing/isolated/input.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/isolated/logging.py` & `hbutils-0.8.6/hbutils/testing/isolated/logging.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/requires/cmd.py` & `hbutils-0.8.6/hbutils/testing/requires/cmd.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/requires/expr.py` & `hbutils-0.8.6/hbutils/testing/requires/expr.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/requires/version.py` & `hbutils-0.8.6/hbutils/testing/requires/version.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils/testing/simulate/entry.py` & `hbutils-0.8.6/hbutils/testing/simulate/entry.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils.egg-info/PKG-INFO` & `hbutils-0.8.6/hbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbutils
-Version: 0.8.5
+Version: 0.8.6
 Summary: Some useful functions and classes in Python infrastructure development.
 Home-page: https://github.com/hansbug/hbutils
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hbutils-0.8.5/hbutils.egg-info/SOURCES.txt` & `hbutils-0.8.6/hbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.5/hbutils.egg-info/requires.txt` & `hbutils-0.8.6/hbutils.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pytest-xdist>=1.34.0
 pytest-rerunfailures~=10.2
 pytest-timeout~=2.0.2
 easydict<2,>=1.7
 click>=7.0.0
 requests>=2.20
 testtools>=2
+tqdm
 
 [test:implementation_name != "pypy" or platform_system != "Windows" or python_version >= "3.8"]
 numpy>=1.20
 
 [test:python_version < "3.11" and implementation_name != "pypy"]
 torch>=1.1.0
```

### Comparing `hbutils-0.8.5/setup.py` & `hbutils-0.8.6/setup.py`

 * *Files identical despite different names*

