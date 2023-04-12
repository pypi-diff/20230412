# Comparing `tmp/singular_client-0.1.3.tar.gz` & `tmp/singular_client-0.1.4.tar.gz`

## Comparing `singular_client-0.1.3.tar` & `singular_client-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,30 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.3/.DS_Store
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 singular_client-0.1.3/.python-version
--rw-r--r--   0        0        0    99036 2020-02-02 00:00:00.000000 singular_client-0.1.3/copilot magic documents.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/__init__.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/_bases.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/api.py
--rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/arguments.py
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/documents.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.3/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 singular_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 singular_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.4/.DS_Store
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 singular_client-0.1.4/.python-version
+-rw-r--r--   0        0        0    40764 2020-02-02 00:00:00.000000 singular_client-0.1.4/ALL Dimensions and Metrics.csv
+-rw-r--r--   0        0        0    27890 2020-02-02 00:00:00.000000 singular_client-0.1.4/ALL Dimensions and Metrics.xlsx
+-rw-r--r--   0        0        0    40690 2020-02-02 00:00:00.000000 singular_client-0.1.4/all_dimensions_and_metrics.csv
+-rw-r--r--   0        0        0    99036 2020-02-02 00:00:00.000000 singular_client-0.1.4/copilot magic documents.png
+-rw-r--r--   0        0        0    66321 2020-02-02 00:00:00.000000 singular_client-0.1.4/dimensions_and_metrics.py
+-rw-r--r--   0        0        0    15837 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client.zip
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 singular_client-0.1.4/test.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/.DS_Store
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/__init__.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/_bases.py
+-rw-r--r--   0        0        0   133384 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/_generate_dim_and_metric_types.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/all_arguments.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/api.py
+-rwxr-xr-x   0        0        0    15519 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/arguments.py
+-rw-r--r--   0        0        0    67995 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/dimensions_and_metrics.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/documents.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.4/README.md
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 singular_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 singular_client-0.1.4/PKG-INFO
```

### Comparing `singular_client-0.1.3/.DS_Store` & `singular_client-0.1.4/.DS_Store`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000c  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 000d  ................
 00000050: 0000 0001 0000 1000 6c67 3153 636f 6d70  ........lg1Scomp
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,46 +26,46 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 000c 0000 0004  ................
+00000200: 0000 0000 0000 0000 0000 000d 0000 0004  ................
 00000210: 0064 0069 0073 0074 6c67 3153 636f 6d70  .d.i.s.tlg1Scomp
 00000220: 0000 0000 0000 6468 0000 0004 0064 0069  ......dh.....d.i
 00000230: 0073 0074 6d6f 4444 626c 6f62 0000 0008  .s.tmoDDblob....
 00000240: 9f50 81a7 c3f1 c441 0000 0004 0064 0069  .P.....A.....d.i
 00000250: 0073 0074 6d6f 6444 626c 6f62 0000 0008  .s.tmodDblob....
 00000260: 9f50 81a7 c3f1 c441 0000 0004 0064 0069  .P.....A.....d.i
 00000270: 0073 0074 7068 3153 636f 6d70 0000 0000  .s.tph1Scomp....
 00000280: 0000 7000 0000 000f 0073 0069 006e 0067  ..p......s.i.n.g
 00000290: 0075 006c 0061 0072 005f 0063 006c 0069  .u.l.a.r._.c.l.i
-000002a0: 0065 006e 0074 6c67 3153 636f 6d70 0000  .e.n.tlg1Scomp..
-000002b0: 0000 0002 7803 0000 000f 0073 0069 006e  ....x......s.i.n
-000002c0: 0067 0075 006c 0061 0072 005f 0063 006c  .g.u.l.a.r._.c.l
-000002d0: 0069 0065 006e 0074 6d6f 4444 626c 6f62  .i.e.n.tmoDDblob
-000002e0: 0000 0008 0000 80cc dbf1 c441 0000 000f  ...........A....
-000002f0: 0073 0069 006e 0067 0075 006c 0061 0072  .s.i.n.g.u.l.a.r
-00000300: 005f 0063 006c 0069 0065 006e 0074 6d6f  ._.c.l.i.e.n.tmo
-00000310: 6444 626c 6f62 0000 0008 0000 80cc dbf1  dDblob..........
-00000320: c441 0000 000f 0073 0069 006e 0067 0075  .A.....s.i.n.g.u
-00000330: 006c 0061 0072 005f 0063 006c 0069 0065  .l.a.r._.c.l.i.e
-00000340: 006e 0074 7068 3153 636f 6d70 0000 0000  .n.tph1Scomp....
-00000350: 0003 9000 0000 0004 0074 0065 0073 0074  .........t.e.s.t
-00000360: 6c67 3153 636f 6d70 0000 0000 0000 104c  lg1Scomp.......L
-00000370: 0000 0004 0074 0065 0073 0074 6d6f 4444  .....t.e.s.tmoDD
-00000380: 626c 6f62 0000 0008 0000 00c7 bff1 c441  blob...........A
-00000390: 0000 0004 0074 0065 0073 0074 6d6f 6444  .....t.e.s.tmodD
-000003a0: 626c 6f62 0000 0008 0000 00c7 bff1 c441  blob...........A
-000003b0: 0000 0004 0074 0065 0073 0074 7068 3153  .....t.e.s.tph1S
-000003c0: 636f 6d70 0000 0000 0000 2000 0000 0000  comp...... .....
-000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0065 006e 0074 6473 636c 626f 6f6c 0100  .e.n.tdsclbool..
+000002b0: 0000 0f00 7300 6900 6e00 6700 7500 6c00  ....s.i.n.g.u.l.
+000002c0: 6100 7200 5f00 6300 6c00 6900 6500 6e00  a.r._.c.l.i.e.n.
+000002d0: 746c 6731 5363 6f6d 7000 0000 0000 0278  tlg1Scomp......x
+000002e0: 0300 0000 0f00 7300 6900 6e00 6700 7500  ......s.i.n.g.u.
+000002f0: 6c00 6100 7200 5f00 6300 6c00 6900 6500  l.a.r._.c.l.i.e.
+00000300: 6e00 746d 6f44 4462 6c6f 6200 0000 0800  n.tmoDDblob.....
+00000310: 0080 ccdb f1c4 4100 0000 0f00 7300 6900  ......A.....s.i.
+00000320: 6e00 6700 7500 6c00 6100 7200 5f00 6300  n.g.u.l.a.r._.c.
+00000330: 6c00 6900 6500 6e00 746d 6f64 4462 6c6f  l.i.e.n.tmodDblo
+00000340: 6200 0000 0800 0080 ccdb f1c4 4100 0000  b...........A...
+00000350: 0f00 7300 6900 6e00 6700 7500 6c00 6100  ..s.i.n.g.u.l.a.
+00000360: 7200 5f00 6300 6c00 6900 6500 6e00 7470  r._.c.l.i.e.n.tp
+00000370: 6831 5363 6f6d 7000 0000 0000 0390 0000  h1Scomp.........
+00000380: 0000 0400 7400 6500 7300 746c 6731 5363  ....t.e.s.tlg1Sc
+00000390: 6f6d 7000 0000 0000 0010 4c00 0000 0400  omp.......L.....
+000003a0: 7400 6500 7300 746d 6f44 4462 6c6f 6200  t.e.s.tmoDDblob.
+000003b0: 0000 0800 0000 c7bf f1c4 4100 0000 0400  ..........A.....
+000003c0: 7400 6500 7300 746d 6f64 4462 6c6f 6200  t.e.s.tmodDblob.
+000003d0: 0000 0800 0000 c7bf f1c4 4100 0000 0400  ..........A.....
+000003e0: 7400 6500 7300 7470 6831 5363 6f6d 7000  t.e.s.tph1Scomp.
+000003f0: 0000 0000 0020 0000 0000 0000 0000 0000  ..... ..........
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `singular_client-0.1.3/copilot magic documents.png` & `singular_client-0.1.4/copilot magic documents.png`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.3/singular_client/_bases.py` & `singular_client-0.1.4/singular_client/_bases.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.3/singular_client/api.py` & `singular_client-0.1.4/singular_client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 from typing import (
     Optional,
     Literal,
 )
 import os
 
+from singular_client import TESTING
 from singular_client.documents import *
 from singular_client.arguments import *
 
 
 class SingularAPI:
     """
     A simple class to store endpoint instances, and handle authentication and base url
@@ -24,14 +25,15 @@
 
     key: str
 
     def __init__(self, key: Optional[str]=None):
         if not key:
             key = os.environ.get("SINGULAR_API_KEY")
             assert key, "No API key provided"
+
         self.key = key
 
         from singular_client import endpoints
 
         # Reporting
         self.combined_report = endpoints.CombinedReportEndpoint(self)
         self.network_report = endpoints.NetworkReportEndpoint(self)
```

