# Comparing `tmp/plons-0.0.7.tar.gz` & `tmp/plons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plons-0.0.7.tar", last modified: Wed Mar 22 16:04:09 2023, max compression
+gzip compressed data, was "plons-0.0.9.tar", last modified: Wed Apr  5 14:48:24 2023, max compression
```

## Comparing `plons-0.0.7.tar` & `plons-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:04:09.107857 plons-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-22 16:03:56.000000 plons-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50239 2023-03-22 16:04:09.107857 plons-0.0.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     8948 2023-03-22 16:03:56.000000 plons-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-22 16:03:56.000000 plons-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 16:04:09.107857 plons-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:04:09.103857 plons-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:04:09.107857 plons-0.0.7/src/plons/
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/ArchimedianSpiral.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22461 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/CMF_meanRho.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/ConversionFactors_cgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13379 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/GeometricalFunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/LoadDataPHANTOM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13996 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/LoadDump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5532 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/LoadSetup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12700 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/LoadSink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30649 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/OrbitalEvolution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3880 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/PhysicalQuantities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22053 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/Profiles1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12276 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/RadialStructurePlots1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6099 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/RhoRradialFit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34755 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/SlicePlots2D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9347 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/SmoothingKernelScript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26055 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/TerminalVelocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3748 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/Tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9727 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/Tubes.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/animationSlicePlots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9529 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17171 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/merge1DPlotsDion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22924 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/profile_1D_spherical_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5429 2023-03-22 16:03:56.000000 plons-0.0.7/src/plons/userSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:04:09.107857 plons-0.0.7/src/plons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50239 2023-03-22 16:04:09.000000 plons-0.0.7/src/plons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-22 16:04:09.000000 plons-0.0.7/src/plons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:04:09.000000 plons-0.0.7/src/plons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-22 16:04:09.000000 plons-0.0.7/src/plons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 16:04:09.000000 plons-0.0.7/src/plons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:04:09.107857 plons-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-22 16:03:56.000000 plons-0.0.7/tests/test_SmoothingKernelScript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:48:24.301936 plons-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-05 14:48:11.000000 plons-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49503 2023-04-05 14:48:24.301936 plons-0.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8212 2023-04-05 14:48:11.000000 plons-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-05 14:48:11.000000 plons-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:48:24.301936 plons-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:48:24.293936 plons-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:48:24.297936 plons-0.0.9/src/plons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/ArchimedianSpiral.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22380 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/CMF_meanRho.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/ConversionFactors_cgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13379 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/GeometricalFunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2908 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/LoadDataPHANTOM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14024 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/LoadDump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5468 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/LoadSetup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12450 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/LoadSink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30914 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/OrbitalEvolution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31481 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/OrbitalEvolutionWAql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3915 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/PhysicalQuantities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22032 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/Profiles1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11997 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/RadialStructurePlots1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5886 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/RhoRradialFit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34585 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/SlicePlots2D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9347 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/SmoothingKernelScript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26089 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/TerminalVelocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3748 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/Tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/Tubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9437 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9485 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/mainWAql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22930 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/profile_1D_spherical_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5433 2023-04-05 14:48:11.000000 plons-0.0.9/src/plons/userSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:48:24.301936 plons-0.0.9/src/plons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49503 2023-04-05 14:48:24.000000 plons-0.0.9/src/plons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-05 14:48:24.000000 plons-0.0.9/src/plons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:48:24.000000 plons-0.0.9/src/plons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-05 14:48:24.000000 plons-0.0.9/src/plons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 14:48:24.000000 plons-0.0.9/src/plons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:48:24.301936 plons-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-05 14:48:11.000000 plons-0.0.9/tests/test_SmoothingKernelScript.py
```

### Comparing `plons-0.0.7/LICENSE` & `plons-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plons-0.0.7/PKG-INFO` & `plons-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plons
-Version: 0.0.7
+Version: 0.0.9
 Summary: PLOtting tool for Nice Simulations
 Author-email: Jolien Malfait <jolien.malfait@kuleuven.be>, Mats Esseldeurs <mats.esseldeurs@kuleuven.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,113 +690,101 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 
 
 
 -------------------------------
