# Comparing `tmp/sparseml_nightly-1.5.0.20230404-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.5.0.20230412-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 944783 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1780 b- defN 23-Apr-04 03:01 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Apr-04 03:01 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-04 03:01 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Apr-04 03:01 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Apr-04 03:01 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Apr-04 03:01 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Apr-04 03:01 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Apr-04 03:01 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Apr-04 03:01 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Apr-04 03:01 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Apr-04 03:01 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Apr-04 03:01 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Apr-04 03:01 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Apr-04 03:01 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Apr-04 03:01 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Apr-04 03:01 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4751 b- defN 23-Apr-04 03:01 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Apr-04 03:01 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Apr-04 03:01 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Apr-04 03:01 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      961 b- defN 23-Apr-04 03:01 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Apr-04 03:01 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Apr-04 03:01 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Apr-04 03:01 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Apr-04 03:01 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Apr-04 03:01 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Apr-04 03:01 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Apr-04 03:01 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Apr-04 03:01 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Apr-04 03:01 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Apr-04 03:01 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Apr-04 03:01 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Apr-04 03:01 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Apr-04 03:01 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Apr-04 03:01 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Apr-04 03:01 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Apr-04 03:01 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Apr-04 03:01 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Apr-04 03:01 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Apr-04 03:01 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Apr-04 03:01 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Apr-04 03:01 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-04 03:01 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Apr-04 03:01 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Apr-04 03:01 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Apr-04 03:01 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Apr-04 03:01 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Apr-04 03:01 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Apr-04 03:01 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1027 b- defN 23-Apr-04 03:01 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Apr-04 03:01 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Apr-04 03:01 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Apr-04 03:01 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Apr-04 03:01 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Apr-04 03:01 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13274 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19634 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14520 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Apr-04 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Apr-04 03:01 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Apr-04 03:01 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Apr-04 03:01 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Apr-04 03:01 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13002 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    41311 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31586 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Apr-04 03:01 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      725 b- defN 23-Apr-04 03:01 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3694 b- defN 23-Apr-04 03:01 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Apr-04 03:01 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Apr-04 03:01 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Apr-04 03:01 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Apr-04 03:01 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Apr-04 03:01 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Apr-04 03:01 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Apr-04 03:01 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Apr-04 03:01 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Apr-04 03:01 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-Apr-04 03:01 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Apr-04 03:01 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10826 b- defN 23-Apr-04 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Apr-04 03:01 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Apr-04 03:01 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Apr-04 03:01 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      750 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Apr-04 03:01 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40931 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Apr-04 03:01 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-04 03:01 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Apr-04 03:01 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Apr-04 03:01 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Apr-04 03:01 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-04 03:01 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26830 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Apr-04 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Apr-04 03:01 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Apr-04 03:01 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Apr-04 03:01 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Apr-04 03:01 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24133 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26253 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69783 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Apr-04 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      741 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    40790 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Apr-04 03:01 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31056 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    38949 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8382 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Apr-04 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Apr-04 03:01 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Apr-04 03:01 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-04 03:01 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Apr-04 03:01 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Apr-04 03:01 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Apr-04 03:01 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Apr-04 03:01 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Apr-04 03:01 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Apr-04 03:01 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Apr-04 03:01 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Apr-04 03:01 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Apr-04 03:01 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Apr-04 03:01 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Apr-04 03:01 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      985 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Apr-04 03:01 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     4388 b- defN 23-Apr-04 03:01 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    19721 b- defN 23-Apr-04 03:01 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30936 b- defN 23-Apr-04 03:01 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36738 b- defN 23-Apr-04 03:01 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40358 b- defN 23-Apr-04 03:01 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34464 b- defN 23-Apr-04 03:01 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Apr-04 03:01 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Apr-04 03:01 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43756 b- defN 23-Apr-04 03:01 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Apr-04 03:01 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Apr-04 03:01 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Apr-04 03:01 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Apr-04 03:01 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    15797 b- defN 23-Apr-04 03:01 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Apr-04 03:01 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Apr-04 03:01 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-Apr-04 03:01 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Apr-04 03:01 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-04 03:01 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Apr-04 03:01 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Apr-04 03:01 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Apr-04 03:01 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Apr-04 03:01 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Apr-04 03:01 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4018 b- defN 23-Apr-04 03:01 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Apr-04 03:01 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     3264 b- defN 23-Apr-04 03:01 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Apr-04 03:01 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Apr-04 03:01 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Apr-04 03:01 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx      956 b- defN 23-Apr-04 03:01 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5762 b- defN 23-Apr-04 03:01 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2121 b- defN 23-Apr-04 03:01 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Apr-04 03:01 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     6806 b- defN 23-Apr-04 03:01 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    30600 b- defN 23-Apr-04 03:01 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2243 b- defN 23-Apr-04 03:01 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8032 b- defN 23-Apr-04 03:01 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Apr-04 03:01 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6298 b- defN 23-Apr-04 03:01 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     1355 b- defN 23-Apr-04 03:01 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/LICENSE
--rw-rw-r--  2.0 unx    20658 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2372 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36575 b- defN 23-Apr-04 03:04 sparseml_nightly-1.5.0.20230404.dist-info/RECORD
-368 files, 3418632 bytes uncompressed, 885575 bytes compressed:  74.1%
+Zip file size: 946339 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Apr-12 03:01 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Apr-12 03:01 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-12 03:01 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Apr-12 03:01 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Apr-12 03:01 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Apr-12 03:01 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Apr-12 03:01 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Apr-12 03:01 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Apr-12 03:01 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Apr-12 03:01 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Apr-12 03:01 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Apr-12 03:01 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Apr-12 03:01 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Apr-12 03:01 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-12 03:01 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Apr-12 03:01 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4751 b- defN 23-Apr-12 03:01 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Apr-12 03:01 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Apr-12 03:01 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-Apr-12 03:01 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Apr-12 03:01 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Apr-12 03:01 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Apr-12 03:01 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Apr-12 03:01 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Apr-12 03:01 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Apr-12 03:01 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Apr-12 03:01 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Apr-12 03:01 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Apr-12 03:01 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Apr-12 03:01 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Apr-12 03:01 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Apr-12 03:01 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Apr-12 03:01 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Apr-12 03:01 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Apr-12 03:01 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-12 03:01 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Apr-12 03:01 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Apr-12 03:01 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Apr-12 03:01 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Apr-12 03:01 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Apr-12 03:01 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Apr-12 03:01 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Apr-12 03:01 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Apr-12 03:01 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Apr-12 03:01 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Apr-12 03:01 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Apr-12 03:01 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Apr-12 03:01 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13274 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19634 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14520 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4514 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13002 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    41311 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31586 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      734 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3694 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Apr-12 03:01 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Apr-12 03:01 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Apr-12 03:01 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Apr-12 03:01 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Apr-12 03:01 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Apr-12 03:01 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Apr-12 03:01 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Apr-12 03:01 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Apr-12 03:01 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10826 b- defN 23-Apr-12 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Apr-12 03:01 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Apr-12 03:01 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26253 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69783 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      744 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    40790 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31056 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    38949 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Apr-12 03:01 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Apr-12 03:01 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-12 03:01 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Apr-12 03:01 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Apr-12 03:01 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Apr-12 03:01 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Apr-12 03:01 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Apr-12 03:01 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Apr-12 03:01 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Apr-12 03:01 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     4390 b- defN 23-Apr-12 03:01 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    19721 b- defN 23-Apr-12 03:01 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30936 b- defN 23-Apr-12 03:01 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36738 b- defN 23-Apr-12 03:01 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40358 b- defN 23-Apr-12 03:01 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34464 b- defN 23-Apr-12 03:01 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43756 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    15797 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Apr-12 03:01 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Apr-12 03:01 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-Apr-12 03:01 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Apr-12 03:01 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-12 03:01 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Apr-12 03:01 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Apr-12 03:01 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Apr-12 03:01 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Apr-12 03:01 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Apr-12 03:01 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Apr-12 03:01 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     3266 b- defN 23-Apr-12 03:01 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Apr-12 03:01 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Apr-12 03:01 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Apr-12 03:01 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx      958 b- defN 23-Apr-12 03:01 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Apr-12 03:01 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2845 b- defN 23-Apr-12 03:01 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Apr-12 03:01 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7318 b- defN 23-Apr-12 03:01 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    33189 b- defN 23-Apr-12 03:01 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2710 b- defN 23-Apr-12 03:01 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     7666 b- defN 23-Apr-12 03:01 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Apr-12 03:01 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6298 b- defN 23-Apr-12 03:01 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     2534 b- defN 23-Apr-12 03:01 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    20659 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2372 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36575 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/RECORD
+368 files, 3423725 bytes uncompressed, 887131 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/LICENSE
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/METADATA
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/NOTICE
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/WHEEL
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/top_level.txt
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230404.dist-info/RECORD
+Filename: sparseml_nightly-1.5.0.20230412.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/__init__.py

