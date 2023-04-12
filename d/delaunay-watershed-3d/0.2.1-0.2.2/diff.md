# Comparing `tmp/delaunay_watershed_3d-0.2.1.tar.gz` & `tmp/delaunay_watershed_3d-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-ux5a4ndb/delaunay_watershed_3d-0.2.1.tar", last modified: Wed Apr 12 16:46:22 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-3o4qv7iu/delaunay_watershed_3d-0.2.2.tar", last modified: Wed Apr 12 17:18:32 2023, max compression
```

## Comparing `delaunay_watershed_3d-0.2.1.tar` & `delaunay_watershed_3d-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.308648 delaunay_watershed_3d-0.2.1/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 16:46:22.308939 delaunay_watershed_3d-0.2.1/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.1/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-12 16:46:22.309951 delaunay_watershed_3d-0.2.1/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.287397 delaunay_watershed_3d-0.2.1/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.292802 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-12 16:46:22.000000 delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 16:46:22.307785 delaunay_watershed_3d-0.2.1/src/dw3d/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Curvature.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    21435 2023-04-12 12:16:26.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Dcel.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9381 2023-04-12 16:44:44.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Geometric_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    13451 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Geometry.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Graph_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Mask_reconstruction.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/Networkx_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/__init__.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.1/src/dw3d/functions.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.118678 delaunay_watershed_3d-0.2.2/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 17:18:32.118879 delaunay_watershed_3d-0.2.2/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.2/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-12 17:18:32.119633 delaunay_watershed_3d-0.2.2/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.102437 delaunay_watershed_3d-0.2.2/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.106364 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.118228 delaunay_watershed_3d-0.2.2/src/dw3d/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Curvature.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    21435 2023-04-12 12:16:26.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Dcel.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6880 2023-04-12 17:10:03.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Geometric_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    13501 2023-04-12 17:17:47.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Geometry.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Graph_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Mask_reconstruction.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Networkx_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/__init__.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/functions.py
```

### Comparing `delaunay_watershed_3d-0.2.1/PKG-INFO` & `delaunay_watershed_3d-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.2.1
+Version: 0.2.2
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delaunay_watershed_3d-0.2.1/README.md` & `delaunay_watershed_3d-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/setup.cfg` & `delaunay_watershed_3d-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.2.1
+version = 0.2.2
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/VirtualEmbryo/delaunay-watershed
 project_urls =
```

### Comparing `delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-watershed-3d
-Version: 0.2.1
+Version: 0.2.2
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delaunay_watershed_3d-0.2.1/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Curvature.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Curvature.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Dcel.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Dcel.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Geometric_utilities.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Geometric_utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -110,90 +110,14 @@
     EDT_1 = euclidean_dt(mask_1)
     inv = np.amax(EDT_2)-EDT_2
     Total_EDT = (EDT_1+np.amax(EDT_2))*mask_1 + inv*mask_2
     t2 = time()
     if prints : print("EDT computed in ",np.round(t2-t1,2))
 
     seeds_coords = []
