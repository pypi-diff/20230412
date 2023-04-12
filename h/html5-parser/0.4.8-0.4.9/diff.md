# Comparing `tmp/html5-parser-0.4.8.tar.gz` & `tmp/html5-parser-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/html5-parser-0.4.8.tar", last modified: Thu Jul 25 06:04:47 2019, max compression
+gzip compressed data, was "dist/html5-parser-0.4.9.tar", last modified: Sun Nov  3 03:14:21 2019, max compression
```

## Comparing `html5-parser-0.4.8.tar` & `html5-parser-0.4.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-07-25 06:04:47.000000 html5-parser-0.4.8/
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2450 2017-06-10 03:00:55.000000 html5-parser-0.4.8/gentags.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      189 2017-07-28 04:44:30.000000 html5-parser-0.4.8/MANIFEST.in
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2599 2017-06-07 17:01:19.000000 html5-parser-0.4.8/setup.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      860 2019-07-25 06:04:47.000000 html5-parser-0.4.8/PKG-INFO
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-07-25 06:04:47.000000 html5-parser-0.4.8/gumbo/
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10328 2017-11-07 05:47:17.000000 html5-parser-0.4.8/gumbo/utf8.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7771 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/error.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3737 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/tokenizer_states.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4750 2017-06-13 11:23:21.000000 html5-parser-0.4.8/gumbo/tag_enum.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2689 2017-07-25 08:58:18.000000 html5-parser-0.4.8/gumbo/attribute.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10115 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/error.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)   129364 2017-07-25 05:47:25.000000 html5-parser-0.4.8/gumbo/char_ref.rl
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3495 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/vector.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4938 2017-11-07 05:47:47.000000 html5-parser-0.4.8/gumbo/utf8.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9021 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/gumbo_edit.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)   750568 2017-07-25 09:00:19.000000 html5-parser-0.4.8/gumbo/char_ref.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)      308 2017-11-07 04:56:10.000000 html5-parser-0.4.8/gumbo/replacement.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2049 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/parser.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)    14643 2017-06-13 11:23:22.000000 html5-parser-0.4.8/gumbo/tag_perf.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1170 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/string_piece.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1897 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/insertion_mode.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2686 2017-06-13 11:23:21.000000 html5-parser-0.4.8/gumbo/tag_strings.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)   118676 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/tokenizer.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1255 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/attribute.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3149 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/string_buffer.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)   184604 2018-10-10 05:30:36.000000 html5-parser-0.4.8/gumbo/parser.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3037 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/tag.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4608 2017-07-27 18:29:35.000000 html5-parser-0.4.8/gumbo/tokenizer.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1469 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/util.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4440 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/string_buffer.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2033 2017-06-05 12:03:56.000000 html5-parser-0.4.8/gumbo/util.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10862 2017-11-07 05:24:23.000000 html5-parser-0.4.8/gumbo/svg_attrs.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2219 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/char_ref.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1109 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/token_type.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)      872 2017-06-13 11:23:21.000000 html5-parser-0.4.8/gumbo/tag_sizes.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5224 2017-06-04 00:44:31.000000 html5-parser-0.4.8/gumbo/gumbo_edit.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2169 2017-05-31 14:57:06.000000 html5-parser-0.4.8/gumbo/vector.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)    23466 2017-11-07 05:46:36.000000 html5-parser-0.4.8/gumbo/gumbo.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8858 2017-11-07 05:20:46.000000 html5-parser-0.4.8/gumbo/svg_tags.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1484 2017-07-25 08:58:29.000000 html5-parser-0.4.8/gumbo/string_piece.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1097 2017-06-14 15:12:46.000000 html5-parser-0.4.8/README.rst
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3564 2017-07-27 17:24:23.000000 html5-parser-0.4.8/run_tests.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-07-25 06:04:47.000000 html5-parser-0.4.8/test/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4326 2019-05-23 12:30:55.000000 html5-parser-0.4.8/test/adapt.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4275 2017-07-27 18:39:37.000000 html5-parser-0.4.8/test/basic.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      754 2018-10-10 05:30:36.000000 html5-parser-0.4.8/test/malformed.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      711 2017-06-13 09:16:26.000000 html5-parser-0.4.8/test/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9530 2017-07-27 18:44:25.000000 html5-parser-0.4.8/test/html5lib_adapter.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7988 2017-06-13 06:16:57.000000 html5-parser-0.4.8/test/namespace.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3096 2019-05-23 12:30:55.000000 html5-parser-0.4.8/test/soup.py
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     3471 2017-07-05 09:19:25.000000 html5-parser-0.4.8/genattrs.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7509 2017-07-27 15:48:34.000000 html5-parser-0.4.8/win-ci.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-07-25 06:04:47.000000 html5-parser-0.4.8/src/
--rw-r--r--   0 kovid     (1000) kovid     (1000)    24518 2017-07-05 09:19:33.000000 html5-parser-0.4.8/src/attr_perf.h
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-07-25 06:04:47.000000 html5-parser-0.4.8/src/html5_parser.egg-info/
--rw-r--r--   0 kovid     (1000) kovid     (1000)      860 2019-07-25 06:04:46.000000 html5-parser-0.4.8/src/html5_parser.egg-info/PKG-INFO
--rw-r--r--   0 kovid     (1000) kovid     (1000)       13 2019-07-25 06:04:46.000000 html5-parser-0.4.8/src/html5_parser.egg-info/top_level.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2019-07-25 06:04:46.000000 html5-parser-0.4.8/src/html5_parser.egg-info/dependency_links.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)       43 2019-07-25 06:04:46.000000 html5-parser-0.4.8/src/html5_parser.egg-info/requires.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1420 2019-07-25 06:04:46.000000 html5-parser-0.4.8/src/html5_parser.egg-info/SOURCES.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2044 2017-07-05 08:33:29.000000 html5-parser-0.4.8/src/data-types.h
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-07-25 06:04:47.000000 html5-parser-0.4.8/src/html5_parser/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     6326 2017-06-13 14:11:49.000000 html5-parser-0.4.8/src/html5_parser/encoding_names.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1525 2017-06-06 18:09:03.000000 html5-parser-0.4.8/src/html5_parser/stdlib_etree.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    11618 2017-06-13 15:25:31.000000 html5-parser-0.4.8/src/html5_parser/encoding_parser.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8012 2017-07-27 15:44:32.000000 html5-parser-0.4.8/src/html5_parser/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2633 2017-06-06 15:52:48.000000 html5-parser-0.4.8/src/html5_parser/dom.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4216 2019-07-25 06:04:21.000000 html5-parser-0.4.8/src/html5_parser/soup.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7034 2017-11-07 05:28:50.000000 html5-parser-0.4.8/src/as-python-tree.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     6813 2019-07-25 06:04:21.000000 html5-parser-0.4.8/src/python-wrapper.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4734 2017-07-05 09:19:27.000000 html5-parser-0.4.8/src/attr_strings.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)    15893 2018-04-27 01:26:09.000000 html5-parser-0.4.8/src/as-libxml.c
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1298 2017-07-05 09:19:27.000000 html5-parser-0.4.8/src/attr_sizes.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)      433 2017-07-05 16:54:32.000000 html5-parser-0.4.8/src/as-python-tree.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1689 2017-06-08 15:51:40.000000 html5-parser-0.4.8/src/stack.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7694 2017-07-05 09:19:27.000000 html5-parser-0.4.8/src/attr_enum.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)      409 2017-06-07 05:10:59.000000 html5-parser-0.4.8/src/as-libxml.h
--rw-r--r--   0 kovid     (1000) kovid     (1000)    11357 2017-06-01 05:40:16.000000 html5-parser-0.4.8/LICENSE
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     1197 2017-06-13 14:11:40.000000 html5-parser-0.4.8/genencodings.py
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)    10924 2018-09-21 06:13:20.000000 html5-parser-0.4.8/build.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      362 2019-07-25 06:04:47.000000 html5-parser-0.4.8/setup.cfg
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-11-03 03:14:21.000000 html5-parser-0.4.9/
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2450 2017-06-10 03:00:55.000000 html5-parser-0.4.9/gentags.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      189 2017-07-28 04:44:30.000000 html5-parser-0.4.9/MANIFEST.in
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2599 2017-06-07 17:01:19.000000 html5-parser-0.4.9/setup.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      860 2019-11-03 03:14:21.000000 html5-parser-0.4.9/PKG-INFO
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-11-03 03:14:20.000000 html5-parser-0.4.9/gumbo/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10328 2017-11-07 05:47:17.000000 html5-parser-0.4.9/gumbo/utf8.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7771 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/error.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3737 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/tokenizer_states.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4750 2017-06-13 11:23:21.000000 html5-parser-0.4.9/gumbo/tag_enum.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2689 2017-07-25 08:58:18.000000 html5-parser-0.4.9/gumbo/attribute.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10115 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/error.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)   129364 2017-07-25 05:47:25.000000 html5-parser-0.4.9/gumbo/char_ref.rl
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3495 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/vector.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4938 2017-11-07 05:47:47.000000 html5-parser-0.4.9/gumbo/utf8.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9021 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/gumbo_edit.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)   750568 2017-07-25 09:00:19.000000 html5-parser-0.4.9/gumbo/char_ref.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      308 2017-11-07 04:56:10.000000 html5-parser-0.4.9/gumbo/replacement.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2049 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/parser.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    14643 2017-06-13 11:23:22.000000 html5-parser-0.4.9/gumbo/tag_perf.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1170 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/string_piece.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1897 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/insertion_mode.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2686 2017-06-13 11:23:21.000000 html5-parser-0.4.9/gumbo/tag_strings.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)   118676 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/tokenizer.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1255 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/attribute.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3149 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/string_buffer.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)   184604 2018-10-10 05:30:36.000000 html5-parser-0.4.9/gumbo/parser.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3037 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/tag.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4608 2017-07-27 18:29:35.000000 html5-parser-0.4.9/gumbo/tokenizer.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1469 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/util.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4440 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/string_buffer.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2033 2017-06-05 12:03:56.000000 html5-parser-0.4.9/gumbo/util.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10862 2017-11-07 05:24:23.000000 html5-parser-0.4.9/gumbo/svg_attrs.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2219 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/char_ref.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1109 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/token_type.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      872 2017-06-13 11:23:21.000000 html5-parser-0.4.9/gumbo/tag_sizes.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5224 2017-06-04 00:44:31.000000 html5-parser-0.4.9/gumbo/gumbo_edit.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2169 2017-05-31 14:57:06.000000 html5-parser-0.4.9/gumbo/vector.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    23466 2017-11-07 05:46:36.000000 html5-parser-0.4.9/gumbo/gumbo.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8858 2017-11-07 05:20:46.000000 html5-parser-0.4.9/gumbo/svg_tags.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1484 2017-07-25 08:58:29.000000 html5-parser-0.4.9/gumbo/string_piece.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1097 2017-06-14 15:12:46.000000 html5-parser-0.4.9/README.rst
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3564 2017-07-27 17:24:23.000000 html5-parser-0.4.9/run_tests.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-11-03 03:14:21.000000 html5-parser-0.4.9/test/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4326 2019-05-23 12:30:55.000000 html5-parser-0.4.9/test/adapt.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4275 2017-07-27 18:39:37.000000 html5-parser-0.4.9/test/basic.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      754 2018-10-10 05:30:36.000000 html5-parser-0.4.9/test/malformed.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      711 2017-06-13 09:16:26.000000 html5-parser-0.4.9/test/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9530 2017-07-27 18:44:25.000000 html5-parser-0.4.9/test/html5lib_adapter.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8363 2019-11-03 03:13:57.000000 html5-parser-0.4.9/test/namespace.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3096 2019-05-23 12:30:55.000000 html5-parser-0.4.9/test/soup.py
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     3471 2017-07-05 09:19:25.000000 html5-parser-0.4.9/genattrs.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7509 2017-07-27 15:48:34.000000 html5-parser-0.4.9/win-ci.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-11-03 03:14:21.000000 html5-parser-0.4.9/src/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    24518 2017-07-05 09:19:33.000000 html5-parser-0.4.9/src/attr_perf.h
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-11-03 03:14:21.000000 html5-parser-0.4.9/src/html5_parser.egg-info/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      860 2019-11-03 03:14:20.000000 html5-parser-0.4.9/src/html5_parser.egg-info/PKG-INFO
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       13 2019-11-03 03:14:20.000000 html5-parser-0.4.9/src/html5_parser.egg-info/top_level.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2019-11-03 03:14:20.000000 html5-parser-0.4.9/src/html5_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       43 2019-11-03 03:14:20.000000 html5-parser-0.4.9/src/html5_parser.egg-info/requires.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1420 2019-11-03 03:14:20.000000 html5-parser-0.4.9/src/html5_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2044 2017-07-05 08:33:29.000000 html5-parser-0.4.9/src/data-types.h
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2019-11-03 03:14:21.000000 html5-parser-0.4.9/src/html5_parser/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     6326 2017-06-13 14:11:49.000000 html5-parser-0.4.9/src/html5_parser/encoding_names.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1525 2017-06-06 18:09:03.000000 html5-parser-0.4.9/src/html5_parser/stdlib_etree.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    11618 2017-06-13 15:25:31.000000 html5-parser-0.4.9/src/html5_parser/encoding_parser.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8012 2017-07-27 15:44:32.000000 html5-parser-0.4.9/src/html5_parser/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2633 2017-06-06 15:52:48.000000 html5-parser-0.4.9/src/html5_parser/dom.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4216 2019-07-25 06:04:21.000000 html5-parser-0.4.9/src/html5_parser/soup.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7034 2017-11-07 05:28:50.000000 html5-parser-0.4.9/src/as-python-tree.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     6813 2019-11-03 03:13:57.000000 html5-parser-0.4.9/src/python-wrapper.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4734 2017-07-05 09:19:27.000000 html5-parser-0.4.9/src/attr_strings.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    15828 2019-11-03 03:13:57.000000 html5-parser-0.4.9/src/as-libxml.c
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1298 2017-07-05 09:19:27.000000 html5-parser-0.4.9/src/attr_sizes.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      433 2017-07-05 16:54:32.000000 html5-parser-0.4.9/src/as-python-tree.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1689 2017-06-08 15:51:40.000000 html5-parser-0.4.9/src/stack.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7694 2017-07-05 09:19:27.000000 html5-parser-0.4.9/src/attr_enum.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      409 2017-06-07 05:10:59.000000 html5-parser-0.4.9/src/as-libxml.h
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    11357 2017-06-01 05:40:16.000000 html5-parser-0.4.9/LICENSE
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     1197 2017-06-13 14:11:40.000000 html5-parser-0.4.9/genencodings.py
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)    10924 2018-09-21 06:13:20.000000 html5-parser-0.4.9/build.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      362 2019-11-03 03:14:21.000000 html5-parser-0.4.9/setup.cfg
```

### Comparing `html5-parser-0.4.8/gentags.py` & `html5-parser-0.4.9/gentags.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/setup.py` & `html5-parser-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/PKG-INFO` & `html5-parser-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: html5-parser
-Version: 0.4.8
+Version: 0.4.9
 Summary: Fast C based HTML 5 parsing for python
 Home-page: https://html5-parser.readthedocs.io
 Author: Kovid Goyal
 Author-email: redacted@acme.com
 License: Apache 2.0
