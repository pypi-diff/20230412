# Comparing `tmp/elasticcsv-0.2.2.tar.gz` & `tmp/elasticcsv-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticcsv-0.2.2.tar", last modified: Tue Jul 26 16:06:21 2022, max compression
+gzip compressed data, was "elasticcsv-0.2.3.tar", max compression
```

## Comparing `elasticcsv-0.2.2.tar` & `elasticcsv-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,9 @@
-drwxr-xr-x   0 juguerre  (1001) sudo        (27)        0 2022-07-26 16:06:21.342227 elasticcsv-0.2.2/
--rw-r--r--   0 juguerre  (1001) sudo        (27)     1084 2022-05-06 06:56:24.000000 elasticcsv-0.2.2/LICENSE.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)       24 2022-05-06 06:56:24.000000 elasticcsv-0.2.2/MANIFEST.in
--rw-r--r--   0 juguerre  (1001) sudo        (27)     2996 2022-07-26 16:06:21.342227 elasticcsv-0.2.2/PKG-INFO
--rw-r--r--   0 juguerre  (1001) sudo        (27)     2765 2022-07-26 15:50:04.000000 elasticcsv-0.2.2/README.md
-drwxr-xr-x   0 juguerre  (1001) sudo        (27)        0 2022-07-26 16:06:21.342227 elasticcsv-0.2.2/elasticcsv/
--rw-r--r--   0 juguerre  (1001) sudo        (27)        0 2022-05-06 06:56:24.000000 elasticcsv-0.2.2/elasticcsv/__init__.py
--rw-r--r--   0 juguerre  (1001) sudo        (27)     3389 2022-07-26 16:00:52.000000 elasticcsv-0.2.2/elasticcsv/csv2es.py
--rw-r--r--   0 juguerre  (1001) sudo        (27)     7956 2022-07-26 15:42:18.000000 elasticcsv-0.2.2/elasticcsv/elastic_csv.py
--rw-r--r--   0 juguerre  (1001) sudo        (27)     5190 2022-06-25 10:15:11.000000 elasticcsv-0.2.2/elasticcsv/elastic_wrapper.py
-drwxr-xr-x   0 juguerre  (1001) sudo        (27)        0 2022-07-26 16:06:21.342227 elasticcsv-0.2.2/elasticcsv.egg-info/
--rw-r--r--   0 juguerre  (1001) sudo        (27)     2996 2022-07-26 16:06:21.000000 elasticcsv-0.2.2/elasticcsv.egg-info/PKG-INFO
--rw-r--r--   0 juguerre  (1001) sudo        (27)      390 2022-07-26 16:06:21.000000 elasticcsv-0.2.2/elasticcsv.egg-info/SOURCES.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)        1 2022-07-26 16:06:21.000000 elasticcsv-0.2.2/elasticcsv.egg-info/dependency_links.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)       49 2022-07-26 16:06:21.000000 elasticcsv-0.2.2/elasticcsv.egg-info/entry_points.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)      363 2022-07-26 16:06:21.000000 elasticcsv-0.2.2/elasticcsv.egg-info/requires.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)       11 2022-07-26 16:06:21.000000 elasticcsv-0.2.2/elasticcsv.egg-info/top_level.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)      149 2022-06-25 09:24:11.000000 elasticcsv-0.2.2/pyproject.toml
--rw-r--r--   0 juguerre  (1001) sudo        (27)      380 2022-05-06 06:56:24.000000 elasticcsv-0.2.2/requirements.txt
--rw-r--r--   0 juguerre  (1001) sudo        (27)       78 2022-07-26 16:06:21.346227 elasticcsv-0.2.2/setup.cfg
--rw-r--r--   0 juguerre  (1001) sudo        (27)      781 2022-07-26 16:06:13.000000 elasticcsv-0.2.2/setup.py
+-rw-r--r--   0        0        0     1085 2022-12-03 16:21:05.538512 elasticcsv-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     2765 2022-12-03 16:21:05.414512 elasticcsv-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2022-12-03 16:21:05.566512 elasticcsv-0.2.3/elasticcsv/__init__.py
+-rw-r--r--   0        0        0     3741 2023-04-12 17:54:09.123621 elasticcsv-0.2.3/elasticcsv/csv2es.py
+-rw-r--r--   0        0        0     8762 2023-04-12 18:11:45.640277 elasticcsv-0.2.3/elasticcsv/elastic_csv.py
+-rw-r--r--   0        0        0     5223 2022-12-03 16:21:05.574512 elasticcsv-0.2.3/elasticcsv/elastic_wrapper.py
+-rw-r--r--   0        0        0      652 2023-04-12 18:46:01.429253 elasticcsv-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3687 1970-01-01 00:00:00.000000 elasticcsv-0.2.3/setup.py
+-rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 elasticcsv-0.2.3/PKG-INFO
```

### Comparing `elasticcsv-0.2.2/LICENSE.txt` & `elasticcsv-0.2.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `elasticcsv-0.2.2/PKG-INFO` & `elasticcsv-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: elasticcsv
-Version: 0.2.2
-Summary: Elasctic load CSV utility
-Home-page: 
-Author: juguerre
-Author-email: juguerre@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Elastic CSV Loader
 
 This command line utility loads csv file into an elasticsearch index, using a provided yaml config file.
 
 `load-csv` considerations:
 
 - CSV files MUST include a header with field names
```