-    print("checkpoint a")
-    nx,ny,nz = labels.shape
-    table_coords = create_coords(nx,ny,nz)
-    print("checkpoint b")
-    values_lbls = np.unique(labels) 
-    print("checkpoint c")
-        
-    flat_edt = Total_EDT.flatten()
-    flat_labels = labels.flatten()
-    print("checkpoint d")
-    
-    for i in values_lbls:
-        f_i = (flat_labels==i)
-        print("checkpoint 1")
-        seed = np.argmax(flat_edt[f_i])
-        print("checkpoint 2")
-        seeds_coords.append(table_coords[f_i][seed])
-        print("checkpoint 3")
-    print("checkpoint e")
-        
-    seeds_coords = np.array(seeds_coords)
-    seeds_indices = values_lbls
-    print("checkpoint f")
-    corners = give_corners(Total_EDT)
-    print("checkpoint g")
-    
-    t3 = time()
-    if prints : print("Searching local extremas ...")
-    EDT =Total_EDT + np.random.rand(nx,ny,nz)*1e-5
-    T = torch.tensor(EDT).unsqueeze(0)
-    kernel_size = min_distance
-    padding = kernel_size//2
-    F = torch.nn.MaxPool3d((kernel_size,kernel_size,kernel_size), stride=(1,1,1), padding=padding, dilation=1, return_indices=False, ceil_mode=False)
-
-    minpooled = F(-T)[0].numpy()
-    markers_min = (EDT+minpooled)==0
-    local_mins = table_coords[markers_min.flatten()]
-    if prints : print("Number of local minimas :",len(local_mins))
-
-    maxpooled = F(T)[0].numpy()
-    markers_max = (EDT-maxpooled)==0
-    local_maxes = table_coords[markers_max.flatten()]
-    if prints : print("Number of local maxes :",len(local_maxes))
-    
-    t4 = time()
-    if prints : print("Local minimas computed in ",np.round(t4-t3,2))
-    
-    all_points = np.vstack((corners,local_maxes,local_mins))
-    
-    if prints : print("Starting triangulation..")
-    
-    tesselation=Delaunay(all_points)
-
-    t5 = time()
-    if prints : print("Triangulation build in ",np.round(t5-t4,2))
-    
-    return(seeds_coords,seeds_indices, tesselation,Total_EDT)
-"""
-def build_triangulation_torch(labels,min_distance=5,prints=False):#,size_shell=2,dist_shell=4):
-    if prints : 
-        print("Mode == Torch")
-        print("Kernel size =",min_distance)
-        print("Computing EDT ...")
-    t1 = time()
-    b = StandardLabelToBoundary()(labels)[0]
-    mask_2 = b
-    EDT_2 = euclidean_dt(mask_2)
-    #b = pad_mask(b)
-    mask_1 = 1-b
-    EDT_1 = euclidean_dt(mask_1)
-    inv = np.amax(EDT_2)-EDT_2
-    Total_EDT = (EDT_1+np.amax(EDT_2))*mask_1 + inv*mask_2
-    t2 = time()
-    if prints : print("EDT computed in ",np.round(t2-t1,2))
-
-    seeds_coords = []
 
     nx,ny,nz = labels.shape
     table_coords = create_coords(nx,ny,nz)
     values_lbls = np.unique(labels) 
         
     flat_edt = Total_EDT.flatten()
     flat_labels = labels.flatten()
@@ -203,15 +127,14 @@
         seeds_coords.append(table_coords[f_i][seed])
         
     seeds_coords = np.array(seeds_coords)
     seeds_indices = values_lbls
 
     corners = give_corners(Total_EDT)
     
-    
     t3 = time()
     if prints : print("Searching local extremas ...")
     EDT =Total_EDT + np.random.rand(nx,ny,nz)*1e-5
     T = torch.tensor(EDT).unsqueeze(0)
     kernel_size = min_distance
     padding = kernel_size//2
     F = torch.nn.MaxPool3d((kernel_size,kernel_size,kernel_size), stride=(1,1,1), padding=padding, dilation=1, return_indices=False, ceil_mode=False)
@@ -236,15 +159,14 @@
     tesselation=Delaunay(all_points)
 
     t5 = time()
     if prints : print("Triangulation build in ",np.round(t5-t4,2))
     
     return(seeds_coords,seeds_indices, tesselation,Total_EDT)
 
-"""
 
 
 
 def build_triangulation_skimage(labels,min_distance=5,prints=False):
     if prints : 
         print("Mode == Skimage")
         print("min_distance =",min_distance)
