# Comparing `tmp/optim3d-0.1.9.tar.gz` & `tmp/optim3d-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\optim3d-0.1.9.tar", last modified: Thu Apr  6 15:17:41 2023, max compression
+gzip compressed data, was "dist\optim3d-0.2.1.tar", last modified: Wed Apr 12 14:14:33 2023, max compression
```

## Comparing `optim3d-0.1.9.tar` & `optim3d-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 15:17:41.000000 optim3d-0.1.9/
--rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.1.9/COPYING
--rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.1.9/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d/
-drwxrwxrwx   0        0        0        0 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d/config/
--rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.1.9/optim3d/config/reconstruct.json
--rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.1.9/optim3d/config/reconstruct_.json
--rw-rw-rw-   0        0        0    22145 2023-04-06 15:13:15.000000 optim3d-0.1.9/optim3d/main.py
--rw-rw-rw-   0        0        0        0 2023-04-06 14:11:05.000000 optim3d-0.1.9/optim3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    12418 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0      323 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 15:17:41.000000 optim3d-0.1.9/optim3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12418 2023-04-06 15:17:41.000000 optim3d-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    11381 2023-04-06 15:17:11.000000 optim3d-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 15:17:41.000000 optim3d-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-04-06 15:17:37.000000 optim3d-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:14:33.000000 optim3d-0.2.1/
+-rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.1/COPYING
+-rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-12 14:14:33.000000 optim3d-0.2.1/optim3d.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:14:32.000000 optim3d-0.2.1/optim3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-12 14:14:32.000000 optim3d-0.2.1/optim3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    14778 2023-04-12 14:14:32.000000 optim3d-0.2.1/optim3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:14:32.000000 optim3d-0.2.1/optim3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      222 2023-04-12 14:14:32.000000 optim3d-0.2.1/optim3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 14:14:32.000000 optim3d-0.2.1/optim3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14778 2023-04-12 14:14:33.000000 optim3d-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13741 2023-04-12 14:06:45.000000 optim3d-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:14:33.000000 optim3d-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-04-12 14:14:21.000000 optim3d-0.2.1/setup.py
```

### Comparing `optim3d-0.1.9/COPYING` & `optim3d-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `optim3d-0.1.9/LICENSE` & `optim3d-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optim3d-0.1.9/optim3d.egg-info/PKG-INFO` & `optim3d-0.2.1/optim3d.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.1.9
+Version: 0.2.1
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,35 +16,41 @@
 # Optimized reconstruction of large-scale 3D building models
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
 *Command-Line Interface (CLI) application for efficient and optimized reconstruction of large-scale 3D building models.*
 
-[GeoFlow](https://github.com/geoflow3d/geoflow-bundle) is a software tool that can be used to automatically reconstruct 3D building models from point clouds, with a high level of detail. It is a powerful tool for creating detailed and accurate 3D models of buildings and can be used in a variety of applications. The software is fully automated, making it easy to use and efficient for large-scale projects.
-
-Our program is based on GeoFlow and makes use of it to perform 3D reconstruction of buildings. The process is inspired by the 3D BAG project, which is an up-to-date dataset containing detailed 3D building models of the Netherlands, based on the official BAG data and national AHN point cloud. The optimization of the reconstruction process is achieved by indexing and tiling of the input data which reduces the processing time and resources needed to generate large-scale 3D building models. The indexing and tiling of both, 3D point cloud and 2D footprints, allows for more efficient processing and handling of the 3D reconstruction workflow.
+Optim3D is a powerful tool for optimized automatic reconstruction of highly detailed and large-scale 3D building models. Our tool is based on the [GeoFlow](https://github.com/geoflow3d/geoflow-bundle) software and makes use of it to perform the 3D reconstruction of buildings. The process is inspired by the 3D BAG project and optimized for large-scale projects through indexing and tiling of the input data, which significantly reduces the processing time and resources required to generate large-scale 3D building models.
 
 <img src="https://user-images.githubusercontent.com/72500344/212364590-b7fd444d-ec26-4a8b-bda9-fd4e1669bc6e.png" alt="Workflow of 3D Reconstruction" width="500"/>
 
+## Documentation
+
+If you are using Optim3D, we highly recommend that you take the time to read the [documentation](https://optim3d.readthedocs.io/en/latest/). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
+
 ## Installation
 
 You can install optim3d in your Conda environment by simply running:
 
 ```bash
