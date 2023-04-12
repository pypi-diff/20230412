# Comparing `tmp/triton_model_navigator-0.5.1-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,131 +1,131 @@
-Zip file size: 212734 bytes, number of entries: 129
--rw-r--r--  2.0 unx      881 b- defN 23-Mar-29 08:29 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Mar-29 10:37 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3668 b- defN 23-Mar-29 08:29 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     9474 b- defN 23-Mar-29 08:29 model_navigator/execution_context.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Mar-29 08:29 model_navigator/logger.py
--rw-r--r--  2.0 unx     1520 b- defN 23-Mar-29 08:29 model_navigator/api/__init__.py
--rw-r--r--  2.0 unx    21958 b- defN 23-Mar-29 08:29 model_navigator/api/config.py
--rw-r--r--  2.0 unx     6362 b- defN 23-Mar-29 08:29 model_navigator/api/jax.py
--rw-r--r--  2.0 unx     5372 b- defN 23-Mar-29 08:29 model_navigator/api/onnx.py
--rw-r--r--  2.0 unx    11854 b- defN 23-Mar-29 08:29 model_navigator/api/package.py
--rw-r--r--  2.0 unx     4861 b- defN 23-Mar-29 08:29 model_navigator/api/python.py
--rw-r--r--  2.0 unx     7800 b- defN 23-Mar-29 08:29 model_navigator/api/pytriton.py
--rw-r--r--  2.0 unx     6462 b- defN 23-Mar-29 08:29 model_navigator/api/tensorflow.py
--rw-r--r--  2.0 unx     6257 b- defN 23-Mar-29 08:29 model_navigator/api/torch.py
--rw-r--r--  2.0 unx     1553 b- defN 23-Mar-29 08:29 model_navigator/api/triton.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/__init__.py
--rw-r--r--  2.0 unx     4938 b- defN 23-Mar-29 08:29 model_navigator/commands/base.py
--rw-r--r--  2.0 unx    10071 b- defN 23-Mar-29 08:29 model_navigator/commands/infer_metadata.py
--rw-r--r--  2.0 unx     3289 b- defN 23-Mar-29 08:29 model_navigator/commands/load.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/__init__.py
--rw-r--r--  2.0 unx     7015 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/base.py
--rw-r--r--  2.0 unx     7838 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/tf.py
--rw-r--r--  2.0 unx    10151 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/torch.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/converters/__init__.py
--rw-r--r--  2.0 unx     3418 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/converters/ts2onnx.py
--rw-r--r--  2.0 unx     4992 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-r--r--  2.0 unx      680 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/onnx/__init__.py
--rw-r--r--  2.0 unx     1728 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    10453 b- defN 23-Mar-29 10:37 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-r--r--  2.0 unx     2236 b- defN 23-Mar-29 08:29 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/copy/__init__.py
--rw-r--r--  2.0 unx     1729 b- defN 23-Mar-29 08:29 model_navigator/commands/copy/onnx.py
--rw-r--r--  2.0 unx      678 b- defN 23-Mar-29 08:29 model_navigator/commands/correctness/__init__.py
--rw-r--r--  2.0 unx     5595 b- defN 23-Mar-29 08:29 model_navigator/commands/correctness/correctness.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Mar-29 08:29 model_navigator/commands/correctness/correctness_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/data_dump/__init__.py
--rw-r--r--  2.0 unx    11168 b- defN 23-Mar-29 08:29 model_navigator/commands/data_dump/samples.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/export/__init__.py
--rw-r--r--  2.0 unx     3527 b- defN 23-Mar-29 08:29 model_navigator/commands/export/jax.py
--rw-r--r--  2.0 unx     5486 b- defN 23-Mar-29 08:29 model_navigator/commands/export/tf.py
--rw-r--r--  2.0 unx     8895 b- defN 23-Mar-29 08:29 model_navigator/commands/export/torch.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Mar-29 08:29 model_navigator/commands/export/exporters/__init__.py
--rw-r--r--  2.0 unx     3945 b- defN 23-Mar-29 08:29 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-r--r--  2.0 unx     3172 b- defN 23-Mar-29 08:29 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-r--r--  2.0 unx     3123 b- defN 23-Mar-29 08:29 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Mar-29 08:29 model_navigator/commands/export/exporters/torch2onnx.py
--rw-r--r--  2.0 unx     2603 b- defN 23-Mar-29 08:29 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-r--r--  2.0 unx      715 b- defN 23-Mar-29 08:29 model_navigator/commands/find_max_batch_size/__init__.py
--rw-r--r--  2.0 unx     6397 b- defN 23-Mar-29 08:29 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-r--r--  2.0 unx     2985 b- defN 23-Mar-29 08:29 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-r--r--  2.0 unx      688 b- defN 23-Mar-29 08:29 model_navigator/commands/performance/__init__.py
--rw-r--r--  2.0 unx    15771 b- defN 23-Mar-29 08:29 model_navigator/commands/performance/performance.py
--rw-r--r--  2.0 unx     3038 b- defN 23-Mar-29 08:29 model_navigator/commands/performance/performance_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/commands/verification/__init__.py
--rw-r--r--  2.0 unx     5447 b- defN 23-Mar-29 08:29 model_navigator/commands/verification/verify.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/configuration/__init__.py
--rw-r--r--  2.0 unx     2478 b- defN 23-Mar-29 08:29 model_navigator/configuration/common_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/configuration/model/__init__.py
--rw-r--r--  2.0 unx    14775 b- defN 23-Mar-29 08:29 model_navigator/configuration/model/model_config.py
--rw-r--r--  2.0 unx    13263 b- defN 23-Mar-29 08:29 model_navigator/configuration/model/model_config_builder.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/core/__init__.py
--rw-r--r--  2.0 unx     1213 b- defN 23-Mar-29 08:29 model_navigator/core/constants.py
--rw-rw-rw-  2.0 unx    20118 b- defN 23-Mar-29 12:11 model_navigator/core/package.py
--rw-r--r--  2.0 unx    20332 b- defN 23-Mar-29 08:29 model_navigator/core/status.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/pipelines/__init__.py
--rw-r--r--  2.0 unx     5405 b- defN 23-Mar-29 08:29 model_navigator/pipelines/pipeline.py
--rw-r--r--  2.0 unx     7334 b- defN 23-Mar-29 08:29 model_navigator/pipelines/pipeline_manager.py
--rw-r--r--  2.0 unx     9810 b- defN 23-Mar-29 08:29 model_navigator/pipelines/validation.py
--rw-r--r--  2.0 unx     1884 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/__init__.py
--rw-r--r--  2.0 unx     2036 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/correctness.py
--rw-r--r--  2.0 unx     4749 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-r--r--  2.0 unx     1647 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/jax.py
--rw-r--r--  2.0 unx     2395 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/onnx.py
--rw-r--r--  2.0 unx     2365 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/preprocessing.py
--rw-r--r--  2.0 unx     2685 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/profiling.py
--rw-r--r--  2.0 unx     2869 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/tensorflow.py
--rw-r--r--  2.0 unx     3261 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/torch.py
--rw-r--r--  2.0 unx     2042 b- defN 23-Mar-29 08:29 model_navigator/pipelines/builders/verify.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Mar-29 08:29 model_navigator/runners/__init__.py
--rw-r--r--  2.0 unx    10683 b- defN 23-Mar-29 08:29 model_navigator/runners/base.py
--rw-r--r--  2.0 unx     2620 b- defN 23-Mar-29 08:29 model_navigator/runners/jax.py
--rw-r--r--  2.0 unx     4513 b- defN 23-Mar-29 08:29 model_navigator/runners/onnx.py
--rw-r--r--  2.0 unx     2267 b- defN 23-Mar-29 08:29 model_navigator/runners/python.py
--rw-r--r--  2.0 unx     2285 b- defN 23-Mar-29 08:29 model_navigator/runners/registry.py
--rw-r--r--  2.0 unx     7980 b- defN 23-Mar-29 08:29 model_navigator/runners/tensorflow.py
--rw-r--r--  2.0 unx     2468 b- defN 23-Mar-29 08:29 model_navigator/runners/tensorrt.py
--rw-r--r--  2.0 unx     7631 b- defN 23-Mar-29 08:29 model_navigator/runners/torch.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Mar-29 08:29 model_navigator/runners/utils.py
--rw-r--r--  2.0 unx      937 b- defN 23-Mar-29 08:29 model_navigator/runtime_analyzer/__init__.py
--rw-r--r--  2.0 unx    11706 b- defN 23-Mar-29 08:29 model_navigator/runtime_analyzer/analyzer.py
--rw-r--r--  2.0 unx     2304 b- defN 23-Mar-29 08:29 model_navigator/runtime_analyzer/strategy.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/triton/__init__.py
--rw-r--r--  2.0 unx     3182 b- defN 23-Mar-29 08:29 model_navigator/triton/model_config.py
--rw-r--r--  2.0 unx     5218 b- defN 23-Mar-29 08:29 model_navigator/triton/model_config_builder.py
--rw-r--r--  2.0 unx    23090 b- defN 23-Mar-29 08:29 model_navigator/triton/model_config_generator.py
--rw-r--r--  2.0 unx    15198 b- defN 23-Mar-29 08:29 model_navigator/triton/model_repository.py
--rw-r--r--  2.0 unx     2082 b- defN 23-Mar-29 08:29 model_navigator/triton/utils.py
--rw-r--r--  2.0 unx      944 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/__init__.py
--rw-r--r--  2.0 unx     2874 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/base_model_config.py
--rw-r--r--  2.0 unx    22326 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/common.py
--rw-r--r--  2.0 unx     2231 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/internal.py
--rw-r--r--  2.0 unx     2685 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-r--r--  2.0 unx     1785 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/python_model_config.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-r--r--  2.0 unx     3162 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Mar-29 08:29 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-29 08:29 model_navigator/utils/__init__.py
--rw-r--r--  2.0 unx     7436 b- defN 23-Mar-29 08:29 model_navigator/utils/common.py
--rw-r--r--  2.0 unx     8001 b- defN 23-Mar-29 08:29 model_navigator/utils/dataloader.py
--rw-r--r--  2.0 unx     3902 b- defN 23-Mar-29 08:29 model_navigator/utils/devices.py
--rw-r--r--  2.0 unx     1308 b- defN 23-Mar-29 08:29 model_navigator/utils/enums.py
--rw-r--r--  2.0 unx     6163 b- defN 23-Mar-29 08:29 model_navigator/utils/environment.py
--rw-r--r--  2.0 unx     3533 b- defN 23-Mar-29 08:29 model_navigator/utils/format_helpers.py
--rw-r--r--  2.0 unx     2497 b- defN 23-Mar-29 08:29 model_navigator/utils/framework.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Mar-29 08:29 model_navigator/utils/jax.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Mar-29 08:29 model_navigator/utils/module.py
--rw-r--r--  2.0 unx     1085 b- defN 23-Mar-29 08:29 model_navigator/utils/onnx.py
--rw-r--r--  2.0 unx     3239 b- defN 23-Mar-29 08:29 model_navigator/utils/package.py
--rw-r--r--  2.0 unx     1331 b- defN 23-Mar-29 08:29 model_navigator/utils/pipelines.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Mar-29 08:29 model_navigator/utils/runners.py
--rw-r--r--  2.0 unx     8054 b- defN 23-Mar-29 08:29 model_navigator/utils/tensor.py
--rw-r--r--  2.0 unx     2848 b- defN 23-Mar-29 08:29 model_navigator/utils/tensorrt.py
--rw-r--r--  2.0 unx     1508 b- defN 23-Mar-29 08:29 model_navigator/utils/torch.py
--rw-r--r--  2.0 unx    10140 b- defN 23-Mar-29 16:10 triton_model_navigator-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    12550 b- defN 23-Mar-29 16:10 triton_model_navigator-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-29 16:10 triton_model_navigator-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-29 16:10 triton_model_navigator-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    12813 b- defN 23-Mar-29 16:10 triton_model_navigator-0.5.1.dist-info/RECORD
-129 files, 626603 bytes uncompressed, 191866 bytes compressed:  69.4%
+Zip file size: 212950 bytes, number of entries: 129
+-rw-r--r--  2.0 unx      881 b- defN 23-Apr-12 10:00 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Apr-12 10:00 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3668 b- defN 23-Apr-12 10:00 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     9474 b- defN 23-Apr-12 10:00 model_navigator/execution_context.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Apr-12 10:00 model_navigator/logger.py
+-rw-rw-rw-  2.0 unx     1520 b- defN 23-Apr-12 10:00 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    21958 b- defN 23-Apr-12 10:00 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6362 b- defN 23-Apr-12 10:00 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5372 b- defN 23-Apr-12 10:00 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    11854 b- defN 23-Apr-12 10:00 model_navigator/api/package.py
+-rw-rw-rw-  2.0 unx     4861 b- defN 23-Apr-12 10:00 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7800 b- defN 23-Apr-12 10:00 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6462 b- defN 23-Apr-12 10:00 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6257 b- defN 23-Apr-12 10:00 model_navigator/api/torch.py
+-rw-rw-rw-  2.0 unx     1553 b- defN 23-Apr-12 10:00 model_navigator/api/triton.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     4938 b- defN 23-Apr-12 10:00 model_navigator/commands/base.py
+-rw-rw-rw-  2.0 unx    10071 b- defN 23-Apr-12 10:00 model_navigator/commands/infer_metadata.py
+-rw-rw-rw-  2.0 unx     3289 b- defN 23-Apr-12 10:00 model_navigator/commands/load.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     7039 b- defN 23-Apr-12 12:21 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7838 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx    10151 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/torch.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/__init__.py
+-rw-rw-rw-  2.0 unx     3418 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-rw-rw-  2.0 unx     3105 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-rw-rw-  2.0 unx     4992 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-rw-rw-  2.0 unx      680 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1728 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    10453 b- defN 23-Apr-12 12:21 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-rw-rw-  2.0 unx     2236 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/copy/__init__.py
+-rw-rw-rw-  2.0 unx     1729 b- defN 23-Apr-12 10:00 model_navigator/commands/copy/onnx.py
+-rw-rw-rw-  2.0 unx      678 b- defN 23-Apr-12 10:00 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5595 b- defN 23-Apr-12 10:00 model_navigator/commands/correctness/correctness.py
+-rw-rw-rw-  2.0 unx     4631 b- defN 23-Apr-12 12:21 model_navigator/commands/correctness/correctness_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/data_dump/__init__.py
+-rw-rw-rw-  2.0 unx    11168 b- defN 23-Apr-12 10:00 model_navigator/commands/data_dump/samples.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/export/__init__.py
+-rw-rw-rw-  2.0 unx     3527 b- defN 23-Apr-12 10:00 model_navigator/commands/export/jax.py
+-rw-rw-rw-  2.0 unx     5486 b- defN 23-Apr-12 10:00 model_navigator/commands/export/tf.py
+-rw-rw-rw-  2.0 unx     8895 b- defN 23-Apr-12 10:00 model_navigator/commands/export/torch.py
+-rw-rw-rw-  2.0 unx     1061 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/__init__.py
+-rw-rw-rw-  2.0 unx     3945 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-rw-rw-  2.0 unx     3172 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-rw-rw-  2.0 unx     3123 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-rw-rw-  2.0 unx     3077 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-rw-rw-  2.0 unx     2603 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-rw-rw-  2.0 unx      715 b- defN 23-Apr-12 10:00 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-rw-rw-  2.0 unx     6397 b- defN 23-Apr-12 10:00 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-rw-rw-  2.0 unx     2985 b- defN 23-Apr-12 10:00 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-rw-rw-  2.0 unx      688 b- defN 23-Apr-12 10:00 model_navigator/commands/performance/__init__.py
+-rw-rw-rw-  2.0 unx    15771 b- defN 23-Apr-12 10:00 model_navigator/commands/performance/performance.py
+-rw-rw-rw-  2.0 unx     3038 b- defN 23-Apr-12 10:00 model_navigator/commands/performance/performance_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/verification/__init__.py
+-rw-rw-rw-  2.0 unx     5447 b- defN 23-Apr-12 10:00 model_navigator/commands/verification/verify.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2478 b- defN 23-Apr-12 10:00 model_navigator/configuration/common_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    14775 b- defN 23-Apr-12 10:00 model_navigator/configuration/model/model_config.py
+-rw-rw-rw-  2.0 unx    13482 b- defN 23-Apr-12 10:00 model_navigator/configuration/model/model_config_builder.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1213 b- defN 23-Apr-12 10:00 model_navigator/core/constants.py
+-rw-rw-rw-  2.0 unx    20118 b- defN 23-Apr-12 10:00 model_navigator/core/package.py
+-rw-rw-rw-  2.0 unx    20332 b- defN 23-Apr-12 10:00 model_navigator/core/status.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/pipelines/__init__.py
+-rw-rw-rw-  2.0 unx     5451 b- defN 23-Apr-12 10:00 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx     7334 b- defN 23-Apr-12 10:00 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9810 b- defN 23-Apr-12 10:00 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1884 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/__init__.py
+-rw-rw-rw-  2.0 unx     2036 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     4749 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-rw-rw-  2.0 unx     1647 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2395 b- defN 23-Apr-12 12:21 model_navigator/pipelines/builders/onnx.py
+-rw-rw-rw-  2.0 unx     2365 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/preprocessing.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2869 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3261 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/torch.py
+-rw-rw-rw-  2.0 unx     2042 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/verify.py
+-rw-rw-rw-  2.0 unx     1513 b- defN 23-Apr-12 12:21 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    10683 b- defN 23-Apr-12 12:21 model_navigator/runners/base.py
+-rw-rw-rw-  2.0 unx     2620 b- defN 23-Apr-12 10:00 model_navigator/runners/jax.py
+-rw-rw-rw-  2.0 unx     4513 b- defN 23-Apr-12 12:21 model_navigator/runners/onnx.py
+-rw-rw-rw-  2.0 unx     2267 b- defN 23-Apr-12 10:00 model_navigator/runners/python.py
+-rw-rw-rw-  2.0 unx     2285 b- defN 23-Apr-12 10:00 model_navigator/runners/registry.py
+-rw-rw-rw-  2.0 unx     7980 b- defN 23-Apr-12 10:00 model_navigator/runners/tensorflow.py
+-rw-rw-rw-  2.0 unx     2468 b- defN 23-Apr-12 12:21 model_navigator/runners/tensorrt.py
+-rw-rw-rw-  2.0 unx     7631 b- defN 23-Apr-12 10:00 model_navigator/runners/torch.py
+-rw-rw-rw-  2.0 unx     1153 b- defN 23-Apr-12 10:00 model_navigator/runners/utils.py
+-rw-rw-rw-  2.0 unx      937 b- defN 23-Apr-12 10:00 model_navigator/runtime_analyzer/__init__.py
+-rw-rw-rw-  2.0 unx    11706 b- defN 23-Apr-12 10:00 model_navigator/runtime_analyzer/analyzer.py
+-rw-rw-rw-  2.0 unx     2304 b- defN 23-Apr-12 10:00 model_navigator/runtime_analyzer/strategy.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/triton/__init__.py
+-rw-rw-rw-  2.0 unx     3182 b- defN 23-Apr-12 10:00 model_navigator/triton/model_config.py
+-rw-rw-rw-  2.0 unx     5218 b- defN 23-Apr-12 10:00 model_navigator/triton/model_config_builder.py
+-rw-rw-rw-  2.0 unx    23090 b- defN 23-Apr-12 10:00 model_navigator/triton/model_config_generator.py
+-rw-rw-rw-  2.0 unx    15198 b- defN 23-Apr-12 10:00 model_navigator/triton/model_repository.py
+-rw-rw-rw-  2.0 unx     2082 b- defN 23-Apr-12 10:00 model_navigator/triton/utils.py
+-rw-rw-rw-  2.0 unx      944 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/__init__.py
+-rw-rw-rw-  2.0 unx     2874 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-rw-rw-  2.0 unx    22326 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/common.py
+-rw-rw-rw-  2.0 unx     2231 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/internal.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-rw-rw-  2.0 unx     1785 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-rw-rw-  2.0 unx     2239 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-rw-rw-  2.0 unx     3162 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-rw-rw-  2.0 unx     3040 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx     7436 b- defN 23-Apr-12 12:21 model_navigator/utils/common.py
+-rw-rw-rw-  2.0 unx     8001 b- defN 23-Apr-12 10:00 model_navigator/utils/dataloader.py
+-rw-rw-rw-  2.0 unx     3902 b- defN 23-Apr-12 10:00 model_navigator/utils/devices.py
+-rw-rw-rw-  2.0 unx     1308 b- defN 23-Apr-12 10:00 model_navigator/utils/enums.py
+-rw-rw-rw-  2.0 unx     6163 b- defN 23-Apr-12 10:00 model_navigator/utils/environment.py
+-rw-rw-rw-  2.0 unx     3533 b- defN 23-Apr-12 10:00 model_navigator/utils/format_helpers.py
+-rw-rw-rw-  2.0 unx     2497 b- defN 23-Apr-12 12:21 model_navigator/utils/framework.py
+-rw-rw-rw-  2.0 unx     1554 b- defN 23-Apr-12 10:00 model_navigator/utils/jax.py
+-rw-rw-rw-  2.0 unx     2325 b- defN 23-Apr-12 10:00 model_navigator/utils/module.py
+-rw-rw-rw-  2.0 unx     1085 b- defN 23-Apr-12 10:00 model_navigator/utils/onnx.py
+-rw-rw-rw-  2.0 unx     3239 b- defN 23-Apr-12 10:00 model_navigator/utils/package.py
+-rw-rw-rw-  2.0 unx     1331 b- defN 23-Apr-12 10:00 model_navigator/utils/pipelines.py
+-rw-rw-rw-  2.0 unx     3171 b- defN 23-Apr-12 10:00 model_navigator/utils/runners.py
+-rw-rw-rw-  2.0 unx     8054 b- defN 23-Apr-12 10:00 model_navigator/utils/tensor.py
+-rw-rw-rw-  2.0 unx     2848 b- defN 23-Apr-12 12:21 model_navigator/utils/tensorrt.py
+-rw-rw-rw-  2.0 unx     1508 b- defN 23-Apr-12 10:00 model_navigator/utils/torch.py
+-rw-rw-rw-  2.0 unx    10140 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13041 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12813 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/RECORD
+129 files, 627383 bytes uncompressed, 192082 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -366,23 +366,23 @@
 
 Filename: model_navigator/utils/tensorrt.py
 Comment: 
 
 Filename: model_navigator/utils/torch.py
 Comment: 
 
