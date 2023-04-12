# Comparing `tmp/np_gui-0.0.3.tar.gz` & `tmp/np_gui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_gui-0.0.3.tar", max compression
+gzip compressed data, was "np_gui-0.0.4.tar", max compression
```

## Comparing `np_gui-0.0.3.tar` & `np_gui-0.0.4.tar`

### file list

```diff
@@ -1,305 +1,305 @@
--rw-r--r--   0        0        0     2773 2023-04-11 12:23:04.710895 np_gui-0.0.3/README.md
--rw-r--r--   0        0        0     1454 2023-04-10 21:22:19.221466 np_gui-0.0.3/np_gui/__init__.py
--rw-r--r--   0        0        0      120 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char0.png
--rw-r--r--   0        0        0      123 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char1.png
--rw-r--r--   0        0        0      106 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char10.png
--rw-r--r--   0        0        0      136 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char11.png
--rw-r--r--   0        0        0       79 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char12.png
--rw-r--r--   0        0        0       97 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char13.png
--rw-r--r--   0        0        0      164 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char14.png
--rw-r--r--   0        0        0      244 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char15.png
--rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char16.png
--rw-r--r--   0        0        0      242 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char17.png
--rw-r--r--   0        0        0      258 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char18.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char19.png
--rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char2.png
--rw-r--r--   0        0        0      205 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char20.png
--rw-r--r--   0        0        0      276 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char21.png
--rw-r--r--   0        0        0      214 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char22.png
--rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char23.png
--rw-r--r--   0        0        0      273 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char24.png
--rw-r--r--   0        0        0      110 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char25.png
--rw-r--r--   0        0        0      157 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char26.png
--rw-r--r--   0        0        0      217 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char27.png
--rw-r--r--   0        0        0       88 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char28.png
--rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char29.png
--rw-r--r--   0        0        0      297 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char3.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char30.png
--rw-r--r--   0        0        0      496 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char31.png
--rw-r--r--   0        0        0      298 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char32.png
--rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char33.png
--rw-r--r--   0        0        0      252 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char34.png
--rw-r--r--   0        0        0      246 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char35.png
--rw-r--r--   0        0        0      178 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char36.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char37.png
--rw-r--r--   0        0        0      269 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char38.png
--rw-r--r--   0        0        0      158 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char39.png
--rw-r--r--   0        0        0      408 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char4.png
--rw-r--r--   0        0        0      114 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char40.png
--rw-r--r--   0        0        0      161 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char41.png
--rw-r--r--   0        0        0      330 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char42.png
--rw-r--r--   0        0        0      141 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char43.png
--rw-r--r--   0        0        0      323 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char44.png
--rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char5.png
--rw-r--r--   0        0        0       93 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char6.png
--rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char7.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char8.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char9.png
--rw-r--r--   0        0        0      285 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char0.png
--rw-r--r--   0        0        0      290 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char1.png
--rw-r--r--   0        0        0      367 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char10.png
--rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char11.png
--rw-r--r--   0        0        0      270 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char12.png
--rw-r--r--   0        0        0      112 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char13.png
--rw-r--r--   0        0        0      172 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char14.png
--rw-r--r--   0        0        0      111 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char15.png
--rw-r--r--   0        0        0      225 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char16.png
--rw-r--r--   0        0        0       94 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char17.png
--rw-r--r--   0        0        0      134 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char18.png
--rw-r--r--   0        0        0      198 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char19.png
--rw-r--r--   0        0        0      204 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char2.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char20.png
--rw-r--r--   0        0        0      192 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char21.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char22.png
--rw-r--r--   0        0        0      202 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char23.png
--rw-r--r--   0        0        0      167 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char24.png
--rw-r--r--   0        0        0      318 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char25.png
--rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char26.png
--rw-r--r--   0        0        0      137 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char27.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char28.png
--rw-r--r--   0        0        0      256 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char29.png
--rw-r--r--   0        0        0      342 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char3.png
--rw-r--r--   0        0        0      113 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char30.png
--rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char31.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char32.png
--rw-r--r--   0        0        0      213 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char33.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char34.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char35.png
--rw-r--r--   0        0        0      139 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char36.png
--rw-r--r--   0        0        0      222 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char37.png
--rw-r--r--   0        0        0      140 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char38.png
--rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char39.png
--rw-r--r--   0        0        0      275 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char4.png
--rw-r--r--   0        0        0      236 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char40.png
--rw-r--r--   0        0        0      282 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char41.png
--rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char42.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char43.png
--rw-r--r--   0        0        0      230 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char44.png
--rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char45.png
--rw-r--r--   0        0        0       78 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char46.png
--rw-r--r--   0        0        0      189 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char47.png
--rw-r--r--   0        0        0      179 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char48.png
--rw-r--r--   0        0        0      291 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char5.png
--rw-r--r--   0        0        0      147 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char6.png
--rw-r--r--   0        0        0      207 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char7.png
--rw-r--r--   0        0        0      315 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char8.png
--rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char9.png
--rw-r--r--   0        0        0      124 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char0.png
--rw-r--r--   0        0        0       84 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char1.png
--rw-r--r--   0        0        0      366 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char10.png
--rw-r--r--   0        0        0      385 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char11.png
--rw-r--r--   0        0        0      383 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char12.png
--rw-r--r--   0        0        0      353 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char13.png
--rw-r--r--   0        0        0      352 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char14.png
--rw-r--r--   0        0        0      292 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char15.png
--rw-r--r--   0        0        0      308 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char16.png
--rw-r--r--   0        0        0      248 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char17.png
--rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char18.png
--rw-r--r--   0        0        0      255 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char19.png
--rw-r--r--   0        0        0      327 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char2.png
--rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char20.png
--rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char21.png
--rw-r--r--   0        0        0      171 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char22.png
--rw-r--r--   0        0        0      194 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char23.png
--rw-r--r--   0        0        0      162 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char24.png
--rw-r--r--   0        0        0      245 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char25.png
--rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char26.png
--rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char27.png
--rw-r--r--   0        0        0      348 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char28.png
--rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char29.png
--rw-r--r--   0        0        0      122 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char3.png
--rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char30.png
--rw-r--r--   0        0        0      333 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char31.png
--rw-r--r--   0        0        0      227 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char32.png
--rw-r--r--   0        0        0      397 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char33.png
--rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char34.png
--rw-r--r--   0        0        0      272 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char35.png
--rw-r--r--   0        0        0      293 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char36.png
--rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char37.png
--rw-r--r--   0        0        0      347 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char38.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char39.png
--rw-r--r--   0        0        0      390 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char4.png
--rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char40.png
--rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char41.png
--rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char42.png
--rw-r--r--   0        0        0      261 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char43.png
--rw-r--r--   0        0        0      168 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char5.png
--rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char6.png
--rw-r--r--   0        0        0      232 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char7.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char8.png
--rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char9.png
--rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char0.png
--rw-r--r--   0        0        0      246 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char1.png
--rw-r--r--   0        0        0      164 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char10.png
--rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char11.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char12.png
--rw-r--r--   0        0        0      312 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char13.png
--rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char14.png
--rw-r--r--   0        0        0      275 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char15.png
--rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char16.png
--rw-r--r--   0        0        0      292 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char17.png
--rw-r--r--   0        0        0      286 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char18.png
--rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char19.png
--rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char2.png
--rw-r--r--   0        0        0      128 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char20.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char21.png
--rw-r--r--   0        0        0      220 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char22.png
--rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char23.png
--rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char24.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char25.png
--rw-r--r--   0        0        0      348 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char26.png
--rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char27.png
--rw-r--r--   0        0        0      333 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char28.png
--rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char29.png
--rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char3.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char30.png
--rw-r--r--   0        0        0      372 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char31.png
--rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char32.png
--rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char33.png
--rw-r--r--   0        0        0      245 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char34.png
--rw-r--r--   0        0        0      316 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char35.png
--rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char36.png
--rw-r--r--   0        0        0      330 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char37.png
--rw-r--r--   0        0        0      270 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char38.png
--rw-r--r--   0        0        0      298 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char39.png
--rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char4.png
--rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char40.png
--rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char41.png
--rw-r--r--   0        0        0      278 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char42.png
--rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char43.png
--rw-r--r--   0        0        0      272 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char44.png
--rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char45.png
--rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char46.png
--rw-r--r--   0        0        0      198 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char47.png
--rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char48.png
--rw-r--r--   0        0        0      265 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char5.png
--rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char6.png
--rw-r--r--   0        0        0      279 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char7.png
--rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char8.png
--rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char9.png
--rw-r--r--   0        0        0      250 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char0.png
--rw-r--r--   0        0        0      263 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char1.png
--rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char10.png
--rw-r--r--   0        0        0      379 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char11.png
--rw-r--r--   0        0        0      306 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char12.png
--rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char13.png
--rw-r--r--   0        0        0      327 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char14.png
--rw-r--r--   0        0        0      365 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char15.png
--rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char16.png
--rw-r--r--   0        0        0      255 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char17.png
--rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char18.png
--rw-r--r--   0        0        0      185 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char19.png
--rw-r--r--   0        0        0      227 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char2.png
--rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char20.png
--rw-r--r--   0        0        0      178 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char21.png
--rw-r--r--   0        0        0      127 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char22.png
--rw-r--r--   0        0        0      122 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char23.png
--rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char24.png
--rw-r--r--   0        0        0      173 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char25.png
--rw-r--r--   0        0        0      154 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char26.png
--rw-r--r--   0        0        0      175 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char27.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char28.png
--rw-r--r--   0        0        0      112 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char29.png
--rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char3.png
--rw-r--r--   0        0        0      179 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char30.png
--rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char31.png
--rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char32.png
--rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char33.png
--rw-r--r--   0        0        0      392 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char34.png
--rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char35.png
--rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char36.png
--rw-r--r--   0        0        0      204 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char37.png
--rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char38.png
--rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char39.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char4.png
--rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char40.png
--rw-r--r--   0        0        0      202 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char41.png
--rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char42.png
--rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char43.png
--rw-r--r--   0        0        0      143 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char44.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char45.png
--rw-r--r--   0        0        0      170 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char46.png
--rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char47.png
--rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char48.png
--rw-r--r--   0        0        0      340 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char49.png
--rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char5.png
--rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char6.png
--rw-r--r--   0        0        0      277 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char7.png
--rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char8.png
--rw-r--r--   0        0        0      388 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char9.png
--rw-r--r--   0        0        0      207 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char0.png
--rw-r--r--   0        0        0      367 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char1.png
--rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char10.png
--rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char11.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char12.png
--rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char13.png
--rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char14.png
--rw-r--r--   0        0        0      189 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char15.png
--rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char16.png
--rw-r--r--   0        0        0      190 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char17.png
--rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char18.png
--rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char19.png
--rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char2.png
--rw-r--r--   0        0        0      351 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char20.png
--rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char21.png
--rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char22.png
--rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char23.png
--rw-r--r--   0        0        0      342 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char24.png
--rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char25.png
--rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char26.png
--rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char27.png
--rw-r--r--   0        0        0      203 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char28.png
--rw-r--r--   0        0        0      197 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char29.png
--rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char3.png
--rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char30.png
--rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char31.png
--rw-r--r--   0        0        0      152 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char32.png
--rw-r--r--   0        0        0      148 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char33.png
--rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char34.png
--rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char35.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char36.png
--rw-r--r--   0        0        0      172 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char37.png
--rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char38.png
--rw-r--r--   0        0        0      211 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char4.png
--rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char5.png
--rw-r--r--   0        0        0      303 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char6.png
--rw-r--r--   0        0        0      228 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char7.png
--rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char8.png
--rw-r--r--   0        0        0      266 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char9.png
--rw-r--r--   0        0        0      209 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char0.png
--rw-r--r--   0        0        0      289 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char1.png
--rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char10.png
--rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char11.png
--rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char12.png
--rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char13.png
--rw-r--r--   0        0        0      311 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char14.png
--rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char15.png
--rw-r--r--   0        0        0      359 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char16.png
--rw-r--r--   0        0        0      297 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char17.png
--rw-r--r--   0        0        0       90 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char18.png
--rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char2.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char3.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char4.png
--rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char5.png
--rw-r--r--   0        0        0      194 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char6.png
--rw-r--r--   0        0        0      484 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char7.png
--rw-r--r--   0        0        0      344 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char8.png
--rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char9.png
--rw-r--r--   0        0        0     8692 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/metadata.csv
--rw-r--r--   0        0        0   426999 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/my_alphabet.png
--rw-r--r--   0        0        0      792 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/transcription.txt
--rw-r--r--   0        0        0     4127 2023-04-09 21:38:45.641967 np_gui-0.0.3/np_gui/colors.py
--rw-r--r--   0        0        0     8110 2023-04-09 22:40:46.825641 np_gui-0.0.3/np_gui/image_annotation.py
--rw-r--r--   0        0        0    23218 2023-04-08 18:48:07.876574 np_gui-0.0.3/np_gui/np_clickable_image.py
--rw-r--r--   0        0        0      564 2023-04-11 14:47:45.313214 np_gui-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3370 1970-01-01 00:00:00.000000 np_gui-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3002 2023-04-12 16:13:30.350935 np_gui-0.0.4/README.md
+-rw-r--r--   0        0        0     1454 2023-04-10 21:22:19.221466 np_gui-0.0.4/np_gui/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char0.png
+-rw-r--r--   0        0        0      123 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char1.png
+-rw-r--r--   0        0        0      106 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char10.png
+-rw-r--r--   0        0        0      136 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char11.png
+-rw-r--r--   0        0        0       79 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char12.png
+-rw-r--r--   0        0        0       97 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char13.png
+-rw-r--r--   0        0        0      164 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char14.png
+-rw-r--r--   0        0        0      244 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char15.png
+-rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char16.png
+-rw-r--r--   0        0        0      242 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char17.png
+-rw-r--r--   0        0        0      258 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char18.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char19.png
+-rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char2.png
+-rw-r--r--   0        0        0      205 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char20.png
+-rw-r--r--   0        0        0      276 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char21.png
+-rw-r--r--   0        0        0      214 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char22.png
+-rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char23.png
+-rw-r--r--   0        0        0      273 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char24.png
+-rw-r--r--   0        0        0      110 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char25.png
+-rw-r--r--   0        0        0      157 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char26.png
+-rw-r--r--   0        0        0      217 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char27.png
+-rw-r--r--   0        0        0       88 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char28.png
+-rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char29.png
+-rw-r--r--   0        0        0      297 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char3.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char30.png
+-rw-r--r--   0        0        0      496 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char31.png
+-rw-r--r--   0        0        0      298 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char32.png
+-rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char33.png
+-rw-r--r--   0        0        0      252 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char34.png
+-rw-r--r--   0        0        0      246 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char35.png
+-rw-r--r--   0        0        0      178 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char36.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char37.png
+-rw-r--r--   0        0        0      269 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char38.png
+-rw-r--r--   0        0        0      158 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char39.png
+-rw-r--r--   0        0        0      408 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char4.png
+-rw-r--r--   0        0        0      114 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char40.png
+-rw-r--r--   0        0        0      161 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char41.png
+-rw-r--r--   0        0        0      330 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char42.png
+-rw-r--r--   0        0        0      141 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char43.png
+-rw-r--r--   0        0        0      323 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char44.png
+-rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char5.png
+-rw-r--r--   0        0        0       93 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char6.png
+-rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char7.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char8.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_0_char9.png
+-rw-r--r--   0        0        0      285 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char0.png
+-rw-r--r--   0        0        0      290 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char1.png
+-rw-r--r--   0        0        0      367 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char10.png
+-rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char11.png
+-rw-r--r--   0        0        0      270 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char12.png
+-rw-r--r--   0        0        0      112 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char13.png
+-rw-r--r--   0        0        0      172 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char14.png
+-rw-r--r--   0        0        0      111 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char15.png
+-rw-r--r--   0        0        0      225 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char16.png
+-rw-r--r--   0        0        0       94 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char17.png
+-rw-r--r--   0        0        0      134 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char18.png
+-rw-r--r--   0        0        0      198 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char19.png
+-rw-r--r--   0        0        0      204 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char2.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char20.png
+-rw-r--r--   0        0        0      192 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char21.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char22.png
+-rw-r--r--   0        0        0      202 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char23.png
+-rw-r--r--   0        0        0      167 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char24.png
+-rw-r--r--   0        0        0      318 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char25.png
+-rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char26.png
+-rw-r--r--   0        0        0      137 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char27.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char28.png
+-rw-r--r--   0        0        0      256 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char29.png
+-rw-r--r--   0        0        0      342 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char3.png
+-rw-r--r--   0        0        0      113 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char30.png
+-rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char31.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char32.png
+-rw-r--r--   0        0        0      213 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char33.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char34.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char35.png
+-rw-r--r--   0        0        0      139 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char36.png
+-rw-r--r--   0        0        0      222 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char37.png
+-rw-r--r--   0        0        0      140 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char38.png
+-rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char39.png
+-rw-r--r--   0        0        0      275 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char4.png
+-rw-r--r--   0        0        0      236 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char40.png
+-rw-r--r--   0        0        0      282 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char41.png
+-rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char42.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char43.png
+-rw-r--r--   0        0        0      230 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char44.png
+-rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char45.png
+-rw-r--r--   0        0        0       78 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char46.png
+-rw-r--r--   0        0        0      189 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char47.png
+-rw-r--r--   0        0        0      179 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char48.png
+-rw-r--r--   0        0        0      291 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char5.png
+-rw-r--r--   0        0        0      147 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char6.png
+-rw-r--r--   0        0        0      207 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char7.png
+-rw-r--r--   0        0        0      315 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char8.png
+-rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_1_char9.png
+-rw-r--r--   0        0        0      124 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char0.png
+-rw-r--r--   0        0        0       84 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char1.png
+-rw-r--r--   0        0        0      366 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char10.png
+-rw-r--r--   0        0        0      385 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char11.png
+-rw-r--r--   0        0        0      383 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char12.png
+-rw-r--r--   0        0        0      353 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char13.png
+-rw-r--r--   0        0        0      352 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char14.png
+-rw-r--r--   0        0        0      292 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char15.png
+-rw-r--r--   0        0        0      308 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char16.png
+-rw-r--r--   0        0        0      248 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char17.png
+-rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char18.png
+-rw-r--r--   0        0        0      255 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char19.png
+-rw-r--r--   0        0        0      327 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char2.png
+-rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char20.png
+-rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char21.png
+-rw-r--r--   0        0        0      171 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char22.png
+-rw-r--r--   0        0        0      194 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char23.png
+-rw-r--r--   0        0        0      162 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char24.png
+-rw-r--r--   0        0        0      245 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char25.png
+-rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char26.png
+-rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char27.png
+-rw-r--r--   0        0        0      348 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char28.png
+-rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char29.png
+-rw-r--r--   0        0        0      122 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char3.png
+-rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char30.png
+-rw-r--r--   0        0        0      333 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char31.png
+-rw-r--r--   0        0        0      227 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char32.png
+-rw-r--r--   0        0        0      397 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char33.png
+-rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char34.png
+-rw-r--r--   0        0        0      272 2023-04-07 15:50:41.218884 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char35.png
+-rw-r--r--   0        0        0      293 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char36.png
+-rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char37.png
+-rw-r--r--   0        0        0      347 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char38.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char39.png
+-rw-r--r--   0        0        0      390 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char4.png
+-rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char40.png
+-rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char41.png
+-rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char42.png
+-rw-r--r--   0        0        0      261 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char43.png
+-rw-r--r--   0        0        0      168 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char5.png
+-rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char6.png
+-rw-r--r--   0        0        0      232 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char7.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char8.png
+-rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_2_char9.png
+-rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char0.png
+-rw-r--r--   0        0        0      246 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char1.png
+-rw-r--r--   0        0        0      164 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char10.png
+-rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char11.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char12.png
+-rw-r--r--   0        0        0      312 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char13.png
+-rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char14.png
+-rw-r--r--   0        0        0      275 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char15.png
+-rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char16.png
+-rw-r--r--   0        0        0      292 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char17.png
+-rw-r--r--   0        0        0      286 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char18.png
+-rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char19.png
+-rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char2.png
+-rw-r--r--   0        0        0      128 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char20.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char21.png
+-rw-r--r--   0        0        0      220 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char22.png
+-rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char23.png
+-rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char24.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char25.png
+-rw-r--r--   0        0        0      348 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char26.png
+-rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char27.png
+-rw-r--r--   0        0        0      333 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char28.png
+-rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char29.png
+-rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char3.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char30.png
+-rw-r--r--   0        0        0      372 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char31.png
+-rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char32.png
+-rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char33.png
+-rw-r--r--   0        0        0      245 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char34.png
+-rw-r--r--   0        0        0      316 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char35.png
+-rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char36.png
+-rw-r--r--   0        0        0      330 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char37.png
+-rw-r--r--   0        0        0      270 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char38.png
+-rw-r--r--   0        0        0      298 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char39.png
+-rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char4.png
+-rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char40.png
+-rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char41.png
+-rw-r--r--   0        0        0      278 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char42.png
+-rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char43.png
+-rw-r--r--   0        0        0      272 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char44.png
+-rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char45.png
+-rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char46.png
+-rw-r--r--   0        0        0      198 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char47.png
+-rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char48.png
+-rw-r--r--   0        0        0      265 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char5.png
+-rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char6.png
+-rw-r--r--   0        0        0      279 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char7.png
+-rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char8.png
+-rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_3_char9.png
+-rw-r--r--   0        0        0      250 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char0.png
+-rw-r--r--   0        0        0      263 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char1.png
+-rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char10.png
+-rw-r--r--   0        0        0      379 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char11.png
+-rw-r--r--   0        0        0      306 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char12.png
+-rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char13.png
+-rw-r--r--   0        0        0      327 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char14.png
+-rw-r--r--   0        0        0      365 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char15.png
+-rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char16.png
+-rw-r--r--   0        0        0      255 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char17.png
+-rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char18.png
+-rw-r--r--   0        0        0      185 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char19.png
+-rw-r--r--   0        0        0      227 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char2.png
+-rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char20.png
+-rw-r--r--   0        0        0      178 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char21.png
+-rw-r--r--   0        0        0      127 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char22.png
+-rw-r--r--   0        0        0      122 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char23.png
+-rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char24.png
+-rw-r--r--   0        0        0      173 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char25.png
+-rw-r--r--   0        0        0      154 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char26.png
+-rw-r--r--   0        0        0      175 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char27.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char28.png
+-rw-r--r--   0        0        0      112 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char29.png
+-rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char3.png
+-rw-r--r--   0        0        0      179 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char30.png
+-rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char31.png
+-rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char32.png
+-rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char33.png
+-rw-r--r--   0        0        0      392 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char34.png
+-rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char35.png
+-rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char36.png
+-rw-r--r--   0        0        0      204 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char37.png
+-rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char38.png
+-rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char39.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char4.png
+-rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char40.png
+-rw-r--r--   0        0        0      202 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char41.png
+-rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char42.png
+-rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char43.png
+-rw-r--r--   0        0        0      143 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char44.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char45.png
+-rw-r--r--   0        0        0      170 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char46.png
+-rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char47.png
+-rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char48.png
+-rw-r--r--   0        0        0      340 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char49.png
+-rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char5.png
+-rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char6.png
+-rw-r--r--   0        0        0      277 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char7.png
+-rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char8.png
+-rw-r--r--   0        0        0      388 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_4_char9.png
+-rw-r--r--   0        0        0      207 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char0.png
+-rw-r--r--   0        0        0      367 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char1.png
+-rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char10.png
+-rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char11.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char12.png
+-rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char13.png
+-rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char14.png
+-rw-r--r--   0        0        0      189 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char15.png
+-rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char16.png
+-rw-r--r--   0        0        0      190 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char17.png
+-rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char18.png
+-rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char19.png
+-rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char2.png
+-rw-r--r--   0        0        0      351 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char20.png
+-rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char21.png
+-rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char22.png
+-rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char23.png
+-rw-r--r--   0        0        0      342 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char24.png
+-rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char25.png
+-rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char26.png
+-rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char27.png
+-rw-r--r--   0        0        0      203 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char28.png
+-rw-r--r--   0        0        0      197 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char29.png
+-rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char3.png
+-rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char30.png
+-rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char31.png
+-rw-r--r--   0        0        0      152 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char32.png
+-rw-r--r--   0        0        0      148 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char33.png
+-rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char34.png
+-rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char35.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char36.png
+-rw-r--r--   0        0        0      172 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char37.png
+-rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char38.png
+-rw-r--r--   0        0        0      211 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char4.png
+-rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char5.png
+-rw-r--r--   0        0        0      303 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char6.png
+-rw-r--r--   0        0        0      228 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char7.png
+-rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char8.png
+-rw-r--r--   0        0        0      266 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_5_char9.png
+-rw-r--r--   0        0        0      209 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char0.png
+-rw-r--r--   0        0        0      289 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char1.png
+-rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char10.png
+-rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char11.png
+-rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char12.png
+-rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char13.png
+-rw-r--r--   0        0        0      311 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char14.png
+-rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char15.png
+-rw-r--r--   0        0        0      359 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char16.png
+-rw-r--r--   0        0        0      297 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char17.png
+-rw-r--r--   0        0        0       90 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char18.png
+-rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char2.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char3.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char4.png
+-rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char5.png
+-rw-r--r--   0        0        0      194 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char6.png
+-rw-r--r--   0        0        0      484 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char7.png
+-rw-r--r--   0        0        0      344 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char8.png
+-rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/line_6_char9.png
+-rw-r--r--   0        0        0     8692 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/metadata.csv
+-rw-r--r--   0        0        0   426999 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/my_alphabet.png
+-rw-r--r--   0        0        0      792 2023-04-07 15:50:41.222883 np_gui-0.0.4/np_gui/alphabet/liberation_serif/transcription.txt
+-rw-r--r--   0        0        0     4127 2023-04-09 21:38:45.641967 np_gui-0.0.4/np_gui/colors.py
+-rw-r--r--   0        0        0     8110 2023-04-09 22:40:46.825641 np_gui-0.0.4/np_gui/image_annotation.py
+-rw-r--r--   0        0        0    23218 2023-04-08 18:48:07.876574 np_gui-0.0.4/np_gui/np_clickable_image.py
+-rw-r--r--   0        0        0      565 2023-04-12 15:55:40.224480 np_gui-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 np_gui-0.0.4/PKG-INFO
```

### Comparing `np_gui-0.0.3/README.md` & `np_gui-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -37,36 +37,41 @@
 ## Installation
 This package can be installed with pip as follows.
 
 ```
 $ pip install np_gui
 ```
 