### Comparing `elasticcsv-0.2.2/README.md` & `elasticcsv-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: elasticcsv
+Version: 0.2.3
+Summary: elasticsearch csv upload download utility
+Author: J. Andres Guerrero
+Author-email: jaguerrero@caixabanktech.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: elasticsearch (<8.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: python-box (>=7.0.1,<8.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Description-Content-Type: text/markdown
+
 # Elastic CSV Loader
 
 This command line utility loads csv file into an elasticsearch index, using a provided yaml config file.
 
 `load-csv` considerations:
 
 - CSV files MUST include a header with field names
@@ -92,7 +114,8 @@
 Example:
 
 ```text
 csv2es load-csv --csv ./pathtomyfile/file.csv --index myindex --sep ";"
 
 csv2es download-index --csv ./pathtomyfile/file.csv --index myindex --sep ";" -d
 ```
+
```

### Comparing `elasticcsv-0.2.2/elasticcsv/csv2es.py` & `elasticcsv-0.2.3/elasticcsv/csv2es.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 @click.group()
 def cli():
     logging.basicConfig(
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s", level="WARNING"
     )
     logging.getLogger(__name__).setLevel(logging.DEBUG)
     logging.getLogger("elasticcsv").setLevel(logging.DEBUG)
+    logging.getLogger("elasticsearch").setLevel(logging.INFO)
 
 
 @cli.command()
 @click.option("--csv", type=click.Path(exists=True), help="CSV File", required=True)
 @click.option("--sep", type=click.STRING, help="CSV field sepator", required=True)
 @click.option("--index", type=click.STRING, help="Elastic Index", required=True)
 @click.option("--csv_offset", type=click.INT, help="CSV file offset", default=0)
@@ -54,40 +55,49 @@
     "--delete-if-exists",
     "-d",
     type=click.BOOL,
     is_flag=True,
     help="Flag for deleting index before running load",
     default=False,
 )
+@click.option(
+    "--dict-columns",
+    type=click.STRING,
+    help="Comma separated list of colums of type dict to load as dicts",
+    required=False,
+)
 def load_csv(
     csv: str,
     csv_offset: int,
     index: str,
     csv_date_format: str,
     sep: str,
     logic_date: datetime,
     delete_if_exists: bool,
+    dict_columns: str,
 ):
     """Loads csv to elastic index"""
     _load_config()
     logger.info(f"Loading file: {csv}")
     logger.info(f"CSV Date Format: {csv_date_format}")
 
     logic_date = logic_date.date() if logic_date else date.today()
     if delete_if_exists:
         if not elastic_csv.delete_index(config, index=index):
             logger.warning(f"Index {index} not exists and will not be deleted. Continuing anyway")
+    dict_columns = dict_columns.strip().split(",") if dict_columns else None
     elastic_csv.load_csv(
         config=config,
         csv_file_name=csv,
         index=index,
         delimiter=sep,
         csv_date_format=csv_date_format,
         logic_date=logic_date,
         csv_offset=csv_offset,
+        dict_columns=dict_columns,
     )
 
 
 @cli.command()
 @click.option("--csv", type=click.Path(exists=False), help="CSV File", required=True)
 @click.option("--sep", type=click.STRING, help="CSV field sepator", required=True)
 @click.option("--index", type=click.STRING, help="Elastic Index", required=True)
```

### Comparing `elasticcsv-0.2.2/elasticcsv/elastic_csv.py` & `elasticcsv-0.2.3/elasticcsv/elastic_csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 import csv
 import logging
 import math
 import re
 from datetime import datetime, date
 from typing import Iterator, List, Any, Dict, Generator, Literal
+
 import pandas as pd
 import pytz
 from box import Box
 from tqdm import tqdm
 
 from elasticcsv.elastic_wrapper import ElasticWrapper
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_CSV_WRITE_CHUNK_SIZE = 50000
 
 
 def download_csv(
     config: Box, csv_file_name: str, index: str, delimiter: str, file_mode: Literal["a", "w"] = "a"
-):
+) -> int:
     """Main process to load csv to elastic
     :param file_mode: Open mode for CSV file (a: append, w: write), write mode resets file before write
     :param config: Dictionary with elasctic connection data
     :param csv_file_name: csv file path
     :param index: index name (_index)
     :param delimiter: csv delimiter
     """
     e_wrapper = ElasticWrapper(config.elastic_connection)
     es_iterator = e_wrapper.scan(index=index)