-Filename: triton_model_navigator-0.5.1.dist-info/LICENSE
+Filename: triton_model_navigator-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.5.1.dist-info/METADATA
+Filename: triton_model_navigator-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.5.1.dist-info/WHEEL
+Filename: triton_model_navigator-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.5.1.dist-info/top_level.txt
+Filename: triton_model_navigator-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.5.1.dist-info/RECORD
+Filename: triton_model_navigator-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.5.1"
+__version__ = "0.5.2"
```

## model_navigator/commands/convert/base.py

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ConvertONNX2TRT command."""
 
-from typing import Callable, Iterable, Optional
+from typing import Callable, Generator, Iterable, Optional
 
 from model_navigator.api.config import TensorRTProfile
 from model_navigator.commands.base import Command
 from model_navigator.core.constants import DEFAULT_MAX_BATCH_SIZE_HALVING
 from model_navigator.logger import LOGGER
 
 
@@ -111,15 +111,15 @@
             yield device_max_batch_size
         else:
             yield dataloader_max_batch_size
 
     @staticmethod
     def _get_conversion_fallback_batch_sizes(
         device_max_batch_size: int, dataloader_max_batch_size: int
-    ) -> Iterable[int]:
+    ) -> Generator[int, None, None]:
         max_batch_size_halving_left = DEFAULT_MAX_BATCH_SIZE_HALVING  # TODO what is the best value?
         max_batch_size = device_max_batch_size // 2
         while max_batch_size > dataloader_max_batch_size and max_batch_size_halving_left > 0:
             yield max_batch_size
             max_batch_size //= 2
             max_batch_size_halving_left -= 1
         yield dataloader_max_batch_size
```

