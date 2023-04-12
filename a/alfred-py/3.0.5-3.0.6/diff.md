# Comparing `tmp/alfred-py-3.0.5.tar.gz` & `tmp/alfred-py-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-py-3.0.5.tar", last modified: Sat Apr  8 07:48:12 2023, max compression
+gzip compressed data, was "alfred-py-3.0.6.tar", last modified: Wed Apr 12 11:13:40 2023, max compression
```

## Comparing `alfred-py-3.0.5.tar` & `alfred-py-3.0.6.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.429320 alfred-py-3.0.5/
--rw-rw-rw-   0        0        0    35786 2023-04-08 07:17:55.000000 alfred-py-3.0.5/LICENSE
--rw-rw-rw-   0        0        0      151 2023-04-08 07:17:55.000000 alfred-py-3.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    25052 2023-04-08 07:48:12.429320 alfred-py-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    24015 2023-04-08 07:17:55.000000 alfred-py-3.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.149055 alfred-py-3.0.5/alfred/
--rw-rw-rw-   0        0        0     1303 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/__init__.py
--rw-rw-rw-   0        0        0    26424 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/alfred.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.112537 alfred-py-3.0.5/alfred/deploy/
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.157183 alfred-py-3.0.5/alfred/deploy/tensorrt/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/deploy/tensorrt/__init__.py
--rw-rw-rw-   0        0        0     2234 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/deploy/tensorrt/calibrator.py
--rw-rw-rw-   0        0        0    20962 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/deploy/tensorrt/common.py
--rw-rw-rw-   0        0        0     3337 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/deploy/tensorrt/process.py
--rw-rw-rw-   0        0        0     4021 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/deploy/tensorrt/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.159178 alfred-py-3.0.5/alfred/dl/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.114532 alfred-py-3.0.5/alfred/dl/data/
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.161173 alfred-py-3.0.5/alfred/dl/data/common/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/common/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/common/coco_dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.167877 alfred-py-3.0.5/alfred/dl/data/meta/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/meta/__init__.py
--rw-rw-rw-   0        0        0     1532 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/meta/concatenated_dataset.py
--rw-rw-rw-   0        0        0     3032 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/meta/dataset_mixin.py
--rw-rw-rw-   0        0        0     3261 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/meta/getter_dataset.py
--rw-rw-rw-   0        0        0     5205 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/data/meta/sliceable_dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.170869 alfred-py-3.0.5/alfred/dl/evaluator/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/evaluator/__init__.py
--rw-rw-rw-   0        0        0    11447 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/evaluator/yolo_evaluator.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.173861 alfred-py-3.0.5/alfred/dl/inference/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/inference/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/inference/image_inference.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.177850 alfred-py-3.0.5/alfred/dl/metrics/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/metrics/__init__.py
--rw-rw-rw-   0        0        0    11818 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/metrics/iou_loss.py
--rw-rw-rw-   0        0        0     7993 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/metrics/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.178847 alfred-py-3.0.5/alfred/dl/tf/
--rw-rw-rw-   0        0        0     1133 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/tf/common.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.189818 alfred-py-3.0.5/alfred/dl/torch/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/__init__.py
--rw-rw-rw-   0        0        0     3054 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/common.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.190818 alfred-py-3.0.5/alfred/dl/torch/distribute/
--rw-rw-rw-   0        0        0     8464 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/distribute/utils.py
--rw-rw-rw-   0        0        0     3374 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/env.py
--rw-rw-rw-   0        0        0     1101 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/gpu.py
--rw-rw-rw-   0        0        0    11624 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/metrics.py
--rw-rw-rw-   0        0        0     6369 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/model_summary.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.194805 alfred-py-3.0.5/alfred/dl/torch/nn/
--rw-rw-rw-   0        0        0     1038 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/nn/__init__.py
--rw-rw-rw-   0        0        0     1205 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/nn/functional.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.199792 alfred-py-3.0.5/alfred/dl/torch/nn/modules/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/nn/modules/__init__.py
--rw-rw-rw-   0        0        0     3882 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/nn/modules/common.py
--rw-rw-rw-   0        0        0     1195 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/nn/modules/normalization.py
--rw-rw-rw-   0        0        0     2049 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/nn/weights_init.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.202784 alfred-py-3.0.5/alfred/dl/torch/ops/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/ops/__init__.py
--rw-rw-rw-   0        0        0     2003 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/ops/array_ops.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.203781 alfred-py-3.0.5/alfred/dl/torch/runner/
--rw-rw-rw-   0        0        0    10080 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/runner/checkpoint.py
--rw-rw-rw-   0        0        0     3245 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.213756 alfred-py-3.0.5/alfred/dl/torch/train/
--rw-rw-rw-   0        0        0     1216 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/__init__.py
--rw-rw-rw-   0        0        0     7564 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/checkpoint.py
--rw-rw-rw-   0        0        0     1651 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/common.py
--rw-rw-rw-   0        0        0    12713 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/fastai_optim.py
--rw-rw-rw-   0        0        0     7598 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/learning_schedules.py
--rw-rw-rw-   0        0        0     6500 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/learning_schedules_fastai.py
--rw-rw-rw-   0        0        0     5101 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/dl/torch/train/optim.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.215749 alfred-py-3.0.5/alfred/fonts/
--rw-rw-rw-   0        0        0  2763148 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/fonts/FZSSJW.TTF
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.234699 alfred-py-3.0.5/alfred/fusion/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/fusion/__init__.py
--rw-rw-rw-   0        0        0     5638 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/fusion/common.py
--rw-rw-rw-   0        0        0     2097 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/fusion/geometry.py
--rw-rw-rw-   0        0        0     9435 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/fusion/kitti_fusion.py
--rw-rw-rw-   0        0        0     4013 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/fusion/nuscenes_fusion.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.236693 alfred-py-3.0.5/alfred/modules/
--rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.249658 alfred-py-3.0.5/alfred/modules/cabinet/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/__init__.py
--rw-rw-rw-   0        0        0     1075 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/changesource.py
--rw-rw-rw-   0        0        0     1660 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/count_file.py
--rw-rw-rw-   0        0        0    19617 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/gtrend.py
--rw-rw-rw-   0        0        0    24437 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/license.py
--rw-rw-rw-   0        0        0     5791 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/markdown_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.255642 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.263621 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/formatters/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/formatters/__init__.py
--rw-rw-rw-   0        0        0      346 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/formatters/html.py
--rw-rw-rw-   0        0        0      945 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/formatters/pdf.py
--rw-rw-rw-   0        0        0      214 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/formatters/simple.py
--rw-rw-rw-   0        0        0     4992 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/image_downloader.py
--rw-rw-rw-   0        0        0      437 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/string_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.266613 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.268608 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/html/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/html/__init__.py
--rw-rw-rw-   0        0        0     2209 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/html/transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.271600 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/md/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/md/__init__.py
--rw-rw-rw-   0        0        0     2196 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/md/transformer.py
--rw-rw-rw-   0        0        0     1842 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/mdparse/www_tools.py
--rw-rw-rw-   0        0        0     2657 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/split_txt.py
--rw-rw-rw-   0        0        0     1780 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/stack_imgs.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.287557 alfred-py-3.0.5/alfred/modules/cabinet/templates/
--rw-rw-rw-   0        0        0      742 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/agpl-v3.tmpl
--rw-rw-rw-   0        0        0      868 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/apache-2.tmpl
--rw-rw-rw-   0        0        0      170 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/bsd-3.tmpl
--rw-rw-rw-   0        0        0     1448 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/cecill-B.tmpl
--rw-rw-rw-   0        0        0     1448 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/cecill-C.tmpl
--rw-rw-rw-   0        0        0     1442 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/cecill.tmpl
--rw-rw-rw-   0        0        0      721 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/gpl-v3.tmpl
--rw-rw-rw-   0        0        0      744 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl
--rw-rw-rw-   0        0        0      742 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/templates/lgpl-v3.tmpl
--rw-rw-rw-   0        0        0     2140 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/cabinet/webcam.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.320469 alfred-py-3.0.5/alfred/modules/data/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/coco2voc.py
--rw-rw-rw-   0        0        0     2928 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/coco2yolo.py
--rw-rw-rw-   0        0        0     3618 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/convert_csv2voc.py
--rw-rw-rw-   0        0        0     7363 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/convert_cvat2voc.py
--rw-rw-rw-   0        0        0     4280 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/convert_labelone2voc.py
--rw-rw-rw-   0        0        0      156 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/eval_coco.py
--rw-rw-rw-   0        0        0    38129 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/eval_voc.py
--rw-rw-rw-   0        0        0     5868 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/extract_voc.py
--rw-rw-rw-   0        0        0     2546 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/gather_voclabels.py
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/labelone_view.py
--rw-rw-rw-   0        0        0     4422 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/mergevoc.py
--rw-rw-rw-   0        0        0     2366 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/split_coco.py
--rw-rw-rw-   0        0        0     1629 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/split_voc.py
--rw-rw-rw-   0        0        0     3580 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/txt2voc.py
--rw-rw-rw-   0        0        0    10384 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/view_coco.py
--rw-rw-rw-   0        0        0     3218 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/view_txt.py
--rw-rw-rw-   0        0        0     4921 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/view_voc.py
--rw-rw-rw-   0        0        0     2894 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/view_yolo.py
--rw-rw-rw-   0        0        0     8501 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/voc2coco.py
--rw-rw-rw-   0        0        0     1986 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/voc2yolo.py
--rw-rw-rw-   0        0        0     4373 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/data/yolo2voc.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.322464 alfred-py-3.0.5/alfred/modules/dltool/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/dltool/__init__.py
--rw-rw-rw-   0        0        0     5475 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/dltool/cal_anchors.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.327451 alfred-py-3.0.5/alfred/modules/scrap/
--rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/scrap/__init__.py
--rw-rw-rw-   0        0        0     4430 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/scrap/image_scraper.py
--rw-rw-rw-   0        0        0     5017 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/scrap/scraper_images.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.328448 alfred-py-3.0.5/alfred/modules/text/
--rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.337424 alfred-py-3.0.5/alfred/modules/vision/
--rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/vision/__init__.py
--rw-rw-rw-   0        0        0     4315 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/vision/face_extractor.py
--rw-rw-rw-   0        0        0     3104 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/vision/to_video.py
--rw-rw-rw-   0        0        0     2849 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/vision/video_extractor.py
--rw-rw-rw-   0        0        0     2972 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/vision/video_reducer.py
--rw-rw-rw-   0        0        0     9581 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/modules/vision/vis_kit.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.339418 alfred-py-3.0.5/alfred/protos/
--rw-rw-rw-   0        0        0     5249 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/protos/labelmap_pb2.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.343408 alfred-py-3.0.5/alfred/siren/
--rw-rw-rw-   0        0        0     9211 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/siren/handler.py
--rw-rw-rw-   0        0        0     3808 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/siren/models.py
--rw-rw-rw-   0        0        0      552 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/siren/topicgen.py
--rw-rw-rw-   0        0        0     2118 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.363496 alfred-py-3.0.5/alfred/utils/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/__init__.py
--rw-rw-rw-   0        0        0     1323 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/base_config.py
--rw-rw-rw-   0        0        0     1509 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/communicate.py
--rw-rw-rw-   0        0        0      792 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/cv_wrapper.py
--rw-rw-rw-   0        0        0    30051 2023-04-08 07:44:03.000000 alfred-py-3.0.5/alfred/utils/file_io.py
--rw-rw-rw-   0        0        0      865 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/image_convertor.py
--rw-rw-rw-   0        0        0     2084 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/log.py
--rw-rw-rw-   0        0        0     1782 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/mana.py
--rw-rw-rw-   0        0        0     1093 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/math_utils.py
--rw-rw-rw-   0        0        0      572 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/pprint.py
--rw-rw-rw-   0        0        0     3327 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/utils/timer.py
--rw-rw-rw-   0        0        0      595 2023-04-08 07:45:19.000000 alfred-py-3.0.5/alfred/version.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.364493 alfred-py-3.0.5/alfred/vis/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.386435 alfred-py-3.0.5/alfred/vis/image/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/__init__.py
--rw-rw-rw-   0        0        0     5377 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/common.py
--rw-rw-rw-   0        0        0     4804 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/constants.py
--rw-rw-rw-   0        0        0    33098 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/det.py
--rw-rw-rw-   0        0        0     1228 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/face.py
--rw-rw-rw-   0        0        0    12540 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/get_dataset_color_map.py
--rw-rw-rw-   0        0        0    57388 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/get_dataset_label_map.py
--rw-rw-rw-   0        0        0    16379 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/mask.py
--rw-rw-rw-   0        0        0    21942 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose.py
--rw-rw-rw-   0        0        0     6154 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_dataset_info.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.399400 alfred-py-3.0.5/alfred/vis/image/pose_datasets/
--rw-rw-rw-   0        0        0     5581 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/animalpose.py
--rw-rw-rw-   0        0        0     5433 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco.py
--rw-rw-rw-   0        0        0    31889 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco_wholebody.py
--rw-rw-rw-   0        0        0    11622 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco_wholebody_face.py
--rw-rw-rw-   0        0        0     5145 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco_wholebody_hand.py
--rw-rw-rw-   0        0        0     4915 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/interhand2d.py
--rw-rw-rw-   0        0        0    13576 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/interhand3d.py
--rw-rw-rw-   0        0        0     4765 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/mpii.py
--rw-rw-rw-   0        0        0     4918 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_datasets/onehand10k.py
--rw-rw-rw-   0        0        0     6115 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/pose_hand.py
--rw-rw-rw-   0        0        0      355 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/process.py
--rw-rw-rw-   0        0        0     2544 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/image/seg.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.407379 alfred-py-3.0.5/alfred/vis/mesh3d/
--rw-rw-rw-   0        0        0    36188 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/mesh3d/o3d_visconfig.py
--rw-rw-rw-   0        0        0     8595 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/mesh3d/o3dsocket.py
--rw-rw-rw-   0        0        0    15713 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/mesh3d/o3dwrapper.py
--rw-rw-rw-   0        0        0     5696 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/mesh3d/skelmodel.py
--rw-rw-rw-   0        0        0     9602 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/mesh3d/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.410371 alfred-py-3.0.5/alfred/vis/pointcloud/
--rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/pointcloud/__init__.py
--rw-rw-rw-   0        0        0     4572 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/pointcloud/pointcloud_vis.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.413363 alfred-py-3.0.5/alfred/vis/renders/
--rw-rw-rw-   0        0        0     8587 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/renders/render_p3d.py
--rw-rw-rw-   0        0        0     4753 2023-04-08 07:17:55.000000 alfred-py-3.0.5/alfred/vis/renders/render_prd.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:48:12.426328 alfred-py-3.0.5/alfred_py.egg-info/
--rw-rw-rw-   0        0        0    25052 2023-04-08 07:48:11.000000 alfred-py-3.0.5/alfred_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6148 2023-04-08 07:48:12.000000 alfred-py-3.0.5/alfred_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 07:48:11.000000 alfred-py-3.0.5/alfred_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-08 07:48:11.000000 alfred-py-3.0.5/alfred_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      174 2023-04-08 07:48:11.000000 alfred-py-3.0.5/alfred_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-08 07:48:11.000000 alfred-py-3.0.5/alfred_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      441 2023-04-08 07:48:12.430317 alfred-py-3.0.5/setup.cfg
--rw-rw-rw-   0        0        0     5160 2023-04-08 07:17:55.000000 alfred-py-3.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.074607 alfred-py-3.0.6/
+-rw-rw-rw-   0        0        0    35786 2023-02-10 05:13:33.000000 alfred-py-3.0.6/LICENSE
+-rw-rw-rw-   0        0        0      151 2023-02-10 05:13:33.000000 alfred-py-3.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    25052 2023-04-12 11:13:40.075152 alfred-py-3.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    24015 2023-02-10 05:13:33.000000 alfred-py-3.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.842231 alfred-py-3.0.6/alfred/
+-rw-rw-rw-   0        0        0     1303 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/__init__.py
+-rw-rw-rw-   0        0        0    26424 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/alfred.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.817298 alfred-py-3.0.6/alfred/deploy/
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.849214 alfred-py-3.0.6/alfred/deploy/tensorrt/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/__init__.py
+-rw-rw-rw-   0        0        0     2234 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/calibrator.py
+-rw-rw-rw-   0        0        0    20962 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/common.py
+-rw-rw-rw-   0        0        0     3337 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/process.py
+-rw-rw-rw-   0        0        0     4021 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.850211 alfred-py-3.0.6/alfred/dl/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.819292 alfred-py-3.0.6/alfred/dl/data/
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.853202 alfred-py-3.0.6/alfred/dl/data/common/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/common/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/common/coco_dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.859186 alfred-py-3.0.6/alfred/dl/data/meta/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/__init__.py
+-rw-rw-rw-   0        0        0     1532 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/concatenated_dataset.py
+-rw-rw-rw-   0        0        0     3032 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/dataset_mixin.py
+-rw-rw-rw-   0        0        0     3261 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/getter_dataset.py
+-rw-rw-rw-   0        0        0     5205 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/sliceable_dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.861181 alfred-py-3.0.6/alfred/dl/evaluator/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/evaluator/__init__.py
+-rw-rw-rw-   0        0        0    11447 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/evaluator/yolo_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.864173 alfred-py-3.0.6/alfred/dl/inference/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/inference/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/inference/image_inference.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.868162 alfred-py-3.0.6/alfred/dl/metrics/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/metrics/__init__.py
+-rw-rw-rw-   0        0        0    11818 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/metrics/iou_loss.py
+-rw-rw-rw-   0        0        0     7993 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/metrics/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.869161 alfred-py-3.0.6/alfred/dl/tf/
+-rw-rw-rw-   0        0        0     1133 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/tf/common.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.879134 alfred-py-3.0.6/alfred/dl/torch/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/__init__.py
+-rw-rw-rw-   0        0        0     3054 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/common.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.880131 alfred-py-3.0.6/alfred/dl/torch/distribute/
+-rw-rw-rw-   0        0        0     8464 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/distribute/utils.py
+-rw-rw-rw-   0        0        0     3374 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/env.py
+-rw-rw-rw-   0        0        0     1101 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/gpu.py
+-rw-rw-rw-   0        0        0    11624 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/metrics.py
+-rw-rw-rw-   0        0        0     6369 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/model_summary.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.885118 alfred-py-3.0.6/alfred/dl/torch/nn/
+-rw-rw-rw-   0        0        0     1038 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/__init__.py
+-rw-rw-rw-   0        0        0     1205 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/functional.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.889107 alfred-py-3.0.6/alfred/dl/torch/nn/modules/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0     3882 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/modules/common.py
+-rw-rw-rw-   0        0        0     1195 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/modules/normalization.py
+-rw-rw-rw-   0        0        0     2049 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/weights_init.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.891101 alfred-py-3.0.6/alfred/dl/torch/ops/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/ops/__init__.py
+-rw-rw-rw-   0        0        0     2003 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/ops/array_ops.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.893095 alfred-py-3.0.6/alfred/dl/torch/runner/
+-rw-rw-rw-   0        0        0    10080 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/runner/checkpoint.py
+-rw-rw-rw-   0        0        0     3245 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.903070 alfred-py-3.0.6/alfred/dl/torch/train/
+-rw-rw-rw-   0        0        0     1216 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/__init__.py
+-rw-rw-rw-   0        0        0     7564 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/checkpoint.py
+-rw-rw-rw-   0        0        0     1651 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/common.py
+-rw-rw-rw-   0        0        0    12713 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/fastai_optim.py
+-rw-rw-rw-   0        0        0     7598 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules.py
+-rw-rw-rw-   0        0        0     6500 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules_fastai.py
+-rw-rw-rw-   0        0        0     5101 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/optim.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.904067 alfred-py-3.0.6/alfred/fonts/
+-rw-rw-rw-   0        0        0  2763148 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fonts/FZSSJW.TTF
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.914040 alfred-py-3.0.6/alfred/fusion/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/__init__.py
+-rw-rw-rw-   0        0        0     5638 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/common.py
+-rw-rw-rw-   0        0        0     2097 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/geometry.py
+-rw-rw-rw-   0        0        0     9435 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/kitti_fusion.py
+-rw-rw-rw-   0        0        0     4013 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/nuscenes_fusion.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.914981 alfred-py-3.0.6/alfred/modules/
+-rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.927984 alfred-py-3.0.6/alfred/modules/cabinet/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/__init__.py
+-rw-rw-rw-   0        0        0     1075 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/changesource.py
+-rw-rw-rw-   0        0        0     1660 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/count_file.py
+-rw-rw-rw-   0        0        0    19617 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/gtrend.py
+-rw-rw-rw-   0        0        0    24437 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/license.py
+-rw-rw-rw-   0        0        0     5791 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/markdown_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.932971 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.937958 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/__init__.py
+-rw-rw-rw-   0        0        0      346 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/html.py
+-rw-rw-rw-   0        0        0      945 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/pdf.py
+-rw-rw-rw-   0        0        0      214 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/simple.py
+-rw-rw-rw-   0        0        0     4992 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/image_downloader.py
+-rw-rw-rw-   0        0        0      437 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/string_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.939952 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.941946 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/__init__.py
+-rw-rw-rw-   0        0        0     2209 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.945936 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/__init__.py
+-rw-rw-rw-   0        0        0     2196 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/transformer.py
+-rw-rw-rw-   0        0        0     1842 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/www_tools.py
+-rw-rw-rw-   0        0        0     2657 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/split_txt.py
+-rw-rw-rw-   0        0        0     1780 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/stack_imgs.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.957904 alfred-py-3.0.6/alfred/modules/cabinet/templates/
+-rw-rw-rw-   0        0        0      742 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/agpl-v3.tmpl
+-rw-rw-rw-   0        0        0      868 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/apache-2.tmpl
+-rw-rw-rw-   0        0        0      170 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/bsd-3.tmpl
+-rw-rw-rw-   0        0        0     1448 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-B.tmpl
+-rw-rw-rw-   0        0        0     1448 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-C.tmpl
+-rw-rw-rw-   0        0        0     1442 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill.tmpl
+-rw-rw-rw-   0        0        0      721 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/gpl-v3.tmpl
+-rw-rw-rw-   0        0        0      744 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl
+-rw-rw-rw-   0        0        0      742 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v3.tmpl
+-rw-rw-rw-   0        0        0     2140 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/webcam.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.987824 alfred-py-3.0.6/alfred/modules/data/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/coco2voc.py
+-rw-rw-rw-   0        0        0     2928 2023-04-04 07:40:56.000000 alfred-py-3.0.6/alfred/modules/data/coco2yolo.py
+-rw-rw-rw-   0        0        0     3618 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/convert_csv2voc.py
+-rw-rw-rw-   0        0        0     7363 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/convert_cvat2voc.py
+-rw-rw-rw-   0        0        0     4280 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/convert_labelone2voc.py
+-rw-rw-rw-   0        0        0      156 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/eval_coco.py
+-rw-rw-rw-   0        0        0    38129 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/eval_voc.py
+-rw-rw-rw-   0        0        0     5868 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/extract_voc.py
+-rw-rw-rw-   0        0        0     2546 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/gather_voclabels.py
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/labelone_view.py
+-rw-rw-rw-   0        0        0     4422 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/mergevoc.py
+-rw-rw-rw-   0        0        0     2366 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/split_coco.py
+-rw-rw-rw-   0        0        0     1629 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/split_voc.py
+-rw-rw-rw-   0        0        0     3580 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/txt2voc.py
+-rw-rw-rw-   0        0        0    10384 2023-04-04 07:40:56.000000 alfred-py-3.0.6/alfred/modules/data/view_coco.py
+-rw-rw-rw-   0        0        0     3218 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/view_txt.py
+-rw-rw-rw-   0        0        0     4921 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/view_voc.py
+-rw-rw-rw-   0        0        0     2894 2023-04-04 07:40:56.000000 alfred-py-3.0.6/alfred/modules/data/view_yolo.py
+-rw-rw-rw-   0        0        0     8501 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/voc2coco.py
+-rw-rw-rw-   0        0        0     1986 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/voc2yolo.py
+-rw-rw-rw-   0        0        0     4373 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/yolo2voc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.990834 alfred-py-3.0.6/alfred/modules/dltool/
+-rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/dltool/__init__.py
+-rw-rw-rw-   0        0        0     5475 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/dltool/cal_anchors.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.994805 alfred-py-3.0.6/alfred/modules/scrap/
+-rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/scrap/__init__.py
+-rw-rw-rw-   0        0        0     4430 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/scrap/image_scraper.py
+-rw-rw-rw-   0        0        0     5017 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/scrap/scraper_images.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.995803 alfred-py-3.0.6/alfred/modules/text/
+-rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.003781 alfred-py-3.0.6/alfred/modules/vision/
+-rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/__init__.py
+-rw-rw-rw-   0        0        0     4315 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/face_extractor.py
+-rw-rw-rw-   0        0        0     3104 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/to_video.py
+-rw-rw-rw-   0        0        0     2849 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/video_extractor.py
+-rw-rw-rw-   0        0        0     2972 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/video_reducer.py
+-rw-rw-rw-   0        0        0     9581 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/vis_kit.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.004780 alfred-py-3.0.6/alfred/protos/
+-rw-rw-rw-   0        0        0     5249 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/protos/labelmap_pb2.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.008767 alfred-py-3.0.6/alfred/siren/
+-rw-rw-rw-   0        0        0     9211 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/siren/handler.py
+-rw-rw-rw-   0        0        0     3808 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/siren/models.py
+-rw-rw-rw-   0        0        0      552 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/siren/topicgen.py
+-rw-rw-rw-   0        0        0     2118 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.022730 alfred-py-3.0.6/alfred/utils/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/__init__.py
+-rw-rw-rw-   0        0        0     1323 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/base_config.py
+-rw-rw-rw-   0        0        0     1509 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/communicate.py
+-rw-rw-rw-   0        0        0      792 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/cv_wrapper.py
+-rw-rw-rw-   0        0        0    29308 2023-04-11 03:00:54.000000 alfred-py-3.0.6/alfred/utils/file_io.py
+-rw-rw-rw-   0        0        0      695 2023-04-10 06:58:27.000000 alfred-py-3.0.6/alfred/utils/image_convertor.py
+-rw-rw-rw-   0        0        0     2084 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/log.py
+-rw-rw-rw-   0        0        0     1782 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/mana.py
+-rw-rw-rw-   0        0        0     1093 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/math_utils.py
+-rw-rw-rw-   0        0        0      572 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/pprint.py
+-rw-rw-rw-   0        0        0     3327 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/timer.py
+-rw-rw-rw-   0        0        0      595 2023-04-12 11:13:37.000000 alfred-py-3.0.6/alfred/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.023728 alfred-py-3.0.6/alfred/vis/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.040682 alfred-py-3.0.6/alfred/vis/image/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/__init__.py
+-rw-rw-rw-   0        0        0     5377 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/common.py
+-rw-rw-rw-   0        0        0     4804 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/constants.py
+-rw-rw-rw-   0        0        0    33098 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/det.py
+-rw-rw-rw-   0        0        0     1228 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/face.py
+-rw-rw-rw-   0        0        0    12540 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/get_dataset_color_map.py
+-rw-rw-rw-   0        0        0    57388 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/get_dataset_label_map.py
+-rw-rw-rw-   0        0        0    16379 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/mask.py
+-rw-rw-rw-   0        0        0    21942 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose.py
+-rw-rw-rw-   0        0        0     6154 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_dataset_info.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.053648 alfred-py-3.0.6/alfred/vis/image/pose_datasets/
+-rw-rw-rw-   0        0        0     5581 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/animalpose.py
+-rw-rw-rw-   0        0        0     5433 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco.py
+-rw-rw-rw-   0        0        0    31889 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody.py
+-rw-rw-rw-   0        0        0    11622 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_face.py
+-rw-rw-rw-   0        0        0     5145 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_hand.py
+-rw-rw-rw-   0        0        0     4915 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/interhand2d.py
+-rw-rw-rw-   0        0        0    13576 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/interhand3d.py
+-rw-rw-rw-   0        0        0     4765 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/mpii.py
+-rw-rw-rw-   0        0        0     4918 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/onehand10k.py
+-rw-rw-rw-   0        0        0     6115 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_hand.py
+-rw-rw-rw-   0        0        0      355 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/process.py
+-rw-rw-rw-   0        0        0     2544 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/seg.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.059632 alfred-py-3.0.6/alfred/vis/mesh3d/
+-rw-rw-rw-   0        0        0    36188 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/o3d_visconfig.py
+-rw-rw-rw-   0        0        0     8595 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/o3dsocket.py
+-rw-rw-rw-   0        0        0    15713 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/o3dwrapper.py
+-rw-rw-rw-   0        0        0     5696 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/skelmodel.py
+-rw-rw-rw-   0        0        0     9602 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.061627 alfred-py-3.0.6/alfred/vis/pointcloud/
+-rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/pointcloud/__init__.py
+-rw-rw-rw-   0        0        0     4572 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/pointcloud/pointcloud_vis.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.064619 alfred-py-3.0.6/alfred/vis/renders/
+-rw-rw-rw-   0        0        0     8587 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/renders/render_p3d.py
+-rw-rw-rw-   0        0        0     4753 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/renders/render_prd.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.073011 alfred-py-3.0.6/alfred_py.egg-info/
+-rw-rw-rw-   0        0        0    25052 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6148 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      441 2023-04-12 11:13:40.075701 alfred-py-3.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     5160 2023-02-10 05:13:33.000000 alfred-py-3.0.6/setup.py
```

### Comparing `alfred-py-3.0.5/LICENSE` & `alfred-py-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/PKG-INFO` & `alfred-py-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-py
-Version: 3.0.5
+Version: 3.0.6
 Summary: Alfred is a DeepLearning utility library.
 Home-page: https://github.com/jinfagang/alfred
 Author: Lucas Jin
 Author-email: jinfagang19@163.com
 License: GPL-3.0
 Keywords: deep learning,script helper,tools
 Platform: any
