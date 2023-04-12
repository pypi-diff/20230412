# Comparing `tmp/xeye-0.38.tar.gz` & `tmp/xeye-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeye-0.38.tar", last modified: Tue Apr 11 15:32:27 2023, max compression
+gzip compressed data, was "xeye-0.39.tar", last modified: Wed Apr 12 21:32:16 2023, max compression
```

## Comparing `xeye-0.38.tar` & `xeye-0.39.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.281905 xeye-0.38/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.38/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15112 2023-04-11 15:32:27.281387 xeye-0.38/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13357 2023-04-11 13:22:43.000000 xeye-0.38/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-04-11 15:16:08.000000 xeye-0.38/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-11 15:32:27.282001 xeye-0.38/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.274474 xeye-0.38/src/
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.278746 xeye-0.38/src/xeye/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      268 2023-04-11 15:16:12.000000 xeye-0.38/src/xeye/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-0.38/src/xeye/build_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14287 2023-04-11 15:29:52.000000 xeye-0.38/src/xeye/dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-0.38/src/xeye/fast_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-0.38/src/xeye/manual_dataset.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.280760 xeye-0.38/src/xeye.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15112 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      310 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/top_level.txt
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-12 21:32:16.614309 xeye-0.39/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.39/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    16104 2023-04-12 21:32:16.613751 xeye-0.39/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14349 2023-04-12 21:11:08.000000 xeye-0.39/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-04-12 21:30:21.000000 xeye-0.39/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-12 21:32:16.614445 xeye-0.39/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-12 21:32:16.611145 xeye-0.39/xeye/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      268 2023-04-12 21:30:16.000000 xeye-0.39/xeye/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-0.39/xeye/build_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14901 2023-04-11 16:04:14.000000 xeye-0.39/xeye/dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-0.39/xeye/fast_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-0.39/xeye/manual_dataset.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-12 21:32:16.613082 xeye-0.39/xeye.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    16104 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      270 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/top_level.txt
```

### Comparing `xeye-0.38/LICENSE` & `xeye-0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `xeye-0.38/PKG-INFO` & `xeye-0.39/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.38
+Version: 0.39
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,74 +28,109 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  
-- [Installation](#installation)
-- [Create a dataset with full UI](#create-a-dataset-with-full-ui)
-  - [Other useful functions](#other-useful-functions)
-  - [Script example](#script-example)
-- [Create a dataset with fast UI](#create-a-dataset-with-fast-ui)
-- [Create a dataset with manual UI](#create-a-dataset-with-manual-ui)
-  - [How to take pictures manually](#how-to-take-pictures-manually)
-- [Build datasets from different .npz files](#build-datasets-from-different-npz-files)
-  - [Script example](#script-example-1)
-- [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
+# Xeye
+[![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
+
+- [Xeye](#xeye)
+  - [Installation](#installation)
+  - [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
+  - [Xeye functionalities](#xeye-functionalities)
+  - [Create a dataset with full terminal UI (Dataset)](#create-a-dataset-with-full-terminal-ui-dataset)
+    - [Other useful methods](#other-useful-methods)
+    - [Script example](#script-example)
+  - [Create a dataset with fast UI (FastDataset)](#create-a-dataset-with-fast-ui-fastdataset)
+  - [Create a dataset with manual UI (ManualDataset)](#create-a-dataset-with-manual-ui-manualdataset)
+    - [How to take pictures manually](#how-to-take-pictures-manually)
+  - [Build datasets from different npz files (BuildDataset)](#build-datasets-from-different-npz-files-builddataset)
+    - [Script example](#script-example-1)
   
 
+
 Xeye is a package for data collection to build computer vision applications based on inferential results of deep learning models. The main reasons to use Xeye are:
 
 * Create a dataset using only a laptop and its integrated camera (or alternatively an external USB camera);
 * Create a dataset already structured like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist);
 * Create a dataset that can be used for building models with [Tensorflow](https://www.tensorflow.org/) or [Pytorch](https://pytorch.org/).
 
+<hr>
 
 
 <div id='installation'/>
 
 ## Installation
 
 To install the package, 
 
 ```
 pip install xeye
 ```
 
+<hr>
+
+<div id='xeye-datasets-for-deep-learning'/>
+
+## Xeye datasets for deep learning 
+
+In the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository, you can find examples of deep learning model implementations based on datasets produced by the Xeye package (made with [Tensorflow](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/tensorflow) or [Pytorch](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/pytorch) frameworks).
+
+
+* [Binary dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing two types of grayscale images (with labels: 0=keyboard, 1=mouse).
+* [MultiLabel dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing three types of rgb images (three types of security cameras with labels: 0=dome, 1=bullet, 2=cube)
+
+Additionally, the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository contains examples of scripts that use the Xeye package to build datasets ([examples link](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/xeye-example)).
+
 <div id='create-a-dataset-with-full-ui'/>
 
-## Create a dataset with full UI 
+<hr>
+
+## Xeye functionalities
+
+The Xeye package includes three major approaches (classes) for creating a dataset from scratch: Dataset, FastDataset, and ManualDataset.
+
+* **Dataset**: Uses the full UI terminal interface.
+* **FastDataset**: Uses the constructor with all the specifications of the dataset.
+* **ManualDataset**: Same as FastDataset, but every image is shot manually one at a time.
+  
+Additionally, the package provides a method for combining datasets created with the **BuildDataset** class.
+
+<hr>
+
+## Create a dataset with full terminal UI (Dataset)
 
 First of all, load the module datapipe from the package:
 
 ```python
 import xeye
 ```
 
 then initialize the instance like this 
 
 ```python
 data = xeye.Dataset()
 ```
-set the parameters related to the images with the **init** function
+set the parameters related to the images with the **setup** method
 
 ```python
 data.setup()
-
 ```
-the execution of this function causes the starting of the user interface in the **terminal** 
+
+the execution of this method causes the starting of the user interface in the **terminal** 
 
 
 ```console
 --- CAMERA SETTING ---
 Select the index of the camera that you want to use for creating the dataset: 1
 ``` 
 
-the **init** function arises multiple questions that set the parameters' values
+the **setup** method arises multiple questions that set the parameters' values
 
 
 ```console
 --- IMAGE SETTINGS ---
 Num. of types of images to scan: 2
 Name of image type (1): keyboard
 Name of image type (2): mouse