## model_navigator/configuration/model/model_config_builder.py

```diff
@@ -91,15 +91,17 @@
 
         if Format.TENSORFLOW in target_formats:
             ModelConfigBuilder.get_source_tensorflow_config(model_configs)
 
         if Format.JAX in target_formats:
             ModelConfigBuilder.get_source_jax_config(model_configs)
 
-        if framework == Framework.TORCH and (Format.TORCHSCRIPT in target_formats or Format.ONNX in target_formats):
+        onnx_custom_config = _get_custom_config(custom_configs_for_format, config_api.OnnxConfig, framework=framework)
+        extended_onnx_export = Format.ONNX in target_formats and onnx_custom_config.onnx_extended_conversion
+        if framework == Framework.TORCH and (Format.TORCHSCRIPT in target_formats or extended_onnx_export):
             ModelConfigBuilder.get_torchscript_config(custom_configs_for_format, model_configs)
 
         if Format.TORCH_TRT in target_formats:
             ModelConfigBuilder.get_torch_trt_config(custom_configs_for_format, model_configs)
 
         if Format.TF_SAVEDMODEL in target_formats:
             ModelConfigBuilder.get_savedmodel_config(custom_configs_for_format, model_configs, framework=framework)
```

## model_navigator/pipelines/pipeline.py

