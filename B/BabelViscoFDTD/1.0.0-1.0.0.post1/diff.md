# Comparing `tmp/BabelViscoFDTD-1.0.0.tar.gz` & `tmp/BabelViscoFDTD-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BabelViscoFDTD-1.0.0.tar", last modified: Mon Jan 30 08:27:56 2023, max compression
+gzip compressed data, was "BabelViscoFDTD-1.0.0.post1.tar", last modified: Wed Apr 12 03:51:24 2023, max compression
```

## Comparing `BabelViscoFDTD-1.0.0.tar` & `BabelViscoFDTD-1.0.0.post1.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.156021 BabelViscoFDTD-1.0.0/
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.141622 BabelViscoFDTD-1.0.0/BabelViscoFDTD/
--rw-r--r--   0 spichardo   (501) staff       (20)     6611 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/H5pySimple.py
--rw-r--r--   0 spichardo   (501) staff       (20)    40993 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/PropagationModel.py
--rw-r--r--   0 spichardo   (501) staff       (20)     1262 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation.py
--rw-r--r--   0 spichardo   (501) staff       (20)    13088 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_BASE.py
--rw-r--r--   0 spichardo   (501) staff       (20)    12836 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_CUDA.py
--rw-r--r--   0 spichardo   (501) staff       (20)    23867 2023-01-15 08:55:44.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_METAL.py
--rw-r--r--   0 spichardo   (501) staff       (20)     9270 2023-01-15 08:55:44.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_OPENCL.py
--rw-r--r--   0 spichardo   (501) staff       (20)        2 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/__init__.py
--rw-rw-r--   0 spichardo   (501) staff       (20)   335700 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/_gpu_kernel.c
--rw-rw-r--   0 spichardo   (501) staff       (20)    19872 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/_indexing.h
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.142802 BabelViscoFDTD-1.0.0/BabelViscoFDTD/tools/
--rw-r--r--   0 spichardo   (501) staff       (20)    56104 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/tools/RayleighAndBHTE.py
--rw-r--r--   0 spichardo   (501) staff       (20)        2 2023-01-15 08:55:44.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD/tools/__init__.py
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.142522 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/
--rw-rw-r--   0 spichardo   (501) staff       (20)    24711 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/PKG-INFO
--rw-rw-r--   0 spichardo   (501) staff       (20)     3185 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/SOURCES.txt
--rw-rw-r--   0 spichardo   (501) staff       (20)        1 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/dependency_links.txt
--rw-rw-r--   0 spichardo   (501) staff       (20)        2 2021-12-04 04:09:54.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/not-zip-safe
--rw-rw-r--   0 spichardo   (501) staff       (20)       45 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/requires.txt
--rw-rw-r--   0 spichardo   (501) staff       (20)       95 2023-01-30 08:27:56.000000 BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/top_level.txt
--rw-r--r--   0 spichardo   (501) staff       (20)      750 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/CMakeLists.txt
--rw-r--r--   0 spichardo   (501) staff       (20)     1463 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/LICENSE
--rw-r--r--   0 spichardo   (501) staff       (20)       32 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/MANIFEST.in
--rw-r--r--   0 spichardo   (501) staff       (20)    24711 2023-01-30 08:27:56.156111 BabelViscoFDTD-1.0.0/PKG-INFO
--rw-r--r--   0 spichardo   (501) staff       (20)    24168 2023-01-30 08:27:36.000000 BabelViscoFDTD-1.0.0/README.md
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.138655 BabelViscoFDTD-1.0.0/pi_ocl/
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.145321 BabelViscoFDTD-1.0.0/pi_ocl/build/
--rw-rw-r--   0 spichardo   (501) staff       (20)    15649 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeCache.txt
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.148248 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.149669 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/
--rw-rw-r--   0 spichardo   (501) staff       (20)     2647 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeCCompiler.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)     5594 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeCXXCompiler.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)    51200 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_C.bin
--rw-rw-r--   0 spichardo   (501) staff       (20)    51200 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_CXX.bin
--rw-rw-r--   0 spichardo   (501) staff       (20)      276 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeRCCompiler.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)      395 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeSystem.cmake
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.150404 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/
--rw-rw-r--   0 spichardo   (501) staff       (20)    21419 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.c
--rw-rw-r--   0 spichardo   (501) staff       (20)    96256 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.exe
--rw-rw-r--   0 spichardo   (501) staff       (20)     1793 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.obj
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.150973 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/
--rw-rw-r--   0 spichardo   (501) staff       (20)    21228 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rw-rw-r--   0 spichardo   (501) staff       (20)    96256 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.exe
--rw-rw-r--   0 spichardo   (501) staff       (20)     1814 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.obj
--rw-rw-r--   0 spichardo   (501) staff       (20)      643 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)     4583 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/CMakeError.log
--rw-rw-r--   0 spichardo   (501) staff       (20)     5728 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/CMakeOutput.log
--rw-rw-r--   0 spichardo   (501) staff       (20)     9085 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/Makefile.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)     3678 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/Makefile2
--rw-rw-r--   0 spichardo   (501) staff       (20)      272 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/TargetDirectories.txt
--rw-rw-r--   0 spichardo   (501) staff       (20)       86 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/cmake.check_cache
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.153154 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/
--rw-rw-r--   0 spichardo   (501) staff       (20)     1152 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/C.includecache
--rw-rw-r--   0 spichardo   (501) staff       (20)      716 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/DependInfo.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)     5261 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/build.make
--rw-rw-r--   0 spichardo   (501) staff       (20)      293 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/cmake_clean.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)      515 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/depend.internal
--rw-rw-r--   0 spichardo   (501) staff       (20)      495 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/depend.make
--rw-rw-r--   0 spichardo   (501) staff       (20)      406 2021-09-17 03:20:08.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/embed.manifest
--rw-rw-r--   0 spichardo   (501) staff       (20)      367 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/flags.make
--rw-rw-r--   0 spichardo   (501) staff       (20)      381 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/intermediate.manifest
--rw-rw-r--   0 spichardo   (501) staff       (20)      192 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/manifest.rc
--rw-rw-r--   0 spichardo   (501) staff       (20)      472 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/manifest.res
--rw-rw-r--   0 spichardo   (501) staff       (20)       36 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/objects1.rsp
--rw-rw-r--   0 spichardo   (501) staff       (20)    32355 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/pi_ocl.c.obj
--rw-rw-r--   0 spichardo   (501) staff       (20)       46 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/progress.make
--rw-rw-r--   0 spichardo   (501) staff       (20)    86016 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/vc140.pdb
--rw-rw-r--   0 spichardo   (501) staff       (20)        3 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/progress.marks
--rw-rw-r--   0 spichardo   (501) staff       (20)     5555 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/Makefile
--rw-rw-r--   0 spichardo   (501) staff       (20)     1495 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/cmake_install.cmake
--rw-rw-r--   0 spichardo   (501) staff       (20)    65024 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/pi_ocl.exe
--rw-rw-r--   0 spichardo   (501) staff       (20)   668160 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/pi_ocl.ilk
--rw-rw-r--   0 spichardo   (501) staff       (20)   954368 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0/pi_ocl/build/pi_ocl.pdb
--rw-r--r--   0 spichardo   (501) staff       (20)       61 2023-01-30 08:27:56.156325 BabelViscoFDTD-1.0.0/setup.cfg
--rw-r--r--   0 spichardo   (501) staff       (20)    12776 2023-01-25 20:17:27.000000 BabelViscoFDTD-1.0.0/setup.py
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.155183 BabelViscoFDTD-1.0.0/src/
--rw-r--r--   0 spichardo   (501) staff       (20)     3560 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/src/CMakeLists.txt
--rw-r--r--   0 spichardo   (501) staff       (20)     7685 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/src/FDTD3D_CPU_VERSION.h
--rw-r--r--   0 spichardo   (501) staff       (20)    19772 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/src/FDTDStaggered3D_with_relaxation_python.c
--rw-r--r--   0 spichardo   (501) staff       (20)       52 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/src/FDTDStaggered3D_with_relaxation_python.cu
--rw-r--r--   0 spichardo   (501) staff       (20)    22799 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0/src/GPU_KERNELS.h
--rw-r--r--   0 spichardo   (501) staff       (20)    19872 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0/src/Indexing.h
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.155409 BabelViscoFDTD-1.0.0/src/Metal/
--rw-r--r--   0 spichardo   (501) staff       (20)     1003 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0/src/Metal/Package.swift
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.139245 BabelViscoFDTD-1.0.0/src/Metal/Sources/
-drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-01-30 08:27:56.155804 BabelViscoFDTD-1.0.0/src/Metal/Sources/BabelMetal/
--rw-r--r--   0 spichardo   (501) staff       (20)     2644 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0/src/Metal/Sources/BabelMetal/Babel.metal
--rw-r--r--   0 spichardo   (501) staff       (20)    14387 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0/src/Metal/Sources/BabelMetal/BabelMetal.swift
--rw-r--r--   0 spichardo   (501) staff       (20)    11716 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0/src/ParticleKernel.h
--rw-r--r--   0 spichardo   (501) staff       (20)     3484 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0/src/SensorsKernel.h
--rw-r--r--   0 spichardo   (501) staff       (20)    22490 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0/src/StressKernel.h
--rw-r--r--   0 spichardo   (501) staff       (20)    11888 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/src/commonDef.h
--rw-r--r--   0 spichardo   (501) staff       (20)    42357 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0/src/commonDefGPU.h
--rw-r--r--   0 spichardo   (501) staff       (20)     9249 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0/src/kernelparamsMetal.h
--rw-r--r--   0 spichardo   (501) staff       (20)     2074 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0/src/kernelparamsOpenCL.h
--rw-r--r--   0 spichardo   (501) staff       (20)     6590 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0/src/page_memory.c
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.598920 BabelViscoFDTD-1.0.0.post1/
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.583378 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/
+-rw-r--r--   0 spichardo   (501) staff       (20)     6611 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/H5pySimple.py
+-rw-r--r--   0 spichardo   (501) staff       (20)    40993 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/PropagationModel.py
+-rw-r--r--   0 spichardo   (501) staff       (20)     1262 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation.py
+-rw-r--r--   0 spichardo   (501) staff       (20)    13088 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_BASE.py
+-rw-r--r--   0 spichardo   (501) staff       (20)    12836 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_CUDA.py
+-rw-r--r--   0 spichardo   (501) staff       (20)    23867 2023-02-08 03:27:22.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_METAL.py
+-rw-r--r--   0 spichardo   (501) staff       (20)     9270 2023-01-15 08:55:44.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_OPENCL.py
+-rw-r--r--   0 spichardo   (501) staff       (20)        2 2023-01-15 08:55:33.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/__init__.py
+-rw-rw-r--   0 spichardo   (501) staff       (20)   335700 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/_gpu_kernel.c
+-rw-r--r--   0 spichardo   (501) staff       (20)   120502 2023-04-04 04:57:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/_gpu_kernel2D.c
+-rw-rw-r--   0 spichardo   (501) staff       (20)    19872 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/_indexing.h
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.584632 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/tools/
+-rw-r--r--   0 spichardo   (501) staff       (20)    56104 2023-01-30 09:20:40.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/tools/RayleighAndBHTE.py
+-rw-r--r--   0 spichardo   (501) staff       (20)        2 2023-01-15 08:55:44.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/tools/__init__.py
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.584337 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/
+-rw-rw-r--   0 spichardo   (501) staff       (20)    24822 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/PKG-INFO
+-rw-rw-r--   0 spichardo   (501) staff       (20)     3216 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/SOURCES.txt
+-rw-rw-r--   0 spichardo   (501) staff       (20)        1 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/dependency_links.txt
+-rw-rw-r--   0 spichardo   (501) staff       (20)        2 2021-12-04 04:09:54.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/not-zip-safe
+-rw-rw-r--   0 spichardo   (501) staff       (20)       45 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/requires.txt
+-rw-rw-r--   0 spichardo   (501) staff       (20)       95 2023-04-12 03:51:24.000000 BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/top_level.txt
+-rw-r--r--   0 spichardo   (501) staff       (20)      750 2023-04-06 21:11:09.000000 BabelViscoFDTD-1.0.0.post1/CMakeLists.txt
+-rw-r--r--   0 spichardo   (501) staff       (20)     1463 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/LICENSE
+-rw-r--r--   0 spichardo   (501) staff       (20)       32 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/MANIFEST.in
+-rw-r--r--   0 spichardo   (501) staff       (20)    24822 2023-04-12 03:51:24.599014 BabelViscoFDTD-1.0.0.post1/PKG-INFO
+-rw-r--r--   0 spichardo   (501) staff       (20)    24312 2023-04-12 03:48:25.000000 BabelViscoFDTD-1.0.0.post1/README.md
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.579994 BabelViscoFDTD-1.0.0.post1/pi_ocl/
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.587513 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/
+-rw-rw-r--   0 spichardo   (501) staff       (20)    15649 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeCache.txt
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.590201 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.591546 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/
+-rw-rw-r--   0 spichardo   (501) staff       (20)     2647 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeCCompiler.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)     5594 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeCXXCompiler.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)    51200 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_C.bin
+-rw-rw-r--   0 spichardo   (501) staff       (20)    51200 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_CXX.bin
+-rw-rw-r--   0 spichardo   (501) staff       (20)      276 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeRCCompiler.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)      395 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeSystem.cmake
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.592285 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/
+-rw-rw-r--   0 spichardo   (501) staff       (20)    21419 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.c
+-rw-rw-r--   0 spichardo   (501) staff       (20)    96256 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.exe
+-rw-rw-r--   0 spichardo   (501) staff       (20)     1793 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.obj
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.592951 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/
+-rw-rw-r--   0 spichardo   (501) staff       (20)    21228 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rw-rw-r--   0 spichardo   (501) staff       (20)    96256 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.exe
+-rw-rw-r--   0 spichardo   (501) staff       (20)     1814 2021-09-17 03:19:54.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.obj
+-rw-rw-r--   0 spichardo   (501) staff       (20)      643 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)     4583 2021-09-17 03:19:56.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/CMakeError.log
+-rw-rw-r--   0 spichardo   (501) staff       (20)     5728 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/CMakeOutput.log
+-rw-rw-r--   0 spichardo   (501) staff       (20)     9085 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/Makefile.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)     3678 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/Makefile2
+-rw-rw-r--   0 spichardo   (501) staff       (20)      272 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/TargetDirectories.txt
+-rw-rw-r--   0 spichardo   (501) staff       (20)       86 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/cmake.check_cache
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.595423 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/
+-rw-rw-r--   0 spichardo   (501) staff       (20)     1152 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/C.includecache
+-rw-rw-r--   0 spichardo   (501) staff       (20)      716 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/DependInfo.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)     5261 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/build.make
+-rw-rw-r--   0 spichardo   (501) staff       (20)      293 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/cmake_clean.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)      515 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/depend.internal
+-rw-rw-r--   0 spichardo   (501) staff       (20)      495 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/depend.make
+-rw-rw-r--   0 spichardo   (501) staff       (20)      406 2021-09-17 03:20:08.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/embed.manifest
+-rw-rw-r--   0 spichardo   (501) staff       (20)      367 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/flags.make
+-rw-rw-r--   0 spichardo   (501) staff       (20)      381 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/intermediate.manifest
+-rw-rw-r--   0 spichardo   (501) staff       (20)      192 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/manifest.rc
+-rw-rw-r--   0 spichardo   (501) staff       (20)      472 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/manifest.res
+-rw-rw-r--   0 spichardo   (501) staff       (20)       36 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/objects1.rsp
+-rw-rw-r--   0 spichardo   (501) staff       (20)    32355 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/pi_ocl.c.obj
+-rw-rw-r--   0 spichardo   (501) staff       (20)       46 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/progress.make
+-rw-rw-r--   0 spichardo   (501) staff       (20)    86016 2021-09-17 03:58:12.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/vc140.pdb
+-rw-rw-r--   0 spichardo   (501) staff       (20)        3 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/progress.marks
+-rw-rw-r--   0 spichardo   (501) staff       (20)     5555 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/Makefile
+-rw-rw-r--   0 spichardo   (501) staff       (20)     1495 2021-09-17 03:19:58.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/cmake_install.cmake
+-rw-rw-r--   0 spichardo   (501) staff       (20)    65024 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/pi_ocl.exe
+-rw-rw-r--   0 spichardo   (501) staff       (20)   668160 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/pi_ocl.ilk
+-rw-rw-r--   0 spichardo   (501) staff       (20)   954368 2021-09-17 03:58:14.000000 BabelViscoFDTD-1.0.0.post1/pi_ocl/build/pi_ocl.pdb
+-rw-r--r--   0 spichardo   (501) staff       (20)       61 2023-04-12 03:51:24.599289 BabelViscoFDTD-1.0.0.post1/setup.cfg
+-rw-r--r--   0 spichardo   (501) staff       (20)    12778 2023-04-12 03:48:52.000000 BabelViscoFDTD-1.0.0.post1/setup.py
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.597721 BabelViscoFDTD-1.0.0.post1/src/
+-rw-r--r--   0 spichardo   (501) staff       (20)     3560 2023-04-06 21:11:09.000000 BabelViscoFDTD-1.0.0.post1/src/CMakeLists.txt
+-rw-r--r--   0 spichardo   (501) staff       (20)     7685 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/src/FDTD3D_CPU_VERSION.h
+-rw-r--r--   0 spichardo   (501) staff       (20)    19772 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/src/FDTDStaggered3D_with_relaxation_python.c
+-rw-r--r--   0 spichardo   (501) staff       (20)       52 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/src/FDTDStaggered3D_with_relaxation_python.cu
+-rw-r--r--   0 spichardo   (501) staff       (20)    22799 2023-01-25 20:16:29.000000 BabelViscoFDTD-1.0.0.post1/src/GPU_KERNELS.h
+-rw-r--r--   0 spichardo   (501) staff       (20)    19872 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0.post1/src/Indexing.h
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.598108 BabelViscoFDTD-1.0.0.post1/src/Metal/
+-rw-r--r--   0 spichardo   (501) staff       (20)     1003 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0.post1/src/Metal/Package.swift
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.580663 BabelViscoFDTD-1.0.0.post1/src/Metal/Sources/
+drwxr-xr-x   0 spichardo   (501) staff       (20)        0 2023-04-12 03:51:24.598704 BabelViscoFDTD-1.0.0.post1/src/Metal/Sources/BabelMetal/
+-rw-r--r--   0 spichardo   (501) staff       (20)     2644 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0.post1/src/Metal/Sources/BabelMetal/Babel.metal
+-rw-r--r--   0 spichardo   (501) staff       (20)    14387 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0.post1/src/Metal/Sources/BabelMetal/BabelMetal.swift
+-rw-r--r--   0 spichardo   (501) staff       (20)    11716 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0.post1/src/ParticleKernel.h
+-rw-r--r--   0 spichardo   (501) staff       (20)     3484 2023-02-05 23:59:47.000000 BabelViscoFDTD-1.0.0.post1/src/SensorsKernel.h
+-rw-r--r--   0 spichardo   (501) staff       (20)    22490 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0.post1/src/StressKernel.h
+-rw-r--r--   0 spichardo   (501) staff       (20)    11888 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/src/commonDef.h
+-rw-r--r--   0 spichardo   (501) staff       (20)    42357 2023-01-15 08:56:16.000000 BabelViscoFDTD-1.0.0.post1/src/commonDefGPU.h
+-rw-r--r--   0 spichardo   (501) staff       (20)     9249 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0.post1/src/kernelparamsMetal.h
+-rw-r--r--   0 spichardo   (501) staff       (20)     2074 2023-01-15 08:56:43.000000 BabelViscoFDTD-1.0.0.post1/src/kernelparamsOpenCL.h
+-rw-r--r--   0 spichardo   (501) staff       (20)     6590 2023-01-15 08:56:35.000000 BabelViscoFDTD-1.0.0.post1/src/page_memory.c
```

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/H5pySimple.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/H5pySimple.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/PropagationModel.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/PropagationModel.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_BASE.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_BASE.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_CUDA.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_CUDA.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_METAL.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_METAL.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_OPENCL.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_OPENCL.py`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/_gpu_kernel.c` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/_gpu_kernel.c`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/_indexing.h` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/_indexing.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD/tools/RayleighAndBHTE.py` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD/tools/RayleighAndBHTE.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,29 +36,29 @@
             }
             
             R2 = (d_output[coord] >= Tref)?0.5:0.25; 
             R1 = (d_input[coord] >= Tref)?0.5:0.25;
 
             if(fabs(d_output[coord]-d_input[coord])<0.0001)
             {
-                d_output2[coord] = d_input2[coord] + dt * pow(float(R1),float((Tref-d_input[coord])));
+                d_output2[coord] = d_input2[coord] + dt * pow((float)R1,(float)(Tref-d_input[coord]));
             }
             else
             {
                 if(R1 == R2)
                 {
-                    d_output2[coord] = d_input2[coord] + (pow(float(R2),float((Tref-d_output[coord]))) - pow(float(R1),float((Tref-d_input[coord])))) / 
+                    d_output2[coord] = d_input2[coord] + (pow((float)R2,(float)(Tref-d_output[coord])) - pow((float)R1,(float)(Tref-d_input[coord]))) / 
                                    ( -(d_output[coord]-d_input[coord])/ dt * log(R1));
                 }
                 else
                 {
                     dtp = dt * (Tref - d_input[coord])/(d_output[coord] - d_input[coord]);
 
-                    d_output2[coord] = d_input2[coord] + (1 - pow(float(R1),float((Tref-d_input[coord]))))     / (- (Tref - d_input[coord])/ dtp * log(R1)) + 
-                                   (pow(float(R2),float((Tref-d_output[coord]))) - 1) / (-(d_output[coord] - Tref)/(dt - dtp) * log(R2));
+                    d_output2[coord] = d_input2[coord] + (1 - pow((float)R1,(float)(Tref-d_input[coord])))     / (- (Tref - d_input[coord])/ dtp * log(R1)) + 
+                                   (pow((float)R2,(float)(Tref-d_output[coord])) - 1) / (-(d_output[coord] - Tref)/(dt - dtp) * log(R2));
                 }
             }
 
             if (gtidy==SelJ && (n_Step % nFactorMonitoring ==0))
             {
                  d_MonitorSlice[gtidx*outerDimz*TotalStepsMonitoring+gtidz*TotalStepsMonitoring+ n_Step/nFactorMonitoring] =d_output[coord];
             }