@@ -103,262 +138,250 @@
 Single frame HEIGHT: 720
 Single frame WIDTH:  720
 num. of waiting time (in sec.) between every frame: 0
 ``` 
 
 Precisely the questions refer to:
 
-* **Select the index of the camera that you want to use for creating the dataset**: generally 0 for integrated camera, 1 for USB external camera.
-* **Num. of types of images to scan**: answer 2 if you want to create a dataset with two objects (e.g. keyboard and mouse). In general, answer with the number of object types to include in your dataset.
-* **Name of image type**: insert the name of every specific object you want to include in the dataset. The **init** function creates a named folder for every image type. 
-* **Num. of frames to shoot for every image type**: select the number of images you want to shoot and save them in every object folder. 
-* **Single frame HEIGHT**: frame height values.
-* **Single frame WIDTH**: frame width values.
+* **Select the index of the camera that you want to use for creating the dataset**: Generally 0 for integrated camera, 1 for USB external camera.
+* **Num. of types of images to scan**: Answer 2 if you want to create a dataset with two objects (e.g. keyboard and mouse). In general, answer with the number of object types to include in your dataset.
+* **Name of image type**: Insert the name of every specific object you want to include in the dataset. The **setup** method creates a named folder for every image type. 
+* **Num. of frames to shoot for every image type**: Select the number of images you want to shoot and save them in every object folder. 
+* **Single frame HEIGHT**: Frame height values.
+* **Single frame WIDTH**: Frame width values.
 * **Num. of waiting time (in sec.) between every frame**: e.g 0.2 causes a waiting time of 0.2 seconds between every shoot.
 
-After the parameters setting, you can invoke the function to start shooting images. Datapipe module provides two different formats of images:
+After the parameters setting, you can invoke the method to start shooting images. Datapipe module provides two different formats of images:
 
-* Grayscale image with the **gray** function;
-* Color image with the **rgb** function.
+* Grayscale image with the **gray** method;
+* Color image with the **rgb** method.
   
-Let's produce a dataset based on RGB images with the **rgb** function:
+Let's produce a dataset based on RGB images with the **rgb** method:
 
 ```python
 data.rgb()
 ```
-In the terminal keypress [b], to make photos for the image types passed to the **init** function.
+In the terminal keypress [b], to make photos for the image types passed to the **setup** method.
 
 ```console
 --- START TAKING PHOTOS ---
 Press [b] on the keyboard to start data collection of image type [keyboard]
 b
 Press [b] on the keyboard to start data collection of image type [mouse]
 b
 ``` 
 
-On the directory of the script, you can find the folders that contain the images produced by the **rbg** function (e.g. keyboard folder and mouse folder). 
+On the directory of the script, you can find the folders that contain the images produced by the **rbg** method (e.g. keyboard folder and mouse folder). 
 
 
 
-Images collected in the folders can be used for building datasets like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist). The first approach to achieve this result is calling the **compress_train_test** function:
+Images collected in the folders can be used for building datasets like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist). The first approach to achieve this result is calling the **compress_train_test** method:
 
 ```python
 data.compress_train_test()
 ```
 
 That produces the following output in the terminal window 
 
 ```console
 --- DATASET SETTING ---
 percentage of images in the test set: 0.2
 ``` 
 
-In which you can select the portion of images to use in the train and test datasets (write a value between (0,1)). By doing so, the function produces a **.npz** file formed by these specific tensors:
+In which you can select the portion of images to use in the train and test datasets (write a value between (0,1)). By doing so, the method produces a **.npz** file formed by these specific tensors:
 
 * Train set:
-  * **X_train**: matrices/tensors of every single image in the train dataset;
-  * **y_train**: classes (ordinal values) are associated with every image in the train dataset.
+  * **X_train**: Matrices/tensors of every single image in the train dataset;
+  * **y_train**: Classes (ordinal values) are associated with every image in the train dataset.
 * Test set:
-  * **X_test**: matrices/tensors of every single image in the test dataset;
-  * **y_test**: classes (ordinal values) are associated with every image in the test dataset.
+  * **X_test**: Matrices/tensors of every single image in the test dataset;
+  * **y_test**: Classes (ordinal values) are associated with every image in the test dataset.
   
 (matrices for grayscale images: [Height $\times$ Width $\times$ 1], tensors for RGB images:[Height $\times$ Width $\times$ 3]).
 
-An alternative approach is represented by the use of the function **compress_all**
+An alternative approach is represented by the use of the **compress_all** method
 
 ```python
 data.compress_all()
 ```
 
 In this case, the images are united in a unique tensor that contains all the frames produced previously. 
 
 * Unique tensor:
-  * **X**: matricies/tensors of every single image produced;
-  * **y**: classes (ordinal values) are associated with every image produced.
+  * **X**: Matricies/tensors of every single image produced;
+  * **y**: Classes (ordinal values) are associated with every image produced.
 
-Finally, you can use the **just_compress** function to create a unique tensor with all the images produced.
+Finally, you can use the **just_compress** method to create a unique tensor with all the images produced.
 
 ```python
 data.just_compress()
 ```
 In the terminal, you have to insert the dataset’s name
 
 ```console
 --- DATASET SETTING ---
 Select a name for the compressed file: batch_test
 ``` 
-If you pass 0, by default the dataset will be save with the name **dataset_raw.npz**. The dataset produced by this function can be used by the class **BuildDataset** to put together more .npz files and create a dataset like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist).
+If you pass 0, by default the dataset will be save with the name **dataset_raw.npz**. The dataset produced by this method can be used by the class **BuildDataset** to put together more .npz files and create a dataset like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist).
 
-<div id='other-useful-functions'/>
+<div id='other-useful-methods'/>
 
-### Other useful functions
+### Other useful methods
 
-* **preview**: open the camera stream to check the framing. 
-  ![](img/1.png)
-* **var_control**: print the values of the parameters set with the **init** function. 
+* **preview**: Open the camera stream to check the framing. 
+* **var_control**: Print the values of the parameters set with the **setup** method. 
+  
 ```console
 --- PARAMETERS CONTROL ---
 camera index: 1
 num. of images types: 2
 labels of images types: ['keyboard', 'mouse']
 num. of images for types: 20
 Single frame HEIGHT: 720
 Single frame WIDTH:  720
 waiting time between frames: 0.0
 percentage of images in train dataset: 0.2
-statusGray: 1
-statusRGB: 0
 ``` 
 
 <div id='script-example-1'/>
 
 ### Script example 
 
 Example of a script to use the **Dataset** class:
 
 ```python
 import xeye
 data = xeye.dataset()
-data.init()
+data.setup()
 data.preview()
 data.rgb()
 data.compress_train_test()
 data.compress_all()
 data.just_compress()
-
 ```
+
+<hr>
+
 <div id='create-a-dataset-with-fast-ui'/>
 
-## Create a dataset with fast UI 
-A faster way to use the datapipe module is represented by the **FastDataset** class. In this case, there isn't a complete terminal UI that guides you in the construction of the dataset. With **FastDataset**, you only pass the parameters to the class, and then call the functions you need. 
+## Create a dataset with fast UI (FastDataset)
+
+The **FastDataset** class provides a faster way to use the datapipe module. Unlike the **Dataset** class, it does not have a complete terminal UI to guide you through the dataset construction process. Instead, you simply pass the parameters to the class and call the necessary methods.
 
 ```python
 import xeye
-
 # define parameters values
 index = 0
 img_types = 2
 label = ['keyboard', 'mouse']
 num = 20
 height = 100
 width = 100
 standby_time = 0
 # percentage of images in the test set 
 perc = 0.2
