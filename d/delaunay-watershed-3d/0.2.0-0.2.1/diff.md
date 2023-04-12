# Comparing `tmp/delaunay_watershed_3d-0.2.0.tar.gz` & `tmp/delaunay_watershed_3d-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-ay5cnd5_/delaunay_watershed_3d-0.2.0.tar", last modified: Wed Apr 12 12:29:05 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-ux5a4ndb/delaunay_watershed_3d-0.2.1.tar", last modified: Wed Apr 12 16:46:22 2023, max compression
```

## Comparing `delaunay_watershed_3d-0.2.0.tar` & `delaunay_watershed_3d-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.869233 delaunay_watershed_3d-0.2.0/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 12:29:05.869374 delaunay_watershed_3d-0.2.0/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.0/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-12 12:29:05.870362 delaunay_watershed_3d-0.2.0/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.849294 delaunay_watershed_3d-0.2.0/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.862196 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.868895 delaunay_watershed_3d-0.2.0/src/dw3d/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Curvature.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    21435 2023-04-12 12:16:26.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Dcel.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6883 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Geometric_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    13451 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Geometry.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Graph_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Mask_reconstruction.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Networkx_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/__init__.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/functions.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.308648 delaunay_watershed_3d-0.2.1/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 16:46:22.308939 delaunay_watershed_3d-0.2.1/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.1/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-12 16:46:22.309951 delaunay_watershed_3d-0.2.1/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.287397 delaunay_watershed_3d-0.2.1/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.292802 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.307785 delaunay_watershed_3d-0.2.1/src/dw3d/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Curvature.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    21435 2023-04-12 12:16:26.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Dcel.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9381 2023-04-12 16:44:44.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Geometric_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    13451 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Geometry.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Graph_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Mask_reconstruction.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Networkx_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/__init__.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/functions.py
```

### Comparing `delaunay_watershed_3d-0.2.0/PKG-INFO` & `delaunay_watershed_3d-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.2.0
+Version: 0.2.1
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delaunay_watershed_3d-0.2.0/README.md` & `delaunay_watershed_3d-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/setup.cfg` & `delaunay_watershed_3d-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.2.0
+version = 0.2.1
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/VirtualEmbryo/delaunay-watershed
 project_urls =
```

### Comparing `delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-watershed-3d
-Version: 0.2.0
+Version: 0.2.1
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Curvature.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Curvature.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Dcel.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Dcel.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Geometric_utilities.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Geometric_utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -91,14 +91,91 @@
 
 def build_triangulation(labels,min_distance=5,mode='torch',prints=False):
     if mode == 'torch': 
         return(build_triangulation_torch(labels,(min_distance//2)*2 +1,prints))
     else : 
         return(build_triangulation_skimage(labels,min_distance,prints))
 
+
+def build_triangulation_torch(labels,min_distance=5,prints=False):#,size_shell=2,dist_shell=4):
+    if prints : 
+        print("Mode == Torch")
+        print("Kernel size =",min_distance)
+        print("Computing EDT ...")
+    t1 = time()
+    b = StandardLabelToBoundary()(labels)[0]
+    mask_2 = b
+    EDT_2 = euclidean_dt(mask_2)
+    #b = pad_mask(b)
+    mask_1 = 1-b
+    EDT_1 = euclidean_dt(mask_1)
+    inv = np.amax(EDT_2)-EDT_2
+    Total_EDT = (EDT_1+np.amax(EDT_2))*mask_1 + inv*mask_2
+    t2 = time()
+    if prints : print("EDT computed in ",np.round(t2-t1,2))
+
+    seeds_coords = []
+    print("checkpoint a")
+    nx,ny,nz = labels.shape
+    table_coords = create_coords(nx,ny,nz)
+    print("checkpoint b")
+    values_lbls = np.unique(labels) 
+    print("checkpoint c")
+        
+    flat_edt = Total_EDT.flatten()
+    flat_labels = labels.flatten()
+    print("checkpoint d")
+    
+    for i in values_lbls:
+        f_i = (flat_labels==i)
+        print("checkpoint 1")
+        seed = np.argmax(flat_edt[f_i])
+        print("checkpoint 2")
+        seeds_coords.append(table_coords[f_i][seed])
+        print("checkpoint 3")
+    print("checkpoint e")
+        
+    seeds_coords = np.array(seeds_coords)
+    seeds_indices = values_lbls
+    print("checkpoint f")
+    corners = give_corners(Total_EDT)
+    print("checkpoint g")
+    
+    t3 = time()
+    if prints : print("Searching local extremas ...")
+    EDT =Total_EDT + np.random.rand(nx,ny,nz)*1e-5
+    T = torch.tensor(EDT).unsqueeze(0)
+    kernel_size = min_distance
+    padding = kernel_size//2
+    F = torch.nn.MaxPool3d((kernel_size,kernel_size,kernel_size), stride=(1,1,1), padding=padding, dilation=1, return_indices=False, ceil_mode=False)
+
+    minpooled = F(-T)[0].numpy()
+    markers_min = (EDT+minpooled)==0
+    local_mins = table_coords[markers_min.flatten()]
+    if prints : print("Number of local minimas :",len(local_mins))
+
+    maxpooled = F(T)[0].numpy()
+    markers_max = (EDT-maxpooled)==0
+    local_maxes = table_coords[markers_max.flatten()]
+    if prints : print("Number of local maxes :",len(local_maxes))
+    
+    t4 = time()
+    if prints : print("Local minimas computed in ",np.round(t4-t3,2))
+    
+    all_points = np.vstack((corners,local_maxes,local_mins))
+    
+    if prints : print("Starting triangulation..")
+    
+    tesselation=Delaunay(all_points)
+
+    t5 = time()
+    if prints : print("Triangulation build in ",np.round(t5-t4,2))
+    
+    return(seeds_coords,seeds_indices, tesselation,Total_EDT)
+"""
 def build_triangulation_torch(labels,min_distance=5,prints=False):#,size_shell=2,dist_shell=4):
     if prints : 
         print("Mode == Torch")
         print("Kernel size =",min_distance)
         print("Computing EDT ...")
     t1 = time()
     b = StandardLabelToBoundary()(labels)[0]
@@ -159,14 +236,16 @@
     tesselation=Delaunay(all_points)
 
     t5 = time()
     if prints : print("Triangulation build in ",np.round(t5-t4,2))
     
     return(seeds_coords,seeds_indices, tesselation,Total_EDT)
 
+"""
+
 
 
 def build_triangulation_skimage(labels,min_distance=5,prints=False):
     if prints : 
         print("Mode == Skimage")
         print("min_distance =",min_distance)
         print("Computing EDT ...")
```

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Geometry.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Geometry.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Graph_functions.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Graph_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Mask_reconstruction.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Mesh_utilities.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/Networkx_functions.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/Networkx_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.0/src/dw3d/functions.py` & `delaunay_watershed_3d-0.2.1/src/dw3d/functions.py`

 * *Files identical despite different names*