```diff
@@ -42,20 +42,8 @@
     sparsification_info,
     save_sparsification_info,
     load_sparsification_info,
 )
 from .analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("python.import")
-
-try:
-    from sparsezoo.package import check_package_version as _check_package_version
-
-    _check_package_version(
-        package_name=__name__ if is_release else f"{__name__}-nightly",
-        package_version=version,
-    )
-except Exception as err:
-    print(
-        f"Need sparsezoo version above 0.9.0 to run Neural Magic's latest-version check\n{err}"
-    )
+_analytics.send_event("python__init")
```

## sparseml/keras/__init__.py

```diff
@@ -21,8 +21,8 @@
 from sparseml.analytics import sparseml_analytics as _analytics
 
 from .base import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import sparsification_info
 
 
-_analytics.send_event("keras.init")
+_analytics.send_event("python__keras__init")
```

## sparseml/onnx/__init__.py

```diff
@@ -22,8 +22,8 @@
 
 from .base import *
 from .benchmark import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import ModelInfo, get_analyzer_impls, sparsification_info
 
 
-_analytics.send_event("onnx.init")
+_analytics.send_event("python__onnx__init")
```

## sparseml/openpifpaf/__init__.py

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("openpifpaf.init")
+_analytics.send_event("python__openpifpaf__init")
```

## sparseml/pytorch/image_classification/__init__.py

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("python.pytorch.image_classification.init")
+_analytics.send_event("python__pytorch__image_classification__init")
```

## sparseml/pytorch/models/classification/resnet.py

```diff
@@ -136,34 +136,17 @@
         _init_batch_norm(self.bn)
 
     @staticmethod
     def required(in_channels: int, out_channels: int, stride: int) -> bool:
         return in_channels != out_channels or stride > 1
 
 
-class _AddReLU(Module):
-    """
-    Wrapper for the FloatFunctional class that enables QATWrapper used to
-    quantize the first input to the Add operation
-    """
-
-    def __init__(self, num_channels):
-        super().__init__()
-        if FloatFunctional:
-            self.functional = FloatFunctional()
-            self.wrap_qat = True
-            self.qat_wrapper_kwargs = {"num_inputs": 1, "num_outputs": 1}
-        else:
-            self.functional = ReLU(num_channels=num_channels, inplace=True)
-
-    def forward(self, x, y):
-        if isinstance(self.functional, FloatFunctional):
-            return self.functional.add_relu(x, y)
-        else:
-            return self.functional(x + y)
+class AddInput(Module):
+    def forward(self, x):
+        return x
 
 
 class _BasicBlock(Module):
     def __init__(self, in_channels: int, out_channels: int, stride: int = 1):
         super().__init__()
         self.conv1 = Conv2d(
             in_channels,
@@ -181,33 +164,34 @@
         self.bn2 = BatchNorm2d(out_channels)
         self.identity = (
             _IdentityModifier(in_channels, out_channels, stride)
             if _IdentityModifier.required(in_channels, out_channels, stride)
             else None
         )
 
-        # self.add_relu = _AddReLU(out_channels)
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
         if FloatFunctional:
             self.add_relu = FloatFunctional()
         else:
             self.add_relu = ReLU(num_channels=out_channels, inplace=True)
 
         self.initialize()
 
     def forward(self, inp: Tensor):
         out = self.conv1(inp)
         out = self.bn1(out)
         out = self.act1(out)
 
         out = self.conv2(out)
         out = self.bn2(out)
+        out = self.add_input_conv(out)
 
         identity_val = self.identity(inp) if self.identity is not None else inp
-        # out = self.add_relu(identity_val, out)
-        # return out
+        identity_val = self.add_input_identity(identity_val)
 
         if isinstance(self.add_relu, FloatFunctional):
             return self.add_relu.add_relu(identity_val, out)
         else:
             return self.add_relu(identity_val + out)
 
     def initialize(self):
@@ -246,15 +230,16 @@
         self.bn3 = BatchNorm2d(out_channels)
         self.identity = (
             _IdentityModifier(in_channels, out_channels, stride)
             if _IdentityModifier.required(in_channels, out_channels, stride)
             else None
         )
 
-        # self.add_relu = _AddReLU(out_channels)
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
         if FloatFunctional:
             self.add_relu = FloatFunctional()
         else:
             self.add_relu = ReLU(num_channels=out_channels, inplace=True)
 
         self.initialize()
 
@@ -265,19 +250,18 @@
 
         out = self.conv2(out)
         out = self.bn2(out)
         out = self.act2(out)
 
         out = self.conv3(out)
         out = self.bn3(out)
+        out = self.add_input_conv(out)
 
         identity_val = self.identity(inp) if self.identity is not None else inp
-
-        # out = self.add_relu(identity_val, out)
-        # return out
+        identity_val = self.add_input_identity(identity_val)
 
         if isinstance(self.add_relu, FloatFunctional):
             return self.add_relu.add_relu(identity_val, out)
         else:
             return self.add_relu(identity_val + out)
 
     def initialize(self):
@@ -311,28 +295,33 @@
 
         self.identity = (
             Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=False)
             if in_channels != out_channels or stride != 1
             else None
         )
 
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
+
         self.initialize()
 
     def forward(self, inp: Tensor):
         identity = inp
 
         out = self.bn1(inp)
         out = self.act1(out)
         if self.identity is not None:
             identity = self.identity(out)
+            identity = self.add_input_identity(identity)
         out = self.conv1(out)
 
         out = self.bn2(out)
         out = self.act2(out)
         out = self.conv2(out)
+        out = self.add_input_conv(out)
 
         out += identity
 
         return out
 
     def initialize(self):
         _init_conv(self.conv1)
@@ -373,33 +362,37 @@
         self.conv3 = Conv2d(proj_channels, out_channels, kernel_size=1, bias=False)
 
         self.identity = (
             Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=False)
             if in_channels != out_channels or stride != 1
             else None
         )
+        self.add_input_conv = AddInput()
+        self.add_input_identity = AddInput()
 
         self.initialize()
 
     def forward(self, inp: Tensor):
         identity = inp
 
         out = self.bn1(inp)
         out = self.act1(out)
         if self.identity is not None:
             identity = self.identity(out)
+            identity = self.add_input_identity(identity)
         out = self.conv1(out)
 
         out = self.bn2(out)
         out = self.act2(out)
         out = self.conv2(out)
 
         out = self.bn3(out)
         out = self.act3(out)
         out = self.conv3(out)
+        out = self.add_input_conv(out)
 
         out += identity
 
         return out
 
     def initialize(self):
         _init_batch_norm(self.bn1)
```

## sparseml/pytorch/optim/manager.py

```diff
@@ -300,15 +300,15 @@
         return manager
 
     def __init__(
         self,
         modifiers: List[ScheduledModifier],
         metadata: Optional[Dict[str, Any]] = None,
     ):
-        sparseml_analytics.send_event("python.pytorch.manager")
+        sparseml_analytics.send_event("python__pytorch__manager__init")
         super().__init__(modifiers=modifiers, metadata=metadata)
         self._initialize_epoch = 0
 
     def state_dict(self) -> Dict[str, Dict]:
         """
         :return: Dictionary to store any state variables for this manager.
             Includes all modifiers nested under this manager as sub keys in the dict.
```

## sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py

```diff
@@ -290,15 +290,14 @@
             super().check_mask_update(
                 module,
                 epoch,
                 steps_per_epoch,
                 recomputation_sparsity=recomputation_sparsity,
             )
 
-        torch.cuda.empty_cache()
         self._last_applied_sparsity = to_apply_sparsities
         if self._scorer._is_main_proc:
             self._scorer._enabled_grad_buffering = False
 
     def _get_mask_creator(
         self, param_names: List[str], params: List[Parameter]
     ) -> PruningMaskCreator:
@@ -384,15 +383,15 @@
         self,
         params: List[Parameter],
         num_grads: int,
         damp: float,
         fisher_block_size: int,
         mask_type: str,
     ):
-        super().__init__(params)
+        super().__init__(params, dist_backend="nccl")
         self._num_grads = num_grads
         self._damp = damp
         self._fisher_block_size = fisher_block_size
         self._mask_type = mask_type
 
         self._finvs = None  # type: List[EmpiricalBlockFisherInverse]
         self._enabled_grad_buffering = False
```

## sparseml/pytorch/torchvision/__init__.py

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("python.pytorch.torchvision.init")
+_analytics.send_event("python__pytorch__torchvision__init")
```

## sparseml/pytorch/utils/sparsification.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """
 Helper functions for retrieving information related to model sparsification
 """
 
 import json
+import logging
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
     Iterator,
@@ -42,14 +43,16 @@
 
 
 __all__ = [
     "ModuleSparsificationInfo",
     "GradSampler",
 ]
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class ModuleSparsificationInfo:
     """
     Helper class for providing information related to torch Module parameters
     and the amount of sparsification applied. Includes information for pruning
     and quantization
 
@@ -250,8 +253,15 @@
                     # yield so gradients can be collected
                     computed_grads += 1
                     yield computed_grads
                     if progress_bar:
                         pbar.update(1)
                     if computed_grads >= num_grads:
                         break
+                if computed_grads < num_grads:
+                    _LOGGER.warning(
+                        f"The requested num_grads:{num_grads} is greater than allowed by the dataset. \
+                        Proceeding with less than requested. \
+                        Please reduce num_grads to suppress the warning."
+                    )
+                    break
         module.zero_grad()
```

