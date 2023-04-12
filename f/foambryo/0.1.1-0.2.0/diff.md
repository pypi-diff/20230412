# Comparing `tmp/foambryo-0.1.1.tar.gz` & `tmp/foambryo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Virtual_Embryo/Gitlab/pip_libraries/foambryo/dist/.tmp-6fldxvu_/foambryo-0.1.1.tar", last modified: Mon Feb  6 20:36:29 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-8bmil7we/foambryo-0.2.0.tar", last modified: Wed Apr 12 12:41:04 2023, max compression
```

## Comparing `foambryo-0.1.1.tar` & `foambryo-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-02-06 20:36:29.323499 foambryo-0.1.1/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     8996 2023-02-06 20:36:29.323627 foambryo-0.1.1/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     8366 2023-02-06 20:35:27.000000 foambryo-0.1.1/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2022-07-13 10:39:51.000000 foambryo-0.1.1/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-02-06 20:36:29.324348 foambryo-0.1.1/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-02-06 20:36:29.311488 foambryo-0.1.1/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-02-06 20:36:29.314672 foambryo-0.1.1/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      220 2023-02-06 20:31:47.000000 foambryo-0.1.1/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-02-06 20:36:29.323052 foambryo-0.1.1/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     8996 2023-02-06 20:36:29.000000 foambryo-0.1.1/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      238 2023-02-06 20:36:29.000000 foambryo-0.1.1/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-02-06 20:36:29.000000 foambryo-0.1.1/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-02-06 20:36:29.000000 foambryo-0.1.1/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-02-06 20:36:29.000000 foambryo-0.1.1/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:41:04.462907 foambryo-0.2.0/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9426 2023-04-12 12:41:04.463110 foambryo-0.2.0/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     8796 2023-04-12 12:39:41.000000 foambryo-0.2.0/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2022-07-13 10:39:51.000000 foambryo-0.2.0/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-04-12 12:41:04.463988 foambryo-0.2.0/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:41:04.448097 foambryo-0.2.0/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:41:04.458360 foambryo-0.2.0/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    25141 2023-04-12 12:12:23.000000 foambryo-0.2.0/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-01-27 11:24:29.000000 foambryo-0.2.0/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-01-27 11:39:04.000000 foambryo-0.2.0/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10498 2023-02-06 20:31:53.000000 foambryo-0.2.0/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     8906 2023-01-27 12:31:28.000000 foambryo-0.2.0/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28913 2023-02-06 20:17:59.000000 foambryo-0.2.0/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-03-03 13:34:52.000000 foambryo-0.2.0/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 12:41:04.462388 foambryo-0.2.0/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9426 2023-04-12 12:41:04.000000 foambryo-0.2.0/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-04-12 12:41:04.000000 foambryo-0.2.0/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 12:41:04.000000 foambryo-0.2.0/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-04-12 12:41:04.000000 foambryo-0.2.0/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-04-12 12:41:04.000000 foambryo-0.2.0/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.1.1/PKG-INFO` & `foambryo-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,34 +13,34 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### foambryo
 
-**foambryor** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids `pip install foambryo`
+**foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids `pip install foambryo`
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
 Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
 
-<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
 
 
 
 
 We rely on **delaunay-watershed**, a tool we designed to reconstruct efficiently multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junctional angles and surfaces curvatures, and invert **Young-Dupré** and **Laplace** laws, to find back the physical parameters involved in the mechanical equilibrium: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
-pip install delaunaywatershed3d foambryo
+pip install foambryo
 ```
 
 ```py
 from dw3d import DCEL_Data, geometry_reconstruction_3d
 from foambryo import plot_force_inference, plot_tension_inference
 
 ## Load the labels
@@ -62,15 +62,15 @@
 ### Installation
 
 `pip install foambryo `
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
 
 They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
 The two main laws involved are: 
 - **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$
 - **Laplace Law:** $P_j - P_i = 2 \gamma_{ij} h_{ij}$ where $h_{ij}$ is the mean curvature of the interface between the cell i and j. `
 
 
@@ -128,29 +128,29 @@
 
 ---
 ### Biological use-cases
 #### Phallusia mammillata
 Phallusia mammillata is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
 We use data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
 #### C.elegans, constrained within a shell
 Caenorhabditis elegans is a widely studied model organism, with one of the most reproducible development. This earthworm is developing in a shell. As the shell topology is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to deduce the surface tensions of the membranes. We use data from the [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
 Gaussian and mean curvature can be plotted on our meshes, and are useful to study the properties of surfaces obtained from simulations. 
 We also plot the vertex area and volume derivatives, that appears in our variational formulas, the difference between the two principal curvatures and the sphere-fit residual that can be used to detect robust non-spherical CMC surfaces (see our paper for more details)
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
@@ -160,7 +160,8 @@
 If you use this tool, please cite the associated preprint: 
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **foambryo** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
 
 
 
+
```