```diff
@@ -107,20 +107,21 @@
                 )  # pytype: disable=not-instantiable
             except ModelNavigatorUserInputError as e:
                 command_output = CommandOutput(status=CommandStatus.FAIL)
 
                 if config.verbose and e.__context__:
                     LOGGER.info(e.__context__)
 
+                error = traceback.format_exc()
                 LOGGER.warning(
                     "Command finished with ModelNavigatorUserInputError. "
                     "The error is considered as external error. Usually caused by "
                     "incompatibilities between the model and the target formats and/or runtimes. "
                     "Please review the command output.\n"
-                    f"{str(e)}"
+                    f"{error}"
                 )
             except Exception:
                 command_output = CommandOutput(status=CommandStatus.FAIL)
                 error = traceback.format_exc()
                 LOGGER.error(f"Command finished with unexpected error: {error}")
 
             if command_output.status == CommandStatus.FAIL and execution_unit.command.is_required():
```

## Comparing `triton_model_navigator-0.5.1.dist-info/LICENSE` & `triton_model_navigator-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.5.1.dist-info/METADATA` & `triton_model_navigator-0.5.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.5.1
+Version: 0.5.2
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: <4,>=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: coloredlogs (>=15.0.0)
 Requires-Dist: dacite (>=1.6.0)
 Requires-Dist: fire (>=0.4.0)
 Requires-Dist: jsonlines (>=3.1.0)
 Requires-Dist: mpmath (<1.0.0)
 Requires-Dist: numpy (<1.24,~=1.21)
