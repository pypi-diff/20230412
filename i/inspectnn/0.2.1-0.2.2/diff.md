# Comparing `tmp/inspectnn-0.2.1.tar.gz` & `tmp/inspectnn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectnn-0.2.1.tar", last modified: Thu Apr  6 12:59:25 2023, max compression
+gzip compressed data, was "inspectnn-0.2.2.tar", last modified: Wed Apr 12 15:56:25 2023, max compression
```

## Comparing `inspectnn-0.2.1.tar` & `inspectnn-0.2.2.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.834547 inspectnn-0.2.1/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)    35149 2023-02-09 09:23:24.000000 inspectnn-0.2.1/LICENSE
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      984 2023-04-06 12:59:25.834547 inspectnn-0.2.1/PKG-INFO
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5936 2023-03-03 09:10:48.000000 inspectnn-0.2.1/README.md
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.819547 inspectnn-0.2.1/inspectnn/
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.820547 inspectnn-0.2.1/inspectnn/Add/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3243 2023-04-05 14:20:24.000000 inspectnn-0.2.1/inspectnn/Add/AddLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:07:07.000000 inspectnn-0.2.1/inspectnn/Add/Add_kernel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Add/__init__.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3342 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/BaseLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1922 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/ComMultiply.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.820547 inspectnn-0.2.1/inspectnn/Concatenate/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2261 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Concatenate/ConcatenateLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Concatenate/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.820547 inspectnn-0.2.1/inspectnn/Conv/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4758 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Conv/ConvLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2634 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Conv/ConvLayer_TF.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     6950 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Conv/ConvLayer_TFLITE.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2714 2023-03-14 11:07:07.000000 inspectnn-0.2.1/inspectnn/Conv/Conv_kernel.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5168 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Conv/Conv_kernel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Conv/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.821547 inspectnn-0.2.1/inspectnn/Dataset/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2206 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dataset/Dataset_cifar10.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1266 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dataset/Dataset_mnist.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      143 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dataset/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.821547 inspectnn-0.2.1/inspectnn/Dense/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4341 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dense/DenseLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3249 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dense/DenseLayer_TF.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4605 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dense/DenseLayer_TFLITE.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2428 2023-03-14 11:07:07.000000 inspectnn-0.2.1/inspectnn/Dense/Dense_kernel.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1484 2023-03-14 11:07:07.000000 inspectnn-0.2.1/inspectnn/Dense/Dense_kernel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Dense/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.821547 inspectnn-0.2.1/inspectnn/Flatten/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1931 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Flatten/FlattenLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Flatten/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.822547 inspectnn-0.2.1/inspectnn/Model/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     6226 2023-04-06 07:17:22.000000 inspectnn-0.2.1/inspectnn/Model/BaseModel.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3230 2023-04-06 10:06:16.000000 inspectnn-0.2.1/inspectnn/Model/BaseModel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)    24568 2023-04-06 10:06:16.000000 inspectnn-0.2.1/inspectnn/Model/GenericModel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)    12175 2023-04-05 14:52:50.000000 inspectnn-0.2.1/inspectnn/Model/NetworkModel.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3407 2023-04-05 14:20:21.000000 inspectnn-0.2.1/inspectnn/Model/NetworkModel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Model/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.822547 inspectnn-0.2.1/inspectnn/Pooling/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1908 2023-03-14 11:07:07.000000 inspectnn-0.2.1/inspectnn/Pooling/Pool_kernel.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3230 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Pooling/PoolingLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3357 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Pooling/PoolingLayer_TFLITE.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Pooling/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.822547 inspectnn-0.2.1/inspectnn/Quantizate/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2859 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Quantizate/DequantizateLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2885 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Quantizate/Quant_kernel_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4013 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Quantizate/QuantizateLayer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Quantizate/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.823547 inspectnn-0.2.1/inspectnn/Utils/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/Utils/__init__.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1477 2023-03-03 09:10:48.000000 inspectnn-0.2.1/inspectnn/Utils/cpu_utils.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1151 2023-03-03 09:10:48.000000 inspectnn-0.2.1/inspectnn/Utils/utils.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5508 2023-03-14 11:07:07.000000 inspectnn-0.2.1/inspectnn/Utils/utils_tflite.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5705 2023-04-05 14:14:34.000000 inspectnn-0.2.1/inspectnn/ValidateMultiply.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      603 2023-04-06 12:59:09.000000 inspectnn-0.2.1/inspectnn/__init__.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.819547 inspectnn-0.2.1/inspectnn.egg-info/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      984 2023-04-06 12:59:25.000000 inspectnn-0.2.1/inspectnn.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5069 2023-04-06 12:59:25.000000 inspectnn-0.2.1/inspectnn.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)        1 2023-04-06 12:59:25.000000 inspectnn-0.2.1/inspectnn.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      127 2023-04-06 12:59:25.000000 inspectnn-0.2.1/inspectnn.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)       17 2023-04-06 12:59:25.000000 inspectnn-0.2.1/inspectnn.egg-info/top_level.txt
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)       38 2023-04-06 12:59:25.834547 inspectnn-0.2.1/setup.cfg
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1674 2023-04-06 12:59:16.000000 inspectnn-0.2.1/setup.py
-drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 12:59:25.834547 inspectnn-0.2.1/tflite/
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/AbsOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      221 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ActivationFunctionType.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/AddNOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2382 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/AddOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ArgMaxOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ArgMinOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2229 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/BatchMatMulOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1316 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/BatchToSpaceNDOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4895 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/BidirectionalSequenceLSTMOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3817 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/BidirectionalSequenceRNNOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2603 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Buffer.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2638 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/BuiltinOperator.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2745 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/BuiltinOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1729 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/CallOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2249 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/CastOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      159 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/CombinerType.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5360 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ConcatEmbeddingsOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2404 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ConcatenationOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4403 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Conv2DOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/CosOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      147 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/CustomOptionsFormat.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2789 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/CustomQuantization.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1267 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DensifyOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1808 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DepthToSpaceOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5141 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DepthwiseConv2DOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DequantizeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4712 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DimensionMetadata.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      154 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DimensionType.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1851 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/DivOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1878 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/EmbeddingLookupSparseOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/EqualOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ExpOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ExpandDimsOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3198 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/FakeQuantOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/FillOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/FloorDivOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/FloorModOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3684 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/FullyConnectedOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      183 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/FullyConnectedOptionsWeightsFormat.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/GatherNdOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1709 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/GatherOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1302 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/GreaterEqualOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1267 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/GreaterOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/HardSwishOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2348 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/IfOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2698 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Int32Vector.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1878 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/L2NormOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1770 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LSHProjectionOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      170 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LSHProjectionType.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      149 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LSTMKernelType.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3970 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LSTMOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1753 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LeakyReluOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LessEqualOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LessOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3408 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LocalResponseNormalizationOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LogSoftmaxOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LogicalAndOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LogicalNotOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/LogicalOrOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/MatrixDiagOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1309 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/MatrixSetDiagOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1316 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/MaximumMinimumOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2151 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Metadata.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      155 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/MirrorPadMode.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1734 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/MirrorPadOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     9113 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Model.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1851 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/MulOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/NegOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1351 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/NonMaxSuppressionV4Options.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1351 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/NonMaxSuppressionV5Options.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/NotEqualOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1709 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/OneHotOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)    11163 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Operator.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3365 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/OperatorCode.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2199 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/PackOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/PadOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/PadV2Options.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      142 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Padding.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4340 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Pool2DOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/PowOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      167 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/QuantizationDetails.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     9091 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/QuantizationParameters.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/QuantizeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2482 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/RNNOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/RangeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/RankOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1762 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ReducerOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2767 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ReshapeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2443 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ResizeBilinearOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2519 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ResizeNearestNeighborOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2311 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ReverseSequenceOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ReverseV2Options.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2938 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SVDFOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ScatterNdOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SegmentSumOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1260 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SelectOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SelectV2Options.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3082 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SequenceRNNOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1725 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ShapeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2857 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SkipGramOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SliceOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1726 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SoftmaxOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1316 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SpaceToBatchNDOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1808 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SpaceToDepthOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      199 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SparseIndexVector.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1879 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SparseToDenseOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5892 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SparsityParameters.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1745 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SplitOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1754 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SplitVOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1260 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SquareOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1337 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SquaredDifferenceOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2812 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SqueezeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3906 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/StridedSliceOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     7253 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SubGraph.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2382 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/SubOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     7404 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Tensor.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)      302 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/TensorType.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/TileOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1260 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/TopKV2Options.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2777 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/TransposeConvOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/TransposeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2713 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Uint16Vector.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2698 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/Uint8Vector.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4345 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/UnidirectionalSequenceLSTMOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/UniqueOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2149 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/UnpackOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/WhereOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2381 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/WhileOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/ZerosLikeOptions.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4860 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/__init__.py
--rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2157 2023-03-14 11:18:55.000000 inspectnn-0.2.1/tflite/utils.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.904234 inspectnn-0.2.2/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)    35149 2023-02-09 09:23:24.000000 inspectnn-0.2.2/LICENSE
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      984 2023-04-12 15:56:25.904234 inspectnn-0.2.2/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5936 2023-03-03 09:10:48.000000 inspectnn-0.2.2/README.md
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.891234 inspectnn-0.2.2/inspectnn/
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.892234 inspectnn-0.2.2/inspectnn/Add/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3243 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Add/AddLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Add/Add_kernel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Add/__init__.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3342 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/BaseLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1922 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/ComMultiply.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.892234 inspectnn-0.2.2/inspectnn/Concatenate/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2261 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Concatenate/ConcatenateLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Concatenate/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.892234 inspectnn-0.2.2/inspectnn/Conv/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4758 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Conv/ConvLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2634 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Conv/ConvLayer_TF.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     6950 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Conv/ConvLayer_TFLITE.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2714 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Conv/Conv_kernel.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5168 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Conv/Conv_kernel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Conv/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.893234 inspectnn-0.2.2/inspectnn/Dataset/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2206 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dataset/Dataset_cifar10.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1266 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dataset/Dataset_mnist.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      143 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dataset/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.893234 inspectnn-0.2.2/inspectnn/Dense/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4341 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dense/DenseLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3249 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dense/DenseLayer_TF.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4605 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dense/DenseLayer_TFLITE.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2428 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dense/Dense_kernel.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1484 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dense/Dense_kernel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Dense/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.893234 inspectnn-0.2.2/inspectnn/Flatten/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1931 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Flatten/FlattenLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Flatten/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.894234 inspectnn-0.2.2/inspectnn/Model/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     6226 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Model/BaseModel.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3230 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Model/BaseModel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)    24495 2023-04-12 15:28:51.000000 inspectnn-0.2.2/inspectnn/Model/GenericModel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)    12175 2023-04-12 15:38:59.000000 inspectnn-0.2.2/inspectnn/Model/NetworkModel.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3407 2023-04-12 15:42:43.000000 inspectnn-0.2.2/inspectnn/Model/NetworkModel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Model/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.894234 inspectnn-0.2.2/inspectnn/Pooling/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1908 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Pooling/Pool_kernel.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3230 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Pooling/PoolingLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3357 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Pooling/PoolingLayer_TFLITE.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Pooling/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.894234 inspectnn-0.2.2/inspectnn/Quantizate/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2859 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Quantizate/DequantizateLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2885 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Quantizate/Quant_kernel_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4145 2023-04-12 15:33:13.000000 inspectnn-0.2.2/inspectnn/Quantizate/QuantizateLayer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Quantizate/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.894234 inspectnn-0.2.2/inspectnn/Utils/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        0 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Utils/__init__.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1477 2023-03-03 09:10:48.000000 inspectnn-0.2.2/inspectnn/Utils/cpu_utils.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1151 2023-03-03 09:10:48.000000 inspectnn-0.2.2/inspectnn/Utils/utils.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5508 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/Utils/utils_tflite.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5705 2023-04-06 13:00:40.000000 inspectnn-0.2.2/inspectnn/ValidateMultiply.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      779 2023-04-12 15:55:16.000000 inspectnn-0.2.2/inspectnn/__init__.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.892234 inspectnn-0.2.2/inspectnn.egg-info/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      984 2023-04-12 15:56:25.000000 inspectnn-0.2.2/inspectnn.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5069 2023-04-12 15:56:25.000000 inspectnn-0.2.2/inspectnn.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)        1 2023-04-12 15:56:25.000000 inspectnn-0.2.2/inspectnn.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      127 2023-04-12 15:56:25.000000 inspectnn-0.2.2/inspectnn.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)       17 2023-04-12 15:56:25.000000 inspectnn-0.2.2/inspectnn.egg-info/top_level.txt
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)       38 2023-04-12 15:56:25.904234 inspectnn-0.2.2/setup.cfg
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1674 2023-04-12 15:55:12.000000 inspectnn-0.2.2/setup.py
+drwxr-xr-x   0 ssaa      (1000) labembedded  (1000)        0 2023-04-12 15:56:25.904234 inspectnn-0.2.2/tflite/
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/AbsOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      221 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ActivationFunctionType.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/AddNOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2382 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/AddOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ArgMaxOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ArgMinOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2229 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/BatchMatMulOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1316 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/BatchToSpaceNDOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4895 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/BidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3817 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/BidirectionalSequenceRNNOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2603 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Buffer.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2638 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/BuiltinOperator.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2745 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/BuiltinOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1729 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/CallOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2249 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/CastOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      159 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/CombinerType.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5360 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ConcatEmbeddingsOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2404 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ConcatenationOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4403 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Conv2DOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/CosOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      147 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/CustomOptionsFormat.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2789 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/CustomQuantization.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1267 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DensifyOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1808 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DepthToSpaceOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5141 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DepthwiseConv2DOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DequantizeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4712 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DimensionMetadata.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      154 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DimensionType.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1851 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/DivOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1878 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/EmbeddingLookupSparseOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/EqualOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ExpOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ExpandDimsOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3198 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/FakeQuantOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/FillOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/FloorDivOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/FloorModOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3684 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/FullyConnectedOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      183 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/FullyConnectedOptionsWeightsFormat.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/GatherNdOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1709 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/GatherOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1302 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/GreaterEqualOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1267 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/GreaterOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/HardSwishOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2348 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/IfOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2698 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Int32Vector.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1878 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/L2NormOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1770 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LSHProjectionOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      170 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LSHProjectionType.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      149 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LSTMKernelType.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3970 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LSTMOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1753 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LeakyReluOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LessEqualOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LessOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3408 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LocalResponseNormalizationOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LogSoftmaxOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LogicalAndOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LogicalNotOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/LogicalOrOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/MatrixDiagOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1309 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/MatrixSetDiagOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1316 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/MaximumMinimumOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2151 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Metadata.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      155 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/MirrorPadMode.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1734 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/MirrorPadOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     9113 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Model.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1851 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/MulOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/NegOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1351 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/NonMaxSuppressionV4Options.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1351 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/NonMaxSuppressionV5Options.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/NotEqualOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1709 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/OneHotOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)    11163 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Operator.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3365 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/OperatorCode.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2199 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/PackOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/PadOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/PadV2Options.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      142 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Padding.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4340 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Pool2DOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1239 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/PowOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      167 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/QuantizationDetails.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     9091 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/QuantizationParameters.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/QuantizeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2482 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/RNNOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/RangeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/RankOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1762 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ReducerOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2767 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ReshapeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2443 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ResizeBilinearOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2519 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ResizeNearestNeighborOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2311 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ReverseSequenceOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ReverseV2Options.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2938 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SVDFOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ScatterNdOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1288 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SegmentSumOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1260 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SelectOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1274 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SelectV2Options.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3082 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SequenceRNNOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1725 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ShapeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2857 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SkipGramOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SliceOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1726 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SoftmaxOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1316 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SpaceToBatchNDOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1808 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SpaceToDepthOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      199 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SparseIndexVector.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1879 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SparseToDenseOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     5892 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SparsityParameters.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1745 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SplitOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1754 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SplitVOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1260 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SquareOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1337 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SquaredDifferenceOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2812 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SqueezeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     3906 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/StridedSliceOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     7253 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SubGraph.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2382 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/SubOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     7404 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Tensor.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)      302 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/TensorType.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1246 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/TileOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1260 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/TopKV2Options.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2777 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/TransposeConvOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/TransposeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2713 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Uint16Vector.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2698 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/Uint8Vector.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4345 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/UnidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1761 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/UniqueOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2149 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/UnpackOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1253 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/WhereOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2381 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/WhileOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     1281 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/ZerosLikeOptions.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     4860 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/__init__.py
+-rw-r--r--   0 ssaa      (1000) labembedded  (1000)     2157 2023-03-14 11:18:55.000000 inspectnn-0.2.2/tflite/utils.py
```

### Comparing `inspectnn-0.2.1/LICENSE` & `inspectnn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/PKG-INFO` & `inspectnn-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectnn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Inference eNgine uSing aPproximate arithmEtic ComponenTs for Neural Networks
 Home-page: https://github.com/SalvatoreBarone/inspect-nn
 Author: Salvatore Barone, Filippo Ferrandino
 Author-email: salvatore.barone@unina.it, fi.ferrandino@studenti.unina.it
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/inspect-nn/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/inspect-nn
```

### Comparing `inspectnn-0.2.1/README.md` & `inspectnn-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Add/AddLayer.py` & `inspectnn-0.2.2/inspectnn/Add/AddLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Add/Add_kernel_tflite.py` & `inspectnn-0.2.2/inspectnn/Add/Add_kernel_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/BaseLayer.py` & `inspectnn-0.2.2/inspectnn/BaseLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/ComMultiply.py` & `inspectnn-0.2.2/inspectnn/ComMultiply.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Concatenate/ConcatenateLayer.py` & `inspectnn-0.2.2/inspectnn/Concatenate/ConcatenateLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Conv/ConvLayer.py` & `inspectnn-0.2.2/inspectnn/Conv/ConvLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Conv/ConvLayer_TF.py` & `inspectnn-0.2.2/inspectnn/Conv/ConvLayer_TF.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Conv/ConvLayer_TFLITE.py` & `inspectnn-0.2.2/inspectnn/Conv/ConvLayer_TFLITE.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Conv/Conv_kernel.py` & `inspectnn-0.2.2/inspectnn/Conv/Conv_kernel.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Conv/Conv_kernel_tflite.py` & `inspectnn-0.2.2/inspectnn/Conv/Conv_kernel_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dataset/Dataset_cifar10.py` & `inspectnn-0.2.2/inspectnn/Dataset/Dataset_cifar10.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dataset/Dataset_mnist.py` & `inspectnn-0.2.2/inspectnn/Dataset/Dataset_mnist.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dense/DenseLayer.py` & `inspectnn-0.2.2/inspectnn/Dense/DenseLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dense/DenseLayer_TF.py` & `inspectnn-0.2.2/inspectnn/Dense/DenseLayer_TF.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dense/DenseLayer_TFLITE.py` & `inspectnn-0.2.2/inspectnn/Dense/DenseLayer_TFLITE.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dense/Dense_kernel.py` & `inspectnn-0.2.2/inspectnn/Dense/Dense_kernel.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Dense/Dense_kernel_tflite.py` & `inspectnn-0.2.2/inspectnn/Dense/Dense_kernel_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Flatten/FlattenLayer.py` & `inspectnn-0.2.2/inspectnn/Flatten/FlattenLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Model/BaseModel.py` & `inspectnn-0.2.2/inspectnn/Model/BaseModel.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Model/BaseModel_tflite.py` & `inspectnn-0.2.2/inspectnn/Model/BaseModel_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Model/GenericModel_tflite.py` & `inspectnn-0.2.2/inspectnn/Model/GenericModel_tflite.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from inspectnn.Model.BaseModel_tflite import BaseModel_tflite
 from inspectnn.Quantizate.QuantizateLayer import QuantizateLayer
 
 import tflite
 import numpy as np, time, tensorflow as tf
 
 class GenericModelTflite(BaseModel_tflite):