```

### Comparing `alfred-py-3.0.5/README.md` & `alfred-py-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/__init__.py` & `alfred-py-3.0.6/alfred/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/alfred.py` & `alfred-py-3.0.6/alfred/alfred.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/deploy/tensorrt/calibrator.py` & `alfred-py-3.0.6/alfred/deploy/tensorrt/calibrator.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/deploy/tensorrt/common.py` & `alfred-py-3.0.6/alfred/deploy/tensorrt/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/deploy/tensorrt/process.py` & `alfred-py-3.0.6/alfred/deploy/tensorrt/process.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/deploy/tensorrt/wrapper.py` & `alfred-py-3.0.6/alfred/deploy/tensorrt/wrapper.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/__init__.py` & `alfred-py-3.0.6/alfred/dl/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/data/common/coco_dataset.py` & `alfred-py-3.0.6/alfred/dl/data/common/coco_dataset.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/data/meta/concatenated_dataset.py` & `alfred-py-3.0.6/alfred/dl/data/meta/concatenated_dataset.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/data/meta/dataset_mixin.py` & `alfred-py-3.0.6/alfred/dl/data/meta/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/data/meta/getter_dataset.py` & `alfred-py-3.0.6/alfred/dl/data/meta/getter_dataset.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/data/meta/sliceable_dataset.py` & `alfred-py-3.0.6/alfred/dl/data/meta/sliceable_dataset.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/evaluator/yolo_evaluator.py` & `alfred-py-3.0.6/alfred/dl/evaluator/yolo_evaluator.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/inference/__init__.py` & `alfred-py-3.0.6/alfred/dl/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/inference/image_inference.py` & `alfred-py-3.0.6/alfred/dl/inference/image_inference.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/metrics/iou_loss.py` & `alfred-py-3.0.6/alfred/dl/metrics/iou_loss.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/metrics/utils.py` & `alfred-py-3.0.6/alfred/dl/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/tf/common.py` & `alfred-py-3.0.6/alfred/dl/tf/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/__init__.py` & `alfred-py-3.0.6/alfred/dl/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/common.py` & `alfred-py-3.0.6/alfred/dl/torch/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/distribute/utils.py` & `alfred-py-3.0.6/alfred/dl/torch/distribute/utils.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/env.py` & `alfred-py-3.0.6/alfred/dl/torch/env.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/gpu.py` & `alfred-py-3.0.6/alfred/dl/torch/gpu.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/metrics.py` & `alfred-py-3.0.6/alfred/dl/torch/metrics.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/model_summary.py` & `alfred-py-3.0.6/alfred/dl/torch/model_summary.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/nn/__init__.py` & `alfred-py-3.0.6/alfred/dl/torch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/nn/functional.py` & `alfred-py-3.0.6/alfred/dl/torch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/nn/modules/__init__.py` & `alfred-py-3.0.6/alfred/dl/torch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/nn/modules/common.py` & `alfred-py-3.0.6/alfred/dl/torch/nn/modules/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/nn/modules/normalization.py` & `alfred-py-3.0.6/alfred/dl/torch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/nn/weights_init.py` & `alfred-py-3.0.6/alfred/dl/torch/nn/weights_init.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/ops/__init__.py` & `alfred-py-3.0.6/alfred/dl/torch/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/ops/array_ops.py` & `alfred-py-3.0.6/alfred/dl/torch/ops/array_ops.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/runner/checkpoint.py` & `alfred-py-3.0.6/alfred/dl/torch/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/tools.py` & `alfred-py-3.0.6/alfred/dl/torch/tools.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/__init__.py` & `alfred-py-3.0.6/alfred/dl/torch/train/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/checkpoint.py` & `alfred-py-3.0.6/alfred/dl/torch/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/common.py` & `alfred-py-3.0.6/alfred/dl/torch/train/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/fastai_optim.py` & `alfred-py-3.0.6/alfred/dl/torch/train/fastai_optim.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/learning_schedules.py` & `alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/learning_schedules_fastai.py` & `alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules_fastai.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/dl/torch/train/optim.py` & `alfred-py-3.0.6/alfred/dl/torch/train/optim.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/fonts/FZSSJW.TTF` & `alfred-py-3.0.6/alfred/fonts/FZSSJW.TTF`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/fusion/__init__.py` & `alfred-py-3.0.6/alfred/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/fusion/common.py` & `alfred-py-3.0.6/alfred/fusion/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/fusion/geometry.py` & `alfred-py-3.0.6/alfred/fusion/geometry.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/fusion/kitti_fusion.py` & `alfred-py-3.0.6/alfred/fusion/kitti_fusion.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/fusion/nuscenes_fusion.py` & `alfred-py-3.0.6/alfred/fusion/nuscenes_fusion.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/__init__.py` & `alfred-py-3.0.6/alfred/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/__init__.py` & `alfred-py-3.0.6/alfred/modules/cabinet/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/changesource.py` & `alfred-py-3.0.6/alfred/modules/cabinet/changesource.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/count_file.py` & `alfred-py-3.0.6/alfred/modules/cabinet/count_file.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/gtrend.py` & `alfred-py-3.0.6/alfred/modules/cabinet/gtrend.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/license.py` & `alfred-py-3.0.6/alfred/modules/cabinet/license.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/markdown_tool.py` & `alfred-py-3.0.6/alfred/modules/cabinet/markdown_tool.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/mdparse/formatters/pdf.py` & `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/pdf.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/mdparse/image_downloader.py` & `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/image_downloader.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/html/transformer.py` & `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/transformer.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/mdparse/transformers/md/transformer.py` & `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/transformer.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/mdparse/www_tools.py` & `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/www_tools.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/split_txt.py` & `alfred-py-3.0.6/alfred/modules/cabinet/split_txt.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/stack_imgs.py` & `alfred-py-3.0.6/alfred/modules/cabinet/stack_imgs.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/agpl-v3.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/agpl-v3.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/apache-2.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/apache-2.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/cecill-B.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-B.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/cecill-C.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-C.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/cecill.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/gpl-v3.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/gpl-v3.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/templates/lgpl-v3.tmpl` & `alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v3.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/cabinet/webcam.py` & `alfred-py-3.0.6/alfred/modules/cabinet/webcam.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/__init__.py` & `alfred-py-3.0.6/alfred/modules/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/coco2yolo.py` & `alfred-py-3.0.6/alfred/modules/data/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/convert_csv2voc.py` & `alfred-py-3.0.6/alfred/modules/data/convert_csv2voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/convert_cvat2voc.py` & `alfred-py-3.0.6/alfred/modules/data/convert_cvat2voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/convert_labelone2voc.py` & `alfred-py-3.0.6/alfred/modules/data/convert_labelone2voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/eval_voc.py` & `alfred-py-3.0.6/alfred/modules/data/eval_voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/extract_voc.py` & `alfred-py-3.0.6/alfred/modules/data/extract_voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/gather_voclabels.py` & `alfred-py-3.0.6/alfred/modules/data/gather_voclabels.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/labelone_view.py` & `alfred-py-3.0.6/alfred/modules/data/labelone_view.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/mergevoc.py` & `alfred-py-3.0.6/alfred/modules/data/mergevoc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/split_coco.py` & `alfred-py-3.0.6/alfred/modules/data/split_coco.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/split_voc.py` & `alfred-py-3.0.6/alfred/modules/data/split_voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/txt2voc.py` & `alfred-py-3.0.6/alfred/modules/data/txt2voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/view_coco.py` & `alfred-py-3.0.6/alfred/modules/data/view_coco.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/view_txt.py` & `alfred-py-3.0.6/alfred/modules/data/view_txt.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/view_voc.py` & `alfred-py-3.0.6/alfred/modules/data/view_voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/view_yolo.py` & `alfred-py-3.0.6/alfred/modules/data/view_yolo.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/voc2coco.py` & `alfred-py-3.0.6/alfred/modules/data/voc2coco.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/voc2yolo.py` & `alfred-py-3.0.6/alfred/modules/data/voc2yolo.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/data/yolo2voc.py` & `alfred-py-3.0.6/alfred/modules/data/yolo2voc.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/dltool/cal_anchors.py` & `alfred-py-3.0.6/alfred/modules/dltool/cal_anchors.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/scrap/__init__.py` & `alfred-py-3.0.6/alfred/modules/scrap/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/scrap/image_scraper.py` & `alfred-py-3.0.6/alfred/modules/scrap/image_scraper.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/scrap/scraper_images.py` & `alfred-py-3.0.6/alfred/modules/scrap/scraper_images.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/text/__init__.py` & `alfred-py-3.0.6/alfred/modules/text/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/vision/__init__.py` & `alfred-py-3.0.6/alfred/modules/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/vision/face_extractor.py` & `alfred-py-3.0.6/alfred/modules/vision/face_extractor.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/vision/to_video.py` & `alfred-py-3.0.6/alfred/modules/vision/to_video.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/vision/video_extractor.py` & `alfred-py-3.0.6/alfred/modules/vision/video_extractor.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/vision/video_reducer.py` & `alfred-py-3.0.6/alfred/modules/vision/video_reducer.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/modules/vision/vis_kit.py` & `alfred-py-3.0.6/alfred/modules/vision/vis_kit.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/protos/labelmap_pb2.py` & `alfred-py-3.0.6/alfred/protos/labelmap_pb2.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/siren/handler.py` & `alfred-py-3.0.6/alfred/siren/handler.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/siren/models.py` & `alfred-py-3.0.6/alfred/siren/models.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/siren/topicgen.py` & `alfred-py-3.0.6/alfred/siren/topicgen.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/tests.py` & `alfred-py-3.0.6/alfred/tests.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/__init__.py` & `alfred-py-3.0.6/alfred/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/base_config.py` & `alfred-py-3.0.6/alfred/utils/base_config.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/communicate.py` & `alfred-py-3.0.6/alfred/utils/communicate.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/cv_wrapper.py` & `alfred-py-3.0.6/alfred/utils/cv_wrapper.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/file_io.py` & `alfred-py-3.0.6/alfred/utils/file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,14 +563,15 @@
 
 
 class SourceIter:
     def __init__(self, src, exit_auto=True):
         self.src = src
         self.srcs = []
         self.crt_index = 0
+        self.crt_filename = ''
         self.video_mode = False
         self.webcam_mode = False
         self.cap = None
         self.ok = True
         self.exit_auto = exit_auto
 
     def __len__(self):
@@ -591,30 +592,31 @@
                     self.ok = False
             else:
                 return frame
         else:
             if self.crt_index < len(self.srcs):
                 p = self.srcs[self.crt_index]
                 self.crt_index += 1
+                self.crt_filename = os.path.basename(p)
                 return p
             else:
                 if self.exit_auto:
                     print("Seems iteration done. bye~")
                     exit(0)
                 else:
                     self.ok = False
                 # raise StopIteration
 
 
 class ImageSourceIter(SourceIter):
-    def __init__(self, src, exit_auto=True, save_res_video=False):
+    def __init__(self, src, exit_auto=True):
         super(ImageSourceIter, self).__init__(src, exit_auto)
 
         self._index_sources()
-        self.is_written = save_res_video
+        self.is_written = False
         self.save_f = None
         assert len(self.srcs) > 0, "srcs indexed empty: {}".format(self.srcs)
         self.lens = len(self.srcs)
         if self.video_mode and not self.webcam_mode:
             self.is_save_video_called = False
             fourcc = cv.VideoWriter_fourcc(*"XVID")
             self.video_width = int(self.cap.get(cv.CAP_PROP_FRAME_WIDTH) + 0.5)
@@ -622,15 +624,15 @@
             self.video_height = int(self.cap.get(cv.CAP_PROP_FRAME_HEIGHT) + 0.5)
             if self.video_mode:
                 self.filename = os.path.basename(src).split(".")[0]
                 self.save_f = os.path.join(
                     os.path.dirname(src), self.filename + "_result.mp4"
                 )
                 self.lens = self.video_frame_count
-            elif self.webcam_mode:
+            else:
                 os.makedirs("results", exist_ok=True)
                 self.save_f = os.path.join("results/webcam_result.mp4")
             self.video_writter = cv.VideoWriter(
                 self.save_f, fourcc, 25.0, (self.video_width, self.video_height)
             )
 
     def get_specific_frames(self, frame_indexes, verbose=True):
@@ -712,45 +714,26 @@
         if self.video_mode:
             self.cap.release()
             if not self.webcam_mode:
                 self.video_writter.release()
             if self.is_written and self.is_save_video_called:
                 print("your wrote video result file should saved into: ", self.save_f)
             else:
-                if self.save_f is not None:
-                    pass
-                    # if os.path.exists(self.save_f):
-                    #     # clean up remove saved file.
-                    #     os.remove(self.save_f)
-
-    def clear_early_quit(self):
-        if self.video_mode:
-            self.cap.release()
-            if not self.webcam_mode:
-                self.video_writter.release()
-            if self.is_written and self.is_save_video_called:
-                print("your wrote video result file should saved into: ", self.save_f)
-            else:
-                if self.save_f is not None:
-                    if os.path.exists(self.save_f):
-                        # clean up remove saved file.
-                        os.remove(self.save_f)
+                if self.save_f and os.path.exists(self.save_f):
+                    # clean up remove saved file.
+                    os.remove(self.save_f)
 
     def waitKey(self):
         if self.video_mode:
-            if cv.waitKey(1) > 0:
-                print('key pressed, exit show..')
-                self.ok = False
-                self.clear_early_quit()
-                # exit(0)
+            cv.waitKey(1)
         else:
             cv.waitKey(0)
     
-    def show(self, winname, mat):
-        cv.imshow(winname, mat)
+    def show(self, winname, img):
+        cv.imshow(winname, img)
 
 
 def next_item(iter):
     itm = next(iter)
     if isinstance(itm, str):
         itm = cv.imread(itm)
     return itm
```

