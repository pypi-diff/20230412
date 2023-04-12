# Comparing `tmp/delaunay_watershed_3d-0.1.3.tar.gz` & `tmp/delaunay_watershed_3d-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Virtual_Embryo/Gitlab/pip_libraries/delaunay_watershed_3d/dist/.tmp-1ss08d0n/delaunay_watersh", last modified: Fri Jan 27 12:51:59 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-ay5cnd5_/delaunay_watershed_3d-0.2.0.tar", last modified: Wed Apr 12 12:29:05 2023, max compression
```

## Comparing `delaunay_watershed_3d-0.1.3.tar` & `delaunay_watershed_3d-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-01-27 12:51:59.938749 delaunay_watershed_3d-0.1.3/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5748 2023-01-27 12:51:59.938915 delaunay_watershed_3d-0.1.3/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5059 2023-01-27 11:33:46.000000 delaunay_watershed_3d-0.1.3/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2022-07-13 10:39:51.000000 delaunay_watershed_3d-0.1.3/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     1022 2023-01-27 12:51:59.939806 delaunay_watershed_3d-0.1.3/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-01-27 12:51:59.926147 delaunay_watershed_3d-0.1.3/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-01-27 12:51:59.930502 delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5748 2023-01-27 12:51:59.000000 delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-01-27 12:51:59.000000 delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-01-27 12:51:59.000000 delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-01-27 12:51:59.000000 delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-01-27 12:51:59.000000 delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-01-27 12:51:59.938306 delaunay_watershed_3d-0.1.3/src/dw3d/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-01-27 12:26:53.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Curvature.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    21137 2023-01-27 12:26:35.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Dcel.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6883 2022-05-26 21:56:38.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Geometric_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11939 2023-01-27 12:40:58.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Geometry.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-01-27 11:54:21.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Graph_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2022-07-13 13:26:49.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Mask_reconstruction.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10504 2023-01-27 11:56:56.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2022-05-26 21:56:53.000000 delaunay_watershed_3d-0.1.3/src/dw3d/Networkx_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2022-07-13 14:27:19.000000 delaunay_watershed_3d-0.1.3/src/dw3d/__init__.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-01-27 11:55:05.000000 delaunay_watershed_3d-0.1.3/src/dw3d/functions.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.869233 delaunay_watershed_3d-0.2.0/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 12:29:05.869374 delaunay_watershed_3d-0.2.0/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.0/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-12 12:29:05.870362 delaunay_watershed_3d-0.2.0/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.849294 delaunay_watershed_3d-0.2.0/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.862196 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-12 12:29:05.000000 delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:29:05.868895 delaunay_watershed_3d-0.2.0/src/dw3d/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Curvature.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    21435 2023-04-12 12:16:26.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Dcel.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6883 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Geometric_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    13451 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Geometry.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Graph_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Mask_reconstruction.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/Networkx_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/__init__.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.0/src/dw3d/functions.py
```

### Comparing `delaunay_watershed_3d-0.1.3/PKG-INFO` & `delaunay_watershed_3d-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.1.3
+Version: 0.2.0
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
-Home-page: https://github.com/sacha-ichbiah/delaunay_watershed_3d
+Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Delaunay-Watershed 3D
 