-    def __init__(self,path_tf_file="/home/filippo/Git/PhD_AdversarialAttack/Models/ResNet8-quantized.tflite",input_no_normalizate=True):
+    def __init__(self,path_tf_file, input_no_normalizate=True):
 
         self.quant_nbits = 7
         save_csv_path=''
         self.input_no_normalizate = input_no_normalizate
```

### Comparing `inspectnn-0.2.1/inspectnn/Model/NetworkModel.py` & `inspectnn-0.2.2/inspectnn/Model/NetworkModel.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Model/NetworkModel_tflite.py` & `inspectnn-0.2.2/inspectnn/Model/NetworkModel_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Pooling/Pool_kernel.py` & `inspectnn-0.2.2/inspectnn/Pooling/Pool_kernel.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Pooling/PoolingLayer.py` & `inspectnn-0.2.2/inspectnn/Pooling/PoolingLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Pooling/PoolingLayer_TFLITE.py` & `inspectnn-0.2.2/inspectnn/Pooling/PoolingLayer_TFLITE.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Quantizate/DequantizateLayer.py` & `inspectnn-0.2.2/inspectnn/Quantizate/DequantizateLayer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Quantizate/Quant_kernel_tflite.py` & `inspectnn-0.2.2/inspectnn/Quantizate/Quant_kernel_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Quantizate/QuantizateLayer.py` & `inspectnn-0.2.2/inspectnn/Quantizate/QuantizateLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,21 @@
         super().__init__(self, name = name,quant_nbits=quant_nbits)
         self.type=type
         
     def __deepcopy__(self, memo = None):
         return QuantizateLayer( name = self.name,type=self.type,quant_nbits=self.quant_nbits)
 
     def forward_pass(self, **kwargs):