```

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Geometry.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #Sacha Ichbiah, Sept 2021
 import numpy as np 
+from tqdm import tqdm
 
 def find_key_multiplier(num_points): 
     key_multiplier = 1
     while num_points//key_multiplier != 0 : 
         key_multiplier*=10
     return(key_multiplier)    
 
@@ -16,15 +17,15 @@
         Length_trijunctions[key] = np.sum(Compute_length_edges_trijunctions(Mesh.v,Edges_trijunctions[key]))
     return(Length_trijunctions)
 
 def Compute_length_edges_trijunctions(verts,Edges_trijunctions):
     Pos = verts[Edges_trijunctions]
     Lengths = np.linalg.norm(Pos[:,0]-Pos[:,1],axis=1)
     return(Lengths)
-
+"""
     F = Mesh.f
     E = np.vstack((F[:,[0,1]],F[:,[0,2]],F[:,[1,2]]))
     E = np.sort(E,axis=1)
     Zones = np.vstack((F[:,[3,4]],F[:,[3,4]],F[:,[3,4]]))
     key_mult = find_key_multiplier(len(Mesh.v)+1)
     K = (E[:,0]+1) + (E[:,1]+1)*key_mult
     Array,Index_first_occurence,Index_inverse,Index_counts = np.unique(K, return_index=True, return_inverse=True, return_counts=True)
@@ -57,15 +58,15 @@
             assert(E[x[0]][0]==E[x[1]][0]==E[x[2]][0] and E[x[0]][1]==E[x[1]][1]==E[x[2]][1])
     
     Output_dict = {}
     for key in sorted(Trijunctional_line.keys()):
         Output_dict[key] = np.vstack(Trijunctional_line[key])
     return(Output_dict)
 
-
+"""
 def extract_edges_trijunctions(Mesh,prints=False):
     F = Mesh.f
     E = np.vstack((F[:,[0,1]],F[:,[0,2]],F[:,[1,2]]))
     E = np.sort(E,axis=1)
     Zones = np.vstack((F[:,[3,4]],F[:,[3,4]],F[:,[3,4]]))
     key_mult = find_key_multiplier(len(Mesh.v)+1)
     K = (E[:,0]+1) + (E[:,1]+1)*key_mult
@@ -168,15 +169,15 @@
     for i, face in enumerate(Faces):
         i_x,i_y,i_z = Faces[i]
         a,b = Faces_label[i]
         List_indices_faces_per_vertices_x[(a,b)][i_x].append(i)
         List_indices_faces_per_vertices_y[(a,b)][i_y].append(i)
         List_indices_faces_per_vertices_z[(a,b)][i_z].append(i)
 
-    for key in DA.keys():
+    for key in tqdm(DA.keys()):
         for iv in range(len(Verts)):
             DA[key][iv] = np.vstack((cross_e3_x[List_indices_faces_per_vertices_x[key][iv]],
                                      cross_e3_y[List_indices_faces_per_vertices_y[key][iv]],
                                      cross_e3_z[List_indices_faces_per_vertices_z[key][iv]])).sum(axis=0)
 
     return(DA)
 
@@ -219,15 +220,15 @@
     DV = {key:np.zeros((len(Verts),3)) for key in materials}
 
     Coords = Verts[Faces]
     X,Y,Z = Coords[:,0],Coords[:,1],Coords[:,2]
     Cross_XY = np.cross(X,Y)/6
     Cross_YZ = np.cross(Y,Z)/6
     Cross_ZX = np.cross(Z,X)/6
-    Faces_material = np.zeros((len(materials),len(Faces)))
+    Faces_material = {mat:np.zeros(len(Faces)) for mat in materials}
     for n in materials:
         Faces_material[n][Faces_label[:,0]==1]=1
         Faces_material[n][Faces_label[:,1]==1]=-1
 
     List_indices_faces_per_vertices_pos_x={key:[[] for i in range(len(Verts))] for key in materials}
     List_indices_faces_per_vertices_pos_y={key:[[] for i in range(len(Verts))] for key in materials}
     List_indices_faces_per_vertices_pos_z={key:[[] for i in range(len(Verts))] for key in materials}
@@ -243,15 +244,15 @@
         List_indices_faces_per_vertices_pos_y[a][i_y].append(i)
         List_indices_faces_per_vertices_pos_z[a][i_z].append(i)
         
         List_indices_faces_per_vertices_neg_x[b][i_x].append(i)
         List_indices_faces_per_vertices_neg_y[b][i_y].append(i)
         List_indices_faces_per_vertices_neg_z[b][i_z].append(i)
     
-    for n in materials:
+    for n in tqdm(materials):
         for iv in range(len(Verts)):
             DV[n][iv] = np.vstack((Cross_YZ[List_indices_faces_per_vertices_pos_x[n][iv]],
                                       Cross_ZX[List_indices_faces_per_vertices_pos_y[n][iv]],
                                       Cross_XY[List_indices_faces_per_vertices_pos_z[n][iv]],
                                       - Cross_YZ[List_indices_faces_per_vertices_neg_x[n][iv]],
                                       - Cross_ZX[List_indices_faces_per_vertices_neg_y[n][iv]],
                                       - Cross_XY[List_indices_faces_per_vertices_neg_z[n][iv]])).sum(axis=0)
```

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Graph_functions.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Graph_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Mask_reconstruction.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Mesh_utilities.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/Networkx_functions.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/Networkx_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.1/src/dw3d/functions.py` & `delaunay_watershed_3d-0.2.2/src/dw3d/functions.py`

 * *Files identical despite different names*

