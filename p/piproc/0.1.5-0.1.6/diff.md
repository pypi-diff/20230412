# Comparing `tmp/piproc-0.1.5.tar.gz` & `tmp/piproc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piproc-0.1.5.tar", last modified: Wed Feb  8 20:34:51 2023, max compression
+gzip compressed data, was "piproc-0.1.6.tar", last modified: Wed Apr 12 12:37:11 2023, max compression
```

## Comparing `piproc-0.1.5.tar` & `piproc-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 20:34:51.714248 piproc-0.1.5/
--rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      266 2023-02-08 20:34:51.714248 piproc-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 20:34:51.695788 piproc-0.1.5/piproc/
--rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.5/piproc/__init__.py
--rw-rw-rw-   0        0        0    12050 2023-02-08 13:27:04.000000 piproc-0.1.5/piproc/main.py
--rw-rw-rw-   0        0        0     1570 2023-02-08 13:26:10.000000 piproc-0.1.5/piproc/tables.py
-drwxrwxrwx   0        0        0        0 2023-02-08 20:34:51.713248 piproc-0.1.5/piproc.egg-info/
--rw-rw-rw-   0        0        0      266 2023-02-08 20:34:51.000000 piproc-0.1.5/piproc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-02-08 20:34:51.000000 piproc-0.1.5/piproc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 20:34:51.000000 piproc-0.1.5/piproc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-02-08 20:34:51.000000 piproc-0.1.5/piproc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-08 20:34:51.000000 piproc-0.1.5/piproc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      356 2023-02-08 20:34:51.716242 piproc-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:37:10.995529 piproc-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-04-12 12:37:10.995529 piproc-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 12:37:10.978688 piproc-0.1.6/piproc/
+-rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.6/piproc/__init__.py
+-rw-rw-rw-   0        0        0    14204 2023-04-12 12:34:42.000000 piproc-0.1.6/piproc/main.py
+-rw-rw-rw-   0        0        0     2834 2023-04-12 12:34:42.000000 piproc-0.1.6/piproc/tables.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:37:10.994487 piproc-0.1.6/piproc.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 12:37:10.000000 piproc-0.1.6/piproc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      366 2023-04-12 12:37:10.997520 piproc-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.6/setup.py
```

### Comparing `piproc-0.1.5/LICENSE` & `piproc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `piproc-0.1.5/README.md` & `piproc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `piproc-0.1.5/piproc/main.py` & `piproc-0.1.6/piproc/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import os
 import yaml
 import boto3
 import psycopg2
 import sqlalchemy
 
 from sqlalchemy.orm import sessionmaker
+from shapely.geometry import Polygon
 from os.path import dirname as up
 
-from .tables import Processing, Products
+from .tables import Processing, Products, PlanetProc, PlanetProd
 
 class Piproc:
     '''
     Base class for piproc which handles all the communications between the Plastic-i
     modules and the processing database.
     '''
     def __init__(self):
@@ -54,15 +55,44 @@
 
     def close(self):
         '''
         Close the database connection
         '''
         self.session.close()
 
-    def check_download(self, tile_dict):
+    def check_planet_download(self, tile_dict, redownload):
+        '''
+        A function to check in the Plastic-i processing db if a Planet SuperDove scene has already
+        been downloaded.
+        '''
+        product_id = tile_dict['id']
+
+        tile_date = tile_dict['properties']['acquired']
+        tile_date = datetime.datetime.strptime(tile_date, '%Y-%m-%dT%H:%M:%SZ')
+        out_tile_date = datetime.datetime.strftime(tile_date, '%Y%m%d%H%M%S')
+
+        # TODO: This needs to be checked it produces the correct output with clipped imagery
+        bounds = Polygon(tile_dict['geometry']['coordinates'][0]).bounds
+        lats = str([bounds[1], bounds[3]])
+        lons = str([bounds[0], bounds[2]])
+
+        # Check that file hasn't already been downloaded
+        file = self.session.query(PlanetProc).get(product_id)
+        if file and not redownload:
+            return True, None, None
+        elif file and redownload:
+            return False, product_id, out_tile_date
+        else:
+
+            file = PlanetProc(id=product_id, lons=lons, lats=lats, tile_date=tile_date, 
+                              downloaded=0)
+            self.session.add(file)
+            return False, product_id, out_tile_date
+
+    def check_download(self, tile_dict, redownload):
         '''
         A function to check in the Plastic-i processing db if a tile has already been
         downloaded.
         '''
         product_id = tile_dict['id']
 
         try:
@@ -78,29 +108,35 @@
 
         bbox = tile_dict['bbox']
         lats = str([bbox[1], bbox[3]])
         lons = str([bbox[0], bbox[2]])
 
         # Check that file hasn't already been downloaded
         file = self.session.query(Processing).get(product_id)
-        if file:
+        if file and not redownload:
             return True, None, None