-Download-URL: https://pypi.python.org/packages/source/m/html5-parser/html5-parser-0.4.8.tar.gz
+Download-URL: https://pypi.python.org/packages/source/m/html5-parser/html5-parser-0.4.9.tar.gz
 Description: UNKNOWN
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `html5-parser-0.4.8/gumbo/utf8.c` & `html5-parser-0.4.9/gumbo/utf8.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/error.h` & `html5-parser-0.4.9/gumbo/error.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tokenizer_states.h` & `html5-parser-0.4.9/gumbo/tokenizer_states.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tag_enum.h` & `html5-parser-0.4.9/gumbo/tag_enum.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/attribute.c` & `html5-parser-0.4.9/gumbo/attribute.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/error.c` & `html5-parser-0.4.9/gumbo/error.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/char_ref.rl` & `html5-parser-0.4.9/gumbo/char_ref.rl`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/vector.c` & `html5-parser-0.4.9/gumbo/vector.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/utf8.h` & `html5-parser-0.4.9/gumbo/utf8.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/gumbo_edit.c` & `html5-parser-0.4.9/gumbo/gumbo_edit.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/char_ref.c` & `html5-parser-0.4.9/gumbo/char_ref.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/parser.h` & `html5-parser-0.4.9/gumbo/parser.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tag_perf.h` & `html5-parser-0.4.9/gumbo/tag_perf.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/string_piece.h` & `html5-parser-0.4.9/gumbo/string_piece.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/insertion_mode.h` & `html5-parser-0.4.9/gumbo/insertion_mode.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tag_strings.h` & `html5-parser-0.4.9/gumbo/tag_strings.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tokenizer.c` & `html5-parser-0.4.9/gumbo/tokenizer.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/attribute.h` & `html5-parser-0.4.9/gumbo/attribute.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/string_buffer.h` & `html5-parser-0.4.9/gumbo/string_buffer.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/parser.c` & `html5-parser-0.4.9/gumbo/parser.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tag.c` & `html5-parser-0.4.9/gumbo/tag.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tokenizer.h` & `html5-parser-0.4.9/gumbo/tokenizer.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/util.c` & `html5-parser-0.4.9/gumbo/util.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/string_buffer.c` & `html5-parser-0.4.9/gumbo/string_buffer.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/util.h` & `html5-parser-0.4.9/gumbo/util.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/svg_attrs.c` & `html5-parser-0.4.9/gumbo/svg_attrs.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/char_ref.h` & `html5-parser-0.4.9/gumbo/char_ref.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/token_type.h` & `html5-parser-0.4.9/gumbo/token_type.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/tag_sizes.h` & `html5-parser-0.4.9/gumbo/tag_sizes.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/gumbo_edit.h` & `html5-parser-0.4.9/gumbo/gumbo_edit.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/vector.h` & `html5-parser-0.4.9/gumbo/vector.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/gumbo.h` & `html5-parser-0.4.9/gumbo/gumbo.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/svg_tags.c` & `html5-parser-0.4.9/gumbo/svg_tags.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/gumbo/string_piece.c` & `html5-parser-0.4.9/gumbo/string_piece.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/README.rst` & `html5-parser-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/run_tests.py` & `html5-parser-0.4.9/run_tests.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/test/adapt.py` & `html5-parser-0.4.9/test/adapt.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/test/basic.py` & `html5-parser-0.4.9/test/basic.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/test/malformed.py` & `html5-parser-0.4.9/test/malformed.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/test/__init__.py` & `html5-parser-0.4.9/test/__init__.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/test/html5lib_adapter.py` & `html5-parser-0.4.9/test/html5lib_adapter.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/test/namespace.py` & `html5-parser-0.4.9/test/namespace.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,7 +173,16 @@
         p = root[-1][0]
         self.ae(p.tag, '{%s}p' % XHTML)
         self.ae(p.nsmap, {None: XHTML, 'a': '1', 'b': '2'})
         self.ae(p.attrib, {'id': 'p'})
         a = p[0]
         self.ae(a.attrib, {'{1}a': 'a', '{2}a': 'b', 'n': 'm'})
         self.ae(a.tag, '{1}one')