### Comparing `singular_client-0.1.3/singular_client/endpoints/links.py` & `singular_client-0.1.4/singular_client/endpoints/links.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.3/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.4/singular_client/endpoints/links_legacy.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.3/singular_client/endpoints/monetization.py` & `singular_client-0.1.4/singular_client/endpoints/monetization.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.3/singular_client/endpoints/reporting.py` & `singular_client-0.1.4/singular_client/endpoints/reporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
     endpoint = "v2.0/get_report_status"
     data_path = ["value"]
     res_type = ReportStatusResponse
     cacheable = False
     request_times: Dict[str, float] = {}
     returns_collection = False
+    report_id: str
 
     def request(self, report_id: str) -> Optional[ReportStatusResponse]:
         recent_time = self.request_times.get(report_id, 0)
         if time.time() - recent_time < 10:
             print(
                 "Please wait at least 10 seconds between report status requests, per report"
             )
@@ -219,14 +220,16 @@
                 display_unenriched=display_unenriched,
             ),
         )
         report_id.api = self.api
         return report_id
 
 
+# class GeneralReportEndpoint(_AggReportEndpoint[DimensionInGeneral, MetricInGeneral]):
+
 class CombinedReportEndpoint(_AggReportEndpoint[CombinedDimension, CombinedMetric]):
     available_dimensions = COMBINED_DIMENSIONS
     available_metrics = COMBINED_METRICS
 
 
 class NetworkReportEndpoint(_AggReportEndpoint[NetworkDimension, NetworkMetric]):
     available_dimensions = NETWORK_DIMENSIONS
```

### Comparing `singular_client-0.1.3/singular_client/endpoints/skan.py` & `singular_client-0.1.4/singular_client/endpoints/skan.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.3/pyproject.toml` & `singular_client-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.3"
+version = "0.1.4"
 python_requires = ">=3.8"
-description = "Singular API client"
+description = "A modern Singular API client, with rigorous static type checking."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/ryayoung/singular-client"
 repository = "https://github.com/ryayoung/singular-client"
```

### Comparing `singular_client-0.1.3/PKG-INFO` & `singular_client-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: singular-client
-Version: 0.1.3
-Summary: Singular API client
+Version: 0.1.4
+Summary: A modern Singular API client, with rigorous static type checking.
 Author-email: Ryan Young <dev@ryayoung.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