-
-        file = Processing(id=product_id, tile=tilename, lons=lons, 
-                        lats=lats, tile_date=tile_date, crs=crs,
-                        downloaded=0)
-        self.session.add(file)
-        return False, product_id, out_tile_date
+        elif file and redownload:
+            return False, product_id, out_tile_date
+        else:
+
+            file = Processing(id=product_id, tile=tilename, lons=lons, 
+                            lats=lats, tile_date=tile_date, crs=crs,
+                            downloaded=0)
+            self.session.add(file)
+            return False, product_id, out_tile_date
         
-    def update_download(self, product_id, file_path, result=2, env=None):
+    def update_download(self, product_id, file_path, result=2, env=None, satellite='sentinel2'):
         '''
         Update the processing db with the status of a sentinel-2 download
         '''
 
-        file = self.session.query(Processing).get(product_id)
+        if satellite == 'sentinel2':
+            file = self.session.query(Processing).get(product_id)
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProc).get(product_id)
 
         # Update database with download path, download status and number of times downloaded
         file.downloaded = result
         if result == 2:
             # Only update number of times downloaded if download was successful
             try:
                 file.no_downloaded += 1
@@ -111,22 +147,26 @@
             file.indexed = 0
 
             if env == 'k8s':
                 # Notify message queue that file has been downloaded when running with kubernetes.
                 self.notify(product_id, 'pifind_download')
         self.session.commit()
 
-    def check_indexing(self):
+    def check_indexing(self, satellite='sentinel2'):
         '''
         A function to check in the Plastic-i processing db if a tile has already been 
         indexed to the Plastic-i datacube.
         '''
 
-        file = self.session.query(Processing).filter(Processing.downloaded == 2,
-                                                Processing.indexed == 0).limit(1)
+        if satellite == 'sentinel2':
+            file = self.session.query(Processing).filter(Processing.downloaded == 2,
+                                                    Processing.indexed == 0).first()
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProc).filter(PlanetProc.downloaded == 2, 
+                                                        PlanetProc.indexed == 0).first()
 
         # Update row in db to indicate file is being processed
         file.indexed = -1
         self.session.commit()
 
         output = {'path': file.download_path,
                 'dt': file.tile_date,
@@ -149,33 +189,39 @@
         output = {'path': file.download_path,
                 'dt': file.tile_date,
                 'crs': file.crs,
                 'id': file.id
                 }
         return output
 
-    def update_index(self, product_id, yaml_path, result=2, env=None):
+    def update_index(self, product_id, yaml_path, satellite='sentinel2', result=2, env=None):
         '''
         Update the processing db with the status of a Sentinel-2 index process.
         '''
 
-        file = self.session.query(Processing).get(product_id)
+        if satellite == 'sentinel2':
+            file = self.session.query(Processing).get(product_id)
+        elif satellite == 'planet':
+            file = self.session.query(PlanetProc).get(product_id)
+
         file.indexed = result
 
         if result == 2:
             # Only update number of times downloaded if download was successful
             try:
                 file.no_indexed += 1
             except TypeError:
                 file.no_indexed = 1
             file.date_indexed = datetime.datetime.now()
             file.index_path = yaml_path
-            file.fdi = 0
             file.prediction = 0
 
+            if satellite == 'sentinel2':
+                file.fdi = 0
+            
             if env == 'k8s':
                 # Notify message queue that file has been downloaded when running with kubernetes.
                 self.notify(product_id, 'pifind_index')
 
         self.session.commit()
 
     def check_fdi(self):
```

### Comparing `piproc-0.1.5/piproc/tables.py` & `piproc-0.1.6/piproc/tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,8 +45,51 @@
     pred_path = Column(String)
     model = Column(String)
     avg = Column(Float)
     min = Column(Float)
     max = Column(Float)
     std = Column(Float)
     area = Column(Integer)
+    length = Column(Float)
+
+class PlanetProc(Base):
+    __tablename__ = 'planet_processing'
+
+    id = Column(String, primary_key=True)
+    lons = Column(String)
+    lats = Column(String)
+    tile_date = Column(DateTime)
+    crs = Column(Integer)
+    downloaded = Column(Integer)
+    no_downloaded = Column(Integer)
+    date_downloaded = Column(DateTime)
+    download_path = Column(String)
+    indexed = Column(Integer)
+    no_indexed = Column(Integer)
+    date_indexed = Column(DateTime)
+    index_path = Column(String)
+    prediction = Column(Integer)
+    no_prediction = Column(Integer)
+    date_prediction = Column(DateTime)
+    pred_path = Column(String)
+    model = Column(String)
+
+class PlanetProd(Base):
+    __tablename__ = 'planet_products'
+
+    id = Column(String, primary_key=True)
+    base_id = Column(String)
+    lons = Column(String)
+    lats = Column(String)
+    tile_date = Column(DateTime)
+    crs = Column(Integer)
+    prediction = Column(Integer)
+    no_prediction = Column(Integer)
+    date_prediction = Column(DateTime)
+    pred_path = Column(String)
+    model = Column(String)
+    avg = Column(Float)
+    min = Column(Float)
+    max = Column(Float)
+    std = Column(Float)
+    area = Column(Integer)
     length = Column(Float)
```