+
+    def test_xlink(self):
+        src = '''<html xmlns:xlink="xl"><svg><image xlink:href="x"/>'''
+        root = parse(src, maybe_xhtml=True)
+        self.ae(
+            tostring(root),
+            '''<html xmlns="http://www.w3.org/1999/xhtml" xmlns:xlink="xl"><head/><body>\
+<svg xmlns="http://www.w3.org/2000/svg"><image xlink:href="x"/></svg></body></html>'''
+        )
```

### Comparing `html5-parser-0.4.8/test/soup.py` & `html5-parser-0.4.9/test/soup.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/genattrs.py` & `html5-parser-0.4.9/genattrs.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/win-ci.py` & `html5-parser-0.4.9/win-ci.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/attr_perf.h` & `html5-parser-0.4.9/src/attr_perf.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser.egg-info/PKG-INFO` & `html5-parser-0.4.9/src/html5_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: html5-parser
-Version: 0.4.8
+Version: 0.4.9
 Summary: Fast C based HTML 5 parsing for python
 Home-page: https://html5-parser.readthedocs.io
 Author: Kovid Goyal
 Author-email: redacted@acme.com
 License: Apache 2.0
-Download-URL: https://pypi.python.org/packages/source/m/html5-parser/html5-parser-0.4.8.tar.gz
+Download-URL: https://pypi.python.org/packages/source/m/html5-parser/html5-parser-0.4.9.tar.gz
 Description: UNKNOWN
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `html5-parser-0.4.8/src/html5_parser.egg-info/SOURCES.txt` & `html5-parser-0.4.9/src/html5_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/data-types.h` & `html5-parser-0.4.9/src/data-types.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser/encoding_names.py` & `html5-parser-0.4.9/src/html5_parser/encoding_names.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser/stdlib_etree.py` & `html5-parser-0.4.9/src/html5_parser/stdlib_etree.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser/encoding_parser.py` & `html5-parser-0.4.9/src/html5_parser/encoding_parser.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser/__init__.py` & `html5-parser-0.4.9/src/html5_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser/dom.py` & `html5-parser-0.4.9/src/html5_parser/dom.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/html5_parser/soup.py` & `html5-parser-0.4.9/src/html5_parser/soup.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/as-python-tree.c` & `html5-parser-0.4.9/src/as-python-tree.c`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/python-wrapper.c` & `html5-parser-0.4.9/src/python-wrapper.c`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 #include "../gumbo/gumbo.h"
 #include "as-libxml.h"
 #include "as-python-tree.h"
 
 #define MAJOR 0
 #define MINOR 4
-#define PATCH 8
+#define PATCH 9
 
 static char *NAME =  "libxml2:xmlDoc";
 static char *DESTRUCTOR = "destructor:xmlFreeDoc";
 
 static inline libxml_doc*
 convert_tree(GumboOutput *output, Options *opts) {
     char *errmsg = NULL;
```