+conda create --name optimenv python==3.6
+conda activate optimenv
+conda install -c conda-forge pdal python-pdal
+conda install -c conda-forge entwine
 pip install optim3d
 ```
 
-Youc can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
+You can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
 
-**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the License before using it.
+**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the LICENSE file.
 
 ## Usage of the CLI
 
-### Binary package
+### Python package
 
 After installation, you have a small program called <code>optim3d</code>. Use <code>optim3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d [OPTIONS] COMMAND [ARGS]...
 
   CLI tool to manage full optimized reconstruction of large-scale 3D
@@ -57,15 +63,15 @@
   index2d      QuadTree indexing and tiling of 2D building footprints.
   index3d      OcTree indexing of 3D point cloud using Entwine.
   tiler3d      Tiling of point cloud using the calculated processing areas.
   reconstruct  Optimized 3D reconstruction of buildings using GeoFlow.
   post         Post-processing generated CityJSON files.
 ```
 
-The process consists of five distinct steps or <code>commands</code> that must be executed in a specific order to achieve the desired outcome.
+The process consists of five steps or <code>commands</code> that must be executed in a specific order to achieve the desired outcome.
 
 #### Step 1 : 2D building footprints indexing and tiling
 
 Quadtree-based tiling scheme is used for spatial partitioning of building footprints. This assures that the reconstruction time per tile is more or less the same and that the tiles available for download are similar in file size. This is done using the first command <code>index2d</code>. Use <code>optim3d index2d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d index2d [OPTIONS] [FOOTPRINTS]
@@ -83,29 +89,29 @@
   --max INTEGER                   Maximum number of buildings per tile.
                                   [default: 3500]
   --help                          Show this message and exit.
 ```
 
 #### Step 2 : OcTree indexing of the 3D point cloud
 
-Processing large point cloud datasets is hardware-intensive. Therefore, it is necessary to index the 3D point cloud before processing. The index structure makes it possible to stream only the parts of the data that are required, without having to download the entire dataset. In this case, the spatial indexing of the airborne point cloud is performed using an octree structure. This can be easily done using Entwine, an open-source library for organizing and indexing large point cloud datasets using an octree data structure that allows fast and efficient spatial queries. This is done using the second command <code>index3d</code>. Use <code>optim3d index3d --help</code> to see the detailed help:
+Processing large point cloud datasets is hardware-intensive. Therefore, it is necessary to index the 3D point cloud before processing. The index structure makes it possible to stream only the parts of the data that are required, without having to download the entire dataset. In this case, the spatial indexing of the airborne point cloud is performed using an octree structure. This is done using the second command <code>index3d</code>. Use <code>optim3d index3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d index3d [OPTIONS] POINTCLOUD
 
   OcTree indexing of 3D point cloud using Entwine.
 
 Options:
   --output PATH  Output directory.  [default: ./output]
   --help         Show this message and exit.
 ```
 
 #### Step 3 : Tiling of the 3D point cloud
 
-The tiling of the indexed point cloud is based on processing areas calculated when the footprints were indexed. This is achieved using the third command <code>tiler3d</code>. Use <code>optim3d tiler3d --help</code> to see the detailed help:
+The tiling of the indexed point cloud is based on the processing areas already calculated. This is achieved using the third command <code>tiler3d</code>. Use <code>optim3d tiler3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d tiler3d [OPTIONS]
 
   Tiling of 3D point cloud using the calculated processing areas.
 
 Options:
@@ -115,15 +121,15 @@
                   ./output/indexed_pointcloud]
   --output PATH   Output directory.  [default: ./output]
   --help          Show this message and exit.
 ```
 
 #### Step 4 : 3D reconstruction of building models tile by tile
 
-The 3D reconstruction of building models is performed in this step. The process make use of GeoFlow to generate hight detailed 3D building models tile by tile. This is achieved using the fourth command <code>reconstruct</code>. Use <code>optim3d reconstruct --help</code> to see the detailed help:
+In this step, we perform the 3D reconstruction of building models. The process make use of GeoFlow to generate highly detailed 3D building models tile by tile. This is achieved using the fourth command <code>reconstruct</code>. Use <code>optim3d reconstruct --help</code> to see the detailed help:
 
 ```
 Usage: optim3d reconstruct [OPTIONS]
 
   Optimized 3D reconstruction of buildings using GeoFlow.
 
 Options:
@@ -133,39 +139,86 @@
                      ./output/footprint_tiles]
   --output PATH      Output directory.  [default: ./output]
   --help             Show this message and exit.
 ```
 
 #### Step 5 : Post-processing of CityJSON files
 
-The generated CityJSON files should be processed to add information about tiles to 3D objects. This is done using the fifth command <code>post</code>. Use <code>optim3d post --help</code> to see the detailed help:
+The generated CityJSON files should be post-processed to correct the City Objects IDs. This is done using the fifth command <code>post</code>. Use <code>optim3d post --help</code> to see the detailed help:
 
 ```
 Usage: optim3d post [OPTIONS]
 
   Postprocess the generated CityJSON files.
 
 Options:
   --cityjson PATH  CityJSON files directory.  [default:
                    ./output/model/cityjson]
   --help           Show this message and exit.
 ```
 
 ### Docker Image
 
-Coming soon.
+Optim3D is also available as [Docker image](https://hub.docker.com/r/yarroudh/optim3d). If you are using a Windows operating system, we recommend running the Docker container inside the Windows Subsystem for Linux 2 (WSL2) environment. Please ensure that Geoflow is installed on the WSL2 environment to ensure compatibility with the container.
+
+These are the steps to run Optim3D as a Docker container:
+
+1. First pull the image using the <code>docker pull</code> command:
+
+```bash
+docker pull yarroudh/optim3d
+```
+
+2. To run the Docker container and mount your data inside it, use the <code>docker run</code> command with the <code>-v</code> option to specify the path to the host directory and the path to the container directory where you want to mount the data folder. For example:
+
+```bash
+docker run -d -v ABSOLUTE_PATH_TO_HOST_DATA:/home/user/data yarroudh/optim3d
+```
+
+This command will start a Docker container in detached mode, mount the **ABSOLUTE_PATH_TO_HOST_DATA** directory on the host machine to the **/home/user/data** directory inside the container, and run the <code>yarroudh/optim3d</code> image. Do not change the path of the directory inside the container.
+
+3. Find the container ID and copy it. You can use the <code>docker ps</code> command to list all running containers and their IDs.
+4. Launch a command inside the container using <code>docker exec</code>, use the container ID or name and the command you want to run. For example:
 
+```bash
+docker exec CONTAINER_ID optim3d index2d data/FILE_NAME
+```
+This command will execute the QuadTree indexing of the 2D footprints data, which can be a Shapefile (.shp) or a GeoPackage (.gpkg).
+
+For the <code>reconstruct</code> command, make sure to copy Geoflow-bundle folder to the <code>$PATH</code> environment variable of the container before running the reconstruction:
+
+```bash
+docker cp PATH_TO_GEOFLOW_BUNDLE CONTAINER_ID:$PATH
+docker exec CONTAINER_ID optim3d reconstruct
+```
+
+5. To copy the output of the command from the container to a local path, use the <code>docker cp</code> command with the container ID or name, the path to the file inside the container, and the path to the destination on the host machine. For example:
+
+- To copy the output of one command:
+```bash
+docker cp CONTAINER_ID:/home/user/output/footprint_tiles PATH_ON_HOST_MACHINE
+```
+- Top copy the output of all the commands:
+```bash
+docker cp CONTAINER_ID:/home/user/output PATH_ON_HOST_MACHINE
+```
+
+6. Finally, after executing all the commands and copying the results to your local machine, you can stop the Docker container using the <code>docker stop</code> command followed by the container ID or name:
+
+```bash
+docker stop CONTAINER_ID
+```
 
 ### Building from source
 
-If you want to build the solution from source, you should follow the steps in [INSTALL.md](). The commands can be used as decribed for the Binary package.
+If you want to build the solution from source, you should follow the steps in [INSTALL.md]().
 
 ## Results
 
-The results of each command are saved in the <code>output</code> folder, which will look like this after executing all the commands:
+The results of each command are saved in the <code>output</code> folder with the following structure:
 
 ```bash
 â”œâ”€â”€ output
 â”‚   â”œâ”€â”€ flowcharts
 â”‚   â”‚   â”œâ”€â”€ *.json
 â”‚   â”œâ”€â”€ footprint_tiles
 â”‚   â”‚   â”œâ”€â”€ *.cpg
@@ -190,15 +243,15 @@
 â”‚   â”‚   â”œâ”€â”€ *.obj.mtl
 â”‚   â”œâ”€â”€ pointcloud_tiles
 â”‚   â”‚   â”œâ”€â”€ *.las
 â”‚   â”œâ”€â”€ processing_areas.gpkg
 â”‚   â””â”€â”€ quadtree.gpkg
 ```
 
-The 3D building models can be viewd using [Ninja](https://github.com/cityjson/ninja), the official web viewer for CityJSON files.
+The 3D building models can be inspected using [Ninja](https://github.com/cityjson/ninja), the official web viewer for CityJSON files.
 
 ![image](https://user-images.githubusercontent.com/72500344/216613188-82d54c75-7e03-4ee7-8c1c-d081e0c1d4ac.png)
 
 ## Related repositories
 
 [Automatic correction of buildings ground floor elevation in 3D City Models](https://github.com/Yarroudh/ZRect3D)
 
@@ -225,7 +278,8 @@
 Yarroudh, A. (2023). Optim3D: Optimized reconstruction of large-scale 3D building models [GitHub repository]. Retrieved from https://github.com/Yarroudh/Optim3D
 
 ## About Optim3D
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
 
+
```

### Comparing `optim3d-0.1.9/PKG-INFO` & `optim3d-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.1.9
+Version: 0.2.1
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,35 +16,41 @@
 # Optimized reconstruction of large-scale 3D building models
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
 *Command-Line Interface (CLI) application for efficient and optimized reconstruction of large-scale 3D building models.*
 