-    _write_csv(es_iterator, csv_file_name=csv_file_name, delimiter=delimiter, file_mode=file_mode)
+    regs: int = _write_csv(
+        es_iterator, csv_file_name=csv_file_name, delimiter=delimiter, file_mode=file_mode
+    )
+    return regs
 
 
 def load_csv(
     config: Box,
     csv_file_name: str,
     index: str,
     delimiter: str,
     csv_date_format: str = None,
     logic_date: date = date.today(),
     csv_offset: int = 0,
+    dict_columns: List[str] = None,
 ):
     """Main process to load csv to elastic
+    :param csv_offset:
+    :param dict_columns:
     :param config: Dictionary with elasctic connection data
     :param csv_file_name: csv file path
     :param index: index name (_index)
     :param delimiter: csv delimiter
     :param csv_date_format: date format spec as '%Y-%m-%d'
     :param logic_date:
     """
@@ -53,17 +60,18 @@
         filepath=csv_file_name,
         delimiter=delimiter,
         logic_date=logic_date,
         transform_to_data=parent_data,
         count_lines=True,
         csv_date_format=csv_date_format,
         csv_offset=csv_offset,
+        dict_columns=dict_columns,
     )
     e_wrapper = ElasticWrapper(config.elastic_connection)
-    e_wrapper.bulk_dataset(data_iterator=csv_iterator, index=index)
+    return e_wrapper.bulk_dataset(data_iterator=csv_iterator, index=index)
 
 
 def delete_index(config: Box, index: str) -> bool:
     e_wrapper = ElasticWrapper(config.elastic_connection)
     return e_wrapper.delete_index(index=index)
 
 
@@ -72,14 +80,15 @@
     delimiter: str = None,
     chunk_size: int = 10000,
     logic_date: date = date.today(),
     transform_to_data: bool = True,
     count_lines: bool = False,
     csv_date_format: str = None,
     csv_offset: int = 0,
+    dict_columns: List[str] = None,
 ) -> Generator[dict, None, None]:
     """Returns an iterator of dicts
 
     :param filepath:
     :param delimiter:
     :param chunk_size:
     :param logic_date:
@@ -118,55 +127,63 @@
         chunk.fillna("", inplace=True)
         chunk["@timestamp"] = ts
         chunk["date"] = date_str
         chunk = chunk.astype(str)
 
         if csv_date_format:
             _format_date_columns(chunk, csv_date_format)
+        if dict_columns:
+            _eval_dict_columns(chunk, dict_columns)
 
         for d in chunk.to_dict("records"):
             if transform_to_data:
-                d = {k: value.strip() for k, value in d.items() if isinstance(value, str)}
+                d = {
+                    k: value
+                    for k, value in d.items()
+                    if isinstance(value, str) or isinstance(value, dict)
+                }
                 yield _transform_to_data_struct(d)
             else:
                 yield d
 
 
 def _write_csv(
     es_iterator: Iterator[dict],
     csv_file_name: str,
     delimiter: str,
     file_mode: Literal["a", "w"],
     chunk_size: int = DEFAULT_CSV_WRITE_CHUNK_SIZE,
     encoding: str = "utf-8",
-):
+) -> int:
     """
 
     :param es_iterator: elastic iterator returning hits
     :param csv_file_name: file to append hits as csv rows
     :param file_mode: File open mode (a, w)
     :param encoding:
     :param chunk_size:
 