-<img src="Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
 
 
 **Delaunay-Watershed-3D** is an algorithm designed to reconstruct a sparse representation of the geometry of tissues and cell nuclei from instance segmentations, in 3D. It accomplishes this by building multimaterial meshes from segmentation masks. These multimaterial meshes are perfectly suited for **storage, geometrical analysis, sharing** and **visualisation of data**. We provide high level APIs to extract geometrical features from the meshes, as well as visualisation tools based on [polyscope](https://polyscope.run) and [napari](https://napari.org).
 
 Delaunay-Watershed was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah, Matthieu Perez and Hervé Turlier. For support, please open an issue.
 A preprint of the method will be published soon. If you use our library in your work please cite the paper. 
 
 Introductory notebooks with precise use case are provided.
 The algorithm takes as input segmentation masks and return multimaterial triangle meshes (3D).
 
-This method is used as a backend for [forceviewer3d](https://www.todo), our 3D tension inference library.
+This method is used as a backend for [foambryo](https://github.com/VirtualEmbryo/foambryo), our 3D tension inference library.
 
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, and extract its geometry:
 
 ```shell
@@ -52,16 +52,17 @@
 DW.plot_cells_polyscope()
 v = DW.plot_in_napari(add_mesh=True)
 
 ## Use the mesh to analyze the geometry:
 Mesh=DW.return_dcel()
 Mesh.compute_curvatures_interfaces()
 Mesh.compute_areas_interfaces()
-Mesh.compute_volume_cells()
+Mesh.compute_volumes_cells()
 Mesh.compute_length_trijunctions()
+Mesh.compute_angles_junctions()
 
 ```
 
 ### Installation
 
 `pip install delaunay-watershed-3d`
 
@@ -93,32 +94,32 @@
     - `self.return_dcel()` return a `DCEL_Data` object, i.e a Half-edge implementation of the mesh
 
 #### 3 - Analyze the geometry
 
 A `DCEL_Data` object can be used to analyze the geometry:
 
 - `DCEL_Data:`
-    - `self.compute_angles_tri()` returns a dictionnary with the values of every angles formed by the cells (in rad)
+    - `self.compute_angles_junctions()` returns a dictionnary with the values of every angles formed by the cells (in rad)
     - `self.compute_compute_curvatures(laplacian = "robust",weighted = True)` returns a dictionnary with the values of the mean curvature averaged on all the vertices of all the interfaces. `laplacian` can be either "cotan" or "robust". If `weighted`, the sum is scaled with vertices areas.
-    - `self.compute_length_halfedges(), self.compute_areas_faces(), self.compute_centroids_cells(), self.compute_areas_cells(), self.compute_areas_interfaces(), self.compute_volume_cells(), compute_length_trijunctions()
+    - `self.compute_length_halfedges(), self.compute_areas_faces(), self.compute_centroids_cells(), self.compute_areas_cells(), self.compute_areas_interfaces(), self.compute_volumes_cells(), compute_length_trijunctions()
 
 ---
 ### Biological use-cases
 
 #### Geometrical reconstruction of P.Mammilata Embryo
 Data from [Guignard et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-![](Figures_readme/DW_3d.png "Title")
+![](https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/DW_3d.png "Title")
 
 #### Geometrical reconstruction of Cell Nuclei
 Data from [Stardist](https://github.com/stardist/stardist)
 
-![](Figures_readme/DW_3d_nuclei.png "Title")
+![](https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/DW_3d_nuclei.png "Title")
 
 ---
 
 
 ### Credits, contact, citations
-If you use this tool, please cite the associated preprint: 
+If you use this tool, please cite the associated preprint.
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **Delaunay-Watershed** could help biologists and physicists to shed light on the mechanical aspects of early development.
```

### Comparing `delaunay_watershed_3d-0.1.3/README.md` & `delaunay_watershed_3d-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Delaunay-Watershed 3D
 
-<img src="Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
 
 
 **Delaunay-Watershed-3D** is an algorithm designed to reconstruct a sparse representation of the geometry of tissues and cell nuclei from instance segmentations, in 3D. It accomplishes this by building multimaterial meshes from segmentation masks. These multimaterial meshes are perfectly suited for **storage, geometrical analysis, sharing** and **visualisation of data**. We provide high level APIs to extract geometrical features from the meshes, as well as visualisation tools based on [polyscope](https://polyscope.run) and [napari](https://napari.org).
 
 Delaunay-Watershed was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah, Matthieu Perez and Hervé Turlier. For support, please open an issue.
 A preprint of the method will be published soon. If you use our library in your work please cite the paper. 
 
 Introductory notebooks with precise use case are provided.
 The algorithm takes as input segmentation masks and return multimaterial triangle meshes (3D).
 
-This method is used as a backend for [forceviewer3d](https://www.todo), our 3D tension inference library.
+This method is used as a backend for [foambryo](https://github.com/VirtualEmbryo/foambryo), our 3D tension inference library.
 
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, and extract its geometry:
 
 ```shell
@@ -35,16 +35,17 @@
 DW.plot_cells_polyscope()
 v = DW.plot_in_napari(add_mesh=True)
 
 ## Use the mesh to analyze the geometry:
 Mesh=DW.return_dcel()
 Mesh.compute_curvatures_interfaces()
 Mesh.compute_areas_interfaces()
-Mesh.compute_volume_cells()
+Mesh.compute_volumes_cells()
 Mesh.compute_length_trijunctions()
+Mesh.compute_angles_junctions()
 
 ```
 
 ### Installation
 
 `pip install delaunay-watershed-3d`
 
@@ -76,32 +77,32 @@
     - `self.return_dcel()` return a `DCEL_Data` object, i.e a Half-edge implementation of the mesh
 
 #### 3 - Analyze the geometry
 
 A `DCEL_Data` object can be used to analyze the geometry:
 
 - `DCEL_Data:`
-    - `self.compute_angles_tri()` returns a dictionnary with the values of every angles formed by the cells (in rad)
+    - `self.compute_angles_junctions()` returns a dictionnary with the values of every angles formed by the cells (in rad)
     - `self.compute_compute_curvatures(laplacian = "robust",weighted = True)` returns a dictionnary with the values of the mean curvature averaged on all the vertices of all the interfaces. `laplacian` can be either "cotan" or "robust". If `weighted`, the sum is scaled with vertices areas.
-    - `self.compute_length_halfedges(), self.compute_areas_faces(), self.compute_centroids_cells(), self.compute_areas_cells(), self.compute_areas_interfaces(), self.compute_volume_cells(), compute_length_trijunctions()
+    - `self.compute_length_halfedges(), self.compute_areas_faces(), self.compute_centroids_cells(), self.compute_areas_cells(), self.compute_areas_interfaces(), self.compute_volumes_cells(), compute_length_trijunctions()
 
 ---
 ### Biological use-cases
 
 #### Geometrical reconstruction of P.Mammilata Embryo
 Data from [Guignard et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-![](Figures_readme/DW_3d.png "Title")
+![](https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/DW_3d.png "Title")
 
 #### Geometrical reconstruction of Cell Nuclei
 Data from [Stardist](https://github.com/stardist/stardist)
 
-![](Figures_readme/DW_3d_nuclei.png "Title")
+![](https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/DW_3d_nuclei.png "Title")
 
 ---
 
 
 ### Credits, contact, citations
-If you use this tool, please cite the associated preprint: 
+If you use this tool, please cite the associated preprint.
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **Delaunay-Watershed** could help biologists and physicists to shed light on the mechanical aspects of early development.
```

### Comparing `delaunay_watershed_3d-0.1.3/setup.cfg` & `delaunay_watershed_3d-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.1.3
+version = 0.2.0
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/sacha-ichbiah/delaunay_watershed_3d
+url = https://github.com/VirtualEmbryo/delaunay-watershed
 project_urls = 
 	Team website = https://www.turlierlab.com/
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
```

### Comparing `delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: delaunay-watershed-3d
-Version: 0.1.3
+Version: 0.2.0
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
-Home-page: https://github.com/sacha-ichbiah/delaunay_watershed_3d
+Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Delaunay-Watershed 3D
 
-<img src="Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
 
 
 **Delaunay-Watershed-3D** is an algorithm designed to reconstruct a sparse representation of the geometry of tissues and cell nuclei from instance segmentations, in 3D. It accomplishes this by building multimaterial meshes from segmentation masks. These multimaterial meshes are perfectly suited for **storage, geometrical analysis, sharing** and **visualisation of data**. We provide high level APIs to extract geometrical features from the meshes, as well as visualisation tools based on [polyscope](https://polyscope.run) and [napari](https://napari.org).
 
 Delaunay-Watershed was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah, Matthieu Perez and Hervé Turlier. For support, please open an issue.
 A preprint of the method will be published soon. If you use our library in your work please cite the paper. 
 
 Introductory notebooks with precise use case are provided.
 The algorithm takes as input segmentation masks and return multimaterial triangle meshes (3D).
 
-This method is used as a backend for [forceviewer3d](https://www.todo), our 3D tension inference library.
+This method is used as a backend for [foambryo](https://github.com/VirtualEmbryo/foambryo), our 3D tension inference library.
 
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, and extract its geometry:
 
 ```shell
@@ -52,16 +52,17 @@
 DW.plot_cells_polyscope()
 v = DW.plot_in_napari(add_mesh=True)
 
 ## Use the mesh to analyze the geometry:
 Mesh=DW.return_dcel()
 Mesh.compute_curvatures_interfaces()
 Mesh.compute_areas_interfaces()
-Mesh.compute_volume_cells()
+Mesh.compute_volumes_cells()
 Mesh.compute_length_trijunctions()
+Mesh.compute_angles_junctions()
 
 ```
 
 ### Installation
 
 `pip install delaunay-watershed-3d`
 
@@ -93,32 +94,32 @@
     - `self.return_dcel()` return a `DCEL_Data` object, i.e a Half-edge implementation of the mesh
 
 #### 3 - Analyze the geometry
 
 A `DCEL_Data` object can be used to analyze the geometry:
 
 - `DCEL_Data:`
-    - `self.compute_angles_tri()` returns a dictionnary with the values of every angles formed by the cells (in rad)
+    - `self.compute_angles_junctions()` returns a dictionnary with the values of every angles formed by the cells (in rad)
     - `self.compute_compute_curvatures(laplacian = "robust",weighted = True)` returns a dictionnary with the values of the mean curvature averaged on all the vertices of all the interfaces. `laplacian` can be either "cotan" or "robust". If `weighted`, the sum is scaled with vertices areas.
-    - `self.compute_length_halfedges(), self.compute_areas_faces(), self.compute_centroids_cells(), self.compute_areas_cells(), self.compute_areas_interfaces(), self.compute_volume_cells(), compute_length_trijunctions()
+    - `self.compute_length_halfedges(), self.compute_areas_faces(), self.compute_centroids_cells(), self.compute_areas_cells(), self.compute_areas_interfaces(), self.compute_volumes_cells(), compute_length_trijunctions()
 
 ---
 ### Biological use-cases
 
 #### Geometrical reconstruction of P.Mammilata Embryo
 Data from [Guignard et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-![](Figures_readme/DW_3d.png "Title")
+![](https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/DW_3d.png "Title")
 
 #### Geometrical reconstruction of Cell Nuclei
 Data from [Stardist](https://github.com/stardist/stardist)
 
-![](Figures_readme/DW_3d_nuclei.png "Title")
+![](https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/DW_3d_nuclei.png "Title")
 
 ---
 
 
 ### Credits, contact, citations
-If you use this tool, please cite the associated preprint: 
+If you use this tool, please cite the associated preprint.
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **Delaunay-Watershed** could help biologists and physicists to shed light on the mechanical aspects of early development.
```

### Comparing `delaunay_watershed_3d-0.1.3/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.2.0/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Curvature.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Curvature.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Dcel.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Dcel.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,43 +274,46 @@
     Verts,Faces = Mesh.v, Mesh.f
         
     Clusters,Clusters_idx = separate_faces_dict_keep_idx(Faces)
     maxkey = np.amax(Faces[:,3:])
     All_verts=[]
     All_faces=[]
     All_idx=[]
+    All_faces_cluster_idx=[]
     offset = 0 
     embryo_centroid = np.mean(Verts,axis=0)
     clusters_displacements = {}
 
     for key in sorted(list(Clusters.keys())) : 
         if key ==0 : 
             continue
         faces = np.array(Clusters[key])
 
         vn,fn = renormalize_verts(Verts,faces)
         
-        #to change with a formula from ddg
+        #to change with a formula from DDG
         array_centroid = np.mean(vn,axis=0)
         vn = vn + coeff * (array_centroid - embryo_centroid)
         clusters_displacements[key]=(coeff * (array_centroid - embryo_centroid)).copy()
 
         All_verts.append(vn.copy())
         All_faces.append(fn.copy()+offset)
         All_idx.append(Clusters_idx[key])
-        
+        All_faces_cluster_idx.append(np.ones(len(fn))*key)
+
         offset+=len(vn)
     All_verts = np.vstack(All_verts)
     All_faces = np.vstack(All_faces)
+    All_faces_cluster_idx = np.hstack(All_faces_cluster_idx)
     All_idx = np.hstack(All_idx)
     Mesh.v_scattered = All_verts
     Mesh.f_scattered = All_faces
     Mesh.idx_scattered = All_idx
     Mesh.clusters_displacements = clusters_displacements
-        
+    Mesh.cluster_idx_scattered = All_faces_cluster_idx
 
 class DCEL_Data:
     """DCEL Graph containing faces, half-edges and vertices."""
     #Take a multimaterial mesh as an entry
     def __init__(self,Verts,Faces):
         for i, f in enumerate(Faces): 
             if f[3]>f[4]: 
@@ -376,14 +379,17 @@
 
     def compute_volumes_cells(self): 
         return(compute_volume_cells(self))
     
     def compute_volume_derivatives(self):
         return(compute_volume_derivative_dict(self))
 
+    def compute_angles_junctions(self,unique=True):
+        return(compute_angles_tri(self,unique=unique)[0])
+
     def compute_angles_tri(self,unique=True):
         return(compute_angles_tri(self,unique=unique))
 
     def compute_curvatures_interfaces(self,laplacian="robust",weighted=True):
         #"robust" or "cotan"
         return(compute_curvature_interfaces(self,laplacian=laplacian,weighted=weighted))
```

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Geometric_utilities.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Geometric_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Geometry.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Geometry.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     return(Length_trijunctions)
 
 def Compute_length_edges_trijunctions(verts,Edges_trijunctions):
     Pos = verts[Edges_trijunctions]
     Lengths = np.linalg.norm(Pos[:,0]-Pos[:,1],axis=1)
     return(Lengths)
 
-def extract_edges_trijunctions(Mesh,prints=False):
     F = Mesh.f
     E = np.vstack((F[:,[0,1]],F[:,[0,2]],F[:,[1,2]]))
     E = np.sort(E,axis=1)
     Zones = np.vstack((F[:,[3,4]],F[:,[3,4]],F[:,[3,4]]))
     key_mult = find_key_multiplier(len(Mesh.v)+1)
     K = (E[:,0]+1) + (E[:,1]+1)*key_mult
     Array,Index_first_occurence,Index_inverse,Index_counts = np.unique(K, return_index=True, return_inverse=True, return_counts=True)
@@ -59,14 +58,55 @@
     
     Output_dict = {}
     for key in sorted(Trijunctional_line.keys()):
         Output_dict[key] = np.vstack(Trijunctional_line[key])
     return(Output_dict)
 
 
+def extract_edges_trijunctions(Mesh,prints=False):
+    F = Mesh.f
+    E = np.vstack((F[:,[0,1]],F[:,[0,2]],F[:,[1,2]]))
+    E = np.sort(E,axis=1)
+    Zones = np.vstack((F[:,[3,4]],F[:,[3,4]],F[:,[3,4]]))
+    key_mult = find_key_multiplier(len(Mesh.v)+1)
+    K = (E[:,0]+1) + (E[:,1]+1)*key_mult
+    Array,Index_first_occurence,Index_inverse,Index_counts = np.unique(K, return_index=True, return_inverse=True, return_counts=True)
+    if prints : 
+        print("Number of trijunctional edges :",np.sum(Index_counts==3))
+    Edges_trijunctions = E[Index_first_occurence[Index_counts==3]]
+    
+
+    Indices = np.arange(len(Index_counts))
+    Map = {key:[] for key in Indices[Index_counts==3]}
+    Table = np.zeros(len(Index_counts))
+    Table[Index_counts==3]+=1
+
+    for i in range(len(Index_inverse)): 
+        inverse = Index_inverse[i]
+        if Table[inverse]==1 : 
+            Map[inverse].append(i)
+
+    Trijunctional_line={}
+    for key in sorted(Map.keys()) : 
+        x = Map[key]
+        regions = np.hstack((Zones[x[0]],Zones[x[1]],Zones[x[2]]))
+        u = np.unique(regions)
+        if len(u)>4 : 
+            print("oui")
+            continue
+        else : 
+            Trijunctional_line[tuple(u)]=Trijunctional_line.get(tuple(u),[])
+            Trijunctional_line[tuple(u)].append(E[x[0]])
+            assert(E[x[0]][0]==E[x[1]][0]==E[x[2]][0] and E[x[0]][1]==E[x[1]][1]==E[x[2]][1])
+    
+    Output_dict = {}
+    for key in sorted(Trijunctional_line.keys()):
+        Output_dict[key] = np.vstack(Trijunctional_line[key])
+    return(Output_dict)
+
 ## AREAS AND DERIVATIVES
 
 def Compute_Area_Faces(Verts,Faces):
     Pos = Verts[Faces]
     Sides = Pos-Pos[:,[2,0,1]]
 
     Lengths_sides =np.norm(Sides,dim=2)
```

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Graph_functions.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Graph_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Mask_reconstruction.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Mesh_utilities.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Mesh_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,19 +81,19 @@
 
     # dtype # 3 unsigned integers (long long) for the triangles # 2 integers for the labels
     dt=np.dtype([('triangles',np.uint64,(3,)), ('labels',np.int32,(2,))])
     t=np.fromfile(mesh_file,count=num_triangles,dtype=dt)
     mesh_file.close()
 
     Faces_num=t['triangles']
-    Faces_labels=t['labels'] - 1
+    Faces_labels=t['labels']
     Faces = np.hstack((Faces_num,Faces_labels))
     return(Verts, Faces.astype(int),np.array([num_vertices,num_triangles]))
 
-def read_rec_file_num(filename,offset=-1): 
+def read_rec_file_num(filename,offset=0): 
     mesh_file = open(filename, 'rb')
     Ns= []
     Verts = []
     Faces= []
 
     Lines=[]
     for line in mesh_file.readlines():
```

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/Networkx_functions.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/Networkx_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.1.3/src/dw3d/functions.py` & `delaunay_watershed_3d-0.2.0/src/dw3d/functions.py`

 * *Files identical despite different names*