### Comparing `alfred-py-3.0.5/alfred/utils/log.py` & `alfred-py-3.0.6/alfred/utils/log.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/mana.py` & `alfred-py-3.0.6/alfred/utils/mana.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/math_utils.py` & `alfred-py-3.0.6/alfred/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/pprint.py` & `alfred-py-3.0.6/alfred/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/utils/timer.py` & `alfred-py-3.0.6/alfred/utils/timer.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/version.py` & `alfred-py-3.0.6/alfred/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Lucas Jin. All rights reserved.
 from datetime import datetime
 
 major_num = 2
 
-__version__ = "3.0.5"
+__version__ = "3.0.6"
 short_version = __version__
 
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split("."):
         if x.isdigit():
```

### Comparing `alfred-py-3.0.5/alfred/vis/__init__.py` & `alfred-py-3.0.6/alfred/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/__init__.py` & `alfred-py-3.0.6/alfred/vis/image/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/common.py` & `alfred-py-3.0.6/alfred/vis/image/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/constants.py` & `alfred-py-3.0.6/alfred/vis/image/constants.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/det.py` & `alfred-py-3.0.6/alfred/vis/image/det.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/face.py` & `alfred-py-3.0.6/alfred/vis/image/face.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/get_dataset_color_map.py` & `alfred-py-3.0.6/alfred/vis/image/get_dataset_color_map.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/get_dataset_label_map.py` & `alfred-py-3.0.6/alfred/vis/image/get_dataset_label_map.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/mask.py` & `alfred-py-3.0.6/alfred/vis/image/mask.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose.py` & `alfred-py-3.0.6/alfred/vis/image/pose.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_dataset_info.py` & `alfred-py-3.0.6/alfred/vis/image/pose_dataset_info.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/animalpose.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/animalpose.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco_wholebody.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco_wholebody_face.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_face.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/coco_wholebody_hand.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_hand.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/interhand2d.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/interhand2d.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/interhand3d.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/interhand3d.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/mpii.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/mpii.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_datasets/onehand10k.py` & `alfred-py-3.0.6/alfred/vis/image/pose_datasets/onehand10k.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/pose_hand.py` & `alfred-py-3.0.6/alfred/vis/image/pose_hand.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/image/seg.py` & `alfred-py-3.0.6/alfred/vis/image/seg.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/mesh3d/o3d_visconfig.py` & `alfred-py-3.0.6/alfred/vis/mesh3d/o3d_visconfig.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/mesh3d/o3dsocket.py` & `alfred-py-3.0.6/alfred/vis/mesh3d/o3dsocket.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/mesh3d/o3dwrapper.py` & `alfred-py-3.0.6/alfred/vis/mesh3d/o3dwrapper.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/mesh3d/skelmodel.py` & `alfred-py-3.0.6/alfred/vis/mesh3d/skelmodel.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/mesh3d/utils.py` & `alfred-py-3.0.6/alfred/vis/mesh3d/utils.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/pointcloud/__init__.py` & `alfred-py-3.0.6/alfred/vis/pointcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/pointcloud/pointcloud_vis.py` & `alfred-py-3.0.6/alfred/vis/pointcloud/pointcloud_vis.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/renders/render_p3d.py` & `alfred-py-3.0.6/alfred/vis/renders/render_p3d.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred/vis/renders/render_prd.py` & `alfred-py-3.0.6/alfred/vis/renders/render_prd.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/alfred_py.egg-info/PKG-INFO` & `alfred-py-3.0.6/alfred_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-py
-Version: 3.0.5
+Version: 3.0.6
 Summary: Alfred is a DeepLearning utility library.
 Home-page: https://github.com/jinfagang/alfred
 Author: Lucas Jin
 Author-email: jinfagang19@163.com
 License: GPL-3.0
 Keywords: deep learning,script helper,tools
 Platform: any
```

### Comparing `alfred-py-3.0.5/alfred_py.egg-info/SOURCES.txt` & `alfred-py-3.0.6/alfred_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.5/setup.py` & `alfred-py-3.0.6/setup.py`

 * *Files identical despite different names*