@@ -47,14 +47,15 @@
 Requires-Dist: build (>=0.8) ; extra == 'dev'
 Requires-Dist: ipython (>=7.16) ; extra == 'dev'
 Requires-Dist: isort (>=5.10) ; extra == 'dev'
 Requires-Dist: pdbpp (>=0.10) ; extra == 'dev'
 Requires-Dist: pip (>=21.1) ; extra == 'dev'
 Requires-Dist: pre-commit (>=2.20.0) ; extra == 'dev'
 Requires-Dist: psutil (~=5.1) ; extra == 'dev'
+Requires-Dist: twine (>=4.0) ; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: GitPython (>=3.1.30) ; extra == 'doc'
 Requires-Dist: mike (>=1.1.0) ; extra == 'doc'
 Requires-Dist: mkdocs-htmlproofer-plugin (>=0.8.0) ; extra == 'doc'
 Requires-Dist: mkdocs-material (>=8.5.6) ; extra == 'doc'
 Requires-Dist: mkdocstrings[python] (>=0.19.0) ; extra == 'doc'
 Provides-Extra: jax
@@ -67,238 +68,261 @@
 Requires-Dist: pytest-mock (>=3.8.2) ; extra == 'test'
 Requires-Dist: pytype (!=2021.11.18,!=2022.2.17) ; extra == 'test'
 Requires-Dist: pre-commit (>=2.20.0) ; extra == 'test'
 Requires-Dist: pytest-unordered (~=0.5) ; extra == 'test'
 Requires-Dist: tox (>=3.23.1) ; extra == 'test'
 Requires-Dist: tqdm (>=4.64.1) ; extra == 'test'
 