-To avoid [depency hell](https://en.wikipedia.org/wiki/Dependency_hell), you might consider installing this package in a virtual environment.
+
+To avoid [depency hell](https://en.wikipedia.org/wiki/Dependency_hell),
+you might consider installing this package in a virtual environment.
+
+Alternatively, you can check the pyproject.toml file to see if this package is
+compatible with your setup ; which is likely.
 
 ## Documentation
 
 A detailed documentation of this package is available in pdf and html
 format within the ./doc/ folder of [its GitHub repository](https://github.com/completementgaga/npGUI).
 
 ## Demo
 
 Some demonstration scripts are provided on the [GitHub repository](https://github.com/completementgaga/npGUI).
 
 These are:
 * ./demo/puzzles/puzzles.py 
     | Preview of the puzzles.py demo.|
     |:-----------------------------:|
-    |<img src="./screenshots/puzzles_screenshot.png"  width="300em" title="clock.py preview">|
+    |<img src="https://github.com/completementgaga/npGUI/raw/master/screenshots/puzzles_screenshot.png"  width="300em" title="clock.py preview">|
 
 * ./demo/clock/clock.py
 
     | Preview of the clock.py demo.|
     |:-----------------------------:|
-    |<img src="./screenshots/clock_screenshot.png"  width="300em" title="clock.py preview">|
+    |<img src="https://github.com/completementgaga/npGUI/raw/master/screenshots/clock_screenshot.png"  width="300em" title="clock.py preview">|
 
 ## Further developments of the project
 This package could benefit from several enhancements, among other things:
  
  * develop additional specialized subclasses of ClickableImage,
  * include keyboard interactions,
  * lighten its memory usage.
```

### Comparing `np_gui-0.0.3/np_gui/__init__.py` & `np_gui-0.0.4/np_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/np_gui/alphabet/liberation_serif/metadata.csv` & `np_gui-0.0.4/np_gui/alphabet/liberation_serif/metadata.csv`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/np_gui/alphabet/liberation_serif/my_alphabet.png` & `np_gui-0.0.4/np_gui/alphabet/liberation_serif/my_alphabet.png`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/np_gui/alphabet/liberation_serif/transcription.txt` & `np_gui-0.0.4/np_gui/alphabet/liberation_serif/transcription.txt`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/np_gui/colors.py` & `np_gui-0.0.4/np_gui/colors.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/np_gui/image_annotation.py` & `np_gui-0.0.4/np_gui/image_annotation.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/np_gui/np_clickable_image.py` & `np_gui-0.0.4/np_gui/np_clickable_image.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.3/pyproject.toml` & `np_gui-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "np_gui"
-version = "0.0.3"
+version = "0.0.4"
 description = "This package implements Graphical User Interfaces from a NumPy user perspective."
 authors = ["Gaël Cousin <gcousin333@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "np_gui"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.10.6"
 typeguard = "^3.0.0"
 numpy = "^1.21.0"
 matplotlib = "^3.0.0"
-scikit-image = "0.19.0"
+scikit-image = "^0.19.0"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^6.1.3"
 autodocsumm = "^0.2.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `np_gui-0.0.3/PKG-INFO` & `np_gui-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: np-gui
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package implements Graphical User Interfaces from a NumPy user perspective.
 License: MIT
 Author: Gaël Cousin
 Author-email: gcousin333@gmail.com
 Requires-Python: >=3.10.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: scikit-image (==0.19.0)
+Requires-Dist: scikit-image (>=0.19.0,<0.20.0)
 Requires-Dist: typeguard (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # npGUI
 
 This package implements Graphical User Interfaces from a NumPy user
 perspective: every image corresponds to an ndarray.
@@ -54,36 +54,41 @@
 ## Installation
 This package can be installed with pip as follows.
 
 ```
 $ pip install np_gui
 ```
 
-To avoid [depency hell](https://en.wikipedia.org/wiki/Dependency_hell), you might consider installing this package in a virtual environment.
+
+To avoid [depency hell](https://en.wikipedia.org/wiki/Dependency_hell),
+you might consider installing this package in a virtual environment.
+
+Alternatively, you can check the pyproject.toml file to see if this package is
+compatible with your setup ; which is likely.
 
 ## Documentation
 
 A detailed documentation of this package is available in pdf and html
 format within the ./doc/ folder of [its GitHub repository](https://github.com/completementgaga/npGUI).
 
 ## Demo
 
 Some demonstration scripts are provided on the [GitHub repository](https://github.com/completementgaga/npGUI).
 
 These are:
 * ./demo/puzzles/puzzles.py 
     | Preview of the puzzles.py demo.|
     |:-----------------------------:|
-    |<img src="./screenshots/puzzles_screenshot.png"  width="300em" title="clock.py preview">|
+    |<img src="https://github.com/completementgaga/npGUI/raw/master/screenshots/puzzles_screenshot.png"  width="300em" title="clock.py preview">|
 
 * ./demo/clock/clock.py
 
     | Preview of the clock.py demo.|
     |:-----------------------------:|
-    |<img src="./screenshots/clock_screenshot.png"  width="300em" title="clock.py preview">|
+    |<img src="https://github.com/completementgaga/npGUI/raw/master/screenshots/clock_screenshot.png"  width="300em" title="clock.py preview">|
 
 ## Further developments of the project
 This package could benefit from several enhancements, among other things:
  
  * develop additional specialized subclasses of ClickableImage,
  * include keyboard interactions,
  * lighten its memory usage.
```