```

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/PKG-INFO` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: BabelViscoFDTD
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: GPU/CPU 3D FDTD solution of viscoelastic equation
-Home-page: UNKNOWN
 Author-email: samuel.pichardo@ucalgary.ca
 License: BSD License
 Keywords: FDTD,CUDA,OpenCL,Metal,viscoelastic
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 BabelViscoFDTD
 =============
-Samuel Pichardo, Ph.D  
-Associate Professor  
-Radiology and Clinical Neurosciences, Hotchkiss Brain Institute  
-Cumming School of Medicine,  
-University of Calgary   
-samuel.pichardo@ucalgary.ca  
+Samuel Pichardo, Ph.D
+Associate Professor
+Radiology and Clinical Neurosciences, Hotchkiss Brain Institute
+Cumming School of Medicine,
+University of Calgary
+samuel.pichardo@ucalgary.ca
 www.neurofus.ca
 
 **Software library for FDTD of the viscoelastic equation using a staggered grid arrangement and including the superposition method, with multiple CPU- and GPU-based backends (OpenMP, CUDA, OpenCL and Metal)**
 
 This tool solves in the time domain the viscoelastic equation for wave propagation using a staggered grid solution. The solution is primarily based on a paper from Virieux (Virieux, J., 1986. P-SV wave propagation in heterogeneous media: Velocity-stress finite-difference method. Geophysics, 51(4), pp.889-901.), who implemented for the first time the staggered grid solution for the viscoelastic equation.
  While the underlying equations and methods were developed primarily for seismic simulation, the BabelViscoFDTD library was developed for biomedical applications to study the ultrasound transmission through bone material, with skull bone as the primary target for study.
 
@@ -60,29 +58,29 @@
 ## Python 3.8 and up
 The use of virtual environments is recommended. Anaconda Python and Enthought EDM are great choices as the main environment in any OS, but overall any Python distribution should do the work. The only limitation in Windows is that wheels for the latest versions of pyopencl are available for Python >=3.8. For Apple Silicon systems, it is recommended to use a native Python for arm64 (see below details).
 
 ## CUDA (For Windows and Linux)
 The code has been verified to work from CUDA 9 to CUDA 11. Highly likely older versions of CUDA (7, 8) should work without a problem. Be sure of installing the CUDA samples and take note of the location where they were installed.
 
 ## CMAKE
-CMAKE version>= 3.16.3. 
+CMAKE version>= 3.16.3.
 
 ## OpenCL
 OpenCL for Windows and Apple Silicon systems is operational via `pyopencl`. In macOS, you can install pyopencl with `pip install pyopencl`. In Windows, use one of the precompiled wheels in https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl. The FDTD kernels code is OpenCL >= 1.2 compliant.
 
 ### Basic Python dependencies:
 latest version of `pip`
 * numpy>=1.15.1 (have this already installed if starting from a clean environment)
 * scipy>=1.1.0 (have this already installed if starting from a clean environment)
 * h5py>=2.9.0 (in native arm64 Python for Apple Silicon, install this via `conda install h5py`)
 * hdf5plugin>=3.2.0
 * pydicom>=1.3.0
 * setuptools >=51.0.0
 * pyopencl>=2020 (if in Windows, install manually a wheel from https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl)
-* cupy-cuda11x in Linux (via pip). In Windows install with conda in windows with `conda install -c conda-forge cupy` 
+* cupy-cuda11x in Linux (via pip). In Windows install with conda in windows with `conda install -c conda-forge cupy`
 
 `h5py`, `hdf5plugin`, `pydicom` and `pyopencl` are installed automatically as requirements if they are no present in the Python enviroment..
 
 ### macOS systems: Manual installation of modified `metalcompute`
 As noted in the release notes below for v0.9.9.20, we use a modified version of `py-metal-compute`. To avoid confusing with the original library, the modified version needs to be installed manually with
 
 `pip install  git+https://github.com/ProteusMRIgHIFU/py-metal-compute.git`