-
         if self.gpu_input_memory is None:
-            inputv = kwargs["inputv"]
+            try:
+                inputv = kwargs["inputv"]
+            except KeyError as e:
+                print(e)
+                print(kwargs)
+                exit()
             if cuda.is_cuda_array(inputv):
                 A_global_mem = inputv
             else:
                 A_global_mem = cuda.to_device(np.ascontiguousarray(inputv))
             input_mul = 1
             input_offset = 0
         else:
```

### Comparing `inspectnn-0.2.1/inspectnn/Utils/cpu_utils.py` & `inspectnn-0.2.2/inspectnn/Utils/cpu_utils.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Utils/utils.py` & `inspectnn-0.2.2/inspectnn/Utils/utils.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/Utils/utils_tflite.py` & `inspectnn-0.2.2/inspectnn/Utils/utils_tflite.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn/ValidateMultiply.py` & `inspectnn-0.2.2/inspectnn/ValidateMultiply.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/inspectnn.egg-info/PKG-INFO` & `inspectnn-0.2.2/inspectnn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectnn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Inference eNgine uSing aPproximate arithmEtic ComponenTs for Neural Networks
 Home-page: https://github.com/SalvatoreBarone/inspect-nn
 Author: Salvatore Barone, Filippo Ferrandino
 Author-email: salvatore.barone@unina.it, fi.ferrandino@studenti.unina.it
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/inspect-nn/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/inspect-nn
```

### Comparing `inspectnn-0.2.1/inspectnn.egg-info/SOURCES.txt` & `inspectnn-0.2.2/inspectnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/setup.py` & `inspectnn-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="inspectnn",
-    version="0.2.1",
+    version="0.2.2",
     description="Inference eNgine uSing aPproximate arithmEtic ComponenTs for Neural Networks",
     long_description="Inference eNgine uSing aPproximate arithmEtic ComponenTs for Neural Networks",
     url="https://github.com/SalvatoreBarone/inspect-nn",
     author="Salvatore Barone, Filippo Ferrandino",
     author_email="salvatore.barone@unina.it, fi.ferrandino@studenti.unina.it",
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

