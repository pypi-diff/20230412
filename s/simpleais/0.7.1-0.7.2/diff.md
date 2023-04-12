# Comparing `tmp/simpleais-0.7.1-py3-none-any.whl.zip` & `tmp/simpleais-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 23470 bytes, number of entries: 8
+Zip file size: 26339 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx    30804 b- defN 19-Jan-16 21:13 simpleais/__init__.py
 -rw-rw-r--  2.0 unx    88691 b- defN 17-Apr-30 01:07 simpleais/aivdm.json
--rw-rw-r--  2.0 unx    29368 b- defN 19-Jan-18 21:18 simpleais/tools.py
--rw-rw-r--  2.0 unx     5334 b- defN 19-Jan-18 21:48 simpleais-0.7.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 19-Jan-18 21:48 simpleais-0.7.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      306 b- defN 19-Jan-18 21:48 simpleais-0.7.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 19-Jan-18 21:48 simpleais-0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      637 b- defN 19-Jan-18 21:48 simpleais-0.7.1.dist-info/RECORD
-8 files, 155242 bytes uncompressed, 22366 bytes compressed:  85.6%
+-rw-rw-r--  2.0 unx    29608 b- defN 23-Apr-11 23:57 simpleais/tools.py
+-rw-rw-r--  2.0 unx     7652 b- defN 23-Apr-12 00:05 simpleais-0.7.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5345 b- defN 23-Apr-12 00:05 simpleais-0.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 00:05 simpleais-0.7.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      305 b- defN 23-Apr-12 00:05 simpleais-0.7.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-12 00:05 simpleais-0.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      727 b- defN 23-Apr-12 00:05 simpleais-0.7.2.dist-info/RECORD
+9 files, 163234 bytes uncompressed, 25093 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: simpleais/aivdm.json
 Comment: 
 
 Filename: simpleais/tools.py
 Comment: 
 
-Filename: simpleais-0.7.1.dist-info/METADATA
+Filename: simpleais-0.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: simpleais-0.7.1.dist-info/WHEEL
+Filename: simpleais-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: simpleais-0.7.1.dist-info/entry_points.txt
+Filename: simpleais-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: simpleais-0.7.1.dist-info/top_level.txt
+Filename: simpleais-0.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: simpleais-0.7.1.dist-info/RECORD
+Filename: simpleais-0.7.2.dist-info/top_level.txt
+Comment: 
+
+Filename: simpleais-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simpleais/tools.py