### Comparing `foambryo-0.1.1/README.md` & `foambryo-0.2.0/src/foambryo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,46 @@
+Metadata-Version: 2.1
+Name: foambryo
+Version: 0.2.0
+Summary: Tension inference for 3D cell assemblies
+Home-page: https://github.com/sacha-ichbiah/foambryo
+Author: Sacha Ichbiah
+Author-email: sacha.ichbiah@college-de-france.fr
+Project-URL: Team website, https://www.turlierlab.com/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 ### foambryo
 
-**foambryor** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids `pip install foambryo`
+**foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids `pip install foambryo`
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
 Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
 
-<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
 
 
 
 
 We rely on **delaunay-watershed**, a tool we designed to reconstruct efficiently multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junctional angles and surfaces curvatures, and invert **Young-Dupré** and **Laplace** laws, to find back the physical parameters involved in the mechanical equilibrium: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
-pip install delaunaywatershed3d foambryo
+pip install foambryo
 ```
 
 ```py
 from dw3d import DCEL_Data, geometry_reconstruction_3d
 from foambryo import plot_force_inference, plot_tension_inference
 
 ## Load the labels
@@ -45,15 +62,15 @@
 ### Installation
 
 `pip install foambryo `
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
 
 They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
 The two main laws involved are: 
 - **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$
 - **Laplace Law:** $P_j - P_i = 2 \gamma_{ij} h_{ij}$ where $h_{ij}$ is the mean curvature of the interface between the cell i and j. `
 
 
@@ -111,29 +128,29 @@
 
 ---
 ### Biological use-cases
 #### Phallusia mammillata
 Phallusia mammillata is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
 We use data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
 #### C.elegans, constrained within a shell
 Caenorhabditis elegans is a widely studied model organism, with one of the most reproducible development. This earthworm is developing in a shell. As the shell topology is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to deduce the surface tensions of the membranes. We use data from the [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
 Gaussian and mean curvature can be plotted on our meshes, and are useful to study the properties of surfaces obtained from simulations. 
 We also plot the vertex area and volume derivatives, that appears in our variational formulas, the difference between the two principal curvatures and the sphere-fit residual that can be used to detect robust non-spherical CMC surfaces (see our paper for more details)
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
@@ -143,7 +160,8 @@
 If you use this tool, please cite the associated preprint: 
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **foambryo** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
 
 
 
+
```

### Comparing `foambryo-0.1.1/setup.cfg` & `foambryo-0.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foambryo
-version = 0.1.1
+version = 0.2.0
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls =
```

### Comparing `foambryo-0.1.1/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,29 @@
-Metadata-Version: 2.1
-Name: foambryo
-Version: 0.1.1
-Summary: Tension inference for 3D cell assemblies
-Home-page: https://github.com/sacha-ichbiah/foambryo
-Author: Sacha Ichbiah
-Author-email: sacha.ichbiah@college-de-france.fr
-Project-URL: Team website, https://www.turlierlab.com/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 ### foambryo
 
-**foambryor** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids `pip install foambryo`
+**foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids `pip install foambryo`
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
 Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
 
-<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
 
 
 
 
 We rely on **delaunay-watershed**, a tool we designed to reconstruct efficiently multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junctional angles and surfaces curvatures, and invert **Young-Dupré** and **Laplace** laws, to find back the physical parameters involved in the mechanical equilibrium: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
-pip install delaunaywatershed3d foambryo
+pip install foambryo
 ```
 
 ```py
 from dw3d import DCEL_Data, geometry_reconstruction_3d
 from foambryo import plot_force_inference, plot_tension_inference
 
 ## Load the labels
@@ -62,15 +45,15 @@
 ### Installation
 
 `pip install foambryo `
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
 
 They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
 The two main laws involved are: 
 - **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$
 - **Laplace Law:** $P_j - P_i = 2 \gamma_{ij} h_{ij}$ where $h_{ij}$ is the mean curvature of the interface between the cell i and j. `
 
 
@@ -128,29 +111,29 @@
 
 ---
 ### Biological use-cases
 #### Phallusia mammillata
 Phallusia mammillata is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
 We use data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
 #### C.elegans, constrained within a shell
 Caenorhabditis elegans is a widely studied model organism, with one of the most reproducible development. This earthworm is developing in a shell. As the shell topology is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to deduce the surface tensions of the membranes. We use data from the [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
 Gaussian and mean curvature can be plotted on our meshes, and are useful to study the properties of surfaces obtained from simulations. 
 We also plot the vertex area and volume derivatives, that appears in our variational formulas, the difference between the two principal curvatures and the sphere-fit residual that can be used to detect robust non-spherical CMC surfaces (see our paper for more details)
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
@@ -160,7 +143,8 @@
 If you use this tool, please cite the associated preprint: 
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **foambryo** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
 
 
 
+
```