## sparseml/tensorflow_v1/__init__.py

```diff
@@ -21,8 +21,8 @@
 from sparseml.analytics import sparseml_analytics as _analytics
 
 from .base import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import sparsification_info
 
 
-_analytics.send_event("python.tensorflow_v1.init")
+_analytics.send_event("python__tensorflow_v1__init")
```

## sparseml/transformers/__init__.py

```diff
@@ -20,15 +20,15 @@
 
 import logging as _logging
 
 import pkg_resources
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("python.transformers.init")
+_analytics.send_event("python__transformers__init")
 
 _EXPECTED_VERSION = "4.23.1"
 
 
 _LOGGER = _logging.getLogger(__name__)
 _NM_TRANSFORMERS_TAR_TEMPLATE = (
     "https://github.com/neuralmagic/transformers/releases/download/"
```

## sparseml/yolact/__init__.py

```diff
@@ -19,15 +19,15 @@
 import importlib
 import logging as _logging
 from collections import namedtuple
 
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("python.yolact.init")
+_analytics.send_event("python__yolact__init")
 
 _LOGGER = _logging.getLogger(__name__)
 _NM_YOLACT_LINK_TEMPLATE = (
     "https://github.com/neuralmagic/yolact/releases/download/"
     "{version}/yolact-0.0.1-py3-none-any.whl"
 )
```

## sparseml/yolov5/__init__.py

```diff
@@ -20,15 +20,15 @@
 import logging as _logging
 
 from sparseml.analytics import sparseml_analytics as _analytics
 
 from .helpers import *
 
 
-_analytics.send_event("python.yolov5.init")
+_analytics.send_event("python__yolov5__init")
 
 try:
     import yolov5 as _yolov5
 
     _yolov5_import_error = None
 except Exception as _yolov5_import_err:
     _yolov5_import_error = _yolov5_import_err
```

## sparseml/yolov8/__init__.py

```diff
@@ -12,14 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import ultralytics
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
-_analytics.send_event("python.yolov8.init")
+_analytics.send_event("python__yolov8__init")
 
 if "8.0.30" not in ultralytics.__version__:
     raise ValueError(
         f"ultralytics==8.0.30 is required, found {ultralytics.__version__}. "
         "To fix run `pip install sparseml[ultralytics]`."
     )
```

## sparseml/yolov8/default.yaml

```diff
@@ -1,11 +1,12 @@
 # Default training settings and hyperparameters for medium-augmentation COCO training
 
 recipe: null
 recipe_args: null
+datasets_dir: null
 
 task: "detect" # choices=['detect', 'segment', 'classify', 'init'] # init is a special case. Specify task to run.
 mode: "train" # choices=['train', 'val', 'predict'] # mode to run task in.
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model: "yolov8n.yaml" # i.e. yolov8n.pt, yolov8n.yaml. Path to model file
 data: "coco128.yaml" # i.e. coco128.yaml. Path to data file
```

## sparseml/yolov8/export.py

```diff
@@ -8,16 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+
 import click
 from sparseml.yolov8.trainers import SparseYOLO
+from ultralytics.yolo.utils import USER_CONFIG_DIR, get_settings, yaml_save
 
 
 # Options generated from
 # https://github.com/ultralytics/ultralytics/blob/main/ultralytics/yolo/configs/default.yaml
 
 
 @click.command(
@@ -59,17 +62,42 @@
     default=0,
     help="Number of samples to export with onnx",
 )
 @click.option(
     "--save-one-shot-torch",
     default=False,
     help="If one-shot recipe is supplied and "
-    "this flag is set to True,mthe torch model with "
+    "this flag is set to True,the torch model with "
     "the one-shot recipe applied will be exported.",
 )
+@click.option(
+    "--deterministic",
+    default=True,
+    is_flag=True,
+    help="whether to enable deterministic mode",
+)
+@click.option(
+    "--device",
+    default=None,
+    type=str,
+    help="cuda device, i.e. 0 or 0,1,2,3 or cpu. Device to run on",
+)
+@click.option(
+    "--datasets-dir",
+    type=str,
+    default=None,
+    help="Path to override default datasets dir.",
+)
 def main(**kwargs):
+    if kwargs["datasets_dir"] is not None:
+        settings = get_settings()
+        settings["datasets_dir"] = os.path.abspath(
+            os.path.expanduser(kwargs["datasets_dir"])
+        )
+        yaml_save(USER_CONFIG_DIR / "settings.yaml", settings)
+
     model = SparseYOLO(kwargs["model"])
     model.export(**kwargs)
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/yolov8/train.py

```diff
@@ -8,17 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import logging
+import os
+
 import click
 from sparseml.yolov8.trainers import SparseYOLO
+from ultralytics.yolo.utils import USER_CONFIG_DIR, get_settings, yaml_save
+
 