-<!--
-Copyright (c) 2021-2023, NVIDIA CORPORATION. All rights reserved.
+..
+    Copyright (c) 2021-2023, NVIDIA CORPORATION. All rights reserved.
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
--->
-
-# Project description
-
-The [Triton Model Navigator](https://github.com/triton-inference-server/model_navigator) automates
-the process of moving model from source to deployment on
-[Triton Inference Server](https://github.com/triton-inference-server/server). The tool validate possible
-export and conversion paths to serializable formats like [TensorRT](https://github.com/NVIDIA/TensorRT) and
-select the most promising format for production deployment.
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+Triton Model Navigator
+========================
+
+The `Triton Model Navigator`_ automates the process of moving model from source to deployment on
+`Triton Inference Server`_. The tool validate possible export and conversion paths to serializable formats like
+`TensorRT`_ and select the most promising format for production deployment.
 
 The Triton Model Navigator is designed to provide a single entrypoint for each supported framework. The usage is
 simple as call a dedicated `optimize` function to start the process of searching for the best
 possible deployment by going through a broad spectrum of model conversions.
 
 The `optimize` internally it performs model export, conversion, correctness testing, performance profiling,
 and saves all generated artifacts in the `navigator_workspace`, which is represented by a returned `package` object.
 The result of `optimize` process can be saved as a portable Navigator Package with the `save` function.
 Saved packages only contain the base model formats along with the best selected format based on latency and throughput.
 The package can be reused to recreate the process on same or different hardware. The configuration and execution status
 is saved in the `status.yaml` file located inside the workspace and the `Navigator Package`.
 
 Finally, the `Navigator Package` can be used for model deployment
-on [NVIDIA Triton Inference Server](https://github.com/triton-inference-server/server). Dedicated API helps with obtaining all
+on `Triton Inference Server`_. Dedicated API helps with obtaining all
 necessary parameters and creating `model_repository` or receive the optimized model for inference in Python environment.
 
-# Installing
+Installation
+--------------
 
-The package can be installed from `pypi.org` using:
+The package can be installed using extra index url:
 
-<!--pytest.mark.skip-->
 
-```shell
-pip install -U triton-model-navigator[<extras,>]
-```
+.. code-block:: text
+
+    pip install -U --extra-index-url https://pypi.ngc.nvidia.com triton-model-navigator[<extras,>]
+
+
+or with nvidia-pyindex:
+
+.. code-block:: text
+
+    pip install nvidia-pyindex
+    pip install -U triton-model-navigator[<extras,>]
+
 
 Extras:
 
-- tensorflow - Model Navigator for TensorFlow2
-- jax - Model Navigator for JAX
+- `tensorflow` - Model Navigator with dependencies for TensorFlow2
+- `jax` - Model Navigator with dependencies for JAX
+
+For using with PyTorch no extras are needed.
 
-# Quick Start
+Quick Start
+-------------
 
 The quick start presents how to optimize Python model for deployment on Triton Inference Server. In the
 example we are using a simple TensorFlow 2 model.
 
-## Export and optimize model
-
 To use Triton Model Navigator you must prepare model and dataloader. We recommend to create following helper
 functions:
 
 - `get_model` - return model object
 - `get_dataloader` - generate samples required for export and conversion
 - `get_verify_func` (optional) - validate the correctness of models based on implemented metric
 
 Next you can use Triton Model Navigator `optimize` function with provided model, dataloader and verify function
 to export and convert model to all supported formats.
 
 See the below example of optimizing a simple TensorFlow model.
 
-```python
-import logging
+.. code-block:: python
 
-import numpy as np
-import tensorflow as tf
+    import logging
 
-import model_navigator as nav
+    import numpy as np
+    import tensorflow as tf
 
-# enable tensorflow memory growth to avoid allocating all GPU memory
-gpus = tf.config.experimental.list_physical_devices("GPU")
-for gpu in gpus:
-    tf.config.experimental.set_memory_growth(gpu, True)
+    import model_navigator as nav
 
-LOGGER = logging.getLogger(__name__)
+    # enable tensorflow memory growth to avoid allocating all GPU memory
+    gpus = tf.config.experimental.list_physical_devices("GPU")
+    for gpu in gpus:
+        tf.config.experimental.set_memory_growth(gpu, True)
 
+    LOGGER = logging.getLogger(__name__)
 
-# dataloader is used for inference and finding input shapes of the model.
-# If you do not have dataloader, create one with samples with min and max shapes.
-def get_dataloader():
-    return [np.random.rand(1, 224, 224, 3).astype("float32") for _ in range(10)]
 
+    # dataloader is used for inference and finding input shapes of the model.
+    # If you do not have dataloader, create one with samples with min and max shapes.
+    def get_dataloader():
+        return [np.random.rand(1, 224, 224, 3).astype("float32") for _ in range(10)]
 
-def get_verify_function():
-    def verify_func(ys_runner, ys_expected):
-        for a, b in zip(ys_runner, ys_expected):
-            if not (np.isclose(a["output__0"], b["output__0"], atol=0.01)).all():
-                return False
 
-        return True
+    def get_verify_function():
+        def verify_func(ys_runner, ys_expected):
+            for a, b in zip(ys_runner, ys_expected):
+                if not (np.isclose(a["output__0"], b["output__0"], atol=0.01)).all():
+                    return False
 
-    return verify_func
+            return True
 
+        return verify_func
 
-# Model inputs must be a Tensor to support deployment on Triton Inference Server.
-def get_model():
-    inp = tf.keras.layers.Input((224, 224, 3))
-    layer_output = tf.keras.layers.Lambda(lambda x: x)(inp)
-    layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
-    layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
-    layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
-    layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
-    model_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
-    return tf.keras.Model(inp, model_output)
 
-# Check documentation for more details about Profiler Configuration options.
-def get_profiler_config():
-    return nav.ProfilerConfig()
+    # Model inputs must be a Tensor to support deployment on Triton Inference Server.
+    def get_model():
+        inp = tf.keras.layers.Input((224, 224, 3))
+        layer_output = tf.keras.layers.Lambda(lambda x: x)(inp)
+        layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
+        layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
+        layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
+        layer_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
+        model_output = tf.keras.layers.Lambda(lambda x: x)(layer_output)
+        return tf.keras.Model(inp, model_output)
 
+    # Check documentation for more details about Profiler Configuration options.
+    def get_profiler_config():
+        return nav.ProfilerConfig()
 
-model = get_model()
-dataloader = get_dataloader()
-verify_func = get_verify_function()
-profiler_config = get_profiler_config()
 
-# Model Navigator optimize starts export, optimization and testing process.
-# The resulting package represents all artifacts produced by Model Navigator.
-package = nav.tensorflow.optimize(
-    model=model,
-    profiler_config=profiler_config,
-    target_formats=(nav.Format.ONNX,),
-    dataloader=dataloader,
-    verify_func=verify_func,
-)
+    model = get_model()
+    dataloader = get_dataloader()
+    verify_func = get_verify_function()
+    profiler_config = get_profiler_config()
 
-# Save nav package that can be used for Triton Inference Server deployment or obtaining model runner later.
-# The package contains base format checkpoints that can be used for all other conversions.
-# Models with minimal latency and maximal throughput are added to the package.
-nav.package.save(package=package, path="mlp.nav")
-```
+    # Model Navigator optimize starts export, optimization and testing process.
+    # The resulting package represents all artifacts produced by Model Navigator.
+    package = nav.tensorflow.optimize(
+        model=model,
+        profiler_config=profiler_config,
+        target_formats=(nav.Format.ONNX,),
+        dataloader=dataloader,
+        verify_func=verify_func,
+    )
 
-You can customize behavior of export and conversion steps
-passing [CustomConfig][model_navigator.api.config.CustomConfig]
-to `optimize` function.
+    # Save nav package that can be used for Triton Inference Server deployment or obtaining model runner later.
+    # The package contains base format checkpoints that can be used for all other conversions.
+    # Models with minimal latency and maximal throughput are added to the package.
+    nav.package.save(package=package, path="mlp.nav")
 
-## NVIDIA Triton Inference Server deployment
+You can customize behavior of export and conversion steps passing CustomConfig to `optimize` function.
 
-If you prefer the standalone [NVIDIA Triton Inference Server](https://github.com/triton-inference-server) you can create
-and use `model_repository`.
+Deploying Model in PyTriton
+-----------------------------
 
-```python
-import logging
-import pathlib
+At this point you can use `PyTriton`_ for easy deployment of the exported model. Below you can find an example
+`serve.py` that will select the best model from a previously saved `Navigator Package`, get the best runner, and use
+it to start `PyTriton`.
 
-from model_navigator.exceptions import (
-    ModelNavigatorEmptyPackageError,
-    ModelNavigatorError,
-    ModelNavigatorWrongParameterError
-)
-import model_navigator as nav
+.. code-block:: python
 
-LOGGER = logging.getLogger(__name__)
+    from pytriton.decorators import batch
+    from pytriton.triton import Triton
 
-package = nav.package.load("mlp.nav", "load_workspace")
+    import model_navigator as nav
 
-# Create model_repository for standalone Triton deployment
-try:
-    nav.triton.model_repository.add_model_from_package(
-        model_repository_path=pathlib.Path("model_repository"), model_name="dummy_model", package=package
-    )
-except (ModelNavigatorWrongParameterError, ModelNavigatorEmptyPackageError, ModelNavigatorError) as e:
-    LOGGER.warning(f"Model repository cannot be created.\n{str(e)}")
-```
+    package = nav.package.load("mlp.nav", "load_workspace")
 
-Use command to start server with provided `model_repository`:
+    pytriton_adapter = nav.pytriton.PyTritonAdapter(package=package)
+    runner = pytriton_adapter.runner
+    runner.activate()
 
-```shell
-$ docker run --gpus=1 --rm \
-  -p8000:8000 \
-  -p8001:8001 \
-  -p8002:8002 \
-  -v ${PWD}/model_repository:/models \
-  nvcr.io/nvidia/tritonserver:23.01-py3 \
-  tritonserver --model-repository=/models
-```
 
-# Examples
+    @batch
+    def infer_func(**inputs):
+        return runner.infer(inputs)
 
-We provide simple examples how to use Triton Model Navigator to optimize the PyTorch, TensorFlow2, JAX and ONNX models
-for deployment on Triton Inference Server.
 
-## Optimize for various frameworks
+    # Connecting inference callback with Triton Inference Server
+    with Triton() as triton:
+        # Load model into Triton Inference Server
+        triton.bind(
+            model_name="mlp",
+            infer_func=infer_func,
+            inputs=pytriton_adapter.inputs,
+            outputs=pytriton_adapter.outputs,
+            config=pytriton_adapter.config,
+        )
+        # Serve model through Triton Inference Server
+        triton.serve()
+
+
+Deploying Model in Triton Inference Server
+--------------------------------------------
+
+If you prefer the standalone `Triton Inference Server`_ you can create and use `model_repository`.
 
-- `PyTorch`:
-  * [Linear Model](https://github.com/triton-inference-server/model_navigator/examples/torch/linear)
-  * [ResNet50](https://github.com/triton-inference-server/model_navigator/examples/torch/resnet50)
-  * [BERT](https://github.com/triton-inference-server/model_navigator/examples/torch/bert)
+.. code-block:: python
 
-- `TensorFlow`:
-  * [Linear Model](https://github.com/triton-inference-server/model_navigator/examples/tensorflow/linear)
-  * [EfficientNet](https://github.com/triton-inference-server/model_navigator/examples/tensorflow/efficientnet)
-  * [BERT](https://github.com/triton-inference-server/model_navigator/examples/tensorflow/bert)
+    import logging
+    import pathlib
 
-- `JAX`:
-  * [Linear Model](https://github.com/triton-inference-server/model_navigator/examples/jax/linear)
-  * [GPT-2](https://github.com/triton-inference-server/model_navigator/examples/jax/gpt2)
+    from model_navigator.exceptions import (
+        ModelNavigatorEmptyPackageError,
+        ModelNavigatorError,
+        ModelNavigatorWrongParameterError
+    )
+    import model_navigator as nav
+
+    LOGGER = logging.getLogger(__name__)
 
-- `ONNX`:
-  * [Identity Model](https://github.com/triton-inference-server/model_navigator/examples/onnx/identity)
+    package = nav.package.load("mlp.nav", "load_workspace")
 
-## Optimize Navigator Package
+    # Create model_repository for standalone Triton deployment
+    try:
+        nav.triton.model_repository.add_model_from_package(
+            model_repository_path=pathlib.Path("model_repository"), model_name="dummy_model", package=package
+        )
+    except (ModelNavigatorWrongParameterError, ModelNavigatorEmptyPackageError, ModelNavigatorError) as e:
+        LOGGER.warning(f"Model repository cannot be created.\n{str(e)}")
 
-The Navigator Package can be reused for optimize e.g. on the new hardware or with newer libraries.
-The example code can be found in [examples/package](https://github.com/triton-inference-server/model_navigator/examples/package).
+Use command to start server with provided `model_repository`:
 
-## Using model on Triton Inference Server
+.. code-block:: text
 
-The optimized model by Triton Model Navigator can be used for serving inference through Triton Inference Server. The
-example code can be found in [examples/triton](https://github.com/triton-inference-server/model_navigator/examples/triton).
+    $ docker run --gpus=1 --rm \
+      -p8000:8000 \
+      -p8001:8001 \
+      -p8002:8002 \
+      -v ${PWD}/model_repository:/models \
+      nvcr.io/nvidia/tritonserver:23.01-py3 \
+      tritonserver --model-repository=/models
 
+Examples
+----------
+
+We provide simple examples how to use Triton Model Navigator to optimize the PyTorch, TensorFlow2, JAX and ONNX models
+for deployment on Triton Inference Server. See more in  https://github.com/triton-inference-server/model_navigator/tree/main/examples.
 
-# Links
+Links
+-------
 
 * Documentation: https://triton-inference-server.github.io/model_navigator
 * Source: https://github.com/triton-inference-server/model_navigator
 * Issues: https://github.com/triton-inference-server/model_navigator/issues
-* Changelog: https://github.com/triton-inference-server/model_navigator/CHANGELOG.md
-* Known Issues: https://github.com/triton-inference-server/model_navigator/docs/known_issues.md
-* Contributing: https://github.com/triton-inference-server/model_navigator/CONTRIBUTING.md
+* Changelog: https://github.com/triton-inference-server/model_navigator/blob/main/CHANGELOG.md
+* Known Issues: https://github.com/triton-inference-server/model_navigator/blob/main/docs/known_issues.md
+* Contributing: https://github.com/triton-inference-server/model_navigator/blob/main/CONTRIBUTING.md
+
+.. _Triton Model Navigator: https://github.com/triton-inference-server/model_navigator
+.. _Triton Inference Server: https://github.com/triton-inference-server/server
+.. _TensorRT: https://github.com/NVIDIA/TensorRT
+.. _PyTriton: https://github.com/triton-inference-server/pytriton
```

## Comparing `triton_model_navigator-0.5.1.dist-info/RECORD` & `triton_model_navigator-0.5.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=AhBdz0hW6zgobgw4p2wnOEiVi-da0VjWix81dmxbtv8,649
+model_navigator/__version__.py,sha256=wdjyiPqcy9thC_Z8iQnQrvUMqi5_PP5GlvWcZrQyGY4,649
 model_navigator/exceptions.py,sha256=6wR9REQeNkmHOklMPQ46SrGC61EJVH4jz0n2BC4e7ek,3668
 model_navigator/execution_context.py,sha256=eYV2YJU4V8X-v-dWTI6Oi5zJl3RdtK41XWtPxPRxNvU,9474
 model_navigator/logger.py,sha256=-qSYoA16yl2NdJOyqazlUUY73jTyWqaMCB6xt0KuNpc,3793
 model_navigator/api/__init__.py,sha256=gnYVwaepcIMj_380kVpdKxdEU0HpyWHDedNoBbZJpAA,1520
 model_navigator/api/config.py,sha256=u2VRwZh1v3s6y_rnEWGi1FLPc1oTv7cXy-axs4ch0Jo,21958
 model_navigator/api/jax.py,sha256=6sZHQuG1wQXl5R0xWn1cCInLhbde4M5CfTWWEP2iBeg,6362
 model_navigator/api/onnx.py,sha256=acon_yfZNeQUw20uZOfdIek3KH0rLiXVxReoxwUFAiM,5372
@@ -14,15 +14,15 @@
 model_navigator/api/torch.py,sha256=nQo2Oa_elF5Ia65fhbohiPYOQTqFSr2VX0-RDb1m9Gs,6257
 model_navigator/api/triton.py,sha256=hdrU_WJn5DFzhJ5slcdJqzRcC7n69vhmP0RKa1B3QYQ,1553
 model_navigator/commands/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/base.py,sha256=O75ENxJH4GtjYHru56h5XSLrR_iqnsbaQE7YHbtOnLk,4938
 model_navigator/commands/infer_metadata.py,sha256=KqWupE_d4wPv6o90uIuT1y3Pze0yxR9S1oesqfk1yjE,10071
 model_navigator/commands/load.py,sha256=7v1YqLbG0VZOf981XW-2Y6ad828d4Ynq2HNmj7_a8ys,3289
 model_navigator/commands/convert/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/convert/base.py,sha256=5UWY1wsQ9m13wo8AmH3FiALfG7YQrvgxqhVHadLx4rw,7015
+model_navigator/commands/convert/base.py,sha256=AqLMNnO5jLkdeOzQtWDALzURMy53RWokTuUYZ6Q9xi0,7039
 model_navigator/commands/convert/tf.py,sha256=tQw4DTmAqzDO0pr7ZPMjzTInmd11qmsNIKW6JsWasNM,7838
 model_navigator/commands/convert/torch.py,sha256=IMZQ-8dYsu_PuEMBSWbJJgejZIAZr-X_Gu-ANS09SDg,10151
 model_navigator/commands/convert/converters/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/converters/sm2tftrt.py,sha256=AcNyKV60yCUrzJ5B501H5SHKjtkr7kaNXNIewnOFJzk,3418
 model_navigator/commands/convert/converters/ts2onnx.py,sha256=ezjlPeHHbhx2LB4HDoLkVlmaZa1dreVMQMk2PL5UMos,3105
 model_navigator/commands/convert/converters/ts2torchtrt.py,sha256=a_mpR0j4y5ClaY6Ik_oIKEAlh45zD-ycCLHigsy1C7M,4992
 model_navigator/commands/convert/onnx/__init__.py,sha256=LwvvDj4oH7rwmUJXVEyRxIOWZnUxix6n_DmkAJzEJBY,680
@@ -54,21 +54,21 @@
 model_navigator/commands/performance/performance_script.py,sha256=KFNDTY_4QDhQyZl-ew34vlWIBebgQcm4yrpS8_MARNg,3038
 model_navigator/commands/verification/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/verification/verify.py,sha256=Rst9gQdWUiJLtTHNWDGb3SyJ3mnHHK8ENDUmjifP5UI,5447
 model_navigator/configuration/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/configuration/common_config.py,sha256=6DWPjzYWN5K6T3WMYZbSiySZIINJpXK-2hQ2Hh4kmPA,2478
 model_navigator/configuration/model/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/configuration/model/model_config.py,sha256=_CS3i4OGmHmWyGAywrgV6T6y0I_9Cd-2NhWT_7U8CN8,14775
-model_navigator/configuration/model/model_config_builder.py,sha256=TGGVAk9VO61esqSGmT-GEm4TR6sFbpFjUTUZh6S37O4,13263
+model_navigator/configuration/model/model_config_builder.py,sha256=HBMlQYpoVHHHdPZpVpnnuf4IqdFywrehDQCR37EDTtw,13482
 model_navigator/core/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/core/constants.py,sha256=ZexQn5QcgGiw1mLBTxgVcgDURGqxCqqBgPIhV7qPrKI,1213
 model_navigator/core/package.py,sha256=dKbkYc0DlIGgVueuz4wZztCuu5cQc3nMcUsYedihia4,20118
 model_navigator/core/status.py,sha256=yX5FeszIQikqL_K5KJnOONWioTutZf5crI7VYR5ePig,20332
 model_navigator/pipelines/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/pipelines/pipeline.py,sha256=MkkrtRGCXAUhTEoYTOMEWzipbqkd2YbWPSkUNm4Ano0,5405
+model_navigator/pipelines/pipeline.py,sha256=vdf2Hp1TRa_biNFo-Af9fVjKBTs9ddOE-lfHKQSdixo,5451
 model_navigator/pipelines/pipeline_manager.py,sha256=YQL2Om9ncR_cpxZJL2hkdwSkEH28311zhLwHbNIoDu0,7334
 model_navigator/pipelines/validation.py,sha256=VI5aXRdamesaGpk0W7QVTzlO3Fvg15s6WROyv4tI6xE,9810
 model_navigator/pipelines/builders/__init__.py,sha256=ACocrstiz-vJgSJDzZAfGS_PlJeUZlgj2gNXebnTd4c,1884
 model_navigator/pipelines/builders/correctness.py,sha256=LIm_qCMu33l1tbKw2FcJ_8rAlumg7hHZxsXwuRylJCM,2036
 model_navigator/pipelines/builders/find_device_max_batch_size.py,sha256=oanNorsNuH9ZWixoL973IfLMTLxNT0VeiyZ_KUR9rJI,4749
 model_navigator/pipelines/builders/jax.py,sha256=Xy-C-ciFrQ7_9QQYCq5JOGm58SLz3t9i-pgMnfxSvlU,1647
 model_navigator/pipelines/builders/onnx.py,sha256=_8xt1Fd-hnskzz64k6pV2Xykr9iKeg5UqyaOLO7F_ho,2395
@@ -118,12 +118,12 @@
 model_navigator/utils/onnx.py,sha256=L3IDVu0r-_BHSdf4htXwsmMVPoInk9Qset6SA66LusI,1085
 model_navigator/utils/package.py,sha256=exDhwNvvNXGQlZXSjRuVOzX6z4N9eI28Nb2VxbqfxnU,3239
 model_navigator/utils/pipelines.py,sha256=70riAoXSEezI3KDv_6el-SiuWyB6pW44EgN_rwYswwY,1331
 model_navigator/utils/runners.py,sha256=euFHUjrB3_sSvHI0ClEAx1pDa5RbvQAlPrRY1LwG4bc,3171
 model_navigator/utils/tensor.py,sha256=C2T3JIj-XYLjAwPD1kR4lOrGeNVhcFQSYdfxM7U1kPE,8054
 model_navigator/utils/tensorrt.py,sha256=qx5Ed47xLZC2CYSQk6kUUf3-nBvsV92GJA8t5_jUWbQ,2848
 model_navigator/utils/torch.py,sha256=czQ3umUl1UtYydDApapftpEOBZsWCAdVyPD5wF9Gjq8,1508
-triton_model_navigator-0.5.1.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.5.1.dist-info/METADATA,sha256=1uDBxH1Fb3JvadqaO3omJNAWZwjRKNVg6DOOu75DNbM,12550
-triton_model_navigator-0.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.5.1.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.5.1.dist-info/RECORD,,
+triton_model_navigator-0.5.2.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.5.2.dist-info/METADATA,sha256=hMMAyRabXVGgp9zPr0g4mQ5CNeRSPmVy_UebAPuKUck,13041
+triton_model_navigator-0.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.5.2.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.5.2.dist-info/RECORD,,
```