@@ -123,40 +121,48 @@
 Overall, any LTS-type distribution is recommended to be sure CUDA compiler supports your default GCC installation. If your installation can run the default examples of CUDA, then you should be good.
 
 You may also need to install OpenCL headers and libraries such as `opencl-headers`, `ocl-icd-opencl-dev`, `intel-opencl-icd` and other libraries required by you GPU manufacturer to support OpenCL. You can verify you have a healthy OpenCL installation with the tool `clinfo`.
 
 #### Linux in Windows through WSL2
 Starting in 2020, support for CUDA execution directly in WSL2 became possible. We have had excellent experiences with it. Just follow the official instructions from NVIDIA (https://docs.nvidia.com/cuda/wsl-user-guide/index.html)
 
-Please note that OpenCL is not supported under WSL2. 
+Please note that OpenCL is not supported under WSL2.
 
 ### Windows native
 You will need a VStudio installation that is compatible with your CUDA version; for example, CUDA 11.2 supports officially VS 2015 to 2019.
 
 ### macOS
 Any recent version of macOS and XCode with the command-line tools should be enough. Most tests have been done in Big Slur and Monterey. The CPU version in macOS supports OpenMP in ARM64 processors (M1, M1 Max, M2 ultra, M2). In X86-64, the OpenMP feature is now turned as experimental; by default, it will run only single-thread. See below for details on how to enable it. For ARM64 version will have OpenMP fully enabled by default.
 
-The OpenCL and Metal backed have been tested in Intel-based integrated GPUs, AMD GPUs and  ARM64-based systems. There are, however, some limitations of AMD GPUs with OpenCL (see below macOS notes for more details). Metal backend is available for both X86-64 and Apple Silicon systems. Overall, Metal is the recommended backend for M1 processors and AMD GPUs. 
+The OpenCL and Metal backed have been tested in Intel-based integrated GPUs, AMD GPUs and  ARM64-based systems. There are, however, some limitations of AMD GPUs with OpenCL (see below macOS notes for more details). Metal backend is available for both X86-64 and Apple Silicon systems. Overall, Metal is the recommended backend for M1 processors and AMD GPUs.
 
 Best scenario for both X64 and ARM64-based systems is to use fully native Python distributions using homebrew:
 1. Install  [homebrew](https://brew.sh/)
 `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
 1. Install miniforge
 `brew install miniforge`
 1. Create and activate a Python environment (for ARM64, Python 3.9 is recommended)
 `conda create —-name Babel python=3.9 scipy numpy`
 `conda activate Babel`
 1. Install BabelViscoFDTD
 `pip install BabelViscoFDTD`
 
 #### macOS experimental OpenMP in X86-64
+
 Thanks to the people who have reported the mitigated success with OpenMP. In my current systems, I didn't have problems, but later some users reported having issues with OpenMP. Then, we turned this feature as **experimental**, the time we can figure out a more stable approach.
-For X86-64, `libomp` and `mkl` must be installed first, otherwise compilation and execution for OpenMP will fail.
-* Install `libomp` with `brew install libomp`  
-* Install `mkl` with `pip install mkl` or `conda install mkl`
+For Intel or Apple Silicon CPU, `libomp` and `mkl` must be installed first, otherwise compilation and execution for OpenMP will fail.
+Install `mkl` with `pip install mkl` or `conda install mkl`
+
+Using Homebrew, install OpenMP and hint location to CMake:
+
+```sh
+brew install libomp
+
+export OpenMP_ROOT=/opt/homebrew/opt/libomp
+```
 
 
 To enable the OpenMP version for macOS install BabelViscoFDTD with:
 ```
 BABEL_MAC_OPENMP_X64=1 pip install BabelViscoFDTD
 ```
 or if you cloned the repository
@@ -181,30 +187,30 @@
 ### Multi-platform single code
 The underlying GPU code (start at `StaggeredFDTD_3D_With_Relaxation_<xx>.py` files) uses extensively C macros to provide a fully agnostic implementation that remains as efficient as possible regardless of using a CPU or GPU backend. It supports via macro definitions compilation for native CPU (X86, arm64), CUDA, OpenCL and Metal architectures; single or double precision.
 
 Regardless if using CUDA, OpenCL or Metal, conceptually the workflow is very similar. However, there are a few implementation details that need to be handled. cupy, pyopencl and metalcompute libraries help to minimize the amount the coding while still providing best performance possible with each backend.
 
 # Important information specific to the different environments for use
 ### macOS notes
-macOS support for HPC has shifted in recent years significantly. In modern macOS versions, the support for NVIDIA cards is inexistent and OpenCL *was supposed to be* officially out of support beyond Big Slur (*it is still running quite well in Monterey*). For macOS, Metal backend is recommended for AMD processors. OpenCL in macOS X86_64 may have other limitations such as the underlying driver may only support 32 bits memory access, even if the card has more than 4 GB of RAM. However, this limitation seems to be case by case. For ARM64 processors, OpenCL drivers can support 64 bit addressing. For an AMD W6800 (32 GB RAM) it only supports 32 bits. The `clinfo` tool (available with homebrew) can provide details if your current GPU and drivers support 64 bits addressing. The OpenCL implementation with ARM64 processors works only with a native Python arm64 installation. 
+macOS support for HPC has shifted in recent years significantly. In modern macOS versions, the support for NVIDIA cards is inexistent and OpenCL *was supposed to be* officially out of support beyond Big Slur (*it is still running quite well in Monterey*). For macOS, Metal backend is recommended for AMD processors. OpenCL in macOS X86_64 may have other limitations such as the underlying driver may only support 32 bits memory access, even if the card has more than 4 GB of RAM. However, this limitation seems to be case by case. For ARM64 processors, OpenCL drivers can support 64 bit addressing. For an AMD W6800 (32 GB RAM) it only supports 32 bits. The `clinfo` tool (available with homebrew) can provide details if your current GPU and drivers support 64 bits addressing. The OpenCL implementation with ARM64 processors works only with a native Python arm64 installation.
 
 ### Metal support
-Overall, Metal requires a bit more coding to prepare the pipelines for compute execution.  A challenge is that Metal for scientific computing still lacks serious examples. Nevertheless, the support for Metal is desirable for Apple Silicon systems. As toolchains, including native Python in arm64, are now becoming widespread available, it is interesting to see how well these devices stand quite well compared to Nvidia or AMD-based systems. There are some limitations such as the maximal number of kernel parameters (32) and that each GPU buffer memory is limited to 3.5 GB RAM for Metal-supported GPUs. But this is a limitation manageable by packing multiple logical arrays across multiple buffers. We explored the use of Metal Argument Buffers, but it ended in poorer performance than packing multiple arrays logically. In the current release of BabelViscoFDTD, it is completely stable to run large domains with AMD GPUs and ARM64-based processors with 32 or more GB of RAM. 
+Overall, Metal requires a bit more coding to prepare the pipelines for compute execution.  A challenge is that Metal for scientific computing still lacks serious examples. Nevertheless, the support for Metal is desirable for Apple Silicon systems. As toolchains, including native Python in arm64, are now becoming widespread available, it is interesting to see how well these devices stand quite well compared to Nvidia or AMD-based systems. There are some limitations such as the maximal number of kernel parameters (32) and that each GPU buffer memory is limited to 3.5 GB RAM for Metal-supported GPUs. But this is a limitation manageable by packing multiple logical arrays across multiple buffers. We explored the use of Metal Argument Buffers, but it ended in poorer performance than packing multiple arrays logically. In the current release of BabelViscoFDTD, it is completely stable to run large domains with AMD GPUs and ARM64-based processors with 32 or more GB of RAM.
 
 While Metal offers better performance overall over OpenCL in both Apple and AMD processors, some issues remain. Extensive testing has indicated that the Python process freezes after running a few tens of thousands of kernel calls. For most of the applications, this won't be an issue. If running very long extensive parametric studies under a single execution, be aware you may need to split your execution into chunks that can be called in separate `python <Myprogram.py>` calls. I suspect some driver issue limiting the number of consecutive kernels calls in a single process.
 
 ## Single precision performance comparison
 Performance between modern AMD, NVIDIA and Apple Silicon GPUs can show important differences. A simulation for a domain of  [414, 219 , 375] grid size and over 2841 temporal steps was used to benchmark multiple backends and systems.
 
 * Nvidia RTX A6000 (48 GB RAM, 10752 CUDA Cores, theoretical 38.7 SP TFLOP , memory bandwidth 768 GB/s)
-* AMD Radeon Pro W6800 (32 GB RAM, 3840  stream processors, theoretical 17.83 SP TFLOP, memory bandwidth 512 GB/s) 
-* AMD Vega 56 (8 GB RAM, 3584  stream processors, theoretical 10.5 SP TFLOP, memory bandwidth  410 GB/s) 
+* AMD Radeon Pro W6800 (32 GB RAM, 3840  stream processors, theoretical 17.83 SP TFLOP, memory bandwidth 512 GB/s)
+* AMD Vega 56 (8 GB RAM, 3584  stream processors, theoretical 10.5 SP TFLOP, memory bandwidth  410 GB/s)
 * M1 Max  (64 GB RAM, 10 CPU cores, 32 GPU Cores, 4096 execution units (which PR material says translates into a theoretical 98304 simultaneous threads), theoretical 10.4 SP TFLOP, memory bandwidth 400 GB/s)
 
-RTX A6000 test was done in 128 GB Xeon W-2125 CPU (4x2 cores) @ 4.00GHz Dell system. AMD Vega 64 and AMD Radeon Pro W6800 were tested in an 128 GB iMac Pro system (10x2 Core Intel Xeon W). The Vega 64 GPU is part of the iMac system, while the Pro W6800 is connected via a Thunderbolt 3 external enclosure. Please note that GPU connectivity should not have an important effect given memory transfers between GPU and CPU are minimal. The M1 Max was configured with 64 GB and installed in a 2021 MacBook Pro system. The Dell system, iMac Pro and MacBook Pro were also used for OpenMP benchmarks. Python 3.9 was used in all systems. The Dell system test used CUDA 11.4 and Visual Studio 2019 Community edition. The latest versions of pycuda and pyopencl at the time of testing (Sep 18, 2022) were used. macOS Monterey 12.5.1 with XCode 14 were used for both iMac Pro and MacBook Pro. 
+RTX A6000 test was done in 128 GB Xeon W-2125 CPU (4x2 cores) @ 4.00GHz Dell system. AMD Vega 64 and AMD Radeon Pro W6800 were tested in an 128 GB iMac Pro system (10x2 Core Intel Xeon W). The Vega 64 GPU is part of the iMac system, while the Pro W6800 is connected via a Thunderbolt 3 external enclosure. Please note that GPU connectivity should not have an important effect given memory transfers between GPU and CPU are minimal. The M1 Max was configured with 64 GB and installed in a 2021 MacBook Pro system. The Dell system, iMac Pro and MacBook Pro were also used for OpenMP benchmarks. Python 3.9 was used in all systems. The Dell system test used CUDA 11.4 and Visual Studio 2019 Community edition. The latest versions of pycuda and pyopencl at the time of testing (Sep 18, 2022) were used. macOS Monterey 12.5.1 with XCode 14 were used for both iMac Pro and MacBook Pro.
 
 Wall-time was measured from the moment preparations to run GPU code started (initiate device operation) to the end of the memory transfer of results, with no access to the main drives involved. Memory transfer between CPU and GPU occurred only at the beginning and end of GPU execution. The numerical difference among different backends was in the order of single precision resolution.
 
 ### Summary of wall-time results for each device
 | Device |  CUDA single | OpenCL single |  Metal single | OpenMP single|
 | --- | --- |  --- |  --- |  ---  |
 | AMD W6800 | - | - |  68 s | - |
@@ -213,59 +219,58 @@
 | M1 Max | - |  94 s |92 s| 1546 s (10 threads) |
 | Xeon W-2125 | - | - | - | 5163 s (8 threads)|
 | iMac Pro (Xeon W) | - | - | - | 2982 s  (20 threads)|
 
 #### Discussion of results
 The number of computing units is becoming a bit useless to compare. There are a few interesting aspects worth mentioning:
 * The ratio of performance between M1 Max and A6000 (CUDA vs. Metal) is not even close to the theoretical difference of raw SP TFLOPS%.
-* Metal and OpenCL performances of the M1 Max are pretty much equal, outmatching the A6000 performance. 
+* Metal and OpenCL performances of the M1 Max are pretty much equal, outmatching the A6000 performance.
 * Multiple tryouts on the CUDA code to adjust grid and block sizes didn't improve performance in the A6000. On the contrary, wall-time was increased, indicating that the recommended method by Nvidia to calculate maximal occupancy used by default in BabelViscoFDTD provided the best performance with the A6000.
-* The other surprise was the W6800 with Metal and OpenCL outperforming by a significant margin the A6000. 
-* The OpenMP performance of the M1 Max is also excellent, showing a dramatic speedup compared to the Dell Xeon and iMac Pro systems. 
+* The other surprise was the W6800 with Metal and OpenCL outperforming by a significant margin the A6000.
+* The OpenMP performance of the M1 Max is also excellent, showing a dramatic speedup compared to the Dell Xeon and iMac Pro systems.
 
 ## Possibility of manual adjustments to improve performance
-All three GPU backends have analogous control to split the calculations in the GPU multiprocessors. BabelViscoFDTD uses the methods that are recommended for each backend to ensure maximal GPU occupancy. However, manual adjustments can provide improvement to the performance. You can specify manually the grid and thread block dimensions with the optional parameters `ManualGroupSize` and `ManualLocalSize`, respectively. Please consult the guidelines of each backend (CUDA, OpenCL and Metal) on how to calculate this correctly, otherwise there is a risk of specifying a too large or too short grid and thread size dimensions. For example, for both CUDA and Metal, the multiplication of `ManualGroupSize` and `ManualLocalSize` must be equal or larger than the domain size ([N1,N2,N3]) to ensure all the domain is covered; for example for a domain of size [231,220,450], `ManualGroupSize=[60,60,115]` with `ManualLocalSize=[4,4,4]` will ensure covering the domain size. For `OpenCL` each entry in `ManualGroupSize` must be equal or larger than [N1,N2,N3] and each entry must be a multiple of its corresponding entry in `ManualLocalSize`; for example for a domain of size [231,220,450], `ManualGroupSize=[240,240,460]` with `ManualLocalSize=[4,4,4]`. Be sure of specifying these parameters as an np.array of type np.int32, such as `ManualLocalSize=np.array([4,4,4]).astype(np.int32)`. 
+All three GPU backends have analogous control to split the calculations in the GPU multiprocessors. BabelViscoFDTD uses the methods that are recommended for each backend to ensure maximal GPU occupancy. However, manual adjustments can provide improvement to the performance. You can specify manually the grid and thread block dimensions with the optional parameters `ManualGroupSize` and `ManualLocalSize`, respectively. Please consult the guidelines of each backend (CUDA, OpenCL and Metal) on how to calculate this correctly, otherwise there is a risk of specifying a too large or too short grid and thread size dimensions. For example, for both CUDA and Metal, the multiplication of `ManualGroupSize` and `ManualLocalSize` must be equal or larger than the domain size ([N1,N2,N3]) to ensure all the domain is covered; for example for a domain of size [231,220,450], `ManualGroupSize=[60,60,115]` with `ManualLocalSize=[4,4,4]` will ensure covering the domain size. For `OpenCL` each entry in `ManualGroupSize` must be equal or larger than [N1,N2,N3] and each entry must be a multiple of its corresponding entry in `ManualLocalSize`; for example for a domain of size [231,220,450], `ManualGroupSize=[240,240,460]` with `ManualLocalSize=[4,4,4]`. Be sure of specifying these parameters as an np.array of type np.int32, such as `ManualLocalSize=np.array([4,4,4]).astype(np.int32)`.
 
 # Supported platforms for Rayleigh's integral
-Since v0.9.2 Rayleigh-Sommerfeld's integral was added as a tool (see tutorial `Tutorial Notebooks\Tools -1 - Rayleigh Integral.ipynb`). This will be useful to combine models that include large volumes of water as the Rayleigh integral benefits considerably a GPU as the Rayleigh-Sommerfeld integral is hyper-parallel. The tool has support for 3 GPU backends: CUDA and OpenCL for Windows and Linux, and Metal and OpenCL for macOS. 
+Since v0.9.2 Rayleigh-Sommerfeld's integral was added as a tool (see tutorial `Tutorial Notebooks\Tools -1 - Rayleigh Integral.ipynb`). This will be useful to combine models that include large volumes of water as the Rayleigh integral benefits considerably a GPU as the Rayleigh-Sommerfeld integral is hyper-parallel. The tool has support for 3 GPU backends: CUDA and OpenCL for Windows and Linux, and Metal and OpenCL for macOS.
 
 # Release notes
+* 1.0.0-1 - To fix pip version that had an incorrect file for OpenCL BHTE
 * 1.0.0 - That is it! After thousands of simulations for a manuscript preparation to introduce the [BabelBrain](https://github.com/ProteusMRIgHIFU/BabelBrain) planning suite (Now public), this is ready for an official 1.0.0 release. 
     * cupy replaces PyCUDA for all CUDA operations. PyCUDA needs a Visual Studio compiler on the path to compile kernels in Windows. BabelBrain uses a lot cupy; switching to it helps to keep using a single interface while benefitting from the availability of Numpy-like methods.
     * Add a new correction parameter for attenuation. One of the findings while preparing the use with BabelBrain was that mapping procedures in the literature linking CT Hounsfield Units (HU) to the speed of sound and, especially, attenuation needs this sort of correction.
 * 0.9.10-1 Nov 16, 2022
-    * Add functions to list devices supported by computing backends 
+    * Add functions to list devices supported by computing backends
 * 0.9.10 Oct 28, 2022
     * Fix the issue with mapping of unique values when attenuation is used, it could cause some divisions by zero
 * 0.9.9.20 Sep 17, 2022
-    * A lot of important improvements to make the final line  
+    * A lot of important improvements to make the final line
         - Metal is (finally) running as fast (sometimes slightly faster) than OpenCL in Apple processors. It took a lot of testing and fine tuning.
         - Use of a modified version of the excellent `py-metal-compute` library (https://github.com/baldand/py-metal-compute) that allows having a similar approach as with pyopencl, cupy and pycuda. Modified library is at https://github.com/ProteusMRIgHIFU/py-metal-compute. Because of this new approach, the old Swift interface to the FDTD code was removed.
         - Add Metal backend for BHTE tool. This version runs way faster than OpenCL in Apple processors (like a 10x factor, need to investigate more if we can replicate such gain)
         - Benchmark metrics above were refreshed
         - Moving forward, OpenCL is not recommended for macOS in X64 systems. Because of the limitation of the underlying 32-bit addressing, pyopencl does not catch easily when a simulation goes beyond 4GB. However, Metal for AMD in macOS runs quite well, so no need to stick with OpenCL
 
 * 0.9.9  Sep 1, 2022
-    * A lot of simplifications allowed having a much more straightforward code. Thanks to Andrew Xie (@IAmAndrewX) for a very productive summer trimming down code, replacing the old MTLPP with Swift, and making a new class arrangement for the different GPU backends. Now BabelViscoFDTD is based completely on pyopencl and pycuda for the FDTD viscoelastic solver. For Metal, the Swift-based wrapper does the interfacing. The old C extension is still around just for the OpenMP backend.  
+    * A lot of simplifications allowed having a much more straightforward code. Thanks to Andrew Xie (@IAmAndrewX) for a very productive summer trimming down code, replacing the old MTLPP with Swift, and making a new class arrangement for the different GPU backends. Now BabelViscoFDTD is based completely on pyopencl and pycuda for the FDTD viscoelastic solver. For Metal, the Swift-based wrapper does the interfacing. The old C extension is still around just for the OpenMP backend.
 * 0.9.7  July 7, 2022
-    * The MTLPP C++ library is now replaced by a Swift interface to access the Metal implementation for the viscoelastic FDTD solution. This will ensure using a more standard Apple development language for the future, as MTLPP is not maintained anymore. While there is a new Apple-based C++ wrapper for Metal, using Swift is still preferred as we created now a C-linking compatible library that in the future can be also used directly in Python. In the long term, we aim to eliminate the C code extension and use only Python code in tandem with pyopencl, pycuda and  Metal 
+    * The MTLPP C++ library is now replaced by a Swift interface to access the Metal implementation for the viscoelastic FDTD solution. This will ensure using a more standard Apple development language for the future, as MTLPP is not maintained anymore. While there is a new Apple-based C++ wrapper for Metal, using Swift is still preferred as we created now a C-linking compatible library that in the future can be also used directly in Python. In the long term, we aim to eliminate the C code extension and use only Python code in tandem with pyopencl, pycuda and  Metal
 * 0.9.6-post-10  June 27, 2022
     * A fix for OpenCL in X64 Mac system that was missing the new kernel names
     * OpenMP for X64 in Mac is being turned back as experimental feature as some systems are unable to run with it correctly and there is not a clear path on how to ensure this will be stable. The feature will remain accessible if installing the library with the BABEL_MAC_OPENMP_X64 option enabled.
 * 0.9.6  Feb 5, 2022.
     * Improved performance in Metal-based devices by using mini-kernels.
     * Minor fixes for Rayleigh-Sommerfeld in Metal
 * 0.9.5  Jan 18, 2022.
     * Very first pip-registered version
     * Possibility of user-specified dimensions of blocks for computations for fine-tuning performance
     * Cleaning some minor bugs and adding BHTE code using pycuda and pyopencl.
-    
+
 * 0.9.3  Sep 29, 2021.
     * Improved support for both Metal and OpenCL. For Metal, stable operation is now feasible for large domains using all available memory in modern high-end GPUs. OpenCL is now supported in all OSs.
 * 0.9.2  June 13, 2021.
     * Add Rayleigh integral support in a homogenous medium with CUDA, OpenCL and Metal backends.
     * Support for stress sources
     * Able to select devices in multiple GPU systems with CUDA
 * 0.9.1  Feb 17, 2021. Pressure calculation added in low-level function.
 * 0.9.0  Dec 2020. First porting from the private repository and big reorganization to make it more user friendly
-
-
```

### Comparing `BabelViscoFDTD-1.0.0/BabelViscoFDTD.egg-info/SOURCES.txt` & `BabelViscoFDTD-1.0.0.post1/BabelViscoFDTD.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation.py
 BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_BASE.py
 BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_CUDA.py
 BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_METAL.py
 BabelViscoFDTD/StaggeredFDTD_3D_With_Relaxation_OPENCL.py
 BabelViscoFDTD/__init__.py
 BabelViscoFDTD/_gpu_kernel.c
+BabelViscoFDTD/_gpu_kernel2D.c
 BabelViscoFDTD/_indexing.h
 BabelViscoFDTD.egg-info/PKG-INFO
 BabelViscoFDTD.egg-info/SOURCES.txt
 BabelViscoFDTD.egg-info/dependency_links.txt
 BabelViscoFDTD.egg-info/not-zip-safe
 BabelViscoFDTD.egg-info/requires.txt
 BabelViscoFDTD.egg-info/top_level.txt
```

### Comparing `BabelViscoFDTD-1.0.0/CMakeLists.txt` & `BabelViscoFDTD-1.0.0.post1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/LICENSE` & `BabelViscoFDTD-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/PKG-INFO` & `BabelViscoFDTD-1.0.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: BabelViscoFDTD
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: GPU/CPU 3D FDTD solution of viscoelastic equation
-Home-page: UNKNOWN
 Author-email: samuel.pichardo@ucalgary.ca
 License: BSD License
 Keywords: FDTD,CUDA,OpenCL,Metal,viscoelastic
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 BabelViscoFDTD
 =============
-Samuel Pichardo, Ph.D  
-Associate Professor  
-Radiology and Clinical Neurosciences, Hotchkiss Brain Institute  
-Cumming School of Medicine,  
-University of Calgary   
-samuel.pichardo@ucalgary.ca  
+Samuel Pichardo, Ph.D
+Associate Professor
+Radiology and Clinical Neurosciences, Hotchkiss Brain Institute
+Cumming School of Medicine,
+University of Calgary
+samuel.pichardo@ucalgary.ca
 www.neurofus.ca
 
 **Software library for FDTD of the viscoelastic equation using a staggered grid arrangement and including the superposition method, with multiple CPU- and GPU-based backends (OpenMP, CUDA, OpenCL and Metal)**
 
 This tool solves in the time domain the viscoelastic equation for wave propagation using a staggered grid solution. The solution is primarily based on a paper from Virieux (Virieux, J., 1986. P-SV wave propagation in heterogeneous media: Velocity-stress finite-difference method. Geophysics, 51(4), pp.889-901.), who implemented for the first time the staggered grid solution for the viscoelastic equation.
  While the underlying equations and methods were developed primarily for seismic simulation, the BabelViscoFDTD library was developed for biomedical applications to study the ultrasound transmission through bone material, with skull bone as the primary target for study.
 
@@ -60,29 +58,29 @@
 ## Python 3.8 and up
 The use of virtual environments is recommended. Anaconda Python and Enthought EDM are great choices as the main environment in any OS, but overall any Python distribution should do the work. The only limitation in Windows is that wheels for the latest versions of pyopencl are available for Python >=3.8. For Apple Silicon systems, it is recommended to use a native Python for arm64 (see below details).
 
 ## CUDA (For Windows and Linux)
 The code has been verified to work from CUDA 9 to CUDA 11. Highly likely older versions of CUDA (7, 8) should work without a problem. Be sure of installing the CUDA samples and take note of the location where they were installed.
 
 ## CMAKE
-CMAKE version>= 3.16.3. 
+CMAKE version>= 3.16.3.
 
 ## OpenCL
 OpenCL for Windows and Apple Silicon systems is operational via `pyopencl`. In macOS, you can install pyopencl with `pip install pyopencl`. In Windows, use one of the precompiled wheels in https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl. The FDTD kernels code is OpenCL >= 1.2 compliant.
 
 ### Basic Python dependencies:
 latest version of `pip`
 * numpy>=1.15.1 (have this already installed if starting from a clean environment)
 * scipy>=1.1.0 (have this already installed if starting from a clean environment)
 * h5py>=2.9.0 (in native arm64 Python for Apple Silicon, install this via `conda install h5py`)
 * hdf5plugin>=3.2.0
 * pydicom>=1.3.0
 * setuptools >=51.0.0
 * pyopencl>=2020 (if in Windows, install manually a wheel from https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl)
-* cupy-cuda11x in Linux (via pip). In Windows install with conda in windows with `conda install -c conda-forge cupy` 
+* cupy-cuda11x in Linux (via pip). In Windows install with conda in windows with `conda install -c conda-forge cupy`
 
 `h5py`, `hdf5plugin`, `pydicom` and `pyopencl` are installed automatically as requirements if they are no present in the Python enviroment..
 
 ### macOS systems: Manual installation of modified `metalcompute`
 As noted in the release notes below for v0.9.9.20, we use a modified version of `py-metal-compute`. To avoid confusing with the original library, the modified version needs to be installed manually with
 
 `pip install  git+https://github.com/ProteusMRIgHIFU/py-metal-compute.git`
@@ -123,40 +121,48 @@
 Overall, any LTS-type distribution is recommended to be sure CUDA compiler supports your default GCC installation. If your installation can run the default examples of CUDA, then you should be good.
 
 You may also need to install OpenCL headers and libraries such as `opencl-headers`, `ocl-icd-opencl-dev`, `intel-opencl-icd` and other libraries required by you GPU manufacturer to support OpenCL. You can verify you have a healthy OpenCL installation with the tool `clinfo`.
 
 #### Linux in Windows through WSL2
 Starting in 2020, support for CUDA execution directly in WSL2 became possible. We have had excellent experiences with it. Just follow the official instructions from NVIDIA (https://docs.nvidia.com/cuda/wsl-user-guide/index.html)
 
-Please note that OpenCL is not supported under WSL2. 
+Please note that OpenCL is not supported under WSL2.
 
 ### Windows native
 You will need a VStudio installation that is compatible with your CUDA version; for example, CUDA 11.2 supports officially VS 2015 to 2019.
 
 ### macOS
 Any recent version of macOS and XCode with the command-line tools should be enough. Most tests have been done in Big Slur and Monterey. The CPU version in macOS supports OpenMP in ARM64 processors (M1, M1 Max, M2 ultra, M2). In X86-64, the OpenMP feature is now turned as experimental; by default, it will run only single-thread. See below for details on how to enable it. For ARM64 version will have OpenMP fully enabled by default.
 
-The OpenCL and Metal backed have been tested in Intel-based integrated GPUs, AMD GPUs and  ARM64-based systems. There are, however, some limitations of AMD GPUs with OpenCL (see below macOS notes for more details). Metal backend is available for both X86-64 and Apple Silicon systems. Overall, Metal is the recommended backend for M1 processors and AMD GPUs. 
+The OpenCL and Metal backed have been tested in Intel-based integrated GPUs, AMD GPUs and  ARM64-based systems. There are, however, some limitations of AMD GPUs with OpenCL (see below macOS notes for more details). Metal backend is available for both X86-64 and Apple Silicon systems. Overall, Metal is the recommended backend for M1 processors and AMD GPUs.
 
 Best scenario for both X64 and ARM64-based systems is to use fully native Python distributions using homebrew:
 1. Install  [homebrew](https://brew.sh/)
 `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
 1. Install miniforge
 `brew install miniforge`
 1. Create and activate a Python environment (for ARM64, Python 3.9 is recommended)
 `conda create —-name Babel python=3.9 scipy numpy`
 `conda activate Babel`
 1. Install BabelViscoFDTD
 `pip install BabelViscoFDTD`
 
 #### macOS experimental OpenMP in X86-64
+
 Thanks to the people who have reported the mitigated success with OpenMP. In my current systems, I didn't have problems, but later some users reported having issues with OpenMP. Then, we turned this feature as **experimental**, the time we can figure out a more stable approach.
-For X86-64, `libomp` and `mkl` must be installed first, otherwise compilation and execution for OpenMP will fail.
-* Install `libomp` with `brew install libomp`  
-* Install `mkl` with `pip install mkl` or `conda install mkl`
+For Intel or Apple Silicon CPU, `libomp` and `mkl` must be installed first, otherwise compilation and execution for OpenMP will fail.
+Install `mkl` with `pip install mkl` or `conda install mkl`
+
+Using Homebrew, install OpenMP and hint location to CMake:
+
+```sh
+brew install libomp
+
+export OpenMP_ROOT=/opt/homebrew/opt/libomp
+```
 
 
 To enable the OpenMP version for macOS install BabelViscoFDTD with:
 ```
 BABEL_MAC_OPENMP_X64=1 pip install BabelViscoFDTD
 ```
 or if you cloned the repository
@@ -181,30 +187,30 @@
 ### Multi-platform single code
 The underlying GPU code (start at `StaggeredFDTD_3D_With_Relaxation_<xx>.py` files) uses extensively C macros to provide a fully agnostic implementation that remains as efficient as possible regardless of using a CPU or GPU backend. It supports via macro definitions compilation for native CPU (X86, arm64), CUDA, OpenCL and Metal architectures; single or double precision.
 
 Regardless if using CUDA, OpenCL or Metal, conceptually the workflow is very similar. However, there are a few implementation details that need to be handled. cupy, pyopencl and metalcompute libraries help to minimize the amount the coding while still providing best performance possible with each backend.
 
 # Important information specific to the different environments for use
 ### macOS notes
-macOS support for HPC has shifted in recent years significantly. In modern macOS versions, the support for NVIDIA cards is inexistent and OpenCL *was supposed to be* officially out of support beyond Big Slur (*it is still running quite well in Monterey*). For macOS, Metal backend is recommended for AMD processors. OpenCL in macOS X86_64 may have other limitations such as the underlying driver may only support 32 bits memory access, even if the card has more than 4 GB of RAM. However, this limitation seems to be case by case. For ARM64 processors, OpenCL drivers can support 64 bit addressing. For an AMD W6800 (32 GB RAM) it only supports 32 bits. The `clinfo` tool (available with homebrew) can provide details if your current GPU and drivers support 64 bits addressing. The OpenCL implementation with ARM64 processors works only with a native Python arm64 installation. 
+macOS support for HPC has shifted in recent years significantly. In modern macOS versions, the support for NVIDIA cards is inexistent and OpenCL *was supposed to be* officially out of support beyond Big Slur (*it is still running quite well in Monterey*). For macOS, Metal backend is recommended for AMD processors. OpenCL in macOS X86_64 may have other limitations such as the underlying driver may only support 32 bits memory access, even if the card has more than 4 GB of RAM. However, this limitation seems to be case by case. For ARM64 processors, OpenCL drivers can support 64 bit addressing. For an AMD W6800 (32 GB RAM) it only supports 32 bits. The `clinfo` tool (available with homebrew) can provide details if your current GPU and drivers support 64 bits addressing. The OpenCL implementation with ARM64 processors works only with a native Python arm64 installation.
 
 ### Metal support
-Overall, Metal requires a bit more coding to prepare the pipelines for compute execution.  A challenge is that Metal for scientific computing still lacks serious examples. Nevertheless, the support for Metal is desirable for Apple Silicon systems. As toolchains, including native Python in arm64, are now becoming widespread available, it is interesting to see how well these devices stand quite well compared to Nvidia or AMD-based systems. There are some limitations such as the maximal number of kernel parameters (32) and that each GPU buffer memory is limited to 3.5 GB RAM for Metal-supported GPUs. But this is a limitation manageable by packing multiple logical arrays across multiple buffers. We explored the use of Metal Argument Buffers, but it ended in poorer performance than packing multiple arrays logically. In the current release of BabelViscoFDTD, it is completely stable to run large domains with AMD GPUs and ARM64-based processors with 32 or more GB of RAM. 
+Overall, Metal requires a bit more coding to prepare the pipelines for compute execution.  A challenge is that Metal for scientific computing still lacks serious examples. Nevertheless, the support for Metal is desirable for Apple Silicon systems. As toolchains, including native Python in arm64, are now becoming widespread available, it is interesting to see how well these devices stand quite well compared to Nvidia or AMD-based systems. There are some limitations such as the maximal number of kernel parameters (32) and that each GPU buffer memory is limited to 3.5 GB RAM for Metal-supported GPUs. But this is a limitation manageable by packing multiple logical arrays across multiple buffers. We explored the use of Metal Argument Buffers, but it ended in poorer performance than packing multiple arrays logically. In the current release of BabelViscoFDTD, it is completely stable to run large domains with AMD GPUs and ARM64-based processors with 32 or more GB of RAM.
 
 While Metal offers better performance overall over OpenCL in both Apple and AMD processors, some issues remain. Extensive testing has indicated that the Python process freezes after running a few tens of thousands of kernel calls. For most of the applications, this won't be an issue. If running very long extensive parametric studies under a single execution, be aware you may need to split your execution into chunks that can be called in separate `python <Myprogram.py>` calls. I suspect some driver issue limiting the number of consecutive kernels calls in a single process.
 
 ## Single precision performance comparison
 Performance between modern AMD, NVIDIA and Apple Silicon GPUs can show important differences. A simulation for a domain of  [414, 219 , 375] grid size and over 2841 temporal steps was used to benchmark multiple backends and systems.
 
 * Nvidia RTX A6000 (48 GB RAM, 10752 CUDA Cores, theoretical 38.7 SP TFLOP , memory bandwidth 768 GB/s)
-* AMD Radeon Pro W6800 (32 GB RAM, 3840  stream processors, theoretical 17.83 SP TFLOP, memory bandwidth 512 GB/s) 
-* AMD Vega 56 (8 GB RAM, 3584  stream processors, theoretical 10.5 SP TFLOP, memory bandwidth  410 GB/s) 
+* AMD Radeon Pro W6800 (32 GB RAM, 3840  stream processors, theoretical 17.83 SP TFLOP, memory bandwidth 512 GB/s)
+* AMD Vega 56 (8 GB RAM, 3584  stream processors, theoretical 10.5 SP TFLOP, memory bandwidth  410 GB/s)
 * M1 Max  (64 GB RAM, 10 CPU cores, 32 GPU Cores, 4096 execution units (which PR material says translates into a theoretical 98304 simultaneous threads), theoretical 10.4 SP TFLOP, memory bandwidth 400 GB/s)
 
-RTX A6000 test was done in 128 GB Xeon W-2125 CPU (4x2 cores) @ 4.00GHz Dell system. AMD Vega 64 and AMD Radeon Pro W6800 were tested in an 128 GB iMac Pro system (10x2 Core Intel Xeon W). The Vega 64 GPU is part of the iMac system, while the Pro W6800 is connected via a Thunderbolt 3 external enclosure. Please note that GPU connectivity should not have an important effect given memory transfers between GPU and CPU are minimal. The M1 Max was configured with 64 GB and installed in a 2021 MacBook Pro system. The Dell system, iMac Pro and MacBook Pro were also used for OpenMP benchmarks. Python 3.9 was used in all systems. The Dell system test used CUDA 11.4 and Visual Studio 2019 Community edition. The latest versions of pycuda and pyopencl at the time of testing (Sep 18, 2022) were used. macOS Monterey 12.5.1 with XCode 14 were used for both iMac Pro and MacBook Pro. 
+RTX A6000 test was done in 128 GB Xeon W-2125 CPU (4x2 cores) @ 4.00GHz Dell system. AMD Vega 64 and AMD Radeon Pro W6800 were tested in an 128 GB iMac Pro system (10x2 Core Intel Xeon W). The Vega 64 GPU is part of the iMac system, while the Pro W6800 is connected via a Thunderbolt 3 external enclosure. Please note that GPU connectivity should not have an important effect given memory transfers between GPU and CPU are minimal. The M1 Max was configured with 64 GB and installed in a 2021 MacBook Pro system. The Dell system, iMac Pro and MacBook Pro were also used for OpenMP benchmarks. Python 3.9 was used in all systems. The Dell system test used CUDA 11.4 and Visual Studio 2019 Community edition. The latest versions of pycuda and pyopencl at the time of testing (Sep 18, 2022) were used. macOS Monterey 12.5.1 with XCode 14 were used for both iMac Pro and MacBook Pro.
 
 Wall-time was measured from the moment preparations to run GPU code started (initiate device operation) to the end of the memory transfer of results, with no access to the main drives involved. Memory transfer between CPU and GPU occurred only at the beginning and end of GPU execution. The numerical difference among different backends was in the order of single precision resolution.
 
 ### Summary of wall-time results for each device
 | Device |  CUDA single | OpenCL single |  Metal single | OpenMP single|
 | --- | --- |  --- |  --- |  ---  |
 | AMD W6800 | - | - |  68 s | - |
@@ -213,59 +219,58 @@
 | M1 Max | - |  94 s |92 s| 1546 s (10 threads) |
 | Xeon W-2125 | - | - | - | 5163 s (8 threads)|
 | iMac Pro (Xeon W) | - | - | - | 2982 s  (20 threads)|
 
 #### Discussion of results
 The number of computing units is becoming a bit useless to compare. There are a few interesting aspects worth mentioning:
 * The ratio of performance between M1 Max and A6000 (CUDA vs. Metal) is not even close to the theoretical difference of raw SP TFLOPS%.
-* Metal and OpenCL performances of the M1 Max are pretty much equal, outmatching the A6000 performance. 
+* Metal and OpenCL performances of the M1 Max are pretty much equal, outmatching the A6000 performance.
 * Multiple tryouts on the CUDA code to adjust grid and block sizes didn't improve performance in the A6000. On the contrary, wall-time was increased, indicating that the recommended method by Nvidia to calculate maximal occupancy used by default in BabelViscoFDTD provided the best performance with the A6000.
-* The other surprise was the W6800 with Metal and OpenCL outperforming by a significant margin the A6000. 
-* The OpenMP performance of the M1 Max is also excellent, showing a dramatic speedup compared to the Dell Xeon and iMac Pro systems. 
+* The other surprise was the W6800 with Metal and OpenCL outperforming by a significant margin the A6000.
+* The OpenMP performance of the M1 Max is also excellent, showing a dramatic speedup compared to the Dell Xeon and iMac Pro systems.
 
 ## Possibility of manual adjustments to improve performance
-All three GPU backends have analogous control to split the calculations in the GPU multiprocessors. BabelViscoFDTD uses the methods that are recommended for each backend to ensure maximal GPU occupancy. However, manual adjustments can provide improvement to the performance. You can specify manually the grid and thread block dimensions with the optional parameters `ManualGroupSize` and `ManualLocalSize`, respectively. Please consult the guidelines of each backend (CUDA, OpenCL and Metal) on how to calculate this correctly, otherwise there is a risk of specifying a too large or too short grid and thread size dimensions. For example, for both CUDA and Metal, the multiplication of `ManualGroupSize` and `ManualLocalSize` must be equal or larger than the domain size ([N1,N2,N3]) to ensure all the domain is covered; for example for a domain of size [231,220,450], `ManualGroupSize=[60,60,115]` with `ManualLocalSize=[4,4,4]` will ensure covering the domain size. For `OpenCL` each entry in `ManualGroupSize` must be equal or larger than [N1,N2,N3] and each entry must be a multiple of its corresponding entry in `ManualLocalSize`; for example for a domain of size [231,220,450], `ManualGroupSize=[240,240,460]` with `ManualLocalSize=[4,4,4]`. Be sure of specifying these parameters as an np.array of type np.int32, such as `ManualLocalSize=np.array([4,4,4]).astype(np.int32)`. 
+All three GPU backends have analogous control to split the calculations in the GPU multiprocessors. BabelViscoFDTD uses the methods that are recommended for each backend to ensure maximal GPU occupancy. However, manual adjustments can provide improvement to the performance. You can specify manually the grid and thread block dimensions with the optional parameters `ManualGroupSize` and `ManualLocalSize`, respectively. Please consult the guidelines of each backend (CUDA, OpenCL and Metal) on how to calculate this correctly, otherwise there is a risk of specifying a too large or too short grid and thread size dimensions. For example, for both CUDA and Metal, the multiplication of `ManualGroupSize` and `ManualLocalSize` must be equal or larger than the domain size ([N1,N2,N3]) to ensure all the domain is covered; for example for a domain of size [231,220,450], `ManualGroupSize=[60,60,115]` with `ManualLocalSize=[4,4,4]` will ensure covering the domain size. For `OpenCL` each entry in `ManualGroupSize` must be equal or larger than [N1,N2,N3] and each entry must be a multiple of its corresponding entry in `ManualLocalSize`; for example for a domain of size [231,220,450], `ManualGroupSize=[240,240,460]` with `ManualLocalSize=[4,4,4]`. Be sure of specifying these parameters as an np.array of type np.int32, such as `ManualLocalSize=np.array([4,4,4]).astype(np.int32)`.
 
 # Supported platforms for Rayleigh's integral
-Since v0.9.2 Rayleigh-Sommerfeld's integral was added as a tool (see tutorial `Tutorial Notebooks\Tools -1 - Rayleigh Integral.ipynb`). This will be useful to combine models that include large volumes of water as the Rayleigh integral benefits considerably a GPU as the Rayleigh-Sommerfeld integral is hyper-parallel. The tool has support for 3 GPU backends: CUDA and OpenCL for Windows and Linux, and Metal and OpenCL for macOS. 
+Since v0.9.2 Rayleigh-Sommerfeld's integral was added as a tool (see tutorial `Tutorial Notebooks\Tools -1 - Rayleigh Integral.ipynb`). This will be useful to combine models that include large volumes of water as the Rayleigh integral benefits considerably a GPU as the Rayleigh-Sommerfeld integral is hyper-parallel. The tool has support for 3 GPU backends: CUDA and OpenCL for Windows and Linux, and Metal and OpenCL for macOS.
 
 # Release notes
+* 1.0.0-1 - To fix pip version that had an incorrect file for OpenCL BHTE
 * 1.0.0 - That is it! After thousands of simulations for a manuscript preparation to introduce the [BabelBrain](https://github.com/ProteusMRIgHIFU/BabelBrain) planning suite (Now public), this is ready for an official 1.0.0 release. 
     * cupy replaces PyCUDA for all CUDA operations. PyCUDA needs a Visual Studio compiler on the path to compile kernels in Windows. BabelBrain uses a lot cupy; switching to it helps to keep using a single interface while benefitting from the availability of Numpy-like methods.
     * Add a new correction parameter for attenuation. One of the findings while preparing the use with BabelBrain was that mapping procedures in the literature linking CT Hounsfield Units (HU) to the speed of sound and, especially, attenuation needs this sort of correction.
 * 0.9.10-1 Nov 16, 2022
-    * Add functions to list devices supported by computing backends 
+    * Add functions to list devices supported by computing backends
 * 0.9.10 Oct 28, 2022
     * Fix the issue with mapping of unique values when attenuation is used, it could cause some divisions by zero
 * 0.9.9.20 Sep 17, 2022
-    * A lot of important improvements to make the final line  
+    * A lot of important improvements to make the final line
         - Metal is (finally) running as fast (sometimes slightly faster) than OpenCL in Apple processors. It took a lot of testing and fine tuning.
         - Use of a modified version of the excellent `py-metal-compute` library (https://github.com/baldand/py-metal-compute) that allows having a similar approach as with pyopencl, cupy and pycuda. Modified library is at https://github.com/ProteusMRIgHIFU/py-metal-compute. Because of this new approach, the old Swift interface to the FDTD code was removed.
         - Add Metal backend for BHTE tool. This version runs way faster than OpenCL in Apple processors (like a 10x factor, need to investigate more if we can replicate such gain)
         - Benchmark metrics above were refreshed
         - Moving forward, OpenCL is not recommended for macOS in X64 systems. Because of the limitation of the underlying 32-bit addressing, pyopencl does not catch easily when a simulation goes beyond 4GB. However, Metal for AMD in macOS runs quite well, so no need to stick with OpenCL
 
 * 0.9.9  Sep 1, 2022
-    * A lot of simplifications allowed having a much more straightforward code. Thanks to Andrew Xie (@IAmAndrewX) for a very productive summer trimming down code, replacing the old MTLPP with Swift, and making a new class arrangement for the different GPU backends. Now BabelViscoFDTD is based completely on pyopencl and pycuda for the FDTD viscoelastic solver. For Metal, the Swift-based wrapper does the interfacing. The old C extension is still around just for the OpenMP backend.  
+    * A lot of simplifications allowed having a much more straightforward code. Thanks to Andrew Xie (@IAmAndrewX) for a very productive summer trimming down code, replacing the old MTLPP with Swift, and making a new class arrangement for the different GPU backends. Now BabelViscoFDTD is based completely on pyopencl and pycuda for the FDTD viscoelastic solver. For Metal, the Swift-based wrapper does the interfacing. The old C extension is still around just for the OpenMP backend.
 * 0.9.7  July 7, 2022
-    * The MTLPP C++ library is now replaced by a Swift interface to access the Metal implementation for the viscoelastic FDTD solution. This will ensure using a more standard Apple development language for the future, as MTLPP is not maintained anymore. While there is a new Apple-based C++ wrapper for Metal, using Swift is still preferred as we created now a C-linking compatible library that in the future can be also used directly in Python. In the long term, we aim to eliminate the C code extension and use only Python code in tandem with pyopencl, pycuda and  Metal 
+    * The MTLPP C++ library is now replaced by a Swift interface to access the Metal implementation for the viscoelastic FDTD solution. This will ensure using a more standard Apple development language for the future, as MTLPP is not maintained anymore. While there is a new Apple-based C++ wrapper for Metal, using Swift is still preferred as we created now a C-linking compatible library that in the future can be also used directly in Python. In the long term, we aim to eliminate the C code extension and use only Python code in tandem with pyopencl, pycuda and  Metal
 * 0.9.6-post-10  June 27, 2022
     * A fix for OpenCL in X64 Mac system that was missing the new kernel names
     * OpenMP for X64 in Mac is being turned back as experimental feature as some systems are unable to run with it correctly and there is not a clear path on how to ensure this will be stable. The feature will remain accessible if installing the library with the BABEL_MAC_OPENMP_X64 option enabled.
 * 0.9.6  Feb 5, 2022.
     * Improved performance in Metal-based devices by using mini-kernels.
     * Minor fixes for Rayleigh-Sommerfeld in Metal
 * 0.9.5  Jan 18, 2022.
     * Very first pip-registered version
     * Possibility of user-specified dimensions of blocks for computations for fine-tuning performance
     * Cleaning some minor bugs and adding BHTE code using pycuda and pyopencl.
-    
+
 * 0.9.3  Sep 29, 2021.
     * Improved support for both Metal and OpenCL. For Metal, stable operation is now feasible for large domains using all available memory in modern high-end GPUs. OpenCL is now supported in all OSs.
 * 0.9.2  June 13, 2021.
     * Add Rayleigh integral support in a homogenous medium with CUDA, OpenCL and Metal backends.
     * Support for stress sources
     * Able to select devices in multiple GPU systems with CUDA
 * 0.9.1  Feb 17, 2021. Pressure calculation added in low-level function.
 * 0.9.0  Dec 2020. First porting from the private repository and big reorganization to make it more user friendly
-
-
```

### Comparing `BabelViscoFDTD-1.0.0/README.md` & `BabelViscoFDTD-1.0.0.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 BabelViscoFDTD
 =============
-Samuel Pichardo, Ph.D  
-Associate Professor  
-Radiology and Clinical Neurosciences, Hotchkiss Brain Institute  
-Cumming School of Medicine,  
-University of Calgary   
-samuel.pichardo@ucalgary.ca  
+Samuel Pichardo, Ph.D
+Associate Professor
+Radiology and Clinical Neurosciences, Hotchkiss Brain Institute
+Cumming School of Medicine,
+University of Calgary
+samuel.pichardo@ucalgary.ca
 www.neurofus.ca
 
 **Software library for FDTD of the viscoelastic equation using a staggered grid arrangement and including the superposition method, with multiple CPU- and GPU-based backends (OpenMP, CUDA, OpenCL and Metal)**
 
 This tool solves in the time domain the viscoelastic equation for wave propagation using a staggered grid solution. The solution is primarily based on a paper from Virieux (Virieux, J., 1986. P-SV wave propagation in heterogeneous media: Velocity-stress finite-difference method. Geophysics, 51(4), pp.889-901.), who implemented for the first time the staggered grid solution for the viscoelastic equation.
  While the underlying equations and methods were developed primarily for seismic simulation, the BabelViscoFDTD library was developed for biomedical applications to study the ultrasound transmission through bone material, with skull bone as the primary target for study.
 
@@ -44,29 +44,29 @@
 ## Python 3.8 and up
 The use of virtual environments is recommended. Anaconda Python and Enthought EDM are great choices as the main environment in any OS, but overall any Python distribution should do the work. The only limitation in Windows is that wheels for the latest versions of pyopencl are available for Python >=3.8. For Apple Silicon systems, it is recommended to use a native Python for arm64 (see below details).
 
 ## CUDA (For Windows and Linux)
 The code has been verified to work from CUDA 9 to CUDA 11. Highly likely older versions of CUDA (7, 8) should work without a problem. Be sure of installing the CUDA samples and take note of the location where they were installed.
 
 ## CMAKE
-CMAKE version>= 3.16.3. 
+CMAKE version>= 3.16.3.
 
 ## OpenCL
 OpenCL for Windows and Apple Silicon systems is operational via `pyopencl`. In macOS, you can install pyopencl with `pip install pyopencl`. In Windows, use one of the precompiled wheels in https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl. The FDTD kernels code is OpenCL >= 1.2 compliant.
 
 ### Basic Python dependencies:
 latest version of `pip`
 * numpy>=1.15.1 (have this already installed if starting from a clean environment)
 * scipy>=1.1.0 (have this already installed if starting from a clean environment)
 * h5py>=2.9.0 (in native arm64 Python for Apple Silicon, install this via `conda install h5py`)
 * hdf5plugin>=3.2.0
 * pydicom>=1.3.0
 * setuptools >=51.0.0
 * pyopencl>=2020 (if in Windows, install manually a wheel from https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl)
-* cupy-cuda11x in Linux (via pip). In Windows install with conda in windows with `conda install -c conda-forge cupy` 
+* cupy-cuda11x in Linux (via pip). In Windows install with conda in windows with `conda install -c conda-forge cupy`
 
 `h5py`, `hdf5plugin`, `pydicom` and `pyopencl` are installed automatically as requirements if they are no present in the Python enviroment..
 
 ### macOS systems: Manual installation of modified `metalcompute`
 As noted in the release notes below for v0.9.9.20, we use a modified version of `py-metal-compute`. To avoid confusing with the original library, the modified version needs to be installed manually with
 
 `pip install  git+https://github.com/ProteusMRIgHIFU/py-metal-compute.git`
@@ -107,40 +107,48 @@
 Overall, any LTS-type distribution is recommended to be sure CUDA compiler supports your default GCC installation. If your installation can run the default examples of CUDA, then you should be good.
 
 You may also need to install OpenCL headers and libraries such as `opencl-headers`, `ocl-icd-opencl-dev`, `intel-opencl-icd` and other libraries required by you GPU manufacturer to support OpenCL. You can verify you have a healthy OpenCL installation with the tool `clinfo`.
 
 #### Linux in Windows through WSL2
 Starting in 2020, support for CUDA execution directly in WSL2 became possible. We have had excellent experiences with it. Just follow the official instructions from NVIDIA (https://docs.nvidia.com/cuda/wsl-user-guide/index.html)
 
-Please note that OpenCL is not supported under WSL2. 
+Please note that OpenCL is not supported under WSL2.
 
 ### Windows native
 You will need a VStudio installation that is compatible with your CUDA version; for example, CUDA 11.2 supports officially VS 2015 to 2019.
 
 ### macOS
 Any recent version of macOS and XCode with the command-line tools should be enough. Most tests have been done in Big Slur and Monterey. The CPU version in macOS supports OpenMP in ARM64 processors (M1, M1 Max, M2 ultra, M2). In X86-64, the OpenMP feature is now turned as experimental; by default, it will run only single-thread. See below for details on how to enable it. For ARM64 version will have OpenMP fully enabled by default.
 
-The OpenCL and Metal backed have been tested in Intel-based integrated GPUs, AMD GPUs and  ARM64-based systems. There are, however, some limitations of AMD GPUs with OpenCL (see below macOS notes for more details). Metal backend is available for both X86-64 and Apple Silicon systems. Overall, Metal is the recommended backend for M1 processors and AMD GPUs. 
+The OpenCL and Metal backed have been tested in Intel-based integrated GPUs, AMD GPUs and  ARM64-based systems. There are, however, some limitations of AMD GPUs with OpenCL (see below macOS notes for more details). Metal backend is available for both X86-64 and Apple Silicon systems. Overall, Metal is the recommended backend for M1 processors and AMD GPUs.
 
 Best scenario for both X64 and ARM64-based systems is to use fully native Python distributions using homebrew:
 1. Install  [homebrew](https://brew.sh/)
 `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
 1. Install miniforge
 `brew install miniforge`
 1. Create and activate a Python environment (for ARM64, Python 3.9 is recommended)
 `conda create —-name Babel python=3.9 scipy numpy`
 `conda activate Babel`
 1. Install BabelViscoFDTD
 `pip install BabelViscoFDTD`
 
 #### macOS experimental OpenMP in X86-64
+
 Thanks to the people who have reported the mitigated success with OpenMP. In my current systems, I didn't have problems, but later some users reported having issues with OpenMP. Then, we turned this feature as **experimental**, the time we can figure out a more stable approach.
-For X86-64, `libomp` and `mkl` must be installed first, otherwise compilation and execution for OpenMP will fail.
-* Install `libomp` with `brew install libomp`  
-* Install `mkl` with `pip install mkl` or `conda install mkl`
+For Intel or Apple Silicon CPU, `libomp` and `mkl` must be installed first, otherwise compilation and execution for OpenMP will fail.
+Install `mkl` with `pip install mkl` or `conda install mkl`
+
+Using Homebrew, install OpenMP and hint location to CMake:
+
+```sh
+brew install libomp
+
+export OpenMP_ROOT=/opt/homebrew/opt/libomp
+```
 
 
 To enable the OpenMP version for macOS install BabelViscoFDTD with:
 ```
 BABEL_MAC_OPENMP_X64=1 pip install BabelViscoFDTD
 ```
 or if you cloned the repository
@@ -165,30 +173,30 @@
 ### Multi-platform single code
 The underlying GPU code (start at `StaggeredFDTD_3D_With_Relaxation_<xx>.py` files) uses extensively C macros to provide a fully agnostic implementation that remains as efficient as possible regardless of using a CPU or GPU backend. It supports via macro definitions compilation for native CPU (X86, arm64), CUDA, OpenCL and Metal architectures; single or double precision.
 
 Regardless if using CUDA, OpenCL or Metal, conceptually the workflow is very similar. However, there are a few implementation details that need to be handled. cupy, pyopencl and metalcompute libraries help to minimize the amount the coding while still providing best performance possible with each backend.
 
 # Important information specific to the different environments for use
 ### macOS notes
-macOS support for HPC has shifted in recent years significantly. In modern macOS versions, the support for NVIDIA cards is inexistent and OpenCL *was supposed to be* officially out of support beyond Big Slur (*it is still running quite well in Monterey*). For macOS, Metal backend is recommended for AMD processors. OpenCL in macOS X86_64 may have other limitations such as the underlying driver may only support 32 bits memory access, even if the card has more than 4 GB of RAM. However, this limitation seems to be case by case. For ARM64 processors, OpenCL drivers can support 64 bit addressing. For an AMD W6800 (32 GB RAM) it only supports 32 bits. The `clinfo` tool (available with homebrew) can provide details if your current GPU and drivers support 64 bits addressing. The OpenCL implementation with ARM64 processors works only with a native Python arm64 installation. 
+macOS support for HPC has shifted in recent years significantly. In modern macOS versions, the support for NVIDIA cards is inexistent and OpenCL *was supposed to be* officially out of support beyond Big Slur (*it is still running quite well in Monterey*). For macOS, Metal backend is recommended for AMD processors. OpenCL in macOS X86_64 may have other limitations such as the underlying driver may only support 32 bits memory access, even if the card has more than 4 GB of RAM. However, this limitation seems to be case by case. For ARM64 processors, OpenCL drivers can support 64 bit addressing. For an AMD W6800 (32 GB RAM) it only supports 32 bits. The `clinfo` tool (available with homebrew) can provide details if your current GPU and drivers support 64 bits addressing. The OpenCL implementation with ARM64 processors works only with a native Python arm64 installation.
 
 ### Metal support
-Overall, Metal requires a bit more coding to prepare the pipelines for compute execution.  A challenge is that Metal for scientific computing still lacks serious examples. Nevertheless, the support for Metal is desirable for Apple Silicon systems. As toolchains, including native Python in arm64, are now becoming widespread available, it is interesting to see how well these devices stand quite well compared to Nvidia or AMD-based systems. There are some limitations such as the maximal number of kernel parameters (32) and that each GPU buffer memory is limited to 3.5 GB RAM for Metal-supported GPUs. But this is a limitation manageable by packing multiple logical arrays across multiple buffers. We explored the use of Metal Argument Buffers, but it ended in poorer performance than packing multiple arrays logically. In the current release of BabelViscoFDTD, it is completely stable to run large domains with AMD GPUs and ARM64-based processors with 32 or more GB of RAM. 
+Overall, Metal requires a bit more coding to prepare the pipelines for compute execution.  A challenge is that Metal for scientific computing still lacks serious examples. Nevertheless, the support for Metal is desirable for Apple Silicon systems. As toolchains, including native Python in arm64, are now becoming widespread available, it is interesting to see how well these devices stand quite well compared to Nvidia or AMD-based systems. There are some limitations such as the maximal number of kernel parameters (32) and that each GPU buffer memory is limited to 3.5 GB RAM for Metal-supported GPUs. But this is a limitation manageable by packing multiple logical arrays across multiple buffers. We explored the use of Metal Argument Buffers, but it ended in poorer performance than packing multiple arrays logically. In the current release of BabelViscoFDTD, it is completely stable to run large domains with AMD GPUs and ARM64-based processors with 32 or more GB of RAM.
 
 While Metal offers better performance overall over OpenCL in both Apple and AMD processors, some issues remain. Extensive testing has indicated that the Python process freezes after running a few tens of thousands of kernel calls. For most of the applications, this won't be an issue. If running very long extensive parametric studies under a single execution, be aware you may need to split your execution into chunks that can be called in separate `python <Myprogram.py>` calls. I suspect some driver issue limiting the number of consecutive kernels calls in a single process.
 
 ## Single precision performance comparison
 Performance between modern AMD, NVIDIA and Apple Silicon GPUs can show important differences. A simulation for a domain of  [414, 219 , 375] grid size and over 2841 temporal steps was used to benchmark multiple backends and systems.
 
 * Nvidia RTX A6000 (48 GB RAM, 10752 CUDA Cores, theoretical 38.7 SP TFLOP , memory bandwidth 768 GB/s)
-* AMD Radeon Pro W6800 (32 GB RAM, 3840  stream processors, theoretical 17.83 SP TFLOP, memory bandwidth 512 GB/s) 
-* AMD Vega 56 (8 GB RAM, 3584  stream processors, theoretical 10.5 SP TFLOP, memory bandwidth  410 GB/s) 
+* AMD Radeon Pro W6800 (32 GB RAM, 3840  stream processors, theoretical 17.83 SP TFLOP, memory bandwidth 512 GB/s)
+* AMD Vega 56 (8 GB RAM, 3584  stream processors, theoretical 10.5 SP TFLOP, memory bandwidth  410 GB/s)
 * M1 Max  (64 GB RAM, 10 CPU cores, 32 GPU Cores, 4096 execution units (which PR material says translates into a theoretical 98304 simultaneous threads), theoretical 10.4 SP TFLOP, memory bandwidth 400 GB/s)
 
-RTX A6000 test was done in 128 GB Xeon W-2125 CPU (4x2 cores) @ 4.00GHz Dell system. AMD Vega 64 and AMD Radeon Pro W6800 were tested in an 128 GB iMac Pro system (10x2 Core Intel Xeon W). The Vega 64 GPU is part of the iMac system, while the Pro W6800 is connected via a Thunderbolt 3 external enclosure. Please note that GPU connectivity should not have an important effect given memory transfers between GPU and CPU are minimal. The M1 Max was configured with 64 GB and installed in a 2021 MacBook Pro system. The Dell system, iMac Pro and MacBook Pro were also used for OpenMP benchmarks. Python 3.9 was used in all systems. The Dell system test used CUDA 11.4 and Visual Studio 2019 Community edition. The latest versions of pycuda and pyopencl at the time of testing (Sep 18, 2022) were used. macOS Monterey 12.5.1 with XCode 14 were used for both iMac Pro and MacBook Pro. 
+RTX A6000 test was done in 128 GB Xeon W-2125 CPU (4x2 cores) @ 4.00GHz Dell system. AMD Vega 64 and AMD Radeon Pro W6800 were tested in an 128 GB iMac Pro system (10x2 Core Intel Xeon W). The Vega 64 GPU is part of the iMac system, while the Pro W6800 is connected via a Thunderbolt 3 external enclosure. Please note that GPU connectivity should not have an important effect given memory transfers between GPU and CPU are minimal. The M1 Max was configured with 64 GB and installed in a 2021 MacBook Pro system. The Dell system, iMac Pro and MacBook Pro were also used for OpenMP benchmarks. Python 3.9 was used in all systems. The Dell system test used CUDA 11.4 and Visual Studio 2019 Community edition. The latest versions of pycuda and pyopencl at the time of testing (Sep 18, 2022) were used. macOS Monterey 12.5.1 with XCode 14 were used for both iMac Pro and MacBook Pro.
 
 Wall-time was measured from the moment preparations to run GPU code started (initiate device operation) to the end of the memory transfer of results, with no access to the main drives involved. Memory transfer between CPU and GPU occurred only at the beginning and end of GPU execution. The numerical difference among different backends was in the order of single precision resolution.
 
 ### Summary of wall-time results for each device
 | Device |  CUDA single | OpenCL single |  Metal single | OpenMP single|
 | --- | --- |  --- |  --- |  ---  |
 | AMD W6800 | - | - |  68 s | - |
@@ -197,56 +205,57 @@
 | M1 Max | - |  94 s |92 s| 1546 s (10 threads) |
 | Xeon W-2125 | - | - | - | 5163 s (8 threads)|
 | iMac Pro (Xeon W) | - | - | - | 2982 s  (20 threads)|
 
 #### Discussion of results
 The number of computing units is becoming a bit useless to compare. There are a few interesting aspects worth mentioning:
 * The ratio of performance between M1 Max and A6000 (CUDA vs. Metal) is not even close to the theoretical difference of raw SP TFLOPS%.
-* Metal and OpenCL performances of the M1 Max are pretty much equal, outmatching the A6000 performance. 
+* Metal and OpenCL performances of the M1 Max are pretty much equal, outmatching the A6000 performance.
 * Multiple tryouts on the CUDA code to adjust grid and block sizes didn't improve performance in the A6000. On the contrary, wall-time was increased, indicating that the recommended method by Nvidia to calculate maximal occupancy used by default in BabelViscoFDTD provided the best performance with the A6000.
-* The other surprise was the W6800 with Metal and OpenCL outperforming by a significant margin the A6000. 
-* The OpenMP performance of the M1 Max is also excellent, showing a dramatic speedup compared to the Dell Xeon and iMac Pro systems. 
+* The other surprise was the W6800 with Metal and OpenCL outperforming by a significant margin the A6000.
+* The OpenMP performance of the M1 Max is also excellent, showing a dramatic speedup compared to the Dell Xeon and iMac Pro systems.
 
 ## Possibility of manual adjustments to improve performance
-All three GPU backends have analogous control to split the calculations in the GPU multiprocessors. BabelViscoFDTD uses the methods that are recommended for each backend to ensure maximal GPU occupancy. However, manual adjustments can provide improvement to the performance. You can specify manually the grid and thread block dimensions with the optional parameters `ManualGroupSize` and `ManualLocalSize`, respectively. Please consult the guidelines of each backend (CUDA, OpenCL and Metal) on how to calculate this correctly, otherwise there is a risk of specifying a too large or too short grid and thread size dimensions. For example, for both CUDA and Metal, the multiplication of `ManualGroupSize` and `ManualLocalSize` must be equal or larger than the domain size ([N1,N2,N3]) to ensure all the domain is covered; for example for a domain of size [231,220,450], `ManualGroupSize=[60,60,115]` with `ManualLocalSize=[4,4,4]` will ensure covering the domain size. For `OpenCL` each entry in `ManualGroupSize` must be equal or larger than [N1,N2,N3] and each entry must be a multiple of its corresponding entry in `ManualLocalSize`; for example for a domain of size [231,220,450], `ManualGroupSize=[240,240,460]` with `ManualLocalSize=[4,4,4]`. Be sure of specifying these parameters as an np.array of type np.int32, such as `ManualLocalSize=np.array([4,4,4]).astype(np.int32)`. 
+All three GPU backends have analogous control to split the calculations in the GPU multiprocessors. BabelViscoFDTD uses the methods that are recommended for each backend to ensure maximal GPU occupancy. However, manual adjustments can provide improvement to the performance. You can specify manually the grid and thread block dimensions with the optional parameters `ManualGroupSize` and `ManualLocalSize`, respectively. Please consult the guidelines of each backend (CUDA, OpenCL and Metal) on how to calculate this correctly, otherwise there is a risk of specifying a too large or too short grid and thread size dimensions. For example, for both CUDA and Metal, the multiplication of `ManualGroupSize` and `ManualLocalSize` must be equal or larger than the domain size ([N1,N2,N3]) to ensure all the domain is covered; for example for a domain of size [231,220,450], `ManualGroupSize=[60,60,115]` with `ManualLocalSize=[4,4,4]` will ensure covering the domain size. For `OpenCL` each entry in `ManualGroupSize` must be equal or larger than [N1,N2,N3] and each entry must be a multiple of its corresponding entry in `ManualLocalSize`; for example for a domain of size [231,220,450], `ManualGroupSize=[240,240,460]` with `ManualLocalSize=[4,4,4]`. Be sure of specifying these parameters as an np.array of type np.int32, such as `ManualLocalSize=np.array([4,4,4]).astype(np.int32)`.
 
 # Supported platforms for Rayleigh's integral
-Since v0.9.2 Rayleigh-Sommerfeld's integral was added as a tool (see tutorial `Tutorial Notebooks\Tools -1 - Rayleigh Integral.ipynb`). This will be useful to combine models that include large volumes of water as the Rayleigh integral benefits considerably a GPU as the Rayleigh-Sommerfeld integral is hyper-parallel. The tool has support for 3 GPU backends: CUDA and OpenCL for Windows and Linux, and Metal and OpenCL for macOS. 
+Since v0.9.2 Rayleigh-Sommerfeld's integral was added as a tool (see tutorial `Tutorial Notebooks\Tools -1 - Rayleigh Integral.ipynb`). This will be useful to combine models that include large volumes of water as the Rayleigh integral benefits considerably a GPU as the Rayleigh-Sommerfeld integral is hyper-parallel. The tool has support for 3 GPU backends: CUDA and OpenCL for Windows and Linux, and Metal and OpenCL for macOS.
 
 # Release notes
+* 1.0.0-1 - To fix pip version that had an incorrect file for OpenCL BHTE
 * 1.0.0 - That is it! After thousands of simulations for a manuscript preparation to introduce the [BabelBrain](https://github.com/ProteusMRIgHIFU/BabelBrain) planning suite (Now public), this is ready for an official 1.0.0 release. 
     * cupy replaces PyCUDA for all CUDA operations. PyCUDA needs a Visual Studio compiler on the path to compile kernels in Windows. BabelBrain uses a lot cupy; switching to it helps to keep using a single interface while benefitting from the availability of Numpy-like methods.
     * Add a new correction parameter for attenuation. One of the findings while preparing the use with BabelBrain was that mapping procedures in the literature linking CT Hounsfield Units (HU) to the speed of sound and, especially, attenuation needs this sort of correction.
 * 0.9.10-1 Nov 16, 2022
-    * Add functions to list devices supported by computing backends 
+    * Add functions to list devices supported by computing backends
 * 0.9.10 Oct 28, 2022
     * Fix the issue with mapping of unique values when attenuation is used, it could cause some divisions by zero
 * 0.9.9.20 Sep 17, 2022
-    * A lot of important improvements to make the final line  
+    * A lot of important improvements to make the final line
         - Metal is (finally) running as fast (sometimes slightly faster) than OpenCL in Apple processors. It took a lot of testing and fine tuning.
         - Use of a modified version of the excellent `py-metal-compute` library (https://github.com/baldand/py-metal-compute) that allows having a similar approach as with pyopencl, cupy and pycuda. Modified library is at https://github.com/ProteusMRIgHIFU/py-metal-compute. Because of this new approach, the old Swift interface to the FDTD code was removed.
         - Add Metal backend for BHTE tool. This version runs way faster than OpenCL in Apple processors (like a 10x factor, need to investigate more if we can replicate such gain)
         - Benchmark metrics above were refreshed
         - Moving forward, OpenCL is not recommended for macOS in X64 systems. Because of the limitation of the underlying 32-bit addressing, pyopencl does not catch easily when a simulation goes beyond 4GB. However, Metal for AMD in macOS runs quite well, so no need to stick with OpenCL
 
 * 0.9.9  Sep 1, 2022
-    * A lot of simplifications allowed having a much more straightforward code. Thanks to Andrew Xie (@IAmAndrewX) for a very productive summer trimming down code, replacing the old MTLPP with Swift, and making a new class arrangement for the different GPU backends. Now BabelViscoFDTD is based completely on pyopencl and pycuda for the FDTD viscoelastic solver. For Metal, the Swift-based wrapper does the interfacing. The old C extension is still around just for the OpenMP backend.  
+    * A lot of simplifications allowed having a much more straightforward code. Thanks to Andrew Xie (@IAmAndrewX) for a very productive summer trimming down code, replacing the old MTLPP with Swift, and making a new class arrangement for the different GPU backends. Now BabelViscoFDTD is based completely on pyopencl and pycuda for the FDTD viscoelastic solver. For Metal, the Swift-based wrapper does the interfacing. The old C extension is still around just for the OpenMP backend.
 * 0.9.7  July 7, 2022
-    * The MTLPP C++ library is now replaced by a Swift interface to access the Metal implementation for the viscoelastic FDTD solution. This will ensure using a more standard Apple development language for the future, as MTLPP is not maintained anymore. While there is a new Apple-based C++ wrapper for Metal, using Swift is still preferred as we created now a C-linking compatible library that in the future can be also used directly in Python. In the long term, we aim to eliminate the C code extension and use only Python code in tandem with pyopencl, pycuda and  Metal 
+    * The MTLPP C++ library is now replaced by a Swift interface to access the Metal implementation for the viscoelastic FDTD solution. This will ensure using a more standard Apple development language for the future, as MTLPP is not maintained anymore. While there is a new Apple-based C++ wrapper for Metal, using Swift is still preferred as we created now a C-linking compatible library that in the future can be also used directly in Python. In the long term, we aim to eliminate the C code extension and use only Python code in tandem with pyopencl, pycuda and  Metal
 * 0.9.6-post-10  June 27, 2022
     * A fix for OpenCL in X64 Mac system that was missing the new kernel names
     * OpenMP for X64 in Mac is being turned back as experimental feature as some systems are unable to run with it correctly and there is not a clear path on how to ensure this will be stable. The feature will remain accessible if installing the library with the BABEL_MAC_OPENMP_X64 option enabled.
 * 0.9.6  Feb 5, 2022.
     * Improved performance in Metal-based devices by using mini-kernels.
     * Minor fixes for Rayleigh-Sommerfeld in Metal
 * 0.9.5  Jan 18, 2022.
     * Very first pip-registered version
     * Possibility of user-specified dimensions of blocks for computations for fine-tuning performance
     * Cleaning some minor bugs and adding BHTE code using pycuda and pyopencl.
-    
+
 * 0.9.3  Sep 29, 2021.
     * Improved support for both Metal and OpenCL. For Metal, stable operation is now feasible for large domains using all available memory in modern high-end GPUs. OpenCL is now supported in all OSs.
 * 0.9.2  June 13, 2021.
     * Add Rayleigh integral support in a homogenous medium with CUDA, OpenCL and Metal backends.
     * Support for stress sources
     * Able to select devices in multiple GPU systems with CUDA
 * 0.9.1  Feb 17, 2021. Pressure calculation added in low-level function.
```

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeCache.txt` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeCCompiler.cmake` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeCCompiler.cmake`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeCXXCompiler.cmake` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeCXXCompiler.cmake`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_C.bin` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_C.bin`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_CXX.bin` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CMakeDetermineCompilerABI_CXX.bin`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.c` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.c`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.exe` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.exe`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.obj` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdC/CMakeCCompilerId.obj`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.exe` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.exe`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.obj` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/3.19.7/CompilerIdCXX/CMakeCXXCompilerId.obj`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/CMakeDirectoryInformation.cmake` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/CMakeError.log` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/CMakeError.log`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/CMakeOutput.log` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/CMakeOutput.log`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/Makefile.cmake` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/Makefile2` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/C.includecache` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/C.includecache`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/DependInfo.cmake` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/build.make` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/build.make`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/depend.internal` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/depend.internal`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/pi_ocl.c.obj` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/pi_ocl.c.obj`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/CMakeFiles/pi_ocl.dir/vc140.pdb` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/CMakeFiles/pi_ocl.dir/vc140.pdb`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/Makefile` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/Makefile`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/cmake_install.cmake` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/pi_ocl.exe` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/pi_ocl.exe`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/pi_ocl.ilk` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/pi_ocl.ilk`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/pi_ocl/build/pi_ocl.pdb` & `BabelViscoFDTD-1.0.0.post1/pi_ocl/build/pi_ocl.pdb`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/setup.py` & `BabelViscoFDTD-1.0.0.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from distutils.unixccompiler import UnixCCompiler
 from shutil import copyfile, copytree,rmtree
 import sysconfig
 
 
 dir_path =path.dirname(os.path.realpath(__file__))+os.sep
 
-version = '1.0.0'
+version = '1.0.0-1'
 
 npinc=np.get_include()+os.sep+'numpy'
 # Filename for the C extension module library
 c_module_name = '_FDTDStaggered3D_with_relaxation'
 
 extra_obj =[]
```

### Comparing `BabelViscoFDTD-1.0.0/src/CMakeLists.txt` & `BabelViscoFDTD-1.0.0.post1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/FDTD3D_CPU_VERSION.h` & `BabelViscoFDTD-1.0.0.post1/src/FDTD3D_CPU_VERSION.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/FDTDStaggered3D_with_relaxation_python.c` & `BabelViscoFDTD-1.0.0.post1/src/FDTDStaggered3D_with_relaxation_python.c`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/GPU_KERNELS.h` & `BabelViscoFDTD-1.0.0.post1/src/GPU_KERNELS.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/Indexing.h` & `BabelViscoFDTD-1.0.0.post1/src/Indexing.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/Metal/Package.swift` & `BabelViscoFDTD-1.0.0.post1/src/Metal/Package.swift`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/Metal/Sources/BabelMetal/Babel.metal` & `BabelViscoFDTD-1.0.0.post1/src/Metal/Sources/BabelMetal/Babel.metal`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/Metal/Sources/BabelMetal/BabelMetal.swift` & `BabelViscoFDTD-1.0.0.post1/src/Metal/Sources/BabelMetal/BabelMetal.swift`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/ParticleKernel.h` & `BabelViscoFDTD-1.0.0.post1/src/ParticleKernel.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/SensorsKernel.h` & `BabelViscoFDTD-1.0.0.post1/src/SensorsKernel.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/StressKernel.h` & `BabelViscoFDTD-1.0.0.post1/src/StressKernel.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/commonDef.h` & `BabelViscoFDTD-1.0.0.post1/src/commonDef.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/commonDefGPU.h` & `BabelViscoFDTD-1.0.0.post1/src/commonDefGPU.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/kernelparamsMetal.h` & `BabelViscoFDTD-1.0.0.post1/src/kernelparamsMetal.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/kernelparamsOpenCL.h` & `BabelViscoFDTD-1.0.0.post1/src/kernelparamsOpenCL.h`

 * *Files identical despite different names*

### Comparing `BabelViscoFDTD-1.0.0/src/page_memory.c` & `BabelViscoFDTD-1.0.0.post1/src/page_memory.c`

 * *Files identical despite different names*