-
 data = xeye.FastDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width, stand_by_time = standby_time)
 data.preview()
 data.rgb()
 data.compress_train_test(perc = perc)
 data.compress_all()
 data.just_compress("batch_test")
 ```
 
 The parameters passed to the class **FastDataset**:
 
-* **index**: generally 0 for integrated camera, 1 for USB external camera.
-* **img_types**: numbers of object types that you want to include in your dataset.
-* **label**: list of object names to include in the dataset. The **init** function creates a named folder for every image type.
-* **num**: select the number of images you want to shoot and save them in every object folder.
-* **height**: frame height values.
-* **width**: frame width values.
+* **index**: Generally 0 for integrated camera, 1 for USB external camera.
+* **img_types**: Numbers of object types that you want to include in your dataset.
+* **label**: List of object names to include in the dataset. The **setup** method creates a named folder for every image type.
+* **num**: Select the number of images you want to shoot and save them in every object folder.
+* **height**: Frame height values.
+* **width**: Frame width values.
 * **standby_time**: e.g 0.2 cause a waiting time of 0.2 seconds between every shoot.
   
-For split images in the train and test dataset, pass a value between (0,1) to the perc parameter of the **compress_train_test** function
+For split images in the train and test dataset, pass a value between (0,1) to the perc parameter of the **compress_train_test** method
 
 * **perc**: the portion of images to use in the test dataset, write a value between (0,1).
 
-If you don't pass any value to the **just_compress** function, the dataset will be saved with the name **dataset_raw.npz**.
-
+If you don't pass any value to the **just_compress** method, the dataset will be saved with the name **dataset_raw.npz**.
 
+<hr>
 
 <div id='create-a-dataset-with-manual-ui'/>
 
-## Create a dataset with manual UI 
+## Create a dataset with manual UI (ManualDataset)
+
 The **ManualDataset** class is how you can build a dataset by taking pictures manually. 
 
 ```python
 import xeye
-
 # define parameters values
 index = 0
 img_types = 2
 label = ['keyboard', 'mouse']
 num = 20
 height = 100
 width = 100
 standby_time = 0
 # percentage of images in the test set 
 perc = 0.2
-
 data = xeye.ManualDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width)
 data.preview()
 data.rgb()
 data.compress_train_test(perc = perc)
 data.compress_all()
 data.just_compress("batch_test")
 ```
 
 As you can see in the code snippet, the **ManualDataset** class works like the **FastDataset** class. The only difference is the absence of the **standby_time option**, which is no more necessary in this case. 
 
 The parameters passed to the class **ManualDataset**:
 
-* **index**: generally 0 for integrated camera, 1 for USB external camera.
-* **img_types**: numbers of object types that you want to include in your dataset.
-* **label**: list of object names to include in the dataset. The **init** function creates a named folder for every image type.
-* **num**: select the number of images you want to shoot and save them in every object folder.
-* **height**: frame height values.
-* **width**: frame width values.
+* **index**: Generally 0 for integrated camera, 1 for USB external camera.
+* **img_types**: Numbers of object types that you want to include in your dataset.
+* **label**: List of object names to include in the dataset. The constructor creates a named folder for every image type.
+* **num**: Select the number of images you want to shoot and save them in every object folder.
+* **height**: Frame height values.
+* **width**: Frame width values.
 
-### How to take pictures manually
 
-On the image window title, after the image type caption it's reported how to take pictures manually with the **ManualDataset**
+### How to take pictures manually
 
-* Press [s] on the keyboard to save the image nr: 1
+In the title bar of the image window, after the caption identifying the image type, there are instructions for manually taking pictures using the ManualDataset. These instructions will be displayed as follows:
 
-![](img/manual.png)
+* Camera view for image type <name-of-image-type>. Press [s] on the keyboard to save image number: <nr-of-image>.
+ 
 
-Press [s] until you reach the number of frames passed to the **num** parameter of the class. 
+<hr>
 
-## Build datasets from different .npz files 
+## Build datasets from different npz files (BuildDataset)
 
-If you want to build datasets made by different types of images, but for example, you can't shoot one of the image types that compose the dataset (because you have to wait a significant amount of time or change location), you can use the **BuildDataset** class. 
+If you want to create a dataset that includes different types of images, but cannot shoot all image types at once (e.g., due to time constraints or location differences), you can use the **BuildDataset** class.
 
-* Create datasets with the **just_compress** function;
+* Create datasets with the **just_compress** method;
 * Create different .npz files for every type of images that composes the dataset (use the same colour spaces in all datasets, RGB or grayscale);
 * Create a new script and call the **BuildDataset** class that merges all the .npz files created before.
 
 <div id='script-example-2'/>
 
 ### Script example 
 
 ```python
 import xeye
 # list of directory (paths for the .npz files)
-path = ['/Users/marcosalvalaggio/code/testxeye/dataset/batch_2.npz', '/Users/marcosalvalaggio/code/testxeye/dataset/batch_3.npz']
+path = ['batch_2.npz', 'batch_3.npz']
 # list of labels associated with the images inside the .npz files
 label = [0,1]
-# initializes the class
 data = xeye.BuildDataset(path=path, label=label, size = None, color=True, split=True, perc=0.2)
 data.build()
 ```
 The parameters passed to the class **BuildDataset**:
 
-* **path**: list of files (.npz) path you want to include in the new dataset
-* **label**: list of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
-* **size**: tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
-* **color**: defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
-* **split**: defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
-* **perc**: defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
+* **path**: List of files (.npz) path you want to include in the new dataset
+* **label**: List of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
+* **size**: Tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
+* **color**: Defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
+* **split**: Defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
+* **perc**: Defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
 
 When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
 
 
-<div id='xeye-datasets-for-deep-learning'/>
-
-## Xeye datasets for deep learning 
-
-In the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository, you can find examples of deep learning model implementations based on datasets produced by the Xeye package (made with [Tensorflow](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/tensorflow) or [Pytorch](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/pytorch) frameworks).
-
-
-* [Binary dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing two types of grayscale images (with labels: 0=keyboard, 1=mouse).
-* [MultiLabel dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing three types of rgb images (three types of security cameras with labels: 0=dome, 1=bullet, 2=cube)
```

### Comparing `xeye-0.38/README.md` & `xeye-0.39/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,103 @@
  