### Comparing `html5-parser-0.4.8/src/attr_strings.h` & `html5-parser-0.4.9/src/attr_strings.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/as-libxml.c` & `html5-parser-0.4.9/src/as-libxml.c`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,33 @@
     }
     return true;
 }
 
 static inline xmlNsPtr
 ensure_xml_ns(xmlDocPtr doc, ParseData *pd, xmlNodePtr node) {
     // By default libxml2 docs do not have the xml: namespace defined.
-    xmlNodePtr root = pd->root ? pd->root : node;
     if (UNLIKELY(!pd->xml)) {
+        xmlNodePtr root = pd->root ? pd->root : node;
         pd->xml = xmlSearchNs(doc, root, BAD_CAST "xml");
     }
     return pd->xml;
 }
 
 static inline xmlNsPtr
+ensure_xlink_ns(xmlDocPtr doc, ParseData *pd, xmlNodePtr node) {
+    if (UNLIKELY(!pd->xlink)) {
+        xmlNodePtr root = pd->root ? pd->root : node;
+        pd->xlink = xmlSearchNs(doc, root, BAD_CAST "xlink");
+        if (UNLIKELY(!pd->xlink)) pd->xlink = xmlNewNs(root, BAD_CAST "http://www.w3.org/1999/xlink", BAD_CAST "xlink");
+    }
+    return pd->xlink;
+}
+
+
+static inline xmlNsPtr
 find_namespace_by_prefix(xmlDocPtr doc, xmlNodePtr node, xmlNodePtr xml_parent, const char* prefix) {
     xmlNsPtr ans = xmlSearchNs(doc, node, BAD_CAST prefix);
     if (ans) return ans;
     if (!xml_parent) return NULL;
     return xmlSearchNs(doc, xml_parent, BAD_CAST prefix);
 }
 