-    README PHANTOM PIPELINE 
+    README PLONS
 -------------------------------
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/build-and-test.yaml/badge.svg)
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/upload-to-pypi.yaml/badge.svg)
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/upload-to-anaconda.yaml/badge.svg)
 
 
-This is the README for the first python pipeline ever to reduce data of hydrodynamical 
-simulations by use of the SPH code PHANTOM (Price, D. J., Wurster, J., Tricco, T. S., 
-et al. 2018, PASA, 35, e031). PHANTOM returns different types of useful data files: 
-'wind_xxxxx'-files and '.ev'-files. The former can only be read in its raw form by the 
-SPH visualisation tool SPLASH (Price, D. J. 2007, PASA, 24, 159; 
-https://users.monash.edu.au/~dprice/splash/). By using SPLASH, the files can be converted 
-to .ascii to use for reduction. The .ev-files can be use straight away, but can also be 
-visualised using SPLASH.
+This is the README for the PLONS PLOtting tool for Nice Simulations. It can be used to
+read in and analyse data of hydrodynamical simulations with the SPH code PHANTOM 
+(Price, D. J., Wurster, J., Tricco, T. S., et al. 2018, PASA, 35, e031). PHANTOM returns 
+(different types of useful data files: 'wind_xxxxx'-files and '.ev'-files. The former can
+also be visualised by the SPH visualisation tool SPLASH (Price, D. J. 2007, PASA, 24, 159; 
+https://users.monash.edu.au/~dprice/splash/), and can be analysed more toroughly with PLONS.
+
 
 PHANTOM
 -------
 
 PHANTOM returns (full) dump files every certain timestep during the evolution of the 
 model. These are the wind_xxxxx-files and contain the relevant data (position, velocity, 
 mass, density, energy, temperature) of the SPH particles in the model. The last x rows of 
 the output are the x sink particles in the model. More detailed information of the sink 
 particles (position, velocity, mass, accreted mass, spin, angular momentum) in function of 
 evolution time of the model, can be retrieved in the .ev files.
 
-Pipeline - General
+PLONS - General
 ------------------
 
-This pipeline is suited for binary and single AGB wind models.
+This pipeline is suited for single, binary and triple AGB wind models.
+
+The following info can be attained:
+
+(1) 2D slice plots of the global structure of the last dump full of the model.
+(2) 1D line plots (radial structure) of the global structure of the last dump of the model along the x-, y- and z-axes.
+(3) Information about the velocity related quantities of the model + Quantitative measurement of the degree of aspherical morphology: morphological parameters eta, Qp and epsilon.
+(4) Cummulative mass fraction in function of the polar coordinate theta.
+(5) Information of the orbital evolution.
+(6) 1D spherical profiles for single star models
 
-By giving the directory where the models are located as input, the last full dump in .ascii 
-and the .ev files of the sink particle(s) are reduced in order to gain relevant information 
-about the model:
-(1)  2D slice plots of the density, speed and temperature are produced (face-on/orbital plane 
-     & edge-on plane).
-(2)  1D radial plots of the density, speed and temperature are produced (along the x-, y- and 
-     z-axes).
-(3)  The terminal velocity in the model is calculated.
-(4)  Four morphological parameters are determined, giving a more quantitative insight in the 
-     degree of aspherity.
-(5)  The cummulative mass fraction and mean density are calculated in function of polar coordinate 
-     theta. This gives an indication about the degree of equatorial density enhancement (EDE).
-(6)  Information about the orbital evolution of the binary system and accreted mass onto the 
-     companion.
 
 
 Pipeline - More detailed information
 ------------------------------------
 
 This pipeline loads the wind.in and wind.setup files first. This is the general setup information 
 of the model (configuration of the system, information of the thermodynamics, evolution time, wind 
 outflow setup,...). Next the last full dump is loaded, and using this data, some other useful 
 quantities are calculated (gas pressure/temperature, speed, sperical coordinates, sound speed of 
 the gas,...).  Lastly, the data of the sink particle(s) is loaded. From this file, also the period 
-and orbital velocity of the sink particles in calculated, if the system is a binary, in function of 
+and orbital velocity of the sink particles is calculated, if the system is a multiple, in function of 
 time. The last entry in the sink data, corresponds to the full dump loaded. Therefore the 
 position/velocity/mass/... of this last entry are also saved in the full dump data for easy usage.
 
-NOTE: If you have paused and restarted your simulation, multiple .ev files will be constructed per 
-sink particle. The code anticipates to this problem, but you have to say so in the code yourself: 
-Uncomment the part starting at line 50 in the LoadSink.py script and put in the correct model. 
-
 
 (1)
 
 The 2D slices in the plots are infinitely thin and calculated by using the smoothing kernel from
-PHANTOM. The density, speed and temperature are calculated by this method on a grid of 300*300 
-pixels, using the data of the 20 nearest neighbours (SPH particles) of those grid points. These 
+PHANTOM. The density, speed and temperature are calculated by this method on a grid of n*n 
+pixels, using the data of the m nearest neighbours (SPH particles) of those grid points. These 
 plots give a visual representation of the morphology present in the AGB wind of the simulation.
 
 
 (2)
 
 In 1D, the data along the x-, y- and z-axes is constructed in the same way as explained in (1), 
 but for a 1D grid. This results in plots of the radial structure, which is an important addition 
 to the 2D slice plots.
 
 
 (3)
 
-The terminal velocity is in the case of the PHANTOM SPH code not an input parameter, so it needs 
-to be calculated. Due to the morphology in the outflow of the AGB star, at a certain radius a wide
-range of speeds will be obtained. Therefore calculating only one value for the terminal velocity 
-is not possible. Instead, three values are obtained, a minimum, mean and maximum terminal velocity. 
-The method used here is binning of the speed in function of the radius of the SHP particle to the 
-AGB star. Bins of 1AU are constructed and per bin, the minimum, mean and maximum speed is calculated.
-Using speed of the outer 20% of the data, three values for the terminal velocity are obtained. 
+The terminal velocity in PHANTOM SPH code is not an input parameter, so it needs to be calculated. 
+Due to the morphology in the outflow of the AGB star, at a certain radius a wide range of speeds 
+will be obtained. Therefore calculating only one value for the terminal velocity is not possible. 
+Instead, three values are obtained, a minimum, mean and maximum terminal velocity. The method used 
+here is binning the speed in function of the radius of the SHP particle to the AGB star. Bins of 
+1AU are constructed and per bin, the minimum, mean and maximum speed is calculated. Using speed of 
+the outer 20% of the data, three values for the terminal velocity are obtained. 
 
 NOTE: For some models (most often with slow initial wind velocity, low mass loss rate and/or low-mass 
 companion), the interaction of the companion has not reached the outer boundary of the model. Therefore, 
 this method will not lead to a correct terminal velocity value and thus the unphysical part of the data 
 will be cut off. Visually, the speed profile in function of radius shows a strong, unphysical linear 
 increase, starting with a clear twist.
 
 
-(4)
-
-In order to get some quantitative indication about the morphology of the models, two morphology 
+In order to get some quantitative indication about the morphology of the models, several morphology 
 parameters are currently in use: 
     - eta = v/v_orb (see Saladino, M. I., Pols, O. R., van der Helm, E., Pelupessy, I., & 
       Portegies Zwart, S. 2018, A&A, 618, A50; El Mellah, I., Bolte, J., Decin, L., Homan, 
       W., & Keppens, R. 2020, arXiv e-prints, arXiv:2001.04482)
     - Qp = p_comp/p_wind 
          = (M_comp v_orb) / (M_wind v_wind)
         (see Decin, L., Montarges, M., Richards, A. M. S., et al. 2020, Science, 369, 1497)
@@ -806,15 +794,15 @@
 Depending on the value of these parameters, the model is expected to show radial/EDE/complex morphology.
 
 Rhill = a(1-e)(M_comp/ 3M_AGB)^(1/3)
 Therefore, Rhill/Rcapt = epsilon, if for both radii the same v_wind is used.
 
 VERY IMPORTANT NOTE: 
 The parameter 'v_wind' is not unambiguously defined. Even more, if only a binary models is used, 
-this parameter is most likely not to be contrained properly. For the different morphological parameters, 
+this parameter is most likely not to be constrained properly. For the different morphological parameters, 
 multiple values for v_wind are used.
 For eta, different velocities/speed v are used:
     - terminal velocity
     - speed of the wind at the location of the companion 
 For Qp and epsilon, two different values are used as v_wind:
     - the mean velocity of the wind at the location is used as calculated from the binning
     - the average of the min and max velocity at the location of the companion is used
@@ -823,15 +811,15 @@
 Better options for v_wind would be to use the velocity of the corresponding single model as follows:
     - speed of the wind at the location of the companion
     - speed resulting from the vector sum of the speed of the wind at the location of the companion 
       and the orbital velocity of the AGB star.
 These can be calculated using the output of this pipeline.
 
 
-(5)
+(4)
 
 The cummulative mass fraction (CMF) is calculated in function of the polar angle theta (theta = 0.5pi 
 is the orbital plane, theta = 0 the north pole), again by using the method of binning. Only the northern 
 hemisphere is used, because of symmetry. Because of asymmetry along the x-axis, the positive (right) 
 and negative (left) part according to x are also calculated seperately. Certainly for eccentric models 
 this can differ. To calculate the CMF, only the selfsimilar part of the outflow it used, therefore a 
 factor (called factor) is given. The inner factor * semi-major axis AU is left out in this calculation.
@@ -841,15 +829,15 @@
 (theta25-theta50)/(theta50-theta75). When this parameter is normalised to the value for the corresponding 
 single model, it gives a measure for the degree of EDE.
 
 Also the mean density is calculated using a similar approach as the CMF, using the method of binning. 
 This mean density can easily be normalised to compare the morphology in different models.
 
 
-(6)
+(5)
 
 In order to get information about the orbital evolution, the sink files are used (.ev), which gives
 relevant quantities of the sink particles in function of time. This file returns plots of the orbit, 
 evolution of orbital separation, orbital velocity and accreted mass of the companion.
```

### Comparing `plons-0.0.7/README.md` & `plons-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,98 @@
 
 
 
 -------------------------------
-    README PHANTOM PIPELINE 
+    README PLONS
 -------------------------------
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/build-and-test.yaml/badge.svg)
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/upload-to-pypi.yaml/badge.svg)
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/upload-to-anaconda.yaml/badge.svg)
 
 
-This is the README for the first python pipeline ever to reduce data of hydrodynamical 
-simulations by use of the SPH code PHANTOM (Price, D. J., Wurster, J., Tricco, T. S., 
-et al. 2018, PASA, 35, e031). PHANTOM returns different types of useful data files: 
-'wind_xxxxx'-files and '.ev'-files. The former can only be read in its raw form by the 
-SPH visualisation tool SPLASH (Price, D. J. 2007, PASA, 24, 159; 
-https://users.monash.edu.au/~dprice/splash/). By using SPLASH, the files can be converted 
-to .ascii to use for reduction. The .ev-files can be use straight away, but can also be 
-visualised using SPLASH.
+This is the README for the PLONS PLOtting tool for Nice Simulations. It can be used to
+read in and analyse data of hydrodynamical simulations with the SPH code PHANTOM 
+(Price, D. J., Wurster, J., Tricco, T. S., et al. 2018, PASA, 35, e031). PHANTOM returns 
+(different types of useful data files: 'wind_xxxxx'-files and '.ev'-files. The former can
+also be visualised by the SPH visualisation tool SPLASH (Price, D. J. 2007, PASA, 24, 159; 
+https://users.monash.edu.au/~dprice/splash/), and can be analysed more toroughly with PLONS.
+
 
 PHANTOM
 -------
 
 PHANTOM returns (full) dump files every certain timestep during the evolution of the 
 model. These are the wind_xxxxx-files and contain the relevant data (position, velocity, 
 mass, density, energy, temperature) of the SPH particles in the model. The last x rows of 
 the output are the x sink particles in the model. More detailed information of the sink 
 particles (position, velocity, mass, accreted mass, spin, angular momentum) in function of 
 evolution time of the model, can be retrieved in the .ev files.
 
-Pipeline - General
+PLONS - General
 ------------------
 
-This pipeline is suited for binary and single AGB wind models.
+This pipeline is suited for single, binary and triple AGB wind models.
+
+The following info can be attained:
+
+(1) 2D slice plots of the global structure of the last dump full of the model.
+(2) 1D line plots (radial structure) of the global structure of the last dump of the model along the x-, y- and z-axes.
+(3) Information about the velocity related quantities of the model + Quantitative measurement of the degree of aspherical morphology: morphological parameters eta, Qp and epsilon.
+(4) Cummulative mass fraction in function of the polar coordinate theta.
+(5) Information of the orbital evolution.
+(6) 1D spherical profiles for single star models
 
-By giving the directory where the models are located as input, the last full dump in .ascii 
-and the .ev files of the sink particle(s) are reduced in order to gain relevant information 
-about the model:
-(1)  2D slice plots of the density, speed and temperature are produced (face-on/orbital plane 
-     & edge-on plane).
-(2)  1D radial plots of the density, speed and temperature are produced (along the x-, y- and 
-     z-axes).
-(3)  The terminal velocity in the model is calculated.
-(4)  Four morphological parameters are determined, giving a more quantitative insight in the 
-     degree of aspherity.
-(5)  The cummulative mass fraction and mean density are calculated in function of polar coordinate 
-     theta. This gives an indication about the degree of equatorial density enhancement (EDE).
-(6)  Information about the orbital evolution of the binary system and accreted mass onto the 
-     companion.
 
 
 Pipeline - More detailed information
 ------------------------------------
 
 This pipeline loads the wind.in and wind.setup files first. This is the general setup information 
 of the model (configuration of the system, information of the thermodynamics, evolution time, wind 
 outflow setup,...). Next the last full dump is loaded, and using this data, some other useful 
 quantities are calculated (gas pressure/temperature, speed, sperical coordinates, sound speed of 
 the gas,...).  Lastly, the data of the sink particle(s) is loaded. From this file, also the period 
-and orbital velocity of the sink particles in calculated, if the system is a binary, in function of 
+and orbital velocity of the sink particles is calculated, if the system is a multiple, in function of 
 time. The last entry in the sink data, corresponds to the full dump loaded. Therefore the 
 position/velocity/mass/... of this last entry are also saved in the full dump data for easy usage.
 
-NOTE: If you have paused and restarted your simulation, multiple .ev files will be constructed per 
-sink particle. The code anticipates to this problem, but you have to say so in the code yourself: 
-Uncomment the part starting at line 50 in the LoadSink.py script and put in the correct model. 
-
 
 (1)
 
 The 2D slices in the plots are infinitely thin and calculated by using the smoothing kernel from
-PHANTOM. The density, speed and temperature are calculated by this method on a grid of 300*300 
-pixels, using the data of the 20 nearest neighbours (SPH particles) of those grid points. These 
+PHANTOM. The density, speed and temperature are calculated by this method on a grid of n*n 
+pixels, using the data of the m nearest neighbours (SPH particles) of those grid points. These 
 plots give a visual representation of the morphology present in the AGB wind of the simulation.
 
 
 (2)
 
 In 1D, the data along the x-, y- and z-axes is constructed in the same way as explained in (1), 
 but for a 1D grid. This results in plots of the radial structure, which is an important addition 
 to the 2D slice plots.
 
 
 (3)
 
-The terminal velocity is in the case of the PHANTOM SPH code not an input parameter, so it needs 
-to be calculated. Due to the morphology in the outflow of the AGB star, at a certain radius a wide
-range of speeds will be obtained. Therefore calculating only one value for the terminal velocity 
-is not possible. Instead, three values are obtained, a minimum, mean and maximum terminal velocity. 
-The method used here is binning of the speed in function of the radius of the SHP particle to the 
-AGB star. Bins of 1AU are constructed and per bin, the minimum, mean and maximum speed is calculated.
-Using speed of the outer 20% of the data, three values for the terminal velocity are obtained. 
+The terminal velocity in PHANTOM SPH code is not an input parameter, so it needs to be calculated. 
+Due to the morphology in the outflow of the AGB star, at a certain radius a wide range of speeds 
+will be obtained. Therefore calculating only one value for the terminal velocity is not possible. 
+Instead, three values are obtained, a minimum, mean and maximum terminal velocity. The method used 
+here is binning the speed in function of the radius of the SHP particle to the AGB star. Bins of 
+1AU are constructed and per bin, the minimum, mean and maximum speed is calculated. Using speed of 
+the outer 20% of the data, three values for the terminal velocity are obtained. 
 
 NOTE: For some models (most often with slow initial wind velocity, low mass loss rate and/or low-mass 
 companion), the interaction of the companion has not reached the outer boundary of the model. Therefore, 
 this method will not lead to a correct terminal velocity value and thus the unphysical part of the data 
 will be cut off. Visually, the speed profile in function of radius shows a strong, unphysical linear 
 increase, starting with a clear twist.
 
 
-(4)
-
-In order to get some quantitative indication about the morphology of the models, two morphology 
+In order to get some quantitative indication about the morphology of the models, several morphology 
 parameters are currently in use: 
     - eta = v/v_orb (see Saladino, M. I., Pols, O. R., van der Helm, E., Pelupessy, I., & 
       Portegies Zwart, S. 2018, A&A, 618, A50; El Mellah, I., Bolte, J., Decin, L., Homan, 
       W., & Keppens, R. 2020, arXiv e-prints, arXiv:2001.04482)
     - Qp = p_comp/p_wind 
          = (M_comp v_orb) / (M_wind v_wind)
         (see Decin, L., Montarges, M., Richards, A. M. S., et al. 2020, Science, 369, 1497)
@@ -114,15 +102,15 @@
 Depending on the value of these parameters, the model is expected to show radial/EDE/complex morphology.
 
 Rhill = a(1-e)(M_comp/ 3M_AGB)^(1/3)
 Therefore, Rhill/Rcapt = epsilon, if for both radii the same v_wind is used.
 
 VERY IMPORTANT NOTE: 
 The parameter 'v_wind' is not unambiguously defined. Even more, if only a binary models is used, 
-this parameter is most likely not to be contrained properly. For the different morphological parameters, 
+this parameter is most likely not to be constrained properly. For the different morphological parameters, 
 multiple values for v_wind are used.
 For eta, different velocities/speed v are used:
     - terminal velocity
     - speed of the wind at the location of the companion 
 For Qp and epsilon, two different values are used as v_wind:
     - the mean velocity of the wind at the location is used as calculated from the binning
     - the average of the min and max velocity at the location of the companion is used
@@ -131,15 +119,15 @@
 Better options for v_wind would be to use the velocity of the corresponding single model as follows:
     - speed of the wind at the location of the companion
     - speed resulting from the vector sum of the speed of the wind at the location of the companion 
       and the orbital velocity of the AGB star.
 These can be calculated using the output of this pipeline.
 
 
-(5)
+(4)
 
 The cummulative mass fraction (CMF) is calculated in function of the polar angle theta (theta = 0.5pi 
 is the orbital plane, theta = 0 the north pole), again by using the method of binning. Only the northern 
 hemisphere is used, because of symmetry. Because of asymmetry along the x-axis, the positive (right) 
 and negative (left) part according to x are also calculated seperately. Certainly for eccentric models 
 this can differ. To calculate the CMF, only the selfsimilar part of the outflow it used, therefore a 
 factor (called factor) is given. The inner factor * semi-major axis AU is left out in this calculation.
@@ -149,15 +137,15 @@
 (theta25-theta50)/(theta50-theta75). When this parameter is normalised to the value for the corresponding 
 single model, it gives a measure for the degree of EDE.
 
 Also the mean density is calculated using a similar approach as the CMF, using the method of binning. 
 This mean density can easily be normalised to compare the morphology in different models.
 
 
-(6)
+(5)
 
 In order to get information about the orbital evolution, the sink files are used (.ev), which gives
 relevant quantities of the sink particles in function of time. This file returns plots of the orbit, 
 evolution of orbital separation, orbital velocity and accreted mass of the companion.
```

### Comparing `plons-0.0.7/pyproject.toml` & `plons-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plons"
-version = "0.0.7"
+version = "0.0.9"
 description = "PLOtting tool for Nice Simulations"
 readme = "README.md"
 authors = [{ name = "Jolien Malfait",  email = "jolien.malfait@kuleuven.be" },
            { name = "Mats Esseldeurs", email = "mats.esseldeurs@kuleuven.be"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -34,15 +34,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Ensor-code/plons"
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `plons-0.0.7/src/plons/ArchimedianSpiral.py` & `plons-0.0.9/src/plons/ArchimedianSpiral.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import scipy.integrate       as integrate
 import matplotlib.pyplot     as plt
 import numpy as np
 import os
-from ConversionFactors_cgs   import au, Msun, G
+from plons.ConversionFactors_cgs   import au, Msun, G
 
 def velocities(run):
     if   run == 'Lucy/High/binary6':
         v_i = 45e5   # km/s
         v_o = 50e5   # km/s 
     elif run == 'Lucy/High/binary9':
         v_i = 45e5   # km/s
```

### Comparing `plons-0.0.7/src/plons/CMF_meanRho.py` & `plons-0.0.9/src/plons/CMF_meanRho.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #Import packages
 import numpy                as np
 import os
 import matplotlib.pyplot    as plt
 import matplotlib.lines     as mlines
 # import certain things from packages
-from collections            import OrderedDict
-from astropy                import constants
-from matplotlib             import rcParams, rc
+from matplotlib             import rcParams
 # Change the matplotlib default parameters
 rcParams.update({'font.size':   11})
 rcParams.update({'figure.dpi': 200})
 #rc('font', family='serif')
 #rc('text', usetex=True)
 
-# own scripts
-import Tools                 as tl
+# import plons scripts
+import plons.Tools                 as tl
 
 # ignore warnings
 import warnings
 warnings.filterwarnings("ignore")
 
 
 '''
```

### Comparing `plons-0.0.7/src/plons/ConversionFactors_cgs.py` & `plons-0.0.9/src/plons/ConversionFactors_cgs.py`

 * *Files identical despite different names*

### Comparing `plons-0.0.7/src/plons/GeometricalFunctions.py` & `plons-0.0.9/src/plons/GeometricalFunctions.py`

 * *Files identical despite different names*

### Comparing `plons-0.0.7/src/plons/LoadDataPHANTOM.py` & `plons-0.0.9/src/plons/LoadDataPHANTOM.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import numpy                    as np
 import math                     as math
-import os
-# own scripts
-import PhysicalQuantities       as pq
-import ConversionFactors_cgs    as cgs
-import LoadDump                 as dmp
-import LoadSink                 as snk
-import LoadSetup                as stp
+
+#import plons scripts
+import plons.LoadDump                 as dmp
+import plons.LoadSink                 as snk
+import plons.LoadSetup                as stp
 
 
 '''
 Load the data for a general model
     * INPUT
         - 'run'     [str]   number of the model 
         - 'loc'     [str]   directory of the output data from PHANTOM
```

### Comparing `plons-0.0.7/src/plons/LoadDump.py` & `plons-0.0.9/src/plons/LoadDump.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy                    as np
 import math                     as math
 import os
-# own scripts
-import PhysicalQuantities       as pq
-import GeometricalFunctions     as gf
-import ConversionFactors_cgs    as cgs
 import sys
 
+# Import plons scripts
+import plons.PhysicalQuantities       as pq
+import plons.GeometricalFunctions     as gf
+import plons.ConversionFactors_cgs    as cgs
+
 '''
 Loads the final full dump of a phantom model, given the number, in cgs-units 
     
 INPUT:
     - 'run'   is the number of the run specifically           [str]
     - 'loc'   is the directory where the model is located     [str]
     - 'setup' is the setup data                               [dict]
```

### Comparing `plons-0.0.7/src/plons/LoadSetup.py` & `plons-0.0.9/src/plons/LoadSetup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import numpy                    as np
 import math                     as math
 import os
 # own scripts
-import PhysicalQuantities       as pq
-import GeometricalFunctions     as gf
-import ConversionFactors_cgs    as cgs
+import plons.PhysicalQuantities       as pq
+import plons.ConversionFactors_cgs    as cgs
 
 
 
 '''
 Only load the prefix.in and prefix.setup files to get general information about the phantom model
       Suited for binary and single model
```

### Comparing `plons-0.0.7/src/plons/LoadSink.py` & `plons-0.0.9/src/plons/LoadSink.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import numpy                    as np
 import math                     as math
 import os
-# own scripts
-import PhysicalQuantities       as pq
-import GeometricalFunctions     as gf
-import ConversionFactors_cgs    as cgs
-import LoadSetup                as stp
 import sys
 
+# Import plons scripts
+import plons.PhysicalQuantities       as pq
+import plons.GeometricalFunctions     as gf
+import plons.ConversionFactors_cgs    as cgs
+
+
 
 
 
 '''
 Load the .ev-files from a phantom model
       - This file gives the specifics of the sink particles present in the model (AGB star and companion, not of the sph particles)
         in function of the evolution time of the model. The last entry corresponds to the data from the last dump.
       - Only suited for a binary model
       - Units in cgs
-      
+
 INPUT:
     - 'run'   is the number of the run specifically           [str]
     - 'loc'   is the directory where the model is located     [str]
     - 'setup' is the setup data                               [dict]
-    
+
 RETURN:
     a dictionary containing the data from the sink files (all units in cgs)
-    
+
 '''
 def LoadSink_cgs(run, loc, setup, userSettingsDictionary):
 
     runName = os.path.join(loc, run)
     userPrefix = userSettingsDictionary["prefix"]
 
     # load the dump file wind_00xxx
     t1, x1, y1, z1, mass1, vx1, vy1, vz1, maccr1 = 0, 0, 0, 0, 0, 0, 0, 0, 0
     t2, x2, y2, z2, mass2, vx2, vy2, vz2, maccr2 = 0, 0, 0, 0, 0, 0, 0, 0, 0
     if setup['triple_star']==True:
         t3, x3, y3, z3, mass3, vx3, vy3, vz3, maccr3 = 0, 0, 0, 0, 0, 0, 0, 0, 0
 
-    numberOfevFiles = findLastWindSinkIndex(runName)
+    numberOfevFiles = findLastWindSinkIndex(runName,userPrefix)
 
     for n in range(1,numberOfevFiles+1):
         #print(n)
         fileName_sink1 = os.path.join(runName, str('%sSink0001N0'%userPrefix+str(n)+'.ev'))
         fileName_sink2 = os.path.join(runName, str('%sSink0002N0'%userPrefix+str(n)+'.ev'))
 
         if setup['triple_star']==True:
@@ -53,15 +54,15 @@
             (t1e, x1e,y1e,z1e, mass1e, vx1e,vy1e,vz1e, maccr1e) = np.loadtxt(fileName_sink1, skiprows=1, usecols=(0,1,2,3,4,5,6,7,11), unpack=True)
             n_file = len(t1e)
             (t2e, x2e,y2e,z2e, mass2e, vx2e,vy2e,vz2e, maccr2e) = np.loadtxt(fileName_sink2, skiprows=1, usecols=(0,1,2,3,4,5,6,7,11), unpack=True)[:, :n_file]
             if setup['triple_star']==True:
                 (t3e, x3e,y3e,z3e, mass3e, vx3e,vy3e,vz3e, maccr3e) = np.loadtxt(fileName_sink3, skiprows=1, usecols=(0,1,2,3,4,5,6,7,11), unpack=True)[:, :n_file]
         except OSError:
             print(' ERROR: No sink files found for this model in the current directory!')
-            
+
         t1     = np.append(t1,t1e)
         x1     = np.append(x1,x1e)
         y1     = np.append(y1,y1e)
         z1     = np.append(z1,z1e)
         mass1  = np.append(mass1, mass1e)
         vx1    = np.append(vx1, vx1e)
         vy1    = np.append(vy1, vy1e)
@@ -73,49 +74,49 @@
         y2     = np.append(y2,y2e)
         z2     = np.append(z2,z2e)
         mass2  = np.append(mass2, mass2e)
         vx2    = np.append(vx2, vx2e)
         vy2    = np.append(vy2, vy2e)
         vz2    = np.append(vz2, vz2e)
         maccr2 = np.append(maccr2, maccr2e)
-        
+
         if setup['triple_star']==True:
             t3     = np.append(t3,t3e)
             x3     = np.append(x3,x3e)
             y3     = np.append(y3,y3e)
             z3     = np.append(z3,z3e)
             mass3  = np.append(mass3, mass3e)
             vx3    = np.append(vx3, vx3e)
             vy3    = np.append(vy3, vy3e)
             vz3    = np.append(vz3, vz3e)
             maccr3 = np.append(maccr3, maccr3e)
 
-        
+
 
 
     # AGB star
 
-    t1     = t1     *  cgs.cu_time()                   # evolution time             [yrs]                                
+    t1     = t1     *  cgs.cu_time()                   # evolution time             [yrs]
     x1     = x1     *  cgs.au                          # position coordinates       [cm]
     y1     = y1     *  cgs.au
     z1     = z1     *  cgs.au
     mass1  = mass1  *  cgs.Msun                        # mass of sph particles      [g]
     vx1    = vx1    *  cgs.cu_vel()                    # velocity components        [cm/s]
     vy1    = vy1    *  cgs.cu_vel()
     vz1    = vz1    *  cgs.cu_vel()
     maccr1 = maccr1 *  cgs.Msun                        # accreted mass              [g]
 
     r1 = gf.calc_r(x1, y1, z1)                         # [cm]
 
     position1 = np.array((x1, y1, z1 )).transpose()
     velocity1 = np.array((vx1,vy1,vz1)).transpose()
-    
+
     # companion star
 
-    t2     = t2     *  cgs.cu_time()                   # evolution time             [yrs]                                 
+    t2     = t2     *  cgs.cu_time()                   # evolution time             [yrs]
     x2     = x2     *  cgs.au                          # position coordinates       [cm]
     y2     = y2     *  cgs.au
     z2     = z2     *  cgs.au
     mass2  = mass2  *  cgs.Msun                        # mass of sph particles      [g]
     vx2    = vx2    *  cgs.cu_vel()                    # velocity components        [cm/s]
     vy2    = vy2    *  cgs.cu_vel()
     vz2    = vz2    *  cgs.cu_vel()
@@ -124,61 +125,61 @@
     r2 = gf.calc_r(x2, y2, z2)                         # [cm]
 
     position2 = np.array((x2, y2, z2 )).transpose()
     velocity2 = np.array((vx2,vy2,vz2)).transpose()
 
     if setup['triple_star']==True:
         #close companion star
-        t3     = t3     *  cgs.cu_time()                   # evolution time             [yrs]                                 
+        t3     = t3     *  cgs.cu_time()                   # evolution time             [yrs]
         x3     = x3     *  cgs.au                          # position coordinates       [cm]
         y3     = y3     *  cgs.au
         z3     = z3     *  cgs.au
         mass3  = mass3  *  cgs.Msun                        # mass of sph particles      [g]
         vx3    = vx3    *  cgs.cu_vel()                    # velocity components        [cm/s]
         vy3    = vy3    *  cgs.cu_vel()
         vz3    = vz3    *  cgs.cu_vel()
         maccr3 = maccr3 *  cgs.Msun                        # accreted mass              [g]
 
         r3 = gf.calc_r(x3, y3, z3)                         # [cm]
 
         position3 = np.array((x3, y3, z3 )).transpose()
         velocity3 = np.array((vx3,vy3,vz3)).transpose()
-        
+
         period_in       = pq.getPeriod(mass1, mass3, (r1 + r3) /cgs.au )
         rHill_in        = pq.getRHill( abs(r1 + r3), mass3, mass1      )              # [cm]
 
-    
-    
-    
-    # orbital information 
+
+
+
+    # orbital information
     # NOT CORRECT!!!
     #period          = pq.getPeriod(mass1, mass2, setup['sma_ini'] )
-    
+
     #print('period 1',period)
     #print('period 2',setup['period'])
     #periodFixed = setup['period']
     #ONLY ORBITAL VEL OF OUTER COMPANION WILL BE CORRECT IN CASE OF TRIPLE, INNER HAS COMPLICATED ORBITAL VELOCITY
     #orbitalVel_AGB  = pq.getOrbitalVelocity(period, r1     /cgs.au_cm() )
     #orbitalVel_comp = pq.getOrbitalVelocity(period, r2     /cgs.au_cm() )
     #orbotalVel_comp_in = pq.getOrbitalVelocity(period_in, r3     /cgs.au_cm() )
-    
-    orbitalVel_AGB  = np.sqrt(np.transpose(velocity1)[0]**2+np.transpose(velocity1)[1]**2) 
+
+    orbitalVel_AGB  = np.sqrt(np.transpose(velocity1)[0]**2+np.transpose(velocity1)[1]**2)
     orbitalVel_comp = np.sqrt(np.transpose(velocity2)[0]**2+np.transpose(velocity2)[1]**2)
     if setup['triple_star']==True:
         orbitalVel_comp_in = np.sqrt(np.transpose(velocity3)[0]**2+np.transpose(velocity3)[1]**2)
-        
-        
-        
+
+
+
     rHill           = pq.getRHill( abs(r1 + r2), mass2, mass1           )         # [cm]
-    
+
     #print('test orbital velocity:')
     #print(np.shape(np.linalg.norm(np.transpose(velocity1))),np.shape(orbitalVel_AGB))
     #print(np.nanmean(np.linalg.norm(np.transpose(velocity1))),np.nanmean(orbitalVel_AGB))
     #print(np.array(np.linalg.norm(velocity1))[0:20],orbitalVel_AGB[0:20])
-    
+
     # output
     #    "_t" stands for the fact that these values are in function of the evolution time, not from the last dump in function of location
     if setup['triple_star']==True:
         data = {'posAGB'      : position1,              # [cm]
                 'velAGB'      : velocity1,              # [cm/s]
                 'massAGB'     : mass1,                  # [gram]
                 'maccrAGB'    : maccr1,                 # [gram]
@@ -213,23 +214,23 @@
                 'massComp'    : mass2,
                 'maccrComp'   : maccr2,
                 'rComp'       : r2,
                 'time'        : t1,                     # [yrs]
                 #'period_t'    : period,                 # [s]
                 'v_orbAGB_t'  : orbitalVel_AGB,         # [cm/s]
                 'v_orbComp_t' : orbitalVel_comp,        # [cm/s]
-                'rHill_t'     : rHill                  # [cm] 
+                'rHill_t'     : rHill                  # [cm]
                 }
-        
+
     #print(np.shape(data['velAGB']))
     #print(np.shape(data['velAGB'][0]))
     #print(np.shape(np.transpose(data['velAGB'])[0]))
 
     return data
-        
+
 
 
 
 
 
 '''
 Load the .ev-files from a phantom model of a SINGLE star
@@ -244,59 +245,58 @@
     userPrefix = userSettingsDictionary["prefix"]
     fileName = os.path.join(runName, '%sSink0001N01.ev'%userPrefix)
 
     # load the dump file prefix_00xxx
     t1, x1, y1, z1, mass1, vx1, vy1, vz1, maccr1 = 0, 0, 0, 0, 0, 0, 0, 0, 0
     try:
        (t1, x1,y1,z1, mass1, vx1,vy1,vz1, maccr1) = np.loadtxt(fileName, skiprows=1, usecols=(0,1,2,3,4,5,6,7,11), unpack=True)
-        
+
 
     except OSError:
 
         print(' ERROR: No sink file found for this model in the current directory!')
         sys.exit()
 
 
     # AGB star
 
-    t1     = t1     *  cgs.cu_time()                   # evolution time             [yrs]                            
+    t1     = t1     *  cgs.cu_time()                   # evolution time             [yrs]
     x1     = x1     *  cgs.au                          # position coordinates       [cm]
     y1     = y1     *  cgs.au
     z1     = z1     *  cgs.au
     mass1  = mass1  *  cgs.Msun                        # mass of sph particles      [g]
     vx1    = vx1    *  cgs.cu_vel()                    # velocity components        [cm/s]
     vy1    = vy1    *  cgs.cu_vel()
     vz1    = vz1    *  cgs.cu_vel()
     maccr1 = maccr1 *  cgs.Msun                        # accreted mass              [g]
 
     r1 = gf.calc_r(x1, y1, z1)                         # [cm]
 
     position1 = np.array((x1, y1, z1 )).transpose()
     velocity1 = np.array((vx1,vy1,vz1)).transpose()
-    
-    
-    
+
+
+
     data = {'posAGB'      : position1,       # [cm]
             'velAGB'      : velocity1,       # [cm/s]
             'massAGB'     : mass1,           # [gram]
             'maccrAGB'    : maccr1,          # [gram]
             'rAGB'        : r1,              # [cm]
             'time'        : t1,              # [yrs]
             }
-    
+
     return data
 
 
 
 # Pick last wind evolution file
-def findLastWindSinkIndex(runName):
-    listevFiles = sortedWindSinkList('windSink0001N0', runName)
+def findLastWindSinkIndex(runName,userPrefix):
+    listevFiles = sortedWindSinkList(userPrefix+'Sink0001N0', runName)
     lastFile = listevFiles[-1]
-    t1 = lastFile.lstrip("windSink0001")
+    t1 = lastFile.lstrip(userPrefix+'Sink0001')
     t2 = t1.lstrip("N")
     t3 = t2.rstrip(".ev")
     lastIndex = int(t3)
     return lastIndex
 
 def sortedWindSinkList(userPrefix, runName):
     return np.sort(list(filter(lambda x: ("%s"%userPrefix in x) and (".ev" in x), os.listdir(runName))))
-
```

### Comparing `plons-0.0.7/src/plons/OrbitalEvolution.py` & `plons-0.0.9/src/plons/OrbitalEvolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Import packages
 import numpy                    as np
 import matplotlib.pyplot        as plt
 import matplotlib.lines         as mlines
 import math                     as math
-from scipy.signal import argrelextrema,find_peaks
+from scipy.signal               import argrelextrema
 
 import os
 from matplotlib                 import rcParams, rc
 # Change the matplotlib default parameters
 rcParams.update({'font.size' :   12})
 rcParams.update({'figure.dpi': 200})
 #rc('font', family='serif')
 #rc('text', usetex=True)
 
-# import own scripts
-import ConversionFactors_cgs    as cgs
-import PhysicalQuantities       as pq
-import Tools                    as tl
-
+# import plons scripts
+import plons.ConversionFactors_cgs    as cgs
+import plons.PhysicalQuantities       as pq
+import plons.Tools                    as tl
 
 '''
 Visualises the orbit of the system
 Uses sinkData = data
 '''
 def plot_orbit(data, setup,loc): 
     
@@ -34,49 +33,45 @@
     yc = data['posComp'].transpose()[1]
     ya = data['posAGB' ].transpose()[1]
     #zc = data['posComp'].transpose()[2]
     #za = data['posAGB' ].transpose()[2]
     
     M1   = data['massComp']
     M2   = data['massAGB' ]
-    
-    ax.axis('equal')
-    ax.set_ylim(-4,4)
-    
+        
     if setup['triple_star']==True:
         xc_in = data['posComp_in'].transpose()[0] 
         yc_in = data['posComp_in'].transpose()[1] 
         #zc_in = data['posComp_in'].transpose()[2] 
         M_in  = data['massComp_in']
         #CoM
         xCOM_in = (M_in*xc_in + M2 * xa)/(M_in+M2)
         yCOM_in = (M_in*yc_in + M2 * ya)/(M_in+M2)
         MCOM_in = M_in + M2
         xCOM_out = ( MCOM_in*xCOM_in + M1 *xc)/(MCOM_in+M1)
         yCOM_out = ( MCOM_in*yCOM_in + M1 *yc)/(MCOM_in+M1)
-        ax.plot(xCOM_in/cgs.au,yCOM_in/cgs.au, color = 'k', label = 'CoM_inner')
-        ax.plot(xCOM_out/cgs.au,yCOM_out/cgs.au,'*', color = 'k', label = 'CoM_outer', markersize = 5)
-        ax.plot(xc_in[1:]/cgs.au,yc_in[1:]/cgs.au, c = 'g', label = 'inner comp')
-        ax.plot(xc[1:]/cgs.au,yc[1:]/cgs.au, c = 'r', label = 'outer comp')
+        ax.plot(xCOM_in/cgs.au,yCOM_in/cgs.au, color = 'navy', label = 'CoM_inner')
+        ax.plot(xCOM_out/cgs.au,yCOM_out/cgs.au,'*', color = 'navy', label = 'CoM_outer', markersize = 5)
+        ax.plot(xc_in[1:]/cgs.au,yc_in[1:]/cgs.au, c = 'lime', label = 'inner comp')
+        ax.plot(xc[1:]/cgs.au,yc[1:]/cgs.au, c = 'crimson', label = 'outer comp')
         #  #FOR SCIENTIST@SCHOOL
-        #ax.set_facecolor('k')
+        #ax.set_facecolor('navy')
         #ax.plot(xCOM_in/cgs.au,yCOM_in/cgs.au, color = 'white')#, label = 'MM')
         #ax.plot(xCOM_out/cgs.au,yCOM_out/cgs.au,'*', color = 'white')#, label = 'MM', markersize = 5)
         #ax.plot(xc_in[1:]/cgs.au,yc_in[1:]/cgs.au, c = 'yellow')#, label = 'S2')
         #ax.plot(xc[1:]/cgs.au,yc[1:]/cgs.au, c = 'yellow')#, label = 'S3')
 
     else:
         xCOM = (M1*xc + M2 * xa)/(M1+M2)
         yCOM = (M1*yc + M2 * ya)/(M1+M2)
         #rCOM = np.sqrt(xCOM**2 + yCOM**2)
-        ax.plot(xCOM/cgs.au,yCOM/cgs.au,'*', color = 'k', label = 'CoM')
-        ax.plot(xc[1:]/cgs.au,yc[1:]/cgs.au, c = 'r', label = 'companion')
+        ax.plot(xCOM/cgs.au,yCOM/cgs.au,'*', color = 'navy', label = 'CoM')
+        ax.plot(xc[1:]/cgs.au,yc[1:]/cgs.au, c = 'crimson', label = 'companion')
     
-
-    ax.plot(xa[1:]/cgs.au,ya[1:]/cgs.au, c = 'b', label = 'AGB'      )
+    ax.plot(xa[1:]/cgs.au,ya[1:]/cgs.au, c = 'gold', label = 'AGB'      )
     ax.set_ylabel('$y$ [au]',fontsize = 15)
     ax.set_xlabel('$x$ [au]',fontsize = 15)
     ax.set_title('$e = $'+str(setup['ecc'])+', $a = $'+ str(setup['sma_ini'])+' AU, $q = $'+ str(setup['massAGB_ini']/setup['massComp_ini']), fontsize = 15)
     ax.tick_params(labelsize=12)
     ax.axis('equal')
     ax.legend(fontsize = 15, loc = 'lower right')
     fig.tight_layout()
@@ -136,23 +131,23 @@
     fig, (ax1)= plt.subplots(1, 1,  gridspec_kw={'height_ratios':[1],'width_ratios': [1]})
     fig.set_size_inches(7, 5)
     #Calculate orbital separation and time at apastron and periastron 
     [apastronOS, periastronOS, timeApa, timePer] = orbSep_apa_per(sinkData, setup) 
     
     ax1.set_xlabel('time [yrs]', fontsize = 16)
     # Plot the apastron orbital separations
-    colorA = 'tab:red'
+    colorA = 'crimson'
     ax1.plot(timeApa,apastronOS/cgs.au, c=colorA, marker= '$*$', linestyle = 'dashed', markersize = 10)
     ax1.vlines(timeApa, 0.99*np.min(apastronOS)/cgs.au,1.01*np.max(apastronOS)/cgs.au, linestyle = 'dotted',color=colorA , linewidth = 0.5)   
     ax1.tick_params(axis='y',labelsize=12, labelcolor = colorA)     
     ax1.set_ylabel('Apastron orb sep [au]', fontsize = 16, color=colorA)
     #add second yaxis
     ax2 = ax1.twinx()
     # Plot the apastron orbital separations
-    colorP = 'tab:blue'
+    colorP = 'navy'
     ax2.plot(timePer,periastronOS/cgs.au, c=colorP, marker = '$*$', linestyle = 'dashed', markersize = 10)
     ax2.vlines(timePer, 0.99*np.min(periastronOS)/cgs.au,1.01*np.max(periastronOS)/cgs.au, linestyle = 'dotted',color=colorP , linewidth = 0.5)   
     ax2.set_ylabel('Periastron orb sep [au]', fontsize = 16, color=colorP)
     ax2.tick_params(axis='y',labelsize=12, labelcolor = colorP)     
     ax1.set_title('Evolution apastron and periastron separation')
     fig.tight_layout()
     plt.savefig(os.path.join(loc, 'pdf/evolution_ApaPer.pdf'))
@@ -184,16 +179,16 @@
         ind.append(i)
     
     # Estimate period using the estimate of a [au], and the masses of the AGB and companion [gram] at these times t
     est_p     = pq.getPeriod(sinkData['massAGB'][ind], sinkData['massComp'][ind], est_a/cgs.au )/cgs.year
     
     # Make plot of orbital period, and add linear line for visualisation 
     fig_p, ((ax_p))= plt.subplots(1, 1,  gridspec_kw={'height_ratios':[1],'width_ratios': [1]})
-    ax_p.plot(t, est_p, label = 'orbital period',marker= '$*$', linestyle = 'dashed', markersize = 10)
-    ax_p.plot([t[0],t[-1]],[est_p[0],est_p[-1]],'--',label='linear')
+    ax_p.plot(t, est_p, label = 'orbital period',marker= '$*$', linestyle = 'solid', color = 'navy',markersize = 10)
+    ax_p.plot([t[0],t[-1]],[est_p[0],est_p[-1]],'--',label='linear',color ='navy',linestyle='dashed',linewidth = 0.8)
     ax_p.set_ylabel('estimate orbital period [yrs]', fontsize = 12)
     ax_p.set_xlabel('time[yrs]', fontsize = 10)
     ax_p.tick_params(labelsize=10)
     ax_p.grid(which='both')
     plt.title('Orbital Period', fontsize = 15)
     plt.legend()
     fig_p.tight_layout()
@@ -202,22 +197,22 @@
     plt.close
 
     #Make plot of estimates of a and e
     fig, (ax1)= plt.subplots(1, 1,  gridspec_kw={'height_ratios':[1],'width_ratios': [1]})
     fig.set_size_inches(7, 5)
     ax1.set_xlabel('time [yrs]', fontsize = 16)
     # Plot the estimates of a
-    color_a = 'tab:red'
+    color_a = 'crimson'
     ax1.plot(t,est_a/cgs.au, c=color_a, marker= '$*$', linestyle = 'dashed', markersize = 10)
     ax1.vlines(t, 0.99*np.min(est_a)/cgs.au,1.01*np.max(est_a)/cgs.au, linestyle = 'dotted',color=color_a , linewidth = 0.5)   
     ax1.tick_params(axis='y',labelsize=12, labelcolor = color_a)     
     ax1.set_ylabel('estimate semi-major axis [au]', fontsize = 16, color=color_a)
     # Plot the estimates of e, with seperate y-axis    
     ax2 = ax1.twinx()
-    color_e = 'tab:blue'
+    color_e = 'navy'
     ax2.plot(t,est_e, c=color_e, marker = '$*$', linestyle = 'dashed', markersize = 10)
     ax2.vlines(t, 0.99*np.min(est_e),1.01*np.max(est_e), linestyle = 'dotted',color=color_e , linewidth = 0.5)   
     ax2.set_ylabel('estimate eccentricity', fontsize = 16, color=color_e)
     ax2.tick_params(axis='y',labelsize=12, labelcolor = color_e)     
     ax1.set_title('Evolution semi-major axis and eccentricity')
     fig.tight_layout()
     plt.savefig(os.path.join(loc, 'pdf/evolution_a_e.pdf'))
@@ -227,24 +222,24 @@
 '''
 Makes plot of the evolution of mass accretion by the companion
 '''
 def plotMassAccr(setup, sinkData, run, loc):
     # Make plot of the mass accretion evolution, very interesting to plot!
     fig = plt.figure(figsize=(8, 5))
     # Legend
-    apaLine       = mlines.Line2D([],[], color = 'k', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
-    perLine       = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
-    periodLine    = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
+    apaLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
+    perLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
+    periodLine    = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
 
     # Plot the accreted mass in function of time
-    plt.plot(sinkData['time'],  sinkData['maccrComp']/cgs.Msun, color = 'royalblue', linestyle = 'solid')
+    plt.plot(sinkData['time'],  sinkData['maccrComp']/cgs.Msun, color = 'crimson', linestyle = 'solid')
     if setup['triple_star']==True:
-        plt.plot(sinkData['time'],  sinkData['maccrComp_in']/cgs.Msun, color = 'red', linestyle = 'solid')
-        comp_out       = mlines.Line2D([],[], color = 'royalblue', linestyle = 'solid', linewidth = 0.5, label = 'outer comp')
-        comp_in        = mlines.Line2D([],[], color = 'r', linestyle = 'solid', linewidth = 0.5, label = 'inner comp')
+        plt.plot(sinkData['time'],  sinkData['maccrComp_in']/cgs.Msun, color = 'lime', linestyle = 'solid')
+        comp_out       = mlines.Line2D([],[], color = 'crimson', linestyle = 'solid', linewidth = 0.5, label = 'outer comp')
+        comp_in        = mlines.Line2D([],[], color = 'lime', linestyle = 'solid', linewidth = 0.5, label = 'inner comp')
         handles_ap    = [periodLine,comp_in,comp_out]
     #else:
         handles_ap    = [apaLine, perLine]
     '''
     # Plot vertical lines indicating where there should be apastron and periastron passages
     period = setup['period'] / cgs.year
     #print('period in years: ',period)
@@ -284,17 +279,17 @@
 Makes plot of the evolution of mass accretion rate by the companion
 returns t_yrs and mass accretion rate to make plot yourself
 '''
 def plotMassAccrRate(setup, sinkData, run, loc):
     # Make plot of the mass accretion evolution, very interesting to plot!
     fig = plt.figure(figsize=(8, 5))
     # Legend
-    apaLine       = mlines.Line2D([],[], color = 'k', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
-    perLine       = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
-    periodLine    = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
+    apaLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
+    perLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
+    periodLine    = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
     
     # Make empty array for accrRates per year
     accrRates    = []
     if setup['triple_star']==True:
         accrRates_in = []
         # Make array with the years
         factor   = 0.5
@@ -317,19 +312,19 @@
         #calculate difference in accreted mass between this and the previous year, to find accretion rate per year in this year
         accrRate = factor*(sinkData['maccrComp'][indices_yrs[-1]]-sinkData['maccrComp'][indices_yrs[-2]])/cgs.Msun
         accrRates.append(accrRate)
         if setup['triple_star']==True:
             accrRate_in = factor*(sinkData['maccrComp_in'][indices_yrs[-1]]-sinkData['maccrComp_in'][indices_yrs[-2]])/cgs.Msun
             accrRates_in.append(accrRate_in)
     
-    plt.plot(t_yrs[:-1], accrRates,color = 'royalblue', linestyle = 'solid')    
+    plt.plot(t_yrs[:-1], accrRates,color = 'crimson', linestyle = 'solid')    
     if setup['triple_star']==True:
-        plt.plot(t_yrs[:-1], accrRates_in,color = 'r', linestyle = 'solid')
-        comp_out       = mlines.Line2D([],[], color = 'royalblue', linestyle = 'solid', linewidth = 0.5, label = 'outer comp')
-        comp_in        = mlines.Line2D([],[], color = 'r', linestyle = 'solid', linewidth = 0.5, label = 'inner comp')
+        plt.plot(t_yrs[:-1], accrRates_in,color = 'lime', linestyle = 'solid')
+        comp_out       = mlines.Line2D([],[], color = 'crimson', linestyle = 'solid', linewidth = 0.5, label = 'outer comp')
+        comp_in        = mlines.Line2D([],[], color = 'lime', linestyle = 'solid', linewidth = 0.5, label = 'inner comp')
         handles_ap    = [periodLine,comp_in,comp_out]
     #else:
         #handles_ap    = [apaLine, perLine]
 
     '''
     # Plot vertical lines indicating where there are apastron and periastron passages
     period = setup['period'] / cgs.year
@@ -372,19 +367,19 @@
 '''
 Makes plot of the evolution of the orbital velocity of the AGB star and companion 
 '''
 def plotOrbVel(setup,sinkData, run, loc):
     fig, ((ax))= plt.subplots(1, 1,  gridspec_kw={'height_ratios':[1],'width_ratios': [1]})
     t    = sinkData['time'][1:]
 
-    ax.plot(t, sinkData['v_orbAGB_t'][1:]/cgs.kms, label = 'AGB')
-    ax.plot(t, sinkData['v_orbComp_t'][1:]/cgs.kms, label ='companion')
+    ax.plot(t, sinkData['v_orbAGB_t'][1:]/cgs.kms, label = 'AGB', c='gold')
+    ax.plot(t, sinkData['v_orbComp_t'][1:]/cgs.kms, label ='companion', c='crimson')
     
     if setup['triple_star']==True:
-        ax.plot(t, sinkData['v_orbComp_in_t'][1:]/cgs.kms, label ='inner companion')
+        ax.plot(t, sinkData['v_orbComp_in_t'][1:]/cgs.kms, label ='inner companion', c='lime')
 
     period = setup['period'] / cgs.year
     i = 0         
     mini = 0
     if setup['triple_star']==True: #(not at apastron at t=0, so difficult)
         maxi = max(np.max(sinkData['v_orbComp_t'][1:]/cgs.kms),np.max(sinkData['v_orbComp_in_t'][1:]/cgs.kms))
         for orbit in range(0, int(sinkData['time'][-1]/period)+1):
@@ -424,38 +419,38 @@
     fig, (ax)= plt.subplots(1, 1,  gridspec_kw={'height_ratios':[1],'width_ratios': [1]})
 
     ax.set_ylabel('$r$ [au]', fontsize = 12)
     ax.set_title('orbital radii', fontsize = 15)
     ra   = sinkData['rAGB'][1:] /cgs.au
     t    = sinkData['time'][1:]
     
-    ax.plot(t, ra, label ='r AGB')
+    ax.plot(t, ra, label ='r AGB', c='gold')
     if setup['triple_star']==True:
         rc_in  = sinkData['rComp_in'][1:] /cgs.au
         rc_out = sinkData['rComp'][1:] /cgs.au
-        ax.plot(t, rc_out, label= 'r outer comp')
-        ax.plot(t, rc_in, label= 'r inner comp')
+        ax.plot(t, rc_out, label= 'r outer comp',c='crimson')
+        ax.plot(t, rc_in, label= 'r inner comp',c='lime')
         
         Mc    = sinkData['massComp'][1:]
         Ma    = sinkData['massAGB' ][1:]
         Mc_in = sinkData['massComp_in'][1:]
         #CoM
         rCOM_in = (Mc_in*rc_in + Ma *ra )/(Mc_in+Ma)
-        ax.plot(t, rCOM_in+rc_out, label = 'Orb sep outer')
+        ax.plot(t, rCOM_in+rc_out, label = 'Orb sep outer',c='navy')
  
         #ax.plot(sinkData['time'], sinkData['rAGB']+sinkData['rComp'], label = 'Orb sep')
     else:
-        ax.plot(t, sinkData['rComp'][1:]/cgs.au, label= 'r comp')
-        ax.plot(t, ra +sinkData['rComp'][1:]/cgs.au, label = 'Orb sep')
+        ax.plot(t, sinkData['rComp'][1:]/cgs.au, label= 'r comp', c='crimson')
+        ax.plot(t, ra +sinkData['rComp'][1:]/cgs.au, label = 'Orb sep', c='navy')
     '''        
     # Plot vertical lines indicating where there should be apastron and periastron passages
     # Legend
-    apaLine       = mlines.Line2D([],[], color = 'k', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
-    perLine       = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
-    periodLine    = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
+    apaLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
+    perLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
+    periodLine    = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
     period = setup['period'] / cgs.year
     #print('period in years: ',period)
     i = 0         # Start at apastron
     mini = 0
     if setup['triple_star']==True: #(not at apastron at t=0, so difficult)
         maxi = np.max(rCOM_in+rc_out)
         for orbit in range(0, int(sinkData['time'][-1]/period)+1):
@@ -500,49 +495,49 @@
     t    = sinkData['time'][1:]
     
     if setup['triple_star']==True:
         ax1 = axs[0][0]
         ax2 = axs[0][1]
         ax3 = axs[1][0]
         ax4 = axs[1][1]
-        ax1.plot(t, ra, label ='r AGB')
+        ax1.plot(t, ra, label ='r AGB',c='gold')
         ax1.set_ylabel('rAGB [au]', fontsize = 12)
         rc_in  = sinkData['rComp_in'][1:] /cgs.au
         rc_out = sinkData['rComp'][1:] /cgs.au
-        ax2.plot(t, rc_out, label= 'r outer comp')
+        ax2.plot(t, rc_out, label= 'r outer comp',c='crimson')
         ax2.set_ylabel('r out comp [au]', fontsize = 12)
-        ax3.plot(t, rc_in, label= 'r inner comp')
+        ax3.plot(t, rc_in, label= 'r inner comp',c='lime')
         ax3.set_ylabel('r inn comp [au]', fontsize = 12)        
         
         Mc    = sinkData['massComp'][1:]
         Ma    = sinkData['massAGB' ][1:]
         Mc_in = sinkData['massComp_in'][1:]
         #CoM
         rCOM_in = (Mc_in*rc_in + Ma *ra )/(Mc_in+Ma)
 
-        ax4.plot(t, rCOM_in+rc_out, label = 'Orb sep outer')
+        ax4.plot(t, rCOM_in+rc_out, label = 'Orb sep outer',c='navy')
         ax4.set_ylabel('orb sep outer [au]', fontsize = 12)  
         
     else:
         ax1 = axs[0]
         ax2 = axs[1]
         ax3 = axs[2]
-        ax1.plot(t, ra, label ='r AGB')
+        ax1.plot(t, ra, label ='r AGB',c='gold')
         ax1.set_ylabel('rAGB [au]', fontsize = 12)
         ax2.set_ylabel('r comp [au]', fontsize = 12)
-        ax2.plot(t, sinkData['rComp'][1:]/cgs.au, label= 'r comp')
+        ax2.plot(t, sinkData['rComp'][1:]/cgs.au, label= 'r comp',c='crimson')
         ax3.set_ylabel('Orb Sep [au]', fontsize = 12)
-        ax3.plot(t, ra +sinkData['rComp'][1:]/cgs.au, label = 'Orb sep')
+        ax3.plot(t, ra +sinkData['rComp'][1:]/cgs.au, label = 'Orb sep',c='navy')
  
     '''
     # Plot vertical lines indicating where there should be apastron and periastron passages
     # Legend
-    #apaLine       = mlines.Line2D([],[], color = 'k', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
-    #perLine       = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
-    #periodLine    = mlines.Line2D([],[], color = 'k', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
+    #apaLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'solid', linewidth = 0.5, label = 'Apastron')
+    #perLine       = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'Periastron')
+    #periodLine    = mlines.Line2D([],[], color = 'navy', linestyle = 'dotted', linewidth = 0.5, label = 'orbital period')
     period = setup['period'] / cgs.year
     i = 0         # Start at apastron
     mini = 0
     if setup['triple_star']==True: #(not at apastron at t=0, so difficult)
         maxi = np.max(rCOM_in+rc_out)
         for orbit in range(0, int(sinkData['time'][-1]/period)+1):
             ax1.vlines(i,mini, maxi,  linestyle = 'dotted' , linewidth = 0.5)
```

### Comparing `plons-0.0.7/src/plons/PhysicalQuantities.py` & `plons-0.0.9/src/plons/PhysicalQuantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import math                     as math
 import numpy                    as np
-import ConversionFactors_cgs    as cgs
-import GeometricalFunctions     as gf
+
+#import plons scripts
+import plons.ConversionFactors_cgs    as cgs
+import plons.GeometricalFunctions     as gf
 
 
 # --- Physical Quantities in cgs ---
 
 '''
 Returns the pressure of a particle, given by the specific internal energy u [erg/g], gamma and density [g/cm^3] in 10^-1 Pa = barye = Ba = g cm^-1 s^-2
 '''
```

### Comparing `plons-0.0.7/src/plons/Profiles1D.py` & `plons-0.0.9/src/plons/Profiles1D.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 @author: Ward Homan, Lionel Siess
 
 Make sure that the path in the sys.append points to the scripts directory of phantom
 """
 import matplotlib.pyplot as plt
 from numpy import *
 from scipy import constants, interpolate
-import userSettings as us
 import os
 import sys
-from ConversionFactors_cgs import Rg, steboltz, kB, au, G, mH, Msun
+from plons.ConversionFactors_cgs import Rg, steboltz, kB, au, G, mH, Msun
 
 # reads the 1D data and computes derived quantities
 def read1D(runName, setup):
     # Read the 1D data
     f       = open(os.path.join(runName,'wind_1D.dat'),'r')
     headers = f.readline()
     headers = headers.split()[0:]
```

### Comparing `plons-0.0.7/src/plons/RadialStructurePlots1D.py` & `plons-0.0.9/src/plons/RadialStructurePlots1D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import numpy                    as np
 import matplotlib.pyplot        as plt
-import matplotlib.lines         as mlines
 import os
 
-# import own scripts
+# import plons scripts
 import plons.SmoothingKernelScript    as sk
 import plons.ConversionFactors_cgs    as cgs
 import plons.PhysicalQuantities       as pq
-import plons.SlicePlots2D             as sp
 
 # import certain things from packages
-from matplotlib                 import colors
-from astropy                    import constants
-from mpl_toolkits.axes_grid1    import AxesGrid
-from matplotlib                 import rcParams, rc
 from matplotlib.ticker          import MultipleLocator
 
 # ignore warnings
 import warnings
 warnings.filterwarnings("ignore")
 
 n_grid = 10000
```

### Comparing `plons-0.0.7/src/plons/RhoRradialFit.py` & `plons-0.0.9/src/plons/RhoRradialFit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import numpy                    as np
 import matplotlib.pyplot        as plt
-import matplotlib.lines         as mlines
 import os
 
-# import own scripts
-import SmoothingKernelScript    as sk
-import ConversionFactors_cgs    as cgs
-import PhysicalQuantities       as pq
+# import plons scripts
+import plons.ConversionFactors_cgs    as cgs
+import plons.PhysicalQuantities       as pq
 
 # import certain things from packages
 from scipy.optimize             import curve_fit
-from matplotlib                 import colors
-from astropy                    import constants
-from mpl_toolkits.axes_grid1    import AxesGrid
-from matplotlib                 import rcParams, rc
+from matplotlib                 import rcParams
 # Change the matplotlib default parameters
 rcParams.update({'font.size':   11})
 rcParams.update({'figure.dpi': 200})
 #rc('font', family='serif')
 #rc('text', usetex=True)
 
 # ignore warnings
```

### Comparing `plons-0.0.7/src/plons/SlicePlots2D.py` & `plons-0.0.9/src/plons/SlicePlots2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 #Import packages
 import numpy                    as np
 import matplotlib.pyplot        as plt
 import os
 import math
 
-# import own scripts
-import SmoothingKernelScript    as sk
-import ConversionFactors_cgs    as cgs
-import PhysicalQuantities       as pq
-import ArchimedianSpiral        as ars
+# import plons scripts
+import plons.SmoothingKernelScript    as sk
+import plons.ConversionFactors_cgs    as cgs
+import plons.PhysicalQuantities       as pq
+import plons.ArchimedianSpiral        as ars
 
 # import certain things from packages
-from matplotlib                 import colors
-from astropy                    import constants
-from mpl_toolkits.axes_grid1    import AxesGrid
-
-from matplotlib                 import rcParams, rc
 from mpl_toolkits.axes_grid1    import make_axes_locatable
 from matplotlib.ticker          import MultipleLocator
 import matplotlib
 matplotlib.use("Agg")
 
 #rc('font', family='serif')
 #rc('text', usetex=True)
```

### Comparing `plons-0.0.7/src/plons/SmoothingKernelScript.py` & `plons-0.0.9/src/plons/SmoothingKernelScript.py`

 * *Files identical despite different names*

### Comparing `plons-0.0.7/src/plons/TerminalVelocity.py` & `plons-0.0.9/src/plons/TerminalVelocity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import math                     as math
 import numpy                    as np
-# own scripts
-import ConversionFactors_cgs    as cgs
-import GeometricalFunctions     as gf
-import Tools                    as tl
-import PhysicalQuantities       as pq
+
+# import plons scripts
+import plons.ConversionFactors_cgs    as cgs
+import plons.GeometricalFunctions     as gf
+import plons.Tools                    as tl
+import plons.PhysicalQuantities       as pq
 # ignore warnings
 import warnings
 warnings.filterwarnings("ignore")
```

### Comparing `plons-0.0.7/src/plons/Tools.py` & `plons-0.0.9/src/plons/Tools.py`

 * *Files identical despite different names*

### Comparing `plons-0.0.7/src/plons/Tubes.py` & `plons-0.0.9/src/plons/Tubes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import math                     as math
 import numpy                    as np
 import matplotlib.pyplot        as plt
 # own scripts
-import ConversionFactors_cgs    as cgs
-import GeometricalFunctions     as gf
-import Tools                    as tl
-import PhysicalQuantities       as pq
+import plons.ConversionFactors_cgs    as cgs
+import plons.GeometricalFunctions     as gf
+import plons.Tools                    as tl
 # ignore warnings
 import warnings
 warnings.filterwarnings("ignore")
 
 
 '''
 Double bin in a dataset 'rho' according to two sets (so in 2D):
```

### Comparing `plons-0.0.7/src/plons/main.py` & `plons-0.0.9/src/plons/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import numpy                        as np
 import sys
 import os
 import warnings
 warnings.filterwarnings("ignore")
 import argparse                     as ap
 
-# own scripts
+# import plons scripts
 import plons.RadialStructurePlots1D       as rs
 import plons.SlicePlots2D                 as sl
 import plons.CMF_meanRho                  as cmf
 import plons.OrbitalEvolution             as ov
 import plons.LoadDataPHANTOM              as ld
 import plons.TerminalVelocity             as tmv
-import plons.Tubes                        as tb
 import plons.Profiles1D                   as dp
 import plons.userSettings                 as us
 import plons.ArchimedianSpiral            as ars
 
 #print('------------------START:', dt.datetime.now(),'---------------------')
 print('')
 
@@ -128,18 +127,18 @@
     if part == '7':
         print('')
         print('(7)  Archimedian spiral')
         ars.ArchimedianSpiral(run, saveloc, setup)
 
 print('')
 print('-------------------------------------------------------')
-print('     Welcome to the very first PHANTOM pipeline!'        )
+print('     Welcome to PLONS!'        )
 print('-------------------------------------------------------')
 print('')
-print('This pipeline reduces PHANTOM output to usable plots and datasets.')
+print('The PLOtting tool for Nice Simulations.')
 print('')
 
 
 # Initialise user settings or load them
 userSettingsFilePath = os.path.join( os.getcwd(), "userSettings.txt")
 if not os.path.isfile(userSettingsFilePath) or os.stat(userSettingsFilePath).st_size == 0: us.create(userSettingsFilePath)
```

### Comparing `plons-0.0.7/src/plons/profile_1D_spherical_model.py` & `plons-0.0.9/src/plons/profile_1D_spherical_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Make sure that the path in the sys.append points to the scripts directory of phantom
 """
 
 
 import matplotlib.pyplot as plt
 from numpy import *
 from scipy import constants, interpolate
-import userSettings as us
+import plons.userSettings as us
 import os
 import sys
 
 userSettingsFilePath = os.path.join( os.getcwd(), "userSettings.txt")
 if not os.path.isfile(userSettingsFilePath) or os.stat(userSettingsFilePath).st_size == 0: us.create(userSettingsFilePath)
 userSettingsDictionary = us.load(userSettingsFilePath,onlyPathToPhantom=True)
 sys.path.append(userSettingsDictionary["hard_path_to_phantom"]+'/scripts')
```

### Comparing `plons-0.0.7/src/plons/userSettings.py` & `plons-0.0.9/src/plons/userSettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,17 @@
                 continue
             break
 
         if (phantom[-1] == '/' or phantom[-1] == '\\'):
             phantom = phantom[:-1]
 
         file.write("prefix = " + prefix + "\n")
-        file.write("data_location = " + loc + "\n")
-        file.write("pipeline_output_location = " + outputloc + "\n")
-        file.write("hard_path_to_phantom = " + phantom + "\n")
+        file.write("data_location = " + loc + "/ \n")
+        file.write("pipeline_output_location = " + outputloc + " \n")
+        file.write("hard_path_to_phantom = " + phantom + " \n")
         print("Settings saved at " + userSettingsFilePath)
         print("--------------------------------------------------------------")
         file.close()
 
 # Load userSettingsFile.txt if it exists
 def load(userSettingsFilePath,onlyPathToPhantom=False):
     dictionary = {}
```

### Comparing `plons-0.0.7/src/plons.egg-info/PKG-INFO` & `plons-0.0.9/src/plons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plons
-Version: 0.0.7
+Version: 0.0.9
 Summary: PLOtting tool for Nice Simulations
 Author-email: Jolien Malfait <jolien.malfait@kuleuven.be>, Mats Esseldeurs <mats.esseldeurs@kuleuven.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,113 +690,101 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 
 
 
 -------------------------------
-    README PHANTOM PIPELINE 
+    README PLONS
 -------------------------------
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/build-and-test.yaml/badge.svg)
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/upload-to-pypi.yaml/badge.svg)
 ![Build status](https://github.com/Ensor-code/plons/actions/workflows/upload-to-anaconda.yaml/badge.svg)
 
 
-This is the README for the first python pipeline ever to reduce data of hydrodynamical 
-simulations by use of the SPH code PHANTOM (Price, D. J., Wurster, J., Tricco, T. S., 
-et al. 2018, PASA, 35, e031). PHANTOM returns different types of useful data files: 
-'wind_xxxxx'-files and '.ev'-files. The former can only be read in its raw form by the 
-SPH visualisation tool SPLASH (Price, D. J. 2007, PASA, 24, 159; 
-https://users.monash.edu.au/~dprice/splash/). By using SPLASH, the files can be converted 
-to .ascii to use for reduction. The .ev-files can be use straight away, but can also be 
-visualised using SPLASH.
+This is the README for the PLONS PLOtting tool for Nice Simulations. It can be used to
+read in and analyse data of hydrodynamical simulations with the SPH code PHANTOM 
+(Price, D. J., Wurster, J., Tricco, T. S., et al. 2018, PASA, 35, e031). PHANTOM returns 
+(different types of useful data files: 'wind_xxxxx'-files and '.ev'-files. The former can
+also be visualised by the SPH visualisation tool SPLASH (Price, D. J. 2007, PASA, 24, 159; 
+https://users.monash.edu.au/~dprice/splash/), and can be analysed more toroughly with PLONS.
+
 
 PHANTOM
 -------
 
 PHANTOM returns (full) dump files every certain timestep during the evolution of the 
 model. These are the wind_xxxxx-files and contain the relevant data (position, velocity, 
 mass, density, energy, temperature) of the SPH particles in the model. The last x rows of 
 the output are the x sink particles in the model. More detailed information of the sink 
 particles (position, velocity, mass, accreted mass, spin, angular momentum) in function of 
 evolution time of the model, can be retrieved in the .ev files.
 
-Pipeline - General
+PLONS - General
 ------------------
 
-This pipeline is suited for binary and single AGB wind models.
+This pipeline is suited for single, binary and triple AGB wind models.
+
+The following info can be attained:
+
+(1) 2D slice plots of the global structure of the last dump full of the model.
+(2) 1D line plots (radial structure) of the global structure of the last dump of the model along the x-, y- and z-axes.
+(3) Information about the velocity related quantities of the model + Quantitative measurement of the degree of aspherical morphology: morphological parameters eta, Qp and epsilon.
+(4) Cummulative mass fraction in function of the polar coordinate theta.
+(5) Information of the orbital evolution.
+(6) 1D spherical profiles for single star models
 
-By giving the directory where the models are located as input, the last full dump in .ascii 
-and the .ev files of the sink particle(s) are reduced in order to gain relevant information 
-about the model:
-(1)  2D slice plots of the density, speed and temperature are produced (face-on/orbital plane 
-     & edge-on plane).
-(2)  1D radial plots of the density, speed and temperature are produced (along the x-, y- and 
-     z-axes).
-(3)  The terminal velocity in the model is calculated.
-(4)  Four morphological parameters are determined, giving a more quantitative insight in the 
-     degree of aspherity.
-(5)  The cummulative mass fraction and mean density are calculated in function of polar coordinate 
-     theta. This gives an indication about the degree of equatorial density enhancement (EDE).
-(6)  Information about the orbital evolution of the binary system and accreted mass onto the 
-     companion.
 
 
 Pipeline - More detailed information
 ------------------------------------
 
 This pipeline loads the wind.in and wind.setup files first. This is the general setup information 
 of the model (configuration of the system, information of the thermodynamics, evolution time, wind 
 outflow setup,...). Next the last full dump is loaded, and using this data, some other useful 
 quantities are calculated (gas pressure/temperature, speed, sperical coordinates, sound speed of 
 the gas,...).  Lastly, the data of the sink particle(s) is loaded. From this file, also the period 
-and orbital velocity of the sink particles in calculated, if the system is a binary, in function of 
+and orbital velocity of the sink particles is calculated, if the system is a multiple, in function of 
 time. The last entry in the sink data, corresponds to the full dump loaded. Therefore the 
 position/velocity/mass/... of this last entry are also saved in the full dump data for easy usage.
 
-NOTE: If you have paused and restarted your simulation, multiple .ev files will be constructed per 
-sink particle. The code anticipates to this problem, but you have to say so in the code yourself: 
-Uncomment the part starting at line 50 in the LoadSink.py script and put in the correct model. 
-
 
 (1)
 
 The 2D slices in the plots are infinitely thin and calculated by using the smoothing kernel from
-PHANTOM. The density, speed and temperature are calculated by this method on a grid of 300*300 
-pixels, using the data of the 20 nearest neighbours (SPH particles) of those grid points. These 
+PHANTOM. The density, speed and temperature are calculated by this method on a grid of n*n 
+pixels, using the data of the m nearest neighbours (SPH particles) of those grid points. These 
 plots give a visual representation of the morphology present in the AGB wind of the simulation.
 
 
 (2)
 
 In 1D, the data along the x-, y- and z-axes is constructed in the same way as explained in (1), 
 but for a 1D grid. This results in plots of the radial structure, which is an important addition 
 to the 2D slice plots.
 
 
 (3)
 
-The terminal velocity is in the case of the PHANTOM SPH code not an input parameter, so it needs 
-to be calculated. Due to the morphology in the outflow of the AGB star, at a certain radius a wide
-range of speeds will be obtained. Therefore calculating only one value for the terminal velocity 
-is not possible. Instead, three values are obtained, a minimum, mean and maximum terminal velocity. 
-The method used here is binning of the speed in function of the radius of the SHP particle to the 
-AGB star. Bins of 1AU are constructed and per bin, the minimum, mean and maximum speed is calculated.
-Using speed of the outer 20% of the data, three values for the terminal velocity are obtained. 
+The terminal velocity in PHANTOM SPH code is not an input parameter, so it needs to be calculated. 
+Due to the morphology in the outflow of the AGB star, at a certain radius a wide range of speeds 
+will be obtained. Therefore calculating only one value for the terminal velocity is not possible. 
+Instead, three values are obtained, a minimum, mean and maximum terminal velocity. The method used 
+here is binning the speed in function of the radius of the SHP particle to the AGB star. Bins of 
+1AU are constructed and per bin, the minimum, mean and maximum speed is calculated. Using speed of 
+the outer 20% of the data, three values for the terminal velocity are obtained. 
 
 NOTE: For some models (most often with slow initial wind velocity, low mass loss rate and/or low-mass 
 companion), the interaction of the companion has not reached the outer boundary of the model. Therefore, 
 this method will not lead to a correct terminal velocity value and thus the unphysical part of the data 
 will be cut off. Visually, the speed profile in function of radius shows a strong, unphysical linear 
 increase, starting with a clear twist.
 
 
-(4)
-
-In order to get some quantitative indication about the morphology of the models, two morphology 
+In order to get some quantitative indication about the morphology of the models, several morphology 
 parameters are currently in use: 
     - eta = v/v_orb (see Saladino, M. I., Pols, O. R., van der Helm, E., Pelupessy, I., & 
       Portegies Zwart, S. 2018, A&A, 618, A50; El Mellah, I., Bolte, J., Decin, L., Homan, 
       W., & Keppens, R. 2020, arXiv e-prints, arXiv:2001.04482)
     - Qp = p_comp/p_wind 
          = (M_comp v_orb) / (M_wind v_wind)
         (see Decin, L., Montarges, M., Richards, A. M. S., et al. 2020, Science, 369, 1497)
@@ -806,15 +794,15 @@
 Depending on the value of these parameters, the model is expected to show radial/EDE/complex morphology.
 
 Rhill = a(1-e)(M_comp/ 3M_AGB)^(1/3)
 Therefore, Rhill/Rcapt = epsilon, if for both radii the same v_wind is used.
 
 VERY IMPORTANT NOTE: 
 The parameter 'v_wind' is not unambiguously defined. Even more, if only a binary models is used, 
-this parameter is most likely not to be contrained properly. For the different morphological parameters, 
+this parameter is most likely not to be constrained properly. For the different morphological parameters, 
 multiple values for v_wind are used.
 For eta, different velocities/speed v are used:
     - terminal velocity
     - speed of the wind at the location of the companion 
 For Qp and epsilon, two different values are used as v_wind:
     - the mean velocity of the wind at the location is used as calculated from the binning
     - the average of the min and max velocity at the location of the companion is used
@@ -823,15 +811,15 @@
 Better options for v_wind would be to use the velocity of the corresponding single model as follows:
     - speed of the wind at the location of the companion
     - speed resulting from the vector sum of the speed of the wind at the location of the companion 
       and the orbital velocity of the AGB star.
 These can be calculated using the output of this pipeline.
 
 
-(5)
+(4)
 
 The cummulative mass fraction (CMF) is calculated in function of the polar angle theta (theta = 0.5pi 
 is the orbital plane, theta = 0 the north pole), again by using the method of binning. Only the northern 
 hemisphere is used, because of symmetry. Because of asymmetry along the x-axis, the positive (right) 
 and negative (left) part according to x are also calculated seperately. Certainly for eccentric models 
 this can differ. To calculate the CMF, only the selfsimilar part of the outflow it used, therefore a 
 factor (called factor) is given. The inner factor * semi-major axis AU is left out in this calculation.
@@ -841,15 +829,15 @@
 (theta25-theta50)/(theta50-theta75). When this parameter is normalised to the value for the corresponding 
 single model, it gives a measure for the degree of EDE.
 
 Also the mean density is calculated using a similar approach as the CMF, using the method of binning. 
 This mean density can easily be normalised to compare the morphology in different models.
 
 
-(6)
+(5)
 
 In order to get information about the orbital evolution, the sink files are used (.ev), which gives
 relevant quantities of the sink particles in function of time. This file returns plots of the orbit, 
 evolution of orbital separation, orbital velocity and accreted mass of the companion.
```

### Comparing `plons-0.0.7/src/plons.egg-info/SOURCES.txt` & `plons-0.0.9/src/plons.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 src/plons/ConversionFactors_cgs.py
 src/plons/GeometricalFunctions.py
 src/plons/LoadDataPHANTOM.py
 src/plons/LoadDump.py
 src/plons/LoadSetup.py
 src/plons/LoadSink.py
 src/plons/OrbitalEvolution.py
+src/plons/OrbitalEvolutionWAql.py
 src/plons/PhysicalQuantities.py
 src/plons/Profiles1D.py
 src/plons/RadialStructurePlots1D.py
 src/plons/RhoRradialFit.py
 src/plons/SlicePlots2D.py
 src/plons/SmoothingKernelScript.py
 src/plons/TerminalVelocity.py
 src/plons/Tools.py
 src/plons/Tubes.py
 src/plons/__init__.py
-src/plons/animationSlicePlots.py
 src/plons/main.py
-src/plons/merge1DPlotsDion.py
+src/plons/mainWAql.py
 src/plons/profile_1D_spherical_model.py
-src/plons/test.py
 src/plons/userSettings.py
 src/plons.egg-info/PKG-INFO
 src/plons.egg-info/SOURCES.txt
 src/plons.egg-info/dependency_links.txt
 src/plons.egg-info/requires.txt
 src/plons.egg-info/top_level.txt
 tests/test_SmoothingKernelScript.py
```