-[GeoFlow](https://github.com/geoflow3d/geoflow-bundle) is a software tool that can be used to automatically reconstruct 3D building models from point clouds, with a high level of detail. It is a powerful tool for creating detailed and accurate 3D models of buildings and can be used in a variety of applications. The software is fully automated, making it easy to use and efficient for large-scale projects.
-
-Our program is based on GeoFlow and makes use of it to perform 3D reconstruction of buildings. The process is inspired by the 3D BAG project, which is an up-to-date dataset containing detailed 3D building models of the Netherlands, based on the official BAG data and national AHN point cloud. The optimization of the reconstruction process is achieved by indexing and tiling of the input data which reduces the processing time and resources needed to generate large-scale 3D building models. The indexing and tiling of both, 3D point cloud and 2D footprints, allows for more efficient processing and handling of the 3D reconstruction workflow.
+Optim3D is a powerful tool for optimized automatic reconstruction of highly detailed and large-scale 3D building models. Our tool is based on the [GeoFlow](https://github.com/geoflow3d/geoflow-bundle) software and makes use of it to perform the 3D reconstruction of buildings. The process is inspired by the 3D BAG project and optimized for large-scale projects through indexing and tiling of the input data, which significantly reduces the processing time and resources required to generate large-scale 3D building models.
 
 <img src="https://user-images.githubusercontent.com/72500344/212364590-b7fd444d-ec26-4a8b-bda9-fd4e1669bc6e.png" alt="Workflow of 3D Reconstruction" width="500"/>
 
+## Documentation
+
+If you are using Optim3D, we highly recommend that you take the time to read the [documentation](https://optim3d.readthedocs.io/en/latest/). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
+
 ## Installation
 
 You can install optim3d in your Conda environment by simply running:
 
 ```bash
+conda create --name optimenv python==3.6
+conda activate optimenv
+conda install -c conda-forge pdal python-pdal
+conda install -c conda-forge entwine
 pip install optim3d
 ```
 
-Youc can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
+You can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
 
-**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the License before using it.
+**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the LICENSE file.
 
 ## Usage of the CLI
 
-### Binary package
+### Python package
 
 After installation, you have a small program called <code>optim3d</code>. Use <code>optim3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d [OPTIONS] COMMAND [ARGS]...
 
   CLI tool to manage full optimized reconstruction of large-scale 3D
@@ -57,15 +63,15 @@
   index2d      QuadTree indexing and tiling of 2D building footprints.
   index3d      OcTree indexing of 3D point cloud using Entwine.
   tiler3d      Tiling of point cloud using the calculated processing areas.
   reconstruct  Optimized 3D reconstruction of buildings using GeoFlow.
   post         Post-processing generated CityJSON files.
 ```
 
-The process consists of five distinct steps or <code>commands</code> that must be executed in a specific order to achieve the desired outcome.
+The process consists of five steps or <code>commands</code> that must be executed in a specific order to achieve the desired outcome.
 
 #### Step 1 : 2D building footprints indexing and tiling
 
 Quadtree-based tiling scheme is used for spatial partitioning of building footprints. This assures that the reconstruction time per tile is more or less the same and that the tiles available for download are similar in file size. This is done using the first command <code>index2d</code>. Use <code>optim3d index2d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d index2d [OPTIONS] [FOOTPRINTS]
@@ -83,29 +89,29 @@
   --max INTEGER                   Maximum number of buildings per tile.
                                   [default: 3500]
   --help                          Show this message and exit.
 ```
 
 #### Step 2 : OcTree indexing of the 3D point cloud
 
-Processing large point cloud datasets is hardware-intensive. Therefore, it is necessary to index the 3D point cloud before processing. The index structure makes it possible to stream only the parts of the data that are required, without having to download the entire dataset. In this case, the spatial indexing of the airborne point cloud is performed using an octree structure. This can be easily done using Entwine, an open-source library for organizing and indexing large point cloud datasets using an octree data structure that allows fast and efficient spatial queries. This is done using the second command <code>index3d</code>. Use <code>optim3d index3d --help</code> to see the detailed help:
+Processing large point cloud datasets is hardware-intensive. Therefore, it is necessary to index the 3D point cloud before processing. The index structure makes it possible to stream only the parts of the data that are required, without having to download the entire dataset. In this case, the spatial indexing of the airborne point cloud is performed using an octree structure. This is done using the second command <code>index3d</code>. Use <code>optim3d index3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d index3d [OPTIONS] POINTCLOUD
 
   OcTree indexing of 3D point cloud using Entwine.
 
 Options:
   --output PATH  Output directory.  [default: ./output]
   --help         Show this message and exit.
 ```
 
 #### Step 3 : Tiling of the 3D point cloud
 
-The tiling of the indexed point cloud is based on processing areas calculated when the footprints were indexed. This is achieved using the third command <code>tiler3d</code>. Use <code>optim3d tiler3d --help</code> to see the detailed help:
+The tiling of the indexed point cloud is based on the processing areas already calculated. This is achieved using the third command <code>tiler3d</code>. Use <code>optim3d tiler3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d tiler3d [OPTIONS]
 
   Tiling of 3D point cloud using the calculated processing areas.
 
 Options:
@@ -115,15 +121,15 @@
                   ./output/indexed_pointcloud]
   --output PATH   Output directory.  [default: ./output]
   --help          Show this message and exit.
 ```
 
 #### Step 4 : 3D reconstruction of building models tile by tile
 
-The 3D reconstruction of building models is performed in this step. The process make use of GeoFlow to generate hight detailed 3D building models tile by tile. This is achieved using the fourth command <code>reconstruct</code>. Use <code>optim3d reconstruct --help</code> to see the detailed help:
+In this step, we perform the 3D reconstruction of building models. The process make use of GeoFlow to generate highly detailed 3D building models tile by tile. This is achieved using the fourth command <code>reconstruct</code>. Use <code>optim3d reconstruct --help</code> to see the detailed help:
 
 ```
 Usage: optim3d reconstruct [OPTIONS]
 
   Optimized 3D reconstruction of buildings using GeoFlow.
 
 Options:
@@ -133,39 +139,86 @@
                      ./output/footprint_tiles]
   --output PATH      Output directory.  [default: ./output]
   --help             Show this message and exit.
 ```
 
 #### Step 5 : Post-processing of CityJSON files
 
-The generated CityJSON files should be processed to add information about tiles to 3D objects. This is done using the fifth command <code>post</code>. Use <code>optim3d post --help</code> to see the detailed help:
+The generated CityJSON files should be post-processed to correct the City Objects IDs. This is done using the fifth command <code>post</code>. Use <code>optim3d post --help</code> to see the detailed help:
 
 ```
 Usage: optim3d post [OPTIONS]
 
   Postprocess the generated CityJSON files.
 
 Options:
   --cityjson PATH  CityJSON files directory.  [default:
                    ./output/model/cityjson]
   --help           Show this message and exit.
 ```
 
 ### Docker Image
 
-Coming soon.
+Optim3D is also available as [Docker image](https://hub.docker.com/r/yarroudh/optim3d). If you are using a Windows operating system, we recommend running the Docker container inside the Windows Subsystem for Linux 2 (WSL2) environment. Please ensure that Geoflow is installed on the WSL2 environment to ensure compatibility with the container.
+
+These are the steps to run Optim3D as a Docker container:
+
+1. First pull the image using the <code>docker pull</code> command:
+
+```bash
+docker pull yarroudh/optim3d
+```
+
+2. To run the Docker container and mount your data inside it, use the <code>docker run</code> command with the <code>-v</code> option to specify the path to the host directory and the path to the container directory where you want to mount the data folder. For example:
+
+```bash
+docker run -d -v ABSOLUTE_PATH_TO_HOST_DATA:/home/user/data yarroudh/optim3d
+```
+
+This command will start a Docker container in detached mode, mount the **ABSOLUTE_PATH_TO_HOST_DATA** directory on the host machine to the **/home/user/data** directory inside the container, and run the <code>yarroudh/optim3d</code> image. Do not change the path of the directory inside the container.
+
+3. Find the container ID and copy it. You can use the <code>docker ps</code> command to list all running containers and their IDs.
+4. Launch a command inside the container using <code>docker exec</code>, use the container ID or name and the command you want to run. For example:
 
+```bash
+docker exec CONTAINER_ID optim3d index2d data/FILE_NAME
+```
+This command will execute the QuadTree indexing of the 2D footprints data, which can be a Shapefile (.shp) or a GeoPackage (.gpkg).
+
+For the <code>reconstruct</code> command, make sure to copy Geoflow-bundle folder to the <code>$PATH</code> environment variable of the container before running the reconstruction:
+
+```bash
+docker cp PATH_TO_GEOFLOW_BUNDLE CONTAINER_ID:$PATH
+docker exec CONTAINER_ID optim3d reconstruct
+```
+
+5. To copy the output of the command from the container to a local path, use the <code>docker cp</code> command with the container ID or name, the path to the file inside the container, and the path to the destination on the host machine. For example:
+
+- To copy the output of one command:
+```bash
+docker cp CONTAINER_ID:/home/user/output/footprint_tiles PATH_ON_HOST_MACHINE
+```
+- Top copy the output of all the commands:
+```bash
+docker cp CONTAINER_ID:/home/user/output PATH_ON_HOST_MACHINE
+```
+
+6. Finally, after executing all the commands and copying the results to your local machine, you can stop the Docker container using the <code>docker stop</code> command followed by the container ID or name:
+
+```bash
+docker stop CONTAINER_ID
+```
 
 ### Building from source
 
-If you want to build the solution from source, you should follow the steps in [INSTALL.md](). The commands can be used as decribed for the Binary package.
+If you want to build the solution from source, you should follow the steps in [INSTALL.md]().
 
 ## Results
 
-The results of each command are saved in the <code>output</code> folder, which will look like this after executing all the commands:
+The results of each command are saved in the <code>output</code> folder with the following structure:
 
 ```bash
 â”œâ”€â”€ output
 â”‚   â”œâ”€â”€ flowcharts
 â”‚   â”‚   â”œâ”€â”€ *.json
 â”‚   â”œâ”€â”€ footprint_tiles
 â”‚   â”‚   â”œâ”€â”€ *.cpg
@@ -190,15 +243,15 @@
 â”‚   â”‚   â”œâ”€â”€ *.obj.mtl
 â”‚   â”œâ”€â”€ pointcloud_tiles
 â”‚   â”‚   â”œâ”€â”€ *.las
 â”‚   â”œâ”€â”€ processing_areas.gpkg
 â”‚   â””â”€â”€ quadtree.gpkg
 ```
 
-The 3D building models can be viewd using [Ninja](https://github.com/cityjson/ninja), the official web viewer for CityJSON files.
+The 3D building models can be inspected using [Ninja](https://github.com/cityjson/ninja), the official web viewer for CityJSON files.
 
 ![image](https://user-images.githubusercontent.com/72500344/216613188-82d54c75-7e03-4ee7-8c1c-d081e0c1d4ac.png)
 
 ## Related repositories
 
 [Automatic correction of buildings ground floor elevation in 3D City Models](https://github.com/Yarroudh/ZRect3D)
 
@@ -225,7 +278,8 @@
 Yarroudh, A. (2023). Optim3D: Optimized reconstruction of large-scale 3D building models [GitHub repository]. Retrieved from https://github.com/Yarroudh/Optim3D
 
 ## About Optim3D
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
 For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
 
+
```

### Comparing `optim3d-0.1.9/README.md` & `optim3d-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,35 +3,41 @@
 # Optimized reconstruction of large-scale 3D building models
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 
 *Command-Line Interface (CLI) application for efficient and optimized reconstruction of large-scale 3D building models.*
 
-[GeoFlow](https://github.com/geoflow3d/geoflow-bundle) is a software tool that can be used to automatically reconstruct 3D building models from point clouds, with a high level of detail. It is a powerful tool for creating detailed and accurate 3D models of buildings and can be used in a variety of applications. The software is fully automated, making it easy to use and efficient for large-scale projects.
-
-Our program is based on GeoFlow and makes use of it to perform 3D reconstruction of buildings. The process is inspired by the 3D BAG project, which is an up-to-date dataset containing detailed 3D building models of the Netherlands, based on the official BAG data and national AHN point cloud. The optimization of the reconstruction process is achieved by indexing and tiling of the input data which reduces the processing time and resources needed to generate large-scale 3D building models. The indexing and tiling of both, 3D point cloud and 2D footprints, allows for more efficient processing and handling of the 3D reconstruction workflow.
+Optim3D is a powerful tool for optimized automatic reconstruction of highly detailed and large-scale 3D building models. Our tool is based on the [GeoFlow](https://github.com/geoflow3d/geoflow-bundle) software and makes use of it to perform the 3D reconstruction of buildings. The process is inspired by the 3D BAG project and optimized for large-scale projects through indexing and tiling of the input data, which significantly reduces the processing time and resources required to generate large-scale 3D building models.
 
 <img src="https://user-images.githubusercontent.com/72500344/212364590-b7fd444d-ec26-4a8b-bda9-fd4e1669bc6e.png" alt="Workflow of 3D Reconstruction" width="500"/>
 
+## Documentation
+
+If you are using Optim3D, we highly recommend that you take the time to read the [documentation](https://optim3d.readthedocs.io/en/latest/). The documentation is an essential resource that will help you understand the features and functionality of our software, as well as provide guidance on how to use it effectively.
+
 ## Installation
 
 You can install optim3d in your Conda environment by simply running:
 
 ```bash
+conda create --name optimenv python==3.6
+conda activate optimenv
+conda install -c conda-forge pdal python-pdal
+conda install -c conda-forge entwine
 pip install optim3d
 ```
 
-Youc can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
+You can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
 
-**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the License before using it.
+**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the LICENSE file.
 
 ## Usage of the CLI
 
-### Binary package
+### Python package
 
 After installation, you have a small program called <code>optim3d</code>. Use <code>optim3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d [OPTIONS] COMMAND [ARGS]...
 
   CLI tool to manage full optimized reconstruction of large-scale 3D
@@ -44,15 +50,15 @@
   index2d      QuadTree indexing and tiling of 2D building footprints.
   index3d      OcTree indexing of 3D point cloud using Entwine.
   tiler3d      Tiling of point cloud using the calculated processing areas.
   reconstruct  Optimized 3D reconstruction of buildings using GeoFlow.
   post         Post-processing generated CityJSON files.
 ```
 
-The process consists of five distinct steps or <code>commands</code> that must be executed in a specific order to achieve the desired outcome.
+The process consists of five steps or <code>commands</code> that must be executed in a specific order to achieve the desired outcome.
 
 #### Step 1 : 2D building footprints indexing and tiling
 
 Quadtree-based tiling scheme is used for spatial partitioning of building footprints. This assures that the reconstruction time per tile is more or less the same and that the tiles available for download are similar in file size. This is done using the first command <code>index2d</code>. Use <code>optim3d index2d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d index2d [OPTIONS] [FOOTPRINTS]
@@ -70,29 +76,29 @@
   --max INTEGER                   Maximum number of buildings per tile.
                                   [default: 3500]
   --help                          Show this message and exit.
 ```
 
 #### Step 2 : OcTree indexing of the 3D point cloud
 
-Processing large point cloud datasets is hardware-intensive. Therefore, it is necessary to index the 3D point cloud before processing. The index structure makes it possible to stream only the parts of the data that are required, without having to download the entire dataset. In this case, the spatial indexing of the airborne point cloud is performed using an octree structure. This can be easily done using Entwine, an open-source library for organizing and indexing large point cloud datasets using an octree data structure that allows fast and efficient spatial queries. This is done using the second command <code>index3d</code>. Use <code>optim3d index3d --help</code> to see the detailed help:
+Processing large point cloud datasets is hardware-intensive. Therefore, it is necessary to index the 3D point cloud before processing. The index structure makes it possible to stream only the parts of the data that are required, without having to download the entire dataset. In this case, the spatial indexing of the airborne point cloud is performed using an octree structure. This is done using the second command <code>index3d</code>. Use <code>optim3d index3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d index3d [OPTIONS] POINTCLOUD
 
   OcTree indexing of 3D point cloud using Entwine.
 
 Options:
   --output PATH  Output directory.  [default: ./output]
   --help         Show this message and exit.
 ```
 
 #### Step 3 : Tiling of the 3D point cloud
 
-The tiling of the indexed point cloud is based on processing areas calculated when the footprints were indexed. This is achieved using the third command <code>tiler3d</code>. Use <code>optim3d tiler3d --help</code> to see the detailed help:
+The tiling of the indexed point cloud is based on the processing areas already calculated. This is achieved using the third command <code>tiler3d</code>. Use <code>optim3d tiler3d --help</code> to see the detailed help:
 
 ```
 Usage: optim3d tiler3d [OPTIONS]
 
   Tiling of 3D point cloud using the calculated processing areas.
 
 Options:
@@ -102,15 +108,15 @@
                   ./output/indexed_pointcloud]
   --output PATH   Output directory.  [default: ./output]
   --help          Show this message and exit.
 ```
 
 #### Step 4 : 3D reconstruction of building models tile by tile
 
-The 3D reconstruction of building models is performed in this step. The process make use of GeoFlow to generate hight detailed 3D building models tile by tile. This is achieved using the fourth command <code>reconstruct</code>. Use <code>optim3d reconstruct --help</code> to see the detailed help:
+In this step, we perform the 3D reconstruction of building models. The process make use of GeoFlow to generate highly detailed 3D building models tile by tile. This is achieved using the fourth command <code>reconstruct</code>. Use <code>optim3d reconstruct --help</code> to see the detailed help:
 
 ```
 Usage: optim3d reconstruct [OPTIONS]
 
   Optimized 3D reconstruction of buildings using GeoFlow.
 
 Options:
@@ -120,39 +126,86 @@
                      ./output/footprint_tiles]
   --output PATH      Output directory.  [default: ./output]
   --help             Show this message and exit.
 ```
 
 #### Step 5 : Post-processing of CityJSON files
 
-The generated CityJSON files should be processed to add information about tiles to 3D objects. This is done using the fifth command <code>post</code>. Use <code>optim3d post --help</code> to see the detailed help:
+The generated CityJSON files should be post-processed to correct the City Objects IDs. This is done using the fifth command <code>post</code>. Use <code>optim3d post --help</code> to see the detailed help:
 
 ```
 Usage: optim3d post [OPTIONS]
 
   Postprocess the generated CityJSON files.
 
 Options:
   --cityjson PATH  CityJSON files directory.  [default:
                    ./output/model/cityjson]
   --help           Show this message and exit.
 ```
 
 ### Docker Image
 
-Coming soon.
+Optim3D is also available as [Docker image](https://hub.docker.com/r/yarroudh/optim3d). If you are using a Windows operating system, we recommend running the Docker container inside the Windows Subsystem for Linux 2 (WSL2) environment. Please ensure that Geoflow is installed on the WSL2 environment to ensure compatibility with the container.
+
+These are the steps to run Optim3D as a Docker container:
+
+1. First pull the image using the <code>docker pull</code> command:
+
+```bash
+docker pull yarroudh/optim3d
+```
+
+2. To run the Docker container and mount your data inside it, use the <code>docker run</code> command with the <code>-v</code> option to specify the path to the host directory and the path to the container directory where you want to mount the data folder. For example:
+
+```bash
+docker run -d -v ABSOLUTE_PATH_TO_HOST_DATA:/home/user/data yarroudh/optim3d
+```
+
+This command will start a Docker container in detached mode, mount the **ABSOLUTE_PATH_TO_HOST_DATA** directory on the host machine to the **/home/user/data** directory inside the container, and run the <code>yarroudh/optim3d</code> image. Do not change the path of the directory inside the container.
+
+3. Find the container ID and copy it. You can use the <code>docker ps</code> command to list all running containers and their IDs.
+4. Launch a command inside the container using <code>docker exec</code>, use the container ID or name and the command you want to run. For example:
+
+```bash
+docker exec CONTAINER_ID optim3d index2d data/FILE_NAME
+```
+This command will execute the QuadTree indexing of the 2D footprints data, which can be a Shapefile (.shp) or a GeoPackage (.gpkg).
+
+For the <code>reconstruct</code> command, make sure to copy Geoflow-bundle folder to the <code>$PATH</code> environment variable of the container before running the reconstruction:
+
+```bash
+docker cp PATH_TO_GEOFLOW_BUNDLE CONTAINER_ID:$PATH
+docker exec CONTAINER_ID optim3d reconstruct
+```
 
+5. To copy the output of the command from the container to a local path, use the <code>docker cp</code> command with the container ID or name, the path to the file inside the container, and the path to the destination on the host machine. For example:
+
+- To copy the output of one command:
+```bash
+docker cp CONTAINER_ID:/home/user/output/footprint_tiles PATH_ON_HOST_MACHINE
+```
+- Top copy the output of all the commands:
+```bash
+docker cp CONTAINER_ID:/home/user/output PATH_ON_HOST_MACHINE
+```
+
+6. Finally, after executing all the commands and copying the results to your local machine, you can stop the Docker container using the <code>docker stop</code> command followed by the container ID or name:
+
+```bash
+docker stop CONTAINER_ID
+```
 
 ### Building from source
 
-If you want to build the solution from source, you should follow the steps in [INSTALL.md](). The commands can be used as decribed for the Binary package.
+If you want to build the solution from source, you should follow the steps in [INSTALL.md]().
 
 ## Results
 
-The results of each command are saved in the <code>output</code> folder, which will look like this after executing all the commands:
+The results of each command are saved in the <code>output</code> folder with the following structure:
 
 ```bash
 ├── output
 │   ├── flowcharts
 │   │   ├── *.json
 │   ├── footprint_tiles
 │   │   ├── *.cpg
@@ -177,15 +230,15 @@
 │   │   ├── *.obj.mtl
 │   ├── pointcloud_tiles
 │   │   ├── *.las
 │   ├── processing_areas.gpkg
 │   └── quadtree.gpkg
 ```
 
-The 3D building models can be viewd using [Ninja](https://github.com/cityjson/ninja), the official web viewer for CityJSON files.
+The 3D building models can be inspected using [Ninja](https://github.com/cityjson/ninja), the official web viewer for CityJSON files.
 
 ![image](https://user-images.githubusercontent.com/72500344/216613188-82d54c75-7e03-4ee7-8c1c-d081e0c1d4ac.png)
 
 ## Related repositories
 
 [Automatic correction of buildings ground floor elevation in 3D City Models](https://github.com/Yarroudh/ZRect3D)
 
@@ -210,8 +263,8 @@
 ```
 
 Yarroudh, A. (2023). Optim3D: Optimized reconstruction of large-scale 3D building models [GitHub repository]. Retrieved from https://github.com/Yarroudh/Optim3D
 
 ## About Optim3D
 
 This software was developped by [Anass Yarroudh](https://www.linkedin.com/in/anass-yarroudh/), a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).
-For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
+For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
```

### Comparing `optim3d-0.1.9/setup.py` & `optim3d-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="optim3d",
-    version='0.1.9',
+    version='0.2.1',
     description="CLI application for efficient and optimized reconstruction of large-scale 3D building models",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author = 'Anass Yarroudh',
     author_email = 'ayarroudh@uliege.be',
     url = 'https://github.com/Yarroudh/Optim3D',
     packages=find_packages(),
```