+logger = logging.getLogger()
 
 # Options generated from
 # https://github.com/ultralytics/ultralytics/blob/main/ultralytics/yolo/configs/default.yaml
 
 
 @click.command(
     context_settings=(
@@ -201,14 +207,27 @@
     "--fliplr", type=float, default=0.5, help="image flip left-right (probability)"
 )
 @click.option("--mosaic", type=float, default=1.0, help="image mosaic (probability)")
 @click.option("--mixup", type=float, default=0.0, help="image mixup (probability)")
 @click.option(
     "--copy-paste", type=float, default=0.0, help="segment copy-paste (probability)"
 )
+@click.option(
+    "--datasets-dir",
+    type=str,
+    default=None,
+    help="Path to override default datasets dir.",
+)
 def main(**kwargs):
+    if kwargs["datasets_dir"] is not None:
+        settings = get_settings()
+        settings["datasets_dir"] = os.path.abspath(
+            os.path.expanduser(kwargs["datasets_dir"])
+        )
+        yaml_save(USER_CONFIG_DIR / "settings.yaml", settings)
+
     model = SparseYOLO(kwargs["model"])
     model.train(**kwargs)
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/yolov8/trainers.py

```diff
@@ -15,28 +15,28 @@
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
 import warnings
 from copy import copy, deepcopy
-from datetime import datetime
+from datetime import datetime, timedelta
 from pathlib import Path
 from typing import List, Optional
 
 import onnx
 import torch
 
 from sparseml.optim.helpers import load_recipe_yaml_str
 from sparseml.pytorch.optim.manager import ScheduledModifierManager
 from sparseml.pytorch.utils import ModuleExporter
 from sparseml.pytorch.utils.helpers import download_framework_model_by_recipe_type
 from sparseml.pytorch.utils.logger import LoggerManager, PythonLogger, WANDBLogger
 from sparseml.yolov8.modules import Bottleneck, Conv
-from sparseml.yolov8.utils import check_coco128_segmentation
+from sparseml.yolov8.utils import check_coco128_segmentation, create_grad_sampler
 from sparseml.yolov8.utils.export_samples import export_sample_inputs_outputs
 from sparseml.yolov8.validators import (
     SparseClassificationValidator,
     SparseDetectionValidator,
     SparseSegmentationValidator,
 )
 from sparsezoo import Model
@@ -318,19 +318,67 @@
             self.scaler = self.manager.modify(
                 self.model.module if hasattr(self.model, "module") else self.model,
                 self.optimizer,
                 steps_per_epoch=self.steps_per_epoch,
                 epoch=self.start_epoch,
                 wrap_optim=self.scaler,
                 loggers=self.logger_manager,
+                grad_sampler={
+                    "data_loader_builder": self._get_data_loader_builder(),
+                    "loss_function": lambda preds, batch: self.criterion(preds, batch)[
+                        0
+                    ]
+                    / self.train_loader.batch_size,
+                },
             )
         else:
             # initialize steps_per_epoch for logging when there's no recipe
             self.steps_per_epoch = len(self.train_loader)
 
+    def _setup_ddp(self, rank, world_size):
+        # increases the timeout for DDP processes
+        torch.cuda.set_device(rank)
+        self.device = torch.device("cuda", rank)
+        LOGGER.info(
+            f"DDP settings: RANK {rank}, WORLD_SIZE {world_size}, DEVICE {self.device}"
+        )
+        torch.distributed.init_process_group(
+            "nccl" if torch.distributed.is_nccl_available() else "gloo",
+            rank=rank,
+            world_size=world_size,
+            timeout=timedelta(seconds=7200),
+        )
+
+    def _get_data_loader_builder(self):
+        train_loader = self.train_loader
+
+        def _data_loader_builder(kwargs):
+            template = dict(train_loader.__dict__)
+            # drop attributes that will be auto-initialized
+            to_drop = [
+                k
+                for k in template
+                if k.startswith("_") or k in ["batch_sampler", "iterator", "sampler"]
+            ]
+            for item in to_drop:
+                template.pop(item)
+
+            # override defaults if kwargs are given, for example via recipe
+            if kwargs:
+                template.update(kwargs)
+            data_loader = type(train_loader)(**template)
+
+            while True:
+                for batch in data_loader:
+                    batch = self.preprocess_batch(batch)
+                    assert batch["img"].device.index == self.device.index
+                    yield [batch["img"]], {}, batch
+
+        return _data_loader_builder
+
     def callback_on_train_epoch_start(self):
         # NOTE: this callback is registered in __init__
 
         model_is_quantized = False
         if self.manager is not None and self.manager.qat_active(epoch=self.epoch):
             model_is_quantized = True
         if self.checkpoint_manager is not None and self.checkpoint_manager.qat_active(
@@ -597,15 +645,35 @@
             LOGGER.info(
                 f"Detected one-shot recipe: {one_shot}. "
                 "Applying it to the model to be exported..."
             )
             for p in self.model.parameters():
                 p.requires_grad = True
             manager = ScheduledModifierManager.from_yaml(one_shot)
-            manager.apply(self.model)
+
+            overrides = self.overrides.copy()
+            # assumes single-GPU or CPU one-shot pathway
+            if kwargs["device"] is not None and "cpu" not in kwargs["device"]:
+                overrides["device"] = "cuda:" + kwargs["device"]
+            overrides["deterministic"] = kwargs["deterministic"]
+            trainer = self.TrainerClass(overrides=overrides)
+            self.model = self.model.to(trainer.device)
+
+            manager.apply(
+                self.model,
+                # maybe we could check whether OBS pruner is in the manager?
+                grad_sampler=create_grad_sampler(trainer, stride=32, model=self.model)
+                if any(
+                    map(
+                        lambda mod: hasattr(mod, "_grad_sampler"),
+                        manager.pruning_modifiers,
+                    )
+                )
+                else None,
+            )
             recipe = (
                 ScheduledModifierManager.compose_staged(recipe, manager)
                 if recipe
                 else manager
             )
 
         name = args.get("name", f"{type(self.model).__name__}.onnx")
@@ -713,19 +781,15 @@
             # use trained imgsz unless custom value is passed
             args.imgsz = self.ckpt["train_args"]["imgsz"]
         args.imgsz = check_imgsz(args.imgsz, max_dim=1)
         if args.task == "segment":
             args = check_coco128_segmentation(args)
 
         validator = self.ValidatorClass(args=args)
-        validator(
-            model=self.model,
-            trainer=self.TrainerClass(overrides=overrides),
-            training=False,
-        )
+        validator(model=self.model)
 
 
 def generate_ddp_command(world_size, trainer):
     # NOTE: copied from ultralytics.yolo.utils.dist.generate_ddp_command
     import __main__  # noqa local import to avoid https://github.com/Lightning-AI/lightning/issues/15218
 
     file_name = os.path.abspath(sys.argv[0])
```

## sparseml/yolov8/val.py

```diff
@@ -8,16 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+
 import click
 from sparseml.yolov8.trainers import SparseYOLO
+from ultralytics.yolo.utils import USER_CONFIG_DIR, get_settings, yaml_save
 
 
 @click.command(
     context_settings=(
         dict(token_normalize_func=lambda x: x.replace("-", "_"), show_default=True)
     )
 )
@@ -64,14 +67,27 @@
     "--max_det", default=300, type=int, help="maximum number of detections per image"
 )
 @click.option("--half", default=False, is_flag=True, help="use half precision (FP16)")
 @click.option(
     "--dnn", default=False, is_flag=True, help="use OpenCV DNN for ONNX inference"
 )
 @click.option("--plots", default=False, is_flag=True, help="show plots during training")
+@click.option(
+    "--datasets-dir",
+    type=str,
+    default=None,
+    help="Path to override default datasets dir.",
+)
 def main(**kwargs):
+    if kwargs["datasets_dir"] is not None:
+        settings = get_settings()
+        settings["datasets_dir"] = os.path.abspath(
+            os.path.expanduser(kwargs["datasets_dir"])
+        )
+        yaml_save(USER_CONFIG_DIR / "settings.yaml", settings)
+
     model = SparseYOLO(kwargs["model"])
     model.val(**kwargs)
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/yolov8/validators.py

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
-from argparse import Namespace
 
 import torch
 from tqdm import tqdm
 
 from ultralytics.nn.autobackend import AutoBackend
 from ultralytics.yolo.data.utils import check_cls_dataset, check_det_dataset
 from ultralytics.yolo.engine.validator import BaseValidator
@@ -27,16 +26,17 @@
 from ultralytics.yolo.utils.torch_utils import de_parallel, select_device
 from ultralytics.yolo.v8.classify.val import ClassificationValidator
 from ultralytics.yolo.v8.detect.val import DetectionValidator
 from ultralytics.yolo.v8.segment.val import SegmentationValidator
 
 
 class SparseValidator(BaseValidator):
-    def __call__(self, trainer=None, model=None, training=True):
-        self.training = trainer is not None and training
+    def __call__(self, trainer=None, model=None):
+        # the **only** difference in this call is that we pass fuse=False to AutoBackend
+        self.training = trainer is not None
         if self.training:
             self.device = trainer.device
             self.data = trainer.data
             if trainer.manager and trainer.manager.quantization_modifiers:
                 # Since we disable the EMA model for QAT, we validate the non-averaged
                 # QAT model
                 model = de_parallel(trainer.model)
@@ -97,16 +97,14 @@
                 self.data.get("val") or self.data.set("test"), self.args.batch
             )
 
             model.eval()
             model.warmup(
                 imgsz=(1 if pt else self.args.batch, 3, imgsz, imgsz)
             )  # warmup
-            trainer.model = model.model
-            trainer.model.args = Namespace(**model.model.args)
 
         dt = Profile(), Profile(), Profile(), Profile()
         n_batches = len(self.dataloader)
         desc = self.get_desc()
         # NOTE: keeping `not self.training` in tqdm will eliminate pbar after
         # segmentation evaluation during training,
         # which may affect classification task since this arg
@@ -125,22 +123,16 @@
 
             # inference
             with dt[1]:
                 preds = model(batch["img"])
 
             # loss
             with dt[2]:
-                if not hasattr(self, "loss"):
-                    self.loss = trainer.criterion(
-                        preds if self.training else preds[1], batch
-                    )[1]
-                else:
-                    self.loss += trainer.criterion(
-                        preds if self.training else preds[1], batch
-                    )[1]
+                if self.training:
+                    self.loss += trainer.criterion(preds, batch)[1]
 
             # pre-process predictions
             with dt[3]:
                 preds = self.postprocess(preds)
 
             # During QAT the resulting preds are grad required, breaking
             # the update metrics function.
@@ -155,34 +147,33 @@
         stats = self.get_stats()
         self.check_stats(stats)
         self.print_results()
         self.speed = tuple(
             x.t / len(self.dataloader.dataset) * 1e3 for x in dt
         )  # speeds per image
         self.run_callbacks("on_val_end")
-        model.float()
-        stats = {
-            **stats,
-            **trainer.label_loss_items(
-                self.loss.cpu() / len(self.dataloader), prefix="val"
-            ),
-        }
         if self.training:
+            model.float()
+            results = {
+                **stats,
+                **trainer.label_loss_items(
+                    self.loss.cpu() / len(self.dataloader), prefix="val"
+                ),
+            }
             return {
-                k: round(float(v), 5) for k, v in stats.items()
+                k: round(float(v), 5) for k, v in results.items()
             }  # return results as 5 decimal place floats
         else:
             self.logger.info(
                 (
                     "Speed: %.1fms pre-process, %.1fms inference, %.1fms loss, %.1fms "
                     "post-process per image"
                 ),
                 *self.speed,
             )
-            self.logger.info(f"Validation loss: {stats['val/Loss']}")
             if self.args.save_json and self.jdict:
                 with open(str(self.save_dir / "predictions.json"), "w") as f:
                     self.logger.info(f"Saving {f.name}...")
                     json.dump(self.jdict, f)  # flatten and save
                 stats = self.eval_json(stats)  # update stats
             return stats
```

## sparseml/yolov8/utils/helpers.py

```diff
@@ -11,17 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import warnings
 from argparse import Namespace
+from typing import Any, Dict
 
+from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
+from ultralytics.yolo.engine.model import DetectionModel
+from ultralytics.yolo.engine.trainer import BaseTrainer
 
-__all__ = ["check_coco128_segmentation"]
+
+__all__ = ["check_coco128_segmentation", "create_grad_sampler"]
 
 
 def check_coco128_segmentation(args: Namespace) -> Namespace:
     """
     Checks if the argument 'data' is coco128.yaml and if so,
     replaces it with coco128-seg.yaml.
     :param args: arguments to check
@@ -32,7 +37,35 @@
         dataset_yaml = dataset_name + "-seg" + dataset_extension
         warnings.warn(
             f"Dataset yaml {args.data} is not supported for segmentation. "
             f"Attempting to use {dataset_yaml} instead."
         )
         args.data = dataset_yaml
     return args
+
+
+def create_grad_sampler(
+    trainer: BaseTrainer, stride: int, model: DetectionModel
+) -> Dict[str, Any]:
+    if not hasattr(trainer, "train_loader"):
+        # initialize train loader (if not already initialized)
+        # and set it as the trainer's attribute
+        train_set_path = trainer.trainset
+        train_loader, _ = create_dataloader(
+            path=train_set_path,
+            imgsz=trainer.args.imgsz,
+            batch_size=trainer.args.batch,
+            stride=stride,
+        )
+        trainer.train_loader = train_loader
+
+    # convert model's arg to a namespace,
+    # this is expected by the trainer's criterion
+    model.args = Namespace(**model.args)
+    trainer.model = model
+
+    grad_sampler = dict(
+        data_loader_builder=trainer._get_data_loader_builder(),
+        loss_function=lambda preds, batch: trainer.criterion(preds, batch)[0]
+        / train_loader.batch_size,
+    )
+    return grad_sampler
```

## Comparing `sparseml_nightly-1.5.0.20230404.dist-info/LICENSE` & `sparseml_nightly-1.5.0.20230412.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230404.dist-info/METADATA` & `sparseml_nightly-1.5.0.20230412.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.5.0.20230404
+Version: 1.5.0.20230412
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -304,15 +304,15 @@
 
 ### Contribute
 
 We appreciate contributions to the code, examples, integrations, and documentation as well as bug reports and feature requests! [Learn how here.](https://github.com/neuralmagic/sparseml/blob/main/CONTRIBUTING.md)
 
 ### Join
 
-For user help or questions about SparseML, sign up or log in to our [**Deep Sparse Community Slack**](https://join.slack.com/t/discuss-neuralmagic/shared_invite/zt-q1a1cnvo-YBoICSIw3L1dmQpjBeDurQ). We are growing the community member by member and happy to see you there. Bugs, feature requests, or additional questions can also be posted to our [GitHub Issue Queue.](https://github.com/neuralmagic/sparseml/issues)
+For user help or questions about SparseML, sign up or log in to our [**Neural Magic Community Slack**](https://join.slack.com/t/discuss-neuralmagic/shared_invite/zt-q1a1cnvo-YBoICSIw3L1dmQpjBeDurQ). We are growing the community member by member and happy to see you there. Bugs, feature requests, or additional questions can also be posted to our [GitHub Issue Queue.](https://github.com/neuralmagic/sparseml/issues)
 
 You can get the latest news, webinar and event invites, research papers, and other ML Performance tidbits by [subscribing](https://neuralmagic.com/subscribe/) to the Neural Magic community.
 
 For more general questions about Neural Magic, please fill out this [form.](http://neuralmagic.com/contact/)
 
 ### Cite
```

## Comparing `sparseml_nightly-1.5.0.20230404.dist-info/NOTICE` & `sparseml_nightly-1.5.0.20230412.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230404.dist-info/entry_points.txt` & `sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230404.dist-info/RECORD` & `sparseml_nightly-1.5.0.20230412.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-sparseml/__init__.py,sha256=hCndjAou3jTbrICVhtfvj6DM-8Gq8ko_mu8GMvlHZCQ,1780
+sparseml/__init__.py,sha256=nxuiUykjTFTYiw28TB9H75wWbdzr6Y0j-2h4dabdp54,1413
 sparseml/analytics.py,sha256=WhXdKgK1-ll9sRzn2n8z-FAikQ02J8rUeWmceiX5S7E,898
 sparseml/base.py,sha256=oOPiaU2JhI0beFwp8Obe7hbt3kUuNvI5XD1wTBCtLnc,10284
 sparseml/log.py,sha256=K5E3goPRIPY7Uc14JcX-4oLXVWu7ecOPf1NYBGHc1r0,2483
 sparseml/version.py,sha256=jmrGrUNSNjL1K4iFHcD1xXttUBhm20Y6rTeTfP-tEvM,1511
 sparseml/benchmark/__init__.py,sha256=WynUhMzXq3-iQAhPwcmcMOj2_xCa9brLubs7gxq9T3U,758
 sparseml/benchmark/info.py,sha256=yRA5QgKQNKjOZhQH9uNvVuWlqL4eXDVikA8pL5Mzha4,17631
 sparseml/benchmark/serialization.py,sha256=FPpcC93x5H86Fqil9YbERUpltu7qhhIQjsyYaSlW_20,10778
@@ -42,15 +42,15 @@
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=lUutqioFTP3ZVa5IIA-Z5WbriNj_8m2mXut_QOyo_J0,8704
 sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
 sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
 sparseml/framework/__init__.py,sha256=EcIX435yx552d7BkbxmAbQ_X3KAISInHVbD9X-AT1Uk,790
 sparseml/framework/info.py,sha256=TaZAMYdhBHcjl9Xyk3PWjJkDB6g3_f4vD3B6KmhgOl8,9479
-sparseml/keras/__init__.py,sha256=tqyou1pWJWROK8_0HAtQozvlIERKUn6mhvfGy74K9rg,961
+sparseml/keras/__init__.py,sha256=G-uSbckWq3vn9YUFr5pD0xbaO694SFgIlc5AVQMDafU,970
 sparseml/keras/base.py,sha256=yt1EO6KIeCkdg8rF37U5Y3FNGeAqOQLVGyxRANsyBy0,8054
 sparseml/keras/datasets/__init__.py,sha256=USLH-kFbXiubqgMW8IMkZfycVByQAOdAtzuPHzTok9I,943
 sparseml/keras/datasets/dataset.py,sha256=W6wdx4WXtyy4r1JVbc8fO0Xt5SM03zm8Vq306uNFkaw,3297
 sparseml/keras/datasets/helpers.py,sha256=PfDBKDMr3A8XG9wP0QRABu4h63eHZT15gDuO8naIXxY,2423
 sparseml/keras/datasets/registry.py,sha256=41aieOOADwl0V1n127OA6zyxhCwLwHy4jo7SkyzSUwo,2761
 sparseml/keras/datasets/classification/__init__.py,sha256=YGWvyTK6h32vDtAD3Vcr3bsNqGvfFXOiQy9wydvzEDc,786
 sparseml/keras/datasets/classification/imagefolder.py,sha256=Ay5xsUH4zR2xgTg6HM7qXiOMs02PMMg3-_pD0tgzzgE,8369
@@ -78,15 +78,15 @@
 sparseml/keras/sparsification/info.py,sha256=HVIGhKG2HHOaYxgvltQ7hjOQXbqbvT2DO3F4gBP1lbc,1356
 sparseml/keras/utils/__init__.py,sha256=JkMJHbL8sCUKcDOfOGNpqexmdsnq6vdQpNUQCbVMNY8,962
 sparseml/keras/utils/callbacks.py,sha256=WqycV-Wq2YEQ1uYuTmqEW-C_5Aeowt_DTB8C4oruOSk,8202
 sparseml/keras/utils/compat.py,sha256=oPMoTw2NKedJTk2PhA_75YBM6Nwxg_Yx0MyUdcgbisw,1022
 sparseml/keras/utils/exporter.py,sha256=mC-and9qFuOT5qVHRR3iBTvvwRpUUz_C8oR1WK078lM,5737
 sparseml/keras/utils/logger.py,sha256=xsOmL5qUHvWwFhGIRlNuQLAO8DMpx_-fxvr5N3QrQt8,6087
 sparseml/keras/utils/model.py,sha256=Or2Vijn7JPrE4QMTwBYX8zgmoucYRQK8y1VVDL9vJ1Q,1738
-sparseml/onnx/__init__.py,sha256=qiIZlO7tYYUnk2XS9jSxoGmXx4HPsApuwzlPK7in6RE,1027
+sparseml/onnx/__init__.py,sha256=KeWF6EQ7cpX_b-fMhiG5n6pVPUvRxiWMpzpiI9EagFI,1036
 sparseml/onnx/base.py,sha256=Kv3YC0Xh1xlxpIuwh9916SHuz96phaf36KbL71DSZWk,6202
 sparseml/onnx/benchmark/__init__.py,sha256=tl8cy1ta02lUmMxwmDfRAYcVQfaj5OpU3igqYJHMGg8,743
 sparseml/onnx/benchmark/info.py,sha256=iCNry2VAuSmTLrPl3a8pxDU_R-U9-Lpcka40QIg5BZg,15366
 sparseml/onnx/framework/__init__.py,sha256=HpgplVizgXIPOmnE24RM1geQLp924227_T12jJjQCaA,823
 sparseml/onnx/framework/info.py,sha256=YzZmDaR6Z1y66xo_OKtmQGA1ZVFOozZNXBJ_Ec74ueU,6116
 sparseml/onnx/optim/__init__.py,sha256=EZeHGH5zDRfb0MrXqh4_3ci0ViBS2WWb8NqhAi8nd3A,820
 sparseml/onnx/optim/analyzer_model.py,sha256=NLxYEH9QaU-xl2h1SagMHyfQ3skEsuYRFTqeYpKTgIM,13274
@@ -104,15 +104,15 @@
 sparseml/onnx/utils/data.py,sha256=6Rw3hkSG1DZ057USkzioSDFcYH92ZLwdHYlQY2PdkwQ,13002
 sparseml/onnx/utils/graph_editor.py,sha256=IBNbKWjOLy7oW-bjsxBkSw5HULHIoeVFQFs2ccYVTs0,16407
 sparseml/onnx/utils/graph_optimizer.py,sha256=AfS2zdxW1tJ6xYAe-2n3KdAdDenxiqslOFUIVAzD-cY,8133
 sparseml/onnx/utils/helpers.py,sha256=NQmCHhRqb3qjs1cjK-LjorgfhEC7yroPvW_f1ajBZJE,41311
 sparseml/onnx/utils/loss.py,sha256=2njnY0qY2n6DS9HHB0kqLz7N8wgPaDTkAi6Z2DLYPLc,1958
 sparseml/onnx/utils/model.py,sha256=ElcSfKhUnqvjpYusg4iD-pL-y77T14mvECDBPPGnNnQ,31586
 sparseml/onnx/utils/sparse_tensor.py,sha256=6Bu9fVJqLCtve3qpg9ScYGqcv4X7ZcRKhVrp8pCLBRI,5437
-sparseml/openpifpaf/__init__.py,sha256=6JkwRvCuYDQwEELDMT7HC1K1-IpBvhwTqfr6CpwWukU,725
+sparseml/openpifpaf/__init__.py,sha256=cRAMNGqBJbWxG6ds0WRxQnTnvtm_DJqaSBwEt0HupT0,734
 sparseml/openpifpaf/export.py,sha256=YkX06A384K17AfKYli1RcYHcoVg4gF79ttZ-73H_6rI,3694
 sparseml/openpifpaf/train.py,sha256=vl5ioCcnzep9XNVMOsveO9QRRrXSn8VDnEM1LGv71Ew,10950
 sparseml/openpifpaf/trainer.py,sha256=Du9W5fW9ImC3XlOVVWesbcBv1SjJOfP_D94_hBUR6VY,4211
 sparseml/optim/__init__.py,sha256=3oGQ4LY0MSrbTAwuyPHEOEyYiZ7JI7OX2BgWup5NPuw,882
 sparseml/optim/analyzer.py,sha256=LUYBYyvfVwaw_V1aAiOmaybUGJQk4vRK5RG3k3nD7pA,6302
 sparseml/optim/helpers.py,sha256=Zb7YPYe07vuVyYUhHJ-BlcMrZa-sxt1TUZ-Ec9Z6o_U,25563
 sparseml/optim/manager.py,sha256=KeDVHj9ea9EUaV908qfvq8ONwS8nUmAvQb1yXflOBWo,25984
@@ -137,15 +137,15 @@
 sparseml/pytorch/datasets/detection/voc.py,sha256=ntif1itgg0o4GRkZHHexBHIm_E9NaJh5opdPSG5jMeQ,10759
 sparseml/pytorch/datasets/image_classification/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py,sha256=yMUOho19OugY5yaH5oXOho41_uYYjkwmvfhzdAA1u4w,9512
 sparseml/pytorch/datasets/recommendation/__init__.py,sha256=Ngvu1hKPBJs8KQ-3f_FnGrp4Zw49VGrTg-3uQbYhIXo,684
 sparseml/pytorch/datasets/video/__init__.py,sha256=FCWCuDjr7Vs7u1UYDOfe0AJvJlGoskWv6Rx0kyc0i9M,693
 sparseml/pytorch/framework/__init__.py,sha256=9PE8aAdkuM75YAo4CKmDJZf49VcZu3d0g9ywcxQUiGE,814
 sparseml/pytorch/framework/info.py,sha256=bD9mZK163Ozqetr14_bwlzn4VJJ5RSUbfiP7V9sEy8o,5580
-sparseml/pytorch/image_classification/__init__.py,sha256=512len4zJ0Osw5Cx95Hqh57-wjr56zIEdVSBYAzzDfk,750
+sparseml/pytorch/image_classification/__init__.py,sha256=tXi9ZUe6trd4y1XOeQYuOPPzFVlr_wjvhwc_dIwPc4o,753
 sparseml/pytorch/image_classification/export.py,sha256=FG3TIe06X5PYlubyGmDjNKWBZHsX24wQ19gbqXMT3BQ,18265
 sparseml/pytorch/image_classification/lr_analysis.py,sha256=qweXU51KeWjW86RJknvsavKPPXMd3PGAO7bcGosjTqE,15494
 sparseml/pytorch/image_classification/pr_sensitivity.py,sha256=RA64lC4NOmFm2H11MO4HSuiw2ImtiRwvixtIw7Rol0o,14444
 sparseml/pytorch/image_classification/train.py,sha256=-My1yUclgRA5wQoV4B_jtoOMRO1nQj389WfDkebu3fs,29287
 sparseml/pytorch/image_classification/utils/__init__.py,sha256=ambjlzpSCaSZ7ZadPk2vMAB6kaZCm7f_hVqOVSWz8k8,682
 sparseml/pytorch/image_classification/utils/cli_helpers.py,sha256=qypcmjezy-fZn2Cjozv9vumZoB44_9PDe_WXnChbvLg,4278
 sparseml/pytorch/image_classification/utils/constants.py,sha256=k01fijyL2BicSWLL1EzhhdvG07WYMMXHZeFz-9fxecM,1257
@@ -156,15 +156,15 @@
 sparseml/pytorch/models/classification/__init__.py,sha256=opnCtf6WMl1kuQ_vRAZRLl1eFZefpG9GFc9o729HndQ,901
 sparseml/pytorch/models/classification/darknet.py,sha256=rR4XXQu7shLADU4Th0D-eodnv-Z3AmA6kj8tDgHmtxU,11658
 sparseml/pytorch/models/classification/efficientnet.py,sha256=Bs88xu2xX9P65TOZ_6rn_qO2CMa6oLsJm5xt-Y6gISI,40293
 sparseml/pytorch/models/classification/inception_v3.py,sha256=wxWU3ja6E0_ERhYniDlzcsnVWi-rvJVfgxmhsyrpuC4,16512
 sparseml/pytorch/models/classification/mnist.py,sha256=RyFLHgKzmbmSvI-7F4nkbUI7xkz5pKElT7ve1ZIn7VU,4164
 sparseml/pytorch/models/classification/mobilenet.py,sha256=0ffCRqolRchhz4YoDH--tyDzLuQ1vyVbXL5LpAkXuIM,9546
 sparseml/pytorch/models/classification/mobilenet_v2.py,sha256=e6SqGzdIuOEzwp_sbvEAXSwrv5eHPpYz-lgHACqrSXs,13014
-sparseml/pytorch/models/classification/resnet.py,sha256=gQzFigjFUWNfUSp6oQWrvKF0ak0HlFpsE5YuupX-HYc,40931
+sparseml/pytorch/models/classification/resnet.py,sha256=wvdwz-53nFlyFWCHGAm2w4KIlV5TQ2C86BmiNUZR528,40800
 sparseml/pytorch/models/classification/vgg.py,sha256=_7Dyaj58dSzvi7KcooOYlUEg8kJGkQsDLhxpIWFhnS0,16649
 sparseml/pytorch/models/detection/__init__.py,sha256=NIlqCw6brqzhSlo6SyGz3eHmj3W1njG0qyvR4n5E3ZM,824
 sparseml/pytorch/models/detection/ssd.py,sha256=38w-HWL9SiM3KvVN1KyPfpJVq-U1i-wx4zZeucxKvss,6820
 sparseml/pytorch/models/detection/ssd_lite.py,sha256=UoXcZlEsOxw_1chviAluKKYEJZajflYvuvLF5lsfsCM,8116
 sparseml/pytorch/models/detection/ssd_mobilenet.py,sha256=fDmIPuCnDh8jvNTV3F7TUZZSc3hugxO7wGFJxrIeF1o,4046
 sparseml/pytorch/models/detection/ssd_resnet.py,sha256=Im4m61GZfDdgwtemTqzVK1hduoCOSf8c_Fnif1zvGZQ,9069
 sparseml/pytorch/models/detection/yolo_v3.py,sha256=18iwLZYstNkHu0JVi3Q9u62_e1zVly0KqmdgrtfLSN4,10188
@@ -176,15 +176,15 @@
 sparseml/pytorch/nn/fatrelu.py,sha256=twbvUqaJsKkjplrUJaVm4mfq-OC63eN-IboG70nhZO8,11854
 sparseml/pytorch/nn/identity.py,sha256=vCs9du3P0fQS6clFFNCacHE-J_OGZiKcvsEz-iHZy4s,1690
 sparseml/pytorch/nn/se.py,sha256=kR9agk8OKTEq_iPRLX8NHlbFUJlZEVFt7Otgtk5LoXQ,2828
 sparseml/pytorch/optim/__init__.py,sha256=pV-8sO8TP23X6gS81BvCfEC9LCnRYws3ek-pylOnaHg,1243
 sparseml/pytorch/optim/analyzer_as.py,sha256=6WCMuxF-8rcFYNTNiNoQMNloISfJBrk_9bYbSiMK1-8,13638
 sparseml/pytorch/optim/analyzer_module.py,sha256=u8E3l-hvIhicNqsGcY4WTrT1hZBtPsIN2unqix8RAhI,17069
 sparseml/pytorch/optim/analyzer_pruning.py,sha256=V-VWmMgTU1nHgcLlVmyl3aNo4yeeG0HGleAfTkhNiyI,3955
-sparseml/pytorch/optim/manager.py,sha256=ehtn9VJ-bADDxOsSylLV598L6bx8BFXA-JhmQAGLNKw,26830
+sparseml/pytorch/optim/manager.py,sha256=abFJNGYSBohaZAq65ZVojG7dl45QuXALmhkJanIVyWg,26838
 sparseml/pytorch/optim/mask_creator_pruning.py,sha256=k0gHVM8fThZqLOBfdfte1l7zoylvDRpaAxfcM32eioc,36844
 sparseml/pytorch/optim/mask_pruning.py,sha256=QqBrPfskL0vJlFOsxrqZp0sCk8NQUf4srj5WNuWHyJY,23085
 sparseml/pytorch/optim/mask_pruning_scorer.py,sha256=IKiIegTFtez2taiWwDwaxJOMvEd8---GQ28CeZD24gI,10449
 sparseml/pytorch/optim/optimizer.py,sha256=f20_TaCsvNRybm0qqG1BqXu1KOQpDeQkIOZWiMvftJc,6605
 sparseml/pytorch/optim/sensitivity_as.py,sha256=9QJiRvMkFXCFCCQYuA77BwJgJRoHDtuQ4fxx3T3cwtY,14879
 sparseml/pytorch/optim/sensitivity_lr.py,sha256=j78fmJBoAhK-NKM8mVLdc78Hh8-6Jzyplba-UJp_Yfg,6101
 sparseml/pytorch/optim/sensitivity_pruning.py,sha256=9cxUlgVW2JFL69rVe2UYX6ID8m9_-d-x4_J6iSN-W1Y,9324
@@ -207,15 +207,15 @@
 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py,sha256=jRMApqylXjFHW31nZY_iMveu265uqQqIqNHrXGzmmyU,10455
 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py,sha256=HsLi7Mdu9Lty5A9w4nY9sTe9NgzDxgJRoM-LzFkl6Ao,33219
 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py,sha256=D3zx4rL5ccwi9kFGsIo1OoPW9zl--ditOu7JKb-9hGs,5757
 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py,sha256=giv8z84R0-nQ7MRfW6MrqBd0C19GFnFTUNjJz_5HlRo,8860
 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py,sha256=5W-H7scPflGySPoeLZaFwyvihbqsYcZP6xwMWsQ75WQ,15595
 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py,sha256=GFJy-obm0cvr2c1vNgCWaUXAhFplvHDxUfmun98rWmY,63519
 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py,sha256=gmRbalMpVEJ-U5xdL5Vh-XcTOhkfr8z_cWlKw_m1c9k,8774
-sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py,sha256=RMCrM66pkjPXo2vufCkJAsayd_nK4rFYbG8zpTbm36Y,24133
+sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py,sha256=bKZojNIl4aWvU0xXxfAvTZztFcS2Q5QCljt43icIux0,24121
 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py,sha256=h7ASPoik7zrBXE_lbdfBO3UkbrTeXG5gGE1Flg75h8s,18245
 sparseml/pytorch/sparsification/pruning/scorer.py,sha256=8gyYSv611GOJwmpQeD7FsWVrLxF8jeM_f59zhQlC6f8,4644
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=VQnQZozal38sffuIZjL1vKs6LeDhmiy-BvKebzewYO4,26253
@@ -224,15 +224,15 @@
 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=LxqptXTzW2PhIN2FuaRVHmo2gtZMOGoLzsel7jUNPh0,69783
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
-sparseml/pytorch/torchvision/__init__.py,sha256=oI1MLZUh5r9h2YF86p_gZfOBnOVPpkdbpGvrncgOt4g,741
+sparseml/pytorch/torchvision/__init__.py,sha256=qPAYUqRxLOdwP3JCQ79MF1N1rXaULmNQLWpqH5osPzY,744
 sparseml/pytorch/torchvision/export_onnx.py,sha256=oiittOzvPEWMBpyldcfX6Yr7GQjKiKkOH4IUX-QQ718,6490
 sparseml/pytorch/torchvision/presets.py,sha256=PMRKjg4sBm6_UdhAV29wSSeOdDR6QlCzjcJbQWSenUA,2870
 sparseml/pytorch/torchvision/sampler.py,sha256=VuebeOVoQWLsafwJEeGgKQrDfF8PxzimHWFLs9odGz8,2530
 sparseml/pytorch/torchvision/train.py,sha256=YwETS0-EgjpGvs9LzKRCbGkcSHh35Mv-iOBJPGatnnM,40790
 sparseml/pytorch/torchvision/transforms.py,sha256=_WfLKV2G9ZLt2zdpKvaHA1ricPGufVIF-lzgKaOL2Ec,7128
 sparseml/pytorch/torchvision/utils.py,sha256=weRmF78Qf9_Kgd-L7aAHERmXKoCVqUP4J8pbSZmav58,16675
 sparseml/pytorch/utils/__init__.py,sha256=WWPrEPVj8YsCZN0JemnAF5z7hOf0nL203uixlqWoAeo,1160
@@ -242,15 +242,15 @@
 sparseml/pytorch/utils/exporter.py,sha256=KfoPciN46ZDHKgvVk7oYBR_cyZwihRPNcCm-EvPnpfg,31056
 sparseml/pytorch/utils/helpers.py,sha256=QF4TobigcGoFG6kCKw7U8BneHESMQu7yNJhxQGAXS5M,38949
 sparseml/pytorch/utils/log_sparsification_info.py,sha256=o9WdrrDU8W1J09NHLnW2cja5PXNq442UFzgpXf8po8M,1663
 sparseml/pytorch/utils/logger.py,sha256=KOhmFXNj46gmy5XovwQOZigBuHidVmNqDnVWMUXD7PE,31374
 sparseml/pytorch/utils/loss.py,sha256=RWFyThMBaB-7jAVuS3_CU5bmsWOVFG1jqzPciSpVsj8,27048
 sparseml/pytorch/utils/model.py,sha256=KCEZ6cNkIzLKd6N8KqJe7GX3GD-PoWErZk05nEbQuJc,11754
 sparseml/pytorch/utils/module.py,sha256=gWKNLqn8bI_q97u_QC95WkxBPAclMCwz3HmrZEHEYtU,39117
-sparseml/pytorch/utils/sparsification.py,sha256=tNsC2E9YAVplcjaqDKyLQOTy3xtyZkY8VGK9dt8IJYQ,8382
+sparseml/pytorch/utils/sparsification.py,sha256=BbH3ePC74YWGddSoLcSenLd0D_0nz-Xk5vx4Ui_KkzY,8809
 sparseml/pytorch/utils/ssd_helpers.py,sha256=05fySE5KNwrt7UF213niHp2STRSeprlU1NbLAjpYRaU,30059
 sparseml/pytorch/utils/yolo_helpers.py,sha256=nFlDPOEWfooq8GrUzKRpr7vS36m9NQMPGZSqCYmGMks,12337
 sparseml/pytorch/utils/sparsification_info/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/pytorch/utils/sparsification_info/configs.py,sha256=lq2RuJWYwrWbtnT2n4eNHtiLcstKyW9YaVhdTms6kqw,10457
 sparseml/pytorch/utils/sparsification_info/helpers.py,sha256=V9sT7dcuAUirBY7wieuwEFL2ENsEv7WdYpQ9lUyoKPg,4309
 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py,sha256=pdP4gEyKmvV7oZBmkBnJkoR3XOKDouVyupOXWHhWYbU,2946
 sparseml/recipe_template/__init__.py,sha256=0HHlF01-zO71wTzxQ9AE8UvqmXbgoyEEykAVGcyVjWA,655
@@ -263,15 +263,15 @@
 sparseml/sparsification/modifier_lr.py,sha256=-3t0ozub6vfyh9NAgvgRgbyXIP1yu9_URuArr5TdTXg,10117
 sparseml/sparsification/modifier_params.py,sha256=n6O1tD4nsOTeeGJ5ym4hB7PQwSEWNduymW8_ObjAO7g,5505
 sparseml/sparsification/modifier_pruning.py,sha256=7_i4dzdkfOFcD7A_d8cublgX5KB-hyOGOJZtU41JUwU,12845
 sparseml/sparsification/oracle.py,sha256=9J8iIdr_aztwc06tRgw-2ZdGN_1RgJBYWZDY1ZfHhAY,3700
 sparseml/sparsification/recipe_builder.py,sha256=i8cFAkDemk8UXiPff5s9necHXECk6WO2AySnqiqr8MU,18570
 sparseml/sparsification/recipe_editor.py,sha256=6PqExzex1nmMj2a0jkE7JUeeuMTGA27GCH32C9B8V40,14413
 sparseml/sparsification/types.py,sha256=wi05A10SkgSBFmBUtzdHIIMTsY4lPTXP0ycZrBgbub0,1250
-sparseml/tensorflow_v1/__init__.py,sha256=uD-tmULKxyXCjWKmwL8NdBwK-Ym5hpbQhj-SAdG6Lf0,985
+sparseml/tensorflow_v1/__init__.py,sha256=JfUGMyYgBnal1xMpGR_i0oA4juUVt2QvkbcBZxFZG6w,987
 sparseml/tensorflow_v1/base.py,sha256=PHZOsjEtcG3gEGRdU7tu2jNRAYYo8KrCmPenZyo5IQo,7272
 sparseml/tensorflow_v1/datasets/__init__.py,sha256=X0o7cmzhXhLwjrawfN3pIqrFTKALH_xftMIerzWaLjQ,925
 sparseml/tensorflow_v1/datasets/dataset.py,sha256=t4OfviMyfbn63kNrNiH19blDvoxcxhyBiLgUh03Ryhc,8121
 sparseml/tensorflow_v1/datasets/helpers.py,sha256=mGy1YuQqERWRG-dknPmOspyWtzUinY9GUSEdSPycGF8,5600
 sparseml/tensorflow_v1/datasets/registry.py,sha256=2H2fG0iUQ0h41XVpZp-GHXM3Ti6axePI1O2LQKqSqhI,2768
 sparseml/tensorflow_v1/datasets/classification/__init__.py,sha256=xNLlq5y7_cssxlZZP95CuYioqEiU6TanVbzMCqoCVTo,807
 sparseml/tensorflow_v1/datasets/classification/cifar.py,sha256=_ETXHcC9cPtQbQIoBLgQQd2GC0Ue6kEO3XXpaZY54xg,12686
@@ -308,15 +308,15 @@
 sparseml/tensorflow_v1/utils/__init__.py,sha256=FhgTPE_G6lftVrwrOCUghTMxmi_1TbRwOX3TYJt5X7A,967
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
-sparseml/transformers/__init__.py,sha256=U8CKn1iGGult1Pc3x-lXSlO3FekIn8PoYU5mbz7tOBM,4388
+sparseml/transformers/__init__.py,sha256=qOQrnlpoWXtpOyp7LEC5d1Xg607wvF3sU6QVfy-_Mwg,4390
 sparseml/transformers/export.py,sha256=JR5cWm0u9pZsn5EiXpJkEZrIHuVLtzSB0js84GsoGn8,19721
 sparseml/transformers/masked_language_modeling.py,sha256=3NVCBveaLUI-BNgTqX5Pm97-apHNFVbyNUDr5z5x1cI,30936
 sparseml/transformers/question_answering.py,sha256=koobYWD4GBcGqWkW1L005QCw4huh5rbFa8rJp_wnWko,36738
 sparseml/transformers/text_classification.py,sha256=9uVAi6vGSl7rF5DHPS005lW0dxOpz2N4ZIXk5-50u8c,40358
 sparseml/transformers/token_classification.py,sha256=6BMBgmEpQvq_RoZzWhLdexQqK4oK9Iv69Qs0IOd-Qds,34464
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
@@ -338,31 +338,31 @@
 sparseml/utils/datasets/coco.py,sha256=5w9Fm0O2kUtrC1upa6DCC4WZ13df-ZlORPUHEwGFDLc,3750
 sparseml/utils/datasets/helpers.py,sha256=1i1jiOoj1q-_Nef5dJBWHoO9v7ZjogggihDjBMNbf_A,1217
 sparseml/utils/datasets/imagenet.py,sha256=qAL7K6tmlfwBY7FI14wcVb-7g3Rzs4wtZIOV1kvoV0w,23366
 sparseml/utils/datasets/imagenette.py,sha256=AIxAI0wfUqu08XPJ1cG8SNUVocjoeFHVepQZDfsztFI,8967
 sparseml/utils/datasets/voc.py,sha256=CzSEnTe-KqWyOLwleame66PtYqF8vuq9EXaNgmms6u0,1009
 sparseml/yolact/COCO.sh,sha256=Q_1I3VZwS4N1e3AwOoimQH2plK2K0athUDWooWR4ZVQ,1875
 sparseml/yolact/COCO_test.sh,sha256=ZoA_h_68zM8EWF510o24_5xBaQtbJLMHenNjSzldYYc,1418
-sparseml/yolact/__init__.py,sha256=XwT-ieD-FPswMv0L1kJJSw4X6ju77J8BSnSXFQr3K44,4018
+sparseml/yolact/__init__.py,sha256=5t9V0aePHnzJBik6z1r4W_3DsSn0lKpYjl3pIuZQft0,4020
 sparseml/yolact/scripts.py,sha256=7GE3xp_B8JJpa2H-Vum6rmiOJHcChyffuno4-yteUUw,1784
-sparseml/yolov5/__init__.py,sha256=JxPj3VB1t3fDcPWhKs-5pYkHoa3UjRF90RXDZ5amec0,3264
+sparseml/yolov5/__init__.py,sha256=k7-HHtzMl2zdGuWrov6hIweSoohqUc_Wi_yKzV89QtQ,3266
 sparseml/yolov5/helpers.py,sha256=jxzJrgKjsb0PHTeGevKICaL8iBOUzxwZXvPAyGyVE-c,4505
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
-sparseml/yolov8/__init__.py,sha256=tHwSC_TcCzW3ZtILLVD8hozIA1qD8c-oItOTNsFi0nE,956
-sparseml/yolov8/default.yaml,sha256=i2dLrqEPkDxJn-7f4KwibqE6RcIRbj16R3P2bIgf1fk,5762
-sparseml/yolov8/export.py,sha256=yEvg4UlV8j8LhFUTGzjC2UScdE7ZDx6cYEmFzIZns8A,2121
+sparseml/yolov8/__init__.py,sha256=4akRvqiJRrRI9kcdXG3rqIiZLWIh7tvA-0zOI2zxO0w,958
+sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
+sparseml/yolov8/export.py,sha256=e6BT4CsAgtm-RIn3eyCsMqxVvRp9XuY71pS12vVMOLc,2845
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
-sparseml/yolov8/train.py,sha256=ZCOFx0oTByrH2b_HtJkymNh0P0a7qT1jxjO79T64Ink,6806
-sparseml/yolov8/trainers.py,sha256=3V4UlTywW5xFACpSXBn4QwCu7fVQaOPlRSF1-YRWNYo,30600
-sparseml/yolov8/val.py,sha256=WLOO9f0mcROGJkCJr22KP9Rsy_KOWBqMhKoYwQvtkEI,2243
-sparseml/yolov8/validators.py,sha256=afpKGHK3ymZ7LkOWM26SEPjPzJVb-kBB1B8HBOakVys,8032
+sparseml/yolov8/train.py,sha256=UKUkpTGaUZ76wRz8w0Rsgi3o9XvsTxdcJ5nmXKOvtkA,7318
+sparseml/yolov8/trainers.py,sha256=s7vfeAyyAVRfaZTgOf9BVd44pOIfnUcjAeHX3w0RwEw,33189
+sparseml/yolov8/val.py,sha256=E1mzjay7F1ErOoqTptBmj9JR310pRu5PI3jp1YVDpH0,2710
+sparseml/yolov8/validators.py,sha256=A65KT1a0SZCGKqsaJufxUHrzsvJsd7VBJbRt3O5aC84,7666
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=YbiV_0cv_W0xrhtZLg6ActLeSRYYikrOzHz0FqJ0LII,6298
-sparseml/yolov8/utils/helpers.py,sha256=4lMfBZIYyZ3rv8JkDBiMHORUfEjnLJrTmCFXQhRr6RI,1355
-sparseml_nightly-1.5.0.20230404.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.5.0.20230404.dist-info/METADATA,sha256=e9L4EXaAOFTOTC7SFd_TApSPCXm3WgpVhIuji_LXme4,20658
-sparseml_nightly-1.5.0.20230404.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.5.0.20230404.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.5.0.20230404.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
-sparseml_nightly-1.5.0.20230404.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.5.0.20230404.dist-info/RECORD,,
+sparseml/yolov8/utils/helpers.py,sha256=P6RyXxq6pyorWlsdcfRy8i_ncezCpvwQNIsXE7vDFSM,2534
+sparseml_nightly-1.5.0.20230412.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.5.0.20230412.dist-info/METADATA,sha256=Er83gTenbV7VOQfPgoHnUx31JuRGwWEVSqDziWBu2b8,20659
+sparseml_nightly-1.5.0.20230412.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.5.0.20230412.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
+sparseml_nightly-1.5.0.20230412.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.5.0.20230412.dist-info/RECORD,,
```