-- [Installation](#installation)
-- [Create a dataset with full UI](#create-a-dataset-with-full-ui)
-  - [Other useful functions](#other-useful-functions)
-  - [Script example](#script-example)
-- [Create a dataset with fast UI](#create-a-dataset-with-fast-ui)
-- [Create a dataset with manual UI](#create-a-dataset-with-manual-ui)
-  - [How to take pictures manually](#how-to-take-pictures-manually)
-- [Build datasets from different .npz files](#build-datasets-from-different-npz-files)
-  - [Script example](#script-example-1)
-- [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
+# Xeye
+[![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
+
+- [Xeye](#xeye)
+  - [Installation](#installation)
+  - [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
+  - [Xeye functionalities](#xeye-functionalities)
+  - [Create a dataset with full terminal UI (Dataset)](#create-a-dataset-with-full-terminal-ui-dataset)
+    - [Other useful methods](#other-useful-methods)
+    - [Script example](#script-example)
+  - [Create a dataset with fast UI (FastDataset)](#create-a-dataset-with-fast-ui-fastdataset)
+  - [Create a dataset with manual UI (ManualDataset)](#create-a-dataset-with-manual-ui-manualdataset)
+    - [How to take pictures manually](#how-to-take-pictures-manually)
+  - [Build datasets from different npz files (BuildDataset)](#build-datasets-from-different-npz-files-builddataset)
+    - [Script example](#script-example-1)
   
 
+
 Xeye is a package for data collection to build computer vision applications based on inferential results of deep learning models. The main reasons to use Xeye are:
 
 * Create a dataset using only a laptop and its integrated camera (or alternatively an external USB camera);
 * Create a dataset already structured like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist);
 * Create a dataset that can be used for building models with [Tensorflow](https://www.tensorflow.org/) or [Pytorch](https://pytorch.org/).
 
+<hr>
 
 
 <div id='installation'/>
 
 ## Installation
 
 To install the package, 
 
 ```
 pip install xeye
 ```
 
+<hr>
+
+<div id='xeye-datasets-for-deep-learning'/>
+
+## Xeye datasets for deep learning 
+
+In the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository, you can find examples of deep learning model implementations based on datasets produced by the Xeye package (made with [Tensorflow](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/tensorflow) or [Pytorch](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/pytorch) frameworks).
+
+
+* [Binary dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing two types of grayscale images (with labels: 0=keyboard, 1=mouse).
+* [MultiLabel dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing three types of rgb images (three types of security cameras with labels: 0=dome, 1=bullet, 2=cube)
+
+Additionally, the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository contains examples of scripts that use the Xeye package to build datasets ([examples link](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/xeye-example)).
+
 <div id='create-a-dataset-with-full-ui'/>
 
-## Create a dataset with full UI 
+<hr>
+
+## Xeye functionalities
+
+The Xeye package includes three major approaches (classes) for creating a dataset from scratch: Dataset, FastDataset, and ManualDataset.
+
+* **Dataset**: Uses the full UI terminal interface.
+* **FastDataset**: Uses the constructor with all the specifications of the dataset.
+* **ManualDataset**: Same as FastDataset, but every image is shot manually one at a time.
+  
+Additionally, the package provides a method for combining datasets created with the **BuildDataset** class.
+
+<hr>
+
+## Create a dataset with full terminal UI (Dataset)
 
 First of all, load the module datapipe from the package:
 
 ```python
 import xeye
 ```
 
 then initialize the instance like this 
 
 ```python
 data = xeye.Dataset()
 ```
-set the parameters related to the images with the **init** function
+set the parameters related to the images with the **setup** method
 
 ```python
 data.setup()
-
 ```
-the execution of this function causes the starting of the user interface in the **terminal** 
+
+the execution of this method causes the starting of the user interface in the **terminal** 
 
 
 ```console
 --- CAMERA SETTING ---
 Select the index of the camera that you want to use for creating the dataset: 1
 ``` 
 
-the **init** function arises multiple questions that set the parameters' values
+the **setup** method arises multiple questions that set the parameters' values
 
 
 ```console
 --- IMAGE SETTINGS ---
 Num. of types of images to scan: 2
 Name of image type (1): keyboard
 Name of image type (2): mouse
@@ -70,262 +105,250 @@
 Single frame HEIGHT: 720
 Single frame WIDTH:  720
 num. of waiting time (in sec.) between every frame: 0
 ``` 
 
 Precisely the questions refer to:
 
-* **Select the index of the camera that you want to use for creating the dataset**: generally 0 for integrated camera, 1 for USB external camera.
-* **Num. of types of images to scan**: answer 2 if you want to create a dataset with two objects (e.g. keyboard and mouse). In general, answer with the number of object types to include in your dataset.
-* **Name of image type**: insert the name of every specific object you want to include in the dataset. The **init** function creates a named folder for every image type. 
-* **Num. of frames to shoot for every image type**: select the number of images you want to shoot and save them in every object folder. 
-* **Single frame HEIGHT**: frame height values.
-* **Single frame WIDTH**: frame width values.
+* **Select the index of the camera that you want to use for creating the dataset**: Generally 0 for integrated camera, 1 for USB external camera.
+* **Num. of types of images to scan**: Answer 2 if you want to create a dataset with two objects (e.g. keyboard and mouse). In general, answer with the number of object types to include in your dataset.
+* **Name of image type**: Insert the name of every specific object you want to include in the dataset. The **setup** method creates a named folder for every image type. 
+* **Num. of frames to shoot for every image type**: Select the number of images you want to shoot and save them in every object folder. 
+* **Single frame HEIGHT**: Frame height values.
+* **Single frame WIDTH**: Frame width values.
 * **Num. of waiting time (in sec.) between every frame**: e.g 0.2 causes a waiting time of 0.2 seconds between every shoot.
 
-After the parameters setting, you can invoke the function to start shooting images. Datapipe module provides two different formats of images:
+After the parameters setting, you can invoke the method to start shooting images. Datapipe module provides two different formats of images:
 
-* Grayscale image with the **gray** function;
-* Color image with the **rgb** function.
+* Grayscale image with the **gray** method;
+* Color image with the **rgb** method.
   
-Let's produce a dataset based on RGB images with the **rgb** function:
+Let's produce a dataset based on RGB images with the **rgb** method:
 
 ```python
 data.rgb()
 ```
-In the terminal keypress [b], to make photos for the image types passed to the **init** function.
+In the terminal keypress [b], to make photos for the image types passed to the **setup** method.
 
 ```console
 --- START TAKING PHOTOS ---
 Press [b] on the keyboard to start data collection of image type [keyboard]
 b
 Press [b] on the keyboard to start data collection of image type [mouse]
 b
 ``` 
 
-On the directory of the script, you can find the folders that contain the images produced by the **rbg** function (e.g. keyboard folder and mouse folder). 
+On the directory of the script, you can find the folders that contain the images produced by the **rbg** method (e.g. keyboard folder and mouse folder). 
 
 
 
-Images collected in the folders can be used for building datasets like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist). The first approach to achieve this result is calling the **compress_train_test** function:
+Images collected in the folders can be used for building datasets like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist). The first approach to achieve this result is calling the **compress_train_test** method:
 
 ```python
 data.compress_train_test()
 ```
 
 That produces the following output in the terminal window 
 
 ```console
 --- DATASET SETTING ---
 percentage of images in the test set: 0.2
 ``` 
 
-In which you can select the portion of images to use in the train and test datasets (write a value between (0,1)). By doing so, the function produces a **.npz** file formed by these specific tensors:
+In which you can select the portion of images to use in the train and test datasets (write a value between (0,1)). By doing so, the method produces a **.npz** file formed by these specific tensors:
 
 * Train set:
-  * **X_train**: matrices/tensors of every single image in the train dataset;
-  * **y_train**: classes (ordinal values) are associated with every image in the train dataset.
+  * **X_train**: Matrices/tensors of every single image in the train dataset;
+  * **y_train**: Classes (ordinal values) are associated with every image in the train dataset.
 * Test set:
-  * **X_test**: matrices/tensors of every single image in the test dataset;
-  * **y_test**: classes (ordinal values) are associated with every image in the test dataset.
+  * **X_test**: Matrices/tensors of every single image in the test dataset;
+  * **y_test**: Classes (ordinal values) are associated with every image in the test dataset.
   
 (matrices for grayscale images: [Height $\times$ Width $\times$ 1], tensors for RGB images:[Height $\times$ Width $\times$ 3]).
 
-An alternative approach is represented by the use of the function **compress_all**
+An alternative approach is represented by the use of the **compress_all** method
 
 ```python
 data.compress_all()
 ```
 
 In this case, the images are united in a unique tensor that contains all the frames produced previously. 
 
 * Unique tensor:
-  * **X**: matricies/tensors of every single image produced;
-  * **y**: classes (ordinal values) are associated with every image produced.
+  * **X**: Matricies/tensors of every single image produced;
+  * **y**: Classes (ordinal values) are associated with every image produced.
 
-Finally, you can use the **just_compress** function to create a unique tensor with all the images produced.
+Finally, you can use the **just_compress** method to create a unique tensor with all the images produced.
 
 ```python
 data.just_compress()
 ```
 In the terminal, you have to insert the dataset’s name
 
 ```console
 --- DATASET SETTING ---
 Select a name for the compressed file: batch_test
 ``` 
-If you pass 0, by default the dataset will be save with the name **dataset_raw.npz**. The dataset produced by this function can be used by the class **BuildDataset** to put together more .npz files and create a dataset like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist).
+If you pass 0, by default the dataset will be save with the name **dataset_raw.npz**. The dataset produced by this method can be used by the class **BuildDataset** to put together more .npz files and create a dataset like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist).
 
-<div id='other-useful-functions'/>
+<div id='other-useful-methods'/>
 
-### Other useful functions
+### Other useful methods
 
-* **preview**: open the camera stream to check the framing. 
-  ![](img/1.png)
-* **var_control**: print the values of the parameters set with the **init** function. 
+* **preview**: Open the camera stream to check the framing. 
+* **var_control**: Print the values of the parameters set with the **setup** method. 
+  
 ```console
 --- PARAMETERS CONTROL ---
 camera index: 1
 num. of images types: 2
 labels of images types: ['keyboard', 'mouse']
 num. of images for types: 20
 Single frame HEIGHT: 720
 Single frame WIDTH:  720
 waiting time between frames: 0.0
 percentage of images in train dataset: 0.2
-statusGray: 1
-statusRGB: 0
 ``` 
 
 <div id='script-example-1'/>
 
 ### Script example 
 
 Example of a script to use the **Dataset** class:
 
 ```python
 import xeye
 data = xeye.dataset()
-data.init()
+data.setup()
 data.preview()
 data.rgb()
 data.compress_train_test()
 data.compress_all()
 data.just_compress()
-
 ```
+
+<hr>
+
 <div id='create-a-dataset-with-fast-ui'/>
 
-## Create a dataset with fast UI 
-A faster way to use the datapipe module is represented by the **FastDataset** class. In this case, there isn't a complete terminal UI that guides you in the construction of the dataset. With **FastDataset**, you only pass the parameters to the class, and then call the functions you need. 
+## Create a dataset with fast UI (FastDataset)
+
+The **FastDataset** class provides a faster way to use the datapipe module. Unlike the **Dataset** class, it does not have a complete terminal UI to guide you through the dataset construction process. Instead, you simply pass the parameters to the class and call the necessary methods.
 
 ```python
 import xeye
-
 # define parameters values
 index = 0
 img_types = 2
 label = ['keyboard', 'mouse']
 num = 20
 height = 100
 width = 100
 standby_time = 0
 # percentage of images in the test set 
 perc = 0.2
-
 data = xeye.FastDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width, stand_by_time = standby_time)
 data.preview()
 data.rgb()
 data.compress_train_test(perc = perc)
 data.compress_all()
 data.just_compress("batch_test")
 ```
 
 The parameters passed to the class **FastDataset**:
 
-* **index**: generally 0 for integrated camera, 1 for USB external camera.
-* **img_types**: numbers of object types that you want to include in your dataset.
-* **label**: list of object names to include in the dataset. The **init** function creates a named folder for every image type.
-* **num**: select the number of images you want to shoot and save them in every object folder.
-* **height**: frame height values.
-* **width**: frame width values.
+* **index**: Generally 0 for integrated camera, 1 for USB external camera.
+* **img_types**: Numbers of object types that you want to include in your dataset.
+* **label**: List of object names to include in the dataset. The **setup** method creates a named folder for every image type.
+* **num**: Select the number of images you want to shoot and save them in every object folder.
+* **height**: Frame height values.
+* **width**: Frame width values.
 * **standby_time**: e.g 0.2 cause a waiting time of 0.2 seconds between every shoot.
   
-For split images in the train and test dataset, pass a value between (0,1) to the perc parameter of the **compress_train_test** function
+For split images in the train and test dataset, pass a value between (0,1) to the perc parameter of the **compress_train_test** method
 
 * **perc**: the portion of images to use in the test dataset, write a value between (0,1).
 
-If you don't pass any value to the **just_compress** function, the dataset will be saved with the name **dataset_raw.npz**.
-
+If you don't pass any value to the **just_compress** method, the dataset will be saved with the name **dataset_raw.npz**.
 
+<hr>
 
 <div id='create-a-dataset-with-manual-ui'/>
 
-## Create a dataset with manual UI 
+## Create a dataset with manual UI (ManualDataset)
+
 The **ManualDataset** class is how you can build a dataset by taking pictures manually. 
 
 ```python
 import xeye
-
 # define parameters values
 index = 0
 img_types = 2
 label = ['keyboard', 'mouse']
 num = 20
 height = 100
 width = 100
 standby_time = 0
 # percentage of images in the test set 
 perc = 0.2
-
 data = xeye.ManualDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width)
 data.preview()
 data.rgb()
 data.compress_train_test(perc = perc)
 data.compress_all()
 data.just_compress("batch_test")
 ```
 
 As you can see in the code snippet, the **ManualDataset** class works like the **FastDataset** class. The only difference is the absence of the **standby_time option**, which is no more necessary in this case. 
 
 The parameters passed to the class **ManualDataset**:
 
-* **index**: generally 0 for integrated camera, 1 for USB external camera.
-* **img_types**: numbers of object types that you want to include in your dataset.
-* **label**: list of object names to include in the dataset. The **init** function creates a named folder for every image type.
-* **num**: select the number of images you want to shoot and save them in every object folder.
-* **height**: frame height values.
-* **width**: frame width values.
+* **index**: Generally 0 for integrated camera, 1 for USB external camera.
+* **img_types**: Numbers of object types that you want to include in your dataset.
+* **label**: List of object names to include in the dataset. The constructor creates a named folder for every image type.
+* **num**: Select the number of images you want to shoot and save them in every object folder.
+* **height**: Frame height values.
+* **width**: Frame width values.
 
-### How to take pictures manually
 
-On the image window title, after the image type caption it's reported how to take pictures manually with the **ManualDataset**
+### How to take pictures manually
 
-* Press [s] on the keyboard to save the image nr: 1
+In the title bar of the image window, after the caption identifying the image type, there are instructions for manually taking pictures using the ManualDataset. These instructions will be displayed as follows:
 
-![](img/manual.png)
+* Camera view for image type <name-of-image-type>. Press [s] on the keyboard to save image number: <nr-of-image>.
+ 
 
-Press [s] until you reach the number of frames passed to the **num** parameter of the class. 
+<hr>
 
-## Build datasets from different .npz files 
+## Build datasets from different npz files (BuildDataset)
 
-If you want to build datasets made by different types of images, but for example, you can't shoot one of the image types that compose the dataset (because you have to wait a significant amount of time or change location), you can use the **BuildDataset** class. 
+If you want to create a dataset that includes different types of images, but cannot shoot all image types at once (e.g., due to time constraints or location differences), you can use the **BuildDataset** class.
 
-* Create datasets with the **just_compress** function;
+* Create datasets with the **just_compress** method;
 * Create different .npz files for every type of images that composes the dataset (use the same colour spaces in all datasets, RGB or grayscale);
 * Create a new script and call the **BuildDataset** class that merges all the .npz files created before.
 
 <div id='script-example-2'/>
 
 ### Script example 
 
 ```python
 import xeye
 # list of directory (paths for the .npz files)
-path = ['/Users/marcosalvalaggio/code/testxeye/dataset/batch_2.npz', '/Users/marcosalvalaggio/code/testxeye/dataset/batch_3.npz']
+path = ['batch_2.npz', 'batch_3.npz']
 # list of labels associated with the images inside the .npz files
 label = [0,1]
-# initializes the class
 data = xeye.BuildDataset(path=path, label=label, size = None, color=True, split=True, perc=0.2)
 data.build()
 ```
 The parameters passed to the class **BuildDataset**:
 
-* **path**: list of files (.npz) path you want to include in the new dataset
-* **label**: list of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
-* **size**: tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
-* **color**: defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
-* **split**: defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
-* **perc**: defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
+* **path**: List of files (.npz) path you want to include in the new dataset
+* **label**: List of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
+* **size**: Tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
+* **color**: Defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
+* **split**: Defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
+* **perc**: Defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
 
 When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
 
 
-<div id='xeye-datasets-for-deep-learning'/>
-
-## Xeye datasets for deep learning 
-
-In the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository, you can find examples of deep learning model implementations based on datasets produced by the Xeye package (made with [Tensorflow](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/tensorflow) or [Pytorch](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/pytorch) frameworks).
-
-
-* [Binary dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing two types of grayscale images (with labels: 0=keyboard, 1=mouse).
-* [MultiLabel dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing three types of rgb images (three types of security cameras with labels: 0=dome, 1=bullet, 2=cube)
```

### Comparing `xeye-0.38/pyproject.toml` & `xeye-0.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xeye"
-version = "0.38"
+version = "0.39"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Create datasets for computer vision applications"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `xeye-0.38/src/xeye/build_dataset.py` & `xeye-0.39/xeye/build_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.38/src/xeye/dataset.py` & `xeye-0.39/xeye/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 import time
 
 
 class Dataset:
     """
     A class for collecting a dataset of images using OpenCV.
 
+    Attributes:
+        index (int): The index of the camera to be used for creating the dataset.
+        label (list): The list of names of the different types of images to be collected.
+        num (int): The number of frames to shoot for every image type.
+        height (int): The height of the individual frames.
+        width (int): The width of the individual frames.
+        standby_time (float): The number of seconds to wait between every frame.
+        perc (int): The percentage of data to use for training (the remaining will be used for validation).
+        name (str): The name of the dataset.
+    
     Examples:
         >>> import xeye
         >>> data = xeye.Dataset()
         >>> data.setup()
         >>> data.var_control()
         >>> data.preview()
         >>> data.rgb() # or data.gray()
```

### Comparing `xeye-0.38/src/xeye/fast_dataset.py` & `xeye-0.39/xeye/fast_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.38/src/xeye/manual_dataset.py` & `xeye-0.39/xeye/manual_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.38/src/xeye.egg-info/PKG-INFO` & `xeye-0.39/xeye.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.38
+Version: 0.39
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,74 +28,109 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  
-- [Installation](#installation)
-- [Create a dataset with full UI](#create-a-dataset-with-full-ui)
-  - [Other useful functions](#other-useful-functions)
-  - [Script example](#script-example)
-- [Create a dataset with fast UI](#create-a-dataset-with-fast-ui)
-- [Create a dataset with manual UI](#create-a-dataset-with-manual-ui)
-  - [How to take pictures manually](#how-to-take-pictures-manually)
-- [Build datasets from different .npz files](#build-datasets-from-different-npz-files)
-  - [Script example](#script-example-1)
-- [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
+# Xeye
+[![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
+
+- [Xeye](#xeye)
+  - [Installation](#installation)
+  - [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
+  - [Xeye functionalities](#xeye-functionalities)
+  - [Create a dataset with full terminal UI (Dataset)](#create-a-dataset-with-full-terminal-ui-dataset)
+    - [Other useful methods](#other-useful-methods)
+    - [Script example](#script-example)
+  - [Create a dataset with fast UI (FastDataset)](#create-a-dataset-with-fast-ui-fastdataset)
+  - [Create a dataset with manual UI (ManualDataset)](#create-a-dataset-with-manual-ui-manualdataset)
+    - [How to take pictures manually](#how-to-take-pictures-manually)
+  - [Build datasets from different npz files (BuildDataset)](#build-datasets-from-different-npz-files-builddataset)
+    - [Script example](#script-example-1)
   
 
+
 Xeye is a package for data collection to build computer vision applications based on inferential results of deep learning models. The main reasons to use Xeye are:
 
 * Create a dataset using only a laptop and its integrated camera (or alternatively an external USB camera);
 * Create a dataset already structured like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist);
 * Create a dataset that can be used for building models with [Tensorflow](https://www.tensorflow.org/) or [Pytorch](https://pytorch.org/).
 
+<hr>
 
 
 <div id='installation'/>
 
 ## Installation
 
 To install the package, 
 
 ```
 pip install xeye
 ```
 
+<hr>
+
+<div id='xeye-datasets-for-deep-learning'/>
+
+## Xeye datasets for deep learning 
+
+In the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository, you can find examples of deep learning model implementations based on datasets produced by the Xeye package (made with [Tensorflow](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/tensorflow) or [Pytorch](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/pytorch) frameworks).
+
+
+* [Binary dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing two types of grayscale images (with labels: 0=keyboard, 1=mouse).
+* [MultiLabel dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing three types of rgb images (three types of security cameras with labels: 0=dome, 1=bullet, 2=cube)
+
+Additionally, the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository contains examples of scripts that use the Xeye package to build datasets ([examples link](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/xeye-example)).
+
 <div id='create-a-dataset-with-full-ui'/>
 
-## Create a dataset with full UI 
+<hr>
+
+## Xeye functionalities
+
+The Xeye package includes three major approaches (classes) for creating a dataset from scratch: Dataset, FastDataset, and ManualDataset.
+
+* **Dataset**: Uses the full UI terminal interface.
+* **FastDataset**: Uses the constructor with all the specifications of the dataset.
+* **ManualDataset**: Same as FastDataset, but every image is shot manually one at a time.
+  
+Additionally, the package provides a method for combining datasets created with the **BuildDataset** class.
+
+<hr>
+
+## Create a dataset with full terminal UI (Dataset)
 
 First of all, load the module datapipe from the package:
 
 ```python
 import xeye
 ```
 
 then initialize the instance like this 
 
 ```python
 data = xeye.Dataset()
 ```
-set the parameters related to the images with the **init** function
+set the parameters related to the images with the **setup** method
 
 ```python
 data.setup()
-
 ```
-the execution of this function causes the starting of the user interface in the **terminal** 
+
+the execution of this method causes the starting of the user interface in the **terminal** 
 
 
 ```console
 --- CAMERA SETTING ---
 Select the index of the camera that you want to use for creating the dataset: 1
 ``` 
 
-the **init** function arises multiple questions that set the parameters' values
+the **setup** method arises multiple questions that set the parameters' values
 
 
 ```console
 --- IMAGE SETTINGS ---
 Num. of types of images to scan: 2
 Name of image type (1): keyboard
 Name of image type (2): mouse
@@ -103,262 +138,250 @@
 Single frame HEIGHT: 720
 Single frame WIDTH:  720
 num. of waiting time (in sec.) between every frame: 0
 ``` 
 
 Precisely the questions refer to:
 
-* **Select the index of the camera that you want to use for creating the dataset**: generally 0 for integrated camera, 1 for USB external camera.
-* **Num. of types of images to scan**: answer 2 if you want to create a dataset with two objects (e.g. keyboard and mouse). In general, answer with the number of object types to include in your dataset.
-* **Name of image type**: insert the name of every specific object you want to include in the dataset. The **init** function creates a named folder for every image type. 
-* **Num. of frames to shoot for every image type**: select the number of images you want to shoot and save them in every object folder. 
-* **Single frame HEIGHT**: frame height values.
-* **Single frame WIDTH**: frame width values.
+* **Select the index of the camera that you want to use for creating the dataset**: Generally 0 for integrated camera, 1 for USB external camera.
+* **Num. of types of images to scan**: Answer 2 if you want to create a dataset with two objects (e.g. keyboard and mouse). In general, answer with the number of object types to include in your dataset.
+* **Name of image type**: Insert the name of every specific object you want to include in the dataset. The **setup** method creates a named folder for every image type. 
+* **Num. of frames to shoot for every image type**: Select the number of images you want to shoot and save them in every object folder. 
+* **Single frame HEIGHT**: Frame height values.
+* **Single frame WIDTH**: Frame width values.
 * **Num. of waiting time (in sec.) between every frame**: e.g 0.2 causes a waiting time of 0.2 seconds between every shoot.
 
-After the parameters setting, you can invoke the function to start shooting images. Datapipe module provides two different formats of images:
+After the parameters setting, you can invoke the method to start shooting images. Datapipe module provides two different formats of images:
 
-* Grayscale image with the **gray** function;
-* Color image with the **rgb** function.
+* Grayscale image with the **gray** method;
+* Color image with the **rgb** method.
   
-Let's produce a dataset based on RGB images with the **rgb** function:
+Let's produce a dataset based on RGB images with the **rgb** method:
 
 ```python
 data.rgb()
 ```
-In the terminal keypress [b], to make photos for the image types passed to the **init** function.
+In the terminal keypress [b], to make photos for the image types passed to the **setup** method.
 
 ```console
 --- START TAKING PHOTOS ---
 Press [b] on the keyboard to start data collection of image type [keyboard]
 b
 Press [b] on the keyboard to start data collection of image type [mouse]
 b
 ``` 
 
-On the directory of the script, you can find the folders that contain the images produced by the **rbg** function (e.g. keyboard folder and mouse folder). 
+On the directory of the script, you can find the folders that contain the images produced by the **rbg** method (e.g. keyboard folder and mouse folder). 
 
 
 
-Images collected in the folders can be used for building datasets like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist). The first approach to achieve this result is calling the **compress_train_test** function:
+Images collected in the folders can be used for building datasets like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist). The first approach to achieve this result is calling the **compress_train_test** method:
 
 ```python
 data.compress_train_test()
 ```
 
 That produces the following output in the terminal window 
 
 ```console
 --- DATASET SETTING ---
 percentage of images in the test set: 0.2
 ``` 
 
-In which you can select the portion of images to use in the train and test datasets (write a value between (0,1)). By doing so, the function produces a **.npz** file formed by these specific tensors:
+In which you can select the portion of images to use in the train and test datasets (write a value between (0,1)). By doing so, the method produces a **.npz** file formed by these specific tensors:
 
 * Train set:
-  * **X_train**: matrices/tensors of every single image in the train dataset;
-  * **y_train**: classes (ordinal values) are associated with every image in the train dataset.
+  * **X_train**: Matrices/tensors of every single image in the train dataset;
+  * **y_train**: Classes (ordinal values) are associated with every image in the train dataset.
 * Test set:
-  * **X_test**: matrices/tensors of every single image in the test dataset;
-  * **y_test**: classes (ordinal values) are associated with every image in the test dataset.
+  * **X_test**: Matrices/tensors of every single image in the test dataset;
+  * **y_test**: Classes (ordinal values) are associated with every image in the test dataset.
   
 (matrices for grayscale images: [Height $\times$ Width $\times$ 1], tensors for RGB images:[Height $\times$ Width $\times$ 3]).
 
-An alternative approach is represented by the use of the function **compress_all**
+An alternative approach is represented by the use of the **compress_all** method
 
 ```python
 data.compress_all()
 ```
 
 In this case, the images are united in a unique tensor that contains all the frames produced previously. 
 
 * Unique tensor:
-  * **X**: matricies/tensors of every single image produced;
-  * **y**: classes (ordinal values) are associated with every image produced.
+  * **X**: Matricies/tensors of every single image produced;
+  * **y**: Classes (ordinal values) are associated with every image produced.
 
-Finally, you can use the **just_compress** function to create a unique tensor with all the images produced.
+Finally, you can use the **just_compress** method to create a unique tensor with all the images produced.
 
 ```python
 data.just_compress()
 ```
 In the terminal, you have to insert the dataset’s name
 
 ```console
 --- DATASET SETTING ---
 Select a name for the compressed file: batch_test
 ``` 
-If you pass 0, by default the dataset will be save with the name **dataset_raw.npz**. The dataset produced by this function can be used by the class **BuildDataset** to put together more .npz files and create a dataset like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist).
+If you pass 0, by default the dataset will be save with the name **dataset_raw.npz**. The dataset produced by this method can be used by the class **BuildDataset** to put together more .npz files and create a dataset like the [mnist](https://www.tensorflow.org/datasets/catalog/mnist).
 
-<div id='other-useful-functions'/>
+<div id='other-useful-methods'/>
 
-### Other useful functions
+### Other useful methods
 
-* **preview**: open the camera stream to check the framing. 
-  ![](img/1.png)
-* **var_control**: print the values of the parameters set with the **init** function. 
+* **preview**: Open the camera stream to check the framing. 
+* **var_control**: Print the values of the parameters set with the **setup** method. 
+  
 ```console
 --- PARAMETERS CONTROL ---
 camera index: 1
 num. of images types: 2
 labels of images types: ['keyboard', 'mouse']
 num. of images for types: 20
 Single frame HEIGHT: 720
 Single frame WIDTH:  720
 waiting time between frames: 0.0
 percentage of images in train dataset: 0.2
-statusGray: 1
-statusRGB: 0
 ``` 
 
 <div id='script-example-1'/>
 
 ### Script example 
 
 Example of a script to use the **Dataset** class:
 
 ```python
 import xeye
 data = xeye.dataset()
-data.init()
+data.setup()
 data.preview()
 data.rgb()
 data.compress_train_test()
 data.compress_all()
 data.just_compress()
-
 ```
+
+<hr>
+
 <div id='create-a-dataset-with-fast-ui'/>
 
-## Create a dataset with fast UI 
-A faster way to use the datapipe module is represented by the **FastDataset** class. In this case, there isn't a complete terminal UI that guides you in the construction of the dataset. With **FastDataset**, you only pass the parameters to the class, and then call the functions you need. 
+## Create a dataset with fast UI (FastDataset)
+
+The **FastDataset** class provides a faster way to use the datapipe module. Unlike the **Dataset** class, it does not have a complete terminal UI to guide you through the dataset construction process. Instead, you simply pass the parameters to the class and call the necessary methods.
 
 ```python
 import xeye
-
 # define parameters values
 index = 0
 img_types = 2
 label = ['keyboard', 'mouse']
 num = 20
 height = 100
 width = 100
 standby_time = 0
 # percentage of images in the test set 
 perc = 0.2
-
 data = xeye.FastDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width, stand_by_time = standby_time)
 data.preview()
 data.rgb()
 data.compress_train_test(perc = perc)
 data.compress_all()
 data.just_compress("batch_test")
 ```
 
 The parameters passed to the class **FastDataset**:
 
-* **index**: generally 0 for integrated camera, 1 for USB external camera.
-* **img_types**: numbers of object types that you want to include in your dataset.
-* **label**: list of object names to include in the dataset. The **init** function creates a named folder for every image type.
-* **num**: select the number of images you want to shoot and save them in every object folder.
-* **height**: frame height values.
-* **width**: frame width values.
+* **index**: Generally 0 for integrated camera, 1 for USB external camera.
+* **img_types**: Numbers of object types that you want to include in your dataset.
+* **label**: List of object names to include in the dataset. The **setup** method creates a named folder for every image type.
+* **num**: Select the number of images you want to shoot and save them in every object folder.
+* **height**: Frame height values.
+* **width**: Frame width values.
 * **standby_time**: e.g 0.2 cause a waiting time of 0.2 seconds between every shoot.
   
-For split images in the train and test dataset, pass a value between (0,1) to the perc parameter of the **compress_train_test** function
+For split images in the train and test dataset, pass a value between (0,1) to the perc parameter of the **compress_train_test** method
 
 * **perc**: the portion of images to use in the test dataset, write a value between (0,1).
 
-If you don't pass any value to the **just_compress** function, the dataset will be saved with the name **dataset_raw.npz**.
-
+If you don't pass any value to the **just_compress** method, the dataset will be saved with the name **dataset_raw.npz**.
 
+<hr>
 
 <div id='create-a-dataset-with-manual-ui'/>
 
-## Create a dataset with manual UI 
+## Create a dataset with manual UI (ManualDataset)
+
 The **ManualDataset** class is how you can build a dataset by taking pictures manually. 
 
 ```python
 import xeye
-
 # define parameters values
 index = 0
 img_types = 2
 label = ['keyboard', 'mouse']
 num = 20
 height = 100
 width = 100
 standby_time = 0
 # percentage of images in the test set 
 perc = 0.2
-
 data = xeye.ManualDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width)
 data.preview()
 data.rgb()
 data.compress_train_test(perc = perc)
 data.compress_all()
 data.just_compress("batch_test")
 ```
 
 As you can see in the code snippet, the **ManualDataset** class works like the **FastDataset** class. The only difference is the absence of the **standby_time option**, which is no more necessary in this case. 
 
 The parameters passed to the class **ManualDataset**:
 
-* **index**: generally 0 for integrated camera, 1 for USB external camera.
-* **img_types**: numbers of object types that you want to include in your dataset.
-* **label**: list of object names to include in the dataset. The **init** function creates a named folder for every image type.
-* **num**: select the number of images you want to shoot and save them in every object folder.
-* **height**: frame height values.
-* **width**: frame width values.
+* **index**: Generally 0 for integrated camera, 1 for USB external camera.
+* **img_types**: Numbers of object types that you want to include in your dataset.
+* **label**: List of object names to include in the dataset. The constructor creates a named folder for every image type.
+* **num**: Select the number of images you want to shoot and save them in every object folder.
+* **height**: Frame height values.
+* **width**: Frame width values.
 
-### How to take pictures manually
 
-On the image window title, after the image type caption it's reported how to take pictures manually with the **ManualDataset**
+### How to take pictures manually
 
-* Press [s] on the keyboard to save the image nr: 1
+In the title bar of the image window, after the caption identifying the image type, there are instructions for manually taking pictures using the ManualDataset. These instructions will be displayed as follows:
 
-![](img/manual.png)
+* Camera view for image type <name-of-image-type>. Press [s] on the keyboard to save image number: <nr-of-image>.
+ 
 
-Press [s] until you reach the number of frames passed to the **num** parameter of the class. 
+<hr>
 
-## Build datasets from different .npz files 
+## Build datasets from different npz files (BuildDataset)
 
-If you want to build datasets made by different types of images, but for example, you can't shoot one of the image types that compose the dataset (because you have to wait a significant amount of time or change location), you can use the **BuildDataset** class. 
+If you want to create a dataset that includes different types of images, but cannot shoot all image types at once (e.g., due to time constraints or location differences), you can use the **BuildDataset** class.
 
-* Create datasets with the **just_compress** function;
+* Create datasets with the **just_compress** method;
 * Create different .npz files for every type of images that composes the dataset (use the same colour spaces in all datasets, RGB or grayscale);
 * Create a new script and call the **BuildDataset** class that merges all the .npz files created before.
 
 <div id='script-example-2'/>
 
 ### Script example 
 
 ```python
 import xeye
 # list of directory (paths for the .npz files)
-path = ['/Users/marcosalvalaggio/code/testxeye/dataset/batch_2.npz', '/Users/marcosalvalaggio/code/testxeye/dataset/batch_3.npz']
+path = ['batch_2.npz', 'batch_3.npz']
 # list of labels associated with the images inside the .npz files
 label = [0,1]
-# initializes the class
 data = xeye.BuildDataset(path=path, label=label, size = None, color=True, split=True, perc=0.2)
 data.build()
 ```
 The parameters passed to the class **BuildDataset**:
 
-* **path**: list of files (.npz) path you want to include in the new dataset
-* **label**: list of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
-* **size**: tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
-* **color**: defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
-* **split**: defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
-* **perc**: defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
+* **path**: List of files (.npz) path you want to include in the new dataset
+* **label**: List of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
+* **size**: Tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
+* **color**: Defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
+* **split**: Defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
+* **perc**: Defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
 
 When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
 
 
-<div id='xeye-datasets-for-deep-learning'/>
-
-## Xeye datasets for deep learning 
-
-In the [xeye-notebooks](https://github.com/marcosalvalaggio/xeye-notebooks) repository, you can find examples of deep learning model implementations based on datasets produced by the Xeye package (made with [Tensorflow](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/tensorflow) or [Pytorch](https://github.com/marcosalvalaggio/xeye-notebooks/tree/main/pytorch) frameworks).
-
-
-* [Binary dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing two types of grayscale images (with labels: 0=keyboard, 1=mouse).
-* [MultiLabel dataset](https://drive.google.com/drive/folders/1qvoFa4SRWirXj7kdWhhcqrQ8mTIHpkuJ?usp=sharing): containing three types of rgb images (three types of security cameras with labels: 0=dome, 1=bullet, 2=cube)
```