-    :return:
+    :return: Total registers
     """
+    total_registers = 0
     data = True
     first_chunk = True
     while data:
         dicts: List[dict] = []
         i = 0
         for i, hit in tqdm(
             enumerate(es_iterator),
             desc=f"Download chunk of hits ({DEFAULT_CSV_WRITE_CHUNK_SIZE})",
             unit=" hit",
         ):
             # ! hit.get("_source")
             dicts.append(hit.get("_source"))
             if i >= chunk_size:
                 break
+            i += 1
         if i < chunk_size:
             data = False
         if not dicts:
             logger.debug(f"Nothing to write to csv_filename: {csv_file_name}")
         else:
             # flatten dict values (only one level) as key1.key11: value11
             if any([isinstance(value, dict) for value in list(dicts[0].values())]):
@@ -176,15 +193,19 @@
                 headers = list((dicts[0].keys()))
                 writer = csv.DictWriter(
                     f, fieldnames=headers, delimiter=delimiter, extrasaction="ignore"
                 )
                 if first_chunk:
                     writer.writeheader()
                 writer.writerows(dicts)
+                total_registers += len(dicts)
             first_chunk = False
+            # * Second chunk has to be append, avoiding "w" config
+            file_mode = "a"
+    return total_registers
 
 
 def _flatten_dict(dct: dict) -> dict:
     new_fields = {}
     for k, v in list(dct.items()):
         if isinstance(v, dict):
             for kk, vv in list(v.items()):
@@ -214,14 +235,15 @@
         keys = list(filter(lambda k: k[0] in ["_", "@"] or k in ["date"], list(registro.keys())))
     new_reg: Dict[str, str] = {
         k: registro[k]
         for k in keys
         if isinstance(registro[k], str)
         or isinstance(registro[k], int)
         or isinstance(registro[k], float)
+        or isinstance(registro[k], dict)
     }
     return new_reg
 
 
 def _count_generator(raw_reader: callable) -> Generator[bytes, None, None]:
     b = raw_reader(1024 * 1024)
     while b:
@@ -248,7 +270,12 @@
             return None
         format_d_str = datetime.strptime(d_str, csv_date_format).isoformat()
         return format_d_str
 
     date_columns = list(filter(lambda c: re.findall(f".*_date$", c), chunk.columns))
     for col in date_columns:
         chunk[col] = chunk[col].apply(format_dates)
+
+
+def _eval_dict_columns(chunk: pd.DataFrame, dict_columns: List[str]):
+    for col in dict_columns:
+        chunk[col] = chunk[col].apply(eval)
```

### Comparing `elasticcsv-0.2.2/elasticcsv/elastic_wrapper.py` & `elasticcsv-0.2.3/elasticcsv/elastic_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         super(MyConnection, self).__init__(*args, **kwargs)
         self.session.proxies = proxies
 
 
 class ElasticWrapper(object):
     """Wrapper for Elasticsearch object"""
 
-    ELASTICSEARCH_TIMEOUT = 80
+    ELASTICSEARCH_TIMEOUT = 120
     DEFAULT_QUERY_SIZE = 10000
     DEFAULT_QUERY_CHUNK_SIZE = 5000
 
     def __init__(self, conn_conf: Box):
         """ElasticWrapper
 
         :param conn_conf: Box instance with connection info
@@ -103,23 +103,23 @@
     # ********
 
     @staticmethod
     def _generate_actions(dataset):
         for element in dataset:
             yield element
 
-    def bulk_dataset(self, data_iterator: Iterator[dict], index: str):
+    def bulk_dataset(self, data_iterator: Iterator[dict], index: str) -> int:
         """
         Función: bulk_dataset
         Descripción: Ingesta Dataset en formato array de objetos Json en elasticsearch
 
         :param data_iterator: Array de documentos ha realizar bulk en elasticsearch
         (Formato: [{..},{..},...])
         :param index: indice sobre el que se van a ingestar los datos
-        :returns: ElasticJobResult
+        :returns: num docs indexed
         """
         logger.info(f"Connection to Elasticsearch : {self._connection}")
         progress = tqdm(unit="docs")
         successes = fails = 0
         action = None
         try:
             for ok, action in streaming_bulk(
@@ -138,14 +138,15 @@
 
                 progress.update(1)
         except ElasticsearchException as ee:
             logger.error(f"Action: {ee.args}, {action if action else None}")
         progress.close()
         logger.info("Documentos indexados: %d", successes)
         logger.warning(f"Documents not indexed: {fails}")
+        return successes
 
     @staticmethod
     def _result_from_generator(es_generator: Iterator) -> dict:
         hits = []
         tick = time.perf_counter_ns()
         for element in es_generator:
             hits.append(element)
```