@@ -71,49 +82,40 @@
 create_attributes(xmlDocPtr doc, xmlNodePtr node, GumboElement *elem, xmlNodePtr xml_parent, bool reprocess, bool *needs_reprocess) {
     GumboAttribute* attr;
     const xmlChar *attr_name;
     const char *aname;
     char buf[50] = {0};
     ParseData *pd = (ParseData*)doc->_private;
     xmlNsPtr ns;
-    xmlNodePtr root;
     int added_lang = 0;
 
     for (unsigned int i = 0; i < elem->attributes.length; ++i) {
         attr = elem->attributes.data[i];
         if (reprocess && attr->original_name.data != REPROCESS.data) continue;
         aname = attr->name;
         ns = NULL;
         switch (attr->attr_namespace) {
             case GUMBO_ATTR_NAMESPACE_XLINK:
-                root = pd->root ? pd->root : node;
-                if (UNLIKELY(!pd->xlink)) {
-                    pd->xlink = xmlNewNs(root, BAD_CAST "http://www.w3.org/1999/xlink", BAD_CAST "xlink");
-                    if(UNLIKELY(!pd->xlink)) return false;
-                }
-                ns = pd->xlink;
+                ns = ensure_xlink_ns(doc, pd, node);
+                if (UNLIKELY(!ns)) return false;
                 break;
             case GUMBO_ATTR_NAMESPACE_XML:
                 ns = ensure_xml_ns(doc, pd, node);
                 if (UNLIKELY(!ns)) return false;
                 if (UNLIKELY(pd->maybe_xhtml && strcmp(aname, "lang") == 0)) {
                     if (!added_lang) {
                         added_lang = 1;
                         if (UNLIKELY(!xmlNewNsPropEatName(node, NULL, (xmlChar*)pd->lang_attribute, BAD_CAST attr->value))) return false;
                     }
                     continue;
                 }
                 break;
             case GUMBO_ATTR_NAMESPACE_XMLNS:
                 if (strncmp(aname, "xlink", 5) == 0) {
-                    root = pd->root ? pd->root : node;
-                    if (UNLIKELY(!pd->xlink)) {
-                        pd->xlink = xmlNewNs(root, BAD_CAST "http://www.w3.org/1999/xlink", BAD_CAST "xlink");
-                        if(UNLIKELY(!pd->xlink)) return false;
-                    }
+                    if (!ensure_xlink_ns(doc, pd, node)) return false;
                     // We ignore the value of this attribute since we dont want
                     // the xlink namespace to be redefined
                     continue;
                 } else if (strncmp(aname, "xmlns", 5) == 0) {
                     // discard since we dont support changing the default
                     // namespace, namespace are decided by tag names alone.
                     continue;
```

### Comparing `html5-parser-0.4.8/src/attr_sizes.h` & `html5-parser-0.4.9/src/attr_sizes.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/stack.h` & `html5-parser-0.4.9/src/stack.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/src/attr_enum.h` & `html5-parser-0.4.9/src/attr_enum.h`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/LICENSE` & `html5-parser-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/genencodings.py` & `html5-parser-0.4.9/genencodings.py`

 * *Files identical despite different names*

### Comparing `html5-parser-0.4.8/build.py` & `html5-parser-0.4.9/build.py`

 * *Files identical despite different names*