```diff
@@ -1,8 +1,9 @@
 import functools
+import logging
 import math
 import os
 import re
 import sys
 from collections import defaultdict
 from contextlib import contextmanager
 from copy import copy
@@ -47,16 +48,19 @@
             # noinspection PyArgumentList
             print(output, flush=True)
 
 
 def sentences_from_sources(sources, log_errors=False):
     if len(sources) > 0:
         for source in sources:
-            for sentence in sentences_from_source(source, log_errors):
-                yield sentence
+            try:
+                for sentence in sentences_from_source(source, log_errors):
+                    yield sentence
+            except:
+                logging.exception("Unexpected failure with source {}; continuing".format(source))
     else:
         for sentence in sentences_from_source(sys.stdin, log_errors):
             yield sentence
 
 
 @click.command()
 @click.argument('sources', nargs=-1)
@@ -134,44 +138,46 @@
         return int(dateutil_parse(string).strftime("%s"))
     else:
         return None
 
 
 @click.command()
 @click.argument('sources', nargs=-1)
-@click.option('--mmsi', '-m', multiple=True)
+@click.option('-m', '--mmsi', multiple=True)
 @click.option('--mmsi-file')
 @click.option('--type', '-t', 'sentence_type', type=int, multiple=True)
 @click.option('--class', 'vessel_class', type=click.Choice(['a', 'b']))
 @click.option('--longitude', '--long', '--lon', 'lon', nargs=2, type=float)
 @click.option('--latitude', '--lat', 'lat', nargs=2, type=float)
 @click.option('--field', '-f', multiple=True)
 @click.option('--value', type=(str, str), multiple=True)
 @click.option('--before')
 @click.option('--after')
 @click.option('--checksum', type=click.Choice(['valid', 'invalid']))
 @click.option('--mode', type=click.Choice(['and', 'or']))
 @click.option('--invert-match', '-v', is_flag=True)
-@click.option('--max-count', '-m', 'max', type=int)
+@click.option('--max-count', 'max', type=int)
 @click.option('--verbose', is_flag=True)
 def grep(sources, mmsi=None, mmsi_file=None, sentence_type=None, vessel_class=None, lon=None, lat=None,
          value=None, before=None, after=None, field=None, checksum=None,
          mode='and', invert_match=False, max=None, verbose=False):
     """ Filters AIS transmissions.  """
+    print(f'mmsi={mmsi}', file=sys.stderr)
     if not mmsi:
         mmsi = frozenset()
     if mmsi_file:
         mmsi = frozenset(mmsi)
         mmsi = mmsi.union(read_mmsi_file(mmsi_file))
     if checksum is None:
         checksum_desire = None
     else:
         checksum_desire = checksum == "valid"
     taster = Taster(mmsi, sentence_type, vessel_class, lon, lat, field, value, parse_date(before), parse_date(after),
                     mode, checksum_desire, invert_match)
+    print(taster.mmsi, file=sys.stderr)
     with wild_disregard_for(BrokenPipeError):
         matches = 0
         for sentence in sentences_from_sources(sources, log_errors=verbose):
             if taster.likes(sentence):
                 print_sentence_source(sentence)
                 matches += 1
                 if max and matches >= max:
@@ -259,15 +265,15 @@
     fname, ext = os.path.splitext(dest)
 
     for sentence in sentences_from_source(source, log_errors=verbose):
         mmsi = sentence['mmsi']
         if not mmsi:
             mmsi = 'other'
         if mmsi not in writers:
-            writers[mmsi] = open("{}-{}{}".format(fname, mmsi, ext), "wt")
+            writers[mmsi] = open("{}-{}{}".format(fname, mmsi, ext), "at")
         print_sentence_source(sentence, writers[mmsi])
 
     for writer in writers.values():
         writer.close()
 
 
 class FieldsHistory:
@@ -732,16 +738,16 @@
         self.recorded_course = None
         self.recorded_voyage = None
 
     def wants(self, sentence):
         time = sentence.time
         if not time:
             raise ValueError("time  needed for refinement in {}".format(sentence))
-        if sentence.type_id() not in self.last_seen_by_type or time - self.last_seen_by_type[
-            sentence.type_id()] > self.BORING_SECONDS:
+        if sentence.type_id() not in self.last_seen_by_type or \
+                time - self.last_seen_by_type[sentence.type_id()] > self.BORING_SECONDS:
             return True
         elif self.is_motion(sentence) and self.motion_interesting(sentence):
             return True
         elif self.is_voyage_info(sentence) and self.voyage_interesting(sentence):
             return True
         return False
```

## Comparing `simpleais-0.7.1.dist-info/METADATA` & `simpleais-0.7.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: simpleais
-Version: 0.7.1
+Version: 0.7.2
 Summary: a simple ais parser
 Home-page: https://github.com/wpietri/simpleais
 Author: William Pietri
 Author-email: william-simpleais-0_7@scissor.com
 License: Apache 2.0
-Platform: UNKNOWN
+License-File: LICENSE
 Requires-Dist: bitstring
 Requires-Dist: testfixtures
-Requires-Dist: Click
+Requires-Dist: Click (<8.1.3)
 Requires-Dist: numpy
 Requires-Dist: python-dateutil
 Provides-Extra: dev
 Requires-Dist: beautifulsoup4 ; extra == 'dev'
 Requires-Dist: nose ; extra == 'dev'
 
 SimpleAIS
@@ -124,9 +124,7 @@
 My main source for protocol information is here:
 http://catb.org/gpsd/AIVDM.html
 
 More protocol info is here:
 http://www.itu.int/dms\_pubrec/itu-r/rec/m/R-REC-M.1371-5-201402-I!!PDF-E.pdf
 
 The protocol checksum is here: https://en.wikipedia.org/wiki/NMEA\_0183
-
-
```