### Comparing `inspectnn-0.2.1/tflite/AbsOptions.py` & `inspectnn-0.2.2/tflite/AbsOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/AddNOptions.py` & `inspectnn-0.2.2/tflite/AddNOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/AddOptions.py` & `inspectnn-0.2.2/tflite/AddOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ArgMaxOptions.py` & `inspectnn-0.2.2/tflite/ArgMaxOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ArgMinOptions.py` & `inspectnn-0.2.2/tflite/ArgMinOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/BatchMatMulOptions.py` & `inspectnn-0.2.2/tflite/BatchMatMulOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/BatchToSpaceNDOptions.py` & `inspectnn-0.2.2/tflite/BatchToSpaceNDOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/BidirectionalSequenceLSTMOptions.py` & `inspectnn-0.2.2/tflite/BidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/BidirectionalSequenceRNNOptions.py` & `inspectnn-0.2.2/tflite/BidirectionalSequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Buffer.py` & `inspectnn-0.2.2/tflite/Buffer.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/BuiltinOperator.py` & `inspectnn-0.2.2/tflite/BuiltinOperator.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/BuiltinOptions.py` & `inspectnn-0.2.2/tflite/BuiltinOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/CallOptions.py` & `inspectnn-0.2.2/tflite/CallOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/CastOptions.py` & `inspectnn-0.2.2/tflite/CastOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ConcatEmbeddingsOptions.py` & `inspectnn-0.2.2/tflite/ConcatEmbeddingsOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ConcatenationOptions.py` & `inspectnn-0.2.2/tflite/ConcatenationOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Conv2DOptions.py` & `inspectnn-0.2.2/tflite/Conv2DOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/CosOptions.py` & `inspectnn-0.2.2/tflite/CosOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/CustomQuantization.py` & `inspectnn-0.2.2/tflite/CustomQuantization.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/DensifyOptions.py` & `inspectnn-0.2.2/tflite/DensifyOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/DepthToSpaceOptions.py` & `inspectnn-0.2.2/tflite/DepthToSpaceOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/DepthwiseConv2DOptions.py` & `inspectnn-0.2.2/tflite/DepthwiseConv2DOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/DequantizeOptions.py` & `inspectnn-0.2.2/tflite/DequantizeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/DimensionMetadata.py` & `inspectnn-0.2.2/tflite/DimensionMetadata.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/DivOptions.py` & `inspectnn-0.2.2/tflite/DivOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/EmbeddingLookupSparseOptions.py` & `inspectnn-0.2.2/tflite/EmbeddingLookupSparseOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/EqualOptions.py` & `inspectnn-0.2.2/tflite/EqualOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ExpOptions.py` & `inspectnn-0.2.2/tflite/ExpOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ExpandDimsOptions.py` & `inspectnn-0.2.2/tflite/ExpandDimsOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/FakeQuantOptions.py` & `inspectnn-0.2.2/tflite/FakeQuantOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/FillOptions.py` & `inspectnn-0.2.2/tflite/FillOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/FloorDivOptions.py` & `inspectnn-0.2.2/tflite/FloorDivOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/FloorModOptions.py` & `inspectnn-0.2.2/tflite/FloorModOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/FullyConnectedOptions.py` & `inspectnn-0.2.2/tflite/FullyConnectedOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/GatherNdOptions.py` & `inspectnn-0.2.2/tflite/GatherNdOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/GatherOptions.py` & `inspectnn-0.2.2/tflite/GatherOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/GreaterEqualOptions.py` & `inspectnn-0.2.2/tflite/GreaterEqualOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/GreaterOptions.py` & `inspectnn-0.2.2/tflite/GreaterOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/HardSwishOptions.py` & `inspectnn-0.2.2/tflite/HardSwishOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/IfOptions.py` & `inspectnn-0.2.2/tflite/IfOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Int32Vector.py` & `inspectnn-0.2.2/tflite/Int32Vector.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/L2NormOptions.py` & `inspectnn-0.2.2/tflite/L2NormOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LSHProjectionOptions.py` & `inspectnn-0.2.2/tflite/LSHProjectionOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LSTMOptions.py` & `inspectnn-0.2.2/tflite/LSTMOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LeakyReluOptions.py` & `inspectnn-0.2.2/tflite/LeakyReluOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LessEqualOptions.py` & `inspectnn-0.2.2/tflite/LessEqualOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LessOptions.py` & `inspectnn-0.2.2/tflite/LessOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LocalResponseNormalizationOptions.py` & `inspectnn-0.2.2/tflite/LocalResponseNormalizationOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LogSoftmaxOptions.py` & `inspectnn-0.2.2/tflite/LogSoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LogicalAndOptions.py` & `inspectnn-0.2.2/tflite/LogicalAndOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LogicalNotOptions.py` & `inspectnn-0.2.2/tflite/LogicalNotOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/LogicalOrOptions.py` & `inspectnn-0.2.2/tflite/LogicalOrOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/MatrixDiagOptions.py` & `inspectnn-0.2.2/tflite/MatrixDiagOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/MatrixSetDiagOptions.py` & `inspectnn-0.2.2/tflite/MatrixSetDiagOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/MaximumMinimumOptions.py` & `inspectnn-0.2.2/tflite/MaximumMinimumOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Metadata.py` & `inspectnn-0.2.2/tflite/Metadata.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/MirrorPadOptions.py` & `inspectnn-0.2.2/tflite/MirrorPadOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Model.py` & `inspectnn-0.2.2/tflite/Model.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/MulOptions.py` & `inspectnn-0.2.2/tflite/MulOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/NegOptions.py` & `inspectnn-0.2.2/tflite/NegOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/NonMaxSuppressionV4Options.py` & `inspectnn-0.2.2/tflite/NonMaxSuppressionV4Options.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/NonMaxSuppressionV5Options.py` & `inspectnn-0.2.2/tflite/NonMaxSuppressionV5Options.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/NotEqualOptions.py` & `inspectnn-0.2.2/tflite/NotEqualOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/OneHotOptions.py` & `inspectnn-0.2.2/tflite/OneHotOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Operator.py` & `inspectnn-0.2.2/tflite/Operator.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/OperatorCode.py` & `inspectnn-0.2.2/tflite/OperatorCode.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/PackOptions.py` & `inspectnn-0.2.2/tflite/PackOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/PadOptions.py` & `inspectnn-0.2.2/tflite/PadOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/PadV2Options.py` & `inspectnn-0.2.2/tflite/PadV2Options.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Pool2DOptions.py` & `inspectnn-0.2.2/tflite/Pool2DOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/PowOptions.py` & `inspectnn-0.2.2/tflite/PowOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/QuantizationParameters.py` & `inspectnn-0.2.2/tflite/QuantizationParameters.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/QuantizeOptions.py` & `inspectnn-0.2.2/tflite/QuantizeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/RNNOptions.py` & `inspectnn-0.2.2/tflite/RNNOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/RangeOptions.py` & `inspectnn-0.2.2/tflite/RangeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/RankOptions.py` & `inspectnn-0.2.2/tflite/RankOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ReducerOptions.py` & `inspectnn-0.2.2/tflite/ReducerOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ReshapeOptions.py` & `inspectnn-0.2.2/tflite/ReshapeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ResizeBilinearOptions.py` & `inspectnn-0.2.2/tflite/ResizeBilinearOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ResizeNearestNeighborOptions.py` & `inspectnn-0.2.2/tflite/ResizeNearestNeighborOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ReverseSequenceOptions.py` & `inspectnn-0.2.2/tflite/ReverseSequenceOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ReverseV2Options.py` & `inspectnn-0.2.2/tflite/ReverseV2Options.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SVDFOptions.py` & `inspectnn-0.2.2/tflite/SVDFOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ScatterNdOptions.py` & `inspectnn-0.2.2/tflite/ScatterNdOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SegmentSumOptions.py` & `inspectnn-0.2.2/tflite/SegmentSumOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SelectOptions.py` & `inspectnn-0.2.2/tflite/SelectOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SelectV2Options.py` & `inspectnn-0.2.2/tflite/SelectV2Options.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SequenceRNNOptions.py` & `inspectnn-0.2.2/tflite/SequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ShapeOptions.py` & `inspectnn-0.2.2/tflite/ShapeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SkipGramOptions.py` & `inspectnn-0.2.2/tflite/SkipGramOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SliceOptions.py` & `inspectnn-0.2.2/tflite/SliceOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SoftmaxOptions.py` & `inspectnn-0.2.2/tflite/SoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SpaceToBatchNDOptions.py` & `inspectnn-0.2.2/tflite/SpaceToBatchNDOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SpaceToDepthOptions.py` & `inspectnn-0.2.2/tflite/SpaceToDepthOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SparseToDenseOptions.py` & `inspectnn-0.2.2/tflite/SparseToDenseOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SparsityParameters.py` & `inspectnn-0.2.2/tflite/SparsityParameters.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SplitOptions.py` & `inspectnn-0.2.2/tflite/SplitOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SplitVOptions.py` & `inspectnn-0.2.2/tflite/SplitVOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SquareOptions.py` & `inspectnn-0.2.2/tflite/SquareOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SquaredDifferenceOptions.py` & `inspectnn-0.2.2/tflite/SquaredDifferenceOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SqueezeOptions.py` & `inspectnn-0.2.2/tflite/SqueezeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/StridedSliceOptions.py` & `inspectnn-0.2.2/tflite/StridedSliceOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SubGraph.py` & `inspectnn-0.2.2/tflite/SubGraph.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/SubOptions.py` & `inspectnn-0.2.2/tflite/SubOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Tensor.py` & `inspectnn-0.2.2/tflite/Tensor.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/TileOptions.py` & `inspectnn-0.2.2/tflite/TileOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/TopKV2Options.py` & `inspectnn-0.2.2/tflite/TopKV2Options.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/TransposeConvOptions.py` & `inspectnn-0.2.2/tflite/TransposeConvOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/TransposeOptions.py` & `inspectnn-0.2.2/tflite/TransposeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Uint16Vector.py` & `inspectnn-0.2.2/tflite/Uint16Vector.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/Uint8Vector.py` & `inspectnn-0.2.2/tflite/Uint8Vector.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/UnidirectionalSequenceLSTMOptions.py` & `inspectnn-0.2.2/tflite/UnidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/UniqueOptions.py` & `inspectnn-0.2.2/tflite/UniqueOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/UnpackOptions.py` & `inspectnn-0.2.2/tflite/UnpackOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/WhereOptions.py` & `inspectnn-0.2.2/tflite/WhereOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/WhileOptions.py` & `inspectnn-0.2.2/tflite/WhileOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/ZerosLikeOptions.py` & `inspectnn-0.2.2/tflite/ZerosLikeOptions.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/__init__.py` & `inspectnn-0.2.2/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `inspectnn-0.2.1/tflite/utils.py` & `inspectnn-0.2.2/tflite/utils.py`

 * *Files identical despite different names*

